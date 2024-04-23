# Comparing `tmp/uvicore-0.2.2.tar.gz` & `tmp/uvicore-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uvicore-0.2.2.tar", max compression
+gzip compressed data, was "uvicore-0.2.3.tar", max compression
```

## Comparing `uvicore-0.2.2.tar` & `uvicore-0.2.3.tar`

### file list

```diff
@@ -1,241 +1,242 @@
--rw-r--r--   0        0        0     1072 2024-04-10 18:24:17.532245 uvicore-0.2.2/LICENSE
--rw-r--r--   0        0        0      995 2024-04-10 18:31:18.243605 uvicore-0.2.2/README.md
--rw-r--r--   0        0        0     6001 2024-04-10 18:31:18.243605 uvicore-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2236 2024-04-10 18:31:18.243605 uvicore-0.2.2/uvicore/__init__.py
--rw-r--r--   0        0        0       47 2021-09-29 18:14:10.395022 uvicore-0.2.2/uvicore/auth/__init__.py
--rw-r--r--   0        0        0       80 2021-02-18 23:17:24.966073 uvicore-0.2.2/uvicore/auth/auth.py
--rw-r--r--   0        0        0       61 2021-09-29 18:14:10.395022 uvicore-0.2.2/uvicore/auth/authenticators/__init__.py
--rw-r--r--   0        0        0     2809 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/auth/authenticators/base.py
--rw-r--r--   0        0        0     2709 2021-10-14 19:18:41.567853 uvicore-0.2.2/uvicore/auth/authenticators/basic.py
--rw-r--r--   0        0        0     9316 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/auth/authenticators/jwt.py
--rw-r--r--   0        0        0      102 2020-09-30 23:16:47.907315 uvicore-0.2.2/uvicore/auth/commands/db.py
--rw-r--r--   0        0        0     3805 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/auth/config/package.py
--rw-r--r--   0        0        0       80 2020-11-29 06:49:41.064263 uvicore-0.2.2/uvicore/auth/contractsOLD/__init__.py
--rw-r--r--   0        0        0      343 2020-11-29 06:49:41.064263 uvicore-0.2.2/uvicore/auth/contractsOLD/group.py
--rw-r--r--   0        0        0      404 2020-11-29 06:49:41.064263 uvicore-0.2.2/uvicore/auth/contractsOLD/user.py
--rw-r--r--   0        0        0      414 2020-11-29 06:49:41.064263 uvicore-0.2.2/uvicore/auth/contractsOLD/user_info.py
--rw-r--r--   0        0        0      291 2021-03-04 01:20:55.374569 uvicore-0.2.2/uvicore/auth/database/seeders/__init__.py
--rw-r--r--   0        0        0      727 2021-03-22 16:30:17.120378 uvicore-0.2.2/uvicore/auth/database/seeders/groups.py
--rw-r--r--   0        0        0     1376 2021-03-04 01:20:55.374569 uvicore-0.2.2/uvicore/auth/database/seeders/permissions.py
--rw-r--r--   0        0        0      901 2021-03-22 21:25:23.217946 uvicore-0.2.2/uvicore/auth/database/seeders/roles.py
--rw-r--r--   0        0        0      994 2021-03-22 21:25:23.217946 uvicore-0.2.2/uvicore/auth/database/seeders/users.py
--rw-r--r--   0        0        0      266 2021-03-04 01:20:55.374569 uvicore-0.2.2/uvicore/auth/database/tables/__init__.py
--rw-r--r--   0        0        0     1108 2021-03-02 19:39:30.880258 uvicore-0.2.2/uvicore/auth/database/tables/group_roles.py
--rw-r--r--   0        0        0      902 2021-03-02 19:39:30.880258 uvicore-0.2.2/uvicore/auth/database/tables/groups.py
--rw-r--r--   0        0        0      908 2021-03-02 19:39:30.880258 uvicore-0.2.2/uvicore/auth/database/tables/permissions.py
--rw-r--r--   0        0        0     1143 2021-03-02 19:39:30.880258 uvicore-0.2.2/uvicore/auth/database/tables/role_permissions.py
--rw-r--r--   0        0        0      894 2021-03-22 21:25:23.217946 uvicore-0.2.2/uvicore/auth/database/tables/roles.py
--rw-r--r--   0        0        0     1211 2021-03-02 19:39:30.880258 uvicore-0.2.2/uvicore/auth/database/tables/user_groups.py
--rw-r--r--   0        0        0     1101 2021-03-04 01:20:55.374569 uvicore-0.2.2/uvicore/auth/database/tables/user_roles.py
--rw-r--r--   0        0        0     2174 2021-03-22 15:01:04.718027 uvicore-0.2.2/uvicore/auth/database/tables/users.py
--rw-r--r--   0        0        0        0 2021-06-30 20:04:15.673495 uvicore-0.2.2/uvicore/auth/http/api/userinfo.py
--rw-r--r--   0        0        0       26 2021-01-28 23:57:53.792892 uvicore-0.2.2/uvicore/auth/http/public/assets/js/app.js
--rw-r--r--   0        0        0        2 2021-01-28 23:57:53.792892 uvicore-0.2.2/uvicore/auth/http/public/robots.txt
--rw-r--r--   0        0        0       15 2021-01-28 23:57:53.792892 uvicore-0.2.2/uvicore/auth/http/public/test.txt
--rw-r--r--   0        0        0     1954 2021-08-18 03:36:20.680024 uvicore-0.2.2/uvicore/auth/http/routes/api.py
--rw-r--r--   0        0        0       88 2021-09-29 18:14:10.395022 uvicore-0.2.2/uvicore/auth/middleware/__init__.py
--rw-r--r--   0        0        0     9337 2021-03-14 14:29:52.918516 uvicore-0.2.2/uvicore/auth/middleware/auth_OLD.py
--rw-r--r--   0        0        0     3102 2021-03-13 03:32:22.779743 uvicore-0.2.2/uvicore/auth/middleware/basic_OLD.py
--rw-r--r--   0        0        0     7288 2021-03-13 03:32:22.779743 uvicore-0.2.2/uvicore/auth/middleware/jwt_OLD.py
--rw-r--r--   0        0        0      121 2021-09-29 18:14:10.395022 uvicore-0.2.2/uvicore/auth/models/__init__.py
--rw-r--r--   0        0        0      985 2021-09-29 18:14:10.395022 uvicore-0.2.2/uvicore/auth/models/group.py
--rw-r--r--   0        0        0      671 2021-09-29 18:14:10.395022 uvicore-0.2.2/uvicore/auth/models/permission.py
--rw-r--r--   0        0        0     1050 2021-09-29 18:14:10.395022 uvicore-0.2.2/uvicore/auth/models/role.py
--rw-r--r--   0        0        0     3385 2021-09-29 18:14:10.395022 uvicore-0.2.2/uvicore/auth/models/user.py
--rw-r--r--   0        0        0     4871 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/auth/package/provider.py
--rw-r--r--   0        0        0     1408 2021-03-02 19:39:30.880258 uvicore-0.2.2/uvicore/auth/support/password.py
--rw-r--r--   0        0        0     3541 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/auth/user_info.py
--rw-r--r--   0        0        0       57 2021-09-29 18:14:10.395022 uvicore-0.2.2/uvicore/auth/user_providers/__init__.py
--rw-r--r--   0        0        0     3106 2021-08-20 00:01:23.896381 uvicore-0.2.2/uvicore/auth/user_providers/jwt.py
--rw-r--r--   0        0        0    11011 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/auth/user_providers/orm.py
--rw-r--r--   0        0        0     9031 2021-10-14 19:18:41.567853 uvicore-0.2.2/uvicore/cache/backends/array.py
--rw-r--r--   0        0        0     7734 2021-10-14 19:18:41.567853 uvicore-0.2.2/uvicore/cache/backends/redis.py
--rw-r--r--   0        0        0     2115 2021-10-01 23:17:25.701767 uvicore-0.2.2/uvicore/cache/manager.py
--rw-r--r--   0        0        0     2201 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/cache/package/provider.py
--rw-r--r--   0        0        0      464 2020-11-29 06:49:41.067596 uvicore-0.2.2/uvicore/configuration/__init__.py
--rw-r--r--   0        0        0      786 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/configuration/commands/config.py
--rw-r--r--   0        0        0     2739 2021-03-02 19:39:30.880258 uvicore-0.2.2/uvicore/configuration/configuration.py
--rw-r--r--   0        0        0     2351 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/configuration/package/provider.py
--rw-r--r--   0        0        0      790 2023-03-06 01:06:43.066631 uvicore-0.2.2/uvicore/console/__init__.py
--rw-r--r--   0        0        0     1475 2021-06-30 20:04:15.673495 uvicore-0.2.2/uvicore/console/asyncclick/LICENSE.rst
--rw-r--r--   0        0        0      341 2021-06-30 20:04:15.673495 uvicore-0.2.2/uvicore/console/asyncclick/README.md
--rw-r--r--   0        0        0     2465 2021-06-30 20:04:15.673495 uvicore-0.2.2/uvicore/console/asyncclick/__init__.py
--rw-r--r--   0        0        0    12412 2021-06-30 20:04:15.673495 uvicore-0.2.2/uvicore/console/asyncclick/_bashcomplete.py
--rw-r--r--   0        0        0    19850 2021-06-30 20:04:15.673495 uvicore-0.2.2/uvicore/console/asyncclick/_compat.py
--rw-r--r--   0        0        0    20701 2021-06-30 20:04:15.673495 uvicore-0.2.2/uvicore/console/asyncclick/_termui_impl.py
--rw-r--r--   0        0        0     1197 2021-06-30 20:04:15.673495 uvicore-0.2.2/uvicore/console/asyncclick/_textwrap.py
--rw-r--r--   0        0        0     3439 2021-06-30 20:04:15.673495 uvicore-0.2.2/uvicore/console/asyncclick/_unicodefun.py
--rw-r--r--   0        0        0     8379 2021-06-30 20:04:15.673495 uvicore-0.2.2/uvicore/console/asyncclick/_winconsole.py
--rw-r--r--   0        0        0    80043 2023-04-16 17:13:46.545521 uvicore-0.2.2/uvicore/console/asyncclick/core.py
--rw-r--r--   0        0        0    11215 2021-06-30 20:04:15.676828 uvicore-0.2.2/uvicore/console/asyncclick/decorators.py
--rw-r--r--   0        0        0     7744 2021-06-30 20:04:15.676828 uvicore-0.2.2/uvicore/console/asyncclick/exceptions.py
--rw-r--r--   0        0        0     9281 2021-06-30 20:04:15.676828 uvicore-0.2.2/uvicore/console/asyncclick/formatting.py
--rw-r--r--   0        0        0     1501 2021-06-30 20:04:15.676828 uvicore-0.2.2/uvicore/console/asyncclick/globals.py
--rw-r--r--   0        0        0    15697 2021-06-30 20:04:15.676828 uvicore-0.2.2/uvicore/console/asyncclick/parser.py
--rw-r--r--   0        0        0    23998 2021-06-30 20:04:15.676828 uvicore-0.2.2/uvicore/console/asyncclick/termui.py
--rw-r--r--   0        0        0    12886 2021-06-30 20:04:15.676828 uvicore-0.2.2/uvicore/console/asyncclick/testing.py
--rw-r--r--   0        0        0    24845 2021-06-30 20:04:15.676828 uvicore-0.2.2/uvicore/console/asyncclick/types.py
--rw-r--r--   0        0        0    15642 2021-06-30 20:04:15.676828 uvicore-0.2.2/uvicore/console/asyncclick/utils.py
--rw-r--r--   0        0        0     6189 2023-03-06 01:06:46.553354 uvicore-0.2.2/uvicore/console/click_colors.py
--rw-r--r--   0        0        0     1764 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/console/commands/generators.py
--rw-r--r--   0        0        0     1857 2021-08-19 19:44:45.042716 uvicore-0.2.2/uvicore/console/commands/stubs/command.py
--rw-r--r--   0        0        0     1933 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/console/console.py
--rw-r--r--   0        0        0      756 2023-03-06 01:06:57.420198 uvicore-0.2.2/uvicore/console/decorators.py
--rw-r--r--   0        0        0      717 2023-04-16 17:13:46.545521 uvicore-0.2.2/uvicore/console/events/command.py
--rw-r--r--   0        0        0     2430 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/console/package/bootstrap.py
--rw-r--r--   0        0        0     2938 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/console/package/provider.py
--rw-r--r--   0        0        0     1016 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/console/package/registers.py
--rw-r--r--   0        0        0      101 2020-11-29 06:49:41.070929 uvicore-0.2.2/uvicore/container/__init__.py
--rw-r--r--   0        0        0     2236 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/container/commands/ioc.py
--rw-r--r--   0        0        0    12772 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/container/ioc.py
--rw-r--r--   0        0        0     1185 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/contracts/__init__.py
--rw-r--r--   0        0        0     3449 2021-09-29 18:14:10.395022 uvicore-0.2.2/uvicore/contracts/application.py
--rw-r--r--   0        0        0     1089 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/contracts/authenticator.py
--rw-r--r--   0        0        0      390 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/contracts/auto_api.py
--rw-r--r--   0        0        0     4264 2021-10-14 19:18:41.567853 uvicore-0.2.2/uvicore/contracts/builder.py
--rw-r--r--   0        0        0     2085 2021-05-16 03:31:59.322488 uvicore-0.2.2/uvicore/contracts/cache.py
--rw-r--r--   0        0        0      828 2021-01-23 07:50:00.140302 uvicore-0.2.2/uvicore/contracts/config.py
--rw-r--r--   0        0        0      781 2021-01-23 08:40:53.308916 uvicore-0.2.2/uvicore/contracts/connection.py
--rw-r--r--   0        0        0     5514 2023-04-16 17:13:46.548854 uvicore-0.2.2/uvicore/contracts/database.py
--rw-r--r--   0        0        0     2209 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/contracts/dispatcher.py
--rw-r--r--   0        0        0      433 2021-05-16 03:31:59.322488 uvicore-0.2.2/uvicore/contracts/email.py
--rw-r--r--   0        0        0      564 2021-03-02 19:39:30.880258 uvicore-0.2.2/uvicore/contracts/event.py
--rw-r--r--   0        0        0      759 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/contracts/field.py
--rw-r--r--   0        0        0     2109 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/contracts/ioc.py
--rw-r--r--   0        0        0      588 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/contracts/job.py
--rw-r--r--   0        0        0      570 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/contracts/job_dispatcher.py
--rw-r--r--   0        0        0     2504 2022-12-18 06:36:42.753628 uvicore-0.2.2/uvicore/contracts/logger.py
--rw-r--r--   0        0        0     1377 2021-04-05 21:28:22.231229 uvicore-0.2.2/uvicore/contracts/mapper.py
--rw-r--r--   0        0        0     3814 2022-02-18 20:14:08.924157 uvicore-0.2.2/uvicore/contracts/model.py
--rw-r--r--   0        0        0     3102 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/contracts/package.py
--rw-r--r--   0        0        0     2610 2021-01-22 23:57:24.015514 uvicore-0.2.2/uvicore/contracts/provider.py
--rw-r--r--   0        0        0      742 2020-11-29 06:49:41.074262 uvicore-0.2.2/uvicore/contracts/relation.py
--rw-r--r--   0        0        0     4220 2021-09-22 05:15:43.413436 uvicore-0.2.2/uvicore/contracts/router.py
--rw-r--r--   0        0        0      808 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/contracts/routes-OLD.py
--rw-r--r--   0        0        0      532 2021-03-22 21:25:23.221280 uvicore-0.2.2/uvicore/contracts/server.py
--rw-r--r--   0        0        0      924 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/contracts/template.py
--rw-r--r--   0        0        0     2243 2021-08-20 00:01:23.896381 uvicore-0.2.2/uvicore/contracts/user_info.py
--rw-r--r--   0        0        0     3004 2021-10-14 19:18:41.567853 uvicore-0.2.2/uvicore/contracts/user_provider.py
--rw-r--r--   0        0        0      704 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/database/__init__.py
--rw-r--r--   0        0        0    18719 2023-04-16 17:13:46.548854 uvicore-0.2.2/uvicore/database/builder.py
--rw-r--r--   0        0        0     7979 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/database/commands/db.py
--rw-r--r--   0        0        0     2527 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/database/commands/generators.py
--rw-r--r--   0        0        0     4721 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/database/commands/stubs/seeder.py
--rw-r--r--   0        0        0     3012 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/database/commands/stubs/table.py
--rw-r--r--   0        0        0     9981 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/database/db.py
--rw-r--r--   0        0        0     1728 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/database/package/bootstrap.py
--rw-r--r--   0        0        0     3774 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/database/package/provider.py
--rw-r--r--   0        0        0     3866 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/database/package/registers.py
--rw-r--r--   0        0        0     6117 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/database/query.py
--rw-r--r--   0        0        0     3137 2024-02-10 00:08:36.205626 uvicore-0.2.2/uvicore/database/table.py
--rw-r--r--   0        0        0      302 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/events/__init__.py
--rw-r--r--   0        0        0     1415 2021-09-22 05:15:43.413436 uvicore-0.2.2/uvicore/events/commands/event.py
--rw-r--r--   0        0        0    13029 2021-09-22 05:15:43.413436 uvicore-0.2.2/uvicore/events/dispatcher.py
--rw-r--r--   0        0        0     2180 2024-04-02 23:02:52.114042 uvicore-0.2.2/uvicore/events/event.py
--rw-r--r--   0        0        0      143 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/events/handler.py
--rw-r--r--   0        0        0     2035 2024-04-04 17:37:46.119796 uvicore-0.2.2/uvicore/exceptions/__init__.py
--rw-r--r--   0        0        0       42 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/factories/__init__.py
--rw-r--r--   0        0        0      252 2020-09-30 23:16:47.910648 uvicore-0.2.2/uvicore/factories/logger.py
--rw-r--r--   0        0        0    12711 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/foundation/application.py
--rw-r--r--   0        0        0      306 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/foundation/commands/app.py
--rw-r--r--   0        0        0     3926 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/foundation/config/package.py
--rw-r--r--   0        0        0      291 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/foundation/decorators/__init__.py
--rw-r--r--   0        0        0      435 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/foundation/decorators/composer.py
--rw-r--r--   0        0        0      439 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/foundation/decorators/controller.py
--rw-r--r--   0        0        0      472 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/foundation/decorators/event.py
--rw-r--r--   0        0        0      429 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/foundation/decorators/job.py
--rw-r--r--   0        0        0      522 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/foundation/decorators/model.py
--rw-r--r--   0        0        0      482 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/foundation/decorators/provider.py
--rw-r--r--   0        0        0      431 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/foundation/decorators/routes.py
--rw-r--r--   0        0        0      475 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/foundation/decorators/seeder.py
--rw-r--r--   0        0        0      681 2021-09-07 21:04:46.388597 uvicore-0.2.2/uvicore/foundation/decorators/service.py
--rw-r--r--   0        0        0      470 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/foundation/decorators/table.py
--rw-r--r--   0        0        0      893 2021-09-08 13:16:25.207365 uvicore-0.2.2/uvicore/foundation/events/app.py
--rw-r--r--   0        0        0     5691 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/foundation/package/provider.py
--rw-r--r--   0        0        0      749 2020-09-30 23:16:47.913981 uvicore-0.2.2/uvicore/http/OBSOLETE/router.py
--rw-r--r--   0        0        0     1956 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/http/OBSOLETE/routes-OLD.py
--rw-r--r--   0        0        0      762 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/http/__init__.py
--rw-r--r--   0        0        0     3210 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/http/commands/generators.py
--rw-r--r--   0        0        0      418 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/http/commands/routes.py
--rw-r--r--   0        0        0      570 2020-12-02 20:34:40.502696 uvicore-0.2.2/uvicore/http/commands/serve.py
--rw-r--r--   0        0        0    12327 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/http/commands/stubs/api_controller.py
--rw-r--r--   0        0        0      913 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/http/commands/stubs/composer.py
--rw-r--r--   0        0        0    12890 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/http/commands/stubs/controller.py
--rw-r--r--   0        0        0       62 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/http/controllers/__init__.py
--rw-r--r--   0        0        0     5354 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/http/controllers/api.py
--rw-r--r--   0        0        0     5908 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/http/controllers/web.py
--rw-r--r--   0        0        0      874 2021-03-24 17:46:21.490777 uvicore-0.2.2/uvicore/http/events/server.py
--rw-r--r--   0        0        0     3972 2021-10-14 19:18:41.567853 uvicore-0.2.2/uvicore/http/exceptions/__init__.py
--rw-r--r--   0        0        0     2851 2021-10-14 19:18:41.567853 uvicore-0.2.2/uvicore/http/exceptions/handlers.py
--rw-r--r--   0        0        0      845 2021-03-13 03:32:22.779743 uvicore-0.2.2/uvicore/http/middleware/__init__.py
--rw-r--r--   0        0        0    13312 2024-04-10 18:24:17.538912 uvicore-0.2.2/uvicore/http/middleware/authentication.py
--rw-r--r--   0        0        0     1968 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/http/openapi/docs.py
--rw-r--r--   0        0        0    29150 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/http/package/bootstrap.py
--rw-r--r--   0        0        0     6524 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/http/package/provider.py
--rw-r--r--   0        0        0     4520 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/http/package/registers.py
--rw-r--r--   0        0        0      124 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/http/params.py
--rw-r--r--   0        0        0     1301 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/http/request.py
--rw-r--r--   0        0        0     4661 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/http/response.py
--rw-r--r--   0        0        0      455 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/http/routing/__init__.py
--rw-r--r--   0        0        0    22281 2021-09-22 05:15:43.416770 uvicore-0.2.2/uvicore/http/routing/api_router.py
--rw-r--r--   0        0        0    10476 2021-10-14 19:18:41.567853 uvicore-0.2.2/uvicore/http/routing/auto_api.py
--rw-r--r--   0        0        0     4875 2021-09-07 21:04:46.391931 uvicore-0.2.2/uvicore/http/routing/guard.py
--rw-r--r--   0        0        0    21460 2024-02-21 05:43:11.859354 uvicore-0.2.2/uvicore/http/routing/model_router.py
--rw-r--r--   0        0        0    21451 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/http/routing/router.py
--rw-r--r--   0        0        0    16785 2021-09-22 05:15:43.416770 uvicore-0.2.2/uvicore/http/routing/web_router.py
--rw-r--r--   0        0        0     3521 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/http/server.py
--rw-r--r--   0        0        0      797 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/http/servers/api.py
--rw-r--r--   0        0        0      393 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/http/servers/web.py
--rw-r--r--   0        0        0      865 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/http/static.py
--rw-r--r--   0        0        0     2517 2021-03-02 19:39:30.883592 uvicore-0.2.2/uvicore/http/status.py
--rw-r--r--   0        0        0     1609 2021-10-14 19:18:41.567853 uvicore-0.2.2/uvicore/http/templating/context_functions.py
--rw-r--r--   0        0        0     2280 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/http_client/package/provider.py
--rw-r--r--   0        0        0       88 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/jobs/__init__.py
--rw-r--r--   0        0        0      679 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/jobs/dispatcher.py
--rw-r--r--   0        0        0      902 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/jobs/job.py
--rw-r--r--   0        0        0      332 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/jobs/results.py
--rw-r--r--   0        0        0    14997 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/logging/logger.py
--rw-r--r--   0        0        0     2340 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/logging/package/provider.py
--rw-r--r--   0        0        0     2608 2021-05-16 03:31:59.322488 uvicore-0.2.2/uvicore/mail/__init__.py
--rw-r--r--   0        0        0       29 2021-05-16 03:31:59.322488 uvicore-0.2.2/uvicore/mail/backends/__init__.py
--rw-r--r--   0        0        0     2126 2021-05-16 03:31:59.322488 uvicore-0.2.2/uvicore/mail/backends/mailgun.py
--rw-r--r--   0        0        0     1181 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/mail/package/provider.py
--rw-r--r--   0        0        0      181 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/orm/__init__.py
--rw-r--r--   0        0        0     1395 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/orm/commands/generators.py
--rw-r--r--   0        0        0     9719 2023-04-16 17:13:46.552188 uvicore-0.2.2/uvicore/orm/commands/stubs/model.py
--rw-r--r--   0        0        0      447 2021-09-07 21:04:46.391931 uvicore-0.2.2/uvicore/orm/drivers/api.py
--rw-r--r--   0        0        0        0 2021-03-26 15:13:44.398249 uvicore-0.2.2/uvicore/orm/drivers/sqlalchemy.py
--rw-r--r--   0        0        0    13295 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/orm/fields.py
--rw-r--r--   0        0        0     7967 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/orm/mapper.py
--rw-r--r--   0        0        0    18144 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/orm/metaclass.py
--rw-r--r--   0        0        0    32661 2024-03-26 17:38:31.288155 uvicore-0.2.2/uvicore/orm/model.py
--rw-r--r--   0        0        0     3108 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/orm/package/provider.py
--rw-r--r--   0        0        0    49157 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/orm/query.py
--rw-r--r--   0        0        0      458 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/package/__init__.py
--rw-r--r--   0        0        0     1794 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/package/commands/package.py
--rw-r--r--   0        0        0     3490 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/package/package.py
--rw-r--r--   0        0        0     3676 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/package/provider.py
--rw-r--r--   0        0        0       40 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/redis/__init__.py
--rw-r--r--   0        0        0     1218 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/redis/package/bootstrap.py
--rw-r--r--   0        0        0     3287 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/redis/package/provider.py
--rw-r--r--   0        0        0      272 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/redis/package/registers.py
--rw-r--r--   0        0        0     3277 2021-10-14 19:18:41.567853 uvicore-0.2.2/uvicore/redis/redis.py
--rw-r--r--   0        0        0      407 2020-09-30 23:16:47.913981 uvicore-0.2.2/uvicore/support/README.md
--rw-r--r--   0        0        0      296 2021-03-29 16:45:06.822538 uvicore-0.2.2/uvicore/support/classes.py
--rw-r--r--   0        0        0     5162 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/support/collection.py
--rw-r--r--   0        0        0     2419 2021-03-22 21:25:23.221280 uvicore-0.2.2/uvicore/support/concurrency.py
--rw-r--r--   0        0        0     1237 2021-03-02 19:39:30.886925 uvicore-0.2.2/uvicore/support/dictionary.py
--rw-r--r--   0        0        0     1680 2021-01-27 21:25:20.094702 uvicore-0.2.2/uvicore/support/dumper.py
--rw-r--r--   0        0        0      439 2023-07-16 16:47:20.390563 uvicore-0.2.2/uvicore/support/hash.py
--rw-r--r--   0        0        0     3771 2023-09-26 21:00:07.189986 uvicore-0.2.2/uvicore/support/module.py
--rw-r--r--   0        0        0      567 2020-09-30 23:16:47.917315 uvicore-0.2.2/uvicore/support/path.py
--rw-r--r--   0        0        0     1889 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/support/schematic.py
--rw-r--r--   0        0        0      623 2020-07-20 18:33:04.439377 uvicore-0.2.2/uvicore/support/singleton.py
--rw-r--r--   0        0        0     2066 2020-12-31 21:18:43.991950 uvicore-0.2.2/uvicore/support/str.py
--rw-r--r--   0        0        0     5446 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/templating/engine.py
--rw-r--r--   0        0        0     2904 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/templating/package/bootstrap.py
--rw-r--r--   0        0        0     1686 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/templating/package/provider.py
--rw-r--r--   0        0        0     1024 2024-04-10 18:24:17.542246 uvicore-0.2.2/uvicore/templating/package/registers.py
--rw-r--r--   0        0        0     2452 2021-09-29 18:14:10.398356 uvicore-0.2.2/uvicore/typing/__init__.py
--rw-r--r--   0        0        0    12661 2021-10-15 19:36:53.939029 uvicore-0.2.2/uvicore/typing/dictionary.py
--rw-r--r--   0        0        0     3617 1970-01-01 00:00:00.000000 uvicore-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 18:24:17.532245 uvicore-0.2.3/LICENSE
+-rw-r--r--   0        0        0      995 2024-04-10 18:31:18.243605 uvicore-0.2.3/README.md
+-rw-r--r--   0        0        0     6001 2024-04-23 21:52:40.607108 uvicore-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2236 2024-04-23 21:52:40.607108 uvicore-0.2.3/uvicore/__init__.py
+-rw-r--r--   0        0        0       47 2021-09-29 18:14:10.395022 uvicore-0.2.3/uvicore/auth/__init__.py
+-rw-r--r--   0        0        0       80 2021-02-18 23:17:24.966073 uvicore-0.2.3/uvicore/auth/auth.py
+-rw-r--r--   0        0        0       61 2021-09-29 18:14:10.395022 uvicore-0.2.3/uvicore/auth/authenticators/__init__.py
+-rw-r--r--   0        0        0     2809 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/auth/authenticators/base.py
+-rw-r--r--   0        0        0     2709 2021-10-14 19:18:41.567853 uvicore-0.2.3/uvicore/auth/authenticators/basic.py
+-rw-r--r--   0        0        0     9316 2024-04-22 23:55:13.346380 uvicore-0.2.3/uvicore/auth/authenticators/jwt.py
+-rw-r--r--   0        0        0      102 2020-09-30 23:16:47.907315 uvicore-0.2.3/uvicore/auth/commands/db.py
+-rw-r--r--   0        0        0     3805 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/auth/config/package.py
+-rw-r--r--   0        0        0       80 2020-11-29 06:49:41.064263 uvicore-0.2.3/uvicore/auth/contractsOLD/__init__.py
+-rw-r--r--   0        0        0      343 2020-11-29 06:49:41.064263 uvicore-0.2.3/uvicore/auth/contractsOLD/group.py
+-rw-r--r--   0        0        0      404 2020-11-29 06:49:41.064263 uvicore-0.2.3/uvicore/auth/contractsOLD/user.py
+-rw-r--r--   0        0        0      414 2020-11-29 06:49:41.064263 uvicore-0.2.3/uvicore/auth/contractsOLD/user_info.py
+-rw-r--r--   0        0        0      291 2021-03-04 01:20:55.374569 uvicore-0.2.3/uvicore/auth/database/seeders/__init__.py
+-rw-r--r--   0        0        0      727 2021-03-22 16:30:17.120378 uvicore-0.2.3/uvicore/auth/database/seeders/groups.py
+-rw-r--r--   0        0        0     1376 2021-03-04 01:20:55.374569 uvicore-0.2.3/uvicore/auth/database/seeders/permissions.py
+-rw-r--r--   0        0        0      901 2021-03-22 21:25:23.217946 uvicore-0.2.3/uvicore/auth/database/seeders/roles.py
+-rw-r--r--   0        0        0      994 2021-03-22 21:25:23.217946 uvicore-0.2.3/uvicore/auth/database/seeders/users.py
+-rw-r--r--   0        0        0      266 2021-03-04 01:20:55.374569 uvicore-0.2.3/uvicore/auth/database/tables/__init__.py
+-rw-r--r--   0        0        0     1108 2021-03-02 19:39:30.880258 uvicore-0.2.3/uvicore/auth/database/tables/group_roles.py
+-rw-r--r--   0        0        0      902 2021-03-02 19:39:30.880258 uvicore-0.2.3/uvicore/auth/database/tables/groups.py
+-rw-r--r--   0        0        0      908 2021-03-02 19:39:30.880258 uvicore-0.2.3/uvicore/auth/database/tables/permissions.py
+-rw-r--r--   0        0        0     1143 2021-03-02 19:39:30.880258 uvicore-0.2.3/uvicore/auth/database/tables/role_permissions.py
+-rw-r--r--   0        0        0      894 2021-03-22 21:25:23.217946 uvicore-0.2.3/uvicore/auth/database/tables/roles.py
+-rw-r--r--   0        0        0     1211 2021-03-02 19:39:30.880258 uvicore-0.2.3/uvicore/auth/database/tables/user_groups.py
+-rw-r--r--   0        0        0     1101 2021-03-04 01:20:55.374569 uvicore-0.2.3/uvicore/auth/database/tables/user_roles.py
+-rw-r--r--   0        0        0     2174 2021-03-22 15:01:04.718027 uvicore-0.2.3/uvicore/auth/database/tables/users.py
+-rw-r--r--   0        0        0        0 2021-06-30 20:04:15.673495 uvicore-0.2.3/uvicore/auth/http/api/userinfo.py
+-rw-r--r--   0        0        0       26 2021-01-28 23:57:53.792892 uvicore-0.2.3/uvicore/auth/http/public/assets/js/app.js
+-rw-r--r--   0        0        0        2 2021-01-28 23:57:53.792892 uvicore-0.2.3/uvicore/auth/http/public/robots.txt
+-rw-r--r--   0        0        0       15 2021-01-28 23:57:53.792892 uvicore-0.2.3/uvicore/auth/http/public/test.txt
+-rw-r--r--   0        0        0     1954 2021-08-18 03:36:20.680024 uvicore-0.2.3/uvicore/auth/http/routes/api.py
+-rw-r--r--   0        0        0       88 2021-09-29 18:14:10.395022 uvicore-0.2.3/uvicore/auth/middleware/__init__.py
+-rw-r--r--   0        0        0     9337 2021-03-14 14:29:52.918516 uvicore-0.2.3/uvicore/auth/middleware/auth_OLD.py
+-rw-r--r--   0        0        0     3102 2021-03-13 03:32:22.779743 uvicore-0.2.3/uvicore/auth/middleware/basic_OLD.py
+-rw-r--r--   0        0        0     7288 2021-03-13 03:32:22.779743 uvicore-0.2.3/uvicore/auth/middleware/jwt_OLD.py
+-rw-r--r--   0        0        0      121 2021-09-29 18:14:10.395022 uvicore-0.2.3/uvicore/auth/models/__init__.py
+-rw-r--r--   0        0        0      985 2021-09-29 18:14:10.395022 uvicore-0.2.3/uvicore/auth/models/group.py
+-rw-r--r--   0        0        0      671 2021-09-29 18:14:10.395022 uvicore-0.2.3/uvicore/auth/models/permission.py
+-rw-r--r--   0        0        0     1050 2021-09-29 18:14:10.395022 uvicore-0.2.3/uvicore/auth/models/role.py
+-rw-r--r--   0        0        0     3385 2021-09-29 18:14:10.395022 uvicore-0.2.3/uvicore/auth/models/user.py
+-rw-r--r--   0        0        0     4871 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/auth/package/provider.py
+-rw-r--r--   0        0        0     1408 2021-03-02 19:39:30.880258 uvicore-0.2.3/uvicore/auth/support/password.py
+-rw-r--r--   0        0        0     3541 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/auth/user_info.py
+-rw-r--r--   0        0        0       57 2021-09-29 18:14:10.395022 uvicore-0.2.3/uvicore/auth/user_providers/__init__.py
+-rw-r--r--   0        0        0     3106 2021-08-20 00:01:23.896381 uvicore-0.2.3/uvicore/auth/user_providers/jwt.py
+-rw-r--r--   0        0        0    11011 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/auth/user_providers/orm.py
+-rw-r--r--   0        0        0     9031 2021-10-14 19:18:41.567853 uvicore-0.2.3/uvicore/cache/backends/array.py
+-rw-r--r--   0        0        0     7734 2021-10-14 19:18:41.567853 uvicore-0.2.3/uvicore/cache/backends/redis.py
+-rw-r--r--   0        0        0     2115 2021-10-01 23:17:25.701767 uvicore-0.2.3/uvicore/cache/manager.py
+-rw-r--r--   0        0        0     2201 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/cache/package/provider.py
+-rw-r--r--   0        0        0      464 2020-11-29 06:49:41.067596 uvicore-0.2.3/uvicore/configuration/__init__.py
+-rw-r--r--   0        0        0      786 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/configuration/commands/config.py
+-rw-r--r--   0        0        0     2739 2021-03-02 19:39:30.880258 uvicore-0.2.3/uvicore/configuration/configuration.py
+-rw-r--r--   0        0        0     2351 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/configuration/package/provider.py
+-rw-r--r--   0        0        0      790 2023-03-06 01:06:43.066631 uvicore-0.2.3/uvicore/console/__init__.py
+-rw-r--r--   0        0        0     1475 2021-06-30 20:04:15.673495 uvicore-0.2.3/uvicore/console/asyncclick/LICENSE.rst
+-rw-r--r--   0        0        0      341 2021-06-30 20:04:15.673495 uvicore-0.2.3/uvicore/console/asyncclick/README.md
+-rw-r--r--   0        0        0     2465 2021-06-30 20:04:15.673495 uvicore-0.2.3/uvicore/console/asyncclick/__init__.py
+-rw-r--r--   0        0        0    12412 2021-06-30 20:04:15.673495 uvicore-0.2.3/uvicore/console/asyncclick/_bashcomplete.py
+-rw-r--r--   0        0        0    19850 2021-06-30 20:04:15.673495 uvicore-0.2.3/uvicore/console/asyncclick/_compat.py
+-rw-r--r--   0        0        0    20701 2021-06-30 20:04:15.673495 uvicore-0.2.3/uvicore/console/asyncclick/_termui_impl.py
+-rw-r--r--   0        0        0     1197 2021-06-30 20:04:15.673495 uvicore-0.2.3/uvicore/console/asyncclick/_textwrap.py
+-rw-r--r--   0        0        0     3439 2021-06-30 20:04:15.673495 uvicore-0.2.3/uvicore/console/asyncclick/_unicodefun.py
+-rw-r--r--   0        0        0     8379 2021-06-30 20:04:15.673495 uvicore-0.2.3/uvicore/console/asyncclick/_winconsole.py
+-rw-r--r--   0        0        0    80043 2023-04-16 17:13:46.545521 uvicore-0.2.3/uvicore/console/asyncclick/core.py
+-rw-r--r--   0        0        0    11215 2021-06-30 20:04:15.676828 uvicore-0.2.3/uvicore/console/asyncclick/decorators.py
+-rw-r--r--   0        0        0     7744 2021-06-30 20:04:15.676828 uvicore-0.2.3/uvicore/console/asyncclick/exceptions.py
+-rw-r--r--   0        0        0     9281 2021-06-30 20:04:15.676828 uvicore-0.2.3/uvicore/console/asyncclick/formatting.py
+-rw-r--r--   0        0        0     1501 2021-06-30 20:04:15.676828 uvicore-0.2.3/uvicore/console/asyncclick/globals.py
+-rw-r--r--   0        0        0    15697 2021-06-30 20:04:15.676828 uvicore-0.2.3/uvicore/console/asyncclick/parser.py
+-rw-r--r--   0        0        0    23998 2021-06-30 20:04:15.676828 uvicore-0.2.3/uvicore/console/asyncclick/termui.py
+-rw-r--r--   0        0        0    12886 2021-06-30 20:04:15.676828 uvicore-0.2.3/uvicore/console/asyncclick/testing.py
+-rw-r--r--   0        0        0    24845 2021-06-30 20:04:15.676828 uvicore-0.2.3/uvicore/console/asyncclick/types.py
+-rw-r--r--   0        0        0    15642 2021-06-30 20:04:15.676828 uvicore-0.2.3/uvicore/console/asyncclick/utils.py
+-rw-r--r--   0        0        0     6189 2023-03-06 01:06:46.553354 uvicore-0.2.3/uvicore/console/click_colors.py
+-rw-r--r--   0        0        0     1764 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/console/commands/generators.py
+-rw-r--r--   0        0        0     1857 2021-08-19 19:44:45.042716 uvicore-0.2.3/uvicore/console/commands/stubs/command.py
+-rw-r--r--   0        0        0     1933 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/console/console.py
+-rw-r--r--   0        0        0      756 2023-03-06 01:06:57.420198 uvicore-0.2.3/uvicore/console/decorators.py
+-rw-r--r--   0        0        0      717 2023-04-16 17:13:46.545521 uvicore-0.2.3/uvicore/console/events/command.py
+-rw-r--r--   0        0        0     2430 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/console/package/bootstrap.py
+-rw-r--r--   0        0        0     2938 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/console/package/provider.py
+-rw-r--r--   0        0        0     1016 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/console/package/registers.py
+-rw-r--r--   0        0        0      101 2020-11-29 06:49:41.070929 uvicore-0.2.3/uvicore/container/__init__.py
+-rw-r--r--   0        0        0     2236 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/container/commands/ioc.py
+-rw-r--r--   0        0        0    12772 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/container/ioc.py
+-rw-r--r--   0        0        0     1185 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/contracts/__init__.py
+-rw-r--r--   0        0        0     3449 2021-09-29 18:14:10.395022 uvicore-0.2.3/uvicore/contracts/application.py
+-rw-r--r--   0        0        0     1089 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/contracts/authenticator.py
+-rw-r--r--   0        0        0      390 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/contracts/auto_api.py
+-rw-r--r--   0        0        0     4264 2021-10-14 19:18:41.567853 uvicore-0.2.3/uvicore/contracts/builder.py
+-rw-r--r--   0        0        0     2085 2021-05-16 03:31:59.322488 uvicore-0.2.3/uvicore/contracts/cache.py
+-rw-r--r--   0        0        0      828 2021-01-23 07:50:00.140302 uvicore-0.2.3/uvicore/contracts/config.py
+-rw-r--r--   0        0        0      781 2021-01-23 08:40:53.308916 uvicore-0.2.3/uvicore/contracts/connection.py
+-rw-r--r--   0        0        0     5514 2023-04-16 17:13:46.548854 uvicore-0.2.3/uvicore/contracts/database.py
+-rw-r--r--   0        0        0     2209 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/contracts/dispatcher.py
+-rw-r--r--   0        0        0      433 2021-05-16 03:31:59.322488 uvicore-0.2.3/uvicore/contracts/email.py
+-rw-r--r--   0        0        0      564 2021-03-02 19:39:30.880258 uvicore-0.2.3/uvicore/contracts/event.py
+-rw-r--r--   0        0        0      759 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/contracts/field.py
+-rw-r--r--   0        0        0     2109 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/contracts/ioc.py
+-rw-r--r--   0        0        0      588 2024-04-21 21:54:30.726005 uvicore-0.2.3/uvicore/contracts/job.py
+-rw-r--r--   0        0        0      570 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/contracts/job_dispatcher.py
+-rw-r--r--   0        0        0     2504 2022-12-18 06:36:42.753628 uvicore-0.2.3/uvicore/contracts/logger.py
+-rw-r--r--   0        0        0     1377 2021-04-05 21:28:22.231229 uvicore-0.2.3/uvicore/contracts/mapper.py
+-rw-r--r--   0        0        0     3814 2022-02-18 20:14:08.924157 uvicore-0.2.3/uvicore/contracts/model.py
+-rw-r--r--   0        0        0     3102 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/contracts/package.py
+-rw-r--r--   0        0        0     2610 2021-01-22 23:57:24.015514 uvicore-0.2.3/uvicore/contracts/provider.py
+-rw-r--r--   0        0        0      742 2020-11-29 06:49:41.074262 uvicore-0.2.3/uvicore/contracts/relation.py
+-rw-r--r--   0        0        0     4254 2024-04-23 21:52:40.607108 uvicore-0.2.3/uvicore/contracts/router.py
+-rw-r--r--   0        0        0      808 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/contracts/routes-OLD.py
+-rw-r--r--   0        0        0      532 2021-03-22 21:25:23.221280 uvicore-0.2.3/uvicore/contracts/server.py
+-rw-r--r--   0        0        0      924 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/contracts/template.py
+-rw-r--r--   0        0        0     2243 2021-08-20 00:01:23.896381 uvicore-0.2.3/uvicore/contracts/user_info.py
+-rw-r--r--   0        0        0     3004 2021-10-14 19:18:41.567853 uvicore-0.2.3/uvicore/contracts/user_provider.py
+-rw-r--r--   0        0        0      704 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/database/__init__.py
+-rw-r--r--   0        0        0    18719 2023-04-16 17:13:46.548854 uvicore-0.2.3/uvicore/database/builder.py
+-rw-r--r--   0        0        0     7979 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/database/commands/db.py
+-rw-r--r--   0        0        0     2527 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/database/commands/generators.py
+-rw-r--r--   0        0        0     4721 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/database/commands/stubs/seeder.py
+-rw-r--r--   0        0        0     3012 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/database/commands/stubs/table.py
+-rw-r--r--   0        0        0     9981 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/database/db.py
+-rw-r--r--   0        0        0     1728 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/database/package/bootstrap.py
+-rw-r--r--   0        0        0     3774 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/database/package/provider.py
+-rw-r--r--   0        0        0     3866 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/database/package/registers.py
+-rw-r--r--   0        0        0     6117 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/database/query.py
+-rw-r--r--   0        0        0     3137 2024-02-10 00:08:36.205626 uvicore-0.2.3/uvicore/database/table.py
+-rw-r--r--   0        0        0      302 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/events/__init__.py
+-rw-r--r--   0        0        0     1415 2021-09-22 05:15:43.413436 uvicore-0.2.3/uvicore/events/commands/event.py
+-rw-r--r--   0        0        0    13029 2021-09-22 05:15:43.413436 uvicore-0.2.3/uvicore/events/dispatcher.py
+-rw-r--r--   0        0        0     2180 2024-04-02 23:02:52.114042 uvicore-0.2.3/uvicore/events/event.py
+-rw-r--r--   0        0        0      143 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/events/handler.py
+-rw-r--r--   0        0        0     2035 2024-04-04 17:37:46.119796 uvicore-0.2.3/uvicore/exceptions/__init__.py
+-rw-r--r--   0        0        0       42 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/factories/__init__.py
+-rw-r--r--   0        0        0      252 2020-09-30 23:16:47.910648 uvicore-0.2.3/uvicore/factories/logger.py
+-rw-r--r--   0        0        0    12711 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/foundation/application.py
+-rw-r--r--   0        0        0      306 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/foundation/commands/app.py
+-rw-r--r--   0        0        0     3926 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/foundation/config/package.py
+-rw-r--r--   0        0        0      291 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/foundation/decorators/__init__.py
+-rw-r--r--   0        0        0      435 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/foundation/decorators/composer.py
+-rw-r--r--   0        0        0      439 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/foundation/decorators/controller.py
+-rw-r--r--   0        0        0      472 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/foundation/decorators/event.py
+-rw-r--r--   0        0        0      429 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/foundation/decorators/job.py
+-rw-r--r--   0        0        0      522 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/foundation/decorators/model.py
+-rw-r--r--   0        0        0      482 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/foundation/decorators/provider.py
+-rw-r--r--   0        0        0      431 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/foundation/decorators/routes.py
+-rw-r--r--   0        0        0      475 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/foundation/decorators/seeder.py
+-rw-r--r--   0        0        0      681 2021-09-07 21:04:46.388597 uvicore-0.2.3/uvicore/foundation/decorators/service.py
+-rw-r--r--   0        0        0      470 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/foundation/decorators/table.py
+-rw-r--r--   0        0        0      893 2021-09-08 13:16:25.207365 uvicore-0.2.3/uvicore/foundation/events/app.py
+-rw-r--r--   0        0        0     5691 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/foundation/package/provider.py
+-rw-r--r--   0        0        0      749 2020-09-30 23:16:47.913981 uvicore-0.2.3/uvicore/http/OBSOLETE/router.py
+-rw-r--r--   0        0        0     1956 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/http/OBSOLETE/routes-OLD.py
+-rw-r--r--   0        0        0      762 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/http/__init__.py
+-rw-r--r--   0        0        0     3210 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/http/commands/generators.py
+-rw-r--r--   0        0        0      418 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/http/commands/routes.py
+-rw-r--r--   0        0        0      570 2020-12-02 20:34:40.502696 uvicore-0.2.3/uvicore/http/commands/serve.py
+-rw-r--r--   0        0        0    12519 2024-04-23 21:52:40.607108 uvicore-0.2.3/uvicore/http/commands/stubs/api_controller.py
+-rw-r--r--   0        0        0      913 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/http/commands/stubs/composer.py
+-rw-r--r--   0        0        0    12890 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/http/commands/stubs/controller.py
+-rw-r--r--   0        0        0       62 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/http/controllers/__init__.py
+-rw-r--r--   0        0        0     5354 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/http/controllers/api.py
+-rw-r--r--   0        0        0     5908 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/http/controllers/web.py
+-rw-r--r--   0        0        0      874 2021-03-24 17:46:21.490777 uvicore-0.2.3/uvicore/http/events/server.py
+-rw-r--r--   0        0        0     4784 2024-04-23 21:52:40.607108 uvicore-0.2.3/uvicore/http/exceptions/__init__.py
+-rw-r--r--   0        0        0     2695 2024-04-23 21:52:40.607108 uvicore-0.2.3/uvicore/http/exceptions/handlers.py
+-rw-r--r--   0        0        0      845 2021-03-13 03:32:22.779743 uvicore-0.2.3/uvicore/http/middleware/__init__.py
+-rw-r--r--   0        0        0    13312 2024-04-10 18:24:17.538912 uvicore-0.2.3/uvicore/http/middleware/authentication.py
+-rw-r--r--   0        0        0     1968 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/http/openapi/docs.py
+-rw-r--r--   0        0        0    30278 2024-04-23 21:52:40.610441 uvicore-0.2.3/uvicore/http/package/bootstrap.py
+-rw-r--r--   0        0        0     3964 2024-04-23 21:52:40.610441 uvicore-0.2.3/uvicore/http/package/provider.py
+-rw-r--r--   0        0        0     4520 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/http/package/registers.py
+-rw-r--r--   0        0        0      855 2024-04-23 21:52:40.610441 uvicore-0.2.3/uvicore/http/params.py
+-rw-r--r--   0        0        0     1787 2024-04-23 21:52:40.610441 uvicore-0.2.3/uvicore/http/rapidoc/docs.py
+-rw-r--r--   0        0        0     1940 2024-04-23 21:52:40.610441 uvicore-0.2.3/uvicore/http/request.py
+-rw-r--r--   0        0        0     4981 2024-04-23 21:52:40.610441 uvicore-0.2.3/uvicore/http/response.py
+-rw-r--r--   0        0        0      455 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/http/routing/__init__.py
+-rw-r--r--   0        0        0    22814 2024-04-23 21:52:40.610441 uvicore-0.2.3/uvicore/http/routing/api_router.py
+-rw-r--r--   0        0        0    10476 2021-10-14 19:18:41.567853 uvicore-0.2.3/uvicore/http/routing/auto_api.py
+-rw-r--r--   0        0        0     4875 2024-04-22 21:55:39.125226 uvicore-0.2.3/uvicore/http/routing/guard.py
+-rw-r--r--   0        0        0    21460 2024-02-21 05:43:11.859354 uvicore-0.2.3/uvicore/http/routing/model_router.py
+-rw-r--r--   0        0        0    21451 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/http/routing/router.py
+-rw-r--r--   0        0        0    16785 2021-09-22 05:15:43.416770 uvicore-0.2.3/uvicore/http/routing/web_router.py
+-rw-r--r--   0        0        0     3521 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/http/server.py
+-rw-r--r--   0        0        0      797 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/http/servers/api.py
+-rw-r--r--   0        0        0      393 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/http/servers/web.py
+-rw-r--r--   0        0        0      865 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/http/static.py
+-rw-r--r--   0        0        0     2517 2021-03-02 19:39:30.883592 uvicore-0.2.3/uvicore/http/status.py
+-rw-r--r--   0        0        0     1609 2021-10-14 19:18:41.567853 uvicore-0.2.3/uvicore/http/templating/context_functions.py
+-rw-r--r--   0        0        0     2280 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/http_client/package/provider.py
+-rw-r--r--   0        0        0       88 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/jobs/__init__.py
+-rw-r--r--   0        0        0      679 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/jobs/dispatcher.py
+-rw-r--r--   0        0        0      902 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/jobs/job.py
+-rw-r--r--   0        0        0      453 2024-04-23 21:52:40.610441 uvicore-0.2.3/uvicore/jobs/results.py
+-rw-r--r--   0        0        0    14997 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/logging/logger.py
+-rw-r--r--   0        0        0     2340 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/logging/package/provider.py
+-rw-r--r--   0        0        0     2608 2021-05-16 03:31:59.322488 uvicore-0.2.3/uvicore/mail/__init__.py
+-rw-r--r--   0        0        0       29 2021-05-16 03:31:59.322488 uvicore-0.2.3/uvicore/mail/backends/__init__.py
+-rw-r--r--   0        0        0     2126 2021-05-16 03:31:59.322488 uvicore-0.2.3/uvicore/mail/backends/mailgun.py
+-rw-r--r--   0        0        0     1181 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/mail/package/provider.py
+-rw-r--r--   0        0        0      181 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/orm/__init__.py
+-rw-r--r--   0        0        0     1395 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/orm/commands/generators.py
+-rw-r--r--   0        0        0     9719 2023-04-16 17:13:46.552188 uvicore-0.2.3/uvicore/orm/commands/stubs/model.py
+-rw-r--r--   0        0        0      447 2021-09-07 21:04:46.391931 uvicore-0.2.3/uvicore/orm/drivers/api.py
+-rw-r--r--   0        0        0        0 2021-03-26 15:13:44.398249 uvicore-0.2.3/uvicore/orm/drivers/sqlalchemy.py
+-rw-r--r--   0        0        0    13295 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/orm/fields.py
+-rw-r--r--   0        0        0     7967 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/orm/mapper.py
+-rw-r--r--   0        0        0    18144 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/orm/metaclass.py
+-rw-r--r--   0        0        0    32661 2024-03-26 17:38:31.288155 uvicore-0.2.3/uvicore/orm/model.py
+-rw-r--r--   0        0        0     3108 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/orm/package/provider.py
+-rw-r--r--   0        0        0    49157 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/orm/query.py
+-rw-r--r--   0        0        0      458 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/package/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/package/commands/package.py
+-rw-r--r--   0        0        0     3490 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/package/package.py
+-rw-r--r--   0        0        0     3676 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/package/provider.py
+-rw-r--r--   0        0        0       40 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/redis/__init__.py
+-rw-r--r--   0        0        0     1218 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/redis/package/bootstrap.py
+-rw-r--r--   0        0        0     3287 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/redis/package/provider.py
+-rw-r--r--   0        0        0      272 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/redis/package/registers.py
+-rw-r--r--   0        0        0     3277 2021-10-14 19:18:41.567853 uvicore-0.2.3/uvicore/redis/redis.py
+-rw-r--r--   0        0        0      407 2020-09-30 23:16:47.913981 uvicore-0.2.3/uvicore/support/README.md
+-rw-r--r--   0        0        0      296 2021-03-29 16:45:06.822538 uvicore-0.2.3/uvicore/support/classes.py
+-rw-r--r--   0        0        0     5162 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/support/collection.py
+-rw-r--r--   0        0        0     2419 2021-03-22 21:25:23.221280 uvicore-0.2.3/uvicore/support/concurrency.py
+-rw-r--r--   0        0        0     1237 2021-03-02 19:39:30.886925 uvicore-0.2.3/uvicore/support/dictionary.py
+-rw-r--r--   0        0        0     1680 2021-01-27 21:25:20.094702 uvicore-0.2.3/uvicore/support/dumper.py
+-rw-r--r--   0        0        0      439 2023-07-16 16:47:20.390563 uvicore-0.2.3/uvicore/support/hash.py
+-rw-r--r--   0        0        0     3771 2023-09-26 21:00:07.189986 uvicore-0.2.3/uvicore/support/module.py
+-rw-r--r--   0        0        0      567 2020-09-30 23:16:47.917315 uvicore-0.2.3/uvicore/support/path.py
+-rw-r--r--   0        0        0     1889 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/support/schematic.py
+-rw-r--r--   0        0        0      623 2020-07-20 18:33:04.439377 uvicore-0.2.3/uvicore/support/singleton.py
+-rw-r--r--   0        0        0     2066 2020-12-31 21:18:43.991950 uvicore-0.2.3/uvicore/support/str.py
+-rw-r--r--   0        0        0     5446 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/templating/engine.py
+-rw-r--r--   0        0        0     2904 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/templating/package/bootstrap.py
+-rw-r--r--   0        0        0     1686 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/templating/package/provider.py
+-rw-r--r--   0        0        0     1024 2024-04-10 18:24:17.542246 uvicore-0.2.3/uvicore/templating/package/registers.py
+-rw-r--r--   0        0        0     2452 2021-09-29 18:14:10.398356 uvicore-0.2.3/uvicore/typing/__init__.py
+-rw-r--r--   0        0        0    12661 2024-04-21 22:06:32.495183 uvicore-0.2.3/uvicore/typing/dictionary.py
+-rw-r--r--   0        0        0     3617 1970-01-01 00:00:00.000000 uvicore-0.2.3/PKG-INFO
```

### Comparing `uvicore-0.2.2/LICENSE` & `uvicore-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/README.md` & `uvicore-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/pyproject.toml` & `uvicore-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uvicore"
-version = "0.2.2"
+version = "0.2.3"
 license = "MIT"
 authors = ["Matthew Reschke <mail@mreschke.com>"]
 description = "The Fullstack Async Web, API and CLI Python Framework"
 readme = "README.md"
 homepage = "https://github.com/uvicore/framework"
 documentation = "https://github.com/uvicore/framework"
 repository = "https://github.com/uvicore/framework"
