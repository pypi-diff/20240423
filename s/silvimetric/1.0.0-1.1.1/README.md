# Comparing `tmp/silvimetric-1.0.0.tar.gz` & `tmp/silvimetric-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silvimetric-1.0.0.tar", last modified: Tue Feb  6 14:44:27 2024, max compression
+gzip compressed data, was "silvimetric-1.1.1.tar", last modified: Tue Apr 23 19:22:39 2024, max compression
```

## Comparing `silvimetric-1.0.0.tar` & `silvimetric-1.1.1.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:44:27.006785 silvimetric-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-06 14:44:10.000000 silvimetric-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-06 14:44:27.002784 silvimetric-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-02-06 14:44:10.000000 silvimetric-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-02-06 14:44:10.000000 silvimetric-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 14:44:27.006785 silvimetric-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:44:26.998784 silvimetric-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:44:26.998784 silvimetric-1.0.0/src/silvimetric/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:44:26.998784 silvimetric-1.0.0/src/silvimetric/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/cli/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:44:27.002784 silvimetric-1.0.0/src/silvimetric/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/commands/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/commands/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/commands/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/commands/shatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:44:27.002784 silvimetric-1.0.0/src/silvimetric/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/resources/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/resources/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/resources/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/resources/extents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/resources/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/resources/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/resources/names.py
--rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-02-06 14:44:10.000000 silvimetric-1.0.0/src/silvimetric/resources/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:44:27.002784 silvimetric-1.0.0/src/silvimetric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-06 14:44:26.000000 silvimetric-1.0.0/src/silvimetric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-02-06 14:44:26.000000 silvimetric-1.0.0/src/silvimetric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 14:44:26.000000 silvimetric-1.0.0/src/silvimetric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-06 14:44:26.000000 silvimetric-1.0.0/src/silvimetric.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-06 14:44:26.000000 silvimetric-1.0.0/src/silvimetric.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 14:44:27.002784 silvimetric-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-02-06 14:44:10.000000 silvimetric-1.0.0/tests/test_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-02-06 14:44:10.000000 silvimetric-1.0.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-06 14:44:10.000000 silvimetric-1.0.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-02-06 14:44:10.000000 silvimetric-1.0.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-02-06 14:44:10.000000 silvimetric-1.0.0/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-02-06 14:44:10.000000 silvimetric-1.0.0/tests/test_shatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-02-06 14:44:10.000000 silvimetric-1.0.0/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-06 14:44:10.000000 silvimetric-1.0.0/tests/test_western.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.104859 silvimetric-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-23 19:22:24.000000 silvimetric-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-23 19:22:39.104859 silvimetric-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-23 19:22:24.000000 silvimetric-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-23 19:22:24.000000 silvimetric-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:22:39.104859 silvimetric-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.096859 silvimetric-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.100859 silvimetric-1.1.1/src/silvimetric/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.100859 silvimetric-1.1.1/src/silvimetric/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10000 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/cli/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.100859 silvimetric-1.1.1/src/silvimetric/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/commands/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/commands/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/commands/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/commands/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/commands/shatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.104859 silvimetric-1.1.1/src/silvimetric/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/extents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-04-23 19:22:24.000000 silvimetric-1.1.1/src/silvimetric/resources/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.104859 silvimetric-1.1.1/src/silvimetric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-23 19:22:39.000000 silvimetric-1.1.1/src/silvimetric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-23 19:22:39.000000 silvimetric-1.1.1/src/silvimetric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:22:39.000000 silvimetric-1.1.1/src/silvimetric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 19:22:39.000000 silvimetric-1.1.1/src/silvimetric.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 19:22:39.000000 silvimetric-1.1.1/src/silvimetric.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:22:39.104859 silvimetric-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_shatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-23 19:22:24.000000 silvimetric-1.1.1/tests/test_western.py
```

### Comparing `silvimetric-1.0.0/LICENSE.txt` & `silvimetric-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `silvimetric-1.0.0/pyproject.toml` & `silvimetric-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silvimetric-1.0.0/src/silvimetric/cli/cli.py` & `silvimetric-1.1.1/src/silvimetric/cli/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,111 @@
 import click
 from dask.distributed import performance_report
 import pyproj
 import logging
 
 
-from ..resources import Bounds, Log
-from ..resources import Attribute, Metric
+from .. import __version__
+from ..resources import Attribute, Metric, Bounds, Log
 from ..resources import StorageConfig, ShatterConfig, ExtractConfig, ApplicationConfig
-from ..commands import shatter, extract, scan, info, initialize
+from ..commands import shatter, extract, scan, info, initialize, manage
 from .common import BoundsParamType, CRSParamType, AttrParamType, MetricParamType
-from .common import dask_handle
+from .common import dask_handle, close_dask
 
 @click.group()
 @click.option("--database", '-d', type=click.Path(exists=False), help="Database path")
-@click.option("--debug", is_flag=True, default=False, help="Print debug messages?")
-@click.option("--log-level", default="INFO", help="Log level (INFO/DEBUG)")
+@click.option("--debug", is_flag=True, default=False, help="Changes logging level from INFO to DEBUG.")
 @click.option("--log-dir", default=None, help="Directory for log output", type=str)
-@click.option("--progress", default=True, type=bool, help="Report progress")
+@click.option("--progress", is_flag=True, default=True, type=bool, help="Report progress")
 @click.option("--workers", type=int, default=12, help="Number of workers for Dask")
 @click.option("--threads", type=int, default=4, help="Number of threads per worker for Dask")
 @click.option("--watch", is_flag=True, default=False, type=bool,
         help="Open dask diagnostic page in default web browser.")
 @click.option("--dasktype", default='processes', type=click.Choice(['threads',
         'processes']), help="What Dask uses for parallelization. For more"
         "information see here https://docs.dask.org/en/stable/scheduling.html#local-threads")
 @click.option("--scheduler", default='distributed', type=click.Choice(['distributed',
         'local', 'single-threaded']), help="Type of dask scheduler. Both are "
         "local, but are run with different dask libraries. See more here "
         "https://docs.dask.org/en/stable/scheduling.html.")
+@click.version_option(__version__)
 @click.pass_context
-def cli(ctx, database, debug, log_level, log_dir, progress, dasktype, scheduler,
+def cli(ctx, database, debug, log_dir, progress, dasktype, scheduler,
         workers, threads, watch):
 
     # Set up logging
+    if debug:
+        log_level = 'DEBUG'
+    else:
+        log_level = 'INFO'
+
     numeric_level = getattr(logging, log_level.upper(), None)
     if not isinstance(numeric_level, int):
         raise ValueError(f"Invalid log level: {log_level}")
 
     log = Log(log_level, log_dir)
     app = ApplicationConfig(tdb_dir=database,
             log=log,
             debug=debug,
             progress=progress,
-            scheduler=scheduler)
-    dask_handle(dasktype, scheduler, workers, threads, watch, app.log)
+            scheduler=scheduler,
+            dasktype=dasktype,
+            workers=workers,
+            threads=threads,
+            watch=watch)
     ctx.obj = app
+    ctx.call_on_close(close_dask)
 
 
 @cli.command("info")
 @click.option("--bounds", type=BoundsParamType(), default=None,
         help="Bounds to filter by")
 @click.option("--date", type=click.DateTime(['%Y-%m-%d','%Y-%m-%dT%H:%M:%SZ']),
         help="Select processes with this date")
+@click.option("--history", type=bool, is_flag=True, default=False,
+        help="Show the history section of the output.")
+@click.option("--metadata", type=bool, is_flag=True, default=False,
+        help="Show the metadata section of the output.")
+@click.option("--attributes", type=bool, is_flag=True, default=False,
+        help="Show the attributes section of the output.")
 @click.option("--dates", type=click.Tuple([
         click.DateTime(['%Y-%m-%d','%Y-%m-%dT%H:%M:%SZ']),
         click.DateTime(['%Y-%m-%d','%Y-%m-%dT%H:%M:%SZ'])]), nargs=2,
         help="Select processes within this date range")
 @click.option("--name", type=str, default=None,
         help="Select processes with this name")
 @click.pass_obj
-def info_cmd(app, bounds, date, dates, name):
+def info_cmd(app, bounds, date, dates, name, history, metadata, attributes):
     import json
     if date is not None and dates is not None:
-        app.log.warning("Both 'date' and 'dates' specified. Prioritizing 'dates'")
+        app.log.warning("Both 'date' and 'dates' specified. Prioritizing"
+            "'dates'")
 
     start_date = dates[0] if dates else date
     end_date = dates[1] if dates else date
 
     i = info.info(app.tdb_dir, bounds=bounds, start_time=start_date,
         end_time=end_date, name=name)
-    app.log.info(json.dumps(i, indent=2))
+
+    if any([history, metadata, attributes]):
+        filtered = { }
+        if history:
+            filtered['history'] = i['history']
+        if metadata:
+            filtered['metadata'] = i['metadata']
+        if attributes:
+            filtered['attributes'] = i['attributes']
+
+        app.log.info(json.dumps(filtered, indent=2))
+
+    else:
+        app.log.info(json.dumps(i, indent=2))
+        return
+
+
 
 
 @cli.command("scan")
 @click.argument("pointcloud", type=str)
 @click.option("--resolution", type=float, default=100,
         help="Summary pixel resolution")
 @click.option("--filter", is_flag=True, type=bool, default=False,
@@ -82,17 +114,20 @@
         help="Point count threshold.")
 @click.option("--depth", type=int, default=6,
         help="Quadtree depth threshold.")
 @click.option("--bounds", type=BoundsParamType(), default=None,
         help="Bounds to scan.")
 @click.pass_obj
 def scan_cmd(app, resolution, point_count, pointcloud, bounds, depth, filter):
-    """Scan point cloud and determine the optimal tile size."""
+    """Scan point cloud, output information on it, and determine the optimal
+    tile size."""
+    dask_handle(app.dasktype, app.scheduler, app.workers, app.threads,
+            app.watch, app.log)
     return scan.scan(app.tdb_dir, pointcloud, bounds, point_count, resolution,
-            depth, filter)
+            depth, filter, log=app.log)
 
 
 @cli.command('initialize')
 @click.option("--bounds", type=BoundsParamType(), required=True,
         help="Root bounds that encapsulates all data")
 @click.option("--crs", type=CRSParamType(), required=True,
         help="Coordinate system of data")
@@ -102,16 +137,16 @@
         help="List of metrics to include in Database")
 @click.option("--resolution", type=float, default=30.0,
         help="Summary pixel resolution")
 @click.pass_obj
 def initialize_cmd(app: ApplicationConfig, bounds: Bounds, crs: pyproj.CRS,
         attributes: list[Attribute], resolution: float, metrics: list[Metric]):
     import itertools
-    """Initialize silvimetrics DATABASE
-    """
+    """Initialize silvimetrics DATABASE"""
+
     storageconfig = StorageConfig(tdb_dir = app.tdb_dir,
             log = app.log,
             root = bounds,
             crs = crs,
             attrs = attributes,
             metrics = list(itertools.chain(*metrics)),
             resolution = resolution)
@@ -130,22 +165,25 @@
         help="Date the data was produced.")
 @click.option("--dates", type=click.Tuple([
         click.DateTime(['%Y-%m-%d','%Y-%m-%dT%H:%M:%SZ']),
         click.DateTime(['%Y-%m-%d','%Y-%m-%dT%H:%M:%SZ'])]), nargs=2,
         help="Date range the data was produced during")
 @click.pass_obj
 def shatter_cmd(app, pointcloud, bounds, report, tilesize, date, dates):
+    """Insert data provided by POINTCLOUD into the silvimetric DATABASE"""
+
+    dask_handle(app.dasktype, app.scheduler, app.workers, app.threads,
+            app.watch, app.log)
 
     if date is not None and dates is not None:
         app.log.warning("Both 'date' and 'dates' specified. Prioritizing 'dates'")
 
     if date is None and dates is None:
         raise ValueError("One of '--date' or '--dates' must be provided.")
 
-    """Insert data provided by POINTCLOUD into the silvimetric DATABASE"""
     config = ShatterConfig(tdb_dir = app.tdb_dir,
             date=dates if dates else tuple([date]),
             log = app.log,
             filename = pointcloud,
             bounds = bounds,
             tile_size=tilesize)
 
@@ -158,17 +196,17 @@
             shatter.shatter(config)
         print(f'Writing report to {report_path}.')
     else:
         shatter.shatter(config)
 
 
 @cli.command('extract')
-@click.option("--attributes", "-a", multiple=True, type=AttrParamType(),
+@click.option("--attributes", "-a", multiple=True, type=AttrParamType(), default=[],
         help="List of attributes to include output")
-@click.option("--metrics", "-m", multiple=True, type=MetricParamType(),
+@click.option("--metrics", "-m", multiple=True, type=MetricParamType(), default=[],
         help="List of metrics to include in output")
 @click.option("--bounds", type=BoundsParamType(), default=None,
         help="Bounds for data to include in output")
 @click.option("--outdir", "-o", type=click.Path(exists=False), required=True,
         help="Output directory.")
 @click.pass_obj
 def extract_cmd(app, attributes, metrics, outdir, bounds):
@@ -181,10 +219,30 @@
             log = app.log,
             out_dir= outdir,
             attrs = attributes,
             metrics = metrics,
             bounds = bounds)
     extract.extract(config)
 
+@cli.command('delete')
+@click.option('--id', type=click.UUID, required=True,
+    help="Shatter Task UUID.")
+@click.pass_obj
+def delete_cmd(app, id):
+    manage.delete(app.tdb_dir, id)
+
+@cli.command('restart')
+@click.option('--id', type=click.UUID, required=True,
+    help="Shatter Task UUID.")
+@click.pass_obj
+def restart_cmd(app, id):
+    manage.restart(tdb_dir=app.tdb_dir, name=id)
+
+@cli.command('resume')
+@click.option('--id', type=click.UUID, required=True,
+    help="Shatter Task UUID.")
+@click.pass_obj
+def resume_cmd(app, id):
+    manage.resume(tdb_dir=app.tdb_dir, name=id)
 
 if __name__ == "__main__":
-    cli()
+    cli()
```

