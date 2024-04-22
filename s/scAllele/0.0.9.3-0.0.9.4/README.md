# Comparing `tmp/scAllele-0.0.9.3.tar.gz` & `tmp/scallele-0.0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/u/project/gxxiao4/giovas/projects/scAllele/scAllele_packaging_v2/dist/.tmp-az9m9azo/scAllele-0.0.9.3.tar", last modified: Tue Mar  7 07:01:10 2023, max compression
+gzip compressed data, was "scallele-0.0.9.4.tar", last modified: Mon Apr 22 21:50:26 2024, max compression
```

## Comparing `scAllele-0.0.9.3.tar` & `scallele-0.0.9.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 giovas   (11935) gxxiao    (8285)        0 2023-03-07 07:01:10.796974 scAllele-0.0.9.3/
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)     1291 2023-03-07 06:46:16.000000 scAllele-0.0.9.3/LICENSE
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)    11352 2023-03-07 07:01:10.796850 scAllele-0.0.9.3/PKG-INFO
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)    10791 2023-03-07 07:00:49.000000 scAllele-0.0.9.3/README.md
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)      104 2022-05-18 22:25:41.000000 scAllele-0.0.9.3/pyproject.toml
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)     1080 2023-03-07 07:01:10.800960 scAllele-0.0.9.3/setup.cfg
-drwxr-xr-x   0 giovas   (11935) gxxiao    (8285)        0 2023-03-07 07:01:10.696558 scAllele-0.0.9.3/src/
-drwxr-xr-x   0 giovas   (11935) gxxiao    (8285)        0 2023-03-07 07:01:10.739969 scAllele-0.0.9.3/src/scAllele/
--rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)        0 2022-04-04 01:59:03.000000 scAllele-0.0.9.3/src/scAllele/__init__.py
-drwxr-xr-x   0 giovas   (11935) gxxiao    (8285)        0 2023-03-07 07:01:10.794124 scAllele-0.0.9.3/src/scAllele/glm/
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)      779 2022-05-17 21:03:29.000000 scAllele-0.0.9.3/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.DELETION.glm.pickle
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)      779 2022-05-17 21:03:29.000000 scAllele-0.0.9.3/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.INSERTION.glm.pickle
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)      779 2022-05-17 21:03:29.000000 scAllele-0.0.9.3/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.SNP.glm.pickle
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)      757 2022-05-17 21:03:29.000000 scAllele-0.0.9.3/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.SNV.glm.pickle
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)        0 2022-04-04 01:59:03.000000 scAllele-0.0.9.3/src/scAllele/glm/__init__.py
--rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)    13311 2022-05-21 23:27:51.000000 scAllele-0.0.9.3/src/scAllele/gqv_bam_utils.py
--rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)    20753 2022-05-22 00:04:14.000000 scAllele-0.0.9.3/src/scAllele/gqv_dbg_utils.py
--rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)     9204 2023-03-07 06:25:08.000000 scAllele-0.0.9.3/src/scAllele/gqv_glm.py
--rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)     7622 2022-05-18 20:45:52.000000 scAllele-0.0.9.3/src/scAllele/gqv_mutual_information.py
--rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)     1845 2022-05-19 21:02:37.000000 scAllele-0.0.9.3/src/scAllele/gqv_software_management.py
--rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)    52264 2022-09-20 21:56:42.000000 scAllele-0.0.9.3/src/scAllele/gqv_utils.py
--rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)    22943 2022-05-18 18:50:47.000000 scAllele-0.0.9.3/src/scAllele/gqv_vartool.py
--rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)    14458 2023-03-07 06:58:50.000000 scAllele-0.0.9.3/src/scAllele/scAllele.py
-drwxr-xr-x   0 giovas   (11935) gxxiao    (8285)        0 2023-03-07 07:01:10.776122 scAllele-0.0.9.3/src/scAllele.egg-info/
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)    11352 2023-03-07 07:01:10.000000 scAllele-0.0.9.3/src/scAllele.egg-info/PKG-INFO
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)      859 2023-03-07 07:01:10.000000 scAllele-0.0.9.3/src/scAllele.egg-info/SOURCES.txt
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)        1 2023-03-07 07:01:10.000000 scAllele-0.0.9.3/src/scAllele.egg-info/dependency_links.txt
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)       91 2023-03-07 07:01:10.000000 scAllele-0.0.9.3/src/scAllele.egg-info/entry_points.txt
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)      177 2023-03-07 07:01:10.000000 scAllele-0.0.9.3/src/scAllele.egg-info/requires.txt
--rw-r--r--   0 giovas   (11935) gxxiao    (8285)        9 2023-03-07 07:01:10.000000 scAllele-0.0.9.3/src/scAllele.egg-info/top_level.txt
+drwxr-xr-x   0 giovas   (11935) gxxiao    (8285)        0 2024-04-22 21:50:26.469977 scallele-0.0.9.4/
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)     1291 2023-03-07 06:46:16.000000 scallele-0.0.9.4/LICENSE
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)    11868 2024-04-22 21:50:26.467431 scallele-0.0.9.4/PKG-INFO
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)    10914 2023-03-07 09:09:23.000000 scallele-0.0.9.4/README.md
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)      104 2022-05-18 22:25:41.000000 scallele-0.0.9.4/pyproject.toml
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)     1072 2024-04-22 21:50:26.476523 scallele-0.0.9.4/setup.cfg
+drwxr-xr-x   0 giovas   (11935) gxxiao    (8285)        0 2024-04-22 21:50:26.305758 scallele-0.0.9.4/src/
+drwxr-xr-x   0 giovas   (11935) gxxiao    (8285)        0 2024-04-22 21:50:26.391670 scallele-0.0.9.4/src/scAllele/
+-rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)        0 2022-04-04 01:59:03.000000 scallele-0.0.9.4/src/scAllele/__init__.py
+drwxr-xr-x   0 giovas   (11935) gxxiao    (8285)        0 2024-04-22 21:50:26.454426 scallele-0.0.9.4/src/scAllele/glm/
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)      779 2022-05-17 21:03:29.000000 scallele-0.0.9.4/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.DELETION.glm.pickle
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)      779 2022-05-17 21:03:29.000000 scallele-0.0.9.4/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.INSERTION.glm.pickle
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)      779 2022-05-17 21:03:29.000000 scallele-0.0.9.4/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.SNP.glm.pickle
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)      757 2022-05-17 21:03:29.000000 scallele-0.0.9.4/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.SNV.glm.pickle
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)        0 2022-04-04 01:59:03.000000 scallele-0.0.9.4/src/scAllele/glm/__init__.py
+-rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)    13311 2022-05-21 23:27:51.000000 scallele-0.0.9.4/src/scAllele/gqv_bam_utils.py
+-rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)    20753 2022-05-22 00:04:14.000000 scallele-0.0.9.4/src/scAllele/gqv_dbg_utils.py
+-rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)     9204 2023-03-07 06:25:08.000000 scallele-0.0.9.4/src/scAllele/gqv_glm.py
+-rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)     7622 2022-05-18 20:45:52.000000 scallele-0.0.9.4/src/scAllele/gqv_mutual_information.py
+-rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)     1845 2022-05-19 21:02:37.000000 scallele-0.0.9.4/src/scAllele/gqv_software_management.py
+-rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)    52542 2024-04-22 20:22:42.000000 scallele-0.0.9.4/src/scAllele/gqv_utils.py
+-rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)    22953 2024-04-22 21:50:04.000000 scallele-0.0.9.4/src/scAllele/gqv_vartool.py
+-rwxr-xr-x   0 giovas   (11935) gxxiao    (8285)    14520 2024-04-22 20:15:36.000000 scallele-0.0.9.4/src/scAllele/scAllele.py
+drwxr-xr-x   0 giovas   (11935) gxxiao    (8285)        0 2024-04-22 21:50:26.460426 scallele-0.0.9.4/src/scAllele.egg-info/
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)    11868 2024-04-22 21:50:26.000000 scallele-0.0.9.4/src/scAllele.egg-info/PKG-INFO
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)      859 2024-04-22 21:50:26.000000 scallele-0.0.9.4/src/scAllele.egg-info/SOURCES.txt
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)        1 2024-04-22 21:50:26.000000 scallele-0.0.9.4/src/scAllele.egg-info/dependency_links.txt
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)       91 2024-04-22 21:50:26.000000 scallele-0.0.9.4/src/scAllele.egg-info/entry_points.txt
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)      169 2024-04-22 21:50:26.000000 scallele-0.0.9.4/src/scAllele.egg-info/requires.txt
+-rw-r--r--   0 giovas   (11935) gxxiao    (8285)        9 2024-04-22 21:50:26.000000 scallele-0.0.9.4/src/scAllele.egg-info/top_level.txt
```

### Comparing `scAllele-0.0.9.3/LICENSE` & `scallele-0.0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scAllele-0.0.9.3/PKG-INFO` & `scallele-0.0.9.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: scAllele
-Version: 0.0.9.3
-Summary: A versatile tool for the detection and analysis of nucleotide variants in scRNA-seq
-Home-page: https://github.com/gxiaolab/scAllele
-Author: Giovanni Quinones Valdez
-Author-email: giovas@ucla.edu
-Project-URL: Bug Tracker, https://github.com/gxiaolab/scAllele/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # **scAllele**
 _______________________________________
 [![](https://img.shields.io/badge/scAllele-v0.0.9.3-blue)](https://test.pypi.org/project/scAllele/)
 
 [Github](https://github.com/gxiaolab/scAllele/)
 
 ## **About**
@@ -26,15 +11,15 @@
 scAllele makes use local reassembly via de-Bruijn graph to identify sequence differences and infers nucleotide variants at the read level. \
 The read level variant-call allows for the analysis of the role variants in the context of splicing. 
 Using mutual information, scAllele identifies allelic linkage between nucleotide variants and splicing
 isoforms.
 
 ## **Table of contents**
 - [Outline](#Outline)
-- [Download](#Download)
+- [Installation](#Installation)
 - [Usage](#Usage)
 	- [Basic usage](#Basic-usage)
 	- [Preprocessing](#Preprocessing)
 	- [Stranded data](#Stranded-data)
 	- [Local variant call](#Local-variant-call)
 	- [Filtering variants](#Filtering-variants)
 	- [Training a new classifier](#Training-a-new-classifier)
@@ -47,27 +32,51 @@
 
 | ![alt text](img/screenshot_Fig1.png) |
 |:--:|
 | *a. Illustration of the main algorithm of scAllele for variant calling. The reads and the reference genomic sequence overlapping a read cluster (RC) are decomposed into k-mers and are reasembled into a de Bruijn graph. b. Variants (green box in a) identified from the graph are then scored using a generalized linear model (GLM). The GLM was trained with different features (green box) to assign a confidence score to the variants. c. To identify allele-specific splicing (i.e., variant linkage), scAllele performs a mutual information calculation between nucleotide variants (SNVs, microindels) and intronic parts (where the ‘alleles’ are the different overlapping introns), to calculate allelic linkage of splicing isoforms.* |  
 
 _______________________________________
 
-## **Download**
+## **Installation**
+
+scAllele is available through **PyPi**. To download simply type:
+
+```
+pip install scAllele
+```
+
+The download was tested with PyPi version >= 20.0.1.
+
+Alternatively, you can clone this **GitHub** repository:
+
+```
+git clone git@github.com:gxiaolab/scAllele.git 
+pip install .
+```
 
-scAllele is available through PyPi. To download simply type:
+Or
 
 ```
-$ pip install scAllele
+git clone https://github.com/gxiaolab/scAllele.git
+pip install .
 ```
 
-The download was tested with PyPi version >= 20.0.1
+You can also download the **Singularity** container:
+
+```
+singularity pull library://giovas/collection/s5
+# run
+singularity exec s5_latest.sif scAllele
+```
 
 If succesful, the program is ready to use. The installation incorporates console script entrypoints to directly call scAllele:
+
 ```
-$ scAllele
+scAllele
+
 Usage: 
 	scAllele -b <file.bam> -g <genome.fa> -o <output prefix>
 A variant caller and variant analysis tool for scRNA-seq data.
 Options:
   -h, --help            show this help message and exit
   -b INPUT_BAM, --input-bam=INPUT_BAM
                         [Required] Input bam file, (or comma-seprated list of
@@ -131,21 +140,21 @@
 
 The minimum requirements to run scAllele are:
 1. A bam file (sorted and indexed) `samtools sort file.bam file.sorted ; samtools index file.sorted.bam` 
 2. A reference genome fasta file (indexed) `samtools faidx genome.fa`
 3. A prefix for the output files.
 
 ```
-$ scAllele -b file.sorted.bam -g genome.fa -o path/to/output_prefix
+scAllele -b file.sorted.bam -g genome.fa -o path/to/output_prefix
 ```
 
 Using the provided test data: 
 
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
 ```
 
 
 ### *Preprocessing* 
@@ -157,98 +166,99 @@
 | *Recommended pipeline* |
 
 ### *Stranded data*
 If your scRNA-seq is strand-specific, then you can specify the strandedness of your data (default: non-strand specific). \
 Strand-specific data helps resolve ambiguous alignments on overlapping genes. It also helps detect more accurate ASAS events. \
 Most strand-specific libraries in RNA-Seq are `fr-firststrand` (second read pair is sense to the RNA). You can specify this in your command:
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
     --strandedness='fr-firststrand'
 ```
 Alternatively, you can use the option `--strandedness=fr-secondstrand` if the first read pair is sense to the RNA.  
 
 ### *Local variant call*
 By default, scAllele searches for variants in all the regions of the transcriptome covered by reads. If you wish to search for variants in a custom genomic interval, you can do so with the `-c` option. 
 ```
 ## Only search chromosome 21
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
     -c chr21
 ## Only search within these coordinates
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
     -c chr21:34582111-34628004
 ```
 
 scAllele will search for read clusters within these regions only. Bare in mind that it's possible to find no read clusters in the spcified region, and that, if a specified region does not contain the entirety of a gene, it may miss some ASAS events. 
 
 
 ### *Filtering variants* 
 
 Although it is recommended to filter variants downstream of your analysis (via bcftools or others), it's possible to filter variants from the start. If you wish, for example, to only report variants with 3 reads supporting the alternative allele (AC) and 5 reads overall, then you can run the following command:
 
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
     --AC=3 
     --DP=5
 ```
 
 The default is `AC=2 and DP=2`. 
 
 ### *Training a new classifier* 
 
 scAllele offers the option to retrain the variant classifier. Sequencing data from different platforms or resulting from different library preparation protocols may have different error profiles. If you wish to retrain scAllele's classifier run it in training mode: 
 
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/new_clf 
     --run_mode='Training' 
 ```
 
 This will return a feature file (`.feature_matrix.tab`) containing the variant calls and all the features used for the training of the classifier.  
 Then, run scAllele's training function. The supervised classifier will require a set of ground-truth variants to fit the model.  
 
 ```
-$ scAllele_train 
+scAllele_train 
     -i path/to/new_clf.feature_matrix.tab 
     -v truth.vcf 
     -g testdata/hg38.chr21.fa
 ```
 
 This will return 3 pickle objects:
 
 * path/to/new_clf.feature_matrix.tab.DELETION.glm.pickle
 * path/to/new_clf.feature_matrix.tab.INSERTION.glm.pickle
 * path/to/new_clf.feature_matrix.tab.SNP.glm.pickle
 
 Finally, to use these new classifiers to call variants run:
 
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o new_path/to/output_prefix 
     --glm_clf_name path/to/new_clf.feature_matrix.tab  
 ```
 
 _____________________________________
 
 
+
 ## **Output**
 
 scAllele generates 4 files as output:
 
 * path/to/output_prefix.vcf
 * path/to/output_prefix.mi_summary.tab
 * path/to/output_prefix.read_cluster_info.tab
@@ -272,14 +282,7 @@
 ```
 
 If one or more dependencies fail to install, make sure you have the latest version of pip:
 
 ```
 pip install --upgrade pip
 ```
-
-If the error persists, download the `requires.txt` file from this repository and install the dependencies prior to scAllele installation:
-
-```
-pip install -r requires.txt
-pip install -i https://test.pypi.org/simple/ scAllele==0.0.9.3
-```
```

### Comparing `scAllele-0.0.9.3/README.md` & `scallele-0.0.9.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: scAllele
+Version: 0.0.9.4
+Summary: A versatile tool for the detection and analysis of nucleotide variants in scRNA-seq
+Home-page: https://github.com/gxiaolab/scAllele
+Author: Giovanni Quinones Valdez
+Author-email: giovas@ucla.edu
+Project-URL: Bug Tracker, https://github.com/gxiaolab/scAllele/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: biopython
+Requires-Dist: glob2
+Requires-Dist: HTSeq
+Requires-Dist: multiprocess
+Requires-Dist: networkx>=2.4
+Requires-Dist: numpy
+Requires-Dist: pandas>=1.3
+Requires-Dist: pickleshare
+Requires-Dist: psutil
+Requires-Dist: pyfaidx>=0.5.9.5
+Requires-Dist: pysam>=0.9.1
+Requires-Dist: vcfpy
+Requires-Dist: scikit-learn>=0.23.1
+Requires-Dist: scipy
+Requires-Dist: statsmodels>=0.11.1
+
 # **scAllele**
 _______________________________________
 [![](https://img.shields.io/badge/scAllele-v0.0.9.3-blue)](https://test.pypi.org/project/scAllele/)
 
 [Github](https://github.com/gxiaolab/scAllele/)
 
 ## **About**
@@ -11,15 +41,15 @@
 scAllele makes use local reassembly via de-Bruijn graph to identify sequence differences and infers nucleotide variants at the read level. \
 The read level variant-call allows for the analysis of the role variants in the context of splicing. 
 Using mutual information, scAllele identifies allelic linkage between nucleotide variants and splicing
 isoforms.
 
 ## **Table of contents**
 - [Outline](#Outline)
-- [Download](#Download)
+- [Installation](#Installation)
 - [Usage](#Usage)
 	- [Basic usage](#Basic-usage)
 	- [Preprocessing](#Preprocessing)
 	- [Stranded data](#Stranded-data)
 	- [Local variant call](#Local-variant-call)
 	- [Filtering variants](#Filtering-variants)
 	- [Training a new classifier](#Training-a-new-classifier)
@@ -32,27 +62,51 @@
 
 | ![alt text](img/screenshot_Fig1.png) |
 |:--:|
 | *a. Illustration of the main algorithm of scAllele for variant calling. The reads and the reference genomic sequence overlapping a read cluster (RC) are decomposed into k-mers and are reasembled into a de Bruijn graph. b. Variants (green box in a) identified from the graph are then scored using a generalized linear model (GLM). The GLM was trained with different features (green box) to assign a confidence score to the variants. c. To identify allele-specific splicing (i.e., variant linkage), scAllele performs a mutual information calculation between nucleotide variants (SNVs, microindels) and intronic parts (where the ‘alleles’ are the different overlapping introns), to calculate allelic linkage of splicing isoforms.* |  
 
 _______________________________________
 
-## **Download**
+## **Installation**
+
+scAllele is available through **PyPi**. To download simply type:
+
+```
+pip install scAllele
+```
+
+The download was tested with PyPi version >= 20.0.1.
+
+Alternatively, you can clone this **GitHub** repository:
+
+```
+git clone git@github.com:gxiaolab/scAllele.git 
+pip install .
+```
 
-scAllele is available through PyPi. To download simply type:
+Or
 
 ```
-$ pip install scAllele
+git clone https://github.com/gxiaolab/scAllele.git
+pip install .
 ```
 
-The download was tested with PyPi version >= 20.0.1
+You can also download the **Singularity** container:
+
+```
+singularity pull library://giovas/collection/s5
+# run
+singularity exec s5_latest.sif scAllele
+```
 
 If succesful, the program is ready to use. The installation incorporates console script entrypoints to directly call scAllele:
+
 ```
-$ scAllele
+scAllele
+
 Usage: 
 	scAllele -b <file.bam> -g <genome.fa> -o <output prefix>
 A variant caller and variant analysis tool for scRNA-seq data.
 Options:
   -h, --help            show this help message and exit
   -b INPUT_BAM, --input-bam=INPUT_BAM
                         [Required] Input bam file, (or comma-seprated list of
@@ -116,21 +170,21 @@
 
 The minimum requirements to run scAllele are:
 1. A bam file (sorted and indexed) `samtools sort file.bam file.sorted ; samtools index file.sorted.bam` 
 2. A reference genome fasta file (indexed) `samtools faidx genome.fa`
 3. A prefix for the output files.
 
 ```
-$ scAllele -b file.sorted.bam -g genome.fa -o path/to/output_prefix
+scAllele -b file.sorted.bam -g genome.fa -o path/to/output_prefix
 ```
 
 Using the provided test data: 
 
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
 ```
 
 
 ### *Preprocessing* 
@@ -142,98 +196,99 @@
 | *Recommended pipeline* |
 
 ### *Stranded data*
 If your scRNA-seq is strand-specific, then you can specify the strandedness of your data (default: non-strand specific). \
 Strand-specific data helps resolve ambiguous alignments on overlapping genes. It also helps detect more accurate ASAS events. \
 Most strand-specific libraries in RNA-Seq are `fr-firststrand` (second read pair is sense to the RNA). You can specify this in your command:
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
     --strandedness='fr-firststrand'
 ```
 Alternatively, you can use the option `--strandedness=fr-secondstrand` if the first read pair is sense to the RNA.  
 
 ### *Local variant call*
 By default, scAllele searches for variants in all the regions of the transcriptome covered by reads. If you wish to search for variants in a custom genomic interval, you can do so with the `-c` option. 
 ```
 ## Only search chromosome 21
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
     -c chr21
 ## Only search within these coordinates
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
     -c chr21:34582111-34628004
 ```
 
 scAllele will search for read clusters within these regions only. Bare in mind that it's possible to find no read clusters in the spcified region, and that, if a specified region does not contain the entirety of a gene, it may miss some ASAS events. 
 
 
 ### *Filtering variants* 
 
 Although it is recommended to filter variants downstream of your analysis (via bcftools or others), it's possible to filter variants from the start. If you wish, for example, to only report variants with 3 reads supporting the alternative allele (AC) and 5 reads overall, then you can run the following command:
 
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
     --AC=3 
     --DP=5
 ```
 
 The default is `AC=2 and DP=2`. 
 
 ### *Training a new classifier* 
 
 scAllele offers the option to retrain the variant classifier. Sequencing data from different platforms or resulting from different library preparation protocols may have different error profiles. If you wish to retrain scAllele's classifier run it in training mode: 
 
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/new_clf 
     --run_mode='Training' 
 ```
 
 This will return a feature file (`.feature_matrix.tab`) containing the variant calls and all the features used for the training of the classifier.  
 Then, run scAllele's training function. The supervised classifier will require a set of ground-truth variants to fit the model.  
 
 ```
-$ scAllele_train 
+scAllele_train 
     -i path/to/new_clf.feature_matrix.tab 
     -v truth.vcf 
     -g testdata/hg38.chr21.fa
 ```
 
 This will return 3 pickle objects:
 
 * path/to/new_clf.feature_matrix.tab.DELETION.glm.pickle
 * path/to/new_clf.feature_matrix.tab.INSERTION.glm.pickle
 * path/to/new_clf.feature_matrix.tab.SNP.glm.pickle
 
 Finally, to use these new classifiers to call variants run:
 
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o new_path/to/output_prefix 
     --glm_clf_name path/to/new_clf.feature_matrix.tab  
 ```
 
 _____________________________________
 
 
+
 ## **Output**
 
 scAllele generates 4 files as output:
 
 * path/to/output_prefix.vcf
 * path/to/output_prefix.mi_summary.tab
 * path/to/output_prefix.read_cluster_info.tab
@@ -257,14 +312,7 @@
 ```
 
 If one or more dependencies fail to install, make sure you have the latest version of pip:
 
 ```
 pip install --upgrade pip
 ```
-
-If the error persists, download the `requires.txt` file from this repository and install the dependencies prior to scAllele installation:
-
-```
-pip install -r requires.txt
-pip install -i https://test.pypi.org/simple/ scAllele==0.0.9.3
-```
```

### Comparing `scAllele-0.0.9.3/setup.cfg` & `scallele-0.0.9.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scAllele
-version = 0.0.9.3
+version = 0.0.9.4
 author = Giovanni Quinones Valdez
 author_email = giovas@ucla.edu
 description = A versatile tool for the detection and analysis of nucleotide variants in scRNA-seq
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/gxiaolab/scAllele
 project_urls = 
@@ -22,16 +22,16 @@
 python_requires = >=3.8
 install_requires = 
 	biopython
 	glob2
 	HTSeq
 	multiprocess
 	networkx>=2.4
-	numpy>=1.18.5
-	pandas==1.3
+	numpy
+	pandas>=1.3
 	pickleshare
 	psutil
 	pyfaidx>=0.5.9.5
 	pysam>=0.9.1
 	vcfpy
 	scikit-learn>=0.23.1
 	scipy
```

### Comparing `scAllele-0.0.9.3/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.DELETION.glm.pickle` & `scallele-0.0.9.4/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.DELETION.glm.pickle`

 * *Files identical despite different names*

### Comparing `scAllele-0.0.9.3/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.INSERTION.glm.pickle` & `scallele-0.0.9.4/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.INSERTION.glm.pickle`

 * *Files identical despite different names*

### Comparing `scAllele-0.0.9.3/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.SNP.glm.pickle` & `scallele-0.0.9.4/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.SNP.glm.pickle`

 * *Files identical despite different names*

### Comparing `scAllele-0.0.9.3/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.SNV.glm.pickle` & `scallele-0.0.9.4/src/scAllele/glm/GM12878_smartseq2.all.feature_matrix.tab.SNV.glm.pickle`

 * *Files identical despite different names*

### Comparing `scAllele-0.0.9.3/src/scAllele/gqv_bam_utils.py` & `scallele-0.0.9.4/src/scAllele/gqv_bam_utils.py`

 * *Files identical despite different names*

### Comparing `scAllele-0.0.9.3/src/scAllele/gqv_dbg_utils.py` & `scallele-0.0.9.4/src/scAllele/gqv_dbg_utils.py`

 * *Files identical despite different names*

### Comparing `scAllele-0.0.9.3/src/scAllele/gqv_glm.py` & `scallele-0.0.9.4/src/scAllele/gqv_glm.py`

 * *Files identical despite different names*

### Comparing `scAllele-0.0.9.3/src/scAllele/gqv_mutual_information.py` & `scallele-0.0.9.4/src/scAllele/gqv_mutual_information.py`

 * *Files identical despite different names*

### Comparing `scAllele-0.0.9.3/src/scAllele/gqv_software_management.py` & `scallele-0.0.9.4/src/scAllele/gqv_software_management.py`

 * *Files identical despite different names*

### Comparing `scAllele-0.0.9.3/src/scAllele/gqv_utils.py` & `scallele-0.0.9.4/src/scAllele/gqv_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-
+import os
 import sys
 import copy
 import numpy as np ; np.seterr(all = "ignore")
 import _pickle as pickle
 import itertools
 import datetime
 import scipy.stats as stats
@@ -1224,56 +1224,67 @@
 
 def read_genome_fasta(gf):
     fasta = pyfaidx.Faidx(gf)
     return fasta
 
 
 def write_feat_file(var_list, FeatFile):
-    Feat_Handle = open(FeatFile, 'w')
-    Title = False
-    feat_list = []
+    if os.path.exists(FeatFile):
+        Feat_Handle = open(FeatFile, 'a')
+        Title = True
+    else:
+        Feat_Handle = open(FeatFile, 'w')
+        Title = False
+
+    feat_list = []          
 
     for genomic_pos in sorted(var_list):
         for ALT, line in var_list[genomic_pos].items():
 
             flat_dict = {} 
 
-            for f, v in line.items():
+            for feat, v in line.items():
                 if not isinstance(v, dict):
-                    flat_dict[f] = v
-
-            if abs(line['INDEL_LEN']) > 20:
-                continue
+                    flat_dict[feat] = v
 
-            for f, v in line.items():
+            for sm, v in line.items():
                 if isinstance(v, dict):
                                         
-                    for feat, value in line[f]['FEAT'].items():
+                    for feat, value in line[sm]['FEAT'].items():
                         flat_dict[feat] = value
 
-                    if not Title:
-                        feat_list  = list(flat_dict.keys())
-                        title_line = [str(_feat) for _feat in feat_list]
+                    feat_list  = sorted(list(flat_dict.keys()))
+
+                    if not Title: # title is missing
+                        title_line = [str(_feat) for _feat in feat_list] ; print(title_line)
                         Feat_Handle.write('\t'.join(["SM"] + title_line) + '\n')
                         Title = True
 
-                    outline = [f] + [str(flat_dict[_feat]) for _feat in feat_list]
+                    if abs(flat_dict['INDEL_LEN']) > 20:
+                        continue
+
+                    outline = [sm] + [str(flat_dict[_feat]) for _feat in feat_list] 
                     Feat_Handle.write('\t'.join(outline) + '\n')
 
     Feat_Handle.close()
 
 
 def write_readcluster_file(ALL_READ_CLUSTERS, outfile):
-    with open(outfile, 'w') as f:
-        f.write("bam_file\tindex\tchrom\tstart\tend\tstrand\tmax_coverage\n")
-        for (sm, bam), rc_list in ALL_READ_CLUSTERS.items():
-            for rc in rc_list:
-                outline = [sm] + list(rc)
-                f.write("\t".join(map(str, outline)) + "\n")
+    if os.path.exists(outfile):
+        f = open(outfile, 'a')
+    else:
+        f = open(outfile, 'w')
+        f.write("bam_file\tindex\tchrom\tstrand\tstart\tend\tmax_coverage\n")
+
+    for (sm, bam), rc_list in ALL_READ_CLUSTERS.items():
+        for rc in rc_list:
+            outline = [sm] + list(rc)
+            f.write("\t".join(map(str, outline)) + "\n")
 
+    f.close()
 
 
 def write_vcf_header(search_regions, genome_fasta, VcfFile, SM_names):
 
     genome_faidx = read_genome_fasta(genome_fasta)
 
     VCF_handle = open(VcfFile, 'w')
```

### Comparing `scAllele-0.0.9.3/src/scAllele/gqv_vartool.py` & `scallele-0.0.9.4/src/scAllele/gqv_vartool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 import re
 import sys
 import numpy as np ; np.seterr(all = "ignore")
 import itertools 
 import HTSeq
 from time import time
-from collections import defaultdict, Hashable
+from collections import defaultdict, abc 
 from Bio import pairwise2
 import functools
 
 sys.setrecursionlimit(100000)
 
 ## General scoring
 
@@ -21,15 +21,15 @@
 
 ## Short sequence scoring
 
 _gap_open, _gap_ext = -0.6*_Gap, -0.4*_Gap  
 
 _base_pair_score = {}
 
-bases = ["A", "C", "G", "T", "I", "N"]
+bases = ["A", "C", "G", "T", "I", "N", "Y", "X"]
 
 for b1, b2 in itertools.product(bases, bases):
 	if b1 == b2:
 		_base_pair_score[(b1, b2)] = 0.0
 	elif b1 == "I" or b2 == "I":
 		_base_pair_score[(b1, b2)] = -1*_Intron_Gap
 	elif b1 == "N" or b2 == "N":
@@ -42,15 +42,15 @@
 
 class memoized(object):
 	def __init__(self, function_name):
 		self.function_name = function_name
 		self.cache = {}
 
 	def __call__(self, *args):
-		if not isinstance(args, Hashable):
+		if not isinstance(args, abc.Hashable):
 			return self.function_name(*args)
 		if args in self.cache:
 			return self.cache[args]
 		else:
 			value = self.function_name(*args)
 			self.cache[args] = value
 			return value
```

### Comparing `scAllele-0.0.9.3/src/scAllele/scAllele.py` & `scallele-0.0.9.4/src/scAllele/scAllele.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from . import gqv_glm
 from . import gqv_vartool
 from . import gqv_software_management as SOFTMAN
 from . import gqv_mutual_information  as MUTINFO
 
 
 
-__version__ = "0.0.9.3"
+__version__ = "0.0.9.4"
 
 
 def process_read_cluster_1(ARGs):
 	
 	RC_info, options, bam_file, SM = ARGs
 
 	RC_Index, chrom, strand, RC_Start, RC_End, MaxCov = RC_info 
@@ -358,19 +358,21 @@
 	Search_Regions = parse_chroms(bam_list, options)
 
 	SAMPLE_list = [(bam_file, gqv_bam_utils.get_sample_name(bam_file)) for bam_file in bam_list]
 
 
 	if options.run_mode in ("Full", "Variant_Caller"):
 		gqv_utils.write_vcf_header(Search_Regions, options.Genome, 
-									options.output_prefix + ".vcf", SAMPLE_list)
-		gqv_utils.write_introns_header(options.output_prefix + ".intronic_parts.bed")
+									f"{options.output_prefix}.vcf", SAMPLE_list)
+		gqv_utils.write_introns_header(f"{options.output_prefix}.intronic_parts.bed")
 
 	if options.run_mode in ("Full"):
-		gqv_utils.write_mutinfo_header(options.output_prefix + ".mi_summary.tab")
+		gqv_utils.write_mutinfo_header(f"{options.output_prefix}.mi_summary.tab")
+
+	os.system(f"rm -f {options.output_prefix}.*")
 
 
 	n = min(options.nodes, multiprocessing.cpu_count())
 	pool = multiprocessing.Pool(n)
 
 
 	for Search_Region in Search_Regions:	
@@ -430,41 +432,40 @@
 		for rc_VAR_LIST in pool.imap_unordered(process_read_cluster_2, ARGs): 
 			SOFTMAN.merge_copy(chrom_VAR_LIST, rc_VAR_LIST)
 
 
 		
 		if options.run_mode in ("Full", "Variant_Caller"):
 
-			gqv_utils.write_introns_bed(chrom_VAR_LIST, options.output_prefix + ".intronic_parts.bed")
+			gqv_utils.write_introns_bed(chrom_VAR_LIST,  f"{options.output_prefix}.intronic_parts.bed")
 			chrom_VAR_LIST = gqv_utils.merge_SM_VAR_LIST(chrom_VAR_LIST)
 			chrom_VAR_LIST = gqv_vartool.merge_introns(chrom_VAR_LIST, 'merged_SM')
 			gqv_glm.update_vars(GLM_INS, GLM_DEL, GLM_SNP, chrom_VAR_LIST, 'merged_SM', options)
 
 		if options.run_mode in ("Full",):
 
 			mi_outlines = MUTINFO.mi_parse_variants(chrom_VAR_LIST, 'merged_SM', options)
 			chrom_VAR_MUTINFO.extend(mi_outlines)
 
 
 		SOFTMAN.delete_reads(chrom_VAR_LIST)
 
 
 		if options.run_mode in ("Full", "Variant_Caller"):
-			gqv_utils.write_vcf_file(chrom_VAR_LIST, options.output_prefix + ".vcf", SAMPLE_list)
-			gqv_utils.write_introns_bed(chrom_VAR_LIST, options.output_prefix + ".intronic_parts.bed")
+			gqv_utils.write_vcf_file(chrom_VAR_LIST,    f"{options.output_prefix}.vcf", SAMPLE_list)
+			gqv_utils.write_introns_bed(chrom_VAR_LIST, f"{options.output_prefix}.intronic_parts.bed")
 
 		if options.run_mode in ("Full",):
-			gqv_utils.write_mutinfo_file(chrom_VAR_MUTINFO, options.output_prefix + ".mi_summary.tab")
+			gqv_utils.write_mutinfo_file(chrom_VAR_MUTINFO, f"{options.output_prefix}.mi_summary.tab")
 
-		if options.run_mode == "Training":
-			gqv_utils.write_feat_file(ALL_VARS_LIST, options.output_prefix + ".feature_matrix.tab")
+		if options.run_mode == "Training" and chrom_VAR_LIST:
+			gqv_utils.write_feat_file(chrom_VAR_LIST, f"{options.output_prefix}.feature_matrix.tab")
 
 
-		gqv_utils.write_readcluster_file(ALL_READ_CLUSTERS, 
-									options.output_prefix + ".read_cluster_info.tab")
+		gqv_utils.write_readcluster_file(ALL_READ_CLUSTERS, f"{options.output_prefix}.read_cluster_info.tab")
 
 
 		SOFTMAN.rm_nested_dict(chrom_VAR_LIST)
 		SOFTMAN.rm_nested_dict(ALL_READ_CLUSTERS)
 		gc.collect()
```

### Comparing `scAllele-0.0.9.3/src/scAllele.egg-info/PKG-INFO` & `scallele-0.0.9.4/src/scAllele.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 Metadata-Version: 2.1
 Name: scAllele
-Version: 0.0.9.3
+Version: 0.0.9.4
 Summary: A versatile tool for the detection and analysis of nucleotide variants in scRNA-seq
 Home-page: https://github.com/gxiaolab/scAllele
 Author: Giovanni Quinones Valdez
 Author-email: giovas@ucla.edu
 Project-URL: Bug Tracker, https://github.com/gxiaolab/scAllele/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biopython
+Requires-Dist: glob2
+Requires-Dist: HTSeq
+Requires-Dist: multiprocess
+Requires-Dist: networkx>=2.4
+Requires-Dist: numpy
+Requires-Dist: pandas>=1.3
+Requires-Dist: pickleshare
+Requires-Dist: psutil
+Requires-Dist: pyfaidx>=0.5.9.5
+Requires-Dist: pysam>=0.9.1
+Requires-Dist: vcfpy
+Requires-Dist: scikit-learn>=0.23.1
+Requires-Dist: scipy
+Requires-Dist: statsmodels>=0.11.1
 
 # **scAllele**
 _______________________________________
 [![](https://img.shields.io/badge/scAllele-v0.0.9.3-blue)](https://test.pypi.org/project/scAllele/)
 
 [Github](https://github.com/gxiaolab/scAllele/)
 
@@ -26,15 +41,15 @@
 scAllele makes use local reassembly via de-Bruijn graph to identify sequence differences and infers nucleotide variants at the read level. \
 The read level variant-call allows for the analysis of the role variants in the context of splicing. 
 Using mutual information, scAllele identifies allelic linkage between nucleotide variants and splicing
 isoforms.
 
 ## **Table of contents**
 - [Outline](#Outline)
-- [Download](#Download)
+- [Installation](#Installation)
 - [Usage](#Usage)
 	- [Basic usage](#Basic-usage)
 	- [Preprocessing](#Preprocessing)
 	- [Stranded data](#Stranded-data)
 	- [Local variant call](#Local-variant-call)
 	- [Filtering variants](#Filtering-variants)
 	- [Training a new classifier](#Training-a-new-classifier)
@@ -47,27 +62,51 @@
 
 | ![alt text](img/screenshot_Fig1.png) |
 |:--:|
 | *a. Illustration of the main algorithm of scAllele for variant calling. The reads and the reference genomic sequence overlapping a read cluster (RC) are decomposed into k-mers and are reasembled into a de Bruijn graph. b. Variants (green box in a) identified from the graph are then scored using a generalized linear model (GLM). The GLM was trained with different features (green box) to assign a confidence score to the variants. c. To identify allele-specific splicing (i.e., variant linkage), scAllele performs a mutual information calculation between nucleotide variants (SNVs, microindels) and intronic parts (where the ‘alleles’ are the different overlapping introns), to calculate allelic linkage of splicing isoforms.* |  
 
 _______________________________________
 
-## **Download**
+## **Installation**
 
-scAllele is available through PyPi. To download simply type:
+scAllele is available through **PyPi**. To download simply type:
 
 ```
-$ pip install scAllele
+pip install scAllele
 ```
 
-The download was tested with PyPi version >= 20.0.1
+The download was tested with PyPi version >= 20.0.1.
+
+Alternatively, you can clone this **GitHub** repository:
+
+```
+git clone git@github.com:gxiaolab/scAllele.git 
+pip install .
+```
+
+Or
+
+```
+git clone https://github.com/gxiaolab/scAllele.git
+pip install .
+```
+
+You can also download the **Singularity** container:
+
+```
+singularity pull library://giovas/collection/s5
+# run
+singularity exec s5_latest.sif scAllele
+```
 
 If succesful, the program is ready to use. The installation incorporates console script entrypoints to directly call scAllele:
+
 ```
-$ scAllele
+scAllele
+
 Usage: 
 	scAllele -b <file.bam> -g <genome.fa> -o <output prefix>
 A variant caller and variant analysis tool for scRNA-seq data.
 Options:
   -h, --help            show this help message and exit
   -b INPUT_BAM, --input-bam=INPUT_BAM
                         [Required] Input bam file, (or comma-seprated list of
@@ -131,21 +170,21 @@
 
 The minimum requirements to run scAllele are:
 1. A bam file (sorted and indexed) `samtools sort file.bam file.sorted ; samtools index file.sorted.bam` 
 2. A reference genome fasta file (indexed) `samtools faidx genome.fa`
 3. A prefix for the output files.
 
 ```
-$ scAllele -b file.sorted.bam -g genome.fa -o path/to/output_prefix
+scAllele -b file.sorted.bam -g genome.fa -o path/to/output_prefix
 ```
 
 Using the provided test data: 
 
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
 ```
 
 
 ### *Preprocessing* 
@@ -157,98 +196,99 @@
 | *Recommended pipeline* |
 
 ### *Stranded data*
 If your scRNA-seq is strand-specific, then you can specify the strandedness of your data (default: non-strand specific). \
 Strand-specific data helps resolve ambiguous alignments on overlapping genes. It also helps detect more accurate ASAS events. \
 Most strand-specific libraries in RNA-Seq are `fr-firststrand` (second read pair is sense to the RNA). You can specify this in your command:
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
     --strandedness='fr-firststrand'
 ```
 Alternatively, you can use the option `--strandedness=fr-secondstrand` if the first read pair is sense to the RNA.  
 
 ### *Local variant call*
 By default, scAllele searches for variants in all the regions of the transcriptome covered by reads. If you wish to search for variants in a custom genomic interval, you can do so with the `-c` option. 
 ```
 ## Only search chromosome 21
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
     -c chr21
 ## Only search within these coordinates
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
     -c chr21:34582111-34628004
 ```
 
 scAllele will search for read clusters within these regions only. Bare in mind that it's possible to find no read clusters in the spcified region, and that, if a specified region does not contain the entirety of a gene, it may miss some ASAS events. 
 
 
 ### *Filtering variants* 
 
 Although it is recommended to filter variants downstream of your analysis (via bcftools or others), it's possible to filter variants from the start. If you wish, for example, to only report variants with 3 reads supporting the alternative allele (AC) and 5 reads overall, then you can run the following command:
 
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/output_prefix 
     --AC=3 
     --DP=5
 ```
 
 The default is `AC=2 and DP=2`. 
 
 ### *Training a new classifier* 
 
 scAllele offers the option to retrain the variant classifier. Sequencing data from different platforms or resulting from different library preparation protocols may have different error profiles. If you wish to retrain scAllele's classifier run it in training mode: 
 
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o path/to/new_clf 
     --run_mode='Training' 
 ```
 
 This will return a feature file (`.feature_matrix.tab`) containing the variant calls and all the features used for the training of the classifier.  
 Then, run scAllele's training function. The supervised classifier will require a set of ground-truth variants to fit the model.  
 
 ```
-$ scAllele_train 
+scAllele_train 
     -i path/to/new_clf.feature_matrix.tab 
     -v truth.vcf 
     -g testdata/hg38.chr21.fa
 ```
 
 This will return 3 pickle objects:
 
 * path/to/new_clf.feature_matrix.tab.DELETION.glm.pickle
 * path/to/new_clf.feature_matrix.tab.INSERTION.glm.pickle
 * path/to/new_clf.feature_matrix.tab.SNP.glm.pickle
 
 Finally, to use these new classifiers to call variants run:
 
 ```
-$ scAllele 
+scAllele 
     -b testdata/gm12878.chr21.bam 
     -g testdata/hg38.chr21.fa 
     -o new_path/to/output_prefix 
     --glm_clf_name path/to/new_clf.feature_matrix.tab  
 ```
 
 _____________________________________
 
 
+
 ## **Output**
 
 scAllele generates 4 files as output:
 
 * path/to/output_prefix.vcf
 * path/to/output_prefix.mi_summary.tab
 * path/to/output_prefix.read_cluster_info.tab
@@ -272,14 +312,7 @@
 ```
 
 If one or more dependencies fail to install, make sure you have the latest version of pip:
 
 ```
 pip install --upgrade pip
 ```
-
-If the error persists, download the `requires.txt` file from this repository and install the dependencies prior to scAllele installation:
-
-```
-pip install -r requires.txt
-pip install -i https://test.pypi.org/simple/ scAllele==0.0.9.3
-```
```

### Comparing `scAllele-0.0.9.3/src/scAllele.egg-info/SOURCES.txt` & `scallele-0.0.9.4/src/scAllele.egg-info/SOURCES.txt`

 * *Files identical despite different names*