```

### Comparing `uvicore-0.2.2/uvicore/__init__.py` & `uvicore-0.2.3/uvicore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # type: ignore
 from . import contracts
 from uvicore.typing import Dict
 from uvicore.foundation.decorators import event, job, model, seeder, service, table, provider, routes, controller, composer
 
 
 # Uvicore version.  Also available in app.version
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 
 # Core (non service provider based) singletons as globals
 ioc: contracts.Ioc = None
 events: contracts.Dispatcher = None
 jobs: contracts.JobDispatcher = None
 app: contracts.Application = None
```

### Comparing `uvicore-0.2.2/uvicore/auth/authenticators/base.py` & `uvicore-0.2.3/uvicore/auth/authenticators/base.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/authenticators/basic.py` & `uvicore-0.2.3/uvicore/auth/authenticators/basic.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/authenticators/jwt.py` & `uvicore-0.2.3/uvicore/auth/authenticators/jwt.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/config/package.py` & `uvicore-0.2.3/uvicore/auth/config/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/database/seeders/groups.py` & `uvicore-0.2.3/uvicore/auth/database/seeders/groups.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/database/seeders/permissions.py` & `uvicore-0.2.3/uvicore/auth/database/seeders/permissions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/database/seeders/roles.py` & `uvicore-0.2.3/uvicore/auth/database/seeders/roles.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/database/seeders/users.py` & `uvicore-0.2.3/uvicore/auth/database/seeders/users.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/database/tables/group_roles.py` & `uvicore-0.2.3/uvicore/auth/database/tables/group_roles.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/database/tables/groups.py` & `uvicore-0.2.3/uvicore/auth/database/tables/groups.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/database/tables/permissions.py` & `uvicore-0.2.3/uvicore/auth/database/tables/permissions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/database/tables/role_permissions.py` & `uvicore-0.2.3/uvicore/auth/database/tables/role_permissions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/database/tables/roles.py` & `uvicore-0.2.3/uvicore/auth/database/tables/roles.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/database/tables/user_groups.py` & `uvicore-0.2.3/uvicore/auth/database/tables/user_groups.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/database/tables/user_roles.py` & `uvicore-0.2.3/uvicore/auth/database/tables/user_roles.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/database/tables/users.py` & `uvicore-0.2.3/uvicore/auth/database/tables/users.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/http/routes/api.py` & `uvicore-0.2.3/uvicore/auth/http/routes/api.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/middleware/auth_OLD.py` & `uvicore-0.2.3/uvicore/auth/middleware/auth_OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/middleware/basic_OLD.py` & `uvicore-0.2.3/uvicore/auth/middleware/basic_OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/middleware/jwt_OLD.py` & `uvicore-0.2.3/uvicore/auth/middleware/jwt_OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/models/group.py` & `uvicore-0.2.3/uvicore/auth/models/group.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/models/permission.py` & `uvicore-0.2.3/uvicore/auth/models/permission.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/models/role.py` & `uvicore-0.2.3/uvicore/auth/models/role.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/models/user.py` & `uvicore-0.2.3/uvicore/auth/models/user.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/package/provider.py` & `uvicore-0.2.3/uvicore/auth/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/support/password.py` & `uvicore-0.2.3/uvicore/auth/support/password.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/user_info.py` & `uvicore-0.2.3/uvicore/auth/user_info.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/user_providers/jwt.py` & `uvicore-0.2.3/uvicore/auth/user_providers/jwt.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/auth/user_providers/orm.py` & `uvicore-0.2.3/uvicore/auth/user_providers/orm.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/cache/backends/array.py` & `uvicore-0.2.3/uvicore/cache/backends/array.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/cache/backends/redis.py` & `uvicore-0.2.3/uvicore/cache/backends/redis.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/cache/manager.py` & `uvicore-0.2.3/uvicore/cache/manager.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/cache/package/provider.py` & `uvicore-0.2.3/uvicore/cache/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/configuration/commands/config.py` & `uvicore-0.2.3/uvicore/configuration/commands/config.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/configuration/configuration.py` & `uvicore-0.2.3/uvicore/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/configuration/package/provider.py` & `uvicore-0.2.3/uvicore/configuration/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/__init__.py` & `uvicore-0.2.3/uvicore/console/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/LICENSE.rst` & `uvicore-0.2.3/uvicore/console/asyncclick/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/__init__.py` & `uvicore-0.2.3/uvicore/console/asyncclick/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/_bashcomplete.py` & `uvicore-0.2.3/uvicore/console/asyncclick/_bashcomplete.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/_compat.py` & `uvicore-0.2.3/uvicore/console/asyncclick/_compat.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/_termui_impl.py` & `uvicore-0.2.3/uvicore/console/asyncclick/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/_textwrap.py` & `uvicore-0.2.3/uvicore/console/asyncclick/_textwrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/_unicodefun.py` & `uvicore-0.2.3/uvicore/console/asyncclick/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/_winconsole.py` & `uvicore-0.2.3/uvicore/console/asyncclick/_winconsole.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/core.py` & `uvicore-0.2.3/uvicore/console/asyncclick/core.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/decorators.py` & `uvicore-0.2.3/uvicore/console/asyncclick/decorators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/exceptions.py` & `uvicore-0.2.3/uvicore/console/asyncclick/exceptions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/formatting.py` & `uvicore-0.2.3/uvicore/console/asyncclick/formatting.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/globals.py` & `uvicore-0.2.3/uvicore/console/asyncclick/globals.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/parser.py` & `uvicore-0.2.3/uvicore/console/asyncclick/parser.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/termui.py` & `uvicore-0.2.3/uvicore/console/asyncclick/termui.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/testing.py` & `uvicore-0.2.3/uvicore/console/asyncclick/testing.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/types.py` & `uvicore-0.2.3/uvicore/console/asyncclick/types.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/asyncclick/utils.py` & `uvicore-0.2.3/uvicore/console/asyncclick/utils.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/click_colors.py` & `uvicore-0.2.3/uvicore/console/click_colors.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/commands/generators.py` & `uvicore-0.2.3/uvicore/console/commands/generators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/commands/stubs/command.py` & `uvicore-0.2.3/uvicore/console/commands/stubs/command.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/console.py` & `uvicore-0.2.3/uvicore/console/console.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/decorators.py` & `uvicore-0.2.3/uvicore/console/decorators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/events/command.py` & `uvicore-0.2.3/uvicore/console/events/command.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/package/bootstrap.py` & `uvicore-0.2.3/uvicore/console/package/bootstrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/package/provider.py` & `uvicore-0.2.3/uvicore/console/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/console/package/registers.py` & `uvicore-0.2.3/uvicore/console/package/registers.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/container/commands/ioc.py` & `uvicore-0.2.3/uvicore/container/commands/ioc.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/container/ioc.py` & `uvicore-0.2.3/uvicore/container/ioc.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/__init__.py` & `uvicore-0.2.3/uvicore/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/application.py` & `uvicore-0.2.3/uvicore/contracts/application.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/authenticator.py` & `uvicore-0.2.3/uvicore/contracts/authenticator.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/builder.py` & `uvicore-0.2.3/uvicore/contracts/builder.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/cache.py` & `uvicore-0.2.3/uvicore/contracts/cache.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/config.py` & `uvicore-0.2.3/uvicore/contracts/config.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/connection.py` & `uvicore-0.2.3/uvicore/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/database.py` & `uvicore-0.2.3/uvicore/contracts/database.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/dispatcher.py` & `uvicore-0.2.3/uvicore/contracts/dispatcher.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/event.py` & `uvicore-0.2.3/uvicore/contracts/event.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/field.py` & `uvicore-0.2.3/uvicore/contracts/field.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/ioc.py` & `uvicore-0.2.3/uvicore/contracts/ioc.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/job.py` & `uvicore-0.2.3/uvicore/contracts/job.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/job_dispatcher.py` & `uvicore-0.2.3/uvicore/contracts/job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/logger.py` & `uvicore-0.2.3/uvicore/contracts/logger.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/mapper.py` & `uvicore-0.2.3/uvicore/contracts/mapper.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/model.py` & `uvicore-0.2.3/uvicore/contracts/model.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/package.py` & `uvicore-0.2.3/uvicore/contracts/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/provider.py` & `uvicore-0.2.3/uvicore/contracts/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/relation.py` & `uvicore-0.2.3/uvicore/contracts/relation.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/router.py` & `uvicore-0.2.3/uvicore/contracts/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     # This is still a fully dynamic SuperDict!
     path: str
     name: str
     prefix: bool
     endpoint: Callable
     methods: List[str]
     response_model: Optional[Any]
