# Comparing `tmp/ie-eval-0.1.0.tar.gz` & `tmp/ie-eval-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ie-eval-0.1.0.tar", last modified: Fri Feb  2 14:40:05 2024, max compression
+gzip compressed data, was "ie-eval-0.2.0a1.tar", last modified: Tue Apr 23 07:56:53 2024, max compression
```

## Comparing `ie-eval-0.1.0.tar` & `ie-eval-0.2.0a1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 14:40:05.472782 ie-eval-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-02-02 14:09:46.000000 ie-eval-0.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-02-02 14:09:46.000000 ie-eval-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2732 2024-02-02 14:40:05.472782 ie-eval-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      373 2024-02-02 14:09:46.000000 ie-eval-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 14:40:05.472782 ie-eval-0.1.0/ie_eval/
--rw-rw-rw-   0 root         (0) root         (0)      125 2024-02-02 14:09:46.000000 ie-eval-0.1.0/ie_eval/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3906 2024-02-02 14:09:46.000000 ie-eval-0.1.0/ie_eval/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 14:40:05.472782 ie-eval-0.1.0/ie_eval/metrics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-02 14:39:55.000000 ie-eval-0.1.0/ie_eval/metrics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7790 2024-02-02 14:09:46.000000 ie-eval-0.1.0/ie_eval/metrics/bag_of_entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1380 2024-02-02 14:09:46.000000 ie-eval-0.1.0/ie_eval/metrics/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6679 2024-02-02 14:09:46.000000 ie-eval-0.1.0/ie_eval/scorer.py
--rw-rw-rw-   0 root         (0) root         (0)     2638 2024-02-02 14:09:46.000000 ie-eval-0.1.0/ie_eval/table_formatter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 14:40:05.472782 ie-eval-0.1.0/ie_eval.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2732 2024-02-02 14:40:05.000000 ie-eval-0.1.0/ie_eval.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      474 2024-02-02 14:40:05.000000 ie-eval-0.1.0/ie_eval.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-02 14:40:05.000000 ie-eval-0.1.0/ie_eval.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-02-02 14:40:05.000000 ie-eval-0.1.0/ie_eval.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      217 2024-02-02 14:40:05.000000 ie-eval-0.1.0/ie_eval.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-02-02 14:40:05.000000 ie-eval-0.1.0/ie_eval.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2478 2024-02-02 14:22:21.000000 ie-eval-0.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-02-02 14:09:46.000000 ie-eval-0.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-02 14:40:05.472782 ie-eval-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1458 2024-02-02 14:22:21.000000 ie-eval-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 14:40:05.472782 ie-eval-0.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-02-02 14:09:46.000000 ie-eval-0.1.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22862 2024-02-02 14:09:46.000000 ie-eval-0.1.0/tests/test_bag_of_entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:56:53.523027 ie-eval-0.2.0a1/
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-04-23 07:56:53.523027 ie-eval-0.2.0a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      373 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:56:53.519027 ie-eval-0.2.0a1/ie_eval/
+-rw-rw-rw-   0 root         (0) root         (0)      125 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/ie_eval/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5755 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/ie_eval/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:56:53.523027 ie-eval-0.2.0a1/ie_eval/metrics/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 07:56:44.000000 ie-eval-0.2.0a1/ie_eval/metrics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4049 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/ie_eval/metrics/assignment_based.py
+-rw-rw-rw-   0 root         (0) root         (0)     6897 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/ie_eval/metrics/bag_of_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/ie_eval/metrics/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    16068 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/ie_eval/scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4897 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/ie_eval/table_formatter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:56:53.519027 ie-eval-0.2.0a1/ie_eval.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-04-23 07:56:53.000000 ie-eval-0.2.0a1/ie_eval.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      541 2024-04-23 07:56:53.000000 ie-eval-0.2.0a1/ie_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 07:56:53.000000 ie-eval-0.2.0a1/ie_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-23 07:56:53.000000 ie-eval-0.2.0a1/ie_eval.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      232 2024-04-23 07:56:53.000000 ie-eval-0.2.0a1/ie_eval.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-23 07:56:53.000000 ie-eval-0.2.0a1/ie_eval.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 07:56:53.523027 ie-eval-0.2.0a1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1458 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:56:53.523027 ie-eval-0.2.0a1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22862 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/tests/test_bag_of_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     8844 2024-04-23 07:54:11.000000 ie-eval-0.2.0a1/tests/test_ecer_ewer_nerval.py
```

### Comparing `ie-eval-0.1.0/LICENSE` & `ie-eval-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ie-eval-0.1.0/PKG-INFO` & `ie-eval-0.2.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ie-eval
-Version: 0.1.0
-Author-email: Oliver Tüselmann <oliver.tueselmann@tu-dortmund.de>, David Villanova Aparisi <davilap@inf.upv.es>, Yoann Schneider <yschneider@teklia.com>, Solène Tarride <starride@teklia.com>
+Version: 0.2.0a1
+Author-email: Solène Tarride <starride@teklia.com>, David Villanova Aparisi <davilap@inf.upv.es>, Yoann Schneider <yschneider@teklia.com>
 Maintainer-email: Yoann Schneider <yschneider@teklia.com>, Solène Tarride <starride@teklia.com>
 License: MIT License
         
         Copyright (c) 2023 TEKLIA
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ie-eval-0.1.0/ie_eval/cli.py` & `ie-eval-0.2.0a1/ie_eval/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """Command Line Arguments"""
 
 import argparse
 from pathlib import Path
 
