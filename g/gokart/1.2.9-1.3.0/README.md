# Comparing `tmp/gokart-1.2.9.tar.gz` & `tmp/gokart-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokart-1.2.9.tar", max compression
+gzip compressed data, was "gokart-1.3.0.tar", max compression
```

## Comparing `gokart-1.2.9.tar` & `gokart-1.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1065 2024-04-05 02:41:37.673605 gokart-1.2.9/LICENSE
--rw-r--r--   0        0        0     3657 2024-04-05 02:41:37.673605 gokart-1.2.9/README.md
--rw-r--r--   0        0        0      635 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/__init__.py
--rw-r--r--   0        0        0     3388 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/build.py
--rw-r--r--   0        0        0     1534 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/config_params.py
--rw-r--r--   0        0        0     4426 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/conflict_prevention_lock/task_lock.py
--rw-r--r--   0        0        0     3962 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/conflict_prevention_lock/task_lock_wrappers.py
--rw-r--r--   0        0        0     9582 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/file_processor.py
--rw-r--r--   0        0        0     1004 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/gcs_config.py
--rw-r--r--   0        0        0     1380 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/gcs_zip_client.py
--rw-r--r--   0        0        0     1555 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/info.py
--rw-r--r--   0        0        0     2389 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/object_storage.py
--rw-r--r--   0        0        0     1754 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/pandas_type_config.py
--rw-r--r--   0        0        0     3266 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/parameter.py
--rw-r--r--   0        0        0        0 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/py.typed
--rw-r--r--   0        0        0     3899 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/run.py
--rw-r--r--   0        0        0      834 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/s3_config.py
--rw-r--r--   0        0        0     1657 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/s3_zip_client.py
--rw-r--r--   0        0        0      191 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/slack/__init__.py
--rw-r--r--   0        0        0     1693 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/slack/event_aggregator.py
--rw-r--r--   0        0        0     1819 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/slack/slack_api.py
--rw-r--r--   0        0        0      685 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/slack/slack_config.py
--rw-r--r--   0        0        0     8322 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/target.py
--rw-r--r--   0        0        0    24299 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/task.py
--rw-r--r--   0        0        0      471 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/task_complete_check.py
--rw-r--r--   0        0        0      204 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/testing/__init__.py
--rw-r--r--   0        0        0     3045 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/testing/check_if_run_with_empty_data_frame.py
--rw-r--r--   0        0        0     1289 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/testing/pandas_assert.py
--rw-r--r--   0        0        0     3918 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/tree/task_info.py
--rw-r--r--   0        0        0     4792 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/tree/task_info_formatter.py
--rw-r--r--   0        0        0      199 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/utils.py
--rw-r--r--   0        0        0     1177 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/workspace_management.py
--rw-r--r--   0        0        0     1402 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/zip_client.py
--rw-r--r--   0        0        0      432 2024-04-05 02:41:37.677605 gokart-1.2.9/gokart/zip_client_util.py
--rw-r--r--   0        0        0     1972 2024-04-05 02:41:49.521626 gokart-1.2.9/pyproject.toml
--rw-r--r--   0        0        0     4810 1970-01-01 00:00:00.000000 gokart-1.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-23 07:31:08.592507 gokart-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3657 2024-04-23 07:31:08.592507 gokart-1.3.0/README.md
+-rw-r--r--   0        0        0      635 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/__init__.py
+-rw-r--r--   0        0        0     3590 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/build.py
+-rw-r--r--   0        0        0     1534 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/config_params.py
+-rw-r--r--   0        0        0     4426 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/conflict_prevention_lock/task_lock.py
+-rw-r--r--   0        0        0     3962 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/conflict_prevention_lock/task_lock_wrappers.py
+-rw-r--r--   0        0        0     9574 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/file_processor.py
+-rw-r--r--   0        0        0     1004 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/gcs_config.py
+-rw-r--r--   0        0        0     1380 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/gcs_zip_client.py
+-rw-r--r--   0        0        0     1555 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/info.py
+-rw-r--r--   0        0        0     2389 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/object_storage.py
+-rw-r--r--   0        0        0     1754 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/pandas_type_config.py
+-rw-r--r--   0        0        0     3266 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/parameter.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/py.typed
+-rw-r--r--   0        0        0     3899 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/run.py
+-rw-r--r--   0        0        0      834 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/s3_config.py
+-rw-r--r--   0        0        0     1657 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/s3_zip_client.py
+-rw-r--r--   0        0        0      191 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/slack/__init__.py
+-rw-r--r--   0        0        0     1693 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/slack/event_aggregator.py
+-rw-r--r--   0        0        0     1819 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/slack/slack_api.py
+-rw-r--r--   0        0        0      685 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/slack/slack_config.py
+-rw-r--r--   0        0        0     8322 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/target.py
+-rw-r--r--   0        0        0    25051 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/task.py
+-rw-r--r--   0        0        0      471 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/task_complete_check.py
+-rw-r--r--   0        0        0      204 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/testing/__init__.py
+-rw-r--r--   0        0        0     3055 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/testing/check_if_run_with_empty_data_frame.py
+-rw-r--r--   0        0        0     1289 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/testing/pandas_assert.py
+-rw-r--r--   0        0        0     3918 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/tree/task_info.py
+-rw-r--r--   0        0        0     4766 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/tree/task_info_formatter.py
+-rw-r--r--   0        0        0     1735 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/utils.py
+-rw-r--r--   0        0        0     1174 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/workspace_management.py
+-rw-r--r--   0        0        0     1402 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/zip_client.py
+-rw-r--r--   0        0        0      432 2024-04-23 07:31:08.596506 gokart-1.3.0/gokart/zip_client_util.py
+-rw-r--r--   0        0        0     1983 2024-04-23 07:31:20.180573 gokart-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4830 1970-01-01 00:00:00.000000 gokart-1.3.0/PKG-INFO
```

### Comparing `gokart-1.2.9/LICENSE` & `gokart-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/README.md` & `gokart-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/__init__.py` & `gokart-1.3.0/gokart/__init__.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/build.py` & `gokart-1.3.0/gokart/build.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from typing import Any, Optional
 
 import backoff
 import luigi
 
 import gokart
 from gokart.conflict_prevention_lock.task_lock import TaskLockException
