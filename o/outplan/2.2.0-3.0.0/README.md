# Comparing `tmp/outplan-2.2.0.tar.gz` & `tmp/outplan-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/outplan/outplan/dist/tmp4i5n6ngl/outplan-2.2.0.tar", last modified: Fri Jan 19 07:59:03 2024, max compression
+gzip compressed data, was "/home/runner/work/outplan/outplan/dist/.tmp-yfgcoqid/outplan-3.0.0.tar", last modified: Tue Apr 23 12:06:04 2024, max compression
```

## Comparing `outplan-2.2.0.tar` & `outplan-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 07:59:03.000000 outplan-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-01-19 07:58:52.000000 outplan-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-01-19 07:58:52.000000 outplan-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-19 07:58:52.000000 outplan-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-01-19 07:59:03.000000 outplan-2.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 07:59:03.000000 outplan-2.2.0/outplan/
--rw-r--r--   0 runner    (1001) docker     (127)    12942 2024-01-19 07:58:52.000000 outplan-2.2.0/outplan/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-01-19 07:58:52.000000 outplan-2.2.0/outplan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-01-19 07:58:52.000000 outplan-2.2.0/outplan/local.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-19 07:58:52.000000 outplan-2.2.0/outplan/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-19 07:58:52.000000 outplan-2.2.0/outplan/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-01-19 07:58:52.000000 outplan-2.2.0/outplan/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 07:59:03.000000 outplan-2.2.0/outplan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-19 07:59:03.000000 outplan-2.2.0/outplan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-19 07:59:03.000000 outplan-2.2.0/outplan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 07:59:03.000000 outplan-2.2.0/outplan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-01-19 07:59:03.000000 outplan-2.2.0/outplan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-19 07:59:03.000000 outplan-2.2.0/outplan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-01-19 07:58:52.000000 outplan-2.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-19 07:59:03.000000 outplan-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:06:04.000000 outplan-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-23 12:05:59.000000 outplan-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-23 12:06:04.000000 outplan-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-23 12:05:59.000000 outplan-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:06:04.000000 outplan-3.0.0/outplan/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-23 12:05:59.000000 outplan-3.0.0/outplan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-04-23 12:05:59.000000 outplan-3.0.0/outplan/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 12:05:59.000000 outplan-3.0.0/outplan/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 12:05:59.000000 outplan-3.0.0/outplan/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14202 2024-04-23 12:05:59.000000 outplan-3.0.0/outplan/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-23 12:05:59.000000 outplan-3.0.0/outplan/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:06:04.000000 outplan-3.0.0/outplan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-23 12:06:04.000000 outplan-3.0.0/outplan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-23 12:06:04.000000 outplan-3.0.0/outplan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:06:04.000000 outplan-3.0.0/outplan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 12:06:04.000000 outplan-3.0.0/outplan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 12:06:04.000000 outplan-3.0.0/outplan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-23 12:05:59.000000 outplan-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 12:06:04.000000 outplan-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:06:04.000000 outplan-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    30837 2024-04-23 12:05:59.000000 outplan-3.0.0/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-23 12:05:59.000000 outplan-3.0.0/tests/test_local.py
```

### Comparing `outplan-2.2.0/README.md` & `outplan-3.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -36,14 +36,17 @@
 
 # nested experiment/namespace is defined at `tests/test_experiment.py`
 ```
 
 # Dev
 
 ```shell
+# install deps (once)
+pip install -e .[test]
+
 # run test
 make test
 
 # commit
 pip install pre-commit
 # and commit here
 ```
```

### Comparing `outplan-2.2.0/LICENSE` & `outplan-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `outplan-2.2.0/outplan/client.py` & `outplan-3.0.0/outplan/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,28 @@
+import json
 import time
 from contextlib import contextmanager
 from typing import Any, Callable, Dict, Iterator, List, Optional, Union
 
-import simplejson
 from typing_extensions import Protocol
 
 from .const import ONE_MINUTE
 from .exceptions import ExperimentValidateError
 from .experiment import NamespaceItem, TrackingGroup
 from .local import experiment_context
 
 
 class _TrackingClient(Protocol):