+    response_class: Optional[Any]
     tags: Optional[List]
     middleware: Optional[List]
     summary: Optional[str]
     description: Optional[str]
     original_path: str
     original_name: str
```

### Comparing `uvicore-0.2.2/uvicore/contracts/routes-OLD.py` & `uvicore-0.2.3/uvicore/contracts/routes-OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/server.py` & `uvicore-0.2.3/uvicore/contracts/server.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/template.py` & `uvicore-0.2.3/uvicore/contracts/template.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/user_info.py` & `uvicore-0.2.3/uvicore/contracts/user_info.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/contracts/user_provider.py` & `uvicore-0.2.3/uvicore/contracts/user_provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/database/__init__.py` & `uvicore-0.2.3/uvicore/database/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/database/builder.py` & `uvicore-0.2.3/uvicore/database/builder.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/database/commands/db.py` & `uvicore-0.2.3/uvicore/database/commands/db.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/database/commands/generators.py` & `uvicore-0.2.3/uvicore/database/commands/generators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/database/commands/stubs/seeder.py` & `uvicore-0.2.3/uvicore/database/commands/stubs/seeder.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/database/commands/stubs/table.py` & `uvicore-0.2.3/uvicore/database/commands/stubs/table.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/database/db.py` & `uvicore-0.2.3/uvicore/database/db.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/database/package/bootstrap.py` & `uvicore-0.2.3/uvicore/database/package/bootstrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/database/package/provider.py` & `uvicore-0.2.3/uvicore/database/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/database/package/registers.py` & `uvicore-0.2.3/uvicore/database/package/registers.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/database/query.py` & `uvicore-0.2.3/uvicore/database/query.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/database/table.py` & `uvicore-0.2.3/uvicore/database/table.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/events/commands/event.py` & `uvicore-0.2.3/uvicore/events/commands/event.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/events/dispatcher.py` & `uvicore-0.2.3/uvicore/events/dispatcher.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/events/event.py` & `uvicore-0.2.3/uvicore/events/event.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/exceptions/__init__.py` & `uvicore-0.2.3/uvicore/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/foundation/application.py` & `uvicore-0.2.3/uvicore/foundation/application.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/foundation/config/package.py` & `uvicore-0.2.3/uvicore/foundation/config/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/foundation/decorators/model.py` & `uvicore-0.2.3/uvicore/foundation/decorators/model.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/foundation/decorators/service.py` & `uvicore-0.2.3/uvicore/foundation/decorators/service.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/foundation/events/app.py` & `uvicore-0.2.3/uvicore/foundation/events/app.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/foundation/package/provider.py` & `uvicore-0.2.3/uvicore/foundation/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/OBSOLETE/router.py` & `uvicore-0.2.3/uvicore/http/OBSOLETE/router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/OBSOLETE/routes-OLD.py` & `uvicore-0.2.3/uvicore/http/OBSOLETE/routes-OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/__init__.py` & `uvicore-0.2.3/uvicore/http/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/commands/generators.py` & `uvicore-0.2.3/uvicore/http/commands/generators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/commands/serve.py` & `uvicore-0.2.3/uvicore/http/commands/serve.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/commands/stubs/api_controller.py` & `uvicore-0.2.3/uvicore/http/commands/stubs/api_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import uvicore
+from uvicore.typing import Dict
 from uvicore.http import Request
