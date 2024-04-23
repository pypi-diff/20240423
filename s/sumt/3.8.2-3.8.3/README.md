# Comparing `tmp/sumt-3.8.2.tar.gz` & `tmp/sumt-3.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumt-3.8.2.tar", last modified: Thu Feb  8 06:53:54 2024, max compression
+gzip compressed data, was "sumt-3.8.3.tar", last modified: Tue Apr 23 14:04:58 2024, max compression
```

## Comparing `sumt-3.8.2.tar` & `sumt-3.8.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2024-02-08 06:53:54.776767 sumt-3.8.2/
--rw-r--r--   0 agpe       (502) staff       (20)    35149 2022-02-20 16:31:26.000000 sumt-3.8.2/LICENSE
--rw-r--r--   0 agpe       (502) staff       (20)    29451 2024-02-08 06:53:54.776664 sumt-3.8.2/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)    28917 2024-02-08 06:53:09.000000 sumt-3.8.2/README.md
--rw-r--r--   0 agpe       (502) staff       (20)      104 2021-11-24 21:14:07.000000 sumt-3.8.2/pyproject.toml
--rw-r--r--   0 agpe       (502) staff       (20)      650 2024-02-08 06:53:54.777100 sumt-3.8.2/setup.cfg
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2024-02-08 06:53:54.776385 sumt-3.8.2/sumt.egg-info/
--rw-r--r--   0 agpe       (502) staff       (20)    29451 2024-02-08 06:53:54.000000 sumt-3.8.2/sumt.egg-info/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)      220 2024-02-08 06:53:54.000000 sumt-3.8.2/sumt.egg-info/SOURCES.txt
--rw-r--r--   0 agpe       (502) staff       (20)        1 2024-02-08 06:53:54.000000 sumt-3.8.2/sumt.egg-info/dependency_links.txt
--rw-r--r--   0 agpe       (502) staff       (20)       35 2024-02-08 06:53:54.000000 sumt-3.8.2/sumt.egg-info/entry_points.txt
--rw-r--r--   0 agpe       (502) staff       (20)       28 2024-02-08 06:53:54.000000 sumt-3.8.2/sumt.egg-info/requires.txt
--rw-r--r--   0 agpe       (502) staff       (20)        5 2024-02-08 06:53:54.000000 sumt-3.8.2/sumt.egg-info/top_level.txt
--rwxr-xr-x   0 agpe       (502) staff       (20)    47095 2024-01-30 12:49:57.000000 sumt-3.8.2/sumt.py
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2024-04-23 14:04:58.295313 sumt-3.8.3/
+-rw-------   0 agpe       (502) staff       (20)    35149 2022-02-20 16:31:26.000000 sumt-3.8.3/LICENSE
+-rw-r--r--   0 agpe       (502) staff       (20)    29451 2024-04-23 14:04:58.295132 sumt-3.8.3/PKG-INFO
+-rw-------   0 agpe       (502) staff       (20)    28917 2024-04-23 14:04:41.000000 sumt-3.8.3/README.md
+-rw-------   0 agpe       (502) staff       (20)      104 2021-11-24 21:14:07.000000 sumt-3.8.3/pyproject.toml
+-rw-------   0 agpe       (502) staff       (20)      650 2024-04-23 14:04:58.295622 sumt-3.8.3/setup.cfg
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2024-04-23 14:04:58.294833 sumt-3.8.3/sumt.egg-info/
+-rw-r--r--   0 agpe       (502) staff       (20)    29451 2024-04-23 14:04:58.000000 sumt-3.8.3/sumt.egg-info/PKG-INFO
+-rw-------   0 agpe       (502) staff       (20)      220 2024-04-23 14:04:58.000000 sumt-3.8.3/sumt.egg-info/SOURCES.txt
+-rw-------   0 agpe       (502) staff       (20)        1 2024-04-23 14:04:58.000000 sumt-3.8.3/sumt.egg-info/dependency_links.txt
+-rw-------   0 agpe       (502) staff       (20)       35 2024-04-23 14:04:58.000000 sumt-3.8.3/sumt.egg-info/entry_points.txt
+-rw-------   0 agpe       (502) staff       (20)       28 2024-04-23 14:04:58.000000 sumt-3.8.3/sumt.egg-info/requires.txt
+-rw-------   0 agpe       (502) staff       (20)        5 2024-04-23 14:04:58.000000 sumt-3.8.3/sumt.egg-info/top_level.txt
+-rwxr-xr-x   0 agpe       (502) staff       (20)    47171 2024-04-23 14:04:31.000000 sumt-3.8.3/sumt.py
```

### Comparing `sumt-3.8.2/LICENSE` & `sumt-3.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sumt-3.8.2/PKG-INFO` & `sumt-3.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumt
-Version: 3.8.2
+Version: 3.8.3
 Summary: Computes consensus trees and other phylogenetic tree summaries
 Home-page: https://github.com/agormp/sumt
 Author: Anders Gorm Pedersen
 Author-email: agpe@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: phylotreelib>=1.26.1
 Requires-Dist: psutil
 
 # sumt
 
