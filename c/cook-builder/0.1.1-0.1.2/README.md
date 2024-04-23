# Comparing `tmp/cook_builder-0.1.1.tar.gz` & `tmp/cook_builder-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cook_builder-0.1.1.tar", last modified: Sat Apr 20 13:36:05 2024, max compression
+gzip compressed data, was "cook_builder-0.1.2.tar", last modified: Tue Apr 23 18:17:07 2024, max compression
```

## Comparing `cook_builder-0.1.1.tar` & `cook_builder-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-20 13:36:05.090545 cook_builder-0.1.1/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.1.1/LICENSE
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3006 2024-04-20 13:36:05.090545 cook_builder-0.1.1/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      877 2024-04-19 18:55:28.000000 cook_builder-0.1.1/README.md
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-20 13:36:05.090545 cook_builder-0.1.1/cook/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       35 2024-04-20 08:35:09.000000 cook_builder-0.1.1/cook/__init__.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1204 2024-04-20 08:24:26.000000 cook_builder-0.1.1/cook/build.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1757 2024-04-20 11:07:01.000000 cook_builder-0.1.1/cook/cli.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     4851 2024-04-20 08:51:37.000000 cook_builder-0.1.1/cook/configuration.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2762 2024-04-20 09:11:32.000000 cook_builder-0.1.1/cook/cook.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      150 2024-04-16 14:39:30.000000 cook_builder-0.1.1/cook/exception.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2050 2024-04-20 09:06:17.000000 cook_builder-0.1.1/cook/executors.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      809 2024-04-20 09:16:35.000000 cook_builder-0.1.1/cook/logger.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1129 2024-04-20 09:17:16.000000 cook_builder-0.1.1/cook/main.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1030 2024-04-13 20:33:00.000000 cook_builder-0.1.1/cook/recipe.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2146 2024-04-20 09:09:37.000000 cook_builder-0.1.1/cook/rsync.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1383 2024-04-20 08:25:29.000000 cook_builder-0.1.1/cook/sync.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      381 2024-04-20 09:09:37.000000 cook_builder-0.1.1/cook/watchers.py
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-20 13:36:05.090545 cook_builder-0.1.1/cook_builder.egg-info/
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3006 2024-04-20 13:36:05.000000 cook_builder-0.1.1/cook_builder.egg-info/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      451 2024-04-20 13:36:05.000000 cook_builder-0.1.1/cook_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-04-20 13:36:05.000000 cook_builder-0.1.1/cook_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-20 13:36:05.000000 cook_builder-0.1.1/cook_builder.egg-info/entry_points.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       27 2024-04-20 13:36:05.000000 cook_builder-0.1.1/cook_builder.egg-info/requires.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-04-20 13:36:05.000000 cook_builder-0.1.1/cook_builder.egg-info/top_level.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1141 2024-04-20 13:35:33.000000 cook_builder-0.1.1/pyproject.toml
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-20 13:36:05.090545 cook_builder-0.1.1/setup.cfg
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-23 18:17:07.876594 cook_builder-0.1.2/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.1.2/LICENSE
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3006 2024-04-23 18:17:07.876594 cook_builder-0.1.2/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      877 2024-04-19 18:55:28.000000 cook_builder-0.1.2/README.md
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-23 18:17:07.876594 cook_builder-0.1.2/cook/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       35 2024-04-20 08:35:09.000000 cook_builder-0.1.2/cook/__init__.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1204 2024-04-20 08:24:26.000000 cook_builder-0.1.2/cook/build.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2609 2024-04-23 18:16:32.000000 cook_builder-0.1.2/cook/cli.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     4851 2024-04-20 08:51:37.000000 cook_builder-0.1.2/cook/configuration.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3050 2024-04-22 20:22:09.000000 cook_builder-0.1.2/cook/cook.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      150 2024-04-16 14:39:30.000000 cook_builder-0.1.2/cook/exception.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2407 2024-04-23 16:22:15.000000 cook_builder-0.1.2/cook/executors.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      984 2024-04-22 20:26:52.000000 cook_builder-0.1.2/cook/logger.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1840 2024-04-23 18:11:15.000000 cook_builder-0.1.2/cook/main.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1030 2024-04-22 19:33:15.000000 cook_builder-0.1.2/cook/recipe.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2310 2024-04-22 20:00:03.000000 cook_builder-0.1.2/cook/rsync.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1383 2024-04-20 08:25:29.000000 cook_builder-0.1.2/cook/sync.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      381 2024-04-20 09:09:37.000000 cook_builder-0.1.2/cook/watchers.py
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-23 18:17:07.876594 cook_builder-0.1.2/cook_builder.egg-info/
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3006 2024-04-23 18:17:07.000000 cook_builder-0.1.2/cook_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      451 2024-04-23 18:17:07.000000 cook_builder-0.1.2/cook_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-04-23 18:17:07.000000 cook_builder-0.1.2/cook_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-23 18:17:07.000000 cook_builder-0.1.2/cook_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       27 2024-04-23 18:17:07.000000 cook_builder-0.1.2/cook_builder.egg-info/requires.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-04-23 18:17:07.000000 cook_builder-0.1.2/cook_builder.egg-info/top_level.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1141 2024-04-23 18:16:47.000000 cook_builder-0.1.2/pyproject.toml
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-23 18:17:07.876594 cook_builder-0.1.2/setup.cfg
```

### Comparing `cook_builder-0.1.1/LICENSE` & `cook_builder-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.1/PKG-INFO` & `cook_builder-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.1.1
+Version: 0.1.2
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cook_builder-0.1.1/README.md` & `cook_builder-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.1/cook/build.py` & `cook_builder-0.1.2/cook/build.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.1/cook/cli.py` & `cook_builder-0.1.2/cook/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,77 @@
 import argparse
 import pathlib
 