+from uvicore.http.exceptions import HTTPException
 from uvicore.http.routing import ApiRouter, Controller
 
 # Extra
 # from uvicore.auth import UserInfo
 # from uvicore.http.routing import Guard
 # from uvicore.typing import Dict, List, Optional
 # from uvicore.http.exceptions import HTTPException
@@ -49,15 +51,18 @@
 
         # ----------------------------------------------------------------------
         # Example: Basic route responding with a view dict to JSON blob
         # ----------------------------------------------------------------------
         @route.get('/example1', tags=['Examples'])
         async def example1() -> Dict:
             """This docstring shows up in openapi"""
-            return {'welcome': 'to uvicore API!'}
+            try:
+                return {'welcome': 'to uvicore API!'}
+            except Exception as e:
+                raise HTTPException(500, exception=e)
 
 
         # ----------------------------------------------------------------------
         # Example: Route returning a Model schema with python return type hint
         # ----------------------------------------------------------------------
         # @route.get('/example2', tags=['Examples'])
         # async def example2()) -> List[models.Post]:
```

### Comparing `uvicore-0.2.2/uvicore/http/commands/stubs/composer.py` & `uvicore-0.2.3/uvicore/http/commands/stubs/composer.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/commands/stubs/controller.py` & `uvicore-0.2.3/uvicore/http/commands/stubs/controller.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/controllers/api.py` & `uvicore-0.2.3/uvicore/http/controllers/api.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/controllers/web.py` & `uvicore-0.2.3/uvicore/http/controllers/web.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/events/server.py` & `uvicore-0.2.3/uvicore/http/events/server.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/exceptions/__init__.py` & `uvicore-0.2.3/uvicore/http/exceptions/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import uvicore
+import traceback
 from uvicore.typing import Any, Dict, Optional, List
 from starlette.exceptions import HTTPException as _HTTPException
 from uvicore.http import status
