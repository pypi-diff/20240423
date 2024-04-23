# Comparing `tmp/snakemake_executor_plugin_lsf-0.2.3.tar.gz` & `tmp/snakemake_executor_plugin_lsf-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_executor_plugin_lsf-0.2.3.tar", max compression
+gzip compressed data, was "snakemake_executor_plugin_lsf-0.2.4.tar", max compression
```

## Comparing `snakemake_executor_plugin_lsf-0.2.3.tar` & `snakemake_executor_plugin_lsf-0.2.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2024-03-22 14:08:07.619478 snakemake_executor_plugin_lsf-0.2.3/LICENSE
--rw-r--r--   0        0        0     5786 2024-03-22 14:08:07.619478 snakemake_executor_plugin_lsf-0.2.3/README.md
--rw-r--r--   0        0        0     1193 2024-03-22 14:08:07.619478 snakemake_executor_plugin_lsf-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    25650 2024-03-22 14:08:07.619478 snakemake_executor_plugin_lsf-0.2.3/snakemake_executor_plugin_lsf/__init__.py
--rw-r--r--   0        0        0     6832 1970-01-01 00:00:00.000000 snakemake_executor_plugin_lsf-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-23 20:37:48.484738 snakemake_executor_plugin_lsf-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5668 2024-04-23 20:37:48.484738 snakemake_executor_plugin_lsf-0.2.4/README.md
+-rw-r--r--   0        0        0     1193 2024-04-23 20:37:48.484738 snakemake_executor_plugin_lsf-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    25647 2024-04-23 20:37:48.484738 snakemake_executor_plugin_lsf-0.2.4/snakemake_executor_plugin_lsf/__init__.py
+-rw-r--r--   0        0        0     6714 1970-01-01 00:00:00.000000 snakemake_executor_plugin_lsf-0.2.4/PKG-INFO
```

### Comparing `snakemake_executor_plugin_lsf-0.2.3/LICENSE` & `snakemake_executor_plugin_lsf-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_lsf-0.2.3/README.md` & `snakemake_executor_plugin_lsf-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 This will give jobs from this rule 14GB of memory and 8 CPU cores. It is
 advisable to use resonable default resources, such that you don\'t need
 to specify them for every rule. Snakemake already has reasonable
 defaults built in, which are automatically activated when using any non-local executor
 (hence also with lsf). Use mem_mb_per_cpu to give the standard LSF type memory per CPU
 
-## MPI jobs {#cluster-lsf-mpi}
+## MPI jobs
 
 Snakemake\'s LSF backend also supports MPI jobs, see
 `snakefiles-mpi`{.interpreted-text role="ref"} for details.
 
 ``` python
 rule calc_pi:
   output:
@@ -93,15 +93,14 @@
 
 You can use the following specifications:
 
 | LSF                                | Snakemake        | Description                            |
 |------------------------------------|------------------|----------------------------------------|
 | `-q`                               | `lsf_queue`      | the queue a rule/job is to use         |
 | `--W`                              | `walltime`       | the walltime per job in minutes        |
-| `--constraint`                     | `constraint`     | may hold features on some clusters     |
 | `-R "rusage[mem=<memory_amount>]"` | `mem`, `mem_mb`  | memory a cluster node must provide     |
 |                                    |                  | (`mem`: string with unit, `mem_mb`: i) |
 | `-R "rusage[mem=<memory_amount>]"` | `mem_mb_per_cpu` | memory per reserved CPU                |
 | omit `-R span[hosts=1]`            | `mpi`            | Allow splitting across nodes for MPI   |
 | `-R span[ptile=<ptile>]`           | `ptile`          | Processors per host. Reqires `mpi`     |
 | Other `bsub` arguments             | `lsf_extra`      | Other args to pass to `bsub` (str)     |
```

### Comparing `snakemake_executor_plugin_lsf-0.2.3/pyproject.toml` & `snakemake_executor_plugin_lsf-0.2.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-executor-plugin-lsf"
-version = "0.2.3"
+version = "0.2.4"
 description = "A Snakemake executor plugin for submitting jobs to a LSF cluster."
 authors = [
     "Brian Fulton-Howard <brian.fulton-howard@mssm.edu>",
     "Christian Meesters <meesters@uni-mainz.de>",
     "David Lähnemann <david.laehnemann@dkfz-heidelberg.de>",
     "Johannes Koester <johannes.koester@uni-due.de>",
 ]
```

### Comparing `snakemake_executor_plugin_lsf-0.2.3/snakemake_executor_plugin_lsf/__init__.py` & `snakemake_executor_plugin_lsf-0.2.4/snakemake_executor_plugin_lsf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import os
 import re
 import subprocess
 import time
 from typing import List, Generator
 from collections import Counter
 import uuid
+import math
 from snakemake_interface_executor_plugins.executors.base import SubmittedJobInfo
 from snakemake_interface_executor_plugins.executors.remote import RemoteExecutor
 from snakemake_interface_executor_plugins.settings import CommonSettings
 from snakemake_interface_executor_plugins.jobs import (
     JobExecutorInterface,
 )
 from snakemake_interface_common.exceptions import WorkflowError
@@ -133,17 +134,14 @@
                 )
             cpus_per_task = job.resources.cpus_per_task
         # ensure that at least 1 cpu is requested
         # because 0 is not allowed by LSF
         cpus_per_task = max(1, cpus_per_task)
         call += f" -n {cpus_per_task}"
 