-from .main import main, settings
+from .main import Main
+
+
+class Settings:
+    def __init__(self):
+        self.args = {}
+        self.flags = []
+
+
+settings = Settings()
 
 
 def parse_user_args(user_args):
-    res = {}
-    for arg in user_args:
-        key, value = arg.split('=')
-        res[key] = value
-    return res
+    args = {}
+    flags = []
 
+    for user_arg in user_args:
+        if '=' in user_arg:
+            key, value = user_arg.split('=')
+            args[key] = value
+        else:
+            flags.append(user_arg)
+    return args, flags
 
-def cli():
-    global settings
 
+def cli():
     epilog_text = '\n'.join(
         (
             'example usage:',
             '  %(prog)s my_project name=latest -p ./example/ -b local',
         )
     )
 
     parser = argparse.ArgumentParser(
         description='Build script aggregator and remote executor', epilog=epilog_text, formatter_class=argparse.RawDescriptionHelpFormatter
     )
 
-    parser.add_argument('-p', '--recipe_path', default='.', help='Path to directory containing `recipe.py` file.')
+    parser.add_argument('-r', '--recipe_path', default='.', help='Path to directory containing `recipe.py` file.')
     parser.add_argument('-b', '--build_server', help='Build server to use. Uses value of `default_build_server` if left unspecified.')
-    parser.add_argument('-r', '--rich_output', action='store_true')
-    parser.add_argument('project', nargs='?', help='Project to build. Uses value of `default_project` if left unspecified.')
-    parser.add_argument('user_args', nargs='*', default=[], help='User arguments. Can be used in recipe file. Format: `key=value`')
-
-    # TODO: add dry run
-    # TODO: add quiet option
-    # TODO: add user flag args
-    # TODO: use better user args, e.g. --name latest
+    parser.add_argument('-f', '--format', action='store_true', help='Format output using Rich.')
+    parser.add_argument('-t', '--targets', action='store_true', help='List available projects.')
+    parser.add_argument('-d', '--dry', action='store_true', help='Dry run.')
+    parser.add_argument('-q', '--quiet', action='store_true', help='Suppress stdout.')
+    parser.add_argument('-u', '--user_args', nargs='*', default=[], help='User arguments. Can be used in recipe file. Format either `key=value` or `flag`.')
+    parser.add_argument('-p', '--project', default=None, help='Project to build. Uses value of `default_project` if left unspecified.')
 
     args = parser.parse_args()
-    settings.recipe_base_path = (pathlib.Path.cwd() / args.recipe_path).resolve()
-    settings.build_server = args.build_server
-    if args.project and '=' in args.project:
-        settings.project = None
-        args.user_args.insert(0, args.project)
-    else:
-        settings.project = args.project
-    settings.user_args.update(parse_user_args(args.user_args))
-    settings.rich_output = args.rich_output
 
-    main()
+    recipe_base_path = (pathlib.Path.cwd() / args.recipe_path).resolve()
+    build_server = args.build_server
+    project = args.project
+
+    user_args, user_flags = parse_user_args(args.user_args)
+    settings.args.update(user_args)
+    settings.flags.extend(user_flags)
+
+    rich_output = args.format
+    quiet = args.quiet
+
+    list_targets = args.targets
+    dry_run = args.dry
+
+    main_program = Main(recipe_base_path, project, build_server, rich_output=rich_output, quiet=quiet)
+    main_program.initialize()
+
+    if list_targets:
+        projects, default_project = main_program.get_projects()
+        recipe_path = main_program.get_recipe_path()
+        print(f'Projects defined in {recipe_path}:')
+        for project in projects:
+            print('  ' + project, '<- default' if project == default_project else '')
+        return
+
+    main_program.run(dry_run=dry_run)
```

### Comparing `cook_builder-0.1.1/cook/configuration.py` & `cook_builder-0.1.2/cook/configuration.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.1/cook/cook.py` & `cook_builder-0.1.2/cook/cook.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 
 class Cook:
     def __init__(self, recipe, configuration, logger):
         self.recipe = recipe
         self.configuration = configuration
         self.logger = logger
