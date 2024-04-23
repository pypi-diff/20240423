# Comparing `tmp/citation-rabbot-3.9.tar.gz` & `tmp/citation-rabbot-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation-rabbot-3.9.tar", last modified: Fri Dec 15 06:39:33 2023, max compression
+gzip compressed data, was "citation-rabbot-3.9.1.tar", last modified: Sat Dec 16 22:38:56 2023, max compression
```

## Comparing `citation-rabbot-3.9.tar` & `citation-rabbot-3.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:39:33.390508 citation-rabbot-3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-15 06:39:25.000000 citation-rabbot-3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-12-15 06:39:33.390508 citation-rabbot-3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-15 06:39:25.000000 citation-rabbot-3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:39:33.390508 citation-rabbot-3.9/citation_rabbot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 06:39:25.000000 citation-rabbot-3.9/citation_rabbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2023-12-15 06:39:25.000000 citation-rabbot-3.9/citation_rabbot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-12-15 06:39:25.000000 citation-rabbot-3.9/citation_rabbot/arg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:39:33.390508 citation-rabbot-3.9/citation_rabbot/jumps/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-15 06:39:25.000000 citation-rabbot-3.9/citation_rabbot/jumps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2023-12-15 06:39:25.000000 citation-rabbot-3.9/citation_rabbot/jumps/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-12-15 06:39:25.000000 citation-rabbot-3.9/citation_rabbot/jumps/papers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2023-12-15 06:39:25.000000 citation-rabbot-3.9/citation_rabbot/jumps/papers_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2023-12-15 06:39:25.000000 citation-rabbot-3.9/citation_rabbot/jumps/papers_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2023-12-15 06:39:25.000000 citation-rabbot-3.9/citation_rabbot/jumps/papers_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-15 06:39:25.000000 citation-rabbot-3.9/citation_rabbot/jumps/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2023-12-15 06:39:25.000000 citation-rabbot-3.9/citation_rabbot/rabbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-12-15 06:39:25.000000 citation-rabbot-3.9/citation_rabbot/start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:39:33.390508 citation-rabbot-3.9/citation_rabbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-12-15 06:39:33.000000 citation-rabbot-3.9/citation_rabbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-15 06:39:33.000000 citation-rabbot-3.9/citation_rabbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 06:39:33.000000 citation-rabbot-3.9/citation_rabbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-15 06:39:33.000000 citation-rabbot-3.9/citation_rabbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-15 06:39:33.000000 citation-rabbot-3.9/citation_rabbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-15 06:39:33.390508 citation-rabbot-3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-12-15 06:39:25.000000 citation-rabbot-3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 22:38:56.569542 citation-rabbot-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2023-12-16 22:38:56.569542 citation-rabbot-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 22:38:56.569542 citation-rabbot-3.9.1/citation_rabbot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/citation_rabbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/citation_rabbot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/citation_rabbot/arg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 22:38:56.569542 citation-rabbot-3.9.1/citation_rabbot/jumps/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/citation_rabbot/jumps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/citation_rabbot/jumps/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/citation_rabbot/jumps/papers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/citation_rabbot/jumps/papers_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/citation_rabbot/jumps/papers_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/citation_rabbot/jumps/papers_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/citation_rabbot/jumps/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/citation_rabbot/rabbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/citation_rabbot/start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 22:38:56.569542 citation-rabbot-3.9.1/citation_rabbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2023-12-16 22:38:56.000000 citation-rabbot-3.9.1/citation_rabbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-16 22:38:56.000000 citation-rabbot-3.9.1/citation_rabbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 22:38:56.000000 citation-rabbot-3.9.1/citation_rabbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-16 22:38:56.000000 citation-rabbot-3.9.1/citation_rabbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-16 22:38:56.000000 citation-rabbot-3.9.1/citation_rabbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 22:38:56.569542 citation-rabbot-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-16 22:38:44.000000 citation-rabbot-3.9.1/setup.py
```

### Comparing `citation-rabbot-3.9/LICENSE` & `citation-rabbot-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `citation-rabbot-3.9/PKG-INFO` & `citation-rabbot-3.9.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-rabbot
-Version: 3.9
+Version: 3.9.1
 Summary: A telegram bot jumping in your citation database like a rabbit!
 Home-page: https://github.com/yindaheng98/citation-rabbot
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citation-rabbot-3.9/citation_rabbot/__main__.py` & `citation-rabbot-3.9.1/citation_rabbot/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 logging.basicConfig(
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
     level=logging.INFO
 )
 
 parser = argparse.ArgumentParser()
 
-parser.add_argument("--auth", type=str, default=None, help=f'Auth to neo4j database.')
+parser.add_argument("--username", type=str, default=None, help=f'Auth username to neo4j database.')
+parser.add_argument("--password", type=str, default=None, help=f'Auth password to neo4j database.')
 parser.add_argument("--uri", type=str, required=True, help=f'URI to neo4j database.')
 parser.add_argument("--token", type=str, required=True, help=f'Telegram bot token.')
 add_argument_jump(parser, defaults_desc=defaults_desc)
 
 
 args = parser.parse_args()
 jump_list = parse_args_jump(parser)
@@ -43,14 +44,14 @@
         desc_order.append(name)
 
 
 async def post_init(application: Application):
     await application.bot.set_my_commands([('start', "Let's jump!")])
 application = ApplicationBuilder().token(args.token).post_init(post_init).build()
 
-with GraphDatabase.driver(args.uri, auth=args.auth) as driver:
+with GraphDatabase.driver(args.uri, auth=(args.username, args.password)) as driver:
     with driver.session() as session:
         rabbot = Rabbot(app=application, session=session)
         for name, (parser, message2query, result2message) in jump_dict.items():
             rabbot.add_jump(name, parser, message2query, result2message)
         rabbot.add_jump('start', None, start_args2querys, gen_start_results2message(desc_order, desc_dict))
         application.run_polling()
```

