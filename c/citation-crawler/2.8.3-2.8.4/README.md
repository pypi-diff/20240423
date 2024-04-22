# Comparing `tmp/citation_crawler-2.8.3.tar.gz` & `tmp/citation_crawler-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_crawler-2.8.3.tar", last modified: Mon Apr 15 01:11:18 2024, max compression
+gzip compressed data, was "citation_crawler-2.8.4.tar", last modified: Mon Apr 22 07:04:00 2024, max compression
```

## Comparing `citation_crawler-2.8.3.tar` & `citation_crawler-2.8.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:18.207524 citation_crawler-2.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-15 01:11:18.207524 citation_crawler-2.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:18.203524 citation_crawler-2.8.3/citation_crawler/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/arg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:18.207524 citation_crawler-2.8.3/citation_crawler/crawlers/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/crawlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/crawlers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/crawlers/ss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:18.207524 citation_crawler-2.8.3/citation_crawler/init/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/init/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:18.207524 citation_crawler-2.8.3/citation_crawler/summarizers/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/summarizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/summarizers/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/citation_crawler/summarizers/nx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:18.203524 citation_crawler-2.8.3/citation_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-15 01:11:17.000000 citation_crawler-2.8.3/citation_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 01:11:18.000000 citation_crawler-2.8.3/citation_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 01:11:17.000000 citation_crawler-2.8.3/citation_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 01:11:17.000000 citation_crawler-2.8.3/citation_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 01:11:17.000000 citation_crawler-2.8.3/citation_crawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 01:11:18.207524 citation_crawler-2.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-15 01:10:35.000000 citation_crawler-2.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:04:00.715383 citation_crawler-2.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-22 07:04:00.715383 citation_crawler-2.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:04:00.711383 citation_crawler-2.8.4/citation_crawler/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/arg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:04:00.711383 citation_crawler-2.8.4/citation_crawler/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/crawlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/crawlers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/crawlers/ss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:04:00.711383 citation_crawler-2.8.4/citation_crawler/init/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/init/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:04:00.715383 citation_crawler-2.8.4/citation_crawler/summarizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/summarizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/summarizers/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/citation_crawler/summarizers/nx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:04:00.711383 citation_crawler-2.8.4/citation_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-22 07:04:00.000000 citation_crawler-2.8.4/citation_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 07:04:00.000000 citation_crawler-2.8.4/citation_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 07:04:00.000000 citation_crawler-2.8.4/citation_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 07:04:00.000000 citation_crawler-2.8.4/citation_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 07:04:00.000000 citation_crawler-2.8.4/citation_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 07:04:00.715383 citation_crawler-2.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-22 07:03:53.000000 citation_crawler-2.8.4/setup.py
```

### Comparing `citation_crawler-2.8.3/LICENSE` & `citation_crawler-2.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.3/PKG-INFO` & `citation_crawler-2.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation_crawler
-Version: 2.8.3
+Version: 2.8.4
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citation_crawler-2.8.3/README.md` & `citation_crawler-2.8.4/README.md`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.3/citation_crawler/__main__.py` & `citation_crawler-2.8.4/citation_crawler/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,24 +108,25 @@
             yield paper
 
 
 parser_n4j = subparsers.add_parser('neo4j', help='Write result to neo4j database')
 parser_n4j.add_argument("--username", type=str, default=None, help=f'Auth username to neo4j database.')
 parser_n4j.add_argument("--password", type=str, default=None, help=f'Auth password to neo4j database.')
 parser_n4j.add_argument("--uri", type=str, required=True, help=f'URI to neo4j database.')
+parser_n4j.add_argument("--no-skip-exists", action="store_true", help=f'Do not skip exists references. Use it when you want to rewrite all papers.')
 
 
 async def func_parser_n4j_async(parser):
     from neo4j import AsyncGraphDatabase
     year, keywords, pid_list, aid_list, limit = func_parser(parser)
     args = parser.parse_args()
     logger.info(f"Specified uri and auth: {args.uri} {args.username} {'******' if args.password else 'none'}")
     async with AsyncGraphDatabase.driver(args.uri, auth=(args.username, args.password)) as driver:
         async with driver.session() as session:
-            summarizer = DefaultNeo4jSummarizer(session)
+            summarizer = DefaultNeo4jSummarizer(session, not args.no_skip_exists)
             crawler = DefaultSemanticScholarCrawler(
                 year, keywords,
                 aid_list,
                 paperId_list=pid_list, summarizer=summarizer
             )
             await bfs_to_end(crawler, limit)
```