+from ie_eval.metrics.assignment_based import (
+    compute_oiecerewer,
+    compute_oinerval,
+)
 from ie_eval.metrics.bag_of_entities import (
     compute_bag_of_entities,
     compute_bag_of_tagged_words,
     compute_bag_of_words,
 )
 from ie_eval.metrics.utils import compute_all_metrics
 
@@ -94,14 +98,67 @@
         "--by-category",
         "-c",
         action="store_true",
         help="Whether to compute scores for each semantic category.",
     )
 
 
+def add_ecer_ewer_parser(commands):
+    """Add parser for the ECER and EWER computation subcommand."""
+    parser = commands.add_parser(
+        "ecer-ewer",
+        help="Compute OIECER and OIEWER metrics.",
+    )
+    parser.set_defaults(func=compute_oiecerewer)
+    parser.add_argument(
+        "--label-dir",
+        "-l",
+        type=Path,
+        required=True,
+        help="Path to the directory containing BIO label files.",
+    )
+    parser.add_argument(
+        "--prediction-dir",
+        "-p",
+        type=Path,
+        required=True,
+        help="Path to the directory containing BIO prediction files.",
+    )
+
+
+def add_nerval_parser(commands):
+    """Add parser for the Nerval computation subcommand."""
+    parser = commands.add_parser(
+        "nerval",
+        help="Compute OINerval Precision, Recall and F1 scores.",
+    )
+    parser.set_defaults(func=compute_oinerval)
+    parser.add_argument(
+        "--label-dir",
+        "-l",
+        type=Path,
+        required=True,
+        help="Path to the directory containing BIO label files.",
+    )
+    parser.add_argument(
+        "--prediction-dir",
+        "-p",
+        type=Path,
+        required=True,
+        help="Path to the directory containing BIO prediction files.",
+    )
+    parser.add_argument(
+        "--nerval-threshold",
+        "-t",
+        type=float,
+        default=30.0,
+        help="Threshold of acceptable character errors, must be in the range: [0.0, 100.0]",
+    )
+
+
 def add_summary_parser(commands):
     """Add parser subcommand to compute all metrics."""
     parser = commands.add_parser(
         "all",
         help="Compute all metrics.",
     )
     parser.set_defaults(func=compute_all_metrics)
@@ -116,14 +173,21 @@
         "--prediction-dir",
         "-p",
         type=Path,
         required=True,
         help="Path to the directory containing BIO prediction files.",
     )
     parser.add_argument(
+        "--nerval-threshold",
+        "-t",
+        type=float,
+        default=30.0,
+        help="Threshold of acceptable character errors for Nerval, must be in the range: [0.0, 100.0]",
+    )
+    parser.add_argument(
         "--by-category",
         "-c",
         action="store_true",
         help="Whether to compute scores for each semantic category.",
     )
 
 
@@ -135,14 +199,16 @@
 
     commands = parser.add_subparsers(
         help="Available metrics to evaluate IE models.",
     )
     add_bow_parser(commands)
     add_botw_parser(commands)
     add_boe_parser(commands)
+    add_ecer_ewer_parser(commands)
+    add_nerval_parser(commands)
     add_summary_parser(commands)
 
     args = vars(parser.parse_args())
     if "func" in args:
         args.pop("func")(**args)
     else:
         parser.print_help()
