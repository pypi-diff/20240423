# Comparing `tmp/climush-0.0.6.tar.gz` & `tmp/climush-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climush-0.0.6.tar", last modified: Wed Apr 10 18:31:05 2024, max compression
+gzip compressed data, was "climush-0.0.7.tar", last modified: Mon Apr 22 22:20:56 2024, max compression
```

## Comparing `climush-0.0.6.tar` & `climush-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-10 18:31:05.345249 climush-0.0.6/
--rw-r--r--   0 root         (0) staff       (20)     2135 2024-04-10 18:31:05.345054 climush-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1234 2024-04-04 09:14:41.000000 climush-0.0.6/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-10 18:31:05.343958 climush-0.0.6/climush/
--rw-r--r--   0 root         (0) staff       (20)      152 2024-04-07 02:45:45.000000 climush-0.0.6/climush/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    24466 2024-02-03 09:44:16.000000 climush-0.0.6/climush/binfo_old.py
--rw-r--r--   0 root         (0) staff       (20)    64734 2024-04-10 02:05:17.000000 climush-0.0.6/climush/bioinfo.py
--rw-r--r--   0 root         (0) staff       (20)      380 2024-04-07 02:13:39.000000 climush-0.0.6/climush/config.py
--rw-r--r--   0 root         (0) staff       (20)     1125 2024-03-12 03:14:02.000000 climush-0.0.6/climush/constants.py
--rw-r--r--   0 root         (0) staff       (20)    44331 2024-04-10 18:29:42.000000 climush-0.0.6/climush/utilities.py
--rw-r--r--   0 root         (0) staff       (20)     5770 2024-02-23 04:02:34.000000 climush-0.0.6/climush/viz.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-10 18:31:05.344862 climush-0.0.6/climush.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     2135 2024-04-10 18:31:05.000000 climush-0.0.6/climush.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      313 2024-04-10 18:31:05.000000 climush-0.0.6/climush.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-10 18:31:05.000000 climush-0.0.6/climush.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       50 2024-04-10 18:31:05.000000 climush-0.0.6/climush.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        8 2024-04-10 18:31:05.000000 climush-0.0.6/climush.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)      929 2024-04-10 18:30:07.000000 climush-0.0.6/pyproject.toml
--rw-r--r--   0 root         (0) staff       (20)       38 2024-04-10 18:31:05.345291 climush-0.0.6/setup.cfg
+drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-22 22:20:56.164366 climush-0.0.7/
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     2098 2024-04-22 22:20:56.164189 climush-0.0.7/PKG-INFO
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     1234 2024-04-04 09:14:41.000000 climush-0.0.7/README.md
+drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-22 22:20:56.163161 climush-0.0.7/climush/
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)      152 2024-04-07 02:45:45.000000 climush-0.0.7/climush/__init__.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)    24466 2024-02-03 09:44:16.000000 climush-0.0.7/climush/binfo_old.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)    64732 2024-04-22 21:54:33.000000 climush-0.0.7/climush/bioinfo.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)      380 2024-04-07 02:13:39.000000 climush-0.0.7/climush/config.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     1125 2024-03-12 03:14:02.000000 climush-0.0.7/climush/constants.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)    44331 2024-04-10 18:29:42.000000 climush-0.0.7/climush/utilities.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     5770 2024-02-23 04:02:34.000000 climush-0.0.7/climush/viz.py
+drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-22 22:20:56.164005 climush-0.0.7/climush.egg-info/
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     2098 2024-04-22 22:20:56.000000 climush-0.0.7/climush.egg-info/PKG-INFO
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)      313 2024-04-22 22:20:56.000000 climush-0.0.7/climush.egg-info/SOURCES.txt
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)        1 2024-04-22 22:20:56.000000 climush-0.0.7/climush.egg-info/dependency_links.txt
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)       50 2024-04-22 22:20:56.000000 climush-0.0.7/climush.egg-info/requires.txt
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)        8 2024-04-22 22:20:56.000000 climush-0.0.7/climush.egg-info/top_level.txt
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)      930 2024-04-22 22:19:36.000000 climush-0.0.7/pyproject.toml
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)       38 2024-04-22 22:20:56.164404 climush-0.0.7/setup.cfg
```

### Comparing `climush-0.0.6/PKG-INFO` & `climush-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: climush
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tools to run the CliMush bioinformatics pipeline.
 Author-email: Carolyn Delevich <cdelevic@uoregon.edu>
 Project-URL: Homepage, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline
 Project-URL: Repository, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline/climush_py-package
 Project-URL: Issues, https://github.com/cdelevich/climush/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: numpy