-    def track(self, user_id, pdid, event_name, properties=None) -> Any:
-        ...
+    def track(self, user_id, pdid, event_name, properties=None) -> Any: ...
 
 
 class _Logger(Protocol):
-    def error(self, msg: str):
-        ...
+    def error(self, msg: str): ...
 
-    def info(self, msg: str):
-        ...
+    def info(self, msg: str): ...
 
 
 class ExperimentGroupClient:
     """experiment group client"""
 
     def __init__(
         self,
@@ -33,24 +30,21 @@
         lazy_load_namespaces_func: Optional[Callable] = None,
         lazy_load_namespace_item_func: Optional[Callable] = None,
         tracking_client: Optional[_TrackingClient] = None,
         logger: Optional[_Logger] = None,
         lazy_load_expire: int = 10 * ONE_MINUTE,
         get_specified_group_func: Optional[Callable] = None,
     ) -> None:
-
         self.namespaces_items = namespaces_items
         self.namespaces = {namespace.name: namespace for namespace in namespaces_items}
         self.tracking_client = tracking_client
         self.logger = logger
         self.lazy_load_namespaces: List[str] = []
         self.lazy_load_expire = lazy_load_expire
-        self._lazy_load_init_ts: Dict[
-            str, int
-        ] = {}  # 记录 lazy load 的 namespace 初始化时间，expire 之后重新 load
+        self._lazy_load_init_ts: Dict[str, int] = {}  # 记录 lazy load 的 namespace 初始化时间,expire 之后重新 load
         self.lazy_load_namespace_items: Dict[str, NamespaceItem] = {}
         self.lazy_load_namespace_item_func = lazy_load_namespace_item_func
         self._get_specified_group_func = get_specified_group_func
         self.lazy_load_namespaces_func = lazy_load_namespaces_func
 
         self.validate()
 
@@ -64,51 +58,46 @@
 
         return False
 
     def load_lazy_namespaces(self):
         """加载有效的 namespace name 列表"""
         cache_key = "lazy_load_namespaces"
         if self.is_key_expire(cache_key):
-            self.lazy_load_namespaces = (
-                self.lazy_load_namespaces_func() if self.lazy_load_namespaces_func else []
-            )
+            self.lazy_load_namespaces = self.lazy_load_namespaces_func() if self.lazy_load_namespaces_func else []
 
             self.refresh_key_expire_time(cache_key)
 
     def validate(self):
         names = set()
         for namespace in self.namespaces_items:
             if namespace.name in names:
                 raise ExperimentValidateError("namespace name 冲突")
 
             names.add(namespace.name)
 
     def get_namespace_item(self, namespace_name: str) -> NamespaceItem:
-
         # 代码里显式定义的实验直接返回
         if namespace_name in self.namespaces:
             return self.namespaces[namespace_name]
 
         self.load_lazy_namespaces()
         if namespace_name not in self.lazy_load_namespaces:
-            raise ExperimentValidateError("Namespace {} not found.".format(namespace_name))
+            raise ExperimentValidateError(f"Namespace {namespace_name} not found.")
 
         if not self.lazy_load_namespace_item_func:
             raise ExperimentValidateError("lazy_load_namespace_item_func not found")
 
         # 已经 load 过 并且 没过期
-        if namespace_name in self.lazy_load_namespace_items and not self.is_key_expire(
-            namespace_name
-        ):
+        if namespace_name in self.lazy_load_namespace_items and not self.is_key_expire(namespace_name):
             return self.lazy_load_namespace_items[namespace_name]
 
-        # 过期了或者没有 load 过，需要重新 load
+        # 过期了或者没有 load 过,需要重新 load
         _ns = self.lazy_load_namespace_item_func(namespace_name)
         if not _ns:
-            raise ExperimentValidateError("Namespace {} not found".format(namespace_name))
+            raise ExperimentValidateError(f"Namespace {namespace_name} not found")
 
         self.lazy_load_namespace_items[namespace_name] = _ns
         self.refresh_key_expire_time(namespace_name)
         return self.lazy_load_namespace_items[namespace_name]
 
     def get_tracking_group(
         self,
@@ -116,15 +105,15 @@
         unit: Union[str, int] = "",
         user_id: int = 0,
         pdid: str = "",
         track: bool = True,
         cache: bool = True,
         **params,
     ) -> Optional[TrackingGroup]:
-        """取分组的全局唯一标识符，带上实验链的信息"""
+        """取分组的全局唯一标识符,带上实验链的信息"""
         try:
             allow_specify_group = experiment_context.allow_specify_group
         except AttributeError:
             allow_specify_group = False
         try:
             cached_group = experiment_context.cached_group
         except AttributeError:
@@ -135,15 +124,20 @@
             unit = {"pdid": pdid, "user_id": user_id}.get(namespace_item.unit_type, "")  # type: ignore
 
         if namespace_item.auto_upper_unit:
             unit = str(unit).upper()
 
         if unit and allow_specify_group and callable(self._get_specified_group_func):
             group = self._get_specified_group_func(
-                experiment_context, namespace_name, unit, user_id=user_id, pdid=pdid, **params
+                experiment_context,
+                namespace_name,
+                unit,
+                user_id=user_id,
+                pdid=pdid,
+                **params,
             )
             if group:
                 _tracking_group = self.get_tracking_group_by_group_name(namespace_name, group)
                 if _tracking_group:
                     if self.tracking_client and track:
                         self.tracking_client.track(
                             user_id=user_id or 0,
@@ -152,15 +146,15 @@
                             properties=dict(
                                 experiment=_tracking_group.experiment_trace(),
                                 group=_tracking_group.group_trace(),
                             ),
                         )
                     return _tracking_group
 
-        key = "tracking_group{%s}{%s}" % (namespace_name, unit)
+        key = f"tracking_group{{{namespace_name}}}{{{unit}}}"
 
         if unit and cache and key in cached_group:
             return cached_group[key]
 
         tracking_group = namespace_item.get_group(unit, user_id=user_id, pdid=pdid, **params)
         if not tracking_group:
             return None
@@ -185,26 +179,22 @@
         namespace_name: str,
         unit: Union[str, int] = "",
         user_id: int = 0,
         pdid: str = "",
         track: bool = True,
         **params,
     ) -> Optional[str]:
-        tracking_group = self.get_tracking_group(
-            namespace_name, unit, user_id, pdid, track, **params
-        )
+        tracking_group = self.get_tracking_group(namespace_name, unit, user_id, pdid, track, **params)
         if not tracking_group:
             return None
 
         return tracking_group.last_group
 
