# Comparing `tmp/b2aiprep-0.8.1.tar.gz` & `tmp/b2aiprep-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2aiprep-0.8.1.tar", last modified: Mon Apr  8 18:01:43 2024, max compression
+gzip compressed data, was "b2aiprep-0.9.0.tar", last modified: Mon Apr  8 21:25:12 2024, max compression
```

## Comparing `b2aiprep-0.8.1.tar` & `b2aiprep-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:01:43.339659 b2aiprep-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-04-08 18:01:43.339659 b2aiprep-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:01:43.339659 b2aiprep-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:01:43.335659 b2aiprep-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:01:43.335659 b2aiprep-0.8.1/src/b2aiprep/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/src/b2aiprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 18:01:43.339659 b2aiprep-0.8.1/src/b2aiprep/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/src/b2aiprep/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/src/b2aiprep/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:01:43.339659 b2aiprep-0.8.1/src/b2aiprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-04-08 18:01:43.000000 b2aiprep-0.8.1/src/b2aiprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-08 18:01:43.000000 b2aiprep-0.8.1/src/b2aiprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:01:43.000000 b2aiprep-0.8.1/src/b2aiprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 18:01:43.000000 b2aiprep-0.8.1/src/b2aiprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-08 18:01:43.000000 b2aiprep-0.8.1/src/b2aiprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 18:01:43.000000 b2aiprep-0.8.1/src/b2aiprep.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:01:43.339659 b2aiprep-0.8.1/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/src/tests/test_speech_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/src/tests/test_voice_converstion.py
--rw-r--r--   0 runner    (1001) docker     (127)    86892 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:25:12.971995 b2aiprep-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-08 21:25:05.000000 b2aiprep-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-04-08 21:25:12.971995 b2aiprep-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-08 21:25:05.000000 b2aiprep-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-08 21:25:05.000000 b2aiprep-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 21:25:12.971995 b2aiprep-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 21:25:05.000000 b2aiprep-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:25:12.967995 b2aiprep-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:25:12.967995 b2aiprep-0.9.0/src/b2aiprep/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 21:25:05.000000 b2aiprep-0.9.0/src/b2aiprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 21:25:12.971995 b2aiprep-0.9.0/src/b2aiprep/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-04-08 21:25:05.000000 b2aiprep-0.9.0/src/b2aiprep/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-04-08 21:25:05.000000 b2aiprep-0.9.0/src/b2aiprep/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:25:12.967995 b2aiprep-0.9.0/src/b2aiprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-04-08 21:25:12.000000 b2aiprep-0.9.0/src/b2aiprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-08 21:25:12.000000 b2aiprep-0.9.0/src/b2aiprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:25:12.000000 b2aiprep-0.9.0/src/b2aiprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 21:25:12.000000 b2aiprep-0.9.0/src/b2aiprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-08 21:25:12.000000 b2aiprep-0.9.0/src/b2aiprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 21:25:12.000000 b2aiprep-0.9.0/src/b2aiprep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:25:12.967995 b2aiprep-0.9.0/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 21:25:05.000000 b2aiprep-0.9.0/src/tests/test_speech_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-08 21:25:05.000000 b2aiprep-0.9.0/src/tests/test_voice_converstion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86892 2024-04-08 21:25:05.000000 b2aiprep-0.9.0/versioneer.py
```

### Comparing `b2aiprep-0.8.1/LICENSE` & `b2aiprep-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b2aiprep-0.8.1/PKG-INFO` & `b2aiprep-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b2aiprep
-Version: 0.8.1
+Version: 0.9.0
 Summary: A small package to generate features from acoustic
 Author-email: Rahul Brito <rfbrito@mit.edu>, SenseIn Group <sensein-social@mit.edu>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -129,14 +129,16 @@
     b2aiprep-cli convert test_audio.wav s1 mpt
     ```
 
     It will save a pytorch `.pt` file with a dictionary of features. This can be
     loaded by `torch.load()`. The file is named following a simple convention:
     `sub-<subject_id>_task-<task_name>_md5-<checksum>_features.pt`
 
+    To enable speech to text transcription, specify the `--speech2text` flag.
+
 2. Batch process audio files
 
     This requires a CSV file, where each line is of the form:
     path/to/audio.wav
 
     This also supports a CSV file where each line is of the form:
     path/to/audio.wav,subject_id,task_name
@@ -147,17 +149,19 @@
     b2aiprep-cli batchconvert filelist.csv --plugin cf n_procs=2 --outdir out --save_figures
     ```
 
     The above command uses pydra under the hood to parallel process the audio files.
     All outputs are currently stored in a single directory specified by the `--outdir`
     flag.
 