-![](https://img.shields.io/badge/version-3.8.2-blue)
+![](https://img.shields.io/badge/version-3.8.3-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=PyPI%20downloads&service=github)](https://pepy.tech/project/sumt)
 [![DOI](https://zenodo.org/badge/461522623.svg)](https://zenodo.org/doi/10.5281/zenodo.10148693)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute four different kinds of main tree summaries:
```

### Comparing `sumt-3.8.2/README.md` & `sumt-3.8.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # sumt
 
-![](https://img.shields.io/badge/version-3.8.2-blue)
+![](https://img.shields.io/badge/version-3.8.3-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=PyPI%20downloads&service=github)](https://pepy.tech/project/sumt)
 [![DOI](https://zenodo.org/badge/461522623.svg)](https://zenodo.org/doi/10.5281/zenodo.10148693)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute four different kinds of main tree summaries:
```

### Comparing `sumt-3.8.2/setup.cfg` & `sumt-3.8.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sumt
-version = 3.8.2
+version = 3.8.3
 author = Anders Gorm Pedersen
 author_email = agpe@dtu.dk
 description = Computes consensus trees and other phylogenetic tree summaries
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/agormp/sumt
 classifiers =
```

### Comparing `sumt-3.8.2/sumt.egg-info/PKG-INFO` & `sumt-3.8.3/sumt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumt
-Version: 3.8.2
+Version: 3.8.3
 Summary: Computes consensus trees and other phylogenetic tree summaries
 Home-page: https://github.com/agormp/sumt
 Author: Anders Gorm Pedersen
 Author-email: agpe@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: phylotreelib>=1.26.1
 Requires-Dist: psutil
 
 # sumt
 
-![](https://img.shields.io/badge/version-3.8.2-blue)
+![](https://img.shields.io/badge/version-3.8.3-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=PyPI%20downloads&service=github)](https://pepy.tech/project/sumt)
 [![DOI](https://zenodo.org/badge/461522623.svg)](https://zenodo.org/doi/10.5281/zenodo.10148693)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute four different kinds of main tree summaries:
```

### Comparing `sumt-3.8.2/sumt.py` & `sumt-3.8.3/sumt.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,17 +199,19 @@
             infilepath = args.infilelist[0]
         else:
             wt, infilepath = args.fileweights[0]
         args.outbase = Path(infilepath.stem.split('.')[0])
 
     if args.burninfrac is None:
         args.burninfrac = [0.0] * len(args.infilelist)
+    elif len(args.burninfrac) == 1:
+        burnin_value = args.burninfrac[0]
+        args.burninfrac = [burnin_value] * len(args.infilelist)
     elif len(args.burninfrac) != len(args.infilelist):
-        msg = "number of burnin values {len(args.burninfrac)} must match number of input files len(args.infilelist){}"
-        raise parser.error(msg)
+        parser.error("either provide one burnin value, or one value per input file")
 
     if any(x < 0 or x > 1 for x in args.burninfrac):
         parser.error("option -b: NUM must be between 0.0 and 1.0")
 
     if args.treeprobs and (args.treeprobs > 1 or args.treeprobs < 0):
         parser.error(f"option -t: NUM must be between 0.0 and 1.0 (provided value: -t {args.treeprobs})")
 
@@ -368,15 +370,15 @@
                       help="root summary tree on bipartition where root is located most frequently in input trees. " +
                            "NOTE: only meaningful if input trees are estimated using clock model")
 
     ####################################################################################
 
     bayes_grp = parser.add_argument_group("Bayesian phylogeny options")
 
-    bayes_grp.add_argument("-b", dest="burninfrac", metavar="NUM", type=float, default=None, nargs='*',
+    bayes_grp.add_argument("-b", dest="burninfrac", metavar="NUM", type=float, default=None, nargs='+',
                            help="burnin: fraction of trees to discard [0 - 1; default: %(default)s]. "
                            + "Either one value (used on all input files), or one value per input file.")
 
     bayes_grp.add_argument("-t", type=float, dest="treeprobs", metavar="NUM",
                       help="compute tree probabilities, report NUM percent credible interval [0 - 1]")
 
     bayes_grp.add_argument("-s", action="store_true", dest="std",
```