-        # if job.resources.get("constraint"):
-        #    call += f" -C {job.resources.constraint}"
-
         conv_fcts = {"K": 1024, "M": 1, "G": 1 / 1024, "T": 1 / (1024**2)}
         mem_unit = self.lsf_config.get("LSF_UNIT_FOR_LIMITS", "MB")
         conv_fct = conv_fcts[mem_unit[0]]
         if job.resources.get("mem_mb_per_cpu"):
             mem_ = job.resources.mem_mb_per_cpu * conv_fct
         elif job.resources.get("mem_mb"):
             mem_ = job.resources.mem_mb * conv_fct / cpus_per_task
@@ -556,34 +554,34 @@
     if type(w) in [int, float]:
         # convert int minutes to hours minutes and seconds
         return w
     elif type(w) is str:
         if re.match(r"^\d+(ms|[smhdw])$", w):
             return w
         elif re.match(r"^\d+:\d+$", w):
-            # convert "HH:MM" to hours minutes and seconds
+            # convert "HH:MM" to hours and minutes
             h, m = map(float, w.split(":"))
         elif re.match(r"^\d+:\d+:\d+$", w):
             # convert "HH:MM:SS" to hours minutes and seconds
             h, m, s = map(float, w.split(":"))
         elif re.match(r"^\d+:\d+\.\d+$", w):
             # convert "HH:MM.XX" to hours minutes and seconds
             h, m = map(float, w.split(":"))
             s = (m % 1) * 60
             m = round(m)
         elif re.match(r"^\d+\.\d+$", w):
-            return float(w)
+            return math.ceil(w)
         elif re.match(r"^\d+$", w):
             return int(w)
         else:
             raise ValueError(f"Invalid walltime format: {w}")
     h = int(h)
     m = int(m)
     s = int(s)
-    return (h * 60) + m + (s / 60)
+    return math.ceil((h * 60) + m + (s / 60))
 
 
 def generalize_lsf(rules, runtime=True, memory="perthread_to_perjob"):
     """
     Convert LSF specific resources to generic resources
     """
     re_mem = re.compile(r"^([0-9.]+)(B|KB|MB|GB|TB|PB|KiB|MiB|GiB|TiB|PiB)$")
@@ -594,15 +592,18 @@
                 runtime_ = walltime_lsf_to_generic(res_["walltime"])
                 del rules._rules[k].rule.resources["walltime"]
             elif "time_min" in res_.keys():
                 runtime_ = walltime_lsf_to_generic(res_["time_min"])
                 del rules._rules[k].rule.resources["time_min"]
             elif "runtime" in res_.keys():
                 runtime_ = walltime_lsf_to_generic(res_["runtime"])
-            rules._rules[k].rule.resources["runtime"] = runtime_
+            else:
+                runtime_ = False
+            if runtime_:
+                rules._rules[k].rule.resources["runtime"] = runtime_
         if memory == "perthread_to_perjob":
             if "mem_mb" in res_.keys():
                 mem_ = float(res_["mem_mb"]) * res_["_cores"]
                 if mem_ % 1 == 0:
                     rules._rules[k].rule.resources["mem_mb"] = int(mem_)
                 else:
                     rules._rules[k].rule.resources["mem_mb"] = mem_
```

### Comparing `snakemake_executor_plugin_lsf-0.2.3/PKG-INFO` & `snakemake_executor_plugin_lsf-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-executor-plugin-lsf
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Snakemake executor plugin for submitting jobs to a LSF cluster.
 Home-page: https://github.com/befh/snakemake-executor-plugin-lsf
 License: MIT
 Keywords: snakemake,plugin,executor,cluster,lsf
 Author: Brian Fulton-Howard
 Author-email: brian.fulton-howard@mssm.edu
 Requires-Python: >=3.11,<4.0
@@ -80,15 +80,15 @@
 
 This will give jobs from this rule 14GB of memory and 8 CPU cores. It is
 advisable to use resonable default resources, such that you don\'t need
 to specify them for every rule. Snakemake already has reasonable
 defaults built in, which are automatically activated when using any non-local executor
 (hence also with lsf). Use mem_mb_per_cpu to give the standard LSF type memory per CPU
 
-## MPI jobs {#cluster-lsf-mpi}
+## MPI jobs
 
 Snakemake\'s LSF backend also supports MPI jobs, see
 `snakefiles-mpi`{.interpreted-text role="ref"} for details.
 
 ``` python
 rule calc_pi:
   output:
@@ -115,15 +115,14 @@
 
 You can use the following specifications:
 
 | LSF                                | Snakemake        | Description                            |
 |------------------------------------|------------------|----------------------------------------|
 | `-q`                               | `lsf_queue`      | the queue a rule/job is to use         |
 | `--W`                              | `walltime`       | the walltime per job in minutes        |
-| `--constraint`                     | `constraint`     | may hold features on some clusters     |
 | `-R "rusage[mem=<memory_amount>]"` | `mem`, `mem_mb`  | memory a cluster node must provide     |
 |                                    |                  | (`mem`: string with unit, `mem_mb`: i) |
 | `-R "rusage[mem=<memory_amount>]"` | `mem_mb_per_cpu` | memory per reserved CPU                |
 | omit `-R span[hosts=1]`            | `mpi`            | Allow splitting across nodes for MPI   |
 | `-R span[ptile=<ptile>]`           | `ptile`          | Processors per host. Reqires `mpi`     |
 | Other `bsub` arguments             | `lsf_extra`      | Other args to pass to `bsub` (str)     |
```