### Comparing `citation_crawler-2.8.3/citation_crawler/arg.py` & `citation_crawler-2.8.4/citation_crawler/arg.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.3/citation_crawler/crawlers/common.py` & `citation_crawler-2.8.4/citation_crawler/crawlers/common.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.3/citation_crawler/crawlers/ss.py` & `citation_crawler-2.8.4/citation_crawler/crawlers/ss.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.3/citation_crawler/graph.py` & `citation_crawler-2.8.4/citation_crawler/graph.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.3/citation_crawler/init/neo4j.py` & `citation_crawler-2.8.4/citation_crawler/init/neo4j.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.3/citation_crawler/items.py` & `citation_crawler-2.8.4/citation_crawler/items.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.3/citation_crawler/summarizers/neo4j.py` & `citation_crawler-2.8.4/citation_crawler/summarizers/neo4j.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,49 +86,50 @@
     await tx.run("MERGE (p:Publication {title_hash: $title_hash}) " +
                  ('MERGE (a:Person {%s}) ' % (",".join([f'{k}: ${k}' for k in author_kv]))) +
                  (f'SET {",".join([f"a.{k}=${k}" for k in write_fields])}' if len(write_fields) > 0 else "") +
                  " MERGE (a)-[:WRITE]->(p)",
                  title_hash=paper.title_hash(), **write_fields)
 
 
-async def _add_references(tx, paper: Paper):
+async def _add_references(tx, paper: Paper, skip_exists=True):
     title_hash_exists = set([
         title_hash for (title_hash,) in
         await (await tx.run("MATCH (a:Publication)-[:CITE]->(p:Publication {title_hash: $title_hash}) RETURN a.title_hash",
                title_hash=paper.title_hash())).values()
     ])
     async for ref in paper.get_references():
-        if ref.title_hash() in title_hash_exists:
+        if skip_exists and ref.title_hash() in title_hash_exists:
             continue
         await add_paper(tx, ref)
         await add_reference(tx, paper, ref)
 
 
-async def _add_citations(tx, paper: Paper):
+async def _add_citations(tx, paper: Paper, skip_exists=True):
     title_hash_exists = set([
         title_hash for (title_hash,) in
         await (await tx.run("MATCH (p:Publication {title_hash: $title_hash})-[:CITE]->(a:Publication) RETURN a.title_hash",
                title_hash=paper.title_hash())).values()
     ])
     async for cit in paper.get_references():
-        if cit.title_hash() in title_hash_exists:
+        if skip_exists and cit.title_hash() in title_hash_exists:
             continue
         await add_paper(tx, cit)
         await add_reference(tx, cit, paper)
 
 
 class Neo4jSummarizer(Summarizer):
-    def __init__(self, session: AsyncSession, *args, **kwargs):
+    def __init__(self, session: AsyncSession, skip_exists=True, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.session = session
+        self.skip_exists = skip_exists
 
     async def write_paper(self, paper) -> None:
         await self.session.execute_write(add_paper, paper)
-        await self.session.execute_write(_add_references, paper)
-        await self.session.execute_write(_add_citations, paper)
+        await self.session.execute_write(_add_references, paper, self.skip_exists)
+        await self.session.execute_write(_add_citations, paper, self.skip_exists)
 
     async def write_reference(self, paper, reference) -> None:
         await self.session.execute_write(add_reference, paper, reference)
 
     async def get_corrlated_authors(self, paper: Paper) -> AsyncIterable[dict]:
         authors = set()
         for author in await self.session.execute_read(match_corrlated_authors, paper):
```

### Comparing `citation_crawler-2.8.3/citation_crawler/summarizers/nx.py` & `citation_crawler-2.8.4/citation_crawler/summarizers/nx.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.3/citation_crawler.egg-info/PKG-INFO` & `citation_crawler-2.8.4/citation_crawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-crawler
-Version: 2.8.3
+Version: 2.8.4
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citation_crawler-2.8.3/citation_crawler.egg-info/SOURCES.txt` & `citation_crawler-2.8.4/citation_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.8.3/setup.py` & `citation_crawler-2.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'citation_crawler.crawlers': 'citation_crawler/crawlers',
     'citation_crawler.summarizers': 'citation_crawler/summarizers',
     'citation_crawler.init': 'citation_crawler/init',
 }
 
 setup(
     name='citation_crawler',
-    version='2.8.3',
+    version='2.8.4',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/citation-crawler',
     description=u'Asynchronous high-concurrency citation crawler, use with caution!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