-    One can also generate a hugging face dataset in the output directoryby specifying the
+    One can also generate a hugging face dataset in the output directory by specifying the
      `--dataset` flag.
 
+    To enable speech to text transcription, specify the `--speech2text` flag.
+
 3. Generate csv file to feed to batchconvert
 
     ```bash
     b2aiprep-cli createbatchcsv input_dir outfile
     ```
 
     The input directory should point to the location of the `Production` directory pulled from Wasabi e.g. `/Users/b2ai/production`.
```

### Comparing `b2aiprep-0.8.1/README.md` & `b2aiprep-0.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     b2aiprep-cli convert test_audio.wav s1 mpt
     ```
 
     It will save a pytorch `.pt` file with a dictionary of features. This can be
     loaded by `torch.load()`. The file is named following a simple convention:
     `sub-<subject_id>_task-<task_name>_md5-<checksum>_features.pt`
 
+    To enable speech to text transcription, specify the `--speech2text` flag.
+
 2. Batch process audio files
 
     This requires a CSV file, where each line is of the form:
     path/to/audio.wav
 
     This also supports a CSV file where each line is of the form:
     path/to/audio.wav,subject_id,task_name
@@ -44,17 +46,19 @@
     b2aiprep-cli batchconvert filelist.csv --plugin cf n_procs=2 --outdir out --save_figures
     ```
 
     The above command uses pydra under the hood to parallel process the audio files.
     All outputs are currently stored in a single directory specified by the `--outdir`
     flag.
 
-    One can also generate a hugging face dataset in the output directoryby specifying the
+    One can also generate a hugging face dataset in the output directory by specifying the
      `--dataset` flag.
 
+    To enable speech to text transcription, specify the `--speech2text` flag.
+
 3. Generate csv file to feed to batchconvert
 
     ```bash
     b2aiprep-cli createbatchcsv input_dir outfile
     ```
 
     The input directory should point to the location of the `Production` directory pulled from Wasabi e.g. `/Users/b2ai/production`.