-    def get_tracking_group_by_group_name(
-        self, namespace_name: str, group_name: str
-    ) -> Optional[TrackingGroup]:
-        """ 根据实验组名获取tracking_group """
+    def get_tracking_group_by_group_name(self, namespace_name: str, group_name: str) -> Optional[TrackingGroup]:
+        """根据实验组名获取tracking_group"""
         namespace_item = self.get_namespace_item(namespace_name)  # type: NamespaceItem
         result = namespace_item.get_experiment_and_group_by_name(group_name)
         if result:
             exp, group = result
             return TrackingGroup(
                 group_name=group.name,
                 experiment_name=exp.name,
@@ -253,101 +243,81 @@
             >>>     if group == Group.a:
             >>>         return "it's a"
             >>>     elif group == Group.control:
             >>>         return "it's control"
         """
         try:
             device_id = experiment_context.device_id
-            if (
-                not params.get("user_id")
-                and hasattr(experiment_context, "user_id")
-                and experiment_context.user_id
-            ):
+            if not params.get("user_id") and hasattr(experiment_context, "user_id") and experiment_context.user_id:
                 params["user_id"] = experiment_context.user_id
 
             yield self.get_group(namespace_name, unit=device_id, pdid=device_id, **params)
 
         except Exception as e:
             # 这里需要被 fallback 到 control 组
             if self.logger:
                 self.logger.error(
-                    f"auto_group error: namespace_name: {namespace_name}, msg: {str(e)}, params: {simplejson.dumps(params)}",
+                    f"auto_group error: namespace_name: {namespace_name}, msg: {e!s}, params: {json.dumps(params)}",
                 )
             yield None
 
     @contextmanager
-    def auto_tracking_group_by_device_id(
-        self, namespace_name: str, **params
-    ) -> Iterator[Optional[TrackingGroup]]:
+    def auto_tracking_group_by_device_id(self, namespace_name: str, **params) -> Iterator[Optional[TrackingGroup]]:
         try:
             device_id = experiment_context.device_id
-            if (
-                not params.get("user_id")
-                and hasattr(experiment_context, "user_id")
-                and experiment_context.user_id
-            ):
+            if not params.get("user_id") and hasattr(experiment_context, "user_id") and experiment_context.user_id:
                 params["user_id"] = experiment_context.user_id
 
             yield self.get_tracking_group(namespace_name, unit=device_id, pdid=device_id, **params)
 
         except Exception as e:
             if self.logger:
                 self.logger.error(
-                    f"auto_tracking_group error: namespace_name: {namespace_name}, msg: {str(e)}, params: {simplejson.dumps(params)}",
+                    f"auto_tracking_group error: namespace_name: {namespace_name}, msg: {e!s}, params: {json.dumps(params)}",  # noqa: E501
                 )
             yield None
 
     @contextmanager
-    def auto_tracking_group_by_user_id(
-        self, namespace_name: str, **params
-    ) -> Iterator[Optional[TrackingGroup]]:
+    def auto_tracking_group_by_user_id(self, namespace_name: str, **params) -> Iterator[Optional[TrackingGroup]]:
         experiment_error = True
         try:
             user_id = experiment_context.user_id
-            if (
-                not params.get("pdid")
-                and hasattr(experiment_context, "device_id")
-                and experiment_context.device_id
-            ):
+            if not params.get("pdid") and hasattr(experiment_context, "device_id") and experiment_context.device_id:
                 params["pdid"] = experiment_context.device_id
 
             res = self.get_tracking_group(namespace_name, unit=user_id, user_id=user_id, **params)
             experiment_error = False
             yield res
         except Exception as e:
             if self.logger and experiment_error:
                 self.logger.error(
-                    f"auto_tracking_group error: namespace_name: {namespace_name}, msg: {str(e)}, params: {simplejson.dumps(params)}",
+                    f"auto_tracking_group error: namespace_name: {namespace_name}, msg: {e!s}, params: {json.dumps(params)}",  # noqa: E501
                 )
 
             # 实验错误需要被 fallback 到 control 组
             # 业务异常直接抛出
             if experiment_error:
                 yield None
             else:
                 raise e
 
     @contextmanager
     def auto_group_by_user_id(self, namespace_name, **params) -> Iterator[Optional[str]]:
         experiment_error = True
         try:
             user_id = experiment_context.user_id or 0
-            if (
-                not params.get("pdid")
-                and hasattr(experiment_context, "device_id")
-                and experiment_context.device_id
-            ):
+            if not params.get("pdid") and hasattr(experiment_context, "device_id") and experiment_context.device_id:
                 params["pdid"] = experiment_context.device_id
 
             res = self.get_group(namespace_name, unit=user_id, user_id=user_id, **params)
             experiment_error = False
             yield res
         except Exception as e:
             # 这里需要被 fallback 到 control 组
             if self.logger and experiment_error:
                 self.logger.error(
-                    f"auto_group error: namespace_name: {namespace_name}, msg: {str(e)}, params: {simplejson.dumps(params)}",
+                    f"auto_group error: namespace_name: {namespace_name}, msg: {e!s}, params: {json.dumps(params)}",
                 )
             if experiment_error:
                 yield None
             else:
                 raise e
```

### Comparing `outplan-2.2.0/outplan/local.py` & `outplan-3.0.0/outplan/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# coding: utf-8
-
 from os import getpid
 
-
 try:
     from greenlet import getcurrent as get_ident
 except ImportError:
     try:
         from thread import get_ident
     except ImportError:
         from _thread import get_ident
@@ -20,15 +17,15 @@
         # greenlet.getcurrent() return greenlet.greenlet object.
         ident = id(ident)
 
     idents = [ident, int(getpid())]
     return "-".join(str(i) for i in idents)
 
 
-class Local(object):
+class Local:
     """A fork-safe Greenlet-local object.
 
     Example:
 
         >>> l = Local()
         >>> l.a = 10
         >>> assert l.a == 10
```

### Comparing `outplan-2.2.0/outplan/experiment.py` & `outplan-3.0.0/outplan/experiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# coding: utf-8
+import json
 from collections import namedtuple
 from decimal import Decimal
-from typing import Any, Callable, Dict, List, Optional, Tuple # noqa
+from typing import Any, Callable, Dict, List, Optional, Tuple  # noqa
 
-import simplejson
 from planout.experiment import DefaultExperiment
 from planout.namespace import SimpleNamespace
 from planout.ops.random import WeightedChoice
 
 from .const import GroupResultType, UserTagFilterType
-from .exceptions import ExperimentGroupNotFindError, ExperimentValidateError
+from .exceptions import ExperimentValidateError
 
 
-class TrackingGroup(object):
+class TrackingGroup:
     """Group object with group trace info"""
 
     def __init__(self, group_name=None, experiment_name=None, group_extra_params=None):
         self.group_names = []
         self.experiment_names = []
         self.group_extra_params = group_extra_params
         if group_name:
@@ -55,15 +54,15 @@
     # type: (ExperimentItem) -> DefaultExperiment
 
     class _PlanoutExperiment(DefaultExperiment):
         def assign(self, params, unit, **kwargs):
             params.group = WeightedChoice(
                 choices=experiment_item.group_items,
                 weights=[group.weight for group in experiment_item.group_items],
-                unit=unit
+                unit=unit,
             )
             params.experiment_name = experiment_item.name
 
     return _PlanoutExperiment
 
 
 def generate_planout_namespace(namespace_item, valid_experiment_items):
@@ -74,17 +73,15 @@
             self.name = namespace_item.name
             self.primary_unit = namespace_item.unit
             self.num_segments = namespace_item.bucket
 
         def setup_experiments(self):
             for experiment_item in valid_experiment_items:
                 self.add_experiment(
-                    experiment_item.name,
-                    generate_planout_experiment(experiment_item),
-                    experiment_item.bucket
+                    experiment_item.name, generate_planout_experiment(experiment_item), experiment_item.bucket
                 )
 
     return _PlanoutNamespace
 
 
 def get_namespace_group_names(namespace_item):
     """取该 namespace 下的所有分组 ID 和 name"""
@@ -95,52 +92,51 @@
             for namespace in group_item.layer_namespaces:
                 _names = get_namespace_group_names(namespace)
                 names.extend(_names)
 
     return names
 
 
-class NamespaceItem(object):
-    """一个 namespace 对应一个总体，里面可以有多个实验，
-    但如果多个实验影响同一个结果，则多个实验必须处于同一个 namespace
+class NamespaceItem:
+    """一个 namespace 对应一个总体,里面可以有多个实验,
+    但如果多个实验影响同一个结果,则多个实验必须处于同一个 namespace
     """
 
     def __init__(self, name, experiment_items, bucket=10, unit="unit", unit_type="", auto_upper_unit=False):
         if not all([name, experiment_items]):
             raise ValueError("Namespace name and experiment_items required.")
 
         self.name = name
-        self.experiment_items = experiment_items    # type: List[ExperimentItem]
+        self.experiment_items = experiment_items  # type: List[ExperimentItem]
         self.bucket = bucket
         self.unit = unit
         self.unit_type = unit_type
         self.auto_upper_unit = auto_upper_unit
 
         self.validate()
 
     def validate(self):
         experiment_total_bucket = 0
         experiment_names = set()
         for experiment_item in self.experiment_items:
-
             experiment_total_bucket += experiment_item.bucket
 
             if experiment_item.name in experiment_names:
-                raise ExperimentValidateError(u"experiment name: {} 重复".format(experiment_item.name))
+                raise ExperimentValidateError(f"experiment name: {experiment_item.name} 重复")
 
             experiment_names.add(experiment_item.name)
 
         if experiment_total_bucket > self.bucket:
-            raise ExperimentValidateError(u"实验({})总 bucket 数小于 namespace bucket 数".format(self.name))
+            raise ExperimentValidateError(f"实验({self.name})总 bucket 数小于 namespace bucket 数")
 
         # 同一个 namespace 下的 group name 必须唯一
         group_names = get_namespace_group_names(self)
 
         if len(group_names) != len(set(group_names)):
-            raise ExperimentValidateError("实验({}) group name 重复".format(self.name))
+            raise ExperimentValidateError(f"实验({self.name}) group name 重复")
 
     def get_group_by_name(self, group_name):
         # type: (str) -> Optional[GroupItem]
         result = self.get_experiment_and_group_by_name(group_name)
         if result is None:
             return None
         _, group_object = result
@@ -151,15 +147,15 @@
         for experiment_item in self.experiment_items:
             for group in experiment_item.group_items:
                 group_object = group.get_group_by_name(group_name)
                 if group_object:
                     return experiment_item, group_object
         return None
 
-    def get_group(self, unit="", **params):
+    def get_group(self, unit="", **params):  # noqa: PLR0912
         if not unit:
             unit = params.get(self.unit_type, "")
 
         valid_experiment_items = []
         for experiment_item in self.experiment_items:
             if callable(experiment_item.pre_condition):
                 if not experiment_item.pre_condition(**params):
@@ -167,26 +163,30 @@
 
             if experiment_item.user_tags and experiment_item.tag_filter_func:
                 res = None
                 # 多个标签为 AND 关系
                 if experiment_item.tag_filter_type == UserTagFilterType.AND:
                     res = True
                     for user_tag in experiment_item.user_tags:
-                        _res = experiment_item.tag_filter_func(experiment_item.name, user_tag.tag_id, user_tag_columns=user_tag.columns, **params)
+                        _res = experiment_item.tag_filter_func(
+                            experiment_item.name, user_tag.tag_id, user_tag_columns=user_tag.columns, **params
+                        )
                         if user_tag.not_in:
                             _res = not _res
 
                         res &= _res
                         if not res:
                             break
                 # 多个标签为 OR 关系
                 elif experiment_item.tag_filter_type == UserTagFilterType.OR:
                     res = False
                     for user_tag in experiment_item.user_tags:
-                        _res = experiment_item.tag_filter_func(experiment_item.name, user_tag.tag_id, user_tag_columns=user_tag.columns, **params)
+                        _res = experiment_item.tag_filter_func(
+                            experiment_item.name, user_tag.tag_id, user_tag_columns=user_tag.columns, **params
+                        )
                         if user_tag.not_in:
                             _res = not _res
 
                         res |= _res
                         if res:
                             break
 
@@ -207,18 +207,17 @@
             return None
 
         group_names, exp_names = [group_item.name], [res.get('experiment_name')]
         if group_item.result_type == GroupResultType.group:
             return TrackingGroup(
                 group_name=group_item.name,
                 experiment_name=res.get('experiment_name'),
-                group_extra_params=group_item.extra_params
+                group_extra_params=group_item.extra_params,
             )
         elif group_item.result_type == GroupResultType.layer:
-
             # 直到取到最底层分组
             while True:
                 _res = group_item.get_group(unit, **params)
                 if isinstance(_res, TrackingGroup):
                     for group_name, exp_name in zip(group_names, exp_names):
                         _res.add_group_name(group_name)
                         _res.add_experiment_name(exp_name)
@@ -232,57 +231,57 @@
     @classmethod
     def from_json(cls, json_namespace, tag_filter_func=None):
         # type: (str, Optional[Callable]) -> NamespaceItem
 
         if not json_namespace:
             raise ExperimentValidateError("json_namespace required.")
 
-        namespace_spec = simplejson.loads(json_namespace)
+        namespace_spec = json.loads(json_namespace)
         return cls.from_dict(namespace_spec, tag_filter_func=tag_filter_func)
 
     @classmethod
     def from_dict(cls, data, tag_filter_func=None):
         # type: (Dict[str, Any], Optional[Callable]) -> NamespaceItem
         return cls(
             name=data['name'],
             bucket=int(data.get('bucket', 10)),
             experiment_items=[ExperimentItem.from_dict(spec, tag_filter_func) for spec in data['experiment_items']],
             unit_type=data.get('unit_type'),
             auto_upper_unit=data.get('auto_upper_unit', False),
         )
 
 
-class ExperimentItem(object):
+class ExperimentItem:
     """实验类"""
 
     def __init__(self, name, bucket, group_items, pre_condition=None, user_tags=None, tag_filter_func=None):
         self.name = name
         self.bucket = bucket
-        self.group_items = group_items                  # type: List[GroupItem]
+        self.group_items = group_items  # type: List[GroupItem]
         self.pre_condition = pre_condition
-        self.tag_filter_type = UserTagFilterType.AND    # 多个 tag_ids 为 and 关系
+        self.tag_filter_type = UserTagFilterType.AND  # 多个 tag_ids 为 and 关系
         self.tag_filter_func = tag_filter_func
 
         try:
             self.user_tags = self._parse_user_tag(user_tags)
         except Exception as e:
-            raise ExperimentValidateError("实验({})标签格式错误:{}".format(self.name, str(e)))
+            raise ExperimentValidateError(f"实验({self.name})标签格式错误:{e!s}")
 
         self.validate()
 
     def validate(self):
         group_names = set()
         for group_item in self.group_items:
             if group_item.name in group_names:
-                raise ExperimentValidateError("group_name {} 冲突".format(group_item.name))
+                raise ExperimentValidateError(f"group_name {group_item.name} 冲突")
 
             group_names.add(group_item.name)
 
         if sum([Decimal(str(group.weight)) for group in self.group_items]) != 1:
-            raise ExperimentValidateError("实验({}) 分组的 weight 总数不为 1".format(self.name))
+            raise ExperimentValidateError(f"实验({self.name}) 分组的 weight 总数不为 1")
 
     @classmethod
     def from_dict(cls, data, tag_filter_func=None):
         # type: (Dict[str, Any], Optional[Callable]) -> ExperimentItem
         return cls(
             name=data['name'],
             bucket=int(data['bucket']),
@@ -300,24 +299,26 @@
         """
         UserTag = namedtuple("UserTag", ["tag_id", "columns", "not_in"])
         if not user_tags:
             return []
 
         res = []
         for user_tag in user_tags:
-            res.append(UserTag(
-                tag_id=user_tag['id'],
-                columns=user_tag['columns'],
-                not_in=user_tag.get('not_in', False)    # not_in 表示该标签的互斥，不在该标签里
-            ))
+            res.append(
+                UserTag(
+                    tag_id=user_tag['id'],
+                    columns=user_tag['columns'],
+                    not_in=user_tag.get('not_in', False),  # not_in 表示该标签的互斥,不在该标签里
+                )
+            )
 
         return res
 
 
-class GroupItem(object):
+class GroupItem:
     def __init__(self, name, weight, layer_namespaces=None, extra_params=None):
         self.name = name
         self.weight = weight
         self.layer_namespaces = layer_namespaces or []  # type: List[NamespaceItem]
         self.result_type = None
         self.extra_params = extra_params
 
@@ -326,22 +327,22 @@
     def validate(self):
         # 分层
         if self.layer_namespaces:
             self.result_type = GroupResultType.layer
             namespace_names = set()
             for namespace_item in self.layer_namespaces:
                 if namespace_item.name in namespace_names:
-                    raise ExperimentValidateError("namespace name({}) 冲突".format(namespace_item.name))
+                    raise ExperimentValidateError(f"namespace name({namespace_item.name}) 冲突")
 
                 namespace_names.add(namespace_item.name)
         # 分组
         else:
             self.result_type = GroupResultType.group
             if self.weight > 1:
-                raise ExperimentValidateError("group weight({}) 必须小于等于 1".format(self.name))
+                raise ExperimentValidateError(f"group weight({self.name}) 必须小于等于 1")
 
     def get_group(self, unit, **params):
         if self.result_type == GroupResultType.group:
             return self.name
         elif self.result_type == GroupResultType.layer:
             # 这里所有复制出来的 namespace 只有一个返回 group
             for namespace in self.layer_namespaces:
@@ -367,10 +368,13 @@
 
     @classmethod
     def from_dict(cls, data, tag_filter_func=None):
         # type: (Dict[str, Any], Optional[Callable]) -> GroupItem
         return cls(
             name=data['name'],
             weight=float(data['weight']),
-            layer_namespaces=[NamespaceItem.from_dict(spec, tag_filter_func=tag_filter_func) for spec in data.get('layer_namespaces', [])],
-            extra_params=data.get('extra_params')
+            layer_namespaces=[
+                NamespaceItem.from_dict(spec, tag_filter_func=tag_filter_func)
+                for spec in data.get('layer_namespaces', [])
+            ],
+            extra_params=data.get('extra_params'),
         )
```