### Comparing `silvimetric-1.0.0/src/silvimetric/cli/common.py` & `silvimetric-1.1.1/src/silvimetric/cli/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,18 +29,23 @@
         except Exception as e:
             self.fail(f"{value!r} is not a CRS type with error {e}", param, ctx)
 
 class AttrParamType(click.ParamType):
     name="Attrs"
     #TODO add import similar to metrics
     def convert(self, value, param, ctx) -> list[Attribute]:
-        try:
-            return [Attributes[a] for a in value]
-        except Exception as e:
-            self.fail(f"{value!r} is not available in Attributes, {e}", param, ctx)
+        if isinstance(value, list):
+            try:
+                return [Attributes[a] for a in value]
+            except Exception as e:
+                self.fail(f"{value!r} is not available in Attributes, {e}", param, ctx)
+        elif isinstance(value, str):
+            return Attributes[value]
+        else:
+            self.fail(f"{value!r} is of an invalid type, {e}", param, ctx)
 
 class MetricParamType(click.ParamType):
     name="Metrics"
     def convert(self, value, param, ctx) -> list[Metric]:
         if '.py' in value:
             try:
                 import importlib.util
@@ -63,15 +68,15 @@
 
             for m in ms:
                 if not isinstance(m, Metric):
                     self.fail(f"Invalid Metric supplied: {m}")
             return user_metrics.metrics()
 
         try:
-            return [ Metrics[value] ]
+            return Metrics[value]
         except Exception as e:
             self.fail(f"{value!r} is not available in Metrics, {e}", param, ctx)
 
 def dask_handle(dasktype: str, scheduler: str, workers: int, threads: int,
         watch: bool, log: Log):
     dask_config = { }
 
@@ -104,13 +109,15 @@
         client = Client(cluster)
         client.get_versions(check=True)
         dask_config['distributed.client'] = client
         if watch:
             webbrowser.open(client.cluster.dashboard_link)
 
     elif scheduler == 'single-threaded':
-        if scheduler != 'distributed':
-            log.warning("""Selected scheduler type does not support continuously\
-                            updated config information.""")
         dask_config['scheduler'] = scheduler
 
     dask.config.set(dask_config)
+
+def close_dask():
+    client = dask.config.get('distributed.client')
+    if isinstance(client, Client):
+        client.close()
```

### Comparing `silvimetric-1.0.0/src/silvimetric/commands/extract.py` & `silvimetric-1.1.1/src/silvimetric/commands/extract.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from osgeo import gdal, osr
 import numpy as np
 from pathlib import Path
 import pandas as pd
 import dask
 import dask.dataframe as dd
-import dask.bag as db
+
+from typing import Dict
 
 from ..resources import Storage, ExtractConfig, Metric, Attribute
 from ..resources import Extents
 
 np_to_gdal_types = {
     np.dtype(np.byte).str: gdal.GDT_Byte,
     np.dtype(np.int8).str: gdal.GDT_Int16,
@@ -19,15 +20,24 @@
     np.dtype(np.uint64).str: gdal.GDT_UInt64,
     np.dtype(np.int64).str: gdal.GDT_Int64,
     np.dtype(np.float32).str: gdal.GDT_Float32,
     np.dtype(np.float64).str: gdal.GDT_Float64
 }
 
 def write_tif(xsize: int, ysize: int, data:np.ndarray, name: str,
-              config: ExtractConfig):
+              config: ExtractConfig) -> None:
+    """
+    Write out a raster with GDAL
+
+    :param xsize: Length of X plane.
+    :param ysize: Length of Y plane.
+    :param data: Data to write to raster.
+    :param name: Name of raster to write.
+    :param config: ExtractConfig.
+    """
     osr.UseExceptions()
     path = Path(config.out_dir) / f'{name}.tif'
     crs = config.crs
     srs = osr.SpatialReference()
     srs.ImportFromWkt(crs.to_wkt())
     # transform = [x, res, 0, y, 0, res]
     b = config.bounds
