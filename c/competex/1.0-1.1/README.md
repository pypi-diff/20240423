# Comparing `tmp/competex-1.0.tar.gz` & `tmp/competex-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "competex-1.0.tar", last modified: Mon Apr 22 15:12:28 2024, max compression
+gzip compressed data, was "competex-1.1.tar", last modified: Mon Apr 22 15:37:40 2024, max compression
```

## Comparing `competex-1.0.tar` & `competex-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-22 15:12:28.736705 competex-1.0/
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     1052 2024-04-21 20:35:54.000000 competex-1.0/LICENSE
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       25 2024-04-21 17:17:02.000000 competex-1.0/MANIFEST.in
--rw-r--r--   0 vaxraxd   (1000) vaxraxd   (1000)     2188 2024-04-22 15:12:28.736705 competex-1.0/PKG-INFO
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     1858 2024-04-22 04:26:58.000000 competex-1.0/README.md
-drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-22 15:12:28.736705 competex-1.0/competex/
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       22 2024-04-22 07:47:37.000000 competex-1.0/competex/__init__.py
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)    13411 2024-04-22 15:08:49.000000 competex-1.0/competex/main.py
-drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-22 15:12:28.736705 competex-1.0/competex.egg-info/
--rw-r--r--   0 vaxraxd   (1000) vaxraxd   (1000)     2188 2024-04-22 15:12:28.000000 competex-1.0/competex.egg-info/PKG-INFO
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)      210 2024-04-22 15:12:28.000000 competex-1.0/competex.egg-info/SOURCES.txt
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)        1 2024-04-22 15:12:28.000000 competex-1.0/competex.egg-info/dependency_links.txt
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)        9 2024-04-22 15:12:28.000000 competex-1.0/competex.egg-info/top_level.txt
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)      307 2024-04-22 15:12:01.000000 competex-1.0/pyproject.toml
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       38 2024-04-22 15:12:28.736705 competex-1.0/setup.cfg
+drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-22 15:37:40.713652 competex-1.1/
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     1052 2024-04-21 20:35:54.000000 competex-1.1/LICENSE
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       25 2024-04-21 17:17:02.000000 competex-1.1/MANIFEST.in
+-rw-r--r--   0 vaxraxd   (1000) vaxraxd   (1000)     2188 2024-04-22 15:37:40.713652 competex-1.1/PKG-INFO
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     1858 2024-04-22 04:26:58.000000 competex-1.1/README.md
+drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-22 15:37:40.713652 competex-1.1/competex/
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       22 2024-04-22 07:47:37.000000 competex-1.1/competex/__init__.py
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)    13414 2024-04-22 15:37:01.000000 competex-1.1/competex/main.py
+drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-22 15:37:40.713652 competex-1.1/competex.egg-info/
+-rw-r--r--   0 vaxraxd   (1000) vaxraxd   (1000)     2188 2024-04-22 15:37:40.000000 competex-1.1/competex.egg-info/PKG-INFO
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)      210 2024-04-22 15:37:40.000000 competex-1.1/competex.egg-info/SOURCES.txt
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)        1 2024-04-22 15:37:40.000000 competex-1.1/competex.egg-info/dependency_links.txt
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)        9 2024-04-22 15:37:40.000000 competex-1.1/competex.egg-info/top_level.txt
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)      307 2024-04-22 15:37:20.000000 competex-1.1/pyproject.toml
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       38 2024-04-22 15:37:40.713652 competex-1.1/setup.cfg
```

### Comparing `competex-1.0/LICENSE` & `competex-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `competex-1.0/PKG-INFO` & `competex-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: competex
-Version: 1.0
+Version: 1.1
 Author-email: Sike Brothers <sikebros@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `competex-1.0/README.md` & `competex-1.1/README.md`

 * *Files identical despite different names*

### Comparing `competex-1.0/competex/main.py` & `competex-1.1/competex/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,31 +409,30 @@
             edge_betweenness_centrality,
             eigenvector_centrality,
         ) = compute_centrality_measures(G)
         print("Degree Centrality:")
         for node, centrality in degree_centrality.items():
             print(f"Node {node}: {centrality}")
 
-        print("\nBetweenness Centrality:")
+        print("\\nBetweenness Centrality:")
         for node, centrality in betweenness_centrality.items():
             print(f"Node {node}: {centrality}")
 
-        print("\nEdge Betweenness Centrality:")
+        print("\\nEdge Betweenness Centrality:")
         for edge, centrality in edge_betweenness_centrality.items():
             print(f"Edge {edge}: {centrality}")
 
-        print("\nEigenvector Centrality:")
+        print("\\nEigenvector Centrality:")
         for node, centrality in eigenvector_centrality.items():
             print(f"Node {node}: {centrality}")
 
-        print("\nBridges:")
+        print("\\nBridges:")
         bridges = find_bridges(G)
         print(bridges)
 
-
     if __name__ == "__main__":
         main()
     '''
     
     fb_network='''
     1 4
     1 5
```

### Comparing `competex-1.0/competex.egg-info/PKG-INFO` & `competex-1.1/competex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: competex
-Version: 1.0
+Version: 1.1
 Author-email: Sike Brothers <sikebros@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