+from uvicore.support.dumper import dump
+from uvicore.support.collection import haskey
 
 # This is how you could do it, if you wanted to log
 #log = lambda : uvicore.log.name('uvicore.http')
 
 # See https://www.restapitutorial.com/httpstatuscodes.html for a good list to follow
 
 class HTTPException(_HTTPException):
@@ -19,14 +22,31 @@
         detail: Optional[str] = None,
         *,
         message: Optional[str] = None,
         exception: Optional[str] = None,
         extra: Optional[Dict] = None,
         headers: Optional[Dict[str, Any]] = None
     ) -> None:
+        # Detect if we were raised from another HTTPException with a status_code
+        # If so, grab values from that first exception
+        if exception is not None and haskey(exception, 'status_code'):
+            status_code = exception.status_code
+            message = exception.message
+            detail = exception.detail
+            extra = exception.extra
+            headers = exception.headers
+            exception = None
+        else:
+            # Standard try catch that raises HTTPException
+            st = traceback.format_exc()
+            if 'NoneType' in st: st = None
+            message = message or str(exception)
+            detail = detail or message
+            exception = st
+
         # Call starlette exception where their detail is my message
         super().__init__(status_code=status_code, detail=message)
 
         # Swap starlette detail to my message
         self.message = self.detail
         self.detail = detail
         self.exception = exception if uvicore.config.app.debug else None  # Hidden unless in debug mode