```

### Comparing `ie-eval-0.1.0/ie_eval/metrics/bag_of_entities.py` & `ie-eval-0.2.0a1/ie_eval/metrics/bag_of_entities.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Compute the bag-of-words/bag-of-tagged-words/bag-of-entities metrics from a label/prediction dataset."""
 
 import logging
 from collections import defaultdict
 from enum import Enum
+from pathlib import Path
 
 from bio_parser import GLOBAL_STAT_NAME
 from bio_parser.parse.document import Document
 from bio_parser.utils import load_dataset
 from prettytable import PrettyTable
 
 from ie_eval.scorer import (
@@ -23,60 +24,28 @@
     """Word Type."""
 
     word = "word"
     tagged_word = "tagged_word"
     entity = "entity"
 
 
-def prepare_word_list(document: Document) -> dict[str, list[str]]:
-    """Get list of words (overall and by category).
+def prepare(document: Document, attr_name: str, with_category: bool = False):
+    """Get list of words, tagged words or entities (overall and by category).
 
     Args:
-        document (Document): An input document.
-
-    Returns:
-        A dictionary with categories as keys and corresponding list of words as values.
-    """
-    words = defaultdict(list)
-    for category, text in document.word_entities:
-        words[category].append(text)
-        words[GLOBAL_STAT_NAME].append(text)
-    return words
-
-
-def prepare_tagged_word_list(document: Document) -> dict[str, list[tuple[str, str]]]:
-    """Get list of tagged words (overall and by category).
-
-    Args:
-        document (Document): An input document.
-
-    Returns:
-        A dictionary with categories as keys and corresponding list of tagged words as values.
-    """
-    words = defaultdict(list)
-    for category, text in document.word_entities:
-        words[category].append((category, text))
-        words[GLOBAL_STAT_NAME].append((category, text))
-    return words
-
-
-def prepare_tagged_entity_list(document: Document) -> dict[str, list[tuple[str, str]]]:
-    """Get list of tagged entities/fields (overall and by category).
-
-    Args:
-        document (Document): An input document.
-
-    Returns:
-        A dictionary with categories as keys and corresponding list of tagged entities as values.
-    """
-    words = defaultdict(list)
-    for category, text in document.entities:
-        words[category].append((category, text))
-        words[GLOBAL_STAT_NAME].append((category, text))
-    return words
+        document (Document): Processed document
+        attr_name (str): Name of the attribute which holds the objects to store
+        with_category (bool, optional): Store the category along the word. Defaults to False.
+    """
+    prepared_data = defaultdict(list)
+    for category, text in getattr(document, attr_name):
+        data = (category, text) if with_category else text
+        prepared_data[category].append(data)
+        prepared_data[GLOBAL_STAT_NAME].append(data)
+    return prepared_data
 
 
 def tokenize_entities(
     label: Document,
     prediction: Document,
     word_type: WordType,
 ) -> tuple[
@@ -90,36 +59,32 @@
         prediction (Document): the prediction document
         word_type (WordType): Whether to consider a list of words, list tagged words, or list of tagged entities.
 
     Returns:
         a label dictionary with categories as keys and corresponding list of words, tagged words or tagged entities as values.
         a prediction dictionary with categories as keys and corresponding list of words, tagged words or tagged entities as values.
     """
+    kwargs = {}
     match word_type:
         case WordType.word:
             # Return list of words
-            return (prepare_word_list(label), prepare_word_list(prediction))
+            kwargs = {"attr_name": "word_entities"}
         case WordType.tagged_word:
             # Return list of tagged words
-            return (
-                prepare_tagged_word_list(label),
-                prepare_tagged_word_list(prediction),
-            )
-        case _:
+            kwargs = {"attr_name": "word_entities", "with_category": True}
+        case WordType.entity:
             # Return list of tagged entities
-            return (
-                prepare_tagged_entity_list(label),
-                prepare_tagged_entity_list(prediction),
-            )
+            kwargs = {"attr_name": "entities", "with_category": True}
+    return (prepare(document=label, **kwargs), prepare(document=prediction, **kwargs))
 
 
 def compute_bag_of_anything(
     dataset: list[tuple[Document, Document]],
     by_category: bool = False,
-    word_type: str = WordType.word,
+    word_type: WordType = WordType.word,
     print_table: bool = True,
 ) -> PrettyTable:
     """Compute bag-of-words, bag-of-tagged-words, or bag-of-entities.
 
     Args:
         dataset (list[tuple[Document, Document]]): a dataset containing a list of tuple with the label and corresponding prediction.
         word_type (WordType): Type of words to use for bag-of-words computation.
@@ -174,16 +139,16 @@
     )
     if print_table:
         print(table)  # noqa: T201
     return table
 
 
 def compute_bag_of_words(
-    label_dir: Document,
-    prediction_dir: Document,
+    label_dir: Path,
+    prediction_dir: Path,
     by_category: bool = False,
 ) -> PrettyTable:
     """Compute bag-of-words.
 
     Args:
         label_dir (Path): Path to the label directory.
         prediction_dir (Path): Path to the prediction directory.
