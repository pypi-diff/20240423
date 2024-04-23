# Comparing `tmp/ecs_session-24.4.4.tar.gz` & `tmp/ecs_session-24.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_session-24.4.4.tar", max compression
+gzip compressed data, was "ecs_session-24.4.5.tar", max compression
```

## Comparing `ecs_session-24.4.4.tar` & `ecs_session-24.4.5.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      869 2024-04-22 17:39:27.026743 ecs_session-24.4.4/README.md
--rw-r--r--   0        0        0     3343 2024-04-22 18:19:36.616747 ecs_session-24.4.4/ecs_session/__init__.py
--rw-r--r--   0        0        0     6076 2024-04-22 18:19:30.941594 ecs_session-24.4.4/ecs_session/cli.py
--rw-r--r--   0        0        0      477 2024-04-22 18:19:46.199006 ecs_session-24.4.4/pyproject.toml
--rw-r--r--   0        0        0     1940 1970-01-01 00:00:00.000000 ecs_session-24.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1160 2024-04-23 07:37:20.808381 ecs_session-24.4.5/README.md
+-rw-r--r--   0        0        0     3859 2024-04-23 07:44:18.396818 ecs_session-24.4.5/ecs_session/__init__.py
+-rw-r--r--   0        0        0     6147 2024-04-23 08:10:06.349342 ecs_session-24.4.5/ecs_session/cli.py
+-rw-r--r--   0        0        0      477 2024-04-23 08:10:43.680882 ecs_session-24.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 ecs_session-24.4.5/setup.py
+-rw-r--r--   0        0        0     2180 1970-01-01 00:00:00.000000 ecs_session-24.4.5/PKG-INFO
```

### Comparing `ecs_session-24.4.4/README.md` & `ecs_session-24.4.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -5,30 +5,36 @@
 Provides a tool to interact with AWS ECS tasks.
 
 Currently provides:
 
 * interactive execute-command (e.g. shell)
 * port-forwarding
 
-You can supply command-line arguments to specify which cluster/service/task/... to use or will be prompted
-with a nice menu.
+You can supply command-line arguments to specify which cluster/service/task/... to use or will be prompted with a nice menu.
 
 ## Installation
 
 ```
 pip install ecs-session
 ```
 
 ## Pre-requisites
 
-### Tools
+### [session-manager-plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html)
 
-* [session-manager-plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html)
+#### Linux
+
+```bash
+curl https://s3.amazonaws.com/session-manager-downloads/plugin/latest/ubuntu_64bit/session-manager-plugin.deb -o "/tmp/session-manager-plugin.deb"
+mkdir -p ~/bin
+dpkg-deb --fsys-tarfile /tmp/session-manager-plugin.deb | tar --strip-components=4 -C ~/bin/ -xvf - usr/local/sessionmanagerplugin/bin/session-manager-plugin
+```
+
+#### MacOS
 
-MacOS users can alternatively install this via Homebrew:
 `brew install --cask session-manager-plugin`
 
 ### Infrastructure
 
 Use [ecs-exec-checker](https://github.com/aws-containers/amazon-ecs-exec-checker) to check for the pre-requisites to use ECS exec.
```

### Comparing `ecs_session-24.4.4/ecs_session/cli.py` & `ecs_session-24.4.5/ecs_session/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,18 @@
 def show_menu(items: list, title: str, source: list = None, clear_screen: bool = True):
     """
     menu function
     """
     index = None
     source = source or items
     menu = TerminalMenu(
-        items, title=title, show_search_hint=True, clear_screen=clear_screen
+        items,
+        title=f"? {title}:\n",
+        show_search_hint=True,
+        clear_screen=clear_screen,
     )
     index = menu.show()
     if index is None:
         exit(0)
     return source[index], index
 
 
@@ -214,16 +217,18 @@
         task=task,
         task_details=task_details,
     )
     function = {
         "forward": ecs_session.port_forward,
         "command": ecs_session.execute_command,
     }
+    print(f"---")
     print(f"cluster: {cluster}")
     print(f"service: {service}")
     print(f"task: {task}")
     print(f"container: {container}")
+    print(f"---")
     function.get(arguments.action)()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ecs_session-24.4.4/PKG-INFO` & `ecs_session-24.4.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecs-session
-Version: 24.4.4
+Version: 24.4.5
 Summary: ECS SSM tool
 Home-page: https://github.com/morph027/ecs-session
 License: MIT
 Author: Stefan Heitmüller
 Author-email: stefan.heitmueller@gmx.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3
 Requires-Dist: configargparse
 Requires-Dist: shtab
 Requires-Dist: simple_term_menu
 Project-URL: Repository, https://github.com/morph027/ecs-session
 Description-Content-Type: text/markdown
 
@@ -33,30 +32,36 @@
 Provides a tool to interact with AWS ECS tasks.
 
 Currently provides:
 
 * interactive execute-command (e.g. shell)
 * port-forwarding
 
-You can supply command-line arguments to specify which cluster/service/task/... to use or will be prompted
-with a nice menu.
+You can supply command-line arguments to specify which cluster/service/task/... to use or will be prompted with a nice menu.
 
 ## Installation
 
 ```
 pip install ecs-session
 ```
 
 ## Pre-requisites
 
-### Tools
+### [session-manager-plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html)
 
-* [session-manager-plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html)
+#### Linux
+
+```bash
+curl https://s3.amazonaws.com/session-manager-downloads/plugin/latest/ubuntu_64bit/session-manager-plugin.deb -o "/tmp/session-manager-plugin.deb"
+mkdir -p ~/bin
+dpkg-deb --fsys-tarfile /tmp/session-manager-plugin.deb | tar --strip-components=4 -C ~/bin/ -xvf - usr/local/sessionmanagerplugin/bin/session-manager-plugin
+```
+
+#### MacOS
 
-MacOS users can alternatively install this via Homebrew:
 `brew install --cask session-manager-plugin`
 
 ### Infrastructure
 
 Use [ecs-exec-checker](https://github.com/aws-containers/amazon-ecs-exec-checker) to check for the pre-requisites to use ECS exec.
```