### Comparing `citation-rabbot-3.9/citation_rabbot/arg.py` & `citation-rabbot-3.9.1/citation_rabbot/arg.py`

 * *Files identical despite different names*

### Comparing `citation-rabbot-3.9/citation_rabbot/jumps/detail.py` & `citation-rabbot-3.9.1/citation_rabbot/jumps/detail.py`

 * *Files identical despite different names*

### Comparing `citation-rabbot-3.9/citation_rabbot/jumps/papers.py` & `citation-rabbot-3.9.1/citation_rabbot/jumps/papers.py`

 * *Files identical despite different names*

### Comparing `citation-rabbot-3.9/citation_rabbot/jumps/papers_args.py` & `citation-rabbot-3.9.1/citation_rabbot/jumps/papers_args.py`

 * *Files identical despite different names*

### Comparing `citation-rabbot-3.9/citation_rabbot/jumps/papers_display.py` & `citation-rabbot-3.9.1/citation_rabbot/jumps/papers_display.py`

 * *Files identical despite different names*

### Comparing `citation-rabbot-3.9/citation_rabbot/jumps/papers_query.py` & `citation-rabbot-3.9.1/citation_rabbot/jumps/papers_query.py`

 * *Files identical despite different names*

### Comparing `citation-rabbot-3.9/citation_rabbot/jumps/search.py` & `citation-rabbot-3.9.1/citation_rabbot/jumps/search.py`

 * *Files identical despite different names*

### Comparing `citation-rabbot-3.9/citation_rabbot/rabbot.py` & `citation-rabbot-3.9.1/citation_rabbot/rabbot.py`

 * *Files identical despite different names*

### Comparing `citation-rabbot-3.9/citation_rabbot/start.py` & `citation-rabbot-3.9.1/citation_rabbot/start.py`

 * *Files identical despite different names*

### Comparing `citation-rabbot-3.9/citation_rabbot.egg-info/PKG-INFO` & `citation-rabbot-3.9.1/citation_rabbot.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-rabbot
-Version: 3.9
+Version: 3.9.1
 Summary: A telegram bot jumping in your citation database like a rabbit!
 Home-page: https://github.com/yindaheng98/citation-rabbot
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citation-rabbot-3.9/citation_rabbot.egg-info/SOURCES.txt` & `citation-rabbot-3.9.1/citation_rabbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citation-rabbot-3.9/setup.py` & `citation-rabbot-3.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 package_dir = {
     'citation_rabbot': 'citation_rabbot',
     'citation_rabbot.jumps': 'citation_rabbot/jumps'
 }
 
 setup(
     name='citation-rabbot',
-    version='3.9',
+    version='3.9.1',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/citation-rabbot',
     description=u'A telegram bot jumping in your citation database like a rabbit!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