```

### Comparing `climush-0.0.6/README.md` & `climush-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `climush-0.0.6/climush/binfo_old.py` & `climush-0.0.7/climush/binfo_old.py`

 * *Files identical despite different names*

### Comparing `climush-0.0.6/climush/bioinfo.py` & `climush-0.0.7/climush/bioinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     # DEFINE RELEVANT FILE PATHS ####################################################################
     # get the paths needed for demux
     mapping_dir = file_map['config']['bc_mapping']  # directory containing all mapping files
     mapping_files = list(mapping_dir.glob('*'))  # get mapping files, as list (will reuse + exhaust)
 
     # ACCESS USER SETTINGS FROM CONFIG ##############################################################
-    run_name = settings['run_details']['run_name']  # name to use for this bioinformatics run
+    run_name = settings_dict['run_details']['run_name']  # name to use for this bioinformatics run
 
     # CONSTRUCT REGEX CONSTANTS #####################################################################
     # column name regex; column names vary among mapping files
     FWD_COL_RE = '(fwd)|(forward)'
     REV_COL_RE = '(rev)|(reverse)'
     SAMPLE_ID_RE = '^sample'
 
@@ -568,34 +568,34 @@
     max_untrimmed = int(cutadapt_settings['max_untrimmed'])
 
     if paired_end:
         paired_dict = pair_reads(input_files)
 
         for file in paired_dict.keys():
 
-            fwd_read_out = add_prefix(file_path=file, prefix=TRIMMED_PREFIX, dest_dir=trim_path, action='None')
-            rev_read_out = add_prefix(file_path=paired_dict[file], prefix=TRIMMED_PREFIX, dest_dir=trim_path, action='None')
+            fwd_read_out = add_prefix(file_path=file, prefix=TRIMMED_PREFIX, dest_dir=trim_path, action=None)
+            rev_read_out = add_prefix(file_path=paired_dict[file], prefix=TRIMMED_PREFIX, dest_dir=trim_path, action=None)
 
             cutadapt_cmd = ['cutadapt', '--report=minimal',
                             '-a', fwd_primer, '-A', rev_primer,
                             '-n', '2', '-e', str(max_err),
                             '-o', fwd_read_out, '-p', rev_read_out,
                             file, paired_dict[file]]
 
             run_subprocess(cutadapt_cmd, dest_dir=trim_primers_parent)
 
     else:
 
         for file in input_files:
 