```

### Comparing `b2aiprep-0.8.1/pyproject.toml` & `b2aiprep-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `b2aiprep-0.8.1/src/b2aiprep/cli.py` & `b2aiprep-0.9.0/src/b2aiprep/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,24 +37,36 @@
 @click.option("-s", "--subject", type=ty.Optional[str], default=None)
 @click.option("-t", "--task", type=ty.Optional[str], default=None)
 @click.option("--outdir", type=click.Path(), default=os.getcwd(), show_default=True)
 @click.option("--save_figures/--no-save_figures", default=False, show_default=True)
 @click.option("--n_mels", type=int, default=20, show_default=True)
 @click.option("--n_coeff", type=int, default=20, show_default=True)
 @click.option("--compute_deltas/--no-compute_deltas", default=True, show_default=True)
+@click.option("--speech2text/--no-speech2text", type=bool, default=False, show_default=True)
 @click.option("--opensmile", nargs=2, default=["eGeMAPSv02", "Functionals"], show_default=True)
 def convert(
-    filename, subject, task, outdir, save_figures, n_mels, n_coeff, compute_deltas, opensmile
+    filename,
+    subject,
+    task,
+    outdir,
+    save_figures,
+    n_mels,
+    n_coeff,
+    compute_deltas,
+    speech2text,
+    opensmile,
 ):
+    os.makedirs(outdir, exist_ok=True)
     to_features(
         filename,
         subject,
         task,
         outdir=Path(outdir),
         save_figures=save_figures,
+        extract_text=speech2text,
         n_mels=n_mels,
         n_coeff=n_coeff,
         compute_deltas=compute_deltas,
         opensmile_feature_set=opensmile[0],
         opensmile_feature_level=opensmile[1],
     )
 
@@ -78,25 +90,27 @@
     "-c",
     "--cache",
     default=os.path.join(os.getcwd(), "cache-wf"),
     help="Cache dir",
     show_default=True,
 )
 @click.option("--dataset/--no-dataset", type=bool, default=False, show_default=True)
+@click.option("--speech2text/--no-speech2text", type=bool, default=False, show_default=True)
 @click.option("--opensmile", nargs=2, default=["eGeMAPSv02", "Functionals"], show_default=True)
 def batchconvert(
     csvfile,
     outdir,
     save_figures,
     n_mels,
     n_coeff,
     compute_deltas,
     plugin,
     cache,
     dataset,
+    speech2text,
     opensmile,
 ):
     plugin_args = dict()
     for item in plugin[1].split():
         key, value = item.split("=")
         if plugin[0] == "cf" and key == "n_procs":
             value = int(value)
@@ -105,14 +119,15 @@
     featurize_pdt = pydratask(annotate({"return": {"features": ty.Any}})(to_features))
     featurize_task = featurize_pdt(
         n_mels=n_mels,
         n_coeff=n_coeff,
         compute_deltas=compute_deltas,
         cache_dir=Path(cache).absolute(),
         save_figures=save_figures,
+        extract_text=speech2text,
         opensmile_feature_set=opensmile[0],
         opensmile_feature_level=opensmile[1],
     )
 
     with open(csvfile, "r") as f:
         reader = csv.DictReader(f)
         num_cols = len(reader.fieldnames)
@@ -204,15 +219,14 @@
 
 @main.command()
 @click.argument("audio_file", type=click.Path(exists=True))
 @click.option("--model_id", type=str, default="openai/whisper-tiny", show_default=True)
 @click.option("--max_new_tokens", type=int, default=128, show_default=True)
 @click.option("--chunk_length_s", type=int, default=30, show_default=True)
 @click.option("--batch_size", type=int, default=16, show_default=True)
-@click.option("--batch_size", type=int, default=16, show_default=True)
 @click.option("--device", type=str, default=None, help="Device to use for inference.")
 @click.option(
     "--return_timestamps",
     type=str,
     default="false",
     help="Return timestamps with the transcription. Can be 'true', 'false', or 'word'.",
 )
```