```

### Comparing `uvicore-0.2.2/uvicore/http/exceptions/handlers.py` & `uvicore-0.2.3/uvicore/http/exceptions/handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-from uvicore.http import response
 from uvicore.http import Request
+from uvicore.http import response
 from uvicore.http.exceptions import HTTPException
-from uvicore.support.dumper import dump
 
 
 async def api(request: Request, e: HTTPException) -> response.JSON:
     """Main exception handler for all API endpoints"""
 
-    # Get error payload (smart based on uvicore or starlette HTTPException)
-    (status_code, detail, message, exception, extra, headers) = _get_payload(e)
+    # Get error payload (smart based on uvicore or stock HTTPException)
+    (status_code, detail, message, exception, extra, headers) = expand_payload(e)
     return response.JSON(
         {
             "status_code": status_code,
             "message": message,
             "detail": detail,
             "exception": exception,
             "extra": extra,
         }, status_code=status_code, headers=headers
     )
 
 
 async def web(request: Request, e: HTTPException) -> response.HTML:
     """Main exception handler for all Web endpoints"""
 
-    # Get error payload (smart based on uvicore or starlette HTTPException)
-    (status_code, detail, message, exception, extra, headers) = _get_payload(e)
+    # Get error payload (smart based on uvicore or stock HTTPException)
+    (status_code, detail, message, exception, extra, headers) = expand_payload(e)
 
     try:
         # Try to respond with a errors template, if exists
         return await response.View('errors/' + str(status_code) + '.j2', {
             'request': request,
             **e.__dict__,
         })
     except:
 
         try:
             # Try to respond with a catch_all template, if exists