+from gokart.target import TargetOnKart
 from gokart.task import TaskOnKart
 
 
 class LoggerConfig:
     def __init__(self, level: int):
         self.logger = getLogger(__name__)
         self.default_level = self.logger.level
         self.level = level
-        print(f'LoggerConfig: {self.default_level} -> {self.level}')
 
     def __enter__(self):
         logging.disable(self.level - 10)  # subtract 10 to disable below self.level
         self.logger.setLevel(self.level)
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
@@ -39,19 +39,22 @@
 class TaskLockExceptionRaisedFlag:
     def __init__(self):
         self.flag: bool = False
 
 
 def _get_output(task: TaskOnKart) -> Any:
     output = task.output()
+    # FIXME: currently, nested output is not supported
     if isinstance(output, list) or isinstance(output, tuple):
-        return [t.load() for t in output]
+        return [t.load() for t in output if isinstance(t, TargetOnKart)]
     if isinstance(output, dict):
-        return {k: t.load() for k, t in output.items()}
-    return output.load()
+        return {k: t.load() for k, t in output.items() if isinstance(t, TargetOnKart)}
+    if isinstance(output, TargetOnKart):
+        return output.load()
+    raise ValueError(f'output type is not supported: {type(output)}')
 
 
 def _reset_register(keep={'gokart', 'luigi'}):
     """reset luigi.task_register.Register._reg everytime gokart.build called to avoid TaskClassAmbigiousException"""
     luigi.task_register.Register._reg = [
         x
         for x in luigi.task_register.Register._reg
```

### Comparing `gokart-1.2.9/gokart/config_params.py` & `gokart-1.3.0/gokart/config_params.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/conflict_prevention_lock/task_lock.py` & `gokart-1.3.0/gokart/conflict_prevention_lock/task_lock.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/conflict_prevention_lock/task_lock_wrappers.py` & `gokart-1.3.0/gokart/conflict_prevention_lock/task_lock_wrappers.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/file_processor.py` & `gokart-1.3.0/gokart/file_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
-import pickle
 import xml.etree.ElementTree as ET
 from abc import abstractmethod
 from io import BytesIO
 from logging import getLogger
 
+import dill
 import luigi
 import luigi.contrib.s3
 import luigi.format
 import numpy as np
 import pandas as pd
 import pandas.errors
 from luigi.format import TextFormat
@@ -78,19 +78,19 @@
 
 class PickleFileProcessor(FileProcessor):
     def format(self):
         return luigi.format.Nop
 
     def load(self, file):
         if not ObjectStorage.is_buffered_reader(file):
-            return pickle.loads(file.read())
-        return pickle.load(_ChunkedLargeFileReader(file))
+            return dill.loads(file.read())
+        return dill.load(_ChunkedLargeFileReader(file))
 
     def dump(self, obj, file):
-        self._write(pickle.dumps(obj, protocol=4), file)
+        self._write(dill.dumps(obj, protocol=4), file)
 
     @staticmethod
     def _write(buffer, file):
         n = len(buffer)
         idx = 0
         while idx < n:
             logger.info(f'writing a file with total_bytes={n}...')
```

### Comparing `gokart-1.2.9/gokart/gcs_config.py` & `gokart-1.3.0/gokart/gcs_config.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/gcs_zip_client.py` & `gokart-1.3.0/gokart/gcs_zip_client.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/info.py` & `gokart-1.3.0/gokart/info.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/object_storage.py` & `gokart-1.3.0/gokart/object_storage.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/pandas_type_config.py` & `gokart-1.3.0/gokart/pandas_type_config.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/parameter.py` & `gokart-1.3.0/gokart/parameter.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/run.py` & `gokart-1.3.0/gokart/run.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/s3_config.py` & `gokart-1.3.0/gokart/s3_config.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/s3_zip_client.py` & `gokart-1.3.0/gokart/s3_zip_client.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/slack/event_aggregator.py` & `gokart-1.3.0/gokart/slack/event_aggregator.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/slack/slack_api.py` & `gokart-1.3.0/gokart/slack/slack_api.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/slack/slack_config.py` & `gokart-1.3.0/gokart/slack/slack_config.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/target.py` & `gokart-1.3.0/gokart/target.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/task.py` & `gokart-1.3.0/gokart/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 from typing import Any, Callable, Dict, List, Optional, Set, Union
 
 import luigi
 import pandas as pd
 from luigi.parameter import ParameterVisibility
 
 import gokart
+import gokart.target
 from gokart.conflict_prevention_lock.task_lock import make_task_lock_params, make_task_lock_params_for_run
 from gokart.conflict_prevention_lock.task_lock_wrappers import wrap_run_with_lock
 from gokart.file_processor import FileProcessor
 from gokart.pandas_type_config import PandasTypeConfigMap
 from gokart.parameter import ExplicitBoolParameter, ListTaskInstanceParameter, TaskInstanceParameter
 from gokart.target import TargetOnKart
 from gokart.task_complete_check import task_complete_check_wrapper
+from gokart.utils import FlattenableItems, flatten
 
 logger = getLogger(__name__)
 
 
 class TaskOnKart(luigi.Task):
     """
     This is a wrapper class of luigi.Task.
@@ -99,18 +101,21 @@
         if self.should_lock_run:
             self._lock_at_dump = False
             assert self.redis_host is not None, 'redis_host must be set when should_lock_run is True.'
             assert self.redis_port is not None, 'redis_port must be set when should_lock_run is True.'
             task_lock_params = make_task_lock_params_for_run(task_self=self)
             self.run = wrap_run_with_lock(run_func=self.run, task_lock_params=task_lock_params)
 
-    def output(self):
+    def input(self) -> FlattenableItems[TargetOnKart]:
+        return super().input()
+
+    def output(self) -> FlattenableItems[TargetOnKart]:
         return self.make_target()
 
-    def requires(self):
+    def requires(self) -> FlattenableItems['TaskOnKart']:
         tasks = self.make_task_instance_dictionary()
         return tasks or []  # when tasks is empty dict, then this returns empty list.
 
     def make_task_instance_dictionary(self) -> Dict[str, 'TaskOnKart']:
         return {key: var for key, var in vars(self).items() if self.is_task_on_kart(var)}
 
     @staticmethod
@@ -126,35 +131,35 @@
             return
         for key, value in dict(config[section]).items():
             if key not in kwargs and key in class_variables:
                 kwargs[key] = class_variables[key].parse(value)
 
     def complete(self) -> bool:
         if self._rerun_state:
-            for target in luigi.task.flatten(self.output()):
+            for target in flatten(self.output()):
                 target.remove()
             self._rerun_state = False
             return False
 
-        is_completed = all([t.exists() for t in luigi.task.flatten(self.output())])
+        is_completed = all([t.exists() for t in flatten(self.output())])
 
         if self.strict_check or self.modification_time_check:
-            requirements = luigi.task.flatten(self.requires())
-            inputs = luigi.task.flatten(self.input())
+            requirements = flatten(self.requires())
+            inputs = flatten(self.input())
             is_completed = is_completed and all([task.complete() for task in requirements]) and all([i.exists() for i in inputs])
 
         if not self.modification_time_check or not is_completed or not self.input():
             return is_completed
 
         return self._check_modification_time()
 
     def _check_modification_time(self):
-        common_path = set(t.path() for t in luigi.task.flatten(self.input())) & set(t.path() for t in luigi.task.flatten(self.output()))
-        input_tasks = [t for t in luigi.task.flatten(self.input()) if t.path() not in common_path]
-        output_tasks = [t for t in luigi.task.flatten(self.output()) if t.path() not in common_path]
+        common_path = set(t.path() for t in flatten(self.input())) & set(t.path() for t in flatten(self.output()))
+        input_tasks = [t for t in flatten(self.input()) if t.path() not in common_path]
+        output_tasks = [t for t in flatten(self.output()) if t.path() not in common_path]
 
         input_modification_time = max([target.last_modification_time() for target in input_tasks]) if input_tasks else None
         output_modification_time = min([target.last_modification_time() for target in output_tasks]) if output_tasks else None
 
         if input_modification_time is None or output_modification_time is None:
             return True
 
@@ -330,34 +335,43 @@
                 return str(task.make_unique_id()) if task.significant else None
 
             if not isinstance(task, luigi.Task):
                 raise ValueError(f'Task.requires method returns {type(task)}. You should return luigi.Task.')
 
             return task.to_str_params(only_significant=True)
 
-        dependencies = [_to_str_params(task) for task in luigi.task.flatten(self.requires())]
+        dependencies = [_to_str_params(task) for task in flatten(self.requires())]
         dependencies = [d for d in dependencies if d is not None]
         dependencies.append(self.to_str_params(only_significant=True))
         dependencies.append(self.__class__.__name__)
         if self.serialized_task_definition_check:
             dependencies.append(self.get_own_code())
         return hashlib.md5(str(dependencies).encode()).hexdigest()
 
-    def _get_input_targets(self, target: Union[None, str, TargetOnKart]) -> Union[TargetOnKart, List[TargetOnKart]]:
+    def _get_input_targets(self, target: Union[None, str, TargetOnKart]) -> FlattenableItems[TargetOnKart]:
         if target is None:
             return self.input()
         if isinstance(target, str):
-            return self.input()[target]
+            input = self.input()
+            assert isinstance(input, dict), f'input must be dict[str, TargetOnKart], but {type(input)} is passed.'
+            result: FlattenableItems[TargetOnKart] = input[target]
+            return result
         return target
 
     def _get_output_target(self, target: Union[None, str, TargetOnKart]) -> TargetOnKart:
         if target is None:
-            return self.output()
+            output = self.output()
+            assert isinstance(output, TargetOnKart), f'output must be TargetOnKart, but {type(output)} is passed.'
+            return output
         if isinstance(target, str):
-            return self.output()[target]
+            output = self.output()
+            assert isinstance(output, dict), f'output must be dict[str, TargetOnKart], but {type(output)} is passed.'
+            result = output[target]
+            assert isinstance(result, TargetOnKart), f'output must be dict[str, TargetOnKart], but {type(output)} is passed.'
+            return result
         return target
 
     def get_info(self, only_significant=False):
         params_str = {}
         params = dict(self.get_params())
         for param_name, param_value in self.param_kwargs.items():
             if (not only_significant) or params[param_name].significant:
@@ -376,15 +390,15 @@
             return self.task_log
         if target.exists():
             return self.load(target)
         return dict()
 
     @luigi.Task.event_handler(luigi.Event.SUCCESS)
     def _dump_task_log(self):
-        self.task_log['file_path'] = [target.path() for target in luigi.task.flatten(self.output())]
+        self.task_log['file_path'] = [target.path() for target in flatten(self.output())]
         if self.should_dump_supplementary_log_files:
             self.dump(self.task_log, self._get_task_log_target())
 
     def _get_task_params_target(self):
         return self.make_target(f'log/task_params/{type(self).__name__}.pkl')
 
     def get_task_params(self) -> Dict:
```

### Comparing `gokart-1.2.9/gokart/testing/check_if_run_with_empty_data_frame.py` & `gokart-1.3.0/gokart/testing/check_if_run_with_empty_data_frame.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import List, Optional
 
 import luigi
 import pandas as pd
 from luigi.cmdline_parser import CmdlineParser
 
 import gokart
+from gokart.utils import flatten
 
 test_logger = logging.getLogger(__name__)
 test_logger.addHandler(logging.StreamHandler())
 test_logger.setLevel(logging.INFO)
 
 
 class test_run(gokart.TaskOnKart):
@@ -35,15 +36,18 @@
         return s
 
     def fail(self) -> bool:
         return self.status != 'OK'
 
 
 def _get_all_tasks(task: gokart.TaskOnKart) -> List[gokart.TaskOnKart]:
-    return luigi.task.flatten([_get_all_tasks(o) for o in luigi.task.flatten(task.requires()) if isinstance(o, gokart.TaskOnKart)] + [task])
+    result = [task]
+    for o in flatten(task.requires()):
+        result.extend(_get_all_tasks(o))
+    return result
 
 
 def _run_with_test_status(task: gokart.TaskOnKart):
     test_message = _TestStatus(task)
     try:
         task.run()
     except Exception as e:
```

### Comparing `gokart-1.2.9/gokart/testing/pandas_assert.py` & `gokart-1.3.0/gokart/testing/pandas_assert.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/tree/task_info.py` & `gokart-1.3.0/gokart/tree/task_info.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/gokart/tree/task_info_formatter.py` & `gokart-1.3.0/gokart/tree/task_info_formatter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import typing
 import warnings
 from dataclasses import dataclass
-from typing import Dict, List, NamedTuple, Optional, Set, Union
-
-import luigi
+from typing import Dict, List, NamedTuple, Optional, Set
 
 from gokart.task import TaskOnKart
+from gokart.utils import FlattenableItems, flatten
 
 
 @dataclass
 class TaskInfo:
     name: str
     unique_id: str
-    output_paths: List[TaskOnKart]
+    output_paths: List[str]
     params: dict
     processing_time: str
     is_complete: str
     task_log: dict
-    requires: Union['RequiredTask', List['RequiredTask'], Dict[str, 'RequiredTask']]
+    requires: FlattenableItems['RequiredTask']
     children_task_infos: List['TaskInfo']
 
     def get_task_id(self):
         return f'{self.name}_{self.unique_id}'
 
     def get_task_title(self):
         return f'({self.is_complete}) {self.name}[{self.unique_id}]'
@@ -61,30 +60,30 @@
 def make_task_info_tree(task: TaskOnKart, ignore_task_names: Optional[List[str]] = None, cache: Optional[Dict[str, TaskInfo]] = None) -> TaskInfo:
     with warnings.catch_warnings():
         warnings.filterwarnings(action='ignore', message='Task .* without outputs has no custom complete() method')
         is_task_complete = task.complete()
 
     name = task.__class__.__name__
     unique_id = task.make_unique_id()
-    output_paths = [t.path() for t in luigi.task.flatten(task.output())]
+    output_paths: List[str] = [t.path() for t in flatten(task.output())]
 
     cache = {} if cache is None else cache
     cache_id = f'{name}_{unique_id}_{is_task_complete}'
     if cache_id in cache:
         return cache[cache_id]
 
     params = task.get_info(only_significant=True)
     processing_time = task.get_processing_time()
     if isinstance(processing_time, float):
         processing_time = str(processing_time) + 's'
     is_complete = 'COMPLETE' if is_task_complete else 'PENDING'
     task_log = dict(task.get_task_log())
     requires = _make_requires_info(task.requires())
 
-    children = luigi.task.flatten(task.requires())
+    children = flatten(task.requires())
     children_task_infos: List[TaskInfo] = []
     for child in children:
         if ignore_task_names is None or child.__class__.__name__ not in ignore_task_names:
             children_task_infos.append(make_task_info_tree(child, ignore_task_names=ignore_task_names, cache=cache))
     task_info = TaskInfo(
         name=name,
         unique_id=unique_id,
```

### Comparing `gokart-1.2.9/gokart/workspace_management.py` & `gokart-1.3.0/gokart/workspace_management.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import itertools
 import os
 import pathlib
 from logging import getLogger
 
-import luigi
-
 import gokart
+from gokart.utils import flatten
 
 logger = getLogger(__name__)
 
 
 def _get_all_output_file_paths(task: gokart.TaskOnKart):
-    output_paths = [t.path() for t in luigi.task.flatten(task.output())]
-    children = luigi.task.flatten(task.requires())
+    output_paths = [t.path() for t in flatten(task.output())]
+    children = flatten(task.requires())
     output_paths.extend(itertools.chain.from_iterable([_get_all_output_file_paths(child) for child in children]))
     return output_paths
 
 
 def delete_local_unnecessary_outputs(task: gokart.TaskOnKart):
     task.make_unique_id()  # this is required to make unique ids.
     all_files = {str(path) for path in pathlib.Path(task.workspace_directory).rglob('*.*')}
```

### Comparing `gokart-1.2.9/gokart/zip_client.py` & `gokart-1.3.0/gokart/zip_client.py`

 * *Files identical despite different names*

### Comparing `gokart-1.2.9/pyproject.toml` & `gokart-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gokart"
-version = "1.2.9"  # using poetry-dynamic-versioning
+version = "1.3.0"  # using poetry-dynamic-versioning
 description="Gokart solves reproducibility, task dependencies, constraints of good code, and ease of use for Machine Learning Pipeline. [Documentation](https://gokart.readthedocs.io/en/latest/)"
 authors = ["M3, inc."]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/m3dev/gokart"
 repository = "https://github.com/m3dev/gokart"
 documentation = "https://gokart.readthedocs.io/en/latest/"
@@ -25,14 +25,15 @@
 tqdm = "*"
 google-auth = "*"
 pyarrow = "*"
 uritemplate = "*"
 google-api-python-client = "*"
 APScheduler = "*"
 redis = "*"
+dill = "*"
 backoff = "^2.2.1"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "*"
 tox = "*"
 moto = "*"
 testfixtures = "*"
```

### Comparing `gokart-1.2.9/PKG-INFO` & `gokart-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: gokart
-Version: 1.2.9
+Version: 1.3.0
 Summary: Gokart solves reproducibility, task dependencies, constraints of good code, and ease of use for Machine Learning Pipeline. [Documentation](https://gokart.readthedocs.io/en/latest/)
 Home-page: https://github.com/m3dev/gokart
 License: MIT
 Author: M3, inc.
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: APScheduler
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: boto3
+Requires-Dist: dill
 Requires-Dist: google-api-python-client
 Requires-Dist: google-auth
 Requires-Dist: luigi
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: redis
```

