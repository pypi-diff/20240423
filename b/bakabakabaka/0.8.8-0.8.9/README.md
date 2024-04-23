# Comparing `tmp/bakabakabaka-0.8.8.tar.gz` & `tmp/bakabakabaka-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bakabakabaka-0.8.8.tar", last modified: Sat Apr 13 05:22:11 2024, max compression
+gzip compressed data, was "bakabakabaka-0.8.9.tar", last modified: Tue Apr 23 03:47:07 2024, max compression
```

## Comparing `bakabakabaka-0.8.8.tar` & `bakabakabaka-0.8.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:22:11.683558 bakabakabaka-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 05:22:03.000000 bakabakabaka-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-13 05:22:11.679558 bakabakabaka-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-13 05:22:03.000000 bakabakabaka-0.8.8/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)    33225 2024-04-13 05:22:03.000000 bakabakabaka-0.8.8/baka.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:22:11.679558 bakabakabaka-0.8.8/bakabakabaka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-13 05:22:11.000000 bakabakabaka-0.8.8/bakabakabaka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-13 05:22:11.000000 bakabakabaka-0.8.8/bakabakabaka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:22:11.000000 bakabakabaka-0.8.8/bakabakabaka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-13 05:22:11.000000 bakabakabaka-0.8.8/bakabakabaka.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-13 05:22:11.000000 bakabakabaka-0.8.8/bakabakabaka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 05:22:11.683558 bakabakabaka-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-13 05:22:03.000000 bakabakabaka-0.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:47:07.793903 bakabakabaka-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 03:46:58.000000 bakabakabaka-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-23 03:47:07.793903 bakabakabaka-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-23 03:46:58.000000 bakabakabaka-0.8.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33549 2024-04-23 03:46:58.000000 bakabakabaka-0.8.9/baka.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:47:07.789903 bakabakabaka-0.8.9/bakabakabaka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-23 03:47:07.000000 bakabakabaka-0.8.9/bakabakabaka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-23 03:47:07.000000 bakabakabaka-0.8.9/bakabakabaka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 03:47:07.000000 bakabakabaka-0.8.9/bakabakabaka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-23 03:47:07.000000 bakabakabaka-0.8.9/bakabakabaka.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 03:47:07.000000 bakabakabaka-0.8.9/bakabakabaka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 03:47:07.793903 bakabakabaka-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-23 03:46:58.000000 bakabakabaka-0.8.9/setup.py
```

### Comparing `bakabakabaka-0.8.8/LICENSE` & `bakabakabaka-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bakabakabaka-0.8.8/PKG-INFO` & `bakabakabaka-0.8.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakabakabaka
-Version: 0.8.8
+Version: 0.8.9
 Summary: the stupid configuration tracker using the stupid content tracker
 Home-page: https://github.com/elesiuta/baka
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bakabakabaka-0.8.8/README.md` & `bakabakabaka-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `bakabakabaka-0.8.8/baka.py` & `bakabakabaka-0.8.9/baka.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,27 +15,28 @@
 
 # https://github.com/elesiuta/baka
 
 import argparse
 import datetime
 import email
 import email.mime.text
+import functools
 import hashlib
 import json
 import os
 import shlex
 import shutil
 import smtplib
 import socket
 import subprocess
 import sys
 import time
 import typing
 
-__version__: typing.Final[str] = "0.8.8"
+__version__: typing.Final[str] = "0.8.9"
 BASE_PATH: typing.Final[str] = os.path.expanduser("~/.baka")
 
 
 def init_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(description="the stupid configuration tracker using the stupid content tracker",
                                      usage="%(prog)s [--dry-run] <argument>")
     parser.add_argument("--version", action="version", version=__version__)
@@ -476,18 +477,21 @@
         cmds.append(["git", "commit", "-m", f"baka file {config.hostname}"])
     elif args.job:
         if args.interactive:
             config.jobs[args.job]["interactive"] = True
         cmds = config.jobs[args.job]["commands"]
     elif args.list:
         cmds = [
-            ["echo", "Prompt\tExit!0\tJob Name\n========================"],
-            *[["echo", "%s\t%s\t%s" % ("interactive" in config.jobs[job] and config.jobs[job]["interactive"],
-                                       "exit_non_zero" in config.jobs[job] and config.jobs[job]["exit_non_zero"],
-                                       job)] for job in config.jobs]
+            ["echo", "Email\tExit!0\tInter.\tVerb.\tWrite\tJob Name\n================================================"],
+            *[["echo", "%s\t%s\t%s\t%s\t%s\t%s" % (str(functools.reduce(lambda d, k : d.get(k) if isinstance(d, dict) and d.get(k) else False, ("email", "to"), config.jobs[job]))[:6],
+                                                   bool(config.jobs[job].get("exit_non_zero")),
+                                                   bool(config.jobs[job].get("interactive")),
+                                                   str(config.jobs[job].get("verbosity", "debug"))[:6],
+                                                   str(config.jobs[job].get("write", False))[:6],
+                                                   job)] for job in config.jobs]
         ]
     elif args.system_checks:
         assert ("history" not in config.system_checks)
         assert all([key not in config.system_scans for key in config.system_checks])
         cmds = [
             *copy_and_git_add_all(),
             ["git", "commit", "-m", "baka pre-sysck"],
@@ -537,24 +541,24 @@
                 command_output.append("dry-run")
                 command_output.append(">>> " + shlex.join(cmd))
                 continue
             # execute command if not dry-run
             if args.job:
                 # run command as part of job, otherwise run command normally
                 capture_output = bool(
-                    ("write" in config.jobs[args.job] and config.jobs[args.job]["write"]) or
-                    ("email" in config.jobs[args.job] and config.jobs[args.job]["email"] and config.jobs[args.job]["email"]["to"])
+                    (config.jobs[args.job].get("write")) or
+                    (isinstance(config.jobs[args.job].get("email"), dict) and config.jobs[args.job]["email"].get("to"))
                 )
                 verbosity = config.jobs[args.job].get("verbosity", "debug")
                 verbosity = verbosity if verbosity else "debug"
                 verbosity = verbosity.lower()
                 assert verbosity in ["debug", "info", "error", "silent"]
                 if verbosity in ["debug"]:
                     print("\033[94m%s\033[0m" % shlex.join(cmd))
-                if config.jobs[args.job].get("interactive", False):
+                if config.jobs[args.job].get("interactive"):
                     response = input("\033[92mContinue (yes/no/skip)?\033[0m ")
                     if response.strip().lower().startswith("y"):
                         pass
                     elif response.strip().lower().startswith("n"):
                         break
                     elif response.strip().lower().startswith("s"):
                         continue
@@ -571,15 +575,15 @@
                         proc_err = sys.stderr
                 proc = subprocess.run(cmd, stdout=proc_out, stderr=proc_err, input=proc_input)
                 if proc.returncode != 0:
                     if args.error_interactive:
                         return_code += 1
                         print(f"Error: exit {proc.returncode} for `{shlex.join(cmd)}`, continuing in interactive mode")
                         config.jobs[args.job]["interactive"] = True
-                    elif config.jobs[args.job].get("exit_non_zero", False):
+                    elif config.jobs[args.job].get("exit_non_zero"):
                         return_code = proc.returncode
                         error_message = "Error: baka job encountered a non-zero exit code for `%s`, exiting" % shlex.join(cmd)
                         command_output.append(error_message)
                         print(error_message, file=sys.stderr)
                         break
                     else:
                         return_code += 1
@@ -630,22 +634,22 @@
         if error_message:
             log_entry += " " + error_message
         with open(os.path.join(BASE_PATH, "history.log"), "a", encoding="utf-8", errors="surrogateescape") as log_file:
             log_file.write(log_entry + "\n")
     # email or write command output
     if args.job:
         command_output = "\n".join(command_output)
-        if "email" in config.jobs[args.job] and config.jobs[args.job]["email"] and config.jobs[args.job]["email"]["to"]:
+        if isinstance(config.jobs[args.job].get("email"), dict) and config.jobs[args.job]["email"].get("to"):
             try:
                 send_email(config.email, config.jobs[args.job]["email"], command_output)
             except Exception as e:
                 error_email = "--- %s ---\nEmail Error: %s %s\nMessage:\n%s" % (time.ctime(), type(e).__name__, e.args, command_output)
                 with open(os.path.join(BASE_PATH, "error.log"), "a", encoding="utf-8", errors="surrogateescape") as log_file:
                     log_file.write(error_email + "\n")
-        if "write" in config.jobs[args.job] and config.jobs[args.job]["write"]:
+        if config.jobs[args.job].get("write"):
             file_path = os.path.abspath(datetime.datetime.now().strftime(config.jobs[args.job]["write"]))
             os.makedirs(os.path.dirname(file_path), exist_ok=True)
             with open(file_path, "w", encoding="utf-8", errors="backslashreplace") as f:
                 f.write(command_output)
     return return_code
```

### Comparing `bakabakabaka-0.8.8/bakabakabaka.egg-info/PKG-INFO` & `bakabakabaka-0.8.9/bakabakabaka.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakabakabaka
-Version: 0.8.8
+Version: 0.8.9
 Summary: the stupid configuration tracker using the stupid content tracker
 Home-page: https://github.com/elesiuta/baka
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bakabakabaka-0.8.8/setup.py` & `bakabakabaka-0.8.9/setup.py`

 * *Files identical despite different names*