-            trim_out = add_prefix(file_path=file, prefix=TRIMMED_PREFIX, dest_dir=trim_path, action='None')
+            trim_out = add_prefix(file_path=file, prefix=TRIMMED_PREFIX, dest_dir=trim_path, action=None)
 
             if cutadapt_settings['keep_untrimmed']:
                 notrim_out = add_prefix(file_path=file, prefix=flip_prefix(TRIMMED_PREFIX),
-                                        dest_dir=notrim_path, action='None')
+                                        dest_dir=notrim_path, action=None)
                 untrim_cmd = f'--untrimmed-output={notrim_out}'
             else:
                 untrim_cmd = ''
 
 
             cutadapt_cmd = ['cutadapt', '--report=minimal',
                             '-a', f'^{fwd_primer}...{rev_revcomp_primer}$',
@@ -678,38 +678,38 @@
 
     qfilt_path = mkdir_exist_ok(new_dir=f'./{QUALFILT_PREFIX}_{run_name}', parent_dir=qfilt_parent)
     nofilt_path = mkdir_exist_ok(new_dir=f'./{flip_prefix(QUALFILT_PREFIX)}_{run_name}', parent_dir=qfilt_parent)
 
     if premerged:
         for file in input_files:
             qfilt_out = add_prefix(file_path=file, prefix=QUALFILT_PREFIX,
-                                           dest_dir=qfilt_path, action='None')
+                                           dest_dir=qfilt_path, action=None)
             nofilt_out = add_prefix(file_path=file, prefix=flip_prefix(QUALFILT_PREFIX),
-                                        dest_dir=nofilt_path, action='None')
+                                        dest_dir=nofilt_path, action=None)
 
             vsearch_filt_cmd = ['vsearch', '--fastq_filter', file,
                                 '--fastqout', qfilt_out,
                                 '--fastqout_discarded', nofilt_out,
                                 '-fastq_maxee', str(max_error), '--fastq_maxlen', str(max_len),
                                 '--fastq_minlen', str(min_len), '--sizeout']
 
             run_subprocess(vsearch_filt_cmd, dest_dir=qfilt_parent)
     else:
         paired_dict = pair_reads(input_files)
         for file in paired_dict.keys():
 
             qfilt_fwd_out = add_prefix(file_path=file, prefix=QUALFILT_PREFIX,
-                                       dest_dir=qfilt_path, action='None')
+                                       dest_dir=qfilt_path, action=None)
             nofilt_fwd_out = add_prefix(file_path=file, prefix=flip_prefix(QUALFILT_PREFIX),
-                                        dest_dir=nofilt_path, action='None')
+                                        dest_dir=nofilt_path, action=None)
 
             qfilt_rev_out = add_prefix(file_path=paired_dict[file], prefix=QUALFILT_PREFIX,
-                                       dest_dir=qfilt_path, action='None')
+                                       dest_dir=qfilt_path, action=None)
             nofilt_rev_out = add_prefix(file_path=paired_dict[file], prefix=flip_prefix(QUALFILT_PREFIX),
-                                        dest_dir=nofilt_path, action='None')
+                                        dest_dir=nofilt_path, action=None)
 
             vsearch_filt_cmd = ['vsearch', '--fastq_filter', file, '--reverse', paired_dict[file],
                                 '--fastqout', qfilt_fwd_out, '--fastqout_rev', qfilt_rev_out,
                                 '--fastqout_discarded', nofilt_fwd_out, '--fastqout_discarded_rev', nofilt_rev_out,
                                 '-fastq_maxee', str(max_error), '--fastq_maxlen', str(max_len),
                                 '--fastq_minlen', str(min_len), '--sizeout']
 
@@ -763,15 +763,15 @@
 
     itsx_parent = mkdir_exist_ok(new_dir=file_map['pipeline-output']['separate-subregions'])
 
     itsx_path = mkdir_exist_ok(new_dir=f'./{ITSX_PREFIX}_{run_name}',  parent_dir=itsx_parent)
 
     for file in input_files:
 
-        itsx_output_basename = add_prefix(file_path=file, prefix=ITSX_PREFIX, dest_dir=itsx_path).with_suffix('')
+        itsx_output_basename = add_prefix(file_path=file, prefix=ITSX_PREFIX, dest_dir=itsx_path, action=None).with_suffix('')
 
         itsx_command = ['ITSx', '-i', file, '-o', itsx_output_basename, '-t', 'F', '--multi_thread', 'T',
                         '--save_regions', 'all']
 
         run_subprocess(itsx_command, dest_dir=itsx_parent)
 
     return None
```

### Comparing `climush-0.0.6/climush/constants.py` & `climush-0.0.7/climush/constants.py`

 * *Files identical despite different names*

### Comparing `climush-0.0.6/climush/utilities.py` & `climush-0.0.7/climush/utilities.py`

 * *Files identical despite different names*

### Comparing `climush-0.0.6/climush/viz.py` & `climush-0.0.7/climush/viz.py`

 * *Files identical despite different names*

### Comparing `climush-0.0.6/climush.egg-info/PKG-INFO` & `climush-0.0.7/climush.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: climush
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tools to run the CliMush bioinformatics pipeline.
 Author-email: Carolyn Delevich <cdelevic@uoregon.edu>
 Project-URL: Homepage, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline
 Project-URL: Repository, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline/climush_py-package
 Project-URL: Issues, https://github.com/cdelevich/climush/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: numpy
```

### Comparing `climush-0.0.6/pyproject.toml` & `climush-0.0.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'climush'
-version = '0.0.6'
+version = '0.0.7'
 authors = [
     { name='Carolyn Delevich', email='cdelevic@uoregon.edu' }]
 description = 'Tools to run the CliMush bioinformatics pipeline.'
 readme = 'README.md'
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
-    'Operating System :: Unix',
+#    'Operating System :: Unix',
     'Development Status :: 3 - Alpha',
     'Topic :: Scientific/Engineering :: Bio-Informatics',
 ]
 requires-python = ">=3.10"
 dependencies = [
     'pandas',
     'scipy',
```

