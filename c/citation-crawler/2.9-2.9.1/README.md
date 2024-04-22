# Comparing `tmp/citation_crawler-2.9.tar.gz` & `tmp/citation_crawler-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_crawler-2.9.tar", last modified: Mon Apr 22 22:27:52 2024, max compression
+gzip compressed data, was "citation_crawler-2.9.1.tar", last modified: Mon Apr 22 22:42:53 2024, max compression
```

## Comparing `citation_crawler-2.9.tar` & `citation_crawler-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:27:52.251619 citation_crawler-2.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 22:27:44.000000 citation_crawler-2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-04-22 22:27:52.251619 citation_crawler-2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-22 22:27:44.000000 citation_crawler-2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:27:52.247619 citation_crawler-2.9/citation_crawler/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/arg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:27:52.251619 citation_crawler-2.9/citation_crawler/crawlers/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/crawlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/crawlers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/crawlers/ss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:27:52.251619 citation_crawler-2.9/citation_crawler/init/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/init/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:27:52.251619 citation_crawler-2.9/citation_crawler/summarizers/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/summarizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/summarizers/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 22:27:44.000000 citation_crawler-2.9/citation_crawler/summarizers/nx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:27:52.247619 citation_crawler-2.9/citation_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-04-22 22:27:52.000000 citation_crawler-2.9/citation_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 22:27:52.000000 citation_crawler-2.9/citation_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:27:52.000000 citation_crawler-2.9/citation_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 22:27:52.000000 citation_crawler-2.9/citation_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 22:27:52.000000 citation_crawler-2.9/citation_crawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:27:52.251619 citation_crawler-2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-22 22:27:44.000000 citation_crawler-2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/citation_crawler/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/arg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/citation_crawler/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/crawlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/crawlers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/crawlers/ss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/citation_crawler/init/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/init/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/citation_crawler/summarizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/summarizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/summarizers/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/citation_crawler/summarizers/nx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/citation_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-22 22:42:53.000000 citation_crawler-2.9.1/citation_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 22:42:53.000000 citation_crawler-2.9.1/citation_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:42:53.000000 citation_crawler-2.9.1/citation_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 22:42:53.000000 citation_crawler-2.9.1/citation_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 22:42:53.000000 citation_crawler-2.9.1/citation_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:42:53.741102 citation_crawler-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-22 22:42:45.000000 citation_crawler-2.9.1/setup.py
```

### Comparing `citation_crawler-2.9/LICENSE` & `citation_crawler-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9/PKG-INFO` & `citation_crawler-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation_crawler
-Version: 2.9
+Version: 2.9.1
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -103,15 +103,18 @@
 * `HTTP_TIMEOUT`
   * Timeout for each http request, in seconds
 * `HTTP_CONCORRENT`
   * Concurrent HTTP requests
   * default: `8`
 * `HTTP_HEADERS`
   * Headers for HTTP requests
-  * default: None
+  * default: `None`
+* `HTTP_SLEEP`
+  * Sleep after request (in seconds)
+  * default: `0`
 
 ### Write to a JSON file
 
 e.g. write to `summary.json`:
 
 ```sh
 python -m citation_crawler -k video -k edge -p 27d5dc70280c8628f181a7f8881912025f808256 -a 1681457 networkx --dest summary.json
```

