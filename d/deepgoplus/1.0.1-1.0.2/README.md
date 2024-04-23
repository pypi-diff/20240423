# Comparing `tmp/deepgoplus-1.0.1.tar.gz` & `tmp/deepgoplus-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deepgoplus-1.0.1.tar", last modified: Thu Jan  7 11:47:28 2021, max compression
+gzip compressed data, was "/home/zhapacfp/Git/deepgoplus/dist/.tmp-vwtnh_ij/deepgoplus-1.0.2.tar", last modified: Tue Apr 23 08:01:41 2024, max compression
```

## Comparing `deepgoplus-1.0.1.tar` & `deepgoplus-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 kulmanm   (1000) kulmanm   (1000)        0 2021-01-07 11:47:28.000000 deepgoplus-1.0.1/
--rw-r--r--   0 kulmanm   (1000) kulmanm   (1000)     3413 2021-01-07 11:47:28.000000 deepgoplus-1.0.1/PKG-INFO
--rw-r--r--   0 kulmanm   (1000) kulmanm   (1000)     2517 2021-01-07 11:18:00.000000 deepgoplus-1.0.1/README.md
-drwxr-xr-x   0 kulmanm   (1000) kulmanm   (1000)        0 2021-01-07 11:47:28.000000 deepgoplus-1.0.1/deepgoplus/
--rw-rw-r--   0 kulmanm   (1000) kulmanm   (1000)        0 2020-08-11 11:09:04.000000 deepgoplus-1.0.1/deepgoplus/__init__.py
--rw-rw-r--   0 kulmanm   (1000) kulmanm   (1000)     1113 2020-08-11 11:09:04.000000 deepgoplus-1.0.1/deepgoplus/aminoacids.py
--rwxr-xr-x   0 kulmanm   (1000) kulmanm   (1000)     8384 2020-12-27 07:38:00.000000 deepgoplus-1.0.1/deepgoplus/main.py
--rw-rw-r--   0 kulmanm   (1000) kulmanm   (1000)     7954 2020-08-11 11:09:04.000000 deepgoplus-1.0.1/deepgoplus/utils.py
-drwxr-xr-x   0 kulmanm   (1000) kulmanm   (1000)        0 2021-01-07 11:47:28.000000 deepgoplus-1.0.1/deepgoplus.egg-info/
--rw-rw-r--   0 kulmanm   (1000) kulmanm   (1000)     3413 2021-01-07 11:47:28.000000 deepgoplus-1.0.1/deepgoplus.egg-info/PKG-INFO
--rw-rw-r--   0 kulmanm   (1000) kulmanm   (1000)      340 2021-01-07 11:47:28.000000 deepgoplus-1.0.1/deepgoplus.egg-info/SOURCES.txt
--rw-rw-r--   0 kulmanm   (1000) kulmanm   (1000)        1 2021-01-07 11:47:28.000000 deepgoplus-1.0.1/deepgoplus.egg-info/dependency_links.txt
--rw-rw-r--   0 kulmanm   (1000) kulmanm   (1000)       53 2021-01-07 11:47:28.000000 deepgoplus-1.0.1/deepgoplus.egg-info/entry_points.txt
--rw-rw-r--   0 kulmanm   (1000) kulmanm   (1000)       54 2021-01-07 11:47:28.000000 deepgoplus-1.0.1/deepgoplus.egg-info/requires.txt
--rw-rw-r--   0 kulmanm   (1000) kulmanm   (1000)       11 2021-01-07 11:47:28.000000 deepgoplus-1.0.1/deepgoplus.egg-info/top_level.txt
--rw-rw-r--   0 kulmanm   (1000) kulmanm   (1000)        1 2020-08-12 03:49:35.000000 deepgoplus-1.0.1/deepgoplus.egg-info/zip-safe
--rw-r--r--   0 kulmanm   (1000) kulmanm   (1000)       38 2021-01-07 11:47:28.000000 deepgoplus-1.0.1/setup.cfg
--rw-r--r--   0 kulmanm   (1000) kulmanm   (1000)     1385 2021-01-07 11:46:15.000000 deepgoplus-1.0.1/setup.py
+drwxrwxr-x   0 zhapacfp (178802) g-zhapacfp (1178802)        0 2024-04-23 08:01:41.000000 deepgoplus-1.0.2/
+-rw-rw-r--   0 zhapacfp (178802) g-zhapacfp (1178802)     1535 2024-03-21 14:03:45.000000 deepgoplus-1.0.2/LICENSE
+-rw-rw-r--   0 zhapacfp (178802) g-zhapacfp (1178802)     2881 2024-04-23 08:01:41.000000 deepgoplus-1.0.2/PKG-INFO
+-rw-rw-r--   0 zhapacfp (178802) g-zhapacfp (1178802)     2517 2024-03-21 14:03:45.000000 deepgoplus-1.0.2/README.md
+drwxrwxr-x   0 zhapacfp (178802) g-zhapacfp (1178802)        0 2024-04-23 08:01:41.000000 deepgoplus-1.0.2/deepgoplus/
+-rw-rw-r--   0 zhapacfp (178802) g-zhapacfp (1178802)        0 2024-03-21 14:03:45.000000 deepgoplus-1.0.2/deepgoplus/__init__.py
+-rw-rw-r--   0 zhapacfp (178802) g-zhapacfp (1178802)     1113 2024-03-21 14:03:45.000000 deepgoplus-1.0.2/deepgoplus/aminoacids.py
+-rwxrwxr-x   0 zhapacfp (178802) g-zhapacfp (1178802)     8592 2024-04-23 06:47:12.000000 deepgoplus-1.0.2/deepgoplus/main.py
+-rw-rw-r--   0 zhapacfp (178802) g-zhapacfp (1178802)     7954 2024-03-21 14:03:45.000000 deepgoplus-1.0.2/deepgoplus/utils.py
+drwxrwxr-x   0 zhapacfp (178802) g-zhapacfp (1178802)        0 2024-04-23 08:01:41.000000 deepgoplus-1.0.2/deepgoplus.egg-info/
+-rw-r--r--   0 zhapacfp (178802) g-zhapacfp (1178802)     2881 2024-04-23 08:01:41.000000 deepgoplus-1.0.2/deepgoplus.egg-info/PKG-INFO
+-rw-rw-r--   0 zhapacfp (178802) g-zhapacfp (1178802)      348 2024-04-23 08:01:41.000000 deepgoplus-1.0.2/deepgoplus.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhapacfp (178802) g-zhapacfp (1178802)        1 2024-04-23 08:01:41.000000 deepgoplus-1.0.2/deepgoplus.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhapacfp (178802) g-zhapacfp (1178802)       52 2024-04-23 08:01:41.000000 deepgoplus-1.0.2/deepgoplus.egg-info/entry_points.txt
+-rw-rw-r--   0 zhapacfp (178802) g-zhapacfp (1178802)       59 2024-04-23 08:01:41.000000 deepgoplus-1.0.2/deepgoplus.egg-info/requires.txt
+-rw-rw-r--   0 zhapacfp (178802) g-zhapacfp (1178802)       11 2024-04-23 08:01:41.000000 deepgoplus-1.0.2/deepgoplus.egg-info/top_level.txt
+-rw-rw-r--   0 zhapacfp (178802) g-zhapacfp (1178802)        1 2024-03-21 15:04:51.000000 deepgoplus-1.0.2/deepgoplus.egg-info/zip-safe
+-rw-rw-r--   0 zhapacfp (178802) g-zhapacfp (1178802)       38 2024-04-23 08:01:41.000000 deepgoplus-1.0.2/setup.cfg
+-rw-rw-r--   0 zhapacfp (178802) g-zhapacfp (1178802)     1390 2024-04-23 07:30:30.000000 deepgoplus-1.0.2/setup.py
```

### Comparing `deepgoplus-1.0.1/PKG-INFO` & `deepgoplus-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,75 @@
 Metadata-Version: 2.1
 Name: deepgoplus
