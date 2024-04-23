# Comparing `tmp/centralcli-2.4.0.tar.gz` & `tmp/centralcli-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "centralcli-2.4.0.tar", max compression
+gzip compressed data, was "centralcli-3.0.0.tar", max compression
```

## Comparing `centralcli-2.4.0.tar` & `centralcli-3.0.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
--rw-r--r--   0        0        0     1067 2023-08-30 16:01:18.948011 centralcli-2.4.0/LICENSE
--rw-r--r--   0        0        0    12115 2023-08-30 16:01:34.228021 centralcli-2.4.0/README.md
--rw-r--r--   0        0        0     3924 2023-09-01 00:12:28.883691 centralcli-2.4.0/centralcli/__init__.py
--rw-r--r--   0        0        0     1265 2023-09-08 18:43:03.749878 centralcli-2.4.0/centralcli/boilerplate/README.md
--rw-r--r--   0        0        0  1156225 2024-03-22 20:25:45.394496 centralcli-2.4.0/centralcli/boilerplate/allcalls.py
--rw-r--r--   0        0        0    12139 2023-08-30 16:01:18.948011 centralcli-2.4.0/centralcli/caas.py
--rw-r--r--   0        0        0    96513 2024-02-07 15:12:08.963480 centralcli-2.4.0/centralcli/cache.py
--rw-r--r--   0        0        0   207104 2024-04-13 05:23:36.606216 centralcli-2.4.0/centralcli/central.py
--rw-r--r--   0        0        0    49032 2024-04-13 05:13:06.944949 centralcli-2.4.0/centralcli/cleaner.py
--rw-r--r--   0        0        0    44476 2024-04-11 21:23:36.244344 centralcli-2.4.0/centralcli/cli.py
--rw-r--r--   0        0        0    29819 2023-09-09 20:57:36.962267 centralcli-2.4.0/centralcli/cliadd.py
--rw-r--r--   0        0        0     5372 2023-11-04 00:53:25.674537 centralcli-2.4.0/centralcli/cliassign.py
--rw-r--r--   0        0        0    95394 2024-04-11 19:54:41.383365 centralcli-2.4.0/centralcli/clibatch.py
--rw-r--r--   0        0        0    16403 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/clicaas.py
--rw-r--r--   0        0        0     2995 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/cliclone.py
--rw-r--r--   0        0        0    24868 2024-04-13 05:26:13.386524 centralcli-2.4.0/centralcli/clicommon.py
--rw-r--r--   0        0        0    28061 2024-02-07 17:39:25.172142 centralcli-2.4.0/centralcli/clidel.py
--rw-r--r--   0        0        0     4765 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/clikick.py
--rw-r--r--   0        0        0     3251 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/clirefresh.py
--rw-r--r--   0        0        0     5400 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/clirename.py
--rw-r--r--   0        0        0   145124 2024-04-13 05:26:51.046626 centralcli-2.4.0/centralcli/clishow.py
--rw-r--r--   0        0        0     3943 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/clishowbranch.py
--rw-r--r--   0        0        0     7645 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/clishowfirmware.py
--rw-r--r--   0        0        0    12980 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/clishowospf.py
--rw-r--r--   0        0        0    10571 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/clishowoverlay.py
--rw-r--r--   0        0        0     5161 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/clishowtshoot.py
--rw-r--r--   0        0        0    21550 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/clishowwids.py
--rw-r--r--   0        0        0     8288 2024-04-13 04:14:07.380022 centralcli-2.4.0/centralcli/clitest.py
--rw-r--r--   0        0        0    14323 2023-09-28 15:17:31.254705 centralcli-2.4.0/centralcli/clitshoot.py
--rw-r--r--   0        0        0     5888 2023-10-17 20:00:18.020614 centralcli-2.4.0/centralcli/cliunassign.py
--rw-r--r--   0        0        0    24518 2024-01-17 17:37:06.993460 centralcli-2.4.0/centralcli/cliupdate.py
--rw-r--r--   0        0        0     8998 2024-02-07 17:51:24.043436 centralcli-2.4.0/centralcli/cliupgrade.py
--rw-r--r--   0        0        0    25806 2024-01-17 17:05:54.453455 centralcli-2.4.0/centralcli/config.py
--rw-r--r--   0        0        0    40143 2024-04-13 05:21:28.905980 centralcli-2.4.0/centralcli/constants.py
--rw-r--r--   0        0        0      486 2023-09-09 22:06:46.585586 centralcli-2.4.0/centralcli/exceptions.py
--rw-r--r--   0        0        0     7182 2023-10-04 00:21:24.483615 centralcli-2.4.0/centralcli/logger.py
--rw-r--r--   0        0        0    17944 2024-02-07 17:51:17.423429 centralcli-2.4.0/centralcli/models.py
--rw-r--r--   0        0        0     3488 2023-10-26 00:01:09.236218 centralcli-2.4.0/centralcli/objects.py
--rw-r--r--   0        0        0    17382 2024-04-13 04:31:39.931505 centralcli-2.4.0/centralcli/render.py
--rw-r--r--   0        0        0    38994 2024-04-13 03:48:57.324702 centralcli-2.4.0/centralcli/response.py
--rw-r--r--   0        0        0       96 2021-10-13 20:41:19.000000 centralcli-2.4.0/centralcli/setup.py
--rw-r--r--   0        0        0     1150 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/static/favicon.ico
--rw-r--r--   0        0        0    14655 2023-10-10 17:46:32.627231 centralcli-2.4.0/centralcli/strings.py
--rw-r--r--   0        0        0    31102 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/utils.py
--rw-r--r--   0        0        0     5407 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/vscodeargs.py
--rw-r--r--   0        0        0    15335 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/wh2snow.py
--rw-r--r--   0        0        0    16108 2023-11-17 17:52:25.095728 centralcli-2.4.0/centralcli/wh_proxy.py
--rw-r--r--   0        0        0      393 2023-08-30 16:01:18.958011 centralcli-2.4.0/centralcli/wh_proxy_service.py
--rw-r--r--   0        0        0     2256 2024-04-11 21:37:01.039728 centralcli-2.4.0/pyproject.toml
--rw-r--r--   0        0        0    14176 1970-01-01 00:00:00.000000 centralcli-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-30 16:01:18.948011 centralcli-3.0.0/LICENSE
+-rw-r--r--   0        0        0    12115 2023-08-30 16:01:34.228021 centralcli-3.0.0/README.md
+-rw-r--r--   0        0        0     3924 2024-04-23 04:35:06.029220 centralcli-3.0.0/centralcli/__init__.py
+-rw-r--r--   0        0        0     1265 2023-09-08 18:43:03.749878 centralcli-3.0.0/centralcli/boilerplate/README.md
+-rw-r--r--   0        0        0  1156225 2024-03-22 20:25:45.394496 centralcli-3.0.0/centralcli/boilerplate/allcalls.py
+-rw-r--r--   0        0        0    12139 2023-08-30 16:01:18.948011 centralcli-3.0.0/centralcli/caas.py
+-rw-r--r--   0        0        0    96690 2024-04-23 03:46:22.846007 centralcli-3.0.0/centralcli/cache.py
+-rw-r--r--   0        0        0   209096 2024-04-23 01:59:34.046750 centralcli-3.0.0/centralcli/central.py
+-rw-r--r--   0        0        0    49057 2024-04-23 02:24:45.402520 centralcli-3.0.0/centralcli/cleaner.py
+-rw-r--r--   0        0        0    44531 2024-04-18 21:24:06.418846 centralcli-3.0.0/centralcli/cli.py
+-rw-r--r--   0        0        0    29819 2023-09-09 20:57:36.962267 centralcli-3.0.0/centralcli/cliadd.py
+-rw-r--r--   0        0        0     5372 2023-11-04 00:53:25.674537 centralcli-3.0.0/centralcli/cliassign.py
+-rw-r--r--   0        0        0    95394 2024-04-11 19:54:41.383365 centralcli-3.0.0/centralcli/clibatch.py
+-rw-r--r--   0        0        0    16403 2023-08-30 16:01:18.958011 centralcli-3.0.0/centralcli/clicaas.py
+-rw-r--r--   0        0        0     2995 2023-08-30 16:01:18.958011 centralcli-3.0.0/centralcli/cliclone.py
+-rw-r--r--   0        0        0    24868 2024-04-13 05:26:13.386524 centralcli-3.0.0/centralcli/clicommon.py
+-rw-r--r--   0        0        0    25402 2024-04-23 01:51:01.305794 centralcli-3.0.0/centralcli/clidel.py
+-rw-r--r--   0        0        0     3249 2024-04-23 01:56:25.646381 centralcli-3.0.0/centralcli/clidelfirmware.py
+-rw-r--r--   0        0        0     4765 2023-08-30 16:01:18.958011 centralcli-3.0.0/centralcli/clikick.py
+-rw-r--r--   0        0        0     3251 2023-08-30 16:01:18.958011 centralcli-3.0.0/centralcli/clirefresh.py
+-rw-r--r--   0        0        0     5400 2023-08-30 16:01:18.958011 centralcli-3.0.0/centralcli/clirename.py
+-rw-r--r--   0        0        0      712 2024-04-22 23:50:21.991969 centralcli-3.0.0/centralcli/cliset.py
+-rw-r--r--   0        0        0     3624 2024-04-23 01:57:48.666559 centralcli-3.0.0/centralcli/clisetfirmware.py
+-rw-r--r--   0        0        0   146406 2024-04-23 04:50:22.433257 centralcli-3.0.0/centralcli/clishow.py
+-rw-r--r--   0        0        0     3943 2023-08-30 16:01:18.958011 centralcli-3.0.0/centralcli/clishowbranch.py
+-rw-r--r--   0        0        0     7334 2024-04-23 02:03:29.597164 centralcli-3.0.0/centralcli/clishowfirmware.py
+-rw-r--r--   0        0        0    12980 2023-08-30 16:01:18.958011 centralcli-3.0.0/centralcli/clishowospf.py
+-rw-r--r--   0        0        0    10809 2024-04-22 23:42:36.251725 centralcli-3.0.0/centralcli/clishowoverlay.py
+-rw-r--r--   0        0        0     5161 2023-08-30 16:01:18.958011 centralcli-3.0.0/centralcli/clishowtshoot.py
+-rw-r--r--   0        0        0    21550 2023-08-30 16:01:18.958011 centralcli-3.0.0/centralcli/clishowwids.py
+-rw-r--r--   0        0        0     8288 2024-04-13 04:14:07.380022 centralcli-3.0.0/centralcli/clitest.py
+-rw-r--r--   0        0        0    14323 2023-09-28 15:17:31.254705 centralcli-3.0.0/centralcli/clitshoot.py
+-rw-r--r--   0        0        0     5888 2023-10-17 20:00:18.020614 centralcli-3.0.0/centralcli/cliunassign.py
+-rw-r--r--   0        0        0    24518 2024-01-17 17:37:06.993460 centralcli-3.0.0/centralcli/cliupdate.py
+-rw-r--r--   0        0        0     8998 2024-02-07 17:51:24.043436 centralcli-3.0.0/centralcli/cliupgrade.py
+-rw-r--r--   0        0        0    25806 2024-04-23 04:34:41.379051 centralcli-3.0.0/centralcli/config.py
+-rw-r--r--   0        0        0    40143 2024-04-22 23:58:26.942271 centralcli-3.0.0/centralcli/constants.py
+-rw-r--r--   0        0        0      487 2024-04-23 00:38:18.706030 centralcli-3.0.0/centralcli/exceptions.py
+-rw-r--r--   0        0        0     7182 2023-10-04 00:21:24.483615 centralcli-3.0.0/centralcli/logger.py
+-rw-r--r--   0        0        0    17944 2024-02-07 17:51:17.423429 centralcli-3.0.0/centralcli/models.py
+-rw-r--r--   0        0        0     3488 2023-10-26 00:01:09.236218 centralcli-3.0.0/centralcli/objects.py
+-rw-r--r--   0        0        0    17382 2024-04-13 04:31:39.931505 centralcli-3.0.0/centralcli/render.py
+-rw-r--r--   0        0        0    38994 2024-04-13 03:48:57.324702 centralcli-3.0.0/centralcli/response.py
+-rw-r--r--   0        0        0       96 2021-10-13 20:41:19.000000 centralcli-3.0.0/centralcli/setup.py
+-rw-r--r--   0        0        0     1150 2023-08-30 16:01:18.958011 centralcli-3.0.0/centralcli/static/favicon.ico
+-rw-r--r--   0        0        0    14655 2023-10-10 17:46:32.627231 centralcli-3.0.0/centralcli/strings.py
+-rw-r--r--   0        0        0    31102 2023-08-30 16:01:18.958011 centralcli-3.0.0/centralcli/utils.py
+-rw-r--r--   0        0        0     5407 2023-08-30 16:01:18.958011 centralcli-3.0.0/centralcli/vscodeargs.py
+-rw-r--r--   0        0        0    15335 2023-08-30 16:01:18.958011 centralcli-3.0.0/centralcli/wh2snow.py
+-rw-r--r--   0        0        0    16108 2023-11-17 17:52:25.095728 centralcli-3.0.0/centralcli/wh_proxy.py
+-rw-r--r--   0        0        0      393 2023-08-30 16:01:18.958011 centralcli-3.0.0/centralcli/wh_proxy_service.py
+-rw-r--r--   0        0        0     2256 2024-04-23 04:48:49.112998 centralcli-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    14176 1970-01-01 00:00:00.000000 centralcli-3.0.0/PKG-INFO
```

### Comparing `centralcli-2.4.0/LICENSE` & `centralcli-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/README.md` & `centralcli-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/__init__.py` & `centralcli-3.0.0/centralcli/__init__.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/boilerplate/README.md` & `centralcli-3.0.0/centralcli/boilerplate/README.md`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/boilerplate/allcalls.py` & `centralcli-3.0.0/centralcli/boilerplate/allcalls.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/caas.py` & `centralcli-3.0.0/centralcli/caas.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/cache.py` & `centralcli-3.0.0/centralcli/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
-# Used to debug completion
-# from rich.console import Console
-# console = Console(stderr=True)
 import asyncio
 import time
 from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Literal, Sequence, Set, Union
 
 import typer
@@ -28,14 +25,15 @@
 try:
     from fuzzywuzzy import process  # type: ignore noqa
     FUZZ = True
 except Exception:
     FUZZ = False
     pass
 
+# Used to debug completion
 err_console = Console(stderr=True)
 TinyDB.default_table_name = "devices"
 
 # DBType = Literal["dev", "site", "template", "group"]
 DEV_COMPLETION = ["move", "device", ""]
 SITE_COMPLETION = ["site"]
 GROUP_COMPLETION = ["group", "wlan"]
@@ -84,14 +82,15 @@
         # When building Central Object from Inventory this is necessary
         # TODO maybe pydantic model
         if self.is_dev and self.data:
             self.name = self.data["name"] = self.data.get("name", self.data["serial"])
             self.status = self.data["status"] = self.data.get("status")
             self.ip = self.data["ip"] = self.data.get("ip")
             self.site = self.data["site"] = self.data.get("site")
+            self.swack_id = self.data["swack_id"] = self.data.get("swack_id")
 
     def __bool__(self):
         return bool(self.data)
 
     def __repr__(self):
         _ = f"<{self.__module__}.{type(self).__name__} ({self.cache}|{self.get('name', bool(self))}) object at {hex(id(self))}>"
         return _
@@ -1020,14 +1019,15 @@
         out = []
         if match:
             match = [m for m in match if m.name not in args]
             for m in sorted(match, key=lambda i: i.name):
                 out += [tuple([m.name if " " not in m.name else f"'{m.name}'", m.help_text])]
 
         for m in out:
+            # err_console.print(f'{m=}')
             yield m
 
     def template_completion(
         self,
         incomplete: str,
         args: List[str] = None,
     ):
@@ -1913,71 +1913,79 @@
                 raise typer.Exit(1)
             else:
                 return None
 
     def get_site_identifier(
         self,
         query_str: Union[str, List[str], tuple],
-        ret_field: str = "id",
         retry: bool = True,
-        multi_ok: bool = False,
         completion: bool = False,
         silent: bool = False,
     ) -> CentralObject:
         retry = False if completion else retry
         if isinstance(query_str, (list, tuple)):
             query_str = " ".join(query_str)
 
 
         if completion and query_str == "":
             return [CentralObject("site", s) for s in self.sites]
 
         match = None
         for _ in range(0, 2 if retry else 1):
-            # TODO match on name first then the other stuff
-            # 'm' returns Pommore          main-batch-demo  mb1-batch-demo
-            #   because Pommore is in Milford
-            # try exact site match
+            # try exact match by name
             match = self.SiteDB.search(
                 (self.Q.name == query_str)
-                | (self.Q.id.test(lambda v: str(v) == query_str))
-                | (self.Q.zipcode == query_str)
-                | (self.Q.address == query_str)
-                | (self.Q.city == query_str)
-                | (self.Q.state == query_str)
-                | (self.Q.state.test(lambda v: constants.state_abbrev_to_pretty.get(query_str.upper(), query_str).title() == v.title()))
             )
 
-            # raise ValueError(f'>{query_str}<, {type(query_str)}, {", ".join([m["name"] for m in match])} {bool(match)}')
+            # try exact match by other fields
+            if not match:
+                match = self.SiteDB.search(
+                    (self.Q.id.test(lambda v: str(v) == query_str))
+                    | (self.Q.zipcode == query_str)
+                    | (self.Q.address == query_str)
+                    | (self.Q.city == query_str)
+                    | (self.Q.state == query_str)
+                    | (self.Q.state.test(lambda v: constants.state_abbrev_to_pretty.get(query_str.upper(), query_str).title() == v.title()))
+                )
 
-            # retry with case insensitive name & address match if no match with original query
+            # try case insensitive name
             if not match:
                 match = self.SiteDB.search(
                     (self.Q.name.test(lambda v: v.lower() == query_str.lower()))
-                    | self.Q.address.test(lambda v: v.lower().replace(" ", "") == query_str.lower().replace(" ", ""))
+                )
+            # try case insensitve address match
+            if not match:
+                match = self.SiteDB.search(
+                    self.Q.address.test(lambda v: v.lower().replace(" ", "") == query_str.lower().replace(" ", ""))
                 )
 
-            # swap _ and - and case insensitive
+            # try case insensitive name swapping _ and -
             if not match:
                 if "-" in query_str:
                     match = self.SiteDB.search(self.Q.name.test(lambda v: v.lower() == query_str.lower().replace("-", "_")))
                 elif "_" in query_str:
                     match = self.SiteDB.search(self.Q.name.test(lambda v: v.lower() == query_str.lower().replace("_", "-")))
 
-            # Last Chance try to match name if it startswith provided value
+            # try case insensitive name starts with
             if not match:
                 match = self.SiteDB.search(
                     self.Q.name.test(lambda v: v.lower().startswith(query_str.lower()))
-                    | self.Q.zipcode.test(lambda v: v.startswith(query_str))
+                )
+
+            # Last Chance try other fields case insensitive startswith provided value
+            if not match:
+                match = self.SiteDB.search(
+                    self.Q.zipcode.test(lambda v: v.startswith(query_str))
                     | self.Q.city.test(lambda v: v.lower().startswith(query_str.lower()))
                     | self.Q.state.test(lambda v: v.lower().startswith(query_str.lower()))
                     | self.Q.address.test(lambda v: v.lower().startswith(query_str.lower()))
                     | self.Q.address.test(lambda v: " ".join(v.split(" ")[1:]).lower().startswith(query_str.lower()))
                 )
 
+            # err_console.print(f'\n{match=} {query_str=} {retry=} {completion=} {silent=}')  # DEBUG
             if retry and not match and self.central.get_all_sites not in self.updated:
                 if FUZZ and not completion:
                     fuzz_match, fuzz_confidence = process.extract(query_str, [s["name"] for s in self.sites], limit=1)[0]
                     confirm_str = render.rich_capture(f"[bright_red]{query_str}[/] not found in cache.  Did you mean [green3]{fuzz_match}[/]?")
                     if fuzz_confidence >= 70 and typer.confirm(confirm_str):
                         match = self.SiteDB.search(self.Q.name == fuzz_match)
                 if not match:
@@ -1988,15 +1996,15 @@
                 break
 
         if completion:
             return match
 
         if match:
             if len(match) > 1:
-                match = self.handle_multi_match(match, query_str=query_str, query_type="site",)  # multi_ok=multi_ok)
+                match = self.handle_multi_match(match, query_str=query_str, query_type="site",)
 
             return match[0]
 
         elif retry:
             log.error(f"Unable to gather site info from provided identifier {query_str}", show=not silent)
             raise typer.Exit(1)
 
@@ -2306,15 +2314,15 @@
                     if qry_mac or len(qry_mac) == len(qry_mac_fuzzy):
                         match = self.ClientDB.search(
                             self.Q.mac.test(lambda v: v.lower().startswith(utils.Mac(query_str, fuzzy=completion).cols.lower()))
                         )
 
             # no match found initiate cache update
             if retry and not match and self.central.get_clients not in self.updated:
-                if FUZZ:
+                if FUZZ and self.clients:
                     fuzz_match, fuzz_confidence = process.extract(query_str, [d["name"] for d in self.clients], limit=1)[0]
                     confirm_str = render.rich_capture(f"[bright_red]{query_str}[/] not found in cache.  Did you mean [green3]{fuzz_match}[/]?")
                     if fuzz_confidence >= 70 and typer.confirm(confirm_str):
                         match = self.ClientDB.search(self.Q.name == fuzz_match)
                 if not match:
                     print(f"[bright_red]No Match Found[/] for [cyan]{query_str}[/], Updating Client Cache")
                     asyncio.run(self.update_client_db("wireless"))  # on demand update only for WLAN as kick only applies to WLAN currently
```

### Comparing `centralcli-2.4.0/centralcli/central.py` & `centralcli-3.0.0/centralcli/central.py`

 * *Files 1% similar despite different names*

```diff
@@ -8414,4531 +8414,4656 @@
 00020dd0: 6172 616d 7329 0a0a 2020 2020 4465 7654  arams)..    DevT
 00020de0: 7970 6520 3d20 4c69 7465 7261 6c5b 2249  ype = Literal["I
 00020df0: 4150 222c 2022 4850 222c 2022 434f 4e54  AP", "HP", "CONT
 00020e00: 524f 4c4c 4552 225d 0a0a 2020 2020 6173  ROLLER"]..    as
 00020e10: 796e 6320 6465 6620 6765 745f 6669 726d  ync def get_firm
 00020e20: 7761 7265 5f63 6f6d 706c 6961 6e63 6528  ware_compliance(
 00020e30: 7365 6c66 2c20 6465 7669 6365 5f74 7970  self, device_typ
-00020e40: 653a 2044 6576 5479 7065 2c20 6772 6f75  e: DevType, grou
-00020e50: 703a 2073 7472 203d 204e 6f6e 6529 202d  p: str = None) -
-00020e60: 3e20 5265 7370 6f6e 7365 3a0a 2020 2020  > Response:.    
-00020e70: 2020 2020 2222 2247 6574 2046 6972 6d77      """Get Firmw
-00020e80: 6172 6520 436f 6d70 6c69 616e 6365 2056  are Compliance V
-00020e90: 6572 7369 6f6e 2e0a 0a20 2020 2020 2020  ersion...       
-00020ea0: 202f 2f20 5573 6564 2062 7920 7368 6f77   // Used by show
-00020eb0: 2066 6972 6d77 6172 6520 636f 6d70 6c69   firmware compli
-00020ec0: 616e 6365 205b 6170 7c67 777c 7377 5d20  ance [ap|gw|sw] 
-00020ed0: 5b67 726f 7570 2d6e 616d 655d 202f 2f0a  [group-name] //.
-00020ee0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00020ef0: 2020 2020 2020 2020 2020 2064 6576 6963             devic
-00020f00: 655f 7479 7065 2028 7374 7229 3a20 5370  e_type (str): Sp
-00020f10: 6563 6966 7920 6f6e 6520 6f66 2022 4941  ecify one of "IA
-00020f20: 502f 4d41 532f 4850 2f43 4f4e 5452 4f4c  P/MAS/HP/CONTROL
-00020f30: 4c45 5222 0a20 2020 2020 2020 2020 2020  LER".           
-00020f40: 2067 726f 7570 2028 7374 722c 206f 7074   group (str, opt
-00020f50: 696f 6e61 6c29 3a20 4772 6f75 7020 6e61  ional): Group na
-00020f60: 6d65 2e20 4465 6661 756c 7473 2074 6f20  me. Defaults to 
-00020f70: 4e6f 6e65 2028 476c 6f62 616c 2043 6f6d  None (Global Com
-00020f80: 706c 6961 6e63 6529 0a0a 2020 2020 2020  pliance)..      
-00020f90: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00020fa0: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
-00020fb0: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
-00020fc0: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
-00020fd0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00020fe0: 2320 4150 4920 6d65 7468 6f64 2072 6574  # API method ret
-00020ff0: 7572 6e73 2034 3034 2069 6620 636f 6d70  urns 404 if comp
-00021000: 6c69 616e 6365 2069 7320 6e6f 7420 7365  liance is not se
-00021010: 7421 0a20 2020 2020 2020 2075 726c 203d  t!.        url =
-00021020: 2022 2f66 6972 6d77 6172 652f 7631 2f75   "/firmware/v1/u
-00021030: 7067 7261 6465 2f63 6f6d 706c 6961 6e63  pgrade/complianc
-00021040: 655f 7665 7273 696f 6e22 0a0a 2020 2020  e_version"..    
-00021050: 2020 2020 7061 7261 6d73 203d 207b 0a20      params = {. 
-00021060: 2020 2020 2020 2020 2020 2027 6465 7669             'devi
-00021070: 6365 5f74 7970 6527 3a20 6465 7669 6365  ce_type': device
-00021080: 5f74 7970 652c 0a20 2020 2020 2020 2020  _type,.         
-00021090: 2020 2027 6772 6f75 7027 3a20 6772 6f75     'group': grou
-000210a0: 700a 2020 2020 2020 2020 7d0a 0a20 2020  p.        }..   
-000210b0: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
-000210c0: 7420 7365 6c66 2e67 6574 2875 726c 2c20  t self.get(url, 
-000210d0: 7061 7261 6d73 3d70 6172 616d 7329 0a0a  params=params)..
-000210e0: 2020 2020 6173 796e 6320 6465 6620 6465      async def de
-000210f0: 6c65 7465 5f66 6972 6d77 6172 655f 636f  lete_firmware_co
-00021100: 6d70 6c69 616e 6365 2873 656c 662c 2064  mpliance(self, d
-00021110: 6576 6963 655f 7479 7065 3a20 7374 722c  evice_type: str,
-00021120: 2067 726f 7570 3a20 7374 7220 3d20 4e6f   group: str = No
-00021130: 6e65 2920 2d3e 2052 6573 706f 6e73 653a  ne) -> Response:
-00021140: 0a20 2020 2020 2020 2022 2222 436c 6561  .        """Clea
-00021150: 7220 4669 726d 7761 7265 2043 6f6d 706c  r Firmware Compl
-00021160: 6961 6e63 6520 5665 7273 696f 6e2e 0a0a  iance Version...
-00021170: 2020 2020 2020 2020 2f2f 2055 7365 6420          // Used 
-00021180: 6279 2064 656c 6574 6520 6669 726d 7761  by delete firmwa
-00021190: 7265 2063 6f6d 706c 6961 6e63 6520 5b61  re compliance [a
-000211a0: 707c 6777 7c73 7769 7463 685d 205b 6772  p|gw|switch] [gr
-000211b0: 6f75 705d 202f 2f0a 0a20 2020 2020 2020  oup] //..       
-000211c0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-000211d0: 2020 2064 6576 6963 655f 7479 7065 2028     device_type (
-000211e0: 7374 7229 3a20 5370 6563 6966 7920 6f6e  str): Specify on
-000211f0: 6520 6f66 2022 4941 502f 4d41 532f 4850  e of "IAP/MAS/HP
-00021200: 2f43 4f4e 5452 4f4c 4c45 5222 0a20 2020  /CONTROLLER".   
-00021210: 2020 2020 2020 2020 2067 726f 7570 2028           group (
-00021220: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
-00021230: 4772 6f75 7020 6e61 6d65 2e20 4465 6661  Group name. Defa
-00021240: 756c 7473 2074 6f20 4e6f 6e65 2028 476c  ults to None (Gl
-00021250: 6f62 616c 2043 6f6d 706c 6961 6e63 6529  obal Compliance)
-00021260: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00021270: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-00021280: 6573 706f 6e73 653a 2043 656e 7472 616c  esponse: Central
-00021290: 4150 4920 5265 7370 6f6e 7365 206f 626a  API Response obj
-000212a0: 6563 740a 2020 2020 2020 2020 2222 220a  ect.        """.
-000212b0: 2020 2020 2020 2020 7572 6c20 3d20 222f          url = "/
-000212c0: 6669 726d 7761 7265 2f76 312f 7570 6772  firmware/v1/upgr
-000212d0: 6164 652f 636f 6d70 6c69 616e 6365 5f76  ade/compliance_v
-000212e0: 6572 7369 6f6e 220a 0a20 2020 2020 2020  ersion"..       
-000212f0: 2070 6172 616d 7320 3d20 7b0a 2020 2020   params = {.    
-00021300: 2020 2020 2020 2020 2764 6576 6963 655f          'device_
-00021310: 7479 7065 273a 2064 6576 6963 655f 7479  type': device_ty
-00021320: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
-00021330: 2767 726f 7570 273a 2067 726f 7570 0a20  'group': group. 
-00021340: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-00021350: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
-00021360: 656c 662e 6465 6c65 7465 2875 726c 2c20  elf.delete(url, 
-00021370: 7061 7261 6d73 3d70 6172 616d 7329 0a0a  params=params)..
-00021380: 2020 2020 6173 796e 6320 6465 6620 6d6f      async def mo
-00021390: 7665 5f64 6576 6963 6573 5f74 6f5f 6772  ve_devices_to_gr
-000213a0: 6f75 7028 0a20 2020 2020 2020 2073 656c  oup(.        sel
-000213b0: 662c 0a20 2020 2020 2020 2067 726f 7570  f,.        group
-000213c0: 3a20 7374 722c 0a20 2020 2020 2020 2073  : str,.        s
-000213d0: 6572 6961 6c5f 6e75 6d73 3a20 556e 696f  erial_nums: Unio
-000213e0: 6e5b 7374 722c 204c 6973 745b 7374 725d  n[str, List[str]
-000213f0: 5d2c 0a20 2020 2020 2020 202a 2c0a 2020  ],.        *,.  
-00021400: 2020 2020 2020 6378 5f72 6574 6169 6e5f        cx_retain_
-00021410: 636f 6e66 6967 3a20 626f 6f6c 203d 2054  config: bool = T
-00021420: 7275 652c 2020 2320 544f 444f 2063 616e  rue,  # TODO can
-00021430: 2077 6520 7365 6e64 2074 6869 7320 6174   we send this at
-00021440: 7472 6962 7574 6520 6576 656e 2069 6620  tribute even if 
-00021450: 6974 2773 206e 6f74 2043 582c 2077 696c  it's not CX, wil
-00021460: 6c20 6974 2069 676e 6f72 6520 6f72 2065  l it ignore or e
-00021470: 7272 6f72 0a20 2020 2029 202d 3e20 5265  rror.    ) -> Re
-00021480: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
-00021490: 2222 224d 6f76 6520 6465 7669 6365 7320  """Move devices 
-000214a0: 746f 2061 2067 726f 7570 2e0a 0a20 2020  to a group...   
-000214b0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-000214c0: 2020 2020 2020 2067 726f 7570 2028 7374         group (st
-000214d0: 7229 3a20 4772 6f75 7020 4e61 6d65 2074  r): Group Name t
-000214e0: 6f20 6d6f 7665 2064 6576 6963 6520 746f  o move device to
-000214f0: 2e0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00021500: 7269 616c 7320 284c 6973 745b 7374 725d  rials (List[str]
-00021510: 293a 2053 6572 6961 6c20 6e75 6d62 6572  ): Serial number
-00021520: 7320 6f66 2064 6576 6963 6573 2074 6f20  s of devices to 
-00021530: 6265 2061 6464 6564 2074 6f20 6772 6f75  be added to grou
-00021540: 702e 0a0a 2020 2020 2020 2020 5265 7475  p...        Retu
-00021550: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00021560: 2052 6573 706f 6e73 653a 2043 656e 7472   Response: Centr
-00021570: 616c 4150 4920 5265 7370 6f6e 7365 206f  alAPI Response o
-00021580: 626a 6563 740a 2020 2020 2020 2020 2222  bject.        ""
-00021590: 220a 2020 2020 2020 2020 2320 4150 492d  ".        # API-
-000215a0: 464c 4157 2072 6570 6f72 7420 666c 6177  FLAW report flaw
-000215b0: 6564 2041 5049 206d 6574 686f 640a 2020  ed API method.  
-000215c0: 2020 2020 2020 2320 5265 7475 726e 7320        # Returns 
-000215d0: 3530 3020 7374 6174 7573 2063 6f64 6520  500 status code 
-000215e0: 7768 656e 2072 6573 756c 7420 6973 2065  when result is e
-000215f0: 7373 656e 7469 616c 6c79 2073 7563 6365  ssentially succe
-00021600: 7373 0a20 2020 2020 2020 2023 2050 6c65  ss.        # Ple
-00021610: 6173 6520 436f 6e66 6972 6d3a 206d 6f76  ase Confirm: mov
-00021620: 6520 4172 7562 6139 3030 345f 3831 5f45  e Aruba9004_81_E
-00021630: 385f 4641 2026 2050 6f6d 6d6f 7265 4757  8_FA & PommoreGW
-00021640: 3120 746f 2067 726f 7570 2057 4c4e 4554  1 to group WLNET
-00021650: 3f20 5b79 2f4e 5d3a 2079 0a20 2020 2020  ? [y/N]: y.     
-00021660: 2020 2023 20e2 9c96 2053 656e 6469 6e67     # ... Sending
-00021670: 2044 6174 6120 5b63 6f6e 6669 6775 7261   Data [configura
-00021680: 7469 6f6e 2f76 312f 6465 7669 6365 732f  tion/v1/devices/
-00021690: 6d6f 7665 5d0a 2020 2020 2020 2020 2320  move].        # 
-000216a0: 7374 6174 7573 2063 6f64 653a 2035 3030  status code: 500
-000216b0: 203c 2d2d 2035 3030 206f 6e20 7375 6363   <-- 500 on succ
-000216c0: 6573 732e 2020 4174 206c 6561 7374 2066  ess.  At least f
-000216d0: 6f72 2067 7720 776f 756c 6420 6e65 6564  or gw would need
-000216e0: 2074 6f20 646f 7562 6c65 2063 6865 636b   to double check
-000216f0: 206f 7468 6572 732e 0a20 2020 2020 2020   others..       
-00021700: 2023 2064 6573 6372 6970 7469 6f6e 3a0a   # description:.
-00021710: 2020 2020 2020 2020 2320 436f 6e74 726f          # Contro
-00021720: 6c6c 6572 2f47 6174 6577 6179 2067 726f  ller/Gateway gro
-00021730: 7570 206d 6f76 6520 6861 7320 6265 656e  up move has been
-00021740: 2069 6e69 7469 6174 6564 2c20 706c 6561   initiated, plea
-00021750: 7365 2063 6865 636b 2061 7564 6974 2074  se check audit t
-00021760: 7261 696c 2066 6f72 2064 6574 6169 6c73  rail for details
-00021770: 0a20 2020 2020 2020 2023 2065 7272 6f72  .        # error
-00021780: 5f63 6f64 653a 2030 3030 310a 2020 2020  _code: 0001.    
-00021790: 2020 2020 2320 7365 7276 6963 655f 6e61      # service_na
-000217a0: 6d65 3a20 436f 6e66 6967 7572 6174 696f  me: Configuratio
-000217b0: 6e0a 2020 2020 2020 2020 7572 6c20 3d20  n.        url = 
-000217c0: 222f 636f 6e66 6967 7572 6174 696f 6e2f  "/configuration/
-000217d0: 7631 2f64 6576 6963 6573 2f6d 6f76 6522  v1/devices/move"
-000217e0: 0a20 2020 2020 2020 2073 6572 6961 6c5f  .        serial_
-000217f0: 6e75 6d73 203d 2075 7469 6c73 2e6c 6973  nums = utils.lis
-00021800: 7469 6679 2873 6572 6961 6c5f 6e75 6d73  tify(serial_nums
-00021810: 290a 0a20 2020 2020 2020 206a 736f 6e5f  )..        json_
-00021820: 6461 7461 203d 207b 0a20 2020 2020 2020  data = {.       
-00021830: 2020 2020 2027 6772 6f75 7027 3a20 6772       'group': gr
-00021840: 6f75 702c 0a20 2020 2020 2020 2020 2020  oup,.           
-00021850: 2027 7365 7269 616c 7327 3a20 7365 7269   'serials': seri
-00021860: 616c 5f6e 756d 730a 2020 2020 2020 2020  al_nums.        
-00021870: 7d0a 0a20 2020 2020 2020 2069 6620 6378  }..        if cx
-00021880: 5f72 6574 6169 6e5f 636f 6e66 6967 3a0a  _retain_config:.
-00021890: 2020 2020 2020 2020 2020 2020 6a73 6f6e              json
-000218a0: 5f64 6174 615b 2270 7265 7365 7276 655f  _data["preserve_
-000218b0: 636f 6e66 6967 5f6f 7665 7272 6964 6573  config_overrides
-000218c0: 225d 203d 205b 2241 4f53 5f43 5822 5d0a  "] = ["AOS_CX"].
-000218d0: 0a20 2020 2020 2020 2072 6573 7020 3d20  .        resp = 
-000218e0: 6177 6169 7420 7365 6c66 2e70 6f73 7428  await self.post(
-000218f0: 7572 6c2c 206a 736f 6e5f 6461 7461 3d6a  url, json_data=j
-00021900: 736f 6e5f 6461 7461 290a 0a20 2020 2020  son_data)..     
-00021910: 2020 2023 2054 6869 7320 6d65 7468 6f64     # This method
-00021920: 2072 6574 7572 6e73 2073 7461 7475 7320   returns status 
-00021930: 3530 3020 7769 7468 206d 7367 2074 6861  500 with msg tha
-00021940: 7420 6d6f 7665 2069 7320 696e 6974 6961  t move is initia
-00021950: 7465 6420 6f6e 2073 7563 6365 7373 2e0a  ted on success..
-00021960: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-00021970: 6573 7020 616e 6420 7265 7370 2e73 7461  esp and resp.sta
-00021980: 7475 7320 3d3d 2035 3030 3a0a 2020 2020  tus == 500:.    
-00021990: 2020 2020 2020 2020 6d61 7463 685f 7374          match_st
-000219a0: 7220 3d20 2267 726f 7570 206d 6f76 6520  r = "group move 
-000219b0: 6861 7320 6265 656e 2069 6e69 7469 6174  has been initiat
-000219c0: 6564 2c20 706c 6561 7365 2063 6865 636b  ed, please check
-000219d0: 2061 7564 6974 2074 7261 696c 2066 6f72   audit trail for
-000219e0: 2064 6574 6169 6c73 220a 2020 2020 2020   details".      
-000219f0: 2020 2020 2020 6966 206d 6174 6368 5f73        if match_s
-00021a00: 7472 2069 6e20 7265 7370 2e6f 7574 7075  tr in resp.outpu
-00021a10: 742e 6765 7428 2264 6573 6372 6970 7469  t.get("descripti
-00021a20: 6f6e 222c 2022 2229 3a0a 2020 2020 2020  on", ""):.      
-00021a30: 2020 2020 2020 2020 2020 7265 7370 2e6f            resp.o
-00021a40: 6b20 3d20 5472 7565 0a0a 2020 2020 2020  k = True..      
-00021a50: 2020 7265 7475 726e 2072 6573 700a 0a20    return resp.. 
-00021a60: 2020 2061 7379 6e63 2064 6566 2067 6574     async def get
-00021a70: 5f64 6566 6175 6c74 5f67 726f 7570 2873  _default_group(s
-00021a80: 656c 662c 2920 2d3e 2052 6573 706f 6e73  elf,) -> Respons
-00021a90: 653a 0a20 2020 2020 2020 2022 2222 4765  e:.        """Ge
-00021aa0: 7420 6465 6661 756c 7420 6772 6f75 702e  t default group.
-00021ab0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00021ac0: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-00021ad0: 6573 706f 6e73 653a 2043 656e 7472 616c  esponse: Central
-00021ae0: 4150 4920 5265 7370 6f6e 7365 206f 626a  API Response obj
-00021af0: 6563 740a 2020 2020 2020 2020 2222 220a  ect.        """.
-00021b00: 2020 2020 2020 2020 7572 6c20 3d20 222f          url = "/
-00021b10: 636f 6e66 6967 7572 6174 696f 6e2f 7631  configuration/v1
-00021b20: 2f67 726f 7570 732f 6465 6661 756c 745f  /groups/default_
-00021b30: 6772 6f75 7022 0a0a 2020 2020 2020 2020  group"..        
-00021b40: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
-00021b50: 662e 6765 7428 7572 6c29 0a0a 2020 2020  f.get(url)..    
-00021b60: 6173 796e 6320 6465 6620 6d6f 7665 5f64  async def move_d
-00021b70: 6576 6963 6573 5f74 6f5f 7369 7465 280a  evices_to_site(.
-00021b80: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00021b90: 2020 2020 2020 7369 7465 5f69 643a 2069        site_id: i
-00021ba0: 6e74 2c0a 2020 2020 2020 2020 7365 7269  nt,.        seri
-00021bb0: 616c 5f6e 756d 733a 2055 6e69 6f6e 5b73  al_nums: Union[s
-00021bc0: 7472 2c20 4c69 7374 5b73 7472 5d5d 2c0a  tr, List[str]],.
-00021bd0: 2020 2020 2020 2020 6465 7669 6365 5f74          device_t
-00021be0: 7970 653a 204c 6974 6572 616c 5b22 6170  ype: Literal["ap
-00021bf0: 222c 2022 6378 222c 2022 7377 222c 2022  ", "cx", "sw", "
-00021c00: 7377 6974 6368 222c 2022 6777 225d 2c0a  switch", "gw"],.
-00021c10: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
-00021c20: 653a 0a20 2020 2020 2020 2022 2222 4173  e:.        """As
-00021c30: 736f 6369 6174 6520 6c69 7374 206f 6620  sociate list of 
-00021c40: 6465 7669 6365 7320 746f 2061 2073 6974  devices to a sit
-00021c50: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
-00021c60: 3a0a 2020 2020 2020 2020 2020 2020 7369  :.            si
-00021c70: 7465 5f69 6420 2869 6e74 293a 2053 6974  te_id (int): Sit
-00021c80: 6520 4944 0a20 2020 2020 2020 2020 2020  e ID.           
-00021c90: 2064 6576 6963 655f 7479 7065 2028 7374   device_type (st
-00021ca0: 7229 3a20 4465 7669 6365 2074 7970 652e  r): Device type.
-00021cb0: 2056 616c 6964 2056 616c 7565 733a 2061   Valid Values: a
-00021cc0: 702c 2063 782c 2073 772c 2073 7769 7463  p, cx, sw, switc
-00021cd0: 682c 2067 770a 2020 2020 2020 2020 2020  h, gw.          
-00021ce0: 2020 2020 2020 6378 2061 6e64 2073 7720        cx and sw 
-00021cf0: 6172 6520 7468 6520 7361 6d65 2061 7320  are the same as 
-00021d00: 7468 6520 6d6f 7265 2067 656e 6572 6963  the more generic
-00021d10: 2073 7769 7463 682e 0a20 2020 2020 2020   switch..       
-00021d20: 2020 2020 2073 6572 6961 6c5f 6e75 6d73       serial_nums
-00021d30: 2028 4c69 7374 5b73 7472 5d29 3a20 4c69   (List[str]): Li
-00021d40: 7374 206f 6620 6465 7669 6365 2073 6572  st of device ser
-00021d50: 6961 6c20 6e75 6d62 6572 7320 6f66 2074  ial numbers of t
-00021d60: 6865 2064 6576 6963 6573 2074 6f20 7768  he devices to wh
-00021d70: 6963 6820 7468 6520 7369 7465 0a20 2020  ich the site.   
-00021d80: 2020 2020 2020 2020 2020 2020 2068 6173               has
-00021d90: 2074 6f20 6265 2075 6e2f 6173 736f 6369   to be un/associ
-00021da0: 6174 6564 2077 6974 682e 2041 206d 6178  ated with. A max
-00021db0: 696d 756d 206f 6620 3530 3030 2064 6576  imum of 5000 dev
-00021dc0: 6963 6520 7365 7269 616c 7320 6172 6520  ice serials are 
-00021dd0: 616c 6c6f 7765 6420 6174 206f 6e63 652e  allowed at once.
-00021de0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00021df0: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-00021e00: 6573 706f 6e73 653a 2043 656e 7472 616c  esponse: Central
-00021e10: 4150 4920 5265 7370 6f6e 7365 206f 626a  API Response obj
-00021e20: 6563 740a 2020 2020 2020 2020 2222 220a  ect.        """.
-00021e30: 2020 2020 2020 2020 2320 544f 444f 206d          # TODO m
-00021e40: 616b 6520 6465 7669 6365 5f74 7970 6573  ake device_types
-00021e50: 2063 6f6e 7369 7374 656e 7420 7468 726f   consistent thro
-00021e60: 7567 686f 7574 0a20 2020 2020 2020 2064  ughout.        d
-00021e70: 6576 6963 655f 7479 7065 203d 2063 6f6e  evice_type = con
-00021e80: 7374 616e 7473 2e6c 6962 5f74 6f5f 6170  stants.lib_to_ap
-00021e90: 6928 2273 6974 6522 2c20 6465 7669 6365  i("site", device
-00021ea0: 5f74 7970 6529 0a20 2020 2020 2020 2069  _type).        i
-00021eb0: 6620 6e6f 7420 6465 7669 6365 5f74 7970  f not device_typ
-00021ec0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00021ed0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00021ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021ef0: 2066 2249 6e76 616c 6964 2056 616c 7565   f"Invalid Value
-00021f00: 2066 6f72 2064 6576 6963 655f 7479 7065   for device_type
-00021f10: 2e20 2053 7570 706f 7274 6564 2056 616c  .  Supported Val
-00021f20: 7565 733a 207b 636f 6e73 7461 6e74 732e  ues: {constants.
-00021f30: 6c69 625f 746f 5f61 7069 2e76 616c 6964  lib_to_api.valid
-00021f40: 5f73 7472 7d22 0a20 2020 2020 2020 2020  _str}".         
-00021f50: 2020 2029 0a0a 2020 2020 2020 2020 7572     )..        ur
-00021f60: 6c20 3d20 222f 6365 6e74 7261 6c2f 7632  l = "/central/v2
-00021f70: 2f73 6974 6573 2f61 7373 6f63 6961 7469  /sites/associati
-00021f80: 6f6e 7322 0a20 2020 2020 2020 2073 6572  ons".        ser
-00021f90: 6961 6c5f 6e75 6d73 203d 2075 7469 6c73  ial_nums = utils
-00021fa0: 2e6c 6973 7469 6679 2873 6572 6961 6c5f  .listify(serial_
-00021fb0: 6e75 6d73 290a 0a20 2020 2020 2020 206a  nums)..        j
-00021fc0: 736f 6e5f 6461 7461 203d 207b 0a20 2020  son_data = {.   
-00021fd0: 2020 2020 2020 2020 2027 7369 7465 5f69           'site_i
-00021fe0: 6427 3a20 7369 7465 5f69 642c 0a20 2020  d': site_id,.   
-00021ff0: 2020 2020 2020 2020 2027 6465 7669 6365           'device
-00022000: 5f69 6473 273a 2073 6572 6961 6c5f 6e75  _ids': serial_nu
-00022010: 6d73 2c0a 2020 2020 2020 2020 2020 2020  ms,.            
-00022020: 2764 6576 6963 655f 7479 7065 273a 2064  'device_type': d
-00022030: 6576 6963 655f 7479 7065 0a20 2020 2020  evice_type.     
-00022040: 2020 207d 0a0a 2020 2020 2020 2020 7265     }..        re
-00022050: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
-00022060: 706f 7374 2875 726c 2c20 6a73 6f6e 5f64  post(url, json_d
-00022070: 6174 613d 6a73 6f6e 5f64 6174 6129 0a0a  ata=json_data)..
-00022080: 2020 2020 6173 796e 6320 6465 6620 7265      async def re
-00022090: 6d6f 7665 5f64 6576 6963 6573 5f66 726f  move_devices_fro
-000220a0: 6d5f 7369 7465 280a 2020 2020 2020 2020  m_site(.        
-000220b0: 7365 6c66 2c0a 2020 2020 2020 2020 7369  self,.        si
-000220c0: 7465 5f69 643a 2069 6e74 2c0a 2020 2020  te_id: int,.    
-000220d0: 2020 2020 7365 7269 616c 5f6e 756d 733a      serial_nums:
-000220e0: 204c 6973 745b 7374 725d 2c0a 2020 2020   List[str],.    
-000220f0: 2020 2020 6465 7669 6365 5f74 7970 653a      device_type:
-00022100: 204c 6974 6572 616c 5b22 6170 222c 2022   Literal["ap", "
-00022110: 6378 222c 2022 7377 222c 2022 7377 6974  cx", "sw", "swit
-00022120: 6368 222c 2022 6777 225d 2c0a 2020 2020  ch", "gw"],.    
-00022130: 2920 2d3e 2052 6573 706f 6e73 653a 0a20  ) -> Response:. 
-00022140: 2020 2020 2020 2022 2222 5265 6d6f 7665         """Remove
-00022150: 2061 206c 6973 7420 6f66 2064 6576 6963   a list of devic
-00022160: 6573 2066 726f 6d20 6120 7369 7465 2e0a  es from a site..
-00022170: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00022180: 2020 2020 2020 2020 2020 2073 6974 655f             site_
-00022190: 6964 2028 696e 7429 3a20 5369 7465 2049  id (int): Site I
-000221a0: 440a 2020 2020 2020 2020 2020 2020 6465  D.            de
-000221b0: 7669 6365 5f74 7970 6520 2873 7472 293a  vice_type (str):
-000221c0: 2044 6576 6963 6520 7479 7065 2e20 5661   Device type. Va
-000221d0: 6c69 6420 5661 6c75 6573 3a20 6170 2c20  lid Values: ap, 
-000221e0: 6378 2c20 7377 2c20 7377 6974 6368 2c20  cx, sw, switch, 
-000221f0: 6777 0a20 2020 2020 2020 2020 2020 2020  gw.             
-00022200: 2020 2063 7820 616e 6420 7377 2061 7265     cx and sw are
-00022210: 2074 6865 2073 616d 6520 6173 2074 6865   the same as the
-00022220: 206d 6f72 6520 6765 6e65 7269 6320 7377   more generic sw
-00022230: 6974 6368 2e0a 2020 2020 2020 2020 2020  itch..          
-00022240: 2020 7365 7269 616c 5f6e 756d 7320 284c    serial_nums (L
-00022250: 6973 745b 7374 725d 293a 204c 6973 7420  ist[str]): List 
-00022260: 6f66 2064 6576 6963 6520 7365 7269 616c  of device serial
-00022270: 206e 756d 6265 7273 206f 6620 7468 6520   numbers of the 
-00022280: 6465 7669 6365 7320 746f 2077 6869 6368  devices to which
-00022290: 2074 6865 2073 6974 650a 2020 2020 2020   the site.      
-000222a0: 2020 2020 2020 2020 2020 6861 7320 746f            has to
-000222b0: 2062 6520 756e 2f61 7373 6f63 6961 7465   be un/associate
-000222c0: 6420 7769 7468 2e20 4120 6d61 7869 6d75  d with. A maximu
-000222d0: 6d20 6f66 2035 3030 3020 6465 7669 6365  m of 5000 device
-000222e0: 2073 6572 6961 6c73 2061 7265 2061 6c6c   serials are all
-000222f0: 6f77 6564 2061 7420 6f6e 6365 2e0a 0a20  owed at once... 
-00022300: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00022310: 2020 2020 2020 2020 2020 2020 5265 7370              Resp
-00022320: 6f6e 7365 3a20 4365 6e74 7261 6c41 5049  onse: CentralAPI
-00022330: 2052 6573 706f 6e73 6520 6f62 6a65 6374   Response object
-00022340: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00022350: 2020 2020 2064 6576 6963 655f 7479 7065       device_type
-00022360: 203d 2063 6f6e 7374 616e 7473 2e6c 6962   = constants.lib
-00022370: 5f74 6f5f 6170 6928 2273 6974 6522 2c20  _to_api("site", 
-00022380: 6465 7669 6365 5f74 7970 6529 0a20 2020  device_type).   
-00022390: 2020 2020 2069 6620 6e6f 7420 6465 7669       if not devi
-000223a0: 6365 5f74 7970 653a 0a20 2020 2020 2020  ce_type:.       
-000223b0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-000223c0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-000223d0: 2020 2020 2020 2066 2249 6e76 616c 6964         f"Invalid
-000223e0: 2056 616c 7565 2066 6f72 2064 6576 6963   Value for devic
-000223f0: 655f 7479 7065 2e20 2053 7570 706f 7274  e_type.  Support
-00022400: 6564 2056 616c 7565 733a 207b 636f 6e73  ed Values: {cons
-00022410: 7461 6e74 732e 6c69 625f 746f 5f61 7069  tants.lib_to_api
-00022420: 2e76 616c 6964 5f73 7472 7d22 0a20 2020  .valid_str}".   
-00022430: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00022440: 2020 2020 7572 6c20 3d20 222f 6365 6e74      url = "/cent
-00022450: 7261 6c2f 7632 2f73 6974 6573 2f61 7373  ral/v2/sites/ass
-00022460: 6f63 6961 7469 6f6e 7322 0a20 2020 2020  ociations".     
-00022470: 2020 2073 6572 6961 6c5f 6e75 6d73 203d     serial_nums =
-00022480: 2075 7469 6c73 2e6c 6973 7469 6679 2873   utils.listify(s
-00022490: 6572 6961 6c5f 6e75 6d73 290a 0a20 2020  erial_nums)..   
-000224a0: 2020 2020 206a 736f 6e5f 6461 7461 203d       json_data =
-000224b0: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-000224c0: 7369 7465 5f69 6427 3a20 7369 7465 5f69  site_id': site_i
-000224d0: 642c 0a20 2020 2020 2020 2020 2020 2027  d,.            '
-000224e0: 6465 7669 6365 5f69 6473 273a 2073 6572  device_ids': ser
-000224f0: 6961 6c5f 6e75 6d73 2c0a 2020 2020 2020  ial_nums,.      
-00022500: 2020 2020 2020 2764 6576 6963 655f 7479        'device_ty
-00022510: 7065 273a 2064 6576 6963 655f 7479 7065  pe': device_type
-00022520: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-00022530: 2020 2020 2320 4150 492d 464c 4157 3a20      # API-FLAW: 
-00022540: 5468 6973 206d 6574 686f 6420 7265 7475  This method retu
-00022550: 726e 7320 3230 3020 7768 656e 2066 6169  rns 200 when fai
-00022560: 6c75 7265 7320 6f63 6375 722e 0a20 2020  lures occur..   
-00022570: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
-00022580: 7420 7365 6c66 2e64 656c 6574 6528 7572  t self.delete(ur
-00022590: 6c2c 206a 736f 6e5f 6461 7461 3d6a 736f  l, json_data=jso
-000225a0: 6e5f 6461 7461 290a 0a20 2020 2061 7379  n_data)..    asy
-000225b0: 6e63 2064 6566 2063 7265 6174 655f 6c61  nc def create_la
-000225c0: 6265 6c28 0a20 2020 2020 2020 2073 656c  bel(.        sel
-000225d0: 662c 0a20 2020 2020 2020 206c 6162 656c  f,.        label
-000225e0: 5f6e 616d 653a 2073 7472 2c0a 2020 2020  _name: str,.    
-000225f0: 2020 2020 6361 7465 676f 7279 5f69 643a      category_id:
-00022600: 2069 6e74 203d 2031 2c0a 2020 2020 2920   int = 1,.    ) 
-00022610: 2d3e 2052 6573 706f 6e73 653a 0a20 2020  -> Response:.   
-00022620: 2020 2020 2022 2222 4372 6561 7465 204c       """Create L
-00022630: 6162 656c 2e0a 0a20 2020 2020 2020 2041  abel...        A
-00022640: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00022650: 206c 6162 656c 5f6e 616d 6520 2873 7472   label_name (str
-00022660: 293a 204c 6162 656c 206e 616d 650a 2020  ): Label name.  
-00022670: 2020 2020 2020 2020 2020 6361 7465 676f            catego
-00022680: 7279 5f69 6420 2869 6e74 2c20 6f70 7469  ry_id (int, opti
-00022690: 6f6e 616c 293a 204c 6162 656c 2063 6174  onal): Label cat
-000226a0: 6567 6f72 7920 4944 2064 6566 6175 6c74  egory ID default
-000226b0: 7320 746f 2031 0a20 2020 2020 2020 2020  s to 1.         
-000226c0: 2020 2020 2020 2031 203d 2064 6566 6175         1 = defau
-000226d0: 6c74 206c 6162 656c 2063 6174 6567 6f72  lt label categor
-000226e0: 792c 2032 203d 2073 6974 650a 0a20 2020  y, 2 = site..   
-000226f0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00022700: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
-00022710: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
-00022720: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
-00022730: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00022740: 2020 2075 726c 203d 2022 2f63 656e 7472     url = "/centr
-00022750: 616c 2f76 312f 6c61 6265 6c73 220a 0a20  al/v1/labels".. 
-00022760: 2020 2020 2020 206a 736f 6e5f 6461 7461         json_data
-00022770: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-00022780: 2027 6361 7465 676f 7279 5f69 6427 3a20   'category_id': 
-00022790: 6361 7465 676f 7279 5f69 642c 0a20 2020  category_id,.   
-000227a0: 2020 2020 2020 2020 2027 6c61 6265 6c5f           'label_
-000227b0: 6e61 6d65 273a 206c 6162 656c 5f6e 616d  name': label_nam
-000227c0: 650a 2020 2020 2020 2020 7d0a 0a20 2020  e.        }..   
-000227d0: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
-000227e0: 7420 7365 6c66 2e70 6f73 7428 7572 6c2c  t self.post(url,
-000227f0: 206a 736f 6e5f 6461 7461 3d6a 736f 6e5f   json_data=json_
-00022800: 6461 7461 290a 0a20 2020 2061 7379 6e63  data)..    async
-00022810: 2064 6566 2067 6574 5f6c 6162 656c 7328   def get_labels(
-00022820: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00022830: 2020 2020 2020 2063 616c 6375 6c61 7465         calculate
-00022840: 5f74 6f74 616c 3a20 626f 6f6c 203d 204e  _total: bool = N
-00022850: 6f6e 652c 0a20 2020 2020 2020 2072 6576  one,.        rev
-00022860: 6572 7365 3a20 626f 6f6c 203d 2046 616c  erse: bool = Fal
-00022870: 7365 2c0a 2020 2020 2020 2020 6f66 6673  se,.        offs
-00022880: 6574 3a20 696e 7420 3d20 302c 0a20 2020  et: int = 0,.   
-00022890: 2020 2020 206c 696d 6974 3a20 696e 7420       limit: int 
-000228a0: 3d20 3130 302c 0a20 2020 2029 202d 3e20  = 100,.    ) -> 
-000228b0: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
-000228c0: 2020 2222 224c 6973 7420 4c61 6265 6c73    """List Labels
-000228d0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-000228e0: 0a20 2020 2020 2020 2020 2020 2063 616c  .            cal
-000228f0: 6375 6c61 7465 5f74 6f74 616c 2028 626f  culate_total (bo
-00022900: 6f6c 2c20 6f70 7469 6f6e 616c 293a 2057  ol, optional): W
-00022910: 6865 7468 6572 2074 6f20 6361 6c63 756c  hether to calcul
-00022920: 6174 6520 746f 7461 6c20 4c61 6265 6c73  ate total Labels
-00022930: 0a20 2020 2020 2020 2020 2020 2072 6576  .            rev
-00022940: 6572 7365 2028 626f 6f6c 2c20 6f70 7469  erse (bool, opti
-00022950: 6f6e 616c 293a 204c 6973 7420 6c61 6265  onal): List labe
-00022960: 6c73 2069 6e20 7265 7665 7273 6520 616c  ls in reverse al
-00022970: 7068 6162 6574 6963 616c 206f 7264 6572  phabetical order
-00022980: 2e20 4465 6661 756c 7473 2074 6f20 4661  . Defaults to Fa
-00022990: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-000229a0: 6f66 6673 6574 2028 696e 742c 206f 7074  offset (int, opt
-000229b0: 696f 6e61 6c29 3a20 5061 6769 6e61 7469  ional): Paginati
-000229c0: 6f6e 206f 6666 7365 7420 4465 6661 756c  on offset Defaul
-000229d0: 7473 2074 6f20 302e 0a20 2020 2020 2020  ts to 0..       
-000229e0: 2020 2020 206c 696d 6974 2028 696e 742c       limit (int,
-000229f0: 206f 7074 696f 6e61 6c29 3a20 5061 6769   optional): Pagi
-00022a00: 6e61 7469 6f6e 206c 696d 6974 2e20 4465  nation limit. De
-00022a10: 6661 756c 7420 6973 2031 3030 2061 6e64  fault is 100 and
-00022a20: 206d 6178 2069 7320 3130 3030 2044 6566   max is 1000 Def
-00022a30: 6175 6c74 7320 746f 2031 3030 2e0a 0a20  aults to 100... 
-00022a40: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00022a50: 2020 2020 2020 2020 2020 2020 5265 7370              Resp
-00022a60: 6f6e 7365 3a20 4365 6e74 7261 6c41 5049  onse: CentralAPI
-00022a70: 2052 6573 706f 6e73 6520 6f62 6a65 6374   Response object
-00022a80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00022a90: 2020 2020 2075 726c 203d 2022 2f63 656e       url = "/cen
-00022aa0: 7472 616c 2f76 322f 6c61 6265 6c73 220a  tral/v2/labels".
-00022ab0: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-00022ac0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00022ad0: 2263 616c 6375 6c61 7465 5f74 6f74 616c  "calculate_total
-00022ae0: 223a 2063 616c 6375 6c61 7465 5f74 6f74  ": calculate_tot
-00022af0: 616c 2c0a 2020 2020 2020 2020 2020 2020  al,.            
-00022b00: 226f 6666 7365 7422 3a20 6f66 6673 6574  "offset": offset
-00022b10: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
-00022b20: 696d 6974 223a 206c 696d 6974 0a20 2020  imit": limit.   
-00022b30: 2020 2020 207d 0a20 2020 2020 2020 2069       }.        i
-00022b40: 6620 7265 7665 7273 653a 0a20 2020 2020  f reverse:.     
-00022b50: 2020 2020 2020 2070 6172 616d 735b 2273         params["s
-00022b60: 6f72 7422 5d20 3d20 222d 6c61 6265 6c5f  ort"] = "-label_
-00022b70: 6e61 6d65 220a 0a20 2020 2020 2020 2072  name"..        r
-00022b80: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-00022b90: 2e67 6574 2875 726c 2c20 7061 7261 6d73  .get(url, params
-00022ba0: 3d70 6172 616d 7329 0a0a 2020 2020 6173  =params)..    as
-00022bb0: 796e 6320 6465 6620 6173 7369 676e 5f6c  ync def assign_l
-00022bc0: 6162 656c 5f74 6f5f 6465 7669 6365 7328  abel_to_devices(
-00022bd0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00022be0: 2020 2020 2020 206c 6162 656c 5f69 643a         label_id:
-00022bf0: 2069 6e74 2c0a 2020 2020 2020 2020 6465   int,.        de
-00022c00: 7669 6365 5f74 7970 653a 2063 6f6e 7374  vice_type: const
-00022c10: 616e 7473 2e47 656e 6572 6963 4465 7654  ants.GenericDevT
-00022c20: 7970 6573 2c0a 2020 2020 2020 2020 7365  ypes,.        se
-00022c30: 7269 616c 5f6e 756d 733a 2055 6e69 6f6e  rial_nums: Union
-00022c40: 5b73 7472 2c20 4c69 7374 5b73 7472 5d5d  [str, List[str]]
-00022c50: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
-00022c60: 6e73 653a 0a20 2020 2020 2020 2022 2222  nse:.        """
-00022c70: 4173 736f 6369 6174 6520 4c61 6265 6c20  Associate Label 
-00022c80: 746f 2061 206c 6973 7420 6f66 2064 6576  to a list of dev
-00022c90: 6963 6573 2e0a 0a20 2020 2020 2020 2041  ices...        A
-00022ca0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00022cb0: 206c 6162 656c 5f69 6420 2869 6e74 293a   label_id (int):
-00022cc0: 204c 6162 656c 2049 440a 2020 2020 2020   Label ID.      
-00022cd0: 2020 2020 2020 6465 7669 6365 5f74 7970        device_typ
-00022ce0: 6520 2873 7472 293a 2044 6576 6963 6520  e (str): Device 
-00022cf0: 7479 7065 2e20 5661 6c69 6420 5661 6c75  type. Valid Valu
-00022d00: 6573 3a20 6170 2c20 6777 2c20 7377 6974  es: ap, gw, swit
-00022d10: 6368 0a20 2020 2020 2020 2020 2020 2073  ch.            s
-00022d20: 6572 6961 6c5f 6e75 6d73 2028 7374 7220  erial_nums (str 
-00022d30: 7c20 4c69 7374 5b73 7472 5d29 3a20 4c69  | List[str]): Li
-00022d40: 7374 206f 6620 6465 7669 6365 2073 6572  st of device ser
-00022d50: 6961 6c20 6e75 6d62 6572 7320 6f66 2074  ial numbers of t
-00022d60: 6865 2064 6576 6963 6573 2074 6f20 7768  he devices to wh
-00022d70: 6963 6820 7468 6520 6c61 6265 6c0a 2020  ich the label.  
-00022d80: 2020 2020 2020 2020 2020 2020 2020 6861                ha
-00022d90: 7320 746f 2062 6520 756e 2f61 7373 6f63  s to be un/assoc
-00022da0: 6961 7465 6420 7769 7468 2e20 4120 6d61  iated with. A ma
-00022db0: 7869 6d75 6d20 6f66 2035 3030 3020 6465  ximum of 5000 de
-00022dc0: 7669 6365 2073 6572 6961 6c73 2061 7265  vice serials are
-00022dd0: 2061 6c6c 6f77 6564 2061 7420 6f6e 6365   allowed at once
-00022de0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00022df0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00022e00: 5265 7370 6f6e 7365 3a20 4365 6e74 7261  Response: Centra
-00022e10: 6c41 5049 2052 6573 706f 6e73 6520 6f62  lAPI Response ob
-00022e20: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
-00022e30: 0a20 2020 2020 2020 2075 726c 203d 2022  .        url = "
-00022e40: 2f63 656e 7472 616c 2f76 322f 6c61 6265  /central/v2/labe
-00022e50: 6c73 2f61 7373 6f63 6961 7469 6f6e 7322  ls/associations"
-00022e60: 0a20 2020 2020 2020 2073 6572 6961 6c5f  .        serial_
-00022e70: 6e75 6d73 203d 2075 7469 6c73 2e6c 6973  nums = utils.lis
-00022e80: 7469 6679 2873 6572 6961 6c5f 6e75 6d73  tify(serial_nums
-00022e90: 290a 2020 2020 2020 2020 6465 7669 6365  ).        device
-00022ea0: 5f74 7970 6520 3d20 636f 6e73 7461 6e74  _type = constant
-00022eb0: 732e 6c69 625f 746f 5f61 7069 2822 7369  s.lib_to_api("si
-00022ec0: 7465 222c 2064 6576 6963 655f 7479 7065  te", device_type
-00022ed0: 290a 0a20 2020 2020 2020 206a 736f 6e5f  )..        json_
-00022ee0: 6461 7461 203d 207b 0a20 2020 2020 2020  data = {.       
-00022ef0: 2020 2020 2027 6c61 6265 6c5f 6964 273a       'label_id':
-00022f00: 206c 6162 656c 5f69 642c 0a20 2020 2020   label_id,.     
-00022f10: 2020 2020 2020 2027 6465 7669 6365 5f74         'device_t
-00022f20: 7970 6527 3a20 6465 7669 6365 5f74 7970  ype': device_typ
-00022f30: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
-00022f40: 6465 7669 6365 5f69 6473 273a 2073 6572  device_ids': ser
-00022f50: 6961 6c5f 6e75 6d73 0a20 2020 2020 2020  ial_nums.       
-00022f60: 207d 0a0a 2020 2020 2020 2020 7265 7475   }..        retu
-00022f70: 726e 2061 7761 6974 2073 656c 662e 706f  rn await self.po
-00022f80: 7374 2875 726c 2c20 6a73 6f6e 5f64 6174  st(url, json_dat
-00022f90: 613d 6a73 6f6e 5f64 6174 6129 0a0a 2020  a=json_data)..  
-00022fa0: 2020 2320 544f 444f 206d 616b 6520 666f    # TODO make fo
-00022fb0: 726d 6174 206f 6620 7468 6973 2061 6e64  rmat of this and
-00022fc0: 206f 7468 6572 206c 6162 656c 206d 6574   other label met
-00022fd0: 686f 6473 206d 6174 6368 2073 6974 6520  hods match site 
-00022fe0: 6d65 7468 6f64 730a 2020 2020 6173 796e  methods.    asyn
-00022ff0: 6320 6465 6620 7265 6d6f 7665 5f6c 6162  c def remove_lab
-00023000: 656c 5f66 726f 6d5f 6465 7669 6365 7328  el_from_devices(
-00023010: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00023020: 2020 2020 2020 206c 6162 656c 5f69 643a         label_id:
-00023030: 2069 6e74 2c0a 2020 2020 2020 2020 6465   int,.        de
-00023040: 7669 6365 5f74 7970 653a 2073 7472 2c0a  vice_type: str,.
-00023050: 2020 2020 2020 2020 7365 7269 616c 5f6e          serial_n
-00023060: 756d 733a 204c 6973 745b 7374 725d 2c0a  ums: List[str],.
-00023070: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
-00023080: 653a 0a20 2020 2020 2020 2022 2222 756e  e:.        """un
-00023090: 6173 7369 676e 2061 206c 6162 656c 2066  assign a label f
-000230a0: 726f 6d20 6120 6c69 7374 206f 6620 6465  rom a list of de
-000230b0: 7669 6365 732e 0a0a 2020 2020 2020 2020  vices...        
-000230c0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-000230d0: 2020 6c61 6265 6c5f 6964 2028 696e 7429    label_id (int)
-000230e0: 3a20 4c61 6265 6c20 4944 0a20 2020 2020  : Label ID.     
-000230f0: 2020 2020 2020 2064 6576 6963 655f 7479         device_ty
-00023100: 7065 2028 7374 7229 3a20 4465 7669 6365  pe (str): Device
-00023110: 2074 7970 652e 204f 6e65 206f 6620 6170   type. One of ap
-00023120: 2c20 6777 2c20 7377 6974 6368 0a20 2020  , gw, switch.   
-00023130: 2020 2020 2020 2020 2073 6572 6961 6c5f           serial_
-00023140: 6e75 6d73 2028 7374 7220 7c20 4c69 7374  nums (str | List
-00023150: 5b73 7472 5d29 3a20 4c69 7374 206f 6620  [str]): List of 
-00023160: 6465 7669 6365 2073 6572 6961 6c20 6e75  device serial nu
-00023170: 6d62 6572 7320 6f66 2074 6865 2064 6576  mbers of the dev
-00023180: 6963 6573 2074 6f20 7768 6963 6820 7468  ices to which th
-00023190: 6520 6c61 6265 6c0a 2020 2020 2020 2020  e label.        
-000231a0: 2020 2020 2020 2020 6861 7320 746f 2062          has to b
-000231b0: 6520 756e 2f61 7373 6f63 6961 7465 6420  e un/associated 
-000231c0: 7769 7468 2e20 4120 6d61 7869 6d75 6d20  with. A maximum 
-000231d0: 6f66 2035 3030 3020 6465 7669 6365 2073  of 5000 device s
-000231e0: 6572 6961 6c73 2061 7265 2061 6c6c 6f77  erials are allow
-000231f0: 6564 2061 7420 6f6e 6365 2e0a 0a20 2020  ed at once...   
-00023200: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00023210: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
-00023220: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
-00023230: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
-00023240: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00023250: 2020 2075 726c 203d 2022 2f63 656e 7472     url = "/centr
-00023260: 616c 2f76 322f 6c61 6265 6c73 2f61 7373  al/v2/labels/ass
-00023270: 6f63 6961 7469 6f6e 7322 0a20 2020 2020  ociations".     
-00023280: 2020 2073 6572 6961 6c5f 6e75 6d73 203d     serial_nums =
-00023290: 2075 7469 6c73 2e6c 6973 7469 6679 2873   utils.listify(s
-000232a0: 6572 6961 6c5f 6e75 6d73 290a 2020 2020  erial_nums).    
-000232b0: 2020 2020 6465 7669 6365 5f74 7970 6520      device_type 
-000232c0: 3d20 636f 6e73 7461 6e74 732e 6c69 625f  = constants.lib_
-000232d0: 746f 5f61 7069 2822 7369 7465 222c 2064  to_api("site", d
-000232e0: 6576 6963 655f 7479 7065 290a 0a20 2020  evice_type)..   
-000232f0: 2020 2020 206a 736f 6e5f 6461 7461 203d       json_data =
-00023300: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-00023310: 6c61 6265 6c5f 6964 273a 206c 6162 656c  label_id': label
-00023320: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-00023330: 2027 6465 7669 6365 5f74 7970 6527 3a20   'device_type': 
-00023340: 6465 7669 6365 5f74 7970 652c 0a20 2020  device_type,.   
-00023350: 2020 2020 2020 2020 2027 6465 7669 6365           'device
-00023360: 5f69 6473 273a 2073 6572 6961 6c5f 6e75  _ids': serial_nu
-00023370: 6d73 0a20 2020 2020 2020 207d 0a0a 2020  ms.        }..  
-00023380: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-00023390: 6974 2073 656c 662e 6465 6c65 7465 2875  it self.delete(u
-000233a0: 726c 2c20 6a73 6f6e 5f64 6174 613d 6a73  rl, json_data=js
-000233b0: 6f6e 5f64 6174 6129 0a0a 2020 2020 2320  on_data)..    # 
-000233c0: 4150 492d 464c 4157 2072 6574 7572 6e73  API-FLAW returns
-000233d0: 2065 6d70 7479 2070 6179 6c6f 6164 202f   empty payload /
-000233e0: 2072 6573 706f 6e73 6520 6f6e 2073 7563   response on suc
-000233f0: 6365 7373 2032 3030 0a20 2020 2061 7379  cess 200.    asy
-00023400: 6e63 2064 6566 2064 656c 6574 655f 6c61  nc def delete_la
-00023410: 6265 6c28 0a20 2020 2020 2020 2073 656c  bel(.        sel
-00023420: 662c 0a20 2020 2020 2020 206c 6162 656c  f,.        label
-00023430: 5f69 643a 2069 6e74 2c0a 2020 2020 2920  _id: int,.    ) 
-00023440: 2d3e 2052 6573 706f 6e73 653a 0a20 2020  -> Response:.   
-00023450: 2020 2020 2022 2222 4465 6c65 7465 204c       """Delete L
-00023460: 6162 656c 2e0a 0a20 2020 2020 2020 2041  abel...        A
-00023470: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00023480: 206c 6162 656c 5f69 6420 2869 6e74 293a   label_id (int):
-00023490: 204c 6162 656c 2049 440a 0a20 2020 2020   Label ID..     
-000234a0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-000234b0: 2020 2020 2020 2020 5265 7370 6f6e 7365          Response
-000234c0: 3a20 4365 6e74 7261 6c41 5049 2052 6573  : CentralAPI Res
-000234d0: 706f 6e73 6520 6f62 6a65 6374 0a20 2020  ponse object.   
-000234e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000234f0: 2075 726c 203d 2066 222f 6365 6e74 7261   url = f"/centra
-00023500: 6c2f 7631 2f6c 6162 656c 732f 7b6c 6162  l/v1/labels/{lab
-00023510: 656c 5f69 647d 220a 0a20 2020 2020 2020  el_id}"..       
-00023520: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-00023530: 6c66 2e64 656c 6574 6528 7572 6c29 0a0a  lf.delete(url)..
-00023540: 2020 2020 6173 796e 6320 6465 6620 6765      async def ge
-00023550: 745f 6465 7669 6365 5f69 705f 726f 7574  t_device_ip_rout
-00023560: 6573 280a 2020 2020 2020 2020 7365 6c66  es(.        self
-00023570: 2c0a 2020 2020 2020 2020 7365 7269 616c  ,.        serial
-00023580: 5f6e 756d 3a20 7374 722c 0a20 2020 2020  _num: str,.     
-00023590: 2020 2061 7069 3a20 7374 7220 3d20 2256     api: str = "V
-000235a0: 3122 2c0a 2020 2020 2020 2020 6f66 6673  1",.        offs
-000235b0: 6574 3a20 696e 7420 3d20 302c 0a20 2020  et: int = 0,.   
-000235c0: 2020 2020 206c 696d 6974 3a20 696e 7420       limit: int 
-000235d0: 3d20 3130 300a 2020 2020 2920 2d3e 2052  = 100.    ) -> R
-000235e0: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
-000235f0: 2022 2222 4765 7420 726f 7574 6573 2066   """Get routes f
-00023600: 6f72 2061 2064 6576 6963 652e 0a0a 2020  or a device...  
-00023610: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00023620: 2020 2020 2020 2020 7365 7269 616c 5f6e          serial_n
-00023630: 756d 2028 7374 7229 3a20 4465 7669 6365  um (str): Device
-00023640: 2073 6572 6961 6c20 6e75 6d62 6572 0a20   serial number. 
-00023650: 2020 2020 2020 2020 2020 2061 7069 2028             api (
-00023660: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
-00023670: 4150 4920 7665 7273 696f 6e20 2856 307c  API version (V0|
-00023680: 5631 292c 2044 6566 6175 6c74 7320 746f  V1), Defaults to
-00023690: 2056 312e 0a20 2020 2020 2020 2020 2020   V1..           
-000236a0: 206f 6666 7365 7420 2873 7472 2c20 6f70   offset (str, op
-000236b0: 7469 6f6e 616c 293a 2050 6167 696e 6174  tional): Paginat
-000236c0: 696f 6e20 6f66 6673 6574 2e0a 2020 2020  ion offset..    
-000236d0: 2020 2020 2020 2020 6c69 6d69 7420 2869          limit (i
-000236e0: 6e74 2c20 6f70 7469 6f6e 616c 293a 2070  nt, optional): p
-000236f0: 6167 6520 7369 7a65 2044 6566 6175 6c74  age size Default
-00023700: 7320 746f 2031 3030 2e0a 0a20 2020 2020  s to 100...     
-00023710: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00023720: 2020 2020 2020 2020 5265 7370 6f6e 7365          Response
-00023730: 3a20 4365 6e74 7261 6c41 5049 2052 6573  : CentralAPI Res
-00023740: 706f 6e73 6520 6f62 6a65 6374 0a20 2020  ponse object.   
-00023750: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00023760: 2075 726c 203d 2022 2f61 7069 2f72 6f75   url = "/api/rou
-00023770: 7469 6e67 2f76 312f 726f 7574 6522 0a0a  ting/v1/route"..
-00023780: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
-00023790: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-000237a0: 6465 7669 6365 273a 2073 6572 6961 6c5f  device': serial_
-000237b0: 6e75 6d2c 0a20 2020 2020 2020 2020 2020  num,.           
-000237c0: 2027 6170 6927 3a20 6170 692c 0a20 2020   'api': api,.   
-000237d0: 2020 2020 2020 2020 2027 6d61 726b 6572           'marker
-000237e0: 273a 206f 6666 7365 742c 0a20 2020 2020  ': offset,.     
-000237f0: 2020 2020 2020 2027 6c69 6d69 7427 3a20         'limit': 
-00023800: 6c69 6d69 740a 2020 2020 2020 2020 7d0a  limit.        }.
-00023810: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00023820: 6177 6169 7420 7365 6c66 2e67 6574 2875  await self.get(u
-00023830: 726c 2c20 7061 7261 6d73 3d70 6172 616d  rl, params=param
-00023840: 7329 0a0a 2020 2020 2320 544f 444f 206d  s)..    # TODO m
-00023850: 616b 6520 6164 645f 6465 7669 6365 2061  ake add_device a
-00023860: 6374 7561 6c20 6675 6e63 2073 6570 2061  ctual func sep a
-00023870: 6e64 206d 616b 6520 7468 6973 2061 6e20  nd make this an 
-00023880: 6167 6772 6567 6174 6f72 2074 6861 7420  aggregator that 
-00023890: 6361 6c6c 7320 6974 2061 6e64 2061 6e79  calls it and any
-000238a0: 7468 696e 6720 656c 7365 2062 6173 6564  thing else based
-000238b0: 206f 6e20 7061 7261 6d73 0a20 2020 2061   on params.    a
-000238c0: 7379 6e63 2064 6566 2061 6464 5f64 6576  sync def add_dev
-000238d0: 6963 6573 280a 2020 2020 2020 2020 7365  ices(.        se
-000238e0: 6c66 2c0a 2020 2020 2020 2020 6d61 635f  lf,.        mac_
-000238f0: 6164 6472 6573 733a 2073 7472 203d 204e  address: str = N
-00023900: 6f6e 652c 0a20 2020 2020 2020 2073 6572  one,.        ser
-00023910: 6961 6c5f 6e75 6d3a 2073 7472 203d 204e  ial_num: str = N
-00023920: 6f6e 652c 0a20 2020 2020 2020 2067 726f  one,.        gro
-00023930: 7570 3a20 7374 7220 3d20 4e6f 6e65 2c0a  up: str = None,.
-00023940: 2020 2020 2020 2020 2320 7369 7465 3a20          # site: 
-00023950: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-00023960: 2020 2020 7061 7274 5f6e 756d 3a20 7374      part_num: st
-00023970: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00023980: 2020 6c69 6365 6e73 653a 2055 6e69 6f6e    license: Union
-00023990: 5b73 7472 2c20 4c69 7374 5b73 7472 5d5d  [str, List[str]]
-000239a0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000239b0: 2064 6576 6963 655f 6c69 7374 3a20 4c69   device_list: Li
-000239c0: 7374 5b44 6963 745b 7374 722c 2073 7472  st[Dict[str, str
-000239d0: 5d5d 203d 204e 6f6e 650a 2020 2020 2920  ]] = None.    ) 
-000239e0: 2d3e 2055 6e69 6f6e 5b52 6573 706f 6e73  -> Union[Respons
-000239f0: 652c 204c 6973 745b 5265 7370 6f6e 7365  e, List[Response
-00023a00: 5d5d 3a0a 2020 2020 2020 2020 2222 2241  ]]:.        """A
-00023a10: 6464 2064 6576 6963 6528 7329 2075 7369  dd device(s) usi
-00023a20: 6e67 204d 6163 2061 6e64 2053 6572 6961  ng Mac and Seria
-00023a30: 6c20 6e75 6d62 6572 2028 7061 7274 5f6e  l number (part_n
-00023a40: 756d 2061 6c73 6f20 7265 7175 6972 6564  um also required
-00023a50: 2066 6f72 2043 6f50 290a 2020 2020 2020   for CoP).      
-00023a60: 2020 5769 6c6c 2061 6c73 6f20 7072 652d    Will also pre-
-00023a70: 6173 7369 676e 2064 6576 6963 6520 746f  assign device to
-00023a80: 2067 726f 7570 2069 6620 7072 6f76 6964   group if provid
-00023a90: 6564 0a0a 2020 2020 2020 2020 4569 7468  ed..        Eith
-00023aa0: 6572 206d 6163 5f61 6464 7265 7373 2061  er mac_address a
-00023ab0: 6e64 2073 6572 6961 6c5f 6e75 6d20 6f72  nd serial_num or
-00023ac0: 2064 6576 6963 655f 6c69 7374 2028 7768   device_list (wh
-00023ad0: 6963 6820 7368 6f75 6c64 2063 6f6e 7461  ich should conta
-00023ae0: 696e 2061 2064 6963 7420 7769 7468 206d  in a dict with m
-00023af0: 6163 2073 6572 6961 6c29 2061 7265 2072  ac serial) are r
-00023b00: 6571 7569 7265 642e 0a20 2020 2020 2020  equired..       
-00023b10: 202f 2f20 5573 6564 2062 7920 6164 6420   // Used by add 
-00023b20: 6465 7669 6365 2061 6e64 2062 6174 6368  device and batch
-00023b30: 2061 6464 2064 6576 6963 6573 202f 2f0a   add devices //.
-00023b40: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00023b50: 2020 2020 2020 2020 2020 206d 6163 5f61             mac_a
-00023b60: 6464 7265 7373 2028 7374 722c 206f 7074  ddress (str, opt
-00023b70: 696f 6e61 6c29 3a20 4d41 4320 6164 6472  ional): MAC addr
-00023b80: 6573 7320 6f66 2064 6576 6963 6520 746f  ess of device to
-00023b90: 2062 6520 6164 6465 640a 2020 2020 2020   be added.      
-00023ba0: 2020 2020 2020 7365 7269 616c 5f6e 756d        serial_num
-00023bb0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-00023bc0: 3a20 5365 7269 616c 206e 756d 6265 7220  : Serial number 
-00023bd0: 6f66 2064 6576 6963 6520 746f 2062 6520  of device to be 
-00023be0: 6164 6465 640a 2020 2020 2020 2020 2020  added.          
-00023bf0: 2020 6772 6f75 7020 2873 7472 2c20 6f70    group (str, op
-00023c00: 7469 6f6e 616c 293a 2041 6464 2064 6576  tional): Add dev
-00023c10: 6963 6520 746f 2070 7265 2d70 726f 7669  ice to pre-provi
-00023c20: 7369 6f6e 6564 2067 726f 7570 2028 6164  sioned group (ad
-00023c30: 6469 7469 6f6e 616c 2041 5049 2063 616c  ditional API cal
-00023c40: 6c20 6973 206d 6164 6529 0a20 2020 2020  l is made).     
-00023c50: 2020 2020 2020 2073 6974 6520 2869 6e74         site (int
-00023c60: 2c20 6f70 7469 6f6e 616c 293a 202d 2d20  , optional): -- 
-00023c70: 4e6f 7420 696d 706c 656d 656e 7465 6420  Not implemented 
-00023c80: 2d2d 2053 6974 6520 4944 0a20 2020 2020  -- Site ID.     
-00023c90: 2020 2020 2020 2070 6172 745f 6e75 6d20         part_num 
-00023ca0: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
-00023cb0: 2050 6172 7420 4e75 6d62 6572 2069 7320   Part Number is 
-00023cc0: 7265 7175 6972 6564 2066 6f72 2043 656e  required for Cen
-00023cd0: 7472 616c 204f 6e20 5072 656d 2e0a 2020  tral On Prem..  
-00023ce0: 2020 2020 2020 2020 2020 6c69 6365 6e73            licens
-00023cf0: 6520 2873 7472 7c4c 6973 7428 7374 7229  e (str|List(str)
-00023d00: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-00023d10: 2073 7562 7363 7269 7074 696f 6e20 6c69   subscription li
-00023d20: 6365 6e73 6528 7329 2074 6f20 6173 7369  cense(s) to assi
-00023d30: 676e 2e0a 2020 2020 2020 2020 2020 2020  gn..            
-00023d40: 6465 7669 6365 5f6c 6973 7420 284c 6973  device_list (Lis
-00023d50: 745b 4469 6374 5b73 7472 2c20 7374 725d  t[Dict[str, str]
-00023d60: 5d2c 206f 7074 696f 6e61 6c29 3a20 4c69  ], optional): Li
-00023d70: 7374 206f 6620 6469 6374 7320 7769 7468  st of dicts with
-00023d80: 206d 6163 2c20 7365 7269 616c 2066 6f72   mac, serial for
-00023d90: 2065 6163 6820 6465 7669 6365 0a20 2020   each device.   
-00023da0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-00023db0: 206f 7074 696f 6e61 6c6c 7920 6772 6f75   optionally grou
-00023dc0: 702c 2070 6172 745f 6e75 6d2c 206c 6963  p, part_num, lic
-00023dd0: 656e 7365 2c0a 0a20 2020 2020 2020 2052  ense,..        R
-00023de0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00023df0: 2020 2020 5265 7370 6f6e 7365 3a20 4365      Response: Ce
-00023e00: 6e74 7261 6c41 5049 2052 6573 706f 6e73  ntralAPI Respons
-00023e10: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
-00023e20: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
-00023e30: 203d 2022 2f70 6c61 7466 6f72 6d2f 6465   = "/platform/de
-00023e40: 7669 6365 5f69 6e76 656e 746f 7279 2f76  vice_inventory/v
-00023e50: 312f 6465 7669 6365 7322 0a20 2020 2020  1/devices".     
-00023e60: 2020 206c 6963 656e 7365 5f6b 7761 7267     license_kwarg
-00023e70: 7320 3d20 5b5d 0a0a 2020 2020 2020 2020  s = []..        
-00023e80: 6966 206c 6963 656e 7365 3a0a 2020 2020  if license:.    
-00023e90: 2020 2020 2020 2020 6c69 6365 6e73 655f          license_
-00023ea0: 6b77 6172 6773 203d 205b 7b22 7365 7269  kwargs = [{"seri
-00023eb0: 616c 7322 3a20 5b73 6572 6961 6c5f 6e75  als": [serial_nu
-00023ec0: 6d5d 2c20 2273 6572 7669 6365 7322 3a20  m], "services": 
-00023ed0: 7574 696c 732e 6c69 7374 6966 7928 6c69  utils.listify(li
-00023ee0: 6365 6e73 6529 7d5d 0a20 2020 2020 2020  cense)}].       
-00023ef0: 2069 6620 7365 7269 616c 5f6e 756d 2061   if serial_num a
-00023f00: 6e64 206d 6163 5f61 6464 7265 7373 3a0a  nd mac_address:.
-00023f10: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-00023f20: 6576 6963 655f 6c69 7374 3a0a 2020 2020  evice_list:.    
-00023f30: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00023f40: 6520 5661 6c75 6545 7272 6f72 2822 7365  e ValueError("se
-00023f50: 7269 616c 5f6e 756d 2061 6e64 206d 6163  rial_num and mac
-00023f60: 5f61 6464 7265 7373 2061 7265 206e 6f74  _address are not
-00023f70: 2065 7870 6563 7465 6420 7768 656e 2064   expected when d
-00023f80: 6576 6963 655f 6c69 7374 2069 7320 6265  evice_list is be
-00023f90: 696e 6720 7072 6f76 6964 6564 2e22 290a  ing provided.").
-00023fa0: 0a20 2020 2020 2020 2020 2020 2074 6f5f  .            to_
-00023fb0: 6772 6f75 7020 3d20 4e6f 6e65 2069 6620  group = None if 
-00023fc0: 6e6f 7420 6772 6f75 7020 656c 7365 207b  not group else {
-00023fd0: 6772 6f75 703a 205b 7365 7269 616c 5f6e  group: [serial_n
-00023fe0: 756d 5d7d 0a20 2020 2020 2020 2020 2020  um]}.           
-00023ff0: 2023 2074 6f5f 7369 7465 203d 204e 6f6e   # to_site = Non
-00024000: 6520 6966 206e 6f74 2073 6974 6520 656c  e if not site el
-00024010: 7365 207b 7369 7465 3a20 5b73 6572 6961  se {site: [seria
-00024020: 6c5f 6e75 6d5d 7d0a 0a20 2020 2020 2020  l_num]}..       
-00024030: 2020 2020 206d 6163 203d 2075 7469 6c73       mac = utils
-00024040: 2e4d 6163 286d 6163 5f61 6464 7265 7373  .Mac(mac_address
-00024050: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00024060: 206e 6f74 206d 6163 3a0a 2020 2020 2020   not mac:.      
-00024070: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00024080: 5661 6c75 6545 7272 6f72 2866 226d 6163  ValueError(f"mac
-00024090: 5f61 6464 7265 7373 207b 6d61 635f 6164  _address {mac_ad
-000240a0: 6472 6573 737d 2061 7070 6561 7273 2074  dress} appears t
-000240b0: 6f20 6265 2069 6e76 616c 6964 2e22 290a  o be invalid.").
-000240c0: 0a20 2020 2020 2020 2020 2020 206a 736f  .            jso
-000240d0: 6e5f 6461 7461 203d 205b 0a20 2020 2020  n_data = [.     
-000240e0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-000240f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024100: 2022 6d61 6322 3a20 6d61 632e 636f 6c73   "mac": mac.cols
-00024110: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00024120: 2020 2020 2020 2273 6572 6961 6c22 3a20        "serial": 
-00024130: 7365 7269 616c 5f6e 756d 0a20 2020 2020  serial_num.     
-00024140: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00024150: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00024160: 2020 2020 2020 2069 6620 7061 7274 5f6e         if part_n
-00024170: 756d 3a0a 2020 2020 2020 2020 2020 2020  um:.            
-00024180: 2020 2020 6a73 6f6e 5f64 6174 615b 305d      json_data[0]
-00024190: 5b22 7061 7274 4e75 6d62 6572 225d 203d  ["partNumber"] =
-000241a0: 2070 6172 745f 6e75 6d0a 0a20 2020 2020   part_num..     
-000241b0: 2020 2065 6c69 6620 6465 7669 6365 5f6c     elif device_l
-000241c0: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
-000241d0: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-000241e0: 6365 2864 6576 6963 655f 6c69 7374 2c20  ce(device_list, 
-000241f0: 6c69 7374 2920 616e 6420 6e6f 7420 616c  list) and not al
-00024200: 6c28 6973 696e 7374 616e 6365 2864 2c20  l(isinstance(d, 
-00024210: 6469 6374 2920 666f 7220 6420 696e 2064  dict) for d in d
-00024220: 6576 6963 655f 6c69 7374 293a 0a20 2020  evice_list):.   
-00024230: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00024240: 7365 2056 616c 7565 4572 726f 7228 2257  se ValueError("W
-00024250: 6865 6e20 7573 696e 6720 6465 7669 6365  hen using device
-00024260: 5f6c 6973 7420 746f 2062 6174 6368 2061  _list to batch a
-00024270: 6464 2064 6576 6963 6573 2c20 7468 6579  dd devices, they
-00024280: 2073 686f 756c 6420 6265 2070 726f 7669   should be provi
-00024290: 6465 6420 6173 2061 206c 6973 7420 6f66  ded as a list of
-000242a0: 2064 6963 7473 2229 0a0a 2020 2020 2020   dicts")..      
-000242b0: 2020 2020 2020 5f6b 6579 7320 3d20 7b0a        _keys = {.
-000242c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000242d0: 226d 6163 5f61 6464 7265 7373 223a 2022  "mac_address": "
-000242e0: 6d61 6322 2c0a 2020 2020 2020 2020 2020  mac",.          
-000242f0: 2020 2020 2020 2273 6572 6961 6c5f 6e75        "serial_nu
-00024300: 6d22 3a20 2273 6572 6961 6c22 2c0a 2020  m": "serial",.  
-00024310: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00024320: 6172 745f 6e75 6d22 3a20 2270 6172 744e  art_num": "partN
-00024330: 756d 6265 7222 0a20 2020 2020 2020 2020  umber".         
-00024340: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
-00024350: 2020 6a73 6f6e 5f64 6174 6120 3d20 5b5d    json_data = []
-00024360: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00024370: 2064 2069 6e20 6465 7669 6365 5f6c 6973   d in device_lis
-00024380: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00024390: 2020 206d 6163 203d 2064 2e67 6574 2822     mac = d.get("
-000243a0: 6d61 6322 2c20 642e 6765 7428 226d 6163  mac", d.get("mac
-000243b0: 5f61 6464 7265 7373 2229 290a 2020 2020  _address")).    
-000243c0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-000243d0: 6f74 206d 6163 3a0a 2020 2020 2020 2020  ot mac:.        
-000243e0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000243f0: 6520 5661 6c75 6545 7272 6f72 2866 224e  e ValueError(f"N
-00024400: 6f20 4d61 6320 4164 6472 6573 7320 666f  o Mac Address fo
-00024410: 756e 6420 666f 7220 656e 7472 7920 7b64  und for entry {d
-00024420: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-00024430: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00024440: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00024450: 6320 3d20 7574 696c 732e 4d61 6328 6d61  c = utils.Mac(ma
-00024460: 6329 0a20 2020 2020 2020 2020 2020 2020  c).             
-00024470: 2020 2020 2020 2069 6620 6e6f 7420 6d61         if not ma
-00024480: 633a 0a20 2020 2020 2020 2020 2020 2020  c:.             
-00024490: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000244a0: 2056 616c 7565 4572 726f 7228 6622 4d61   ValueError(f"Ma
-000244b0: 6320 4164 6472 6573 7320 7b6d 6163 7d20  c Address {mac} 
-000244c0: 6170 7065 6172 7320 746f 2062 6520 696e  appears to be in
-000244d0: 7661 6c69 642e 2229 0a20 2020 2020 2020  valid.").       
-000244e0: 2020 2020 2020 2020 2073 6572 6961 6c20           serial 
-000244f0: 3d20 642e 6765 7428 2273 6572 6961 6c22  = d.get("serial"
-00024500: 2c20 642e 6765 7428 2273 6572 6961 6c5f  , d.get("serial_
-00024510: 6e75 6d22 2929 0a20 2020 2020 2020 2020  num")).         
-00024520: 2020 2020 2020 205f 7468 6973 5f64 6963         _this_dic
-00024530: 7420 3d20 7b22 6d61 6322 3a20 6d61 632e  t = {"mac": mac.
-00024540: 636f 6c73 2c20 2273 6572 6961 6c22 3a20  cols, "serial": 
-00024550: 7365 7269 616c 7d0a 2020 2020 2020 2020  serial}.        
-00024560: 2020 2020 2020 2020 7061 7274 5f6e 756d          part_num
-00024570: 203d 2064 2e67 6574 2822 7061 7274 5f6e   = d.get("part_n
-00024580: 756d 222c 2064 2e67 6574 2822 7061 7274  um", d.get("part
-00024590: 4e75 6d62 6572 2229 290a 2020 2020 2020  Number")).      
-000245a0: 2020 2020 2020 2020 2020 6966 2070 6172            if par
-000245b0: 745f 6e75 6d3a 0a20 2020 2020 2020 2020  t_num:.         
-000245c0: 2020 2020 2020 2020 2020 205f 7468 6973             _this
-000245d0: 5f64 6963 745b 2270 6172 744e 756d 6265  _dict["partNumbe
-000245e0: 7222 5d20 3d20 7061 7274 5f6e 756d 0a0a  r"] = part_num..
-000245f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024600: 6a73 6f6e 5f64 6174 6120 2b3d 205b 5f74  json_data += [_t
-00024610: 6869 735f 6469 6374 5d0a 0a20 2020 2020  his_dict]..     
-00024620: 2020 2020 2020 2074 6f5f 6772 6f75 7020         to_group 
-00024630: 3d20 7b64 2e67 6574 2822 6772 6f75 7022  = {d.get("group"
-00024640: 293a 205b 5d20 666f 7220 6420 696e 2064  ): [] for d in d
-00024650: 6576 6963 655f 6c69 7374 2069 6620 2267  evice_list if "g
-00024660: 726f 7570 2220 696e 2064 7d0a 2020 2020  roup" in d}.    
-00024670: 2020 2020 2020 2020 666f 7220 6420 696e          for d in
-00024680: 2064 6576 6963 655f 6c69 7374 3a0a 2020   device_list:.  
-00024690: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000246a0: 2022 6772 6f75 7022 2069 6e20 643a 0a20   "group" in d:. 
-000246b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000246c0: 2020 2074 6f5f 6772 6f75 705b 645b 2267     to_group[d["g
-000246d0: 726f 7570 225d 5d2e 6170 7065 6e64 2864  roup"]].append(d
-000246e0: 2e67 6574 2822 7365 7269 616c 5f6e 756d  .get("serial_num
-000246f0: 222c 2064 2e67 6574 2822 7365 7269 616c  ", d.get("serial
-00024700: 2229 2929 0a0a 2020 2020 2020 2020 2020  ")))..          
-00024710: 2020 2320 746f 5f73 6974 6520 3d20 7b64    # to_site = {d
-00024720: 2e67 6574 2822 7369 7465 2229 3a20 5b5d  .get("site"): []
-00024730: 2066 6f72 2064 2069 6e20 6465 7669 6365   for d in device
-00024740: 5f6c 6973 7420 6966 2022 7369 7465 2220  _list if "site" 
-00024750: 696e 2064 7d0a 2020 2020 2020 2020 2020  in d}.          
-00024760: 2020 2320 666f 7220 6420 696e 2064 6576    # for d in dev
-00024770: 6963 655f 6c69 7374 3a0a 2020 2020 2020  ice_list:.      
-00024780: 2020 2020 2020 2320 2020 2020 6966 2022        #     if "
-00024790: 7369 7465 2220 696e 2064 3a0a 2020 2020  site" in d:.    
-000247a0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-000247b0: 2020 746f 5f73 6974 655b 645b 2273 6974    to_site[d["sit
-000247c0: 6522 5d5d 2e61 7070 656e 6428 642e 6765  e"]].append(d.ge
-000247d0: 7428 2273 6572 6961 6c5f 6e75 6d22 2c20  t("serial_num", 
-000247e0: 642e 6765 7428 2273 6572 6961 6c22 2929  d.get("serial"))
-000247f0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00024800: 2047 6174 6865 7220 616c 6c20 7365 7269   Gather all seri
-00024810: 616c 7320 666f 7220 6561 6368 206c 6963  als for each lic
-00024820: 656e 7365 2063 6f6d 6269 6e61 7469 6f6e  ense combination
-00024830: 2066 726f 6d20 6465 7669 6365 5f6c 6973   from device_lis
-00024840: 740a 2020 2020 2020 2020 2020 2020 2320  t.            # 
-00024850: 544f 444f 2074 6869 7320 6e65 6564 7320  TODO this needs 
-00024860: 746f 2062 6520 7465 7374 6564 0a20 2020  to be tested.   
-00024870: 2020 2020 2020 2020 205f 6c69 635f 6b77           _lic_kw
-00024880: 6172 6773 203d 207b 7d0a 2020 2020 2020  args = {}.      
-00024890: 2020 2020 2020 666f 7220 6420 696e 2064        for d in d
-000248a0: 6576 6963 655f 6c69 7374 3a0a 2020 2020  evice_list:.    
-000248b0: 2020 2020 2020 2020 2020 2020 6966 2022              if "
-000248c0: 6c69 6365 6e73 6522 206e 6f74 2069 6e20  license" not in 
-000248d0: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
-000248e0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-000248f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024900: 2064 5b22 6c69 6365 6e73 6522 5d20 3d20   d["license"] = 
-00024910: 7574 696c 732e 6c69 7374 6966 7928 645b  utils.listify(d[
-00024920: 226c 6963 656e 7365 225d 290a 2020 2020  "license"]).    
-00024930: 2020 2020 2020 2020 2020 2020 5f6b 6579              _key
-00024940: 203d 2066 227b 645b 276c 6963 656e 7365   = f"{d['license
-00024950: 275d 2069 6620 6c65 6e28 645b 276c 6963  '] if len(d['lic
-00024960: 656e 7365 275d 2920 3d3d 2031 2065 6c73  ense']) == 1 els
-00024970: 6520 277c 272e 6a6f 696e 2873 6f72 7465  e '|'.join(sorte
-00024980: 6428 645b 276c 6963 656e 7365 275d 2929  d(d['license']))
-00024990: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-000249a0: 2020 205f 7365 7269 616c 203d 2064 2e67     _serial = d.g
-000249b0: 6574 2822 7365 7269 616c 5f6e 756d 222c  et("serial_num",
-000249c0: 2064 2e67 6574 2822 7365 7269 616c 2229   d.get("serial")
-000249d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000249e0: 2020 6966 206e 6f74 205f 7365 7269 616c    if not _serial
-000249f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00024a00: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00024a10: 6545 7272 6f72 2866 224e 6f20 7365 7269  eError(f"No seri
-00024a20: 616c 2066 6f75 6e64 2066 6f72 2064 6576  al found for dev
-00024a30: 6963 653a 207b 647d 2229 0a0a 2020 2020  ice: {d}")..    
-00024a40: 2020 2020 2020 2020 2020 2020 6966 205f              if _
-00024a50: 6b65 7920 696e 205f 6c69 635f 6b77 6172  key in _lic_kwar
-00024a60: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00024a70: 2020 2020 2020 2020 5f6c 6963 5f6b 7761          _lic_kwa
-00024a80: 7267 735b 5f6b 6579 5d5b 2273 6572 6961  rgs[_key]["seria
-00024a90: 6c73 225d 202b 3d20 7574 696c 732e 6c69  ls"] += utils.li
-00024aa0: 7374 6966 7928 5f73 6572 6961 6c29 0a20  stify(_serial). 
-00024ab0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00024ac0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00024ad0: 2020 2020 2020 2020 205f 6c69 635f 6b77           _lic_kw
-00024ae0: 6172 6773 5b5f 6b65 795d 203d 207b 0a20  args[_key] = {. 
-00024af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024b00: 2020 2020 2020 2022 7365 7276 6963 6573         "services
-00024b10: 223a 2075 7469 6c73 2e6c 6973 7469 6679  ": utils.listify
-00024b20: 2864 5b22 6c69 6365 6e73 6522 5d29 2c0a  (d["license"]),.
-00024b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024b40: 2020 2020 2020 2020 2273 6572 6961 6c73          "serials
-00024b50: 223a 2075 7469 6c73 2e6c 6973 7469 6679  ": utils.listify
-00024b60: 285f 7365 7269 616c 290a 2020 2020 2020  (_serial).      
-00024b70: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00024b80: 2020 2020 2020 2020 2020 2020 6c69 6365              lice
-00024b90: 6e73 655f 6b77 6172 6773 203d 206c 6973  nse_kwargs = lis
-00024ba0: 7428 5f6c 6963 5f6b 7761 7267 732e 7661  t(_lic_kwargs.va
-00024bb0: 6c75 6573 2829 290a 0a20 2020 2020 2020  lues())..       
-00024bc0: 2020 2020 2023 206c 6963 656e 7365 5f61       # license_a
-00024bd0: 7267 7320 3d20 5b5b 5d2c 205b 5d5d 0a20  rgs = [[], []]. 
-00024be0: 2020 2020 2020 2020 2020 2023 2062 795f             # by_
-00024bf0: 7365 7220 3d20 7b64 5b22 7365 7269 616c  ser = {d["serial
-00024c00: 5f6e 756d 225d 3a20 7574 696c 732e 6c69  _num"]: utils.li
-00024c10: 7374 6966 7928 642e 6765 7428 226c 6963  stify(d.get("lic
-00024c20: 656e 7365 2229 2920 666f 7220 6420 696e  ense")) for d in
-00024c30: 2064 6576 6963 655f 6c69 7374 2069 6620   device_list if 
-00024c40: 642e 6765 7428 226c 6963 656e 7365 2229  d.get("license")
-00024c50: 7d0a 2020 2020 2020 2020 2020 2020 2320  }.            # 
-00024c60: 544f 444f 206d 6f73 7420 6566 6669 6369  TODO most effici
-00024c70: 656e 7420 7061 6972 696e 6720 6f66 2070  ent pairing of p
-00024c80: 6f73 7369 626c 6520 6c69 632f 6465 7620  ossible lic/dev 
-00024c90: 666f 7220 6665 7765 7374 2063 616c 6c0a  for fewest call.
-00024ca0: 2020 2020 2020 2020 2020 2020 2320 544f              # TO
-00024cb0: 444f 206c 6963 656e 7365 2076 6961 206c  DO license via l
-00024cc0: 6973 7420 6e6f 7420 696d 706c 656d 656e  ist not implemen
-00024cd0: 7465 6420 7965 742e 0a0a 2020 2020 2020  ted yet...      
-00024ce0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00024cf0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00024d00: 7272 6f72 2822 6d61 635f 6164 6472 6573  rror("mac_addres
-00024d10: 7320 616e 6420 7365 7269 616c 5f6e 756d  s and serial_num
-00024d20: 206f 7220 6465 7669 6365 5f6c 6973 7420   or device_list 
-00024d30: 6973 2072 6571 7569 7265 6422 290a 0a20  is required").. 
-00024d40: 2020 2020 2020 2023 2050 6572 666f 726d         # Perform
-00024d50: 2041 5049 2063 616c 6c28 7329 2074 6f20   API call(s) to 
-00024d60: 4365 6e74 7261 6c20 4150 4920 4757 0a20  Central API GW. 
-00024d70: 2020 2020 2020 2023 2054 4f44 4f20 6272         # TODO br
-00024d80: 6561 6b20 6f75 7420 7468 6520 6164 6420  eak out the add 
-00024d90: 6465 7669 6365 2063 616c 6c20 696e 746f  device call into
-00024da0: 2069 7427 7320 6f77 6e20 6d65 7468 6f64   it's own method
-00024db0: 2e0a 2020 2020 2020 2020 6966 2074 6f5f  ..        if to_
-00024dc0: 6772 6f75 7020 6f72 206c 6963 656e 7365  group or license
-00024dd0: 5f6b 7761 7267 733a 0a20 2020 2020 2020  _kwargs:.       
-00024de0: 2020 2020 2023 2041 6464 2064 6576 6963       # Add devic
-00024df0: 6573 2074 6f20 6365 6e74 7261 6c2e 2020  es to central.  
-00024e00: 3120 4150 4920 6361 6c6c 2066 6f72 2031  1 API call for 1
-00024e10: 206f 7220 6d61 6e79 2064 6576 6963 6573   or many devices
-00024e20: 2e0a 2020 2020 2020 2020 2020 2020 6272  ..            br
-00024e30: 203d 2073 656c 662e 4261 7463 6852 6571   = self.BatchReq
-00024e40: 7565 7374 0a20 2020 2020 2020 2020 2020  uest.           
-00024e50: 2072 6571 7320 3d20 5b0a 2020 2020 2020   reqs = [.      
-00024e60: 2020 2020 2020 2020 2020 6272 2873 656c            br(sel
-00024e70: 662e 706f 7374 2c20 7572 6c2c 206a 736f  f.post, url, jso
-00024e80: 6e5f 6461 7461 3d6a 736f 6e5f 6461 7461  n_data=json_data
-00024e90: 292c 0a20 2020 2020 2020 2020 2020 205d  ),.            ]
-00024ea0: 0a20 2020 2020 2020 2020 2020 2023 2041  .            # A
-00024eb0: 7373 6967 6e20 6465 7669 6365 7320 746f  ssign devices to
-00024ec0: 2070 7265 2d70 726f 7669 7369 6f6e 6564   pre-provisioned
-00024ed0: 2067 726f 7570 2e20 2031 2041 5049 2063   group.  1 API c
-00024ee0: 616c 6c20 7065 7220 6772 6f75 700a 2020  all per group.  
-00024ef0: 2020 2020 2020 2020 2020 2320 544f 444f            # TODO
-00024f00: 2074 6573 7420 7468 6174 2074 6869 7320   test that this 
-00024f10: 6973 2031 2041 5049 2063 616c 6c20 7065  is 1 API call pe
-00024f20: 7220 6772 6f75 702e 0a20 2020 2020 2020  r group..       
-00024f30: 2020 2020 2069 6620 746f 5f67 726f 7570       if to_group
-00024f40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00024f50: 2020 6772 6f75 705f 7265 7173 203d 205b    group_reqs = [
-00024f60: 6272 2873 656c 662e 7072 6570 726f 7669  br(self.preprovi
-00024f70: 7369 6f6e 5f64 6576 6963 655f 746f 5f67  sion_device_to_g
-00024f80: 726f 7570 2c20 2867 2c20 6465 7673 2929  roup, (g, devs))
-00024f90: 2066 6f72 2067 2c20 6465 7673 2069 6e20   for g, devs in 
-00024fa0: 746f 5f67 726f 7570 2e69 7465 6d73 2829  to_group.items()
-00024fb0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00024fc0: 2020 7265 7173 203d 205b 2a72 6571 732c    reqs = [*reqs,
-00024fd0: 202a 6772 6f75 705f 7265 7173 5d0a 0a20   *group_reqs].. 
-00024fe0: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
-00024ff0: 4f20 596f 7520 6361 6e20 6164 6420 7468  O You can add th
-00025000: 6520 6465 7669 6365 2074 6f20 6120 7369  e device to a si
-00025010: 7465 2061 6674 6572 2069 7427 7320 6265  te after it's be
-00025020: 656e 2070 7265 2d61 7373 6967 6e65 640a  en pre-assigned.
-00025030: 2020 2020 2020 2020 2020 2020 2320 6966              # if
-00025040: 2074 6f5f 7369 7465 3a0a 2020 2020 2020   to_site:.      
-00025050: 2020 2020 2020 2320 2020 2020 7369 7465        #     site
-00025060: 5f72 6571 7320 3d20 5b62 7228 7365 6c66  _reqs = [br(self
-00025070: 2e6d 6f76 655f 6465 7669 6365 735f 746f  .move_devices_to
-00025080: 5f73 6974 652c 2028 732c 2064 6576 732c  _site, (s, devs,
-00025090: 2022 6777 2229 2920 666f 7220 732c 2064   "gw")) for s, d
-000250a0: 6576 7320 696e 2074 6f5f 7369 7465 2e69  evs in to_site.i
-000250b0: 7465 6d73 2829 5d0a 2020 2020 2020 2020  tems()].        
-000250c0: 2020 2020 2320 2020 2020 7265 7173 203d      #     reqs =
-000250d0: 205b 2a72 6571 732c 202a 7369 7465 5f72   [*reqs, *site_r
-000250e0: 6571 735d 0a0a 2020 2020 2020 2020 2020  eqs]..          
-000250f0: 2020 2320 4173 7369 676e 206c 6963 656e    # Assign licen
-00025100: 7365 2074 6f20 6465 7669 6365 732e 2020  se to devices.  
-00025110: 3120 4150 4920 6361 6c6c 2066 6f72 2061  1 API call for a
-00025120: 6c6c 2064 6576 6963 6573 2077 6974 6820  ll devices with 
-00025130: 7361 6d65 2063 6f6d 6269 6e61 7469 6f6e  same combination
-00025140: 206f 6620 6c69 6365 6e73 6573 0a20 2020   of licenses.   
-00025150: 2020 2020 2020 2020 2069 6620 6c69 6365           if lice
-00025160: 6e73 655f 6b77 6172 6773 3a0a 2020 2020  nse_kwargs:.    
-00025170: 2020 2020 2020 2020 2020 2020 6c69 635f              lic_
-00025180: 7265 7173 203d 205b 6272 2873 656c 662e  reqs = [br(self.
-00025190: 6173 7369 676e 5f6c 6963 656e 7365 732c  assign_licenses,
-000251a0: 202a 2a6b 7761 7267 7329 2066 6f72 206b   **kwargs) for k
-000251b0: 7761 7267 7320 696e 206c 6963 656e 7365  wargs in license
-000251c0: 5f6b 7761 7267 735d 0a20 2020 2020 2020  _kwargs].       
-000251d0: 2020 2020 2020 2020 2072 6571 7320 3d20           reqs = 
-000251e0: 5b2a 7265 7173 2c20 2a6c 6963 5f72 6571  [*reqs, *lic_req
-000251f0: 735d 0a0a 2020 2020 2020 2020 2020 2020  s]..            
-00025200: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
-00025210: 662e 5f62 6174 6368 5f72 6571 7565 7374  f._batch_request
-00025220: 2872 6571 732c 2063 6f6e 7469 6e75 655f  (reqs, continue_
-00025230: 6f6e 5f66 6169 6c3d 5472 7565 290a 2020  on_fail=True).  
-00025240: 2020 2020 2020 2320 656c 6966 2074 6f5f        # elif to_
-00025250: 7369 7465 3a0a 2020 2020 2020 2020 2320  site:.        # 
-00025260: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00025270: 7272 6f72 2822 5369 7465 2063 616e 206f  rror("Site can o
-00025280: 6e6c 7920 6265 2070 7265 2d61 7373 6967  nly be pre-assig
-00025290: 6e65 6420 6966 2064 6576 6963 6520 6973  ned if device is
-000252a0: 2070 7265 2d70 726f 7669 7369 6f6e 6564   pre-provisioned
-000252b0: 2074 6f20 6120 6772 6f75 7022 290a 2020   to a group").  
-000252c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000252d0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-000252e0: 7761 6974 2073 656c 662e 706f 7374 2875  wait self.post(u
-000252f0: 726c 2c20 6a73 6f6e 5f64 6174 613d 6a73  rl, json_data=js
-00025300: 6f6e 5f64 6174 6129 0a0a 2020 2020 6173  on_data)..    as
-00025310: 796e 6320 6465 6620 636f 705f 6465 6c65  ync def cop_dele
-00025320: 7465 5f64 6576 6963 655f 6672 6f6d 5f69  te_device_from_i
-00025330: 6e76 656e 746f 7279 280a 2020 2020 2020  nventory(.      
-00025340: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00025350: 6465 7669 6365 733a 204c 6973 745b 7374  devices: List[st
-00025360: 725d 203d 204e 6f6e 652c 0a20 2020 2029  r] = None,.    )
-00025370: 202d 3e20 5265 7370 6f6e 7365 3a0a 2020   -> Response:.  
-00025380: 2020 2020 2020 2222 2244 656c 6574 6520        """Delete 
-00025390: 6465 7669 6365 7320 7573 696e 6720 5365  devices using Se
-000253a0: 7269 616c 206e 756d 6265 722e 2020 4f6e  rial number.  On
-000253b0: 6c79 2061 7070 6c69 6573 2074 6f20 436f  ly applies to Co
-000253c0: 5020 6465 706c 6f79 6d65 6e74 732e 0a0a  P deployments...
-000253d0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-000253e0: 2020 2020 2020 2020 2020 6465 7669 6365            device
-000253f0: 7320 286c 6973 742c 206f 7074 696f 6e61  s (list, optiona
-00025400: 6c29 3a20 4c69 7374 206f 6620 6465 7669  l): List of devi
-00025410: 6365 7320 746f 2062 6520 6465 6c65 7465  ces to be delete
-00025420: 6420 6672 6f6d 0a20 2020 2020 2020 2020  d from.         
-00025430: 2020 2020 2020 2047 7265 656e 4c61 6b65         GreenLake
-00025440: 2069 6e76 656e 746f 7279 2e20 204f 6e6c   inventory.  Onl
-00025450: 7920 6170 706c 6965 7320 746f 2043 6f50  y applies to CoP
-00025460: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00025470: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-00025480: 6573 706f 6e73 653a 2043 656e 7472 616c  esponse: Central
-00025490: 4150 4920 5265 7370 6f6e 7365 206f 626a  API Response obj
-000254a0: 6563 740a 2020 2020 2020 2020 2222 220a  ect.        """.
-000254b0: 2020 2020 2020 2020 7572 6c20 3d20 222f          url = "/
-000254c0: 706c 6174 666f 726d 2f64 6576 6963 655f  platform/device_
-000254d0: 696e 7665 6e74 6f72 792f 7631 2f64 6576  inventory/v1/dev
-000254e0: 6963 6573 220a 0a20 2020 2020 2020 2064  ices"..        d
-000254f0: 6576 6963 6573 203d 205b 7b22 7365 7269  evices = [{"seri
-00025500: 616c 223a 2073 6572 6961 6c7d 2066 6f72  al": serial} for
-00025510: 2073 6572 6961 6c20 696e 2064 6576 6963   serial in devic
-00025520: 6573 5d0a 0a20 2020 2020 2020 2072 6574  es]..        ret
-00025530: 7572 6e20 6177 6169 7420 7365 6c66 2e64  urn await self.d
-00025540: 656c 6574 6528 7572 6c2c 206a 736f 6e5f  elete(url, json_
-00025550: 6461 7461 3d64 6576 6963 6573 290a 0a20  data=devices).. 
-00025560: 2020 2023 2054 4f44 4f20 6d61 7962 6520     # TODO maybe 
-00025570: 6865 6c70 6572 206d 6574 686f 6420 746f  helper method to
-00025580: 2064 656c 6574 655f 6465 7669 6365 2074   delete_device t
-00025590: 6861 7420 6361 6c6c 7320 7468 6573 650a  hat calls these.
-000255a0: 2020 2020 6173 796e 6320 6465 6620 6465      async def de
-000255b0: 6c65 7465 5f67 6174 6577 6179 280a 2020  lete_gateway(.  
-000255c0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-000255d0: 2020 2020 7365 7269 616c 3a20 7374 722c      serial: str,
-000255e0: 0a20 2020 2029 202d 3e20 5265 7370 6f6e  .    ) -> Respon
-000255f0: 7365 3a0a 2020 2020 2020 2020 2222 2244  se:.        """D
-00025600: 656c 6574 6520 4761 7465 7761 792e 0a0a  elete Gateway...
-00025610: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00025620: 2020 2020 2020 2020 2020 7365 7269 616c            serial
-00025630: 2028 7374 7229 3a20 5365 7269 616c 204e   (str): Serial N
-00025640: 756d 6265 7220 6f66 2047 6174 6577 6179  umber of Gateway
-00025650: 2074 6f20 6265 2064 656c 6574 6564 0a0a   to be deleted..
-00025660: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00025670: 0a20 2020 2020 2020 2020 2020 2052 6573  .            Res
-00025680: 706f 6e73 653a 2043 656e 7472 616c 4150  ponse: CentralAP
-00025690: 4920 5265 7370 6f6e 7365 206f 626a 6563  I Response objec
-000256a0: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
-000256b0: 2020 2020 2020 7572 6c20 3d20 6622 2f6d        url = f"/m
-000256c0: 6f6e 6974 6f72 696e 672f 7632 2f6d 6f62  onitoring/v2/mob
-000256d0: 696c 6974 795f 636f 6e74 726f 6c6c 6572  ility_controller
-000256e0: 732f 7b73 6572 6961 6c7d 2220 6966 2063  s/{serial}" if c
-000256f0: 6f6e 6669 672e 6973 5f63 6f70 2065 6c73  onfig.is_cop els
-00025700: 6520 6622 2f6d 6f6e 6974 6f72 696e 672f  e f"/monitoring/
-00025710: 7631 2f67 6174 6577 6179 732f 7b73 6572  v1/gateways/{ser
-00025720: 6961 6c7d 220a 0a20 2020 2020 2020 2072  ial}"..        r
-00025730: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-00025740: 2e64 656c 6574 6528 7572 6c29 0a0a 2020  .delete(url)..  
-00025750: 2020 6173 796e 6320 6465 6620 6465 6c65    async def dele
-00025760: 7465 5f73 7769 7463 6828 0a20 2020 2020  te_switch(.     
-00025770: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00025780: 2073 6572 6961 6c3a 2073 7472 2c0a 2020   serial: str,.  
-00025790: 2020 2920 2d3e 2052 6573 706f 6e73 653a    ) -> Response:
-000257a0: 0a20 2020 2020 2020 2022 2222 4465 6c65  .        """Dele
-000257b0: 7465 2053 7769 7463 682e 0a0a 2020 2020  te Switch...    
-000257c0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000257d0: 2020 2020 2020 7365 7269 616c 2028 7374        serial (st
-000257e0: 7229 3a20 5365 7269 616c 206e 756d 6265  r): Serial numbe
-000257f0: 7220 6f66 2073 7769 7463 6820 746f 2062  r of switch to b
-00025800: 6520 6465 6c65 7465 640a 0a20 2020 2020  e deleted..     
-00025810: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00025820: 2020 2020 2020 2020 5265 7370 6f6e 7365          Response
-00025830: 3a20 4365 6e74 7261 6c41 5049 2052 6573  : CentralAPI Res
-00025840: 706f 6e73 6520 6f62 6a65 6374 0a20 2020  ponse object.   
-00025850: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00025860: 2075 726c 203d 2066 222f 6d6f 6e69 746f   url = f"/monito
-00025870: 7269 6e67 2f76 312f 7377 6974 6368 6573  ring/v1/switches
-00025880: 2f7b 7365 7269 616c 7d22 0a0a 2020 2020  /{serial}"..    
-00025890: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-000258a0: 2073 656c 662e 6465 6c65 7465 2875 726c   self.delete(url
-000258b0: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-000258c0: 2064 656c 6574 655f 7374 6163 6b28 0a20   delete_stack(. 
-000258d0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000258e0: 2020 2020 2073 7461 636b 5f69 643a 2073       stack_id: s
-000258f0: 7472 2c0a 2020 2020 2920 2d3e 2052 6573  tr,.    ) -> Res
-00025900: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
-00025910: 2222 4465 6c65 7465 2053 7769 7463 6820  ""Delete Switch 
-00025920: 5374 6163 6b2e 0a0a 2020 2020 2020 2020  Stack...        
-00025930: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00025940: 2020 7374 6163 6b5f 6964 2028 7374 7229    stack_id (str)
-00025950: 3a20 4669 6c74 6572 2062 7920 5377 6974  : Filter by Swit
-00025960: 6368 2073 7461 636b 5f69 640a 0a20 2020  ch stack_id..   
-00025970: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00025980: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
-00025990: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
-000259a0: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
-000259b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000259c0: 2020 2075 726c 203d 2066 222f 6d6f 6e69     url = f"/moni
-000259d0: 746f 7269 6e67 2f76 312f 7377 6974 6368  toring/v1/switch
-000259e0: 5f73 7461 636b 732f 7b73 7461 636b 5f69  _stacks/{stack_i
-000259f0: 647d 220a 0a20 2020 2020 2020 2072 6574  d}"..        ret
-00025a00: 7572 6e20 6177 6169 7420 7365 6c66 2e64  urn await self.d
-00025a10: 656c 6574 6528 7572 6c29 0a0a 2020 2020  elete(url)..    
-00025a20: 6173 796e 6320 6465 6620 6465 6c65 7465  async def delete
-00025a30: 5f61 7028 0a20 2020 2020 2020 2073 656c  _ap(.        sel
-00025a40: 662c 0a20 2020 2020 2020 2073 6572 6961  f,.        seria
-00025a50: 6c3a 2073 7472 2c0a 2020 2020 2920 2d3e  l: str,.    ) ->
-00025a60: 2052 6573 706f 6e73 653a 0a20 2020 2020   Response:.     
-00025a70: 2020 2022 2222 4465 6c65 7465 2041 502e     """Delete AP.
-00025a80: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00025a90: 2020 2020 2020 2020 2020 2020 7365 7269              seri
-00025aa0: 616c 2028 7374 7229 3a20 5365 7269 616c  al (str): Serial
-00025ab0: 204e 756d 6265 7220 6f66 2041 5020 746f   Number of AP to
-00025ac0: 2062 6520 6465 6c65 7465 640a 0a20 2020   be deleted..   
-00025ad0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00025ae0: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
-00025af0: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
-00025b00: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
-00025b10: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00025b20: 2020 2075 726c 203d 2066 222f 6d6f 6e69     url = f"/moni
-00025b30: 746f 7269 6e67 2f76 312f 6170 732f 7b73  toring/v1/aps/{s
-00025b40: 6572 6961 6c7d 220a 0a20 2020 2020 2020  erial}"..       
-00025b50: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-00025b60: 6c66 2e64 656c 6574 6528 7572 6c29 0a0a  lf.delete(url)..
-00025b70: 2020 2020 2320 544f 444f 206d 6179 2072      # TODO may r
-00025b80: 656d 6f76 6520 7468 6973 2077 6f75 6c64  emove this would
-00025b90: 2073 686f 7720 7468 6520 6465 7669 6365   show the device
-00025ba0: 2069 6e20 7468 6520 6772 6f75 702c 2062   in the group, b
-00025bb0: 7574 2064 6964 6e27 7420 6265 6861 7665  ut didn't behave
-00025bc0: 2061 7320 6578 7065 6374 6564 2028 6465   as expected (de
-00025bd0: 7669 6365 2077 6173 206e 6f74 2069 6e20  vice was not in 
-00025be0: 6465 7669 6365 206c 6973 7429 0a20 2020  device list).   
-00025bf0: 2061 7379 6e63 2064 6566 2061 7373 6967   async def assig
-00025c00: 6e5f 6465 7669 6365 735f 746f 5f67 726f  n_devices_to_gro
-00025c10: 7570 2873 656c 662c 2020 6772 6f75 703a  up(self,  group:
-00025c20: 2073 7472 2c20 7365 7269 616c 5f6e 756d   str, serial_num
-00025c30: 733a 2055 6e69 6f6e 5b4c 6973 745b 7374  s: Union[List[st
-00025c40: 725d 2c20 7374 725d 2920 2d3e 2052 6573  r], str]) -> Res
-00025c50: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
-00025c60: 2222 4173 7369 676e 2064 6576 6963 6573  ""Assign devices
-00025c70: 2074 6f20 7072 652d 7072 6f76 6973 696f   to pre-provisio
-00025c80: 6e65 6420 6772 6f75 702e 0a0a 2020 2020  ned group...    
-00025c90: 2020 2020 2f2f 2055 7365 6420 696e 6469      // Used indi
-00025ca0: 7265 6374 6c79 2062 7920 6164 6420 6465  rectly by add de
-00025cb0: 7669 6365 2028 7768 656e 2067 726f 7570  vice (when group
-00025cc0: 206f 7074 696f 6e20 7072 6f76 6964 6564   option provided
-00025cd0: 2920 2f2f 0a0a 2020 2020 2020 2020 4172  ) //..        Ar
-00025ce0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00025cf0: 6772 6f75 7020 2873 7472 293a 2047 726f  group (str): Gro
-00025d00: 7570 206e 616d 650a 2020 2020 2020 2020  up name.        
-00025d10: 2020 2020 7365 7269 616c 7320 284c 6973      serials (Lis
-00025d20: 745b 7374 725d 7c73 7472 293a 2044 6576  t[str]|str): Dev
-00025d30: 6963 6520 7365 7269 616c 206e 756d 6265  ice serial numbe
-00025d40: 7220 6f72 206c 6973 7420 6f66 2064 6576  r or list of dev
-00025d50: 6963 6520 7365 7269 616c 206e 756d 6265  ice serial numbe
-00025d60: 7273 2e0a 0a20 2020 2020 2020 2052 6574  rs...        Ret
-00025d70: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00025d80: 2020 5265 7370 6f6e 7365 3a20 4365 6e74    Response: Cent
-00025d90: 7261 6c41 5049 2052 6573 706f 6e73 6520  ralAPI Response 
-00025da0: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
-00025db0: 2222 0a20 2020 2020 2020 2075 726c 203d  "".        url =
-00025dc0: 2022 2f64 6576 6963 655f 6d61 6e61 6765   "/device_manage
-00025dd0: 6d65 6e74 2f76 312f 6772 6f75 702f 6173  ment/v1/group/as
-00025de0: 7369 676e 220a 2020 2020 2020 2020 7365  sign".        se
-00025df0: 7269 616c 5f6e 756d 7320 3d20 7574 696c  rial_nums = util
-00025e00: 732e 6c69 7374 6966 7928 7365 7269 616c  s.listify(serial
-00025e10: 5f6e 756d 7329 0a0a 2020 2020 2020 2020  _nums)..        
-00025e20: 6a73 6f6e 5f64 6174 6120 3d20 7b0a 2020  json_data = {.  
-00025e30: 2020 2020 2020 2020 2020 2773 6572 6961            'seria
-00025e40: 6c73 273a 2073 6572 6961 6c5f 6e75 6d73  ls': serial_nums
-00025e50: 2c0a 2020 2020 2020 2020 2020 2020 2767  ,.            'g
-00025e60: 726f 7570 273a 2067 726f 7570 0a20 2020  roup': group.   
-00025e70: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-00025e80: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
-00025e90: 662e 706f 7374 2875 726c 2c20 6a73 6f6e  f.post(url, json
-00025ea0: 5f64 6174 613d 6a73 6f6e 5f64 6174 6129  _data=json_data)
-00025eb0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-00025ec0: 7072 6570 726f 7669 7369 6f6e 5f64 6576  preprovision_dev
-00025ed0: 6963 655f 746f 5f67 726f 7570 280a 2020  ice_to_group(.  
-00025ee0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00025ef0: 2020 2020 6772 6f75 705f 6e61 6d65 3a20      group_name: 
-00025f00: 7374 722c 0a20 2020 2020 2020 2073 6572  str,.        ser
-00025f10: 6961 6c5f 6e75 6d73 3a20 4c69 7374 5b73  ial_nums: List[s
-00025f20: 7472 5d20 7c20 7374 722c 0a20 2020 2020  tr] | str,.     
-00025f30: 2020 2074 656e 616e 745f 6964 3a20 7374     tenant_id: st
-00025f40: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2920  r = None,.    ) 
-00025f50: 2d3e 2052 6573 706f 6e73 653a 0a20 2020  -> Response:.   
-00025f60: 2020 2020 2022 2222 5072 6520 5072 6f76       """Pre Prov
-00025f70: 6973 696f 6e20 6120 6772 6f75 7020 746f  ision a group to
-00025f80: 2074 6865 2064 6576 6963 652e 0a0a 2020   the device...  
-00025f90: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00025fa0: 2020 2020 2020 2020 6465 7669 6365 5f69          device_i
-00025fb0: 6420 284c 6973 745b 7374 725d 293a 2064  d (List[str]): d
-00025fc0: 6576 6963 655f 6964 0a20 2020 2020 2020  evice_id.       
-00025fd0: 2020 2020 2067 726f 7570 5f6e 616d 6520       group_name 
-00025fe0: 2873 7472 293a 2047 726f 7570 206e 616d  (str): Group nam
-00025ff0: 650a 2020 2020 2020 2020 2020 2020 7465  e.            te
-00026000: 6e61 6e74 5f69 6420 2873 7472 293a 2054  nant_id (str): T
-00026010: 656e 616e 7420 6964 2c20 286f 6e6c 7920  enant id, (only 
-00026020: 6170 706c 6963 6162 6c65 2077 6974 6820  applicable with 
-00026030: 4d53 5020 6d6f 6465 290a 0a20 2020 2020  MSP mode)..     
-00026040: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00026050: 2020 2020 2020 2020 5265 7370 6f6e 7365          Response
-00026060: 3a20 4365 6e74 7261 6c41 5049 2052 6573  : CentralAPI Res
-00026070: 706f 6e73 6520 6f62 6a65 6374 0a20 2020  ponse object.   
-00026080: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00026090: 2075 726c 203d 2022 2f63 6f6e 6669 6775   url = "/configu
-000260a0: 7261 7469 6f6e 2f76 312f 7072 6561 7373  ration/v1/preass
-000260b0: 6967 6e22 0a0a 2020 2020 2020 2020 6a73  ign"..        js
-000260c0: 6f6e 5f64 6174 6120 3d20 7b0a 2020 2020  on_data = {.    
-000260d0: 2020 2020 2020 2020 2764 6576 6963 655f          'device_
-000260e0: 6964 273a 2075 7469 6c73 2e6c 6973 7469  id': utils.listi
-000260f0: 6679 2873 6572 6961 6c5f 6e75 6d73 292c  fy(serial_nums),
-00026100: 0a20 2020 2020 2020 2020 2020 2027 6772  .            'gr
-00026110: 6f75 705f 6e61 6d65 273a 2067 726f 7570  oup_name': group
-00026120: 5f6e 616d 652c 0a20 2020 2020 2020 207d  _name,.        }
-00026130: 0a0a 2020 2020 2020 2020 6966 2074 656e  ..        if ten
-00026140: 616e 745f 6964 2069 7320 6e6f 7420 4e6f  ant_id is not No
-00026150: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00026160: 6a73 6f6e 5f64 6174 615b 2274 656e 616e  json_data["tenan
-00026170: 745f 6964 225d 203d 2073 7472 2874 656e  t_id"] = str(ten
-00026180: 616e 745f 6964 290a 0a20 2020 2020 2020  ant_id)..       
-00026190: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-000261a0: 6c66 2e70 6f73 7428 7572 6c2c 206a 736f  lf.post(url, jso
-000261b0: 6e5f 6461 7461 3d6a 736f 6e5f 6461 7461  n_data=json_data
-000261c0: 290a 0a20 2020 2023 2054 4f44 4f20 7665  )..    # TODO ve
-000261d0: 7269 6679 2074 7970 652d 6869 6e74 2066  rify type-hint f
-000261e0: 6f72 2064 6576 6963 655f 6c69 7374 2069  or device_list i
-000261f0: 7320 7468 6520 7269 6768 7420 7761 7920  s the right way 
-00026200: 746f 2064 6f20 7468 6174 2e0a 2020 2020  to do that..    
-00026210: 6173 796e 6320 6465 6620 7665 7269 6679  async def verify
-00026220: 5f64 6576 6963 655f 6164 6469 7469 6f6e  _device_addition
-00026230: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00026240: 2020 2020 2020 2020 7365 7269 616c 5f6e          serial_n
-00026250: 756d 3a20 7374 7220 3d20 4e6f 6e65 2c0a  um: str = None,.
-00026260: 2020 2020 2020 2020 6d61 635f 6164 6472          mac_addr
-00026270: 6573 733a 2073 7472 203d 204e 6f6e 652c  ess: str = None,
-00026280: 0a20 2020 2020 2020 2064 6576 6963 655f  .        device_
-00026290: 6c69 7374 3a20 4c69 7374 5b44 6963 745b  list: List[Dict[
-000262a0: 4c69 7465 7261 6c5b 226d 6163 5f61 6464  Literal["mac_add
-000262b0: 7265 7373 222c 2022 7365 7269 616c 5f6e  ress", "serial_n
-000262c0: 756d 225d 2c20 7374 725d 5d20 3d20 5b5d  um"], str]] = []
-000262d0: 0a20 2020 2029 202d 3e20 5265 7370 6f6e  .    ) -> Respon
-000262e0: 7365 3a0a 2020 2020 2020 2020 2222 2256  se:.        """V
-000262f0: 6572 6966 7920 4465 7669 6365 2041 6464  erify Device Add
-00026300: 6974 696f 6e0a 0a20 2020 2020 2020 2041  ition..        A
-00026310: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00026320: 2073 6572 6961 6c5f 6e75 6d20 2873 7472   serial_num (str
-00026330: 2c20 6f70 7469 6f6e 616c 293a 2053 6572  , optional): Ser
-00026340: 6961 6c20 4e75 6d62 6572 206f 6620 6465  ial Number of de
-00026350: 7669 6365 2074 6f20 7665 7269 6679 2e20  vice to verify. 
-00026360: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
-00026370: 2e0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
-00026380: 635f 6164 6472 6573 7320 2873 7472 2c20  c_address (str, 
-00026390: 6f70 7469 6f6e 616c 293a 204d 6163 2041  optional): Mac A
-000263a0: 6464 7265 7373 206f 6620 6465 7669 6365  ddress of device
-000263b0: 2074 6f20 7665 7269 6679 2e20 4465 6661   to verify. Defa
-000263c0: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
-000263d0: 2020 2020 2020 2020 2020 6465 7669 6365            device
-000263e0: 5f6c 6973 7420 284c 6973 745b 4469 6374  _list (List[Dict
-000263f0: 5b4c 6974 6572 616c 5b2c 206f 7074 696f  [Literal[, optio
-00026400: 6e61 6c29 3a20 6465 7669 6365 5f6c 6973  nal): device_lis
-00026410: 7420 6c69 7374 206f 6620 6469 6374 7320  t list of dicts 
-00026420: 7769 7468 0a20 2020 2020 2020 2020 2020  with.           
-00026430: 2020 2020 2022 7365 7269 616c 5f6e 756d       "serial_num
-00026440: 2220 616e 6420 226d 6163 5f61 6464 7265  " and "mac_addre
-00026450: 7373 2220 666f 7220 6561 6368 2064 6576  ss" for each dev
-00026460: 6963 6520 746f 2076 6572 6966 792e 2044  ice to verify. D
-00026470: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
-00026480: 0a0a 2020 2020 2020 2020 4d75 7374 2070  ..        Must p
-00026490: 726f 7669 6465 2073 6572 6961 6c5f 6e75  rovide serial_nu
-000264a0: 6d20 616e 6420 6d61 635f 6164 6472 6573  m and mac_addres
-000264b0: 7320 666f 7220 6561 6368 2064 6576 6963  s for each devic
-000264c0: 6520 6569 7468 6572 2076 6961 206b 6579  e either via key
-000264d0: 776f 7264 2061 7267 756d 656e 7420 6f72  word argument or
-000264e0: 206c 6973 742e 0a0a 2020 2020 2020 2020   list...        
-000264f0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00026500: 2020 2020 2052 6573 706f 6e73 653a 2043       Response: C
-00026510: 656e 7472 616c 4150 4920 5265 7370 6f6e  entralAPI Respon
-00026520: 7365 206f 626a 6563 740a 2020 2020 2020  se object.      
-00026530: 2020 2222 220a 2020 2020 2020 2020 7572    """.        ur
-00026540: 6c20 3d20 222f 706c 6174 666f 726d 2f64  l = "/platform/d
-00026550: 6576 6963 655f 696e 7665 6e74 6f72 792f  evice_inventory/
-00026560: 7631 2f64 6576 6963 6573 2f76 6572 6966  v1/devices/verif
-00026570: 7922 0a20 2020 2020 2020 2069 6620 7365  y".        if se
-00026580: 7269 616c 5f6e 756d 2061 6e64 206d 6163  rial_num and mac
-00026590: 5f61 6464 7265 7373 3a0a 2020 2020 2020  _address:.      
-000265a0: 2020 2020 2020 6465 7669 6365 5f6c 6973        device_lis
-000265b0: 7420 2b3d 207b 0a20 2020 2020 2020 2020  t += {.         
-000265c0: 2020 2020 2020 2022 7365 7269 616c 5f6e         "serial_n
-000265d0: 756d 223a 2073 6572 6961 6c5f 6e75 6d2c  um": serial_num,
-000265e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000265f0: 2022 6d61 635f 6164 6472 6573 7322 3a20   "mac_address": 
-00026600: 6d61 635f 6164 6472 6573 732c 0a20 2020  mac_address,.   
-00026610: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
-00026620: 2020 2020 6966 206e 6f74 2064 6576 6963      if not devic
-00026630: 655f 6c69 7374 3a0a 2020 2020 2020 2020  e_list:.        
-00026640: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00026650: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-00026660: 2020 2020 2020 2249 6e76 616c 6964 2070        "Invalid p
-00026670: 6172 616d 6574 6572 7320 6578 7065 6374  arameters expect
-00026680: 696e 6720 7365 7269 616c 5f6e 756d 2061  ing serial_num a
-00026690: 6e64 206d 6163 5f61 6464 7265 7373 2066  nd mac_address f
-000266a0: 6f72 2065 6163 6820 6465 7669 6365 2022  or each device "
-000266b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000266c0: 2022 6569 7468 6572 2076 6961 206b 6579   "either via key
-000266d0: 776f 7264 2061 7267 756d 656e 7420 6f72  word argument or
-000266e0: 204c 6973 745b 6469 6374 5d2e 220a 2020   List[dict].".  
-000266f0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00026700: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
-00026710: 7420 7365 6c66 2e70 6f73 7428 7572 6c2c  t self.post(url,
-00026720: 206a 736f 6e5f 6461 7461 3d64 6576 6963   json_data=devic
-00026730: 655f 6c69 7374 290a 0a20 2020 2061 7379  e_list)..    asy
-00026740: 6e63 2064 6566 2075 706c 6f61 645f 6365  nc def upload_ce
-00026750: 7274 6966 6963 6174 6528 0a20 2020 2020  rtificate(.     
-00026760: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00026770: 2070 6173 7370 6872 6173 653a 2073 7472   passphrase: str
-00026780: 203d 2022 222c 0a20 2020 2020 2020 2063   = "",.        c
-00026790: 6572 745f 6669 6c65 3a20 556e 696f 6e5b  ert_file: Union[
-000267a0: 7374 722c 2050 6174 685d 203d 204e 6f6e  str, Path] = Non
-000267b0: 652c 0a20 2020 2020 2020 2063 6572 745f  e,.        cert_
-000267c0: 6e61 6d65 3a20 7374 7220 3d20 4e6f 6e65  name: str = None
-000267d0: 2c0a 2020 2020 2020 2020 6365 7274 5f66  ,.        cert_f
-000267e0: 6f72 6d61 743a 204c 6974 6572 616c 5b22  ormat: Literal["
-000267f0: 5045 4d22 2c20 2244 4552 222c 2022 504b  PEM", "DER", "PK
-00026800: 4353 3132 225d 203d 204e 6f6e 652c 0a20  CS12"] = None,. 
-00026810: 2020 2020 2020 2063 6572 745f 6461 7461         cert_data
-00026820: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00026830: 2020 2020 2020 7365 7276 6572 5f63 6572        server_cer
-00026840: 743a 2062 6f6f 6c20 3d20 4661 6c73 652c  t: bool = False,
-00026850: 0a20 2020 2020 2020 2063 615f 6365 7274  .        ca_cert
-00026860: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-00026870: 2020 2020 2020 2020 6372 6c3a 2062 6f6f          crl: boo
-00026880: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
-00026890: 2020 2069 6e74 5f63 615f 6365 7274 3a20     int_ca_cert: 
-000268a0: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-000268b0: 2020 2020 2020 6f63 7370 5f72 6573 705f        ocsp_resp_
-000268c0: 6365 7274 3a20 626f 6f6c 203d 2046 616c  cert: bool = Fal
-000268d0: 7365 2c0a 2020 2020 2020 2020 6f63 7370  se,.        ocsp
-000268e0: 5f73 6967 6e65 725f 6365 7274 3a20 626f  _signer_cert: bo
-000268f0: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-00026900: 2020 2020 7373 685f 7075 625f 6b65 793a      ssh_pub_key:
-00026910: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-00026920: 2020 2029 202d 3e20 5265 7370 6f6e 7365     ) -> Response
-00026930: 3a0a 2020 2020 2020 2020 2222 2255 706c  :.        """Upl
-00026940: 6f61 6420 6120 6365 7274 6966 6963 6174  oad a certificat
-00026950: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
-00026960: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-00026970: 7373 7068 7261 7365 2028 7374 7229 3a20  ssphrase (str): 
-00026980: 7061 7373 7068 7261 7365 0a20 2020 2020  passphrase.     
-00026990: 2020 2020 2020 2063 6572 745f 6669 6c65         cert_file
-000269a0: 2028 5061 7468 7c73 7472 2c20 6f70 7469   (Path|str, opti
-000269b0: 6f6e 616c 293a 2043 6572 7420 6669 6c65  onal): Cert file
-000269c0: 2074 6f20 7570 6c6f 6164 2c20 6966 2066   to upload, if f
-000269d0: 696c 6520 6973 2070 726f 7669 6465 6420  ile is provided 
-000269e0: 6365 7274 5f6e 616d 650a 2020 2020 2020  cert_name.      
-000269f0: 2020 2020 2020 2020 2020 616e 6420 6365            and ce
-00026a00: 7274 5f66 6f72 6d61 7420 7769 6c6c 2062  rt_format will b
-00026a10: 6520 6465 7269 7665 6420 6672 6f6d 2066  e derived from f
-00026a20: 696c 6520 6e61 6d65 202f 2065 7874 656e  ile name / exten
-00026a30: 7369 6f6e 2c20 756e 6c65 7373 2074 686f  sion, unless tho
-00026a40: 7365 2070 6172 616d 730a 2020 2020 2020  se params.      
-00026a50: 2020 2020 2020 2020 2020 6172 6520 616c            are al
-00026a60: 736f 2070 726f 7669 6465 642e 0a20 2020  so provided..   
-00026a70: 2020 2020 2020 2020 2063 6572 745f 6e61           cert_na
-00026a80: 6d65 2028 7374 722c 206f 7074 696f 6e61  me (str, optiona
-00026a90: 6c29 3a20 5468 6520 6e61 6d65 206f 6620  l): The name of 
-00026aa0: 7468 6520 6365 7274 6966 6963 6174 652e  the certificate.
-00026ab0: 0a20 2020 2020 2020 2020 2020 2063 6572  .            cer
-00026ac0: 745f 666f 726d 6174 2028 4c69 7465 7261  t_format (Litera
-00026ad0: 6c5b 2250 454d 222c 2022 4445 5222 2c20  l["PEM", "DER", 
-00026ae0: 2250 4b43 5331 3222 5d2c 206f 7074 696f  "PKCS12"], optio
-00026af0: 6e61 6c29 3a20 6365 7274 5f66 6f72 6d61  nal): cert_forma
-00026b00: 7420 2056 616c 6964 2056 616c 7565 733a  t  Valid Values:
-00026b10: 2050 454d 2c20 4445 522c 2050 4b43 5331   PEM, DER, PKCS1
-00026b20: 320a 2020 2020 2020 2020 2020 2020 6365  2.            ce
-00026b30: 7274 5f64 6174 6120 2873 7472 2c20 6f70  rt_data (str, op
-00026b40: 7469 6f6e 616c 293a 2043 6572 7469 6669  tional): Certifi
-00026b50: 6361 7465 2063 6f6e 7465 6e74 2065 6e63  cate content enc
-00026b60: 6f64 6564 2069 6e20 6261 7365 3634 2066  oded in base64 f
-00026b70: 6f72 2061 6c6c 2066 6f72 6d61 7420 6365  or all format ce
-00026b80: 7274 6966 6963 6174 6573 2e0a 2020 2020  rtificates..    
-00026b90: 2020 2020 2020 2020 7365 7276 6572 5f63          server_c
-00026ba0: 6572 7420 2862 6f6f 6c2c 206f 7074 696f  ert (bool, optio
-00026bb0: 6e61 6c29 3a20 5365 7420 746f 2054 7275  nal): Set to Tru
-00026bc0: 6520 6966 2063 6572 7420 6973 2061 2073  e if cert is a s
-00026bd0: 6572 7665 7220 6365 7274 6966 6963 6174  erver certificat
-00026be0: 652e 2044 6566 6175 6c74 7320 746f 2046  e. Defaults to F
-00026bf0: 616c 7365 2e0a 2020 2020 2020 2020 2020  alse..          
-00026c00: 2020 6361 5f63 6572 7420 2862 6f6f 6c2c    ca_cert (bool,
-00026c10: 206f 7074 696f 6e61 6c29 3a20 5365 7420   optional): Set 
-00026c20: 746f 2054 7275 6520 6966 2063 6572 7420  to True if cert 
-00026c30: 6973 2061 2043 4120 4365 7274 6966 6963  is a CA Certific
-00026c40: 6174 652e 2044 6566 6175 6c74 7320 746f  ate. Defaults to
-00026c50: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
-00026c60: 2020 2020 6372 6c20 2862 6f6f 6c2c 206f      crl (bool, o
-00026c70: 7074 696f 6e61 6c29 3a20 5365 7420 746f  ptional): Set to
-00026c80: 2054 7275 6520 6966 2064 6174 6120 6973   True if data is
-00026c90: 2061 2063 6572 7469 6669 6361 7465 2072   a certificate r
-00026ca0: 6576 6f63 6174 696f 6e20 6c69 7374 2e20  evocation list. 
-00026cb0: 4465 6661 756c 7473 2074 6f20 4661 6c73  Defaults to Fals
-00026cc0: 652e 0a20 2020 2020 2020 2020 2020 2069  e..            i
-00026cd0: 6e74 5f63 615f 6365 7274 2028 626f 6f6c  nt_ca_cert (bool
-00026ce0: 2c20 6f70 7469 6f6e 616c 293a 2053 6574  , optional): Set
-00026cf0: 2074 6f20 5472 7565 2069 6620 6365 7274   to True if cert
-00026d00: 6966 6963 6174 6520 6973 2061 6e20 696e  ificate is an in
-00026d10: 7465 726d 6564 6961 7465 2043 4120 6365  termediate CA ce
-00026d20: 7274 2e20 4465 6661 756c 7473 2074 6f20  rt. Defaults to 
-00026d30: 4661 6c73 652e 0a20 2020 2020 2020 2020  False..         
-00026d40: 2020 206f 6373 705f 7265 7370 5f63 6572     ocsp_resp_cer
-00026d50: 7420 2862 6f6f 6c2c 206f 7074 696f 6e61  t (bool, optiona
-00026d60: 6c29 3a20 5365 7420 746f 2054 7275 6520  l): Set to True 
-00026d70: 6966 2063 6572 7469 6669 6361 7465 2069  if certificate i
-00026d80: 7320 616e 204f 4353 5020 7265 7370 6f6e  s an OCSP respon
-00026d90: 6465 7220 6365 7274 2e20 4465 6661 756c  der cert. Defaul
-00026da0: 7473 2074 6f20 4661 6c73 652e 0a20 2020  ts to False..   
-00026db0: 2020 2020 2020 2020 206f 6373 705f 7369           ocsp_si
-00026dc0: 676e 6572 5f63 6572 7420 2862 6f6f 6c2c  gner_cert (bool,
-00026dd0: 206f 7074 696f 6e61 6c29 3a20 5365 7420   optional): Set 
-00026de0: 746f 2054 7275 6520 6966 2063 6572 7469  to True if certi
-00026df0: 6669 6361 7465 2069 7320 616e 204f 4353  ficate is an OCS
-00026e00: 5020 7369 676e 6572 2063 6572 742e 2044  P signer cert. D
-00026e10: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
-00026e20: 2e0a 2020 2020 2020 2020 2020 2020 7373  ..            ss
-00026e30: 685f 7075 625f 6b65 7920 2862 6f6f 6c2c  h_pub_key (bool,
-00026e40: 206f 7074 696f 6e61 6c29 3a20 5365 7420   optional): Set 
-00026e50: 746f 2054 7275 6520 6966 2063 6572 7469  to True if certi
-00026e60: 6669 6361 7465 2069 7320 616e 2053 5348  ficate is an SSH
-00026e70: 2050 7562 206b 6579 2e20 4465 6661 756c   Pub key. Defaul
-00026e80: 7473 2074 6f20 4661 6c73 652e 0a20 2020  ts to False..   
-00026e90: 2020 2020 2020 2020 2020 2020 2073 7368               ssh
-00026ea0: 5f70 7562 5f6b 6579 206e 6565 6473 2074  _pub_key needs t
-00026eb0: 6f20 6265 2069 6e20 5045 4d20 666f 726d  o be in PEM form
-00026ec0: 6174 2c20 7373 682d 7273 6120 6973 206e  at, ssh-rsa is n
-00026ed0: 6f74 2073 7570 706f 7274 6564 2e0a 0a20  ot supported... 
-00026ee0: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
-00026ef0: 2020 2020 2020 2020 2020 2056 616c 7565             Value
-00026f00: 4572 726f 723a 2052 6169 7365 6420 6966  Error: Raised if
-00026f10: 2069 6e76 616c 6964 2063 6f6d 6269 6e61   invalid combina
-00026f20: 7469 6f6e 206f 6620 6172 6775 6d65 6e74  tion of argument
-00026f30: 7320 6973 2070 726f 7669 6465 642e 0a0a  s is provided...
-00026f40: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00026f50: 0a20 2020 2020 2020 2020 2020 2052 6573  .            Res
-00026f60: 706f 6e73 653a 2043 656e 7472 616c 4150  ponse: CentralAP
-00026f70: 4920 5265 7370 6f6e 7365 206f 626a 6563  I Response objec
-00026f80: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
-00026f90: 2020 2020 2020 2320 4150 492d 464c 4157        # API-FLAW
-00026fa0: 2041 5049 206d 6574 686f 642c 2050 5542   API method, PUB
-00026fb0: 4c49 435f 4345 5254 2069 7320 6e6f 7420  LIC_CERT is not 
-00026fc0: 6163 6365 7074 6564 0a20 2020 2020 2020  accepted.       
-00026fd0: 2075 726c 203d 2022 2f63 6f6e 6669 6775   url = "/configu
-00026fe0: 7261 7469 6f6e 2f76 312f 6365 7274 6966  ration/v1/certif
-00026ff0: 6963 6174 6573 220a 2020 2020 2020 2020  icates".        
-00027000: 7661 6c69 645f 7479 7065 7320 3d20 5b0a  valid_types = [.
-00027010: 2020 2020 2020 2020 2020 2020 2253 4552              "SER
-00027020: 5645 525f 4345 5254 222c 0a20 2020 2020  VER_CERT",.     
-00027030: 2020 2020 2020 2022 4341 5f43 4552 5422         "CA_CERT"
-00027040: 2c0a 2020 2020 2020 2020 2020 2020 2243  ,.            "C
-00027050: 524c 222c 0a20 2020 2020 2020 2020 2020  RL",.           
-00027060: 2022 494e 5445 524d 4544 4941 5445 5f43   "INTERMEDIATE_C
-00027070: 4122 2c0a 2020 2020 2020 2020 2020 2020  A",.            
-00027080: 224f 4353 505f 5245 5350 4f4e 4445 525f  "OCSP_RESPONDER_
-00027090: 4345 5254 222c 0a20 2020 2020 2020 2020  CERT",.         
-000270a0: 2020 2022 4f43 5350 5f53 4947 4e45 525f     "OCSP_SIGNER_
-000270b0: 4345 5254 222c 0a20 2020 2020 2020 2020  CERT",.         
-000270c0: 2020 2022 5055 424c 4943 5f43 4552 5422     "PUBLIC_CERT"
-000270d0: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-000270e0: 2020 2074 7970 655f 7661 7273 203d 205b     type_vars = [
-000270f0: 7365 7276 6572 5f63 6572 742c 2063 615f  server_cert, ca_
-00027100: 6365 7274 2c20 6372 6c2c 2069 6e74 5f63  cert, crl, int_c
-00027110: 615f 6365 7274 2c20 6f63 7370 5f72 6573  a_cert, ocsp_res
-00027120: 705f 6365 7274 2c20 6f63 7370 5f73 6967  p_cert, ocsp_sig
-00027130: 6e65 725f 6365 7274 2c20 7373 685f 7075  ner_cert, ssh_pu
-00027140: 625f 6b65 795d 0a20 2020 2020 2020 2069  b_key].        i
-00027150: 6620 7479 7065 5f76 6172 732e 636f 756e  f type_vars.coun
-00027160: 7428 5472 7565 2920 3e20 313a 0a20 2020  t(True) > 1:.   
-00027170: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00027180: 616c 7565 4572 726f 7228 2250 726f 7669  alueError("Provi
-00027190: 6465 6420 636f 6e66 6c69 6374 696e 6720  ded conflicting 
-000271a0: 6365 7274 6966 6963 6174 6520 7479 7065  certificate type
-000271b0: 732c 206f 6e6c 7920 3120 7368 6f75 6c64  s, only 1 should
-000271c0: 2062 6520 7365 7420 746f 2054 7275 652e   be set to True.
-000271d0: 2229 0a20 2020 2020 2020 2065 6c69 6620  ").        elif 
-000271e0: 616c 6c28 5b6e 6f74 2062 6f6f 6c28 7661  all([not bool(va
-000271f0: 7229 2066 6f72 2076 6172 2069 6e20 7479  r) for var in ty
-00027200: 7065 5f76 6172 735d 293a 0a20 2020 2020  pe_vars]):.     
-00027210: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00027220: 7565 4572 726f 7228 224e 6f20 6365 7274  ueError("No cert
-00027230: 5f74 7970 6520 7072 6f76 6964 6564 2c20  _type provided, 
-00027240: 6f6e 6520 6f66 2074 6865 2063 6572 745f  one of the cert_
-00027250: 7479 7065 7320 7368 6f75 6c64 2062 6520  types should be 
-00027260: 7365 7420 746f 2054 7275 6522 290a 0a20  set to True").. 
-00027270: 2020 2020 2020 2069 6620 6365 7274 5f66         if cert_f
-00027280: 6f72 6d61 7420 616e 6420 6365 7274 5f66  ormat and cert_f
-00027290: 6f72 6d61 742e 7570 7065 7228 2920 6e6f  ormat.upper() no
-000272a0: 7420 696e 205b 2250 454d 222c 2022 4445  t in ["PEM", "DE
-000272b0: 5222 2c20 2250 4b43 5331 3222 5d3a 0a20  R", "PKCS12"]:. 
-000272c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000272d0: 2056 616c 7565 4572 726f 7228 6622 496e   ValueError(f"In
-000272e0: 7661 6c69 6420 6365 7274 5f66 6f72 6d61  valid cert_forma
-000272f0: 7420 7b63 6572 745f 666f 726d 6174 7d2c  t {cert_format},
-00027300: 2076 616c 6964 2076 616c 7565 7320 6172   valid values ar
-00027310: 6520 2750 454d 272c 2027 4445 5227 2c20  e 'PEM', 'DER', 
-00027320: 2750 4b43 5331 3227 2229 0a20 2020 2020  'PKCS12'").     
-00027330: 2020 2065 6c69 6620 6e6f 7420 6365 7274     elif not cert
-00027340: 5f66 6f72 6d61 7420 616e 6420 6e6f 7420  _format and not 
-00027350: 6365 7274 5f66 696c 653a 0a20 2020 2020  cert_file:.     
-00027360: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00027370: 7565 4572 726f 7228 2263 6572 745f 666f  ueError("cert_fo
-00027380: 726d 6174 2069 7320 7265 7175 6972 6564  rmat is required
-00027390: 2077 6865 6e20 6e6f 7420 7072 6f76 6964   when not provid
-000273a0: 696e 6720 6365 7274 6966 6963 6174 6520  ing certificate 
-000273b0: 7669 6120 6669 6c65 2e22 290a 0a20 2020  via file.")..   
-000273c0: 2020 2020 2069 6620 6e6f 7420 6365 7274       if not cert
-000273d0: 5f64 6174 6120 616e 6420 6e6f 7420 6365  _data and not ce
-000273e0: 7274 5f66 696c 653a 0a20 2020 2020 2020  rt_file:.       
-000273f0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00027400: 4572 726f 7228 224f 6e65 206f 6620 6365  Error("One of ce
-00027410: 7274 5f66 696c 6520 6f72 2063 6572 745f  rt_file or cert_
-00027420: 6461 7461 2073 686f 756c 6420 6265 2070  data should be p
-00027430: 726f 7669 6465 6422 290a 2020 2020 2020  rovided").      
-00027440: 2020 656c 6966 2063 6572 745f 6461 7461    elif cert_data
-00027450: 2061 6e64 2063 6572 745f 6669 6c65 3a0a   and cert_file:.
-00027460: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00027470: 6520 5661 6c75 6545 7272 6f72 2822 4f6e  e ValueError("On
-00027480: 6c79 206f 6e65 206f 6620 6365 7274 5f66  ly one of cert_f
-00027490: 696c 6520 616e 6420 6365 7274 5f64 6174  ile and cert_dat
-000274a0: 6120 7368 6f75 6c64 2062 6520 7072 6f76  a should be prov
-000274b0: 6964 6564 2229 0a0a 2020 2020 2020 2020  ided")..        
-000274c0: 666f 7220 6365 7274 5f74 7970 652c 2076  for cert_type, v
-000274d0: 6172 2069 6e20 7a69 7028 7661 6c69 645f  ar in zip(valid_
-000274e0: 7479 7065 732c 2074 7970 655f 7661 7273  types, type_vars
-000274f0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00027500: 6620 7661 723a 0a20 2020 2020 2020 2020  f var:.         
-00027510: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
-00027520: 2020 2020 2020 6966 2063 6572 745f 6669        if cert_fi
-00027530: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-00027540: 6365 7274 5f66 696c 6520 3d20 5061 7468  cert_file = Path
-00027550: 2863 6572 745f 6669 6c65 2920 6966 206e  (cert_file) if n
-00027560: 6f74 2069 7369 6e73 7461 6e63 6528 6365  ot isinstance(ce
-00027570: 7274 5f66 696c 652c 2050 6174 6829 2065  rt_file, Path) e
-00027580: 6c73 6520 6365 7274 5f66 696c 650a 2020  lse cert_file.  
-00027590: 2020 2020 2020 2020 2020 6365 7274 5f6e            cert_n
-000275a0: 616d 6520 3d20 6365 7274 5f6e 616d 6520  ame = cert_name 
-000275b0: 6f72 2063 6572 745f 6669 6c65 2e73 7465  or cert_file.ste
-000275c0: 6d0a 2020 2020 2020 2020 2020 2020 6966  m.            if
-000275d0: 206e 6f74 2063 6572 745f 666f 726d 6174   not cert_format
-000275e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000275f0: 2020 6966 2063 6572 745f 6669 6c65 2e73    if cert_file.s
-00027600: 7566 6669 782e 6c6f 7765 7228 2920 696e  uffix.lower() in
-00027610: 205b 222e 7066 7822 2c20 222e 7031 3222   [".pfx", ".p12"
-00027620: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00027630: 2020 2020 2020 2063 6572 745f 666f 726d         cert_form
-00027640: 6174 203d 2022 504b 4353 3132 220a 2020  at = "PKCS12".  
-00027650: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00027660: 6966 2063 6572 745f 6669 6c65 2e73 7566  if cert_file.suf
-00027670: 6669 782e 6c6f 7765 7228 2920 696e 205b  fix.lower() in [
-00027680: 222e 7065 6d22 2c20 222e 6365 7222 5d3a  ".pem", ".cer"]:
-00027690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000276a0: 2020 2020 2063 6572 745f 666f 726d 6174       cert_format
-000276b0: 203d 2022 5045 4d22 0a20 2020 2020 2020   = "PEM".       
-000276c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000276d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000276e0: 2020 2023 2054 4f44 4f20 6465 7465 726d     # TODO determ
-000276f0: 696e 6520 666f 726d 6174 2075 7369 6e67  ine format using
-00027700: 2063 7279 7074 6f67 7261 7068 7920 6c69   cryptography li
-00027710: 620a 2020 2020 2020 2020 2020 2020 2020  b.              
-00027720: 2020 2020 2020 6365 7274 5f66 6f72 6d61        cert_forma
-00027730: 7420 3d20 2244 4552 220a 2020 2020 2020  t = "DER".      
-00027740: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00027750: 2020 2020 2020 2020 2020 2020 6365 7274              cert
-00027760: 5f66 6f72 6d61 7420 3d20 6365 7274 5f66  _format = cert_f
-00027770: 6f72 6d61 742e 7570 7065 7228 290a 0a20  ormat.upper().. 
-00027780: 2020 2020 2020 2020 2020 2063 6572 745f             cert_
-00027790: 6461 7461 203d 2063 6572 745f 6669 6c65  data = cert_file
-000277a0: 2e72 6561 645f 7465 7874 2829 0a0a 2020  .read_text()..  
-000277b0: 2020 2020 2020 6365 7274 5f62 7974 6573        cert_bytes
-000277c0: 203d 2063 6572 745f 6461 7461 2e65 6e63   = cert_data.enc
-000277d0: 6f64 6528 2275 7466 2d38 2229 0a20 2020  ode("utf-8").   
-000277e0: 2020 2020 2063 6572 745f 6236 3420 3d20       cert_b64 = 
-000277f0: 6261 7365 3634 2e62 3634 656e 636f 6465  base64.b64encode
-00027800: 2863 6572 745f 6279 7465 7329 2e64 6563  (cert_bytes).dec
-00027810: 6f64 6528 2275 7466 2d38 2229 0a0a 2020  ode("utf-8")..  
-00027820: 2020 2020 2020 6a73 6f6e 5f64 6174 6120        json_data 
-00027830: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00027840: 2763 6572 745f 6e61 6d65 273a 2063 6572  'cert_name': cer
-00027850: 745f 6e61 6d65 2c0a 2020 2020 2020 2020  t_name,.        
-00027860: 2020 2020 2763 6572 745f 7479 7065 273a      'cert_type':
-00027870: 2063 6572 745f 7479 7065 2c0a 2020 2020   cert_type,.    
-00027880: 2020 2020 2020 2020 2763 6572 745f 666f          'cert_fo
-00027890: 726d 6174 273a 2063 6572 745f 666f 726d  rmat': cert_form
-000278a0: 6174 2c0a 2020 2020 2020 2020 2020 2020  at,.            
-000278b0: 2770 6173 7370 6872 6173 6527 3a20 7061  'passphrase': pa
-000278c0: 7373 7068 7261 7365 2c0a 2020 2020 2020  ssphrase,.      
-000278d0: 2020 2020 2020 2763 6572 745f 6461 7461        'cert_data
-000278e0: 273a 2063 6572 745f 6236 340a 2020 2020  ': cert_b64.    
-000278f0: 2020 2020 7d0a 0a20 2020 2020 2020 2072      }..        r
-00027900: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-00027910: 2e70 6f73 7428 7572 6c2c 206a 736f 6e5f  .post(url, json_
-00027920: 6461 7461 3d6a 736f 6e5f 6461 7461 290a  data=json_data).
-00027930: 0a20 2020 2061 7379 6e63 2064 6566 2067  .    async def g
-00027940: 6574 5f73 7562 7363 7269 7074 696f 6e73  et_subscriptions
-00027950: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00027960: 2020 2020 2020 2020 6c69 6365 6e73 655f          license_
-00027970: 7479 7065 3a20 7374 7220 3d20 4e6f 6e65  type: str = None
-00027980: 2c0a 2020 2020 2020 2020 6f66 6673 6574  ,.        offset
-00027990: 3a20 696e 7420 3d20 302c 0a20 2020 2020  : int = 0,.     
-000279a0: 2020 206c 696d 6974 3a20 696e 7420 3d20     limit: int = 
-000279b0: 3130 3030 2c20 2023 2044 6f65 736e 2774  1000,  # Doesn't
-000279c0: 2061 7070 6561 7220 746f 2068 6176 6520   appear to have 
-000279d0: 6d61 782c 2061 6c6c 6f77 6564 2031 306b  max, allowed 10k
-000279e0: 206c 696d 6974 2069 6e20 7377 6167 6765   limit in swagge
-000279f0: 720a 2020 2020 2920 2d3e 2052 6573 706f  r.    ) -> Respo
-00027a00: 6e73 653a 0a20 2020 2020 2020 2022 2222  nse:.        """
-00027a10: 4765 7420 7573 6572 2073 7562 7363 7269  Get user subscri
-00027a20: 7074 696f 6e20 6b65 7973 2e0a 0a20 2020  ption keys...   
-00027a30: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00027a40: 2020 2020 2020 206c 6963 656e 7365 5f74         license_t
-00027a50: 7970 6520 2873 7472 2c20 6f70 7469 6f6e  ype (str, option
-00027a60: 616c 293a 2053 7570 706f 7274 7320 4261  al): Supports Ba
-00027a70: 7369 632c 2053 6572 7669 6365 2054 6f6b  sic, Service Tok
-00027a80: 656e 2061 6e64 204d 756c 7469 2054 6965  en and Multi Tie
-00027a90: 7220 6c69 6365 6e73 696e 6720 7479 7065  r licensing type
-00027aa0: 7320 6173 2077 656c 6c0a 2020 2020 2020  s as well.      
-00027ab0: 2020 2020 2020 6f66 6673 6574 2028 696e        offset (in
-00027ac0: 742c 206f 7074 696f 6e61 6c29 3a20 6f66  t, optional): of
-00027ad0: 6673 6574 206f 7220 7061 6765 206e 756d  fset or page num
-00027ae0: 6265 7220 4465 6661 756c 7473 2074 6f20  ber Defaults to 
-00027af0: 302e 0a20 2020 2020 2020 2020 2020 206c  0..            l
-00027b00: 696d 6974 2028 696e 742c 206f 7074 696f  imit (int, optio
-00027b10: 6e61 6c29 3a20 4e75 6d62 6572 206f 6620  nal): Number of 
-00027b20: 7375 6273 6372 6970 7469 6f6e 7320 746f  subscriptions to
-00027b30: 2067 6574 2044 6566 6175 6c74 7320 746f   get Defaults to
-00027b40: 2031 3030 2e0a 0a20 2020 2020 2020 2052   100...        R
-00027b50: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00027b60: 2020 2020 5265 7370 6f6e 7365 3a20 4365      Response: Ce
-00027b70: 6e74 7261 6c41 5049 2052 6573 706f 6e73  ntralAPI Respons
-00027b80: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
-00027b90: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
-00027ba0: 203d 2022 2f70 6c61 7466 6f72 6d2f 6c69   = "/platform/li
-00027bb0: 6365 6e73 696e 672f 7631 2f73 7562 7363  censing/v1/subsc
-00027bc0: 7269 7074 696f 6e73 220a 0a20 2020 2020  riptions"..     
-00027bd0: 2020 2070 6172 616d 7320 3d20 7b0a 2020     params = {.  
-00027be0: 2020 2020 2020 2020 2020 276c 6963 656e            'licen
-00027bf0: 7365 5f74 7970 6527 3a20 6c69 6365 6e73  se_type': licens
-00027c00: 655f 7479 7065 2c0a 2020 2020 2020 2020  e_type,.        
-00027c10: 2020 2020 276f 6666 7365 7427 3a20 6f66      'offset': of
-00027c20: 6673 6574 2c0a 2020 2020 2020 2020 2020  fset,.          
-00027c30: 2020 276c 696d 6974 273a 206c 696d 6974    'limit': limit
-00027c40: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-00027c50: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-00027c60: 2073 656c 662e 6765 7428 7572 6c2c 2070   self.get(url, p
-00027c70: 6172 616d 733d 7061 7261 6d73 290a 0a20  arams=params).. 
-00027c80: 2020 2061 7379 6e63 2064 6566 2067 6574     async def get
-00027c90: 5f73 7562 7363 7269 7074 696f 6e5f 7374  _subscription_st
-00027ca0: 6174 7328 0a20 2020 2020 2020 2073 656c  ats(.        sel
-00027cb0: 662c 0a20 2020 2020 2020 206c 6963 656e  f,.        licen
-00027cc0: 7365 5f74 7970 653a 2073 7472 203d 2027  se_type: str = '
-00027cd0: 616c 6c27 2c0a 2020 2020 2020 2020 7365  all',.        se
-00027ce0: 7276 6963 653a 2073 7472 203d 204e 6f6e  rvice: str = Non
-00027cf0: 652c 0a20 2020 2020 2020 2061 7070 5f6f  e,.        app_o
-00027d00: 6e6c 795f 7374 6174 733a 2062 6f6f 6c20  nly_stats: bool 
-00027d10: 3d20 4e6f 6e65 2c0a 2020 2020 2920 2d3e  = None,.    ) ->
-00027d20: 2052 6573 706f 6e73 653a 0a20 2020 2020   Response:.     
-00027d30: 2020 2022 2222 4765 7420 7375 6273 6372     """Get subscr
-00027d40: 6970 7469 6f6e 2073 7461 7473 2e0a 0a20  iption stats... 
-00027d50: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00027d60: 2020 2020 2020 2020 206c 6963 656e 7365           license
-00027d70: 5f74 7970 6520 2873 7472 2c20 6f70 7469  _type (str, opti
-00027d80: 6f6e 616c 293a 2053 7570 706f 7274 7320  onal): Supports 
-00027d90: 6261 7369 632f 7370 6563 6961 6c2f 616c  basic/special/al
-00027da0: 6c2e 0a20 2020 2020 2020 2020 2020 2020  l..             
-00027db0: 2020 2073 7065 6369 616c 202d 2077 696c     special - wil
-00027dc0: 6c20 6665 7463 6820 7468 6520 7374 6174  l fetch the stat
-00027dd0: 6973 7469 6373 206f 6620 7370 6563 6961  istics of specia
-00027de0: 6c20 6365 6e74 7261 6c20 7365 7276 6963  l central servic
-00027df0: 6573 206c 696b 6520 7061 2c20 7563 632c  es like pa, ucc,
-00027e00: 2063 6c61 7269 7479 2065 7463 2e0a 2020   clarity etc..  
-00027e10: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-00027e20: 7369 6320 2d20 7769 6c6c 2066 6574 6368  sic - will fetch
-00027e30: 2074 6865 2073 7461 7469 7374 6963 7320   the statistics 
-00027e40: 6f66 2064 6576 6963 6520 6d61 6e61 6765  of device manage
-00027e50: 6d65 6e74 2073 6572 7669 6365 206c 6963  ment service lic
-00027e60: 656e 7365 732e 0a20 2020 2020 2020 2020  enses..         
-00027e70: 2020 2020 2020 2061 6c6c 202d 2077 696c         all - wil
-00027e80: 6c20 6665 7463 6820 626f 7468 206f 6620  l fetch both of 
-00027e90: 7468 6573 6520 6c69 6365 6e73 6520 7479  these license ty
-00027ea0: 7065 732e 0a0a 2020 2020 2020 2020 2020  pes...          
-00027eb0: 2020 2020 2020 416c 736f 2073 7570 706f        Also suppo
-00027ec0: 7274 7320 6d75 6c74 6920 7469 6572 206c  rts multi tier l
-00027ed0: 6963 656e 7365 2074 7970 6573 2073 7563  icense types suc
-00027ee0: 6820 666f 756e 6461 7469 6f6e 5f61 702c  h foundation_ap,
-00027ef0: 2061 6476 616e 6365 645f 7377 6974 6368   advanced_switch
-00027f00: 5f36 3330 302c 0a20 2020 2020 2020 2020  _6300,.         
-00027f10: 2020 2020 2020 2066 6f75 6e64 6174 696f         foundatio
-00027f20: 6e5f 3730 5858 2065 7463 2e0a 0a20 2020  n_70XX etc...   
-00027f30: 2020 2020 2020 2020 2073 6572 7669 6365           service
-00027f40: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-00027f50: 3a20 5365 7276 6963 6520 7479 7065 3a20  : Service type: 
-00027f60: 7061 2f70 612c 636c 6172 6974 792c 666f  pa/pa,clarity,fo
-00027f70: 756e 6461 7469 6f6e 5f61 702c 0a20 2020  undation_ap,.   
-00027f80: 2020 2020 2020 2020 2020 2020 2061 6476               adv
-00027f90: 616e 6365 645f 7377 6974 6368 5f36 3330  anced_switch_630
-00027fa0: 302c 2066 6f75 6e64 6174 696f 6e5f 3730  0, foundation_70
-00027fb0: 5858 2020 6574 632e 0a20 2020 2020 2020  XX  etc..       
-00027fc0: 2020 2020 2061 7070 5f6f 6e6c 795f 7374       app_only_st
-00027fd0: 6174 7320 2862 6f6f 6c2c 206f 7074 696f  ats (bool, optio
-00027fe0: 6e61 6c29 3a20 4966 2076 616c 7565 2069  nal): If value i
-00027ff0: 7320 5472 7565 2c20 7374 6174 7320 6f6e  s True, stats on
-00028000: 6c79 2066 6f72 2074 6865 2063 7572 7265  ly for the curre
-00028010: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
-00028020: 2020 2061 7070 6c69 6361 7469 6f6e 2072     application r
-00028030: 6574 7572 6e65 6420 7261 7468 6572 2074  eturned rather t
-00028040: 6861 6e20 676c 6f62 616c 2073 7461 7473  han global stats
-00028050: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00028060: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-00028070: 6573 706f 6e73 653a 2043 656e 7472 616c  esponse: Central
-00028080: 4150 4920 5265 7370 6f6e 7365 206f 626a  API Response obj
-00028090: 6563 740a 2020 2020 2020 2020 2222 220a  ect.        """.
-000280a0: 2020 2020 2020 2020 7572 6c20 3d20 222f          url = "/
-000280b0: 706c 6174 666f 726d 2f6c 6963 656e 7369  platform/licensi
-000280c0: 6e67 2f76 312f 7375 6273 6372 6970 7469  ng/v1/subscripti
-000280d0: 6f6e 732f 7374 6174 7322 0a0a 2020 2020  ons/stats"..    
-000280e0: 2020 2020 7061 7261 6d73 203d 207b 0a20      params = {. 
-000280f0: 2020 2020 2020 2020 2020 2027 6c69 6365             'lice
-00028100: 6e73 655f 7479 7065 273a 206c 6963 656e  nse_type': licen
-00028110: 7365 5f74 7970 652c 0a20 2020 2020 2020  se_type,.       
-00028120: 2020 2020 2027 7365 7276 6963 6527 3a20       'service': 
-00028130: 7365 7276 6963 652c 0a20 2020 2020 2020  service,.       
-00028140: 2020 2020 2027 6170 705f 6f6e 6c79 5f73       'app_only_s
-00028150: 7461 7473 273a 2061 7070 5f6f 6e6c 795f  tats': app_only_
-00028160: 7374 6174 730a 2020 2020 2020 2020 7d0a  stats.        }.
-00028170: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00028180: 6177 6169 7420 7365 6c66 2e67 6574 2875  await self.get(u
-00028190: 726c 2c20 7061 7261 6d73 3d70 6172 616d  rl, params=param
-000281a0: 7329 0a0a 2020 2020 6173 796e 6320 6465  s)..    async de
-000281b0: 6620 6765 745f 7661 6c69 645f 7375 6273  f get_valid_subs
-000281c0: 6372 6970 7469 6f6e 5f6e 616d 6573 280a  cription_names(.
-000281d0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000281e0: 2020 2020 2020 7365 7276 6963 655f 6361        service_ca
-000281f0: 7465 676f 7279 3a20 7374 7220 3d20 4e6f  tegory: str = No
-00028200: 6e65 2c0a 2020 2020 2020 2020 6465 7669  ne,.        devi
-00028210: 6365 5f74 7970 653a 2073 7472 203d 204e  ce_type: str = N
-00028220: 6f6e 652c 0a20 2020 2029 202d 3e20 5265  one,.    ) -> Re
-00028230: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
-00028240: 2222 2247 6574 2056 616c 6964 2073 7562  """Get Valid sub
-00028250: 7363 7269 7074 696f 6e20 6e61 6d65 7320  scription names 
-00028260: 6672 6f6d 2043 656e 7472 616c 2e0a 0a20  from Central... 
-00028270: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00028280: 2020 2020 2020 2020 2073 6572 7669 6365           service
-00028290: 5f63 6174 6567 6f72 7920 2873 7472 2c20  _category (str, 
-000282a0: 6f70 7469 6f6e 616c 293a 2053 6572 7669  optional): Servi
-000282b0: 6365 2063 6174 6567 6f72 7920 2d20 646d  ce category - dm
-000282c0: 2f6e 6574 776f 726b 0a20 2020 2020 2020  /network.       
-000282d0: 2020 2020 2064 6576 6963 655f 7479 7065       device_type
-000282e0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-000282f0: 3a20 4465 7669 6365 2054 7970 6520 2d20  : Device Type - 
-00028300: 6961 702f 6361 702f 7377 6974 6368 2f62  iap/cap/switch/b
-00028310: 6f63 2f63 6f6e 7472 6f6c 6c65 720a 0a20  oc/controller.. 
-00028320: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00028330: 2020 2020 2020 2020 2020 2020 5265 7370              Resp
-00028340: 6f6e 7365 3a20 4365 6e74 7261 6c41 5049  onse: CentralAPI
-00028350: 2052 6573 706f 6e73 6520 6f62 6a65 6374   Response object
-00028360: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00028370: 2020 2020 2075 726c 203d 2022 2f70 6c61       url = "/pla
-00028380: 7466 6f72 6d2f 6c69 6365 6e73 696e 672f  tform/licensing/
-00028390: 7631 2f73 6572 7669 6365 732f 636f 6e66  v1/services/conf
-000283a0: 6967 220a 0a20 2020 2020 2020 2070 6172  ig"..        par
-000283b0: 616d 7320 3d20 7b0a 2020 2020 2020 2020  ams = {.        
-000283c0: 2020 2020 2773 6572 7669 6365 5f63 6174      'service_cat
-000283d0: 6567 6f72 7927 3a20 7365 7276 6963 655f  egory': service_
-000283e0: 6361 7465 676f 7279 2c0a 2020 2020 2020  category,.      
-000283f0: 2020 2020 2020 2764 6576 6963 655f 7479        'device_ty
-00028400: 7065 273a 2064 6576 6963 655f 7479 7065  pe': device_type
-00028410: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-00028420: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-00028430: 2073 656c 662e 6765 7428 7572 6c2c 2070   self.get(url, p
-00028440: 6172 616d 733d 7061 7261 6d73 290a 0a20  arams=params).. 
-00028450: 2020 2061 7379 6e63 2064 6566 2061 7373     async def ass
-00028460: 6967 6e5f 6c69 6365 6e73 6573 2873 656c  ign_licenses(sel
-00028470: 662c 2073 6572 6961 6c73 3a20 556e 696f  f, serials: Unio
-00028480: 6e5b 7374 722c 204c 6973 745b 7374 725d  n[str, List[str]
-00028490: 5d2c 2073 6572 7669 6365 733a 2055 6e69  ], services: Uni
-000284a0: 6f6e 5b73 7472 2c20 4c69 7374 5b73 7472  on[str, List[str
-000284b0: 5d5d 2920 2d3e 2052 6573 706f 6e73 653a  ]]) -> Response:
-000284c0: 0a20 2020 2020 2020 2022 2222 4173 7369  .        """Assi
-000284d0: 676e 2073 7562 7363 7269 7074 696f 6e20  gn subscription 
-000284e0: 746f 2061 2064 6576 6963 652e 0a0a 2020  to a device...  
-000284f0: 2020 2020 2020 2f2f 2055 7365 6420 696e        // Used in
-00028500: 6469 7265 6374 6c79 2062 7920 6164 6420  directly by add 
-00028510: 6465 7669 6365 2077 6865 6e20 2d2d 6c69  device when --li
-00028520: 6365 6e73 6520 3c6c 6963 656e 7365 3e20  cense <license> 
-00028530: 6973 2070 726f 7669 6465 6420 616e 6420  is provided and 
-00028540: 6261 7463 6820 6164 6420 6465 7669 6365  batch add device
-00028550: 7320 7769 7468 206c 6963 656e 7365 202f  s with license /
-00028560: 2f0a 0a20 2020 2020 2020 2041 7267 733a  /..        Args:
-00028570: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
-00028580: 6961 6c73 2028 7374 7220 7c20 4c69 7374  ials (str | List
-00028590: 5b73 7472 5d29 3a20 4c69 7374 206f 6620  [str]): List of 
-000285a0: 7365 7269 616c 206e 756d 6265 7220 6f66  serial number of
-000285b0: 2064 6576 6963 652e 0a20 2020 2020 2020   device..       
-000285c0: 2020 2020 2073 6572 7669 6365 7320 2873       services (s
-000285d0: 7472 207c 204c 6973 745b 7374 725d 293a  tr | List[str]):
-000285e0: 204c 6973 7420 6f66 2073 6572 7669 6365   List of service
-000285f0: 206e 616d 6573 2e20 4361 6c6c 2073 6572   names. Call ser
-00028600: 7669 6365 732f 636f 6e66 6967 2041 5049  vices/config API
-00028610: 2074 6f20 6765 7420 7468 6520 6c69 7374   to get the list
-00028620: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
-00028630: 2020 2020 7661 6c69 6420 7365 7276 6963      valid servic
-00028640: 6520 6e61 6d65 732e 0a0a 2020 2020 2020  e names...      
-00028650: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00028660: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
-00028670: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
-00028680: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
-00028690: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000286a0: 7572 6c20 3d20 222f 706c 6174 666f 726d  url = "/platform
-000286b0: 2f6c 6963 656e 7369 6e67 2f76 312f 7375  /licensing/v1/su
-000286c0: 6273 6372 6970 7469 6f6e 732f 6173 7369  bscriptions/assi
-000286d0: 676e 220a 2020 2020 2020 2020 7365 7269  gn".        seri
-000286e0: 616c 7320 3d20 7574 696c 732e 6c69 7374  als = utils.list
-000286f0: 6966 7928 7365 7269 616c 7329 0a20 2020  ify(serials).   
-00028700: 2020 2020 2073 6572 7669 6365 7320 3d20       services = 
-00028710: 7574 696c 732e 6c69 7374 6966 7928 7365  utils.listify(se
-00028720: 7276 6963 6573 290a 0a20 2020 2020 2020  rvices)..       
-00028730: 206a 736f 6e5f 6461 7461 203d 207b 0a20   json_data = {. 
-00028740: 2020 2020 2020 2020 2020 2027 7365 7269             'seri
-00028750: 616c 7327 3a20 7365 7269 616c 732c 0a20  als': serials,. 
-00028760: 2020 2020 2020 2020 2020 2027 7365 7276             'serv
-00028770: 6963 6573 273a 2073 6572 7669 6365 730a  ices': services.
-00028780: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00028790: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-000287a0: 7365 6c66 2e70 6f73 7428 7572 6c2c 206a  self.post(url, j
-000287b0: 736f 6e5f 6461 7461 3d6a 736f 6e5f 6461  son_data=json_da
-000287c0: 7461 290a 0a20 2020 2061 7379 6e63 2064  ta)..    async d
-000287d0: 6566 2075 6e61 7373 6967 6e5f 6c69 6365  ef unassign_lice
-000287e0: 6e73 6573 2873 656c 662c 2073 6572 6961  nses(self, seria
-000287f0: 6c73 3a20 556e 696f 6e5b 7374 722c 204c  ls: Union[str, L
-00028800: 6973 745b 7374 725d 5d2c 2073 6572 7669  ist[str]], servi
-00028810: 6365 733a 2055 6e69 6f6e 5b73 7472 2c20  ces: Union[str, 
-00028820: 4c69 7374 5b73 7472 5d5d 2920 2d3e 2052  List[str]]) -> R
-00028830: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
-00028840: 2022 2222 556e 6173 7369 676e 2073 7562   """Unassign sub
-00028850: 7363 7269 7074 696f 6e28 7329 2066 726f  scription(s) fro
-00028860: 6d20 6465 7669 6365 2873 292e 0a0a 2020  m device(s)...  
-00028870: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00028880: 2020 2020 2020 2020 7365 7269 616c 7320          serials 
-00028890: 2873 7472 207c 204c 6973 745b 7374 725d  (str | List[str]
-000288a0: 293a 204c 6973 7420 6f66 2073 6572 6961  ): List of seria
-000288b0: 6c20 6e75 6d62 6572 206f 6620 6465 7669  l number of devi
-000288c0: 6365 2e0a 2020 2020 2020 2020 2020 2020  ce..            
-000288d0: 7365 7276 6963 6573 2028 7374 7220 7c20  services (str | 
-000288e0: 4c69 7374 5b73 7472 5d29 3a20 4c69 7374  List[str]): List
-000288f0: 206f 6620 7365 7276 6963 6520 6e61 6d65   of service name
-00028900: 732e 2043 616c 6c20 7365 7276 6963 6573  s. Call services
-00028910: 2f63 6f6e 6669 6720 4150 4920 746f 2067  /config API to g
-00028920: 6574 2074 6865 206c 6973 7420 6f66 0a20  et the list of. 
-00028930: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00028940: 616c 6964 2073 6572 7669 6365 206e 616d  alid service nam
-00028950: 6573 2e0a 0a20 2020 2020 2020 2052 6574  es...        Ret
-00028960: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00028970: 2020 5265 7370 6f6e 7365 3a20 4365 6e74    Response: Cent
-00028980: 7261 6c41 5049 2052 6573 706f 6e73 6520  ralAPI Response 
-00028990: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
-000289a0: 2222 0a20 2020 2020 2020 2075 726c 203d  "".        url =
-000289b0: 2022 2f70 6c61 7466 6f72 6d2f 6c69 6365   "/platform/lice
-000289c0: 6e73 696e 672f 7631 2f73 7562 7363 7269  nsing/v1/subscri
-000289d0: 7074 696f 6e73 2f75 6e61 7373 6967 6e22  ptions/unassign"
-000289e0: 0a20 2020 2020 2020 2073 6572 6961 6c73  .        serials
-000289f0: 203d 2075 7469 6c73 2e6c 6973 7469 6679   = utils.listify
-00028a00: 2873 6572 6961 6c73 290a 2020 2020 2020  (serials).      
-00028a10: 2020 7365 7276 6963 6573 203d 2075 7469    services = uti
-00028a20: 6c73 2e6c 6973 7469 6679 2873 6572 7669  ls.listify(servi
-00028a30: 6365 7329 0a0a 2020 2020 2020 2020 6a73  ces)..        js
-00028a40: 6f6e 5f64 6174 6120 3d20 7b0a 2020 2020  on_data = {.    
-00028a50: 2020 2020 2020 2020 2773 6572 6961 6c73          'serials
-00028a60: 273a 2073 6572 6961 6c73 2c0a 2020 2020  ': serials,.    
-00028a70: 2020 2020 2020 2020 2773 6572 7669 6365          'service
-00028a80: 7327 3a20 7365 7276 6963 6573 0a20 2020  s': services.   
-00028a90: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-00028aa0: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
-00028ab0: 662e 706f 7374 2875 726c 2c20 6a73 6f6e  f.post(url, json
-00028ac0: 5f64 6174 613d 6a73 6f6e 5f64 6174 6129  _data=json_data)
-00028ad0: 0a0a 2020 2020 2320 544f 444f 2062 7569  ..    # TODO bui
-00028ae0: 6c64 2061 6767 7265 6761 746f 7220 746f  ld aggregator to
-00028af0: 2072 756e 2072 6570 6f72 7420 7368 6f77   run report show
-00028b00: 696e 6720 726f 6775 6573 2f69 6e74 6572  ing rogues/inter
-00028b10: 6665 7269 6e67 2f6e 6569 6768 626f 7273  fering/neighbors
-00028b20: 0a20 2020 2023 2061 7379 6e63 2064 6566  .    # async def
-00028b30: 2077 6964 735f 6765 745f 616c 6c28 7365   wids_get_all(se
-00028b40: 6c66 293a 0a0a 2020 2020 6173 796e 6320  lf):..    async 
-00028b50: 6465 6620 7769 6473 5f67 6574 5f72 6f67  def wids_get_rog
-00028b60: 7565 5f61 7073 280a 2020 2020 2020 2020  ue_aps(.        
-00028b70: 7365 6c66 2c0a 2020 2020 2020 2020 6772  self,.        gr
-00028b80: 6f75 703a 204c 6973 745b 7374 725d 203d  oup: List[str] =
-00028b90: 204e 6f6e 652c 0a20 2020 2020 2020 206c   None,.        l
-00028ba0: 6162 656c 3a20 4c69 7374 5b73 7472 5d20  abel: List[str] 
-00028bb0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00028bc0: 7369 7465 3a20 4c69 7374 5b73 7472 5d20  site: List[str] 
-00028bd0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00028be0: 7374 6172 743a 2069 6e74 203d 204e 6f6e  start: int = Non
-00028bf0: 652c 0a20 2020 2020 2020 2065 6e64 3a20  e,.        end: 
-00028c00: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-00028c10: 2020 2020 7377 6172 6d5f 6964 3a20 7374      swarm_id: st
-00028c20: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00028c30: 2020 6672 6f6d 5f74 696d 6573 7461 6d70    from_timestamp
-00028c40: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-00028c50: 2020 2020 2020 746f 5f74 696d 6573 7461        to_timesta
-00028c60: 6d70 3a20 696e 7420 3d20 4e6f 6e65 2c0a  mp: int = None,.
-00028c70: 2020 2020 2020 2020 6f66 6673 6574 3a20          offset: 
-00028c80: 696e 7420 3d20 302c 0a20 2020 2020 2020  int = 0,.       
-00028c90: 206c 696d 6974 3a20 696e 7420 3d20 3130   limit: int = 10
-00028ca0: 300a 2020 2020 2920 2d3e 2052 6573 706f  0.    ) -> Respo
-00028cb0: 6e73 653a 0a20 2020 2020 2020 2022 2222  nse:.        """
-00028cc0: 4c69 7374 2052 6f67 7565 2041 5073 2e0a  List Rogue APs..
-00028cd0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00028ce0: 2020 2020 2020 2020 2020 2067 726f 7570             group
-00028cf0: 2028 4c69 7374 5b73 7472 5d2c 206f 7074   (List[str], opt
-00028d00: 696f 6e61 6c29 3a20 4c69 7374 206f 6620  ional): List of 
-00028d10: 6772 6f75 7020 6e61 6d65 730a 2020 2020  group names.    
-00028d20: 2020 2020 2020 2020 6c61 6265 6c20 284c          label (L
-00028d30: 6973 745b 7374 725d 2c20 6f70 7469 6f6e  ist[str], option
-00028d40: 616c 293a 204c 6973 7420 6f66 206c 6162  al): List of lab
-00028d50: 656c 206e 616d 6573 0a20 2020 2020 2020  el names.       
-00028d60: 2020 2020 2073 6974 6520 284c 6973 745b       site (List[
-00028d70: 7374 725d 2c20 6f70 7469 6f6e 616c 293a  str], optional):
-00028d80: 204c 6973 7420 6f66 2073 6974 6520 6e61   List of site na
-00028d90: 6d65 730a 2020 2020 2020 2020 2020 2020  mes.            
-00028da0: 7374 6172 7420 2869 6e74 2c20 6f70 7469  start (int, opti
-00028db0: 6f6e 616c 293a 204e 6565 6420 696e 666f  onal): Need info
-00028dc0: 726d 6174 696f 6e20 6672 6f6d 2074 6869  rmation from thi
-00028dd0: 7320 7469 6d65 7374 616d 702e 2054 696d  s timestamp. Tim
-00028de0: 6573 7461 6d70 2069 7320 6570 6f63 6820  estamp is epoch 
-00028df0: 696e 0a20 2020 2020 2020 2020 2020 2020  in.             
-00028e00: 2020 206d 696c 6c69 7365 636f 6e64 732e     milliseconds.
-00028e10: 2044 6566 6175 6c74 2069 7320 6375 7272   Default is curr
-00028e20: 656e 7420 7469 6d65 7374 616d 7020 6d69  ent timestamp mi
-00028e30: 6e75 7320 3320 686f 7572 730a 2020 2020  nus 3 hours.    
-00028e40: 2020 2020 2020 2020 656e 6420 2869 6e74          end (int
-00028e50: 2c20 6f70 7469 6f6e 616c 293a 204e 6565  , optional): Nee
-00028e60: 6420 696e 666f 726d 6174 696f 6e20 746f  d information to
-00028e70: 2074 6869 7320 7469 6d65 7374 616d 702e   this timestamp.
-00028e80: 2054 696d 6573 7461 6d70 2069 7320 6570   Timestamp is ep
-00028e90: 6f63 6820 696e 0a20 2020 2020 2020 2020  och in.         
-00028ea0: 2020 2020 2020 206d 696c 6c69 7365 636f         milliseco
-00028eb0: 6e64 732e 2044 6566 6175 6c74 2069 7320  nds. Default is 
-00028ec0: 6375 7272 656e 7420 7469 6d65 7374 616d  current timestam
-00028ed0: 700a 2020 2020 2020 2020 2020 2020 7377  p.            sw
-00028ee0: 6172 6d5f 6964 2028 7374 722c 206f 7074  arm_id (str, opt
-00028ef0: 696f 6e61 6c29 3a20 4669 6c74 6572 2062  ional): Filter b
-00028f00: 7920 5377 6172 6d20 4944 0a20 2020 2020  y Swarm ID.     
-00028f10: 2020 2020 2020 2066 726f 6d5f 7469 6d65         from_time
-00028f20: 7374 616d 7020 2869 6e74 2c20 6f70 7469  stamp (int, opti
-00028f30: 6f6e 616c 293a 2054 6869 7320 7061 7261  onal): This para
-00028f40: 6d65 7465 7220 7375 7065 7263 6564 6573  meter supercedes
-00028f50: 2073 7461 7274 2070 6172 616d 6574 6572   start parameter
-00028f60: 2e20 4e65 6564 0a20 2020 2020 2020 2020  . Need.         
-00028f70: 2020 2020 2020 2069 6e66 6f72 6d61 7469         informati
-00028f80: 6f6e 2066 726f 6d20 7468 6973 2074 696d  on from this tim
-00028f90: 6573 7461 6d70 2e20 5469 6d65 7374 616d  estamp. Timestam
-00028fa0: 7020 6973 2065 706f 6368 2069 6e20 7365  p is epoch in se
-00028fb0: 636f 6e64 732e 2044 6566 6175 6c74 2069  conds. Default i
-00028fc0: 7320 6375 7272 656e 740a 2020 2020 2020  s current.      
-00028fd0: 2020 2020 2020 2020 2020 5554 4320 7469            UTC ti
-00028fe0: 6d65 7374 616d 7020 6d69 6e75 7320 3320  mestamp minus 3 
-00028ff0: 686f 7572 730a 2020 2020 2020 2020 2020  hours.          
-00029000: 2020 746f 5f74 696d 6573 7461 6d70 2028    to_timestamp (
-00029010: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
-00029020: 5468 6973 2070 6172 616d 6574 6572 2073  This parameter s
-00029030: 7570 6572 6365 6465 7320 656e 6420 7061  upercedes end pa
-00029040: 7261 6d65 7465 722e 204e 6565 6420 696e  rameter. Need in
-00029050: 666f 726d 6174 696f 6e0a 2020 2020 2020  formation.      
-00029060: 2020 2020 2020 2020 2020 746f 2074 6869            to thi
-00029070: 7320 7469 6d65 7374 616d 702e 2054 696d  s timestamp. Tim
-00029080: 6573 7461 6d70 2069 7320 6570 6f63 6820  estamp is epoch 
-00029090: 696e 2073 6563 6f6e 6473 2e20 4465 6661  in seconds. Defa
-000290a0: 756c 7420 6973 2063 7572 7265 6e74 2055  ult is current U
-000290b0: 5443 2074 696d 6573 7461 6d70 0a20 2020  TC timestamp.   
-000290c0: 2020 2020 2020 2020 206f 6666 7365 7420           offset 
-000290d0: 2869 6e74 2c20 6f70 7469 6f6e 616c 293a  (int, optional):
-000290e0: 2050 6167 696e 6174 696f 6e20 6f66 6673   Pagination offs
-000290f0: 6574 2028 6465 6661 756c 7420 3d20 3029  et (default = 0)
-00029100: 2044 6566 6175 6c74 7320 746f 2030 2e0a   Defaults to 0..
-00029110: 2020 2020 2020 2020 2020 2020 6c69 6d69              limi
-00029120: 7420 2869 6e74 2c20 6f70 7469 6f6e 616c  t (int, optional
-00029130: 293a 2070 6167 696e 6174 696f 6e20 7369  ): pagination si
-00029140: 7a65 2028 6465 6661 756c 7420 3d20 3130  ze (default = 10
-00029150: 3029 2044 6566 6175 6c74 7320 746f 2031  0) Defaults to 1
-00029160: 3030 2e0a 0a20 2020 2020 2020 2052 6574  00...        Ret
-00029170: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00029180: 2020 5265 7370 6f6e 7365 3a20 4365 6e74    Response: Cent
-00029190: 7261 6c41 5049 2052 6573 706f 6e73 6520  ralAPI Response 
-000291a0: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
-000291b0: 2222 0a20 2020 2020 2020 2075 726c 203d  "".        url =
-000291c0: 2022 2f72 6170 6964 732f 7631 2f72 6f67   "/rapids/v1/rog
-000291d0: 7565 5f61 7073 220a 0a20 2020 2020 2020  ue_aps"..       
-000291e0: 2070 6172 616d 7320 3d20 7b0a 2020 2020   params = {.    
-000291f0: 2020 2020 2020 2020 2767 726f 7570 273a          'group':
-00029200: 2067 726f 7570 2c0a 2020 2020 2020 2020   group,.        
-00029210: 2020 2020 276c 6162 656c 273a 206c 6162      'label': lab
-00029220: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
-00029230: 2773 6974 6527 3a20 7369 7465 2c0a 2020  'site': site,.  
-00029240: 2020 2020 2020 2020 2020 2773 7461 7274            'start
-00029250: 273a 2073 7461 7274 2c0a 2020 2020 2020  ': start,.      
-00029260: 2020 2020 2020 2765 6e64 273a 2065 6e64        'end': end
-00029270: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
-00029280: 7761 726d 5f69 6427 3a20 7377 6172 6d5f  warm_id': swarm_
-00029290: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-000292a0: 2766 726f 6d5f 7469 6d65 7374 616d 7027  'from_timestamp'
-000292b0: 3a20 6672 6f6d 5f74 696d 6573 7461 6d70  : from_timestamp
-000292c0: 2c0a 2020 2020 2020 2020 2020 2020 2774  ,.            't
-000292d0: 6f5f 7469 6d65 7374 616d 7027 3a20 746f  o_timestamp': to
-000292e0: 5f74 696d 6573 7461 6d70 2c0a 2020 2020  _timestamp,.    
-000292f0: 2020 2020 2020 2020 276f 6666 7365 7427          'offset'
-00029300: 3a20 6f66 6673 6574 2c0a 2020 2020 2020  : offset,.      
-00029310: 2020 2020 2020 276c 696d 6974 273a 206c        'limit': l
-00029320: 696d 6974 0a20 2020 2020 2020 207d 0a0a  imit.        }..
-00029330: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00029340: 7761 6974 2073 656c 662e 6765 7428 7572  wait self.get(ur
-00029350: 6c2c 2070 6172 616d 733d 7061 7261 6d73  l, params=params
-00029360: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-00029370: 2077 6964 735f 6765 745f 696e 7465 7266   wids_get_interf
-00029380: 6572 696e 675f 6170 7328 0a20 2020 2020  ering_aps(.     
-00029390: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-000293a0: 2067 726f 7570 3a20 4c69 7374 5b73 7472   group: List[str
-000293b0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-000293c0: 2020 6c61 6265 6c3a 204c 6973 745b 7374    label: List[st
-000293d0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-000293e0: 2020 2073 6974 653a 204c 6973 745b 7374     site: List[st
-000293f0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00029400: 2020 2073 7461 7274 3a20 696e 7420 3d20     start: int = 
-00029410: 4e6f 6e65 2c0a 2020 2020 2020 2020 656e  None,.        en
-00029420: 643a 2069 6e74 203d 204e 6f6e 652c 0a20  d: int = None,. 
-00029430: 2020 2020 2020 2073 7761 726d 5f69 643a         swarm_id:
-00029440: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00029450: 2020 2020 2066 726f 6d5f 7469 6d65 7374       from_timest
-00029460: 616d 703a 2069 6e74 203d 204e 6f6e 652c  amp: int = None,
-00029470: 0a20 2020 2020 2020 2074 6f5f 7469 6d65  .        to_time
-00029480: 7374 616d 703a 2069 6e74 203d 204e 6f6e  stamp: int = Non
-00029490: 652c 0a20 2020 2020 2020 206f 6666 7365  e,.        offse
-000294a0: 743a 2069 6e74 203d 2030 2c0a 2020 2020  t: int = 0,.    
-000294b0: 2020 2020 6c69 6d69 743a 2069 6e74 203d      limit: int =
-000294c0: 2031 3030 0a20 2020 2029 202d 3e20 5265   100.    ) -> Re
-000294d0: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
-000294e0: 2222 224c 6973 7420 496e 7465 7266 6572  """List Interfer
-000294f0: 696e 6720 4150 732e 0a0a 2020 2020 2020  ing APs...      
-00029500: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00029510: 2020 2020 6772 6f75 7020 284c 6973 745b      group (List[
-00029520: 7374 725d 2c20 6f70 7469 6f6e 616c 293a  str], optional):
-00029530: 204c 6973 7420 6f66 2067 726f 7570 206e   List of group n
-00029540: 616d 6573 0a20 2020 2020 2020 2020 2020  ames.           
-00029550: 206c 6162 656c 2028 4c69 7374 5b73 7472   label (List[str
-00029560: 5d2c 206f 7074 696f 6e61 6c29 3a20 4c69  ], optional): Li
-00029570: 7374 206f 6620 6c61 6265 6c20 6e61 6d65  st of label name
-00029580: 730a 2020 2020 2020 2020 2020 2020 7369  s.            si
-00029590: 7465 2028 4c69 7374 5b73 7472 5d2c 206f  te (List[str], o
-000295a0: 7074 696f 6e61 6c29 3a20 4c69 7374 206f  ptional): List o
-000295b0: 6620 7369 7465 206e 616d 6573 0a20 2020  f site names.   
-000295c0: 2020 2020 2020 2020 2073 7461 7274 2028           start (
-000295d0: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
-000295e0: 4e65 6564 2069 6e66 6f72 6d61 7469 6f6e  Need information
-000295f0: 2066 726f 6d20 7468 6973 2074 696d 6573   from this times
-00029600: 7461 6d70 2e20 5469 6d65 7374 616d 7020  tamp. Timestamp 
-00029610: 6973 2065 706f 6368 2069 6e0a 2020 2020  is epoch in.    
-00029620: 2020 2020 2020 2020 2020 2020 6d69 6c6c              mill
-00029630: 6973 6563 6f6e 6473 2e20 4465 6661 756c  iseconds. Defaul
-00029640: 7420 6973 2063 7572 7265 6e74 2074 696d  t is current tim
-00029650: 6573 7461 6d70 206d 696e 7573 2033 2068  estamp minus 3 h
-00029660: 6f75 7273 0a20 2020 2020 2020 2020 2020  ours.           
-00029670: 2065 6e64 2028 696e 742c 206f 7074 696f   end (int, optio
-00029680: 6e61 6c29 3a20 4e65 6564 2069 6e66 6f72  nal): Need infor
-00029690: 6d61 7469 6f6e 2074 6f20 7468 6973 2074  mation to this t
-000296a0: 696d 6573 7461 6d70 2e20 5469 6d65 7374  imestamp. Timest
-000296b0: 616d 7020 6973 2065 706f 6368 2069 6e0a  amp is epoch in.
-000296c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000296d0: 6d69 6c6c 6973 6563 6f6e 6473 2e20 4465  milliseconds. De
-000296e0: 6661 756c 7420 6973 2063 7572 7265 6e74  fault is current
-000296f0: 2074 696d 6573 7461 6d70 0a20 2020 2020   timestamp.     
-00029700: 2020 2020 2020 2073 7761 726d 5f69 6420         swarm_id 
-00029710: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
-00029720: 2046 696c 7465 7220 6279 2053 7761 726d   Filter by Swarm
-00029730: 2049 440a 2020 2020 2020 2020 2020 2020   ID.            
-00029740: 6672 6f6d 5f74 696d 6573 7461 6d70 2028  from_timestamp (
-00029750: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
-00029760: 5468 6973 2070 6172 616d 6574 6572 2073  This parameter s
-00029770: 7570 6572 6365 6465 7320 7374 6172 7420  upercedes start 
-00029780: 7061 7261 6d65 7465 722e 204e 6565 640a  parameter. Need.
-00029790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000297a0: 696e 666f 726d 6174 696f 6e20 6672 6f6d  information from
-000297b0: 2074 6869 7320 7469 6d65 7374 616d 702e   this timestamp.
-000297c0: 2054 696d 6573 7461 6d70 2069 7320 6570   Timestamp is ep
-000297d0: 6f63 6820 696e 2073 6563 6f6e 6473 2e20  och in seconds. 
-000297e0: 4465 6661 756c 7420 6973 2063 7572 7265  Default is curre
-000297f0: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
-00029800: 2020 2055 5443 2074 696d 6573 7461 6d70     UTC timestamp
-00029810: 206d 696e 7573 2033 2068 6f75 7273 0a20   minus 3 hours. 
-00029820: 2020 2020 2020 2020 2020 2074 6f5f 7469             to_ti
-00029830: 6d65 7374 616d 7020 2869 6e74 2c20 6f70  mestamp (int, op
-00029840: 7469 6f6e 616c 293a 2054 6869 7320 7061  tional): This pa
-00029850: 7261 6d65 7465 7220 7375 7065 7263 6564  rameter superced
-00029860: 6573 2065 6e64 2070 6172 616d 6574 6572  es end parameter
-00029870: 2e20 4e65 6564 2069 6e66 6f72 6d61 7469  . Need informati
-00029880: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
-00029890: 2020 2074 6f20 7468 6973 2074 696d 6573     to this times
-000298a0: 7461 6d70 2e20 5469 6d65 7374 616d 7020  tamp. Timestamp 
-000298b0: 6973 2065 706f 6368 2069 6e20 7365 636f  is epoch in seco
-000298c0: 6e64 732e 2044 6566 6175 6c74 2069 7320  nds. Default is 
-000298d0: 6375 7272 656e 7420 5554 4320 7469 6d65  current UTC time
-000298e0: 7374 616d 700a 2020 2020 2020 2020 2020  stamp.          
-000298f0: 2020 6f66 6673 6574 2028 696e 742c 206f    offset (int, o
-00029900: 7074 696f 6e61 6c29 3a20 5061 6769 6e61  ptional): Pagina
-00029910: 7469 6f6e 206f 6666 7365 7420 2864 6566  tion offset (def
-00029920: 6175 6c74 203d 2030 2920 4465 6661 756c  ault = 0) Defaul
-00029930: 7473 2074 6f20 302e 0a20 2020 2020 2020  ts to 0..       
-00029940: 2020 2020 206c 696d 6974 2028 696e 742c       limit (int,
-00029950: 206f 7074 696f 6e61 6c29 3a20 7061 6769   optional): pagi
-00029960: 6e61 7469 6f6e 2073 697a 6520 2864 6566  nation size (def
-00029970: 6175 6c74 203d 2031 3030 2920 4465 6661  ault = 100) Defa
-00029980: 756c 7473 2074 6f20 3130 302e 0a0a 2020  ults to 100...  
-00029990: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-000299a0: 2020 2020 2020 2020 2020 2052 6573 706f             Respo
-000299b0: 6e73 653a 2043 656e 7472 616c 4150 4920  nse: CentralAPI 
-000299c0: 5265 7370 6f6e 7365 206f 626a 6563 740a  Response object.
-000299d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000299e0: 2020 2020 7572 6c20 3d20 222f 7261 7069      url = "/rapi
-000299f0: 6473 2f76 312f 696e 7465 7266 6572 696e  ds/v1/interferin
-00029a00: 675f 6170 7322 0a0a 2020 2020 2020 2020  g_aps"..        
-00029a10: 7061 7261 6d73 203d 207b 0a20 2020 2020  params = {.     
-00029a20: 2020 2020 2020 2027 6772 6f75 7027 3a20         'group': 
-00029a30: 6772 6f75 702c 0a20 2020 2020 2020 2020  group,.         
-00029a40: 2020 2027 6c61 6265 6c27 3a20 6c61 6265     'label': labe
-00029a50: 6c2c 0a20 2020 2020 2020 2020 2020 2027  l,.            '
-00029a60: 7369 7465 273a 2073 6974 652c 0a20 2020  site': site,.   
-00029a70: 2020 2020 2020 2020 2027 7374 6172 7427           'start'
-00029a80: 3a20 7374 6172 742c 0a20 2020 2020 2020  : start,.       
-00029a90: 2020 2020 2027 656e 6427 3a20 656e 642c       'end': end,
-00029aa0: 0a20 2020 2020 2020 2020 2020 2027 7377  .            'sw
-00029ab0: 6172 6d5f 6964 273a 2073 7761 726d 5f69  arm_id': swarm_i
-00029ac0: 642c 0a20 2020 2020 2020 2020 2020 2027  d,.            '
-00029ad0: 6672 6f6d 5f74 696d 6573 7461 6d70 273a  from_timestamp':
-00029ae0: 2066 726f 6d5f 7469 6d65 7374 616d 702c   from_timestamp,
-00029af0: 0a20 2020 2020 2020 2020 2020 2027 746f  .            'to
-00029b00: 5f74 696d 6573 7461 6d70 273a 2074 6f5f  _timestamp': to_
-00029b10: 7469 6d65 7374 616d 702c 0a20 2020 2020  timestamp,.     
-00029b20: 2020 2020 2020 2027 6f66 6673 6574 273a         'offset':
-00029b30: 206f 6666 7365 742c 0a20 2020 2020 2020   offset,.       
-00029b40: 2020 2020 2027 6c69 6d69 7427 3a20 6c69       'limit': li
-00029b50: 6d69 740a 2020 2020 2020 2020 7d0a 0a20  mit.        }.. 
-00029b60: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
-00029b70: 6169 7420 7365 6c66 2e67 6574 2875 726c  ait self.get(url
-00029b80: 2c20 7061 7261 6d73 3d70 6172 616d 7329  , params=params)
-00029b90: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-00029ba0: 7769 6473 5f67 6574 5f73 7573 7065 6374  wids_get_suspect
-00029bb0: 5f61 7073 280a 2020 2020 2020 2020 7365  _aps(.        se
-00029bc0: 6c66 2c0a 2020 2020 2020 2020 6772 6f75  lf,.        grou
-00029bd0: 703a 204c 6973 745b 7374 725d 203d 204e  p: List[str] = N
-00029be0: 6f6e 652c 0a20 2020 2020 2020 206c 6162  one,.        lab
-00029bf0: 656c 3a20 4c69 7374 5b73 7472 5d20 3d20  el: List[str] = 
-00029c00: 4e6f 6e65 2c0a 2020 2020 2020 2020 7369  None,.        si
-00029c10: 7465 3a20 4c69 7374 5b73 7472 5d20 3d20  te: List[str] = 
-00029c20: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-00029c30: 6172 743a 2069 6e74 203d 204e 6f6e 652c  art: int = None,
-00029c40: 0a20 2020 2020 2020 2065 6e64 3a20 696e  .        end: in
-00029c50: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-00029c60: 2020 7377 6172 6d5f 6964 3a20 7374 7220    swarm_id: str 
-00029c70: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00029c80: 6672 6f6d 5f74 696d 6573 7461 6d70 3a20  from_timestamp: 
-00029c90: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-00029ca0: 2020 2020 746f 5f74 696d 6573 7461 6d70      to_timestamp
-00029cb0: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-00029cc0: 2020 2020 2020 6f66 6673 6574 3a20 696e        offset: in
-00029cd0: 7420 3d20 302c 0a20 2020 2020 2020 206c  t = 0,.        l
-00029ce0: 696d 6974 3a20 696e 7420 3d20 3130 300a  imit: int = 100.
-00029cf0: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
-00029d00: 653a 0a20 2020 2020 2020 2022 2222 4c69  e:.        """Li
-00029d10: 7374 2073 7573 7065 6374 2041 5073 2e0a  st suspect APs..
-00029d20: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00029d30: 2020 2020 2020 2020 2020 2067 726f 7570             group
-00029d40: 2028 4c69 7374 5b73 7472 5d2c 206f 7074   (List[str], opt
-00029d50: 696f 6e61 6c29 3a20 4c69 7374 206f 6620  ional): List of 
-00029d60: 6772 6f75 7020 6e61 6d65 730a 2020 2020  group names.    
-00029d70: 2020 2020 2020 2020 6c61 6265 6c20 284c          label (L
-00029d80: 6973 745b 7374 725d 2c20 6f70 7469 6f6e  ist[str], option
-00029d90: 616c 293a 204c 6973 7420 6f66 206c 6162  al): List of lab
-00029da0: 656c 206e 616d 6573 0a20 2020 2020 2020  el names.       
-00029db0: 2020 2020 2073 6974 6520 284c 6973 745b       site (List[
-00029dc0: 7374 725d 2c20 6f70 7469 6f6e 616c 293a  str], optional):
-00029dd0: 204c 6973 7420 6f66 2073 6974 6520 6e61   List of site na
-00029de0: 6d65 730a 2020 2020 2020 2020 2020 2020  mes.            
-00029df0: 7374 6172 7420 2869 6e74 2c20 6f70 7469  start (int, opti
-00029e00: 6f6e 616c 293a 204e 6565 6420 696e 666f  onal): Need info
-00029e10: 726d 6174 696f 6e20 6672 6f6d 2074 6869  rmation from thi
-00029e20: 7320 7469 6d65 7374 616d 702e 2054 696d  s timestamp. Tim
-00029e30: 6573 7461 6d70 2069 7320 6570 6f63 6820  estamp is epoch 
-00029e40: 696e 0a20 2020 2020 2020 2020 2020 2020  in.             
-00029e50: 2020 206d 696c 6c69 7365 636f 6e64 732e     milliseconds.
-00029e60: 2044 6566 6175 6c74 2069 7320 6375 7272   Default is curr
-00029e70: 656e 7420 7469 6d65 7374 616d 7020 6d69  ent timestamp mi
-00029e80: 6e75 7320 3320 686f 7572 730a 2020 2020  nus 3 hours.    
-00029e90: 2020 2020 2020 2020 656e 6420 2869 6e74          end (int
-00029ea0: 2c20 6f70 7469 6f6e 616c 293a 204e 6565  , optional): Nee
-00029eb0: 6420 696e 666f 726d 6174 696f 6e20 746f  d information to
-00029ec0: 2074 6869 7320 7469 6d65 7374 616d 702e   this timestamp.
-00029ed0: 2054 696d 6573 7461 6d70 2069 7320 6570   Timestamp is ep
-00029ee0: 6f63 6820 696e 0a20 2020 2020 2020 2020  och in.         
-00029ef0: 2020 2020 2020 206d 696c 6c69 7365 636f         milliseco
-00029f00: 6e64 732e 2044 6566 6175 6c74 2069 7320  nds. Default is 
-00029f10: 6375 7272 656e 7420 7469 6d65 7374 616d  current timestam
-00029f20: 700a 2020 2020 2020 2020 2020 2020 7377  p.            sw
-00029f30: 6172 6d5f 6964 2028 7374 722c 206f 7074  arm_id (str, opt
-00029f40: 696f 6e61 6c29 3a20 4669 6c74 6572 2062  ional): Filter b
-00029f50: 7920 5377 6172 6d20 4944 0a20 2020 2020  y Swarm ID.     
-00029f60: 2020 2020 2020 2066 726f 6d5f 7469 6d65         from_time
-00029f70: 7374 616d 7020 2869 6e74 2c20 6f70 7469  stamp (int, opti
-00029f80: 6f6e 616c 293a 2054 6869 7320 7061 7261  onal): This para
-00029f90: 6d65 7465 7220 7375 7065 7263 6564 6573  meter supercedes
-00029fa0: 2073 7461 7274 2070 6172 616d 6574 6572   start parameter
-00029fb0: 2e20 4e65 6564 0a20 2020 2020 2020 2020  . Need.         
-00029fc0: 2020 2020 2020 2069 6e66 6f72 6d61 7469         informati
-00029fd0: 6f6e 2066 726f 6d20 7468 6973 2074 696d  on from this tim
-00029fe0: 6573 7461 6d70 2e20 5469 6d65 7374 616d  estamp. Timestam
-00029ff0: 7020 6973 2065 706f 6368 2069 6e20 7365  p is epoch in se
-0002a000: 636f 6e64 732e 2044 6566 6175 6c74 2069  conds. Default i
-0002a010: 7320 6375 7272 656e 740a 2020 2020 2020  s current.      
-0002a020: 2020 2020 2020 2020 2020 5554 4320 7469            UTC ti
-0002a030: 6d65 7374 616d 7020 6d69 6e75 7320 3320  mestamp minus 3 
-0002a040: 686f 7572 730a 2020 2020 2020 2020 2020  hours.          
-0002a050: 2020 746f 5f74 696d 6573 7461 6d70 2028    to_timestamp (
-0002a060: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
-0002a070: 5468 6973 2070 6172 616d 6574 6572 2073  This parameter s
-0002a080: 7570 6572 6365 6465 7320 656e 6420 7061  upercedes end pa
-0002a090: 7261 6d65 7465 722e 204e 6565 6420 696e  rameter. Need in
-0002a0a0: 666f 726d 6174 696f 6e0a 2020 2020 2020  formation.      
-0002a0b0: 2020 2020 2020 2020 2020 746f 2074 6869            to thi
-0002a0c0: 7320 7469 6d65 7374 616d 702e 2054 696d  s timestamp. Tim
-0002a0d0: 6573 7461 6d70 2069 7320 6570 6f63 6820  estamp is epoch 
-0002a0e0: 696e 2073 6563 6f6e 6473 2e20 4465 6661  in seconds. Defa
-0002a0f0: 756c 7420 6973 2063 7572 7265 6e74 2055  ult is current U
-0002a100: 5443 2074 696d 6573 7461 6d70 0a20 2020  TC timestamp.   
-0002a110: 2020 2020 2020 2020 206f 6666 7365 7420           offset 
-0002a120: 2869 6e74 2c20 6f70 7469 6f6e 616c 293a  (int, optional):
-0002a130: 2050 6167 696e 6174 696f 6e20 6f66 6673   Pagination offs
-0002a140: 6574 2028 6465 6661 756c 7420 3d20 3029  et (default = 0)
-0002a150: 2044 6566 6175 6c74 7320 746f 2030 2e0a   Defaults to 0..
-0002a160: 2020 2020 2020 2020 2020 2020 6c69 6d69              limi
-0002a170: 7420 2869 6e74 2c20 6f70 7469 6f6e 616c  t (int, optional
-0002a180: 293a 2070 6167 696e 6174 696f 6e20 7369  ): pagination si
-0002a190: 7a65 2028 6465 6661 756c 7420 3d20 3130  ze (default = 10
-0002a1a0: 3029 2044 6566 6175 6c74 7320 746f 2031  0) Defaults to 1
-0002a1b0: 3030 2e0a 0a20 2020 2020 2020 2052 6574  00...        Ret
-0002a1c0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-0002a1d0: 2020 5265 7370 6f6e 7365 3a20 4365 6e74    Response: Cent
-0002a1e0: 7261 6c41 5049 2052 6573 706f 6e73 6520  ralAPI Response 
-0002a1f0: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
-0002a200: 2222 0a20 2020 2020 2020 2075 726c 203d  "".        url =
-0002a210: 2022 2f72 6170 6964 732f 7631 2f73 7573   "/rapids/v1/sus
-0002a220: 7065 6374 5f61 7073 220a 0a20 2020 2020  pect_aps"..     
-0002a230: 2020 2070 6172 616d 7320 3d20 7b0a 2020     params = {.  
-0002a240: 2020 2020 2020 2020 2020 2767 726f 7570            'group
-0002a250: 273a 2067 726f 7570 2c0a 2020 2020 2020  ': group,.      
-0002a260: 2020 2020 2020 276c 6162 656c 273a 206c        'label': l
-0002a270: 6162 656c 2c0a 2020 2020 2020 2020 2020  abel,.          
-0002a280: 2020 2773 6974 6527 3a20 7369 7465 2c0a    'site': site,.
-0002a290: 2020 2020 2020 2020 2020 2020 2773 7461              'sta
-0002a2a0: 7274 273a 2073 7461 7274 2c0a 2020 2020  rt': start,.    
-0002a2b0: 2020 2020 2020 2020 2765 6e64 273a 2065          'end': e
-0002a2c0: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
-0002a2d0: 2773 7761 726d 5f69 6427 3a20 7377 6172  'swarm_id': swar
-0002a2e0: 6d5f 6964 2c0a 2020 2020 2020 2020 2020  m_id,.          
-0002a2f0: 2020 2766 726f 6d5f 7469 6d65 7374 616d    'from_timestam
-0002a300: 7027 3a20 6672 6f6d 5f74 696d 6573 7461  p': from_timesta
-0002a310: 6d70 2c0a 2020 2020 2020 2020 2020 2020  mp,.            
-0002a320: 2774 6f5f 7469 6d65 7374 616d 7027 3a20  'to_timestamp': 
-0002a330: 746f 5f74 696d 6573 7461 6d70 2c0a 2020  to_timestamp,.  
-0002a340: 2020 2020 2020 2020 2020 276f 6666 7365            'offse
-0002a350: 7427 3a20 6f66 6673 6574 2c0a 2020 2020  t': offset,.    
-0002a360: 2020 2020 2020 2020 276c 696d 6974 273a          'limit':
-0002a370: 206c 696d 6974 0a20 2020 2020 2020 207d   limit.        }
-0002a380: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0002a390: 2061 7761 6974 2073 656c 662e 6765 7428   await self.get(
-0002a3a0: 7572 6c2c 2070 6172 616d 733d 7061 7261  url, params=para
-0002a3b0: 6d73 290a 0a20 2020 2061 7379 6e63 2064  ms)..    async d
-0002a3c0: 6566 2077 6964 735f 6765 745f 6e65 6967  ef wids_get_neig
-0002a3d0: 6862 6f72 5f61 7073 280a 2020 2020 2020  hbor_aps(.      
-0002a3e0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0002a3f0: 6772 6f75 703a 204c 6973 745b 7374 725d  group: List[str]
+00020e40: 653a 2063 6f6e 7374 616e 7473 2e44 6576  e: constants.Dev
+00020e50: 5479 7065 732c 2067 726f 7570 3a20 7374  Types, group: st
+00020e60: 7220 3d20 4e6f 6e65 2920 2d3e 2052 6573  r = None) -> Res
+00020e70: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
+00020e80: 2222 4765 7420 4669 726d 7761 7265 2043  ""Get Firmware C
+00020e90: 6f6d 706c 6961 6e63 6520 5665 7273 696f  ompliance Versio
+00020ea0: 6e2e 0a0a 2020 2020 2020 2020 2f2f 2055  n...        // U
+00020eb0: 7365 6420 6279 2073 686f 7720 6669 726d  sed by show firm
+00020ec0: 7761 7265 2063 6f6d 706c 6961 6e63 6520  ware compliance 
+00020ed0: 5b61 707c 6777 7c73 777c 6378 5d20 5b67  [ap|gw|sw|cx] [g
+00020ee0: 726f 7570 2d6e 616d 655d 202f 2f0a 0a20  roup-name] //.. 
+00020ef0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00020f00: 2020 2020 2020 2020 2064 6576 6963 655f           device_
+00020f10: 7479 7065 2028 7374 7229 3a20 5370 6563  type (str): Spec
+00020f20: 6966 7920 6f6e 6520 6f66 2022 6170 7c67  ify one of "ap|g
+00020f30: 777c 7377 7c73 7822 0a20 2020 2020 2020  w|sw|sx".       
+00020f40: 2020 2020 2067 726f 7570 2028 7374 722c       group (str,
+00020f50: 206f 7074 696f 6e61 6c29 3a20 4772 6f75   optional): Grou
+00020f60: 7020 6e61 6d65 0a0a 2020 2020 2020 2020  p name..        
+00020f70: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00020f80: 2020 2020 2052 6573 706f 6e73 653a 2043       Response: C
+00020f90: 656e 7472 616c 4150 4920 5265 7370 6f6e  entralAPI Respon
+00020fa0: 7365 206f 626a 6563 740a 2020 2020 2020  se object.      
+00020fb0: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
+00020fc0: 4150 4920 6d65 7468 6f64 2072 6574 7572  API method retur
+00020fd0: 6e73 2034 3034 2069 6620 636f 6d70 6c69  ns 404 if compli
+00020fe0: 616e 6365 2069 7320 6e6f 7420 7365 7421  ance is not set!
+00020ff0: 0a20 2020 2020 2020 2075 726c 203d 2022  .        url = "
+00021000: 2f66 6972 6d77 6172 652f 7631 2f75 7067  /firmware/v1/upg
+00021010: 7261 6465 2f63 6f6d 706c 6961 6e63 655f  rade/compliance_
+00021020: 7665 7273 696f 6e22 0a20 2020 2020 2020  version".       
+00021030: 2064 6576 6963 655f 7479 7065 203d 2063   device_type = c
+00021040: 6f6e 7374 616e 7473 2e6c 6962 5f74 6f5f  onstants.lib_to_
+00021050: 6170 6928 2766 6972 6d77 6172 6527 2c20  api('firmware', 
+00021060: 6465 7669 6365 5f74 7970 6529 0a0a 2020  device_type)..  
+00021070: 2020 2020 2020 7061 7261 6d73 203d 207b        params = {
+00021080: 0a20 2020 2020 2020 2020 2020 2027 6465  .            'de
+00021090: 7669 6365 5f74 7970 6527 3a20 6465 7669  vice_type': devi
+000210a0: 6365 5f74 7970 652c 0a20 2020 2020 2020  ce_type,.       
+000210b0: 2020 2020 2027 6772 6f75 7027 3a20 6772       'group': gr
+000210c0: 6f75 700a 2020 2020 2020 2020 7d0a 0a20  oup.        }.. 
+000210d0: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
+000210e0: 6169 7420 7365 6c66 2e67 6574 2875 726c  ait self.get(url
+000210f0: 2c20 7061 7261 6d73 3d70 6172 616d 7329  , params=params)
+00021100: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00021110: 6465 6c65 7465 5f66 6972 6d77 6172 655f  delete_firmware_
+00021120: 636f 6d70 6c69 616e 6365 2873 656c 662c  compliance(self,
+00021130: 2064 6576 6963 655f 7479 7065 3a20 636f   device_type: co
+00021140: 6e73 7461 6e74 732e 4465 7654 7970 6573  nstants.DevTypes
+00021150: 2c20 6772 6f75 703a 2073 7472 203d 204e  , group: str = N
+00021160: 6f6e 6529 202d 3e20 5265 7370 6f6e 7365  one) -> Response
+00021170: 3a0a 2020 2020 2020 2020 2222 2243 6c65  :.        """Cle
+00021180: 6172 2046 6972 6d77 6172 6520 436f 6d70  ar Firmware Comp
+00021190: 6c69 616e 6365 2056 6572 7369 6f6e 2e0a  liance Version..
+000211a0: 0a20 2020 2020 2020 202f 2f20 5573 6564  .        // Used
+000211b0: 2062 7920 6465 6c65 7465 2066 6972 6d77   by delete firmw
+000211c0: 6172 6520 636f 6d70 6c69 616e 6365 205b  are compliance [
+000211d0: 6170 7c67 777c 7377 7c63 785d 205b 6772  ap|gw|sw|cx] [gr
+000211e0: 6f75 705d 202f 2f0a 0a20 2020 2020 2020  oup] //..       
+000211f0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00021200: 2020 2064 6576 6963 655f 7479 7065 2028     device_type (
+00021210: 7374 7229 3a20 5370 6563 6966 7920 6f6e  str): Specify on
+00021220: 6520 6f66 2022 6170 7c67 777c 7377 7c63  e of "ap|gw|sw|c
+00021230: 7822 0a20 2020 2020 2020 2020 2020 2067  x".            g
+00021240: 726f 7570 2028 7374 722c 206f 7074 696f  roup (str, optio
+00021250: 6e61 6c29 3a20 4772 6f75 7020 6e61 6d65  nal): Group name
+00021260: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
+00021270: 6e65 2028 476c 6f62 616c 2043 6f6d 706c  ne (Global Compl
+00021280: 6961 6e63 6529 0a0a 2020 2020 2020 2020  iance)..        
+00021290: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+000212a0: 2020 2020 2052 6573 706f 6e73 653a 2043       Response: C
+000212b0: 656e 7472 616c 4150 4920 5265 7370 6f6e  entralAPI Respon
+000212c0: 7365 206f 626a 6563 740a 2020 2020 2020  se object.      
+000212d0: 2020 2222 220a 2020 2020 2020 2020 7572    """.        ur
+000212e0: 6c20 3d20 222f 6669 726d 7761 7265 2f76  l = "/firmware/v
+000212f0: 312f 7570 6772 6164 652f 636f 6d70 6c69  1/upgrade/compli
+00021300: 616e 6365 5f76 6572 7369 6f6e 220a 2020  ance_version".  
+00021310: 2020 2020 2020 6465 7669 6365 5f74 7970        device_typ
+00021320: 6520 3d20 636f 6e73 7461 6e74 732e 6c69  e = constants.li
+00021330: 625f 746f 5f61 7069 2827 6669 726d 7761  b_to_api('firmwa
+00021340: 7265 272c 2064 6576 6963 655f 7479 7065  re', device_type
+00021350: 290a 0a20 2020 2020 2020 2070 6172 616d  )..        param
+00021360: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
+00021370: 2020 2764 6576 6963 655f 7479 7065 273a    'device_type':
+00021380: 2064 6576 6963 655f 7479 7065 2c0a 2020   device_type,.  
+00021390: 2020 2020 2020 2020 2020 2767 726f 7570            'group
+000213a0: 273a 2067 726f 7570 0a20 2020 2020 2020  ': group.       
+000213b0: 207d 0a0a 2020 2020 2020 2020 7265 7475   }..        retu
+000213c0: 726e 2061 7761 6974 2073 656c 662e 6465  rn await self.de
+000213d0: 6c65 7465 2875 726c 2c20 7061 7261 6d73  lete(url, params
+000213e0: 3d70 6172 616d 7329 0a0a 2020 2020 6173  =params)..    as
+000213f0: 796e 6320 6465 6620 7365 745f 6669 726d  ync def set_firm
+00021400: 7761 7265 5f63 6f6d 706c 6961 6e63 6528  ware_compliance(
+00021410: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00021420: 2020 2020 2020 2064 6576 6963 655f 7479         device_ty
+00021430: 7065 3a20 636f 6e73 7461 6e74 732e 4465  pe: constants.De
+00021440: 7654 7970 6573 2c0a 2020 2020 2020 2020  vTypes,.        
+00021450: 6772 6f75 703a 2073 7472 2c0a 2020 2020  group: str,.    
+00021460: 2020 2020 7665 7273 696f 6e3a 2073 7472      version: str
+00021470: 2c0a 2020 2020 2020 2020 636f 6d70 6c69  ,.        compli
+00021480: 616e 6365 5f73 6368 6564 756c 6564 5f61  ance_scheduled_a
+00021490: 743a 2069 6e74 2c0a 2020 2020 2020 2020  t: int,.        
+000214a0: 7265 626f 6f74 3a20 626f 6f6c 203d 2054  reboot: bool = T
+000214b0: 7275 652c 2020 2320 4f6e 6c79 2061 7070  rue,  # Only app
+000214c0: 6c69 6573 2074 6f20 4d41 5320 616c 6c20  lies to MAS all 
+000214d0: 6f74 6865 7273 2072 6562 6f6f 7420 7265  others reboot re
+000214e0: 6761 7264 6c65 7373 2e20 2063 656e 636c  gardless.  cencl
+000214f0: 6920 646f 6573 6e27 7420 7375 7070 6f72  i doesn't suppor
+00021500: 7420 4d41 530a 2020 2020 2020 2020 616c  t MAS.        al
+00021510: 6c6f 775f 756e 7375 7070 6f72 7465 645f  low_unsupported_
+00021520: 7665 7273 696f 6e3a 2062 6f6f 6c20 3d20  version: bool = 
+00021530: 4661 6c73 652c 0a20 2020 2029 202d 3e20  False,.    ) -> 
+00021540: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
+00021550: 2020 2222 2253 6574 2046 6972 6d77 6172    """Set Firmwar
+00021560: 6520 436f 6d70 6c69 616e 6365 2076 6572  e Compliance ver
+00021570: 7369 6f6e 2028 666f 7220 6772 6f75 702f  sion (for group/
+00021580: 6465 7669 6365 2d74 7970 6529 2e0a 0a20  device-type)... 
+00021590: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+000215a0: 2020 2020 2020 2020 2064 6576 6963 655f           device_
+000215b0: 7479 7065 2028 7374 7229 3a20 5370 6563  type (str): Spec
+000215c0: 6966 7920 6f6e 6520 6f66 2022 6170 7c73  ify one of "ap|s
+000215d0: 777c 6378 7c67 7722 0a20 2020 2020 2020  w|cx|gw".       
+000215e0: 2020 2020 2067 726f 7570 2028 7374 7229       group (str)
+000215f0: 3a20 4772 6f75 7020 6e61 6d65 0a20 2020  : Group name.   
+00021600: 2020 2020 2020 2020 2066 6972 6d77 6172           firmwar
+00021610: 655f 636f 6d70 6c69 616e 6365 5f76 6572  e_compliance_ver
+00021620: 7369 6f6e 2028 7374 7229 3a20 4669 726d  sion (str): Firm
+00021630: 7761 7265 2063 6f6d 706c 6961 6e63 6520  ware compliance 
+00021640: 7665 7273 696f 6e20 666f 7220 7370 6563  version for spec
+00021650: 6966 6963 2064 6576 6963 655f 7479 7065  ific device_type
+00021660: 2e0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+00021670: 6d70 6c69 616e 6365 5f73 6368 6564 756c  mpliance_schedul
+00021680: 6564 5f61 7420 2869 6e74 293a 2046 6972  ed_at (int): Fir
+00021690: 6d77 6172 6520 636f 6d70 6c69 616e 6365  mware compliance
+000216a0: 2077 696c 6c20 6265 2073 6368 6564 756c   will be schedul
+000216b0: 6520 6174 2c0a 2020 2020 2020 2020 2020  e at,.          
+000216c0: 2020 2020 2020 636f 6d70 6c69 616e 6365        compliance
+000216d0: 5f73 6368 6564 756c 6564 5f61 7420 2d20  _scheduled_at - 
+000216e0: 6375 7272 656e 7420 7469 6d65 2e20 636f  current time. co
+000216f0: 6d70 6c69 616e 6365 5f73 6368 6564 756c  mpliance_schedul
+00021700: 6564 5f61 7420 6973 2065 706f 6368 2069  ed_at is epoch i
+00021710: 6e20 7365 636f 6e64 730a 2020 2020 2020  n seconds.      
+00021720: 2020 2020 2020 2020 2020 616e 6420 6465            and de
+00021730: 6661 756c 7420 7661 6c75 6520 6973 2063  fault value is c
+00021740: 7572 7265 6e74 2074 696d 652e 0a20 2020  urrent time..   
+00021750: 2020 2020 2020 2020 2072 6562 6f6f 7420           reboot 
+00021760: 2862 6f6f 6c29 3a20 5573 6520 5472 7565  (bool): Use True
+00021770: 2066 6f72 2061 7574 6f20 7265 626f 6f74   for auto reboot
+00021780: 2061 6674 6572 2073 7563 6365 7373 6675   after successfu
+00021790: 6c20 6669 726d 7761 7265 2064 6f77 6e6c  l firmware downl
+000217a0: 6f61 642e 2044 6566 6175 6c74 0a20 2020  oad. Default.   
+000217b0: 2020 2020 2020 2020 2020 2020 2076 616c               val
+000217c0: 7565 2069 7320 4661 6c73 652e 2041 7070  ue is False. App
+000217d0: 6c69 6361 626c 6520 6f6e 6c79 206f 6e20  licable only on 
+000217e0: 4d41 532c 2061 7275 6261 2073 7769 7463  MAS, aruba switc
+000217f0: 6865 732c 2043 5820 7377 6974 6368 6573  hes, CX switches
+00021800: 2c20 616e 6420 636f 6e74 726f 6c6c 6572  , and controller
+00021810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021820: 2073 696e 6365 2049 4150 2072 6562 6f6f   since IAP reboo
+00021830: 7473 2061 7574 6f6d 6174 6963 616c 6c79  ts automatically
+00021840: 2061 6674 6572 2066 6972 6d77 6172 6520   after firmware 
+00021850: 646f 776e 6c6f 6164 2e0a 2020 2020 2020  download..      
+00021860: 2020 2020 2020 616c 6c6f 775f 756e 7375        allow_unsu
+00021870: 7070 6f72 7465 645f 7665 7273 696f 6e20  pported_version 
+00021880: 2862 6f6f 6c29 3a20 5573 6520 5472 7565  (bool): Use True
+00021890: 2074 6f20 7365 7420 756e 7375 7070 6f72   to set unsuppor
+000218a0: 7465 6420 7665 7273 696f 6e20 6173 2066  ted version as f
+000218b0: 6972 6d77 6172 650a 2020 2020 2020 2020  irmware.        
+000218c0: 2020 2020 2020 2020 636f 6d70 6c69 616e          complian
+000218d0: 6365 2076 6572 7369 6f6e 2066 6f72 2073  ce version for s
+000218e0: 7065 6369 6669 6320 6465 7669 6365 5f74  pecific device_t
+000218f0: 7970 652e 2044 6566 6175 6c74 2069 7320  ype. Default is 
+00021900: 4661 6c73 652e 0a0a 2020 2020 2020 2020  False...        
+00021910: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00021920: 2020 2020 2052 6573 706f 6e73 653a 2043       Response: C
+00021930: 656e 7472 616c 4150 4920 5265 7370 6f6e  entralAPI Respon
+00021940: 7365 206f 626a 6563 740a 2020 2020 2020  se object.      
+00021950: 2020 2222 220a 2020 2020 2020 2020 7572    """.        ur
+00021960: 6c20 3d20 222f 6669 726d 7761 7265 2f76  l = "/firmware/v
+00021970: 322f 7570 6772 6164 652f 636f 6d70 6c69  2/upgrade/compli
+00021980: 616e 6365 5f76 6572 7369 6f6e 220a 2020  ance_version".  
+00021990: 2020 2020 2020 6465 7669 6365 5f74 7970        device_typ
+000219a0: 6520 3d20 636f 6e73 7461 6e74 732e 6c69  e = constants.li
+000219b0: 625f 746f 5f61 7069 2827 6669 726d 7761  b_to_api('firmwa
+000219c0: 7265 272c 2064 6576 6963 655f 7479 7065  re', device_type
+000219d0: 290a 0a0a 2020 2020 2020 2020 6a73 6f6e  )...        json
+000219e0: 5f64 6174 6120 3d20 7b0a 2020 2020 2020  _data = {.      
+000219f0: 2020 2020 2020 2764 6576 6963 655f 7479        'device_ty
+00021a00: 7065 273a 2064 6576 6963 655f 7479 7065  pe': device_type
+00021a10: 2c0a 2020 2020 2020 2020 2020 2020 2767  ,.            'g
+00021a20: 726f 7570 273a 2067 726f 7570 2c0a 2020  roup': group,.  
+00021a30: 2020 2020 2020 2020 2020 2766 6972 6d77            'firmw
+00021a40: 6172 655f 636f 6d70 6c69 616e 6365 5f76  are_compliance_v
+00021a50: 6572 7369 6f6e 273a 2076 6572 7369 6f6e  ersion': version
+00021a60: 2c0a 2020 2020 2020 2020 2020 2020 2772  ,.            'r
+00021a70: 6562 6f6f 7427 3a20 7265 626f 6f74 2c0a  eboot': reboot,.
+00021a80: 2020 2020 2020 2020 2020 2020 2761 6c6c              'all
+00021a90: 6f77 5f75 6e73 7570 706f 7274 6564 5f76  ow_unsupported_v
+00021aa0: 6572 7369 6f6e 273a 2061 6c6c 6f77 5f75  ersion': allow_u
+00021ab0: 6e73 7570 706f 7274 6564 5f76 6572 7369  nsupported_versi
+00021ac0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+00021ad0: 2763 6f6d 706c 6961 6e63 655f 7363 6865  'compliance_sche
+00021ae0: 6475 6c65 645f 6174 273a 2063 6f6d 706c  duled_at': compl
+00021af0: 6961 6e63 655f 7363 6865 6475 6c65 645f  iance_scheduled_
+00021b00: 6174 0a20 2020 2020 2020 207d 0a0a 2020  at.        }..  
+00021b10: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+00021b20: 6974 2073 656c 662e 706f 7374 2875 726c  it self.post(url
+00021b30: 2c20 6a73 6f6e 5f64 6174 613d 6a73 6f6e  , json_data=json
+00021b40: 5f64 6174 6129 0a0a 2020 2020 6173 796e  _data)..    asyn
+00021b50: 6320 6465 6620 6d6f 7665 5f64 6576 6963  c def move_devic
+00021b60: 6573 5f74 6f5f 6772 6f75 7028 0a20 2020  es_to_group(.   
+00021b70: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00021b80: 2020 2067 726f 7570 3a20 7374 722c 0a20     group: str,. 
+00021b90: 2020 2020 2020 2073 6572 6961 6c5f 6e75         serial_nu
+00021ba0: 6d73 3a20 556e 696f 6e5b 7374 722c 204c  ms: Union[str, L
+00021bb0: 6973 745b 7374 725d 5d2c 0a20 2020 2020  ist[str]],.     
+00021bc0: 2020 202a 2c0a 2020 2020 2020 2020 6378     *,.        cx
+00021bd0: 5f72 6574 6169 6e5f 636f 6e66 6967 3a20  _retain_config: 
+00021be0: 626f 6f6c 203d 2054 7275 652c 2020 2320  bool = True,  # 
+00021bf0: 544f 444f 2063 616e 2077 6520 7365 6e64  TODO can we send
+00021c00: 2074 6869 7320 6174 7472 6962 7574 6520   this attribute 
+00021c10: 6576 656e 2069 6620 6974 2773 206e 6f74  even if it's not
+00021c20: 2043 582c 2077 696c 6c20 6974 2069 676e   CX, will it ign
+00021c30: 6f72 6520 6f72 2065 7272 6f72 0a20 2020  ore or error.   
+00021c40: 2029 202d 3e20 5265 7370 6f6e 7365 3a0a   ) -> Response:.
+00021c50: 2020 2020 2020 2020 2222 224d 6f76 6520          """Move 
+00021c60: 6465 7669 6365 7320 746f 2061 2067 726f  devices to a gro
+00021c70: 7570 2e0a 0a20 2020 2020 2020 2041 7267  up...        Arg
+00021c80: 733a 0a20 2020 2020 2020 2020 2020 2067  s:.            g
+00021c90: 726f 7570 2028 7374 7229 3a20 4772 6f75  roup (str): Grou
+00021ca0: 7020 4e61 6d65 2074 6f20 6d6f 7665 2064  p Name to move d
+00021cb0: 6576 6963 6520 746f 2e0a 2020 2020 2020  evice to..      
+00021cc0: 2020 2020 2020 7365 7269 616c 7320 284c        serials (L
+00021cd0: 6973 745b 7374 725d 293a 2053 6572 6961  ist[str]): Seria
+00021ce0: 6c20 6e75 6d62 6572 7320 6f66 2064 6576  l numbers of dev
+00021cf0: 6963 6573 2074 6f20 6265 2061 6464 6564  ices to be added
+00021d00: 2074 6f20 6772 6f75 702e 0a0a 2020 2020   to group...    
+00021d10: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00021d20: 2020 2020 2020 2020 2052 6573 706f 6e73           Respons
+00021d30: 653a 2043 656e 7472 616c 4150 4920 5265  e: CentralAPI Re
+00021d40: 7370 6f6e 7365 206f 626a 6563 740a 2020  sponse object.  
+00021d50: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00021d60: 2020 2320 4150 492d 464c 4157 2072 6570    # API-FLAW rep
+00021d70: 6f72 7420 666c 6177 6564 2041 5049 206d  ort flawed API m
+00021d80: 6574 686f 640a 2020 2020 2020 2020 2320  ethod.        # 
+00021d90: 5265 7475 726e 7320 3530 3020 7374 6174  Returns 500 stat
+00021da0: 7573 2063 6f64 6520 7768 656e 2072 6573  us code when res
+00021db0: 756c 7420 6973 2065 7373 656e 7469 616c  ult is essential
+00021dc0: 6c79 2073 7563 6365 7373 0a20 2020 2020  ly success.     
+00021dd0: 2020 2023 2050 6c65 6173 6520 436f 6e66     # Please Conf
+00021de0: 6972 6d3a 206d 6f76 6520 4172 7562 6139  irm: move Aruba9
+00021df0: 3030 345f 3831 5f45 385f 4641 2026 2050  004_81_E8_FA & P
+00021e00: 6f6d 6d6f 7265 4757 3120 746f 2067 726f  ommoreGW1 to gro
+00021e10: 7570 2057 4c4e 4554 3f20 5b79 2f4e 5d3a  up WLNET? [y/N]:
+00021e20: 2079 0a20 2020 2020 2020 2023 20e2 9c96   y.        # ...
+00021e30: 2053 656e 6469 6e67 2044 6174 6120 5b63   Sending Data [c
+00021e40: 6f6e 6669 6775 7261 7469 6f6e 2f76 312f  onfiguration/v1/
+00021e50: 6465 7669 6365 732f 6d6f 7665 5d0a 2020  devices/move].  
+00021e60: 2020 2020 2020 2320 7374 6174 7573 2063        # status c
+00021e70: 6f64 653a 2035 3030 203c 2d2d 2035 3030  ode: 500 <-- 500
+00021e80: 206f 6e20 7375 6363 6573 732e 2020 4174   on success.  At
+00021e90: 206c 6561 7374 2066 6f72 2067 7720 776f   least for gw wo
+00021ea0: 756c 6420 6e65 6564 2074 6f20 646f 7562  uld need to doub
+00021eb0: 6c65 2063 6865 636b 206f 7468 6572 732e  le check others.
+00021ec0: 0a20 2020 2020 2020 2023 2064 6573 6372  .        # descr
+00021ed0: 6970 7469 6f6e 3a0a 2020 2020 2020 2020  iption:.        
+00021ee0: 2320 436f 6e74 726f 6c6c 6572 2f47 6174  # Controller/Gat
+00021ef0: 6577 6179 2067 726f 7570 206d 6f76 6520  eway group move 
+00021f00: 6861 7320 6265 656e 2069 6e69 7469 6174  has been initiat
+00021f10: 6564 2c20 706c 6561 7365 2063 6865 636b  ed, please check
+00021f20: 2061 7564 6974 2074 7261 696c 2066 6f72   audit trail for
+00021f30: 2064 6574 6169 6c73 0a20 2020 2020 2020   details.       
+00021f40: 2023 2065 7272 6f72 5f63 6f64 653a 2030   # error_code: 0
+00021f50: 3030 310a 2020 2020 2020 2020 2320 7365  001.        # se
+00021f60: 7276 6963 655f 6e61 6d65 3a20 436f 6e66  rvice_name: Conf
+00021f70: 6967 7572 6174 696f 6e0a 2020 2020 2020  iguration.      
+00021f80: 2020 7572 6c20 3d20 222f 636f 6e66 6967    url = "/config
+00021f90: 7572 6174 696f 6e2f 7631 2f64 6576 6963  uration/v1/devic
+00021fa0: 6573 2f6d 6f76 6522 0a20 2020 2020 2020  es/move".       
+00021fb0: 2073 6572 6961 6c5f 6e75 6d73 203d 2075   serial_nums = u
+00021fc0: 7469 6c73 2e6c 6973 7469 6679 2873 6572  tils.listify(ser
+00021fd0: 6961 6c5f 6e75 6d73 290a 0a20 2020 2020  ial_nums)..     
+00021fe0: 2020 206a 736f 6e5f 6461 7461 203d 207b     json_data = {
+00021ff0: 0a20 2020 2020 2020 2020 2020 2027 6772  .            'gr
+00022000: 6f75 7027 3a20 6772 6f75 702c 0a20 2020  oup': group,.   
+00022010: 2020 2020 2020 2020 2027 7365 7269 616c           'serial
+00022020: 7327 3a20 7365 7269 616c 5f6e 756d 730a  s': serial_nums.
+00022030: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00022040: 2020 2069 6620 6378 5f72 6574 6169 6e5f     if cx_retain_
+00022050: 636f 6e66 6967 3a0a 2020 2020 2020 2020  config:.        
+00022060: 2020 2020 6a73 6f6e 5f64 6174 615b 2270      json_data["p
+00022070: 7265 7365 7276 655f 636f 6e66 6967 5f6f  reserve_config_o
+00022080: 7665 7272 6964 6573 225d 203d 205b 2241  verrides"] = ["A
+00022090: 4f53 5f43 5822 5d0a 0a20 2020 2020 2020  OS_CX"]..       
+000220a0: 2072 6573 7020 3d20 6177 6169 7420 7365   resp = await se
+000220b0: 6c66 2e70 6f73 7428 7572 6c2c 206a 736f  lf.post(url, jso
+000220c0: 6e5f 6461 7461 3d6a 736f 6e5f 6461 7461  n_data=json_data
+000220d0: 290a 0a20 2020 2020 2020 2023 2054 6869  )..        # Thi
+000220e0: 7320 6d65 7468 6f64 2072 6574 7572 6e73  s method returns
+000220f0: 2073 7461 7475 7320 3530 3020 7769 7468   status 500 with
+00022100: 206d 7367 2074 6861 7420 6d6f 7665 2069   msg that move i
+00022110: 7320 696e 6974 6961 7465 6420 6f6e 2073  s initiated on s
+00022120: 7563 6365 7373 2e0a 2020 2020 2020 2020  uccess..        
+00022130: 6966 206e 6f74 2072 6573 7020 616e 6420  if not resp and 
+00022140: 7265 7370 2e73 7461 7475 7320 3d3d 2035  resp.status == 5
+00022150: 3030 3a0a 2020 2020 2020 2020 2020 2020  00:.            
+00022160: 6d61 7463 685f 7374 7220 3d20 2267 726f  match_str = "gro
+00022170: 7570 206d 6f76 6520 6861 7320 6265 656e  up move has been
+00022180: 2069 6e69 7469 6174 6564 2c20 706c 6561   initiated, plea
+00022190: 7365 2063 6865 636b 2061 7564 6974 2074  se check audit t
+000221a0: 7261 696c 2066 6f72 2064 6574 6169 6c73  rail for details
+000221b0: 220a 2020 2020 2020 2020 2020 2020 6966  ".            if
+000221c0: 206d 6174 6368 5f73 7472 2069 6e20 7265   match_str in re
+000221d0: 7370 2e6f 7574 7075 742e 6765 7428 2264  sp.output.get("d
+000221e0: 6573 6372 6970 7469 6f6e 222c 2022 2229  escription", "")
+000221f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00022200: 2020 7265 7370 2e6f 6b20 3d20 5472 7565    resp.ok = True
+00022210: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00022220: 2072 6573 700a 0a20 2020 2061 7379 6e63   resp..    async
+00022230: 2064 6566 2067 6574 5f64 6566 6175 6c74   def get_default
+00022240: 5f67 726f 7570 2873 656c 662c 2920 2d3e  _group(self,) ->
+00022250: 2052 6573 706f 6e73 653a 0a20 2020 2020   Response:.     
+00022260: 2020 2022 2222 4765 7420 6465 6661 756c     """Get defaul
+00022270: 7420 6772 6f75 702e 0a0a 2020 2020 2020  t group...      
+00022280: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00022290: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
+000222a0: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
+000222b0: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
+000222c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000222d0: 7572 6c20 3d20 222f 636f 6e66 6967 7572  url = "/configur
+000222e0: 6174 696f 6e2f 7631 2f67 726f 7570 732f  ation/v1/groups/
+000222f0: 6465 6661 756c 745f 6772 6f75 7022 0a0a  default_group"..
+00022300: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00022310: 7761 6974 2073 656c 662e 6765 7428 7572  wait self.get(ur
+00022320: 6c29 0a0a 2020 2020 6173 796e 6320 6465  l)..    async de
+00022330: 6620 6d6f 7665 5f64 6576 6963 6573 5f74  f move_devices_t
+00022340: 6f5f 7369 7465 280a 2020 2020 2020 2020  o_site(.        
+00022350: 7365 6c66 2c0a 2020 2020 2020 2020 7369  self,.        si
+00022360: 7465 5f69 643a 2069 6e74 2c0a 2020 2020  te_id: int,.    
+00022370: 2020 2020 7365 7269 616c 5f6e 756d 733a      serial_nums:
+00022380: 2055 6e69 6f6e 5b73 7472 2c20 4c69 7374   Union[str, List
+00022390: 5b73 7472 5d5d 2c0a 2020 2020 2020 2020  [str]],.        
+000223a0: 6465 7669 6365 5f74 7970 653a 204c 6974  device_type: Lit
+000223b0: 6572 616c 5b22 6170 222c 2022 6378 222c  eral["ap", "cx",
+000223c0: 2022 7377 222c 2022 7377 6974 6368 222c   "sw", "switch",
+000223d0: 2022 6777 225d 2c0a 2020 2020 2920 2d3e   "gw"],.    ) ->
+000223e0: 2052 6573 706f 6e73 653a 0a20 2020 2020   Response:.     
+000223f0: 2020 2022 2222 4173 736f 6369 6174 6520     """Associate 
+00022400: 6c69 7374 206f 6620 6465 7669 6365 7320  list of devices 
+00022410: 746f 2061 2073 6974 652e 0a0a 2020 2020  to a site...    
+00022420: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00022430: 2020 2020 2020 7369 7465 5f69 6420 2869        site_id (i
+00022440: 6e74 293a 2053 6974 6520 4944 0a20 2020  nt): Site ID.   
+00022450: 2020 2020 2020 2020 2064 6576 6963 655f           device_
+00022460: 7479 7065 2028 7374 7229 3a20 4465 7669  type (str): Devi
+00022470: 6365 2074 7970 652e 2056 616c 6964 2056  ce type. Valid V
+00022480: 616c 7565 733a 2061 702c 2063 782c 2073  alues: ap, cx, s
+00022490: 772c 2073 7769 7463 682c 2067 770a 2020  w, switch, gw.  
+000224a0: 2020 2020 2020 2020 2020 2020 2020 6378                cx
+000224b0: 2061 6e64 2073 7720 6172 6520 7468 6520   and sw are the 
+000224c0: 7361 6d65 2061 7320 7468 6520 6d6f 7265  same as the more
+000224d0: 2067 656e 6572 6963 2073 7769 7463 682e   generic switch.
+000224e0: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
+000224f0: 6961 6c5f 6e75 6d73 2028 4c69 7374 5b73  ial_nums (List[s
+00022500: 7472 5d29 3a20 4c69 7374 206f 6620 6465  tr]): List of de
+00022510: 7669 6365 2073 6572 6961 6c20 6e75 6d62  vice serial numb
+00022520: 6572 7320 6f66 2074 6865 2064 6576 6963  ers of the devic
+00022530: 6573 2074 6f20 7768 6963 6820 7468 6520  es to which the 
+00022540: 7369 7465 0a20 2020 2020 2020 2020 2020  site.           
+00022550: 2020 2020 2068 6173 2074 6f20 6265 2075       has to be u
+00022560: 6e2f 6173 736f 6369 6174 6564 2077 6974  n/associated wit
+00022570: 682e 2041 206d 6178 696d 756d 206f 6620  h. A maximum of 
+00022580: 3530 3030 2064 6576 6963 6520 7365 7269  5000 device seri
+00022590: 616c 7320 6172 6520 616c 6c6f 7765 6420  als are allowed 
+000225a0: 6174 206f 6e63 652e 0a0a 2020 2020 2020  at once...      
+000225b0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+000225c0: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
+000225d0: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
+000225e0: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
+000225f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00022600: 2320 544f 444f 206d 616b 6520 6465 7669  # TODO make devi
+00022610: 6365 5f74 7970 6573 2063 6f6e 7369 7374  ce_types consist
+00022620: 656e 7420 7468 726f 7567 686f 7574 0a20  ent throughout. 
+00022630: 2020 2020 2020 2064 6576 6963 655f 7479         device_ty
+00022640: 7065 203d 2063 6f6e 7374 616e 7473 2e6c  pe = constants.l
+00022650: 6962 5f74 6f5f 6170 6928 2273 6974 6522  ib_to_api("site"
+00022660: 2c20 6465 7669 6365 5f74 7970 6529 0a20  , device_type). 
+00022670: 2020 2020 2020 2069 6620 6e6f 7420 6465         if not de
+00022680: 7669 6365 5f74 7970 653a 0a20 2020 2020  vice_type:.     
+00022690: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+000226a0: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
+000226b0: 2020 2020 2020 2020 2066 2249 6e76 616c           f"Inval
+000226c0: 6964 2056 616c 7565 2066 6f72 2064 6576  id Value for dev
+000226d0: 6963 655f 7479 7065 2e20 2053 7570 706f  ice_type.  Suppo
+000226e0: 7274 6564 2056 616c 7565 733a 207b 636f  rted Values: {co
+000226f0: 6e73 7461 6e74 732e 6c69 625f 746f 5f61  nstants.lib_to_a
+00022700: 7069 2e76 616c 6964 5f73 7472 7d22 0a20  pi.valid_str}". 
+00022710: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00022720: 2020 2020 2020 7572 6c20 3d20 222f 6365        url = "/ce
+00022730: 6e74 7261 6c2f 7632 2f73 6974 6573 2f61  ntral/v2/sites/a
+00022740: 7373 6f63 6961 7469 6f6e 7322 0a20 2020  ssociations".   
+00022750: 2020 2020 2073 6572 6961 6c5f 6e75 6d73       serial_nums
+00022760: 203d 2075 7469 6c73 2e6c 6973 7469 6679   = utils.listify
+00022770: 2873 6572 6961 6c5f 6e75 6d73 290a 0a20  (serial_nums).. 
+00022780: 2020 2020 2020 206a 736f 6e5f 6461 7461         json_data
+00022790: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+000227a0: 2027 7369 7465 5f69 6427 3a20 7369 7465   'site_id': site
+000227b0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+000227c0: 2027 6465 7669 6365 5f69 6473 273a 2073   'device_ids': s
+000227d0: 6572 6961 6c5f 6e75 6d73 2c0a 2020 2020  erial_nums,.    
+000227e0: 2020 2020 2020 2020 2764 6576 6963 655f          'device_
+000227f0: 7479 7065 273a 2064 6576 6963 655f 7479  type': device_ty
+00022800: 7065 0a20 2020 2020 2020 207d 0a0a 2020  pe.        }..  
+00022810: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+00022820: 6974 2073 656c 662e 706f 7374 2875 726c  it self.post(url
+00022830: 2c20 6a73 6f6e 5f64 6174 613d 6a73 6f6e  , json_data=json
+00022840: 5f64 6174 6129 0a0a 2020 2020 6173 796e  _data)..    asyn
+00022850: 6320 6465 6620 7265 6d6f 7665 5f64 6576  c def remove_dev
+00022860: 6963 6573 5f66 726f 6d5f 7369 7465 280a  ices_from_site(.
+00022870: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00022880: 2020 2020 2020 7369 7465 5f69 643a 2069        site_id: i
+00022890: 6e74 2c0a 2020 2020 2020 2020 7365 7269  nt,.        seri
+000228a0: 616c 5f6e 756d 733a 204c 6973 745b 7374  al_nums: List[st
+000228b0: 725d 2c0a 2020 2020 2020 2020 6465 7669  r],.        devi
+000228c0: 6365 5f74 7970 653a 204c 6974 6572 616c  ce_type: Literal
+000228d0: 5b22 6170 222c 2022 6378 222c 2022 7377  ["ap", "cx", "sw
+000228e0: 222c 2022 7377 6974 6368 222c 2022 6777  ", "switch", "gw
+000228f0: 225d 2c0a 2020 2020 2920 2d3e 2052 6573  "],.    ) -> Res
+00022900: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
+00022910: 2222 5265 6d6f 7665 2061 206c 6973 7420  ""Remove a list 
+00022920: 6f66 2064 6576 6963 6573 2066 726f 6d20  of devices from 
+00022930: 6120 7369 7465 2e0a 0a20 2020 2020 2020  a site...       
+00022940: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00022950: 2020 2073 6974 655f 6964 2028 696e 7429     site_id (int)
+00022960: 3a20 5369 7465 2049 440a 2020 2020 2020  : Site ID.      
+00022970: 2020 2020 2020 6465 7669 6365 5f74 7970        device_typ
+00022980: 6520 2873 7472 293a 2044 6576 6963 6520  e (str): Device 
+00022990: 7479 7065 2e20 5661 6c69 6420 5661 6c75  type. Valid Valu
+000229a0: 6573 3a20 6170 2c20 6378 2c20 7377 2c20  es: ap, cx, sw, 
+000229b0: 7377 6974 6368 2c20 6777 0a20 2020 2020  switch, gw.     
+000229c0: 2020 2020 2020 2020 2020 2063 7820 616e             cx an
+000229d0: 6420 7377 2061 7265 2074 6865 2073 616d  d sw are the sam
+000229e0: 6520 6173 2074 6865 206d 6f72 6520 6765  e as the more ge
+000229f0: 6e65 7269 6320 7377 6974 6368 2e0a 2020  neric switch..  
+00022a00: 2020 2020 2020 2020 2020 7365 7269 616c            serial
+00022a10: 5f6e 756d 7320 284c 6973 745b 7374 725d  _nums (List[str]
+00022a20: 293a 204c 6973 7420 6f66 2064 6576 6963  ): List of devic
+00022a30: 6520 7365 7269 616c 206e 756d 6265 7273  e serial numbers
+00022a40: 206f 6620 7468 6520 6465 7669 6365 7320   of the devices 
+00022a50: 746f 2077 6869 6368 2074 6865 2073 6974  to which the sit
+00022a60: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00022a70: 2020 6861 7320 746f 2062 6520 756e 2f61    has to be un/a
+00022a80: 7373 6f63 6961 7465 6420 7769 7468 2e20  ssociated with. 
+00022a90: 4120 6d61 7869 6d75 6d20 6f66 2035 3030  A maximum of 500
+00022aa0: 3020 6465 7669 6365 2073 6572 6961 6c73  0 device serials
+00022ab0: 2061 7265 2061 6c6c 6f77 6564 2061 7420   are allowed at 
+00022ac0: 6f6e 6365 2e0a 0a20 2020 2020 2020 2052  once...        R
+00022ad0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00022ae0: 2020 2020 5265 7370 6f6e 7365 3a20 4365      Response: Ce
+00022af0: 6e74 7261 6c41 5049 2052 6573 706f 6e73  ntralAPI Respons
+00022b00: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
+00022b10: 2022 2222 0a20 2020 2020 2020 2064 6576   """.        dev
+00022b20: 6963 655f 7479 7065 203d 2063 6f6e 7374  ice_type = const
+00022b30: 616e 7473 2e6c 6962 5f74 6f5f 6170 6928  ants.lib_to_api(
+00022b40: 2273 6974 6522 2c20 6465 7669 6365 5f74  "site", device_t
+00022b50: 7970 6529 0a20 2020 2020 2020 2069 6620  ype).        if 
+00022b60: 6e6f 7420 6465 7669 6365 5f74 7970 653a  not device_type:
+00022b70: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00022b80: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+00022b90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00022ba0: 2249 6e76 616c 6964 2056 616c 7565 2066  "Invalid Value f
+00022bb0: 6f72 2064 6576 6963 655f 7479 7065 2e20  or device_type. 
+00022bc0: 2053 7570 706f 7274 6564 2056 616c 7565   Supported Value
+00022bd0: 733a 207b 636f 6e73 7461 6e74 732e 6c69  s: {constants.li
+00022be0: 625f 746f 5f61 7069 2e76 616c 6964 5f73  b_to_api.valid_s
+00022bf0: 7472 7d22 0a20 2020 2020 2020 2020 2020  tr}".           
+00022c00: 2029 0a0a 2020 2020 2020 2020 7572 6c20   )..        url 
+00022c10: 3d20 222f 6365 6e74 7261 6c2f 7632 2f73  = "/central/v2/s
+00022c20: 6974 6573 2f61 7373 6f63 6961 7469 6f6e  ites/association
+00022c30: 7322 0a20 2020 2020 2020 2073 6572 6961  s".        seria
+00022c40: 6c5f 6e75 6d73 203d 2075 7469 6c73 2e6c  l_nums = utils.l
+00022c50: 6973 7469 6679 2873 6572 6961 6c5f 6e75  istify(serial_nu
+00022c60: 6d73 290a 0a20 2020 2020 2020 206a 736f  ms)..        jso
+00022c70: 6e5f 6461 7461 203d 207b 0a20 2020 2020  n_data = {.     
+00022c80: 2020 2020 2020 2027 7369 7465 5f69 6427         'site_id'
+00022c90: 3a20 7369 7465 5f69 642c 0a20 2020 2020  : site_id,.     
+00022ca0: 2020 2020 2020 2027 6465 7669 6365 5f69         'device_i
+00022cb0: 6473 273a 2073 6572 6961 6c5f 6e75 6d73  ds': serial_nums
+00022cc0: 2c0a 2020 2020 2020 2020 2020 2020 2764  ,.            'd
+00022cd0: 6576 6963 655f 7479 7065 273a 2064 6576  evice_type': dev
+00022ce0: 6963 655f 7479 7065 0a20 2020 2020 2020  ice_type.       
+00022cf0: 207d 0a0a 2020 2020 2020 2020 2320 4150   }..        # AP
+00022d00: 492d 464c 4157 3a20 5468 6973 206d 6574  I-FLAW: This met
+00022d10: 686f 6420 7265 7475 726e 7320 3230 3020  hod returns 200 
+00022d20: 7768 656e 2066 6169 6c75 7265 7320 6f63  when failures oc
+00022d30: 6375 722e 0a20 2020 2020 2020 2072 6574  cur..        ret
+00022d40: 7572 6e20 6177 6169 7420 7365 6c66 2e64  urn await self.d
+00022d50: 656c 6574 6528 7572 6c2c 206a 736f 6e5f  elete(url, json_
+00022d60: 6461 7461 3d6a 736f 6e5f 6461 7461 290a  data=json_data).
+00022d70: 0a20 2020 2061 7379 6e63 2064 6566 2063  .    async def c
+00022d80: 7265 6174 655f 6c61 6265 6c28 0a20 2020  reate_label(.   
+00022d90: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00022da0: 2020 206c 6162 656c 5f6e 616d 653a 2073     label_name: s
+00022db0: 7472 2c0a 2020 2020 2020 2020 6361 7465  tr,.        cate
+00022dc0: 676f 7279 5f69 643a 2069 6e74 203d 2031  gory_id: int = 1
+00022dd0: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
+00022de0: 6e73 653a 0a20 2020 2020 2020 2022 2222  nse:.        """
+00022df0: 4372 6561 7465 204c 6162 656c 2e0a 0a20  Create Label... 
+00022e00: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00022e10: 2020 2020 2020 2020 206c 6162 656c 5f6e           label_n
+00022e20: 616d 6520 2873 7472 293a 204c 6162 656c  ame (str): Label
+00022e30: 206e 616d 650a 2020 2020 2020 2020 2020   name.          
+00022e40: 2020 6361 7465 676f 7279 5f69 6420 2869    category_id (i
+00022e50: 6e74 2c20 6f70 7469 6f6e 616c 293a 204c  nt, optional): L
+00022e60: 6162 656c 2063 6174 6567 6f72 7920 4944  abel category ID
+00022e70: 2064 6566 6175 6c74 7320 746f 2031 0a20   defaults to 1. 
+00022e80: 2020 2020 2020 2020 2020 2020 2020 2031                 1
+00022e90: 203d 2064 6566 6175 6c74 206c 6162 656c   = default label
+00022ea0: 2063 6174 6567 6f72 792c 2032 203d 2073   category, 2 = s
+00022eb0: 6974 650a 0a20 2020 2020 2020 2052 6574  ite..        Ret
+00022ec0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00022ed0: 2020 5265 7370 6f6e 7365 3a20 4365 6e74    Response: Cent
+00022ee0: 7261 6c41 5049 2052 6573 706f 6e73 6520  ralAPI Response 
+00022ef0: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
+00022f00: 2222 0a20 2020 2020 2020 2075 726c 203d  "".        url =
+00022f10: 2022 2f63 656e 7472 616c 2f76 312f 6c61   "/central/v1/la
+00022f20: 6265 6c73 220a 0a20 2020 2020 2020 206a  bels"..        j
+00022f30: 736f 6e5f 6461 7461 203d 207b 0a20 2020  son_data = {.   
+00022f40: 2020 2020 2020 2020 2027 6361 7465 676f           'catego
+00022f50: 7279 5f69 6427 3a20 6361 7465 676f 7279  ry_id': category
+00022f60: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+00022f70: 2027 6c61 6265 6c5f 6e61 6d65 273a 206c   'label_name': l
+00022f80: 6162 656c 5f6e 616d 650a 2020 2020 2020  abel_name.      
+00022f90: 2020 7d0a 0a20 2020 2020 2020 2072 6574    }..        ret
+00022fa0: 7572 6e20 6177 6169 7420 7365 6c66 2e70  urn await self.p
+00022fb0: 6f73 7428 7572 6c2c 206a 736f 6e5f 6461  ost(url, json_da
+00022fc0: 7461 3d6a 736f 6e5f 6461 7461 290a 0a20  ta=json_data).. 
+00022fd0: 2020 2061 7379 6e63 2064 6566 2067 6574     async def get
+00022fe0: 5f6c 6162 656c 7328 0a20 2020 2020 2020  _labels(.       
+00022ff0: 2073 656c 662c 0a20 2020 2020 2020 2063   self,.        c
+00023000: 616c 6375 6c61 7465 5f74 6f74 616c 3a20  alculate_total: 
+00023010: 626f 6f6c 203d 204e 6f6e 652c 0a20 2020  bool = None,.   
+00023020: 2020 2020 2072 6576 6572 7365 3a20 626f       reverse: bo
+00023030: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+00023040: 2020 2020 6f66 6673 6574 3a20 696e 7420      offset: int 
+00023050: 3d20 302c 0a20 2020 2020 2020 206c 696d  = 0,.        lim
+00023060: 6974 3a20 696e 7420 3d20 3130 302c 0a20  it: int = 100,. 
+00023070: 2020 2029 202d 3e20 5265 7370 6f6e 7365     ) -> Response
+00023080: 3a0a 2020 2020 2020 2020 2222 224c 6973  :.        """Lis
+00023090: 7420 4c61 6265 6c73 2e0a 0a20 2020 2020  t Labels...     
+000230a0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+000230b0: 2020 2020 2063 616c 6375 6c61 7465 5f74       calculate_t
+000230c0: 6f74 616c 2028 626f 6f6c 2c20 6f70 7469  otal (bool, opti
+000230d0: 6f6e 616c 293a 2057 6865 7468 6572 2074  onal): Whether t
+000230e0: 6f20 6361 6c63 756c 6174 6520 746f 7461  o calculate tota
+000230f0: 6c20 4c61 6265 6c73 0a20 2020 2020 2020  l Labels.       
+00023100: 2020 2020 2072 6576 6572 7365 2028 626f       reverse (bo
+00023110: 6f6c 2c20 6f70 7469 6f6e 616c 293a 204c  ol, optional): L
+00023120: 6973 7420 6c61 6265 6c73 2069 6e20 7265  ist labels in re
+00023130: 7665 7273 6520 616c 7068 6162 6574 6963  verse alphabetic
+00023140: 616c 206f 7264 6572 2e20 4465 6661 756c  al order. Defaul
+00023150: 7473 2074 6f20 4661 6c73 650a 2020 2020  ts to False.    
+00023160: 2020 2020 2020 2020 6f66 6673 6574 2028          offset (
+00023170: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
+00023180: 5061 6769 6e61 7469 6f6e 206f 6666 7365  Pagination offse
+00023190: 7420 4465 6661 756c 7473 2074 6f20 302e  t Defaults to 0.
+000231a0: 0a20 2020 2020 2020 2020 2020 206c 696d  .            lim
+000231b0: 6974 2028 696e 742c 206f 7074 696f 6e61  it (int, optiona
+000231c0: 6c29 3a20 5061 6769 6e61 7469 6f6e 206c  l): Pagination l
+000231d0: 696d 6974 2e20 4465 6661 756c 7420 6973  imit. Default is
+000231e0: 2031 3030 2061 6e64 206d 6178 2069 7320   100 and max is 
+000231f0: 3130 3030 2044 6566 6175 6c74 7320 746f  1000 Defaults to
+00023200: 2031 3030 2e0a 0a20 2020 2020 2020 2052   100...        R
+00023210: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00023220: 2020 2020 5265 7370 6f6e 7365 3a20 4365      Response: Ce
+00023230: 6e74 7261 6c41 5049 2052 6573 706f 6e73  ntralAPI Respons
+00023240: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
+00023250: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
+00023260: 203d 2022 2f63 656e 7472 616c 2f76 322f   = "/central/v2/
+00023270: 6c61 6265 6c73 220a 0a20 2020 2020 2020  labels"..       
+00023280: 2070 6172 616d 7320 3d20 7b0a 2020 2020   params = {.    
+00023290: 2020 2020 2020 2020 2263 616c 6375 6c61          "calcula
+000232a0: 7465 5f74 6f74 616c 223a 2063 616c 6375  te_total": calcu
+000232b0: 6c61 7465 5f74 6f74 616c 2c0a 2020 2020  late_total,.    
+000232c0: 2020 2020 2020 2020 226f 6666 7365 7422          "offset"
+000232d0: 3a20 6f66 6673 6574 2c0a 2020 2020 2020  : offset,.      
+000232e0: 2020 2020 2020 226c 696d 6974 223a 206c        "limit": l
+000232f0: 696d 6974 0a20 2020 2020 2020 207d 0a20  imit.        }. 
+00023300: 2020 2020 2020 2069 6620 7265 7665 7273         if revers
+00023310: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+00023320: 6172 616d 735b 2273 6f72 7422 5d20 3d20  arams["sort"] = 
+00023330: 222d 6c61 6265 6c5f 6e61 6d65 220a 0a20  "-label_name".. 
+00023340: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
+00023350: 6169 7420 7365 6c66 2e67 6574 2875 726c  ait self.get(url
+00023360: 2c20 7061 7261 6d73 3d70 6172 616d 7329  , params=params)
+00023370: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00023380: 6173 7369 676e 5f6c 6162 656c 5f74 6f5f  assign_label_to_
+00023390: 6465 7669 6365 7328 0a20 2020 2020 2020  devices(.       
+000233a0: 2073 656c 662c 0a20 2020 2020 2020 206c   self,.        l
+000233b0: 6162 656c 5f69 643a 2069 6e74 2c0a 2020  abel_id: int,.  
+000233c0: 2020 2020 2020 6465 7669 6365 5f74 7970        device_typ
+000233d0: 653a 2063 6f6e 7374 616e 7473 2e47 656e  e: constants.Gen
+000233e0: 6572 6963 4465 7654 7970 6573 2c0a 2020  ericDevTypes,.  
+000233f0: 2020 2020 2020 7365 7269 616c 5f6e 756d        serial_num
+00023400: 733a 2055 6e69 6f6e 5b73 7472 2c20 4c69  s: Union[str, Li
+00023410: 7374 5b73 7472 5d5d 2c0a 2020 2020 2920  st[str]],.    ) 
+00023420: 2d3e 2052 6573 706f 6e73 653a 0a20 2020  -> Response:.   
+00023430: 2020 2020 2022 2222 4173 736f 6369 6174       """Associat
+00023440: 6520 4c61 6265 6c20 746f 2061 206c 6973  e Label to a lis
+00023450: 7420 6f66 2064 6576 6963 6573 2e0a 0a20  t of devices... 
+00023460: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00023470: 2020 2020 2020 2020 206c 6162 656c 5f69           label_i
+00023480: 6420 2869 6e74 293a 204c 6162 656c 2049  d (int): Label I
+00023490: 440a 2020 2020 2020 2020 2020 2020 6465  D.            de
+000234a0: 7669 6365 5f74 7970 6520 2873 7472 293a  vice_type (str):
+000234b0: 2044 6576 6963 6520 7479 7065 2e20 5661   Device type. Va
+000234c0: 6c69 6420 5661 6c75 6573 3a20 6170 2c20  lid Values: ap, 
+000234d0: 6777 2c20 7377 6974 6368 0a20 2020 2020  gw, switch.     
+000234e0: 2020 2020 2020 2073 6572 6961 6c5f 6e75         serial_nu
+000234f0: 6d73 2028 7374 7220 7c20 4c69 7374 5b73  ms (str | List[s
+00023500: 7472 5d29 3a20 4c69 7374 206f 6620 6465  tr]): List of de
+00023510: 7669 6365 2073 6572 6961 6c20 6e75 6d62  vice serial numb
+00023520: 6572 7320 6f66 2074 6865 2064 6576 6963  ers of the devic
+00023530: 6573 2074 6f20 7768 6963 6820 7468 6520  es to which the 
+00023540: 6c61 6265 6c0a 2020 2020 2020 2020 2020  label.          
+00023550: 2020 2020 2020 6861 7320 746f 2062 6520        has to be 
+00023560: 756e 2f61 7373 6f63 6961 7465 6420 7769  un/associated wi
+00023570: 7468 2e20 4120 6d61 7869 6d75 6d20 6f66  th. A maximum of
+00023580: 2035 3030 3020 6465 7669 6365 2073 6572   5000 device ser
+00023590: 6961 6c73 2061 7265 2061 6c6c 6f77 6564  ials are allowed
+000235a0: 2061 7420 6f6e 6365 2e0a 0a20 2020 2020   at once...     
+000235b0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+000235c0: 2020 2020 2020 2020 5265 7370 6f6e 7365          Response
+000235d0: 3a20 4365 6e74 7261 6c41 5049 2052 6573  : CentralAPI Res
+000235e0: 706f 6e73 6520 6f62 6a65 6374 0a20 2020  ponse object.   
+000235f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00023600: 2075 726c 203d 2022 2f63 656e 7472 616c   url = "/central
+00023610: 2f76 322f 6c61 6265 6c73 2f61 7373 6f63  /v2/labels/assoc
+00023620: 6961 7469 6f6e 7322 0a20 2020 2020 2020  iations".       
+00023630: 2073 6572 6961 6c5f 6e75 6d73 203d 2075   serial_nums = u
+00023640: 7469 6c73 2e6c 6973 7469 6679 2873 6572  tils.listify(ser
+00023650: 6961 6c5f 6e75 6d73 290a 2020 2020 2020  ial_nums).      
+00023660: 2020 6465 7669 6365 5f74 7970 6520 3d20    device_type = 
+00023670: 636f 6e73 7461 6e74 732e 6c69 625f 746f  constants.lib_to
+00023680: 5f61 7069 2822 7369 7465 222c 2064 6576  _api("site", dev
+00023690: 6963 655f 7479 7065 290a 0a20 2020 2020  ice_type)..     
+000236a0: 2020 206a 736f 6e5f 6461 7461 203d 207b     json_data = {
+000236b0: 0a20 2020 2020 2020 2020 2020 2027 6c61  .            'la
+000236c0: 6265 6c5f 6964 273a 206c 6162 656c 5f69  bel_id': label_i
+000236d0: 642c 0a20 2020 2020 2020 2020 2020 2027  d,.            '
+000236e0: 6465 7669 6365 5f74 7970 6527 3a20 6465  device_type': de
+000236f0: 7669 6365 5f74 7970 652c 0a20 2020 2020  vice_type,.     
+00023700: 2020 2020 2020 2027 6465 7669 6365 5f69         'device_i
+00023710: 6473 273a 2073 6572 6961 6c5f 6e75 6d73  ds': serial_nums
+00023720: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+00023730: 2020 2020 7265 7475 726e 2061 7761 6974      return await
+00023740: 2073 656c 662e 706f 7374 2875 726c 2c20   self.post(url, 
+00023750: 6a73 6f6e 5f64 6174 613d 6a73 6f6e 5f64  json_data=json_d
+00023760: 6174 6129 0a0a 2020 2020 2320 544f 444f  ata)..    # TODO
+00023770: 206d 616b 6520 666f 726d 6174 206f 6620   make format of 
+00023780: 7468 6973 2061 6e64 206f 7468 6572 206c  this and other l
+00023790: 6162 656c 206d 6574 686f 6473 206d 6174  abel methods mat
+000237a0: 6368 2073 6974 6520 6d65 7468 6f64 730a  ch site methods.
+000237b0: 2020 2020 6173 796e 6320 6465 6620 7265      async def re
+000237c0: 6d6f 7665 5f6c 6162 656c 5f66 726f 6d5f  move_label_from_
+000237d0: 6465 7669 6365 7328 0a20 2020 2020 2020  devices(.       
+000237e0: 2073 656c 662c 0a20 2020 2020 2020 206c   self,.        l
+000237f0: 6162 656c 5f69 643a 2069 6e74 2c0a 2020  abel_id: int,.  
+00023800: 2020 2020 2020 6465 7669 6365 5f74 7970        device_typ
+00023810: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+00023820: 7365 7269 616c 5f6e 756d 733a 204c 6973  serial_nums: Lis
+00023830: 745b 7374 725d 2c0a 2020 2020 2920 2d3e  t[str],.    ) ->
+00023840: 2052 6573 706f 6e73 653a 0a20 2020 2020   Response:.     
+00023850: 2020 2022 2222 756e 6173 7369 676e 2061     """unassign a
+00023860: 206c 6162 656c 2066 726f 6d20 6120 6c69   label from a li
+00023870: 7374 206f 6620 6465 7669 6365 732e 0a0a  st of devices...
+00023880: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00023890: 2020 2020 2020 2020 2020 6c61 6265 6c5f            label_
+000238a0: 6964 2028 696e 7429 3a20 4c61 6265 6c20  id (int): Label 
+000238b0: 4944 0a20 2020 2020 2020 2020 2020 2064  ID.            d
+000238c0: 6576 6963 655f 7479 7065 2028 7374 7229  evice_type (str)
+000238d0: 3a20 4465 7669 6365 2074 7970 652e 204f  : Device type. O
+000238e0: 6e65 206f 6620 6170 2c20 6777 2c20 7377  ne of ap, gw, sw
+000238f0: 6974 6368 0a20 2020 2020 2020 2020 2020  itch.           
+00023900: 2073 6572 6961 6c5f 6e75 6d73 2028 7374   serial_nums (st
+00023910: 7220 7c20 4c69 7374 5b73 7472 5d29 3a20  r | List[str]): 
+00023920: 4c69 7374 206f 6620 6465 7669 6365 2073  List of device s
+00023930: 6572 6961 6c20 6e75 6d62 6572 7320 6f66  erial numbers of
+00023940: 2074 6865 2064 6576 6963 6573 2074 6f20   the devices to 
+00023950: 7768 6963 6820 7468 6520 6c61 6265 6c0a  which the label.
+00023960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023970: 6861 7320 746f 2062 6520 756e 2f61 7373  has to be un/ass
+00023980: 6f63 6961 7465 6420 7769 7468 2e20 4120  ociated with. A 
+00023990: 6d61 7869 6d75 6d20 6f66 2035 3030 3020  maximum of 5000 
+000239a0: 6465 7669 6365 2073 6572 6961 6c73 2061  device serials a
+000239b0: 7265 2061 6c6c 6f77 6564 2061 7420 6f6e  re allowed at on
+000239c0: 6365 2e0a 0a20 2020 2020 2020 2052 6574  ce...        Ret
+000239d0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+000239e0: 2020 5265 7370 6f6e 7365 3a20 4365 6e74    Response: Cent
+000239f0: 7261 6c41 5049 2052 6573 706f 6e73 6520  ralAPI Response 
+00023a00: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
+00023a10: 2222 0a20 2020 2020 2020 2075 726c 203d  "".        url =
+00023a20: 2022 2f63 656e 7472 616c 2f76 322f 6c61   "/central/v2/la
+00023a30: 6265 6c73 2f61 7373 6f63 6961 7469 6f6e  bels/association
+00023a40: 7322 0a20 2020 2020 2020 2073 6572 6961  s".        seria
+00023a50: 6c5f 6e75 6d73 203d 2075 7469 6c73 2e6c  l_nums = utils.l
+00023a60: 6973 7469 6679 2873 6572 6961 6c5f 6e75  istify(serial_nu
+00023a70: 6d73 290a 2020 2020 2020 2020 6465 7669  ms).        devi
+00023a80: 6365 5f74 7970 6520 3d20 636f 6e73 7461  ce_type = consta
+00023a90: 6e74 732e 6c69 625f 746f 5f61 7069 2822  nts.lib_to_api("
+00023aa0: 7369 7465 222c 2064 6576 6963 655f 7479  site", device_ty
+00023ab0: 7065 290a 0a20 2020 2020 2020 206a 736f  pe)..        jso
+00023ac0: 6e5f 6461 7461 203d 207b 0a20 2020 2020  n_data = {.     
+00023ad0: 2020 2020 2020 2027 6c61 6265 6c5f 6964         'label_id
+00023ae0: 273a 206c 6162 656c 5f69 642c 0a20 2020  ': label_id,.   
+00023af0: 2020 2020 2020 2020 2027 6465 7669 6365           'device
+00023b00: 5f74 7970 6527 3a20 6465 7669 6365 5f74  _type': device_t
+00023b10: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
+00023b20: 2027 6465 7669 6365 5f69 6473 273a 2073   'device_ids': s
+00023b30: 6572 6961 6c5f 6e75 6d73 0a20 2020 2020  erial_nums.     
+00023b40: 2020 207d 0a0a 2020 2020 2020 2020 7265     }..        re
+00023b50: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+00023b60: 6465 6c65 7465 2875 726c 2c20 6a73 6f6e  delete(url, json
+00023b70: 5f64 6174 613d 6a73 6f6e 5f64 6174 6129  _data=json_data)
+00023b80: 0a0a 2020 2020 2320 4150 492d 464c 4157  ..    # API-FLAW
+00023b90: 2072 6574 7572 6e73 2065 6d70 7479 2070   returns empty p
+00023ba0: 6179 6c6f 6164 202f 2072 6573 706f 6e73  ayload / respons
+00023bb0: 6520 6f6e 2073 7563 6365 7373 2032 3030  e on success 200
+00023bc0: 0a20 2020 2061 7379 6e63 2064 6566 2064  .    async def d
+00023bd0: 656c 6574 655f 6c61 6265 6c28 0a20 2020  elete_label(.   
+00023be0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00023bf0: 2020 206c 6162 656c 5f69 643a 2069 6e74     label_id: int
+00023c00: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
+00023c10: 6e73 653a 0a20 2020 2020 2020 2022 2222  nse:.        """
+00023c20: 4465 6c65 7465 204c 6162 656c 2e0a 0a20  Delete Label... 
+00023c30: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00023c40: 2020 2020 2020 2020 206c 6162 656c 5f69           label_i
+00023c50: 6420 2869 6e74 293a 204c 6162 656c 2049  d (int): Label I
+00023c60: 440a 0a20 2020 2020 2020 2052 6574 7572  D..        Retur
+00023c70: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00023c80: 5265 7370 6f6e 7365 3a20 4365 6e74 7261  Response: Centra
+00023c90: 6c41 5049 2052 6573 706f 6e73 6520 6f62  lAPI Response ob
+00023ca0: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
+00023cb0: 0a20 2020 2020 2020 2075 726c 203d 2066  .        url = f
+00023cc0: 222f 6365 6e74 7261 6c2f 7631 2f6c 6162  "/central/v1/lab
+00023cd0: 656c 732f 7b6c 6162 656c 5f69 647d 220a  els/{label_id}".
+00023ce0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00023cf0: 6177 6169 7420 7365 6c66 2e64 656c 6574  await self.delet
+00023d00: 6528 7572 6c29 0a0a 2020 2020 6173 796e  e(url)..    asyn
+00023d10: 6320 6465 6620 6765 745f 6465 7669 6365  c def get_device
+00023d20: 5f69 705f 726f 7574 6573 280a 2020 2020  _ip_routes(.    
+00023d30: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00023d40: 2020 7365 7269 616c 5f6e 756d 3a20 7374    serial_num: st
+00023d50: 722c 0a20 2020 2020 2020 2061 7069 3a20  r,.        api: 
+00023d60: 7374 7220 3d20 2256 3122 2c0a 2020 2020  str = "V1",.    
+00023d70: 2020 2020 6f66 6673 6574 3a20 696e 7420      offset: int 
+00023d80: 3d20 302c 0a20 2020 2020 2020 206c 696d  = 0,.        lim
+00023d90: 6974 3a20 696e 7420 3d20 3130 300a 2020  it: int = 100.  
+00023da0: 2020 2920 2d3e 2052 6573 706f 6e73 653a    ) -> Response:
+00023db0: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+00023dc0: 726f 7574 6573 2066 6f72 2061 2064 6576  routes for a dev
+00023dd0: 6963 652e 0a0a 2020 2020 2020 2020 4172  ice...        Ar
+00023de0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00023df0: 7365 7269 616c 5f6e 756d 2028 7374 7229  serial_num (str)
+00023e00: 3a20 4465 7669 6365 2073 6572 6961 6c20  : Device serial 
+00023e10: 6e75 6d62 6572 0a20 2020 2020 2020 2020  number.         
+00023e20: 2020 2061 7069 2028 7374 722c 206f 7074     api (str, opt
+00023e30: 696f 6e61 6c29 3a20 4150 4920 7665 7273  ional): API vers
+00023e40: 696f 6e20 2856 307c 5631 292c 2044 6566  ion (V0|V1), Def
+00023e50: 6175 6c74 7320 746f 2056 312e 0a20 2020  aults to V1..   
+00023e60: 2020 2020 2020 2020 206f 6666 7365 7420           offset 
+00023e70: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+00023e80: 2050 6167 696e 6174 696f 6e20 6f66 6673   Pagination offs
+00023e90: 6574 2e0a 2020 2020 2020 2020 2020 2020  et..            
+00023ea0: 6c69 6d69 7420 2869 6e74 2c20 6f70 7469  limit (int, opti
+00023eb0: 6f6e 616c 293a 2070 6167 6520 7369 7a65  onal): page size
+00023ec0: 2044 6566 6175 6c74 7320 746f 2031 3030   Defaults to 100
+00023ed0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00023ee0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00023ef0: 5265 7370 6f6e 7365 3a20 4365 6e74 7261  Response: Centra
+00023f00: 6c41 5049 2052 6573 706f 6e73 6520 6f62  lAPI Response ob
+00023f10: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
+00023f20: 0a20 2020 2020 2020 2075 726c 203d 2022  .        url = "
+00023f30: 2f61 7069 2f72 6f75 7469 6e67 2f76 312f  /api/routing/v1/
+00023f40: 726f 7574 6522 0a0a 2020 2020 2020 2020  route"..        
+00023f50: 7061 7261 6d73 203d 207b 0a20 2020 2020  params = {.     
+00023f60: 2020 2020 2020 2027 6465 7669 6365 273a         'device':
+00023f70: 2073 6572 6961 6c5f 6e75 6d2c 0a20 2020   serial_num,.   
+00023f80: 2020 2020 2020 2020 2027 6170 6927 3a20           'api': 
+00023f90: 6170 692c 0a20 2020 2020 2020 2020 2020  api,.           
+00023fa0: 2027 6d61 726b 6572 273a 206f 6666 7365   'marker': offse
+00023fb0: 742c 0a20 2020 2020 2020 2020 2020 2027  t,.            '
+00023fc0: 6c69 6d69 7427 3a20 6c69 6d69 740a 2020  limit': limit.  
+00023fd0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00023fe0: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
+00023ff0: 6c66 2e67 6574 2875 726c 2c20 7061 7261  lf.get(url, para
+00024000: 6d73 3d70 6172 616d 7329 0a0a 2020 2020  ms=params)..    
+00024010: 2320 544f 444f 206d 616b 6520 6164 645f  # TODO make add_
+00024020: 6465 7669 6365 2061 6374 7561 6c20 6675  device actual fu
+00024030: 6e63 2073 6570 2061 6e64 206d 616b 6520  nc sep and make 
+00024040: 7468 6973 2061 6e20 6167 6772 6567 6174  this an aggregat
+00024050: 6f72 2074 6861 7420 6361 6c6c 7320 6974  or that calls it
+00024060: 2061 6e64 2061 6e79 7468 696e 6720 656c   and anything el
+00024070: 7365 2062 6173 6564 206f 6e20 7061 7261  se based on para
+00024080: 6d73 0a20 2020 2061 7379 6e63 2064 6566  ms.    async def
+00024090: 2061 6464 5f64 6576 6963 6573 280a 2020   add_devices(.  
+000240a0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000240b0: 2020 2020 6d61 635f 6164 6472 6573 733a      mac_address:
+000240c0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000240d0: 2020 2020 2073 6572 6961 6c5f 6e75 6d3a       serial_num:
+000240e0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000240f0: 2020 2020 2067 726f 7570 3a20 7374 7220       group: str 
+00024100: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00024110: 2320 7369 7465 3a20 696e 7420 3d20 4e6f  # site: int = No
+00024120: 6e65 2c0a 2020 2020 2020 2020 7061 7274  ne,.        part
+00024130: 5f6e 756d 3a20 7374 7220 3d20 4e6f 6e65  _num: str = None
+00024140: 2c0a 2020 2020 2020 2020 6c69 6365 6e73  ,.        licens
+00024150: 653a 2055 6e69 6f6e 5b73 7472 2c20 4c69  e: Union[str, Li
+00024160: 7374 5b73 7472 5d5d 203d 204e 6f6e 652c  st[str]] = None,
+00024170: 0a20 2020 2020 2020 2064 6576 6963 655f  .        device_
+00024180: 6c69 7374 3a20 4c69 7374 5b44 6963 745b  list: List[Dict[
+00024190: 7374 722c 2073 7472 5d5d 203d 204e 6f6e  str, str]] = Non
+000241a0: 650a 2020 2020 2920 2d3e 2055 6e69 6f6e  e.    ) -> Union
+000241b0: 5b52 6573 706f 6e73 652c 204c 6973 745b  [Response, List[
+000241c0: 5265 7370 6f6e 7365 5d5d 3a0a 2020 2020  Response]]:.    
+000241d0: 2020 2020 2222 2241 6464 2064 6576 6963      """Add devic
+000241e0: 6528 7329 2075 7369 6e67 204d 6163 2061  e(s) using Mac a
+000241f0: 6e64 2053 6572 6961 6c20 6e75 6d62 6572  nd Serial number
+00024200: 2028 7061 7274 5f6e 756d 2061 6c73 6f20   (part_num also 
+00024210: 7265 7175 6972 6564 2066 6f72 2043 6f50  required for CoP
+00024220: 290a 2020 2020 2020 2020 5769 6c6c 2061  ).        Will a
+00024230: 6c73 6f20 7072 652d 6173 7369 676e 2064  lso pre-assign d
+00024240: 6576 6963 6520 746f 2067 726f 7570 2069  evice to group i
+00024250: 6620 7072 6f76 6964 6564 0a0a 2020 2020  f provided..    
+00024260: 2020 2020 4569 7468 6572 206d 6163 5f61      Either mac_a
+00024270: 6464 7265 7373 2061 6e64 2073 6572 6961  ddress and seria
+00024280: 6c5f 6e75 6d20 6f72 2064 6576 6963 655f  l_num or device_
+00024290: 6c69 7374 2028 7768 6963 6820 7368 6f75  list (which shou
+000242a0: 6c64 2063 6f6e 7461 696e 2061 2064 6963  ld contain a dic
+000242b0: 7420 7769 7468 206d 6163 2073 6572 6961  t with mac seria
+000242c0: 6c29 2061 7265 2072 6571 7569 7265 642e  l) are required.
+000242d0: 0a20 2020 2020 2020 202f 2f20 5573 6564  .        // Used
+000242e0: 2062 7920 6164 6420 6465 7669 6365 2061   by add device a
+000242f0: 6e64 2062 6174 6368 2061 6464 2064 6576  nd batch add dev
+00024300: 6963 6573 202f 2f0a 0a20 2020 2020 2020  ices //..       
+00024310: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00024320: 2020 206d 6163 5f61 6464 7265 7373 2028     mac_address (
+00024330: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+00024340: 4d41 4320 6164 6472 6573 7320 6f66 2064  MAC address of d
+00024350: 6576 6963 6520 746f 2062 6520 6164 6465  evice to be adde
+00024360: 640a 2020 2020 2020 2020 2020 2020 7365  d.            se
+00024370: 7269 616c 5f6e 756d 2028 7374 722c 206f  rial_num (str, o
+00024380: 7074 696f 6e61 6c29 3a20 5365 7269 616c  ptional): Serial
+00024390: 206e 756d 6265 7220 6f66 2064 6576 6963   number of devic
+000243a0: 6520 746f 2062 6520 6164 6465 640a 2020  e to be added.  
+000243b0: 2020 2020 2020 2020 2020 6772 6f75 7020            group 
+000243c0: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+000243d0: 2041 6464 2064 6576 6963 6520 746f 2070   Add device to p
+000243e0: 7265 2d70 726f 7669 7369 6f6e 6564 2067  re-provisioned g
+000243f0: 726f 7570 2028 6164 6469 7469 6f6e 616c  roup (additional
+00024400: 2041 5049 2063 616c 6c20 6973 206d 6164   API call is mad
+00024410: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
+00024420: 6974 6520 2869 6e74 2c20 6f70 7469 6f6e  ite (int, option
+00024430: 616c 293a 202d 2d20 4e6f 7420 696d 706c  al): -- Not impl
+00024440: 656d 656e 7465 6420 2d2d 2053 6974 6520  emented -- Site 
+00024450: 4944 0a20 2020 2020 2020 2020 2020 2070  ID.            p
+00024460: 6172 745f 6e75 6d20 2873 7472 2c20 6f70  art_num (str, op
+00024470: 7469 6f6e 616c 293a 2050 6172 7420 4e75  tional): Part Nu
+00024480: 6d62 6572 2069 7320 7265 7175 6972 6564  mber is required
+00024490: 2066 6f72 2043 656e 7472 616c 204f 6e20   for Central On 
+000244a0: 5072 656d 2e0a 2020 2020 2020 2020 2020  Prem..          
+000244b0: 2020 6c69 6365 6e73 6520 2873 7472 7c4c    license (str|L
+000244c0: 6973 7428 7374 7229 2c20 6f70 7469 6f6e  ist(str), option
+000244d0: 616c 293a 2054 6865 2073 7562 7363 7269  al): The subscri
+000244e0: 7074 696f 6e20 6c69 6365 6e73 6528 7329  ption license(s)
+000244f0: 2074 6f20 6173 7369 676e 2e0a 2020 2020   to assign..    
+00024500: 2020 2020 2020 2020 6465 7669 6365 5f6c          device_l
+00024510: 6973 7420 284c 6973 745b 4469 6374 5b73  ist (List[Dict[s
+00024520: 7472 2c20 7374 725d 5d2c 206f 7074 696f  tr, str]], optio
+00024530: 6e61 6c29 3a20 4c69 7374 206f 6620 6469  nal): List of di
+00024540: 6374 7320 7769 7468 206d 6163 2c20 7365  cts with mac, se
+00024550: 7269 616c 2066 6f72 2065 6163 6820 6465  rial for each de
+00024560: 7669 6365 0a20 2020 2020 2020 2020 2020  vice.           
+00024570: 2020 2020 2061 6e64 206f 7074 696f 6e61       and optiona
+00024580: 6c6c 7920 6772 6f75 702c 2070 6172 745f  lly group, part_
+00024590: 6e75 6d2c 206c 6963 656e 7365 2c0a 0a20  num, license,.. 
+000245a0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+000245b0: 2020 2020 2020 2020 2020 2020 5265 7370              Resp
+000245c0: 6f6e 7365 3a20 4365 6e74 7261 6c41 5049  onse: CentralAPI
+000245d0: 2052 6573 706f 6e73 6520 6f62 6a65 6374   Response object
+000245e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000245f0: 2020 2020 2075 726c 203d 2022 2f70 6c61       url = "/pla
+00024600: 7466 6f72 6d2f 6465 7669 6365 5f69 6e76  tform/device_inv
+00024610: 656e 746f 7279 2f76 312f 6465 7669 6365  entory/v1/device
+00024620: 7322 0a20 2020 2020 2020 206c 6963 656e  s".        licen
+00024630: 7365 5f6b 7761 7267 7320 3d20 5b5d 0a0a  se_kwargs = []..
+00024640: 2020 2020 2020 2020 6966 206c 6963 656e          if licen
+00024650: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00024660: 6c69 6365 6e73 655f 6b77 6172 6773 203d  license_kwargs =
+00024670: 205b 7b22 7365 7269 616c 7322 3a20 5b73   [{"serials": [s
+00024680: 6572 6961 6c5f 6e75 6d5d 2c20 2273 6572  erial_num], "ser
+00024690: 7669 6365 7322 3a20 7574 696c 732e 6c69  vices": utils.li
+000246a0: 7374 6966 7928 6c69 6365 6e73 6529 7d5d  stify(license)}]
+000246b0: 0a20 2020 2020 2020 2069 6620 7365 7269  .        if seri
+000246c0: 616c 5f6e 756d 2061 6e64 206d 6163 5f61  al_num and mac_a
+000246d0: 6464 7265 7373 3a0a 2020 2020 2020 2020  ddress:.        
+000246e0: 2020 2020 6966 2064 6576 6963 655f 6c69      if device_li
+000246f0: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+00024700: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00024710: 7272 6f72 2822 7365 7269 616c 5f6e 756d  rror("serial_num
+00024720: 2061 6e64 206d 6163 5f61 6464 7265 7373   and mac_address
+00024730: 2061 7265 206e 6f74 2065 7870 6563 7465   are not expecte
+00024740: 6420 7768 656e 2064 6576 6963 655f 6c69  d when device_li
+00024750: 7374 2069 7320 6265 696e 6720 7072 6f76  st is being prov
+00024760: 6964 6564 2e22 290a 0a20 2020 2020 2020  ided.")..       
+00024770: 2020 2020 2074 6f5f 6772 6f75 7020 3d20       to_group = 
+00024780: 4e6f 6e65 2069 6620 6e6f 7420 6772 6f75  None if not grou
+00024790: 7020 656c 7365 207b 6772 6f75 703a 205b  p else {group: [
+000247a0: 7365 7269 616c 5f6e 756d 5d7d 0a20 2020  serial_num]}.   
+000247b0: 2020 2020 2020 2020 2023 2074 6f5f 7369           # to_si
+000247c0: 7465 203d 204e 6f6e 6520 6966 206e 6f74  te = None if not
+000247d0: 2073 6974 6520 656c 7365 207b 7369 7465   site else {site
+000247e0: 3a20 5b73 6572 6961 6c5f 6e75 6d5d 7d0a  : [serial_num]}.
+000247f0: 0a20 2020 2020 2020 2020 2020 206d 6163  .            mac
+00024800: 203d 2075 7469 6c73 2e4d 6163 286d 6163   = utils.Mac(mac
+00024810: 5f61 6464 7265 7373 290a 2020 2020 2020  _address).      
+00024820: 2020 2020 2020 6966 206e 6f74 206d 6163        if not mac
+00024830: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00024840: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00024850: 6f72 2866 226d 6163 5f61 6464 7265 7373  or(f"mac_address
+00024860: 207b 6d61 635f 6164 6472 6573 737d 2061   {mac_address} a
+00024870: 7070 6561 7273 2074 6f20 6265 2069 6e76  ppears to be inv
+00024880: 616c 6964 2e22 290a 0a20 2020 2020 2020  alid.")..       
+00024890: 2020 2020 206a 736f 6e5f 6461 7461 203d       json_data =
+000248a0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+000248b0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+000248c0: 2020 2020 2020 2020 2022 6d61 6322 3a20           "mac": 
+000248d0: 6d61 632e 636f 6c73 2c0a 2020 2020 2020  mac.cols,.      
+000248e0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+000248f0: 6572 6961 6c22 3a20 7365 7269 616c 5f6e  erial": serial_n
+00024900: 756d 0a20 2020 2020 2020 2020 2020 2020  um.             
+00024910: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+00024920: 205d 0a20 2020 2020 2020 2020 2020 2069   ].            i
+00024930: 6620 7061 7274 5f6e 756d 3a0a 2020 2020  f part_num:.    
+00024940: 2020 2020 2020 2020 2020 2020 6a73 6f6e              json
+00024950: 5f64 6174 615b 305d 5b22 7061 7274 4e75  _data[0]["partNu
+00024960: 6d62 6572 225d 203d 2070 6172 745f 6e75  mber"] = part_nu
+00024970: 6d0a 0a20 2020 2020 2020 2065 6c69 6620  m..        elif 
+00024980: 6465 7669 6365 5f6c 6973 743a 0a20 2020  device_list:.   
+00024990: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000249a0: 6973 696e 7374 616e 6365 2864 6576 6963  isinstance(devic
+000249b0: 655f 6c69 7374 2c20 6c69 7374 2920 616e  e_list, list) an
+000249c0: 6420 6e6f 7420 616c 6c28 6973 696e 7374  d not all(isinst
+000249d0: 616e 6365 2864 2c20 6469 6374 2920 666f  ance(d, dict) fo
+000249e0: 7220 6420 696e 2064 6576 6963 655f 6c69  r d in device_li
+000249f0: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+00024a00: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00024a10: 4572 726f 7228 2257 6865 6e20 7573 696e  Error("When usin
+00024a20: 6720 6465 7669 6365 5f6c 6973 7420 746f  g device_list to
+00024a30: 2062 6174 6368 2061 6464 2064 6576 6963   batch add devic
+00024a40: 6573 2c20 7468 6579 2073 686f 756c 6420  es, they should 
+00024a50: 6265 2070 726f 7669 6465 6420 6173 2061  be provided as a
+00024a60: 206c 6973 7420 6f66 2064 6963 7473 2229   list of dicts")
+00024a70: 0a0a 2020 2020 2020 2020 2020 2020 5f6b  ..            _k
+00024a80: 6579 7320 3d20 7b0a 2020 2020 2020 2020  eys = {.        
+00024a90: 2020 2020 2020 2020 226d 6163 5f61 6464          "mac_add
+00024aa0: 7265 7373 223a 2022 6d61 6322 2c0a 2020  ress": "mac",.  
+00024ab0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00024ac0: 6572 6961 6c5f 6e75 6d22 3a20 2273 6572  erial_num": "ser
+00024ad0: 6961 6c22 2c0a 2020 2020 2020 2020 2020  ial",.          
+00024ae0: 2020 2020 2020 2270 6172 745f 6e75 6d22        "part_num"
+00024af0: 3a20 2270 6172 744e 756d 6265 7222 0a20  : "partNumber". 
+00024b00: 2020 2020 2020 2020 2020 207d 0a0a 2020             }..  
+00024b10: 2020 2020 2020 2020 2020 6a73 6f6e 5f64            json_d
+00024b20: 6174 6120 3d20 5b5d 0a20 2020 2020 2020  ata = [].       
+00024b30: 2020 2020 2066 6f72 2064 2069 6e20 6465       for d in de
+00024b40: 7669 6365 5f6c 6973 743a 0a20 2020 2020  vice_list:.     
+00024b50: 2020 2020 2020 2020 2020 206d 6163 203d             mac =
+00024b60: 2064 2e67 6574 2822 6d61 6322 2c20 642e   d.get("mac", d.
+00024b70: 6765 7428 226d 6163 5f61 6464 7265 7373  get("mac_address
+00024b80: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
+00024b90: 2020 2020 6966 206e 6f74 206d 6163 3a0a      if not mac:.
+00024ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024bb0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00024bc0: 7272 6f72 2866 224e 6f20 4d61 6320 4164  rror(f"No Mac Ad
+00024bd0: 6472 6573 7320 666f 756e 6420 666f 7220  dress found for 
+00024be0: 656e 7472 7920 7b64 7d22 290a 2020 2020  entry {d}").    
+00024bf0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00024c00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00024c10: 2020 2020 2020 6d61 6320 3d20 7574 696c        mac = util
+00024c20: 732e 4d61 6328 6d61 6329 0a20 2020 2020  s.Mac(mac).     
+00024c30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00024c40: 6620 6e6f 7420 6d61 633a 0a20 2020 2020  f not mac:.     
+00024c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024c60: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00024c70: 726f 7228 6622 4d61 6320 4164 6472 6573  ror(f"Mac Addres
+00024c80: 7320 7b6d 6163 7d20 6170 7065 6172 7320  s {mac} appears 
+00024c90: 746f 2062 6520 696e 7661 6c69 642e 2229  to be invalid.")
+00024ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024cb0: 2073 6572 6961 6c20 3d20 642e 6765 7428   serial = d.get(
+00024cc0: 2273 6572 6961 6c22 2c20 642e 6765 7428  "serial", d.get(
+00024cd0: 2273 6572 6961 6c5f 6e75 6d22 2929 0a20  "serial_num")). 
+00024ce0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00024cf0: 7468 6973 5f64 6963 7420 3d20 7b22 6d61  this_dict = {"ma
+00024d00: 6322 3a20 6d61 632e 636f 6c73 2c20 2273  c": mac.cols, "s
+00024d10: 6572 6961 6c22 3a20 7365 7269 616c 7d0a  erial": serial}.
+00024d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024d30: 7061 7274 5f6e 756d 203d 2064 2e67 6574  part_num = d.get
+00024d40: 2822 7061 7274 5f6e 756d 222c 2064 2e67  ("part_num", d.g
+00024d50: 6574 2822 7061 7274 4e75 6d62 6572 2229  et("partNumber")
+00024d60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00024d70: 2020 6966 2070 6172 745f 6e75 6d3a 0a20    if part_num:. 
+00024d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024d90: 2020 205f 7468 6973 5f64 6963 745b 2270     _this_dict["p
+00024da0: 6172 744e 756d 6265 7222 5d20 3d20 7061  artNumber"] = pa
+00024db0: 7274 5f6e 756d 0a0a 2020 2020 2020 2020  rt_num..        
+00024dc0: 2020 2020 2020 2020 6a73 6f6e 5f64 6174          json_dat
+00024dd0: 6120 2b3d 205b 5f74 6869 735f 6469 6374  a += [_this_dict
+00024de0: 5d0a 0a20 2020 2020 2020 2020 2020 2074  ]..            t
+00024df0: 6f5f 6772 6f75 7020 3d20 7b64 2e67 6574  o_group = {d.get
+00024e00: 2822 6772 6f75 7022 293a 205b 5d20 666f  ("group"): [] fo
+00024e10: 7220 6420 696e 2064 6576 6963 655f 6c69  r d in device_li
+00024e20: 7374 2069 6620 2267 726f 7570 2220 696e  st if "group" in
+00024e30: 2064 7d0a 2020 2020 2020 2020 2020 2020   d}.            
+00024e40: 666f 7220 6420 696e 2064 6576 6963 655f  for d in device_
+00024e50: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
+00024e60: 2020 2020 2020 6966 2022 6772 6f75 7022        if "group"
+00024e70: 2069 6e20 643a 0a20 2020 2020 2020 2020   in d:.         
+00024e80: 2020 2020 2020 2020 2020 2074 6f5f 6772             to_gr
+00024e90: 6f75 705b 645b 2267 726f 7570 225d 5d2e  oup[d["group"]].
+00024ea0: 6170 7065 6e64 2864 2e67 6574 2822 7365  append(d.get("se
+00024eb0: 7269 616c 5f6e 756d 222c 2064 2e67 6574  rial_num", d.get
+00024ec0: 2822 7365 7269 616c 2229 2929 0a0a 2020  ("serial")))..  
+00024ed0: 2020 2020 2020 2020 2020 2320 746f 5f73            # to_s
+00024ee0: 6974 6520 3d20 7b64 2e67 6574 2822 7369  ite = {d.get("si
+00024ef0: 7465 2229 3a20 5b5d 2066 6f72 2064 2069  te"): [] for d i
+00024f00: 6e20 6465 7669 6365 5f6c 6973 7420 6966  n device_list if
+00024f10: 2022 7369 7465 2220 696e 2064 7d0a 2020   "site" in d}.  
+00024f20: 2020 2020 2020 2020 2020 2320 666f 7220            # for 
+00024f30: 6420 696e 2064 6576 6963 655f 6c69 7374  d in device_list
+00024f40: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00024f50: 2020 2020 6966 2022 7369 7465 2220 696e      if "site" in
+00024f60: 2064 3a0a 2020 2020 2020 2020 2020 2020   d:.            
+00024f70: 2320 2020 2020 2020 2020 746f 5f73 6974  #         to_sit
+00024f80: 655b 645b 2273 6974 6522 5d5d 2e61 7070  e[d["site"]].app
+00024f90: 656e 6428 642e 6765 7428 2273 6572 6961  end(d.get("seria
+00024fa0: 6c5f 6e75 6d22 2c20 642e 6765 7428 2273  l_num", d.get("s
+00024fb0: 6572 6961 6c22 2929 290a 0a20 2020 2020  erial")))..     
+00024fc0: 2020 2020 2020 2023 2047 6174 6865 7220         # Gather 
+00024fd0: 616c 6c20 7365 7269 616c 7320 666f 7220  all serials for 
+00024fe0: 6561 6368 206c 6963 656e 7365 2063 6f6d  each license com
+00024ff0: 6269 6e61 7469 6f6e 2066 726f 6d20 6465  bination from de
+00025000: 7669 6365 5f6c 6973 740a 2020 2020 2020  vice_list.      
+00025010: 2020 2020 2020 2320 544f 444f 2074 6869        # TODO thi
+00025020: 7320 6e65 6564 7320 746f 2062 6520 7465  s needs to be te
+00025030: 7374 6564 0a20 2020 2020 2020 2020 2020  sted.           
+00025040: 205f 6c69 635f 6b77 6172 6773 203d 207b   _lic_kwargs = {
+00025050: 7d0a 2020 2020 2020 2020 2020 2020 666f  }.            fo
+00025060: 7220 6420 696e 2064 6576 6963 655f 6c69  r d in device_li
+00025070: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+00025080: 2020 2020 6966 2022 6c69 6365 6e73 6522      if "license"
+00025090: 206e 6f74 2069 6e20 643a 0a20 2020 2020   not in d:.     
+000250a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000250b0: 6f6e 7469 6e75 650a 0a20 2020 2020 2020  ontinue..       
+000250c0: 2020 2020 2020 2020 2064 5b22 6c69 6365           d["lice
+000250d0: 6e73 6522 5d20 3d20 7574 696c 732e 6c69  nse"] = utils.li
+000250e0: 7374 6966 7928 645b 226c 6963 656e 7365  stify(d["license
+000250f0: 225d 290a 2020 2020 2020 2020 2020 2020  "]).            
+00025100: 2020 2020 5f6b 6579 203d 2066 227b 645b      _key = f"{d[
+00025110: 276c 6963 656e 7365 275d 2069 6620 6c65  'license'] if le
+00025120: 6e28 645b 276c 6963 656e 7365 275d 2920  n(d['license']) 
+00025130: 3d3d 2031 2065 6c73 6520 277c 272e 6a6f  == 1 else '|'.jo
+00025140: 696e 2873 6f72 7465 6428 645b 276c 6963  in(sorted(d['lic
+00025150: 656e 7365 275d 2929 7d22 0a20 2020 2020  ense']))}".     
+00025160: 2020 2020 2020 2020 2020 205f 7365 7269             _seri
+00025170: 616c 203d 2064 2e67 6574 2822 7365 7269  al = d.get("seri
+00025180: 616c 5f6e 756d 222c 2064 2e67 6574 2822  al_num", d.get("
+00025190: 7365 7269 616c 2229 290a 2020 2020 2020  serial")).      
+000251a0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+000251b0: 205f 7365 7269 616c 3a0a 2020 2020 2020   _serial:.      
+000251c0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+000251d0: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
+000251e0: 224e 6f20 7365 7269 616c 2066 6f75 6e64  "No serial found
+000251f0: 2066 6f72 2064 6576 6963 653a 207b 647d   for device: {d}
+00025200: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
+00025210: 2020 2020 6966 205f 6b65 7920 696e 205f      if _key in _
+00025220: 6c69 635f 6b77 6172 6773 3a0a 2020 2020  lic_kwargs:.    
+00025230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025240: 5f6c 6963 5f6b 7761 7267 735b 5f6b 6579  _lic_kwargs[_key
+00025250: 5d5b 2273 6572 6961 6c73 225d 202b 3d20  ]["serials"] += 
+00025260: 7574 696c 732e 6c69 7374 6966 7928 5f73  utils.listify(_s
+00025270: 6572 6961 6c29 0a20 2020 2020 2020 2020  erial).         
+00025280: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00025290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000252a0: 205f 6c69 635f 6b77 6172 6773 5b5f 6b65   _lic_kwargs[_ke
+000252b0: 795d 203d 207b 0a20 2020 2020 2020 2020  y] = {.         
+000252c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000252d0: 7365 7276 6963 6573 223a 2075 7469 6c73  services": utils
+000252e0: 2e6c 6973 7469 6679 2864 5b22 6c69 6365  .listify(d["lice
+000252f0: 6e73 6522 5d29 2c0a 2020 2020 2020 2020  nse"]),.        
+00025300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025310: 2273 6572 6961 6c73 223a 2075 7469 6c73  "serials": utils
+00025320: 2e6c 6973 7469 6679 285f 7365 7269 616c  .listify(_serial
+00025330: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00025340: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00025350: 2020 2020 6c69 6365 6e73 655f 6b77 6172      license_kwar
+00025360: 6773 203d 206c 6973 7428 5f6c 6963 5f6b  gs = list(_lic_k
+00025370: 7761 7267 732e 7661 6c75 6573 2829 290a  wargs.values()).
+00025380: 0a20 2020 2020 2020 2020 2020 2023 206c  .            # l
+00025390: 6963 656e 7365 5f61 7267 7320 3d20 5b5b  icense_args = [[
+000253a0: 5d2c 205b 5d5d 0a20 2020 2020 2020 2020  ], []].         
+000253b0: 2020 2023 2062 795f 7365 7220 3d20 7b64     # by_ser = {d
+000253c0: 5b22 7365 7269 616c 5f6e 756d 225d 3a20  ["serial_num"]: 
+000253d0: 7574 696c 732e 6c69 7374 6966 7928 642e  utils.listify(d.
+000253e0: 6765 7428 226c 6963 656e 7365 2229 2920  get("license")) 
+000253f0: 666f 7220 6420 696e 2064 6576 6963 655f  for d in device_
+00025400: 6c69 7374 2069 6620 642e 6765 7428 226c  list if d.get("l
+00025410: 6963 656e 7365 2229 7d0a 2020 2020 2020  icense")}.      
+00025420: 2020 2020 2020 2320 544f 444f 206d 6f73        # TODO mos
+00025430: 7420 6566 6669 6369 656e 7420 7061 6972  t efficient pair
+00025440: 696e 6720 6f66 2070 6f73 7369 626c 6520  ing of possible 
+00025450: 6c69 632f 6465 7620 666f 7220 6665 7765  lic/dev for fewe
+00025460: 7374 2063 616c 6c0a 2020 2020 2020 2020  st call.        
+00025470: 2020 2020 2320 544f 444f 206c 6963 656e      # TODO licen
+00025480: 7365 2076 6961 206c 6973 7420 6e6f 7420  se via list not 
+00025490: 696d 706c 656d 656e 7465 6420 7965 742e  implemented yet.
+000254a0: 0a0a 2020 2020 2020 2020 656c 7365 3a0a  ..        else:.
+000254b0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000254c0: 6520 5661 6c75 6545 7272 6f72 2822 6d61  e ValueError("ma
+000254d0: 635f 6164 6472 6573 7320 616e 6420 7365  c_address and se
+000254e0: 7269 616c 5f6e 756d 206f 7220 6465 7669  rial_num or devi
+000254f0: 6365 5f6c 6973 7420 6973 2072 6571 7569  ce_list is requi
+00025500: 7265 6422 290a 0a20 2020 2020 2020 2023  red")..        #
+00025510: 2050 6572 666f 726d 2041 5049 2063 616c   Perform API cal
+00025520: 6c28 7329 2074 6f20 4365 6e74 7261 6c20  l(s) to Central 
+00025530: 4150 4920 4757 0a20 2020 2020 2020 2023  API GW.        #
+00025540: 2054 4f44 4f20 6272 6561 6b20 6f75 7420   TODO break out 
+00025550: 7468 6520 6164 6420 6465 7669 6365 2063  the add device c
+00025560: 616c 6c20 696e 746f 2069 7427 7320 6f77  all into it's ow
+00025570: 6e20 6d65 7468 6f64 2e0a 2020 2020 2020  n method..      
+00025580: 2020 6966 2074 6f5f 6772 6f75 7020 6f72    if to_group or
+00025590: 206c 6963 656e 7365 5f6b 7761 7267 733a   license_kwargs:
+000255a0: 0a20 2020 2020 2020 2020 2020 2023 2041  .            # A
+000255b0: 6464 2064 6576 6963 6573 2074 6f20 6365  dd devices to ce
+000255c0: 6e74 7261 6c2e 2020 3120 4150 4920 6361  ntral.  1 API ca
+000255d0: 6c6c 2066 6f72 2031 206f 7220 6d61 6e79  ll for 1 or many
+000255e0: 2064 6576 6963 6573 2e0a 2020 2020 2020   devices..      
+000255f0: 2020 2020 2020 6272 203d 2073 656c 662e        br = self.
+00025600: 4261 7463 6852 6571 7565 7374 0a20 2020  BatchRequest.   
+00025610: 2020 2020 2020 2020 2072 6571 7320 3d20           reqs = 
+00025620: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00025630: 2020 6272 2873 656c 662e 706f 7374 2c20    br(self.post, 
+00025640: 7572 6c2c 206a 736f 6e5f 6461 7461 3d6a  url, json_data=j
+00025650: 736f 6e5f 6461 7461 292c 0a20 2020 2020  son_data),.     
+00025660: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00025670: 2020 2020 2023 2041 7373 6967 6e20 6465       # Assign de
+00025680: 7669 6365 7320 746f 2070 7265 2d70 726f  vices to pre-pro
+00025690: 7669 7369 6f6e 6564 2067 726f 7570 2e20  visioned group. 
+000256a0: 2031 2041 5049 2063 616c 6c20 7065 7220   1 API call per 
+000256b0: 6772 6f75 700a 2020 2020 2020 2020 2020  group.          
+000256c0: 2020 2320 544f 444f 2074 6573 7420 7468    # TODO test th
+000256d0: 6174 2074 6869 7320 6973 2031 2041 5049  at this is 1 API
+000256e0: 2063 616c 6c20 7065 7220 6772 6f75 702e   call per group.
+000256f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00025700: 746f 5f67 726f 7570 3a0a 2020 2020 2020  to_group:.      
+00025710: 2020 2020 2020 2020 2020 6772 6f75 705f            group_
+00025720: 7265 7173 203d 205b 6272 2873 656c 662e  reqs = [br(self.
+00025730: 7072 6570 726f 7669 7369 6f6e 5f64 6576  preprovision_dev
+00025740: 6963 655f 746f 5f67 726f 7570 2c20 2867  ice_to_group, (g
+00025750: 2c20 6465 7673 2929 2066 6f72 2067 2c20  , devs)) for g, 
+00025760: 6465 7673 2069 6e20 746f 5f67 726f 7570  devs in to_group
+00025770: 2e69 7465 6d73 2829 5d0a 2020 2020 2020  .items()].      
+00025780: 2020 2020 2020 2020 2020 7265 7173 203d            reqs =
+00025790: 205b 2a72 6571 732c 202a 6772 6f75 705f   [*reqs, *group_
+000257a0: 7265 7173 5d0a 0a20 2020 2020 2020 2020  reqs]..         
+000257b0: 2020 2023 2054 4f44 4f20 596f 7520 6361     # TODO You ca
+000257c0: 6e20 6164 6420 7468 6520 6465 7669 6365  n add the device
+000257d0: 2074 6f20 6120 7369 7465 2061 6674 6572   to a site after
+000257e0: 2069 7427 7320 6265 656e 2070 7265 2d61   it's been pre-a
+000257f0: 7373 6967 6e65 640a 2020 2020 2020 2020  ssigned.        
+00025800: 2020 2020 2320 6966 2074 6f5f 7369 7465      # if to_site
+00025810: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00025820: 2020 2020 7369 7465 5f72 6571 7320 3d20      site_reqs = 
+00025830: 5b62 7228 7365 6c66 2e6d 6f76 655f 6465  [br(self.move_de
+00025840: 7669 6365 735f 746f 5f73 6974 652c 2028  vices_to_site, (
+00025850: 732c 2064 6576 732c 2022 6777 2229 2920  s, devs, "gw")) 
+00025860: 666f 7220 732c 2064 6576 7320 696e 2074  for s, devs in t
+00025870: 6f5f 7369 7465 2e69 7465 6d73 2829 5d0a  o_site.items()].
+00025880: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+00025890: 2020 7265 7173 203d 205b 2a72 6571 732c    reqs = [*reqs,
+000258a0: 202a 7369 7465 5f72 6571 735d 0a0a 2020   *site_reqs]..  
+000258b0: 2020 2020 2020 2020 2020 2320 4173 7369            # Assi
+000258c0: 676e 206c 6963 656e 7365 2074 6f20 6465  gn license to de
+000258d0: 7669 6365 732e 2020 3120 4150 4920 6361  vices.  1 API ca
+000258e0: 6c6c 2066 6f72 2061 6c6c 2064 6576 6963  ll for all devic
+000258f0: 6573 2077 6974 6820 7361 6d65 2063 6f6d  es with same com
+00025900: 6269 6e61 7469 6f6e 206f 6620 6c69 6365  bination of lice
+00025910: 6e73 6573 0a20 2020 2020 2020 2020 2020  nses.           
+00025920: 2069 6620 6c69 6365 6e73 655f 6b77 6172   if license_kwar
+00025930: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00025940: 2020 2020 6c69 635f 7265 7173 203d 205b      lic_reqs = [
+00025950: 6272 2873 656c 662e 6173 7369 676e 5f6c  br(self.assign_l
+00025960: 6963 656e 7365 732c 202a 2a6b 7761 7267  icenses, **kwarg
+00025970: 7329 2066 6f72 206b 7761 7267 7320 696e  s) for kwargs in
+00025980: 206c 6963 656e 7365 5f6b 7761 7267 735d   license_kwargs]
+00025990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000259a0: 2072 6571 7320 3d20 5b2a 7265 7173 2c20   reqs = [*reqs, 
+000259b0: 2a6c 6963 5f72 6571 735d 0a0a 2020 2020  *lic_reqs]..    
+000259c0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+000259d0: 7761 6974 2073 656c 662e 5f62 6174 6368  wait self._batch
+000259e0: 5f72 6571 7565 7374 2872 6571 732c 2063  _request(reqs, c
+000259f0: 6f6e 7469 6e75 655f 6f6e 5f66 6169 6c3d  ontinue_on_fail=
+00025a00: 5472 7565 290a 2020 2020 2020 2020 2320  True).        # 
+00025a10: 656c 6966 2074 6f5f 7369 7465 3a0a 2020  elif to_site:.  
+00025a20: 2020 2020 2020 2320 2020 2020 7261 6973        #     rais
+00025a30: 6520 5661 6c75 6545 7272 6f72 2822 5369  e ValueError("Si
+00025a40: 7465 2063 616e 206f 6e6c 7920 6265 2070  te can only be p
+00025a50: 7265 2d61 7373 6967 6e65 6420 6966 2064  re-assigned if d
+00025a60: 6576 6963 6520 6973 2070 7265 2d70 726f  evice is pre-pro
+00025a70: 7669 7369 6f6e 6564 2074 6f20 6120 6772  visioned to a gr
+00025a80: 6f75 7022 290a 2020 2020 2020 2020 656c  oup").        el
+00025a90: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00025aa0: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+00025ab0: 662e 706f 7374 2875 726c 2c20 6a73 6f6e  f.post(url, json
+00025ac0: 5f64 6174 613d 6a73 6f6e 5f64 6174 6129  _data=json_data)
+00025ad0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00025ae0: 636f 705f 6465 6c65 7465 5f64 6576 6963  cop_delete_devic
+00025af0: 655f 6672 6f6d 5f69 6e76 656e 746f 7279  e_from_inventory
+00025b00: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00025b10: 2020 2020 2020 2020 6465 7669 6365 733a          devices:
+00025b20: 204c 6973 745b 7374 725d 203d 204e 6f6e   List[str] = Non
+00025b30: 652c 0a20 2020 2029 202d 3e20 5265 7370  e,.    ) -> Resp
+00025b40: 6f6e 7365 3a0a 2020 2020 2020 2020 2222  onse:.        ""
+00025b50: 2244 656c 6574 6520 6465 7669 6365 7320  "Delete devices 
+00025b60: 7573 696e 6720 5365 7269 616c 206e 756d  using Serial num
+00025b70: 6265 722e 2020 4f6e 6c79 2061 7070 6c69  ber.  Only appli
+00025b80: 6573 2074 6f20 436f 5020 6465 706c 6f79  es to CoP deploy
+00025b90: 6d65 6e74 732e 0a0a 2020 2020 2020 2020  ments...        
+00025ba0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00025bb0: 2020 6465 7669 6365 7320 286c 6973 742c    devices (list,
+00025bc0: 206f 7074 696f 6e61 6c29 3a20 4c69 7374   optional): List
+00025bd0: 206f 6620 6465 7669 6365 7320 746f 2062   of devices to b
+00025be0: 6520 6465 6c65 7465 6420 6672 6f6d 0a20  e deleted from. 
+00025bf0: 2020 2020 2020 2020 2020 2020 2020 2047                 G
+00025c00: 7265 656e 4c61 6b65 2069 6e76 656e 746f  reenLake invento
+00025c10: 7279 2e20 204f 6e6c 7920 6170 706c 6965  ry.  Only applie
+00025c20: 7320 746f 2043 6f50 0a0a 2020 2020 2020  s to CoP..      
+00025c30: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00025c40: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
+00025c50: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
+00025c60: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
+00025c70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00025c80: 7572 6c20 3d20 222f 706c 6174 666f 726d  url = "/platform
+00025c90: 2f64 6576 6963 655f 696e 7665 6e74 6f72  /device_inventor
+00025ca0: 792f 7631 2f64 6576 6963 6573 220a 0a20  y/v1/devices".. 
+00025cb0: 2020 2020 2020 2064 6576 6963 6573 203d         devices =
+00025cc0: 205b 7b22 7365 7269 616c 223a 2073 6572   [{"serial": ser
+00025cd0: 6961 6c7d 2066 6f72 2073 6572 6961 6c20  ial} for serial 
+00025ce0: 696e 2064 6576 6963 6573 5d0a 0a20 2020  in devices]..   
+00025cf0: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
+00025d00: 7420 7365 6c66 2e64 656c 6574 6528 7572  t self.delete(ur
+00025d10: 6c2c 206a 736f 6e5f 6461 7461 3d64 6576  l, json_data=dev
+00025d20: 6963 6573 290a 0a20 2020 2023 2054 4f44  ices)..    # TOD
+00025d30: 4f20 6d61 7962 6520 6865 6c70 6572 206d  O maybe helper m
+00025d40: 6574 686f 6420 746f 2064 656c 6574 655f  ethod to delete_
+00025d50: 6465 7669 6365 2074 6861 7420 6361 6c6c  device that call
+00025d60: 7320 7468 6573 650a 2020 2020 6173 796e  s these.    asyn
+00025d70: 6320 6465 6620 6465 6c65 7465 5f67 6174  c def delete_gat
+00025d80: 6577 6179 280a 2020 2020 2020 2020 7365  eway(.        se
+00025d90: 6c66 2c0a 2020 2020 2020 2020 7365 7269  lf,.        seri
+00025da0: 616c 3a20 7374 722c 0a20 2020 2029 202d  al: str,.    ) -
+00025db0: 3e20 5265 7370 6f6e 7365 3a0a 2020 2020  > Response:.    
+00025dc0: 2020 2020 2222 2244 656c 6574 6520 4761      """Delete Ga
+00025dd0: 7465 7761 792e 0a0a 2020 2020 2020 2020  teway...        
+00025de0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00025df0: 2020 7365 7269 616c 2028 7374 7229 3a20    serial (str): 
+00025e00: 5365 7269 616c 204e 756d 6265 7220 6f66  Serial Number of
+00025e10: 2047 6174 6577 6179 2074 6f20 6265 2064   Gateway to be d
+00025e20: 656c 6574 6564 0a0a 2020 2020 2020 2020  eleted..        
+00025e30: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00025e40: 2020 2020 2052 6573 706f 6e73 653a 2043       Response: C
+00025e50: 656e 7472 616c 4150 4920 5265 7370 6f6e  entralAPI Respon
+00025e60: 7365 206f 626a 6563 740a 2020 2020 2020  se object.      
+00025e70: 2020 2222 220a 2020 2020 2020 2020 7572    """.        ur
+00025e80: 6c20 3d20 6622 2f6d 6f6e 6974 6f72 696e  l = f"/monitorin
+00025e90: 672f 7632 2f6d 6f62 696c 6974 795f 636f  g/v2/mobility_co
+00025ea0: 6e74 726f 6c6c 6572 732f 7b73 6572 6961  ntrollers/{seria
+00025eb0: 6c7d 2220 6966 2063 6f6e 6669 672e 6973  l}" if config.is
+00025ec0: 5f63 6f70 2065 6c73 6520 6622 2f6d 6f6e  _cop else f"/mon
+00025ed0: 6974 6f72 696e 672f 7631 2f67 6174 6577  itoring/v1/gatew
+00025ee0: 6179 732f 7b73 6572 6961 6c7d 220a 0a20  ays/{serial}".. 
+00025ef0: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
+00025f00: 6169 7420 7365 6c66 2e64 656c 6574 6528  ait self.delete(
+00025f10: 7572 6c29 0a0a 2020 2020 6173 796e 6320  url)..    async 
+00025f20: 6465 6620 6465 6c65 7465 5f73 7769 7463  def delete_switc
+00025f30: 6828 0a20 2020 2020 2020 2073 656c 662c  h(.        self,
+00025f40: 0a20 2020 2020 2020 2073 6572 6961 6c3a  .        serial:
+00025f50: 2073 7472 2c0a 2020 2020 2920 2d3e 2052   str,.    ) -> R
+00025f60: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
+00025f70: 2022 2222 4465 6c65 7465 2053 7769 7463   """Delete Switc
+00025f80: 682e 0a0a 2020 2020 2020 2020 4172 6773  h...        Args
+00025f90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00025fa0: 7269 616c 2028 7374 7229 3a20 5365 7269  rial (str): Seri
+00025fb0: 616c 206e 756d 6265 7220 6f66 2073 7769  al number of swi
+00025fc0: 7463 6820 746f 2062 6520 6465 6c65 7465  tch to be delete
+00025fd0: 640a 0a20 2020 2020 2020 2052 6574 7572  d..        Retur
+00025fe0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00025ff0: 5265 7370 6f6e 7365 3a20 4365 6e74 7261  Response: Centra
+00026000: 6c41 5049 2052 6573 706f 6e73 6520 6f62  lAPI Response ob
+00026010: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
+00026020: 0a20 2020 2020 2020 2075 726c 203d 2066  .        url = f
+00026030: 222f 6d6f 6e69 746f 7269 6e67 2f76 312f  "/monitoring/v1/
+00026040: 7377 6974 6368 6573 2f7b 7365 7269 616c  switches/{serial
+00026050: 7d22 0a0a 2020 2020 2020 2020 7265 7475  }"..        retu
+00026060: 726e 2061 7761 6974 2073 656c 662e 6465  rn await self.de
+00026070: 6c65 7465 2875 726c 290a 0a20 2020 2061  lete(url)..    a
+00026080: 7379 6e63 2064 6566 2064 656c 6574 655f  sync def delete_
+00026090: 7374 6163 6b28 0a20 2020 2020 2020 2073  stack(.        s
+000260a0: 656c 662c 0a20 2020 2020 2020 2073 7461  elf,.        sta
+000260b0: 636b 5f69 643a 2073 7472 2c0a 2020 2020  ck_id: str,.    
+000260c0: 2920 2d3e 2052 6573 706f 6e73 653a 0a20  ) -> Response:. 
+000260d0: 2020 2020 2020 2022 2222 4465 6c65 7465         """Delete
+000260e0: 2053 7769 7463 6820 5374 6163 6b2e 0a0a   Switch Stack...
+000260f0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00026100: 2020 2020 2020 2020 2020 7374 6163 6b5f            stack_
+00026110: 6964 2028 7374 7229 3a20 4669 6c74 6572  id (str): Filter
+00026120: 2062 7920 5377 6974 6368 2073 7461 636b   by Switch stack
+00026130: 5f69 640a 0a20 2020 2020 2020 2052 6574  _id..        Ret
+00026140: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00026150: 2020 5265 7370 6f6e 7365 3a20 4365 6e74    Response: Cent
+00026160: 7261 6c41 5049 2052 6573 706f 6e73 6520  ralAPI Response 
+00026170: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
+00026180: 2222 0a20 2020 2020 2020 2075 726c 203d  "".        url =
+00026190: 2066 222f 6d6f 6e69 746f 7269 6e67 2f76   f"/monitoring/v
+000261a0: 312f 7377 6974 6368 5f73 7461 636b 732f  1/switch_stacks/
+000261b0: 7b73 7461 636b 5f69 647d 220a 0a20 2020  {stack_id}"..   
+000261c0: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
+000261d0: 7420 7365 6c66 2e64 656c 6574 6528 7572  t self.delete(ur
+000261e0: 6c29 0a0a 2020 2020 6173 796e 6320 6465  l)..    async de
+000261f0: 6620 6465 6c65 7465 5f61 7028 0a20 2020  f delete_ap(.   
+00026200: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00026210: 2020 2073 6572 6961 6c3a 2073 7472 2c0a     serial: str,.
+00026220: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
+00026230: 653a 0a20 2020 2020 2020 2022 2222 4465  e:.        """De
+00026240: 6c65 7465 2041 502e 0a0a 2020 2020 2020  lete AP...      
+00026250: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00026260: 2020 2020 7365 7269 616c 2028 7374 7229      serial (str)
+00026270: 3a20 5365 7269 616c 204e 756d 6265 7220  : Serial Number 
+00026280: 6f66 2041 5020 746f 2062 6520 6465 6c65  of AP to be dele
+00026290: 7465 640a 0a20 2020 2020 2020 2052 6574  ted..        Ret
+000262a0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+000262b0: 2020 5265 7370 6f6e 7365 3a20 4365 6e74    Response: Cent
+000262c0: 7261 6c41 5049 2052 6573 706f 6e73 6520  ralAPI Response 
+000262d0: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
+000262e0: 2222 0a20 2020 2020 2020 2075 726c 203d  "".        url =
+000262f0: 2066 222f 6d6f 6e69 746f 7269 6e67 2f76   f"/monitoring/v
+00026300: 312f 6170 732f 7b73 6572 6961 6c7d 220a  1/aps/{serial}".
+00026310: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00026320: 6177 6169 7420 7365 6c66 2e64 656c 6574  await self.delet
+00026330: 6528 7572 6c29 0a0a 2020 2020 2320 544f  e(url)..    # TO
+00026340: 444f 206d 6179 2072 656d 6f76 6520 7468  DO may remove th
+00026350: 6973 2077 6f75 6c64 2073 686f 7720 7468  is would show th
+00026360: 6520 6465 7669 6365 2069 6e20 7468 6520  e device in the 
+00026370: 6772 6f75 702c 2062 7574 2064 6964 6e27  group, but didn'
+00026380: 7420 6265 6861 7665 2061 7320 6578 7065  t behave as expe
+00026390: 6374 6564 2028 6465 7669 6365 2077 6173  cted (device was
+000263a0: 206e 6f74 2069 6e20 6465 7669 6365 206c   not in device l
+000263b0: 6973 7429 0a20 2020 2061 7379 6e63 2064  ist).    async d
+000263c0: 6566 2061 7373 6967 6e5f 6465 7669 6365  ef assign_device
+000263d0: 735f 746f 5f67 726f 7570 2873 656c 662c  s_to_group(self,
+000263e0: 2020 6772 6f75 703a 2073 7472 2c20 7365    group: str, se
+000263f0: 7269 616c 5f6e 756d 733a 2055 6e69 6f6e  rial_nums: Union
+00026400: 5b4c 6973 745b 7374 725d 2c20 7374 725d  [List[str], str]
+00026410: 2920 2d3e 2052 6573 706f 6e73 653a 0a20  ) -> Response:. 
+00026420: 2020 2020 2020 2022 2222 4173 7369 676e         """Assign
+00026430: 2064 6576 6963 6573 2074 6f20 7072 652d   devices to pre-
+00026440: 7072 6f76 6973 696f 6e65 6420 6772 6f75  provisioned grou
+00026450: 702e 0a0a 2020 2020 2020 2020 2f2f 2055  p...        // U
+00026460: 7365 6420 696e 6469 7265 6374 6c79 2062  sed indirectly b
+00026470: 7920 6164 6420 6465 7669 6365 2028 7768  y add device (wh
+00026480: 656e 2067 726f 7570 206f 7074 696f 6e20  en group option 
+00026490: 7072 6f76 6964 6564 2920 2f2f 0a0a 2020  provided) //..  
+000264a0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+000264b0: 2020 2020 2020 2020 6772 6f75 7020 2873          group (s
+000264c0: 7472 293a 2047 726f 7570 206e 616d 650a  tr): Group name.
+000264d0: 2020 2020 2020 2020 2020 2020 7365 7269              seri
+000264e0: 616c 7320 284c 6973 745b 7374 725d 7c73  als (List[str]|s
+000264f0: 7472 293a 2044 6576 6963 6520 7365 7269  tr): Device seri
+00026500: 616c 206e 756d 6265 7220 6f72 206c 6973  al number or lis
+00026510: 7420 6f66 2064 6576 6963 6520 7365 7269  t of device seri
+00026520: 616c 206e 756d 6265 7273 2e0a 0a20 2020  al numbers...   
+00026530: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00026540: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
+00026550: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
+00026560: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
+00026570: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00026580: 2020 2075 726c 203d 2022 2f64 6576 6963     url = "/devic
+00026590: 655f 6d61 6e61 6765 6d65 6e74 2f76 312f  e_management/v1/
+000265a0: 6772 6f75 702f 6173 7369 676e 220a 2020  group/assign".  
+000265b0: 2020 2020 2020 7365 7269 616c 5f6e 756d        serial_num
+000265c0: 7320 3d20 7574 696c 732e 6c69 7374 6966  s = utils.listif
+000265d0: 7928 7365 7269 616c 5f6e 756d 7329 0a0a  y(serial_nums)..
+000265e0: 2020 2020 2020 2020 6a73 6f6e 5f64 6174          json_dat
+000265f0: 6120 3d20 7b0a 2020 2020 2020 2020 2020  a = {.          
+00026600: 2020 2773 6572 6961 6c73 273a 2073 6572    'serials': ser
+00026610: 6961 6c5f 6e75 6d73 2c0a 2020 2020 2020  ial_nums,.      
+00026620: 2020 2020 2020 2767 726f 7570 273a 2067        'group': g
+00026630: 726f 7570 0a20 2020 2020 2020 207d 0a0a  roup.        }..
+00026640: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00026650: 7761 6974 2073 656c 662e 706f 7374 2875  wait self.post(u
+00026660: 726c 2c20 6a73 6f6e 5f64 6174 613d 6a73  rl, json_data=js
+00026670: 6f6e 5f64 6174 6129 0a0a 2020 2020 6173  on_data)..    as
+00026680: 796e 6320 6465 6620 7072 6570 726f 7669  ync def preprovi
+00026690: 7369 6f6e 5f64 6576 6963 655f 746f 5f67  sion_device_to_g
+000266a0: 726f 7570 280a 2020 2020 2020 2020 7365  roup(.        se
+000266b0: 6c66 2c0a 2020 2020 2020 2020 6772 6f75  lf,.        grou
+000266c0: 705f 6e61 6d65 3a20 7374 722c 0a20 2020  p_name: str,.   
+000266d0: 2020 2020 2073 6572 6961 6c5f 6e75 6d73       serial_nums
+000266e0: 3a20 4c69 7374 5b73 7472 5d20 7c20 7374  : List[str] | st
+000266f0: 722c 0a20 2020 2020 2020 2074 656e 616e  r,.        tenan
+00026700: 745f 6964 3a20 7374 7220 3d20 4e6f 6e65  t_id: str = None
+00026710: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
+00026720: 6e73 653a 0a20 2020 2020 2020 2022 2222  nse:.        """
+00026730: 5072 6520 5072 6f76 6973 696f 6e20 6120  Pre Provision a 
+00026740: 6772 6f75 7020 746f 2074 6865 2064 6576  group to the dev
+00026750: 6963 652e 0a0a 2020 2020 2020 2020 4172  ice...        Ar
+00026760: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00026770: 6465 7669 6365 5f69 6420 284c 6973 745b  device_id (List[
+00026780: 7374 725d 293a 2064 6576 6963 655f 6964  str]): device_id
+00026790: 0a20 2020 2020 2020 2020 2020 2067 726f  .            gro
+000267a0: 7570 5f6e 616d 6520 2873 7472 293a 2047  up_name (str): G
+000267b0: 726f 7570 206e 616d 650a 2020 2020 2020  roup name.      
+000267c0: 2020 2020 2020 7465 6e61 6e74 5f69 6420        tenant_id 
+000267d0: 2873 7472 293a 2054 656e 616e 7420 6964  (str): Tenant id
+000267e0: 2c20 286f 6e6c 7920 6170 706c 6963 6162  , (only applicab
+000267f0: 6c65 2077 6974 6820 4d53 5020 6d6f 6465  le with MSP mode
+00026800: 290a 0a20 2020 2020 2020 2052 6574 7572  )..        Retur
+00026810: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00026820: 5265 7370 6f6e 7365 3a20 4365 6e74 7261  Response: Centra
+00026830: 6c41 5049 2052 6573 706f 6e73 6520 6f62  lAPI Response ob
+00026840: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
+00026850: 0a20 2020 2020 2020 2075 726c 203d 2022  .        url = "
+00026860: 2f63 6f6e 6669 6775 7261 7469 6f6e 2f76  /configuration/v
+00026870: 312f 7072 6561 7373 6967 6e22 0a0a 2020  1/preassign"..  
+00026880: 2020 2020 2020 6a73 6f6e 5f64 6174 6120        json_data 
+00026890: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+000268a0: 2764 6576 6963 655f 6964 273a 2075 7469  'device_id': uti
+000268b0: 6c73 2e6c 6973 7469 6679 2873 6572 6961  ls.listify(seria
+000268c0: 6c5f 6e75 6d73 292c 0a20 2020 2020 2020  l_nums),.       
+000268d0: 2020 2020 2027 6772 6f75 705f 6e61 6d65       'group_name
+000268e0: 273a 2067 726f 7570 5f6e 616d 652c 0a20  ': group_name,. 
+000268f0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+00026900: 2020 6966 2074 656e 616e 745f 6964 2069    if tenant_id i
+00026910: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00026920: 2020 2020 2020 2020 6a73 6f6e 5f64 6174          json_dat
+00026930: 615b 2274 656e 616e 745f 6964 225d 203d  a["tenant_id"] =
+00026940: 2073 7472 2874 656e 616e 745f 6964 290a   str(tenant_id).
+00026950: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00026960: 6177 6169 7420 7365 6c66 2e70 6f73 7428  await self.post(
+00026970: 7572 6c2c 206a 736f 6e5f 6461 7461 3d6a  url, json_data=j
+00026980: 736f 6e5f 6461 7461 290a 0a20 2020 2023  son_data)..    #
+00026990: 2054 4f44 4f20 7665 7269 6679 2074 7970   TODO verify typ
+000269a0: 652d 6869 6e74 2066 6f72 2064 6576 6963  e-hint for devic
+000269b0: 655f 6c69 7374 2069 7320 7468 6520 7269  e_list is the ri
+000269c0: 6768 7420 7761 7920 746f 2064 6f20 7468  ght way to do th
+000269d0: 6174 2e0a 2020 2020 6173 796e 6320 6465  at..    async de
+000269e0: 6620 7665 7269 6679 5f64 6576 6963 655f  f verify_device_
+000269f0: 6164 6469 7469 6f6e 280a 2020 2020 2020  addition(.      
+00026a00: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00026a10: 7365 7269 616c 5f6e 756d 3a20 7374 7220  serial_num: str 
+00026a20: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00026a30: 6d61 635f 6164 6472 6573 733a 2073 7472  mac_address: str
+00026a40: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00026a50: 2064 6576 6963 655f 6c69 7374 3a20 4c69   device_list: Li
+00026a60: 7374 5b44 6963 745b 4c69 7465 7261 6c5b  st[Dict[Literal[
+00026a70: 226d 6163 5f61 6464 7265 7373 222c 2022  "mac_address", "
+00026a80: 7365 7269 616c 5f6e 756d 225d 2c20 7374  serial_num"], st
+00026a90: 725d 5d20 3d20 5b5d 0a20 2020 2029 202d  r]] = [].    ) -
+00026aa0: 3e20 5265 7370 6f6e 7365 3a0a 2020 2020  > Response:.    
+00026ab0: 2020 2020 2222 2256 6572 6966 7920 4465      """Verify De
+00026ac0: 7669 6365 2041 6464 6974 696f 6e0a 0a20  vice Addition.. 
+00026ad0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00026ae0: 2020 2020 2020 2020 2073 6572 6961 6c5f           serial_
+00026af0: 6e75 6d20 2873 7472 2c20 6f70 7469 6f6e  num (str, option
+00026b00: 616c 293a 2053 6572 6961 6c20 4e75 6d62  al): Serial Numb
+00026b10: 6572 206f 6620 6465 7669 6365 2074 6f20  er of device to 
+00026b20: 7665 7269 6679 2e20 4465 6661 756c 7473  verify. Defaults
+00026b30: 2074 6f20 4e6f 6e65 2e0a 2020 2020 2020   to None..      
+00026b40: 2020 2020 2020 6d61 635f 6164 6472 6573        mac_addres
+00026b50: 7320 2873 7472 2c20 6f70 7469 6f6e 616c  s (str, optional
+00026b60: 293a 204d 6163 2041 6464 7265 7373 206f  ): Mac Address o
+00026b70: 6620 6465 7669 6365 2074 6f20 7665 7269  f device to veri
+00026b80: 6679 2e20 4465 6661 756c 7473 2074 6f20  fy. Defaults to 
+00026b90: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
+00026ba0: 2020 6465 7669 6365 5f6c 6973 7420 284c    device_list (L
+00026bb0: 6973 745b 4469 6374 5b4c 6974 6572 616c  ist[Dict[Literal
+00026bc0: 5b2c 206f 7074 696f 6e61 6c29 3a20 6465  [, optional): de
+00026bd0: 7669 6365 5f6c 6973 7420 6c69 7374 206f  vice_list list o
+00026be0: 6620 6469 6374 7320 7769 7468 0a20 2020  f dicts with.   
+00026bf0: 2020 2020 2020 2020 2020 2020 2022 7365               "se
+00026c00: 7269 616c 5f6e 756d 2220 616e 6420 226d  rial_num" and "m
+00026c10: 6163 5f61 6464 7265 7373 2220 666f 7220  ac_address" for 
+00026c20: 6561 6368 2064 6576 6963 6520 746f 2076  each device to v
+00026c30: 6572 6966 792e 2044 6566 6175 6c74 7320  erify. Defaults 
+00026c40: 746f 204e 6f6e 652e 0a0a 2020 2020 2020  to None...      
+00026c50: 2020 4d75 7374 2070 726f 7669 6465 2073    Must provide s
+00026c60: 6572 6961 6c5f 6e75 6d20 616e 6420 6d61  erial_num and ma
+00026c70: 635f 6164 6472 6573 7320 666f 7220 6561  c_address for ea
+00026c80: 6368 2064 6576 6963 6520 6569 7468 6572  ch device either
+00026c90: 2076 6961 206b 6579 776f 7264 2061 7267   via keyword arg
+00026ca0: 756d 656e 7420 6f72 206c 6973 742e 0a0a  ument or list...
+00026cb0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00026cc0: 0a20 2020 2020 2020 2020 2020 2052 6573  .            Res
+00026cd0: 706f 6e73 653a 2043 656e 7472 616c 4150  ponse: CentralAP
+00026ce0: 4920 5265 7370 6f6e 7365 206f 626a 6563  I Response objec
+00026cf0: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
+00026d00: 2020 2020 2020 7572 6c20 3d20 222f 706c        url = "/pl
+00026d10: 6174 666f 726d 2f64 6576 6963 655f 696e  atform/device_in
+00026d20: 7665 6e74 6f72 792f 7631 2f64 6576 6963  ventory/v1/devic
+00026d30: 6573 2f76 6572 6966 7922 0a20 2020 2020  es/verify".     
+00026d40: 2020 2069 6620 7365 7269 616c 5f6e 756d     if serial_num
+00026d50: 2061 6e64 206d 6163 5f61 6464 7265 7373   and mac_address
+00026d60: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
+00026d70: 7669 6365 5f6c 6973 7420 2b3d 207b 0a20  vice_list += {. 
+00026d80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00026d90: 7365 7269 616c 5f6e 756d 223a 2073 6572  serial_num": ser
+00026da0: 6961 6c5f 6e75 6d2c 0a20 2020 2020 2020  ial_num,.       
+00026db0: 2020 2020 2020 2020 2022 6d61 635f 6164           "mac_ad
+00026dc0: 6472 6573 7322 3a20 6d61 635f 6164 6472  dress": mac_addr
+00026dd0: 6573 732c 0a20 2020 2020 2020 2020 2020  ess,.           
+00026de0: 207d 0a0a 2020 2020 2020 2020 6966 206e   }..        if n
+00026df0: 6f74 2064 6576 6963 655f 6c69 7374 3a0a  ot device_list:.
+00026e00: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00026e10: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+00026e20: 2020 2020 2020 2020 2020 2020 2020 2249                "I
+00026e30: 6e76 616c 6964 2070 6172 616d 6574 6572  nvalid parameter
+00026e40: 7320 6578 7065 6374 696e 6720 7365 7269  s expecting seri
+00026e50: 616c 5f6e 756d 2061 6e64 206d 6163 5f61  al_num and mac_a
+00026e60: 6464 7265 7373 2066 6f72 2065 6163 6820  ddress for each 
+00026e70: 6465 7669 6365 2022 0a20 2020 2020 2020  device ".       
+00026e80: 2020 2020 2020 2020 2022 6569 7468 6572           "either
+00026e90: 2076 6961 206b 6579 776f 7264 2061 7267   via keyword arg
+00026ea0: 756d 656e 7420 6f72 204c 6973 745b 6469  ument or List[di
+00026eb0: 6374 5d2e 220a 2020 2020 2020 2020 2020  ct].".          
+00026ec0: 2020 290a 0a20 2020 2020 2020 2072 6574    )..        ret
+00026ed0: 7572 6e20 6177 6169 7420 7365 6c66 2e70  urn await self.p
+00026ee0: 6f73 7428 7572 6c2c 206a 736f 6e5f 6461  ost(url, json_da
+00026ef0: 7461 3d64 6576 6963 655f 6c69 7374 290a  ta=device_list).
+00026f00: 0a20 2020 2061 7379 6e63 2064 6566 2075  .    async def u
+00026f10: 706c 6f61 645f 6365 7274 6966 6963 6174  pload_certificat
+00026f20: 6528 0a20 2020 2020 2020 2073 656c 662c  e(.        self,
+00026f30: 0a20 2020 2020 2020 2070 6173 7370 6872  .        passphr
+00026f40: 6173 653a 2073 7472 203d 2022 222c 0a20  ase: str = "",. 
+00026f50: 2020 2020 2020 2063 6572 745f 6669 6c65         cert_file
+00026f60: 3a20 556e 696f 6e5b 7374 722c 2050 6174  : Union[str, Pat
+00026f70: 685d 203d 204e 6f6e 652c 0a20 2020 2020  h] = None,.     
+00026f80: 2020 2063 6572 745f 6e61 6d65 3a20 7374     cert_name: st
+00026f90: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00026fa0: 2020 6365 7274 5f66 6f72 6d61 743a 204c    cert_format: L
+00026fb0: 6974 6572 616c 5b22 5045 4d22 2c20 2244  iteral["PEM", "D
+00026fc0: 4552 222c 2022 504b 4353 3132 225d 203d  ER", "PKCS12"] =
+00026fd0: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
+00026fe0: 6572 745f 6461 7461 3a20 7374 7220 3d20  ert_data: str = 
+00026ff0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7365  None,.        se
+00027000: 7276 6572 5f63 6572 743a 2062 6f6f 6c20  rver_cert: bool 
+00027010: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
+00027020: 2063 615f 6365 7274 3a20 626f 6f6c 203d   ca_cert: bool =
+00027030: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+00027040: 6372 6c3a 2062 6f6f 6c20 3d20 4661 6c73  crl: bool = Fals
+00027050: 652c 0a20 2020 2020 2020 2069 6e74 5f63  e,.        int_c
+00027060: 615f 6365 7274 3a20 626f 6f6c 203d 2046  a_cert: bool = F
+00027070: 616c 7365 2c0a 2020 2020 2020 2020 6f63  alse,.        oc
+00027080: 7370 5f72 6573 705f 6365 7274 3a20 626f  sp_resp_cert: bo
+00027090: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+000270a0: 2020 2020 6f63 7370 5f73 6967 6e65 725f      ocsp_signer_
+000270b0: 6365 7274 3a20 626f 6f6c 203d 2046 616c  cert: bool = Fal
+000270c0: 7365 2c0a 2020 2020 2020 2020 7373 685f  se,.        ssh_
+000270d0: 7075 625f 6b65 793a 2062 6f6f 6c20 3d20  pub_key: bool = 
+000270e0: 4661 6c73 652c 0a20 2020 2029 202d 3e20  False,.    ) -> 
+000270f0: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
+00027100: 2020 2222 2255 706c 6f61 6420 6120 6365    """Upload a ce
+00027110: 7274 6966 6963 6174 652e 0a0a 2020 2020  rtificate...    
+00027120: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00027130: 2020 2020 2020 7061 7373 7068 7261 7365        passphrase
+00027140: 2028 7374 7229 3a20 7061 7373 7068 7261   (str): passphra
+00027150: 7365 0a20 2020 2020 2020 2020 2020 2063  se.            c
+00027160: 6572 745f 6669 6c65 2028 5061 7468 7c73  ert_file (Path|s
+00027170: 7472 2c20 6f70 7469 6f6e 616c 293a 2043  tr, optional): C
+00027180: 6572 7420 6669 6c65 2074 6f20 7570 6c6f  ert file to uplo
+00027190: 6164 2c20 6966 2066 696c 6520 6973 2070  ad, if file is p
+000271a0: 726f 7669 6465 6420 6365 7274 5f6e 616d  rovided cert_nam
+000271b0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000271c0: 2020 616e 6420 6365 7274 5f66 6f72 6d61    and cert_forma
+000271d0: 7420 7769 6c6c 2062 6520 6465 7269 7665  t will be derive
+000271e0: 6420 6672 6f6d 2066 696c 6520 6e61 6d65  d from file name
+000271f0: 202f 2065 7874 656e 7369 6f6e 2c20 756e   / extension, un
+00027200: 6c65 7373 2074 686f 7365 2070 6172 616d  less those param
+00027210: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00027220: 2020 6172 6520 616c 736f 2070 726f 7669    are also provi
+00027230: 6465 642e 0a20 2020 2020 2020 2020 2020  ded..           
+00027240: 2063 6572 745f 6e61 6d65 2028 7374 722c   cert_name (str,
+00027250: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00027260: 6e61 6d65 206f 6620 7468 6520 6365 7274  name of the cert
+00027270: 6966 6963 6174 652e 0a20 2020 2020 2020  ificate..       
+00027280: 2020 2020 2063 6572 745f 666f 726d 6174       cert_format
+00027290: 2028 4c69 7465 7261 6c5b 2250 454d 222c   (Literal["PEM",
+000272a0: 2022 4445 5222 2c20 2250 4b43 5331 3222   "DER", "PKCS12"
+000272b0: 5d2c 206f 7074 696f 6e61 6c29 3a20 6365  ], optional): ce
+000272c0: 7274 5f66 6f72 6d61 7420 2056 616c 6964  rt_format  Valid
+000272d0: 2056 616c 7565 733a 2050 454d 2c20 4445   Values: PEM, DE
+000272e0: 522c 2050 4b43 5331 320a 2020 2020 2020  R, PKCS12.      
+000272f0: 2020 2020 2020 6365 7274 5f64 6174 6120        cert_data 
+00027300: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+00027310: 2043 6572 7469 6669 6361 7465 2063 6f6e   Certificate con
+00027320: 7465 6e74 2065 6e63 6f64 6564 2069 6e20  tent encoded in 
+00027330: 6261 7365 3634 2066 6f72 2061 6c6c 2066  base64 for all f
+00027340: 6f72 6d61 7420 6365 7274 6966 6963 6174  ormat certificat
+00027350: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
+00027360: 7365 7276 6572 5f63 6572 7420 2862 6f6f  server_cert (boo
+00027370: 6c2c 206f 7074 696f 6e61 6c29 3a20 5365  l, optional): Se
+00027380: 7420 746f 2054 7275 6520 6966 2063 6572  t to True if cer
+00027390: 7420 6973 2061 2073 6572 7665 7220 6365  t is a server ce
+000273a0: 7274 6966 6963 6174 652e 2044 6566 6175  rtificate. Defau
+000273b0: 6c74 7320 746f 2046 616c 7365 2e0a 2020  lts to False..  
+000273c0: 2020 2020 2020 2020 2020 6361 5f63 6572            ca_cer
+000273d0: 7420 2862 6f6f 6c2c 206f 7074 696f 6e61  t (bool, optiona
+000273e0: 6c29 3a20 5365 7420 746f 2054 7275 6520  l): Set to True 
+000273f0: 6966 2063 6572 7420 6973 2061 2043 4120  if cert is a CA 
+00027400: 4365 7274 6966 6963 6174 652e 2044 6566  Certificate. Def
+00027410: 6175 6c74 7320 746f 2046 616c 7365 2e0a  aults to False..
+00027420: 2020 2020 2020 2020 2020 2020 6372 6c20              crl 
+00027430: 2862 6f6f 6c2c 206f 7074 696f 6e61 6c29  (bool, optional)
+00027440: 3a20 5365 7420 746f 2054 7275 6520 6966  : Set to True if
+00027450: 2064 6174 6120 6973 2061 2063 6572 7469   data is a certi
+00027460: 6669 6361 7465 2072 6576 6f63 6174 696f  ficate revocatio
+00027470: 6e20 6c69 7374 2e20 4465 6661 756c 7473  n list. Defaults
+00027480: 2074 6f20 4661 6c73 652e 0a20 2020 2020   to False..     
+00027490: 2020 2020 2020 2069 6e74 5f63 615f 6365         int_ca_ce
+000274a0: 7274 2028 626f 6f6c 2c20 6f70 7469 6f6e  rt (bool, option
+000274b0: 616c 293a 2053 6574 2074 6f20 5472 7565  al): Set to True
+000274c0: 2069 6620 6365 7274 6966 6963 6174 6520   if certificate 
+000274d0: 6973 2061 6e20 696e 7465 726d 6564 6961  is an intermedia
+000274e0: 7465 2043 4120 6365 7274 2e20 4465 6661  te CA cert. Defa
+000274f0: 756c 7473 2074 6f20 4661 6c73 652e 0a20  ults to False.. 
+00027500: 2020 2020 2020 2020 2020 206f 6373 705f             ocsp_
+00027510: 7265 7370 5f63 6572 7420 2862 6f6f 6c2c  resp_cert (bool,
+00027520: 206f 7074 696f 6e61 6c29 3a20 5365 7420   optional): Set 
+00027530: 746f 2054 7275 6520 6966 2063 6572 7469  to True if certi
+00027540: 6669 6361 7465 2069 7320 616e 204f 4353  ficate is an OCS
+00027550: 5020 7265 7370 6f6e 6465 7220 6365 7274  P responder cert
+00027560: 2e20 4465 6661 756c 7473 2074 6f20 4661  . Defaults to Fa
+00027570: 6c73 652e 0a20 2020 2020 2020 2020 2020  lse..           
+00027580: 206f 6373 705f 7369 676e 6572 5f63 6572   ocsp_signer_cer
+00027590: 7420 2862 6f6f 6c2c 206f 7074 696f 6e61  t (bool, optiona
+000275a0: 6c29 3a20 5365 7420 746f 2054 7275 6520  l): Set to True 
+000275b0: 6966 2063 6572 7469 6669 6361 7465 2069  if certificate i
+000275c0: 7320 616e 204f 4353 5020 7369 676e 6572  s an OCSP signer
+000275d0: 2063 6572 742e 2044 6566 6175 6c74 7320   cert. Defaults 
+000275e0: 746f 2046 616c 7365 2e0a 2020 2020 2020  to False..      
+000275f0: 2020 2020 2020 7373 685f 7075 625f 6b65        ssh_pub_ke
+00027600: 7920 2862 6f6f 6c2c 206f 7074 696f 6e61  y (bool, optiona
+00027610: 6c29 3a20 5365 7420 746f 2054 7275 6520  l): Set to True 
+00027620: 6966 2063 6572 7469 6669 6361 7465 2069  if certificate i
+00027630: 7320 616e 2053 5348 2050 7562 206b 6579  s an SSH Pub key
+00027640: 2e20 4465 6661 756c 7473 2074 6f20 4661  . Defaults to Fa
+00027650: 6c73 652e 0a20 2020 2020 2020 2020 2020  lse..           
+00027660: 2020 2020 2073 7368 5f70 7562 5f6b 6579       ssh_pub_key
+00027670: 206e 6565 6473 2074 6f20 6265 2069 6e20   needs to be in 
+00027680: 5045 4d20 666f 726d 6174 2c20 7373 682d  PEM format, ssh-
+00027690: 7273 6120 6973 206e 6f74 2073 7570 706f  rsa is not suppo
+000276a0: 7274 6564 2e0a 0a20 2020 2020 2020 2052  rted...        R
+000276b0: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
+000276c0: 2020 2056 616c 7565 4572 726f 723a 2052     ValueError: R
+000276d0: 6169 7365 6420 6966 2069 6e76 616c 6964  aised if invalid
+000276e0: 2063 6f6d 6269 6e61 7469 6f6e 206f 6620   combination of 
+000276f0: 6172 6775 6d65 6e74 7320 6973 2070 726f  arguments is pro
+00027700: 7669 6465 642e 0a0a 2020 2020 2020 2020  vided...        
+00027710: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00027720: 2020 2020 2052 6573 706f 6e73 653a 2043       Response: C
+00027730: 656e 7472 616c 4150 4920 5265 7370 6f6e  entralAPI Respon
+00027740: 7365 206f 626a 6563 740a 2020 2020 2020  se object.      
+00027750: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
+00027760: 4150 492d 464c 4157 2041 5049 206d 6574  API-FLAW API met
+00027770: 686f 642c 2050 5542 4c49 435f 4345 5254  hod, PUBLIC_CERT
+00027780: 2069 7320 6e6f 7420 6163 6365 7074 6564   is not accepted
+00027790: 0a20 2020 2020 2020 2075 726c 203d 2022  .        url = "
+000277a0: 2f63 6f6e 6669 6775 7261 7469 6f6e 2f76  /configuration/v
+000277b0: 312f 6365 7274 6966 6963 6174 6573 220a  1/certificates".
+000277c0: 2020 2020 2020 2020 7661 6c69 645f 7479          valid_ty
+000277d0: 7065 7320 3d20 5b0a 2020 2020 2020 2020  pes = [.        
+000277e0: 2020 2020 2253 4552 5645 525f 4345 5254      "SERVER_CERT
+000277f0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00027800: 4341 5f43 4552 5422 2c0a 2020 2020 2020  CA_CERT",.      
+00027810: 2020 2020 2020 2243 524c 222c 0a20 2020        "CRL",.   
+00027820: 2020 2020 2020 2020 2022 494e 5445 524d           "INTERM
+00027830: 4544 4941 5445 5f43 4122 2c0a 2020 2020  EDIATE_CA",.    
+00027840: 2020 2020 2020 2020 224f 4353 505f 5245          "OCSP_RE
+00027850: 5350 4f4e 4445 525f 4345 5254 222c 0a20  SPONDER_CERT",. 
+00027860: 2020 2020 2020 2020 2020 2022 4f43 5350             "OCSP
+00027870: 5f53 4947 4e45 525f 4345 5254 222c 0a20  _SIGNER_CERT",. 
+00027880: 2020 2020 2020 2020 2020 2022 5055 424c             "PUBL
+00027890: 4943 5f43 4552 5422 0a20 2020 2020 2020  IC_CERT".       
+000278a0: 205d 0a20 2020 2020 2020 2074 7970 655f   ].        type_
+000278b0: 7661 7273 203d 205b 7365 7276 6572 5f63  vars = [server_c
+000278c0: 6572 742c 2063 615f 6365 7274 2c20 6372  ert, ca_cert, cr
+000278d0: 6c2c 2069 6e74 5f63 615f 6365 7274 2c20  l, int_ca_cert, 
+000278e0: 6f63 7370 5f72 6573 705f 6365 7274 2c20  ocsp_resp_cert, 
+000278f0: 6f63 7370 5f73 6967 6e65 725f 6365 7274  ocsp_signer_cert
+00027900: 2c20 7373 685f 7075 625f 6b65 795d 0a20  , ssh_pub_key]. 
+00027910: 2020 2020 2020 2069 6620 7479 7065 5f76         if type_v
+00027920: 6172 732e 636f 756e 7428 5472 7565 2920  ars.count(True) 
+00027930: 3e20 313a 0a20 2020 2020 2020 2020 2020  > 1:.           
+00027940: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00027950: 7228 2250 726f 7669 6465 6420 636f 6e66  r("Provided conf
+00027960: 6c69 6374 696e 6720 6365 7274 6966 6963  licting certific
+00027970: 6174 6520 7479 7065 732c 206f 6e6c 7920  ate types, only 
+00027980: 3120 7368 6f75 6c64 2062 6520 7365 7420  1 should be set 
+00027990: 746f 2054 7275 652e 2229 0a20 2020 2020  to True.").     
+000279a0: 2020 2065 6c69 6620 616c 6c28 5b6e 6f74     elif all([not
+000279b0: 2062 6f6f 6c28 7661 7229 2066 6f72 2076   bool(var) for v
+000279c0: 6172 2069 6e20 7479 7065 5f76 6172 735d  ar in type_vars]
+000279d0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+000279e0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+000279f0: 224e 6f20 6365 7274 5f74 7970 6520 7072  "No cert_type pr
+00027a00: 6f76 6964 6564 2c20 6f6e 6520 6f66 2074  ovided, one of t
+00027a10: 6865 2063 6572 745f 7479 7065 7320 7368  he cert_types sh
+00027a20: 6f75 6c64 2062 6520 7365 7420 746f 2054  ould be set to T
+00027a30: 7275 6522 290a 0a20 2020 2020 2020 2069  rue")..        i
+00027a40: 6620 6365 7274 5f66 6f72 6d61 7420 616e  f cert_format an
+00027a50: 6420 6365 7274 5f66 6f72 6d61 742e 7570  d cert_format.up
+00027a60: 7065 7228 2920 6e6f 7420 696e 205b 2250  per() not in ["P
+00027a70: 454d 222c 2022 4445 5222 2c20 2250 4b43  EM", "DER", "PKC
+00027a80: 5331 3222 5d3a 0a20 2020 2020 2020 2020  S12"]:.         
+00027a90: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00027aa0: 726f 7228 6622 496e 7661 6c69 6420 6365  ror(f"Invalid ce
+00027ab0: 7274 5f66 6f72 6d61 7420 7b63 6572 745f  rt_format {cert_
+00027ac0: 666f 726d 6174 7d2c 2076 616c 6964 2076  format}, valid v
+00027ad0: 616c 7565 7320 6172 6520 2750 454d 272c  alues are 'PEM',
+00027ae0: 2027 4445 5227 2c20 2750 4b43 5331 3227   'DER', 'PKCS12'
+00027af0: 2229 0a20 2020 2020 2020 2065 6c69 6620  ").        elif 
+00027b00: 6e6f 7420 6365 7274 5f66 6f72 6d61 7420  not cert_format 
+00027b10: 616e 6420 6e6f 7420 6365 7274 5f66 696c  and not cert_fil
+00027b20: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00027b30: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00027b40: 2263 6572 745f 666f 726d 6174 2069 7320  "cert_format is 
+00027b50: 7265 7175 6972 6564 2077 6865 6e20 6e6f  required when no
+00027b60: 7420 7072 6f76 6964 696e 6720 6365 7274  t providing cert
+00027b70: 6966 6963 6174 6520 7669 6120 6669 6c65  ificate via file
+00027b80: 2e22 290a 0a20 2020 2020 2020 2069 6620  .")..        if 
+00027b90: 6e6f 7420 6365 7274 5f64 6174 6120 616e  not cert_data an
+00027ba0: 6420 6e6f 7420 6365 7274 5f66 696c 653a  d not cert_file:
+00027bb0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00027bc0: 7365 2056 616c 7565 4572 726f 7228 224f  se ValueError("O
+00027bd0: 6e65 206f 6620 6365 7274 5f66 696c 6520  ne of cert_file 
+00027be0: 6f72 2063 6572 745f 6461 7461 2073 686f  or cert_data sho
+00027bf0: 756c 6420 6265 2070 726f 7669 6465 6422  uld be provided"
+00027c00: 290a 2020 2020 2020 2020 656c 6966 2063  ).        elif c
+00027c10: 6572 745f 6461 7461 2061 6e64 2063 6572  ert_data and cer
+00027c20: 745f 6669 6c65 3a0a 2020 2020 2020 2020  t_file:.        
+00027c30: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00027c40: 7272 6f72 2822 4f6e 6c79 206f 6e65 206f  rror("Only one o
+00027c50: 6620 6365 7274 5f66 696c 6520 616e 6420  f cert_file and 
+00027c60: 6365 7274 5f64 6174 6120 7368 6f75 6c64  cert_data should
+00027c70: 2062 6520 7072 6f76 6964 6564 2229 0a0a   be provided")..
+00027c80: 2020 2020 2020 2020 666f 7220 6365 7274          for cert
+00027c90: 5f74 7970 652c 2076 6172 2069 6e20 7a69  _type, var in zi
+00027ca0: 7028 7661 6c69 645f 7479 7065 732c 2074  p(valid_types, t
+00027cb0: 7970 655f 7661 7273 293a 0a20 2020 2020  ype_vars):.     
+00027cc0: 2020 2020 2020 2069 6620 7661 723a 0a20         if var:. 
+00027cd0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00027ce0: 7265 616b 0a0a 2020 2020 2020 2020 6966  reak..        if
+00027cf0: 2063 6572 745f 6669 6c65 3a0a 2020 2020   cert_file:.    
+00027d00: 2020 2020 2020 2020 6365 7274 5f66 696c          cert_fil
+00027d10: 6520 3d20 5061 7468 2863 6572 745f 6669  e = Path(cert_fi
+00027d20: 6c65 2920 6966 206e 6f74 2069 7369 6e73  le) if not isins
+00027d30: 7461 6e63 6528 6365 7274 5f66 696c 652c  tance(cert_file,
+00027d40: 2050 6174 6829 2065 6c73 6520 6365 7274   Path) else cert
+00027d50: 5f66 696c 650a 2020 2020 2020 2020 2020  _file.          
+00027d60: 2020 6365 7274 5f6e 616d 6520 3d20 6365    cert_name = ce
+00027d70: 7274 5f6e 616d 6520 6f72 2063 6572 745f  rt_name or cert_
+00027d80: 6669 6c65 2e73 7465 6d0a 2020 2020 2020  file.stem.      
+00027d90: 2020 2020 2020 6966 206e 6f74 2063 6572        if not cer
+00027da0: 745f 666f 726d 6174 3a0a 2020 2020 2020  t_format:.      
+00027db0: 2020 2020 2020 2020 2020 6966 2063 6572            if cer
+00027dc0: 745f 6669 6c65 2e73 7566 6669 782e 6c6f  t_file.suffix.lo
+00027dd0: 7765 7228 2920 696e 205b 222e 7066 7822  wer() in [".pfx"
+00027de0: 2c20 222e 7031 3222 5d3a 0a20 2020 2020  , ".p12"]:.     
+00027df0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00027e00: 6572 745f 666f 726d 6174 203d 2022 504b  ert_format = "PK
+00027e10: 4353 3132 220a 2020 2020 2020 2020 2020  CS12".          
+00027e20: 2020 2020 2020 656c 6966 2063 6572 745f        elif cert_
+00027e30: 6669 6c65 2e73 7566 6669 782e 6c6f 7765  file.suffix.lowe
+00027e40: 7228 2920 696e 205b 222e 7065 6d22 2c20  r() in [".pem", 
+00027e50: 222e 6365 7222 5d3a 0a20 2020 2020 2020  ".cer"]:.       
+00027e60: 2020 2020 2020 2020 2020 2020 2063 6572               cer
+00027e70: 745f 666f 726d 6174 203d 2022 5045 4d22  t_format = "PEM"
+00027e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00027e90: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00027ea0: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
+00027eb0: 4f20 6465 7465 726d 696e 6520 666f 726d  O determine form
+00027ec0: 6174 2075 7369 6e67 2063 7279 7074 6f67  at using cryptog
+00027ed0: 7261 7068 7920 6c69 620a 2020 2020 2020  raphy lib.      
+00027ee0: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+00027ef0: 7274 5f66 6f72 6d61 7420 3d20 2244 4552  rt_format = "DER
+00027f00: 220a 2020 2020 2020 2020 2020 2020 656c  ".            el
+00027f10: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00027f20: 2020 2020 6365 7274 5f66 6f72 6d61 7420      cert_format 
+00027f30: 3d20 6365 7274 5f66 6f72 6d61 742e 7570  = cert_format.up
+00027f40: 7065 7228 290a 0a20 2020 2020 2020 2020  per()..         
+00027f50: 2020 2063 6572 745f 6461 7461 203d 2063     cert_data = c
+00027f60: 6572 745f 6669 6c65 2e72 6561 645f 7465  ert_file.read_te
+00027f70: 7874 2829 0a0a 2020 2020 2020 2020 6365  xt()..        ce
+00027f80: 7274 5f62 7974 6573 203d 2063 6572 745f  rt_bytes = cert_
+00027f90: 6461 7461 2e65 6e63 6f64 6528 2275 7466  data.encode("utf
+00027fa0: 2d38 2229 0a20 2020 2020 2020 2063 6572  -8").        cer
+00027fb0: 745f 6236 3420 3d20 6261 7365 3634 2e62  t_b64 = base64.b
+00027fc0: 3634 656e 636f 6465 2863 6572 745f 6279  64encode(cert_by
+00027fd0: 7465 7329 2e64 6563 6f64 6528 2275 7466  tes).decode("utf
+00027fe0: 2d38 2229 0a0a 2020 2020 2020 2020 6a73  -8")..        js
+00027ff0: 6f6e 5f64 6174 6120 3d20 7b0a 2020 2020  on_data = {.    
+00028000: 2020 2020 2020 2020 2763 6572 745f 6e61          'cert_na
+00028010: 6d65 273a 2063 6572 745f 6e61 6d65 2c0a  me': cert_name,.
+00028020: 2020 2020 2020 2020 2020 2020 2763 6572              'cer
+00028030: 745f 7479 7065 273a 2063 6572 745f 7479  t_type': cert_ty
+00028040: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
+00028050: 2763 6572 745f 666f 726d 6174 273a 2063  'cert_format': c
+00028060: 6572 745f 666f 726d 6174 2c0a 2020 2020  ert_format,.    
+00028070: 2020 2020 2020 2020 2770 6173 7370 6872          'passphr
+00028080: 6173 6527 3a20 7061 7373 7068 7261 7365  ase': passphrase
+00028090: 2c0a 2020 2020 2020 2020 2020 2020 2763  ,.            'c
+000280a0: 6572 745f 6461 7461 273a 2063 6572 745f  ert_data': cert_
+000280b0: 6236 340a 2020 2020 2020 2020 7d0a 0a20  b64.        }.. 
+000280c0: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
+000280d0: 6169 7420 7365 6c66 2e70 6f73 7428 7572  ait self.post(ur
+000280e0: 6c2c 206a 736f 6e5f 6461 7461 3d6a 736f  l, json_data=jso
+000280f0: 6e5f 6461 7461 290a 0a20 2020 2061 7379  n_data)..    asy
+00028100: 6e63 2064 6566 2067 6574 5f73 7562 7363  nc def get_subsc
+00028110: 7269 7074 696f 6e73 280a 2020 2020 2020  riptions(.      
+00028120: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00028130: 6c69 6365 6e73 655f 7479 7065 3a20 7374  license_type: st
+00028140: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00028150: 2020 6f66 6673 6574 3a20 696e 7420 3d20    offset: int = 
+00028160: 302c 0a20 2020 2020 2020 206c 696d 6974  0,.        limit
+00028170: 3a20 696e 7420 3d20 3130 3030 2c20 2023  : int = 1000,  #
+00028180: 2044 6f65 736e 2774 2061 7070 6561 7220   Doesn't appear 
+00028190: 746f 2068 6176 6520 6d61 782c 2061 6c6c  to have max, all
+000281a0: 6f77 6564 2031 306b 206c 696d 6974 2069  owed 10k limit i
+000281b0: 6e20 7377 6167 6765 720a 2020 2020 2920  n swagger.    ) 
+000281c0: 2d3e 2052 6573 706f 6e73 653a 0a20 2020  -> Response:.   
+000281d0: 2020 2020 2022 2222 4765 7420 7573 6572       """Get user
+000281e0: 2073 7562 7363 7269 7074 696f 6e20 6b65   subscription ke
+000281f0: 7973 2e0a 0a20 2020 2020 2020 2041 7267  ys...        Arg
+00028200: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
+00028210: 6963 656e 7365 5f74 7970 6520 2873 7472  icense_type (str
+00028220: 2c20 6f70 7469 6f6e 616c 293a 2053 7570  , optional): Sup
+00028230: 706f 7274 7320 4261 7369 632c 2053 6572  ports Basic, Ser
+00028240: 7669 6365 2054 6f6b 656e 2061 6e64 204d  vice Token and M
+00028250: 756c 7469 2054 6965 7220 6c69 6365 6e73  ulti Tier licens
+00028260: 696e 6720 7479 7065 7320 6173 2077 656c  ing types as wel
+00028270: 6c0a 2020 2020 2020 2020 2020 2020 6f66  l.            of
+00028280: 6673 6574 2028 696e 742c 206f 7074 696f  fset (int, optio
+00028290: 6e61 6c29 3a20 6f66 6673 6574 206f 7220  nal): offset or 
+000282a0: 7061 6765 206e 756d 6265 7220 4465 6661  page number Defa
+000282b0: 756c 7473 2074 6f20 302e 0a20 2020 2020  ults to 0..     
+000282c0: 2020 2020 2020 206c 696d 6974 2028 696e         limit (in
+000282d0: 742c 206f 7074 696f 6e61 6c29 3a20 4e75  t, optional): Nu
+000282e0: 6d62 6572 206f 6620 7375 6273 6372 6970  mber of subscrip
+000282f0: 7469 6f6e 7320 746f 2067 6574 2044 6566  tions to get Def
+00028300: 6175 6c74 7320 746f 2031 3030 2e0a 0a20  aults to 100... 
+00028310: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00028320: 2020 2020 2020 2020 2020 2020 5265 7370              Resp
+00028330: 6f6e 7365 3a20 4365 6e74 7261 6c41 5049  onse: CentralAPI
+00028340: 2052 6573 706f 6e73 6520 6f62 6a65 6374   Response object
+00028350: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00028360: 2020 2020 2075 726c 203d 2022 2f70 6c61       url = "/pla
+00028370: 7466 6f72 6d2f 6c69 6365 6e73 696e 672f  tform/licensing/
+00028380: 7631 2f73 7562 7363 7269 7074 696f 6e73  v1/subscriptions
+00028390: 220a 0a20 2020 2020 2020 2070 6172 616d  "..        param
+000283a0: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
+000283b0: 2020 276c 6963 656e 7365 5f74 7970 6527    'license_type'
+000283c0: 3a20 6c69 6365 6e73 655f 7479 7065 2c0a  : license_type,.
+000283d0: 2020 2020 2020 2020 2020 2020 276f 6666              'off
+000283e0: 7365 7427 3a20 6f66 6673 6574 2c0a 2020  set': offset,.  
+000283f0: 2020 2020 2020 2020 2020 276c 696d 6974            'limit
+00028400: 273a 206c 696d 6974 0a20 2020 2020 2020  ': limit.       
+00028410: 207d 0a0a 2020 2020 2020 2020 7265 7475   }..        retu
+00028420: 726e 2061 7761 6974 2073 656c 662e 6765  rn await self.ge
+00028430: 7428 7572 6c2c 2070 6172 616d 733d 7061  t(url, params=pa
+00028440: 7261 6d73 290a 0a20 2020 2061 7379 6e63  rams)..    async
+00028450: 2064 6566 2067 6574 5f73 7562 7363 7269   def get_subscri
+00028460: 7074 696f 6e5f 7374 6174 7328 0a20 2020  ption_stats(.   
+00028470: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00028480: 2020 206c 6963 656e 7365 5f74 7970 653a     license_type:
+00028490: 2073 7472 203d 2027 616c 6c27 2c0a 2020   str = 'all',.  
+000284a0: 2020 2020 2020 7365 7276 6963 653a 2073        service: s
+000284b0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+000284c0: 2020 2061 7070 5f6f 6e6c 795f 7374 6174     app_only_stat
+000284d0: 733a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  s: bool = None,.
+000284e0: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
+000284f0: 653a 0a20 2020 2020 2020 2022 2222 4765  e:.        """Ge
+00028500: 7420 7375 6273 6372 6970 7469 6f6e 2073  t subscription s
+00028510: 7461 7473 2e0a 0a20 2020 2020 2020 2041  tats...        A
+00028520: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00028530: 206c 6963 656e 7365 5f74 7970 6520 2873   license_type (s
+00028540: 7472 2c20 6f70 7469 6f6e 616c 293a 2053  tr, optional): S
+00028550: 7570 706f 7274 7320 6261 7369 632f 7370  upports basic/sp
+00028560: 6563 6961 6c2f 616c 6c2e 0a20 2020 2020  ecial/all..     
+00028570: 2020 2020 2020 2020 2020 2073 7065 6369             speci
+00028580: 616c 202d 2077 696c 6c20 6665 7463 6820  al - will fetch 
+00028590: 7468 6520 7374 6174 6973 7469 6373 206f  the statistics o
+000285a0: 6620 7370 6563 6961 6c20 6365 6e74 7261  f special centra
+000285b0: 6c20 7365 7276 6963 6573 206c 696b 6520  l services like 
+000285c0: 7061 2c20 7563 632c 2063 6c61 7269 7479  pa, ucc, clarity
+000285d0: 2065 7463 2e0a 2020 2020 2020 2020 2020   etc..          
+000285e0: 2020 2020 2020 6261 7369 6320 2d20 7769        basic - wi
+000285f0: 6c6c 2066 6574 6368 2074 6865 2073 7461  ll fetch the sta
+00028600: 7469 7374 6963 7320 6f66 2064 6576 6963  tistics of devic
+00028610: 6520 6d61 6e61 6765 6d65 6e74 2073 6572  e management ser
+00028620: 7669 6365 206c 6963 656e 7365 732e 0a20  vice licenses.. 
+00028630: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00028640: 6c6c 202d 2077 696c 6c20 6665 7463 6820  ll - will fetch 
+00028650: 626f 7468 206f 6620 7468 6573 6520 6c69  both of these li
+00028660: 6365 6e73 6520 7479 7065 732e 0a0a 2020  cense types...  
+00028670: 2020 2020 2020 2020 2020 2020 2020 416c                Al
+00028680: 736f 2073 7570 706f 7274 7320 6d75 6c74  so supports mult
+00028690: 6920 7469 6572 206c 6963 656e 7365 2074  i tier license t
+000286a0: 7970 6573 2073 7563 6820 666f 756e 6461  ypes such founda
+000286b0: 7469 6f6e 5f61 702c 2061 6476 616e 6365  tion_ap, advance
+000286c0: 645f 7377 6974 6368 5f36 3330 302c 0a20  d_switch_6300,. 
+000286d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000286e0: 6f75 6e64 6174 696f 6e5f 3730 5858 2065  oundation_70XX e
+000286f0: 7463 2e0a 0a20 2020 2020 2020 2020 2020  tc...           
+00028700: 2073 6572 7669 6365 2028 7374 722c 206f   service (str, o
+00028710: 7074 696f 6e61 6c29 3a20 5365 7276 6963  ptional): Servic
+00028720: 6520 7479 7065 3a20 7061 2f70 612c 636c  e type: pa/pa,cl
+00028730: 6172 6974 792c 666f 756e 6461 7469 6f6e  arity,foundation
+00028740: 5f61 702c 0a20 2020 2020 2020 2020 2020  _ap,.           
+00028750: 2020 2020 2061 6476 616e 6365 645f 7377       advanced_sw
+00028760: 6974 6368 5f36 3330 302c 2066 6f75 6e64  itch_6300, found
+00028770: 6174 696f 6e5f 3730 5858 2020 6574 632e  ation_70XX  etc.
+00028780: 0a20 2020 2020 2020 2020 2020 2061 7070  .            app
+00028790: 5f6f 6e6c 795f 7374 6174 7320 2862 6f6f  _only_stats (boo
+000287a0: 6c2c 206f 7074 696f 6e61 6c29 3a20 4966  l, optional): If
+000287b0: 2076 616c 7565 2069 7320 5472 7565 2c20   value is True, 
+000287c0: 7374 6174 7320 6f6e 6c79 2066 6f72 2074  stats only for t
+000287d0: 6865 2063 7572 7265 6e74 0a20 2020 2020  he current.     
+000287e0: 2020 2020 2020 2020 2020 2061 7070 6c69             appli
+000287f0: 6361 7469 6f6e 2072 6574 7572 6e65 6420  cation returned 
+00028800: 7261 7468 6572 2074 6861 6e20 676c 6f62  rather than glob
+00028810: 616c 2073 7461 7473 0a0a 2020 2020 2020  al stats..      
+00028820: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00028830: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
+00028840: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
+00028850: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
+00028860: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00028870: 7572 6c20 3d20 222f 706c 6174 666f 726d  url = "/platform
+00028880: 2f6c 6963 656e 7369 6e67 2f76 312f 7375  /licensing/v1/su
+00028890: 6273 6372 6970 7469 6f6e 732f 7374 6174  bscriptions/stat
+000288a0: 7322 0a0a 2020 2020 2020 2020 7061 7261  s"..        para
+000288b0: 6d73 203d 207b 0a20 2020 2020 2020 2020  ms = {.         
+000288c0: 2020 2027 6c69 6365 6e73 655f 7479 7065     'license_type
+000288d0: 273a 206c 6963 656e 7365 5f74 7970 652c  ': license_type,
+000288e0: 0a20 2020 2020 2020 2020 2020 2027 7365  .            'se
+000288f0: 7276 6963 6527 3a20 7365 7276 6963 652c  rvice': service,
+00028900: 0a20 2020 2020 2020 2020 2020 2027 6170  .            'ap
+00028910: 705f 6f6e 6c79 5f73 7461 7473 273a 2061  p_only_stats': a
+00028920: 7070 5f6f 6e6c 795f 7374 6174 730a 2020  pp_only_stats.  
+00028930: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00028940: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
+00028950: 6c66 2e67 6574 2875 726c 2c20 7061 7261  lf.get(url, para
+00028960: 6d73 3d70 6172 616d 7329 0a0a 2020 2020  ms=params)..    
+00028970: 6173 796e 6320 6465 6620 6765 745f 7661  async def get_va
+00028980: 6c69 645f 7375 6273 6372 6970 7469 6f6e  lid_subscription
+00028990: 5f6e 616d 6573 280a 2020 2020 2020 2020  _names(.        
+000289a0: 7365 6c66 2c0a 2020 2020 2020 2020 7365  self,.        se
+000289b0: 7276 6963 655f 6361 7465 676f 7279 3a20  rvice_category: 
+000289c0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+000289d0: 2020 2020 6465 7669 6365 5f74 7970 653a      device_type:
+000289e0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000289f0: 2029 202d 3e20 5265 7370 6f6e 7365 3a0a   ) -> Response:.
+00028a00: 2020 2020 2020 2020 2222 2247 6574 2056          """Get V
+00028a10: 616c 6964 2073 7562 7363 7269 7074 696f  alid subscriptio
+00028a20: 6e20 6e61 6d65 7320 6672 6f6d 2043 656e  n names from Cen
+00028a30: 7472 616c 2e0a 0a20 2020 2020 2020 2041  tral...        A
+00028a40: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00028a50: 2073 6572 7669 6365 5f63 6174 6567 6f72   service_categor
+00028a60: 7920 2873 7472 2c20 6f70 7469 6f6e 616c  y (str, optional
+00028a70: 293a 2053 6572 7669 6365 2063 6174 6567  ): Service categ
+00028a80: 6f72 7920 2d20 646d 2f6e 6574 776f 726b  ory - dm/network
+00028a90: 0a20 2020 2020 2020 2020 2020 2064 6576  .            dev
+00028aa0: 6963 655f 7479 7065 2028 7374 722c 206f  ice_type (str, o
+00028ab0: 7074 696f 6e61 6c29 3a20 4465 7669 6365  ptional): Device
+00028ac0: 2054 7970 6520 2d20 6961 702f 6361 702f   Type - iap/cap/
+00028ad0: 7377 6974 6368 2f62 6f63 2f63 6f6e 7472  switch/boc/contr
+00028ae0: 6f6c 6c65 720a 0a20 2020 2020 2020 2052  oller..        R
+00028af0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00028b00: 2020 2020 5265 7370 6f6e 7365 3a20 4365      Response: Ce
+00028b10: 6e74 7261 6c41 5049 2052 6573 706f 6e73  ntralAPI Respons
+00028b20: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
+00028b30: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
+00028b40: 203d 2022 2f70 6c61 7466 6f72 6d2f 6c69   = "/platform/li
+00028b50: 6365 6e73 696e 672f 7631 2f73 6572 7669  censing/v1/servi
+00028b60: 6365 732f 636f 6e66 6967 220a 0a20 2020  ces/config"..   
+00028b70: 2020 2020 2070 6172 616d 7320 3d20 7b0a       params = {.
+00028b80: 2020 2020 2020 2020 2020 2020 2773 6572              'ser
+00028b90: 7669 6365 5f63 6174 6567 6f72 7927 3a20  vice_category': 
+00028ba0: 7365 7276 6963 655f 6361 7465 676f 7279  service_category
+00028bb0: 2c0a 2020 2020 2020 2020 2020 2020 2764  ,.            'd
+00028bc0: 6576 6963 655f 7479 7065 273a 2064 6576  evice_type': dev
+00028bd0: 6963 655f 7479 7065 0a20 2020 2020 2020  ice_type.       
+00028be0: 207d 0a0a 2020 2020 2020 2020 7265 7475   }..        retu
+00028bf0: 726e 2061 7761 6974 2073 656c 662e 6765  rn await self.ge
+00028c00: 7428 7572 6c2c 2070 6172 616d 733d 7061  t(url, params=pa
+00028c10: 7261 6d73 290a 0a20 2020 2061 7379 6e63  rams)..    async
+00028c20: 2064 6566 2061 7373 6967 6e5f 6c69 6365   def assign_lice
+00028c30: 6e73 6573 2873 656c 662c 2073 6572 6961  nses(self, seria
+00028c40: 6c73 3a20 556e 696f 6e5b 7374 722c 204c  ls: Union[str, L
+00028c50: 6973 745b 7374 725d 5d2c 2073 6572 7669  ist[str]], servi
+00028c60: 6365 733a 2055 6e69 6f6e 5b73 7472 2c20  ces: Union[str, 
+00028c70: 4c69 7374 5b73 7472 5d5d 2920 2d3e 2052  List[str]]) -> R
+00028c80: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
+00028c90: 2022 2222 4173 7369 676e 2073 7562 7363   """Assign subsc
+00028ca0: 7269 7074 696f 6e20 746f 2061 2064 6576  ription to a dev
+00028cb0: 6963 652e 0a0a 2020 2020 2020 2020 2f2f  ice...        //
+00028cc0: 2055 7365 6420 696e 6469 7265 6374 6c79   Used indirectly
+00028cd0: 2062 7920 6164 6420 6465 7669 6365 2077   by add device w
+00028ce0: 6865 6e20 2d2d 6c69 6365 6e73 6520 3c6c  hen --license <l
+00028cf0: 6963 656e 7365 3e20 6973 2070 726f 7669  icense> is provi
+00028d00: 6465 6420 616e 6420 6261 7463 6820 6164  ded and batch ad
+00028d10: 6420 6465 7669 6365 7320 7769 7468 206c  d devices with l
+00028d20: 6963 656e 7365 202f 2f0a 0a20 2020 2020  icense //..     
+00028d30: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00028d40: 2020 2020 2073 6572 6961 6c73 2028 7374       serials (st
+00028d50: 7220 7c20 4c69 7374 5b73 7472 5d29 3a20  r | List[str]): 
+00028d60: 4c69 7374 206f 6620 7365 7269 616c 206e  List of serial n
+00028d70: 756d 6265 7220 6f66 2064 6576 6963 652e  umber of device.
+00028d80: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
+00028d90: 7669 6365 7320 2873 7472 207c 204c 6973  vices (str | Lis
+00028da0: 745b 7374 725d 293a 204c 6973 7420 6f66  t[str]): List of
+00028db0: 2073 6572 7669 6365 206e 616d 6573 2e20   service names. 
+00028dc0: 4361 6c6c 2073 6572 7669 6365 732f 636f  Call services/co
+00028dd0: 6e66 6967 2041 5049 2074 6f20 6765 7420  nfig API to get 
+00028de0: 7468 6520 6c69 7374 206f 660a 2020 2020  the list of.    
+00028df0: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
+00028e00: 6420 7365 7276 6963 6520 6e61 6d65 732e  d service names.
+00028e10: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00028e20: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
+00028e30: 6573 706f 6e73 653a 2043 656e 7472 616c  esponse: Central
+00028e40: 4150 4920 5265 7370 6f6e 7365 206f 626a  API Response obj
+00028e50: 6563 740a 2020 2020 2020 2020 2222 220a  ect.        """.
+00028e60: 2020 2020 2020 2020 7572 6c20 3d20 222f          url = "/
+00028e70: 706c 6174 666f 726d 2f6c 6963 656e 7369  platform/licensi
+00028e80: 6e67 2f76 312f 7375 6273 6372 6970 7469  ng/v1/subscripti
+00028e90: 6f6e 732f 6173 7369 676e 220a 2020 2020  ons/assign".    
+00028ea0: 2020 2020 7365 7269 616c 7320 3d20 7574      serials = ut
+00028eb0: 696c 732e 6c69 7374 6966 7928 7365 7269  ils.listify(seri
+00028ec0: 616c 7329 0a20 2020 2020 2020 2073 6572  als).        ser
+00028ed0: 7669 6365 7320 3d20 7574 696c 732e 6c69  vices = utils.li
+00028ee0: 7374 6966 7928 7365 7276 6963 6573 290a  stify(services).
+00028ef0: 0a20 2020 2020 2020 206a 736f 6e5f 6461  .        json_da
+00028f00: 7461 203d 207b 0a20 2020 2020 2020 2020  ta = {.         
+00028f10: 2020 2027 7365 7269 616c 7327 3a20 7365     'serials': se
+00028f20: 7269 616c 732c 0a20 2020 2020 2020 2020  rials,.         
+00028f30: 2020 2027 7365 7276 6963 6573 273a 2073     'services': s
+00028f40: 6572 7669 6365 730a 2020 2020 2020 2020  ervices.        
+00028f50: 7d0a 0a20 2020 2020 2020 2072 6574 7572  }..        retur
+00028f60: 6e20 6177 6169 7420 7365 6c66 2e70 6f73  n await self.pos
+00028f70: 7428 7572 6c2c 206a 736f 6e5f 6461 7461  t(url, json_data
+00028f80: 3d6a 736f 6e5f 6461 7461 290a 0a20 2020  =json_data)..   
+00028f90: 2061 7379 6e63 2064 6566 2075 6e61 7373   async def unass
+00028fa0: 6967 6e5f 6c69 6365 6e73 6573 2873 656c  ign_licenses(sel
+00028fb0: 662c 2073 6572 6961 6c73 3a20 556e 696f  f, serials: Unio
+00028fc0: 6e5b 7374 722c 204c 6973 745b 7374 725d  n[str, List[str]
+00028fd0: 5d2c 2073 6572 7669 6365 733a 2055 6e69  ], services: Uni
+00028fe0: 6f6e 5b73 7472 2c20 4c69 7374 5b73 7472  on[str, List[str
+00028ff0: 5d5d 2920 2d3e 2052 6573 706f 6e73 653a  ]]) -> Response:
+00029000: 0a20 2020 2020 2020 2022 2222 556e 6173  .        """Unas
+00029010: 7369 676e 2073 7562 7363 7269 7074 696f  sign subscriptio
+00029020: 6e28 7329 2066 726f 6d20 6465 7669 6365  n(s) from device
+00029030: 2873 292e 0a0a 2020 2020 2020 2020 4172  (s)...        Ar
+00029040: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00029050: 7365 7269 616c 7320 2873 7472 207c 204c  serials (str | L
+00029060: 6973 745b 7374 725d 293a 204c 6973 7420  ist[str]): List 
+00029070: 6f66 2073 6572 6961 6c20 6e75 6d62 6572  of serial number
+00029080: 206f 6620 6465 7669 6365 2e0a 2020 2020   of device..    
+00029090: 2020 2020 2020 2020 7365 7276 6963 6573          services
+000290a0: 2028 7374 7220 7c20 4c69 7374 5b73 7472   (str | List[str
+000290b0: 5d29 3a20 4c69 7374 206f 6620 7365 7276  ]): List of serv
+000290c0: 6963 6520 6e61 6d65 732e 2043 616c 6c20  ice names. Call 
+000290d0: 7365 7276 6963 6573 2f63 6f6e 6669 6720  services/config 
+000290e0: 4150 4920 746f 2067 6574 2074 6865 206c  API to get the l
+000290f0: 6973 7420 6f66 0a20 2020 2020 2020 2020  ist of.         
+00029100: 2020 2020 2020 2076 616c 6964 2073 6572         valid ser
+00029110: 7669 6365 206e 616d 6573 2e0a 0a20 2020  vice names...   
+00029120: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00029130: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
+00029140: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
+00029150: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
+00029160: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00029170: 2020 2075 726c 203d 2022 2f70 6c61 7466     url = "/platf
+00029180: 6f72 6d2f 6c69 6365 6e73 696e 672f 7631  orm/licensing/v1
+00029190: 2f73 7562 7363 7269 7074 696f 6e73 2f75  /subscriptions/u
+000291a0: 6e61 7373 6967 6e22 0a20 2020 2020 2020  nassign".       
+000291b0: 2073 6572 6961 6c73 203d 2075 7469 6c73   serials = utils
+000291c0: 2e6c 6973 7469 6679 2873 6572 6961 6c73  .listify(serials
+000291d0: 290a 2020 2020 2020 2020 7365 7276 6963  ).        servic
+000291e0: 6573 203d 2075 7469 6c73 2e6c 6973 7469  es = utils.listi
+000291f0: 6679 2873 6572 7669 6365 7329 0a0a 2020  fy(services)..  
+00029200: 2020 2020 2020 6a73 6f6e 5f64 6174 6120        json_data 
+00029210: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00029220: 2773 6572 6961 6c73 273a 2073 6572 6961  'serials': seria
+00029230: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
+00029240: 2773 6572 7669 6365 7327 3a20 7365 7276  'services': serv
+00029250: 6963 6573 0a20 2020 2020 2020 207d 0a0a  ices.        }..
+00029260: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00029270: 7761 6974 2073 656c 662e 706f 7374 2875  wait self.post(u
+00029280: 726c 2c20 6a73 6f6e 5f64 6174 613d 6a73  rl, json_data=js
+00029290: 6f6e 5f64 6174 6129 0a0a 2020 2020 2320  on_data)..    # 
+000292a0: 544f 444f 2062 7569 6c64 2061 6767 7265  TODO build aggre
+000292b0: 6761 746f 7220 746f 2072 756e 2072 6570  gator to run rep
+000292c0: 6f72 7420 7368 6f77 696e 6720 726f 6775  ort showing rogu
+000292d0: 6573 2f69 6e74 6572 6665 7269 6e67 2f6e  es/interfering/n
+000292e0: 6569 6768 626f 7273 0a20 2020 2023 2061  eighbors.    # a
+000292f0: 7379 6e63 2064 6566 2077 6964 735f 6765  sync def wids_ge
+00029300: 745f 616c 6c28 7365 6c66 293a 0a0a 2020  t_all(self):..  
+00029310: 2020 6173 796e 6320 6465 6620 7769 6473    async def wids
+00029320: 5f67 6574 5f72 6f67 7565 5f61 7073 280a  _get_rogue_aps(.
+00029330: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00029340: 2020 2020 2020 6772 6f75 703a 204c 6973        group: Lis
+00029350: 745b 7374 725d 203d 204e 6f6e 652c 0a20  t[str] = None,. 
+00029360: 2020 2020 2020 206c 6162 656c 3a20 4c69         label: Li
+00029370: 7374 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  st[str] = None,.
+00029380: 2020 2020 2020 2020 7369 7465 3a20 4c69          site: Li
+00029390: 7374 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  st[str] = None,.
+000293a0: 2020 2020 2020 2020 7374 6172 743a 2069          start: i
+000293b0: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
+000293c0: 2020 2065 6e64 3a20 696e 7420 3d20 4e6f     end: int = No
+000293d0: 6e65 2c0a 2020 2020 2020 2020 7377 6172  ne,.        swar
+000293e0: 6d5f 6964 3a20 7374 7220 3d20 4e6f 6e65  m_id: str = None
+000293f0: 2c0a 2020 2020 2020 2020 6672 6f6d 5f74  ,.        from_t
+00029400: 696d 6573 7461 6d70 3a20 696e 7420 3d20  imestamp: int = 
+00029410: 4e6f 6e65 2c0a 2020 2020 2020 2020 746f  None,.        to
+00029420: 5f74 696d 6573 7461 6d70 3a20 696e 7420  _timestamp: int 
+00029430: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00029440: 6f66 6673 6574 3a20 696e 7420 3d20 302c  offset: int = 0,
+00029450: 0a20 2020 2020 2020 206c 696d 6974 3a20  .        limit: 
+00029460: 696e 7420 3d20 3130 300a 2020 2020 2920  int = 100.    ) 
+00029470: 2d3e 2052 6573 706f 6e73 653a 0a20 2020  -> Response:.   
+00029480: 2020 2020 2022 2222 4c69 7374 2052 6f67       """List Rog
+00029490: 7565 2041 5073 2e0a 0a20 2020 2020 2020  ue APs...       
+000294a0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+000294b0: 2020 2067 726f 7570 2028 4c69 7374 5b73     group (List[s
+000294c0: 7472 5d2c 206f 7074 696f 6e61 6c29 3a20  tr], optional): 
+000294d0: 4c69 7374 206f 6620 6772 6f75 7020 6e61  List of group na
+000294e0: 6d65 730a 2020 2020 2020 2020 2020 2020  mes.            
+000294f0: 6c61 6265 6c20 284c 6973 745b 7374 725d  label (List[str]
+00029500: 2c20 6f70 7469 6f6e 616c 293a 204c 6973  , optional): Lis
+00029510: 7420 6f66 206c 6162 656c 206e 616d 6573  t of label names
+00029520: 0a20 2020 2020 2020 2020 2020 2073 6974  .            sit
+00029530: 6520 284c 6973 745b 7374 725d 2c20 6f70  e (List[str], op
+00029540: 7469 6f6e 616c 293a 204c 6973 7420 6f66  tional): List of
+00029550: 2073 6974 6520 6e61 6d65 730a 2020 2020   site names.    
+00029560: 2020 2020 2020 2020 7374 6172 7420 2869          start (i
+00029570: 6e74 2c20 6f70 7469 6f6e 616c 293a 204e  nt, optional): N
+00029580: 6565 6420 696e 666f 726d 6174 696f 6e20  eed information 
+00029590: 6672 6f6d 2074 6869 7320 7469 6d65 7374  from this timest
+000295a0: 616d 702e 2054 696d 6573 7461 6d70 2069  amp. Timestamp i
+000295b0: 7320 6570 6f63 6820 696e 0a20 2020 2020  s epoch in.     
+000295c0: 2020 2020 2020 2020 2020 206d 696c 6c69             milli
+000295d0: 7365 636f 6e64 732e 2044 6566 6175 6c74  seconds. Default
+000295e0: 2069 7320 6375 7272 656e 7420 7469 6d65   is current time
+000295f0: 7374 616d 7020 6d69 6e75 7320 3320 686f  stamp minus 3 ho
+00029600: 7572 730a 2020 2020 2020 2020 2020 2020  urs.            
+00029610: 656e 6420 2869 6e74 2c20 6f70 7469 6f6e  end (int, option
+00029620: 616c 293a 204e 6565 6420 696e 666f 726d  al): Need inform
+00029630: 6174 696f 6e20 746f 2074 6869 7320 7469  ation to this ti
+00029640: 6d65 7374 616d 702e 2054 696d 6573 7461  mestamp. Timesta
+00029650: 6d70 2069 7320 6570 6f63 6820 696e 0a20  mp is epoch in. 
+00029660: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00029670: 696c 6c69 7365 636f 6e64 732e 2044 6566  illiseconds. Def
+00029680: 6175 6c74 2069 7320 6375 7272 656e 7420  ault is current 
+00029690: 7469 6d65 7374 616d 700a 2020 2020 2020  timestamp.      
+000296a0: 2020 2020 2020 7377 6172 6d5f 6964 2028        swarm_id (
+000296b0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+000296c0: 4669 6c74 6572 2062 7920 5377 6172 6d20  Filter by Swarm 
+000296d0: 4944 0a20 2020 2020 2020 2020 2020 2066  ID.            f
+000296e0: 726f 6d5f 7469 6d65 7374 616d 7020 2869  rom_timestamp (i
+000296f0: 6e74 2c20 6f70 7469 6f6e 616c 293a 2054  nt, optional): T
+00029700: 6869 7320 7061 7261 6d65 7465 7220 7375  his parameter su
+00029710: 7065 7263 6564 6573 2073 7461 7274 2070  percedes start p
+00029720: 6172 616d 6574 6572 2e20 4e65 6564 0a20  arameter. Need. 
+00029730: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00029740: 6e66 6f72 6d61 7469 6f6e 2066 726f 6d20  nformation from 
+00029750: 7468 6973 2074 696d 6573 7461 6d70 2e20  this timestamp. 
+00029760: 5469 6d65 7374 616d 7020 6973 2065 706f  Timestamp is epo
+00029770: 6368 2069 6e20 7365 636f 6e64 732e 2044  ch in seconds. D
+00029780: 6566 6175 6c74 2069 7320 6375 7272 656e  efault is curren
+00029790: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+000297a0: 2020 5554 4320 7469 6d65 7374 616d 7020    UTC timestamp 
+000297b0: 6d69 6e75 7320 3320 686f 7572 730a 2020  minus 3 hours.  
+000297c0: 2020 2020 2020 2020 2020 746f 5f74 696d            to_tim
+000297d0: 6573 7461 6d70 2028 696e 742c 206f 7074  estamp (int, opt
+000297e0: 696f 6e61 6c29 3a20 5468 6973 2070 6172  ional): This par
+000297f0: 616d 6574 6572 2073 7570 6572 6365 6465  ameter supercede
+00029800: 7320 656e 6420 7061 7261 6d65 7465 722e  s end parameter.
+00029810: 204e 6565 6420 696e 666f 726d 6174 696f   Need informatio
+00029820: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00029830: 2020 746f 2074 6869 7320 7469 6d65 7374    to this timest
+00029840: 616d 702e 2054 696d 6573 7461 6d70 2069  amp. Timestamp i
+00029850: 7320 6570 6f63 6820 696e 2073 6563 6f6e  s epoch in secon
+00029860: 6473 2e20 4465 6661 756c 7420 6973 2063  ds. Default is c
+00029870: 7572 7265 6e74 2055 5443 2074 696d 6573  urrent UTC times
+00029880: 7461 6d70 0a20 2020 2020 2020 2020 2020  tamp.           
+00029890: 206f 6666 7365 7420 2869 6e74 2c20 6f70   offset (int, op
+000298a0: 7469 6f6e 616c 293a 2050 6167 696e 6174  tional): Paginat
+000298b0: 696f 6e20 6f66 6673 6574 2028 6465 6661  ion offset (defa
+000298c0: 756c 7420 3d20 3029 2044 6566 6175 6c74  ult = 0) Default
+000298d0: 7320 746f 2030 2e0a 2020 2020 2020 2020  s to 0..        
+000298e0: 2020 2020 6c69 6d69 7420 2869 6e74 2c20      limit (int, 
+000298f0: 6f70 7469 6f6e 616c 293a 2070 6167 696e  optional): pagin
+00029900: 6174 696f 6e20 7369 7a65 2028 6465 6661  ation size (defa
+00029910: 756c 7420 3d20 3130 3029 2044 6566 6175  ult = 100) Defau
+00029920: 6c74 7320 746f 2031 3030 2e0a 0a20 2020  lts to 100...   
+00029930: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00029940: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
+00029950: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
+00029960: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
+00029970: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00029980: 2020 2075 726c 203d 2022 2f72 6170 6964     url = "/rapid
+00029990: 732f 7631 2f72 6f67 7565 5f61 7073 220a  s/v1/rogue_aps".
+000299a0: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
+000299b0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+000299c0: 2767 726f 7570 273a 2067 726f 7570 2c0a  'group': group,.
+000299d0: 2020 2020 2020 2020 2020 2020 276c 6162              'lab
+000299e0: 656c 273a 206c 6162 656c 2c0a 2020 2020  el': label,.    
+000299f0: 2020 2020 2020 2020 2773 6974 6527 3a20          'site': 
+00029a00: 7369 7465 2c0a 2020 2020 2020 2020 2020  site,.          
+00029a10: 2020 2773 7461 7274 273a 2073 7461 7274    'start': start
+00029a20: 2c0a 2020 2020 2020 2020 2020 2020 2765  ,.            'e
+00029a30: 6e64 273a 2065 6e64 2c0a 2020 2020 2020  nd': end,.      
+00029a40: 2020 2020 2020 2773 7761 726d 5f69 6427        'swarm_id'
+00029a50: 3a20 7377 6172 6d5f 6964 2c0a 2020 2020  : swarm_id,.    
+00029a60: 2020 2020 2020 2020 2766 726f 6d5f 7469          'from_ti
+00029a70: 6d65 7374 616d 7027 3a20 6672 6f6d 5f74  mestamp': from_t
+00029a80: 696d 6573 7461 6d70 2c0a 2020 2020 2020  imestamp,.      
+00029a90: 2020 2020 2020 2774 6f5f 7469 6d65 7374        'to_timest
+00029aa0: 616d 7027 3a20 746f 5f74 696d 6573 7461  amp': to_timesta
+00029ab0: 6d70 2c0a 2020 2020 2020 2020 2020 2020  mp,.            
+00029ac0: 276f 6666 7365 7427 3a20 6f66 6673 6574  'offset': offset
+00029ad0: 2c0a 2020 2020 2020 2020 2020 2020 276c  ,.            'l
+00029ae0: 696d 6974 273a 206c 696d 6974 0a20 2020  imit': limit.   
+00029af0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00029b00: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+00029b10: 662e 6765 7428 7572 6c2c 2070 6172 616d  f.get(url, param
+00029b20: 733d 7061 7261 6d73 290a 0a20 2020 2061  s=params)..    a
+00029b30: 7379 6e63 2064 6566 2077 6964 735f 6765  sync def wids_ge
+00029b40: 745f 696e 7465 7266 6572 696e 675f 6170  t_interfering_ap
+00029b50: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
+00029b60: 0a20 2020 2020 2020 2067 726f 7570 3a20  .        group: 
+00029b70: 4c69 7374 5b73 7472 5d20 3d20 4e6f 6e65  List[str] = None
+00029b80: 2c0a 2020 2020 2020 2020 6c61 6265 6c3a  ,.        label:
+00029b90: 204c 6973 745b 7374 725d 203d 204e 6f6e   List[str] = Non
+00029ba0: 652c 0a20 2020 2020 2020 2073 6974 653a  e,.        site:
+00029bb0: 204c 6973 745b 7374 725d 203d 204e 6f6e   List[str] = Non
+00029bc0: 652c 0a20 2020 2020 2020 2073 7461 7274  e,.        start
+00029bd0: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+00029be0: 2020 2020 2020 656e 643a 2069 6e74 203d        end: int =
+00029bf0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+00029c00: 7761 726d 5f69 643a 2073 7472 203d 204e  warm_id: str = N
+00029c10: 6f6e 652c 0a20 2020 2020 2020 2066 726f  one,.        fro
+00029c20: 6d5f 7469 6d65 7374 616d 703a 2069 6e74  m_timestamp: int
+00029c30: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00029c40: 2074 6f5f 7469 6d65 7374 616d 703a 2069   to_timestamp: i
+00029c50: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
+00029c60: 2020 206f 6666 7365 743a 2069 6e74 203d     offset: int =
+00029c70: 2030 2c0a 2020 2020 2020 2020 6c69 6d69   0,.        limi
+00029c80: 743a 2069 6e74 203d 2031 3030 0a20 2020  t: int = 100.   
+00029c90: 2029 202d 3e20 5265 7370 6f6e 7365 3a0a   ) -> Response:.
+00029ca0: 2020 2020 2020 2020 2222 224c 6973 7420          """List 
+00029cb0: 496e 7465 7266 6572 696e 6720 4150 732e  Interfering APs.
+00029cc0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00029cd0: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
+00029ce0: 7020 284c 6973 745b 7374 725d 2c20 6f70  p (List[str], op
+00029cf0: 7469 6f6e 616c 293a 204c 6973 7420 6f66  tional): List of
+00029d00: 2067 726f 7570 206e 616d 6573 0a20 2020   group names.   
+00029d10: 2020 2020 2020 2020 206c 6162 656c 2028           label (
+00029d20: 4c69 7374 5b73 7472 5d2c 206f 7074 696f  List[str], optio
+00029d30: 6e61 6c29 3a20 4c69 7374 206f 6620 6c61  nal): List of la
+00029d40: 6265 6c20 6e61 6d65 730a 2020 2020 2020  bel names.      
+00029d50: 2020 2020 2020 7369 7465 2028 4c69 7374        site (List
+00029d60: 5b73 7472 5d2c 206f 7074 696f 6e61 6c29  [str], optional)
+00029d70: 3a20 4c69 7374 206f 6620 7369 7465 206e  : List of site n
+00029d80: 616d 6573 0a20 2020 2020 2020 2020 2020  ames.           
+00029d90: 2073 7461 7274 2028 696e 742c 206f 7074   start (int, opt
+00029da0: 696f 6e61 6c29 3a20 4e65 6564 2069 6e66  ional): Need inf
+00029db0: 6f72 6d61 7469 6f6e 2066 726f 6d20 7468  ormation from th
+00029dc0: 6973 2074 696d 6573 7461 6d70 2e20 5469  is timestamp. Ti
+00029dd0: 6d65 7374 616d 7020 6973 2065 706f 6368  mestamp is epoch
+00029de0: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
+00029df0: 2020 2020 6d69 6c6c 6973 6563 6f6e 6473      milliseconds
+00029e00: 2e20 4465 6661 756c 7420 6973 2063 7572  . Default is cur
+00029e10: 7265 6e74 2074 696d 6573 7461 6d70 206d  rent timestamp m
+00029e20: 696e 7573 2033 2068 6f75 7273 0a20 2020  inus 3 hours.   
+00029e30: 2020 2020 2020 2020 2065 6e64 2028 696e           end (in
+00029e40: 742c 206f 7074 696f 6e61 6c29 3a20 4e65  t, optional): Ne
+00029e50: 6564 2069 6e66 6f72 6d61 7469 6f6e 2074  ed information t
+00029e60: 6f20 7468 6973 2074 696d 6573 7461 6d70  o this timestamp
+00029e70: 2e20 5469 6d65 7374 616d 7020 6973 2065  . Timestamp is e
+00029e80: 706f 6368 2069 6e0a 2020 2020 2020 2020  poch in.        
+00029e90: 2020 2020 2020 2020 6d69 6c6c 6973 6563          millisec
+00029ea0: 6f6e 6473 2e20 4465 6661 756c 7420 6973  onds. Default is
+00029eb0: 2063 7572 7265 6e74 2074 696d 6573 7461   current timesta
+00029ec0: 6d70 0a20 2020 2020 2020 2020 2020 2073  mp.            s
+00029ed0: 7761 726d 5f69 6420 2873 7472 2c20 6f70  warm_id (str, op
+00029ee0: 7469 6f6e 616c 293a 2046 696c 7465 7220  tional): Filter 
+00029ef0: 6279 2053 7761 726d 2049 440a 2020 2020  by Swarm ID.    
+00029f00: 2020 2020 2020 2020 6672 6f6d 5f74 696d          from_tim
+00029f10: 6573 7461 6d70 2028 696e 742c 206f 7074  estamp (int, opt
+00029f20: 696f 6e61 6c29 3a20 5468 6973 2070 6172  ional): This par
+00029f30: 616d 6574 6572 2073 7570 6572 6365 6465  ameter supercede
+00029f40: 7320 7374 6172 7420 7061 7261 6d65 7465  s start paramete
+00029f50: 722e 204e 6565 640a 2020 2020 2020 2020  r. Need.        
+00029f60: 2020 2020 2020 2020 696e 666f 726d 6174          informat
+00029f70: 696f 6e20 6672 6f6d 2074 6869 7320 7469  ion from this ti
+00029f80: 6d65 7374 616d 702e 2054 696d 6573 7461  mestamp. Timesta
+00029f90: 6d70 2069 7320 6570 6f63 6820 696e 2073  mp is epoch in s
+00029fa0: 6563 6f6e 6473 2e20 4465 6661 756c 7420  econds. Default 
+00029fb0: 6973 2063 7572 7265 6e74 0a20 2020 2020  is current.     
+00029fc0: 2020 2020 2020 2020 2020 2055 5443 2074             UTC t
+00029fd0: 696d 6573 7461 6d70 206d 696e 7573 2033  imestamp minus 3
+00029fe0: 2068 6f75 7273 0a20 2020 2020 2020 2020   hours.         
+00029ff0: 2020 2074 6f5f 7469 6d65 7374 616d 7020     to_timestamp 
+0002a000: 2869 6e74 2c20 6f70 7469 6f6e 616c 293a  (int, optional):
+0002a010: 2054 6869 7320 7061 7261 6d65 7465 7220   This parameter 
+0002a020: 7375 7065 7263 6564 6573 2065 6e64 2070  supercedes end p
+0002a030: 6172 616d 6574 6572 2e20 4e65 6564 2069  arameter. Need i
+0002a040: 6e66 6f72 6d61 7469 6f6e 0a20 2020 2020  nformation.     
+0002a050: 2020 2020 2020 2020 2020 2074 6f20 7468             to th
+0002a060: 6973 2074 696d 6573 7461 6d70 2e20 5469  is timestamp. Ti
+0002a070: 6d65 7374 616d 7020 6973 2065 706f 6368  mestamp is epoch
+0002a080: 2069 6e20 7365 636f 6e64 732e 2044 6566   in seconds. Def
+0002a090: 6175 6c74 2069 7320 6375 7272 656e 7420  ault is current 
+0002a0a0: 5554 4320 7469 6d65 7374 616d 700a 2020  UTC timestamp.  
+0002a0b0: 2020 2020 2020 2020 2020 6f66 6673 6574            offset
+0002a0c0: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
+0002a0d0: 3a20 5061 6769 6e61 7469 6f6e 206f 6666  : Pagination off
+0002a0e0: 7365 7420 2864 6566 6175 6c74 203d 2030  set (default = 0
+0002a0f0: 2920 4465 6661 756c 7473 2074 6f20 302e  ) Defaults to 0.
+0002a100: 0a20 2020 2020 2020 2020 2020 206c 696d  .            lim
+0002a110: 6974 2028 696e 742c 206f 7074 696f 6e61  it (int, optiona
+0002a120: 6c29 3a20 7061 6769 6e61 7469 6f6e 2073  l): pagination s
+0002a130: 697a 6520 2864 6566 6175 6c74 203d 2031  ize (default = 1
+0002a140: 3030 2920 4465 6661 756c 7473 2074 6f20  00) Defaults to 
+0002a150: 3130 302e 0a0a 2020 2020 2020 2020 5265  100...        Re
+0002a160: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+0002a170: 2020 2052 6573 706f 6e73 653a 2043 656e     Response: Cen
+0002a180: 7472 616c 4150 4920 5265 7370 6f6e 7365  tralAPI Response
+0002a190: 206f 626a 6563 740a 2020 2020 2020 2020   object.        
+0002a1a0: 2222 220a 2020 2020 2020 2020 7572 6c20  """.        url 
+0002a1b0: 3d20 222f 7261 7069 6473 2f76 312f 696e  = "/rapids/v1/in
+0002a1c0: 7465 7266 6572 696e 675f 6170 7322 0a0a  terfering_aps"..
+0002a1d0: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
+0002a1e0: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
+0002a1f0: 6772 6f75 7027 3a20 6772 6f75 702c 0a20  group': group,. 
+0002a200: 2020 2020 2020 2020 2020 2027 6c61 6265             'labe
+0002a210: 6c27 3a20 6c61 6265 6c2c 0a20 2020 2020  l': label,.     
+0002a220: 2020 2020 2020 2027 7369 7465 273a 2073         'site': s
+0002a230: 6974 652c 0a20 2020 2020 2020 2020 2020  ite,.           
+0002a240: 2027 7374 6172 7427 3a20 7374 6172 742c   'start': start,
+0002a250: 0a20 2020 2020 2020 2020 2020 2027 656e  .            'en
+0002a260: 6427 3a20 656e 642c 0a20 2020 2020 2020  d': end,.       
+0002a270: 2020 2020 2027 7377 6172 6d5f 6964 273a       'swarm_id':
+0002a280: 2073 7761 726d 5f69 642c 0a20 2020 2020   swarm_id,.     
+0002a290: 2020 2020 2020 2027 6672 6f6d 5f74 696d         'from_tim
+0002a2a0: 6573 7461 6d70 273a 2066 726f 6d5f 7469  estamp': from_ti
+0002a2b0: 6d65 7374 616d 702c 0a20 2020 2020 2020  mestamp,.       
+0002a2c0: 2020 2020 2027 746f 5f74 696d 6573 7461       'to_timesta
+0002a2d0: 6d70 273a 2074 6f5f 7469 6d65 7374 616d  mp': to_timestam
+0002a2e0: 702c 0a20 2020 2020 2020 2020 2020 2027  p,.            '
+0002a2f0: 6f66 6673 6574 273a 206f 6666 7365 742c  offset': offset,
+0002a300: 0a20 2020 2020 2020 2020 2020 2027 6c69  .            'li
+0002a310: 6d69 7427 3a20 6c69 6d69 740a 2020 2020  mit': limit.    
+0002a320: 2020 2020 7d0a 0a20 2020 2020 2020 2072      }..        r
+0002a330: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+0002a340: 2e67 6574 2875 726c 2c20 7061 7261 6d73  .get(url, params
+0002a350: 3d70 6172 616d 7329 0a0a 2020 2020 6173  =params)..    as
+0002a360: 796e 6320 6465 6620 7769 6473 5f67 6574  ync def wids_get
+0002a370: 5f73 7573 7065 6374 5f61 7073 280a 2020  _suspect_aps(.  
+0002a380: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0002a390: 2020 2020 6772 6f75 703a 204c 6973 745b      group: List[
+0002a3a0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+0002a3b0: 2020 2020 206c 6162 656c 3a20 4c69 7374       label: List
+0002a3c0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0002a3d0: 2020 2020 2020 7369 7465 3a20 4c69 7374        site: List
+0002a3e0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0002a3f0: 2020 2020 2020 7374 6172 743a 2069 6e74        start: int
 0002a400: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0002a410: 206c 6162 656c 3a20 4c69 7374 5b73 7472   label: List[str
-0002a420: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0002a430: 2020 7369 7465 3a20 4c69 7374 5b73 7472    site: List[str
-0002a440: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0002a450: 2020 7374 6172 743a 2069 6e74 203d 204e    start: int = N
-0002a460: 6f6e 652c 0a20 2020 2020 2020 2065 6e64  one,.        end
-0002a470: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-0002a480: 2020 2020 2020 7377 6172 6d5f 6964 3a20        swarm_id: 
-0002a490: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0002a4a0: 2020 2020 6672 6f6d 5f74 696d 6573 7461      from_timesta
-0002a4b0: 6d70 3a20 696e 7420 3d20 4e6f 6e65 2c0a  mp: int = None,.
-0002a4c0: 2020 2020 2020 2020 746f 5f74 696d 6573          to_times
-0002a4d0: 7461 6d70 3a20 696e 7420 3d20 4e6f 6e65  tamp: int = None
-0002a4e0: 2c0a 2020 2020 2020 2020 6f66 6673 6574  ,.        offset
-0002a4f0: 3a20 696e 7420 3d20 302c 0a20 2020 2020  : int = 0,.     
-0002a500: 2020 206c 696d 6974 3a20 696e 7420 3d20     limit: int = 
-0002a510: 3130 300a 2020 2020 2920 2d3e 2052 6573  100.    ) -> Res
-0002a520: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
-0002a530: 2222 4c69 7374 206e 6569 6768 626f 7220  ""List neighbor 
-0002a540: 4150 732e 0a0a 2020 2020 2020 2020 4172  APs...        Ar
-0002a550: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0002a560: 6772 6f75 7020 284c 6973 745b 7374 725d  group (List[str]
-0002a570: 2c20 6f70 7469 6f6e 616c 293a 204c 6973  , optional): Lis
-0002a580: 7420 6f66 2067 726f 7570 206e 616d 6573  t of group names
-0002a590: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-0002a5a0: 656c 2028 4c69 7374 5b73 7472 5d2c 206f  el (List[str], o
-0002a5b0: 7074 696f 6e61 6c29 3a20 4c69 7374 206f  ptional): List o
-0002a5c0: 6620 6c61 6265 6c20 6e61 6d65 730a 2020  f label names.  
-0002a5d0: 2020 2020 2020 2020 2020 7369 7465 2028            site (
-0002a5e0: 4c69 7374 5b73 7472 5d2c 206f 7074 696f  List[str], optio
-0002a5f0: 6e61 6c29 3a20 4c69 7374 206f 6620 7369  nal): List of si
-0002a600: 7465 206e 616d 6573 0a20 2020 2020 2020  te names.       
-0002a610: 2020 2020 2073 7461 7274 2028 696e 742c       start (int,
-0002a620: 206f 7074 696f 6e61 6c29 3a20 4e65 6564   optional): Need
-0002a630: 2069 6e66 6f72 6d61 7469 6f6e 2066 726f   information fro
-0002a640: 6d20 7468 6973 2074 696d 6573 7461 6d70  m this timestamp
-0002a650: 2e20 5469 6d65 7374 616d 7020 6973 2065  . Timestamp is e
-0002a660: 706f 6368 2069 6e0a 2020 2020 2020 2020  poch in.        
-0002a670: 2020 2020 2020 2020 6d69 6c6c 6973 6563          millisec
-0002a680: 6f6e 6473 2e20 4465 6661 756c 7420 6973  onds. Default is
-0002a690: 2063 7572 7265 6e74 2074 696d 6573 7461   current timesta
-0002a6a0: 6d70 206d 696e 7573 2033 2068 6f75 7273  mp minus 3 hours
-0002a6b0: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
-0002a6c0: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
-0002a6d0: 3a20 4e65 6564 2069 6e66 6f72 6d61 7469  : Need informati
-0002a6e0: 6f6e 2074 6f20 7468 6973 2074 696d 6573  on to this times
-0002a6f0: 7461 6d70 2e20 5469 6d65 7374 616d 7020  tamp. Timestamp 
-0002a700: 6973 2065 706f 6368 2069 6e0a 2020 2020  is epoch in.    
-0002a710: 2020 2020 2020 2020 2020 2020 6d69 6c6c              mill
-0002a720: 6973 6563 6f6e 6473 2e20 4465 6661 756c  iseconds. Defaul
-0002a730: 7420 6973 2063 7572 7265 6e74 2074 696d  t is current tim
-0002a740: 6573 7461 6d70 0a20 2020 2020 2020 2020  estamp.         
-0002a750: 2020 2073 7761 726d 5f69 6420 2873 7472     swarm_id (str
-0002a760: 2c20 6f70 7469 6f6e 616c 293a 2046 696c  , optional): Fil
-0002a770: 7465 7220 6279 2053 7761 726d 2049 440a  ter by Swarm ID.
-0002a780: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
-0002a790: 5f74 696d 6573 7461 6d70 2028 696e 742c  _timestamp (int,
-0002a7a0: 206f 7074 696f 6e61 6c29 3a20 5468 6973   optional): This
-0002a7b0: 2070 6172 616d 6574 6572 2073 7570 6572   parameter super
-0002a7c0: 6365 6465 7320 7374 6172 7420 7061 7261  cedes start para
-0002a7d0: 6d65 7465 722e 204e 6565 640a 2020 2020  meter. Need.    
-0002a7e0: 2020 2020 2020 2020 2020 2020 696e 666f              info
-0002a7f0: 726d 6174 696f 6e20 6672 6f6d 2074 6869  rmation from thi
-0002a800: 7320 7469 6d65 7374 616d 702e 2054 696d  s timestamp. Tim
-0002a810: 6573 7461 6d70 2069 7320 6570 6f63 6820  estamp is epoch 
-0002a820: 696e 2073 6563 6f6e 6473 2e20 4465 6661  in seconds. Defa
-0002a830: 756c 7420 6973 2063 7572 7265 6e74 0a20  ult is current. 
-0002a840: 2020 2020 2020 2020 2020 2020 2020 2055                 U
-0002a850: 5443 2074 696d 6573 7461 6d70 206d 696e  TC timestamp min
-0002a860: 7573 2033 2068 6f75 7273 0a20 2020 2020  us 3 hours.     
-0002a870: 2020 2020 2020 2074 6f5f 7469 6d65 7374         to_timest
-0002a880: 616d 7020 2869 6e74 2c20 6f70 7469 6f6e  amp (int, option
-0002a890: 616c 293a 2054 6869 7320 7061 7261 6d65  al): This parame
-0002a8a0: 7465 7220 7375 7065 7263 6564 6573 2065  ter supercedes e
-0002a8b0: 6e64 2070 6172 616d 6574 6572 2e20 4e65  nd parameter. Ne
-0002a8c0: 6564 2069 6e66 6f72 6d61 7469 6f6e 0a20  ed information. 
-0002a8d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0002a8e0: 6f20 7468 6973 2074 696d 6573 7461 6d70  o this timestamp
-0002a8f0: 2e20 5469 6d65 7374 616d 7020 6973 2065  . Timestamp is e
-0002a900: 706f 6368 2069 6e20 7365 636f 6e64 732e  poch in seconds.
-0002a910: 2044 6566 6175 6c74 2069 7320 6375 7272   Default is curr
-0002a920: 656e 7420 5554 4320 7469 6d65 7374 616d  ent UTC timestam
-0002a930: 700a 2020 2020 2020 2020 2020 2020 6f66  p.            of
-0002a940: 6673 6574 2028 696e 742c 206f 7074 696f  fset (int, optio
-0002a950: 6e61 6c29 3a20 5061 6769 6e61 7469 6f6e  nal): Pagination
-0002a960: 206f 6666 7365 7420 2864 6566 6175 6c74   offset (default
-0002a970: 203d 2030 2920 4465 6661 756c 7473 2074   = 0) Defaults t
-0002a980: 6f20 302e 0a20 2020 2020 2020 2020 2020  o 0..           
-0002a990: 206c 696d 6974 2028 696e 742c 206f 7074   limit (int, opt
-0002a9a0: 696f 6e61 6c29 3a20 7061 6769 6e61 7469  ional): paginati
-0002a9b0: 6f6e 2073 697a 6520 2864 6566 6175 6c74  on size (default
-0002a9c0: 203d 2031 3030 2920 4465 6661 756c 7473   = 100) Defaults
-0002a9d0: 2074 6f20 3130 302e 0a0a 2020 2020 2020   to 100...      
-0002a9e0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0002a9f0: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
-0002aa00: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
-0002aa10: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
-0002aa20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0002aa30: 7572 6c20 3d20 222f 7261 7069 6473 2f76  url = "/rapids/v
-0002aa40: 312f 6e65 6967 6862 6f72 5f61 7073 220a  1/neighbor_aps".
-0002aa50: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-0002aa60: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-0002aa70: 2767 726f 7570 273a 2067 726f 7570 2c0a  'group': group,.
-0002aa80: 2020 2020 2020 2020 2020 2020 276c 6162              'lab
-0002aa90: 656c 273a 206c 6162 656c 2c0a 2020 2020  el': label,.    
-0002aaa0: 2020 2020 2020 2020 2773 6974 6527 3a20          'site': 
-0002aab0: 7369 7465 2c0a 2020 2020 2020 2020 2020  site,.          
-0002aac0: 2020 2773 7461 7274 273a 2073 7461 7274    'start': start
-0002aad0: 2c0a 2020 2020 2020 2020 2020 2020 2765  ,.            'e
-0002aae0: 6e64 273a 2065 6e64 2c0a 2020 2020 2020  nd': end,.      
-0002aaf0: 2020 2020 2020 2773 7761 726d 5f69 6427        'swarm_id'
-0002ab00: 3a20 7377 6172 6d5f 6964 2c0a 2020 2020  : swarm_id,.    
-0002ab10: 2020 2020 2020 2020 2766 726f 6d5f 7469          'from_ti
-0002ab20: 6d65 7374 616d 7027 3a20 6672 6f6d 5f74  mestamp': from_t
-0002ab30: 696d 6573 7461 6d70 2c0a 2020 2020 2020  imestamp,.      
-0002ab40: 2020 2020 2020 2774 6f5f 7469 6d65 7374        'to_timest
-0002ab50: 616d 7027 3a20 746f 5f74 696d 6573 7461  amp': to_timesta
-0002ab60: 6d70 2c0a 2020 2020 2020 2020 2020 2020  mp,.            
-0002ab70: 276f 6666 7365 7427 3a20 6f66 6673 6574  'offset': offset
-0002ab80: 2c0a 2020 2020 2020 2020 2020 2020 276c  ,.            'l
-0002ab90: 696d 6974 273a 206c 696d 6974 0a20 2020  imit': limit.   
-0002aba0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-0002abb0: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
-0002abc0: 662e 6765 7428 7572 6c2c 2070 6172 616d  f.get(url, param
-0002abd0: 733d 7061 7261 6d73 290a 0a20 2020 2061  s=params)..    a
-0002abe0: 7379 6e63 2064 6566 2077 6964 735f 6765  sync def wids_ge
-0002abf0: 745f 616c 6c28 0a20 2020 2020 2020 2073  t_all(.        s
-0002ac00: 656c 662c 0a20 2020 2020 2020 2067 726f  elf,.        gro
-0002ac10: 7570 3a20 4c69 7374 5b73 7472 5d20 3d20  up: List[str] = 
-0002ac20: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c61  None,.        la
-0002ac30: 6265 6c3a 204c 6973 745b 7374 725d 203d  bel: List[str] =
-0002ac40: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-0002ac50: 6974 653a 204c 6973 745b 7374 725d 203d  ite: List[str] =
-0002ac60: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-0002ac70: 7461 7274 3a20 696e 7420 3d20 4e6f 6e65  tart: int = None
-0002ac80: 2c0a 2020 2020 2020 2020 656e 643a 2069  ,.        end: i
-0002ac90: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-0002aca0: 2020 2073 7761 726d 5f69 643a 2073 7472     swarm_id: str
-0002acb0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0002acc0: 2066 726f 6d5f 7469 6d65 7374 616d 703a   from_timestamp:
-0002acd0: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-0002ace0: 2020 2020 2074 6f5f 7469 6d65 7374 616d       to_timestam
-0002acf0: 703a 2069 6e74 203d 204e 6f6e 652c 0a20  p: int = None,. 
-0002ad00: 2020 2020 2020 206f 6666 7365 743a 2069         offset: i
-0002ad10: 6e74 203d 2030 2c0a 2020 2020 2020 2020  nt = 0,.        
-0002ad20: 6c69 6d69 743a 2069 6e74 203d 2031 3030  limit: int = 100
-0002ad30: 0a20 2020 2029 202d 3e20 5265 7370 6f6e  .    ) -> Respon
-0002ad40: 7365 3a0a 2020 2020 2020 2020 2222 224c  se:.        """L
-0002ad50: 6973 7420 616c 6c20 7769 6473 2063 6c61  ist all wids cla
-0002ad60: 7373 6966 6963 6174 696f 6e73 2e0a 0a20  ssifications... 
-0002ad70: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0002ad80: 2020 2020 2020 2020 2067 726f 7570 2028           group (
-0002ad90: 4c69 7374 5b73 7472 5d2c 206f 7074 696f  List[str], optio
-0002ada0: 6e61 6c29 3a20 4c69 7374 206f 6620 6772  nal): List of gr
-0002adb0: 6f75 7020 6e61 6d65 730a 2020 2020 2020  oup names.      
-0002adc0: 2020 2020 2020 6c61 6265 6c20 284c 6973        label (Lis
-0002add0: 745b 7374 725d 2c20 6f70 7469 6f6e 616c  t[str], optional
-0002ade0: 293a 204c 6973 7420 6f66 206c 6162 656c  ): List of label
-0002adf0: 206e 616d 6573 0a20 2020 2020 2020 2020   names.         
-0002ae00: 2020 2073 6974 6520 284c 6973 745b 7374     site (List[st
-0002ae10: 725d 2c20 6f70 7469 6f6e 616c 293a 204c  r], optional): L
-0002ae20: 6973 7420 6f66 2073 6974 6520 6e61 6d65  ist of site name
-0002ae30: 730a 2020 2020 2020 2020 2020 2020 7374  s.            st
-0002ae40: 6172 7420 2869 6e74 2c20 6f70 7469 6f6e  art (int, option
-0002ae50: 616c 293a 204e 6565 6420 696e 666f 726d  al): Need inform
-0002ae60: 6174 696f 6e20 6672 6f6d 2074 6869 7320  ation from this 
-0002ae70: 7469 6d65 7374 616d 702e 2054 696d 6573  timestamp. Times
-0002ae80: 7461 6d70 2069 7320 6570 6f63 6820 696e  tamp is epoch in
-0002ae90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002aea0: 206d 696c 6c69 7365 636f 6e64 732e 2044   milliseconds. D
-0002aeb0: 6566 6175 6c74 2069 7320 6375 7272 656e  efault is curren
-0002aec0: 7420 7469 6d65 7374 616d 7020 6d69 6e75  t timestamp minu
-0002aed0: 7320 3320 686f 7572 730a 2020 2020 2020  s 3 hours.      
-0002aee0: 2020 2020 2020 656e 6420 2869 6e74 2c20        end (int, 
-0002aef0: 6f70 7469 6f6e 616c 293a 204e 6565 6420  optional): Need 
-0002af00: 696e 666f 726d 6174 696f 6e20 746f 2074  information to t
-0002af10: 6869 7320 7469 6d65 7374 616d 702e 2054  his timestamp. T
-0002af20: 696d 6573 7461 6d70 2069 7320 6570 6f63  imestamp is epoc
-0002af30: 6820 696e 0a20 2020 2020 2020 2020 2020  h in.           
-0002af40: 2020 2020 206d 696c 6c69 7365 636f 6e64       millisecond
-0002af50: 732e 2044 6566 6175 6c74 2069 7320 6375  s. Default is cu
-0002af60: 7272 656e 7420 7469 6d65 7374 616d 700a  rrent timestamp.
-0002af70: 2020 2020 2020 2020 2020 2020 7377 6172              swar
-0002af80: 6d5f 6964 2028 7374 722c 206f 7074 696f  m_id (str, optio
-0002af90: 6e61 6c29 3a20 4669 6c74 6572 2062 7920  nal): Filter by 
-0002afa0: 5377 6172 6d20 4944 0a20 2020 2020 2020  Swarm ID.       
-0002afb0: 2020 2020 2066 726f 6d5f 7469 6d65 7374       from_timest
-0002afc0: 616d 7020 2869 6e74 2c20 6f70 7469 6f6e  amp (int, option
-0002afd0: 616c 293a 2054 6869 7320 7061 7261 6d65  al): This parame
-0002afe0: 7465 7220 7375 7065 7263 6564 6573 2073  ter supercedes s
-0002aff0: 7461 7274 2070 6172 616d 6574 6572 2e20  tart parameter. 
-0002b000: 4e65 6564 0a20 2020 2020 2020 2020 2020  Need.           
-0002b010: 2020 2020 2069 6e66 6f72 6d61 7469 6f6e       information
-0002b020: 2066 726f 6d20 7468 6973 2074 696d 6573   from this times
-0002b030: 7461 6d70 2e20 5469 6d65 7374 616d 7020  tamp. Timestamp 
-0002b040: 6973 2065 706f 6368 2069 6e20 7365 636f  is epoch in seco
-0002b050: 6e64 732e 2044 6566 6175 6c74 2069 7320  nds. Default is 
-0002b060: 6375 7272 656e 740a 2020 2020 2020 2020  current.        
-0002b070: 2020 2020 2020 2020 5554 4320 7469 6d65          UTC time
-0002b080: 7374 616d 7020 6d69 6e75 7320 3320 686f  stamp minus 3 ho
-0002b090: 7572 730a 2020 2020 2020 2020 2020 2020  urs.            
-0002b0a0: 746f 5f74 696d 6573 7461 6d70 2028 696e  to_timestamp (in
-0002b0b0: 742c 206f 7074 696f 6e61 6c29 3a20 5468  t, optional): Th
-0002b0c0: 6973 2070 6172 616d 6574 6572 2073 7570  is parameter sup
-0002b0d0: 6572 6365 6465 7320 656e 6420 7061 7261  ercedes end para
-0002b0e0: 6d65 7465 722e 204e 6565 6420 696e 666f  meter. Need info
-0002b0f0: 726d 6174 696f 6e0a 2020 2020 2020 2020  rmation.        
-0002b100: 2020 2020 2020 2020 746f 2074 6869 7320          to this 
-0002b110: 7469 6d65 7374 616d 702e 2054 696d 6573  timestamp. Times
-0002b120: 7461 6d70 2069 7320 6570 6f63 6820 696e  tamp is epoch in
-0002b130: 2073 6563 6f6e 6473 2e20 4465 6661 756c   seconds. Defaul
-0002b140: 7420 6973 2063 7572 7265 6e74 2055 5443  t is current UTC
-0002b150: 2074 696d 6573 7461 6d70 0a20 2020 2020   timestamp.     
-0002b160: 2020 2020 2020 206f 6666 7365 7420 2869         offset (i
-0002b170: 6e74 2c20 6f70 7469 6f6e 616c 293a 2050  nt, optional): P
-0002b180: 6167 696e 6174 696f 6e20 6f66 6673 6574  agination offset
-0002b190: 2028 6465 6661 756c 7420 3d20 3029 2044   (default = 0) D
-0002b1a0: 6566 6175 6c74 7320 746f 2030 2e0a 2020  efaults to 0..  
-0002b1b0: 2020 2020 2020 2020 2020 6c69 6d69 7420            limit 
-0002b1c0: 2869 6e74 2c20 6f70 7469 6f6e 616c 293a  (int, optional):
-0002b1d0: 2070 6167 696e 6174 696f 6e20 7369 7a65   pagination size
-0002b1e0: 2028 6465 6661 756c 7420 3d20 3130 3029   (default = 100)
-0002b1f0: 2044 6566 6175 6c74 7320 746f 2031 3030   Defaults to 100
-0002b200: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0002b210: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-0002b220: 5265 7370 6f6e 7365 3a20 4365 6e74 7261  Response: Centra
-0002b230: 6c41 5049 2052 6573 706f 6e73 6520 6f62  lAPI Response ob
-0002b240: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
-0002b250: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-0002b260: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-0002b270: 2767 726f 7570 273a 2067 726f 7570 2c0a  'group': group,.
-0002b280: 2020 2020 2020 2020 2020 2020 276c 6162              'lab
-0002b290: 656c 273a 206c 6162 656c 2c0a 2020 2020  el': label,.    
-0002b2a0: 2020 2020 2020 2020 2773 6974 6527 3a20          'site': 
-0002b2b0: 7369 7465 2c0a 2020 2020 2020 2020 2020  site,.          
-0002b2c0: 2020 2773 7461 7274 273a 2073 7461 7274    'start': start
-0002b2d0: 2c0a 2020 2020 2020 2020 2020 2020 2765  ,.            'e
-0002b2e0: 6e64 273a 2065 6e64 2c0a 2020 2020 2020  nd': end,.      
-0002b2f0: 2020 2020 2020 2773 7761 726d 5f69 6427        'swarm_id'
-0002b300: 3a20 7377 6172 6d5f 6964 2c0a 2020 2020  : swarm_id,.    
-0002b310: 2020 2020 2020 2020 2766 726f 6d5f 7469          'from_ti
-0002b320: 6d65 7374 616d 7027 3a20 6672 6f6d 5f74  mestamp': from_t
-0002b330: 696d 6573 7461 6d70 2c0a 2020 2020 2020  imestamp,.      
-0002b340: 2020 2020 2020 2774 6f5f 7469 6d65 7374        'to_timest
-0002b350: 616d 7027 3a20 746f 5f74 696d 6573 7461  amp': to_timesta
-0002b360: 6d70 2c0a 2020 2020 2020 2020 2020 2020  mp,.            
-0002b370: 276f 6666 7365 7427 3a20 6f66 6673 6574  'offset': offset
-0002b380: 2c0a 2020 2020 2020 2020 2020 2020 276c  ,.            'l
-0002b390: 696d 6974 273a 206c 696d 6974 0a20 2020  imit': limit.   
-0002b3a0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-0002b3b0: 6272 203d 2073 656c 662e 4261 7463 6852  br = self.BatchR
-0002b3c0: 6571 7565 7374 0a20 2020 2020 2020 2066  equest.        f
-0002b3d0: 756e 6373 203d 205b 0a20 2020 2020 2020  uncs = [.       
-0002b3e0: 2020 2020 2073 656c 662e 7769 6473 5f67       self.wids_g
-0002b3f0: 6574 5f69 6e74 6572 6665 7269 6e67 5f61  et_interfering_a
-0002b400: 7073 2c0a 2020 2020 2020 2020 2020 2020  ps,.            
-0002b410: 7365 6c66 2e77 6964 735f 6765 745f 6e65  self.wids_get_ne
-0002b420: 6967 6862 6f72 5f61 7073 2c0a 2020 2020  ighbor_aps,.    
-0002b430: 2020 2020 2020 2020 7365 6c66 2e77 6964          self.wid
-0002b440: 735f 6765 745f 7375 7370 6563 745f 6170  s_get_suspect_ap
-0002b450: 732c 0a20 2020 2020 2020 2020 2020 2073  s,.            s
-0002b460: 656c 662e 7769 6473 5f67 6574 5f72 6f67  elf.wids_get_rog
-0002b470: 7565 5f61 7073 2c0a 2020 2020 2020 2020  ue_aps,.        
-0002b480: 5d0a 0a20 2020 2020 2020 2062 6174 6368  ]..        batch
-0002b490: 5f72 6571 203d 205b 0a20 2020 2020 2020  _req = [.       
-0002b4a0: 2020 2020 2062 7228 662c 202a 2a70 6172       br(f, **par
-0002b4b0: 616d 7329 2066 6f72 2066 2069 6e20 6675  ams) for f in fu
-0002b4c0: 6e63 730a 2020 2020 2020 2020 5d0a 0a20  ncs.        ].. 
-0002b4d0: 2020 2020 2020 2062 6174 6368 5f72 6573         batch_res
-0002b4e0: 203d 2061 7761 6974 2073 656c 662e 5f62   = await self._b
-0002b4f0: 6174 6368 5f72 6571 7565 7374 2862 6174  atch_request(bat
-0002b500: 6368 5f72 6571 290a 2020 2020 2020 2020  ch_req).        
-0002b510: 7265 7370 203d 2062 6174 6368 5f72 6573  resp = batch_res
-0002b520: 5b2d 315d 0a20 2020 2020 2020 206f 6b5f  [-1].        ok_
-0002b530: 7265 7320 3d20 5b69 6478 2066 6f72 2069  res = [idx for i
-0002b540: 6478 2c20 7265 7320 696e 2065 6e75 6d65  dx, res in enume
-0002b550: 7261 7465 2862 6174 6368 5f72 6573 2920  rate(batch_res) 
-0002b560: 6966 2072 6573 2e6f 6b5d 0a20 2020 2020  if res.ok].     
-0002b570: 2020 2069 6620 6e6f 7420 6c65 6e28 6f6b     if not len(ok
-0002b580: 5f72 6573 2920 3d3d 206c 656e 2866 756e  _res) == len(fun
-0002b590: 6373 293a 0a20 2020 2020 2020 2020 2020  cs):.           
-0002b5a0: 2066 6169 6c65 6420 3d20 5b78 2066 6f72   failed = [x for
-0002b5b0: 2078 2069 6e20 7261 6e67 6528 302c 206c   x in range(0, l
-0002b5c0: 656e 2866 756e 6373 2929 2069 6620 7820  en(funcs)) if x 
-0002b5d0: 6e6f 7420 696e 206f 6b5f 7265 735d 0a20  not in ok_res]. 
-0002b5e0: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
-0002b5f0: 2069 6e20 6661 696c 6564 3a0a 2020 2020   in failed:.    
-0002b600: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-0002b610: 2069 6e20 7261 6e67 6528 302c 206c 656e   in range(0, len
-0002b620: 2862 6174 6368 5f72 6573 2929 3a0a 2020  (batch_res)):.  
-0002b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b640: 2020 6c6f 672e 6572 726f 7228 6622 7b62    log.error(f"{b
-0002b650: 6174 6368 5f72 6573 5b66 5d2e 6d65 7468  atch_res[f].meth
-0002b660: 6f64 7d20 7b62 6174 6368 5f72 6573 5b66  od} {batch_res[f
-0002b670: 5d2e 7572 6c2e 7061 7468 7d20 5265 7475  ].url.path} Retu
-0002b680: 726e 6564 2045 7272 6f72 2053 7461 7475  rned Error Statu
-0002b690: 7320 7b62 6174 6368 5f72 6573 5b66 5d2e  s {batch_res[f].
-0002b6a0: 7374 6174 7573 7d2e 207b 6261 7463 685f  status}. {batch_
-0002b6b0: 7265 735b 665d 2e6f 7574 7075 7420 6f72  res[f].output or
-0002b6c0: 2062 6174 6368 5f72 6573 5b66 5d2e 6572   batch_res[f].er
-0002b6d0: 726f 727d 222c 2073 686f 773d 5472 7565  ror}", show=True
-0002b6e0: 290a 2020 2020 2020 2020 7261 775f 6b65  ).        raw_ke
-0002b6f0: 7973 203d 205b 2269 6e74 6572 6665 7269  ys = ["interferi
-0002b700: 6e67 5f61 7073 222c 2022 6e65 6967 6862  ng_aps", "neighb
-0002b710: 6f72 5f61 7073 222c 2022 7375 7370 6563  or_aps", "suspec
-0002b720: 745f 6170 7322 5d0a 2020 2020 2020 2020  t_aps"].        
-0002b730: 7265 7370 2e72 6177 203d 207b 2272 6f67  resp.raw = {"rog
-0002b740: 7565 5f61 7073 223a 2072 6573 702e 7261  ue_aps": resp.ra
-0002b750: 772e 6765 7428 2272 6f67 7565 5f61 7073  w.get("rogue_aps
-0002b760: 222c 205b 5d29 2c20 225f 636f 756e 7473  ", []), "_counts
-0002b770: 223a 207b 2272 6f67 7565 7322 3a20 7265  ": {"rogues": re
-0002b780: 7370 2e72 6177 2e67 6574 2822 746f 7461  sp.raw.get("tota
-0002b790: 6c22 297d 7d0a 2020 2020 2020 2020 666f  l")}}.        fo
-0002b7a0: 7220 6964 782c 206b 6579 2069 6e20 656e  r idx, key in en
-0002b7b0: 756d 6572 6174 6528 7261 775f 6b65 7973  umerate(raw_keys
-0002b7c0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-0002b7d0: 6620 6964 7820 696e 206f 6b5f 7265 733a  f idx in ok_res:
-0002b7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b7f0: 2072 6573 702e 7261 7720 3d20 7b2a 2a72   resp.raw = {**r
-0002b800: 6573 702e 7261 772c 202a 2a7b 6b65 793a  esp.raw, **{key:
-0002b810: 2062 6174 6368 5f72 6573 5b69 6478 5d2e   batch_res[idx].
-0002b820: 7261 772e 6765 7428 6b65 792c 205b 5d29  raw.get(key, [])
-0002b830: 7d7d 0a20 2020 2020 2020 2020 2020 2020  }}.             
-0002b840: 2020 2072 6573 702e 7261 775b 225f 636f     resp.raw["_co
-0002b850: 756e 7473 225d 5b6b 6579 2e72 7374 7269  unts"][key.rstri
-0002b860: 7028 225f 6170 7322 295d 203d 2062 6174  p("_aps")] = bat
-0002b870: 6368 5f72 6573 5b69 6478 5d2e 7261 772e  ch_res[idx].raw.
-0002b880: 6765 7428 2274 6f74 616c 2229 0a20 2020  get("total").   
-0002b890: 2020 2020 2020 2020 2020 2020 2072 6573               res
-0002b8a0: 702e 6f75 7470 7574 203d 205b 2a72 6573  p.output = [*res
-0002b8b0: 702e 6f75 7470 7574 2c20 2a62 6174 6368  p.output, *batch
-0002b8c0: 5f72 6573 5b69 6478 5d2e 6f75 7470 7574  _res[idx].output
-0002b8d0: 5d0a 2020 2020 2020 2020 2320 7265 7370  ].        # resp
-0002b8e0: 2e6f 7574 7075 7420 3d20 5b2a 7265 7370  .output = [*resp
-0002b8f0: 2e6f 7574 7075 742c 202a 6261 7463 685f  .output, *batch_
-0002b900: 7265 735b 305d 2e6f 7574 7075 742c 202a  res[0].output, *
-0002b910: 6261 7463 685f 7265 735b 315d 2e6f 7574  batch_res[1].out
-0002b920: 7075 742c 202a 6261 7463 685f 7265 735b  put, *batch_res[
-0002b930: 325d 2e6f 7574 7075 745d 0a20 2020 2020  2].output].     
-0002b940: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0002b950: 2020 2020 7265 7370 2e6f 7574 7075 7420      resp.output 
-0002b960: 3d20 5b6d 6f64 656c 732e 5749 4453 282a  = [models.WIDS(*
-0002b970: 2a64 292e 6469 6374 2829 2066 6f72 2064  *d).dict() for d
-0002b980: 2069 6e20 7265 7370 2e6f 7574 7075 745d   in resp.output]
-0002b990: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-0002b9a0: 4578 6365 7074 696f 6e20 6173 2065 3a0a  Exception as e:.
-0002b9b0: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
-0002b9c0: 7761 726e 696e 6728 6622 6465 7620 6e6f  warning(f"dev no
-0002b9d0: 7465 2e20 7079 6461 6e74 6963 2063 6f6e  te. pydantic con
-0002b9e0: 7665 7273 696f 6e20 6469 6420 6e6f 7420  version did not 
-0002b9f0: 776f 726b 5c6e 7b65 7d22 2c20 7368 6f77  work\n{e}", show
-0002ba00: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
-0002ba10: 7265 7475 726e 2072 6573 700a 0a0a 2020  return resp...  
-0002ba20: 2020 6173 796e 6320 6465 6620 6765 745f    async def get_
-0002ba30: 616c 6572 7473 280a 2020 2020 2020 2020  alerts(.        
-0002ba40: 7365 6c66 2c0a 2020 2020 2020 2020 6375  self,.        cu
-0002ba50: 7374 6f6d 6572 5f69 643a 2073 7472 203d  stomer_id: str =
-0002ba60: 204e 6f6e 652c 0a20 2020 2020 2020 2067   None,.        g
-0002ba70: 726f 7570 3a20 7374 7220 3d20 4e6f 6e65  roup: str = None
-0002ba80: 2c0a 2020 2020 2020 2020 6c61 6265 6c3a  ,.        label:
-0002ba90: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0002baa0: 2020 2020 2073 6572 6961 6c3a 2073 7472       serial: str
-0002bab0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0002bac0: 2073 6974 653a 2073 7472 203d 204e 6f6e   site: str = Non
-0002bad0: 652c 0a20 2020 2020 2020 2066 726f 6d5f  e,.        from_
-0002bae0: 7473 3a20 696e 7420 3d20 4e6f 6e65 2c0a  ts: int = None,.
-0002baf0: 2020 2020 2020 2020 746f 5f74 733a 2069          to_ts: i
-0002bb00: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-0002bb10: 2020 2073 6576 6572 6974 793a 2073 7472     severity: str
-0002bb20: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0002bb30: 2074 7970 653a 2073 7472 203d 204e 6f6e   type: str = Non
-0002bb40: 652c 0a20 2020 2020 2020 2073 6561 7263  e,.        searc
-0002bb50: 683a 2073 7472 203d 204e 6f6e 652c 0a20  h: str = None,. 
-0002bb60: 2020 2020 2020 2023 2063 616c 6375 6c61         # calcula
-0002bb70: 7465 5f74 6f74 616c 3a20 626f 6f6c 203d  te_total: bool =
-0002bb80: 2046 616c 7365 2c20 2023 2044 6f65 736e   False,  # Doesn
-0002bb90: 2774 2061 7070 6561 7220 746f 2069 6d70  't appear to imp
-0002bba0: 6163 7420 616c 7761 7973 2072 6574 7572  act always retur
-0002bbb0: 6e73 2074 6f74 616c 0a20 2020 2020 2020  ns total.       
-0002bbc0: 2061 636b 3a20 626f 6f6c 203d 204e 6f6e   ack: bool = Non
-0002bbd0: 652c 0a20 2020 2020 2020 2066 6965 6c64  e,.        field
-0002bbe0: 733a 2073 7472 203d 204e 6f6e 652c 0a20  s: str = None,. 
-0002bbf0: 2020 2020 2020 206f 6666 7365 743a 2069         offset: i
-0002bc00: 6e74 203d 2030 2c0a 2020 2020 2020 2020  nt = 0,.        
-0002bc10: 6c69 6d69 743a 2069 6e74 203d 2031 3030  limit: int = 100
-0002bc20: 302c 0a20 2020 2029 202d 3e20 5265 7370  0,.    ) -> Resp
-0002bc30: 6f6e 7365 3a0a 2020 2020 2020 2020 2222  onse:.        ""
-0002bc40: 225b 6365 6e74 7261 6c5d 204c 6973 7420  "[central] List 
-0002bc50: 4e6f 7469 6669 6361 7469 6f6e 732f 416c  Notifications/Al
-0002bc60: 6572 7473 2e20 2052 6574 7572 6e73 2031  erts.  Returns 1
-0002bc70: 2064 6179 2062 7920 6465 6661 756c 742e   day by default.
-0002bc80: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-0002bc90: 2020 2020 2020 2020 2020 2020 6375 7374              cust
-0002bca0: 6f6d 6572 5f69 6420 2873 7472 2c20 6f70  omer_id (str, op
-0002bcb0: 7469 6f6e 616c 293a 204d 5350 2075 7365  tional): MSP use
-0002bcc0: 7220 6361 6e20 6669 6c74 6572 206e 6f74  r can filter not
-0002bcd0: 6966 6963 6174 696f 6e73 2062 6173 6564  ifications based
-0002bce0: 206f 6e20 6375 7374 6f6d 6572 2069 640a   on customer id.
-0002bcf0: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
-0002bd00: 7020 2873 7472 2c20 6f70 7469 6f6e 616c  p (str, optional
-0002bd10: 293a 2055 7365 6420 746f 2066 696c 7465  ): Used to filte
-0002bd20: 7220 7468 6520 6e6f 7469 6669 6361 7469  r the notificati
-0002bd30: 6f6e 2074 7970 6573 2062 6173 6564 206f  on types based o
-0002bd40: 6e20 6772 6f75 7020 6e61 6d65 0a20 2020  n group name.   
-0002bd50: 2020 2020 2020 2020 206c 6162 656c 2028           label (
-0002bd60: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
-0002bd70: 5573 6564 2074 6f20 6669 6c74 6572 2074  Used to filter t
-0002bd80: 6865 206e 6f74 6966 6963 6174 696f 6e20  he notification 
-0002bd90: 7479 7065 7320 6261 7365 6420 6f6e 204c  types based on L
-0002bda0: 6162 656c 206e 616d 650a 2020 2020 2020  abel name.      
-0002bdb0: 2020 2020 2020 7365 7269 616c 2028 7374        serial (st
-0002bdc0: 722c 206f 7074 696f 6e61 6c29 3a20 5573  r, optional): Us
-0002bdd0: 6564 2074 6f20 6669 6c74 6572 2074 6865  ed to filter the
-0002bde0: 2072 6573 756c 7420 6261 7365 6420 6f6e   result based on
-0002bdf0: 2073 6572 6961 6c20 6e75 6d62 6572 206f   serial number o
-0002be00: 6620 7468 6520 6465 7669 6365 0a20 2020  f the device.   
-0002be10: 2020 2020 2020 2020 2073 6974 6520 2873           site (s
-0002be20: 7472 2c20 6f70 7469 6f6e 616c 293a 2055  tr, optional): U
-0002be30: 7365 6420 746f 2066 696c 7465 7220 7468  sed to filter th
-0002be40: 6520 6e6f 7469 6669 6361 7469 6f6e 2074  e notification t
-0002be50: 7970 6573 2062 6173 6564 206f 6e20 5369  ypes based on Si
-0002be60: 7465 206e 616d 650a 2020 2020 2020 2020  te name.        
-0002be70: 2020 2020 6672 6f6d 5f74 7320 2869 6e74      from_ts (int
-0002be80: 2c20 6f70 7469 6f6e 616c 293a 2031 2973  , optional): 1)s
-0002be90: 7461 7274 206f 6620 6475 7261 7469 6f6e  tart of duration
-0002bea0: 2077 6974 6869 6e20 7768 6963 6820 616c   within which al
-0002beb0: 6572 7473 2061 7265 2072 6169 7365 640a  erts are raised.
-0002bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bed0: 3229 6465 7363 7269 6265 6420 7573 696e  2)described usin
-0002bee0: 6720 556e 6978 2045 706f 6368 2074 696d  g Unix Epoch tim
-0002bef0: 6520 696e 2073 6563 6f6e 6473 2020 4465  e in seconds  De
-0002bf00: 6661 756c 7420 3330 2064 6179 7320 286d  fault 30 days (m
-0002bf10: 6178 2039 3029 0a20 2020 2020 2020 2020  ax 90).         
-0002bf20: 2020 2074 6f5f 7473 2028 696e 742c 206f     to_ts (int, o
-0002bf30: 7074 696f 6e61 6c29 3a20 3129 656e 6420  ptional): 1)end 
-0002bf40: 6f66 2064 7572 6174 696f 6e20 7769 7468  of duration with
-0002bf50: 696e 2077 6869 6368 2061 6c65 7274 7320  in which alerts 
-0002bf60: 6172 6520 7261 6973 6564 0a20 2020 2020  are raised.     
-0002bf70: 2020 2020 2020 2020 2020 2032 2964 6573             2)des
-0002bf80: 6372 6962 6564 2075 7369 6e67 2055 6e69  cribed using Uni
-0002bf90: 7820 4570 6f63 6820 7469 6d65 2069 6e20  x Epoch time in 
-0002bfa0: 7365 636f 6e64 730a 2020 2020 2020 2020  seconds.        
-0002bfb0: 2020 2020 7365 7665 7269 7479 2028 7374      severity (st
-0002bfc0: 722c 206f 7074 696f 6e61 6c29 3a20 5573  r, optional): Us
-0002bfd0: 6564 2074 6f20 6669 6c74 6572 2074 6865  ed to filter the
-0002bfe0: 206e 6f74 6966 6963 6174 696f 6e20 7479   notification ty
-0002bff0: 7065 7320 6261 7365 6420 6f6e 2073 6576  pes based on sev
-0002c000: 6572 6974 790a 2020 2020 2020 2020 2020  erity.          
-0002c010: 2020 7479 7065 2028 7374 722c 206f 7074    type (str, opt
-0002c020: 696f 6e61 6c29 3a20 5573 6564 2074 6f20  ional): Used to 
-0002c030: 6669 6c74 6572 2074 6865 206e 6f74 6966  filter the notif
-0002c040: 6963 6174 696f 6e20 7479 7065 7320 6261  ication types ba
-0002c050: 7365 6420 6f6e 206e 6f74 6966 6963 6174  sed on notificat
-0002c060: 696f 6e20 7479 7065 0a20 2020 2020 2020  ion type.       
-0002c070: 2020 2020 2020 2020 206e 616d 650a 2020           name.  
-0002c080: 2020 2020 2020 2020 2020 7365 6172 6368            search
-0002c090: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-0002c0a0: 3a20 7465 726d 2075 7365 6420 746f 2073  : term used to s
-0002c0b0: 6561 7263 6820 696e 206e 616d 652c 2063  earch in name, c
-0002c0c0: 6174 6567 6f72 7920 6f66 2074 6865 2061  ategory of the a
-0002c0d0: 6c65 7274 0a20 2020 2020 2020 2020 2020  lert.           
-0002c0e0: 2063 616c 6375 6c61 7465 5f74 6f74 616c   calculate_total
-0002c0f0: 2028 626f 6f6c 2c20 6f70 7469 6f6e 616c   (bool, optional
-0002c100: 293a 2057 6865 7468 6572 2074 6f20 636f  ): Whether to co
-0002c110: 756e 7420 746f 7461 6c20 6974 656d 7320  unt total items 
-0002c120: 696e 2074 6865 2072 6573 706f 6e73 650a  in the response.
-0002c130: 2020 2020 2020 2020 2020 2020 6163 6b20              ack 
-0002c140: 2862 6f6f 6c2c 206f 7074 696f 6e61 6c29  (bool, optional)
-0002c150: 3a20 4669 6c74 6572 2061 636b 6e6f 776c  : Filter acknowl
-0002c160: 6564 6765 6420 6f72 2075 6e61 636b 6e6f  edged or unackno
-0002c170: 776c 6564 6765 6420 6e6f 7469 6669 6361  wledged notifica
-0002c180: 7469 6f6e 732e 2057 6865 6e20 7175 6572  tions. When quer
-0002c190: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-0002c1a0: 2020 7061 7261 6d65 7465 7220 6973 206e    parameter is n
-0002c1b0: 6f74 2073 7065 6369 6669 6564 2c20 626f  ot specified, bo
-0002c1c0: 7468 2061 636b 6e6f 776c 6564 6765 6420  th acknowledged 
-0002c1d0: 616e 6420 756e 6163 6b6e 6f77 6c65 6467  and unacknowledg
-0002c1e0: 6564 206e 6f74 6966 6963 6174 696f 6e73  ed notifications
-0002c1f0: 2061 7265 0a20 2020 2020 2020 2020 2020   are.           
-0002c200: 2020 2020 2069 6e63 6c75 6465 640a 2020       included.  
-0002c210: 2020 2020 2020 2020 2020 6669 656c 6473            fields
-0002c220: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-0002c230: 3a20 436f 6d6d 6120 7365 7061 7261 7465  : Comma separate
-0002c240: 6420 6c69 7374 206f 6620 6669 656c 6473  d list of fields
-0002c250: 2074 6f20 6265 2072 6574 7572 6e65 640a   to be returned.
-0002c260: 2020 2020 2020 2020 2020 2020 6f66 6673              offs
-0002c270: 6574 2028 696e 742c 206f 7074 696f 6e61  et (int, optiona
-0002c280: 6c29 3a20 5061 6769 6e61 7469 6f6e 206f  l): Pagination o
-0002c290: 6666 7365 7420 4465 6661 756c 7473 2074  ffset Defaults t
-0002c2a0: 6f20 302e 0a20 2020 2020 2020 2020 2020  o 0..           
-0002c2b0: 206c 696d 6974 2028 696e 742c 206f 7074   limit (int, opt
-0002c2c0: 696f 6e61 6c29 3a20 5061 6769 6e61 7469  ional): Paginati
-0002c2d0: 6f6e 206c 696d 6974 2e20 4465 6661 756c  on limit. Defaul
-0002c2e0: 7420 6973 2031 3030 2061 6e64 206d 6178  t is 100 and max
-0002c2f0: 2069 7320 3130 3030 2044 6566 6175 6c74   is 1000 Default
-0002c300: 7320 746f 2035 3030 2e0a 0a20 2020 2020  s to 500...     
-0002c310: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0002c320: 2020 2020 2020 2020 5265 7370 6f6e 7365          Response
-0002c330: 3a20 4365 6e74 7261 6c41 5049 2052 6573  : CentralAPI Res
-0002c340: 706f 6e73 6520 6f62 6a65 6374 0a20 2020  ponse object.   
-0002c350: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0002c360: 2075 726c 203d 2022 2f63 656e 7472 616c   url = "/central
-0002c370: 2f76 312f 6e6f 7469 6669 6361 7469 6f6e  /v1/notification
-0002c380: 7322 0a0a 2020 2020 2020 2020 6966 206e  s"..        if n
-0002c390: 6f74 2066 726f 6d5f 7473 3a0a 2020 2020  ot from_ts:.    
-0002c3a0: 2020 2020 2020 2020 6672 6f6d 5f74 7320          from_ts 
-0002c3b0: 3d20 696e 7428 6461 7465 7469 6d65 2e74  = int(datetime.t
-0002c3c0: 696d 6573 7461 6d70 2864 6174 6574 696d  imestamp(datetim
-0002c3d0: 652e 746f 6461 7928 2920 2d20 7469 6d65  e.today() - time
-0002c3e0: 6465 6c74 6128 6461 7973 3d31 2929 290a  delta(days=1))).
-0002c3f0: 2020 2020 2020 2020 6966 2061 636b 2069          if ack i
-0002c400: 6e20 5b54 7275 652c 2046 616c 7365 5d3a  n [True, False]:
-0002c410: 0a20 2020 2020 2020 2020 2020 2061 636b  .            ack
-0002c420: 203d 2073 7472 2861 636b 292e 6c6f 7765   = str(ack).lowe
-0002c430: 7228 290a 0a20 2020 2020 2020 2069 6620  r()..        if 
-0002c440: 746f 5f74 7320 616e 6420 746f 5f74 7320  to_ts and to_ts 
-0002c450: 3c3d 2066 726f 6d5f 7473 3a0a 2020 2020  <= from_ts:.    
-0002c460: 2020 2020 2020 2020 7265 7475 726e 2052          return R
-0002c470: 6573 706f 6e73 6528 6572 726f 723d 6622  esponse(error=f"
-0002c480: 546f 2074 696d 6573 7461 6d70 2028 7b74  To timestamp ({t
-0002c490: 6f5f 7473 7d29 2063 616e 206e 6f74 2062  o_ts}) can not b
-0002c4a0: 6520 6c65 7373 2074 6861 6e20 6672 6f6d  e less than from
-0002c4b0: 2074 696d 6573 7461 6d70 2028 7b66 726f   timestamp ({fro
-0002c4c0: 6d5f 7473 7d29 2229 0a0a 2020 2020 2020  m_ts})")..      
-0002c4d0: 2020 7061 7261 6d73 203d 207b 0a20 2020    params = {.   
-0002c4e0: 2020 2020 2020 2020 2027 6375 7374 6f6d           'custom
-0002c4f0: 6572 5f69 6427 3a20 6375 7374 6f6d 6572  er_id': customer
-0002c500: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-0002c510: 2027 6772 6f75 7027 3a20 6772 6f75 702c   'group': group,
-0002c520: 0a20 2020 2020 2020 2020 2020 2027 6c61  .            'la
-0002c530: 6265 6c27 3a20 6c61 6265 6c2c 0a20 2020  bel': label,.   
-0002c540: 2020 2020 2020 2020 2027 7365 7269 616c           'serial
-0002c550: 273a 2073 6572 6961 6c2c 0a20 2020 2020  ': serial,.     
-0002c560: 2020 2020 2020 2027 7369 7465 273a 2073         'site': s
-0002c570: 6974 652c 0a20 2020 2020 2020 2020 2020  ite,.           
-0002c580: 2027 6672 6f6d 5f74 696d 6573 7461 6d70   'from_timestamp
-0002c590: 273a 2066 726f 6d5f 7473 2c0a 2020 2020  ': from_ts,.    
-0002c5a0: 2020 2020 2020 2020 2774 6f5f 7469 6d65          'to_time
-0002c5b0: 7374 616d 7027 3a20 746f 5f74 732c 0a20  stamp': to_ts,. 
-0002c5c0: 2020 2020 2020 2020 2020 2027 7365 7665             'seve
-0002c5d0: 7269 7479 273a 2073 6576 6572 6974 792c  rity': severity,
-0002c5e0: 0a20 2020 2020 2020 2020 2020 2027 7365  .            'se
-0002c5f0: 6172 6368 273a 2073 6561 7263 682c 0a20  arch': search,. 
-0002c600: 2020 2020 2020 2020 2020 2023 2027 6361             # 'ca
-0002c610: 6c63 756c 6174 655f 746f 7461 6c27 3a20  lculate_total': 
-0002c620: 7374 7228 6361 6c63 756c 6174 655f 746f  str(calculate_to
-0002c630: 7461 6c29 2c0a 2020 2020 2020 2020 2020  tal),.          
-0002c640: 2020 2774 7970 6527 3a20 7479 7065 2c0a    'type': type,.
-0002c650: 2020 2020 2020 2020 2020 2020 2761 636b              'ack
-0002c660: 273a 2061 636b 2c0a 2020 2020 2020 2020  ': ack,.        
-0002c670: 2020 2020 2766 6965 6c64 7327 3a20 6669      'fields': fi
-0002c680: 656c 6473 2c0a 2020 2020 2020 2020 2020  elds,.          
-0002c690: 2020 276f 6666 7365 7427 3a20 6f66 6673    'offset': offs
-0002c6a0: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
-0002c6b0: 276c 696d 6974 273a 206c 696d 6974 2c0a  'limit': limit,.
-0002c6c0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-0002c6d0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-0002c6e0: 7365 6c66 2e67 6574 2875 726c 2c20 7061  self.get(url, pa
-0002c6f0: 7261 6d73 3d70 6172 616d 7329 0a0a 2020  rams=params)..  
-0002c700: 2020 6173 796e 6320 6465 6620 6365 6e74    async def cent
-0002c710: 7261 6c5f 6163 6b6e 6f77 6c65 6467 655f  ral_acknowledge_
-0002c720: 6e6f 7469 6669 6361 7469 6f6e 7328 0a20  notifications(. 
-0002c730: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0002c740: 2020 2020 204e 6f4e 616d 653a 204c 6973       NoName: Lis
-0002c750: 745b 7374 725d 203d 204e 6f6e 652c 0a20  t[str] = None,. 
-0002c760: 2020 2029 202d 3e20 5265 7370 6f6e 7365     ) -> Response
-0002c770: 3a0a 2020 2020 2020 2020 2222 2241 636b  :.        """Ack
-0002c780: 6e6f 776c 6564 6765 204e 6f74 6966 6963  nowledge Notific
-0002c790: 6174 696f 6e73 2062 7920 4944 204c 6973  ations by ID Lis
-0002c7a0: 7420 2f20 416c 6c2e 0a0a 2020 2020 2020  t / All...      
-0002c7b0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0002c7c0: 2020 2020 4e6f 4e61 6d65 2028 4c69 7374      NoName (List
-0002c7d0: 5b73 7472 5d2c 206f 7074 696f 6e61 6c29  [str], optional)
-0002c7e0: 3a20 4163 6b6e 6f77 6c65 6467 6520 6e6f  : Acknowledge no
-0002c7f0: 7469 6669 6361 7469 6f6e 730a 0a20 2020  tifications..   
-0002c800: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-0002c810: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
-0002c820: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
-0002c830: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
-0002c840: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0002c850: 2020 2075 726c 203d 2022 2f63 656e 7472     url = "/centr
-0002c860: 616c 2f76 312f 6e6f 7469 6669 6361 7469  al/v1/notificati
-0002c870: 6f6e 7322 0a0a 2020 2020 2020 2020 7265  ons"..        re
-0002c880: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
-0002c890: 706f 7374 2875 726c 290a 0a20 2020 2061  post(url)..    a
-0002c8a0: 7379 6e63 2064 6566 2063 656e 7472 616c  sync def central
-0002c8b0: 5f67 6574 5f6e 6f74 6966 6963 6174 696f  _get_notificatio
-0002c8c0: 6e5f 636f 6e66 6967 280a 2020 2020 2020  n_config(.      
-0002c8d0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0002c8e0: 7365 6172 6368 3a20 7374 7220 3d20 4e6f  search: str = No
-0002c8f0: 6e65 2c0a 2020 2020 2020 2020 736f 7274  ne,.        sort
-0002c900: 3a20 7374 7220 3d20 272d 6372 6561 7465  : str = '-create
-0002c910: 645f 7473 272c 0a20 2020 2020 2020 206f  d_ts',.        o
-0002c920: 6666 7365 743a 2069 6e74 203d 2030 2c0a  ffset: int = 0,.
-0002c930: 2020 2020 2020 2020 6c69 6d69 743a 2069          limit: i
-0002c940: 6e74 203d 2035 3030 2c0a 2020 2020 2920  nt = 500,.    ) 
-0002c950: 2d3e 2052 6573 706f 6e73 653a 0a20 2020  -> Response:.   
-0002c960: 2020 2020 2022 2222 4c69 7374 2043 6f6e       """List Con
-0002c970: 6669 6775 7261 7469 6f6e 2f53 6574 7469  figuration/Setti
-0002c980: 6e67 7320 666f 7220 616c 6572 7473 2074  ngs for alerts t
-0002c990: 6861 7420 7265 7375 6c74 2069 6e20 6e6f  hat result in no
-0002c9a0: 7469 6669 6361 7469 6f6e 2e0a 0a20 2020  tification...   
-0002c9b0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0002c9c0: 2020 2020 2020 2073 6561 7263 6820 2873         search (s
-0002c9d0: 7472 2c20 6f70 7469 6f6e 616c 293a 2074  tr, optional): t
-0002c9e0: 6572 6d20 7573 6564 2074 6f20 7365 6172  erm used to sear
-0002c9f0: 6368 2069 6e20 6e61 6d65 2c20 6361 7465  ch in name, cate
-0002ca00: 676f 7279 206f 6620 7468 6520 616c 6572  gory of the aler
-0002ca10: 740a 2020 2020 2020 2020 2020 2020 736f  t.            so
-0002ca20: 7274 2028 7374 722c 206f 7074 696f 6e61  rt (str, optiona
-0002ca30: 6c29 3a20 536f 7274 2070 6172 616d 6574  l): Sort paramet
-0002ca40: 6572 206d 6179 2062 6520 6f6e 6520 6f66  er may be one of
-0002ca50: 202b 6372 6561 7465 645f 7473 2c20 2d63   +created_ts, -c
-0002ca60: 7265 6174 6564 5f74 732c 2044 6566 6175  reated_ts, Defau
-0002ca70: 6c74 2069 730a 2020 2020 2020 2020 2020  lt is.          
-0002ca80: 2020 2020 2020 272d 6372 6561 7465 645f        '-created_
-0002ca90: 7473 2720 2056 616c 6964 2056 616c 7565  ts'  Valid Value
-0002caa0: 733a 202d 6372 6561 7465 645f 7473 2c20  s: -created_ts, 
-0002cab0: 2b63 7265 6174 6564 5f74 730a 2020 2020  +created_ts.    
-0002cac0: 2020 2020 2020 2020 6f66 6673 6574 2028          offset (
-0002cad0: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
-0002cae0: 5061 6769 6e61 7469 6f6e 206f 6666 7365  Pagination offse
-0002caf0: 7420 4465 6661 756c 7473 2074 6f20 302e  t Defaults to 0.
-0002cb00: 0a20 2020 2020 2020 2020 2020 206c 696d  .            lim
-0002cb10: 6974 2028 696e 742c 206f 7074 696f 6e61  it (int, optiona
-0002cb20: 6c29 3a20 5061 6769 6e61 7469 6f6e 206c  l): Pagination l
-0002cb30: 696d 6974 2e20 4465 6661 756c 7420 6973  imit. Default is
-0002cb40: 2031 3030 2061 6e64 206d 6178 2069 7320   100 and max is 
-0002cb50: 3130 3030 2044 6566 6175 6c74 7320 746f  1000 Defaults to
-0002cb60: 2031 3030 2e0a 0a20 2020 2020 2020 2052   100...        R
-0002cb70: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0002cb80: 2020 2020 5265 7370 6f6e 7365 3a20 4365      Response: Ce
-0002cb90: 6e74 7261 6c41 5049 2052 6573 706f 6e73  ntralAPI Respons
-0002cba0: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
-0002cbb0: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
-0002cbc0: 203d 2022 2f63 656e 7472 616c 2f76 312f   = "/central/v1/
-0002cbd0: 6e6f 7469 6669 6361 7469 6f6e 732f 7365  notifications/se
-0002cbe0: 7474 696e 6773 220a 0a20 2020 2020 2020  ttings"..       
-0002cbf0: 2070 6172 616d 7320 3d20 7b0a 2020 2020   params = {.    
-0002cc00: 2020 2020 2020 2020 2773 6561 7263 6827          'search'
-0002cc10: 3a20 7365 6172 6368 2c0a 2020 2020 2020  : search,.      
-0002cc20: 2020 2020 2020 2773 6f72 7427 3a20 736f        'sort': so
-0002cc30: 7274 2c0a 2020 2020 2020 2020 2020 2020  rt,.            
-0002cc40: 276f 6666 7365 7427 3a20 6f66 6673 6574  'offset': offset
-0002cc50: 2c0a 2020 2020 2020 2020 2020 2020 276c  ,.            'l
-0002cc60: 696d 6974 273a 206c 696d 6974 0a20 2020  imit': limit.   
-0002cc70: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-0002cc80: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
-0002cc90: 662e 6765 7428 7572 6c2c 2070 6172 616d  f.get(url, param
-0002cca0: 733d 7061 7261 6d73 290a 0a20 2020 2061  s=params)..    a
-0002ccb0: 7379 6e63 2064 6566 2067 6574 5f61 705f  sync def get_ap_
-0002ccc0: 636f 6e66 6967 280a 2020 2020 2020 2020  config(.        
-0002ccd0: 7365 6c66 2c0a 2020 2020 2020 2020 6772  self,.        gr
-0002cce0: 6f75 705f 7377 6172 6d69 643a 2073 7472  oup_swarmid: str
-0002ccf0: 2c0a 2020 2020 2020 2020 7665 7273 696f  ,.        versio
-0002cd00: 6e3a 2073 7472 203d 204e 6f6e 652c 0a20  n: str = None,. 
-0002cd10: 2020 2029 202d 3e20 5265 7370 6f6e 7365     ) -> Response
-0002cd20: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
-0002cd30: 2041 5020 4772 6f75 7020 4c65 7665 6c20   AP Group Level 
-0002cd40: 636f 6e66 6967 7572 6174 696f 6e20 666f  configuration fo
-0002cd50: 7220 5549 2067 726f 7570 2e0a 0a20 2020  r UI group...   
-0002cd60: 2020 2020 202f 2f20 5573 6564 2062 7920       // Used by 
-0002cd70: 7368 6f77 2063 6f6e 6669 6720 3c41 5020  show config <AP 
-0002cd80: 4d41 4320 666f 7220 414f 5331 3020 4150  MAC for AOS10 AP
-0002cd90: 3e20 2f2f 0a0a 2020 2020 2020 2020 4172  > //..        Ar
-0002cda0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0002cdb0: 6772 6f75 705f 7377 6172 6d69 6420 2873  group_swarmid (s
-0002cdc0: 7472 293a 2047 726f 7570 206e 616d 6520  tr): Group name 
-0002cdd0: 6f66 2074 6865 2067 726f 7570 206f 7220  of the group or 
-0002cde0: 6775 6964 206f 6620 7468 6520 7377 6172  guid of the swar
-0002cdf0: 6d2e 0a20 2020 2020 2020 2020 2020 2020  m..             
-0002ce00: 2020 2045 7861 6d70 6c65 3a47 726f 7570     Example:Group
-0002ce10: 5f31 206f 7220 3661 3564 3132 3362 3031  _1 or 6a5d123b01
-0002ce20: 6639 3434 3138 3036 3234 3465 6136 6530  f9441806244ea6e0
-0002ce30: 3233 6661 6235 3834 3162 3737 6338 3238  23fab5841b77c828
-0002ce40: 6130 3835 6630 3466 2e0a 2020 2020 2020  a085f04f..      
-0002ce50: 2020 2020 2020 7665 7273 696f 6e20 2873        version (s
-0002ce60: 7472 2c20 6f70 7469 6f6e 616c 293a 2056  tr, optional): V
-0002ce70: 6572 7369 6f6e 206f 6620 4150 2e0a 0a20  ersion of AP... 
-0002ce80: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0002ce90: 2020 2020 2020 2020 2020 2020 5265 7370              Resp
-0002cea0: 6f6e 7365 3a20 4365 6e74 7261 6c41 5049  onse: CentralAPI
-0002ceb0: 2052 6573 706f 6e73 6520 6f62 6a65 6374   Response object
-0002cec0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0002ced0: 2020 2020 2075 726c 203d 2066 222f 636f       url = f"/co
-0002cee0: 6e66 6967 7572 6174 696f 6e2f 7631 2f61  nfiguration/v1/a
-0002cef0: 705f 636c 692f 7b67 726f 7570 5f73 7761  p_cli/{group_swa
-0002cf00: 726d 6964 7d22 0a0a 2020 2020 2020 2020  rmid}"..        
-0002cf10: 7061 7261 6d73 203d 207b 0a20 2020 2020  params = {.     
-0002cf20: 2020 2020 2020 2027 7665 7273 696f 6e27         'version'
-0002cf30: 3a20 7665 7273 696f 6e0a 2020 2020 2020  : version.      
-0002cf40: 2020 7d0a 0a20 2020 2020 2020 2072 6574    }..        ret
-0002cf50: 7572 6e20 6177 6169 7420 7365 6c66 2e67  urn await self.g
-0002cf60: 6574 2875 726c 2c20 7061 7261 6d73 3d70  et(url, params=p
-0002cf70: 6172 616d 7329 0a0a 2020 2020 6173 796e  arams)..    asyn
-0002cf80: 6320 6465 6620 7265 706c 6163 655f 6170  c def replace_ap
-0002cf90: 5f63 6f6e 6669 6728 0a20 2020 2020 2020  _config(.       
-0002cfa0: 2073 656c 662c 0a20 2020 2020 2020 2067   self,.        g
-0002cfb0: 726f 7570 5f6e 616d 655f 6f72 5f67 7569  roup_name_or_gui
-0002cfc0: 643a 2073 7472 2c0a 2020 2020 2020 2020  d: str,.        
-0002cfd0: 636c 6973 3a20 4c69 7374 5b73 7472 5d2c  clis: List[str],
-0002cfe0: 0a20 2020 2029 202d 3e20 5265 7370 6f6e  .    ) -> Respon
-0002cff0: 7365 3a0a 2020 2020 2020 2020 2222 2252  se:.        """R
-0002d000: 6570 6c61 6365 2041 5020 4772 6f75 7020  eplace AP Group 
-0002d010: 4c65 7665 6c20 636f 6e66 6967 7572 6174  Level configurat
-0002d020: 696f 6e20 666f 7220 5549 2067 726f 7570  ion for UI group
-0002d030: 2e0a 0a20 2020 2020 2020 2053 656e 6420  ...        Send 
-0002d040: 4150 2063 6f6e 6669 6775 7261 7469 6f6e  AP configuration
-0002d050: 2069 6e20 434c 4920 666f 726d 6174 2061   in CLI format a
-0002d060: 7320 6120 6c69 7374 206f 6620 7374 7269  s a list of stri
-0002d070: 6e67 7320 7768 6572 6520 6561 6368 2069  ngs where each i
-0002d080: 7465 6d20 696e 2074 6865 206c 6973 7420  tem in the list 
-0002d090: 6973 0a20 2020 2020 2020 2061 206c 696e  is.        a lin
-0002d0a0: 6520 6672 6f6d 2074 6865 2063 6f6e 6669  e from the confi
-0002d0b0: 672e 2020 5265 7175 6972 6573 2061 6c6c  g.  Requires all
-0002d0c0: 206c 696e 6573 206f 6620 7468 6520 636f   lines of the co
-0002d0d0: 6e66 6967 2c20 6e6f 7420 6120 7061 7274  nfig, not a part
-0002d0e0: 6961 6c20 7570 6461 7465 2e0a 0a20 2020  ial update...   
-0002d0f0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0002d100: 2020 2020 2020 2067 726f 7570 5f6e 616d         group_nam
-0002d110: 655f 6f72 5f67 7569 6420 2873 7472 293a  e_or_guid (str):
-0002d120: 2047 726f 7570 206e 616d 6520 6f66 2074   Group name of t
-0002d130: 6865 2067 726f 7570 206f 7220 6775 6964  he group or guid
-0002d140: 206f 6620 7468 6520 7377 6172 6d2e 0a20   of the swarm.. 
-0002d150: 2020 2020 2020 2020 2020 2020 2020 2045                 E
-0002d160: 7861 6d70 6c65 3a47 726f 7570 5f31 206f  xample:Group_1 o
-0002d170: 7220 3661 3564 3132 3362 3031 6639 3434  r 6a5d123b01f944
-0002d180: 3138 3036 3234 3465 6136 6530 3233 6661  1806244ea6e023fa
-0002d190: 6235 3834 3162 3737 6338 3238 6130 3835  b5841b77c828a085
-0002d1a0: 6630 3466 2e0a 2020 2020 2020 2020 2020  f04f..          
-0002d1b0: 2020 636c 6973 2028 4c69 7374 5b73 7472    clis (List[str
-0002d1c0: 5d29 3a20 5768 6f6c 6520 636f 6e66 6967  ]): Whole config
-0002d1d0: 7572 6174 696f 6e20 4c69 7374 2069 6e20  uration List in 
-0002d1e0: 434c 4920 666f 726d 6174 2e0a 0a20 2020  CLI format...   
-0002d1f0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-0002d200: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
-0002d210: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
-0002d220: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
-0002d230: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0002d240: 2020 2075 726c 203d 2066 222f 636f 6e66     url = f"/conf
-0002d250: 6967 7572 6174 696f 6e2f 7631 2f61 705f  iguration/v1/ap_
-0002d260: 636c 692f 7b67 726f 7570 5f6e 616d 655f  cli/{group_name_
-0002d270: 6f72 5f67 7569 647d 220a 0a20 2020 2020  or_guid}"..     
-0002d280: 2020 206a 736f 6e5f 6461 7461 203d 207b     json_data = {
-0002d290: 0a20 2020 2020 2020 2020 2020 2027 636c  .            'cl
-0002d2a0: 6973 273a 2063 6c69 730a 2020 2020 2020  is': clis.      
-0002d2b0: 2020 7d0a 0a20 2020 2020 2020 2072 6574    }..        ret
-0002d2c0: 7572 6e20 6177 6169 7420 7365 6c66 2e70  urn await self.p
-0002d2d0: 6f73 7428 7572 6c2c 206a 736f 6e5f 6461  ost(url, json_da
-0002d2e0: 7461 3d6a 736f 6e5f 6461 7461 290a 0a20  ta=json_data).. 
-0002d2f0: 2020 2061 7379 6e63 2064 6566 2067 6574     async def get
-0002d300: 5f70 6572 5f61 705f 636f 6e66 6967 280a  _per_ap_config(.
-0002d310: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0002d320: 2020 2020 2020 7365 7269 616c 3a20 7374        serial: st
-0002d330: 722c 0a20 2020 2029 202d 3e20 5265 7370  r,.    ) -> Resp
-0002d340: 6f6e 7365 3a0a 2020 2020 2020 2020 2222  onse:.        ""
-0002d350: 2247 6574 2070 6572 2041 5020 7365 7474  "Get per AP sett
-0002d360: 696e 672e 0a0a 2020 2020 2020 2020 4172  ing...        Ar
-0002d370: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0002d380: 7365 7269 616c 2028 7374 7229 3a20 5365  serial (str): Se
-0002d390: 7269 616c 204e 756d 6265 7220 6f66 2041  rial Number of A
-0002d3a0: 500a 0a20 2020 2020 2020 2052 6574 7572  P..        Retur
-0002d3b0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-0002d3c0: 5265 7370 6f6e 7365 3a20 4365 6e74 7261  Response: Centra
-0002d3d0: 6c41 5049 2052 6573 706f 6e73 6520 6f62  lAPI Response ob
-0002d3e0: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
-0002d3f0: 0a20 2020 2020 2020 2075 726c 203d 2066  .        url = f
-0002d400: 222f 636f 6e66 6967 7572 6174 696f 6e2f  "/configuration/
-0002d410: 7631 2f61 705f 7365 7474 696e 6773 5f63  v1/ap_settings_c
-0002d420: 6c69 2f7b 7365 7269 616c 7d22 0a0a 2020  li/{serial}"..  
-0002d430: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-0002d440: 6974 2073 656c 662e 6765 7428 7572 6c29  it self.get(url)
-0002d450: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-0002d460: 7265 706c 6163 655f 7065 725f 6170 5f63  replace_per_ap_c
-0002d470: 6f6e 6669 6728 0a20 2020 2020 2020 2073  onfig(.        s
-0002d480: 656c 662c 0a20 2020 2020 2020 2073 6572  elf,.        ser
-0002d490: 6961 6c3a 2073 7472 2c0a 2020 2020 2020  ial: str,.      
-0002d4a0: 2020 636c 6973 3a20 4c69 7374 5b73 7472    clis: List[str
-0002d4b0: 5d2c 0a20 2020 2029 202d 3e20 5265 7370  ],.    ) -> Resp
-0002d4c0: 6f6e 7365 3a0a 2020 2020 2020 2020 2222  onse:.        ""
-0002d4d0: 2252 6570 6c61 6365 2070 6572 2041 5020  "Replace per AP 
-0002d4e0: 7365 7474 696e 672e 0a0a 2020 2020 2020  setting...      
-0002d4f0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0002d500: 2020 2020 7365 7269 616c 2028 7374 7229      serial (str)
-0002d510: 3a20 5365 7269 616c 204e 756d 6265 7220  : Serial Number 
-0002d520: 6f66 2041 500a 2020 2020 2020 2020 2020  of AP.          
-0002d530: 2020 636c 6973 2028 4c69 7374 5b73 7472    clis (List[str
-0002d540: 5d29 3a20 416c 6c20 7065 7220 4150 2073  ]): All per AP s
-0002d550: 6574 7469 6e67 204c 6973 7420 696e 2043  etting List in C
-0002d560: 4c49 2066 6f72 6d61 740a 2020 2020 2020  LI format.      
-0002d570: 2020 2020 2020 2020 2020 4d75 7374 2070            Must p
-0002d580: 726f 7669 6465 2061 6c6c 2070 6572 2041  rovide all per A
-0002d590: 5020 7365 7474 696e 6773 2c20 6e6f 7420  P settings, not 
-0002d5a0: 7061 7274 6961 6c0a 0a20 2020 2020 2020  partial..       
-0002d5b0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0002d5c0: 2020 2020 2020 5265 7370 6f6e 7365 3a20        Response: 
-0002d5d0: 4365 6e74 7261 6c41 5049 2052 6573 706f  CentralAPI Respo
-0002d5e0: 6e73 6520 6f62 6a65 6374 0a20 2020 2020  nse object.     
-0002d5f0: 2020 2022 2222 0a20 2020 2020 2020 2075     """.        u
-0002d600: 726c 203d 2066 222f 636f 6e66 6967 7572  rl = f"/configur
-0002d610: 6174 696f 6e2f 7631 2f61 705f 7365 7474  ation/v1/ap_sett
-0002d620: 696e 6773 5f63 6c69 2f7b 7365 7269 616c  ings_cli/{serial
-0002d630: 7d22 0a0a 2020 2020 2020 2020 6a73 6f6e  }"..        json
-0002d640: 5f64 6174 6120 3d20 7b0a 2020 2020 2020  _data = {.      
-0002d650: 2020 2020 2020 2763 6c69 7327 3a20 636c        'clis': cl
-0002d660: 6973 0a20 2020 2020 2020 207d 0a0a 2020  is.        }..  
-0002d670: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-0002d680: 6974 2073 656c 662e 706f 7374 2875 726c  it self.post(url
-0002d690: 2c20 6a73 6f6e 5f64 6174 613d 6a73 6f6e  , json_data=json
-0002d6a0: 5f64 6174 6129 0a0a 2020 2020 6173 796e  _data)..    asyn
-0002d6b0: 6320 6465 6620 6765 745f 6272 6163 685f  c def get_brach_
-0002d6c0: 6865 616c 7468 280a 2020 2020 2020 2020  health(.        
-0002d6d0: 7365 6c66 2c0a 2020 2020 2020 2020 6e61  self,.        na
-0002d6e0: 6d65 3a20 7374 7220 3d20 4e6f 6e65 2c0a  me: str = None,.
-0002d6f0: 2020 2020 2020 2020 636f 6c75 6d6e 3a20          column: 
-0002d700: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-0002d710: 2020 2020 7265 7665 7273 653a 2062 6f6f      reverse: boo
-0002d720: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
-0002d730: 2020 2066 696c 7465 7273 3a20 6469 6374     filters: dict
-0002d740: 203d 207b 7d2c 0a20 2020 2020 2020 206f   = {},.        o
-0002d750: 6666 7365 743a 2069 6e74 203d 2030 2c0a  ffset: int = 0,.
-0002d760: 2020 2020 2020 2020 6c69 6d69 743a 2069          limit: i
-0002d770: 6e74 203d 2031 3030 2c0a 2020 2020 2920  nt = 100,.    ) 
-0002d780: 2d3e 2052 6573 706f 6e73 653a 0a20 2020  -> Response:.   
-0002d790: 2020 2020 2022 2222 4765 7420 6461 7461       """Get data
-0002d7a0: 2066 6f72 2061 6c6c 2073 6974 6573 2e0a   for all sites..
-0002d7b0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0002d7c0: 2020 2020 2020 2020 2020 206e 616d 6520             name 
-0002d7d0: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
-0002d7e0: 2073 6974 6520 2f20 6c61 6265 6c20 6e61   site / label na
-0002d7f0: 6d65 206f 7220 7061 7274 206f 6620 6974  me or part of it
-0002d800: 7320 6e61 6d65 0a20 2020 2020 2020 2020  s name.         
-0002d810: 2020 2063 6f6c 756d 6e20 2869 6e74 2c20     column (int, 
-0002d820: 6f70 7469 6f6e 616c 293a 2043 6f6c 756d  optional): Colum
-0002d830: 6e20 746f 2073 6f72 7420 6f6e 0a20 2020  n to sort on.   
-0002d840: 2020 2020 2020 2020 2072 6576 6572 7365           reverse
-0002d850: 2028 626f 6f6c 2c20 6f70 7469 6f6e 616c   (bool, optional
-0002d860: 293a 2053 6f72 7420 696e 2072 6576 6572  ): Sort in rever
-0002d870: 7365 206f 7264 6572 3a0a 2020 2020 2020  se order:.      
-0002d880: 2020 2020 2020 2020 2020 5661 6c69 6420            Valid 
-0002d890: 5661 6c75 6573 3a20 6173 632c 2064 6573  Values: asc, des
-0002d8a0: 630a 2020 2020 2020 2020 2020 2020 2020  c.              
-0002d8b0: 2020 2a20 6173 6320 2d20 4173 6365 6e64    * asc - Ascend
-0002d8c0: 696e 672c 2066 726f 6d20 4120 746f 205a  ing, from A to Z
-0002d8d0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0002d8e0: 2020 2a20 6465 7363 202d 2044 6573 6365    * desc - Desce
-0002d8f0: 6e64 696e 672c 2066 726f 6d20 5a20 746f  nding, from Z to
-0002d900: 2041 2e0a 0a0a 2020 2020 2020 2020 2020   A....          
-0002d910: 2020 6669 6c74 6572 7320 2873 7472 2c20    filters (str, 
-0002d920: 6f70 7469 6f6e 616c 293a 2053 6974 6520  optional): Site 
-0002d930: 7468 7265 7368 6f6c 6473 0a20 2020 2020  thresholds.     
-0002d940: 2020 2020 2020 2020 2020 2056 616c 6964             Valid
-0002d950: 2056 616c 7565 733a 2067 7420 2028 4772   Values: gt  (Gr
-0002d960: 6561 7465 7220 7468 616e 292c 206c 7420  eater than), lt 
-0002d970: 2028 4c65 7373 2074 6861 6e29 2c20 6774   (Less than), gt
-0002d980: 6520 2847 7265 6174 6572 2074 6861 6e20  e (Greater than 
-0002d990: 6f72 2065 7175 616c 2074 6f29 2c0a 2020  or equal to),.  
-0002d9a0: 2020 2020 2020 2020 2020 2020 2020 6c74                lt
-0002d9b0: 6520 284c 6573 7320 7468 616e 206f 7220  e (Less than or 
-0002d9c0: 6571 7561 6c20 746f 290a 2020 2020 2020  equal to).      
-0002d9d0: 2020 2020 2020 2020 2020 2a20 416c 6c20            * All 
-0002d9e0: 7072 6f70 6572 7469 6573 206f 6620 6120  properties of a 
-0002d9f0: 7369 7465 2063 616e 2062 6520 7573 6564  site can be used
-0002da00: 2061 7320 6669 6c74 6572 2070 6172 616d   as filter param
-0002da10: 6574 6572 7320 7769 7468 2061 2074 6872  eters with a thr
-0002da20: 6573 686f 6c64 0a20 2020 2020 2020 2020  eshold.         
-0002da30: 2020 2020 2020 202a 2054 6865 2072 616e         * The ran
-0002da40: 6765 2066 696c 7465 7273 2063 616e 2062  ge filters can b
-0002da50: 6520 636f 6d62 696e 6564 2077 6974 6820  e combined with 
-0002da60: 7468 6520 636f 6c75 6d6e 206e 616d 6573  the column names
-0002da70: 2077 6974 6820 225c 5f5f 2220 2023 206e   with "\__"  # n
-0002da80: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
-0002da90: 2020 2020 2a20 466f 7220 6567 2e20 2f73      * For eg. /s
-0002daa0: 6974 653f 6465 7669 6365 5f64 6f77 6e5c  ite?device_down\
-0002dab0: 5f5f 6774 3d30 202d 204c 6973 7473 2061  __gt=0 - Lists a
-0002dac0: 6c6c 2073 6974 6573 2074 6861 7420 6861  ll sites that ha
-0002dad0: 7665 206d 6f72 6520 7468 616e 2031 2064  ve more than 1 d
-0002dae0: 6576 6963 6520 696e 2064 6f77 6e20 7374  evice in down st
-0002daf0: 6174 6520 2320 6e6f 7161 0a20 2020 2020  ate # noqa.     
-0002db00: 2020 2020 2020 2020 2020 202a 2046 6f72             * For
-0002db10: 2065 672e 202f 7369 7465 3f77 616e 5f75   eg. /site?wan_u
-0002db20: 706c 696e 6b73 5f64 6f77 6e5c 5f5f 6c74  plinks_down\__lt
-0002db30: 3d31 202d 204c 6973 7473 2061 6c6c 2073  =1 - Lists all s
-0002db40: 6974 6573 2074 6861 7420 6861 7665 206c  ites that have l
-0002db50: 6573 7320 7468 616e 2031 2077 616e 2069  ess than 1 wan i
-0002db60: 6e20 646f 776e 2073 7461 7465 2023 206e  n down state # n
-0002db70: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
-0002db80: 2020 2020 2a20 466f 7220 6567 2e20 2f73      * For eg. /s
-0002db90: 6974 653f 6465 7669 6365 5f75 705f 5f67  ite?device_up__g
-0002dba0: 743d 3126 6465 7669 6365 5f75 705c 5f5f  t=1&device_up\__
-0002dbb0: 6c74 3d31 3020 2d20 4c69 7374 7320 616c  lt=10 - Lists al
-0002dbc0: 6c20 7369 7465 7320 7468 6174 2068 6176  l sites that hav
-0002dbd0: 6520 312d 3130 2064 6576 6963 6573 2075  e 1-10 devices u
-0002dbe0: 7020 2320 6e6f 7161 0a0a 0a20 2020 2020  p # noqa...     
-0002dbf0: 2020 2020 2020 206f 6666 7365 7420 2869         offset (i
-0002dc00: 6e74 2c20 6f70 7469 6f6e 616c 293a 2070  nt, optional): p
-0002dc10: 6167 696e 6174 696f 6e20 7374 6172 7420  agination start 
-0002dc20: 696e 6465 7820 4465 6661 756c 7473 2074  index Defaults t
-0002dc30: 6f20 302e 0a20 2020 2020 2020 2020 2020  o 0..           
-0002dc40: 206c 696d 6974 2028 696e 742c 206f 7074   limit (int, opt
-0002dc50: 696f 6e61 6c29 3a20 7061 6769 6e61 7469  ional): paginati
-0002dc60: 6f6e 2073 697a 6520 4465 6661 756c 7473  on size Defaults
-0002dc70: 2074 6f20 3130 302e 0a0a 2020 2020 2020   to 100...      
-0002dc80: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0002dc90: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
-0002dca0: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
-0002dcb0: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
-0002dcc0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0002dcd0: 7572 6c20 3d20 222f 6272 616e 6368 6865  url = "/branchhe
-0002dce0: 616c 7468 2f76 312f 7369 7465 220a 0a20  alth/v1/site".. 
-0002dcf0: 2020 2020 2020 2070 6172 616d 7320 3d20         params = 
-0002dd00: 7b0a 2020 2020 2020 2020 2020 2020 226e  {.            "n
-0002dd10: 616d 6522 3a20 6e61 6d65 2c0a 2020 2020  ame": name,.    
-0002dd20: 2020 2020 2020 2020 2320 2263 6f6c 756d          # "colum
-0002dd30: 6e22 3a20 636f 6c75 6d6e 2c0a 2020 2020  n": column,.    
-0002dd40: 2020 2020 2020 2020 226f 7264 6572 223a          "order":
-0002dd50: 2022 6173 6322 2069 6620 6e6f 7420 7265   "asc" if not re
-0002dd60: 7665 7273 6520 656c 7365 2022 6465 7363  verse else "desc
-0002dd70: 222c 0a20 2020 2020 2020 2020 2020 2023  ",.            #
-0002dd80: 2022 7761 6e5f 7475 6e6e 656c 735f 646f   "wan_tunnels_do
-0002dd90: 776e 5c5f 5f67 7422 3a20 2230 222c 0a20  wn\__gt": "0",. 
-0002dda0: 2020 2020 2020 2020 2020 2023 2022 7761             # "wa
-0002ddb0: 6e5f 7570 6c69 6e6b 735f 646f 776e 5c5f  n_uplinks_down\_
-0002ddc0: 5f67 7422 3a20 2230 222c 0a20 2020 2020  _gt": "0",.     
-0002ddd0: 2020 2020 2020 2023 202a 2a66 696c 7465         # **filte
-0002dde0: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
-0002ddf0: 226f 6666 7365 7422 3a20 6f66 6673 6574  "offset": offset
-0002de00: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
-0002de10: 696d 6974 223a 206c 696d 6974 2c0a 2020  imit": limit,.  
-0002de20: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
-0002de30: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-0002de40: 6c66 2e67 6574 2875 726c 2c20 7061 7261  lf.get(url, para
-0002de50: 6d73 3d70 6172 616d 7329 0a0a 2020 2020  ms=params)..    
-0002de60: 6173 796e 6320 6465 6620 6765 745f 6172  async def get_ar
-0002de70: 6368 6976 6564 5f64 6576 6963 6573 280a  chived_devices(.
-0002de80: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0002de90: 2020 2020 2020 6f66 6673 6574 3a20 696e        offset: in
-0002dea0: 7420 3d20 302c 0a20 2020 2020 2020 206c  t = 0,.        l
-0002deb0: 696d 6974 3a20 696e 7420 3d20 3130 302c  imit: int = 100,
-0002dec0: 0a20 2020 2029 202d 3e20 5265 7370 6f6e  .    ) -> Respon
-0002ded0: 7365 3a0a 2020 2020 2020 2020 2222 2247  se:.        """G
-0002dee0: 6574 2041 7263 6869 7665 6420 6465 7669  et Archived devi
-0002def0: 6365 7320 6672 6f6d 2064 6576 6963 6520  ces from device 
-0002df00: 696e 7665 6e74 6f72 792e 0a0a 2020 2020  inventory...    
-0002df10: 2020 2020 2f2f 2055 7365 6420 6279 2073      // Used by s
-0002df20: 686f 7720 6172 6368 6976 6564 202f 2f0a  how archived //.
-0002df30: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0002df40: 2020 2020 2020 2020 2020 206f 6666 7365             offse
-0002df50: 7420 2869 6e74 2c20 6f70 7469 6f6e 616c  t (int, optional
-0002df60: 293a 206f 6666 7365 7420 6f72 2070 6167  ): offset or pag
-0002df70: 6520 6e75 6d62 6572 2044 6566 6175 6c74  e number Default
-0002df80: 7320 746f 2030 2e0a 2020 2020 2020 2020  s to 0..        
-0002df90: 2020 2020 6c69 6d69 7420 2869 6e74 2c20      limit (int, 
-0002dfa0: 6f70 7469 6f6e 616c 293a 204e 756d 6265  optional): Numbe
-0002dfb0: 7220 6f66 2064 6576 6963 6573 2074 6f20  r of devices to 
-0002dfc0: 6765 7420 4465 6661 756c 7473 2074 6f20  get Defaults to 
-0002dfd0: 3130 302e 0a0a 2020 2020 2020 2020 5265  100...        Re
-0002dfe0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-0002dff0: 2020 2052 6573 706f 6e73 653a 2043 656e     Response: Cen
-0002e000: 7472 616c 4150 4920 5265 7370 6f6e 7365  tralAPI Response
-0002e010: 206f 626a 6563 740a 2020 2020 2020 2020   object.        
-0002e020: 2222 220a 2020 2020 2020 2020 7572 6c20  """.        url 
-0002e030: 3d20 222f 706c 6174 666f 726d 2f64 6576  = "/platform/dev
-0002e040: 6963 655f 696e 7665 6e74 6f72 792f 7631  ice_inventory/v1
-0002e050: 2f64 6576 6963 6573 2f61 7263 6869 7665  /devices/archive
-0002e060: 220a 0a20 2020 2020 2020 2070 6172 616d  "..        param
-0002e070: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
-0002e080: 2020 276f 6666 7365 7427 3a20 6f66 6673    'offset': offs
-0002e090: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
-0002e0a0: 276c 696d 6974 273a 206c 696d 6974 0a20  'limit': limit. 
-0002e0b0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-0002e0c0: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
-0002e0d0: 656c 662e 6765 7428 7572 6c2c 2070 6172  elf.get(url, par
-0002e0e0: 616d 733d 7061 7261 6d73 290a 0a20 2020  ams=params)..   
-0002e0f0: 2061 7379 6e63 2064 6566 2061 7263 6869   async def archi
-0002e100: 7665 5f64 6576 6963 6573 280a 2020 2020  ve_devices(.    
-0002e110: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0002e120: 2020 7365 7269 616c 733a 204c 6973 745b    serials: List[
-0002e130: 7374 725d 2c0a 2020 2020 2920 2d3e 2052  str],.    ) -> R
-0002e140: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
-0002e150: 2022 2222 4172 6368 6976 6520 6465 7669   """Archive devi
-0002e160: 6365 7320 7573 696e 6720 5365 7269 616c  ces using Serial
-0002e170: 206c 6973 742e 0a0a 2020 2020 2020 2020   list...        
-0002e180: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0002e190: 2020 7365 7269 616c 7320 284c 6973 745b    serials (List[
-0002e1a0: 7374 725d 293a 2073 6572 6961 6c73 0a0a  str]): serials..
-0002e1b0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-0002e1c0: 0a20 2020 2020 2020 2020 2020 2052 6573  .            Res
-0002e1d0: 706f 6e73 653a 2043 656e 7472 616c 4150  ponse: CentralAP
-0002e1e0: 4920 5265 7370 6f6e 7365 206f 626a 6563  I Response objec
-0002e1f0: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
-0002e200: 2020 2020 2020 7572 6c20 3d20 222f 706c        url = "/pl
-0002e210: 6174 666f 726d 2f64 6576 6963 655f 696e  atform/device_in
-0002e220: 7665 6e74 6f72 792f 7631 2f64 6576 6963  ventory/v1/devic
-0002e230: 6573 2f61 7263 6869 7665 220a 0a20 2020  es/archive"..   
-0002e240: 2020 2020 206a 736f 6e5f 6461 7461 203d       json_data =
-0002e250: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-0002e260: 7365 7269 616c 7327 3a20 7574 696c 732e  serials': utils.
-0002e270: 6c69 7374 6966 7928 7365 7269 616c 7329  listify(serials)
-0002e280: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-0002e290: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-0002e2a0: 2073 656c 662e 706f 7374 2875 726c 2c20   self.post(url, 
-0002e2b0: 6a73 6f6e 5f64 6174 613d 6a73 6f6e 5f64  json_data=json_d
-0002e2c0: 6174 6129 0a0a 2020 2020 2320 4150 492d  ata)..    # API-
-0002e2d0: 4e4f 5445 2063 656e 636c 6920 7265 6d6f  NOTE cencli remo
-0002e2e0: 7665 2061 7263 6869 7665 205b 6465 7669  ve archive [devi
-0002e2f0: 6365 735d 0a20 2020 2061 7379 6e63 2064  ces].    async d
-0002e300: 6566 2075 6e61 7263 6869 7665 5f64 6576  ef unarchive_dev
-0002e310: 6963 6573 280a 2020 2020 2020 2020 7365  ices(.        se
-0002e320: 6c66 2c0a 2020 2020 2020 2020 7365 7269  lf,.        seri
-0002e330: 616c 733a 204c 6973 745b 7374 725d 2c0a  als: List[str],.
-0002e340: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
-0002e350: 653a 0a20 2020 2020 2020 2022 2222 556e  e:.        """Un
-0002e360: 6172 6368 6976 6520 6465 7669 6365 7320  archive devices 
-0002e370: 7573 696e 6720 5365 7269 616c 206c 6973  using Serial lis
-0002e380: 742e 0a0a 2020 2020 2020 2020 4172 6773  t...        Args
-0002e390: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002e3a0: 7269 616c 7320 284c 6973 745b 7374 725d  rials (List[str]
-0002e3b0: 293a 2073 6572 6961 6c73 0a0a 2020 2020  ): serials..    
-0002e3c0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0002e3d0: 2020 2020 2020 2020 2052 6573 706f 6e73           Respons
-0002e3e0: 653a 2043 656e 7472 616c 4150 4920 5265  e: CentralAPI Re
-0002e3f0: 7370 6f6e 7365 206f 626a 6563 740a 2020  sponse object.  
-0002e400: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0002e410: 2020 7572 6c20 3d20 222f 706c 6174 666f    url = "/platfo
-0002e420: 726d 2f64 6576 6963 655f 696e 7665 6e74  rm/device_invent
-0002e430: 6f72 792f 7631 2f64 6576 6963 6573 2f75  ory/v1/devices/u
-0002e440: 6e61 7263 6869 7665 220a 0a20 2020 2020  narchive"..     
-0002e450: 2020 206a 736f 6e5f 6461 7461 203d 207b     json_data = {
-0002e460: 0a20 2020 2020 2020 2020 2020 2027 7365  .            'se
-0002e470: 7269 616c 7327 3a20 7574 696c 732e 6c69  rials': utils.li
-0002e480: 7374 6966 7928 7365 7269 616c 7329 0a20  stify(serials). 
-0002e490: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-0002e4a0: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
-0002e4b0: 656c 662e 706f 7374 2875 726c 2c20 6a73  elf.post(url, js
-0002e4c0: 6f6e 5f64 6174 613d 6a73 6f6e 5f64 6174  on_data=json_dat
-0002e4d0: 6129 0a0a 2020 2020 6173 796e 6320 6465  a)..    async de
-0002e4e0: 6620 6765 745f 706f 7274 616c 7328 0a20  f get_portals(. 
-0002e4f0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0002e500: 2020 2020 2073 6f72 743a 2073 7472 203d       sort: str =
-0002e510: 2027 2b6e 616d 6527 2c0a 2020 2020 2020   '+name',.      
-0002e520: 2020 6f66 6673 6574 3a20 696e 7420 3d20    offset: int = 
-0002e530: 302c 0a20 2020 2020 2020 206c 696d 6974  0,.        limit
-0002e540: 3a20 696e 7420 3d20 3130 302c 0a20 2020  : int = 100,.   
-0002e550: 2029 202d 3e20 5265 7370 6f6e 7365 3a0a   ) -> Response:.
-0002e560: 2020 2020 2020 2020 2222 2247 6574 2061          """Get a
-0002e570: 6c6c 2070 6f72 7461 6c73 2077 6974 6820  ll portals with 
-0002e580: 6c69 6d69 7465 6420 6461 7461 2e0a 0a20  limited data... 
-0002e590: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0002e5a0: 2020 2020 2020 2020 2073 6f72 7420 2873           sort (s
-0002e5b0: 7472 2c20 6f70 7469 6f6e 616c 293a 202b  tr, optional): +
-0002e5c0: 2069 7320 666f 7220 6173 6365 6e64 696e   is for ascendin
-0002e5d0: 6720 2061 6e64 202d 2066 6f72 2064 6573  g  and - for des
-0002e5e0: 6365 6e64 696e 6720 6f72 6465 7220 2c20  cending order , 
-0002e5f0: 736f 7274 7320 6279 206e 616d 6520 666f  sorts by name fo
-0002e600: 7220 6e6f 770a 2020 2020 2020 2020 2020  r now.          
-0002e610: 2020 2020 2020 5661 6c69 6420 5661 6c75        Valid Valu
-0002e620: 6573 3a20 2b6e 616d 652c 202d 6e61 6d65  es: +name, -name
-0002e630: 0a20 2020 2020 2020 2020 2020 206f 6666  .            off
-0002e640: 7365 7420 2869 6e74 2c20 6f70 7469 6f6e  set (int, option
-0002e650: 616c 293a 2053 7461 7274 696e 6720 696e  al): Starting in
-0002e660: 6465 7820 6f66 2065 6c65 6d65 6e74 2066  dex of element f
-0002e670: 6f72 2061 2070 6167 696e 6174 6564 2071  or a paginated q
-0002e680: 7565 7279 2044 6566 6175 6c74 7320 746f  uery Defaults to
-0002e690: 2030 2e0a 2020 2020 2020 2020 2020 2020   0..            
-0002e6a0: 6c69 6d69 7420 2869 6e74 2c20 6f70 7469  limit (int, opti
-0002e6b0: 6f6e 616c 293a 204e 756d 6265 7220 6f66  onal): Number of
-0002e6c0: 2069 7465 6d73 2072 6571 7569 7265 6420   items required 
-0002e6d0: 7065 7220 7175 6572 7920 4465 6661 756c  per query Defaul
-0002e6e0: 7473 2074 6f20 3130 302e 0a0a 2020 2020  ts to 100...    
-0002e6f0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0002e700: 2020 2020 2020 2020 2052 6573 706f 6e73           Respons
-0002e710: 653a 2043 656e 7472 616c 4150 4920 5265  e: CentralAPI Re
-0002e720: 7370 6f6e 7365 206f 626a 6563 740a 2020  sponse object.  
-0002e730: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0002e740: 2020 7572 6c20 3d20 222f 6775 6573 742f    url = "/guest/
-0002e750: 7631 2f70 6f72 7461 6c73 220a 0a20 2020  v1/portals"..   
-0002e760: 2020 2020 2070 6172 616d 7320 3d20 7b0a       params = {.
-0002e770: 2020 2020 2020 2020 2020 2020 2773 6f72              'sor
-0002e780: 7427 3a20 736f 7274 2c0a 2020 2020 2020  t': sort,.      
-0002e790: 2020 2020 2020 276f 6666 7365 7427 3a20        'offset': 
-0002e7a0: 6f66 6673 6574 2c0a 2020 2020 2020 2020  offset,.        
-0002e7b0: 2020 2020 276c 696d 6974 273a 206c 696d      'limit': lim
-0002e7c0: 6974 0a20 2020 2020 2020 207d 0a0a 2020  it.        }..  
-0002e7d0: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-0002e7e0: 6974 2073 656c 662e 6765 7428 7572 6c2c  it self.get(url,
-0002e7f0: 2070 6172 616d 733d 7061 7261 6d73 290a   params=params).
-0002e800: 0a20 2020 2061 7379 6e63 2064 6566 2067  .    async def g
-0002e810: 6574 5f76 6973 6974 6f72 7328 0a20 2020  et_visitors(.   
-0002e820: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0002e830: 2020 2070 6f72 7461 6c5f 6964 3a20 7374     portal_id: st
-0002e840: 722c 0a20 2020 2020 2020 2073 6f72 743a  r,.        sort:
-0002e850: 2073 7472 203d 2027 2b6e 616d 6527 2c0a   str = '+name',.
-0002e860: 2020 2020 2020 2020 6669 6c74 6572 5f62          filter_b
-0002e870: 793a 2073 7472 203d 204e 6f6e 652c 0a20  y: str = None,. 
-0002e880: 2020 2020 2020 2066 696c 7465 725f 7661         filter_va
-0002e890: 6c75 653a 2073 7472 203d 204e 6f6e 652c  lue: str = None,
-0002e8a0: 0a20 2020 2020 2020 206f 6666 7365 743a  .        offset:
-0002e8b0: 2069 6e74 203d 2030 2c0a 2020 2020 2020   int = 0,.      
-0002e8c0: 2020 6c69 6d69 743a 2069 6e74 203d 2031    limit: int = 1
-0002e8d0: 3030 2c0a 2020 2020 2920 2d3e 2052 6573  00,.    ) -> Res
-0002e8e0: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
-0002e8f0: 2222 4765 7420 616c 6c20 7669 7369 746f  ""Get all visito
-0002e900: 7273 2063 7265 6174 6564 2061 6761 696e  rs created again
-0002e910: 7374 2061 2070 6f72 7461 6c2e 0a0a 2020  st a portal...  
-0002e920: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-0002e930: 2020 2020 2020 2020 706f 7274 616c 5f69          portal_i
-0002e940: 6420 2873 7472 293a 2050 6f72 7461 6c20  d (str): Portal 
-0002e950: 4944 206f 6620 7468 6520 7370 6c61 7368  ID of the splash
-0002e960: 2070 6167 650a 2020 2020 2020 2020 2020   page.          
-0002e970: 2020 736f 7274 2028 7374 722c 206f 7074    sort (str, opt
-0002e980: 696f 6e61 6c29 3a20 2b20 6973 2066 6f72  ional): + is for
-0002e990: 2061 7363 656e 6469 6e67 2020 616e 6420   ascending  and 
-0002e9a0: 2d20 666f 7220 6465 7363 656e 6469 6e67  - for descending
-0002e9b0: 206f 7264 6572 202c 2073 6f72 7473 2062   order , sorts b
-0002e9c0: 7920 6e61 6d65 2066 6f72 0a20 2020 2020  y name for.     
-0002e9d0: 2020 2020 2020 2020 2020 206e 6f77 2020             now  
-0002e9e0: 5661 6c69 6420 5661 6c75 6573 3a20 2b6e  Valid Values: +n
-0002e9f0: 616d 652c 202d 6e61 6d65 0a20 2020 2020  ame, -name.     
-0002ea00: 2020 2020 2020 2066 696c 7465 725f 6279         filter_by
-0002ea10: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-0002ea20: 3a20 6669 6c74 6572 2062 7920 656d 6169  : filter by emai
-0002ea30: 6c20 6f72 206e 616d 6520 2056 616c 6964  l or name  Valid
-0002ea40: 2056 616c 7565 733a 206e 616d 652c 2065   Values: name, e
-0002ea50: 6d61 696c 0a20 2020 2020 2020 2020 2020  mail.           
-0002ea60: 2066 696c 7465 725f 7661 6c75 6520 2873   filter_value (s
-0002ea70: 7472 2c20 6f70 7469 6f6e 616c 293a 2066  tr, optional): f
-0002ea80: 696c 7465 7220 7661 6c75 650a 2020 2020  ilter value.    
-0002ea90: 2020 2020 2020 2020 6f66 6673 6574 2028          offset (
-0002eaa0: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
-0002eab0: 5374 6172 7469 6e67 2069 6e64 6578 206f  Starting index o
-0002eac0: 6620 656c 656d 656e 7420 666f 7220 6120  f element for a 
-0002ead0: 7061 6769 6e61 7465 6420 7175 6572 7920  paginated query 
-0002eae0: 4465 6661 756c 7473 2074 6f20 302e 0a20  Defaults to 0.. 
-0002eaf0: 2020 2020 2020 2020 2020 206c 696d 6974             limit
-0002eb00: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
-0002eb10: 3a20 4e75 6d62 6572 206f 6620 6974 656d  : Number of item
-0002eb20: 7320 7265 7175 6972 6564 2070 6572 2071  s required per q
-0002eb30: 7565 7279 2044 6566 6175 6c74 7320 746f  uery Defaults to
-0002eb40: 2031 3030 2e0a 0a20 2020 2020 2020 2052   100...        R
-0002eb50: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0002eb60: 2020 2020 5265 7370 6f6e 7365 3a20 4365      Response: Ce
-0002eb70: 6e74 7261 6c41 5049 2052 6573 706f 6e73  ntralAPI Respons
-0002eb80: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
-0002eb90: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
-0002eba0: 203d 2066 222f 6775 6573 742f 7631 2f70   = f"/guest/v1/p
-0002ebb0: 6f72 7461 6c73 2f7b 706f 7274 616c 5f69  ortals/{portal_i
-0002ebc0: 647d 2f76 6973 6974 6f72 7322 0a0a 2020  d}/visitors"..  
-0002ebd0: 2020 2020 2020 7061 7261 6d73 203d 207b        params = {
-0002ebe0: 0a20 2020 2020 2020 2020 2020 2027 736f  .            'so
-0002ebf0: 7274 273a 2073 6f72 742c 0a20 2020 2020  rt': sort,.     
-0002ec00: 2020 2020 2020 2027 6669 6c74 6572 5f62         'filter_b
-0002ec10: 7927 3a20 6669 6c74 6572 5f62 792c 0a20  y': filter_by,. 
-0002ec20: 2020 2020 2020 2020 2020 2027 6669 6c74             'filt
-0002ec30: 6572 5f76 616c 7565 273a 2066 696c 7465  er_value': filte
-0002ec40: 725f 7661 6c75 652c 0a20 2020 2020 2020  r_value,.       
-0002ec50: 2020 2020 2027 6f66 6673 6574 273a 206f       'offset': o
-0002ec60: 6666 7365 742c 0a20 2020 2020 2020 2020  ffset,.         
-0002ec70: 2020 2027 6c69 6d69 7427 3a20 6c69 6d69     'limit': limi
-0002ec80: 740a 2020 2020 2020 2020 7d0a 2020 2020  t.        }.    
-0002ec90: 2020 2020 7061 7261 6d73 203d 2075 7469      params = uti
-0002eca0: 6c73 2e73 7472 6970 5f6e 6f6e 6528 7061  ls.strip_none(pa
-0002ecb0: 7261 6d73 290a 0a20 2020 2020 2020 2072  rams)..        r
-0002ecc0: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-0002ecd0: 2e67 6574 2875 726c 2c20 7061 7261 6d73  .get(url, params
-0002ece0: 3d70 6172 616d 7329 0a0a 0a20 2020 2061  =params)...    a
-0002ecf0: 7379 6e63 2064 6566 2061 6464 5f76 6973  sync def add_vis
-0002ed00: 6974 6f72 280a 2020 2020 2020 2020 7365  itor(.        se
-0002ed10: 6c66 2c0a 2020 2020 2020 2020 706f 7274  lf,.        port
-0002ed20: 616c 5f69 643a 2073 7472 2c0a 2020 2020  al_id: str,.    
-0002ed30: 2020 2020 6e61 6d65 3a20 7374 722c 0a20      name: str,. 
-0002ed40: 2020 2020 2020 2023 2069 643a 2073 7472         # id: str
-0002ed50: 2c0a 2020 2020 2020 2020 7061 7373 776f  ,.        passwo
-0002ed60: 7264 3a20 7374 7220 3d20 4e6f 6e65 2c0a  rd: str = None,.
-0002ed70: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-0002ed80: 2020 2063 6f6d 7061 6e79 5f6e 616d 653a     company_name:
-0002ed90: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0002eda0: 2020 2020 2070 686f 6e65 3a20 7374 7220       phone: str 
-0002edb0: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0a20  | None = None,. 
-0002edc0: 2020 2020 2020 2065 6d61 696c 3a20 7374         email: st
-0002edd0: 7220 7c20 4e6f 6e65 203d 204e 6f6e 652c  r | None = None,
-0002ede0: 0a20 2020 2020 2020 2076 616c 6964 5f66  .        valid_f
-0002edf0: 6f72 6576 6572 3a20 626f 6f6c 203d 2046  orever: bool = F
-0002ee00: 616c 7365 2c0a 2020 2020 2020 2020 7661  alse,.        va
-0002ee10: 6c69 645f 6461 7973 3a20 696e 7420 3d20  lid_days: int = 
-0002ee20: 332c 0a20 2020 2020 2020 2076 616c 6964  3,.        valid
-0002ee30: 5f68 6f75 7273 3a20 696e 7420 3d20 302c  _hours: int = 0,
-0002ee40: 0a20 2020 2020 2020 2076 616c 6964 5f6d  .        valid_m
-0002ee50: 696e 7574 6573 3a20 696e 7420 3d20 302c  inutes: int = 0,
-0002ee60: 0a20 2020 2020 2020 206e 6f74 6966 793a  .        notify:
-0002ee70: 2062 6f6f 6c20 7c20 4e6f 6e65 203d 204e   bool | None = N
-0002ee80: 6f6e 652c 0a20 2020 2020 2020 206e 6f74  one,.        not
-0002ee90: 6966 795f 746f 3a20 636f 6e73 7461 6e74  ify_to: constant
-0002eea0: 732e 4e6f 7469 6679 546f 4172 6773 207c  s.NotifyToArgs |
-0002eeb0: 204e 6f6e 6520 3d20 4e6f 6e65 2c0a 2020   None = None,.  
-0002eec0: 2020 2020 2020 6973 5f65 6e61 626c 6564        is_enabled
-0002eed0: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
-0002eee0: 2020 2020 2020 2023 2073 7461 7475 733a         # status:
-0002eef0: 2062 6f6f 6c2c 0a20 2020 2020 2020 2023   bool,.        #
-0002ef00: 2063 7265 6174 6564 5f61 743a 2073 7472   created_at: str
-0002ef10: 2c0a 2020 2020 2020 2020 2320 6578 7069  ,.        # expi
-0002ef20: 7265 5f61 743a 2073 7472 2c0a 2020 2020  re_at: str,.    
-0002ef30: 2920 2d3e 2052 6573 706f 6e73 653a 0a20  ) -> Response:. 
-0002ef40: 2020 2020 2020 2022 2222 4372 6561 7465         """Create
-0002ef50: 2061 206e 6577 2067 7565 7374 2076 6973   a new guest vis
-0002ef60: 6974 6f72 206f 6620 6120 706f 7274 616c  itor of a portal
-0002ef70: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-0002ef80: 0a20 2020 2020 2020 2020 2020 2070 6f72  .            por
-0002ef90: 7461 6c5f 6964 2028 7374 7229 3a20 506f  tal_id (str): Po
-0002efa0: 7274 616c 2049 4420 6f66 2074 6865 2073  rtal ID of the s
-0002efb0: 706c 6173 6820 7061 6765 0a20 2020 2020  plash page.     
-0002efc0: 2020 2020 2020 206e 616d 6520 2873 7472         name (str
-0002efd0: 293a 2056 6973 6974 6f72 2061 6363 6f75  ): Visitor accou
-0002efe0: 6e74 206e 616d 650a 2020 2020 2020 2020  nt name.        
-0002eff0: 2020 2020 7061 7373 776f 7264 2028 7374      password (st
-0002f000: 7229 3a20 5061 7373 776f 7264 0a20 2020  r): Password.   
-0002f010: 2020 2020 2020 2020 2063 6f6d 7061 6e79           company
-0002f020: 5f6e 616d 6520 2873 7472 293a 2043 6f6d  _name (str): Com
-0002f030: 7061 6e79 206e 616d 6520 6f66 2074 6865  pany name of the
-0002f040: 2076 6973 6974 6f72 0a20 2020 2020 2020   visitor.       
-0002f050: 2020 2020 2070 686f 6e65 2028 7374 7229       phone (str)
-0002f060: 3a20 5068 6f6e 6520 6e75 6d62 6572 206f  : Phone number o
-0002f070: 6620 7468 6520 7669 7369 746f 723b 2046  f the visitor; F
-0002f080: 6f72 6d61 7420 5b2b 436f 756e 7472 7943  ormat [+CountryC
-0002f090: 6f64 655d 5b50 686f 6e65 4e75 6d62 6572  ode][PhoneNumber
-0002f0a0: 5d0a 2020 2020 2020 2020 2020 2020 656d  ].            em
-0002f0b0: 6169 6c20 2873 7472 293a 2045 6d61 696c  ail (str): Email
-0002f0c0: 2061 6464 7265 7373 206f 6620 7468 6520   address of the 
-0002f0d0: 7669 7369 746f 720a 2020 2020 2020 2020  visitor.        
-0002f0e0: 2020 2020 7661 6c69 645f 666f 7265 7665      valid_foreve
-0002f0f0: 7220 2862 6f6f 6c29 3a20 5669 7369 746f  r (bool): Visito
-0002f100: 7220 6163 636f 756e 7420 7769 6c6c 206e  r account will n
-0002f110: 6f74 2065 7870 6972 6520 7768 656e 2074  ot expire when t
-0002f120: 6869 7320 6973 2073 6574 2074 6f20 7472  his is set to tr
-0002f130: 7565 0a20 2020 2020 2020 2020 2020 2076  ue.            v
-0002f140: 616c 6964 5f64 6179 7320 2869 6e74 293a  alid_days (int):
-0002f150: 2041 6363 6f75 6e74 2076 616c 6964 6974   Account validit
-0002f160: 7920 696e 2064 6179 730a 2020 2020 2020  y in days.      
-0002f170: 2020 2020 2020 7661 6c69 645f 686f 7572        valid_hour
-0002f180: 7320 2869 6e74 293a 2041 6363 6f75 6e74  s (int): Account
-0002f190: 2076 616c 6964 6974 7920 696e 2068 6f75   validity in hou
-0002f1a0: 7273 0a20 2020 2020 2020 2020 2020 2076  rs.            v
-0002f1b0: 616c 6964 5f6d 696e 7574 6573 2028 696e  alid_minutes (in
-0002f1c0: 7429 3a20 4163 636f 756e 7420 7661 6c69  t): Account vali
-0002f1d0: 6469 7479 2069 6e20 6d69 6e75 7465 730a  dity in minutes.
-0002f1e0: 2020 2020 2020 2020 2020 2020 6e6f 7469              noti
-0002f1f0: 6679 2028 626f 6f6c 293a 2046 6c61 6720  fy (bool): Flag 
-0002f200: 746f 206e 6f74 6966 7920 7468 6520 7061  to notify the pa
-0002f210: 7373 776f 7264 2076 6961 2065 6d61 696c  ssword via email
-0002f220: 206f 7220 6e75 6d62 6572 0a20 2020 2020   or number.     
-0002f230: 2020 2020 2020 206e 6f74 6966 795f 746f         notify_to
-0002f240: 2028 7374 7229 3a20 4e6f 7469 6679 2074   (str): Notify t
-0002f250: 6f20 656d 6169 6c20 6f72 2070 686f 6e65  o email or phone
-0002f260: 2e20 4465 6675 616c 7420 6973 2070 686f  . Defualt is pho
-0002f270: 6e65 2077 6865 6e20 6974 2069 7320 7072  ne when it is pr
-0002f280: 6f76 6964 6564 0a20 2020 2020 2020 2020  ovided.         
-0002f290: 2020 2020 2020 206f 7468 6572 7769 7365         otherwise
-0002f2a0: 2065 6d61 696c 2e20 2056 616c 6964 2056   email.  Valid V
-0002f2b0: 616c 7565 733a 2065 6d61 696c 2c20 7068  alues: email, ph
-0002f2c0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0002f2d0: 6973 5f65 6e61 626c 6564 2028 626f 6f6c  is_enabled (bool
-0002f2e0: 293a 2045 6e61 626c 6520 6f72 2064 6973  ): Enable or dis
-0002f2f0: 6162 6c65 2074 6865 2076 6973 6974 6f72  able the visitor
-0002f300: 2061 6363 6f75 6e74 0a20 2020 2020 2020   account.       
-0002f310: 2020 2020 2023 2069 6420 2873 7472 293a       # id (str):
-0002f320: 204e 4120 666f 7220 7669 7369 746f 7220   NA for visitor 
-0002f330: 706f 7374 2f70 7574 206d 6574 686f 642e  post/put method.
-0002f340: 2049 4420 6f66 2074 6865 2076 6973 6974   ID of the visit
-0002f350: 6f72 0a20 2020 2020 2020 2020 2020 2023  or.            #
-0002f360: 2073 7461 7475 7320 2862 6f6f 6c29 3a20   status (bool): 
-0002f370: 5468 6973 2066 6965 6c64 2070 726f 7669  This field provi
-0002f380: 6465 7320 7374 6174 7573 206f 6620 7468  des status of th
-0002f390: 6520 6163 636f 756e 742e 2052 6574 7572  e account. Retur
-0002f3a0: 6e73 2074 7275 6520 7768 656e 2065 6e61  ns true when ena
-0002f3b0: 626c 6564 2061 6e64 0a20 2020 2020 2020  bled and.       
-0002f3c0: 2020 2020 2023 2020 2020 206e 6f74 2065       #     not e
-0002f3d0: 7870 6972 6564 2e20 4e41 2066 6f72 2076  xpired. NA for v
-0002f3e0: 6973 6974 6f72 2070 6f73 742f 7075 7420  isitor post/put 
-0002f3f0: 6d65 7468 6f64 2e20 5468 6973 2069 7320  method. This is 
-0002f400: 6f70 7469 6f6e 616c 2066 6965 6c64 732e  optional fields.
-0002f410: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
-0002f420: 7265 6174 6564 5f61 7420 2873 7472 293a  reated_at (str):
-0002f430: 2054 6869 7320 6669 656c 6420 696e 6469   This field indi
-0002f440: 6361 7465 7320 7468 6520 6372 6561 7465  cates the create
-0002f450: 6420 6461 7465 2074 696d 6573 7461 6d70  d date timestamp
-0002f460: 2076 616c 7565 2e20 4974 2069 7320 6765   value. It is ge
-0002f470: 6e65 7261 7465 640a 2020 2020 2020 2020  nerated.        
-0002f480: 2020 2020 2320 2020 2020 7768 696c 6520      #     while 
-0002f490: 6372 6561 7469 6e67 2076 6973 6974 6f72  creating visitor
-0002f4a0: 2e20 4e41 2066 6f72 2076 6973 6974 6f72  . NA for visitor
-0002f4b0: 2070 6f73 742f 7075 7420 6d65 7468 6f64   post/put method
-0002f4c0: 2e20 5468 6973 2069 7320 6f70 7469 6f6e  . This is option
-0002f4d0: 616c 2066 6965 6c64 2e0a 2020 2020 2020  al field..      
-0002f4e0: 2020 2020 2020 2320 6578 7069 7265 5f61        # expire_a
-0002f4f0: 7420 2873 7472 293a 2054 6869 7320 6669  t (str): This fi
-0002f500: 656c 6420 696e 6469 6361 7465 7320 6578  eld indicates ex
-0002f510: 7069 7279 2074 696d 6520 7469 6d65 7374  piry time timest
-0002f520: 616d 7020 7661 6c75 652e 2049 7420 6973  amp value. It is
-0002f530: 2067 656e 6572 6174 6564 2062 6173 6564   generated based
-0002f540: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-0002f550: 2020 206f 6e20 7468 6520 7661 6c69 645f     on the valid_
-0002f560: 7469 6c6c 2076 616c 7565 2061 6e64 2063  till value and c
-0002f570: 7265 6174 6564 5f61 7420 7469 6d65 2e20  reated_at time. 
-0002f580: 4e41 2066 6f72 2076 6973 6974 6f72 2070  NA for visitor p
-0002f590: 6f73 742f 7075 7420 6d65 7468 6f64 2e20  ost/put method. 
-0002f5a0: 5468 6973 2069 730a 2020 2020 2020 2020  This is.        
-0002f5b0: 2020 2020 2320 2020 2020 6f70 7469 6f6e      #     option
-0002f5c0: 616c 2066 6965 6c64 0a0a 2020 2020 2020  al field..      
-0002f5d0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0002f5e0: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
-0002f5f0: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
-0002f600: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
-0002f610: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0002f620: 7572 6c20 3d20 6622 2f67 7565 7374 2f76  url = f"/guest/v
-0002f630: 312f 706f 7274 616c 732f 7b70 6f72 7461  1/portals/{porta
-0002f640: 6c5f 6964 7d2f 7669 7369 746f 7273 220a  l_id}/visitors".
-0002f650: 0a20 2020 2020 2020 2075 7365 725f 6461  .        user_da
-0002f660: 7461 203d 207b 0a20 2020 2020 2020 2020  ta = {.         
-0002f670: 2020 2027 7068 6f6e 6527 3a20 7068 6f6e     'phone': phon
-0002f680: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
-0002f690: 656d 6169 6c27 3a20 656d 6169 6c0a 2020  email': email.  
-0002f6a0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-0002f6b0: 2320 4150 4920 7265 7175 6972 6573 2070  # API requires p
-0002f6c0: 686f 6e65 2061 6e64 2065 6d61 696c 2c20  hone and email, 
-0002f6d0: 6275 7420 616c 6c6f 7773 204e 6f6e 652f  but allows None/
-0002f6e0: 6e75 6c6c 2061 7320 7661 6c75 6520 6465  null as value de
-0002f6f0: 7065 6e64 696e 6720 6f6e 2068 6f77 2070  pending on how p
-0002f700: 6f72 7461 6c20 6973 2063 6f6e 6669 6775  ortal is configu
-0002f710: 7265 640a 2020 2020 2020 2020 2320 7573  red.        # us
-0002f720: 6572 5f64 6174 6120 3d20 7574 696c 732e  er_data = utils.
-0002f730: 7374 7269 705f 6e6f 6e65 2875 7365 725f  strip_none(user_
-0002f740: 6461 7461 290a 0a20 2020 2020 2020 206a  data)..        j
-0002f750: 736f 6e5f 6461 7461 203d 207b 0a20 2020  son_data = {.   
-0002f760: 2020 2020 2020 2020 2027 6e61 6d65 273a           'name':
-0002f770: 206e 616d 652c 0a20 2020 2020 2020 2020   name,.         
-0002f780: 2020 2027 636f 6d70 616e 795f 6e61 6d65     'company_name
-0002f790: 273a 2063 6f6d 7061 6e79 5f6e 616d 652c  ': company_name,
-0002f7a0: 0a20 2020 2020 2020 2020 2020 2027 6973  .            'is
-0002f7b0: 5f65 6e61 626c 6564 273a 2069 735f 656e  _enabled': is_en
-0002f7c0: 6162 6c65 642c 0a20 2020 2020 2020 2020  abled,.         
-0002f7d0: 2020 2027 7661 6c69 645f 7469 6c6c 5f6e     'valid_till_n
-0002f7e0: 6f5f 6c69 6d69 7427 3a20 7661 6c69 645f  o_limit': valid_
-0002f7f0: 666f 7265 7665 722c 0a20 2020 2020 2020  forever,.       
-0002f800: 2020 2020 2027 7661 6c69 645f 7469 6c6c       'valid_till
-0002f810: 5f64 6179 7327 3a20 7661 6c69 645f 6461  _days': valid_da
-0002f820: 7973 2c0a 2020 2020 2020 2020 2020 2020  ys,.            
-0002f830: 2776 616c 6964 5f74 696c 6c5f 686f 7572  'valid_till_hour
-0002f840: 7327 3a20 7661 6c69 645f 686f 7572 732c  s': valid_hours,
-0002f850: 0a20 2020 2020 2020 2020 2020 2027 7661  .            'va
-0002f860: 6c69 645f 7469 6c6c 5f6d 696e 7574 6573  lid_till_minutes
-0002f870: 273a 2076 616c 6964 5f6d 696e 7574 6573  ': valid_minutes
-0002f880: 2c0a 2020 2020 2020 2020 2020 2020 276e  ,.            'n
-0002f890: 6f74 6966 7927 3a20 6e6f 7469 6679 2c0a  otify': notify,.
-0002f8a0: 2020 2020 2020 2020 2020 2020 276e 6f74              'not
-0002f8b0: 6966 795f 746f 273a 206e 6f74 6966 795f  ify_to': notify_
-0002f8c0: 746f 2c0a 2020 2020 2020 2020 2020 2020  to,.            
-0002f8d0: 2770 6173 7377 6f72 6427 3a20 7061 7373  'password': pass
-0002f8e0: 776f 7264 0a20 2020 2020 2020 207d 0a20  word.        }. 
-0002f8f0: 2020 2020 2020 206a 736f 6e5f 6461 7461         json_data
-0002f900: 203d 2075 7469 6c73 2e73 7472 6970 5f6e   = utils.strip_n
-0002f910: 6f6e 6528 6a73 6f6e 5f64 6174 6129 0a20  one(json_data). 
-0002f920: 2020 2020 2020 2069 6620 7573 6572 5f64         if user_d
-0002f930: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
-0002f940: 206a 736f 6e5f 6461 7461 5b22 7573 6572   json_data["user
-0002f950: 225d 203d 2075 7365 725f 6461 7461 0a0a  "] = user_data..
-0002f960: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-0002f970: 7761 6974 2073 656c 662e 706f 7374 2875  wait self.post(u
-0002f980: 726c 2c20 6a73 6f6e 5f64 6174 613d 6a73  rl, json_data=js
-0002f990: 6f6e 5f64 6174 6129 0a0a 2020 2020 2320  on_data)..    # 
-0002f9a0: 544f 444f 2076 616c 6964 6174 6520 4950  TODO validate IP
-0002f9b0: 2061 6464 7265 7373 2066 6f72 6d61 740a   address format.
-0002f9c0: 2020 2020 6173 796e 6320 6465 6620 7570      async def up
-0002f9d0: 6461 7465 5f63 785f 7072 6f70 6572 7469  date_cx_properti
-0002f9e0: 6573 280a 2020 2020 2020 2020 7365 6c66  es(.        self
-0002f9f0: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
-0002fa00: 2020 2020 2073 6572 6961 6c3a 2073 7472       serial: str
-0002fa10: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0002fa20: 2067 726f 7570 3a20 7374 7220 3d20 4e6f   group: str = No
-0002fa30: 6e65 2c0a 2020 2020 2020 2020 6e61 6d65  ne,.        name
-0002fa40: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-0002fa50: 2020 2020 2020 636f 6e74 6163 743a 2073        contact: s
-0002fa60: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-0002fa70: 2020 206c 6f63 6174 696f 6e3a 2073 7472     location: str
-0002fa80: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0002fa90: 2074 696d 657a 6f6e 653a 2063 6f6e 7374   timezone: const
-0002faa0: 616e 7473 2e54 5a44 4220 3d20 4e6f 6e65  ants.TZDB = None
-0002fab0: 2c0a 2020 2020 2020 2020 6d67 6d74 5f76  ,.        mgmt_v
-0002fac0: 7266 3a20 626f 6f6c 203d 204e 6f6e 652c  rf: bool = None,
-0002fad0: 0a20 2020 2020 2020 2064 6e73 5f73 6572  .        dns_ser
-0002fae0: 7665 7273 3a20 4c69 7374 5b73 7472 5d20  vers: List[str] 
-0002faf0: 3d20 5b5d 2c0a 2020 2020 2020 2020 6e74  = [],.        nt
-0002fb00: 705f 7365 7276 6572 733a 204c 6973 745b  p_servers: List[
-0002fb10: 7374 725d 203d 205b 5d2c 0a20 2020 2020  str] = [],.     
-0002fb20: 2020 2061 646d 696e 5f75 7365 723a 2073     admin_user: s
-0002fb30: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-0002fb40: 2020 2061 646d 696e 5f70 6173 733a 2073     admin_pass: s
-0002fb50: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
-0002fb60: 202d 3e20 5265 7370 6f6e 7365 3a0a 2020   -> Response:.  
-0002fb70: 2020 2020 2020 2222 2255 7064 6174 6520        """Update 
-0002fb80: 5072 6f70 6572 7469 6573 2028 4172 7562  Properties (Arub
-0002fb90: 614f 532d 4358 292e 0a0a 2020 2020 2020  aOS-CX)...      
-0002fba0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0002fbb0: 2020 2020 7365 7269 616c 2028 7374 722c      serial (str,
-0002fbc0: 206f 7074 696f 6e61 6c29 3a20 4465 7669   optional): Devi
-0002fbd0: 6365 2073 6572 6961 6c20 6e75 6d62 6572  ce serial number
-0002fbe0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0002fbf0: 2020 4d61 6e64 6174 6f72 7920 666f 7220    Mandatory for 
-0002fc00: 6465 7669 6365 206c 6576 656c 2063 6f6e  device level con
-0002fc10: 6669 6775 7261 7469 6f6e 2e0a 2020 2020  figuration..    
-0002fc20: 2020 2020 2020 2020 2020 2020 3120 616e              1 an
-0002fc30: 6420 6f6e 6c79 2031 206f 6620 7365 7269  d only 1 of seri
-0002fc40: 616c 206f 7220 6772 6f75 7020 6172 6520  al or group are 
-0002fc50: 7265 7175 6972 6564 0a20 2020 2020 2020  required.       
-0002fc60: 2020 2020 2067 726f 7570 2028 7374 722c       group (str,
-0002fc70: 206f 7074 696f 6e61 6c29 3a20 4772 6f75   optional): Grou
-0002fc80: 7020 6e61 6d65 2e0a 2020 2020 2020 2020  p name..        
-0002fc90: 2020 2020 2020 2020 4d61 6e64 6174 6f72          Mandator
-0002fca0: 7920 666f 7220 6772 6f75 7020 6c65 7665  y for group leve
-0002fcb0: 6c20 636f 6e66 6967 7572 6174 696f 6e2e  l configuration.
-0002fcc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002fcd0: 2031 2061 6e64 206f 6e6c 7920 3120 6f66   1 and only 1 of
-0002fce0: 2073 6572 6961 6c20 6f72 2067 726f 7570   serial or group
-0002fcf0: 2061 7265 2072 6571 7569 7265 640a 2020   are required.  
-0002fd00: 2020 2020 2020 2020 2020 6e61 6d65 2028            name (
-0002fd10: 7374 7229 3a20 4f6e 6c79 2063 6f6e 6669  str): Only confi
-0002fd20: 6775 7261 626c 6520 6174 2064 6576 6963  gurable at devic
-0002fd30: 652d 6c65 7665 6c2e 0a20 2020 2020 2020  e-level..       
-0002fd40: 2020 2020 2063 6f6e 7461 6374 2028 7374       contact (st
-0002fd50: 7229 3a20 5061 7474 6572 6e3a 2022 5e5b  r): Pattern: "^[
-0002fd60: 5e22 3f5d 2a24 220a 2020 2020 2020 2020  ^"?]*$".        
-0002fd70: 2020 2020 6c6f 6361 7469 6f6e 2028 7374      location (st
-0002fd80: 7229 3a20 5061 7474 6572 6e3a 2022 5e5b  r): Pattern: "^[
-0002fd90: 5e22 3f5d 2a24 220a 2020 2020 2020 2020  ^"?]*$".        
-0002fda0: 2020 2020 7469 6d65 7a6f 6e65 2028 7374      timezone (st
-0002fdb0: 7229 3a20 7469 6d65 7a6f 6e65 2020 5661  r): timezone  Va
-0002fdc0: 6c69 6420 5661 6c75 6573 3a20 7573 6520  lid Values: use 
-0002fdd0: 747a 2064 6174 6162 6173 6520 666f 726d  tz database form
-0002fde0: 6174 206c 696b 6520 2241 6d65 7269 6361  at like "America
-0002fdf0: 2f43 6869 6361 676f 220a 2020 2020 2020  /Chicago".      
-0002fe00: 2020 2020 2020 6d67 6d74 5f76 7266 2028        mgmt_vrf (
-0002fe10: 626f 6f6c 293a 2055 7365 206d 676d 7420  bool): Use mgmt 
-0002fe20: 5652 462c 2069 6e64 6963 6174 6573 2056  VRF, indicates V
-0002fe30: 5246 2066 6f72 2064 6e73 5f73 6572 7665  RF for dns_serve
-0002fe40: 7273 2061 6e64 206e 7470 5f73 6572 7665  rs and ntp_serve
-0002fe50: 7273 2c20 6966 2046 616c 7365 206f 7220  rs, if False or 
-0002fe60: 6e6f 7420 7072 6f76 6964 6564 2064 6566  not provided def
-0002fe70: 6175 6c74 2056 5246 2069 7320 7573 6564  ault VRF is used
-0002fe80: 2e0a 2020 2020 2020 2020 2020 2020 646e  ..            dn
-0002fe90: 735f 7365 7276 6572 7320 284c 6973 745b  s_servers (List[
-0002fea0: 7374 725d 293a 2069 7076 342f 6970 7636  str]): ipv4/ipv6
-0002feb0: 2061 6464 7265 7373 0a20 2020 2020 2020   address.       
-0002fec0: 2020 2020 206e 7470 5f73 6572 7665 7273       ntp_servers
-0002fed0: 2028 4c69 7374 5b73 7472 5d29 3a20 6970   (List[str]): ip
-0002fee0: 7634 2f69 7076 3620 6164 6472 6573 730a  v4/ipv6 address.
-0002fef0: 2020 2020 2020 2020 2020 2020 6164 6d69              admi
-0002ff00: 6e5f 7573 6572 2028 7374 7229 3a20 6c6f  n_user (str): lo
-0002ff10: 6361 6c20 6164 6d69 6e20 7573 6572 0a20  cal admin user. 
-0002ff20: 2020 2020 2020 2020 2020 2061 646d 696e             admin
-0002ff30: 5f70 6173 7320 2873 7472 293a 206c 6f63  _pass (str): loc
-0002ff40: 616c 2061 646d 696e 2070 6173 7377 6f72  al admin passwor
-0002ff50: 640a 0a20 2020 2020 2020 2052 6574 7572  d..        Retur
-0002ff60: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-0002ff70: 5265 7370 6f6e 7365 3a20 4365 6e74 7261  Response: Centra
-0002ff80: 6c41 5049 2052 6573 706f 6e73 6520 6f62  lAPI Response ob
-0002ff90: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
-0002ffa0: 0a20 2020 2020 2020 2075 726c 203d 2022  .        url = "
-0002ffb0: 2f63 6f6e 6669 6775 7261 7469 6f6e 2f76  /configuration/v
-0002ffc0: 312f 7377 6974 6368 2f63 782f 7072 6f70  1/switch/cx/prop
-0002ffd0: 6572 7469 6573 220a 0a20 2020 2020 2020  erties"..       
-0002ffe0: 2070 6172 616d 7320 3d20 7b0a 2020 2020   params = {.    
-0002fff0: 2020 2020 2020 2020 2764 6576 6963 655f          'device_
-00030000: 7365 7269 616c 273a 2073 6572 6961 6c2c  serial': serial,
-00030010: 0a20 2020 2020 2020 2020 2020 2027 6772  .            'gr
-00030020: 6f75 705f 6e61 6d65 273a 2067 726f 7570  oup_name': group
-00030030: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-00030040: 2020 2020 6a73 6f6e 5f64 6174 6120 3d20      json_data = 
-00030050: 7b0a 2020 2020 2020 2020 2020 2020 276e  {.            'n
-00030060: 616d 6527 3a20 6e61 6d65 2c0a 2020 2020  ame': name,.    
-00030070: 2020 2020 2020 2020 2763 6f6e 7461 6374          'contact
-00030080: 273a 2063 6f6e 7461 6374 2c0a 2020 2020  ': contact,.    
-00030090: 2020 2020 2020 2020 276c 6f63 6174 696f          'locatio
-000300a0: 6e27 3a20 6c6f 6361 7469 6f6e 2c0a 2020  n': location,.  
-000300b0: 2020 2020 2020 2020 2020 2774 696d 657a            'timez
-000300c0: 6f6e 6527 3a20 7469 6d65 7a6f 6e65 2c0a  one': timezone,.
-000300d0: 2020 2020 2020 2020 2020 2020 2764 6e73              'dns
-000300e0: 5f73 6572 7665 7273 273a 2064 6e73 5f73  _servers': dns_s
-000300f0: 6572 7665 7273 2c0a 2020 2020 2020 2020  ervers,.        
-00030100: 2020 2020 276e 7470 5f73 6572 7665 7273      'ntp_servers
-00030110: 273a 206e 7470 5f73 6572 7665 7273 2c0a  ': ntp_servers,.
-00030120: 2020 2020 2020 2020 2020 2020 2761 646d              'adm
-00030130: 696e 5f75 7365 726e 616d 6527 3a20 6164  in_username': ad
-00030140: 6d69 6e5f 7573 6572 2c0a 2020 2020 2020  min_user,.      
-00030150: 2020 2020 2020 2761 646d 696e 5f70 6173        'admin_pas
-00030160: 7377 6f72 6427 3a20 6164 6d69 6e5f 7061  sword': admin_pa
-00030170: 7373 0a20 2020 2020 2020 207d 0a20 2020  ss.        }.   
-00030180: 2020 2020 2069 6620 6d67 6d74 5f76 7266       if mgmt_vrf
-00030190: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000301a0: 2020 2020 2020 2020 2020 6a73 6f6e 5f64            json_d
-000301b0: 6174 615b 2276 7266 225d 203d 2022 6d67  ata["vrf"] = "mg
-000301c0: 6d74 2220 6966 206d 676d 745f 7672 6620  mt" if mgmt_vrf 
-000301d0: 656c 7365 2022 6465 6661 756c 7422 0a20  else "default". 
-000301e0: 2020 2020 2020 2065 6c69 6620 646e 735f         elif dns_
-000301f0: 7365 7276 6572 7320 6f72 206e 7470 5f73  servers or ntp_s
-00030200: 6572 7665 7273 3a0a 2020 2020 2020 2020  ervers:.        
-00030210: 2020 2020 6a73 6f6e 5f64 6174 615b 2276      json_data["v
-00030220: 7266 225d 203d 2022 6465 6661 756c 7422  rf"] = "default"
-00030230: 0a0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
-00030240: 285b 7820 666f 7220 7820 696e 205b 6164  ([x for x in [ad
-00030250: 6d69 6e5f 7573 6572 2c20 6164 6d69 6e5f  min_user, admin_
-00030260: 7061 7373 5d20 6966 2078 2069 7320 6e6f  pass] if x is no
-00030270: 7420 4e6f 6e65 5d29 203d 3d20 313a 0a20  t None]) == 1:. 
-00030280: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00030290: 2056 616c 7565 4572 726f 7228 2249 6620   ValueError("If 
-000302a0: 6569 7468 6572 2061 646d 696e 5f75 7365  either admin_use
-000302b0: 7220 6f72 2061 646d 696e 5f70 6173 7320  r or admin_pass 
-000302c0: 6172 6520 6269 6e67 2075 7064 6174 6564  are bing updated
-000302d0: 2c20 2a62 6f74 682a 2073 686f 756c 6420  , *both* should 
-000302e0: 6265 2070 726f 7669 6465 642e 2229 0a0a  be provided.")..
-000302f0: 2020 2020 2020 2020 6966 206c 656e 285b          if len([
-00030300: 7820 666f 7220 7820 696e 205b 7365 7269  x for x in [seri
-00030310: 616c 2c20 6772 6f75 705d 2069 6620 7820  al, group] if x 
-00030320: 6973 206e 6f74 204e 6f6e 655d 2920 3d3d  is not None]) ==
-00030330: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-00030340: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00030350: 2822 7072 6f76 6964 6520 7365 7269 616c  ("provide serial
-00030360: 2074 6f20 7570 6461 7465 2064 6576 6963   to update devic
-00030370: 6520 6c65 7665 6c20 7072 6f70 6572 7469  e level properti
-00030380: 6573 2c20 6f72 2067 726f 7570 2074 6f20  es, or group to 
-00030390: 7570 6461 7465 2061 7420 7468 6520 6772  update at the gr
-000303a0: 6f75 7020 6c65 7665 6c2e 2020 5072 6f76  oup level.  Prov
-000303b0: 6964 696e 6720 626f 7468 2069 7320 696e  iding both is in
-000303c0: 7661 6c69 642e 2229 0a0a 2020 2020 2020  valid.")..      
-000303d0: 2020 6a73 6f6e 5f64 6174 6120 3d20 7574    json_data = ut
-000303e0: 696c 732e 7374 7269 705f 6e6f 6e65 286a  ils.strip_none(j
-000303f0: 736f 6e5f 6461 7461 2c20 7374 7269 705f  son_data, strip_
-00030400: 656d 7074 795f 6f62 6a3d 5472 7565 290a  empty_obj=True).
-00030410: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00030420: 6177 6169 7420 7365 6c66 2e70 6f73 7428  await self.post(
-00030430: 7572 6c2c 206a 736f 6e5f 6461 7461 3d6a  url, json_data=j
-00030440: 736f 6e5f 6461 7461 2c20 7061 7261 6d73  son_data, params
-00030450: 3d70 6172 616d 7329 0a0a 2020 2020 6173  =params)..    as
-00030460: 796e 6320 6465 6620 6765 745f 6f73 7066  ync def get_ospf
-00030470: 5f61 7265 6128 0a20 2020 2020 2020 2073  _area(.        s
-00030480: 656c 662c 0a20 2020 2020 2020 2064 6576  elf,.        dev
-00030490: 6963 653a 2073 7472 2c0a 2020 2020 2020  ice: str,.      
-000304a0: 2020 6d61 726b 6572 3a20 7374 7220 3d20    marker: str = 
-000304b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c69  None,.        li
-000304c0: 6d69 743a 2069 6e74 203d 2031 3030 2c0a  mit: int = 100,.
-000304d0: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
-000304e0: 653a 0a20 2020 2020 2020 2022 2222 4c69  e:.        """Li
-000304f0: 7374 204f 5350 4620 4172 6561 2049 6e66  st OSPF Area Inf
-00030500: 6f72 6d61 7469 6f6e 2e0a 0a20 2020 2020  ormation...     
-00030510: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00030520: 2020 2020 2064 6576 6963 6520 2873 7472       device (str
-00030530: 293a 2044 6576 6963 6520 7365 7269 616c  ): Device serial
-00030540: 206e 756d 6265 720a 2020 2020 2020 2020   number.        
-00030550: 2020 2020 6d61 726b 6572 2028 7374 722c      marker (str,
-00030560: 206f 7074 696f 6e61 6c29 3a20 4f70 6171   optional): Opaq
-00030570: 7565 2068 616e 646c 6520 746f 2066 6574  ue handle to fet
-00030580: 6368 206e 6578 7420 7061 6765 0a20 2020  ch next page.   
-00030590: 2020 2020 2020 2020 206c 696d 6974 2028           limit (
-000305a0: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
-000305b0: 7061 6765 2073 697a 6520 4465 6661 756c  page size Defaul
-000305c0: 7473 2074 6f20 3130 302e 0a0a 2020 2020  ts to 100...    
-000305d0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-000305e0: 2020 2020 2020 2020 2052 6573 706f 6e73           Respons
-000305f0: 653a 2043 656e 7472 616c 4150 4920 5265  e: CentralAPI Re
-00030600: 7370 6f6e 7365 206f 626a 6563 740a 2020  sponse object.  
-00030610: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00030620: 2020 7572 6c20 3d20 222f 6170 692f 726f    url = "/api/ro
-00030630: 7574 696e 672f 7631 2f6f 7370 662f 6172  uting/v1/ospf/ar
-00030640: 6561 220a 0a20 2020 2020 2020 2070 6172  ea"..        par
-00030650: 616d 7320 3d20 7b0a 2020 2020 2020 2020  ams = {.        
-00030660: 2020 2020 2764 6576 6963 6527 3a20 6465      'device': de
-00030670: 7669 6365 2c0a 2020 2020 2020 2020 2020  vice,.          
-00030680: 2020 276d 6172 6b65 7227 3a20 6d61 726b    'marker': mark
-00030690: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-000306a0: 276c 696d 6974 273a 206c 696d 6974 0a20  'limit': limit. 
-000306b0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-000306c0: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
-000306d0: 656c 662e 6765 7428 7572 6c2c 2070 6172  elf.get(url, par
-000306e0: 616d 733d 7061 7261 6d73 290a 0a20 2020  ams=params)..   
-000306f0: 2061 7379 6e63 2064 6566 2067 6574 5f6f   async def get_o
-00030700: 7370 665f 696e 7465 7266 6163 6528 0a20  spf_interface(. 
-00030710: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00030720: 2020 2020 2064 6576 6963 653a 2073 7472       device: str
-00030730: 2c0a 2020 2020 2020 2020 6d61 726b 6572  ,.        marker
-00030740: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00030750: 2020 2020 2020 6c69 6d69 743a 2069 6e74        limit: int
-00030760: 203d 2031 3030 2c0a 2020 2020 2920 2d3e   = 100,.    ) ->
-00030770: 2052 6573 706f 6e73 653a 0a20 2020 2020   Response:.     
-00030780: 2020 2022 2222 4c69 7374 204f 5350 4620     """List OSPF 
-00030790: 496e 7465 7266 6163 6520 496e 666f 726d  Interface Inform
-000307a0: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
-000307b0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-000307c0: 2020 6465 7669 6365 2028 7374 7229 3a20    device (str): 
-000307d0: 4465 7669 6365 2073 6572 6961 6c20 6e75  Device serial nu
-000307e0: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
-000307f0: 206d 6172 6b65 7220 2873 7472 2c20 6f70   marker (str, op
-00030800: 7469 6f6e 616c 293a 204f 7061 7175 6520  tional): Opaque 
-00030810: 6861 6e64 6c65 2074 6f20 6665 7463 6820  handle to fetch 
-00030820: 6e65 7874 2070 6167 650a 2020 2020 2020  next page.      
-00030830: 2020 2020 2020 6c69 6d69 7420 2869 6e74        limit (int
-00030840: 2c20 6f70 7469 6f6e 616c 293a 2070 6167  , optional): pag
-00030850: 6520 7369 7a65 2044 6566 6175 6c74 7320  e size Defaults 
-00030860: 746f 2031 3030 2e0a 0a20 2020 2020 2020  to 100...       
-00030870: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00030880: 2020 2020 2020 5265 7370 6f6e 7365 3a20        Response: 
-00030890: 4365 6e74 7261 6c41 5049 2052 6573 706f  CentralAPI Respo
-000308a0: 6e73 6520 6f62 6a65 6374 0a20 2020 2020  nse object.     
-000308b0: 2020 2022 2222 0a20 2020 2020 2020 2075     """.        u
-000308c0: 726c 203d 2022 2f61 7069 2f72 6f75 7469  rl = "/api/routi
-000308d0: 6e67 2f76 312f 6f73 7066 2f69 6e74 6572  ng/v1/ospf/inter
-000308e0: 6661 6365 220a 0a20 2020 2020 2020 2070  face"..        p
-000308f0: 6172 616d 7320 3d20 7b0a 2020 2020 2020  arams = {.      
-00030900: 2020 2020 2020 2764 6576 6963 6527 3a20        'device': 
-00030910: 6465 7669 6365 2c0a 2020 2020 2020 2020  device,.        
-00030920: 2020 2020 276d 6172 6b65 7227 3a20 6d61      'marker': ma
-00030930: 726b 6572 2c0a 2020 2020 2020 2020 2020  rker,.          
-00030940: 2020 276c 696d 6974 273a 206c 696d 6974    'limit': limit
-00030950: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-00030960: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-00030970: 2073 656c 662e 6765 7428 7572 6c2c 2070   self.get(url, p
-00030980: 6172 616d 733d 7061 7261 6d73 290a 0a20  arams=params).. 
-00030990: 2020 2061 7379 6e63 2064 6566 2067 6574     async def get
-000309a0: 5f6f 7370 665f 6e65 6967 6862 6f72 280a  _ospf_neighbor(.
-000309b0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000309c0: 2020 2020 2020 6465 7669 6365 3a20 7374        device: st
-000309d0: 722c 0a20 2020 2020 2020 206d 6172 6b65  r,.        marke
-000309e0: 723a 2073 7472 203d 204e 6f6e 652c 0a20  r: str = None,. 
-000309f0: 2020 2020 2020 206c 696d 6974 3a20 696e         limit: in
-00030a00: 7420 3d20 3130 302c 0a20 2020 2029 202d  t = 100,.    ) -
-00030a10: 3e20 5265 7370 6f6e 7365 3a0a 2020 2020  > Response:.    
-00030a20: 2020 2020 2222 224c 6973 7420 4f53 5046      """List OSPF
-00030a30: 206e 6569 6768 626f 7220 496e 666f 726d   neighbor Inform
-00030a40: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
-00030a50: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00030a60: 2020 6465 7669 6365 2028 7374 7229 3a20    device (str): 
-00030a70: 4465 7669 6365 2073 6572 6961 6c20 6e75  Device serial nu
-00030a80: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
-00030a90: 206d 6172 6b65 7220 2873 7472 2c20 6f70   marker (str, op
-00030aa0: 7469 6f6e 616c 293a 204f 7061 7175 6520  tional): Opaque 
-00030ab0: 6861 6e64 6c65 2074 6f20 6665 7463 6820  handle to fetch 
-00030ac0: 6e65 7874 2070 6167 650a 2020 2020 2020  next page.      
-00030ad0: 2020 2020 2020 6c69 6d69 7420 2869 6e74        limit (int
-00030ae0: 2c20 6f70 7469 6f6e 616c 293a 2070 6167  , optional): pag
-00030af0: 6520 7369 7a65 2044 6566 6175 6c74 7320  e size Defaults 
-00030b00: 746f 2031 3030 2e0a 0a20 2020 2020 2020  to 100...       
-00030b10: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00030b20: 2020 2020 2020 5265 7370 6f6e 7365 3a20        Response: 
-00030b30: 4365 6e74 7261 6c41 5049 2052 6573 706f  CentralAPI Respo
-00030b40: 6e73 6520 6f62 6a65 6374 0a20 2020 2020  nse object.     
-00030b50: 2020 2022 2222 0a20 2020 2020 2020 2075     """.        u
-00030b60: 726c 203d 2022 2f61 7069 2f72 6f75 7469  rl = "/api/routi
-00030b70: 6e67 2f76 312f 6f73 7066 2f6e 6569 6768  ng/v1/ospf/neigh
-00030b80: 626f 7222 0a0a 2020 2020 2020 2020 7061  bor"..        pa
-00030b90: 7261 6d73 203d 207b 0a20 2020 2020 2020  rams = {.       
-00030ba0: 2020 2020 2027 6465 7669 6365 273a 2064       'device': d
-00030bb0: 6576 6963 652c 0a20 2020 2020 2020 2020  evice,.         
-00030bc0: 2020 2027 6d61 726b 6572 273a 206d 6172     'marker': mar
-00030bd0: 6b65 722c 0a20 2020 2020 2020 2020 2020  ker,.           
-00030be0: 2027 6c69 6d69 7427 3a20 6c69 6d69 740a   'limit': limit.
-00030bf0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00030c00: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-00030c10: 7365 6c66 2e67 6574 2875 726c 2c20 7061  self.get(url, pa
-00030c20: 7261 6d73 3d70 6172 616d 7329 0a0a 2020  rams=params)..  
-00030c30: 2020 6173 796e 6320 6465 6620 6765 745f    async def get_
-00030c40: 6f73 7066 5f64 6174 6162 6173 6528 0a20  ospf_database(. 
-00030c50: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00030c60: 2020 2020 2064 6576 6963 653a 2073 7472       device: str
-00030c70: 2c0a 2020 2020 2020 2020 6d61 726b 6572  ,.        marker
-00030c80: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00030c90: 2020 2020 2020 6c69 6d69 743a 2069 6e74        limit: int
-00030ca0: 203d 2031 3030 2c0a 2020 2020 2920 2d3e   = 100,.    ) ->
-00030cb0: 2052 6573 706f 6e73 653a 0a20 2020 2020   Response:.     
-00030cc0: 2020 2022 2222 4c69 7374 204f 5350 4620     """List OSPF 
-00030cd0: 4c69 6e6b 2053 7461 7465 2044 6174 6162  Link State Datab
-00030ce0: 6173 6520 496e 666f 726d 6174 696f 6e2e  ase Information.
-00030cf0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00030d00: 2020 2020 2020 2020 2020 2020 6465 7669              devi
-00030d10: 6365 2028 7374 7229 3a20 4465 7669 6365  ce (str): Device
-00030d20: 2073 6572 6961 6c20 6e75 6d62 6572 0a20   serial number. 
-00030d30: 2020 2020 2020 2020 2020 206d 6172 6b65             marke
-00030d40: 7220 2873 7472 2c20 6f70 7469 6f6e 616c  r (str, optional
-00030d50: 293a 204f 7061 7175 6520 6861 6e64 6c65  ): Opaque handle
-00030d60: 2074 6f20 6665 7463 6820 6e65 7874 2070   to fetch next p
-00030d70: 6167 650a 2020 2020 2020 2020 2020 2020  age.            
-00030d80: 6c69 6d69 7420 2869 6e74 2c20 6f70 7469  limit (int, opti
-00030d90: 6f6e 616c 293a 2070 6167 6520 7369 7a65  onal): page size
-00030da0: 2044 6566 6175 6c74 7320 746f 2031 3030   Defaults to 100
-00030db0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00030dc0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00030dd0: 5265 7370 6f6e 7365 3a20 4365 6e74 7261  Response: Centra
-00030de0: 6c41 5049 2052 6573 706f 6e73 6520 6f62  lAPI Response ob
-00030df0: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
-00030e00: 0a20 2020 2020 2020 2075 726c 203d 2022  .        url = "
-00030e10: 2f61 7069 2f72 6f75 7469 6e67 2f76 312f  /api/routing/v1/
-00030e20: 6f73 7066 2f64 6174 6162 6173 6522 0a0a  ospf/database"..
-00030e30: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
-00030e40: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-00030e50: 6465 7669 6365 273a 2064 6576 6963 652c  device': device,
-00030e60: 0a20 2020 2020 2020 2020 2020 2027 6d61  .            'ma
-00030e70: 726b 6572 273a 206d 6172 6b65 722c 0a20  rker': marker,. 
-00030e80: 2020 2020 2020 2020 2020 2027 6c69 6d69             'limi
-00030e90: 7427 3a20 6c69 6d69 740a 2020 2020 2020  t': limit.      
-00030ea0: 2020 7d0a 0a20 2020 2020 2020 2072 6574    }..        ret
-00030eb0: 7572 6e20 6177 6169 7420 7365 6c66 2e67  urn await self.g
-00030ec0: 6574 2875 726c 2c20 7061 7261 6d73 3d70  et(url, params=p
-00030ed0: 6172 616d 7329 0a0a 2020 2020 6173 796e  arams)..    asyn
-00030ee0: 6320 6465 6620 6765 745f 6f76 6572 6c61  c def get_overla
-00030ef0: 795f 636f 6e6e 6563 7469 6f6e 280a 2020  y_connection(.  
-00030f00: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00030f10: 2020 2020 6465 7669 6365 3a20 7374 722c      device: str,
-00030f20: 0a20 2020 2020 2020 206d 6172 6b65 723a  .        marker:
-00030f30: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00030f40: 2020 2020 206c 696d 6974 3a20 696e 7420       limit: int 
-00030f50: 3d20 3130 302c 0a20 2020 2029 202d 3e20  = 100,.    ) -> 
-00030f60: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
-00030f70: 2020 2222 2247 6574 2069 6e66 6f72 6d61    """Get informa
-00030f80: 7469 6f6e 2061 626f 7574 206f 7665 726c  tion about overl
-00030f90: 6179 2063 6f6e 7472 6f6c 2063 6f6e 6e65  ay control conne
-00030fa0: 6374 696f 6e2e 0a0a 2020 2020 2020 2020  ction...        
-00030fb0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00030fc0: 2020 6465 7669 6365 2028 7374 7229 3a20    device (str): 
-00030fd0: 4465 7669 6365 2073 6572 6961 6c20 6e75  Device serial nu
-00030fe0: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
-00030ff0: 206d 6172 6b65 7220 2873 7472 2c20 6f70   marker (str, op
-00031000: 7469 6f6e 616c 293a 204f 7061 7175 6520  tional): Opaque 
-00031010: 6861 6e64 6c65 2074 6f20 6665 7463 6820  handle to fetch 
-00031020: 6e65 7874 2070 6167 650a 2020 2020 2020  next page.      
-00031030: 2020 2020 2020 6c69 6d69 7420 2869 6e74        limit (int
-00031040: 2c20 6f70 7469 6f6e 616c 293a 2070 6167  , optional): pag
-00031050: 6520 7369 7a65 2044 6566 6175 6c74 7320  e size Defaults 
-00031060: 746f 2031 3030 2e0a 0a20 2020 2020 2020  to 100...       
-00031070: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00031080: 2020 2020 2020 5265 7370 6f6e 7365 3a20        Response: 
-00031090: 4365 6e74 7261 6c41 5049 2052 6573 706f  CentralAPI Respo
-000310a0: 6e73 6520 6f62 6a65 6374 0a20 2020 2020  nse object.     
-000310b0: 2020 2022 2222 0a20 2020 2020 2020 2075     """.        u
-000310c0: 726c 203d 2022 2f61 7069 2f72 6f75 7469  rl = "/api/routi
-000310d0: 6e67 2f76 312f 6f76 6572 6c61 792f 636f  ng/v1/overlay/co
-000310e0: 6e6e 6563 7469 6f6e 220a 0a20 2020 2020  nnection"..     
-000310f0: 2020 2070 6172 616d 7320 3d20 7b0a 2020     params = {.  
-00031100: 2020 2020 2020 2020 2020 2764 6576 6963            'devic
-00031110: 6527 3a20 6465 7669 6365 2c0a 2020 2020  e': device,.    
-00031120: 2020 2020 2020 2020 276d 6172 6b65 7227          'marker'
-00031130: 3a20 6d61 726b 6572 2c0a 2020 2020 2020  : marker,.      
-00031140: 2020 2020 2020 276c 696d 6974 273a 206c        'limit': l
-00031150: 696d 6974 0a20 2020 2020 2020 207d 0a0a  imit.        }..
-00031160: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00031170: 7761 6974 2073 656c 662e 6765 7428 7572  wait self.get(ur
-00031180: 6c2c 2070 6172 616d 733d 7061 7261 6d73  l, params=params
-00031190: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-000311a0: 2072 6573 6574 5f6f 7665 726c 6179 5f63   reset_overlay_c
-000311b0: 6f6e 6e65 6374 696f 6e28 0a20 2020 2020  onnection(.     
-000311c0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-000311d0: 2064 6576 6963 653a 2073 7472 2c0a 2020   device: str,.  
-000311e0: 2020 2920 2d3e 2052 6573 706f 6e73 653a    ) -> Response:
-000311f0: 0a20 2020 2020 2020 2022 2222 5265 7365  .        """Rese
-00031200: 7420 6f76 6572 6c61 7920 636f 6e74 726f  t overlay contro
-00031210: 6c20 636f 6e6e 6563 7469 6f6e 2e0a 0a20  l connection... 
-00031220: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00031230: 2020 2020 2020 2020 2064 6576 6963 6520           device 
-00031240: 2873 7472 293a 2044 6576 6963 6520 7365  (str): Device se
-00031250: 7269 616c 206e 756d 6265 720a 0a20 2020  rial number..   
-00031260: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00031270: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
-00031280: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
-00031290: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
-000312a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000312b0: 2020 2075 726c 203d 2022 2f61 7069 2f72     url = "/api/r
-000312c0: 6f75 7469 6e67 2f76 312f 6f76 6572 6c61  outing/v1/overla
-000312d0: 792f 636f 6e6e 6563 7469 6f6e 2f72 6573  y/connection/res
-000312e0: 6574 220a 0a20 2020 2020 2020 2070 6172  et"..        par
-000312f0: 616d 7320 3d20 7b0a 2020 2020 2020 2020  ams = {.        
-00031300: 2020 2020 2764 6576 6963 6527 3a20 6465      'device': de
-00031310: 7669 6365 0a20 2020 2020 2020 207d 0a0a  vice.        }..
-00031320: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00031330: 7761 6974 2073 656c 662e 7075 7428 7572  wait self.put(ur
-00031340: 6c2c 2070 6172 616d 733d 7061 7261 6d73  l, params=params
-00031350: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-00031360: 2067 6574 5f6f 7665 726c 6179 5f72 6f75   get_overlay_rou
-00031370: 7465 735f 6c65 6172 6e65 6428 0a20 2020  tes_learned(.   
-00031380: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00031390: 2020 2064 6576 6963 653a 2073 7472 2c0a     device: str,.
-000313a0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-000313b0: 2020 2062 6573 743a 2062 6f6f 6c20 3d20     best: bool = 
-000313c0: 4661 6c73 652c 0a20 2020 2020 2020 206d  False,.        m
-000313d0: 6172 6b65 723a 2073 7472 203d 204e 6f6e  arker: str = Non
-000313e0: 652c 0a20 2020 2020 2020 206c 696d 6974  e,.        limit
-000313f0: 3a20 696e 7420 3d20 3130 302c 0a20 2020  : int = 100,.   
-00031400: 2029 202d 3e20 5265 7370 6f6e 7365 3a0a   ) -> Response:.
-00031410: 2020 2020 2020 2020 2222 224c 6973 7420          """List 
-00031420: 6f66 206c 6561 726e 6564 2072 6f75 7465  of learned route
-00031430: 7320 6672 6f6d 206f 7665 726c 6179 2e0a  s from overlay..
-00031440: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00031450: 2020 2020 2020 2020 2020 2064 6576 6963             devic
-00031460: 6520 2873 7472 293a 2044 6576 6963 6520  e (str): Device 
-00031470: 7365 7269 616c 206e 756d 6265 720a 2020  serial number.  
-00031480: 2020 2020 2020 2020 2020 6265 7374 2028            best (
-00031490: 626f 6f6c 293a 2052 6574 7572 6e20 6f6e  bool): Return on
-000314a0: 6c79 2062 6573 7420 2f20 7072 6566 6572  ly best / prefer
-000314b0: 7265 6420 726f 7574 6573 0a20 2020 2020  red routes.     
-000314c0: 2020 2020 2020 206d 6172 6b65 7220 2873         marker (s
-000314d0: 7472 2c20 6f70 7469 6f6e 616c 293a 204f  tr, optional): O
-000314e0: 7061 7175 6520 6861 6e64 6c65 2074 6f20  paque handle to 
-000314f0: 6665 7463 6820 6e65 7874 2070 6167 650a  fetch next page.
-00031500: 2020 2020 2020 2020 2020 2020 6c69 6d69              limi
-00031510: 7420 2869 6e74 2c20 6f70 7469 6f6e 616c  t (int, optional
-00031520: 293a 2070 6167 6520 7369 7a65 2044 6566  ): page size Def
-00031530: 6175 6c74 7320 746f 2031 3030 2e0a 0a20  aults to 100... 
-00031540: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00031550: 2020 2020 2020 2020 2020 2020 5265 7370              Resp
-00031560: 6f6e 7365 3a20 4365 6e74 7261 6c41 5049  onse: CentralAPI
-00031570: 2052 6573 706f 6e73 6520 6f62 6a65 6374   Response object
-00031580: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00031590: 2020 2020 2075 726c 203d 2022 2f61 7069       url = "/api
-000315a0: 2f72 6f75 7469 6e67 2f76 312f 6f76 6572  /routing/v1/over
-000315b0: 6c61 792f 726f 7574 652f 6c65 6172 6e65  lay/route/learne
-000315c0: 6422 0a20 2020 2020 2020 2069 6620 6265  d".        if be
-000315d0: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
-000315e0: 7572 6c20 3d20 6627 7b75 726c 7d2f 6265  url = f'{url}/be
-000315f0: 7374 270a 0a20 2020 2020 2020 2070 6172  st'..        par
-00031600: 616d 7320 3d20 7b0a 2020 2020 2020 2020  ams = {.        
-00031610: 2020 2020 2764 6576 6963 6527 3a20 6465      'device': de
-00031620: 7669 6365 2c0a 2020 2020 2020 2020 2020  vice,.          
-00031630: 2020 276d 6172 6b65 7227 3a20 6d61 726b    'marker': mark
-00031640: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-00031650: 276c 696d 6974 273a 206c 696d 6974 0a20  'limit': limit. 
-00031660: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-00031670: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
-00031680: 656c 662e 6765 7428 7572 6c2c 2070 6172  elf.get(url, par
-00031690: 616d 733d 7061 7261 6d73 290a 0a20 2020  ams=params)..   
-000316a0: 2061 7379 6e63 2064 6566 2067 6574 5f6f   async def get_o
-000316b0: 7665 726c 6179 5f72 6f75 7465 735f 6164  verlay_routes_ad
-000316c0: 7665 7274 6973 6564 280a 2020 2020 2020  vertised(.      
-000316d0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000316e0: 6465 7669 6365 3a20 7374 722c 0a20 2020  device: str,.   
-000316f0: 2020 2020 206d 6172 6b65 723a 2073 7472       marker: str
-00031700: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00031710: 206c 696d 6974 3a20 696e 7420 3d20 3130   limit: int = 10
-00031720: 302c 0a20 2020 2029 202d 3e20 5265 7370  0,.    ) -> Resp
-00031730: 6f6e 7365 3a0a 2020 2020 2020 2020 2222  onse:.        ""
-00031740: 224c 6973 7420 6f66 2061 6476 6572 7469  "List of adverti
-00031750: 7365 6420 726f 7574 6573 2074 6f20 6f76  sed routes to ov
-00031760: 6572 6c61 792e 0a0a 2020 2020 2020 2020  erlay...        
-00031770: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00031780: 2020 6465 7669 6365 2028 7374 7229 3a20    device (str): 
-00031790: 4465 7669 6365 2073 6572 6961 6c20 6e75  Device serial nu
-000317a0: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
-000317b0: 206d 6172 6b65 7220 2873 7472 2c20 6f70   marker (str, op
-000317c0: 7469 6f6e 616c 293a 204f 7061 7175 6520  tional): Opaque 
-000317d0: 6861 6e64 6c65 2074 6f20 6665 7463 6820  handle to fetch 
-000317e0: 6e65 7874 2070 6167 650a 2020 2020 2020  next page.      
-000317f0: 2020 2020 2020 6c69 6d69 7420 2869 6e74        limit (int
-00031800: 2c20 6f70 7469 6f6e 616c 293a 2070 6167  , optional): pag
-00031810: 6520 7369 7a65 2044 6566 6175 6c74 7320  e size Defaults 
-00031820: 746f 2031 3030 2e0a 0a20 2020 2020 2020  to 100...       
-00031830: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00031840: 2020 2020 2020 5265 7370 6f6e 7365 3a20        Response: 
-00031850: 4365 6e74 7261 6c41 5049 2052 6573 706f  CentralAPI Respo
-00031860: 6e73 6520 6f62 6a65 6374 0a20 2020 2020  nse object.     
-00031870: 2020 2022 2222 0a20 2020 2020 2020 2075     """.        u
-00031880: 726c 203d 2022 2f61 7069 2f72 6f75 7469  rl = "/api/routi
-00031890: 6e67 2f76 312f 6f76 6572 6c61 792f 726f  ng/v1/overlay/ro
-000318a0: 7574 652f 6164 7665 7274 6973 6564 220a  ute/advertised".
-000318b0: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-000318c0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-000318d0: 2764 6576 6963 6527 3a20 6465 7669 6365  'device': device
-000318e0: 2c0a 2020 2020 2020 2020 2020 2020 276d  ,.            'm
-000318f0: 6172 6b65 7227 3a20 6d61 726b 6572 2c0a  arker': marker,.
-00031900: 2020 2020 2020 2020 2020 2020 276c 696d              'lim
-00031910: 6974 273a 206c 696d 6974 0a20 2020 2020  it': limit.     
-00031920: 2020 207d 0a0a 2020 2020 2020 2020 7265     }..        re
-00031930: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
-00031940: 6765 7428 7572 6c2c 2070 6172 616d 733d  get(url, params=
-00031950: 7061 7261 6d73 290a 0a20 2020 2061 7379  params)..    asy
-00031960: 6e63 2064 6566 2067 6574 5f6f 7665 726c  nc def get_overl
-00031970: 6179 5f69 6e74 6572 6661 6365 7328 0a20  ay_interfaces(. 
-00031980: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00031990: 2020 2020 2064 6576 6963 653a 2073 7472       device: str
-000319a0: 2c0a 2020 2020 2020 2020 6d61 726b 6572  ,.        marker
-000319b0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-000319c0: 2020 2020 2020 6c69 6d69 743a 2069 6e74        limit: int
-000319d0: 203d 2031 3030 2c0a 2020 2020 2920 2d3e   = 100,.    ) ->
-000319e0: 2052 6573 706f 6e73 653a 0a20 2020 2020   Response:.     
-000319f0: 2020 2022 2222 4c69 7374 206f 6620 6f76     """List of ov
-00031a00: 6572 6c61 7920 696e 7465 7266 6163 6573  erlay interfaces
-00031a10: 2028 7475 6e6e 656c 7329 2e0a 0a20 2020   (tunnels)...   
-00031a20: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00031a30: 2020 2020 2020 2064 6576 6963 6520 2873         device (s
-00031a40: 7472 293a 2044 6576 6963 6520 7365 7269  tr): Device seri
-00031a50: 616c 206e 756d 6265 720a 2020 2020 2020  al number.      
-00031a60: 2020 2020 2020 6d61 726b 6572 2028 7374        marker (st
-00031a70: 722c 206f 7074 696f 6e61 6c29 3a20 4f70  r, optional): Op
-00031a80: 6171 7565 2068 616e 646c 6520 746f 2066  aque handle to f
-00031a90: 6574 6368 206e 6578 7420 7061 6765 0a20  etch next page. 
-00031aa0: 2020 2020 2020 2020 2020 206c 696d 6974             limit
-00031ab0: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
-00031ac0: 3a20 7061 6765 2073 697a 6520 4465 6661  : page size Defa
-00031ad0: 756c 7473 2074 6f20 3130 302e 0a0a 2020  ults to 100...  
-00031ae0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00031af0: 2020 2020 2020 2020 2020 2052 6573 706f             Respo
-00031b00: 6e73 653a 2043 656e 7472 616c 4150 4920  nse: CentralAPI 
-00031b10: 5265 7370 6f6e 7365 206f 626a 6563 740a  Response object.
-00031b20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00031b30: 2020 2020 7572 6c20 3d20 222f 6170 692f      url = "/api/
-00031b40: 726f 7574 696e 672f 7631 2f6f 7665 726c  routing/v1/overl
-00031b50: 6179 2f69 6e74 6572 6661 6365 220a 0a20  ay/interface".. 
-00031b60: 2020 2020 2020 2070 6172 616d 7320 3d20         params = 
-00031b70: 7b0a 2020 2020 2020 2020 2020 2020 2764  {.            'd
-00031b80: 6576 6963 6527 3a20 6465 7669 6365 2c0a  evice': device,.
-00031b90: 2020 2020 2020 2020 2020 2020 276d 6172              'mar
-00031ba0: 6b65 7227 3a20 6d61 726b 6572 2c0a 2020  ker': marker,.  
-00031bb0: 2020 2020 2020 2020 2020 276c 696d 6974            'limit
-00031bc0: 273a 206c 696d 6974 0a20 2020 2020 2020  ': limit.       
-00031bd0: 207d 0a0a 2020 2020 2020 2020 7265 7475   }..        retu
-00031be0: 726e 2061 7761 6974 2073 656c 662e 6765  rn await self.ge
-00031bf0: 7428 7572 6c2c 2070 6172 616d 733d 7061  t(url, params=pa
-00031c00: 7261 6d73 290a 0a20 2020 2061 7379 6e63  rams)..    async
-00031c10: 2064 6566 2067 6574 5f64 656e 796c 6973   def get_denylis
-00031c20: 745f 636c 6965 6e74 7328 0a20 2020 2020  t_clients(.     
-00031c30: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00031c40: 2073 6572 6961 6c3a 2073 7472 2c0a 2020   serial: str,.  
-00031c50: 2020 2920 2d3e 2052 6573 706f 6e73 653a    ) -> Response:
-00031c60: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-00031c70: 616c 6c20 6465 6e79 6c69 7374 2063 6c69  all denylist cli
-00031c80: 656e 7420 6d61 6320 6164 6472 6573 7320  ent mac address 
-00031c90: 696e 2064 6576 6963 652e 0a0a 2020 2020  in device...    
-00031ca0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00031cb0: 2020 2020 2020 7365 7269 616c 2028 7374        serial (st
-00031cc0: 7229 3a20 4465 7669 6365 2069 6420 6f66  r): Device id of
-00031cd0: 2076 6972 7475 616c 2063 6f6e 7472 6f6c   virtual control
-00031ce0: 6c65 7220 2841 4f53 3820 4941 5029 206f  ler (AOS8 IAP) o
-00031cf0: 7220 7365 7269 616c 206f 6620 414f 5331  r serial of AOS1
-00031d00: 3020 6170 2e0a 2020 2020 2020 2020 2020  0 ap..          
-00031d10: 2020 2020 2020 4578 616d 706c 653a 3134        Example:14
-00031d20: 6233 3734 3363 3031 6638 3038 3062 6661  b3743c01f8080bfa
-00031d30: 3037 6361 3035 3365 6631 6538 3935 6466  07ca053ef1e895df
-00031d40: 3963 3036 3830 6665 3561 3137 6266 6435  9c0680fe5a17bfd5
-00031d50: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00031d60: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-00031d70: 6573 706f 6e73 653a 2043 656e 7472 616c  esponse: Central
-00031d80: 4150 4920 5265 7370 6f6e 7365 206f 626a  API Response obj
-00031d90: 6563 740a 2020 2020 2020 2020 2222 220a  ect.        """.
-00031da0: 2020 2020 2020 2020 7572 6c20 3d20 6622          url = f"
-00031db0: 2f63 6f6e 6669 6775 7261 7469 6f6e 2f76  /configuration/v
-00031dc0: 312f 7377 6172 6d2f 7b73 6572 6961 6c7d  1/swarm/{serial}
-00031dd0: 2f62 6c61 636b 6c69 7374 696e 6722 0a0a  /blacklisting"..
-00031de0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00031df0: 7761 6974 2073 656c 662e 6765 7428 7572  wait self.get(ur
-00031e00: 6c29 0a0a 0a20 2020 2061 7379 6e63 2064  l)...    async d
-00031e10: 6566 2067 6574 5f61 7574 6f5f 7375 6273  ef get_auto_subs
-00031e20: 6372 6962 6528 0a20 2020 2020 2020 2073  cribe(.        s
-00031e30: 656c 662c 0a20 2020 2029 202d 3e20 5265  elf,.    ) -> Re
-00031e40: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
-00031e50: 2222 2247 6574 2074 6865 2073 6572 7669  """Get the servi
-00031e60: 6365 7320 7768 6963 6820 6861 7665 2061  ces which have a
-00031e70: 7574 6f20 7375 6273 6372 6962 6520 656e  uto subscribe en
-00031e80: 6162 6c65 642e 0a0a 2020 2020 2020 2020  abled...        
-00031e90: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00031ea0: 2020 2020 2052 6573 706f 6e73 653a 2043       Response: C
-00031eb0: 656e 7472 616c 4150 4920 5265 7370 6f6e  entralAPI Respon
-00031ec0: 7365 206f 626a 6563 740a 2020 2020 2020  se object.      
-00031ed0: 2020 2222 220a 2020 2020 2020 2020 7572    """.        ur
-00031ee0: 6c20 3d20 222f 706c 6174 666f 726d 2f6c  l = "/platform/l
-00031ef0: 6963 656e 7369 6e67 2f76 312f 6375 7374  icensing/v1/cust
-00031f00: 6f6d 6572 2f73 6574 7469 6e67 732f 6175  omer/settings/au
-00031f10: 746f 6c69 6365 6e73 6522 0a0a 2020 2020  tolicense"..    
-00031f20: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-00031f30: 2073 656c 662e 6765 7428 7572 6c29 0a0a   self.get(url)..
-00031f40: 2020 2020 6173 796e 6320 6465 6620 656e      async def en
-00031f50: 6162 6c65 5f61 7574 6f5f 7375 6273 6372  able_auto_subscr
-00031f60: 6962 6528 0a20 2020 2020 2020 2073 656c  ibe(.        sel
-00031f70: 662c 0a20 2020 2020 2020 2073 6572 7669  f,.        servi
-00031f80: 6365 733a 204c 6973 745b 7374 725d 207c  ces: List[str] |
-00031f90: 2073 7472 2c0a 2020 2020 2920 2d3e 2052   str,.    ) -> R
-00031fa0: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
-00031fb0: 2022 2222 5374 616e 6461 6c6f 6e65 2043   """Standalone C
-00031fc0: 7573 746f 6d65 7220 4150 493a 2041 7373  ustomer API: Ass
-00031fd0: 6967 6e20 6c69 6365 6e73 6573 2074 6f20  ign licenses to 
-00031fe0: 616c 6c20 6465 7669 6365 7320 616e 6420  all devices and 
-00031ff0: 656e 6162 6c65 2061 7574 6f20 7375 6273  enable auto subs
-00032000: 6372 6962 6520 666f 720a 2020 2020 2020  cribe for.      
-00032010: 2020 6769 7665 6e20 7365 7276 6963 6573    given services
-00032020: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00032030: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
-00032040: 7669 6365 7320 284c 6973 745b 7374 725d  vices (List[str]
-00032050: 293a 206c 6973 7420 6f66 2073 6572 7669  ): list of servi
-00032060: 6365 7320 652e 672e 205b 2770 6127 2c20  ces e.g. ['pa', 
-00032070: 2775 6363 272c 2066 6f75 6e64 6174 696f  'ucc', foundatio
-00032080: 6e5f 6170 2c0a 2020 2020 2020 2020 2020  n_ap,.          
-00032090: 2020 2020 2020 6164 7661 6e63 6564 5f73        advanced_s
-000320a0: 7769 7463 685f 3632 3030 2c20 666f 756e  witch_6200, foun
-000320b0: 6461 7469 6f6e 5f37 3058 5820 6574 6320  dation_70XX etc 
-000320c0: 2e2e 2e5d 2e20 4368 6563 6b0a 2020 2020  ...]. Check.    
-000320d0: 2020 2020 2020 2020 2020 2020 2f70 6c61              /pla
-000320e0: 7466 6f72 6d2f 6c69 6365 6e73 696e 672f  tform/licensing/
-000320f0: 7631 2f73 6572 7669 6365 732f 636f 6e66  v1/services/conf
-00032100: 6967 2041 5049 2072 6573 706f 6e73 6520  ig API response 
-00032110: 746f 206b 6e6f 7720 7468 6520 6c69 7374  to know the list
-00032120: 206f 6620 7375 7070 6f72 7465 640a 2020   of supported.  
-00032130: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00032140: 7276 6963 6573 2e0a 0a20 2020 2020 2020  rvices...       
-00032150: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00032160: 2020 2020 2020 5265 7370 6f6e 7365 3a20        Response: 
-00032170: 4365 6e74 7261 6c41 5049 2052 6573 706f  CentralAPI Respo
-00032180: 6e73 6520 6f62 6a65 6374 0a20 2020 2020  nse object.     
-00032190: 2020 2022 2222 0a20 2020 2020 2020 2075     """.        u
-000321a0: 726c 203d 2022 2f70 6c61 7466 6f72 6d2f  rl = "/platform/
-000321b0: 6c69 6365 6e73 696e 672f 7631 2f63 7573  licensing/v1/cus
-000321c0: 746f 6d65 722f 7365 7474 696e 6773 2f61  tomer/settings/a
-000321d0: 7574 6f6c 6963 656e 7365 220a 0a20 2020  utolicense"..   
-000321e0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-000321f0: 6365 2873 6572 7669 6365 732c 2073 7472  ce(services, str
-00032200: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00032210: 6572 7669 6365 7320 3d20 5b73 6572 7669  ervices = [servi
-00032220: 6365 735d 0a0a 2020 2020 2020 2020 6a73  ces]..        js
-00032230: 6f6e 5f64 6174 6120 3d20 7b0a 2020 2020  on_data = {.    
-00032240: 2020 2020 2020 2020 2773 6572 7669 6365          'service
-00032250: 7327 3a20 7365 7276 6963 6573 0a20 2020  s': services.   
-00032260: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-00032270: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
-00032280: 662e 706f 7374 2875 726c 2c20 6a73 6f6e  f.post(url, json
-00032290: 5f64 6174 613d 6a73 6f6e 5f64 6174 6129  _data=json_data)
-000322a0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-000322b0: 6469 7361 626c 655f 6175 746f 5f73 7562  disable_auto_sub
-000322c0: 7363 7269 6265 280a 2020 2020 2020 2020  scribe(.        
-000322d0: 7365 6c66 2c0a 2020 2020 2020 2020 7365  self,.        se
-000322e0: 7276 6963 6573 3a20 4c69 7374 5b73 7472  rvices: List[str
-000322f0: 5d20 7c20 7374 722c 0a20 2020 2029 202d  ] | str,.    ) -
-00032300: 3e20 5265 7370 6f6e 7365 3a0a 2020 2020  > Response:.    
-00032310: 2020 2020 2222 2253 7461 6e64 616c 6f6e      """Standalon
-00032320: 6520 4375 7374 6f6d 6572 2041 5049 3a20  e Customer API: 
-00032330: 4469 7361 626c 6520 6175 746f 206c 6963  Disable auto lic
-00032340: 656e 7369 6e67 2066 6f72 2067 6976 656e  ensing for given
-00032350: 2073 6572 7669 6365 732e 0a0a 2020 2020   services...    
-00032360: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00032370: 2020 2020 2020 7365 7276 6963 6573 2028        services (
-00032380: 4c69 7374 5b73 7472 5d29 3a20 6c69 7374  List[str]): list
-00032390: 206f 6620 7365 7276 6963 6573 2065 2e67   of services e.g
-000323a0: 2e20 5b27 7061 272c 2027 7563 6327 2c20  . ['pa', 'ucc', 
-000323b0: 666f 756e 6461 7469 6f6e 5f61 702c 0a20  foundation_ap,. 
-000323c0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000323d0: 6476 616e 6365 645f 7377 6974 6368 5f36  dvanced_switch_6
-000323e0: 3230 302c 2066 6f75 6e64 6174 696f 6e5f  200, foundation_
-000323f0: 3730 5858 2065 7463 202e 2e2e 5d2e 2043  70XX etc ...]. C
-00032400: 6865 636b 0a20 2020 2020 2020 2020 2020  heck.           
-00032410: 2020 2020 202f 706c 6174 666f 726d 2f6c       /platform/l
-00032420: 6963 656e 7369 6e67 2f76 312f 7365 7276  icensing/v1/serv
-00032430: 6963 6573 2f63 6f6e 6669 6720 4150 4920  ices/config API 
-00032440: 7265 7370 6f6e 7365 2074 6f20 6b6e 6f77  response to know
-00032450: 2074 6865 206c 6973 7420 6f66 2073 7570   the list of sup
-00032460: 706f 7274 6564 0a20 2020 2020 2020 2020  ported.         
-00032470: 2020 2020 2020 2073 6572 7669 6365 732e         services.
-00032480: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00032490: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-000324a0: 6573 706f 6e73 653a 2043 656e 7472 616c  esponse: Central
-000324b0: 4150 4920 5265 7370 6f6e 7365 206f 626a  API Response obj
-000324c0: 6563 740a 2020 2020 2020 2020 2222 220a  ect.        """.
-000324d0: 2020 2020 2020 2020 7572 6c20 3d20 222f          url = "/
-000324e0: 706c 6174 666f 726d 2f6c 6963 656e 7369  platform/licensi
-000324f0: 6e67 2f76 312f 6375 7374 6f6d 6572 2f73  ng/v1/customer/s
-00032500: 6574 7469 6e67 732f 6175 746f 6c69 6365  ettings/autolice
-00032510: 6e73 6522 0a0a 2020 2020 2020 2020 6966  nse"..        if
-00032520: 2069 7369 6e73 7461 6e63 6528 7365 7276   isinstance(serv
-00032530: 6963 6573 2c20 7374 7229 3a0a 2020 2020  ices, str):.    
-00032540: 2020 2020 2020 2020 7365 7276 6963 6573          services
-00032550: 203d 205b 7365 7276 6963 6573 5d0a 0a20   = [services].. 
-00032560: 2020 2020 2020 206a 736f 6e5f 6461 7461         json_data
-00032570: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-00032580: 2027 7365 7276 6963 6573 273a 2073 6572   'services': ser
-00032590: 7669 6365 730a 2020 2020 2020 2020 7d0a  vices.        }.
-000325a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000325b0: 6177 6169 7420 7365 6c66 2e64 656c 6574  await self.delet
-000325c0: 6528 7572 6c2c 206a 736f 6e5f 6461 7461  e(url, json_data
-000325d0: 3d6a 736f 6e5f 6461 7461 290a 0a20 2020  =json_data)..   
-000325e0: 2023 202f 2f20 2d2d 204e 6f74 2075 7365   # // -- Not use
-000325f0: 6420 6279 2063 6f6d 6d61 6e64 7320 7965  d by commands ye
-00032600: 742e 2020 756e 646f 6375 6d65 6e74 6564  t.  undocumented
-00032610: 206b 6d73 2061 7069 202d 2d20 2f2f 0a20   kms api -- //. 
-00032620: 2020 2061 7379 6e63 2064 6566 206b 6d73     async def kms
-00032630: 5f67 6574 5f73 796e 6365 645f 6170 7328  _get_synced_aps(
-00032640: 7365 6c66 2c20 6d61 633a 2073 7472 2920  self, mac: str) 
-00032650: 2d3e 2052 6573 706f 6e73 653a 0a20 2020  -> Response:.   
-00032660: 2020 2020 2075 726c 203d 2066 222f 6b65       url = f"/ke
-00032670: 796d 676d 742f 7631 2f73 796e 6365 6461  ymgmt/v1/synceda
-00032680: 706c 6973 742f 7b6d 6163 7d22 0a20 2020  plist/{mac}".   
-00032690: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
-000326a0: 7420 7365 6c66 2e67 6574 2875 726c 290a  t self.get(url).
-000326b0: 0a20 2020 2061 7379 6e63 2064 6566 206b  .    async def k
-000326c0: 6d73 5f67 6574 5f63 6c69 656e 745f 7265  ms_get_client_re
-000326d0: 636f 7264 2873 656c 662c 206d 6163 3a20  cord(self, mac: 
-000326e0: 7374 7229 202d 3e20 5265 7370 6f6e 7365  str) -> Response
-000326f0: 3a0a 2020 2020 2020 2020 7572 6c20 3d20  :.        url = 
-00032700: 6622 2f6b 6579 6d67 6d74 2f76 312f 6b65  f"/keymgmt/v1/ke
-00032710: 7963 6163 6865 2f7b 6d61 637d 220a 2020  ycache/{mac}".  
-00032720: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
-00032730: 6974 2073 656c 662e 6765 7428 7572 6c29  it self.get(url)
-00032740: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-00032750: 6b6d 735f 6765 745f 6861 7368 2873 656c  kms_get_hash(sel
-00032760: 6629 202d 3e20 5265 7370 6f6e 7365 3a0a  f) -> Response:.
-00032770: 2020 2020 2020 2020 7572 6c20 3d20 222f          url = "/
-00032780: 6b65 796d 676d 742f 7631 2f6b 6579 6861  keymgmt/v1/keyha
-00032790: 7368 220a 2020 2020 2020 2020 7265 7475  sh".        retu
-000327a0: 726e 2061 7761 6974 2073 656c 662e 6765  rn await self.ge
-000327b0: 7428 7572 6c29 0a0a 2020 2020 6173 796e  t(url)..    asyn
-000327c0: 6320 6465 6620 6b6d 735f 6765 745f 6170  c def kms_get_ap
-000327d0: 5f73 7461 7465 2873 656c 662c 2073 6572  _state(self, ser
-000327e0: 6961 6c3a 2073 7472 2920 2d3e 2052 6573  ial: str) -> Res
-000327f0: 706f 6e73 653a 0a20 2020 2020 2020 2075  ponse:.        u
-00032800: 726c 203d 2066 222f 6b65 796d 676d 742f  rl = f"/keymgmt/
-00032810: 7631 2f53 7461 7473 2f61 702f 7b73 6572  v1/Stats/ap/{ser
-00032820: 6961 6c7d 220a 2020 2020 2020 2020 7265  ial}".        re
-00032830: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
-00032840: 6765 7428 7572 6c29 0a0a 2020 2020 2320  get(url)..    # 
-00032850: 4261 6420 656e 6470 6f69 6e74 2055 524c  Bad endpoint URL
-00032860: 2034 3034 0a20 2020 2061 7379 6e63 2064   404.    async d
-00032870: 6566 206b 6d73 5f67 6574 5f68 6561 6c74  ef kms_get_healt
-00032880: 6828 7365 6c66 2920 2d3e 2052 6573 706f  h(self) -> Respo
-00032890: 6e73 653a 0a20 2020 2020 2020 2075 726c  nse:.        url
-000328a0: 203d 2022 2f6b 6579 6d67 6d74 2f76 312f   = "/keymgmt/v1/
-000328b0: 6865 616c 7468 220a 2020 2020 2020 2020  health".        
-000328c0: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
-000328d0: 662e 6765 7428 7572 6c29 0a0a 6966 205f  f.get(url)..if _
-000328e0: 5f6e 616d 655f 5f20 3d3d 2022 5f5f 6d61  _name__ == "__ma
-000328f0: 696e 5f5f 223a 0a20 2020 2070 6173 730a  in__":.    pass.
+0002a410: 2065 6e64 3a20 696e 7420 3d20 4e6f 6e65   end: int = None
+0002a420: 2c0a 2020 2020 2020 2020 7377 6172 6d5f  ,.        swarm_
+0002a430: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+0002a440: 2020 2020 2020 2020 6672 6f6d 5f74 696d          from_tim
+0002a450: 6573 7461 6d70 3a20 696e 7420 3d20 4e6f  estamp: int = No
+0002a460: 6e65 2c0a 2020 2020 2020 2020 746f 5f74  ne,.        to_t
+0002a470: 696d 6573 7461 6d70 3a20 696e 7420 3d20  imestamp: int = 
+0002a480: 4e6f 6e65 2c0a 2020 2020 2020 2020 6f66  None,.        of
+0002a490: 6673 6574 3a20 696e 7420 3d20 302c 0a20  fset: int = 0,. 
+0002a4a0: 2020 2020 2020 206c 696d 6974 3a20 696e         limit: in
+0002a4b0: 7420 3d20 3130 300a 2020 2020 2920 2d3e  t = 100.    ) ->
+0002a4c0: 2052 6573 706f 6e73 653a 0a20 2020 2020   Response:.     
+0002a4d0: 2020 2022 2222 4c69 7374 2073 7573 7065     """List suspe
+0002a4e0: 6374 2041 5073 2e0a 0a20 2020 2020 2020  ct APs...       
+0002a4f0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0002a500: 2020 2067 726f 7570 2028 4c69 7374 5b73     group (List[s
+0002a510: 7472 5d2c 206f 7074 696f 6e61 6c29 3a20  tr], optional): 
+0002a520: 4c69 7374 206f 6620 6772 6f75 7020 6e61  List of group na
+0002a530: 6d65 730a 2020 2020 2020 2020 2020 2020  mes.            
+0002a540: 6c61 6265 6c20 284c 6973 745b 7374 725d  label (List[str]
+0002a550: 2c20 6f70 7469 6f6e 616c 293a 204c 6973  , optional): Lis
+0002a560: 7420 6f66 206c 6162 656c 206e 616d 6573  t of label names
+0002a570: 0a20 2020 2020 2020 2020 2020 2073 6974  .            sit
+0002a580: 6520 284c 6973 745b 7374 725d 2c20 6f70  e (List[str], op
+0002a590: 7469 6f6e 616c 293a 204c 6973 7420 6f66  tional): List of
+0002a5a0: 2073 6974 6520 6e61 6d65 730a 2020 2020   site names.    
+0002a5b0: 2020 2020 2020 2020 7374 6172 7420 2869          start (i
+0002a5c0: 6e74 2c20 6f70 7469 6f6e 616c 293a 204e  nt, optional): N
+0002a5d0: 6565 6420 696e 666f 726d 6174 696f 6e20  eed information 
+0002a5e0: 6672 6f6d 2074 6869 7320 7469 6d65 7374  from this timest
+0002a5f0: 616d 702e 2054 696d 6573 7461 6d70 2069  amp. Timestamp i
+0002a600: 7320 6570 6f63 6820 696e 0a20 2020 2020  s epoch in.     
+0002a610: 2020 2020 2020 2020 2020 206d 696c 6c69             milli
+0002a620: 7365 636f 6e64 732e 2044 6566 6175 6c74  seconds. Default
+0002a630: 2069 7320 6375 7272 656e 7420 7469 6d65   is current time
+0002a640: 7374 616d 7020 6d69 6e75 7320 3320 686f  stamp minus 3 ho
+0002a650: 7572 730a 2020 2020 2020 2020 2020 2020  urs.            
+0002a660: 656e 6420 2869 6e74 2c20 6f70 7469 6f6e  end (int, option
+0002a670: 616c 293a 204e 6565 6420 696e 666f 726d  al): Need inform
+0002a680: 6174 696f 6e20 746f 2074 6869 7320 7469  ation to this ti
+0002a690: 6d65 7374 616d 702e 2054 696d 6573 7461  mestamp. Timesta
+0002a6a0: 6d70 2069 7320 6570 6f63 6820 696e 0a20  mp is epoch in. 
+0002a6b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0002a6c0: 696c 6c69 7365 636f 6e64 732e 2044 6566  illiseconds. Def
+0002a6d0: 6175 6c74 2069 7320 6375 7272 656e 7420  ault is current 
+0002a6e0: 7469 6d65 7374 616d 700a 2020 2020 2020  timestamp.      
+0002a6f0: 2020 2020 2020 7377 6172 6d5f 6964 2028        swarm_id (
+0002a700: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+0002a710: 4669 6c74 6572 2062 7920 5377 6172 6d20  Filter by Swarm 
+0002a720: 4944 0a20 2020 2020 2020 2020 2020 2066  ID.            f
+0002a730: 726f 6d5f 7469 6d65 7374 616d 7020 2869  rom_timestamp (i
+0002a740: 6e74 2c20 6f70 7469 6f6e 616c 293a 2054  nt, optional): T
+0002a750: 6869 7320 7061 7261 6d65 7465 7220 7375  his parameter su
+0002a760: 7065 7263 6564 6573 2073 7461 7274 2070  percedes start p
+0002a770: 6172 616d 6574 6572 2e20 4e65 6564 0a20  arameter. Need. 
+0002a780: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0002a790: 6e66 6f72 6d61 7469 6f6e 2066 726f 6d20  nformation from 
+0002a7a0: 7468 6973 2074 696d 6573 7461 6d70 2e20  this timestamp. 
+0002a7b0: 5469 6d65 7374 616d 7020 6973 2065 706f  Timestamp is epo
+0002a7c0: 6368 2069 6e20 7365 636f 6e64 732e 2044  ch in seconds. D
+0002a7d0: 6566 6175 6c74 2069 7320 6375 7272 656e  efault is curren
+0002a7e0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0002a7f0: 2020 5554 4320 7469 6d65 7374 616d 7020    UTC timestamp 
+0002a800: 6d69 6e75 7320 3320 686f 7572 730a 2020  minus 3 hours.  
+0002a810: 2020 2020 2020 2020 2020 746f 5f74 696d            to_tim
+0002a820: 6573 7461 6d70 2028 696e 742c 206f 7074  estamp (int, opt
+0002a830: 696f 6e61 6c29 3a20 5468 6973 2070 6172  ional): This par
+0002a840: 616d 6574 6572 2073 7570 6572 6365 6465  ameter supercede
+0002a850: 7320 656e 6420 7061 7261 6d65 7465 722e  s end parameter.
+0002a860: 204e 6565 6420 696e 666f 726d 6174 696f   Need informatio
+0002a870: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+0002a880: 2020 746f 2074 6869 7320 7469 6d65 7374    to this timest
+0002a890: 616d 702e 2054 696d 6573 7461 6d70 2069  amp. Timestamp i
+0002a8a0: 7320 6570 6f63 6820 696e 2073 6563 6f6e  s epoch in secon
+0002a8b0: 6473 2e20 4465 6661 756c 7420 6973 2063  ds. Default is c
+0002a8c0: 7572 7265 6e74 2055 5443 2074 696d 6573  urrent UTC times
+0002a8d0: 7461 6d70 0a20 2020 2020 2020 2020 2020  tamp.           
+0002a8e0: 206f 6666 7365 7420 2869 6e74 2c20 6f70   offset (int, op
+0002a8f0: 7469 6f6e 616c 293a 2050 6167 696e 6174  tional): Paginat
+0002a900: 696f 6e20 6f66 6673 6574 2028 6465 6661  ion offset (defa
+0002a910: 756c 7420 3d20 3029 2044 6566 6175 6c74  ult = 0) Default
+0002a920: 7320 746f 2030 2e0a 2020 2020 2020 2020  s to 0..        
+0002a930: 2020 2020 6c69 6d69 7420 2869 6e74 2c20      limit (int, 
+0002a940: 6f70 7469 6f6e 616c 293a 2070 6167 696e  optional): pagin
+0002a950: 6174 696f 6e20 7369 7a65 2028 6465 6661  ation size (defa
+0002a960: 756c 7420 3d20 3130 3029 2044 6566 6175  ult = 100) Defau
+0002a970: 6c74 7320 746f 2031 3030 2e0a 0a20 2020  lts to 100...   
+0002a980: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+0002a990: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
+0002a9a0: 7365 3a20 4365 6e74 7261 6c41 5049 2052  se: CentralAPI R
+0002a9b0: 6573 706f 6e73 6520 6f62 6a65 6374 0a20  esponse object. 
+0002a9c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0002a9d0: 2020 2075 726c 203d 2022 2f72 6170 6964     url = "/rapid
+0002a9e0: 732f 7631 2f73 7573 7065 6374 5f61 7073  s/v1/suspect_aps
+0002a9f0: 220a 0a20 2020 2020 2020 2070 6172 616d  "..        param
+0002aa00: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
+0002aa10: 2020 2767 726f 7570 273a 2067 726f 7570    'group': group
+0002aa20: 2c0a 2020 2020 2020 2020 2020 2020 276c  ,.            'l
+0002aa30: 6162 656c 273a 206c 6162 656c 2c0a 2020  abel': label,.  
+0002aa40: 2020 2020 2020 2020 2020 2773 6974 6527            'site'
+0002aa50: 3a20 7369 7465 2c0a 2020 2020 2020 2020  : site,.        
+0002aa60: 2020 2020 2773 7461 7274 273a 2073 7461      'start': sta
+0002aa70: 7274 2c0a 2020 2020 2020 2020 2020 2020  rt,.            
+0002aa80: 2765 6e64 273a 2065 6e64 2c0a 2020 2020  'end': end,.    
+0002aa90: 2020 2020 2020 2020 2773 7761 726d 5f69          'swarm_i
+0002aaa0: 6427 3a20 7377 6172 6d5f 6964 2c0a 2020  d': swarm_id,.  
+0002aab0: 2020 2020 2020 2020 2020 2766 726f 6d5f            'from_
+0002aac0: 7469 6d65 7374 616d 7027 3a20 6672 6f6d  timestamp': from
+0002aad0: 5f74 696d 6573 7461 6d70 2c0a 2020 2020  _timestamp,.    
+0002aae0: 2020 2020 2020 2020 2774 6f5f 7469 6d65          'to_time
+0002aaf0: 7374 616d 7027 3a20 746f 5f74 696d 6573  stamp': to_times
+0002ab00: 7461 6d70 2c0a 2020 2020 2020 2020 2020  tamp,.          
+0002ab10: 2020 276f 6666 7365 7427 3a20 6f66 6673    'offset': offs
+0002ab20: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
+0002ab30: 276c 696d 6974 273a 206c 696d 6974 0a20  'limit': limit. 
+0002ab40: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+0002ab50: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
+0002ab60: 656c 662e 6765 7428 7572 6c2c 2070 6172  elf.get(url, par
+0002ab70: 616d 733d 7061 7261 6d73 290a 0a20 2020  ams=params)..   
+0002ab80: 2061 7379 6e63 2064 6566 2077 6964 735f   async def wids_
+0002ab90: 6765 745f 6e65 6967 6862 6f72 5f61 7073  get_neighbor_aps
+0002aba0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0002abb0: 2020 2020 2020 2020 6772 6f75 703a 204c          group: L
+0002abc0: 6973 745b 7374 725d 203d 204e 6f6e 652c  ist[str] = None,
+0002abd0: 0a20 2020 2020 2020 206c 6162 656c 3a20  .        label: 
+0002abe0: 4c69 7374 5b73 7472 5d20 3d20 4e6f 6e65  List[str] = None
+0002abf0: 2c0a 2020 2020 2020 2020 7369 7465 3a20  ,.        site: 
+0002ac00: 4c69 7374 5b73 7472 5d20 3d20 4e6f 6e65  List[str] = None
+0002ac10: 2c0a 2020 2020 2020 2020 7374 6172 743a  ,.        start:
+0002ac20: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
+0002ac30: 2020 2020 2065 6e64 3a20 696e 7420 3d20       end: int = 
+0002ac40: 4e6f 6e65 2c0a 2020 2020 2020 2020 7377  None,.        sw
+0002ac50: 6172 6d5f 6964 3a20 7374 7220 3d20 4e6f  arm_id: str = No
+0002ac60: 6e65 2c0a 2020 2020 2020 2020 6672 6f6d  ne,.        from
+0002ac70: 5f74 696d 6573 7461 6d70 3a20 696e 7420  _timestamp: int 
+0002ac80: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0002ac90: 746f 5f74 696d 6573 7461 6d70 3a20 696e  to_timestamp: in
+0002aca0: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
+0002acb0: 2020 6f66 6673 6574 3a20 696e 7420 3d20    offset: int = 
+0002acc0: 302c 0a20 2020 2020 2020 206c 696d 6974  0,.        limit
+0002acd0: 3a20 696e 7420 3d20 3130 300a 2020 2020  : int = 100.    
+0002ace0: 2920 2d3e 2052 6573 706f 6e73 653a 0a20  ) -> Response:. 
+0002acf0: 2020 2020 2020 2022 2222 4c69 7374 206e         """List n
+0002ad00: 6569 6768 626f 7220 4150 732e 0a0a 2020  eighbor APs...  
+0002ad10: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+0002ad20: 2020 2020 2020 2020 6772 6f75 7020 284c          group (L
+0002ad30: 6973 745b 7374 725d 2c20 6f70 7469 6f6e  ist[str], option
+0002ad40: 616c 293a 204c 6973 7420 6f66 2067 726f  al): List of gro
+0002ad50: 7570 206e 616d 6573 0a20 2020 2020 2020  up names.       
+0002ad60: 2020 2020 206c 6162 656c 2028 4c69 7374       label (List
+0002ad70: 5b73 7472 5d2c 206f 7074 696f 6e61 6c29  [str], optional)
+0002ad80: 3a20 4c69 7374 206f 6620 6c61 6265 6c20  : List of label 
+0002ad90: 6e61 6d65 730a 2020 2020 2020 2020 2020  names.          
+0002ada0: 2020 7369 7465 2028 4c69 7374 5b73 7472    site (List[str
+0002adb0: 5d2c 206f 7074 696f 6e61 6c29 3a20 4c69  ], optional): Li
+0002adc0: 7374 206f 6620 7369 7465 206e 616d 6573  st of site names
+0002add0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+0002ade0: 7274 2028 696e 742c 206f 7074 696f 6e61  rt (int, optiona
+0002adf0: 6c29 3a20 4e65 6564 2069 6e66 6f72 6d61  l): Need informa
+0002ae00: 7469 6f6e 2066 726f 6d20 7468 6973 2074  tion from this t
+0002ae10: 696d 6573 7461 6d70 2e20 5469 6d65 7374  imestamp. Timest
+0002ae20: 616d 7020 6973 2065 706f 6368 2069 6e0a  amp is epoch in.
+0002ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ae40: 6d69 6c6c 6973 6563 6f6e 6473 2e20 4465  milliseconds. De
+0002ae50: 6661 756c 7420 6973 2063 7572 7265 6e74  fault is current
+0002ae60: 2074 696d 6573 7461 6d70 206d 696e 7573   timestamp minus
+0002ae70: 2033 2068 6f75 7273 0a20 2020 2020 2020   3 hours.       
+0002ae80: 2020 2020 2065 6e64 2028 696e 742c 206f       end (int, o
+0002ae90: 7074 696f 6e61 6c29 3a20 4e65 6564 2069  ptional): Need i
+0002aea0: 6e66 6f72 6d61 7469 6f6e 2074 6f20 7468  nformation to th
+0002aeb0: 6973 2074 696d 6573 7461 6d70 2e20 5469  is timestamp. Ti
+0002aec0: 6d65 7374 616d 7020 6973 2065 706f 6368  mestamp is epoch
+0002aed0: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
+0002aee0: 2020 2020 6d69 6c6c 6973 6563 6f6e 6473      milliseconds
+0002aef0: 2e20 4465 6661 756c 7420 6973 2063 7572  . Default is cur
+0002af00: 7265 6e74 2074 696d 6573 7461 6d70 0a20  rent timestamp. 
+0002af10: 2020 2020 2020 2020 2020 2073 7761 726d             swarm
+0002af20: 5f69 6420 2873 7472 2c20 6f70 7469 6f6e  _id (str, option
+0002af30: 616c 293a 2046 696c 7465 7220 6279 2053  al): Filter by S
+0002af40: 7761 726d 2049 440a 2020 2020 2020 2020  warm ID.        
+0002af50: 2020 2020 6672 6f6d 5f74 696d 6573 7461      from_timesta
+0002af60: 6d70 2028 696e 742c 206f 7074 696f 6e61  mp (int, optiona
+0002af70: 6c29 3a20 5468 6973 2070 6172 616d 6574  l): This paramet
+0002af80: 6572 2073 7570 6572 6365 6465 7320 7374  er supercedes st
+0002af90: 6172 7420 7061 7261 6d65 7465 722e 204e  art parameter. N
+0002afa0: 6565 640a 2020 2020 2020 2020 2020 2020  eed.            
+0002afb0: 2020 2020 696e 666f 726d 6174 696f 6e20      information 
+0002afc0: 6672 6f6d 2074 6869 7320 7469 6d65 7374  from this timest
+0002afd0: 616d 702e 2054 696d 6573 7461 6d70 2069  amp. Timestamp i
+0002afe0: 7320 6570 6f63 6820 696e 2073 6563 6f6e  s epoch in secon
+0002aff0: 6473 2e20 4465 6661 756c 7420 6973 2063  ds. Default is c
+0002b000: 7572 7265 6e74 0a20 2020 2020 2020 2020  urrent.         
+0002b010: 2020 2020 2020 2055 5443 2074 696d 6573         UTC times
+0002b020: 7461 6d70 206d 696e 7573 2033 2068 6f75  tamp minus 3 hou
+0002b030: 7273 0a20 2020 2020 2020 2020 2020 2074  rs.            t
+0002b040: 6f5f 7469 6d65 7374 616d 7020 2869 6e74  o_timestamp (int
+0002b050: 2c20 6f70 7469 6f6e 616c 293a 2054 6869  , optional): Thi
+0002b060: 7320 7061 7261 6d65 7465 7220 7375 7065  s parameter supe
+0002b070: 7263 6564 6573 2065 6e64 2070 6172 616d  rcedes end param
+0002b080: 6574 6572 2e20 4e65 6564 2069 6e66 6f72  eter. Need infor
+0002b090: 6d61 7469 6f6e 0a20 2020 2020 2020 2020  mation.         
+0002b0a0: 2020 2020 2020 2074 6f20 7468 6973 2074         to this t
+0002b0b0: 696d 6573 7461 6d70 2e20 5469 6d65 7374  imestamp. Timest
+0002b0c0: 616d 7020 6973 2065 706f 6368 2069 6e20  amp is epoch in 
+0002b0d0: 7365 636f 6e64 732e 2044 6566 6175 6c74  seconds. Default
+0002b0e0: 2069 7320 6375 7272 656e 7420 5554 4320   is current UTC 
+0002b0f0: 7469 6d65 7374 616d 700a 2020 2020 2020  timestamp.      
+0002b100: 2020 2020 2020 6f66 6673 6574 2028 696e        offset (in
+0002b110: 742c 206f 7074 696f 6e61 6c29 3a20 5061  t, optional): Pa
+0002b120: 6769 6e61 7469 6f6e 206f 6666 7365 7420  gination offset 
+0002b130: 2864 6566 6175 6c74 203d 2030 2920 4465  (default = 0) De
+0002b140: 6661 756c 7473 2074 6f20 302e 0a20 2020  faults to 0..   
+0002b150: 2020 2020 2020 2020 206c 696d 6974 2028           limit (
+0002b160: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
+0002b170: 7061 6769 6e61 7469 6f6e 2073 697a 6520  pagination size 
+0002b180: 2864 6566 6175 6c74 203d 2031 3030 2920  (default = 100) 
+0002b190: 4465 6661 756c 7473 2074 6f20 3130 302e  Defaults to 100.
+0002b1a0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0002b1b0: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
+0002b1c0: 6573 706f 6e73 653a 2043 656e 7472 616c  esponse: Central
+0002b1d0: 4150 4920 5265 7370 6f6e 7365 206f 626a  API Response obj
+0002b1e0: 6563 740a 2020 2020 2020 2020 2222 220a  ect.        """.
+0002b1f0: 2020 2020 2020 2020 7572 6c20 3d20 222f          url = "/
+0002b200: 7261 7069 6473 2f76 312f 6e65 6967 6862  rapids/v1/neighb
+0002b210: 6f72 5f61 7073 220a 0a20 2020 2020 2020  or_aps"..       
+0002b220: 2070 6172 616d 7320 3d20 7b0a 2020 2020   params = {.    
+0002b230: 2020 2020 2020 2020 2767 726f 7570 273a          'group':
+0002b240: 2067 726f 7570 2c0a 2020 2020 2020 2020   group,.        
+0002b250: 2020 2020 276c 6162 656c 273a 206c 6162      'label': lab
+0002b260: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
+0002b270: 2773 6974 6527 3a20 7369 7465 2c0a 2020  'site': site,.  
+0002b280: 2020 2020 2020 2020 2020 2773 7461 7274            'start
+0002b290: 273a 2073 7461 7274 2c0a 2020 2020 2020  ': start,.      
+0002b2a0: 2020 2020 2020 2765 6e64 273a 2065 6e64        'end': end
+0002b2b0: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
+0002b2c0: 7761 726d 5f69 6427 3a20 7377 6172 6d5f  warm_id': swarm_
+0002b2d0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0002b2e0: 2766 726f 6d5f 7469 6d65 7374 616d 7027  'from_timestamp'
+0002b2f0: 3a20 6672 6f6d 5f74 696d 6573 7461 6d70  : from_timestamp
+0002b300: 2c0a 2020 2020 2020 2020 2020 2020 2774  ,.            't
+0002b310: 6f5f 7469 6d65 7374 616d 7027 3a20 746f  o_timestamp': to
+0002b320: 5f74 696d 6573 7461 6d70 2c0a 2020 2020  _timestamp,.    
+0002b330: 2020 2020 2020 2020 276f 6666 7365 7427          'offset'
+0002b340: 3a20 6f66 6673 6574 2c0a 2020 2020 2020  : offset,.      
+0002b350: 2020 2020 2020 276c 696d 6974 273a 206c        'limit': l
+0002b360: 696d 6974 0a20 2020 2020 2020 207d 0a0a  imit.        }..
+0002b370: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+0002b380: 7761 6974 2073 656c 662e 6765 7428 7572  wait self.get(ur
+0002b390: 6c2c 2070 6172 616d 733d 7061 7261 6d73  l, params=params
+0002b3a0: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
+0002b3b0: 2077 6964 735f 6765 745f 616c 6c28 0a20   wids_get_all(. 
+0002b3c0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0002b3d0: 2020 2020 2067 726f 7570 3a20 4c69 7374       group: List
+0002b3e0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0002b3f0: 2020 2020 2020 6c61 6265 6c3a 204c 6973        label: Lis
+0002b400: 745b 7374 725d 203d 204e 6f6e 652c 0a20  t[str] = None,. 
+0002b410: 2020 2020 2020 2073 6974 653a 204c 6973         site: Lis
+0002b420: 745b 7374 725d 203d 204e 6f6e 652c 0a20  t[str] = None,. 
+0002b430: 2020 2020 2020 2073 7461 7274 3a20 696e         start: in
+0002b440: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
+0002b450: 2020 656e 643a 2069 6e74 203d 204e 6f6e    end: int = Non
+0002b460: 652c 0a20 2020 2020 2020 2073 7761 726d  e,.        swarm
+0002b470: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+0002b480: 0a20 2020 2020 2020 2066 726f 6d5f 7469  .        from_ti
+0002b490: 6d65 7374 616d 703a 2069 6e74 203d 204e  mestamp: int = N
+0002b4a0: 6f6e 652c 0a20 2020 2020 2020 2074 6f5f  one,.        to_
+0002b4b0: 7469 6d65 7374 616d 703a 2069 6e74 203d  timestamp: int =
+0002b4c0: 204e 6f6e 652c 0a20 2020 2020 2020 206f   None,.        o
+0002b4d0: 6666 7365 743a 2069 6e74 203d 2030 2c0a  ffset: int = 0,.
+0002b4e0: 2020 2020 2020 2020 6c69 6d69 743a 2069          limit: i
+0002b4f0: 6e74 203d 2031 3030 0a20 2020 2029 202d  nt = 100.    ) -
+0002b500: 3e20 5265 7370 6f6e 7365 3a0a 2020 2020  > Response:.    
+0002b510: 2020 2020 2222 224c 6973 7420 616c 6c20      """List all 
+0002b520: 7769 6473 2063 6c61 7373 6966 6963 6174  wids classificat
+0002b530: 696f 6e73 2e0a 0a20 2020 2020 2020 2041  ions...        A
+0002b540: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0002b550: 2067 726f 7570 2028 4c69 7374 5b73 7472   group (List[str
+0002b560: 5d2c 206f 7074 696f 6e61 6c29 3a20 4c69  ], optional): Li
+0002b570: 7374 206f 6620 6772 6f75 7020 6e61 6d65  st of group name
+0002b580: 730a 2020 2020 2020 2020 2020 2020 6c61  s.            la
+0002b590: 6265 6c20 284c 6973 745b 7374 725d 2c20  bel (List[str], 
+0002b5a0: 6f70 7469 6f6e 616c 293a 204c 6973 7420  optional): List 
+0002b5b0: 6f66 206c 6162 656c 206e 616d 6573 0a20  of label names. 
+0002b5c0: 2020 2020 2020 2020 2020 2073 6974 6520             site 
+0002b5d0: 284c 6973 745b 7374 725d 2c20 6f70 7469  (List[str], opti
+0002b5e0: 6f6e 616c 293a 204c 6973 7420 6f66 2073  onal): List of s
+0002b5f0: 6974 6520 6e61 6d65 730a 2020 2020 2020  ite names.      
+0002b600: 2020 2020 2020 7374 6172 7420 2869 6e74        start (int
+0002b610: 2c20 6f70 7469 6f6e 616c 293a 204e 6565  , optional): Nee
+0002b620: 6420 696e 666f 726d 6174 696f 6e20 6672  d information fr
+0002b630: 6f6d 2074 6869 7320 7469 6d65 7374 616d  om this timestam
+0002b640: 702e 2054 696d 6573 7461 6d70 2069 7320  p. Timestamp is 
+0002b650: 6570 6f63 6820 696e 0a20 2020 2020 2020  epoch in.       
+0002b660: 2020 2020 2020 2020 206d 696c 6c69 7365           millise
+0002b670: 636f 6e64 732e 2044 6566 6175 6c74 2069  conds. Default i
+0002b680: 7320 6375 7272 656e 7420 7469 6d65 7374  s current timest
+0002b690: 616d 7020 6d69 6e75 7320 3320 686f 7572  amp minus 3 hour
+0002b6a0: 730a 2020 2020 2020 2020 2020 2020 656e  s.            en
+0002b6b0: 6420 2869 6e74 2c20 6f70 7469 6f6e 616c  d (int, optional
+0002b6c0: 293a 204e 6565 6420 696e 666f 726d 6174  ): Need informat
+0002b6d0: 696f 6e20 746f 2074 6869 7320 7469 6d65  ion to this time
+0002b6e0: 7374 616d 702e 2054 696d 6573 7461 6d70  stamp. Timestamp
+0002b6f0: 2069 7320 6570 6f63 6820 696e 0a20 2020   is epoch in.   
+0002b700: 2020 2020 2020 2020 2020 2020 206d 696c               mil
+0002b710: 6c69 7365 636f 6e64 732e 2044 6566 6175  liseconds. Defau
+0002b720: 6c74 2069 7320 6375 7272 656e 7420 7469  lt is current ti
+0002b730: 6d65 7374 616d 700a 2020 2020 2020 2020  mestamp.        
+0002b740: 2020 2020 7377 6172 6d5f 6964 2028 7374      swarm_id (st
+0002b750: 722c 206f 7074 696f 6e61 6c29 3a20 4669  r, optional): Fi
+0002b760: 6c74 6572 2062 7920 5377 6172 6d20 4944  lter by Swarm ID
+0002b770: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
+0002b780: 6d5f 7469 6d65 7374 616d 7020 2869 6e74  m_timestamp (int
+0002b790: 2c20 6f70 7469 6f6e 616c 293a 2054 6869  , optional): Thi
+0002b7a0: 7320 7061 7261 6d65 7465 7220 7375 7065  s parameter supe
+0002b7b0: 7263 6564 6573 2073 7461 7274 2070 6172  rcedes start par
+0002b7c0: 616d 6574 6572 2e20 4e65 6564 0a20 2020  ameter. Need.   
+0002b7d0: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
+0002b7e0: 6f72 6d61 7469 6f6e 2066 726f 6d20 7468  ormation from th
+0002b7f0: 6973 2074 696d 6573 7461 6d70 2e20 5469  is timestamp. Ti
+0002b800: 6d65 7374 616d 7020 6973 2065 706f 6368  mestamp is epoch
+0002b810: 2069 6e20 7365 636f 6e64 732e 2044 6566   in seconds. Def
+0002b820: 6175 6c74 2069 7320 6375 7272 656e 740a  ault is current.
+0002b830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b840: 5554 4320 7469 6d65 7374 616d 7020 6d69  UTC timestamp mi
+0002b850: 6e75 7320 3320 686f 7572 730a 2020 2020  nus 3 hours.    
+0002b860: 2020 2020 2020 2020 746f 5f74 696d 6573          to_times
+0002b870: 7461 6d70 2028 696e 742c 206f 7074 696f  tamp (int, optio
+0002b880: 6e61 6c29 3a20 5468 6973 2070 6172 616d  nal): This param
+0002b890: 6574 6572 2073 7570 6572 6365 6465 7320  eter supercedes 
+0002b8a0: 656e 6420 7061 7261 6d65 7465 722e 204e  end parameter. N
+0002b8b0: 6565 6420 696e 666f 726d 6174 696f 6e0a  eed information.
+0002b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b8d0: 746f 2074 6869 7320 7469 6d65 7374 616d  to this timestam
+0002b8e0: 702e 2054 696d 6573 7461 6d70 2069 7320  p. Timestamp is 
+0002b8f0: 6570 6f63 6820 696e 2073 6563 6f6e 6473  epoch in seconds
+0002b900: 2e20 4465 6661 756c 7420 6973 2063 7572  . Default is cur
+0002b910: 7265 6e74 2055 5443 2074 696d 6573 7461  rent UTC timesta
+0002b920: 6d70 0a20 2020 2020 2020 2020 2020 206f  mp.            o
+0002b930: 6666 7365 7420 2869 6e74 2c20 6f70 7469  ffset (int, opti
+0002b940: 6f6e 616c 293a 2050 6167 696e 6174 696f  onal): Paginatio
+0002b950: 6e20 6f66 6673 6574 2028 6465 6661 756c  n offset (defaul
+0002b960: 7420 3d20 3029 2044 6566 6175 6c74 7320  t = 0) Defaults 
+0002b970: 746f 2030 2e0a 2020 2020 2020 2020 2020  to 0..          
+0002b980: 2020 6c69 6d69 7420 2869 6e74 2c20 6f70    limit (int, op
+0002b990: 7469 6f6e 616c 293a 2070 6167 696e 6174  tional): paginat
+0002b9a0: 696f 6e20 7369 7a65 2028 6465 6661 756c  ion size (defaul
+0002b9b0: 7420 3d20 3130 3029 2044 6566 6175 6c74  t = 100) Default
+0002b9c0: 7320 746f 2031 3030 2e0a 0a20 2020 2020  s to 100...     
+0002b9d0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0002b9e0: 2020 2020 2020 2020 5265 7370 6f6e 7365          Response
+0002b9f0: 3a20 4365 6e74 7261 6c41 5049 2052 6573  : CentralAPI Res
+0002ba00: 706f 6e73 6520 6f62 6a65 6374 0a20 2020  ponse object.   
+0002ba10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0002ba20: 2070 6172 616d 7320 3d20 7b0a 2020 2020   params = {.    
+0002ba30: 2020 2020 2020 2020 2767 726f 7570 273a          'group':
+0002ba40: 2067 726f 7570 2c0a 2020 2020 2020 2020   group,.        
+0002ba50: 2020 2020 276c 6162 656c 273a 206c 6162      'label': lab
+0002ba60: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
+0002ba70: 2773 6974 6527 3a20 7369 7465 2c0a 2020  'site': site,.  
+0002ba80: 2020 2020 2020 2020 2020 2773 7461 7274            'start
+0002ba90: 273a 2073 7461 7274 2c0a 2020 2020 2020  ': start,.      
+0002baa0: 2020 2020 2020 2765 6e64 273a 2065 6e64        'end': end
+0002bab0: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
+0002bac0: 7761 726d 5f69 6427 3a20 7377 6172 6d5f  warm_id': swarm_
+0002bad0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0002bae0: 2766 726f 6d5f 7469 6d65 7374 616d 7027  'from_timestamp'
+0002baf0: 3a20 6672 6f6d 5f74 696d 6573 7461 6d70  : from_timestamp
+0002bb00: 2c0a 2020 2020 2020 2020 2020 2020 2774  ,.            't
+0002bb10: 6f5f 7469 6d65 7374 616d 7027 3a20 746f  o_timestamp': to
+0002bb20: 5f74 696d 6573 7461 6d70 2c0a 2020 2020  _timestamp,.    
+0002bb30: 2020 2020 2020 2020 276f 6666 7365 7427          'offset'
+0002bb40: 3a20 6f66 6673 6574 2c0a 2020 2020 2020  : offset,.      
+0002bb50: 2020 2020 2020 276c 696d 6974 273a 206c        'limit': l
+0002bb60: 696d 6974 0a20 2020 2020 2020 207d 0a0a  imit.        }..
+0002bb70: 2020 2020 2020 2020 6272 203d 2073 656c          br = sel
+0002bb80: 662e 4261 7463 6852 6571 7565 7374 0a20  f.BatchRequest. 
+0002bb90: 2020 2020 2020 2066 756e 6373 203d 205b         funcs = [
+0002bba0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002bbb0: 662e 7769 6473 5f67 6574 5f69 6e74 6572  f.wids_get_inter
+0002bbc0: 6665 7269 6e67 5f61 7073 2c0a 2020 2020  fering_aps,.    
+0002bbd0: 2020 2020 2020 2020 7365 6c66 2e77 6964          self.wid
+0002bbe0: 735f 6765 745f 6e65 6967 6862 6f72 5f61  s_get_neighbor_a
+0002bbf0: 7073 2c0a 2020 2020 2020 2020 2020 2020  ps,.            
+0002bc00: 7365 6c66 2e77 6964 735f 6765 745f 7375  self.wids_get_su
+0002bc10: 7370 6563 745f 6170 732c 0a20 2020 2020  spect_aps,.     
+0002bc20: 2020 2020 2020 2073 656c 662e 7769 6473         self.wids
+0002bc30: 5f67 6574 5f72 6f67 7565 5f61 7073 2c0a  _get_rogue_aps,.
+0002bc40: 2020 2020 2020 2020 5d0a 0a20 2020 2020          ]..     
+0002bc50: 2020 2062 6174 6368 5f72 6571 203d 205b     batch_req = [
+0002bc60: 0a20 2020 2020 2020 2020 2020 2062 7228  .            br(
+0002bc70: 662c 202a 2a70 6172 616d 7329 2066 6f72  f, **params) for
+0002bc80: 2066 2069 6e20 6675 6e63 730a 2020 2020   f in funcs.    
+0002bc90: 2020 2020 5d0a 0a20 2020 2020 2020 2062      ]..        b
+0002bca0: 6174 6368 5f72 6573 203d 2061 7761 6974  atch_res = await
+0002bcb0: 2073 656c 662e 5f62 6174 6368 5f72 6571   self._batch_req
+0002bcc0: 7565 7374 2862 6174 6368 5f72 6571 290a  uest(batch_req).
+0002bcd0: 2020 2020 2020 2020 7265 7370 203d 2062          resp = b
+0002bce0: 6174 6368 5f72 6573 5b2d 315d 0a20 2020  atch_res[-1].   
+0002bcf0: 2020 2020 206f 6b5f 7265 7320 3d20 5b69       ok_res = [i
+0002bd00: 6478 2066 6f72 2069 6478 2c20 7265 7320  dx for idx, res 
+0002bd10: 696e 2065 6e75 6d65 7261 7465 2862 6174  in enumerate(bat
+0002bd20: 6368 5f72 6573 2920 6966 2072 6573 2e6f  ch_res) if res.o
+0002bd30: 6b5d 0a20 2020 2020 2020 2069 6620 6e6f  k].        if no
+0002bd40: 7420 6c65 6e28 6f6b 5f72 6573 2920 3d3d  t len(ok_res) ==
+0002bd50: 206c 656e 2866 756e 6373 293a 0a20 2020   len(funcs):.   
+0002bd60: 2020 2020 2020 2020 2066 6169 6c65 6420           failed 
+0002bd70: 3d20 5b78 2066 6f72 2078 2069 6e20 7261  = [x for x in ra
+0002bd80: 6e67 6528 302c 206c 656e 2866 756e 6373  nge(0, len(funcs
+0002bd90: 2929 2069 6620 7820 6e6f 7420 696e 206f  )) if x not in o
+0002bda0: 6b5f 7265 735d 0a20 2020 2020 2020 2020  k_res].         
+0002bdb0: 2020 2066 6f72 2066 2069 6e20 6661 696c     for f in fail
+0002bdc0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+0002bdd0: 2020 2020 6966 2066 2069 6e20 7261 6e67      if f in rang
+0002bde0: 6528 302c 206c 656e 2862 6174 6368 5f72  e(0, len(batch_r
+0002bdf0: 6573 2929 3a0a 2020 2020 2020 2020 2020  es)):.          
+0002be00: 2020 2020 2020 2020 2020 6c6f 672e 6572            log.er
+0002be10: 726f 7228 6622 7b62 6174 6368 5f72 6573  ror(f"{batch_res
+0002be20: 5b66 5d2e 6d65 7468 6f64 7d20 7b62 6174  [f].method} {bat
+0002be30: 6368 5f72 6573 5b66 5d2e 7572 6c2e 7061  ch_res[f].url.pa
+0002be40: 7468 7d20 5265 7475 726e 6564 2045 7272  th} Returned Err
+0002be50: 6f72 2053 7461 7475 7320 7b62 6174 6368  or Status {batch
+0002be60: 5f72 6573 5b66 5d2e 7374 6174 7573 7d2e  _res[f].status}.
+0002be70: 207b 6261 7463 685f 7265 735b 665d 2e6f   {batch_res[f].o
+0002be80: 7574 7075 7420 6f72 2062 6174 6368 5f72  utput or batch_r
+0002be90: 6573 5b66 5d2e 6572 726f 727d 222c 2073  es[f].error}", s
+0002bea0: 686f 773d 5472 7565 290a 2020 2020 2020  how=True).      
+0002beb0: 2020 7261 775f 6b65 7973 203d 205b 2269    raw_keys = ["i
+0002bec0: 6e74 6572 6665 7269 6e67 5f61 7073 222c  nterfering_aps",
+0002bed0: 2022 6e65 6967 6862 6f72 5f61 7073 222c   "neighbor_aps",
+0002bee0: 2022 7375 7370 6563 745f 6170 7322 5d0a   "suspect_aps"].
+0002bef0: 2020 2020 2020 2020 7265 7370 2e72 6177          resp.raw
+0002bf00: 203d 207b 2272 6f67 7565 5f61 7073 223a   = {"rogue_aps":
+0002bf10: 2072 6573 702e 7261 772e 6765 7428 2272   resp.raw.get("r
+0002bf20: 6f67 7565 5f61 7073 222c 205b 5d29 2c20  ogue_aps", []), 
+0002bf30: 225f 636f 756e 7473 223a 207b 2272 6f67  "_counts": {"rog
+0002bf40: 7565 7322 3a20 7265 7370 2e72 6177 2e67  ues": resp.raw.g
+0002bf50: 6574 2822 746f 7461 6c22 297d 7d0a 2020  et("total")}}.  
+0002bf60: 2020 2020 2020 666f 7220 6964 782c 206b        for idx, k
+0002bf70: 6579 2069 6e20 656e 756d 6572 6174 6528  ey in enumerate(
+0002bf80: 7261 775f 6b65 7973 293a 0a20 2020 2020  raw_keys):.     
+0002bf90: 2020 2020 2020 2069 6620 6964 7820 696e         if idx in
+0002bfa0: 206f 6b5f 7265 733a 0a20 2020 2020 2020   ok_res:.       
+0002bfb0: 2020 2020 2020 2020 2072 6573 702e 7261           resp.ra
+0002bfc0: 7720 3d20 7b2a 2a72 6573 702e 7261 772c  w = {**resp.raw,
+0002bfd0: 202a 2a7b 6b65 793a 2062 6174 6368 5f72   **{key: batch_r
+0002bfe0: 6573 5b69 6478 5d2e 7261 772e 6765 7428  es[idx].raw.get(
+0002bff0: 6b65 792c 205b 5d29 7d7d 0a20 2020 2020  key, [])}}.     
+0002c000: 2020 2020 2020 2020 2020 2072 6573 702e             resp.
+0002c010: 7261 775b 225f 636f 756e 7473 225d 5b6b  raw["_counts"][k
+0002c020: 6579 2e72 7374 7269 7028 225f 6170 7322  ey.rstrip("_aps"
+0002c030: 295d 203d 2062 6174 6368 5f72 6573 5b69  )] = batch_res[i
+0002c040: 6478 5d2e 7261 772e 6765 7428 2274 6f74  dx].raw.get("tot
+0002c050: 616c 2229 0a20 2020 2020 2020 2020 2020  al").           
+0002c060: 2020 2020 2072 6573 702e 6f75 7470 7574       resp.output
+0002c070: 203d 205b 2a72 6573 702e 6f75 7470 7574   = [*resp.output
+0002c080: 2c20 2a62 6174 6368 5f72 6573 5b69 6478  , *batch_res[idx
+0002c090: 5d2e 6f75 7470 7574 5d0a 2020 2020 2020  ].output].      
+0002c0a0: 2020 2320 7265 7370 2e6f 7574 7075 7420    # resp.output 
+0002c0b0: 3d20 5b2a 7265 7370 2e6f 7574 7075 742c  = [*resp.output,
+0002c0c0: 202a 6261 7463 685f 7265 735b 305d 2e6f   *batch_res[0].o
+0002c0d0: 7574 7075 742c 202a 6261 7463 685f 7265  utput, *batch_re
+0002c0e0: 735b 315d 2e6f 7574 7075 742c 202a 6261  s[1].output, *ba
+0002c0f0: 7463 685f 7265 735b 325d 2e6f 7574 7075  tch_res[2].outpu
+0002c100: 745d 0a20 2020 2020 2020 2074 7279 3a0a  t].        try:.
+0002c110: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+0002c120: 2e6f 7574 7075 7420 3d20 5b6d 6f64 656c  .output = [model
+0002c130: 732e 5749 4453 282a 2a64 292e 6469 6374  s.WIDS(**d).dict
+0002c140: 2829 2066 6f72 2064 2069 6e20 7265 7370  () for d in resp
+0002c150: 2e6f 7574 7075 745d 0a20 2020 2020 2020  .output].       
+0002c160: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+0002c170: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
+0002c180: 2020 2020 6c6f 672e 7761 726e 696e 6728      log.warning(
+0002c190: 6622 6465 7620 6e6f 7465 2e20 7079 6461  f"dev note. pyda
+0002c1a0: 6e74 6963 2063 6f6e 7665 7273 696f 6e20  ntic conversion 
+0002c1b0: 6469 6420 6e6f 7420 776f 726b 5c6e 7b65  did not work\n{e
+0002c1c0: 7d22 2c20 7368 6f77 3d54 7275 6529 0a0a  }", show=True)..
+0002c1d0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0002c1e0: 6573 700a 0a0a 2020 2020 6173 796e 6320  esp...    async 
+0002c1f0: 6465 6620 6765 745f 616c 6572 7473 280a  def get_alerts(.
+0002c200: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0002c210: 2020 2020 2020 6375 7374 6f6d 6572 5f69        customer_i
+0002c220: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+0002c230: 2020 2020 2020 2067 726f 7570 3a20 7374         group: st
+0002c240: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+0002c250: 2020 6c61 6265 6c3a 2073 7472 203d 204e    label: str = N
+0002c260: 6f6e 652c 0a20 2020 2020 2020 2073 6572  one,.        ser
+0002c270: 6961 6c3a 2073 7472 203d 204e 6f6e 652c  ial: str = None,
+0002c280: 0a20 2020 2020 2020 2073 6974 653a 2073  .        site: s
+0002c290: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0002c2a0: 2020 2066 726f 6d5f 7473 3a20 696e 7420     from_ts: int 
+0002c2b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0002c2c0: 746f 5f74 733a 2069 6e74 203d 204e 6f6e  to_ts: int = Non
+0002c2d0: 652c 0a20 2020 2020 2020 2073 6576 6572  e,.        sever
+0002c2e0: 6974 793a 2073 7472 203d 204e 6f6e 652c  ity: str = None,
+0002c2f0: 0a20 2020 2020 2020 2074 7970 653a 2073  .        type: s
+0002c300: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0002c310: 2020 2073 6561 7263 683a 2073 7472 203d     search: str =
+0002c320: 204e 6f6e 652c 0a20 2020 2020 2020 2023   None,.        #
+0002c330: 2063 616c 6375 6c61 7465 5f74 6f74 616c   calculate_total
+0002c340: 3a20 626f 6f6c 203d 2046 616c 7365 2c20  : bool = False, 
+0002c350: 2023 2044 6f65 736e 2774 2061 7070 6561   # Doesn't appea
+0002c360: 7220 746f 2069 6d70 6163 7420 616c 7761  r to impact alwa
+0002c370: 7973 2072 6574 7572 6e73 2074 6f74 616c  ys returns total
+0002c380: 0a20 2020 2020 2020 2061 636b 3a20 626f  .        ack: bo
+0002c390: 6f6c 203d 204e 6f6e 652c 0a20 2020 2020  ol = None,.     
+0002c3a0: 2020 2066 6965 6c64 733a 2073 7472 203d     fields: str =
+0002c3b0: 204e 6f6e 652c 0a20 2020 2020 2020 206f   None,.        o
+0002c3c0: 6666 7365 743a 2069 6e74 203d 2030 2c0a  ffset: int = 0,.
+0002c3d0: 2020 2020 2020 2020 6c69 6d69 743a 2069          limit: i
+0002c3e0: 6e74 203d 2031 3030 302c 0a20 2020 2029  nt = 1000,.    )
+0002c3f0: 202d 3e20 5265 7370 6f6e 7365 3a0a 2020   -> Response:.  
+0002c400: 2020 2020 2020 2222 225b 6365 6e74 7261        """[centra
+0002c410: 6c5d 204c 6973 7420 4e6f 7469 6669 6361  l] List Notifica
+0002c420: 7469 6f6e 732f 416c 6572 7473 2e20 2052  tions/Alerts.  R
+0002c430: 6574 7572 6e73 2031 2064 6179 2062 7920  eturns 1 day by 
+0002c440: 6465 6661 756c 742e 0a0a 2020 2020 2020  default...      
+0002c450: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0002c460: 2020 2020 6375 7374 6f6d 6572 5f69 6420      customer_id 
+0002c470: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+0002c480: 204d 5350 2075 7365 7220 6361 6e20 6669   MSP user can fi
+0002c490: 6c74 6572 206e 6f74 6966 6963 6174 696f  lter notificatio
+0002c4a0: 6e73 2062 6173 6564 206f 6e20 6375 7374  ns based on cust
+0002c4b0: 6f6d 6572 2069 640a 2020 2020 2020 2020  omer id.        
+0002c4c0: 2020 2020 6772 6f75 7020 2873 7472 2c20      group (str, 
+0002c4d0: 6f70 7469 6f6e 616c 293a 2055 7365 6420  optional): Used 
+0002c4e0: 746f 2066 696c 7465 7220 7468 6520 6e6f  to filter the no
+0002c4f0: 7469 6669 6361 7469 6f6e 2074 7970 6573  tification types
+0002c500: 2062 6173 6564 206f 6e20 6772 6f75 7020   based on group 
+0002c510: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
+0002c520: 206c 6162 656c 2028 7374 722c 206f 7074   label (str, opt
+0002c530: 696f 6e61 6c29 3a20 5573 6564 2074 6f20  ional): Used to 
+0002c540: 6669 6c74 6572 2074 6865 206e 6f74 6966  filter the notif
+0002c550: 6963 6174 696f 6e20 7479 7065 7320 6261  ication types ba
+0002c560: 7365 6420 6f6e 204c 6162 656c 206e 616d  sed on Label nam
+0002c570: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
+0002c580: 7269 616c 2028 7374 722c 206f 7074 696f  rial (str, optio
+0002c590: 6e61 6c29 3a20 5573 6564 2074 6f20 6669  nal): Used to fi
+0002c5a0: 6c74 6572 2074 6865 2072 6573 756c 7420  lter the result 
+0002c5b0: 6261 7365 6420 6f6e 2073 6572 6961 6c20  based on serial 
+0002c5c0: 6e75 6d62 6572 206f 6620 7468 6520 6465  number of the de
+0002c5d0: 7669 6365 0a20 2020 2020 2020 2020 2020  vice.           
+0002c5e0: 2073 6974 6520 2873 7472 2c20 6f70 7469   site (str, opti
+0002c5f0: 6f6e 616c 293a 2055 7365 6420 746f 2066  onal): Used to f
+0002c600: 696c 7465 7220 7468 6520 6e6f 7469 6669  ilter the notifi
+0002c610: 6361 7469 6f6e 2074 7970 6573 2062 6173  cation types bas
+0002c620: 6564 206f 6e20 5369 7465 206e 616d 650a  ed on Site name.
+0002c630: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
+0002c640: 5f74 7320 2869 6e74 2c20 6f70 7469 6f6e  _ts (int, option
+0002c650: 616c 293a 2031 2973 7461 7274 206f 6620  al): 1)start of 
+0002c660: 6475 7261 7469 6f6e 2077 6974 6869 6e20  duration within 
+0002c670: 7768 6963 6820 616c 6572 7473 2061 7265  which alerts are
+0002c680: 2072 6169 7365 640a 2020 2020 2020 2020   raised.        
+0002c690: 2020 2020 2020 2020 3229 6465 7363 7269          2)descri
+0002c6a0: 6265 6420 7573 696e 6720 556e 6978 2045  bed using Unix E
+0002c6b0: 706f 6368 2074 696d 6520 696e 2073 6563  poch time in sec
+0002c6c0: 6f6e 6473 2020 4465 6661 756c 7420 3330  onds  Default 30
+0002c6d0: 2064 6179 7320 286d 6178 2039 3029 0a20   days (max 90). 
+0002c6e0: 2020 2020 2020 2020 2020 2074 6f5f 7473             to_ts
+0002c6f0: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
+0002c700: 3a20 3129 656e 6420 6f66 2064 7572 6174  : 1)end of durat
+0002c710: 696f 6e20 7769 7468 696e 2077 6869 6368  ion within which
+0002c720: 2061 6c65 7274 7320 6172 6520 7261 6973   alerts are rais
+0002c730: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
+0002c740: 2020 2032 2964 6573 6372 6962 6564 2075     2)described u
+0002c750: 7369 6e67 2055 6e69 7820 4570 6f63 6820  sing Unix Epoch 
+0002c760: 7469 6d65 2069 6e20 7365 636f 6e64 730a  time in seconds.
+0002c770: 2020 2020 2020 2020 2020 2020 7365 7665              seve
+0002c780: 7269 7479 2028 7374 722c 206f 7074 696f  rity (str, optio
+0002c790: 6e61 6c29 3a20 5573 6564 2074 6f20 6669  nal): Used to fi
+0002c7a0: 6c74 6572 2074 6865 206e 6f74 6966 6963  lter the notific
+0002c7b0: 6174 696f 6e20 7479 7065 7320 6261 7365  ation types base
+0002c7c0: 6420 6f6e 2073 6576 6572 6974 790a 2020  d on severity.  
+0002c7d0: 2020 2020 2020 2020 2020 7479 7065 2028            type (
+0002c7e0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+0002c7f0: 5573 6564 2074 6f20 6669 6c74 6572 2074  Used to filter t
+0002c800: 6865 206e 6f74 6966 6963 6174 696f 6e20  he notification 
+0002c810: 7479 7065 7320 6261 7365 6420 6f6e 206e  types based on n
+0002c820: 6f74 6966 6963 6174 696f 6e20 7479 7065  otification type
+0002c830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002c840: 206e 616d 650a 2020 2020 2020 2020 2020   name.          
+0002c850: 2020 7365 6172 6368 2028 7374 722c 206f    search (str, o
+0002c860: 7074 696f 6e61 6c29 3a20 7465 726d 2075  ptional): term u
+0002c870: 7365 6420 746f 2073 6561 7263 6820 696e  sed to search in
+0002c880: 206e 616d 652c 2063 6174 6567 6f72 7920   name, category 
+0002c890: 6f66 2074 6865 2061 6c65 7274 0a20 2020  of the alert.   
+0002c8a0: 2020 2020 2020 2020 2063 616c 6375 6c61           calcula
+0002c8b0: 7465 5f74 6f74 616c 2028 626f 6f6c 2c20  te_total (bool, 
+0002c8c0: 6f70 7469 6f6e 616c 293a 2057 6865 7468  optional): Wheth
+0002c8d0: 6572 2074 6f20 636f 756e 7420 746f 7461  er to count tota
+0002c8e0: 6c20 6974 656d 7320 696e 2074 6865 2072  l items in the r
+0002c8f0: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
+0002c900: 2020 2020 6163 6b20 2862 6f6f 6c2c 206f      ack (bool, o
+0002c910: 7074 696f 6e61 6c29 3a20 4669 6c74 6572  ptional): Filter
+0002c920: 2061 636b 6e6f 776c 6564 6765 6420 6f72   acknowledged or
+0002c930: 2075 6e61 636b 6e6f 776c 6564 6765 6420   unacknowledged 
+0002c940: 6e6f 7469 6669 6361 7469 6f6e 732e 2057  notifications. W
+0002c950: 6865 6e20 7175 6572 790a 2020 2020 2020  hen query.      
+0002c960: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
+0002c970: 7465 7220 6973 206e 6f74 2073 7065 6369  ter is not speci
+0002c980: 6669 6564 2c20 626f 7468 2061 636b 6e6f  fied, both ackno
+0002c990: 776c 6564 6765 6420 616e 6420 756e 6163  wledged and unac
+0002c9a0: 6b6e 6f77 6c65 6467 6564 206e 6f74 6966  knowledged notif
+0002c9b0: 6963 6174 696f 6e73 2061 7265 0a20 2020  ications are.   
+0002c9c0: 2020 2020 2020 2020 2020 2020 2069 6e63               inc
+0002c9d0: 6c75 6465 640a 2020 2020 2020 2020 2020  luded.          
+0002c9e0: 2020 6669 656c 6473 2028 7374 722c 206f    fields (str, o
+0002c9f0: 7074 696f 6e61 6c29 3a20 436f 6d6d 6120  ptional): Comma 
+0002ca00: 7365 7061 7261 7465 6420 6c69 7374 206f  separated list o
+0002ca10: 6620 6669 656c 6473 2074 6f20 6265 2072  f fields to be r
+0002ca20: 6574 7572 6e65 640a 2020 2020 2020 2020  eturned.        
+0002ca30: 2020 2020 6f66 6673 6574 2028 696e 742c      offset (int,
+0002ca40: 206f 7074 696f 6e61 6c29 3a20 5061 6769   optional): Pagi
+0002ca50: 6e61 7469 6f6e 206f 6666 7365 7420 4465  nation offset De
+0002ca60: 6661 756c 7473 2074 6f20 302e 0a20 2020  faults to 0..   
+0002ca70: 2020 2020 2020 2020 206c 696d 6974 2028           limit (
+0002ca80: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
+0002ca90: 5061 6769 6e61 7469 6f6e 206c 696d 6974  Pagination limit
+0002caa0: 2e20 4465 6661 756c 7420 6973 2031 3030  . Default is 100
+0002cab0: 2061 6e64 206d 6178 2069 7320 3130 3030   and max is 1000
+0002cac0: 2044 6566 6175 6c74 7320 746f 2035 3030   Defaults to 500
+0002cad0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0002cae0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0002caf0: 5265 7370 6f6e 7365 3a20 4365 6e74 7261  Response: Centra
+0002cb00: 6c41 5049 2052 6573 706f 6e73 6520 6f62  lAPI Response ob
+0002cb10: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
+0002cb20: 0a20 2020 2020 2020 2075 726c 203d 2022  .        url = "
+0002cb30: 2f63 656e 7472 616c 2f76 312f 6e6f 7469  /central/v1/noti
+0002cb40: 6669 6361 7469 6f6e 7322 0a0a 2020 2020  fications"..    
+0002cb50: 2020 2020 6966 206e 6f74 2066 726f 6d5f      if not from_
+0002cb60: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+0002cb70: 6672 6f6d 5f74 7320 3d20 696e 7428 6461  from_ts = int(da
+0002cb80: 7465 7469 6d65 2e74 696d 6573 7461 6d70  tetime.timestamp
+0002cb90: 2864 6174 6574 696d 652e 746f 6461 7928  (datetime.today(
+0002cba0: 2920 2d20 7469 6d65 6465 6c74 6128 6461  ) - timedelta(da
+0002cbb0: 7973 3d31 2929 290a 2020 2020 2020 2020  ys=1))).        
+0002cbc0: 6966 2061 636b 2069 6e20 5b54 7275 652c  if ack in [True,
+0002cbd0: 2046 616c 7365 5d3a 0a20 2020 2020 2020   False]:.       
+0002cbe0: 2020 2020 2061 636b 203d 2073 7472 2861       ack = str(a
+0002cbf0: 636b 292e 6c6f 7765 7228 290a 0a20 2020  ck).lower()..   
+0002cc00: 2020 2020 2069 6620 746f 5f74 7320 616e       if to_ts an
+0002cc10: 6420 746f 5f74 7320 3c3d 2066 726f 6d5f  d to_ts <= from_
+0002cc20: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+0002cc30: 7265 7475 726e 2052 6573 706f 6e73 6528  return Response(
+0002cc40: 6572 726f 723d 6622 546f 2074 696d 6573  error=f"To times
+0002cc50: 7461 6d70 2028 7b74 6f5f 7473 7d29 2063  tamp ({to_ts}) c
+0002cc60: 616e 206e 6f74 2062 6520 6c65 7373 2074  an not be less t
+0002cc70: 6861 6e20 6672 6f6d 2074 696d 6573 7461  han from timesta
+0002cc80: 6d70 2028 7b66 726f 6d5f 7473 7d29 2229  mp ({from_ts})")
+0002cc90: 0a0a 2020 2020 2020 2020 7061 7261 6d73  ..        params
+0002cca0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+0002ccb0: 2027 6375 7374 6f6d 6572 5f69 6427 3a20   'customer_id': 
+0002ccc0: 6375 7374 6f6d 6572 5f69 642c 0a20 2020  customer_id,.   
+0002ccd0: 2020 2020 2020 2020 2027 6772 6f75 7027           'group'
+0002cce0: 3a20 6772 6f75 702c 0a20 2020 2020 2020  : group,.       
+0002ccf0: 2020 2020 2027 6c61 6265 6c27 3a20 6c61       'label': la
+0002cd00: 6265 6c2c 0a20 2020 2020 2020 2020 2020  bel,.           
+0002cd10: 2027 7365 7269 616c 273a 2073 6572 6961   'serial': seria
+0002cd20: 6c2c 0a20 2020 2020 2020 2020 2020 2027  l,.            '
+0002cd30: 7369 7465 273a 2073 6974 652c 0a20 2020  site': site,.   
+0002cd40: 2020 2020 2020 2020 2027 6672 6f6d 5f74           'from_t
+0002cd50: 696d 6573 7461 6d70 273a 2066 726f 6d5f  imestamp': from_
+0002cd60: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
+0002cd70: 2774 6f5f 7469 6d65 7374 616d 7027 3a20  'to_timestamp': 
+0002cd80: 746f 5f74 732c 0a20 2020 2020 2020 2020  to_ts,.         
+0002cd90: 2020 2027 7365 7665 7269 7479 273a 2073     'severity': s
+0002cda0: 6576 6572 6974 792c 0a20 2020 2020 2020  everity,.       
+0002cdb0: 2020 2020 2027 7365 6172 6368 273a 2073       'search': s
+0002cdc0: 6561 7263 682c 0a20 2020 2020 2020 2020  earch,.         
+0002cdd0: 2020 2023 2027 6361 6c63 756c 6174 655f     # 'calculate_
+0002cde0: 746f 7461 6c27 3a20 7374 7228 6361 6c63  total': str(calc
+0002cdf0: 756c 6174 655f 746f 7461 6c29 2c0a 2020  ulate_total),.  
+0002ce00: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
+0002ce10: 3a20 7479 7065 2c0a 2020 2020 2020 2020  : type,.        
+0002ce20: 2020 2020 2761 636b 273a 2061 636b 2c0a      'ack': ack,.
+0002ce30: 2020 2020 2020 2020 2020 2020 2766 6965              'fie
+0002ce40: 6c64 7327 3a20 6669 656c 6473 2c0a 2020  lds': fields,.  
+0002ce50: 2020 2020 2020 2020 2020 276f 6666 7365            'offse
+0002ce60: 7427 3a20 6f66 6673 6574 2c0a 2020 2020  t': offset,.    
+0002ce70: 2020 2020 2020 2020 276c 696d 6974 273a          'limit':
+0002ce80: 206c 696d 6974 2c0a 2020 2020 2020 2020   limit,.        
+0002ce90: 7d0a 0a20 2020 2020 2020 2072 6574 7572  }..        retur
+0002cea0: 6e20 6177 6169 7420 7365 6c66 2e67 6574  n await self.get
+0002ceb0: 2875 726c 2c20 7061 7261 6d73 3d70 6172  (url, params=par
+0002cec0: 616d 7329 0a0a 2020 2020 6173 796e 6320  ams)..    async 
+0002ced0: 6465 6620 6365 6e74 7261 6c5f 6163 6b6e  def central_ackn
+0002cee0: 6f77 6c65 6467 655f 6e6f 7469 6669 6361  owledge_notifica
+0002cef0: 7469 6f6e 7328 0a20 2020 2020 2020 2073  tions(.        s
+0002cf00: 656c 662c 0a20 2020 2020 2020 204e 6f4e  elf,.        NoN
+0002cf10: 616d 653a 204c 6973 745b 7374 725d 203d  ame: List[str] =
+0002cf20: 204e 6f6e 652c 0a20 2020 2029 202d 3e20   None,.    ) -> 
+0002cf30: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
+0002cf40: 2020 2222 2241 636b 6e6f 776c 6564 6765    """Acknowledge
+0002cf50: 204e 6f74 6966 6963 6174 696f 6e73 2062   Notifications b
+0002cf60: 7920 4944 204c 6973 7420 2f20 416c 6c2e  y ID List / All.
+0002cf70: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+0002cf80: 2020 2020 2020 2020 2020 2020 4e6f 4e61              NoNa
+0002cf90: 6d65 2028 4c69 7374 5b73 7472 5d2c 206f  me (List[str], o
+0002cfa0: 7074 696f 6e61 6c29 3a20 4163 6b6e 6f77  ptional): Acknow
+0002cfb0: 6c65 6467 6520 6e6f 7469 6669 6361 7469  ledge notificati
+0002cfc0: 6f6e 730a 0a20 2020 2020 2020 2052 6574  ons..        Ret
+0002cfd0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+0002cfe0: 2020 5265 7370 6f6e 7365 3a20 4365 6e74    Response: Cent
+0002cff0: 7261 6c41 5049 2052 6573 706f 6e73 6520  ralAPI Response 
+0002d000: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
+0002d010: 2222 0a20 2020 2020 2020 2075 726c 203d  "".        url =
+0002d020: 2022 2f63 656e 7472 616c 2f76 312f 6e6f   "/central/v1/no
+0002d030: 7469 6669 6361 7469 6f6e 7322 0a0a 2020  tifications"..  
+0002d040: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+0002d050: 6974 2073 656c 662e 706f 7374 2875 726c  it self.post(url
+0002d060: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
+0002d070: 2063 656e 7472 616c 5f67 6574 5f6e 6f74   central_get_not
+0002d080: 6966 6963 6174 696f 6e5f 636f 6e66 6967  ification_config
+0002d090: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0002d0a0: 2020 2020 2020 2020 7365 6172 6368 3a20          search: 
+0002d0b0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+0002d0c0: 2020 2020 736f 7274 3a20 7374 7220 3d20      sort: str = 
+0002d0d0: 272d 6372 6561 7465 645f 7473 272c 0a20  '-created_ts',. 
+0002d0e0: 2020 2020 2020 206f 6666 7365 743a 2069         offset: i
+0002d0f0: 6e74 203d 2030 2c0a 2020 2020 2020 2020  nt = 0,.        
+0002d100: 6c69 6d69 743a 2069 6e74 203d 2035 3030  limit: int = 500
+0002d110: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
+0002d120: 6e73 653a 0a20 2020 2020 2020 2022 2222  nse:.        """
+0002d130: 4c69 7374 2043 6f6e 6669 6775 7261 7469  List Configurati
+0002d140: 6f6e 2f53 6574 7469 6e67 7320 666f 7220  on/Settings for 
+0002d150: 616c 6572 7473 2074 6861 7420 7265 7375  alerts that resu
+0002d160: 6c74 2069 6e20 6e6f 7469 6669 6361 7469  lt in notificati
+0002d170: 6f6e 2e0a 0a20 2020 2020 2020 2041 7267  on...        Arg
+0002d180: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+0002d190: 6561 7263 6820 2873 7472 2c20 6f70 7469  earch (str, opti
+0002d1a0: 6f6e 616c 293a 2074 6572 6d20 7573 6564  onal): term used
+0002d1b0: 2074 6f20 7365 6172 6368 2069 6e20 6e61   to search in na
+0002d1c0: 6d65 2c20 6361 7465 676f 7279 206f 6620  me, category of 
+0002d1d0: 7468 6520 616c 6572 740a 2020 2020 2020  the alert.      
+0002d1e0: 2020 2020 2020 736f 7274 2028 7374 722c        sort (str,
+0002d1f0: 206f 7074 696f 6e61 6c29 3a20 536f 7274   optional): Sort
+0002d200: 2070 6172 616d 6574 6572 206d 6179 2062   parameter may b
+0002d210: 6520 6f6e 6520 6f66 202b 6372 6561 7465  e one of +create
+0002d220: 645f 7473 2c20 2d63 7265 6174 6564 5f74  d_ts, -created_t
+0002d230: 732c 2044 6566 6175 6c74 2069 730a 2020  s, Default is.  
+0002d240: 2020 2020 2020 2020 2020 2020 2020 272d                '-
+0002d250: 6372 6561 7465 645f 7473 2720 2056 616c  created_ts'  Val
+0002d260: 6964 2056 616c 7565 733a 202d 6372 6561  id Values: -crea
+0002d270: 7465 645f 7473 2c20 2b63 7265 6174 6564  ted_ts, +created
+0002d280: 5f74 730a 2020 2020 2020 2020 2020 2020  _ts.            
+0002d290: 6f66 6673 6574 2028 696e 742c 206f 7074  offset (int, opt
+0002d2a0: 696f 6e61 6c29 3a20 5061 6769 6e61 7469  ional): Paginati
+0002d2b0: 6f6e 206f 6666 7365 7420 4465 6661 756c  on offset Defaul
+0002d2c0: 7473 2074 6f20 302e 0a20 2020 2020 2020  ts to 0..       
+0002d2d0: 2020 2020 206c 696d 6974 2028 696e 742c       limit (int,
+0002d2e0: 206f 7074 696f 6e61 6c29 3a20 5061 6769   optional): Pagi
+0002d2f0: 6e61 7469 6f6e 206c 696d 6974 2e20 4465  nation limit. De
+0002d300: 6661 756c 7420 6973 2031 3030 2061 6e64  fault is 100 and
+0002d310: 206d 6178 2069 7320 3130 3030 2044 6566   max is 1000 Def
+0002d320: 6175 6c74 7320 746f 2031 3030 2e0a 0a20  aults to 100... 
+0002d330: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+0002d340: 2020 2020 2020 2020 2020 2020 5265 7370              Resp
+0002d350: 6f6e 7365 3a20 4365 6e74 7261 6c41 5049  onse: CentralAPI
+0002d360: 2052 6573 706f 6e73 6520 6f62 6a65 6374   Response object
+0002d370: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0002d380: 2020 2020 2075 726c 203d 2022 2f63 656e       url = "/cen
+0002d390: 7472 616c 2f76 312f 6e6f 7469 6669 6361  tral/v1/notifica
+0002d3a0: 7469 6f6e 732f 7365 7474 696e 6773 220a  tions/settings".
+0002d3b0: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
+0002d3c0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+0002d3d0: 2773 6561 7263 6827 3a20 7365 6172 6368  'search': search
+0002d3e0: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
+0002d3f0: 6f72 7427 3a20 736f 7274 2c0a 2020 2020  ort': sort,.    
+0002d400: 2020 2020 2020 2020 276f 6666 7365 7427          'offset'
+0002d410: 3a20 6f66 6673 6574 2c0a 2020 2020 2020  : offset,.      
+0002d420: 2020 2020 2020 276c 696d 6974 273a 206c        'limit': l
+0002d430: 696d 6974 0a20 2020 2020 2020 207d 0a0a  imit.        }..
+0002d440: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+0002d450: 7761 6974 2073 656c 662e 6765 7428 7572  wait self.get(ur
+0002d460: 6c2c 2070 6172 616d 733d 7061 7261 6d73  l, params=params
+0002d470: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
+0002d480: 2067 6574 5f61 705f 636f 6e66 6967 280a   get_ap_config(.
+0002d490: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0002d4a0: 2020 2020 2020 6772 6f75 705f 7377 6172        group_swar
+0002d4b0: 6d69 643a 2073 7472 2c0a 2020 2020 2020  mid: str,.      
+0002d4c0: 2020 7665 7273 696f 6e3a 2073 7472 203d    version: str =
+0002d4d0: 204e 6f6e 652c 0a20 2020 2029 202d 3e20   None,.    ) -> 
+0002d4e0: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
+0002d4f0: 2020 2222 2247 6574 2041 5020 4772 6f75    """Get AP Grou
+0002d500: 7020 4c65 7665 6c20 636f 6e66 6967 7572  p Level configur
+0002d510: 6174 696f 6e20 666f 7220 5549 2067 726f  ation for UI gro
+0002d520: 7570 2e0a 0a20 2020 2020 2020 202f 2f20  up...        // 
+0002d530: 5573 6564 2062 7920 7368 6f77 2063 6f6e  Used by show con
+0002d540: 6669 6720 3c41 5020 4d41 4320 666f 7220  fig <AP MAC for 
+0002d550: 414f 5331 3020 4150 3e20 2f2f 0a0a 2020  AOS10 AP> //..  
+0002d560: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+0002d570: 2020 2020 2020 2020 6772 6f75 705f 7377          group_sw
+0002d580: 6172 6d69 6420 2873 7472 293a 2047 726f  armid (str): Gro
+0002d590: 7570 206e 616d 6520 6f66 2074 6865 2067  up name of the g
+0002d5a0: 726f 7570 206f 7220 6775 6964 206f 6620  roup or guid of 
+0002d5b0: 7468 6520 7377 6172 6d2e 0a20 2020 2020  the swarm..     
+0002d5c0: 2020 2020 2020 2020 2020 2045 7861 6d70             Examp
+0002d5d0: 6c65 3a47 726f 7570 5f31 206f 7220 3661  le:Group_1 or 6a
+0002d5e0: 3564 3132 3362 3031 6639 3434 3138 3036  5d123b01f9441806
+0002d5f0: 3234 3465 6136 6530 3233 6661 6235 3834  244ea6e023fab584
+0002d600: 3162 3737 6338 3238 6130 3835 6630 3466  1b77c828a085f04f
+0002d610: 2e0a 2020 2020 2020 2020 2020 2020 7665  ..            ve
+0002d620: 7273 696f 6e20 2873 7472 2c20 6f70 7469  rsion (str, opti
+0002d630: 6f6e 616c 293a 2056 6572 7369 6f6e 206f  onal): Version o
+0002d640: 6620 4150 2e0a 0a20 2020 2020 2020 2052  f AP...        R
+0002d650: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0002d660: 2020 2020 5265 7370 6f6e 7365 3a20 4365      Response: Ce
+0002d670: 6e74 7261 6c41 5049 2052 6573 706f 6e73  ntralAPI Respons
+0002d680: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
+0002d690: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
+0002d6a0: 203d 2066 222f 636f 6e66 6967 7572 6174   = f"/configurat
+0002d6b0: 696f 6e2f 7631 2f61 705f 636c 692f 7b67  ion/v1/ap_cli/{g
+0002d6c0: 726f 7570 5f73 7761 726d 6964 7d22 0a0a  roup_swarmid}"..
+0002d6d0: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
+0002d6e0: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
+0002d6f0: 7665 7273 696f 6e27 3a20 7665 7273 696f  version': versio
+0002d700: 6e0a 2020 2020 2020 2020 7d0a 0a20 2020  n.        }..   
+0002d710: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
+0002d720: 7420 7365 6c66 2e67 6574 2875 726c 2c20  t self.get(url, 
+0002d730: 7061 7261 6d73 3d70 6172 616d 7329 0a0a  params=params)..
+0002d740: 2020 2020 6173 796e 6320 6465 6620 7265      async def re
+0002d750: 706c 6163 655f 6170 5f63 6f6e 6669 6728  place_ap_config(
+0002d760: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0002d770: 2020 2020 2020 2067 726f 7570 5f6e 616d         group_nam
+0002d780: 655f 6f72 5f67 7569 643a 2073 7472 2c0a  e_or_guid: str,.
+0002d790: 2020 2020 2020 2020 636c 6973 3a20 4c69          clis: Li
+0002d7a0: 7374 5b73 7472 5d2c 0a20 2020 2029 202d  st[str],.    ) -
+0002d7b0: 3e20 5265 7370 6f6e 7365 3a0a 2020 2020  > Response:.    
+0002d7c0: 2020 2020 2222 2252 6570 6c61 6365 2041      """Replace A
+0002d7d0: 5020 4772 6f75 7020 4c65 7665 6c20 636f  P Group Level co
+0002d7e0: 6e66 6967 7572 6174 696f 6e20 666f 7220  nfiguration for 
+0002d7f0: 5549 2067 726f 7570 2e0a 0a20 2020 2020  UI group...     
+0002d800: 2020 2053 656e 6420 4150 2063 6f6e 6669     Send AP confi
+0002d810: 6775 7261 7469 6f6e 2069 6e20 434c 4920  guration in CLI 
+0002d820: 666f 726d 6174 2061 7320 6120 6c69 7374  format as a list
+0002d830: 206f 6620 7374 7269 6e67 7320 7768 6572   of strings wher
+0002d840: 6520 6561 6368 2069 7465 6d20 696e 2074  e each item in t
+0002d850: 6865 206c 6973 7420 6973 0a20 2020 2020  he list is.     
+0002d860: 2020 2061 206c 696e 6520 6672 6f6d 2074     a line from t
+0002d870: 6865 2063 6f6e 6669 672e 2020 5265 7175  he config.  Requ
+0002d880: 6972 6573 2061 6c6c 206c 696e 6573 206f  ires all lines o
+0002d890: 6620 7468 6520 636f 6e66 6967 2c20 6e6f  f the config, no
+0002d8a0: 7420 6120 7061 7274 6961 6c20 7570 6461  t a partial upda
+0002d8b0: 7465 2e0a 0a20 2020 2020 2020 2041 7267  te...        Arg
+0002d8c0: 733a 0a20 2020 2020 2020 2020 2020 2067  s:.            g
+0002d8d0: 726f 7570 5f6e 616d 655f 6f72 5f67 7569  roup_name_or_gui
+0002d8e0: 6420 2873 7472 293a 2047 726f 7570 206e  d (str): Group n
+0002d8f0: 616d 6520 6f66 2074 6865 2067 726f 7570  ame of the group
+0002d900: 206f 7220 6775 6964 206f 6620 7468 6520   or guid of the 
+0002d910: 7377 6172 6d2e 0a20 2020 2020 2020 2020  swarm..         
+0002d920: 2020 2020 2020 2045 7861 6d70 6c65 3a47         Example:G
+0002d930: 726f 7570 5f31 206f 7220 3661 3564 3132  roup_1 or 6a5d12
+0002d940: 3362 3031 6639 3434 3138 3036 3234 3465  3b01f9441806244e
+0002d950: 6136 6530 3233 6661 6235 3834 3162 3737  a6e023fab5841b77
+0002d960: 6338 3238 6130 3835 6630 3466 2e0a 2020  c828a085f04f..  
+0002d970: 2020 2020 2020 2020 2020 636c 6973 2028            clis (
+0002d980: 4c69 7374 5b73 7472 5d29 3a20 5768 6f6c  List[str]): Whol
+0002d990: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+0002d9a0: 4c69 7374 2069 6e20 434c 4920 666f 726d  List in CLI form
+0002d9b0: 6174 2e0a 0a20 2020 2020 2020 2052 6574  at...        Ret
+0002d9c0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+0002d9d0: 2020 5265 7370 6f6e 7365 3a20 4365 6e74    Response: Cent
+0002d9e0: 7261 6c41 5049 2052 6573 706f 6e73 6520  ralAPI Response 
+0002d9f0: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
+0002da00: 2222 0a20 2020 2020 2020 2075 726c 203d  "".        url =
+0002da10: 2066 222f 636f 6e66 6967 7572 6174 696f   f"/configuratio
+0002da20: 6e2f 7631 2f61 705f 636c 692f 7b67 726f  n/v1/ap_cli/{gro
+0002da30: 7570 5f6e 616d 655f 6f72 5f67 7569 647d  up_name_or_guid}
+0002da40: 220a 0a20 2020 2020 2020 206a 736f 6e5f  "..        json_
+0002da50: 6461 7461 203d 207b 0a20 2020 2020 2020  data = {.       
+0002da60: 2020 2020 2027 636c 6973 273a 2063 6c69       'clis': cli
+0002da70: 730a 2020 2020 2020 2020 7d0a 0a20 2020  s.        }..   
+0002da80: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
+0002da90: 7420 7365 6c66 2e70 6f73 7428 7572 6c2c  t self.post(url,
+0002daa0: 206a 736f 6e5f 6461 7461 3d6a 736f 6e5f   json_data=json_
+0002dab0: 6461 7461 290a 0a20 2020 2061 7379 6e63  data)..    async
+0002dac0: 2064 6566 2067 6574 5f70 6572 5f61 705f   def get_per_ap_
+0002dad0: 636f 6e66 6967 280a 2020 2020 2020 2020  config(.        
+0002dae0: 7365 6c66 2c0a 2020 2020 2020 2020 7365  self,.        se
+0002daf0: 7269 616c 3a20 7374 722c 0a20 2020 2029  rial: str,.    )
+0002db00: 202d 3e20 5265 7370 6f6e 7365 3a0a 2020   -> Response:.  
+0002db10: 2020 2020 2020 2222 2247 6574 2070 6572        """Get per
+0002db20: 2041 5020 7365 7474 696e 672e 0a0a 2020   AP setting...  
+0002db30: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+0002db40: 2020 2020 2020 2020 7365 7269 616c 2028          serial (
+0002db50: 7374 7229 3a20 5365 7269 616c 204e 756d  str): Serial Num
+0002db60: 6265 7220 6f66 2041 500a 0a20 2020 2020  ber of AP..     
+0002db70: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0002db80: 2020 2020 2020 2020 5265 7370 6f6e 7365          Response
+0002db90: 3a20 4365 6e74 7261 6c41 5049 2052 6573  : CentralAPI Res
+0002dba0: 706f 6e73 6520 6f62 6a65 6374 0a20 2020  ponse object.   
+0002dbb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0002dbc0: 2075 726c 203d 2066 222f 636f 6e66 6967   url = f"/config
+0002dbd0: 7572 6174 696f 6e2f 7631 2f61 705f 7365  uration/v1/ap_se
+0002dbe0: 7474 696e 6773 5f63 6c69 2f7b 7365 7269  ttings_cli/{seri
+0002dbf0: 616c 7d22 0a0a 2020 2020 2020 2020 7265  al}"..        re
+0002dc00: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+0002dc10: 6765 7428 7572 6c29 0a0a 2020 2020 6173  get(url)..    as
+0002dc20: 796e 6320 6465 6620 7265 706c 6163 655f  ync def replace_
+0002dc30: 7065 725f 6170 5f63 6f6e 6669 6728 0a20  per_ap_config(. 
+0002dc40: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0002dc50: 2020 2020 2073 6572 6961 6c3a 2073 7472       serial: str
+0002dc60: 2c0a 2020 2020 2020 2020 636c 6973 3a20  ,.        clis: 
+0002dc70: 4c69 7374 5b73 7472 5d2c 0a20 2020 2029  List[str],.    )
+0002dc80: 202d 3e20 5265 7370 6f6e 7365 3a0a 2020   -> Response:.  
+0002dc90: 2020 2020 2020 2222 2252 6570 6c61 6365        """Replace
+0002dca0: 2070 6572 2041 5020 7365 7474 696e 672e   per AP setting.
+0002dcb0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+0002dcc0: 2020 2020 2020 2020 2020 2020 7365 7269              seri
+0002dcd0: 616c 2028 7374 7229 3a20 5365 7269 616c  al (str): Serial
+0002dce0: 204e 756d 6265 7220 6f66 2041 500a 2020   Number of AP.  
+0002dcf0: 2020 2020 2020 2020 2020 636c 6973 2028            clis (
+0002dd00: 4c69 7374 5b73 7472 5d29 3a20 416c 6c20  List[str]): All 
+0002dd10: 7065 7220 4150 2073 6574 7469 6e67 204c  per AP setting L
+0002dd20: 6973 7420 696e 2043 4c49 2066 6f72 6d61  ist in CLI forma
+0002dd30: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0002dd40: 2020 4d75 7374 2070 726f 7669 6465 2061    Must provide a
+0002dd50: 6c6c 2070 6572 2041 5020 7365 7474 696e  ll per AP settin
+0002dd60: 6773 2c20 6e6f 7420 7061 7274 6961 6c0a  gs, not partial.
+0002dd70: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0002dd80: 3a0a 2020 2020 2020 2020 2020 2020 5265  :.            Re
+0002dd90: 7370 6f6e 7365 3a20 4365 6e74 7261 6c41  sponse: CentralA
+0002dda0: 5049 2052 6573 706f 6e73 6520 6f62 6a65  PI Response obje
+0002ddb0: 6374 0a20 2020 2020 2020 2022 2222 0a20  ct.        """. 
+0002ddc0: 2020 2020 2020 2075 726c 203d 2066 222f         url = f"/
+0002ddd0: 636f 6e66 6967 7572 6174 696f 6e2f 7631  configuration/v1
+0002dde0: 2f61 705f 7365 7474 696e 6773 5f63 6c69  /ap_settings_cli
+0002ddf0: 2f7b 7365 7269 616c 7d22 0a0a 2020 2020  /{serial}"..    
+0002de00: 2020 2020 6a73 6f6e 5f64 6174 6120 3d20      json_data = 
+0002de10: 7b0a 2020 2020 2020 2020 2020 2020 2763  {.            'c
+0002de20: 6c69 7327 3a20 636c 6973 0a20 2020 2020  lis': clis.     
+0002de30: 2020 207d 0a0a 2020 2020 2020 2020 7265     }..        re
+0002de40: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+0002de50: 706f 7374 2875 726c 2c20 6a73 6f6e 5f64  post(url, json_d
+0002de60: 6174 613d 6a73 6f6e 5f64 6174 6129 0a0a  ata=json_data)..
+0002de70: 2020 2020 6173 796e 6320 6465 6620 6765      async def ge
+0002de80: 745f 6272 6163 685f 6865 616c 7468 280a  t_brach_health(.
+0002de90: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0002dea0: 2020 2020 2020 6e61 6d65 3a20 7374 7220        name: str 
+0002deb0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0002dec0: 636f 6c75 6d6e 3a20 696e 7420 3d20 4e6f  column: int = No
+0002ded0: 6e65 2c0a 2020 2020 2020 2020 7265 7665  ne,.        reve
+0002dee0: 7273 653a 2062 6f6f 6c20 3d20 4661 6c73  rse: bool = Fals
+0002def0: 652c 0a20 2020 2020 2020 2066 696c 7465  e,.        filte
+0002df00: 7273 3a20 6469 6374 203d 207b 7d2c 0a20  rs: dict = {},. 
+0002df10: 2020 2020 2020 206f 6666 7365 743a 2069         offset: i
+0002df20: 6e74 203d 2030 2c0a 2020 2020 2020 2020  nt = 0,.        
+0002df30: 6c69 6d69 743a 2069 6e74 203d 2031 3030  limit: int = 100
+0002df40: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
+0002df50: 6e73 653a 0a20 2020 2020 2020 2022 2222  nse:.        """
+0002df60: 4765 7420 6461 7461 2066 6f72 2061 6c6c  Get data for all
+0002df70: 2073 6974 6573 2e0a 0a20 2020 2020 2020   sites...       
+0002df80: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0002df90: 2020 206e 616d 6520 2873 7472 2c20 6f70     name (str, op
+0002dfa0: 7469 6f6e 616c 293a 2073 6974 6520 2f20  tional): site / 
+0002dfb0: 6c61 6265 6c20 6e61 6d65 206f 7220 7061  label name or pa
+0002dfc0: 7274 206f 6620 6974 7320 6e61 6d65 0a20  rt of its name. 
+0002dfd0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+0002dfe0: 6e20 2869 6e74 2c20 6f70 7469 6f6e 616c  n (int, optional
+0002dff0: 293a 2043 6f6c 756d 6e20 746f 2073 6f72  ): Column to sor
+0002e000: 7420 6f6e 0a20 2020 2020 2020 2020 2020  t on.           
+0002e010: 2072 6576 6572 7365 2028 626f 6f6c 2c20   reverse (bool, 
+0002e020: 6f70 7469 6f6e 616c 293a 2053 6f72 7420  optional): Sort 
+0002e030: 696e 2072 6576 6572 7365 206f 7264 6572  in reverse order
+0002e040: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002e050: 2020 5661 6c69 6420 5661 6c75 6573 3a20    Valid Values: 
+0002e060: 6173 632c 2064 6573 630a 2020 2020 2020  asc, desc.      
+0002e070: 2020 2020 2020 2020 2020 2a20 6173 6320            * asc 
+0002e080: 2d20 4173 6365 6e64 696e 672c 2066 726f  - Ascending, fro
+0002e090: 6d20 4120 746f 205a 2e0a 2020 2020 2020  m A to Z..      
+0002e0a0: 2020 2020 2020 2020 2020 2a20 6465 7363            * desc
+0002e0b0: 202d 2044 6573 6365 6e64 696e 672c 2066   - Descending, f
+0002e0c0: 726f 6d20 5a20 746f 2041 2e0a 0a0a 2020  rom Z to A....  
+0002e0d0: 2020 2020 2020 2020 2020 6669 6c74 6572            filter
+0002e0e0: 7320 2873 7472 2c20 6f70 7469 6f6e 616c  s (str, optional
+0002e0f0: 293a 2053 6974 6520 7468 7265 7368 6f6c  ): Site threshol
+0002e100: 6473 0a20 2020 2020 2020 2020 2020 2020  ds.             
+0002e110: 2020 2056 616c 6964 2056 616c 7565 733a     Valid Values:
+0002e120: 2067 7420 2028 4772 6561 7465 7220 7468   gt  (Greater th
+0002e130: 616e 292c 206c 7420 2028 4c65 7373 2074  an), lt  (Less t
+0002e140: 6861 6e29 2c20 6774 6520 2847 7265 6174  han), gte (Great
+0002e150: 6572 2074 6861 6e20 6f72 2065 7175 616c  er than or equal
+0002e160: 2074 6f29 2c0a 2020 2020 2020 2020 2020   to),.          
+0002e170: 2020 2020 2020 6c74 6520 284c 6573 7320        lte (Less 
+0002e180: 7468 616e 206f 7220 6571 7561 6c20 746f  than or equal to
+0002e190: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0002e1a0: 2020 2a20 416c 6c20 7072 6f70 6572 7469    * All properti
+0002e1b0: 6573 206f 6620 6120 7369 7465 2063 616e  es of a site can
+0002e1c0: 2062 6520 7573 6564 2061 7320 6669 6c74   be used as filt
+0002e1d0: 6572 2070 6172 616d 6574 6572 7320 7769  er parameters wi
+0002e1e0: 7468 2061 2074 6872 6573 686f 6c64 0a20  th a threshold. 
+0002e1f0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+0002e200: 2054 6865 2072 616e 6765 2066 696c 7465   The range filte
+0002e210: 7273 2063 616e 2062 6520 636f 6d62 696e  rs can be combin
+0002e220: 6564 2077 6974 6820 7468 6520 636f 6c75  ed with the colu
+0002e230: 6d6e 206e 616d 6573 2077 6974 6820 225c  mn names with "\
+0002e240: 5f5f 2220 2023 206e 6f71 610a 2020 2020  __"  # noqa.    
+0002e250: 2020 2020 2020 2020 2020 2020 2a20 466f              * Fo
+0002e260: 7220 6567 2e20 2f73 6974 653f 6465 7669  r eg. /site?devi
+0002e270: 6365 5f64 6f77 6e5c 5f5f 6774 3d30 202d  ce_down\__gt=0 -
+0002e280: 204c 6973 7473 2061 6c6c 2073 6974 6573   Lists all sites
+0002e290: 2074 6861 7420 6861 7665 206d 6f72 6520   that have more 
+0002e2a0: 7468 616e 2031 2064 6576 6963 6520 696e  than 1 device in
+0002e2b0: 2064 6f77 6e20 7374 6174 6520 2320 6e6f   down state # no
+0002e2c0: 7161 0a20 2020 2020 2020 2020 2020 2020  qa.             
+0002e2d0: 2020 202a 2046 6f72 2065 672e 202f 7369     * For eg. /si
+0002e2e0: 7465 3f77 616e 5f75 706c 696e 6b73 5f64  te?wan_uplinks_d
+0002e2f0: 6f77 6e5c 5f5f 6c74 3d31 202d 204c 6973  own\__lt=1 - Lis
+0002e300: 7473 2061 6c6c 2073 6974 6573 2074 6861  ts all sites tha
+0002e310: 7420 6861 7665 206c 6573 7320 7468 616e  t have less than
+0002e320: 2031 2077 616e 2069 6e20 646f 776e 2073   1 wan in down s
+0002e330: 7461 7465 2023 206e 6f71 610a 2020 2020  tate # noqa.    
+0002e340: 2020 2020 2020 2020 2020 2020 2a20 466f              * Fo
+0002e350: 7220 6567 2e20 2f73 6974 653f 6465 7669  r eg. /site?devi
+0002e360: 6365 5f75 705f 5f67 743d 3126 6465 7669  ce_up__gt=1&devi
+0002e370: 6365 5f75 705c 5f5f 6c74 3d31 3020 2d20  ce_up\__lt=10 - 
+0002e380: 4c69 7374 7320 616c 6c20 7369 7465 7320  Lists all sites 
+0002e390: 7468 6174 2068 6176 6520 312d 3130 2064  that have 1-10 d
+0002e3a0: 6576 6963 6573 2075 7020 2320 6e6f 7161  evices up # noqa
+0002e3b0: 0a0a 0a20 2020 2020 2020 2020 2020 206f  ...            o
+0002e3c0: 6666 7365 7420 2869 6e74 2c20 6f70 7469  ffset (int, opti
+0002e3d0: 6f6e 616c 293a 2070 6167 696e 6174 696f  onal): paginatio
+0002e3e0: 6e20 7374 6172 7420 696e 6465 7820 4465  n start index De
+0002e3f0: 6661 756c 7473 2074 6f20 302e 0a20 2020  faults to 0..   
+0002e400: 2020 2020 2020 2020 206c 696d 6974 2028           limit (
+0002e410: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
+0002e420: 7061 6769 6e61 7469 6f6e 2073 697a 6520  pagination size 
+0002e430: 4465 6661 756c 7473 2074 6f20 3130 302e  Defaults to 100.
+0002e440: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0002e450: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
+0002e460: 6573 706f 6e73 653a 2043 656e 7472 616c  esponse: Central
+0002e470: 4150 4920 5265 7370 6f6e 7365 206f 626a  API Response obj
+0002e480: 6563 740a 2020 2020 2020 2020 2222 220a  ect.        """.
+0002e490: 2020 2020 2020 2020 7572 6c20 3d20 222f          url = "/
+0002e4a0: 6272 616e 6368 6865 616c 7468 2f76 312f  branchhealth/v1/
+0002e4b0: 7369 7465 220a 0a20 2020 2020 2020 2070  site"..        p
+0002e4c0: 6172 616d 7320 3d20 7b0a 2020 2020 2020  arams = {.      
+0002e4d0: 2020 2020 2020 226e 616d 6522 3a20 6e61        "name": na
+0002e4e0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+0002e4f0: 2320 2263 6f6c 756d 6e22 3a20 636f 6c75  # "column": colu
+0002e500: 6d6e 2c0a 2020 2020 2020 2020 2020 2020  mn,.            
+0002e510: 226f 7264 6572 223a 2022 6173 6322 2069  "order": "asc" i
+0002e520: 6620 6e6f 7420 7265 7665 7273 6520 656c  f not reverse el
+0002e530: 7365 2022 6465 7363 222c 0a20 2020 2020  se "desc",.     
+0002e540: 2020 2020 2020 2023 2022 7761 6e5f 7475         # "wan_tu
+0002e550: 6e6e 656c 735f 646f 776e 5c5f 5f67 7422  nnels_down\__gt"
+0002e560: 3a20 2230 222c 0a20 2020 2020 2020 2020  : "0",.         
+0002e570: 2020 2023 2022 7761 6e5f 7570 6c69 6e6b     # "wan_uplink
+0002e580: 735f 646f 776e 5c5f 5f67 7422 3a20 2230  s_down\__gt": "0
+0002e590: 222c 0a20 2020 2020 2020 2020 2020 2023  ",.            #
+0002e5a0: 202a 2a66 696c 7465 7273 2c0a 2020 2020   **filters,.    
+0002e5b0: 2020 2020 2020 2020 226f 6666 7365 7422          "offset"
+0002e5c0: 3a20 6f66 6673 6574 2c0a 2020 2020 2020  : offset,.      
+0002e5d0: 2020 2020 2020 226c 696d 6974 223a 206c        "limit": l
+0002e5e0: 696d 6974 2c0a 2020 2020 2020 2020 7d0a  imit,.        }.
+0002e5f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002e600: 6177 6169 7420 7365 6c66 2e67 6574 2875  await self.get(u
+0002e610: 726c 2c20 7061 7261 6d73 3d70 6172 616d  rl, params=param
+0002e620: 7329 0a0a 2020 2020 6173 796e 6320 6465  s)..    async de
+0002e630: 6620 6765 745f 6172 6368 6976 6564 5f64  f get_archived_d
+0002e640: 6576 6963 6573 280a 2020 2020 2020 2020  evices(.        
+0002e650: 7365 6c66 2c0a 2020 2020 2020 2020 6f66  self,.        of
+0002e660: 6673 6574 3a20 696e 7420 3d20 302c 0a20  fset: int = 0,. 
+0002e670: 2020 2020 2020 206c 696d 6974 3a20 696e         limit: in
+0002e680: 7420 3d20 3130 302c 0a20 2020 2029 202d  t = 100,.    ) -
+0002e690: 3e20 5265 7370 6f6e 7365 3a0a 2020 2020  > Response:.    
+0002e6a0: 2020 2020 2222 2247 6574 2041 7263 6869      """Get Archi
+0002e6b0: 7665 6420 6465 7669 6365 7320 6672 6f6d  ved devices from
+0002e6c0: 2064 6576 6963 6520 696e 7665 6e74 6f72   device inventor
+0002e6d0: 792e 0a0a 2020 2020 2020 2020 2f2f 2055  y...        // U
+0002e6e0: 7365 6420 6279 2073 686f 7720 6172 6368  sed by show arch
+0002e6f0: 6976 6564 202f 2f0a 0a20 2020 2020 2020  ived //..       
+0002e700: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0002e710: 2020 206f 6666 7365 7420 2869 6e74 2c20     offset (int, 
+0002e720: 6f70 7469 6f6e 616c 293a 206f 6666 7365  optional): offse
+0002e730: 7420 6f72 2070 6167 6520 6e75 6d62 6572  t or page number
+0002e740: 2044 6566 6175 6c74 7320 746f 2030 2e0a   Defaults to 0..
+0002e750: 2020 2020 2020 2020 2020 2020 6c69 6d69              limi
+0002e760: 7420 2869 6e74 2c20 6f70 7469 6f6e 616c  t (int, optional
+0002e770: 293a 204e 756d 6265 7220 6f66 2064 6576  ): Number of dev
+0002e780: 6963 6573 2074 6f20 6765 7420 4465 6661  ices to get Defa
+0002e790: 756c 7473 2074 6f20 3130 302e 0a0a 2020  ults to 100...  
+0002e7a0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+0002e7b0: 2020 2020 2020 2020 2020 2052 6573 706f             Respo
+0002e7c0: 6e73 653a 2043 656e 7472 616c 4150 4920  nse: CentralAPI 
+0002e7d0: 5265 7370 6f6e 7365 206f 626a 6563 740a  Response object.
+0002e7e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0002e7f0: 2020 2020 7572 6c20 3d20 222f 706c 6174      url = "/plat
+0002e800: 666f 726d 2f64 6576 6963 655f 696e 7665  form/device_inve
+0002e810: 6e74 6f72 792f 7631 2f64 6576 6963 6573  ntory/v1/devices
+0002e820: 2f61 7263 6869 7665 220a 0a20 2020 2020  /archive"..     
+0002e830: 2020 2070 6172 616d 7320 3d20 7b0a 2020     params = {.  
+0002e840: 2020 2020 2020 2020 2020 276f 6666 7365            'offse
+0002e850: 7427 3a20 6f66 6673 6574 2c0a 2020 2020  t': offset,.    
+0002e860: 2020 2020 2020 2020 276c 696d 6974 273a          'limit':
+0002e870: 206c 696d 6974 0a20 2020 2020 2020 207d   limit.        }
+0002e880: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0002e890: 2061 7761 6974 2073 656c 662e 6765 7428   await self.get(
+0002e8a0: 7572 6c2c 2070 6172 616d 733d 7061 7261  url, params=para
+0002e8b0: 6d73 290a 0a20 2020 2061 7379 6e63 2064  ms)..    async d
+0002e8c0: 6566 2061 7263 6869 7665 5f64 6576 6963  ef archive_devic
+0002e8d0: 6573 280a 2020 2020 2020 2020 7365 6c66  es(.        self
+0002e8e0: 2c0a 2020 2020 2020 2020 7365 7269 616c  ,.        serial
+0002e8f0: 733a 204c 6973 745b 7374 725d 2c0a 2020  s: List[str],.  
+0002e900: 2020 2920 2d3e 2052 6573 706f 6e73 653a    ) -> Response:
+0002e910: 0a20 2020 2020 2020 2022 2222 4172 6368  .        """Arch
+0002e920: 6976 6520 6465 7669 6365 7320 7573 696e  ive devices usin
+0002e930: 6720 5365 7269 616c 206c 6973 742e 0a0a  g Serial list...
+0002e940: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0002e950: 2020 2020 2020 2020 2020 7365 7269 616c            serial
+0002e960: 7320 284c 6973 745b 7374 725d 293a 2073  s (List[str]): s
+0002e970: 6572 6961 6c73 0a0a 2020 2020 2020 2020  erials..        
+0002e980: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0002e990: 2020 2020 2052 6573 706f 6e73 653a 2043       Response: C
+0002e9a0: 656e 7472 616c 4150 4920 5265 7370 6f6e  entralAPI Respon
+0002e9b0: 7365 206f 626a 6563 740a 2020 2020 2020  se object.      
+0002e9c0: 2020 2222 220a 2020 2020 2020 2020 7572    """.        ur
+0002e9d0: 6c20 3d20 222f 706c 6174 666f 726d 2f64  l = "/platform/d
+0002e9e0: 6576 6963 655f 696e 7665 6e74 6f72 792f  evice_inventory/
+0002e9f0: 7631 2f64 6576 6963 6573 2f61 7263 6869  v1/devices/archi
+0002ea00: 7665 220a 0a20 2020 2020 2020 206a 736f  ve"..        jso
+0002ea10: 6e5f 6461 7461 203d 207b 0a20 2020 2020  n_data = {.     
+0002ea20: 2020 2020 2020 2027 7365 7269 616c 7327         'serials'
+0002ea30: 3a20 7574 696c 732e 6c69 7374 6966 7928  : utils.listify(
+0002ea40: 7365 7269 616c 7329 0a20 2020 2020 2020  serials).       
+0002ea50: 207d 0a0a 2020 2020 2020 2020 7265 7475   }..        retu
+0002ea60: 726e 2061 7761 6974 2073 656c 662e 706f  rn await self.po
+0002ea70: 7374 2875 726c 2c20 6a73 6f6e 5f64 6174  st(url, json_dat
+0002ea80: 613d 6a73 6f6e 5f64 6174 6129 0a0a 2020  a=json_data)..  
+0002ea90: 2020 2320 4150 492d 4e4f 5445 2063 656e    # API-NOTE cen
+0002eaa0: 636c 6920 7265 6d6f 7665 2061 7263 6869  cli remove archi
+0002eab0: 7665 205b 6465 7669 6365 735d 0a20 2020  ve [devices].   
+0002eac0: 2061 7379 6e63 2064 6566 2075 6e61 7263   async def unarc
+0002ead0: 6869 7665 5f64 6576 6963 6573 280a 2020  hive_devices(.  
+0002eae0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0002eaf0: 2020 2020 7365 7269 616c 733a 204c 6973      serials: Lis
+0002eb00: 745b 7374 725d 2c0a 2020 2020 2920 2d3e  t[str],.    ) ->
+0002eb10: 2052 6573 706f 6e73 653a 0a20 2020 2020   Response:.     
+0002eb20: 2020 2022 2222 556e 6172 6368 6976 6520     """Unarchive 
+0002eb30: 6465 7669 6365 7320 7573 696e 6720 5365  devices using Se
+0002eb40: 7269 616c 206c 6973 742e 0a0a 2020 2020  rial list...    
+0002eb50: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0002eb60: 2020 2020 2020 7365 7269 616c 7320 284c        serials (L
+0002eb70: 6973 745b 7374 725d 293a 2073 6572 6961  ist[str]): seria
+0002eb80: 6c73 0a0a 2020 2020 2020 2020 5265 7475  ls..        Retu
+0002eb90: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0002eba0: 2052 6573 706f 6e73 653a 2043 656e 7472   Response: Centr
+0002ebb0: 616c 4150 4920 5265 7370 6f6e 7365 206f  alAPI Response o
+0002ebc0: 626a 6563 740a 2020 2020 2020 2020 2222  bject.        ""
+0002ebd0: 220a 2020 2020 2020 2020 7572 6c20 3d20  ".        url = 
+0002ebe0: 222f 706c 6174 666f 726d 2f64 6576 6963  "/platform/devic
+0002ebf0: 655f 696e 7665 6e74 6f72 792f 7631 2f64  e_inventory/v1/d
+0002ec00: 6576 6963 6573 2f75 6e61 7263 6869 7665  evices/unarchive
+0002ec10: 220a 0a20 2020 2020 2020 206a 736f 6e5f  "..        json_
+0002ec20: 6461 7461 203d 207b 0a20 2020 2020 2020  data = {.       
+0002ec30: 2020 2020 2027 7365 7269 616c 7327 3a20       'serials': 
+0002ec40: 7574 696c 732e 6c69 7374 6966 7928 7365  utils.listify(se
+0002ec50: 7269 616c 7329 0a20 2020 2020 2020 207d  rials).        }
+0002ec60: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0002ec70: 2061 7761 6974 2073 656c 662e 706f 7374   await self.post
+0002ec80: 2875 726c 2c20 6a73 6f6e 5f64 6174 613d  (url, json_data=
+0002ec90: 6a73 6f6e 5f64 6174 6129 0a0a 2020 2020  json_data)..    
+0002eca0: 6173 796e 6320 6465 6620 6765 745f 706f  async def get_po
+0002ecb0: 7274 616c 7328 0a20 2020 2020 2020 2073  rtals(.        s
+0002ecc0: 656c 662c 0a20 2020 2020 2020 2073 6f72  elf,.        sor
+0002ecd0: 743a 2073 7472 203d 2027 2b6e 616d 6527  t: str = '+name'
+0002ece0: 2c0a 2020 2020 2020 2020 6f66 6673 6574  ,.        offset
+0002ecf0: 3a20 696e 7420 3d20 302c 0a20 2020 2020  : int = 0,.     
+0002ed00: 2020 206c 696d 6974 3a20 696e 7420 3d20     limit: int = 
+0002ed10: 3130 302c 0a20 2020 2029 202d 3e20 5265  100,.    ) -> Re
+0002ed20: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
+0002ed30: 2222 2247 6574 2061 6c6c 2070 6f72 7461  """Get all porta
+0002ed40: 6c73 2077 6974 6820 6c69 6d69 7465 6420  ls with limited 
+0002ed50: 6461 7461 2e0a 0a20 2020 2020 2020 2041  data...        A
+0002ed60: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0002ed70: 2073 6f72 7420 2873 7472 2c20 6f70 7469   sort (str, opti
+0002ed80: 6f6e 616c 293a 202b 2069 7320 666f 7220  onal): + is for 
+0002ed90: 6173 6365 6e64 696e 6720 2061 6e64 202d  ascending  and -
+0002eda0: 2066 6f72 2064 6573 6365 6e64 696e 6720   for descending 
+0002edb0: 6f72 6465 7220 2c20 736f 7274 7320 6279  order , sorts by
+0002edc0: 206e 616d 6520 666f 7220 6e6f 770a 2020   name for now.  
+0002edd0: 2020 2020 2020 2020 2020 2020 2020 5661                Va
+0002ede0: 6c69 6420 5661 6c75 6573 3a20 2b6e 616d  lid Values: +nam
+0002edf0: 652c 202d 6e61 6d65 0a20 2020 2020 2020  e, -name.       
+0002ee00: 2020 2020 206f 6666 7365 7420 2869 6e74       offset (int
+0002ee10: 2c20 6f70 7469 6f6e 616c 293a 2053 7461  , optional): Sta
+0002ee20: 7274 696e 6720 696e 6465 7820 6f66 2065  rting index of e
+0002ee30: 6c65 6d65 6e74 2066 6f72 2061 2070 6167  lement for a pag
+0002ee40: 696e 6174 6564 2071 7565 7279 2044 6566  inated query Def
+0002ee50: 6175 6c74 7320 746f 2030 2e0a 2020 2020  aults to 0..    
+0002ee60: 2020 2020 2020 2020 6c69 6d69 7420 2869          limit (i
+0002ee70: 6e74 2c20 6f70 7469 6f6e 616c 293a 204e  nt, optional): N
+0002ee80: 756d 6265 7220 6f66 2069 7465 6d73 2072  umber of items r
+0002ee90: 6571 7569 7265 6420 7065 7220 7175 6572  equired per quer
+0002eea0: 7920 4465 6661 756c 7473 2074 6f20 3130  y Defaults to 10
+0002eeb0: 302e 0a0a 2020 2020 2020 2020 5265 7475  0...        Retu
+0002eec0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0002eed0: 2052 6573 706f 6e73 653a 2043 656e 7472   Response: Centr
+0002eee0: 616c 4150 4920 5265 7370 6f6e 7365 206f  alAPI Response o
+0002eef0: 626a 6563 740a 2020 2020 2020 2020 2222  bject.        ""
+0002ef00: 220a 2020 2020 2020 2020 7572 6c20 3d20  ".        url = 
+0002ef10: 222f 6775 6573 742f 7631 2f70 6f72 7461  "/guest/v1/porta
+0002ef20: 6c73 220a 0a20 2020 2020 2020 2070 6172  ls"..        par
+0002ef30: 616d 7320 3d20 7b0a 2020 2020 2020 2020  ams = {.        
+0002ef40: 2020 2020 2773 6f72 7427 3a20 736f 7274      'sort': sort
+0002ef50: 2c0a 2020 2020 2020 2020 2020 2020 276f  ,.            'o
+0002ef60: 6666 7365 7427 3a20 6f66 6673 6574 2c0a  ffset': offset,.
+0002ef70: 2020 2020 2020 2020 2020 2020 276c 696d              'lim
+0002ef80: 6974 273a 206c 696d 6974 0a20 2020 2020  it': limit.     
+0002ef90: 2020 207d 0a0a 2020 2020 2020 2020 7265     }..        re
+0002efa0: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+0002efb0: 6765 7428 7572 6c2c 2070 6172 616d 733d  get(url, params=
+0002efc0: 7061 7261 6d73 290a 0a20 2020 2061 7379  params)..    asy
+0002efd0: 6e63 2064 6566 2067 6574 5f76 6973 6974  nc def get_visit
+0002efe0: 6f72 7328 0a20 2020 2020 2020 2073 656c  ors(.        sel
+0002eff0: 662c 0a20 2020 2020 2020 2070 6f72 7461  f,.        porta
+0002f000: 6c5f 6964 3a20 7374 722c 0a20 2020 2020  l_id: str,.     
+0002f010: 2020 2073 6f72 743a 2073 7472 203d 2027     sort: str = '
+0002f020: 2b6e 616d 6527 2c0a 2020 2020 2020 2020  +name',.        
+0002f030: 6669 6c74 6572 5f62 793a 2073 7472 203d  filter_by: str =
+0002f040: 204e 6f6e 652c 0a20 2020 2020 2020 2066   None,.        f
+0002f050: 696c 7465 725f 7661 6c75 653a 2073 7472  ilter_value: str
+0002f060: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0002f070: 206f 6666 7365 743a 2069 6e74 203d 2030   offset: int = 0
+0002f080: 2c0a 2020 2020 2020 2020 6c69 6d69 743a  ,.        limit:
+0002f090: 2069 6e74 203d 2031 3030 2c0a 2020 2020   int = 100,.    
+0002f0a0: 2920 2d3e 2052 6573 706f 6e73 653a 0a20  ) -> Response:. 
+0002f0b0: 2020 2020 2020 2022 2222 4765 7420 616c         """Get al
+0002f0c0: 6c20 7669 7369 746f 7273 2063 7265 6174  l visitors creat
+0002f0d0: 6564 2061 6761 696e 7374 2061 2070 6f72  ed against a por
+0002f0e0: 7461 6c2e 0a0a 2020 2020 2020 2020 4172  tal...        Ar
+0002f0f0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0002f100: 706f 7274 616c 5f69 6420 2873 7472 293a  portal_id (str):
+0002f110: 2050 6f72 7461 6c20 4944 206f 6620 7468   Portal ID of th
+0002f120: 6520 7370 6c61 7368 2070 6167 650a 2020  e splash page.  
+0002f130: 2020 2020 2020 2020 2020 736f 7274 2028            sort (
+0002f140: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+0002f150: 2b20 6973 2066 6f72 2061 7363 656e 6469  + is for ascendi
+0002f160: 6e67 2020 616e 6420 2d20 666f 7220 6465  ng  and - for de
+0002f170: 7363 656e 6469 6e67 206f 7264 6572 202c  scending order ,
+0002f180: 2073 6f72 7473 2062 7920 6e61 6d65 2066   sorts by name f
+0002f190: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
+0002f1a0: 2020 206e 6f77 2020 5661 6c69 6420 5661     now  Valid Va
+0002f1b0: 6c75 6573 3a20 2b6e 616d 652c 202d 6e61  lues: +name, -na
+0002f1c0: 6d65 0a20 2020 2020 2020 2020 2020 2066  me.            f
+0002f1d0: 696c 7465 725f 6279 2028 7374 722c 206f  ilter_by (str, o
+0002f1e0: 7074 696f 6e61 6c29 3a20 6669 6c74 6572  ptional): filter
+0002f1f0: 2062 7920 656d 6169 6c20 6f72 206e 616d   by email or nam
+0002f200: 6520 2056 616c 6964 2056 616c 7565 733a  e  Valid Values:
+0002f210: 206e 616d 652c 2065 6d61 696c 0a20 2020   name, email.   
+0002f220: 2020 2020 2020 2020 2066 696c 7465 725f           filter_
+0002f230: 7661 6c75 6520 2873 7472 2c20 6f70 7469  value (str, opti
+0002f240: 6f6e 616c 293a 2066 696c 7465 7220 7661  onal): filter va
+0002f250: 6c75 650a 2020 2020 2020 2020 2020 2020  lue.            
+0002f260: 6f66 6673 6574 2028 696e 742c 206f 7074  offset (int, opt
+0002f270: 696f 6e61 6c29 3a20 5374 6172 7469 6e67  ional): Starting
+0002f280: 2069 6e64 6578 206f 6620 656c 656d 656e   index of elemen
+0002f290: 7420 666f 7220 6120 7061 6769 6e61 7465  t for a paginate
+0002f2a0: 6420 7175 6572 7920 4465 6661 756c 7473  d query Defaults
+0002f2b0: 2074 6f20 302e 0a20 2020 2020 2020 2020   to 0..         
+0002f2c0: 2020 206c 696d 6974 2028 696e 742c 206f     limit (int, o
+0002f2d0: 7074 696f 6e61 6c29 3a20 4e75 6d62 6572  ptional): Number
+0002f2e0: 206f 6620 6974 656d 7320 7265 7175 6972   of items requir
+0002f2f0: 6564 2070 6572 2071 7565 7279 2044 6566  ed per query Def
+0002f300: 6175 6c74 7320 746f 2031 3030 2e0a 0a20  aults to 100... 
+0002f310: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+0002f320: 2020 2020 2020 2020 2020 2020 5265 7370              Resp
+0002f330: 6f6e 7365 3a20 4365 6e74 7261 6c41 5049  onse: CentralAPI
+0002f340: 2052 6573 706f 6e73 6520 6f62 6a65 6374   Response object
+0002f350: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0002f360: 2020 2020 2075 726c 203d 2066 222f 6775       url = f"/gu
+0002f370: 6573 742f 7631 2f70 6f72 7461 6c73 2f7b  est/v1/portals/{
+0002f380: 706f 7274 616c 5f69 647d 2f76 6973 6974  portal_id}/visit
+0002f390: 6f72 7322 0a0a 2020 2020 2020 2020 7061  ors"..        pa
+0002f3a0: 7261 6d73 203d 207b 0a20 2020 2020 2020  rams = {.       
+0002f3b0: 2020 2020 2027 736f 7274 273a 2073 6f72       'sort': sor
+0002f3c0: 742c 0a20 2020 2020 2020 2020 2020 2027  t,.            '
+0002f3d0: 6669 6c74 6572 5f62 7927 3a20 6669 6c74  filter_by': filt
+0002f3e0: 6572 5f62 792c 0a20 2020 2020 2020 2020  er_by,.         
+0002f3f0: 2020 2027 6669 6c74 6572 5f76 616c 7565     'filter_value
+0002f400: 273a 2066 696c 7465 725f 7661 6c75 652c  ': filter_value,
+0002f410: 0a20 2020 2020 2020 2020 2020 2027 6f66  .            'of
+0002f420: 6673 6574 273a 206f 6666 7365 742c 0a20  fset': offset,. 
+0002f430: 2020 2020 2020 2020 2020 2027 6c69 6d69             'limi
+0002f440: 7427 3a20 6c69 6d69 740a 2020 2020 2020  t': limit.      
+0002f450: 2020 7d0a 2020 2020 2020 2020 7061 7261    }.        para
+0002f460: 6d73 203d 2075 7469 6c73 2e73 7472 6970  ms = utils.strip
+0002f470: 5f6e 6f6e 6528 7061 7261 6d73 290a 0a20  _none(params).. 
+0002f480: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
+0002f490: 6169 7420 7365 6c66 2e67 6574 2875 726c  ait self.get(url
+0002f4a0: 2c20 7061 7261 6d73 3d70 6172 616d 7329  , params=params)
+0002f4b0: 0a0a 0a20 2020 2061 7379 6e63 2064 6566  ...    async def
+0002f4c0: 2061 6464 5f76 6973 6974 6f72 280a 2020   add_visitor(.  
+0002f4d0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0002f4e0: 2020 2020 706f 7274 616c 5f69 643a 2073      portal_id: s
+0002f4f0: 7472 2c0a 2020 2020 2020 2020 6e61 6d65  tr,.        name
+0002f500: 3a20 7374 722c 0a20 2020 2020 2020 2023  : str,.        #
+0002f510: 2069 643a 2073 7472 2c0a 2020 2020 2020   id: str,.      
+0002f520: 2020 7061 7373 776f 7264 3a20 7374 7220    password: str 
+0002f530: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0002f540: 2a2c 0a20 2020 2020 2020 2063 6f6d 7061  *,.        compa
+0002f550: 6e79 5f6e 616d 653a 2073 7472 203d 204e  ny_name: str = N
+0002f560: 6f6e 652c 0a20 2020 2020 2020 2070 686f  one,.        pho
+0002f570: 6e65 3a20 7374 7220 7c20 4e6f 6e65 203d  ne: str | None =
+0002f580: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
+0002f590: 6d61 696c 3a20 7374 7220 7c20 4e6f 6e65  mail: str | None
+0002f5a0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0002f5b0: 2076 616c 6964 5f66 6f72 6576 6572 3a20   valid_forever: 
+0002f5c0: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+0002f5d0: 2020 2020 2020 7661 6c69 645f 6461 7973        valid_days
+0002f5e0: 3a20 696e 7420 3d20 332c 0a20 2020 2020  : int = 3,.     
+0002f5f0: 2020 2076 616c 6964 5f68 6f75 7273 3a20     valid_hours: 
+0002f600: 696e 7420 3d20 302c 0a20 2020 2020 2020  int = 0,.       
+0002f610: 2076 616c 6964 5f6d 696e 7574 6573 3a20   valid_minutes: 
+0002f620: 696e 7420 3d20 302c 0a20 2020 2020 2020  int = 0,.       
+0002f630: 206e 6f74 6966 793a 2062 6f6f 6c20 7c20   notify: bool | 
+0002f640: 4e6f 6e65 203d 204e 6f6e 652c 0a20 2020  None = None,.   
+0002f650: 2020 2020 206e 6f74 6966 795f 746f 3a20       notify_to: 
+0002f660: 636f 6e73 7461 6e74 732e 4e6f 7469 6679  constants.Notify
+0002f670: 546f 4172 6773 207c 204e 6f6e 6520 3d20  ToArgs | None = 
+0002f680: 4e6f 6e65 2c0a 2020 2020 2020 2020 6973  None,.        is
+0002f690: 5f65 6e61 626c 6564 3a20 626f 6f6c 203d  _enabled: bool =
+0002f6a0: 2054 7275 652c 0a20 2020 2020 2020 2023   True,.        #
+0002f6b0: 2073 7461 7475 733a 2062 6f6f 6c2c 0a20   status: bool,. 
+0002f6c0: 2020 2020 2020 2023 2063 7265 6174 6564         # created
+0002f6d0: 5f61 743a 2073 7472 2c0a 2020 2020 2020  _at: str,.      
+0002f6e0: 2020 2320 6578 7069 7265 5f61 743a 2073    # expire_at: s
+0002f6f0: 7472 2c0a 2020 2020 2920 2d3e 2052 6573  tr,.    ) -> Res
+0002f700: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
+0002f710: 2222 4372 6561 7465 2061 206e 6577 2067  ""Create a new g
+0002f720: 7565 7374 2076 6973 6974 6f72 206f 6620  uest visitor of 
+0002f730: 6120 706f 7274 616c 2e0a 0a20 2020 2020  a portal...     
+0002f740: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0002f750: 2020 2020 2070 6f72 7461 6c5f 6964 2028       portal_id (
+0002f760: 7374 7229 3a20 506f 7274 616c 2049 4420  str): Portal ID 
+0002f770: 6f66 2074 6865 2073 706c 6173 6820 7061  of the splash pa
+0002f780: 6765 0a20 2020 2020 2020 2020 2020 206e  ge.            n
+0002f790: 616d 6520 2873 7472 293a 2056 6973 6974  ame (str): Visit
+0002f7a0: 6f72 2061 6363 6f75 6e74 206e 616d 650a  or account name.
+0002f7b0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+0002f7c0: 776f 7264 2028 7374 7229 3a20 5061 7373  word (str): Pass
+0002f7d0: 776f 7264 0a20 2020 2020 2020 2020 2020  word.           
+0002f7e0: 2063 6f6d 7061 6e79 5f6e 616d 6520 2873   company_name (s
+0002f7f0: 7472 293a 2043 6f6d 7061 6e79 206e 616d  tr): Company nam
+0002f800: 6520 6f66 2074 6865 2076 6973 6974 6f72  e of the visitor
+0002f810: 0a20 2020 2020 2020 2020 2020 2070 686f  .            pho
+0002f820: 6e65 2028 7374 7229 3a20 5068 6f6e 6520  ne (str): Phone 
+0002f830: 6e75 6d62 6572 206f 6620 7468 6520 7669  number of the vi
+0002f840: 7369 746f 723b 2046 6f72 6d61 7420 5b2b  sitor; Format [+
+0002f850: 436f 756e 7472 7943 6f64 655d 5b50 686f  CountryCode][Pho
+0002f860: 6e65 4e75 6d62 6572 5d0a 2020 2020 2020  neNumber].      
+0002f870: 2020 2020 2020 656d 6169 6c20 2873 7472        email (str
+0002f880: 293a 2045 6d61 696c 2061 6464 7265 7373  ): Email address
+0002f890: 206f 6620 7468 6520 7669 7369 746f 720a   of the visitor.
+0002f8a0: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
+0002f8b0: 645f 666f 7265 7665 7220 2862 6f6f 6c29  d_forever (bool)
+0002f8c0: 3a20 5669 7369 746f 7220 6163 636f 756e  : Visitor accoun
+0002f8d0: 7420 7769 6c6c 206e 6f74 2065 7870 6972  t will not expir
+0002f8e0: 6520 7768 656e 2074 6869 7320 6973 2073  e when this is s
+0002f8f0: 6574 2074 6f20 7472 7565 0a20 2020 2020  et to true.     
+0002f900: 2020 2020 2020 2076 616c 6964 5f64 6179         valid_day
+0002f910: 7320 2869 6e74 293a 2041 6363 6f75 6e74  s (int): Account
+0002f920: 2076 616c 6964 6974 7920 696e 2064 6179   validity in day
+0002f930: 730a 2020 2020 2020 2020 2020 2020 7661  s.            va
+0002f940: 6c69 645f 686f 7572 7320 2869 6e74 293a  lid_hours (int):
+0002f950: 2041 6363 6f75 6e74 2076 616c 6964 6974   Account validit
+0002f960: 7920 696e 2068 6f75 7273 0a20 2020 2020  y in hours.     
+0002f970: 2020 2020 2020 2076 616c 6964 5f6d 696e         valid_min
+0002f980: 7574 6573 2028 696e 7429 3a20 4163 636f  utes (int): Acco
+0002f990: 756e 7420 7661 6c69 6469 7479 2069 6e20  unt validity in 
+0002f9a0: 6d69 6e75 7465 730a 2020 2020 2020 2020  minutes.        
+0002f9b0: 2020 2020 6e6f 7469 6679 2028 626f 6f6c      notify (bool
+0002f9c0: 293a 2046 6c61 6720 746f 206e 6f74 6966  ): Flag to notif
+0002f9d0: 7920 7468 6520 7061 7373 776f 7264 2076  y the password v
+0002f9e0: 6961 2065 6d61 696c 206f 7220 6e75 6d62  ia email or numb
+0002f9f0: 6572 0a20 2020 2020 2020 2020 2020 206e  er.            n
+0002fa00: 6f74 6966 795f 746f 2028 7374 7229 3a20  otify_to (str): 
+0002fa10: 4e6f 7469 6679 2074 6f20 656d 6169 6c20  Notify to email 
+0002fa20: 6f72 2070 686f 6e65 2e20 4465 6675 616c  or phone. Defual
+0002fa30: 7420 6973 2070 686f 6e65 2077 6865 6e20  t is phone when 
+0002fa40: 6974 2069 7320 7072 6f76 6964 6564 0a20  it is provided. 
+0002fa50: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0002fa60: 7468 6572 7769 7365 2065 6d61 696c 2e20  therwise email. 
+0002fa70: 2056 616c 6964 2056 616c 7565 733a 2065   Valid Values: e
+0002fa80: 6d61 696c 2c20 7068 6f6e 650a 2020 2020  mail, phone.    
+0002fa90: 2020 2020 2020 2020 6973 5f65 6e61 626c          is_enabl
+0002faa0: 6564 2028 626f 6f6c 293a 2045 6e61 626c  ed (bool): Enabl
+0002fab0: 6520 6f72 2064 6973 6162 6c65 2074 6865  e or disable the
+0002fac0: 2076 6973 6974 6f72 2061 6363 6f75 6e74   visitor account
+0002fad0: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
+0002fae0: 6420 2873 7472 293a 204e 4120 666f 7220  d (str): NA for 
+0002faf0: 7669 7369 746f 7220 706f 7374 2f70 7574  visitor post/put
+0002fb00: 206d 6574 686f 642e 2049 4420 6f66 2074   method. ID of t
+0002fb10: 6865 2076 6973 6974 6f72 0a20 2020 2020  he visitor.     
+0002fb20: 2020 2020 2020 2023 2073 7461 7475 7320         # status 
+0002fb30: 2862 6f6f 6c29 3a20 5468 6973 2066 6965  (bool): This fie
+0002fb40: 6c64 2070 726f 7669 6465 7320 7374 6174  ld provides stat
+0002fb50: 7573 206f 6620 7468 6520 6163 636f 756e  us of the accoun
+0002fb60: 742e 2052 6574 7572 6e73 2074 7275 6520  t. Returns true 
+0002fb70: 7768 656e 2065 6e61 626c 6564 2061 6e64  when enabled and
+0002fb80: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+0002fb90: 2020 206e 6f74 2065 7870 6972 6564 2e20     not expired. 
+0002fba0: 4e41 2066 6f72 2076 6973 6974 6f72 2070  NA for visitor p
+0002fbb0: 6f73 742f 7075 7420 6d65 7468 6f64 2e20  ost/put method. 
+0002fbc0: 5468 6973 2069 7320 6f70 7469 6f6e 616c  This is optional
+0002fbd0: 2066 6965 6c64 732e 0a20 2020 2020 2020   fields..       
+0002fbe0: 2020 2020 2023 2063 7265 6174 6564 5f61       # created_a
+0002fbf0: 7420 2873 7472 293a 2054 6869 7320 6669  t (str): This fi
+0002fc00: 656c 6420 696e 6469 6361 7465 7320 7468  eld indicates th
+0002fc10: 6520 6372 6561 7465 6420 6461 7465 2074  e created date t
+0002fc20: 696d 6573 7461 6d70 2076 616c 7565 2e20  imestamp value. 
+0002fc30: 4974 2069 7320 6765 6e65 7261 7465 640a  It is generated.
+0002fc40: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+0002fc50: 2020 7768 696c 6520 6372 6561 7469 6e67    while creating
+0002fc60: 2076 6973 6974 6f72 2e20 4e41 2066 6f72   visitor. NA for
+0002fc70: 2076 6973 6974 6f72 2070 6f73 742f 7075   visitor post/pu
+0002fc80: 7420 6d65 7468 6f64 2e20 5468 6973 2069  t method. This i
+0002fc90: 7320 6f70 7469 6f6e 616c 2066 6965 6c64  s optional field
+0002fca0: 2e0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0002fcb0: 6578 7069 7265 5f61 7420 2873 7472 293a  expire_at (str):
+0002fcc0: 2054 6869 7320 6669 656c 6420 696e 6469   This field indi
+0002fcd0: 6361 7465 7320 6578 7069 7279 2074 696d  cates expiry tim
+0002fce0: 6520 7469 6d65 7374 616d 7020 7661 6c75  e timestamp valu
+0002fcf0: 652e 2049 7420 6973 2067 656e 6572 6174  e. It is generat
+0002fd00: 6564 2062 6173 6564 0a20 2020 2020 2020  ed based.       
+0002fd10: 2020 2020 2023 2020 2020 206f 6e20 7468       #     on th
+0002fd20: 6520 7661 6c69 645f 7469 6c6c 2076 616c  e valid_till val
+0002fd30: 7565 2061 6e64 2063 7265 6174 6564 5f61  ue and created_a
+0002fd40: 7420 7469 6d65 2e20 4e41 2066 6f72 2076  t time. NA for v
+0002fd50: 6973 6974 6f72 2070 6f73 742f 7075 7420  isitor post/put 
+0002fd60: 6d65 7468 6f64 2e20 5468 6973 2069 730a  method. This is.
+0002fd70: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+0002fd80: 2020 6f70 7469 6f6e 616c 2066 6965 6c64    optional field
+0002fd90: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0002fda0: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
+0002fdb0: 6573 706f 6e73 653a 2043 656e 7472 616c  esponse: Central
+0002fdc0: 4150 4920 5265 7370 6f6e 7365 206f 626a  API Response obj
+0002fdd0: 6563 740a 2020 2020 2020 2020 2222 220a  ect.        """.
+0002fde0: 2020 2020 2020 2020 7572 6c20 3d20 6622          url = f"
+0002fdf0: 2f67 7565 7374 2f76 312f 706f 7274 616c  /guest/v1/portal
+0002fe00: 732f 7b70 6f72 7461 6c5f 6964 7d2f 7669  s/{portal_id}/vi
+0002fe10: 7369 746f 7273 220a 0a20 2020 2020 2020  sitors"..       
+0002fe20: 2075 7365 725f 6461 7461 203d 207b 0a20   user_data = {. 
+0002fe30: 2020 2020 2020 2020 2020 2027 7068 6f6e             'phon
+0002fe40: 6527 3a20 7068 6f6e 652c 0a20 2020 2020  e': phone,.     
+0002fe50: 2020 2020 2020 2027 656d 6169 6c27 3a20         'email': 
+0002fe60: 656d 6169 6c0a 2020 2020 2020 2020 7d0a  email.        }.
+0002fe70: 2020 2020 2020 2020 2320 4150 4920 7265          # API re
+0002fe80: 7175 6972 6573 2070 686f 6e65 2061 6e64  quires phone and
+0002fe90: 2065 6d61 696c 2c20 6275 7420 616c 6c6f   email, but allo
+0002fea0: 7773 204e 6f6e 652f 6e75 6c6c 2061 7320  ws None/null as 
+0002feb0: 7661 6c75 6520 6465 7065 6e64 696e 6720  value depending 
+0002fec0: 6f6e 2068 6f77 2070 6f72 7461 6c20 6973  on how portal is
+0002fed0: 2063 6f6e 6669 6775 7265 640a 2020 2020   configured.    
+0002fee0: 2020 2020 2320 7573 6572 5f64 6174 6120      # user_data 
+0002fef0: 3d20 7574 696c 732e 7374 7269 705f 6e6f  = utils.strip_no
+0002ff00: 6e65 2875 7365 725f 6461 7461 290a 0a20  ne(user_data).. 
+0002ff10: 2020 2020 2020 206a 736f 6e5f 6461 7461         json_data
+0002ff20: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+0002ff30: 2027 6e61 6d65 273a 206e 616d 652c 0a20   'name': name,. 
+0002ff40: 2020 2020 2020 2020 2020 2027 636f 6d70             'comp
+0002ff50: 616e 795f 6e61 6d65 273a 2063 6f6d 7061  any_name': compa
+0002ff60: 6e79 5f6e 616d 652c 0a20 2020 2020 2020  ny_name,.       
+0002ff70: 2020 2020 2027 6973 5f65 6e61 626c 6564       'is_enabled
+0002ff80: 273a 2069 735f 656e 6162 6c65 642c 0a20  ': is_enabled,. 
+0002ff90: 2020 2020 2020 2020 2020 2027 7661 6c69             'vali
+0002ffa0: 645f 7469 6c6c 5f6e 6f5f 6c69 6d69 7427  d_till_no_limit'
+0002ffb0: 3a20 7661 6c69 645f 666f 7265 7665 722c  : valid_forever,
+0002ffc0: 0a20 2020 2020 2020 2020 2020 2027 7661  .            'va
+0002ffd0: 6c69 645f 7469 6c6c 5f64 6179 7327 3a20  lid_till_days': 
+0002ffe0: 7661 6c69 645f 6461 7973 2c0a 2020 2020  valid_days,.    
+0002fff0: 2020 2020 2020 2020 2776 616c 6964 5f74          'valid_t
+00030000: 696c 6c5f 686f 7572 7327 3a20 7661 6c69  ill_hours': vali
+00030010: 645f 686f 7572 732c 0a20 2020 2020 2020  d_hours,.       
+00030020: 2020 2020 2027 7661 6c69 645f 7469 6c6c       'valid_till
+00030030: 5f6d 696e 7574 6573 273a 2076 616c 6964  _minutes': valid
+00030040: 5f6d 696e 7574 6573 2c0a 2020 2020 2020  _minutes,.      
+00030050: 2020 2020 2020 276e 6f74 6966 7927 3a20        'notify': 
+00030060: 6e6f 7469 6679 2c0a 2020 2020 2020 2020  notify,.        
+00030070: 2020 2020 276e 6f74 6966 795f 746f 273a      'notify_to':
+00030080: 206e 6f74 6966 795f 746f 2c0a 2020 2020   notify_to,.    
+00030090: 2020 2020 2020 2020 2770 6173 7377 6f72          'passwor
+000300a0: 6427 3a20 7061 7373 776f 7264 0a20 2020  d': password.   
+000300b0: 2020 2020 207d 0a20 2020 2020 2020 206a       }.        j
+000300c0: 736f 6e5f 6461 7461 203d 2075 7469 6c73  son_data = utils
+000300d0: 2e73 7472 6970 5f6e 6f6e 6528 6a73 6f6e  .strip_none(json
+000300e0: 5f64 6174 6129 0a20 2020 2020 2020 2069  _data).        i
+000300f0: 6620 7573 6572 5f64 6174 613a 0a20 2020  f user_data:.   
+00030100: 2020 2020 2020 2020 206a 736f 6e5f 6461           json_da
+00030110: 7461 5b22 7573 6572 225d 203d 2075 7365  ta["user"] = use
+00030120: 725f 6461 7461 0a0a 2020 2020 2020 2020  r_data..        
+00030130: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+00030140: 662e 706f 7374 2875 726c 2c20 6a73 6f6e  f.post(url, json
+00030150: 5f64 6174 613d 6a73 6f6e 5f64 6174 6129  _data=json_data)
+00030160: 0a0a 2020 2020 2320 544f 444f 2076 616c  ..    # TODO val
+00030170: 6964 6174 6520 4950 2061 6464 7265 7373  idate IP address
+00030180: 2066 6f72 6d61 740a 2020 2020 6173 796e   format.    asyn
+00030190: 6320 6465 6620 7570 6461 7465 5f63 785f  c def update_cx_
+000301a0: 7072 6f70 6572 7469 6573 280a 2020 2020  properties(.    
+000301b0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000301c0: 2020 2a2c 0a20 2020 2020 2020 2073 6572    *,.        ser
+000301d0: 6961 6c3a 2073 7472 203d 204e 6f6e 652c  ial: str = None,
+000301e0: 0a20 2020 2020 2020 2067 726f 7570 3a20  .        group: 
+000301f0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00030200: 2020 2020 6e61 6d65 3a20 7374 7220 3d20      name: str = 
+00030210: 4e6f 6e65 2c0a 2020 2020 2020 2020 636f  None,.        co
+00030220: 6e74 6163 743a 2073 7472 203d 204e 6f6e  ntact: str = Non
+00030230: 652c 0a20 2020 2020 2020 206c 6f63 6174  e,.        locat
+00030240: 696f 6e3a 2073 7472 203d 204e 6f6e 652c  ion: str = None,
+00030250: 0a20 2020 2020 2020 2074 696d 657a 6f6e  .        timezon
+00030260: 653a 2063 6f6e 7374 616e 7473 2e54 5a44  e: constants.TZD
+00030270: 4220 3d20 4e6f 6e65 2c0a 2020 2020 2020  B = None,.      
+00030280: 2020 6d67 6d74 5f76 7266 3a20 626f 6f6c    mgmt_vrf: bool
+00030290: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000302a0: 2064 6e73 5f73 6572 7665 7273 3a20 4c69   dns_servers: Li
+000302b0: 7374 5b73 7472 5d20 3d20 5b5d 2c0a 2020  st[str] = [],.  
+000302c0: 2020 2020 2020 6e74 705f 7365 7276 6572        ntp_server
+000302d0: 733a 204c 6973 745b 7374 725d 203d 205b  s: List[str] = [
+000302e0: 5d2c 0a20 2020 2020 2020 2061 646d 696e  ],.        admin
+000302f0: 5f75 7365 723a 2073 7472 203d 204e 6f6e  _user: str = Non
+00030300: 652c 0a20 2020 2020 2020 2061 646d 696e  e,.        admin
+00030310: 5f70 6173 733a 2073 7472 203d 204e 6f6e  _pass: str = Non
+00030320: 652c 0a20 2020 2029 202d 3e20 5265 7370  e,.    ) -> Resp
+00030330: 6f6e 7365 3a0a 2020 2020 2020 2020 2222  onse:.        ""
+00030340: 2255 7064 6174 6520 5072 6f70 6572 7469  "Update Properti
+00030350: 6573 2028 4172 7562 614f 532d 4358 292e  es (ArubaOS-CX).
+00030360: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00030370: 2020 2020 2020 2020 2020 2020 7365 7269              seri
+00030380: 616c 2028 7374 722c 206f 7074 696f 6e61  al (str, optiona
+00030390: 6c29 3a20 4465 7669 6365 2073 6572 6961  l): Device seria
+000303a0: 6c20 6e75 6d62 6572 2e0a 2020 2020 2020  l number..      
+000303b0: 2020 2020 2020 2020 2020 4d61 6e64 6174            Mandat
+000303c0: 6f72 7920 666f 7220 6465 7669 6365 206c  ory for device l
+000303d0: 6576 656c 2063 6f6e 6669 6775 7261 7469  evel configurati
+000303e0: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+000303f0: 2020 2020 3120 616e 6420 6f6e 6c79 2031      1 and only 1
+00030400: 206f 6620 7365 7269 616c 206f 7220 6772   of serial or gr
+00030410: 6f75 7020 6172 6520 7265 7175 6972 6564  oup are required
+00030420: 0a20 2020 2020 2020 2020 2020 2067 726f  .            gro
+00030430: 7570 2028 7374 722c 206f 7074 696f 6e61  up (str, optiona
+00030440: 6c29 3a20 4772 6f75 7020 6e61 6d65 2e0a  l): Group name..
+00030450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030460: 4d61 6e64 6174 6f72 7920 666f 7220 6772  Mandatory for gr
+00030470: 6f75 7020 6c65 7665 6c20 636f 6e66 6967  oup level config
+00030480: 7572 6174 696f 6e2e 0a20 2020 2020 2020  uration..       
+00030490: 2020 2020 2020 2020 2031 2061 6e64 206f           1 and o
+000304a0: 6e6c 7920 3120 6f66 2073 6572 6961 6c20  nly 1 of serial 
+000304b0: 6f72 2067 726f 7570 2061 7265 2072 6571  or group are req
+000304c0: 7569 7265 640a 2020 2020 2020 2020 2020  uired.          
+000304d0: 2020 6e61 6d65 2028 7374 7229 3a20 4f6e    name (str): On
+000304e0: 6c79 2063 6f6e 6669 6775 7261 626c 6520  ly configurable 
+000304f0: 6174 2064 6576 6963 652d 6c65 7665 6c2e  at device-level.
+00030500: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00030510: 7461 6374 2028 7374 7229 3a20 5061 7474  tact (str): Patt
+00030520: 6572 6e3a 2022 5e5b 5e22 3f5d 2a24 220a  ern: "^[^"?]*$".
+00030530: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
+00030540: 7469 6f6e 2028 7374 7229 3a20 5061 7474  tion (str): Patt
+00030550: 6572 6e3a 2022 5e5b 5e22 3f5d 2a24 220a  ern: "^[^"?]*$".
+00030560: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+00030570: 7a6f 6e65 2028 7374 7229 3a20 7469 6d65  zone (str): time
+00030580: 7a6f 6e65 2020 5661 6c69 6420 5661 6c75  zone  Valid Valu
+00030590: 6573 3a20 7573 6520 747a 2064 6174 6162  es: use tz datab
+000305a0: 6173 6520 666f 726d 6174 206c 696b 6520  ase format like 
+000305b0: 2241 6d65 7269 6361 2f43 6869 6361 676f  "America/Chicago
+000305c0: 220a 2020 2020 2020 2020 2020 2020 6d67  ".            mg
+000305d0: 6d74 5f76 7266 2028 626f 6f6c 293a 2055  mt_vrf (bool): U
+000305e0: 7365 206d 676d 7420 5652 462c 2069 6e64  se mgmt VRF, ind
+000305f0: 6963 6174 6573 2056 5246 2066 6f72 2064  icates VRF for d
+00030600: 6e73 5f73 6572 7665 7273 2061 6e64 206e  ns_servers and n
+00030610: 7470 5f73 6572 7665 7273 2c20 6966 2046  tp_servers, if F
+00030620: 616c 7365 206f 7220 6e6f 7420 7072 6f76  alse or not prov
+00030630: 6964 6564 2064 6566 6175 6c74 2056 5246  ided default VRF
+00030640: 2069 7320 7573 6564 2e0a 2020 2020 2020   is used..      
+00030650: 2020 2020 2020 646e 735f 7365 7276 6572        dns_server
+00030660: 7320 284c 6973 745b 7374 725d 293a 2069  s (List[str]): i
+00030670: 7076 342f 6970 7636 2061 6464 7265 7373  pv4/ipv6 address
+00030680: 0a20 2020 2020 2020 2020 2020 206e 7470  .            ntp
+00030690: 5f73 6572 7665 7273 2028 4c69 7374 5b73  _servers (List[s
+000306a0: 7472 5d29 3a20 6970 7634 2f69 7076 3620  tr]): ipv4/ipv6 
+000306b0: 6164 6472 6573 730a 2020 2020 2020 2020  address.        
+000306c0: 2020 2020 6164 6d69 6e5f 7573 6572 2028      admin_user (
+000306d0: 7374 7229 3a20 6c6f 6361 6c20 6164 6d69  str): local admi
+000306e0: 6e20 7573 6572 0a20 2020 2020 2020 2020  n user.         
+000306f0: 2020 2061 646d 696e 5f70 6173 7320 2873     admin_pass (s
+00030700: 7472 293a 206c 6f63 616c 2061 646d 696e  tr): local admin
+00030710: 2070 6173 7377 6f72 640a 0a20 2020 2020   password..     
+00030720: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00030730: 2020 2020 2020 2020 5265 7370 6f6e 7365          Response
+00030740: 3a20 4365 6e74 7261 6c41 5049 2052 6573  : CentralAPI Res
+00030750: 706f 6e73 6520 6f62 6a65 6374 0a20 2020  ponse object.   
+00030760: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00030770: 2075 726c 203d 2022 2f63 6f6e 6669 6775   url = "/configu
+00030780: 7261 7469 6f6e 2f76 312f 7377 6974 6368  ration/v1/switch
+00030790: 2f63 782f 7072 6f70 6572 7469 6573 220a  /cx/properties".
+000307a0: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
+000307b0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+000307c0: 2764 6576 6963 655f 7365 7269 616c 273a  'device_serial':
+000307d0: 2073 6572 6961 6c2c 0a20 2020 2020 2020   serial,.       
+000307e0: 2020 2020 2027 6772 6f75 705f 6e61 6d65       'group_name
+000307f0: 273a 2067 726f 7570 0a20 2020 2020 2020  ': group.       
+00030800: 207d 0a0a 2020 2020 2020 2020 6a73 6f6e   }..        json
+00030810: 5f64 6174 6120 3d20 7b0a 2020 2020 2020  _data = {.      
+00030820: 2020 2020 2020 276e 616d 6527 3a20 6e61        'name': na
+00030830: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00030840: 2763 6f6e 7461 6374 273a 2063 6f6e 7461  'contact': conta
+00030850: 6374 2c0a 2020 2020 2020 2020 2020 2020  ct,.            
+00030860: 276c 6f63 6174 696f 6e27 3a20 6c6f 6361  'location': loca
+00030870: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+00030880: 2020 2774 696d 657a 6f6e 6527 3a20 7469    'timezone': ti
+00030890: 6d65 7a6f 6e65 2c0a 2020 2020 2020 2020  mezone,.        
+000308a0: 2020 2020 2764 6e73 5f73 6572 7665 7273      'dns_servers
+000308b0: 273a 2064 6e73 5f73 6572 7665 7273 2c0a  ': dns_servers,.
+000308c0: 2020 2020 2020 2020 2020 2020 276e 7470              'ntp
+000308d0: 5f73 6572 7665 7273 273a 206e 7470 5f73  _servers': ntp_s
+000308e0: 6572 7665 7273 2c0a 2020 2020 2020 2020  ervers,.        
+000308f0: 2020 2020 2761 646d 696e 5f75 7365 726e      'admin_usern
+00030900: 616d 6527 3a20 6164 6d69 6e5f 7573 6572  ame': admin_user
+00030910: 2c0a 2020 2020 2020 2020 2020 2020 2761  ,.            'a
+00030920: 646d 696e 5f70 6173 7377 6f72 6427 3a20  dmin_password': 
+00030930: 6164 6d69 6e5f 7061 7373 0a20 2020 2020  admin_pass.     
+00030940: 2020 207d 0a20 2020 2020 2020 2069 6620     }.        if 
+00030950: 6d67 6d74 5f76 7266 2069 7320 6e6f 7420  mgmt_vrf is not 
+00030960: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00030970: 2020 6a73 6f6e 5f64 6174 615b 2276 7266    json_data["vrf
+00030980: 225d 203d 2022 6d67 6d74 2220 6966 206d  "] = "mgmt" if m
+00030990: 676d 745f 7672 6620 656c 7365 2022 6465  gmt_vrf else "de
+000309a0: 6661 756c 7422 0a20 2020 2020 2020 2065  fault".        e
+000309b0: 6c69 6620 646e 735f 7365 7276 6572 7320  lif dns_servers 
+000309c0: 6f72 206e 7470 5f73 6572 7665 7273 3a0a  or ntp_servers:.
+000309d0: 2020 2020 2020 2020 2020 2020 6a73 6f6e              json
+000309e0: 5f64 6174 615b 2276 7266 225d 203d 2022  _data["vrf"] = "
+000309f0: 6465 6661 756c 7422 0a0a 2020 2020 2020  default"..      
+00030a00: 2020 6966 206c 656e 285b 7820 666f 7220    if len([x for 
+00030a10: 7820 696e 205b 6164 6d69 6e5f 7573 6572  x in [admin_user
+00030a20: 2c20 6164 6d69 6e5f 7061 7373 5d20 6966  , admin_pass] if
+00030a30: 2078 2069 7320 6e6f 7420 4e6f 6e65 5d29   x is not None])
+00030a40: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
+00030a50: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00030a60: 726f 7228 2249 6620 6569 7468 6572 2061  ror("If either a
+00030a70: 646d 696e 5f75 7365 7220 6f72 2061 646d  dmin_user or adm
+00030a80: 696e 5f70 6173 7320 6172 6520 6269 6e67  in_pass are bing
+00030a90: 2075 7064 6174 6564 2c20 2a62 6f74 682a   updated, *both*
+00030aa0: 2073 686f 756c 6420 6265 2070 726f 7669   should be provi
+00030ab0: 6465 642e 2229 0a0a 2020 2020 2020 2020  ded.")..        
+00030ac0: 6966 206c 656e 285b 7820 666f 7220 7820  if len([x for x 
+00030ad0: 696e 205b 7365 7269 616c 2c20 6772 6f75  in [serial, grou
+00030ae0: 705d 2069 6620 7820 6973 206e 6f74 204e  p] if x is not N
+00030af0: 6f6e 655d 2920 3d3d 2032 3a0a 2020 2020  one]) == 2:.    
+00030b00: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00030b10: 6c75 6545 7272 6f72 2822 7072 6f76 6964  lueError("provid
+00030b20: 6520 7365 7269 616c 2074 6f20 7570 6461  e serial to upda
+00030b30: 7465 2064 6576 6963 6520 6c65 7665 6c20  te device level 
+00030b40: 7072 6f70 6572 7469 6573 2c20 6f72 2067  properties, or g
+00030b50: 726f 7570 2074 6f20 7570 6461 7465 2061  roup to update a
+00030b60: 7420 7468 6520 6772 6f75 7020 6c65 7665  t the group leve
+00030b70: 6c2e 2020 5072 6f76 6964 696e 6720 626f  l.  Providing bo
+00030b80: 7468 2069 7320 696e 7661 6c69 642e 2229  th is invalid.")
+00030b90: 0a0a 2020 2020 2020 2020 6a73 6f6e 5f64  ..        json_d
+00030ba0: 6174 6120 3d20 7574 696c 732e 7374 7269  ata = utils.stri
+00030bb0: 705f 6e6f 6e65 286a 736f 6e5f 6461 7461  p_none(json_data
+00030bc0: 2c20 7374 7269 705f 656d 7074 795f 6f62  , strip_empty_ob
+00030bd0: 6a3d 5472 7565 290a 0a20 2020 2020 2020  j=True)..       
+00030be0: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
+00030bf0: 6c66 2e70 6f73 7428 7572 6c2c 206a 736f  lf.post(url, jso
+00030c00: 6e5f 6461 7461 3d6a 736f 6e5f 6461 7461  n_data=json_data
+00030c10: 2c20 7061 7261 6d73 3d70 6172 616d 7329  , params=params)
+00030c20: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00030c30: 6765 745f 6f73 7066 5f61 7265 6128 0a20  get_ospf_area(. 
+00030c40: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00030c50: 2020 2020 2064 6576 6963 653a 2073 7472       device: str
+00030c60: 2c0a 2020 2020 2020 2020 6d61 726b 6572  ,.        marker
+00030c70: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00030c80: 2020 2020 2020 6c69 6d69 743a 2069 6e74        limit: int
+00030c90: 203d 2031 3030 2c0a 2020 2020 2920 2d3e   = 100,.    ) ->
+00030ca0: 2052 6573 706f 6e73 653a 0a20 2020 2020   Response:.     
+00030cb0: 2020 2022 2222 4c69 7374 204f 5350 4620     """List OSPF 
+00030cc0: 4172 6561 2049 6e66 6f72 6d61 7469 6f6e  Area Information
+00030cd0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00030ce0: 0a20 2020 2020 2020 2020 2020 2064 6576  .            dev
+00030cf0: 6963 6520 2873 7472 293a 2044 6576 6963  ice (str): Devic
+00030d00: 6520 7365 7269 616c 206e 756d 6265 720a  e serial number.
+00030d10: 2020 2020 2020 2020 2020 2020 6d61 726b              mark
+00030d20: 6572 2028 7374 722c 206f 7074 696f 6e61  er (str, optiona
+00030d30: 6c29 3a20 4f70 6171 7565 2068 616e 646c  l): Opaque handl
+00030d40: 6520 746f 2066 6574 6368 206e 6578 7420  e to fetch next 
+00030d50: 7061 6765 0a20 2020 2020 2020 2020 2020  page.           
+00030d60: 206c 696d 6974 2028 696e 742c 206f 7074   limit (int, opt
+00030d70: 696f 6e61 6c29 3a20 7061 6765 2073 697a  ional): page siz
+00030d80: 6520 4465 6661 756c 7473 2074 6f20 3130  e Defaults to 10
+00030d90: 302e 0a0a 2020 2020 2020 2020 5265 7475  0...        Retu
+00030da0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00030db0: 2052 6573 706f 6e73 653a 2043 656e 7472   Response: Centr
+00030dc0: 616c 4150 4920 5265 7370 6f6e 7365 206f  alAPI Response o
+00030dd0: 626a 6563 740a 2020 2020 2020 2020 2222  bject.        ""
+00030de0: 220a 2020 2020 2020 2020 7572 6c20 3d20  ".        url = 
+00030df0: 222f 6170 692f 726f 7574 696e 672f 7631  "/api/routing/v1
+00030e00: 2f6f 7370 662f 6172 6561 220a 0a20 2020  /ospf/area"..   
+00030e10: 2020 2020 2070 6172 616d 7320 3d20 7b0a       params = {.
+00030e20: 2020 2020 2020 2020 2020 2020 2764 6576              'dev
+00030e30: 6963 6527 3a20 6465 7669 6365 2c0a 2020  ice': device,.  
+00030e40: 2020 2020 2020 2020 2020 276d 6172 6b65            'marke
+00030e50: 7227 3a20 6d61 726b 6572 2c0a 2020 2020  r': marker,.    
+00030e60: 2020 2020 2020 2020 276c 696d 6974 273a          'limit':
+00030e70: 206c 696d 6974 0a20 2020 2020 2020 207d   limit.        }
+00030e80: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00030e90: 2061 7761 6974 2073 656c 662e 6765 7428   await self.get(
+00030ea0: 7572 6c2c 2070 6172 616d 733d 7061 7261  url, params=para
+00030eb0: 6d73 290a 0a20 2020 2061 7379 6e63 2064  ms)..    async d
+00030ec0: 6566 2067 6574 5f6f 7370 665f 696e 7465  ef get_ospf_inte
+00030ed0: 7266 6163 6528 0a20 2020 2020 2020 2073  rface(.        s
+00030ee0: 656c 662c 0a20 2020 2020 2020 2064 6576  elf,.        dev
+00030ef0: 6963 653a 2073 7472 2c0a 2020 2020 2020  ice: str,.      
+00030f00: 2020 6d61 726b 6572 3a20 7374 7220 3d20    marker: str = 
+00030f10: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c69  None,.        li
+00030f20: 6d69 743a 2069 6e74 203d 2031 3030 2c0a  mit: int = 100,.
+00030f30: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
+00030f40: 653a 0a20 2020 2020 2020 2022 2222 4c69  e:.        """Li
+00030f50: 7374 204f 5350 4620 496e 7465 7266 6163  st OSPF Interfac
+00030f60: 6520 496e 666f 726d 6174 696f 6e2e 0a0a  e Information...
+00030f70: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00030f80: 2020 2020 2020 2020 2020 6465 7669 6365            device
+00030f90: 2028 7374 7229 3a20 4465 7669 6365 2073   (str): Device s
+00030fa0: 6572 6961 6c20 6e75 6d62 6572 0a20 2020  erial number.   
+00030fb0: 2020 2020 2020 2020 206d 6172 6b65 7220           marker 
+00030fc0: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+00030fd0: 204f 7061 7175 6520 6861 6e64 6c65 2074   Opaque handle t
+00030fe0: 6f20 6665 7463 6820 6e65 7874 2070 6167  o fetch next pag
+00030ff0: 650a 2020 2020 2020 2020 2020 2020 6c69  e.            li
+00031000: 6d69 7420 2869 6e74 2c20 6f70 7469 6f6e  mit (int, option
+00031010: 616c 293a 2070 6167 6520 7369 7a65 2044  al): page size D
+00031020: 6566 6175 6c74 7320 746f 2031 3030 2e0a  efaults to 100..
+00031030: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00031040: 3a0a 2020 2020 2020 2020 2020 2020 5265  :.            Re
+00031050: 7370 6f6e 7365 3a20 4365 6e74 7261 6c41  sponse: CentralA
+00031060: 5049 2052 6573 706f 6e73 6520 6f62 6a65  PI Response obje
+00031070: 6374 0a20 2020 2020 2020 2022 2222 0a20  ct.        """. 
+00031080: 2020 2020 2020 2075 726c 203d 2022 2f61         url = "/a
+00031090: 7069 2f72 6f75 7469 6e67 2f76 312f 6f73  pi/routing/v1/os
+000310a0: 7066 2f69 6e74 6572 6661 6365 220a 0a20  pf/interface".. 
+000310b0: 2020 2020 2020 2070 6172 616d 7320 3d20         params = 
+000310c0: 7b0a 2020 2020 2020 2020 2020 2020 2764  {.            'd
+000310d0: 6576 6963 6527 3a20 6465 7669 6365 2c0a  evice': device,.
+000310e0: 2020 2020 2020 2020 2020 2020 276d 6172              'mar
+000310f0: 6b65 7227 3a20 6d61 726b 6572 2c0a 2020  ker': marker,.  
+00031100: 2020 2020 2020 2020 2020 276c 696d 6974            'limit
+00031110: 273a 206c 696d 6974 0a20 2020 2020 2020  ': limit.       
+00031120: 207d 0a0a 2020 2020 2020 2020 7265 7475   }..        retu
+00031130: 726e 2061 7761 6974 2073 656c 662e 6765  rn await self.ge
+00031140: 7428 7572 6c2c 2070 6172 616d 733d 7061  t(url, params=pa
+00031150: 7261 6d73 290a 0a20 2020 2061 7379 6e63  rams)..    async
+00031160: 2064 6566 2067 6574 5f6f 7370 665f 6e65   def get_ospf_ne
+00031170: 6967 6862 6f72 280a 2020 2020 2020 2020  ighbor(.        
+00031180: 7365 6c66 2c0a 2020 2020 2020 2020 6465  self,.        de
+00031190: 7669 6365 3a20 7374 722c 0a20 2020 2020  vice: str,.     
+000311a0: 2020 206d 6172 6b65 723a 2073 7472 203d     marker: str =
+000311b0: 204e 6f6e 652c 0a20 2020 2020 2020 206c   None,.        l
+000311c0: 696d 6974 3a20 696e 7420 3d20 3130 302c  imit: int = 100,
+000311d0: 0a20 2020 2029 202d 3e20 5265 7370 6f6e  .    ) -> Respon
+000311e0: 7365 3a0a 2020 2020 2020 2020 2222 224c  se:.        """L
+000311f0: 6973 7420 4f53 5046 206e 6569 6768 626f  ist OSPF neighbo
+00031200: 7220 496e 666f 726d 6174 696f 6e2e 0a0a  r Information...
+00031210: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00031220: 2020 2020 2020 2020 2020 6465 7669 6365            device
+00031230: 2028 7374 7229 3a20 4465 7669 6365 2073   (str): Device s
+00031240: 6572 6961 6c20 6e75 6d62 6572 0a20 2020  erial number.   
+00031250: 2020 2020 2020 2020 206d 6172 6b65 7220           marker 
+00031260: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+00031270: 204f 7061 7175 6520 6861 6e64 6c65 2074   Opaque handle t
+00031280: 6f20 6665 7463 6820 6e65 7874 2070 6167  o fetch next pag
+00031290: 650a 2020 2020 2020 2020 2020 2020 6c69  e.            li
+000312a0: 6d69 7420 2869 6e74 2c20 6f70 7469 6f6e  mit (int, option
+000312b0: 616c 293a 2070 6167 6520 7369 7a65 2044  al): page size D
+000312c0: 6566 6175 6c74 7320 746f 2031 3030 2e0a  efaults to 100..
+000312d0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+000312e0: 3a0a 2020 2020 2020 2020 2020 2020 5265  :.            Re
+000312f0: 7370 6f6e 7365 3a20 4365 6e74 7261 6c41  sponse: CentralA
+00031300: 5049 2052 6573 706f 6e73 6520 6f62 6a65  PI Response obje
+00031310: 6374 0a20 2020 2020 2020 2022 2222 0a20  ct.        """. 
+00031320: 2020 2020 2020 2075 726c 203d 2022 2f61         url = "/a
+00031330: 7069 2f72 6f75 7469 6e67 2f76 312f 6f73  pi/routing/v1/os
+00031340: 7066 2f6e 6569 6768 626f 7222 0a0a 2020  pf/neighbor"..  
+00031350: 2020 2020 2020 7061 7261 6d73 203d 207b        params = {
+00031360: 0a20 2020 2020 2020 2020 2020 2027 6465  .            'de
+00031370: 7669 6365 273a 2064 6576 6963 652c 0a20  vice': device,. 
+00031380: 2020 2020 2020 2020 2020 2027 6d61 726b             'mark
+00031390: 6572 273a 206d 6172 6b65 722c 0a20 2020  er': marker,.   
+000313a0: 2020 2020 2020 2020 2027 6c69 6d69 7427           'limit'
+000313b0: 3a20 6c69 6d69 740a 2020 2020 2020 2020  : limit.        
+000313c0: 7d0a 0a20 2020 2020 2020 2072 6574 7572  }..        retur
+000313d0: 6e20 6177 6169 7420 7365 6c66 2e67 6574  n await self.get
+000313e0: 2875 726c 2c20 7061 7261 6d73 3d70 6172  (url, params=par
+000313f0: 616d 7329 0a0a 2020 2020 6173 796e 6320  ams)..    async 
+00031400: 6465 6620 6765 745f 6f73 7066 5f64 6174  def get_ospf_dat
+00031410: 6162 6173 6528 0a20 2020 2020 2020 2073  abase(.        s
+00031420: 656c 662c 0a20 2020 2020 2020 2064 6576  elf,.        dev
+00031430: 6963 653a 2073 7472 2c0a 2020 2020 2020  ice: str,.      
+00031440: 2020 6d61 726b 6572 3a20 7374 7220 3d20    marker: str = 
+00031450: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c69  None,.        li
+00031460: 6d69 743a 2069 6e74 203d 2031 3030 2c0a  mit: int = 100,.
+00031470: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
+00031480: 653a 0a20 2020 2020 2020 2022 2222 4c69  e:.        """Li
+00031490: 7374 204f 5350 4620 4c69 6e6b 2053 7461  st OSPF Link Sta
+000314a0: 7465 2044 6174 6162 6173 6520 496e 666f  te Database Info
+000314b0: 726d 6174 696f 6e2e 0a0a 2020 2020 2020  rmation...      
+000314c0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000314d0: 2020 2020 6465 7669 6365 2028 7374 7229      device (str)
+000314e0: 3a20 4465 7669 6365 2073 6572 6961 6c20  : Device serial 
+000314f0: 6e75 6d62 6572 0a20 2020 2020 2020 2020  number.         
+00031500: 2020 206d 6172 6b65 7220 2873 7472 2c20     marker (str, 
+00031510: 6f70 7469 6f6e 616c 293a 204f 7061 7175  optional): Opaqu
+00031520: 6520 6861 6e64 6c65 2074 6f20 6665 7463  e handle to fetc
+00031530: 6820 6e65 7874 2070 6167 650a 2020 2020  h next page.    
+00031540: 2020 2020 2020 2020 6c69 6d69 7420 2869          limit (i
+00031550: 6e74 2c20 6f70 7469 6f6e 616c 293a 2070  nt, optional): p
+00031560: 6167 6520 7369 7a65 2044 6566 6175 6c74  age size Default
+00031570: 7320 746f 2031 3030 2e0a 0a20 2020 2020  s to 100...     
+00031580: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00031590: 2020 2020 2020 2020 5265 7370 6f6e 7365          Response
+000315a0: 3a20 4365 6e74 7261 6c41 5049 2052 6573  : CentralAPI Res
+000315b0: 706f 6e73 6520 6f62 6a65 6374 0a20 2020  ponse object.   
+000315c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000315d0: 2075 726c 203d 2022 2f61 7069 2f72 6f75   url = "/api/rou
+000315e0: 7469 6e67 2f76 312f 6f73 7066 2f64 6174  ting/v1/ospf/dat
+000315f0: 6162 6173 6522 0a0a 2020 2020 2020 2020  abase"..        
+00031600: 7061 7261 6d73 203d 207b 0a20 2020 2020  params = {.     
+00031610: 2020 2020 2020 2027 6465 7669 6365 273a         'device':
+00031620: 2064 6576 6963 652c 0a20 2020 2020 2020   device,.       
+00031630: 2020 2020 2027 6d61 726b 6572 273a 206d       'marker': m
+00031640: 6172 6b65 722c 0a20 2020 2020 2020 2020  arker,.         
+00031650: 2020 2027 6c69 6d69 7427 3a20 6c69 6d69     'limit': limi
+00031660: 740a 2020 2020 2020 2020 7d0a 0a20 2020  t.        }..   
+00031670: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
+00031680: 7420 7365 6c66 2e67 6574 2875 726c 2c20  t self.get(url, 
+00031690: 7061 7261 6d73 3d70 6172 616d 7329 0a0a  params=params)..
+000316a0: 2020 2020 6173 796e 6320 6465 6620 6765      async def ge
+000316b0: 745f 6f76 6572 6c61 795f 636f 6e6e 6563  t_overlay_connec
+000316c0: 7469 6f6e 280a 2020 2020 2020 2020 7365  tion(.        se
+000316d0: 6c66 2c0a 2020 2020 2020 2020 6465 7669  lf,.        devi
+000316e0: 6365 3a20 7374 722c 0a20 2020 2020 2020  ce: str,.       
+000316f0: 206d 6172 6b65 723a 2073 7472 203d 204e   marker: str = N
+00031700: 6f6e 652c 0a20 2020 2020 2020 206c 696d  one,.        lim
+00031710: 6974 3a20 696e 7420 3d20 3130 302c 0a20  it: int = 100,. 
+00031720: 2020 2029 202d 3e20 5265 7370 6f6e 7365     ) -> Response
+00031730: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
+00031740: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
+00031750: 7574 206f 7665 726c 6179 2063 6f6e 7472  ut overlay contr
+00031760: 6f6c 2063 6f6e 6e65 6374 696f 6e2e 0a0a  ol connection...
+00031770: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00031780: 2020 2020 2020 2020 2020 6465 7669 6365            device
+00031790: 2028 7374 7229 3a20 4465 7669 6365 2073   (str): Device s
+000317a0: 6572 6961 6c20 6e75 6d62 6572 0a20 2020  erial number.   
+000317b0: 2020 2020 2020 2020 206d 6172 6b65 7220           marker 
+000317c0: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+000317d0: 204f 7061 7175 6520 6861 6e64 6c65 2074   Opaque handle t
+000317e0: 6f20 6665 7463 6820 6e65 7874 2070 6167  o fetch next pag
+000317f0: 650a 2020 2020 2020 2020 2020 2020 6c69  e.            li
+00031800: 6d69 7420 2869 6e74 2c20 6f70 7469 6f6e  mit (int, option
+00031810: 616c 293a 2070 6167 6520 7369 7a65 2044  al): page size D
+00031820: 6566 6175 6c74 7320 746f 2031 3030 2e0a  efaults to 100..
+00031830: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00031840: 3a0a 2020 2020 2020 2020 2020 2020 5265  :.            Re
+00031850: 7370 6f6e 7365 3a20 4365 6e74 7261 6c41  sponse: CentralA
+00031860: 5049 2052 6573 706f 6e73 6520 6f62 6a65  PI Response obje
+00031870: 6374 0a20 2020 2020 2020 2022 2222 0a20  ct.        """. 
+00031880: 2020 2020 2020 2075 726c 203d 2022 2f61         url = "/a
+00031890: 7069 2f72 6f75 7469 6e67 2f76 312f 6f76  pi/routing/v1/ov
+000318a0: 6572 6c61 792f 636f 6e6e 6563 7469 6f6e  erlay/connection
+000318b0: 220a 0a20 2020 2020 2020 2070 6172 616d  "..        param
+000318c0: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
+000318d0: 2020 2764 6576 6963 6527 3a20 6465 7669    'device': devi
+000318e0: 6365 2c0a 2020 2020 2020 2020 2020 2020  ce,.            
+000318f0: 276d 6172 6b65 7227 3a20 6d61 726b 6572  'marker': marker
+00031900: 2c0a 2020 2020 2020 2020 2020 2020 276c  ,.            'l
+00031910: 696d 6974 273a 206c 696d 6974 0a20 2020  imit': limit.   
+00031920: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00031930: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+00031940: 662e 6765 7428 7572 6c2c 2070 6172 616d  f.get(url, param
+00031950: 733d 7061 7261 6d73 290a 0a20 2020 2061  s=params)..    a
+00031960: 7379 6e63 2064 6566 2072 6573 6574 5f6f  sync def reset_o
+00031970: 7665 726c 6179 5f63 6f6e 6e65 6374 696f  verlay_connectio
+00031980: 6e28 0a20 2020 2020 2020 2073 656c 662c  n(.        self,
+00031990: 0a20 2020 2020 2020 2064 6576 6963 653a  .        device:
+000319a0: 2073 7472 2c0a 2020 2020 2920 2d3e 2052   str,.    ) -> R
+000319b0: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
+000319c0: 2022 2222 5265 7365 7420 6f76 6572 6c61   """Reset overla
+000319d0: 7920 636f 6e74 726f 6c20 636f 6e6e 6563  y control connec
+000319e0: 7469 6f6e 2e0a 0a20 2020 2020 2020 2041  tion...        A
+000319f0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00031a00: 2064 6576 6963 6520 2873 7472 293a 2044   device (str): D
+00031a10: 6576 6963 6520 7365 7269 616c 206e 756d  evice serial num
+00031a20: 6265 720a 0a20 2020 2020 2020 2052 6574  ber..        Ret
+00031a30: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00031a40: 2020 5265 7370 6f6e 7365 3a20 4365 6e74    Response: Cent
+00031a50: 7261 6c41 5049 2052 6573 706f 6e73 6520  ralAPI Response 
+00031a60: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
+00031a70: 2222 0a20 2020 2020 2020 2075 726c 203d  "".        url =
+00031a80: 2022 2f61 7069 2f72 6f75 7469 6e67 2f76   "/api/routing/v
+00031a90: 312f 6f76 6572 6c61 792f 636f 6e6e 6563  1/overlay/connec
+00031aa0: 7469 6f6e 2f72 6573 6574 220a 0a20 2020  tion/reset"..   
+00031ab0: 2020 2020 2070 6172 616d 7320 3d20 7b0a       params = {.
+00031ac0: 2020 2020 2020 2020 2020 2020 2764 6576              'dev
+00031ad0: 6963 6527 3a20 6465 7669 6365 0a20 2020  ice': device.   
+00031ae0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00031af0: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+00031b00: 662e 7075 7428 7572 6c2c 2070 6172 616d  f.put(url, param
+00031b10: 733d 7061 7261 6d73 290a 0a20 2020 2061  s=params)..    a
+00031b20: 7379 6e63 2064 6566 2067 6574 5f6f 7665  sync def get_ove
+00031b30: 726c 6179 5f72 6f75 7465 735f 6c65 6172  rlay_routes_lear
+00031b40: 6e65 6428 0a20 2020 2020 2020 2073 656c  ned(.        sel
+00031b50: 662c 0a20 2020 2020 2020 2064 6576 6963  f,.        devic
+00031b60: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+00031b70: 2a2c 0a20 2020 2020 2020 2062 6573 743a  *,.        best:
+00031b80: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+00031b90: 2020 2020 2020 206d 6172 6b65 723a 2073         marker: s
+00031ba0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+00031bb0: 2020 206c 696d 6974 3a20 696e 7420 3d20     limit: int = 
+00031bc0: 3130 302c 0a20 2020 2029 202d 3e20 5265  100,.    ) -> Re
+00031bd0: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
+00031be0: 2222 224c 6973 7420 6f66 206c 6561 726e  """List of learn
+00031bf0: 6564 2072 6f75 7465 7320 6672 6f6d 206f  ed routes from o
+00031c00: 7665 726c 6179 2e0a 0a20 2020 2020 2020  verlay...       
+00031c10: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00031c20: 2020 2064 6576 6963 6520 2873 7472 293a     device (str):
+00031c30: 2044 6576 6963 6520 7365 7269 616c 206e   Device serial n
+00031c40: 756d 6265 720a 2020 2020 2020 2020 2020  umber.          
+00031c50: 2020 6265 7374 2028 626f 6f6c 293a 2052    best (bool): R
+00031c60: 6574 7572 6e20 6f6e 6c79 2062 6573 7420  eturn only best 
+00031c70: 2f20 7072 6566 6572 7265 6420 726f 7574  / preferred rout
+00031c80: 6573 0a20 2020 2020 2020 2020 2020 206d  es.            m
+00031c90: 6172 6b65 7220 2873 7472 2c20 6f70 7469  arker (str, opti
+00031ca0: 6f6e 616c 293a 204f 7061 7175 6520 6861  onal): Opaque ha
+00031cb0: 6e64 6c65 2074 6f20 6665 7463 6820 6e65  ndle to fetch ne
+00031cc0: 7874 2070 6167 650a 2020 2020 2020 2020  xt page.        
+00031cd0: 2020 2020 6c69 6d69 7420 2869 6e74 2c20      limit (int, 
+00031ce0: 6f70 7469 6f6e 616c 293a 2070 6167 6520  optional): page 
+00031cf0: 7369 7a65 2044 6566 6175 6c74 7320 746f  size Defaults to
+00031d00: 2031 3030 2e0a 0a20 2020 2020 2020 2052   100...        R
+00031d10: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00031d20: 2020 2020 5265 7370 6f6e 7365 3a20 4365      Response: Ce
+00031d30: 6e74 7261 6c41 5049 2052 6573 706f 6e73  ntralAPI Respons
+00031d40: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
+00031d50: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
+00031d60: 203d 2022 2f61 7069 2f72 6f75 7469 6e67   = "/api/routing
+00031d70: 2f76 312f 6f76 6572 6c61 792f 726f 7574  /v1/overlay/rout
+00031d80: 652f 6c65 6172 6e65 6422 0a20 2020 2020  e/learned".     
+00031d90: 2020 2069 6620 6265 7374 3a0a 2020 2020     if best:.    
+00031da0: 2020 2020 2020 2020 7572 6c20 3d20 6627          url = f'
+00031db0: 7b75 726c 7d2f 6265 7374 270a 0a20 2020  {url}/best'..   
+00031dc0: 2020 2020 2070 6172 616d 7320 3d20 7b0a       params = {.
+00031dd0: 2020 2020 2020 2020 2020 2020 2764 6576              'dev
+00031de0: 6963 6527 3a20 6465 7669 6365 2c0a 2020  ice': device,.  
+00031df0: 2020 2020 2020 2020 2020 276d 6172 6b65            'marke
+00031e00: 7227 3a20 6d61 726b 6572 2c0a 2020 2020  r': marker,.    
+00031e10: 2020 2020 2020 2020 276c 696d 6974 273a          'limit':
+00031e20: 206c 696d 6974 0a20 2020 2020 2020 207d   limit.        }
+00031e30: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00031e40: 2061 7761 6974 2073 656c 662e 6765 7428   await self.get(
+00031e50: 7572 6c2c 2070 6172 616d 733d 7061 7261  url, params=para
+00031e60: 6d73 290a 0a20 2020 2061 7379 6e63 2064  ms)..    async d
+00031e70: 6566 2067 6574 5f6f 7665 726c 6179 5f72  ef get_overlay_r
+00031e80: 6f75 7465 735f 6164 7665 7274 6973 6564  outes_advertised
+00031e90: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00031ea0: 2020 2020 2020 2020 6465 7669 6365 3a20          device: 
+00031eb0: 7374 722c 0a20 2020 2020 2020 206d 6172  str,.        mar
+00031ec0: 6b65 723a 2073 7472 203d 204e 6f6e 652c  ker: str = None,
+00031ed0: 0a20 2020 2020 2020 206c 696d 6974 3a20  .        limit: 
+00031ee0: 696e 7420 3d20 3130 302c 0a20 2020 2029  int = 100,.    )
+00031ef0: 202d 3e20 5265 7370 6f6e 7365 3a0a 2020   -> Response:.  
+00031f00: 2020 2020 2020 2222 224c 6973 7420 6f66        """List of
+00031f10: 2061 6476 6572 7469 7365 6420 726f 7574   advertised rout
+00031f20: 6573 2074 6f20 6f76 6572 6c61 792e 0a0a  es to overlay...
+00031f30: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00031f40: 2020 2020 2020 2020 2020 6465 7669 6365            device
+00031f50: 2028 7374 7229 3a20 4465 7669 6365 2073   (str): Device s
+00031f60: 6572 6961 6c20 6e75 6d62 6572 0a20 2020  erial number.   
+00031f70: 2020 2020 2020 2020 206d 6172 6b65 7220           marker 
+00031f80: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+00031f90: 204f 7061 7175 6520 6861 6e64 6c65 2074   Opaque handle t
+00031fa0: 6f20 6665 7463 6820 6e65 7874 2070 6167  o fetch next pag
+00031fb0: 650a 2020 2020 2020 2020 2020 2020 6c69  e.            li
+00031fc0: 6d69 7420 2869 6e74 2c20 6f70 7469 6f6e  mit (int, option
+00031fd0: 616c 293a 2070 6167 6520 7369 7a65 2044  al): page size D
+00031fe0: 6566 6175 6c74 7320 746f 2031 3030 2e0a  efaults to 100..
+00031ff0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00032000: 3a0a 2020 2020 2020 2020 2020 2020 5265  :.            Re
+00032010: 7370 6f6e 7365 3a20 4365 6e74 7261 6c41  sponse: CentralA
+00032020: 5049 2052 6573 706f 6e73 6520 6f62 6a65  PI Response obje
+00032030: 6374 0a20 2020 2020 2020 2022 2222 0a20  ct.        """. 
+00032040: 2020 2020 2020 2075 726c 203d 2022 2f61         url = "/a
+00032050: 7069 2f72 6f75 7469 6e67 2f76 312f 6f76  pi/routing/v1/ov
+00032060: 6572 6c61 792f 726f 7574 652f 6164 7665  erlay/route/adve
+00032070: 7274 6973 6564 220a 0a20 2020 2020 2020  rtised"..       
+00032080: 2070 6172 616d 7320 3d20 7b0a 2020 2020   params = {.    
+00032090: 2020 2020 2020 2020 2764 6576 6963 6527          'device'
+000320a0: 3a20 6465 7669 6365 2c0a 2020 2020 2020  : device,.      
+000320b0: 2020 2020 2020 276d 6172 6b65 7227 3a20        'marker': 
+000320c0: 6d61 726b 6572 2c0a 2020 2020 2020 2020  marker,.        
+000320d0: 2020 2020 276c 696d 6974 273a 206c 696d      'limit': lim
+000320e0: 6974 0a20 2020 2020 2020 207d 0a0a 2020  it.        }..  
+000320f0: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+00032100: 6974 2073 656c 662e 6765 7428 7572 6c2c  it self.get(url,
+00032110: 2070 6172 616d 733d 7061 7261 6d73 290a   params=params).
+00032120: 0a20 2020 2061 7379 6e63 2064 6566 2067  .    async def g
+00032130: 6574 5f6f 7665 726c 6179 5f69 6e74 6572  et_overlay_inter
+00032140: 6661 6365 7328 0a20 2020 2020 2020 2073  faces(.        s
+00032150: 656c 662c 0a20 2020 2020 2020 2064 6576  elf,.        dev
+00032160: 6963 653a 2073 7472 2c0a 2020 2020 2020  ice: str,.      
+00032170: 2020 6d61 726b 6572 3a20 7374 7220 3d20    marker: str = 
+00032180: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c69  None,.        li
+00032190: 6d69 743a 2069 6e74 203d 2031 3030 2c0a  mit: int = 100,.
+000321a0: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
+000321b0: 653a 0a20 2020 2020 2020 2022 2222 4c69  e:.        """Li
+000321c0: 7374 206f 6620 6f76 6572 6c61 7920 696e  st of overlay in
+000321d0: 7465 7266 6163 6573 2028 7475 6e6e 656c  terfaces (tunnel
+000321e0: 7329 2e0a 0a20 2020 2020 2020 2041 7267  s)...        Arg
+000321f0: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
+00032200: 6576 6963 6520 2873 7472 293a 2044 6576  evice (str): Dev
+00032210: 6963 6520 7365 7269 616c 206e 756d 6265  ice serial numbe
+00032220: 720a 2020 2020 2020 2020 2020 2020 6d61  r.            ma
+00032230: 726b 6572 2028 7374 722c 206f 7074 696f  rker (str, optio
+00032240: 6e61 6c29 3a20 4f70 6171 7565 2068 616e  nal): Opaque han
+00032250: 646c 6520 746f 2066 6574 6368 206e 6578  dle to fetch nex
+00032260: 7420 7061 6765 0a20 2020 2020 2020 2020  t page.         
+00032270: 2020 206c 696d 6974 2028 696e 742c 206f     limit (int, o
+00032280: 7074 696f 6e61 6c29 3a20 7061 6765 2073  ptional): page s
+00032290: 697a 6520 4465 6661 756c 7473 2074 6f20  ize Defaults to 
+000322a0: 3130 302e 0a0a 2020 2020 2020 2020 5265  100...        Re
+000322b0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+000322c0: 2020 2052 6573 706f 6e73 653a 2043 656e     Response: Cen
+000322d0: 7472 616c 4150 4920 5265 7370 6f6e 7365  tralAPI Response
+000322e0: 206f 626a 6563 740a 2020 2020 2020 2020   object.        
+000322f0: 2222 220a 2020 2020 2020 2020 7572 6c20  """.        url 
+00032300: 3d20 222f 6170 692f 726f 7574 696e 672f  = "/api/routing/
+00032310: 7631 2f6f 7665 726c 6179 2f69 6e74 6572  v1/overlay/inter
+00032320: 6661 6365 220a 0a20 2020 2020 2020 2070  face"..        p
+00032330: 6172 616d 7320 3d20 7b0a 2020 2020 2020  arams = {.      
+00032340: 2020 2020 2020 2764 6576 6963 6527 3a20        'device': 
+00032350: 6465 7669 6365 2c0a 2020 2020 2020 2020  device,.        
+00032360: 2020 2020 276d 6172 6b65 7227 3a20 6d61      'marker': ma
+00032370: 726b 6572 2c0a 2020 2020 2020 2020 2020  rker,.          
+00032380: 2020 276c 696d 6974 273a 206c 696d 6974    'limit': limit
+00032390: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+000323a0: 2020 2020 7265 7475 726e 2061 7761 6974      return await
+000323b0: 2073 656c 662e 6765 7428 7572 6c2c 2070   self.get(url, p
+000323c0: 6172 616d 733d 7061 7261 6d73 290a 0a20  arams=params).. 
+000323d0: 2020 2061 7379 6e63 2064 6566 2067 6574     async def get
+000323e0: 5f64 656e 796c 6973 745f 636c 6965 6e74  _denylist_client
+000323f0: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
+00032400: 0a20 2020 2020 2020 2073 6572 6961 6c3a  .        serial:
+00032410: 2073 7472 2c0a 2020 2020 2920 2d3e 2052   str,.    ) -> R
+00032420: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
+00032430: 2022 2222 4765 7420 616c 6c20 6465 6e79   """Get all deny
+00032440: 6c69 7374 2063 6c69 656e 7420 6d61 6320  list client mac 
+00032450: 6164 6472 6573 7320 696e 2064 6576 6963  address in devic
+00032460: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
+00032470: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00032480: 7269 616c 2028 7374 7229 3a20 4465 7669  rial (str): Devi
+00032490: 6365 2069 6420 6f66 2076 6972 7475 616c  ce id of virtual
+000324a0: 2063 6f6e 7472 6f6c 6c65 7220 2841 4f53   controller (AOS
+000324b0: 3820 4941 5029 206f 7220 7365 7269 616c  8 IAP) or serial
+000324c0: 206f 6620 414f 5331 3020 6170 2e0a 2020   of AOS10 ap..  
+000324d0: 2020 2020 2020 2020 2020 2020 2020 4578                Ex
+000324e0: 616d 706c 653a 3134 6233 3734 3363 3031  ample:14b3743c01
+000324f0: 6638 3038 3062 6661 3037 6361 3035 3365  f8080bfa07ca053e
+00032500: 6631 6538 3935 6466 3963 3036 3830 6665  f1e895df9c0680fe
+00032510: 3561 3137 6266 6435 0a0a 2020 2020 2020  5a17bfd5..      
+00032520: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00032530: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
+00032540: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
+00032550: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
+00032560: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00032570: 7572 6c20 3d20 6622 2f63 6f6e 6669 6775  url = f"/configu
+00032580: 7261 7469 6f6e 2f76 312f 7377 6172 6d2f  ration/v1/swarm/
+00032590: 7b73 6572 6961 6c7d 2f62 6c61 636b 6c69  {serial}/blackli
+000325a0: 7374 696e 6722 0a0a 2020 2020 2020 2020  sting"..        
+000325b0: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+000325c0: 662e 6765 7428 7572 6c29 0a0a 0a20 2020  f.get(url)...   
+000325d0: 2061 7379 6e63 2064 6566 2067 6574 5f61   async def get_a
+000325e0: 7574 6f5f 7375 6273 6372 6962 6528 0a20  uto_subscribe(. 
+000325f0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00032600: 2029 202d 3e20 5265 7370 6f6e 7365 3a0a   ) -> Response:.
+00032610: 2020 2020 2020 2020 2222 2247 6574 2074          """Get t
+00032620: 6865 2073 6572 7669 6365 7320 7768 6963  he services whic
+00032630: 6820 6861 7665 2061 7574 6f20 7375 6273  h have auto subs
+00032640: 6372 6962 6520 656e 6162 6c65 642e 0a0a  cribe enabled...
+00032650: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00032660: 0a20 2020 2020 2020 2020 2020 2052 6573  .            Res
+00032670: 706f 6e73 653a 2043 656e 7472 616c 4150  ponse: CentralAP
+00032680: 4920 5265 7370 6f6e 7365 206f 626a 6563  I Response objec
+00032690: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
+000326a0: 2020 2020 2020 7572 6c20 3d20 222f 706c        url = "/pl
+000326b0: 6174 666f 726d 2f6c 6963 656e 7369 6e67  atform/licensing
+000326c0: 2f76 312f 6375 7374 6f6d 6572 2f73 6574  /v1/customer/set
+000326d0: 7469 6e67 732f 6175 746f 6c69 6365 6e73  tings/autolicens
+000326e0: 6522 0a0a 2020 2020 2020 2020 7265 7475  e"..        retu
+000326f0: 726e 2061 7761 6974 2073 656c 662e 6765  rn await self.ge
+00032700: 7428 7572 6c29 0a0a 2020 2020 6173 796e  t(url)..    asyn
+00032710: 6320 6465 6620 656e 6162 6c65 5f61 7574  c def enable_aut
+00032720: 6f5f 7375 6273 6372 6962 6528 0a20 2020  o_subscribe(.   
+00032730: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00032740: 2020 2073 6572 7669 6365 733a 204c 6973     services: Lis
+00032750: 745b 7374 725d 207c 2073 7472 2c0a 2020  t[str] | str,.  
+00032760: 2020 2920 2d3e 2052 6573 706f 6e73 653a    ) -> Response:
+00032770: 0a20 2020 2020 2020 2022 2222 5374 616e  .        """Stan
+00032780: 6461 6c6f 6e65 2043 7573 746f 6d65 7220  dalone Customer 
+00032790: 4150 493a 2041 7373 6967 6e20 6c69 6365  API: Assign lice
+000327a0: 6e73 6573 2074 6f20 616c 6c20 6465 7669  nses to all devi
+000327b0: 6365 7320 616e 6420 656e 6162 6c65 2061  ces and enable a
+000327c0: 7574 6f20 7375 6273 6372 6962 6520 666f  uto subscribe fo
+000327d0: 720a 2020 2020 2020 2020 6769 7665 6e20  r.        given 
+000327e0: 7365 7276 6963 6573 2e0a 0a20 2020 2020  services...     
+000327f0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00032800: 2020 2020 2073 6572 7669 6365 7320 284c       services (L
+00032810: 6973 745b 7374 725d 293a 206c 6973 7420  ist[str]): list 
+00032820: 6f66 2073 6572 7669 6365 7320 652e 672e  of services e.g.
+00032830: 205b 2770 6127 2c20 2775 6363 272c 2066   ['pa', 'ucc', f
+00032840: 6f75 6e64 6174 696f 6e5f 6170 2c0a 2020  oundation_ap,.  
+00032850: 2020 2020 2020 2020 2020 2020 2020 6164                ad
+00032860: 7661 6e63 6564 5f73 7769 7463 685f 3632  vanced_switch_62
+00032870: 3030 2c20 666f 756e 6461 7469 6f6e 5f37  00, foundation_7
+00032880: 3058 5820 6574 6320 2e2e 2e5d 2e20 4368  0XX etc ...]. Ch
+00032890: 6563 6b0a 2020 2020 2020 2020 2020 2020  eck.            
+000328a0: 2020 2020 2f70 6c61 7466 6f72 6d2f 6c69      /platform/li
+000328b0: 6365 6e73 696e 672f 7631 2f73 6572 7669  censing/v1/servi
+000328c0: 6365 732f 636f 6e66 6967 2041 5049 2072  ces/config API r
+000328d0: 6573 706f 6e73 6520 746f 206b 6e6f 7720  esponse to know 
+000328e0: 7468 6520 6c69 7374 206f 6620 7375 7070  the list of supp
+000328f0: 6f72 7465 640a 2020 2020 2020 2020 2020  orted.          
+00032900: 2020 2020 2020 7365 7276 6963 6573 2e0a        services..
+00032910: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00032920: 3a0a 2020 2020 2020 2020 2020 2020 5265  :.            Re
+00032930: 7370 6f6e 7365 3a20 4365 6e74 7261 6c41  sponse: CentralA
+00032940: 5049 2052 6573 706f 6e73 6520 6f62 6a65  PI Response obje
+00032950: 6374 0a20 2020 2020 2020 2022 2222 0a20  ct.        """. 
+00032960: 2020 2020 2020 2075 726c 203d 2022 2f70         url = "/p
+00032970: 6c61 7466 6f72 6d2f 6c69 6365 6e73 696e  latform/licensin
+00032980: 672f 7631 2f63 7573 746f 6d65 722f 7365  g/v1/customer/se
+00032990: 7474 696e 6773 2f61 7574 6f6c 6963 656e  ttings/autolicen
+000329a0: 7365 220a 0a20 2020 2020 2020 2069 6620  se"..        if 
+000329b0: 6973 696e 7374 616e 6365 2873 6572 7669  isinstance(servi
+000329c0: 6365 732c 2073 7472 293a 0a20 2020 2020  ces, str):.     
+000329d0: 2020 2020 2020 2073 6572 7669 6365 7320         services 
+000329e0: 3d20 5b73 6572 7669 6365 735d 0a0a 2020  = [services]..  
+000329f0: 2020 2020 2020 6a73 6f6e 5f64 6174 6120        json_data 
+00032a00: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00032a10: 2773 6572 7669 6365 7327 3a20 7365 7276  'services': serv
+00032a20: 6963 6573 0a20 2020 2020 2020 207d 0a0a  ices.        }..
+00032a30: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00032a40: 7761 6974 2073 656c 662e 706f 7374 2875  wait self.post(u
+00032a50: 726c 2c20 6a73 6f6e 5f64 6174 613d 6a73  rl, json_data=js
+00032a60: 6f6e 5f64 6174 6129 0a0a 2020 2020 6173  on_data)..    as
+00032a70: 796e 6320 6465 6620 6469 7361 626c 655f  ync def disable_
+00032a80: 6175 746f 5f73 7562 7363 7269 6265 280a  auto_subscribe(.
+00032a90: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00032aa0: 2020 2020 2020 7365 7276 6963 6573 3a20        services: 
+00032ab0: 4c69 7374 5b73 7472 5d20 7c20 7374 722c  List[str] | str,
+00032ac0: 0a20 2020 2029 202d 3e20 5265 7370 6f6e  .    ) -> Respon
+00032ad0: 7365 3a0a 2020 2020 2020 2020 2222 2253  se:.        """S
+00032ae0: 7461 6e64 616c 6f6e 6520 4375 7374 6f6d  tandalone Custom
+00032af0: 6572 2041 5049 3a20 4469 7361 626c 6520  er API: Disable 
+00032b00: 6175 746f 206c 6963 656e 7369 6e67 2066  auto licensing f
+00032b10: 6f72 2067 6976 656e 2073 6572 7669 6365  or given service
+00032b20: 732e 0a0a 2020 2020 2020 2020 4172 6773  s...        Args
+00032b30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00032b40: 7276 6963 6573 2028 4c69 7374 5b73 7472  rvices (List[str
+00032b50: 5d29 3a20 6c69 7374 206f 6620 7365 7276  ]): list of serv
+00032b60: 6963 6573 2065 2e67 2e20 5b27 7061 272c  ices e.g. ['pa',
+00032b70: 2027 7563 6327 2c20 666f 756e 6461 7469   'ucc', foundati
+00032b80: 6f6e 5f61 702c 0a20 2020 2020 2020 2020  on_ap,.         
+00032b90: 2020 2020 2020 2061 6476 616e 6365 645f         advanced_
+00032ba0: 7377 6974 6368 5f36 3230 302c 2066 6f75  switch_6200, fou
+00032bb0: 6e64 6174 696f 6e5f 3730 5858 2065 7463  ndation_70XX etc
+00032bc0: 202e 2e2e 5d2e 2043 6865 636b 0a20 2020   ...]. Check.   
+00032bd0: 2020 2020 2020 2020 2020 2020 202f 706c               /pl
+00032be0: 6174 666f 726d 2f6c 6963 656e 7369 6e67  atform/licensing
+00032bf0: 2f76 312f 7365 7276 6963 6573 2f63 6f6e  /v1/services/con
+00032c00: 6669 6720 4150 4920 7265 7370 6f6e 7365  fig API response
+00032c10: 2074 6f20 6b6e 6f77 2074 6865 206c 6973   to know the lis
+00032c20: 7420 6f66 2073 7570 706f 7274 6564 0a20  t of supported. 
+00032c30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00032c40: 6572 7669 6365 732e 0a0a 2020 2020 2020  ervices...      
+00032c50: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00032c60: 2020 2020 2020 2052 6573 706f 6e73 653a         Response:
+00032c70: 2043 656e 7472 616c 4150 4920 5265 7370   CentralAPI Resp
+00032c80: 6f6e 7365 206f 626a 6563 740a 2020 2020  onse object.    
+00032c90: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00032ca0: 7572 6c20 3d20 222f 706c 6174 666f 726d  url = "/platform
+00032cb0: 2f6c 6963 656e 7369 6e67 2f76 312f 6375  /licensing/v1/cu
+00032cc0: 7374 6f6d 6572 2f73 6574 7469 6e67 732f  stomer/settings/
+00032cd0: 6175 746f 6c69 6365 6e73 6522 0a0a 2020  autolicense"..  
+00032ce0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00032cf0: 6e63 6528 7365 7276 6963 6573 2c20 7374  nce(services, st
+00032d00: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00032d10: 7365 7276 6963 6573 203d 205b 7365 7276  services = [serv
+00032d20: 6963 6573 5d0a 0a20 2020 2020 2020 206a  ices]..        j
+00032d30: 736f 6e5f 6461 7461 203d 207b 0a20 2020  son_data = {.   
+00032d40: 2020 2020 2020 2020 2027 7365 7276 6963           'servic
+00032d50: 6573 273a 2073 6572 7669 6365 730a 2020  es': services.  
+00032d60: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00032d70: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
+00032d80: 6c66 2e64 656c 6574 6528 7572 6c2c 206a  lf.delete(url, j
+00032d90: 736f 6e5f 6461 7461 3d6a 736f 6e5f 6461  son_data=json_da
+00032da0: 7461 290a 0a20 2020 2023 202f 2f20 2d2d  ta)..    # // --
+00032db0: 204e 6f74 2075 7365 6420 6279 2063 6f6d   Not used by com
+00032dc0: 6d61 6e64 7320 7965 742e 2020 756e 646f  mands yet.  undo
+00032dd0: 6375 6d65 6e74 6564 206b 6d73 2061 7069  cumented kms api
+00032de0: 202d 2d20 2f2f 0a20 2020 2061 7379 6e63   -- //.    async
+00032df0: 2064 6566 206b 6d73 5f67 6574 5f73 796e   def kms_get_syn
+00032e00: 6365 645f 6170 7328 7365 6c66 2c20 6d61  ced_aps(self, ma
+00032e10: 633a 2073 7472 2920 2d3e 2052 6573 706f  c: str) -> Respo
+00032e20: 6e73 653a 0a20 2020 2020 2020 2075 726c  nse:.        url
+00032e30: 203d 2066 222f 6b65 796d 676d 742f 7631   = f"/keymgmt/v1
+00032e40: 2f73 796e 6365 6461 706c 6973 742f 7b6d  /syncedaplist/{m
+00032e50: 6163 7d22 0a20 2020 2020 2020 2072 6574  ac}".        ret
+00032e60: 7572 6e20 6177 6169 7420 7365 6c66 2e67  urn await self.g
+00032e70: 6574 2875 726c 290a 0a20 2020 2061 7379  et(url)..    asy
+00032e80: 6e63 2064 6566 206b 6d73 5f67 6574 5f63  nc def kms_get_c
+00032e90: 6c69 656e 745f 7265 636f 7264 2873 656c  lient_record(sel
+00032ea0: 662c 206d 6163 3a20 7374 7229 202d 3e20  f, mac: str) -> 
+00032eb0: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
+00032ec0: 2020 7572 6c20 3d20 6622 2f6b 6579 6d67    url = f"/keymg
+00032ed0: 6d74 2f76 312f 6b65 7963 6163 6865 2f7b  mt/v1/keycache/{
+00032ee0: 6d61 637d 220a 2020 2020 2020 2020 7265  mac}".        re
+00032ef0: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+00032f00: 6765 7428 7572 6c29 0a0a 2020 2020 6173  get(url)..    as
+00032f10: 796e 6320 6465 6620 6b6d 735f 6765 745f  ync def kms_get_
+00032f20: 6861 7368 2873 656c 6629 202d 3e20 5265  hash(self) -> Re
+00032f30: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
+00032f40: 7572 6c20 3d20 222f 6b65 796d 676d 742f  url = "/keymgmt/
+00032f50: 7631 2f6b 6579 6861 7368 220a 2020 2020  v1/keyhash".    
+00032f60: 2020 2020 7265 7475 726e 2061 7761 6974      return await
+00032f70: 2073 656c 662e 6765 7428 7572 6c29 0a0a   self.get(url)..
+00032f80: 2020 2020 6173 796e 6320 6465 6620 6b6d      async def km
+00032f90: 735f 6765 745f 6170 5f73 7461 7465 2873  s_get_ap_state(s
+00032fa0: 656c 662c 2073 6572 6961 6c3a 2073 7472  elf, serial: str
+00032fb0: 2920 2d3e 2052 6573 706f 6e73 653a 0a20  ) -> Response:. 
+00032fc0: 2020 2020 2020 2075 726c 203d 2066 222f         url = f"/
+00032fd0: 6b65 796d 676d 742f 7631 2f53 7461 7473  keymgmt/v1/Stats
+00032fe0: 2f61 702f 7b73 6572 6961 6c7d 220a 2020  /ap/{serial}".  
+00032ff0: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+00033000: 6974 2073 656c 662e 6765 7428 7572 6c29  it self.get(url)
+00033010: 0a0a 2020 2020 2320 4261 6420 656e 6470  ..    # Bad endp
+00033020: 6f69 6e74 2055 524c 2034 3034 0a20 2020  oint URL 404.   
+00033030: 2061 7379 6e63 2064 6566 206b 6d73 5f67   async def kms_g
+00033040: 6574 5f68 6561 6c74 6828 7365 6c66 2920  et_health(self) 
+00033050: 2d3e 2052 6573 706f 6e73 653a 0a20 2020  -> Response:.   
+00033060: 2020 2020 2075 726c 203d 2022 2f6b 6579       url = "/key
+00033070: 6d67 6d74 2f76 312f 6865 616c 7468 220a  mgmt/v1/health".
+00033080: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00033090: 7761 6974 2073 656c 662e 6765 7428 7572  wait self.get(ur
+000330a0: 6c29 0a0a 6966 205f 5f6e 616d 655f 5f20  l)..if __name__ 
+000330b0: 3d3d 2022 5f5f 6d61 696e 5f5f 223a 0a20  == "__main__":. 
+000330c0: 2020 2070 6173 730a                         pass.
```

### Comparing `centralcli-2.4.0/centralcli/cleaner.py` & `centralcli-3.0.0/centralcli/cleaner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1029,15 +1029,15 @@
             "lease_end_ts",
             "lease_time",
             "lease_time_left",
             # "infra_type",
             "client_type",
         ]
 
-    data = [dict(short_value(k, d.get(k)) for k in field_order if k in d) for d in data]
+    data = [{"client name": None, **dict(short_value(k, d.get(k)) for k in field_order if k in d)} for d in data]
     data = strip_no_value(data)
     return data
 
 def get_template_details_for_device(data: str) -> dict:
     """Convert form-data response to dict
 
     Args:
```

### Comparing `centralcli-2.4.0/centralcli/cli.py` & `centralcli-3.0.0/centralcli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,25 +19,25 @@
     hook_enabled = False
 
 import typer
 
 # Detect if called from pypi installed package or via cloned github repo (development)
 try:
     from centralcli import (Response, cleaner, cli, cliadd, cliassign,
-                            clibatch, clicaas, cliclone, clidel, clikick,
+                            clibatch, clicaas, cliclone, clidel, clikick, cliset,
                             clirefresh, clirename, clishow, clitest, clitshoot,
                             cliunassign, cliupdate, cliupgrade, config, log,
                             models, utils)
 except (ImportError, ModuleNotFoundError) as e:
     pkg_dir = Path(__file__).absolute().parent
     if pkg_dir.name == "centralcli":
         sys.path.insert(0, str(pkg_dir.parent))
         from centralcli import (Response, cleaner, cli, cliadd, cliassign,
                                 clibatch, clicaas, cliclone, clidel, clikick,
-                                clirefresh, clirename, clishow, clitest,
+                                cliset, clirefresh, clirename, clishow, clitest,
                                 clitshoot, cliunassign, cliupdate, cliupgrade,
                                 config, log, models, utils)
     else:
         print(pkg_dir.parts)
         raise e
 
 from centralcli.cache import CentralObject
@@ -63,14 +63,15 @@
 app.add_typer(clibatch.app, name="batch",)
 app.add_typer(clicaas.app, name="caas", hidden=True,)
 app.add_typer(clirefresh.app, name="refresh",)
 app.add_typer(clitest.app, name="test",)
 app.add_typer(clitshoot.app, name="tshoot",)
 app.add_typer(clirename.app, name="rename",)
 app.add_typer(clikick.app, name="kick",)
+app.add_typer(cliset.app, name="set",)
 
 
 @app.command(
     help="Move device(s) to a defined group and/or site.",
 )
 def move(
     device: List[str, ] = typer.Argument(None, metavar=iden.dev_many, autocompletion=cli.cache.dev_kwarg_completion),
```

### Comparing `centralcli-2.4.0/centralcli/cliadd.py` & `centralcli-3.0.0/centralcli/cliadd.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/cliassign.py` & `centralcli-3.0.0/centralcli/cliassign.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/clibatch.py` & `centralcli-3.0.0/centralcli/clibatch.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/clicaas.py` & `centralcli-3.0.0/centralcli/clicaas.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/cliclone.py` & `centralcli-3.0.0/centralcli/cliclone.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/clicommon.py` & `centralcli-3.0.0/centralcli/clicommon.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/clidel.py` & `centralcli-3.0.0/centralcli/clidel.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,31 +10,32 @@
 import asyncio
 from rich import print
 from rich.console import Console
 from rich.progress import track
 
 # Detect if called from pypi installed package or via cloned github repo (development)
 try:
-    from centralcli import cli, log, config, utils, Response, BatchRequest
+    from centralcli import cli, log, config, utils, Response, BatchRequest, clidelfirmware
 except (ImportError, ModuleNotFoundError) as e:
     pkg_dir = Path(__file__).absolute().parent
     if pkg_dir.name == "centralcli":
         sys.path.insert(0, str(pkg_dir.parent))
-        from centralcli import cli, log, config, utils, Response, BatchRequest
+        from centralcli import cli, log, config, utils, Response, BatchRequest, clidelfirmware
     else:
         print(pkg_dir.parts)
         raise e
 
 from centralcli.constants import IdenMetaVars
 from centralcli.cache import CentralObject
 from centralcli.exceptions import DevException
 
 iden = IdenMetaVars()
 
 app = typer.Typer()
+app.add_typer(clidelfirmware.app, name="firmware")
 
 
 @app.command(short_help="Delete a certificate")
 def certificate(
     name: str = typer.Argument(..., ),
     yes: bool = typer.Option(False, "-Y", help="Bypass confirmation prompts - Assume Yes"),
     yes_: bool = typer.Option(False, "-y", hidden=True),
@@ -168,77 +169,14 @@
     confirm_2 = typer.style("Delete", fg="bright_red")
     confirm_3 = typer.style(f"Group {group.name}, WLAN {name}", fg="cyan")
     if yes or typer.confirm(f"{confirm_1} {confirm_2} {confirm_3}", abort=True):
         resp = cli.central.request(cli.central.delete_wlan, group.name, name)
         cli.display_results(resp, tablefmt="action")
 
 
-class DelFirmwareArgs(str, Enum):
-    compliance = "compliance"
-
-
-class FirmwareDevType(str, Enum):
-    ap = "ap"
-    gateway = "gateway"
-    switch = "switch"
-
-
-@app.command(short_help="Delete/Clear firmware compliance")
-def firmware(
-    what: DelFirmwareArgs = typer.Argument(...),
-    device_type: FirmwareDevType = typer.Argument(
-        ...,
-        metavar=iden.generic_dev_types,
-        autocompletion=lambda incomplete: [x for x in ["ap", "gw", "switch"] if x.startswith(incomplete.lower())]
-    ),
-    _group: List[str] = typer.Argument(None, metavar="[GROUP-NAME]", autocompletion=cli.cache.group_completion),
-    group_name: str = typer.Option(None, "--group", help="Filter by group", autocompletion=cli.cache.group_completion),
-    yes: bool = typer.Option(False, "-Y", help="Bypass confirmation prompts - Assume Yes"),
-    yes_: bool = typer.Option(False, "-y", hidden=True),
-    debug: bool = typer.Option(False, "--debug", envvar="ARUBACLI_DEBUG", help="Enable Additional Debug Logging",),
-    default: bool = typer.Option(False, "-d", is_flag=True, help="Use default central account", show_default=False,),
-    account: str = typer.Option("central_info",
-                                envvar="ARUBACLI_ACCOUNT",
-                                help="The Aruba Central Account to use (must be defined in the config)",),
-) -> None:
-    _type_to_name = {
-        "ap": "IAP",
-        "gateway": "CONTROLLER",
-        "switch": "HP"
-    }
-    yes = yes_ if yes_ else yes
-
-    if len(_group) > 2:
-        typer.echo(f"Unknown extra arguments in {[x for x in list(_group)[0:-1] if x.lower() != 'group']}")
-        raise typer.Exit(1)
-
-    _group = None if not _group else _group[-1]
-    group = _group or group_name
-    if group:
-        group = cli.cache.get_group_identifier(group).name
-
-    kwargs = {
-        'device_type': _type_to_name.get(device_type.lower(), device_type),
-        'group': group
-    }
-
-    confirm_1 = typer.style("Please Confirm:", fg="cyan")
-    confirm_2 = typer.style("remove", fg="bright_red")
-    confirm_3 = typer.style(f"compliance for {device_type} {'Globally?' if not group else f'in group {group}?'}", fg="cyan")
-    if yes or typer.confirm(f"{confirm_1} {confirm_2} {confirm_3}", abort=True):
-        resp = cli.central.request(cli.central.delete_firmware_compliance, **kwargs)
-        if resp.status == 404 and resp.output.lower() == "not found":
-            resp.output = (
-                f"Invalid URL or No compliance set for {device_type.lower()} "
-                f"{'Globally' if not group else f'in group {group}'}"
-            )
-            typer.echo(str(resp).replace("404", typer.style("404", fg="red")))
-        else:
-            cli.display_results(resp, tablefmt="action")
-
 # TODO cache webhook name/id so they can be deleted by name
 @app.command(help="Delete WebHook")
 def webhook(
     id_: str = typer.Argument(...,),
     yes: bool = typer.Option(False, "-Y", help="Bypass confirmation prompts - Assume Yes"),
     yes_: bool = typer.Option(False, "-y", hidden=True),
     debug: bool = typer.Option(False, "--debug", envvar="ARUBACLI_DEBUG", help="Enable Additional Debug Logging",),
```

### Comparing `centralcli-2.4.0/centralcli/clikick.py` & `centralcli-3.0.0/centralcli/clikick.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/clirefresh.py` & `centralcli-3.0.0/centralcli/clirefresh.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/clirename.py` & `centralcli-3.0.0/centralcli/clirename.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/clishow.py` & `centralcli-3.0.0/centralcli/clishow.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,42 +3,44 @@
 
 from __future__ import annotations
 import typer
 import time
 import pendulum
 import asyncio
 import sys
+import json
 from typing import List, Iterable, Literal
 from pathlib import Path
 from rich import print
 
 try:
     import psutil
     hook_enabled = True
 except (ImportError, ModuleNotFoundError):
     hook_enabled = False
 
 
 # Detect if called from pypi installed package or via cloned github repo (development)
 try:
-    from centralcli import Response, cleaner, clishowfirmware, clishowwids, clishowbranch, clishowospf, clishowtshoot, clishowoverlay, BatchRequest, caas, cli, utils, config
+    from centralcli import Response, cleaner, clishowfirmware, clishowwids, clishowbranch, clishowospf, clishowtshoot, clishowoverlay, BatchRequest, caas, cli, utils, config, log
 except (ImportError, ModuleNotFoundError) as e:
     pkg_dir = Path(__file__).absolute().parent
     if pkg_dir.name == "centralcli":
         sys.path.insert(0, str(pkg_dir.parent))
-        from centralcli import Response, cleaner, clishowfirmware, clishowwids, clishowbranch, clishowospf, clishowtshoot, clishowoverlay, BatchRequest, caas, cli, utils, config
+        from centralcli import Response, cleaner, clishowfirmware, clishowwids, clishowbranch, clishowospf, clishowtshoot, clishowoverlay, BatchRequest, caas, cli, utils, config, log
     else:
         print(pkg_dir.parts)
         raise e
 
 from centralcli.constants import (
     ClientArgs, SortInventoryOptions, ShowInventoryArgs, StatusOptions, SortWlanOptions, IdenMetaVars, CacheArgs, LogAppArgs, LogSortBy, SortSiteOptions,
     DevTypes, SortDevOptions, SortTemplateOptions, SortClientOptions, SortCertOptions, SortVlanOptions, SortSubscriptionOptions, SortRouteOptions, DhcpArgs,
     EventDevTypeArgs, ShowHookProxyArgs, SubscriptionArgs, AlertTypes, SortAlertOptions, AlertSeverity, SortWebHookOptions, TunnelTimeRange, lib_to_api, what_to_pretty  # noqa
 )
+from centralcli.cache import CentralObject
 
 app = typer.Typer()
 app.add_typer(clishowfirmware.app, name="firmware")
 app.add_typer(clishowwids.app, name="wids")
 app.add_typer(clishowbranch.app, name="branch")
 app.add_typer(clishowospf.app, name="ospf")
 app.add_typer(clishowtshoot.app, name="tshoot")
@@ -829,30 +831,31 @@
         outfile=outfile,
         sort_by=sort_by,
         reverse=reverse,
         cleaner=cleaner.get_vlans
     )
 
 
-@app.command(short_help="Show DHCP pool or lease details (gateways only)")
+@app.command()
 def dhcp(
-    what: DhcpArgs = typer.Argument(..., help=["server", "clients"]),
+    what: DhcpArgs = typer.Argument(..., show_default=False,),
     dev: str = typer.Argument(
         ...,
         metavar=f"{iden_meta.dev} (Valid for Gateways Only) ",
         autocompletion=cli.cache.dev_completion,
+        show_default=False,
     ),
     no_res: bool = typer.Option(False, "--no-res", is_flag=True, help="Filter out reservations"),
-    sort_by: str = typer.Option(None, "--sort", help="Field to sort by"),
+    sort_by: str = typer.Option(None, "--sort", help="Field to sort by", show_default=False),
     reverse: bool = typer.Option(False, "-r", help="Reverse sort order", show_default=False,),
     do_json: bool = typer.Option(False, "--json", is_flag=True, help="Output in JSON", show_default=False),
     do_yaml: bool = typer.Option(False, "--yaml", is_flag=True, help="Output in YAML", show_default=False),
     do_csv: bool = typer.Option(False, "--csv", is_flag=True, help="Output in CSV", show_default=False),
     do_table: bool = typer.Option(False, "--table", help="Output in table format", show_default=False),
-    outfile: Path = typer.Option(None, "--out", help="Output to file (and terminal)", writable=True),
+    outfile: Path = typer.Option(None, "--out", help="Output to file (and terminal)", show_default=False, writable=True),
     pager: bool = typer.Option(False, "--pager", help="Enable Paged Output"),
     update_cache: bool = typer.Option(False, "-U", hidden=True),  # Force Update of cli.cache for testing
     default: bool = typer.Option(False, "-d", is_flag=True, help="Use default central account", show_default=False,),
     debug: bool = typer.Option(False, "--debug", envvar="ARUBACLI_DEBUG", help="Enable Additional Debug Logging",),
     account: str = typer.Option(
         "central_info",
         envvar="ARUBACLI_ACCOUNT",
@@ -862,19 +865,19 @@
     verbose2: bool = typer.Option(
         False,
         "-vv",
         help="Show raw response (no formatting) (vertically)",
         show_default=False,
     ),
 ) -> None:
+    """"Show DHCP pool or lease details (gateways only)"
+    """
     central = cli.central
-    dev = cli.cache.get_dev_identifier(dev, dev_type="gw")
+    dev: CentralObject = cli.cache.get_dev_identifier(dev, dev_type="gw")
 
-    # if dev.generic_type != "gw":
-    #     typer.secho(f"show dhcp ... only valid for gateways not {dev.generic_type}", fg="red")
     if what == "server":
         resp = central.request(central.get_dhcp_server, dev.serial)
     else:
         resp = central.request(central.get_dhcp_clients, dev.serial, reservation=not no_res)
 
     tablefmt = cli.get_format(do_json=do_json, do_yaml=do_yaml, do_csv=do_csv, do_table=do_table, default="rich")
 
@@ -908,23 +911,25 @@
     account: str = typer.Option(
         "central_info",
         envvar="ARUBACLI_ACCOUNT",
         help="The Aruba Central Account to use (must be defined in the config)",
         autocompletion=cli.cache.account_completion,
     ),
 ):
-    # TODO The API method only accepts swarm id for IAP which AOS10 does not have / serial rejected
     central = cli.central
     if len(device) > 2:
         typer.echo(f"Unexpected argument {', '.join([a for a in device[0:-1] if a != 'status'])}")
 
     params, dev = {}, None
     if device and device[-1] != "status":
         dev = cli.cache.get_dev_identifier(device[-1])
-        params["serial"] = dev.serial
+        if dev.type == "ap":
+            params["swarm_id"] = dev.swack_id
+        else:
+            params["serial"] = dev.serial
     else:
         print("Missing required parameter [cyan]<device>[/]")
 
     resp = central.request(central.get_upgrade_status, **params)
 
     tablefmt = cli.get_format(do_json=do_json, do_yaml=do_yaml, do_csv=do_csv, do_table=do_table, default="rich")
 
@@ -1366,35 +1371,60 @@
     """
     resp = cli.central.request(cli.central.get_task_status, task_id)
 
     cli.display_results(
         resp, tablefmt="action", title=f"Task {task_id} status")
 
 
-@app.command(short_help="Show last known running config for a device")
+@app.command()
 def run(
-    device: str = typer.Argument(..., metavar=iden_meta.dev, autocompletion=cli.cache.dev_completion),
-    outfile: Path = typer.Option(None, "--out", help="Output to file (and terminal)", writable=True),
+    device: str = typer.Argument(..., metavar=iden_meta.dev, show_default=False, autocompletion=cli.cache.dev_completion),
+    do_yaml: bool = typer.Option(False, "--yaml", is_flag=True, help="Applies to AOS-SW: Output in YAML format [grey42]\[default: JSON][/]", rich_help_panel="Formatting",),
+    outfile: Path = typer.Option(None, "--out", help="Output to file (and terminal)", show_default=False, writable=True),
     pager: bool = typer.Option(False, "--pager", help="Enable Paged Output"),
     update_cache: bool = typer.Option(False, "-U", hidden=True),  # Force Update of cli.cache for testing
     default: bool = typer.Option(False, "-d", is_flag=True, help="Use default central account", show_default=False,),
     debug: bool = typer.Option(False, "--debug", envvar="ARUBACLI_DEBUG", help="Enable Additional Debug Logging",),
     account: str = typer.Option(
         "central_info",
         envvar="ARUBACLI_ACCOUNT",
         help="The Aruba Central Account to use (must be defined in the config)",
         autocompletion=cli.cache.account_completion,
     ),
 ) -> None:
+    """Show last known running config for a device
+
+    Not supported for CX.
+    Gateways and APs returns typical CLI format.
+    AOS-SW returns a JSON (unless --yaml flag is provided).
+    """
 
     central = cli.central
     dev = cli.cache.get_dev_identifier(device)
 
+    if dev.type == "cx":
+        print("[bright_red]Not Supported:[/] Command not supported for CX switches.")
+        raise typer.Exit(1)
+
     resp = central.request(central.get_device_configuration, dev.serial)
-    cli.display_results(resp, pager=pager, outfile=outfile)
+
+    if isinstance(resp.output, str) and resp.output.startswith("{"):
+        try:
+            cli_config = json.loads(resp.output)
+            cli_config = cli_config.get("_data", cli_config)
+            resp.output = cli_config
+        except Exception as e:
+            log.exception(e)
+
+    if isinstance(resp.output, dict):
+        tablefmt = "json" if not do_yaml else "yaml"
+    else:
+        tablefmt = None
+
+    cli.display_results(resp, tablefmt=tablefmt, pager=pager, outfile=outfile)
 
 
 # TODO --status does not work
 # https://web.yammer.com/main/org/hpe.com/threads/eyJfdHlwZSI6IlRocmVhZCIsImlkIjoiMTQyNzU1MDg5MTQ0MjE3NiJ9
 @app.command(
     "config",
     short_help="Show Central Group/Device or cencli Config",
@@ -1676,30 +1706,31 @@
 
 
 # FIXME show clients wireless <tab completion> does not filter based on type of device
 # FIXME show clients wireless AP-NAME does not filter only devices on that AP
 # Same applies for wired
 @app.command(help="Show clients/details")
 def clients(
-    filter: ClientArgs = typer.Argument('all', case_sensitive=False, ),
+    filter: ClientArgs = typer.Argument('all', case_sensitive=False, show_default=False,),
     device: List[str] = typer.Argument(
         None,
         metavar=iden_meta.dev,
         help="Show clients for a specific device or multiple devices.",
         autocompletion=cli.cache.dev_client_completion,
+        show_default=False,
     ),
-    group: str = typer.Option(None, metavar="<Group>", help="Filter by Group", autocompletion=cli.cache.group_completion),
-    site: str = typer.Option(None, metavar="<Site>", help="Filter by Site", autocompletion=cli.cache.site_completion),
-    label: str = typer.Option(None, metavar="<Label>", help="Filter by Label", ),
+    group: str = typer.Option(None, metavar="<Group>", help="Filter by Group", autocompletion=cli.cache.group_completion, show_default=False,),
+    site: str = typer.Option(None, metavar="<Site>", help="Filter by Site", autocompletion=cli.cache.site_completion, show_default=False,),
+    label: str = typer.Option(None, metavar="<Label>", help="Filter by Label", show_default=False,),
     _dev: List[str] = typer.Option(None, "--dev", metavar=iden_meta.dev, help="Filter by Device", hidden=True,),
     do_json: bool = typer.Option(False, "--json", is_flag=True, help="Output in JSON", show_default=False,),
     do_yaml: bool = typer.Option(False, "--yaml", is_flag=True, help="Output in YAML", show_default=False,),
     do_csv: bool = typer.Option(False, "--csv", is_flag=True, help="Output in CSV", show_default=False,),
     do_table: bool = typer.Option(False, "--table", help="Output in table format", show_default=False,),
-    outfile: Path = typer.Option(None, "--out", help="Output to file (and terminal)", writable=True,),
+    outfile: Path = typer.Option(None, "--out", help="Output to file (and terminal)", writable=True, show_default=False,),
     update_cache: bool = typer.Option(False, "-U", hidden=True,),  # Force Update of cli.cache for testing
     sort_by: SortClientOptions = typer.Option(None, "--sort",),
     reverse: bool = typer.Option(False, "-r", help="Reverse output order", show_default=False,),
     verbose: bool = typer.Option(False, "-v", help="additional details (vertically)", show_default=False,),
     verbose2: bool = typer.Option(
         False,
         "-vv",
@@ -1760,15 +1791,20 @@
         elif len(device) > 1:
             print(f"[bright_red]Warning!![/]: Support for multiple devices not implemented yet. showing denylist for {dev.name} only.")
         dev = cli.cache.get_dev_identifier(device[0])
         args = (dev.serial,)
         title = f"{dev.name} Denylisted Clients"
     elif filter.value != "all":  # wired or wireless
         args = (filter.value, device)
-        title = f"All {filter.value.title()} Clients"
+        if device:
+            dev = cli.cache.get_dev_identifier(device[0])
+            kwargs["serial"] = dev.serial
+            title = f"{dev.name} {filter.value.title()} Clients"
+        else:
+            title = f"All {filter.value.title()} Clients"
     else:  # all
         args = (filter.value, device)
         title = "All Clients"
 
     if filter.value != "denylisted":
         if group:
             kwargs["group"] = cli.cache.get_group_identifier(group).name
@@ -1872,15 +1908,15 @@
         "central_info",
         envvar="ARUBACLI_ACCOUNT",
         help="The Aruba Central Account to use (must be defined in the config)",
         autocompletion=cli.cache.account_completion,
         rich_help_panel="Common Options",
     ),
 ) -> None:
-    """Show Tunnel details"""
+    """Show Branch Gateway/VPNC Tunnel details"""
     dev = cli.cache.get_dev_identifier(gateway, dev_type="gw")
     resp = cli.central.request(cli.central.get_gw_tunnels, dev.serial, timerange=time_range.value)
     caption = None
     if resp:
         if resp.output.get("total"):
             caption = f'Tunnel Count: {resp.output["total"]}'
         if resp.output.get("tunnels"):
@@ -2401,24 +2437,24 @@
             dt = pendulum.from_format(start, 'YYYY-MM-DDTHH:mm', tz="local")
             start = (dt.int_timestamp)
             if not end:
                 time_words = pendulum.from_timestamp(start, tz="local").diff_for_humans()
             else:
                 time_words = f'Alerts from {pendulum.from_timestamp(dt.int_timestamp, tz="local").format("MMM DD h:mm:ss A")}'
         except Exception:
-            print(f"[bright_red]Error:[/bright_red] Value for --start should be in format YYYY-MM-DDTHH:mm (That's a literal 'T')[reset]")
+            print("[bright_red]Error:[/bright_red] Value for --start should be in format YYYY-MM-DDTHH:mm (That's a literal 'T')[reset]")
             print(f"  Value: {start} appears to be invalid.")
             raise typer.Exit(1)
     if end:
         try:
             dt = pendulum.from_format(end, 'YYYY-MM-DDTHH:mm', tz="local")
             end = (dt.int_timestamp)
             time_words = f'{time_words} to {pendulum.from_timestamp(dt.int_timestamp, tz="local").format("MMM DD h:mm:ss A")}'
         except Exception:
-            print(f"[bright_red]Error:[/bright_red] Value for --end should be in format YYYY-MM-DDTHH:mm (That's a literal 'T')[reset]")
+            print("[bright_red]Error:[/bright_red] Value for --end should be in format YYYY-MM-DDTHH:mm (That's a literal 'T')[reset]")
             print(f"  Value: {end} appears to be invalid.")
             raise typer.Exit(1)
     if past:
         now = int(time.time())
         past = past.lower().replace(" ", "")
         if past.endswith("d"):
             start = now - (int(past.rstrip("d")) * 86400)
@@ -2449,15 +2485,15 @@
     if resp.ok:
         if len(resp) == 0:
             resp.output = "No Alerts"
         else:
             time_words = f"[reset][cyan]{len(resp)}{' active' if not ack else ' '}[reset] {time_words}"
 
     tablefmt = cli.get_format(do_json, do_yaml, do_csv, do_table, default="rich" if not verbose else "yaml")
-    title = f"Alerts/Notifications (Configured Notification Rules)"
+    title = "Alerts/Notifications (Configured Notification Rules)"
     if device:
         title = f"{title} [reset]for[cyan] {device.generic_type.upper()} {device.name}|{device.serial}[reset]"
 
     cli.display_results(
         resp,
         tablefmt=tablefmt,
         title=title,
```

### Comparing `centralcli-2.4.0/centralcli/clishowbranch.py` & `centralcli-3.0.0/centralcli/clishowbranch.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/clishowfirmware.py` & `centralcli-3.0.0/centralcli/clishowfirmware.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,142 +17,129 @@
     if pkg_dir.name == "centralcli":
         sys.path.insert(0, str(pkg_dir.parent))
         from centralcli import cli, utils, cleaner
     else:
         print(pkg_dir.parts)
         raise e
 
-from centralcli.constants import IdenMetaVars, lib_to_api  # noqa
+from centralcli.constants import IdenMetaVars, lib_to_api, DevTypes  # noqa
+from centralcli.cache import CentralObject
 
 app = typer.Typer()
 
 tty = utils.tty
 iden_meta = IdenMetaVars()
 
 
-class ShowFirmwareDevType(str, Enum):
-    ap = "ap"
-    # gateway = "gateway"
-    gw = "gw"
-    switch = "switch"
-
 
 class ShowFirmwareKwags(str, Enum):
     group = "group"
     type = "type"
 
 
 @app.command(short_help="Show firmware compliance details")
 def compliance(
-    device_type: ShowFirmwareDevType = typer.Argument(..., metavar="[ap|gw|switch]",),
-    _group: List[str] = typer.Argument(None, metavar="[GROUP-NAME]", autocompletion=cli.cache.group_completion),
-    group_name: str = typer.Option(None, "--group", help="Filter by group", autocompletion=cli.cache.group_completion),
-    do_json: bool = typer.Option(False, "--json", is_flag=True, help="Output in JSON"),
-    do_yaml: bool = typer.Option(False, "--yaml", is_flag=True, help="Output in YAML"),
-    do_csv: bool = typer.Option(False, "--csv", is_flag=True, help="Output in CSV"),
+    device_type: DevTypes = typer.Argument(..., show_default=False,),
+    group: List[str] = typer.Argument(None, metavar="[GROUP-NAME]", autocompletion=cli.cache.group_completion, show_default=False,),
+    group_name: str = typer.Option(None, "--group", help="Filter by group", autocompletion=cli.cache.group_completion, show_default=False,),
+    do_json: bool = typer.Option(False, "--json", is_flag=True, help="Output in JSON",),
+    do_yaml: bool = typer.Option(False, "--yaml", is_flag=True, help="Output in YAML",),
+    do_csv: bool = typer.Option(False, "--csv", is_flag=True, help="Output in CSV",),
     do_table: bool = typer.Option(False, "--table", help="Output in table format",),
-    outfile: Path = typer.Option(None, "--out", help="Output to file (and terminal)", writable=True),
-    pager: bool = typer.Option(False, help="Enable Paged Output"),
-    update_cache: bool = typer.Option(False, "-U", hidden=True),  # Force Update of cli.cache for testing
+    outfile: Path = typer.Option(None, "--out", help="Output to file (and terminal)", show_default=False, writable=True,),
+    pager: bool = typer.Option(False, "--pager", help="Enable Paged Output",),
     default: bool = typer.Option(False, "-d", is_flag=True, help="Use default central account", show_default=False,),
     debug: bool = typer.Option(False, "--debug", envvar="ARUBACLI_DEBUG", help="Enable Additional Debug Logging",),
     account: str = typer.Option("central_info",
                                 envvar="ARUBACLI_ACCOUNT",
                                 help="The Aruba Central Account to use (must be defined in the config)",),
-):
+) -> None:
+    """Show firmware compliance details for a group/device type
+    """
     central = cli.central
-    cli.cache(refresh=update_cache)
-    _type_to_name = {
-        "AP": "IAP",
-        "GATEWAY": "CONTROLLER",
-        "GW": "CONTROLLER",
-        "SWITCH": "HP"
-    }
-    # Allows both:
-    # show firmware compliance <dev-type> <group iden>
-    # show firmware compliance <dev-type> group <group iden>
-    if len(_group) > 2:
-        typer.echo(f"Unknown extra arguments in {[x for x in list(_group)[0:-1] if x.lower() != 'group']}")
+
+    # Allows user to add unnecessary "group" keyword before the group
+    if len(group) > 2:
+        typer.echo(f"Unknown extra arguments in {[x for x in list(group)[0:-1] if x.lower() != 'group']}")
         raise typer.Exit(1)
-    _group = None if not _group else _group[-1]
-    group = _group or group_name
+    group = None if not group else group[-1]
+    group = group or group_name
     if group:
-        group = cli.cache.get_group_identifier(group).name
+        group: CentralObject = cli.cache.get_group_identifier(group)
 
     # TODO make device_type optional add 'all' keyword and implied 'all' if no device_type
     #      add macro method to get compliance for all device_types.
     kwargs = {
-        'device_type': _type_to_name.get(device_type.upper(), device_type),
-        'group': group
+        'device_type': device_type,
+        'group': group.name
     }
 
     resp = central.request(central.get_firmware_compliance, **kwargs)
     if resp.status == 404 and resp.output.lower() == "not found":
         resp.output = (
             f"Invalid URL or No compliance set for {device_type.lower()} "
-            f"{'Globally' if not group else f'in group {group}'}"
+            f"{'Globally' if group is None else f'in group {group.name}'}"
         )
         typer.echo(str(resp).replace("404", typer.style("404", fg="red")))
     else:
         tablefmt = cli.get_format(do_json=do_json, do_yaml=do_yaml, do_csv=do_csv, do_table=do_table)
 
         cli.display_results(
             resp,
             tablefmt=tablefmt,
-            title=f"{'Global ' if not group else f'{group} '}Firmware Compliance",
+            title=f"{'Global ' if not group else f'{group.name} '}Firmware Compliance",
             pager=pager,
             outfile=outfile
         )
 
 @app.command("list")
 def _list(
-    device: str = typer.Argument(None, help="Device to get firmware list for", metavar=iden_meta.dev, autocompletion=cli.cache.dev_completion),
-    dev_type: ShowFirmwareDevType = typer.Option(None, metavar="[ap|gw|switch]", help="Get firmware list for a device type (CX not suppoted, specify a CX device to see list)"),
-    swarm_id: str = typer.Option(None, help="Get available firmware for IAP cluster.",),
+    device: str = typer.Argument(None, help="Device to get firmware list for", metavar=iden_meta.dev, autocompletion=cli.cache.dev_completion, show_default=False,),
+    dev_type: DevTypes = typer.Option(None, help="Get firmware list for a device type", show_default=False,),
+    swarm: bool = typer.Option(False, "--swarm", "-s", help="Get available firmware for IAP cluster associated with provided device", show_default=False,),
+    swarm_id: str = typer.Option(None, help="Get available firmware for specified IAP cluster", show_default=False,),
     do_json: bool = typer.Option(False, "--json", is_flag=True, help="Output in JSON"),
     do_yaml: bool = typer.Option(False, "--yaml", is_flag=True, help="Output in YAML"),
     do_csv: bool = typer.Option(False, "--csv", is_flag=True, help="Output in CSV"),
     do_table: bool = typer.Option(False, "--table", help="Output in table format",),
-    outfile: Path = typer.Option(None, "--out", help="Output to file (and terminal)", writable=True),
-    pager: bool = typer.Option(False, help="Enable Paged Output"),
+    outfile: Path = typer.Option(None, "--out", help="Output to file (and terminal)", show_default=False, writable=True),
+    pager: bool = typer.Option(False, "--pager", help="Enable Paged Output"),
     default: bool = typer.Option(False, "-d", is_flag=True, help="Use default central account", show_default=False,),
     debug: bool = typer.Option(False, "--debug", envvar="ARUBACLI_DEBUG", help="Enable Additional Debug Logging",),
     account: str = typer.Option("central_info",
                                 envvar="ARUBACLI_ACCOUNT",
                                 help="The Aruba Central Account to use (must be defined in the config)",),
 ):
     """Show available firmware list for a specific device or a type of device
-
-    Note: Currently to get list for CX switches you need to specify a CX device.  --dev-type cx is not supported
-    by the API endpoint yet.
     """
-    dev = device if not device else cli.cache.get_dev_identifier(device)
+    dev: CentralObject = device if not device else cli.cache.get_dev_identifier(device)
     _dev_type = dev_type if dev_type is None else lib_to_api("firmware", dev_type)
 
-    # HACK API at least for AOS10 APs returns Invalid Value for device <serial>, convert to --dev-type
+    # API-FLAW # HACK API at least for AOS10 APs returns Invalid Value for device <serial>, convert to --dev-type
     if dev and dev.type == "ap":
-        dev_type = "ap"
-        _dev_type = "IAP"
+        if swarm:
+            swarm_id = dev.swack_id
+        else:
+            dev_type = "ap"
+            _dev_type = "IAP"
         dev = None
 
     kwargs = {
         "device_type": _dev_type,
         "swarm_id": swarm_id,
         "serial": None if dev is None else dev.serial
     }
 
     kwargs = utils.strip_none(kwargs)
 
     _error = ""
     if not kwargs:
-        _error += "\n[dark_orange]:warning:[/] Missing Argument / Option.  One of [cyan]<device(name|serial|mac|ip)>[/] (argument), [cyan]--dev-type <ap|gw|switch>[/], or [cyan]--swarm_id <id>[/] is required."
+        _error += "\n[dark_orange]:warning:[/]  [bright_red]Missing Argument / Option[/].  One of [cyan]<device(name|serial|mac|ip)>[/] (argument), [cyan]--dev-type <ap|gw|switch>[/], or [cyan]--swarm_id <id>[/] is required."
     elif len(kwargs) > 1:
-        _error += "\n[dark_orange]:warning:[/] Invalid combination specify only [bold]one[/] of device (argument), --dev-type, [bold]OR[/] --swarm-id."
-    if dev_type and dev_type == "cx":
-        _error += "\nCX is not supported by the API Endpoint as device_type parameter.  To see available releases for CX provide as CX device as argument."
+        _error += "\n[dark_orange]:warning:[/]  [bright_red]Invalid combination[/] specify only [bold]one[/] of device (argument), --dev-type, [bold]OR[/] --swarm-id."
     if _error:
         print(_error)
         raise typer.Exit(1)
 
     tablefmt = cli.get_format(do_json=do_json, do_yaml=do_yaml, do_csv=do_csv, do_table=do_table)
 
     title = f"Available firmware versions for {list(kwargs.keys())[0].replace('_', ' ')}: {list(kwargs.values())[0]}"
```

### Comparing `centralcli-2.4.0/centralcli/clishowospf.py` & `centralcli-3.0.0/centralcli/clishowospf.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/clishowoverlay.py` & `centralcli-3.0.0/centralcli/clishowoverlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 import sys
 import pendulum
 from pathlib import Path
-from time import sleep
-from typing import List
 
 import typer
 from rich import print
 
 # Detect if called from pypi installed package or via cloned github repo (development)
 try:
     from centralcli import cli, utils, cleaner
@@ -40,17 +38,17 @@
         "Up": "[bright_green]Up[/]",
         "Down": "[bright_red]Down[/]"
     }
 
     if resp and "summary" in resp.raw:
         s = resp.raw["summary"]
         oper_state = s.get("oper_state", "").split("_")[-1].title()
-        caption = f'[cyan]Overlay Connection Summary[/]:'
+        caption = '[cyan]Overlay Connection Summary[/]:'
         caption = f'{caption} Last State Change: {" ".join(pendulum.from_timestamp(s.get("last_state_change", 0), tz="local").to_day_datetime_string().split()[1:])}'
-        caption = f'{caption}\n  Admin Status: {"[bright_green]Up[/]" if s.get("admin_status") else ["[bright_red]Down[/]"]}'
+        caption = f'{caption}\n  Admin Status: {"[bright_green]Up[/]" if s.get("admin_status") else "[bright_red]Down[/]"}'
         caption = f'{caption}, Oper State: {color_status.get(oper_state, oper_state)}'
         # caption = f'{caption}\n  [cyan]Counts[/]: Up: [bright_green]{s.get("up_count")}[/], Down: [bright_red]{s.get("down_count")}[/]'
         caption = f'{caption}, interfaces: {s.get("num_interfaces")}'
         caption = f'{caption}\n  [cyan]Routes[/]: Advertised: {s.get("advertised_routes")}, Learned: {s.get("learned_routes")}'
     else:
         caption = None
 
@@ -178,27 +176,35 @@
     """Show overlay connection (OTO/ORO) details
     """
     dev = cli.cache.get_dev_identifier(device, dev_type=("gw", "ap",))
     tablefmt = cli.get_format(do_json=do_json, do_yaml=do_yaml, do_csv=do_csv, do_table=do_table, default="rich")
 
     resp = cli.central.request(cli.central.get_overlay_connection, dev.serial)
 
+    set_width_cols = {"name": 60}
     if "connection" in resp.output:
         resp.output = resp.output["connection"]
+        caption=_build_caption(resp)
+    elif "summary" in resp.output:
+        resp.output = resp.output["summary"]
+        caption = None
+        if resp.output.get("admin_status") is False:
+            set_width_cols = {"admin status": {"min": 55, "max": 100}}
+
 
     cli.display_results(
         resp,
         tablefmt=tablefmt,
         title=f'{dev.name} Overlay Connection Information [italic](site: {dev.site})[/]',
-        caption=_build_caption(resp),
+        caption=caption,
         pager=pager,
         outfile=outfile,
         sort_by=sort_by,
         reverse=reverse,
-        set_width_cols={"name": 60},
+        set_width_cols=set_width_cols,
         cleaner=cleaner.simple_kv_formatter,
     )
 
 @app.callback()
 def callback():
     """
     Show Overlay (OTO/ORO) Information
```

### Comparing `centralcli-2.4.0/centralcli/clishowtshoot.py` & `centralcli-3.0.0/centralcli/clishowtshoot.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/clishowwids.py` & `centralcli-3.0.0/centralcli/clishowwids.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/clitest.py` & `centralcli-3.0.0/centralcli/clitest.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/clitshoot.py` & `centralcli-3.0.0/centralcli/clitshoot.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/cliunassign.py` & `centralcli-3.0.0/centralcli/cliunassign.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/cliupdate.py` & `centralcli-3.0.0/centralcli/cliupdate.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/cliupgrade.py` & `centralcli-3.0.0/centralcli/cliupgrade.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/config.py` & `centralcli-3.0.0/centralcli/config.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/constants.py` & `centralcli-3.0.0/centralcli/constants.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/logger.py` & `centralcli-3.0.0/centralcli/logger.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/models.py` & `centralcli-3.0.0/centralcli/models.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/objects.py` & `centralcli-3.0.0/centralcli/objects.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/render.py` & `centralcli-3.0.0/centralcli/render.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/response.py` & `centralcli-3.0.0/centralcli/response.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/static/favicon.ico` & `centralcli-3.0.0/centralcli/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/strings.py` & `centralcli-3.0.0/centralcli/strings.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/utils.py` & `centralcli-3.0.0/centralcli/utils.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/vscodeargs.py` & `centralcli-3.0.0/centralcli/vscodeargs.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/wh2snow.py` & `centralcli-3.0.0/centralcli/wh2snow.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/centralcli/wh_proxy.py` & `centralcli-3.0.0/centralcli/wh_proxy.py`

 * *Files identical despite different names*

### Comparing `centralcli-2.4.0/pyproject.toml` & `centralcli-3.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "centralcli"
-version = "2.4.0"
+version = "3.0.0"
 description = "A CLI for interacting with Aruba Central (Cloud Management Platform).  Facilitates bulk imports, exports, reporting.  A handy tool if you have devices managed by Aruba Central."
 license = "MIT"
 authors = ["Wade Wells (Pack3tL0ss) <wade@consolepi.org>"]
 maintainers = ["Wade Wells (Pack3tL0ss) <wade@consolepi.org>"]
 readme = "README.md"
 repository = "https://github.com/Pack3tL0ss/central-api-cli"
 documentation = "https://central-api-cli.readthedocs.org"
```

### Comparing `centralcli-2.4.0/PKG-INFO` & `centralcli-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: centralcli
-Version: 2.4.0
+Version: 3.0.0
 Summary: A CLI for interacting with Aruba Central (Cloud Management Platform).  Facilitates bulk imports, exports, reporting.  A handy tool if you have devices managed by Aruba Central.
 Home-page: https://github.com/Pack3tL0ss/central-api-cli
 License: MIT
 Keywords: cli,Aruba,Aruba Networks,Aruba Central,HPE,API,RESTFUL,REST
 Author: Wade Wells (Pack3tL0ss)
 Author-email: wade@consolepi.org
 Maintainer: Wade Wells (Pack3tL0ss)
```

