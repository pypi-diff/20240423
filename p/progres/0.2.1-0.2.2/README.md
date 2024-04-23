# Comparing `tmp/progres-0.2.1.tar.gz` & `tmp/progres-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progres-0.2.1.tar", last modified: Wed Apr 17 18:16:41 2024, max compression
+gzip compressed data, was "progres-0.2.2.tar", last modified: Tue Apr 23 11:38:23 2024, max compression
```

## Comparing `progres-0.2.1.tar` & `progres-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-17 18:16:41.381106 progres-0.2.1/
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)     3635 2024-04-15 18:40:30.000000 progres-0.2.1/LICENSE
--rw-r--r--   0 jgreener  (1000) jgreener  (1000)    12718 2024-04-17 18:16:41.381106 progres-0.2.1/PKG-INFO
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)    12067 2024-04-17 17:35:48.000000 progres-0.2.1/README.md
-drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-17 18:16:41.377106 progres-0.2.1/bin/
--rwxrwxr-x   0 jgreener  (1000) jgreener  (1000)     3876 2024-04-17 17:04:22.000000 progres-0.2.1/bin/progres
-drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-17 18:16:41.377106 progres-0.2.1/progres/
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       23 2022-11-16 16:19:38.000000 progres-0.2.1/progres/__init__.py
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)    23732 2024-04-17 17:30:15.000000 progres-0.2.1/progres/progres.py
-drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-17 18:16:41.381106 progres-0.2.1/progres.egg-info/
--rw-r--r--   0 jgreener  (1000) jgreener  (1000)    12718 2024-04-17 18:16:41.000000 progres-0.2.1/progres.egg-info/PKG-INFO
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)      231 2024-04-17 18:16:41.000000 progres-0.2.1/progres.egg-info/SOURCES.txt
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)        1 2024-04-17 18:16:41.000000 progres-0.2.1/progres.egg-info/dependency_links.txt
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       29 2024-04-17 18:16:41.000000 progres-0.2.1/progres.egg-info/requires.txt
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)        8 2024-04-17 18:16:41.000000 progres-0.2.1/progres.egg-info/top_level.txt
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       38 2024-04-17 18:16:41.381106 progres-0.2.1/setup.cfg
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)      917 2024-04-17 09:53:40.000000 progres-0.2.1/setup.py
+drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-23 11:38:23.221322 progres-0.2.2/
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)     3635 2024-04-15 18:40:30.000000 progres-0.2.2/LICENSE
+-rw-r--r--   0 jgreener  (1000) jgreener  (1000)    13001 2024-04-23 11:38:23.221322 progres-0.2.2/PKG-INFO
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)    12350 2024-04-23 11:31:27.000000 progres-0.2.2/README.md
+drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-23 11:38:23.221322 progres-0.2.2/bin/
+-rwxrwxr-x   0 jgreener  (1000) jgreener  (1000)     4009 2024-04-18 10:02:07.000000 progres-0.2.2/bin/progres
+drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-23 11:38:23.221322 progres-0.2.2/progres/
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       23 2022-11-16 16:19:38.000000 progres-0.2.2/progres/__init__.py
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)    24079 2024-04-23 11:22:48.000000 progres-0.2.2/progres/progres.py
+drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-23 11:38:23.221322 progres-0.2.2/progres.egg-info/
+-rw-r--r--   0 jgreener  (1000) jgreener  (1000)    13001 2024-04-23 11:38:23.000000 progres-0.2.2/progres.egg-info/PKG-INFO
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)      231 2024-04-23 11:38:23.000000 progres-0.2.2/progres.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)        1 2024-04-23 11:38:23.000000 progres-0.2.2/progres.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       29 2024-04-23 11:38:23.000000 progres-0.2.2/progres.egg-info/requires.txt
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)        8 2024-04-23 11:38:23.000000 progres-0.2.2/progres.egg-info/top_level.txt
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       38 2024-04-23 11:38:23.221322 progres-0.2.2/setup.cfg
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)      917 2024-04-23 11:31:43.000000 progres-0.2.2/setup.py
```

### Comparing `progres-0.2.1/LICENSE` & `progres-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `progres-0.2.1/PKG-INFO` & `progres-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progres
-Version: 0.2.1
+Version: 0.2.2
 Summary: Fast protein structure searching using structure graph embeddings
 Home-page: https://github.com/greener-group/progres
 Author: Joe G Greener
 Author-email: jgreener@mrc-lmb.cam.ac.uk
 License: MIT
 Keywords: protein structure search graph embedding
 Classifier: Programming Language :: Python :: 3
@@ -29,46 +29,48 @@
 Searching typically takes 1-2 s and is much faster for multiple queries.
 For the AlphaFold database, initial data loading takes around a minute but subsequent searching takes a tenth of a second per query.
 Currently [SCOPe](https://scop.berkeley.edu), [CATH](http://cathdb.info), [ECOD](http://prodata.swmed.edu/ecod), the [AlphaFold structures for 21 model organisms](https://doi.org/10.1093/nar/gkab1061) and the [AlphaFold database TED domains](https://www.biorxiv.org/content/10.1101/2024.03.18.585509) are provided for searching against.
 
 ## Installation
 
 1. Python 3.8 or later is required. The software is OS-independent.
-2. Install [PyTorch](https://pytorch.org) 1.11 or later, [PyTorch Scatter](https://github.com/rusty1s/pytorch_scatter), [PyTorch Geometric](https://github.com/pyg-team/pytorch_geometric) and [FAISS](https://github.com/facebookresearch/faiss) as appropriate for your system. A GPU is not required and will only provide speedup in certain situations since multiple workers can be used on CPU. Example commands:
+2. Install [PyTorch](https://pytorch.org) 1.11 or later, [PyTorch Scatter](https://github.com/rusty1s/pytorch_scatter), [PyTorch Geometric](https://github.com/pyg-team/pytorch_geometric) and [FAISS](https://github.com/facebookresearch/faiss) as appropriate for your system. A GPU is not required but may provide speedup in certain situations. Example commands:
 ```bash
 conda create -n prog python=3.9
 conda activate prog
 conda install pytorch=1.11 faiss-cpu -c pytorch
 conda install pytorch-scatter pyg -c pyg
 ```
 3. Run `pip install progres`, which will also install [Biopython](https://biopython.org), [mmtf-python](https://github.com/rcsb/mmtf-python) and [einops](https://github.com/arogozhnikov/einops) if they are not already present.
-4. The first time you search with the software the trained model and pre-embedded databases (~220 MB) will be downloaded to the package directory from [Zenodo](https://zenodo.org/record/7782088), which requires an internet connection. This can take a few minutes.
-5. The first time you search against the AlphaFold database TED domains the pre-embedded database (~33 GB) will be downloaded in a similar way. This can take a while. Make sure you have enough disk space!
+4. The first time you search with the software the trained model and pre-embedded databases (~220 MB) will be downloaded to the package directory from [Zenodo](https://zenodo.org/record/7782088), which requires an internet connection. This can take a few minutes. You can set the environmental variable `PROGRES_DATA_DIR` to change where this data is stored, for example if you cannot write to the package directory. Remember to keep it set the next time you run Progres.
+5. The first time you search against the AlphaFold database TED domains the pre-embedded database (~33 GB) will be downloaded similarly. This can take a while. Make sure you have enough disk space!
+
+Alternatively, a Docker file is available in the `docker` directory.
 
 ## Usage
 
 On Unix systems the executable `progres` will be added to the path during installation.
 On Windows you can call the `bin/progres` script with python if you can't access the executable.
 
 Run `progres -h` to see the help text and `progres {mode} -h` to see the help text for each mode.
 The modes are described below but there are other options outlined in the help text.
-For example the `-d` flag sets the device to run on; this is `cpu` by default since this is usually fastest for searching, but `cuda` may be slightly faster when embedding a dataset.
+For example the `-d` flag sets the device to run on; this is `cpu` by default since this is often fastest for searching, but `cuda` may be faster when searching many queries or embedding a dataset.
 
 ## Searching a structure against a database
 
 To search a PDB file `query.pdb` against domains in the SCOPe database and print output:
 ```bash
 progres search -q query.pdb -t scope95
 ```
 ```
 # QUERY_NUM: 1
 # QUERY: query.pdb
 # QUERY_SIZE: 150 residues
 # DATABASE: scope95
-# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.1
+# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.2
 # HIT_N  DOMAIN   HIT_NRES  SIMILARITY  NOTES
       1  d1a6ja_       150      1.0000  d.112.1.1 - Nitrogen regulatory bacterial protein IIa-ntr {Escherichia coli [TaxId: 562]}
       2  d2a0ja_       146      0.9988  d.112.1.0 - automated matches {Neisseria meningitidis [TaxId: 122586]}
       3  d3urra1       151      0.9983  d.112.1.0 - automated matches {Burkholderia thailandensis [TaxId: 271848]}
       4  d3lf6a_       154      0.9971  d.112.1.1 - automated matches {Artificial gene [TaxId: 32630]}
       5  d3oxpa1       147      0.9968  d.112.1.0 - automated matches {Yersinia pestis [TaxId: 214092]}
 ...
@@ -170,7 +172,8 @@
 The trained model and pre-embedded databases are available on [Zenodo](https://zenodo.org/record/7782088).
 
 ## Notes
 
 The implementation of the E(n)-equivariant GNN uses [EGNN PyTorch](https://github.com/lucidrains/egnn-pytorch).
 
 Please open issues or [get in touch](http://jgreener64.github.io) with any feedback.
+Contributions via pull requests are welcome.
```

### Comparing `progres-0.2.1/README.md` & `progres-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,46 +10,48 @@
 Searching typically takes 1-2 s and is much faster for multiple queries.
 For the AlphaFold database, initial data loading takes around a minute but subsequent searching takes a tenth of a second per query.
 Currently [SCOPe](https://scop.berkeley.edu), [CATH](http://cathdb.info), [ECOD](http://prodata.swmed.edu/ecod), the [AlphaFold structures for 21 model organisms](https://doi.org/10.1093/nar/gkab1061) and the [AlphaFold database TED domains](https://www.biorxiv.org/content/10.1101/2024.03.18.585509) are provided for searching against.
 
 ## Installation
 
 1. Python 3.8 or later is required. The software is OS-independent.
-2. Install [PyTorch](https://pytorch.org) 1.11 or later, [PyTorch Scatter](https://github.com/rusty1s/pytorch_scatter), [PyTorch Geometric](https://github.com/pyg-team/pytorch_geometric) and [FAISS](https://github.com/facebookresearch/faiss) as appropriate for your system. A GPU is not required and will only provide speedup in certain situations since multiple workers can be used on CPU. Example commands:
+2. Install [PyTorch](https://pytorch.org) 1.11 or later, [PyTorch Scatter](https://github.com/rusty1s/pytorch_scatter), [PyTorch Geometric](https://github.com/pyg-team/pytorch_geometric) and [FAISS](https://github.com/facebookresearch/faiss) as appropriate for your system. A GPU is not required but may provide speedup in certain situations. Example commands:
 ```bash
 conda create -n prog python=3.9
 conda activate prog
 conda install pytorch=1.11 faiss-cpu -c pytorch
 conda install pytorch-scatter pyg -c pyg
 ```
 3. Run `pip install progres`, which will also install [Biopython](https://biopython.org), [mmtf-python](https://github.com/rcsb/mmtf-python) and [einops](https://github.com/arogozhnikov/einops) if they are not already present.
-4. The first time you search with the software the trained model and pre-embedded databases (~220 MB) will be downloaded to the package directory from [Zenodo](https://zenodo.org/record/7782088), which requires an internet connection. This can take a few minutes.
-5. The first time you search against the AlphaFold database TED domains the pre-embedded database (~33 GB) will be downloaded in a similar way. This can take a while. Make sure you have enough disk space!
+4. The first time you search with the software the trained model and pre-embedded databases (~220 MB) will be downloaded to the package directory from [Zenodo](https://zenodo.org/record/7782088), which requires an internet connection. This can take a few minutes. You can set the environmental variable `PROGRES_DATA_DIR` to change where this data is stored, for example if you cannot write to the package directory. Remember to keep it set the next time you run Progres.
+5. The first time you search against the AlphaFold database TED domains the pre-embedded database (~33 GB) will be downloaded similarly. This can take a while. Make sure you have enough disk space!
+
+Alternatively, a Docker file is available in the `docker` directory.
 
 ## Usage
 
 On Unix systems the executable `progres` will be added to the path during installation.
 On Windows you can call the `bin/progres` script with python if you can't access the executable.
 
 Run `progres -h` to see the help text and `progres {mode} -h` to see the help text for each mode.
 The modes are described below but there are other options outlined in the help text.
-For example the `-d` flag sets the device to run on; this is `cpu` by default since this is usually fastest for searching, but `cuda` may be slightly faster when embedding a dataset.
+For example the `-d` flag sets the device to run on; this is `cpu` by default since this is often fastest for searching, but `cuda` may be faster when searching many queries or embedding a dataset.
 
 ## Searching a structure against a database
 
 To search a PDB file `query.pdb` against domains in the SCOPe database and print output:
 ```bash
 progres search -q query.pdb -t scope95
 ```
 ```
 # QUERY_NUM: 1
 # QUERY: query.pdb
 # QUERY_SIZE: 150 residues
 # DATABASE: scope95
-# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.1
+# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.2
 # HIT_N  DOMAIN   HIT_NRES  SIMILARITY  NOTES
       1  d1a6ja_       150      1.0000  d.112.1.1 - Nitrogen regulatory bacterial protein IIa-ntr {Escherichia coli [TaxId: 562]}
       2  d2a0ja_       146      0.9988  d.112.1.0 - automated matches {Neisseria meningitidis [TaxId: 122586]}
       3  d3urra1       151      0.9983  d.112.1.0 - automated matches {Burkholderia thailandensis [TaxId: 271848]}
       4  d3lf6a_       154      0.9971  d.112.1.1 - automated matches {Artificial gene [TaxId: 32630]}
       5  d3oxpa1       147      0.9968  d.112.1.0 - automated matches {Yersinia pestis [TaxId: 214092]}
 ...
@@ -151,7 +153,8 @@
 The trained model and pre-embedded databases are available on [Zenodo](https://zenodo.org/record/7782088).
 
 ## Notes
 
 The implementation of the E(n)-equivariant GNN uses [EGNN PyTorch](https://github.com/lucidrains/egnn-pytorch).
 
 Please open issues or [get in touch](http://jgreener64.github.io) with any feedback.
+Contributions via pull requests are welcome.
```

### Comparing `progres-0.2.1/bin/progres` & `progres-0.2.2/bin/progres`

 * *Files 5% similar despite different names*

```diff
@@ -45,29 +45,33 @@
     choices=["guess", "pdb", "mmcif", "mmtf", "coords"], default="guess",
     help="file format of the structures, by default guessed from the file extension")
 parser_embed.add_argument("-d", "--device", default="cpu",
     help="device to run on, default is \"cpu\"")
 
 args = parser.parse_args()
 
-if args.mode == "search":
-    from progres import progres_search_print
-    if args.minsimilarity < 0 or args.minsimilarity > 1:
-        raise argparse.ArgumentTypeError("minsimilarity must be between 0 and 1")
-    if args.maxhits < 1:
-        raise argparse.ArgumentTypeError("maxhits must be a positive integer")
-    if args.querystructure:
-        progres_search_print(querystructure=args.querystructure, targetdb=args.targetdb,
-                             fileformat=args.fileformat, minsimilarity=args.minsimilarity,
-                             maxhits=args.maxhits, device=args.device)
-    elif args.querylist:
-        progres_search_print(querylist=args.querylist, targetdb=args.targetdb,
-                             fileformat=args.fileformat, minsimilarity=args.minsimilarity,
-                             maxhits=args.maxhits, device=args.device)
+def main():
+    if args.mode == "search":
+        from progres import progres_search_print
+        if args.minsimilarity < 0 or args.minsimilarity > 1:
+            raise argparse.ArgumentTypeError("minsimilarity must be between 0 and 1")
+        if args.maxhits < 1:
+            raise argparse.ArgumentTypeError("maxhits must be a positive integer")
+        if args.querystructure:
+            progres_search_print(querystructure=args.querystructure, targetdb=args.targetdb,
+                                fileformat=args.fileformat, minsimilarity=args.minsimilarity,
+                                maxhits=args.maxhits, device=args.device)
+        elif args.querylist:
+            progres_search_print(querylist=args.querylist, targetdb=args.targetdb,
+                                fileformat=args.fileformat, minsimilarity=args.minsimilarity,
+                                maxhits=args.maxhits, device=args.device)
+        else:
+            print("One of -q and -l must be given for structure searching", file=sys.stderr)
+    elif args.mode == "embed":
+        from progres import progres_embed
+        progres_embed(structurelist=args.structurelist, outputfile=args.outputfile,
+                    fileformat=args.fileformat, device=args.device)
     else:
-        print("One of -q and -l must be given for structure searching", file=sys.stderr)
-elif args.mode == "embed":
-    from progres import progres_embed
-    progres_embed(structurelist=args.structurelist, outputfile=args.outputfile,
-                  fileformat=args.fileformat, device=args.device)
-else:
-    print("No mode selected, run \"progres -h\" to see help", file=sys.stderr)
+        print("No mode selected, run \"progres -h\" to see help", file=sys.stderr)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `progres-0.2.1/progres/progres.py` & `progres-0.2.2/progres/progres.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,18 @@
 default_maxhits = 100
 pre_embedded_dbs = ["scope95", "scope40", "cath40", "ecod70", "af21org"]
 pre_embedded_dbs_faiss = ["afted"]
 zenodo_record = "10975201" # This only needs to change when the trained model or databases change
 trained_model_subdir = "v_0_2_0" # This only needs to change when the trained model changes
 database_subdir      = "v_0_2_1" # This only needs to change when the databases change
 progres_dir       = os.path.dirname(os.path.realpath(__file__))
-trained_model_dir = os.path.join(progres_dir, "trained_models", trained_model_subdir)
-database_dir      = os.path.join(progres_dir, "databases"     , database_subdir     )
+# Allow data dir to be set from env var if exists, otherwise default to software location
+data_dir          = os.getenv("PROGRES_DATA_DIR", default=progres_dir)
+trained_model_dir = os.path.join(data_dir, "trained_models", trained_model_subdir)
+database_dir      = os.path.join(data_dir, "databases"     , database_subdir     )
 trained_model_fp  = os.path.join(trained_model_dir, "trained_model.pt")
 
 class SinusoidalPositionalEncoding(torch.nn.Module):
     def __init__(self, channels):
         super().__init__()
         channels = int(ceil(channels / 2) * 2)
         inv_freq = 1.0 / (pos_embed_freq_inv ** (torch.arange(0, channels, 2).float() / channels))
@@ -352,15 +354,16 @@
 def get_batch_size(device="cpu", using_faiss=False):
     if using_faiss:
         return 64
     else:
         return 8
 
 def get_num_workers(device="cpu"):
-    if device == "cpu":
+    # Multithreading error on Windows
+    if device == "cpu" and os.name != "nt":
         return torch.get_num_threads()
     else:
         return 0
 
 def download_data_if_required(download_afted=False):
     url_base = f"https://zenodo.org/record/{zenodo_record}/files"
     fps = [trained_model_fp]
@@ -369,29 +372,28 @@
         fps.append(os.path.join(database_dir, targetdb + ".pt"))
         urls.append(f"{url_base}/{targetdb}.pt")
     if download_afted:
         for fn in ["afted.index", "afted_noembs.pt"]:
             fps.append(os.path.join(database_dir, fn))
             urls.append(f"{url_base}/{fn}")
 
-    if not os.path.isdir(trained_model_dir):
-        os.makedirs(trained_model_dir)
-    if not os.path.isdir(database_dir):
-        os.makedirs(database_dir)
+    dirs_that_should_exist = [data_dir, trained_model_dir, database_dir]
+    for dir in dirs_that_should_exist:
+        os.makedirs(dir, exist_ok=True)    
 
     printed = False
     for fp, url in zip(fps, urls):
         if not os.path.isfile(fp):
             if fp.endswith("afted.index"):
                 print("Downloading afted data as first time setup (~33 GB) to ", database_dir,
                       ", internet connection required, this may take a while",
                       sep="", file=sys.stderr)
                 printed = True
             if not printed:
-                print("Downloading data as first time setup (~220 MB) to ", progres_dir,
+                print("Downloading data as first time setup (~220 MB) to ", data_dir,
                       ", internet connection required, this can take a few minutes",
                       sep="", file=sys.stderr)
                 printed = True
             try:
                 request.urlretrieve(url, fp)
                 if not fp.endswith("afted.index"):
                     d = torch.load(fp, map_location="cpu")
@@ -502,14 +504,18 @@
                     "domains":       domids,
                     "hits_nres":     hits_nres,
                     "similarities":  similarities,
                     "notes":         notes,
                 }
                 qi += 1
 
+                if device != "cpu" and search_type == "torch":
+                    del dists
+                    torch.cuda.empty_cache()
+
                 yield result_dict
 
 def progres_search(querystructure=None, querylist=None, queryembeddings=None, targetdb=None,
                    fileformat="guess", minsimilarity=default_minsimilarity, maxhits=default_maxhits,
                    device="cpu", batch_size=None):
     generator = progres_search_generator(querystructure, querylist, queryembeddings, targetdb,
                                          fileformat, minsimilarity, maxhits, device, batch_size)
```

### Comparing `progres-0.2.1/progres.egg-info/PKG-INFO` & `progres-0.2.2/progres.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progres
-Version: 0.2.1
+Version: 0.2.2
 Summary: Fast protein structure searching using structure graph embeddings
 Home-page: https://github.com/greener-group/progres
 Author: Joe G Greener
 Author-email: jgreener@mrc-lmb.cam.ac.uk
 License: MIT
 Keywords: protein structure search graph embedding
 Classifier: Programming Language :: Python :: 3
@@ -29,46 +29,48 @@
 Searching typically takes 1-2 s and is much faster for multiple queries.
 For the AlphaFold database, initial data loading takes around a minute but subsequent searching takes a tenth of a second per query.
 Currently [SCOPe](https://scop.berkeley.edu), [CATH](http://cathdb.info), [ECOD](http://prodata.swmed.edu/ecod), the [AlphaFold structures for 21 model organisms](https://doi.org/10.1093/nar/gkab1061) and the [AlphaFold database TED domains](https://www.biorxiv.org/content/10.1101/2024.03.18.585509) are provided for searching against.
 
 ## Installation
 
 1. Python 3.8 or later is required. The software is OS-independent.
-2. Install [PyTorch](https://pytorch.org) 1.11 or later, [PyTorch Scatter](https://github.com/rusty1s/pytorch_scatter), [PyTorch Geometric](https://github.com/pyg-team/pytorch_geometric) and [FAISS](https://github.com/facebookresearch/faiss) as appropriate for your system. A GPU is not required and will only provide speedup in certain situations since multiple workers can be used on CPU. Example commands:
+2. Install [PyTorch](https://pytorch.org) 1.11 or later, [PyTorch Scatter](https://github.com/rusty1s/pytorch_scatter), [PyTorch Geometric](https://github.com/pyg-team/pytorch_geometric) and [FAISS](https://github.com/facebookresearch/faiss) as appropriate for your system. A GPU is not required but may provide speedup in certain situations. Example commands:
 ```bash
 conda create -n prog python=3.9
 conda activate prog
 conda install pytorch=1.11 faiss-cpu -c pytorch
 conda install pytorch-scatter pyg -c pyg
 ```
 3. Run `pip install progres`, which will also install [Biopython](https://biopython.org), [mmtf-python](https://github.com/rcsb/mmtf-python) and [einops](https://github.com/arogozhnikov/einops) if they are not already present.
-4. The first time you search with the software the trained model and pre-embedded databases (~220 MB) will be downloaded to the package directory from [Zenodo](https://zenodo.org/record/7782088), which requires an internet connection. This can take a few minutes.
-5. The first time you search against the AlphaFold database TED domains the pre-embedded database (~33 GB) will be downloaded in a similar way. This can take a while. Make sure you have enough disk space!
+4. The first time you search with the software the trained model and pre-embedded databases (~220 MB) will be downloaded to the package directory from [Zenodo](https://zenodo.org/record/7782088), which requires an internet connection. This can take a few minutes. You can set the environmental variable `PROGRES_DATA_DIR` to change where this data is stored, for example if you cannot write to the package directory. Remember to keep it set the next time you run Progres.
+5. The first time you search against the AlphaFold database TED domains the pre-embedded database (~33 GB) will be downloaded similarly. This can take a while. Make sure you have enough disk space!
+
+Alternatively, a Docker file is available in the `docker` directory.
 
 ## Usage
 
 On Unix systems the executable `progres` will be added to the path during installation.
 On Windows you can call the `bin/progres` script with python if you can't access the executable.
 
 Run `progres -h` to see the help text and `progres {mode} -h` to see the help text for each mode.
 The modes are described below but there are other options outlined in the help text.
-For example the `-d` flag sets the device to run on; this is `cpu` by default since this is usually fastest for searching, but `cuda` may be slightly faster when embedding a dataset.
+For example the `-d` flag sets the device to run on; this is `cpu` by default since this is often fastest for searching, but `cuda` may be faster when searching many queries or embedding a dataset.
 
 ## Searching a structure against a database
 
 To search a PDB file `query.pdb` against domains in the SCOPe database and print output:
 ```bash
 progres search -q query.pdb -t scope95
 ```
 ```
 # QUERY_NUM: 1
 # QUERY: query.pdb
 # QUERY_SIZE: 150 residues
 # DATABASE: scope95
-# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.1
+# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.2
 # HIT_N  DOMAIN   HIT_NRES  SIMILARITY  NOTES
       1  d1a6ja_       150      1.0000  d.112.1.1 - Nitrogen regulatory bacterial protein IIa-ntr {Escherichia coli [TaxId: 562]}
       2  d2a0ja_       146      0.9988  d.112.1.0 - automated matches {Neisseria meningitidis [TaxId: 122586]}
       3  d3urra1       151      0.9983  d.112.1.0 - automated matches {Burkholderia thailandensis [TaxId: 271848]}
       4  d3lf6a_       154      0.9971  d.112.1.1 - automated matches {Artificial gene [TaxId: 32630]}
       5  d3oxpa1       147      0.9968  d.112.1.0 - automated matches {Yersinia pestis [TaxId: 214092]}
 ...
@@ -170,7 +172,8 @@
 The trained model and pre-embedded databases are available on [Zenodo](https://zenodo.org/record/7782088).
 
 ## Notes
 
 The implementation of the E(n)-equivariant GNN uses [EGNN PyTorch](https://github.com/lucidrains/egnn-pytorch).
 
 Please open issues or [get in touch](http://jgreener64.github.io) with any feedback.
+Contributions via pull requests are welcome.
```

### Comparing `progres-0.2.1/setup.py` & `progres-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="progres",
-    version="0.2.1",
+    version="0.2.2",
     author="Joe G Greener",
     author_email="jgreener@mrc-lmb.cam.ac.uk",
     description="Fast protein structure searching using structure graph embeddings",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/greener-group/progres",
     packages=setuptools.find_packages(),
```