-Version: 1.0.1
+Version: 1.0.2
 Summary: DeepGOPlus function predictor
-Home-page: UNKNOWN
+Download-URL: https://github.com/bio-ontology-research-group/deepgoplus/archive/v1.0.2.tar.gz
 Author: Maxat Kulmanov
 Author-email: maxat.kulmanov@kaust.edu.sa
 License: Apache 2.0
-Download-URL: https://github.com/bio-ontology-research-group/deepgoplus/archive/v1.0.1.tar.gz
-Description: # DeepGOPlus: Improved protein function prediction from sequence
-        
-        DeepGOPlus is a novel method for predicting protein functions from
-        protein sequences using deep neural networks combined with sequence
-        similarity based predictions.
-        
-        This repository contains script which were used to build and train the
-        DeepGOPlus model together with the scripts for evaluating the model's
-        performance.
-        
-        ## Dependencies
-        * The code was developed and tested using python 3.6.
-        * To install python dependencies run:
-          `pip install -r requirements.txt`
-        * Install [diamond](https://github.com/bbuchfink/diamond) program on your system (diamond command should be available)
-        
-        
-        ## Data
-        * http://deepgoplus.bio2vec.net/data/ - Here you can find the data
-        used to train and evaluate our method.
-         * data.tar.gz - Data required to run predict.sh script
-         * data-cafa.tar.gz - CAFA3 challenge dataset
-         * data-2016.tar.gz - Dataset which is used to compare DeepGOPlus with
-           GOLabeler and DeepText2GO
-        
-        ## Installation
-        `pip install deepgoplus`
-        
-        ## Running
-        * Download all the files from http://deepgoplus.bio2vec.net/data/data.tar.gz and place them into data folder
-        * `deepgoplus --data-root <path_to_data_folder> --in-file <input_fasta_filename>`
-        
-        
-        ## Scripts
-        The scripts require GeneOntology in OBO Format.
-        * uni2pandas.py - This script is used to convert data from UniProt
-        database format to pandas dataframe.
-        * deepgoplus_data.py - This script is used to generate training and
-          testing datasets.
-        * deepgoplus.py - This script is used to train the model
-        * evaluate_*.py - The scripts are used to compute Fmax, Smin and AUPR
-        
-        The online version of DeepGOPlus is available at http://deepgoplus.bio2vec.net/
-        
-        ## Citation
-        
-        If you use DeepGOPlus for your research, or incorporate our learning algorithms in your work, please cite:
-        Maxat Kulmanov, Robert Hoehndorf; DeepGOPlus: Improved protein function prediction from sequence, Bioinformatics, https://doi.org/10.1093/bioinformatics/btz595
-        
-        
-        
-        ## New version specifications
-        Current dependencies can be found in the requirements.txt file.
-        The used Python version is 3.7.9.
-        Current version of Tensorflow will require Cuda 10.1 and Cudnn 7.6.5
-        
-        
-        ## Updating
-        
-        The following scripts must be run to update the model using the latest versions of the Gene Ontology (GO) and the SwissProt Database.
-        
-        * update.py - This will download new releases of GO and SwissProt and train the model. If there are not new releases, the process will abort.
-        * new_evaluation.sh - This will compute Fmax, Smin and AUPR metrics. 
-        
-Platform: UNKNOWN
 Requires-Python: >=3.7, <3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# DeepGOPlus: Improved protein function prediction from sequence
+
+DeepGOPlus is a novel method for predicting protein functions from
+protein sequences using deep neural networks combined with sequence
+similarity based predictions.
+
+This repository contains script which were used to build and train the
+DeepGOPlus model together with the scripts for evaluating the model's
+performance.
+
+## Dependencies
+* The code was developed and tested using python 3.7.
+* To install python dependencies run:
+  `pip install -r requirements.txt`
+* Install [diamond](https://github.com/bbuchfink/diamond) program on your system (diamond command should be available)
+
+
+## Data
+* http://deepgoplus.bio2vec.net/data/ - Here you can find the data
+used to train and evaluate our method.
+ * data.tar.gz - Data required to run predict.sh script
+ * data-cafa.tar.gz - CAFA3 challenge dataset
+ * data-2016.tar.gz - Dataset which is used to compare DeepGOPlus with
+   GOLabeler and DeepText2GO
+
+## Installation
+`pip install deepgoplus`
+
+## Running
+* Download all the files from http://deepgoplus.bio2vec.net/data/data.tar.gz and place them into data folder
+* `deepgoplus --data-root <path_to_data_folder> --in-file <input_fasta_filename>`
+
+
+## Scripts
+The scripts require GeneOntology in OBO Format.
+* uni2pandas.py - This script is used to convert data from UniProt
+database format to pandas dataframe.
+* deepgoplus_data.py - This script is used to generate training and
+  testing datasets.
+* deepgoplus.py - This script is used to train the model
+* evaluate_*.py - The scripts are used to compute Fmax, Smin and AUPR
+
+The online version of DeepGOPlus is available at http://deepgoplus.bio2vec.net/
+
+## Citation
+
+If you use DeepGOPlus for your research, or incorporate our learning algorithms in your work, please cite:
+Maxat Kulmanov, Robert Hoehndorf; DeepGOPlus: Improved protein function prediction from sequence, Bioinformatics, https://doi.org/10.1093/bioinformatics/btz595
+
+
+
+## New version specifications
+Current dependencies can be found in the requirements.txt file.
+The used Python version is 3.7.9.
+Current version of Tensorflow will require Cuda 10.1 and Cudnn 7.6.5
+
+
+## Updating
+
+The following scripts must be run to update the model using the latest versions of the Gene Ontology (GO) and the SwissProt Database.
+
+* update.py - This will download new releases of GO and SwissProt and train the model. If there are not new releases, the process will abort.
+* new_evaluation.sh - This will compute Fmax, Smin and AUPR metrics.
```

### Comparing `deepgoplus-1.0.1/README.md` & `deepgoplus-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 similarity based predictions.
 
 This repository contains script which were used to build and train the
 DeepGOPlus model together with the scripts for evaluating the model's
 performance.
 
 ## Dependencies
-* The code was developed and tested using python 3.6.
+* The code was developed and tested using python 3.7.
 * To install python dependencies run:
   `pip install -r requirements.txt`
 * Install [diamond](https://github.com/bbuchfink/diamond) program on your system (diamond command should be available)
 
 
 ## Data
 * http://deepgoplus.bio2vec.net/data/ - Here you can find the data
```

### Comparing `deepgoplus-1.0.1/deepgoplus/aminoacids.py` & `deepgoplus-1.0.2/deepgoplus/aminoacids.py`

 * *Files identical despite different names*

### Comparing `deepgoplus-1.0.1/deepgoplus/main.py` & `deepgoplus-1.0.2/deepgoplus/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from deepgoplus.utils import Ontology, NAMESPACES
 from deepgoplus.aminoacids import to_onehot
 import gzip
 import os
 import sys
 import logging
 import subprocess
+import json
 
 MAXLEN = 2000
 
 @ck.command()
 @ck.option('--data-root', '-dr', default='data/', help='Data root folder', required=True)
 @ck.option('--in-file', '-if', help='Input FASTA file', required=True)
 @ck.option('--out-file', '-of', default='results.tsv', help='Output result file')
@@ -58,19 +59,26 @@
         sys.exit(1)
 
     # Load GO and read list of all terms
     go = Ontology(go_file, with_rels=True)
     terms_df = pd.read_pickle(terms_file)
     terms = terms_df['terms'].values.flatten()
 
+    #Load alphas
+    with open(os.path.join(data_root, 'metadata/last_release.json')) as f:
+        metadata = json.load(f)
+        alphas = metadata['alphas']
+
+    
+    
     # Read known experimental annotations
     annotations = {}
     df = pd.read_pickle(annotations_file)
     for row in df.itertuples():
-        annotations[row.proteins] = set(row.exp_annotations)
+        annotations[row.proteins] = set(row.prop_annotations)
 
     # Generate diamond predictions
     cmd = [
         "diamond", "blastp",  "-d", diamond_db, "--more-sensitive", "-t", "/tmp",
         "-q", in_file, "--outfmt", "6", "qseqid", "sseqid", "bitscore", "-o",
         diamond_file]
     proc = subprocess.run(cmd)
@@ -105,15 +113,15 @@
         for go_id, score in zip(allgos, sim):
             annots[go_id] = score
         diamond_preds[prot_id] = annots
     
     # Load CNN model
     model = load_model(model_file)
     # Alphas for the latest model
-    alphas = {NAMESPACES['mf']: 0.55, NAMESPACES['bp']: 0.59, NAMESPACES['cc']: 0.46}
+    alphas = {NAMESPACES['mf']: alphas["mf"], NAMESPACES['bp']: alphas["bp"], NAMESPACES['cc']: alphas["cc"]}
     # Alphas for the cafa2 model
     # alphas = {NAMESPACES['mf']: 0.63, NAMESPACES['bp']: 0.68, NAMESPACES['cc']: 0.48}
     
     start_time = time.time()
     total_seq = 0
     w = open(out_file, 'w')
     for prot_ids, sequences in read_fasta(in_file, chunk_size):
```

### Comparing `deepgoplus-1.0.1/deepgoplus/utils.py` & `deepgoplus-1.0.2/deepgoplus/utils.py`

 * *Files identical despite different names*

### Comparing `deepgoplus-1.0.1/deepgoplus.egg-info/PKG-INFO` & `deepgoplus-1.0.2/deepgoplus.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,75 @@
 Metadata-Version: 2.1
 Name: deepgoplus
-Version: 1.0.1
+Version: 1.0.2
 Summary: DeepGOPlus function predictor
-Home-page: UNKNOWN
+Download-URL: https://github.com/bio-ontology-research-group/deepgoplus/archive/v1.0.2.tar.gz
 Author: Maxat Kulmanov
 Author-email: maxat.kulmanov@kaust.edu.sa
 License: Apache 2.0
-Download-URL: https://github.com/bio-ontology-research-group/deepgoplus/archive/v1.0.1.tar.gz
-Description: # DeepGOPlus: Improved protein function prediction from sequence
-        
-        DeepGOPlus is a novel method for predicting protein functions from
-        protein sequences using deep neural networks combined with sequence
-        similarity based predictions.
-        
-        This repository contains script which were used to build and train the
-        DeepGOPlus model together with the scripts for evaluating the model's
-        performance.
-        
-        ## Dependencies
-        * The code was developed and tested using python 3.6.
-        * To install python dependencies run:
-          `pip install -r requirements.txt`
-        * Install [diamond](https://github.com/bbuchfink/diamond) program on your system (diamond command should be available)
-        
-        
-        ## Data
-        * http://deepgoplus.bio2vec.net/data/ - Here you can find the data
-        used to train and evaluate our method.
-         * data.tar.gz - Data required to run predict.sh script
-         * data-cafa.tar.gz - CAFA3 challenge dataset
-         * data-2016.tar.gz - Dataset which is used to compare DeepGOPlus with
-           GOLabeler and DeepText2GO
-        
-        ## Installation
-        `pip install deepgoplus`
-        
-        ## Running
-        * Download all the files from http://deepgoplus.bio2vec.net/data/data.tar.gz and place them into data folder
-        * `deepgoplus --data-root <path_to_data_folder> --in-file <input_fasta_filename>`
-        
-        
-        ## Scripts
-        The scripts require GeneOntology in OBO Format.
-        * uni2pandas.py - This script is used to convert data from UniProt
-        database format to pandas dataframe.
-        * deepgoplus_data.py - This script is used to generate training and
-          testing datasets.
-        * deepgoplus.py - This script is used to train the model
-        * evaluate_*.py - The scripts are used to compute Fmax, Smin and AUPR
-        
-        The online version of DeepGOPlus is available at http://deepgoplus.bio2vec.net/
-        
-        ## Citation
-        
-        If you use DeepGOPlus for your research, or incorporate our learning algorithms in your work, please cite:
-        Maxat Kulmanov, Robert Hoehndorf; DeepGOPlus: Improved protein function prediction from sequence, Bioinformatics, https://doi.org/10.1093/bioinformatics/btz595
-        
-        
-        
-        ## New version specifications
-        Current dependencies can be found in the requirements.txt file.
-        The used Python version is 3.7.9.
-        Current version of Tensorflow will require Cuda 10.1 and Cudnn 7.6.5
-        
-        
-        ## Updating
-        
-        The following scripts must be run to update the model using the latest versions of the Gene Ontology (GO) and the SwissProt Database.
-        
-        * update.py - This will download new releases of GO and SwissProt and train the model. If there are not new releases, the process will abort.
-        * new_evaluation.sh - This will compute Fmax, Smin and AUPR metrics. 
-        
-Platform: UNKNOWN
 Requires-Python: >=3.7, <3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# DeepGOPlus: Improved protein function prediction from sequence
+
+DeepGOPlus is a novel method for predicting protein functions from
+protein sequences using deep neural networks combined with sequence
+similarity based predictions.
+
+This repository contains script which were used to build and train the
+DeepGOPlus model together with the scripts for evaluating the model's
+performance.
+
+## Dependencies
+* The code was developed and tested using python 3.7.
+* To install python dependencies run:
+  `pip install -r requirements.txt`
+* Install [diamond](https://github.com/bbuchfink/diamond) program on your system (diamond command should be available)
+
+
+## Data
+* http://deepgoplus.bio2vec.net/data/ - Here you can find the data
+used to train and evaluate our method.
+ * data.tar.gz - Data required to run predict.sh script
+ * data-cafa.tar.gz - CAFA3 challenge dataset
+ * data-2016.tar.gz - Dataset which is used to compare DeepGOPlus with
+   GOLabeler and DeepText2GO
+
+## Installation
+`pip install deepgoplus`
+
+## Running
+* Download all the files from http://deepgoplus.bio2vec.net/data/data.tar.gz and place them into data folder
+* `deepgoplus --data-root <path_to_data_folder> --in-file <input_fasta_filename>`
+
+
+## Scripts
+The scripts require GeneOntology in OBO Format.
+* uni2pandas.py - This script is used to convert data from UniProt
+database format to pandas dataframe.
+* deepgoplus_data.py - This script is used to generate training and
+  testing datasets.
+* deepgoplus.py - This script is used to train the model
+* evaluate_*.py - The scripts are used to compute Fmax, Smin and AUPR
+
+The online version of DeepGOPlus is available at http://deepgoplus.bio2vec.net/
+
+## Citation
+
+If you use DeepGOPlus for your research, or incorporate our learning algorithms in your work, please cite:
+Maxat Kulmanov, Robert Hoehndorf; DeepGOPlus: Improved protein function prediction from sequence, Bioinformatics, https://doi.org/10.1093/bioinformatics/btz595
+
+
+
+## New version specifications
+Current dependencies can be found in the requirements.txt file.
+The used Python version is 3.7.9.
+Current version of Tensorflow will require Cuda 10.1 and Cudnn 7.6.5
+
+
+## Updating
+
+The following scripts must be run to update the model using the latest versions of the Gene Ontology (GO) and the SwissProt Database.
+
+* update.py - This will download new releases of GO and SwissProt and train the model. If there are not new releases, the process will abort.
+* new_evaluation.sh - This will compute Fmax, Smin and AUPR metrics.
```

### Comparing `deepgoplus-1.0.1/setup.py` & `deepgoplus-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,30 @@
     import gittaggers
 
     tagger = gittaggers.EggInfoFromGit
 except ImportError:
     tagger = egg_info_cmd.egg_info
 
 install_requires = [
-    "click < 8", "sklearn", "pandas", "tensorflow < 2.4",
+    "click < 8", "scikit-learn", "pandas", "tensorflow < 2.4",
     "numpy < 2.0", "scipy" 
 ]
 
 needs_pytest = {"pytest", "test", "ptr"}.intersection(sys.argv)
 pytest_runner = ["pytest < 6", "pytest-runner < 5"] if needs_pytest else []
 
 setup(
     name="deepgoplus",
-    version="1.0.1",
+    version="1.0.2",
     description="DeepGOPlus function predictor",
     long_description=open(README).read(),
     long_description_content_type="text/markdown",
     author="Maxat Kulmanov",
     author_email="maxat.kulmanov@kaust.edu.sa",
-    download_url="https://github.com/bio-ontology-research-group/deepgoplus/archive/v1.0.1.tar.gz",
+    download_url="https://github.com/bio-ontology-research-group/deepgoplus/archive/v1.0.2.tar.gz",
     license="Apache 2.0",
     packages=["deepgoplus",],
     package_data={"deepgoplus": [],},
     install_requires=install_requires,
     extras_require={},
     setup_requires=[] + pytest_runner,
     tests_require=["pytest<5"],
```