### Comparing `citation_crawler-2.9/README.md` & `citation_crawler-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -222,174 +222,178 @@
 00000dd0: 5252 454e 5460 0a20 202a 2043 6f6e 6375  RRENT`.  * Concu
 00000de0: 7272 656e 7420 4854 5450 2072 6571 7565  rrent HTTP reque
 00000df0: 7374 730a 2020 2a20 6465 6661 756c 743a  sts.  * default:
 00000e00: 2060 3860 0a2a 2060 4854 5450 5f48 4541   `8`.* `HTTP_HEA
 00000e10: 4445 5253 600a 2020 2a20 4865 6164 6572  DERS`.  * Header
 00000e20: 7320 666f 7220 4854 5450 2072 6571 7565  s for HTTP reque
 00000e30: 7374 730a 2020 2a20 6465 6661 756c 743a  sts.  * default:
-00000e40: 204e 6f6e 650a 0a23 2323 2057 7269 7465   None..### Write
-00000e50: 2074 6f20 6120 4a53 4f4e 2066 696c 650a   to a JSON file.
-00000e60: 0a65 2e67 2e20 7772 6974 6520 746f 2060  .e.g. write to `
-00000e70: 7375 6d6d 6172 792e 6a73 6f6e 603a 0a0a  summary.json`:..
-00000e80: 6060 6073 680a 7079 7468 6f6e 202d 6d20  ```sh.python -m 
-00000e90: 6369 7461 7469 6f6e 5f63 7261 776c 6572  citation_crawler
-00000ea0: 202d 6b20 7669 6465 6f20 2d6b 2065 6467   -k video -k edg
-00000eb0: 6520 2d70 2032 3764 3564 6337 3032 3830  e -p 27d5dc70280
-00000ec0: 6338 3632 3866 3138 3161 3766 3838 3831  c8628f181a7f8881
-00000ed0: 3931 3230 3235 6638 3038 3235 3620 2d61  912025f808256 -a
-00000ee0: 2031 3638 3134 3537 206e 6574 776f 726b   1681457 network
-00000ef0: 7820 2d2d 6465 7374 2073 756d 6d61 7279  x --dest summary
-00000f00: 2e6a 736f 6e0a 6060 600a 0a23 2323 2320  .json.```..#### 
-00000f10: 4a53 4f4e 2066 6f72 6d61 740a 0a60 6060  JSON format..```
-00000f20: 6a73 6f6e 0a7b 0a20 2022 6e6f 6465 7322  json.{.  "nodes"
-00000f30: 3a20 7b0a 2020 2020 223c 7061 7065 7249  : {.    "<paperI
-00000f40: 6420 6f66 2061 2070 6170 6572 2069 6e20  d of a paper in 
-00000f50: 5365 6d61 6e74 6963 2053 6368 6f6c 6172  Semantic Scholar
-00000f60: 3e22 3a20 7b0a 2020 2020 2020 2270 6170  >": {.      "pap
-00000f70: 6572 4964 223a 2022 3c70 6170 6572 4964  erId": "<paperId
-00000f80: 206f 6620 7468 6973 2070 6170 6572 2069   of this paper i
-00000f90: 6e20 5365 6d61 6e74 6963 2053 6368 6f6c  n Semantic Schol
-00000fa0: 6172 3e22 2c0a 2020 2020 2020 2264 626c  ar>",.      "dbl
-00000fb0: 705f 6b65 7922 3a20 223c 6462 6c70 2069  p_key": "<dblp i
-00000fc0: 6420 6f66 2074 6869 7320 7061 7065 723e  d of this paper>
-00000fd0: 222c 0a20 2020 2020 2022 7469 746c 6522  ",.      "title"
-00000fe0: 3a20 223c 7469 746c 6520 6f66 2074 6869  : "<title of thi
-00000ff0: 7320 7061 7065 723e 222c 0a20 2020 2020  s paper>",.     
-00001000: 2022 7965 6172 223a 2022 696e 7420 3c70   "year": "int <p
-00001010: 7562 6c69 7368 2079 6561 7220 6f66 2074  ublish year of t
-00001020: 6869 7320 7061 7065 723e 222c 0a20 2020  his paper>",.   
-00001030: 2020 2022 646f 6922 3a20 223c 646f 6920     "doi": "<doi 
-00001040: 6f66 2074 6869 7320 7061 7065 723e 222c  of this paper>",
-00001050: 0a20 2020 2020 2022 6175 7468 6f72 7322  .      "authors"
-00001060: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
-00001070: 2020 2020 2020 2020 2261 7574 686f 7249          "authorI
-00001080: 6422 3a20 223c 6175 7468 6f72 4964 206f  d": "<authorId o
-00001090: 6620 7468 6973 2070 6572 736f 6e20 696e  f this person in
-000010a0: 2053 656d 616e 7469 6320 5363 686f 6c61   Semantic Schola
-000010b0: 723e 222c 0a20 2020 2020 2020 2020 2022  r>",.          "
-000010c0: 6e61 6d65 223a 2022 3c6e 616d 6520 6f66  name": "<name of
-000010d0: 2074 6869 7320 7065 7273 6f6e 3e22 2c0a   this person>",.
-000010e0: 2020 2020 2020 2020 2020 2264 626c 705f            "dblp_
-000010f0: 6e61 6d65 223a 205b 0a20 2020 2020 2020  name": [.       
-00001100: 2020 2020 2022 3c64 6973 616d 6269 6775       "<disambigu
-00001110: 6174 696f 6e20 6e61 6d65 206f 6620 7468  ation name of th
-00001120: 6973 2070 6572 736f 6e20 696e 2064 626c  is person in dbl
-00001130: 703e 222c 0a20 2020 2020 2020 2020 2020  p>",.           
-00001140: 2022 3c64 6973 616d 6269 6775 6174 696f   "<disambiguatio
-00001150: 6e20 6e61 6d65 206f 6620 7468 6973 2070  n name of this p
-00001160: 6572 736f 6e20 696e 2064 626c 703e 222c  erson in dblp>",
-00001170: 0a20 2020 2020 2020 2020 2020 2022 3c64  .            "<d
-00001180: 6973 616d 6269 6775 6174 696f 6e20 6e61  isambiguation na
-00001190: 6d65 206f 6620 7468 6973 2070 6572 736f  me of this perso
-000011a0: 6e20 696e 2064 626c 703e 222c 0a20 2020  n in dblp>",.   
-000011b0: 2020 2020 2020 2020 2022 2e2e 2e2e 2e2e           "......
-000011c0: 220a 2020 2020 2020 2020 2020 5d0a 2020  ".          ].  
-000011d0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000011e0: 207b 202e 2e2e 2e2e 2e20 7d2c 0a20 2020   { ...... },.   
-000011f0: 2020 2020 207b 202e 2e2e 2e2e 2e20 7d2c       { ...... },
-00001200: 0a20 2020 2020 2020 202e 2e2e 2e2e 2e0a  .        .......
-00001210: 2020 2020 2020 5d0a 2020 2020 7d2c 0a20        ].    },. 
-00001220: 2020 2022 3c70 6170 6572 4964 206f 6620     "<paperId of 
-00001230: 6120 7061 7065 7220 696e 2053 656d 616e  a paper in Seman
-00001240: 7469 6320 5363 686f 6c61 723e 223a 207b  tic Scholar>": {
-00001250: 202e 2e2e 2e2e 2e20 7d2c 0a20 2020 2022   ...... },.    "
-00001260: 3c70 6170 6572 4964 206f 6620 6120 7061  <paperId of a pa
-00001270: 7065 7220 696e 2053 656d 616e 7469 6320  per in Semantic 
-00001280: 5363 686f 6c61 723e 223a 207b 202e 2e2e  Scholar>": { ...
-00001290: 2e2e 2e20 7d2c 0a20 2020 202e 2e2e 2e2e  ... },.    .....
-000012a0: 2e0a 2020 7d2c 0a20 2022 6564 6765 7322  ..  },.  "edges"
-000012b0: 3a20 5b0a 2020 2020 5b0a 2020 2020 2020  : [.    [.      
-000012c0: 2020 223c 7061 7065 7249 6420 6f66 2061    "<paperId of a
-000012d0: 2070 6170 6572 2069 6e20 5365 6d61 6e74   paper in Semant
-000012e0: 6963 2053 6368 6f6c 6172 3e22 2c0a 2020  ic Scholar>",.  
-000012f0: 2020 2020 2020 223c 7061 7065 7249 6420        "<paperId 
-00001300: 6f66 2061 2072 6566 6572 656e 6365 2069  of a reference i
-00001310: 6e20 7468 6520 6162 6f76 6520 7061 7065  n the above pape
-00001320: 723e 220a 2020 2020 5d2c 0a20 2020 205b  r>".    ],.    [
-00001330: 202e 2e2e 2e2e 2e20 5d2c 0a20 2020 205b   ...... ],.    [
-00001340: 202e 2e2e 2e2e 2e20 5d2c 0a20 2020 202e   ...... ],.    .
-00001350: 2e2e 2e2e 2e0a 2020 5d0a 6060 600a 0a23  ......  ].```..#
-00001360: 2323 2057 7269 7465 2074 6f20 6120 4e65  ## Write to a Ne
-00001370: 6f34 4a20 6461 7461 6261 7365 0a0a 6060  o4J database..``
-00001380: 6073 680a 646f 636b 6572 2070 756c 6c20  `sh.docker pull 
-00001390: 6e65 6f34 6a0a 646f 636b 6572 2072 756e  neo4j.docker run
-000013a0: 202d 2d72 6d20 2d69 7420 2d70 2037 3437   --rm -it -p 747
-000013b0: 343a 3734 3734 202d 7020 3736 3837 3a37  4:7474 -p 7687:7
-000013c0: 3638 3720 2d76 2024 2870 7764 2973 6176  687 -v $(pwd)sav
-000013d0: 652f 6e65 6f34 6a3a 2f64 6174 6120 2d65  e/neo4j:/data -e
-000013e0: 204e 454f 344a 5f41 5554 483d 6e6f 6e65   NEO4J_AUTH=none
-000013f0: 206e 656f 346a 0a60 6060 0a0a 652e 672e   neo4j.```..e.g.
-00001400: 2077 7269 7465 2074 6f20 606e 656f 346a   write to `neo4j
-00001410: 3a2f 2f6c 6f63 616c 686f 7374 3a37 3638  ://localhost:768
-00001420: 3760 3a0a 0a60 6060 7368 0a70 7974 686f  7`:..```sh.pytho
-00001430: 6e20 2d6d 2064 626c 705f 6372 6177 6c65  n -m dblp_crawle
-00001440: 7220 2d6b 2076 6964 656f 202d 6b20 6564  r -k video -k ed
-00001450: 6765 202d 7020 3237 6435 6463 3730 3238  ge -p 27d5dc7028
-00001460: 3063 3836 3238 6631 3831 6137 6638 3838  0c8628f181a7f888
-00001470: 3139 3132 3032 3566 3830 3832 3536 202d  1912025f808256 -
-00001480: 6120 3136 3831 3435 3720 6e65 6f34 6a20  a 1681457 neo4j 
-00001490: 2d2d 7572 6920 6e65 6f34 6a3a 2f2f 6c6f  --uri neo4j://lo
-000014a0: 6361 6c68 6f73 743a 3736 3837 0a60 6060  calhost:7687.```
-000014b0: 0a0a 2323 2323 2054 6970 730a 0a57 6974  ..#### Tips..Wit
-000014c0: 686f 7574 2069 6e64 6578 2c20 4e45 4f34  hout index, NEO4
-000014d0: 4a20 7175 6572 7920 7769 6c6c 2062 6520  J query will be 
-000014e0: 7665 7279 2076 6572 7920 736c 6f77 2e20  very very slow. 
-000014f0: 536f 2062 6566 6f72 6520 796f 7520 7374  So before you st
-00001500: 6172 742c 2079 6f75 2073 686f 756c 6420  art, you should 
-00001510: 6164 6420 736f 6d65 2069 6e64 6578 3a0a  add some index:.
-00001520: 0a60 6060 6371 6c0a 4352 4541 5445 2049  .```cql.CREATE I
-00001530: 4e44 4558 2070 7562 6c69 6361 7469 6f6e  NDEX publication
-00001540: 5f74 6974 6c65 5f68 6173 685f 696e 6465  _title_hash_inde
-00001550: 7820 464f 5220 2870 3a50 7562 6c69 6361  x FOR (p:Publica
-00001560: 7469 6f6e 2920 4f4e 2028 702e 7469 746c  tion) ON (p.titl
-00001570: 655f 6861 7368 293b 0a43 5245 4154 4520  e_hash);.CREATE 
-00001580: 494e 4445 5820 7075 626c 6963 6174 696f  INDEX publicatio
-00001590: 6e5f 6462 6c70 5f6b 6579 5f69 6e64 6578  n_dblp_key_index
-000015a0: 2046 4f52 2028 703a 5075 626c 6963 6174   FOR (p:Publicat
-000015b0: 696f 6e29 204f 4e20 2870 2e64 626c 705f  ion) ON (p.dblp_
-000015c0: 6b65 7929 3b0a 4352 4541 5445 2049 4e44  key);.CREATE IND
-000015d0: 4558 2070 7562 6c69 6361 7469 6f6e 5f70  EX publication_p
-000015e0: 6170 6572 5f69 645f 696e 6465 7820 464f  aper_id_index FO
-000015f0: 5220 2870 3a50 7562 6c69 6361 7469 6f6e  R (p:Publication
-00001600: 2920 4f4e 2028 702e 7061 7065 7249 6429  ) ON (p.paperId)
-00001610: 3b0a 4352 4541 5445 2049 4e44 4558 2070  ;.CREATE INDEX p
-00001620: 6572 736f 6e5f 6175 7468 6f72 5f69 645f  erson_author_id_
-00001630: 696e 6465 7820 464f 5220 2870 3a50 6572  index FOR (p:Per
-00001640: 736f 6e29 204f 4e20 2870 2e61 7574 686f  son) ON (p.autho
-00001650: 7249 6429 3b0a 4352 4541 5445 2049 4e44  rId);.CREATE IND
-00001660: 4558 2070 6572 736f 6e5f 6462 6c70 5f70  EX person_dblp_p
-00001670: 6964 5f69 6e64 6578 2046 4f52 2028 703a  id_index FOR (p:
-00001680: 5065 7273 6f6e 2920 4f4e 2028 702e 6462  Person) ON (p.db
-00001690: 6c70 5f70 6964 293b 0a60 6060 0a0a 2323  lp_pid);.```..##
-000016a0: 2320 4765 7420 696e 6974 6961 6c20 7061  # Get initial pa
-000016b0: 7065 7220 6c69 7374 206f 7220 6175 7468  per list or auth
-000016c0: 6f72 206c 6973 7420 6672 6f6d 2061 204e  or list from a N
-000016d0: 656f 344a 2064 6174 6162 6173 650a 0a60  eo4J database..`
-000016e0: 6060 7368 0a70 7974 686f 6e20 2d6d 2064  ``sh.python -m d
-000016f0: 626c 705f 6372 6177 6c65 7220 2d6b 2076  blp_crawler -k v
-00001700: 6964 656f 202d 6b20 6564 6765 202d 6120  ideo -k edge -a 
-00001710: 2269 6d70 6f72 746c 6962 2e69 6d70 6f72  "importlib.impor
-00001720: 745f 6d6f 6475 6c65 2827 6369 7461 7469  t_module('citati
-00001730: 6f6e 5f63 7261 776c 6572 2e69 6e69 7427  on_crawler.init'
-00001740: 292e 7061 7065 7273 5f69 6e5f 6e65 6f34  ).papers_in_neo4
-00001750: 6a28 276e 656f 346a 3a2f 2f6c 6f63 616c  j('neo4j://local
-00001760: 686f 7374 3a37 3638 3727 2922 206e 656f  host:7687')" neo
-00001770: 346a 202d 2d75 7269 206e 656f 346a 3a2f  4j --uri neo4j:/
-00001780: 2f6c 6f63 616c 686f 7374 3a37 3638 370a  /localhost:7687.
-00001790: 6060 600a 0a60 6060 7368 0a70 7974 686f  ```..```sh.pytho
-000017a0: 6e20 2d6d 2064 626c 705f 6372 6177 6c65  n -m dblp_crawle
-000017b0: 7220 2d6b 2076 6964 656f 202d 6b20 6564  r -k video -k ed
-000017c0: 6765 202d 7020 2269 6d70 6f72 746c 6962  ge -p "importlib
-000017d0: 2e69 6d70 6f72 745f 6d6f 6475 6c65 2827  .import_module('
-000017e0: 6369 7461 7469 6f6e 5f63 7261 776c 6572  citation_crawler
-000017f0: 2e69 6e69 7427 292e 6175 7468 6f72 735f  .init').authors_
-00001800: 696e 5f6e 656f 346a 2827 6e65 6f34 6a3a  in_neo4j('neo4j:
-00001810: 2f2f 6c6f 6361 6c68 6f73 743a 3736 3837  //localhost:7687
-00001820: 2729 2220 6e65 6f34 6a20 2d2d 7572 6920  ')" neo4j --uri 
-00001830: 6e65 6f34 6a3a 2f2f 6c6f 6361 6c68 6f73  neo4j://localhos
-00001840: 743a 3736 3837 0a60 6060 0a0a 6069 6d70  t:7687.```..`imp
-00001850: 6f72 746c 6962 2e69 6d70 6f72 745f 6d6f  ortlib.import_mo
-00001860: 6475 6c65 6020 6973 2066 6c65 7869 626c  dule` is flexibl
-00001870: 652c 2079 6f75 2063 616e 2069 6d70 6f72  e, you can impor
-00001880: 7420 796f 7572 206f 776e 2076 6172 6961  t your own varia
-00001890: 626c 6573 2074 6872 6f75 6768 2074 6869  bles through thi
-000018a0: 732e 0a                                  s..
+00000e40: 2060 4e6f 6e65 600a 2a20 6048 5454 505f   `None`.* `HTTP_
+00000e50: 534c 4545 5060 0a20 202a 2053 6c65 6570  SLEEP`.  * Sleep
+00000e60: 2061 6674 6572 2072 6571 7565 7374 2028   after request (
+00000e70: 696e 2073 6563 6f6e 6473 290a 2020 2a20  in seconds).  * 
+00000e80: 6465 6661 756c 743a 2060 3060 0a0a 2323  default: `0`..##
+00000e90: 2320 5772 6974 6520 746f 2061 204a 534f  # Write to a JSO
+00000ea0: 4e20 6669 6c65 0a0a 652e 672e 2077 7269  N file..e.g. wri
+00000eb0: 7465 2074 6f20 6073 756d 6d61 7279 2e6a  te to `summary.j
+00000ec0: 736f 6e60 3a0a 0a60 6060 7368 0a70 7974  son`:..```sh.pyt
+00000ed0: 686f 6e20 2d6d 2063 6974 6174 696f 6e5f  hon -m citation_
+00000ee0: 6372 6177 6c65 7220 2d6b 2076 6964 656f  crawler -k video
+00000ef0: 202d 6b20 6564 6765 202d 7020 3237 6435   -k edge -p 27d5
+00000f00: 6463 3730 3238 3063 3836 3238 6631 3831  dc70280c8628f181
+00000f10: 6137 6638 3838 3139 3132 3032 3566 3830  a7f8881912025f80
+00000f20: 3832 3536 202d 6120 3136 3831 3435 3720  8256 -a 1681457 
+00000f30: 6e65 7477 6f72 6b78 202d 2d64 6573 7420  networkx --dest 
+00000f40: 7375 6d6d 6172 792e 6a73 6f6e 0a60 6060  summary.json.```
+00000f50: 0a0a 2323 2323 204a 534f 4e20 666f 726d  ..#### JSON form
+00000f60: 6174 0a0a 6060 606a 736f 6e0a 7b0a 2020  at..```json.{.  
+00000f70: 226e 6f64 6573 223a 207b 0a20 2020 2022  "nodes": {.    "
+00000f80: 3c70 6170 6572 4964 206f 6620 6120 7061  <paperId of a pa
+00000f90: 7065 7220 696e 2053 656d 616e 7469 6320  per in Semantic 
+00000fa0: 5363 686f 6c61 723e 223a 207b 0a20 2020  Scholar>": {.   
+00000fb0: 2020 2022 7061 7065 7249 6422 3a20 223c     "paperId": "<
+00000fc0: 7061 7065 7249 6420 6f66 2074 6869 7320  paperId of this 
+00000fd0: 7061 7065 7220 696e 2053 656d 616e 7469  paper in Semanti
+00000fe0: 6320 5363 686f 6c61 723e 222c 0a20 2020  c Scholar>",.   
+00000ff0: 2020 2022 6462 6c70 5f6b 6579 223a 2022     "dblp_key": "
+00001000: 3c64 626c 7020 6964 206f 6620 7468 6973  <dblp id of this
+00001010: 2070 6170 6572 3e22 2c0a 2020 2020 2020   paper>",.      
+00001020: 2274 6974 6c65 223a 2022 3c74 6974 6c65  "title": "<title
+00001030: 206f 6620 7468 6973 2070 6170 6572 3e22   of this paper>"
+00001040: 2c0a 2020 2020 2020 2279 6561 7222 3a20  ,.      "year": 
+00001050: 2269 6e74 203c 7075 626c 6973 6820 7965  "int <publish ye
+00001060: 6172 206f 6620 7468 6973 2070 6170 6572  ar of this paper
+00001070: 3e22 2c0a 2020 2020 2020 2264 6f69 223a  >",.      "doi":
+00001080: 2022 3c64 6f69 206f 6620 7468 6973 2070   "<doi of this p
+00001090: 6170 6572 3e22 2c0a 2020 2020 2020 2261  aper>",.      "a
+000010a0: 7574 686f 7273 223a 205b 0a20 2020 2020  uthors": [.     
+000010b0: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+000010c0: 6175 7468 6f72 4964 223a 2022 3c61 7574  authorId": "<aut
+000010d0: 686f 7249 6420 6f66 2074 6869 7320 7065  horId of this pe
+000010e0: 7273 6f6e 2069 6e20 5365 6d61 6e74 6963  rson in Semantic
+000010f0: 2053 6368 6f6c 6172 3e22 2c0a 2020 2020   Scholar>",.    
+00001100: 2020 2020 2020 226e 616d 6522 3a20 223c        "name": "<
+00001110: 6e61 6d65 206f 6620 7468 6973 2070 6572  name of this per
+00001120: 736f 6e3e 222c 0a20 2020 2020 2020 2020  son>",.         
+00001130: 2022 6462 6c70 5f6e 616d 6522 3a20 5b0a   "dblp_name": [.
+00001140: 2020 2020 2020 2020 2020 2020 223c 6469              "<di
+00001150: 7361 6d62 6967 7561 7469 6f6e 206e 616d  sambiguation nam
+00001160: 6520 6f66 2074 6869 7320 7065 7273 6f6e  e of this person
+00001170: 2069 6e20 6462 6c70 3e22 2c0a 2020 2020   in dblp>",.    
+00001180: 2020 2020 2020 2020 223c 6469 7361 6d62          "<disamb
+00001190: 6967 7561 7469 6f6e 206e 616d 6520 6f66  iguation name of
+000011a0: 2074 6869 7320 7065 7273 6f6e 2069 6e20   this person in 
+000011b0: 6462 6c70 3e22 2c0a 2020 2020 2020 2020  dblp>",.        
+000011c0: 2020 2020 223c 6469 7361 6d62 6967 7561      "<disambigua
+000011d0: 7469 6f6e 206e 616d 6520 6f66 2074 6869  tion name of thi
+000011e0: 7320 7065 7273 6f6e 2069 6e20 6462 6c70  s person in dblp
+000011f0: 3e22 2c0a 2020 2020 2020 2020 2020 2020  >",.            
+00001200: 222e 2e2e 2e2e 2e22 0a20 2020 2020 2020  "......".       
+00001210: 2020 205d 0a20 2020 2020 2020 207d 2c0a     ].        },.
+00001220: 2020 2020 2020 2020 7b20 2e2e 2e2e 2e2e          { ......
+00001230: 207d 2c0a 2020 2020 2020 2020 7b20 2e2e   },.        { ..
+00001240: 2e2e 2e2e 207d 2c0a 2020 2020 2020 2020  .... },.        
+00001250: 2e2e 2e2e 2e2e 0a20 2020 2020 205d 0a20  .......      ]. 
+00001260: 2020 207d 2c0a 2020 2020 223c 7061 7065     },.    "<pape
+00001270: 7249 6420 6f66 2061 2070 6170 6572 2069  rId of a paper i
+00001280: 6e20 5365 6d61 6e74 6963 2053 6368 6f6c  n Semantic Schol
+00001290: 6172 3e22 3a20 7b20 2e2e 2e2e 2e2e 207d  ar>": { ...... }
+000012a0: 2c0a 2020 2020 223c 7061 7065 7249 6420  ,.    "<paperId 
+000012b0: 6f66 2061 2070 6170 6572 2069 6e20 5365  of a paper in Se
+000012c0: 6d61 6e74 6963 2053 6368 6f6c 6172 3e22  mantic Scholar>"
+000012d0: 3a20 7b20 2e2e 2e2e 2e2e 207d 2c0a 2020  : { ...... },.  
+000012e0: 2020 2e2e 2e2e 2e2e 0a20 207d 2c0a 2020    .......  },.  
+000012f0: 2265 6467 6573 223a 205b 0a20 2020 205b  "edges": [.    [
+00001300: 0a20 2020 2020 2020 2022 3c70 6170 6572  .        "<paper
+00001310: 4964 206f 6620 6120 7061 7065 7220 696e  Id of a paper in
+00001320: 2053 656d 616e 7469 6320 5363 686f 6c61   Semantic Schola
+00001330: 723e 222c 0a20 2020 2020 2020 2022 3c70  r>",.        "<p
+00001340: 6170 6572 4964 206f 6620 6120 7265 6665  aperId of a refe
+00001350: 7265 6e63 6520 696e 2074 6865 2061 626f  rence in the abo
+00001360: 7665 2070 6170 6572 3e22 0a20 2020 205d  ve paper>".    ]
+00001370: 2c0a 2020 2020 5b20 2e2e 2e2e 2e2e 205d  ,.    [ ...... ]
+00001380: 2c0a 2020 2020 5b20 2e2e 2e2e 2e2e 205d  ,.    [ ...... ]
+00001390: 2c0a 2020 2020 2e2e 2e2e 2e2e 0a20 205d  ,.    .......  ]
+000013a0: 0a60 6060 0a0a 2323 2320 5772 6974 6520  .```..### Write 
+000013b0: 746f 2061 204e 656f 344a 2064 6174 6162  to a Neo4J datab
+000013c0: 6173 650a 0a60 6060 7368 0a64 6f63 6b65  ase..```sh.docke
+000013d0: 7220 7075 6c6c 206e 656f 346a 0a64 6f63  r pull neo4j.doc
+000013e0: 6b65 7220 7275 6e20 2d2d 726d 202d 6974  ker run --rm -it
+000013f0: 202d 7020 3734 3734 3a37 3437 3420 2d70   -p 7474:7474 -p
+00001400: 2037 3638 373a 3736 3837 202d 7620 2428   7687:7687 -v $(
+00001410: 7077 6429 7361 7665 2f6e 656f 346a 3a2f  pwd)save/neo4j:/
+00001420: 6461 7461 202d 6520 4e45 4f34 4a5f 4155  data -e NEO4J_AU
+00001430: 5448 3d6e 6f6e 6520 6e65 6f34 6a0a 6060  TH=none neo4j.``
+00001440: 600a 0a65 2e67 2e20 7772 6974 6520 746f  `..e.g. write to
+00001450: 2060 6e65 6f34 6a3a 2f2f 6c6f 6361 6c68   `neo4j://localh
+00001460: 6f73 743a 3736 3837 603a 0a0a 6060 6073  ost:7687`:..```s
+00001470: 680a 7079 7468 6f6e 202d 6d20 6462 6c70  h.python -m dblp
+00001480: 5f63 7261 776c 6572 202d 6b20 7669 6465  _crawler -k vide
+00001490: 6f20 2d6b 2065 6467 6520 2d70 2032 3764  o -k edge -p 27d
+000014a0: 3564 6337 3032 3830 6338 3632 3866 3138  5dc70280c8628f18
+000014b0: 3161 3766 3838 3831 3931 3230 3235 6638  1a7f8881912025f8
+000014c0: 3038 3235 3620 2d61 2031 3638 3134 3537  08256 -a 1681457
+000014d0: 206e 656f 346a 202d 2d75 7269 206e 656f   neo4j --uri neo
+000014e0: 346a 3a2f 2f6c 6f63 616c 686f 7374 3a37  4j://localhost:7
+000014f0: 3638 370a 6060 600a 0a23 2323 2320 5469  687.```..#### Ti
+00001500: 7073 0a0a 5769 7468 6f75 7420 696e 6465  ps..Without inde
+00001510: 782c 204e 454f 344a 2071 7565 7279 2077  x, NEO4J query w
+00001520: 696c 6c20 6265 2076 6572 7920 7665 7279  ill be very very
+00001530: 2073 6c6f 772e 2053 6f20 6265 666f 7265   slow. So before
+00001540: 2079 6f75 2073 7461 7274 2c20 796f 7520   you start, you 
+00001550: 7368 6f75 6c64 2061 6464 2073 6f6d 6520  should add some 
+00001560: 696e 6465 783a 0a0a 6060 6063 716c 0a43  index:..```cql.C
+00001570: 5245 4154 4520 494e 4445 5820 7075 626c  REATE INDEX publ
+00001580: 6963 6174 696f 6e5f 7469 746c 655f 6861  ication_title_ha
+00001590: 7368 5f69 6e64 6578 2046 4f52 2028 703a  sh_index FOR (p:
+000015a0: 5075 626c 6963 6174 696f 6e29 204f 4e20  Publication) ON 
+000015b0: 2870 2e74 6974 6c65 5f68 6173 6829 3b0a  (p.title_hash);.
+000015c0: 4352 4541 5445 2049 4e44 4558 2070 7562  CREATE INDEX pub
+000015d0: 6c69 6361 7469 6f6e 5f64 626c 705f 6b65  lication_dblp_ke
+000015e0: 795f 696e 6465 7820 464f 5220 2870 3a50  y_index FOR (p:P
+000015f0: 7562 6c69 6361 7469 6f6e 2920 4f4e 2028  ublication) ON (
+00001600: 702e 6462 6c70 5f6b 6579 293b 0a43 5245  p.dblp_key);.CRE
+00001610: 4154 4520 494e 4445 5820 7075 626c 6963  ATE INDEX public
+00001620: 6174 696f 6e5f 7061 7065 725f 6964 5f69  ation_paper_id_i
+00001630: 6e64 6578 2046 4f52 2028 703a 5075 626c  ndex FOR (p:Publ
+00001640: 6963 6174 696f 6e29 204f 4e20 2870 2e70  ication) ON (p.p
+00001650: 6170 6572 4964 293b 0a43 5245 4154 4520  aperId);.CREATE 
+00001660: 494e 4445 5820 7065 7273 6f6e 5f61 7574  INDEX person_aut
+00001670: 686f 725f 6964 5f69 6e64 6578 2046 4f52  hor_id_index FOR
+00001680: 2028 703a 5065 7273 6f6e 2920 4f4e 2028   (p:Person) ON (
+00001690: 702e 6175 7468 6f72 4964 293b 0a43 5245  p.authorId);.CRE
+000016a0: 4154 4520 494e 4445 5820 7065 7273 6f6e  ATE INDEX person
+000016b0: 5f64 626c 705f 7069 645f 696e 6465 7820  _dblp_pid_index 
+000016c0: 464f 5220 2870 3a50 6572 736f 6e29 204f  FOR (p:Person) O
+000016d0: 4e20 2870 2e64 626c 705f 7069 6429 3b0a  N (p.dblp_pid);.
+000016e0: 6060 600a 0a23 2323 2047 6574 2069 6e69  ```..### Get ini
+000016f0: 7469 616c 2070 6170 6572 206c 6973 7420  tial paper list 
+00001700: 6f72 2061 7574 686f 7220 6c69 7374 2066  or author list f
+00001710: 726f 6d20 6120 4e65 6f34 4a20 6461 7461  rom a Neo4J data
+00001720: 6261 7365 0a0a 6060 6073 680a 7079 7468  base..```sh.pyth
+00001730: 6f6e 202d 6d20 6462 6c70 5f63 7261 776c  on -m dblp_crawl
+00001740: 6572 202d 6b20 7669 6465 6f20 2d6b 2065  er -k video -k e
+00001750: 6467 6520 2d61 2022 696d 706f 7274 6c69  dge -a "importli
+00001760: 622e 696d 706f 7274 5f6d 6f64 756c 6528  b.import_module(
+00001770: 2763 6974 6174 696f 6e5f 6372 6177 6c65  'citation_crawle
+00001780: 722e 696e 6974 2729 2e70 6170 6572 735f  r.init').papers_
+00001790: 696e 5f6e 656f 346a 2827 6e65 6f34 6a3a  in_neo4j('neo4j:
+000017a0: 2f2f 6c6f 6361 6c68 6f73 743a 3736 3837  //localhost:7687
+000017b0: 2729 2220 6e65 6f34 6a20 2d2d 7572 6920  ')" neo4j --uri 
+000017c0: 6e65 6f34 6a3a 2f2f 6c6f 6361 6c68 6f73  neo4j://localhos
+000017d0: 743a 3736 3837 0a60 6060 0a0a 6060 6073  t:7687.```..```s
+000017e0: 680a 7079 7468 6f6e 202d 6d20 6462 6c70  h.python -m dblp
+000017f0: 5f63 7261 776c 6572 202d 6b20 7669 6465  _crawler -k vide
+00001800: 6f20 2d6b 2065 6467 6520 2d70 2022 696d  o -k edge -p "im
+00001810: 706f 7274 6c69 622e 696d 706f 7274 5f6d  portlib.import_m
+00001820: 6f64 756c 6528 2763 6974 6174 696f 6e5f  odule('citation_
+00001830: 6372 6177 6c65 722e 696e 6974 2729 2e61  crawler.init').a
+00001840: 7574 686f 7273 5f69 6e5f 6e65 6f34 6a28  uthors_in_neo4j(
+00001850: 276e 656f 346a 3a2f 2f6c 6f63 616c 686f  'neo4j://localho
+00001860: 7374 3a37 3638 3727 2922 206e 656f 346a  st:7687')" neo4j
+00001870: 202d 2d75 7269 206e 656f 346a 3a2f 2f6c   --uri neo4j://l
+00001880: 6f63 616c 686f 7374 3a37 3638 370a 6060  ocalhost:7687.``
+00001890: 600a 0a60 696d 706f 7274 6c69 622e 696d  `..`importlib.im
+000018a0: 706f 7274 5f6d 6f64 756c 6560 2069 7320  port_module` is 
+000018b0: 666c 6578 6962 6c65 2c20 796f 7520 6361  flexible, you ca
+000018c0: 6e20 696d 706f 7274 2079 6f75 7220 6f77  n import your ow
+000018d0: 6e20 7661 7269 6162 6c65 7320 7468 726f  n variables thro
+000018e0: 7567 6820 7468 6973 2e0a                 ugh this..
```

### Comparing `citation_crawler-2.9/citation_crawler/__main__.py` & `citation_crawler-2.9.1/citation_crawler/__main__.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9/citation_crawler/arg.py` & `citation_crawler-2.9.1/citation_crawler/arg.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9/citation_crawler/crawlers/common.py` & `citation_crawler-2.9.1/citation_crawler/crawlers/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import json
 from datetime import datetime, timedelta
 
 import aiohttp
 import logging
 from aiofile import async_open
+import asyncio
 from asyncio import Semaphore
 
 logger = logging.getLogger("common")
 
 
 def getenv_int(key) -> int:
     cache_days = os.getenv(key)
@@ -17,28 +18,39 @@
         try:
             return int(cache_days)
         except:
             pass
     return None
 
 
+def getenv_float(key) -> float:
+    cache_days = os.getenv(key)
+    if cache_days is not None:
+        try:
+            return float(cache_days)
+        except:
+            pass
+    return None
+
+
 def getenv_headers(key) -> Dict:
     headers = os.getenv(key)
     if headers is not None:
         try:
             return json.loads(headers)
         except:
             pass
     return None
 
 
 http_concorent = getenv_int('HTTP_CONCORRENT')
 http_sem = Semaphore(http_concorent if http_concorent is not None else 8)
 file_sem = Semaphore(512)
 http_headers = getenv_headers('HTTP_HEADERS')
+http_sleep = getenv_float('HTTP_SLEEP') or 0
 
 
 def get_cache_datetime(path) -> datetime:
     return datetime.fromtimestamp(os.path.getmtime(path))
 
 
 async def download_item(url: str, path: str, cache_days: int, is_valid: Callable[[str], None]) -> Optional[Dict]:
@@ -71,11 +83,13 @@
                                        timeout=os.getenv("HTTP_TIMEOUT") or 30) as response:
                     logger.debug(" download: %s <- %s" % (path, url))
                     text = await response.text()
                     assert is_valid(text)
                     os.makedirs(os.path.dirname(save_path), exist_ok=True)
                     async with async_open(save_path, 'w') as f:
                         await f.write(text)
+                    if http_sleep is not None:
+                        await asyncio.sleep(http_sleep)
                     return text
         except Exception as e:
             logger.error(" down err: %s" % e)
     return None
```

### Comparing `citation_crawler-2.9/citation_crawler/crawlers/ss.py` & `citation_crawler-2.9.1/citation_crawler/crawlers/ss.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9/citation_crawler/graph.py` & `citation_crawler-2.9.1/citation_crawler/graph.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9/citation_crawler/init/neo4j.py` & `citation_crawler-2.9.1/citation_crawler/init/neo4j.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9/citation_crawler/items.py` & `citation_crawler-2.9.1/citation_crawler/items.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9/citation_crawler/summarizers/neo4j.py` & `citation_crawler-2.9.1/citation_crawler/summarizers/neo4j.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9/citation_crawler/summarizers/nx.py` & `citation_crawler-2.9.1/citation_crawler/summarizers/nx.py`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9/citation_crawler.egg-info/PKG-INFO` & `citation_crawler-2.9.1/citation_crawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-crawler
-Version: 2.9
+Version: 2.9.1
 Summary: Asynchronous high-concurrency citation crawler, use with caution!
 Home-page: https://github.com/yindaheng98/citation-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -103,15 +103,18 @@
 * `HTTP_TIMEOUT`
   * Timeout for each http request, in seconds
 * `HTTP_CONCORRENT`
   * Concurrent HTTP requests
   * default: `8`
 * `HTTP_HEADERS`
   * Headers for HTTP requests
-  * default: None
+  * default: `None`
+* `HTTP_SLEEP`
+  * Sleep after request (in seconds)
+  * default: `0`
 
 ### Write to a JSON file
 
 e.g. write to `summary.json`:
 
 ```sh
 python -m citation_crawler -k video -k edge -p 27d5dc70280c8628f181a7f8881912025f808256 -a 1681457 networkx --dest summary.json
```

### Comparing `citation_crawler-2.9/citation_crawler.egg-info/SOURCES.txt` & `citation_crawler-2.9.1/citation_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citation_crawler-2.9/setup.py` & `citation_crawler-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'citation_crawler.crawlers': 'citation_crawler/crawlers',
     'citation_crawler.summarizers': 'citation_crawler/summarizers',
     'citation_crawler.init': 'citation_crawler/init',
 }
 
 setup(
     name='citation_crawler',
-    version='2.9',
+    version='2.9.1',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/citation-crawler',
     description=u'Asynchronous high-concurrency citation crawler, use with caution!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