@@ -196,16 +161,16 @@
         load_dataset(label_dir=label_dir, prediction_dir=prediction_dir),
         by_category=by_category,
         word_type=WordType.word,
     )
 
 
 def compute_bag_of_tagged_words(
-    label_dir: Document,
-    prediction_dir: Document,
+    label_dir: Path,
+    prediction_dir: Path,
     by_category: bool = False,
 ) -> PrettyTable:
     """Compute bag-of-tagged-words.
 
     Args:
         label_dir (Path): Path to the label directory.
         prediction_dir (Path): Path to the prediction directory.
@@ -218,16 +183,16 @@
         load_dataset(label_dir=label_dir, prediction_dir=prediction_dir),
         by_category=by_category,
         word_type=WordType.tagged_word,
     )
 
 
 def compute_bag_of_entities(
-    label_dir: Document,
-    prediction_dir: Document,
+    label_dir: Path,
+    prediction_dir: Path,
     by_category: bool = False,
 ) -> PrettyTable:
     """Compute bag-of-entities.
 
     Args:
         label_dir (Path): Path to the label directory.
         prediction_dir (Path): Path to the prediction directory.
```

### Comparing `ie-eval-0.1.0/ie_eval/metrics/utils.py` & `ie-eval-0.2.0a1/ie_eval/metrics/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """Utils."""
 
 from pathlib import Path
 
 from bio_parser.utils import load_dataset
 from prettytable import PrettyTable
 
+from ie_eval.metrics.assignment_based import (
+    compute_oiecerewer,
+    compute_oinerval,
+)
 from ie_eval.metrics.bag_of_entities import WordType, compute_bag_of_anything
 from ie_eval.table_formatter import make_summary_table
 
 
 def compute_all_metrics(
     label_dir: Path,
     prediction_dir: Path,
+    nerval_threshold: float = 30.0,
     by_category: bool = False,
 ) -> PrettyTable:
     """Compute all metrics.
 
     Args:
         label_dir (Path): Path to the label directory.
         prediction_dir (Path): Path to the prediction directory.
@@ -39,15 +44,30 @@
     )
     boe_table = compute_bag_of_anything(
         dataset,
         by_category,
         WordType.entity,
         print_table=False,
     )
+    ecer_ewer_table = compute_oiecerewer(
+        label_dir,
+        prediction_dir,
+        by_category,
+        print_table=False,
+    )
+    nerval_table = compute_oinerval(
+        label_dir,
+        prediction_dir,
+        nerval_threshold,
+        by_category,
+        print_table=False,
+    )
 
     table = make_summary_table(
         bow_table=bow_table,
         botw_table=botw_table,
         boe_table=boe_table,
+        ecer_ewer_table=ecer_ewer_table,
+        nerval_table=nerval_table,
     )
     print(table)  # noqa: T201
     return table
```

### Comparing `ie-eval-0.1.0/ie_eval.egg-info/PKG-INFO` & `ie-eval-0.2.0a1/ie_eval.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ie-eval
-Version: 0.1.0
-Author-email: Oliver Tüselmann <oliver.tueselmann@tu-dortmund.de>, David Villanova Aparisi <davilap@inf.upv.es>, Yoann Schneider <yschneider@teklia.com>, Solène Tarride <starride@teklia.com>
+Version: 0.2.0a1
+Author-email: Solène Tarride <starride@teklia.com>, David Villanova Aparisi <davilap@inf.upv.es>, Yoann Schneider <yschneider@teklia.com>
 Maintainer-email: Yoann Schneider <yschneider@teklia.com>, Solène Tarride <starride@teklia.com>
 License: MIT License
         
         Copyright (c) 2023 TEKLIA
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ie-eval-0.1.0/pyproject.toml` & `ie-eval-0.2.0a1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ie-eval"
-version = "0.1.0"
+version = "0.2.0a1"
 dynamic = ["dependencies", "optional-dependencies"]
 authors = [
-    { name = "Oliver Tüselmann", email = "oliver.tueselmann@tu-dortmund.de" },
+    { name = "Solène Tarride", email = "starride@teklia.com" },
     { name = "David Villanova Aparisi", email = "davilap@inf.upv.es" },
     { name = "Yoann Schneider", email = "yschneider@teklia.com" },
-    { name = "Solène Tarride", email = "starride@teklia.com" },
 ]
 maintainers = [
     { name = "Yoann Schneider", email = "yschneider@teklia.com" },
     { name = "Solène Tarride", email = "starride@teklia.com" },
 ]
 requires-python = ">=3.10"
 readme = { file = "README.md", content-type = "text/markdown" }
```

### Comparing `ie-eval-0.1.0/setup.py` & `ie-eval-0.2.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `ie-eval-0.1.0/tests/test_bag_of_entities.py` & `ie-eval-0.2.0a1/tests/test_bag_of_entities.py`

 * *Files identical despite different names*