+        self.dry_run = False
+
+    def set_dry_run(self, dry_run: bool):
+        self.dry_run = dry_run
 
     def cook(self):
         build_type = self.configuration.get_build_type()
         self.build_server = self.configuration.get_build_server()
 
         if build_type == BuildType.LOCAL:
             self._local_build()
@@ -28,33 +32,36 @@
 
     def _local_build(self):
         build_steps = self.configuration.get_build_steps()
 
         if build_steps:
             self.logger.print('local', 'Running local build')
             executor = LocalExecutor('local', self.logger)
+            executor.set_dry_run(self.dry_run)
             executor.run_multiple(build_steps)
 
     def _remote_build(self):
         build_steps = self.configuration.get_build_steps()
         local_base, remote_base = self.configuration.get_base_paths()
         files_to_send = self.configuration.get_files_to_send()
         files_to_receive = self.configuration.get_files_to_receive()
 
         setup_rsync = files_to_send or files_to_receive
         if setup_rsync:
             rsync = Rsync(self.build_server, local_base, remote_base, self.logger)
+            rsync.set_dry_run(self.dry_run)
 
         if files_to_send:
             self.logger.print('remote', 'Sending Files')
             rsync.send(files_to_send)
 
         if build_steps:
             self.logger.print('remote', 'Running Remote Build')
             executor = RemoteExecutor(self.build_server, self.logger)
+            executor.set_dry_run(self.dry_run)
             executor.run_multiple(build_steps)
 
         if files_to_receive:
             self.logger.print('remote', 'Receiving Files')
             rsync.receive(files_to_receive)
 
     def _composite_build(self):
@@ -71,11 +78,12 @@
 
     def _run_component(self, component):
         try:
             sub_configuration = Configuration(self.recipe)
             sub_configuration.setup(component, self.build_server)
 
             sub_cook = Cook(self.recipe, sub_configuration, self.logger)
+            sub_cook.set_dry_run(self.dry_run)
             sub_cook.cook()
         except Exception as e:
             self.logger.print('error', f'Component {component} failed!')
             raise e
```

### Comparing `cook_builder-0.1.1/cook/executors.py` & `cook_builder-0.1.2/cook/executors.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,32 +12,48 @@
     def __init__(self, message, name, return_code):
         super().__init__(message)
         self.name = name
         self.return_code = return_code
 
 
 class Executor:
-    def __init__(self, name=None, logger=None, rich_output=False):
+    def __init__(self, name=None, logger=None):
         self.name = name
+        self.dry_run = False
+
         self.logger = logger
-        self.rich_output = rich_output
+        if self.logger:
+            self.rich_output = self.logger.use_rich_output()
+            self.quiet = self.logger.is_quiet()
+        else:
+            self.rich_output = False
+            self.quiet = False
+
+    def set_dry_run(self, dry_run: bool):
+        self.dry_run = dry_run
 
     def run(self, context, step):
+        if self.dry_run:
+            return
+
         run_args = {'watchers': []}
 
+        if self.quiet:
+            run_args['hide'] = 'out'
+
         if self.rich_output and self.logger:
             rich_printer = RichPrinter(self.logger)
             run_args['hide'] = 'both'
             run_args['watchers'].append(rich_printer)
 
         if step.responders:
             run_args['watchers'].extend(step.responders)
 
         with context.cd(step.workdir):
-            result = context.run(step.command, warn=True, pty=True, **run_args)
+            result = context.run(step.command, warn=True, **run_args)
 
         return_code = result.return_code
         if step.check and return_code != step.expected_return_code:
             raise ProcessError(f'Encountered unexpected exit code {return_code}, expected {step.expected_return_code}', return_code)
 
 
 class LocalExecutor(Executor):
```

### Comparing `cook_builder-0.1.1/cook/main.py` & `cook_builder-0.1.2/cook/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,45 +2,54 @@
 from .cook import Cook
 from .exception import ProcessError
 from .executors import ExecutorError
 from .logger import Logger
 from .recipe import Recipe, RecipeError, RecipeNotFound
 
 