-            # Uvicore does not have one, but mreschke/themes which is usually included with a package DOES!
             return await response.View('errors/catch_all.j2', {
                 'request': request,
                 **e.__dict__,
             })
         except:
-            # Errors status_code or catch_all template does not exist, response with generic HTML error
+            # Errors status_code or catch_all template does not exist.
+            # Response with generic HTML error
             html = f"""
             <div class="error">
                 <h1>{status_code} {message}</h1>
                 <p>{detail or ''}</p>
 
                 <h3>Exception:</h3>
                 <p>{exception or ''}</p>
@@ -57,26 +56,27 @@
             """
             return response.HTML(
                 content=html,
                 status_code=status_code,
                 headers=headers
             )
 
-def _get_payload(e: HTTPException):
-    """Get error payload depending on uvicore or starlette HTTPException"""
+
+def expand_payload(e: HTTPException):
+    """Get error payload depending on uvicore or stock HTTPException"""
     # Defined in the running app config api.exceptions.main
     headers = getattr(e, "headers", None)
 
-    # Base starletting only has status_code and detail
+    # Base only has status_code and detail
     status_code = e.status_code
     detail = e.detail
     exception = None
     if (hasattr(e, 'message')):
         # Error called using uvicores new and expanded HTTPException
         message = e.message
         exception = e.exception
         extra = e.extra
     else:
-        # Error called using starlette HTTPException
+        # Error called using base HTTPException
         message = e.detail
         extra = None
     return (status_code, detail, message, exception, extra, headers)
```

### Comparing `uvicore-0.2.2/uvicore/http/middleware/__init__.py` & `uvicore-0.2.3/uvicore/http/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/middleware/authentication.py` & `uvicore-0.2.3/uvicore/http/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/openapi/docs.py` & `uvicore-0.2.3/uvicore/http/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/package/bootstrap.py` & `uvicore-0.2.3/uvicore/http/package/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from uvicore.http import response
 from uvicore.http.events import server as HttpServerEvents
 from uvicore.http.routing.router import Routes
 from functools import partial, update_wrapper
 from uvicore.http.routing import ApiRoute, WebRoute
 from uvicore.http.routing import Guard
 from uvicore.http.openapi.docs import get_swagger_ui_html, get_swagger_ui_oauth2_redirect_html
+from uvicore.http.rapidoc.docs import get_rapidoc_ui_html, get_rapidoc_pdf_ui_html, get_rapidoc_ui_oauth2_redirect_html
 
 # Temp speed testing variable to swap Web router from FastAPI to Starlette
 # NOTICE if you set this to TRUE, all your type hinded /{vars} and ?vars will NOT
 # work in your routes and you will have to revert to Starlettes way of
 # handling vars with request.path_params['user_id'] which will break all your apps.
 USE_STARLETTE=False
 
@@ -289,15 +290,15 @@
                 debug=debug,
 
                 #openapi_prefix=api_prefix,
                 #root_path=api_prefix,
                 #openapi_url='/api/openapi.json',
 
                 #docs_url='/api/docs',
-                #redoc_url='/api/redoc',
+                #redoc_url='/api/`redoc`',
 
                 # This title is what shows up in OpenAPI <h1>, not the HTML <title>, which is defined in add_api_routes def openapi_docs()
                 title=uvicore.config('app.api.openapi.title'),
 
                 # Get version from main running apps package.version
                 version=uvicore.app.package(main=True).version,
 
@@ -310,16 +311,17 @@
                 #docs_url=uvicore.config('app.api.openapi.docs_url'),
                 #redoc_url=uvicore.config('app.api.openapi.redoc_url'),
 
                 # DISABLE the /docs and /redoc URLs
                 # Why?  Because we add our own CUSTOM one later in add_api_routes()
                 docs_url=None,
 
+                # DISABLE redoc
                 # Can leave redoc on for now, maybe add to config to change /redoc path
-                #redoc_url=None,
+                redoc_url=None,
 
                 #swagger_ui_oauth2_redirect_url=
 
                 #root_path='/api',  #fixme with trying out kong
             )
 
 
@@ -448,25 +450,49 @@
 
         # Do nothing if no api_routes are defined
         if not api_routes: return
 
         # Get important app configs
         api_prefix = self.get_prefix('app.api.prefix')
         openapi = uvicore.config.app.api.openapi
+        rapidoc = uvicore.config.app.api.rapidoc
         oauth2 = uvicore.config.app.auth.oauth2
 
         # Determine if OpenAPI docs oauth2 authentication is enabled
         # If OpenAPI oauth2 is enabled, create a FastAPI OAuth2AuthorizationCodeBearer variable
         if openapi.oauth2_enabled and oauth2:
             from fastapi.security import OAuth2AuthorizationCodeBearer
             oauth2_scheme = OAuth2AuthorizationCodeBearer(
                 authorizationUrl=oauth2.base_url + oauth2.authorize_path,
                 tokenUrl=oauth2.base_url + oauth2.token_path,
             )
 
+        # Create our own custom RapiDoc docs route
+        if rapidoc.path and openapi.path:
+
+            # Oauth2 redirect URL (without api_prefid)
+            rapidoc_redirect_url =  rapidoc.path + '/oauth-receiver.html'
+
+            @api_server.get(rapidoc.path, include_in_schema=False)
+            def rapidoc_docs():
+                return get_rapidoc_ui_html(
+                    openapi_url=api_prefix + openapi.path,
+                )
+
+            @api_server.get(rapidoc.pdf_path, include_in_schema=False)
+            def rapidoc_docs():
+                return get_rapidoc_pdf_ui_html(
+                    openapi_url=api_prefix + openapi.path,
+                )
+
+            @api_server.get(rapidoc_redirect_url, include_in_schema=False)
+            def rapidoc_redirect():
+                return get_rapidoc_ui_oauth2_redirect_html()
+
+
         # Create our own custom OpenAPI docs route
         if openapi.path and openapi.docs.path:
 
             # Oauth2 redirect URL (without api_prefid)
             openapi_redirect_url =  openapi.docs.path + '/login'
 
             @api_server.get(openapi.docs.path, include_in_schema=False)