@@ -41,15 +51,23 @@
     tif.SetGeoTransform(transform)
     tif.SetProjection(srs.ExportToWkt())
     tif.GetRasterBand(1).WriteArray(data)
     tif.GetRasterBand(1).SetNoDataValue(np.nan)
     tif.FlushCache()
     tif = None
 
-def get_metrics(data_in, config: ExtractConfig):
+MetricDict = Dict[str, np.ndarray]
+def get_metrics(data_in: MetricDict, config: ExtractConfig) -> MetricDict:
+    """
+    Reruns a metric over this cell. Only called if there is overlapping data.
+
+    :param data_in: Cell data to be rerun.
+    :param config: ExtractConfig.
+    :return: Combined dict of attribute and newly derived metric data.
+    """
     if data_in is None:
         return None
 
     # make sure it's not empty. No empty writes
     if not np.any(data_in['count']):
         return None
 
@@ -61,15 +79,26 @@
         f'{m.entry_name(attr.name)}': [m(cell_data) for cell_data in data_in[attr.name]]
         for attr in config.attrs for m in config.metrics
     }
     # md = dask.compute(metric_data)[0]
     data_out = data_in | metric_data
     return data_out
 
-def handle_overlaps(config: ExtractConfig, storage: Storage, indices: np.ndarray):
+def handle_overlaps(config: ExtractConfig, storage: Storage, indices: np.ndarray) -> pd.DataFrame:
+    """
+    Handle cells that have overlapping data. We have to re-run metrics over these
+    cells as there's no other accurate way to determined metric values. If there
+    are no overlaps, this will do nothing.
+
+    :param config: ExtractConfig.
+    :param storage: Database storage object.
+    :param indices: Indices with overlap.
+    :return: Dataframe of rerun data.
+    """
+
     ma_list = [ m.entry_name(a.name) for m in config.metrics for a in
         config.attrs ]
     att_list = [ a.name for a in config.attrs ] + [ 'count' ]
     out_list = [ *ma_list, 'X', 'Y' ]
 
     minx = indices['x'].min()
     maxx = indices['x'].max()
@@ -128,15 +157,20 @@
         rs = recs.compute().to_dict(orient='list')
 
         # 3. Should rerun the metrics over them
         metrics = get_metrics(rs, config)
         ms = pd.DataFrame.from_dict(metrics)[out_list]
         return pd.concat((ms, leaves[out_list]))
 
-def extract(config: ExtractConfig):
+def extract(config: ExtractConfig) -> None:
+    """
+    Pull data from database for each desired metric and output them to rasters
+
+    :param config: ExtractConfig.
+    """
 
     dask.config.set({"dataframe.convert-string": False})
 
     ma_list = [ m.entry_name(a.name) for m in config.metrics for a in
         config.attrs ]
```

### Comparing `silvimetric-1.0.0/src/silvimetric/resources/data.py` & `silvimetric-1.1.1/src/silvimetric/resources/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,42 +4,56 @@
 
 import pdal
 
 import pathlib
 import json
 
 class Data:
+    """Represents a point cloud or PDAL pipeline, and performs essential operations
+    necessary to understand and execute a Shatter process."""
 
     def __init__(self,
                  filename: str,
                  storageconfig: StorageConfig,
                  bounds: Bounds = None):
         self.filename = filename
+        """Path to either PDAL pipeline or point cloud file"""
         self.bounds = bounds
+        """Bounds of this section of data"""
 
         self.reader_thread_count = 2
+        """Thread count for PDAL reader. Keep to 2 so we don't hog threads"""
 
         self.storageconfig = storageconfig
+        """:class:`silvimetric.resources.StorageConfig`"""
         self.reader = self.get_reader()
+        """PDAL reader"""
         self.pipeline = self.get_pipeline()
+        """PDAL pipeline"""
         if self.bounds is None:
             self.bounds = Data.get_bounds(self.reader)
 
 
     def is_pipeline(self) -> bool:
-        """Does this instance represent a pdal.Pipeline or a simple filename"""
+        """Does this instance represent a pdal.Pipeline or a simple filename
+
+        :return: Return true if input is a pipeline
+        """
 
         p = pathlib.Path(self.filename)
         if p.suffix == '.json' and p.name != 'ept.json':
             return True
         return False
 
 
     def make_pipeline(self) -> pdal.Pipeline:
-        """Take a COPC or EPT endpoint and generate a PDAL pipeline for it"""
+        """Take a COPC or EPT endpoint and generate a PDAL pipeline for it
+
+        :return: Return PDAL pipeline
+        """
 
         reader = pdal.Reader(self.filename, tag='reader')
         reader._options['threads'] = self.reader_thread_count
         if self.bounds:
             reader._options['bounds'] = str(self.bounds)
         class_zero = pdal.Filter.assign(value="Classification = 0")
         rn = pdal.Filter.assign(value="ReturnNumber = 1 WHERE ReturnNumber < 1")
@@ -49,16 +63,21 @@
         # assign_x = pdal.Filter.assign(
         #     value=f"xi = (X - {self.root.minx}) / {resolution}")
         # assign_y = pdal.Filter.assign(
         #     value=f"yi = ({self.root.maxy} - Y) / {resolution}")
 
         return reader | class_zero | rn | nor #| ferry | assign_x | assign_y #| smrf | hag
 
-    def get_pipeline(self):
-        """Fetch the pipeline for the instance"""
+    def get_pipeline(self) -> pdal.Pipeline:
+        """Fetch the pipeline for the instance
+
+        :raises Exception: File type isn't COPC or EPT
+        :raises Exception: More than one reader detected
+        :return: Return PDAL pipline
+        """
 
         # If we are a pipeline, read and parse it. If we
         # aren't, go make_pipeline using some options that
         # process the data
         if self.is_pipeline():
             p = pathlib.Path(self.filename)
             j = p.read_bytes().decode('utf-8')
@@ -105,29 +124,39 @@
         stages.append(assign_x)
         stages.append(assign_y)
 
         # return our pipeline
         return pdal.Pipeline(stages)
 
     def execute(self):
+        """Execute PDAL pipeline
+
+        :raises Exception: PDAL error message passed from execution
+        """
         try:
             self.pipeline.execute()
             # self.storageconfig.log.debug(f"PDAL log: {self.pipeline.log}")
         except Exception as e:
             print(self.pipeline.pipeline, e)
             raise e
 
     def get_array(self) -> np.ndarray:
-        """Fetch the array from the execute()'d pipeline"""
+        """Fetch the array from the execute()'d pipeline
+
+        :return: get data as a numpy ndarray
+        """
         return self.pipeline.arrays[0]
     array = property(get_array)
 
     def get_reader(self) -> pdal.Reader:
-        """Grab or make the reader for this instance so we can use it to do things like
-        get the count()"""
+        """Grab or make the reader for this instance so we can use it to do things
+        like get the count()
+
+        :return: get PDAL reader for input
+        """
         if self.is_pipeline():
             p = pathlib.Path(self.filename)
             j = p.read_bytes().decode('utf-8')
             stages = pdal.pipeline._parse_stages(j)
             pipeline = pdal.Pipeline(stages)
             for stage in pipeline.stages:
                 stage_type, stage_kind = stage.type.split('.')
@@ -136,30 +165,47 @@
         else:
             reader = pdal.Reader(self.filename)
             reader._options['threads'] = self.reader_thread_count
             return reader
 
     @staticmethod
     def get_bounds(reader: pdal.Reader) -> Bounds:
+        """Get the bounding box of a point cloud from PDAL.
+
+        :param reader: PDAL Reader representing input data
+        :return: bounding box of point cloud
+        """
         p = reader.pipeline()
         qi = p.quickinfo[reader.type]
         return Bounds.from_string(json.dumps(qi['bounds']))
 
     def estimate_count(self, bounds: Bounds) -> int:
-        """For the provided bounds, estimate the maximum number of points that could be inside them for this instance."""
+        """For the provided bounds, estimate the maximum number of points that
+        could be inside them for this instance.
+
+        :param bounds: query bounding box
+        :return: estimated point count
+        """
+
         reader = self.get_reader()
         if bounds:
             reader._options['bounds'] = str(bounds)
         pipeline = reader.pipeline()
         qi = pipeline.quickinfo[reader.type]
         pc = qi['num_points']
 
         return pc
 
     def count(self, bounds: Bounds) -> int:
-        """For the provided bounds, read and count the number of points that are inside them for this instance."""
+        """For the provided bounds, read and count the number of points that are
+        inside them for this instance.
+
+        :param bounds: query bounding box
+        :return: point count
+        """
+
         reader = self.get_reader()
         if bounds:
             reader._options['bounds'] = str(bounds)
         pipeline = reader.pipeline()
         pipeline.execute()
         return len(pipeline.arrays[0])
```

### Comparing `silvimetric-1.0.0/src/silvimetric/resources/log.py` & `silvimetric-1.1.1/src/silvimetric/resources/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 Project: CRREL-NEGGS University of Houston Collaboration
 Date: February 2021
 
 A module for setting up logging.
 """
 import logging
 import pathlib
-import os
+import sys
+
 from typing import Any
 from typing import Dict
-from typing import TYPE_CHECKING
 
 try:
     import websocket
     from pythonjsonlogger import jsonlogger
 except ImportError:
     WebSocketHandler = None
     pass
@@ -58,30 +58,33 @@
                  log_level: int,
                  logdir: str = None,
                  logtype: str = "stream",
                  logfilename: str = "silvimetric-log.txt"):
         """
         Creates logging formatting and structure
 