-class Settings:
-    def __init__(self):
-        self.recipe_base_path = None
-        self.build_server = None
-        self.rich_output = None
-        self.project = None
-        self.user_args = {}
-
-
-settings = Settings()
-
-
-def main():
-    global settings
-
-    logger = Logger(settings.rich_output)
-
-    try:
-        recipe = Recipe(settings.recipe_base_path)
-        recipe.load()
-
-        configuration = Configuration(recipe)
-        configuration.setup(settings.project, settings.build_server)
-
-        cook = Cook(recipe, configuration, logger)
-        cook.cook()
-
-    except (RecipeNotFound, RecipeError, ConfigurationError) as e:
-        logger.print('error', e)
-        exit(1)
-
-    except ProcessError as e:
-        logger.print('error', e)
-        exit(e.return_code)
-
-    except ExecutorError as e:
-        logger.print('error', f'{e.name}: {e}')
-        exit(e.return_code)
+class Main:
+    def __init__(self, recipe_base_path, project, build_server, rich_output=False, quiet=False):
+        self.recipe_base_path = recipe_base_path
+        self.project = project
+        self.build_server = build_server
+        self.rich_output = rich_output
+        self.quiet = quiet
+
+    def get_recipe_path(self):
+        return (self.recipe.base_path / "recipe.py").as_posix()
+
+    def get_projects(self):
+        projects = list(self.recipe.projects.keys())
+        default_project = self.recipe.default_project
+        return projects, default_project
+
+    def initialize(self):
+        self.logger = Logger(self.rich_output, self.quiet)
+
+        if self.rich_output and self.quiet:
+            self.logger.print('warning', 'Suppressing stdout and using formatted output will also suppress stderr!')
+
+        try:
+            self.recipe = Recipe(self.recipe_base_path)
+            self.recipe.load()
+
+            self.configuration = Configuration(self.recipe)
+            self.configuration.setup(self.project, self.build_server)
+
+            self.cook = Cook(self.recipe, self.configuration, self.logger)
+
+        except (RecipeNotFound, RecipeError, ConfigurationError) as e:
+            logger.print('error', e)
+            exit(1)
+
+    def run(self, dry_run=False):
+        try:
+            self.cook.set_dry_run(dry_run)
+            self.cook.cook()
+
+        except ProcessError as e:
+            logger.print('error', e)
+            exit(e.return_code)
+
+        except ExecutorError as e:
+            logger.print('error', f'{e.name}: {e}')
+            exit(e.return_code)
```

### Comparing `cook_builder-0.1.1/cook/recipe.py` & `cook_builder-0.1.2/cook/recipe.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.1/cook/rsync.py` & `cook_builder-0.1.2/cook/rsync.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 
     # TODO: add rsync for local build
     def __init__(self, hostname, local_base, remote_base, logger=None):
         self.hostname = hostname
         self.logger = logger
         self.local_base = local_base
         self.remote_base = remote_base
+        self.dry_run = False
 
-    def sync(self, src, dst, exludes):
-        if self.logger is not None:
-            self.logger.log(f'Transferring: {src} to {dst}\n')
+    def set_dry_run(self, dry_run: bool):
+        self.dry_run = dry_run
 
+    def sync(self, src, dst, exludes):
         cmd = list(Rsync.command)
         cmd.append(src)
         cmd.append(dst)
         cmd.extend([Rsync.exclude + e for e in exludes])
 
         result = subprocess.run(' '.join(cmd), shell=True)
         if result.returncode != 0:
@@ -56,14 +57,20 @@
         for rsync_item in rsync_items:
             is_exclude = getattr(rsync_item, 'is_exclude', False)
             if is_exclude:
                 continue
 
             src, dst = rsync_item.parse(**parser_args)
 
+            if self.logger is not None:
+                self.logger.log(f'Transferring: {src} to {dst}\n')
+
+            if self.dry_run:
+                return
+
             self.sync(src, dst, excludes)
 
     def send(self, rsync_items):
         self.sync_multiple(rsync_items, src_base=self.local_base, dst_host=self.hostname, dst_base=self.remote_base)
 
     def receive(self, rsync_items):
         self.sync_multiple(rsync_items, src_host=self.hostname, src_base=self.remote_base, dst_base=self.local_base)
```

### Comparing `cook_builder-0.1.1/cook/sync.py` & `cook_builder-0.1.2/cook/sync.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.1/cook_builder.egg-info/PKG-INFO` & `cook_builder-0.1.2/cook_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.1.1
+Version: 0.1.2
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cook_builder-0.1.1/pyproject.toml` & `cook_builder-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cook_builder"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
   "fabric==3.2.2",
   "rich==13.7.1",
 ]
 requires-python = ">=3.10"
 authors = [
   { name="Seweryn Rusecki" },
```