@@ -547,14 +573,15 @@
             api_server.add_api_route(
                 #path=(prefix + route.path) or '/',
                 path=(route.path) or '/',
                 endpoint=route.endpoint,
                 methods=route.methods,
                 name=route.name,
                 response_model=route.response_model,
+                response_class=route.response_class or response.JSONResponse,
                 responses=route.responses,
                 tags=route.tags,
                 dependencies=route.middleware,
                 summary=route.summary,
                 description=route.description,
             )
```

### Comparing `uvicore-0.2.2/uvicore/http/package/registers.py` & `uvicore-0.2.3/uvicore/http/package/registers.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/response.py` & `uvicore-0.2.3/uvicore/http/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,29 @@
 from uvicore.typing import Dict, List
 from uvicore.support.dumper import dump
 from uvicore.support.module import load
 from uvicore.http.request import Request
 from starlette.templating import _TemplateResponse
 from starlette.background import BackgroundTask as _BackgroundTask
 
-# Proxy starlette response APIs
+# Proxy starlette and fastapi response APIs
+# Usage: from uvicore.http.response import FileResponse
+#    Or: from uvicore.http import response
+#        response.File
+# See https://fastapi.tiangolo.com/reference/responses/
 from starlette.responses import Response
-from starlette.responses import PlainTextResponse as Text
-from starlette.responses import HTMLResponse as HTML
-from starlette.responses import JSONResponse as JSON
-from fastapi.responses import UJSONResponse as UJSON
-from fastapi.responses import ORJSONResponse as ORJSON
-from starlette.responses import RedirectResponse as Redirect
-from starlette.responses import StreamingResponse as Stream
-from starlette.responses import FileResponse as File
+from starlette.responses import FileResponse, FileResponse as File
+from starlette.responses import HTMLResponse, HTMLResponse as HTML
+from starlette.responses import JSONResponse, JSONResponse as JSON
+from fastapi.responses import UJSONResponse, UJSONResponse as UJSON
+from fastapi.responses import ORJSONResponse, ORJSONResponse as ORJSON
+from starlette.responses import PlainTextResponse, PlainTextResponse as Text
+from starlette.responses import RedirectResponse, RedirectResponse as Redirect
+from starlette.responses import StreamingResponse, StreamingResponse as Stream
+
 
 # Get our current template system from the IoC
 #templates = uvicore.ioc.make('uvicore.http.templating.jinja.Jinja')
 #templates = uvicore.ioc.make('uvicore.http.templating.engine.Templates')
 templates = uvicore.ioc.make('uvicore.templating.engine.Templates')
 #templates = uvicore.ioc.make('Templates') # Fixme when you impliment other templating engines, if ever
```

### Comparing `uvicore-0.2.2/uvicore/http/routing/api_router.py` & `uvicore-0.2.3/uvicore/http/routing/api_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 import uvicore
-from uvicore.typing import Any, Callable, List, Dict, Optional, Decorator, get_type_hints
+from uvicore.typing import Any, Callable, List, Dict, Optional, Decorator, get_type_hints, Union, Type
 from uvicore.http.routing.router import Router
 from uvicore.contracts import ApiRoute as RouteInterface
 from prettyprinter import pretty_call, register_pretty
 from uvicore.support.dumper import dump, dd
 from merge_args import _merge as merge_args
 from functools import partial
+from uvicore.http.response import Response, JSON as JSONResponse
+from fastapi.datastructures import Default, DefaultPlaceholder
 
 
 from uvicore.http.routing.guard import Guard
 #from uvicore.auth.middleware.auth import Guard
 
 # from fastapi import APIRouter as _FastAPIRouter
 # from uvicore.typing import Any, Type, List, Callable, Optional
@@ -35,14 +37,15 @@
         auth: Optional[Guard] = None,
         scopes: Optional[List] = None,
         inherits: Optional[Callable] = None,
 
         # ApiRouter specific
         responses: Optional[Dict] = None,
         response_model: Optional[Any] = None,
+        response_class: Optional[Type[Response]] = None,
         tags: Optional[List[str]] = None,
         summary: Optional[str] = None,
         description: Optional[str] = None,
     ) -> None:
         """Add a new HTTP GET route to the ApiRouter
 
         :param path: URL path, beginning with /
@@ -78,14 +81,15 @@
         auth: Optional[Guard] = None,
         scopes: Optional[List] = None,
         inherits: Optional[Callable] = None,
 
         # ApiRouter specific
         responses: Optional[Dict] = None,
         response_model: Optional[Any] = None,
+        response_class: Optional[Type[Response]] = None,
         tags: Optional[List[str]] = None,
         summary: Optional[str] = None,
         description: Optional[str] = None,
     ):
         """Add a new HTTP POST route to the ApiRouter
 
         :param path: URL path, beginning with /
@@ -121,14 +125,15 @@
         auth: Optional[Guard] = None,
         scopes: Optional[List] = None,
         inherits: Optional[Callable] = None,
 
         # ApiRouter specific
         responses: Optional[Dict] = None,
         response_model: Optional[Any] = None,
+        response_class: Optional[Type[Response]] = None,
         tags: Optional[List[str]] = None,
         summary: Optional[str] = None,
         description: Optional[str] = None,
     ):
         """Add a new HTTP PUT route to the ApiRouter
 
         :param path: URL path, beginning with /
@@ -164,14 +169,15 @@
         auth: Optional[Guard] = None,
         scopes: Optional[List] = None,
         inherits: Optional[Callable] = None,
 
         # ApiRouter specific
         responses: Optional[Dict] = None,
         response_model: Optional[Any] = None,
+        response_class: Optional[Type[Response]] = None,
         tags: Optional[List[str]] = None,
         summary: Optional[str] = None,
         description: Optional[str] = None,
     ):
         """Add a new HTTP PATCH route to the ApiRouter
 
         :param path: URL path, beginning with /
@@ -207,14 +213,15 @@
         auth: Optional[Guard] = None,
         scopes: Optional[List] = None,
         inherits: Optional[Callable] = None,
 
         # ApiRouter specific
         responses: Optional[Dict] = None,
         response_model: Optional[Any] = None,
+        response_class: Optional[Type[Response]] = None,
         tags: Optional[List[str]] = None,
         summary: Optional[str] = None,
         description: Optional[str] = None,
     ):
         """Add a new HTTP DELETE route to the ApiRouter
 
         :param path: URL path, beginning with /
@@ -251,14 +258,15 @@
         auth: Optional[Guard] = None,
         scopes: Optional[List] = None,
         inherits: Optional[Callable] = None,
 
         # ApiRouter specific
         responses: Optional[Dict] = None,
         response_model: Optional[Any] = None,
+        response_class: Optional[Type[Response]] = None,
         tags: Optional[List[str]] = None,
         summary: Optional[str] = None,
         description: Optional[str] = None,
     ) -> Callable[[Decorator], Decorator]:
         """Add a new HTTP method route to the ApiRouter
 
         :param path: URL path, beginning with /
@@ -319,14 +327,15 @@
                 'autoprefix': autoprefix,
                 'original_path': path,
                 'original_name': name,
                 'responses': responses,
 
                 # ApiRouter specific
                 'response_model': response_model,
+                'response_class': response_class,
                 'tags': tags,
                 'summary': summary,
                 'description': description,
             })
             # Full name already contains -POST, -PUT...for uniqueness across methods
             self.routes[full_name] = route
             return route
```

### Comparing `uvicore-0.2.2/uvicore/http/routing/auto_api.py` & `uvicore-0.2.3/uvicore/http/routing/auto_api.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/routing/guard.py` & `uvicore-0.2.3/uvicore/http/routing/guard.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/routing/model_router.py` & `uvicore-0.2.3/uvicore/http/routing/model_router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/routing/router.py` & `uvicore-0.2.3/uvicore/http/routing/router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/routing/web_router.py` & `uvicore-0.2.3/uvicore/http/routing/web_router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/server.py` & `uvicore-0.2.3/uvicore/http/server.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/servers/api.py` & `uvicore-0.2.3/uvicore/http/servers/api.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/static.py` & `uvicore-0.2.3/uvicore/http/static.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/status.py` & `uvicore-0.2.3/uvicore/http/status.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http/templating/context_functions.py` & `uvicore-0.2.3/uvicore/http/templating/context_functions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/http_client/package/provider.py` & `uvicore-0.2.3/uvicore/http_client/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/jobs/dispatcher.py` & `uvicore-0.2.3/uvicore/jobs/dispatcher.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/jobs/job.py` & `uvicore-0.2.3/uvicore/jobs/job.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/logging/logger.py` & `uvicore-0.2.3/uvicore/logging/logger.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/logging/package/provider.py` & `uvicore-0.2.3/uvicore/logging/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/mail/__init__.py` & `uvicore-0.2.3/uvicore/mail/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/mail/backends/mailgun.py` & `uvicore-0.2.3/uvicore/mail/backends/mailgun.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/mail/package/provider.py` & `uvicore-0.2.3/uvicore/mail/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/orm/commands/generators.py` & `uvicore-0.2.3/uvicore/orm/commands/generators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/orm/commands/stubs/model.py` & `uvicore-0.2.3/uvicore/orm/commands/stubs/model.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/orm/fields.py` & `uvicore-0.2.3/uvicore/orm/fields.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/orm/mapper.py` & `uvicore-0.2.3/uvicore/orm/mapper.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/orm/metaclass.py` & `uvicore-0.2.3/uvicore/orm/metaclass.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/orm/model.py` & `uvicore-0.2.3/uvicore/orm/model.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/orm/package/provider.py` & `uvicore-0.2.3/uvicore/orm/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/orm/query.py` & `uvicore-0.2.3/uvicore/orm/query.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/package/commands/package.py` & `uvicore-0.2.3/uvicore/package/commands/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/package/package.py` & `uvicore-0.2.3/uvicore/package/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/package/provider.py` & `uvicore-0.2.3/uvicore/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/redis/package/bootstrap.py` & `uvicore-0.2.3/uvicore/redis/package/bootstrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/redis/package/provider.py` & `uvicore-0.2.3/uvicore/redis/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/redis/redis.py` & `uvicore-0.2.3/uvicore/redis/redis.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/support/collection.py` & `uvicore-0.2.3/uvicore/support/collection.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/support/concurrency.py` & `uvicore-0.2.3/uvicore/support/concurrency.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/support/dictionary.py` & `uvicore-0.2.3/uvicore/support/dictionary.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/support/dumper.py` & `uvicore-0.2.3/uvicore/support/dumper.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/support/module.py` & `uvicore-0.2.3/uvicore/support/module.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/support/path.py` & `uvicore-0.2.3/uvicore/support/path.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/support/schematic.py` & `uvicore-0.2.3/uvicore/support/schematic.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/support/singleton.py` & `uvicore-0.2.3/uvicore/support/singleton.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/support/str.py` & `uvicore-0.2.3/uvicore/support/str.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/templating/engine.py` & `uvicore-0.2.3/uvicore/templating/engine.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/templating/package/bootstrap.py` & `uvicore-0.2.3/uvicore/templating/package/bootstrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/templating/package/provider.py` & `uvicore-0.2.3/uvicore/templating/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/templating/package/registers.py` & `uvicore-0.2.3/uvicore/templating/package/registers.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/typing/__init__.py` & `uvicore-0.2.3/uvicore/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/uvicore/typing/dictionary.py` & `uvicore-0.2.3/uvicore/typing/dictionary.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.2.2/PKG-INFO` & `uvicore-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvicore
-Version: 0.2.2
+Version: 0.2.3
 Summary: The Fullstack Async Web, API and CLI Python Framework
 Home-page: https://github.com/uvicore/framework
 License: MIT
 Author: Matthew Reschke
 Author-email: mail@mreschke.com
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
```