-        Parameters
-        ----------
-        config:
-            Application config representing the runtime config
+        :param config: Application config representing the runtime config
         """
 
+        # need to be careful not to pull logging from previous runs
         self.logger = logging.getLogger("silvimetric")
-        self.logger.setLevel(log_level)
-        self.log_level = log_level
         self.logdir = logdir
         if logdir:
             self.logtype = 'file'
         else:
             self.logtype = logtype
         self.logfilename = logfilename
 
+        # do not recreate handlers if they're already present
+        if self.logger.handlers:
+            self.log_level = self.logger.level
+            return
+
+        self.log_level = log_level
+        self.logger.setLevel(log_level)
 
         # File Handler for Logging
         log_format = logging.Formatter(
             "%(asctime)s - %(name)s - %(levelname)s - %(funcName)s:%(lineno)d - %(message)s"
         )
 
         # We only use a file handler if user specified a logdir
@@ -117,15 +120,15 @@
             except ConnectionRefusedError as err:
                 raise ConnectionRefusedError(f"Connection Refused to {url}")
             log_handler = WebSocketHandler("DEBUG", websocket=self.relay)
             log_handler.setFormatter(formatter)
         else:
             # if the user didn't specify a log dir, we just do the StreamHandler
             if not self.logdir:
-                log_handler = logging.StreamHandler()
+                log_handler = logging.StreamHandler(stream=sys.stdout)
                 log_handler.setFormatter(log_format)
                 self.logger.addHandler(log_handler)
 
     def to_json(self):
         return {'logdir': self.logdir,
                 'log_level': self.log_level,
                 'logtype': self.logtype ,
```

### Comparing `silvimetric-1.0.0/src/silvimetric/resources/metric.py` & `silvimetric-1.1.1/src/silvimetric/resources/metric.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,27 +13,43 @@
 
 MetricFn = Callable[[np.ndarray, Optional[Union[Any, None]]], np.ndarray]
 
 # Derived information about a cell of points
 
 ## TODO should create list of metrics as classes that derive from Metric?
 class Metric(Entry):
-    def __init__(self, name: str, dtype: np.dtype, method: MetricFn, deps: list[Attribute]=None):
+    """
+    A Metric is an Entry representing derived cell data. There is a base set of
+    metrics available through Silvimetric, or you can create your own. A Metric
+    object has all the information necessary to facilitate the derivation of
+    data as well as its insertion into the database.
+    """
+    def __init__(self, name: str, dtype: np.dtype, method: MetricFn, dependencies: list[Attribute]=None):
         super().__init__()
         self.name = name
+        """Metric name. eg. mean"""
         self.dtype = dtype
-        self.dependencies = deps
+        """Numpy data type."""
+        self.dependencies = dependencies
+        """Attributes/Metrics this is dependent on."""
         self._method = method
+        """The method that processes this data."""
 
     def schema(self, attr: Attribute):
+        """
+        Create schema for TileDB creation.
+
+        :param attr: :class:`silvimetric.resources.entry.Atttribute`
+        :return: TileDB Attribute
+        """
         entry_name = self.entry_name(attr.name)
         return Attr(name=entry_name, dtype=self.dtype)
 
-    # common name, storage name
     def entry_name(self, attr: str) -> str:
+        """Name for use in TileDB and extract file generation."""
         return f'm_{attr}_{self.name}'
 
     @dask.delayed
     def delayed(self, data: np.ndarray) -> np.ndarray:
         return self._method(data)
 
     def to_json(self) -> dict[str, any]:
```

### Comparing `silvimetric-1.0.0/src/silvimetric/resources/names.py` & `silvimetric-1.1.1/src/silvimetric/resources/names.py`

 * *Files identical despite different names*

### Comparing `silvimetric-1.0.0/src/silvimetric.egg-info/SOURCES.txt` & `silvimetric-1.1.1/src/silvimetric.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 src/silvimetric/cli/__init__.py
 src/silvimetric/cli/cli.py
 src/silvimetric/cli/common.py
 src/silvimetric/commands/__init__.py
 src/silvimetric/commands/extract.py
 src/silvimetric/commands/info.py
 src/silvimetric/commands/initialize.py
+src/silvimetric/commands/manage.py
 src/silvimetric/commands/scan.py
 src/silvimetric/commands/shatter.py
 src/silvimetric/resources/__init__.py
 src/silvimetric/resources/bounds.py
 src/silvimetric/resources/config.py
 src/silvimetric/resources/data.py
 src/silvimetric/resources/entry.py
 src/silvimetric/resources/extents.py
 src/silvimetric/resources/log.py
 src/silvimetric/resources/metric.py
 src/silvimetric/resources/names.py
 src/silvimetric/resources/storage.py
 tests/test_chunk.py
+tests/test_cli.py
 tests/test_commands.py
 tests/test_configuration.py
 tests/test_data.py
 tests/test_extract.py
 tests/test_shatter.py
 tests/test_storage.py
 tests/test_western.py
```

### Comparing `silvimetric-1.0.0/tests/test_chunk.py` & `silvimetric-1.1.1/tests/test_chunk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 import numpy as np
-import dask
-import pdal
-import pytest
 import datetime
 
 from silvimetric.resources import Extents
 from silvimetric.commands.shatter import run
 
 def check_for_holes(leaves: list[Extents], chunk: Extents):
     ind = np.array([], dtype=chunk.get_indices().dtype)
@@ -79,22 +76,14 @@
     dup = u[c > 1]
     b = np.any([dup['x'], dup['y']])
 
     assert b == False, f"Indices duplicated: {dup}"
 
 
 class TestExtents(object):
-    @pytest.fixture(scope='function', autouse=True)
-    def filtered(self, copc_data, extents: Extents):
-        return list(extents.chunk(copc_data, 1))
-
-    @pytest.fixture(scope='function')
-    def unfiltered(self, extents: Extents):
-        return list(extents.get_leaf_children(30))
-
     def test_indexing(self, extents, filtered, unfiltered):
         check_indexing(extents, filtered)
         check_for_holes(filtered, extents)
         check_indexing(extents, unfiltered)
         check_for_holes(unfiltered, extents)
 
     # def test_cells(self, copc_filepath, unfiltered, resolution):
@@ -118,16 +107,16 @@
     #             bad_chunks.append(leaf)
     #     assert flag == False, f"{[str(leaf) for leaf in bad_chunks]} are bad chunks"
 
     def test_pointcount(self, filtered, unfiltered, test_point_count, shatter_config, storage):
 
         with storage.open('w') as tdb:
             shatter_config.start_time = datetime.datetime.now().timestamp() * 1000
-            fc = run(filtered, shatter_config, storage, tdb)
-            ufc = run(unfiltered, shatter_config, storage, tdb)
+            fc = run(filtered, shatter_config, storage)
+            ufc = run(unfiltered, shatter_config, storage)
 
             assert fc == ufc, f"""
                 Filtered and unfiltered point counts don't match.
                 Filtered: {fc}, Unfiltered: {ufc}"""
             assert test_point_count == fc, f"""
                 Filtered point counts don't match.
                 Expected {test_point_count}, got {fc}"""
```

### Comparing `silvimetric-1.0.0/tests/test_commands.py` & `silvimetric-1.1.1/tests/test_commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,11 @@
-import uuid
-from time import sleep
-from typing import List
-from datetime import datetime
-
-from silvimetric.commands import scan, info, shatter
-from silvimetric.resources import ShatterConfig
-
-import pytest
-import conftest
-
-@pytest.fixture(scope='function')
-def config_split(shatter_config: ShatterConfig) -> List[ShatterConfig]:
-    sc = shatter_config
-    config_split = []
-    day = 1
-    for b in sc.bounds.bisect():
-        day += 1
-        date = datetime(2011, 1, day)
-
-        config_split.append(ShatterConfig(
-            sc.filename,
-            date,
-            sc.attrs,
-            sc.metrics,
-            b,
-            uuid.uuid4(),
-            sc.tile_size,
-            tdb_dir=sc.tdb_dir,
-            log=sc.log
-        ))
-
-    for s in config_split:
-        shatter.shatter(s)
-    sleep(1)
-
-    return config_split
+import json
 
+from silvimetric.commands import scan, info, shatter, manage
+from silvimetric.resources import ShatterConfig, Storage
 
 class TestCommands(object):
 
     def test_scan(self, shatter_config):
         s = shatter_config
         res = scan.scan(s.tdb_dir, s.filename, s.bounds, 10, 10, 5)
         assert res == 1
@@ -63,8 +29,51 @@
         i = info.info(tdb_filepath, name=str(config_split[0].name))
         assert len(i['history']) == 1
         assert i['history'][0] == config_split[0].to_json()
 
         d = config_split[1].date
         i = info.info(tdb_filepath, start_time=d, end_time=d)
         assert len(i['history']) == 1
-        assert i['history'][0] == config_split[1].to_json()
+        assert i['history'][0] == config_split[1].to_json()
+
+    def test_delete(self, tdb_filepath, config_split):
+        ids = [c.name for c in config_split]
+
+        for i in range(1,len(ids)+1):
+            h = info.info(tdb_dir=tdb_filepath)
+
+            assert bool(h['history'])
+            assert len(h['history']) == 5-i
+            idx = i - 1
+            manage.delete(tdb_filepath, ids[idx])
+
+        h = info.info(tdb_dir=tdb_filepath)
+        assert not bool(h['history'])
+
+    def test_restart(self, tdb_filepath, config_split):
+        ids = [c.name for c in config_split]
+
+        for i in range(1,len(ids)+1):
+            h = info.info(tdb_dir=tdb_filepath)
+
+            assert bool(h['history'])
+            assert len(h['history']) == len(ids)
+            manage.restart(tdb_filepath, ids[i-1])
+
+        h = info.info(tdb_dir=tdb_filepath)
+        assert bool(h['history'])
+        assert len(h['history']) == 4
+
+    def test_resume(self, shatter_config: ShatterConfig, test_point_count):
+        # test that shatter only operates on cells not touched by nonempty_domain
+        storage = Storage.from_db(shatter_config.tdb_dir)
+
+        # modify shatter config
+        shatter_config.tile_size=1
+        shatter_config.mbr = (((0,4), (0,4)),)
+        # send to shatter
+        pc = shatter.shatter(shatter_config)
+        assert pc == test_point_count - (test_point_count / 4)
+        # check output config to see what the nonempthy_domain is
+        #   - should be only only values outside of that tuple
+        m = json.loads(storage.getMetadata('shatter', 1))
+        assert len(m['mbr']) == 75
```

### Comparing `silvimetric-1.0.0/tests/test_shatter.py` & `silvimetric-1.1.1/tests/test_shatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os
 import pytest
 import numpy as np
 import dask
 import json
 import uuid
-import platform
-
 
 from silvimetric.commands.shatter import shatter
 from silvimetric.commands.info import info
 from silvimetric.resources import Storage, Extents, ShatterConfig, Log
 
+
 @dask.delayed
 def write(x,y,val, s:Storage, attrs, dims, metrics):
     m_list = [m.entry_name(a.name) for m in metrics for a in attrs]
     data = { a.name: np.array([np.array([val], dims[a.name]), None], object)[:-1]
                 for a in attrs }
 
     for m in m_list:
@@ -34,31 +33,35 @@
             assert y == 10
             assert x == 10
             for xi in range(x):
                 for yi in range(y):
                     a[xi, yi]['Z'].size == 1
                     assert bool(np.all(a[xi, yi]['Z'][0] == ((maxy/storage.config.resolution)-yi)))
 
+        # change attributes to make it a new run
         shatter_config.name = uuid.uuid4()
+        shatter_config.mbr = ()
+        shatter_config.time_slot = 2
+
         shatter(shatter_config)
         with storage.open('r') as a:
             # querying flattens to 20, there will 10 pairs of values
             assert a[:,0]['Z'].shape[0] == 20
             assert a[0,:]['Z'].shape[0] == 20
             # now test that the second set is the same as the first set
             # and test that this value is still the same as the original
             # which was set at ((maxy/resolution)-yindex)
             for xi in range(x):
                 for yi in range(y):
                     a[xi, yi]['Z'].size == 2
                     assert bool(np.all(a[xi, yi]['Z'][1] == a[xi,yi]['Z'][0]))
                     assert bool(np.all(a[xi, yi]['Z'][1] == ((maxy/storage.config.resolution)-yi)))
 
-            m = info(storage.config.tdb_dir)
-            assert len(m['history']) == 2
+        m = info(storage.config.tdb_dir)
+        assert len(m['history']) == 2
 
     def test_parallel(self, storage, attrs, dims, threaded_dask, metrics):
         # test that writing in parallel doesn't affect ordering of values
         # constrained by NumberOfReturns being uint8
 
         count = 255
         tl = [write(0,0,val,storage,attrs,dims, metrics) for val in range(count)]
@@ -71,15 +74,15 @@
                 assert bool(np.all(d['Z'][idx] == d['Intensity'][idx]))
                 assert bool(np.all(d['Intensity'][idx] == d['NumberOfReturns'][idx]))
                 assert bool(np.all(d['NumberOfReturns'][idx] == d['ReturnNumber'][idx]))
 
     def test_config(self, shatter_config, storage, test_point_count):
         shatter(shatter_config)
         try:
-            meta = storage.getMetadata('shatter')
+            meta = storage.getMetadata('shatter', shatter_config.time_slot)
         except BaseException as e:
             pytest.fail("Failed to retrieve 'shatter' metadata key." + e.args)
         meta_j = json.loads(meta)
         pc = meta_j['point_count']
         assert pc == test_point_count
 
     @pytest.mark.parametrize('sh_cfg', ['shatter_config', 'uneven_shatter_config'])
@@ -87,36 +90,40 @@
         s = request.getfixturevalue(sh_cfg)
         storage = Storage.from_db(s.tdb_dir)
         e = Extents.from_storage(s.tdb_dir)
 
         pc = 0
         for b in e.split():
             log = Log(20)
+            time_slot = storage.reserve_time_slot()
             sc = ShatterConfig(tdb_dir = s.tdb_dir,
                                log = log,
                                filename = s.filename,
                                tile_size = s.tile_size,
                                attrs = s.attrs,
                                metrics = s.metrics,
                                debug = s.debug,
                                bounds = b.bounds,
-                               date=s.date)
+                               date=s.date,
+                               time_slot=time_slot)
             pc = pc + shatter(sc)
         history = info(s.tdb_dir)['history']
+        assert len(history) == 4
         assert isinstance(history, list)
         pcs = [ h['point_count'] for h in history ]
         assert sum(pcs) == test_point_count
         assert pc == test_point_count
 
     @pytest.mark.skipif(
         os.environ.get('AWS_SECRET_ACCESS_KEY') is None or
         os.environ.get('AWS_ACCESS_KEY_ID') is None,
         reason='Missing necessary AWS environment variables'
     )
     def test_remote_creation(self, s3_shatter_config, s3_storage):
+        # need processes scheduler to accurately test bug fix
         dask.config.set(scheduler="processes")
         resolution = s3_storage.config.resolution
         maxy = s3_storage.config.root.maxy
         shatter(s3_shatter_config)
         with s3_storage.open('r') as a:
             y = a[:,0]['Z'].shape[0]
             x = a[0,:]['Z'].shape[0]
```

### Comparing `silvimetric-1.0.0/tests/test_storage.py` & `silvimetric-1.1.1/tests/test_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import tiledb
 import numpy as np
 
 from silvimetric.resources import Storage, Metrics, Attribute
+from silvimetric.commands import info
 from silvimetric import __version__ as svversion
 
 class Test_Storage(object):
 
     def test_schema(self, storage: Storage, attrs: list[Attribute]):
         with storage.open('r') as st:
             s:tiledb.ArraySchema = st.schema
             assert s.has_attr('count')
             assert s.attr('count').dtype == np.int32
 
             for a in attrs:
                 assert s.has_attr(a.name)
                 # assert s.attr(a.name) == a.schema()
 
+    def test_time_reserve(self, storage):
+        for x in range(5):
+            time_slot = storage.reserve_time_slot()
+            assert time_slot == x + 1
+
     def test_local(self, storage: Storage, attrs: list[Attribute]):
         with storage.open('r') as st:
             sc = st.schema
             assert sc.has_attr('count')
             assert sc.attr('count').dtype == np.int32
 
             for a in attrs:
```