### Comparing `b2aiprep-0.8.1/src/b2aiprep/process.py` & `b2aiprep-0.9.0/src/b2aiprep/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,14 +193,16 @@
 
 def to_features(
     filename: Path,
     subject: ty.Optional[str] = None,
     task: ty.Optional[str] = None,
     outdir: ty.Optional[Path] = None,
     save_figures: bool = False,
+    stt_kwargs: ty.Optional[ty.Dict] = None,
+    extract_text: bool = False,
     n_mels: int = 20,
     n_coeff: int = 20,
     compute_deltas: bool = True,
     opensmile_feature_set: str = "eGeMAPSv02",
     opensmile_feature_level: str = "Functionals",
     return_features: bool = False,
     mpl_backend: str = "Agg",
@@ -208,14 +210,16 @@
     """Compute features from audio file
 
     :param filename: Path to audio file
     :param subject: Subject ID
     :param task: Task ID
     :param outdir: Output directory
     :param save_figures: Whether to save figures
+    :param extract_text: Whether to extract text
+    :param stt_kwargs: Keyword arguments for SpeechToText
     :param n_mels: Number of Mel bands
     :param n_coeff: Number of MFCC coefficients
     :param compute_deltas: Whether to compute delta features
     :param opensmile_feature_set: OpenSmile feature set
     :param opensmile_feature_level: OpenSmile feature level
     :param return_features: Whether to return features
     :param mpl_backend: matplotlib backend
@@ -240,14 +244,29 @@
         "specgram": features_specgram,
         "melfilterbank": features_melfilterbank,
         "mfcc": features_mfcc,
         "opensmile": features_opensmile,
         "sample_rate": audio.sample_rate,
         "checksum": md5sum,
     }
+    if extract_text:
+        stt_kwargs_default = {
+            "model_id": "openai/whisper-base",
+            "max_new_tokens": 128,
+            "chunk_length_s": 30,
+            "batch_size": 16,
+            "device": None,
+        }
+        if stt_kwargs is not None:
+            stt_kwargs_default.update(**stt_kwargs)
+        stt_kwargs = stt_kwargs_default
+        stt = SpeechToText(**stt_kwargs)
+        transcription = stt.transcribe(audio, language="en")
+        features["transcription"] = transcription
+
     if subject is not None:
         if task is not None:
             prefix = f"sub-{subject}_task-{task}_md5-{md5sum}"
         else:
             prefix = f"sub-{subject}_md5-{md5sum}"
     else:
         prefix = Path(filename).stem
```

### Comparing `b2aiprep-0.8.1/src/b2aiprep.egg-info/PKG-INFO` & `b2aiprep-0.9.0/src/b2aiprep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b2aiprep
-Version: 0.8.1
+Version: 0.9.0
 Summary: A small package to generate features from acoustic
 Author-email: Rahul Brito <rfbrito@mit.edu>, SenseIn Group <sensein-social@mit.edu>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -129,14 +129,16 @@
     b2aiprep-cli convert test_audio.wav s1 mpt
     ```
 
     It will save a pytorch `.pt` file with a dictionary of features. This can be
     loaded by `torch.load()`. The file is named following a simple convention:
     `sub-<subject_id>_task-<task_name>_md5-<checksum>_features.pt`
 
+    To enable speech to text transcription, specify the `--speech2text` flag.
+
 2. Batch process audio files
 
     This requires a CSV file, where each line is of the form:
     path/to/audio.wav
 
     This also supports a CSV file where each line is of the form:
     path/to/audio.wav,subject_id,task_name
@@ -147,17 +149,19 @@
     b2aiprep-cli batchconvert filelist.csv --plugin cf n_procs=2 --outdir out --save_figures
     ```
 
     The above command uses pydra under the hood to parallel process the audio files.
     All outputs are currently stored in a single directory specified by the `--outdir`
     flag.
 
-    One can also generate a hugging face dataset in the output directoryby specifying the
+    One can also generate a hugging face dataset in the output directory by specifying the
      `--dataset` flag.
 
+    To enable speech to text transcription, specify the `--speech2text` flag.
+
 3. Generate csv file to feed to batchconvert
 
     ```bash
     b2aiprep-cli createbatchcsv input_dir outfile
     ```
 
     The input directory should point to the location of the `Production` directory pulled from Wasabi e.g. `/Users/b2ai/production`.
```

### Comparing `b2aiprep-0.8.1/src/tests/test_speech_to_text.py` & `b2aiprep-0.9.0/src/tests/test_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `b2aiprep-0.8.1/src/tests/test_voice_converstion.py` & `b2aiprep-0.9.0/src/tests/test_voice_converstion.py`

 * *Files identical despite different names*

### Comparing `b2aiprep-0.8.1/versioneer.py` & `b2aiprep-0.9.0/versioneer.py`

 * *Files identical despite different names*

