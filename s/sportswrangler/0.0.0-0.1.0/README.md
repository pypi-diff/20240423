# Comparing `tmp/sportswrangler-0.0.0.tar.gz` & `tmp/sportswrangler-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sportswrangler-0.0.0.tar", last modified: Tue Apr  9 04:42:32 2024, max compression
+gzip compressed data, was "sportswrangler-0.1.0.tar", max compression
```

## Comparing `sportswrangler-0.0.0.tar` & `sportswrangler-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,34 @@
-drwxr-xr-x   0 dejon      (501) staff       (20)        0 2024-04-09 04:42:32.769540 sportswrangler-0.0.0/
--rw-r--r--   0 dejon      (501) staff       (20)       58 2024-04-09 04:42:32.769348 sportswrangler-0.0.0/PKG-INFO
--rw-r--r--   0 dejon      (501) staff       (20)        0 2024-04-09 04:42:06.000000 sportswrangler-0.0.0/pyproject.toml
--rw-r--r--   0 dejon      (501) staff       (20)       38 2024-04-09 04:42:32.769577 sportswrangler-0.0.0/setup.cfg
-drwxr-xr-x   0 dejon      (501) staff       (20)        0 2024-04-09 04:42:32.768551 sportswrangler-0.0.0/sportswrangler/
--rw-r--r--   0 dejon      (501) staff       (20)        0 2024-04-09 04:41:30.000000 sportswrangler-0.0.0/sportswrangler/__init__.py
-drwxr-xr-x   0 dejon      (501) staff       (20)        0 2024-04-09 04:42:32.769172 sportswrangler-0.0.0/sportswrangler.egg-info/
--rw-r--r--   0 dejon      (501) staff       (20)       58 2024-04-09 04:42:32.000000 sportswrangler-0.0.0/sportswrangler.egg-info/PKG-INFO
--rw-r--r--   0 dejon      (501) staff       (20)      193 2024-04-09 04:42:32.000000 sportswrangler-0.0.0/sportswrangler.egg-info/SOURCES.txt
--rw-r--r--   0 dejon      (501) staff       (20)        1 2024-04-09 04:42:32.000000 sportswrangler-0.0.0/sportswrangler.egg-info/dependency_links.txt
--rw-r--r--   0 dejon      (501) staff       (20)       15 2024-04-09 04:42:32.000000 sportswrangler-0.0.0/sportswrangler.egg-info/top_level.txt
+-rw-r--r--   0        0        0      454 2024-04-23 02:09:58.022221 sportswrangler-0.1.0/README.md
+-rw-r--r--   0        0        0      422 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      102 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/generic/__init__.py
+-rw-r--r--   0        0        0     2065 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/generic/wrangler.py
+-rw-r--r--   0        0        0      154 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/global_configs.py
+-rw-r--r--   0        0        0        0 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/__init__.py
+-rw-r--r--   0        0        0      206 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/utils/__init__.py
+-rw-r--r--   0        0        0     3732 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/utils/classes.py
+-rw-r--r--   0        0        0      238 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/utils/constants.py
+-rw-r--r--   0        0        0     4739 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/utils/enums.py
+-rw-r--r--   0        0        0      252 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/__init__.py
+-rw-r--r--   0        0        0    20124 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/base.py
+-rw-r--r--   0        0        0     2044 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/epl.py
+-rw-r--r--   0        0        0     2079 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/mlb.py
+-rw-r--r--   0        0        0     1949 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/nba.py
+-rw-r--r--   0        0        0     2276 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/nfl.py
+-rw-r--r--   0        0        0     1352 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/nhl.py
+-rw-r--r--   0        0        0       51 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/sports/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/__init__.py
+-rw-r--r--   0        0        0   531535 2024-04-23 02:09:58.030221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/MLB/players.csv
+-rw-r--r--   0        0        0     5204 2024-04-23 02:09:58.030221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/MLB/teams.csv
+-rw-r--r--   0        0        0   144790 2024-04-23 02:09:58.030221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NBA/players.csv
+-rw-r--r--   0        0        0     3101 2024-04-23 02:09:58.030221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NBA/teams.csv
+-rw-r--r--   0        0        0   774056 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NFL/players.csv
+-rw-r--r--   0        0        0     8878 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NFL/teams.csv
+-rw-r--r--   0        0        0   293594 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NHL/players.csv
+-rw-r--r--   0        0        0     3313 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NHL/teams.csv
+-rw-r--r--   0        0        0    12392 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/wrangler.py
+-rw-r--r--   0        0        0        0 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/utils/__init__.py
+-rw-r--r--   0        0        0      250 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/utils/enums.py
+-rw-r--r--   0        0        0      142 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/utils/helpers.py
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 sportswrangler-0.1.0/PKG-INFO
```

