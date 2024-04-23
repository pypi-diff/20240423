# Comparing `tmp/nyckel-0.4.4.tar.gz` & `tmp/nyckel-0.4.5.tar.gz`

## Comparing `nyckel-0.4.4.tar` & `nyckel-0.4.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 nyckel-0.4.4/mkdocs.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.4.4/requirements.txt
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.4.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.4.4/.github/workflows/docs.yml
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.4.4/.github/workflows/test.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.4.4/.vscode/extensions.json
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 nyckel-0.4.4/.vscode/settings.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/copy_function.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/credentials.md
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/data_classes.md
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/delete_label.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/delete_samples.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/image_classification.md
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/image_tags.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/index.md
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/merge_labels.md
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/multimodal_classification.md
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/quickstart.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/requirements.txt
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/tabular_classification.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/text_classification.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/text_tags.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/assets/favicon.ico
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/assets/nyckel-logo.png
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/__init__.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/auth.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/config.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/data_classes.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/image_processing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/py.typed
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/request_utils.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/__init__.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/__init__.py
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/classification.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/factory.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/function_handler.py
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/image_classification.py
--rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/label_handler.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/sample_handler.py
--rw-r--r--   0        0        0    14969 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/tabular_classification.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/text_classification.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/__init__.py
--rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/image_tags.py
--rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/tabular_tags.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/tags.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/tags_function_factory.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/tags_function_handler.py
--rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/tags_sample_handler.py
--rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/text_tags.py
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/conftest.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_duplicates_handling.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_field_handler.py
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_image_classification_function.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_image_decoder.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_image_tags_function.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_label_handler.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_sample_handler.py
--rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_tabular_classification_function.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_tabular_tags_function.py
--rw-r--r--   0        0        0    10974 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_tags_shared.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_text_classification_function.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_white_background.py
--rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/fixtures/flower.jpg
--rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/fixtures/mixed-alpha-background.png
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.4.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.4.4/LICENSE
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 nyckel-0.4.4/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 nyckel-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 nyckel-0.4.5/mkdocs.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.4.5/requirements.txt
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.4.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.4.5/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.4.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.4.5/.vscode/extensions.json
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 nyckel-0.4.5/.vscode/settings.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/copy_function.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/credentials.md
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/data_classes.md
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/delete_label.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/delete_samples.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/image_classification.md
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/image_tags.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/index.md
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/merge_labels.md
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/multimodal_classification.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/quickstart.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/requirements.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/tabular_classification.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/text_classification.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/text_tags.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/assets/nyckel-logo.png
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.4.5/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/__init__.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/auth.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/config.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/data_classes.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/image_processing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/py.typed
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/request_utils.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/__init__.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/__init__.py
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/classification.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/factory.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/function_handler.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/image_classification.py
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/label_handler.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/sample_handler.py
+-rw-r--r--   0        0        0    14225 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/tabular_classification.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/classification/text_classification.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/__init__.py
+-rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/image_tags.py
+-rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/tabular_tags.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/tags.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/tags_function_factory.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/tags_function_handler.py
+-rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/tags_sample_handler.py
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 nyckel-0.4.5/src/nyckel/functions/tags/text_tags.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/conftest.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_duplicates_handling.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_field_handler.py
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_image_classification_function.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_image_decoder.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_image_tags_function.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_label_handler.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_sample_handler.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_tabular_classification_function.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_tabular_tags_function.py
+-rw-r--r--   0        0        0    10974 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_tags_shared.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_text_classification_function.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/test_white_background.py
+-rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/fixtures/flower.jpg
+-rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 nyckel-0.4.5/tests/fixtures/mixed-alpha-background.png
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.4.5/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.4.5/LICENSE
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 nyckel-0.4.5/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 nyckel-0.4.5/PKG-INFO
```

### Comparing `nyckel-0.4.4/mkdocs.yml` & `nyckel-0.4.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/.github/workflows/build.yml` & `nyckel-0.4.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/.github/workflows/docs.yml` & `nyckel-0.4.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/.github/workflows/test.yml` & `nyckel-0.4.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/.vscode/settings.json` & `nyckel-0.4.5/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/docs/copy_function.md` & `nyckel-0.4.5/docs/copy_function.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/docs/delete_label.md` & `nyckel-0.4.5/docs/delete_label.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/docs/delete_samples.md` & `nyckel-0.4.5/docs/delete_samples.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/docs/index.md` & `nyckel-0.4.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/docs/merge_labels.md` & `nyckel-0.4.5/docs/merge_labels.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/docs/multimodal_classification.md` & `nyckel-0.4.5/docs/multimodal_classification.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/docs/quickstart.md` & `nyckel-0.4.5/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/docs/assets/favicon.ico` & `nyckel-0.4.5/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/docs/assets/nyckel-logo.png` & `nyckel-0.4.5/docs/assets/nyckel-logo.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/__init__.py` & `nyckel-0.4.5/src/nyckel/__init__.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/auth.py` & `nyckel-0.4.5/src/nyckel/auth.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/image_processing.py` & `nyckel-0.4.5/src/nyckel/image_processing.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/request_utils.py` & `nyckel-0.4.5/src/nyckel/request_utils.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/functions/utils.py` & `nyckel-0.4.5/src/nyckel/functions/utils.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/functions/classification/classification.py` & `nyckel-0.4.5/src/nyckel/functions/classification/classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/functions/classification/factory.py` & `nyckel-0.4.5/src/nyckel/functions/classification/factory.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/functions/classification/function_handler.py` & `nyckel-0.4.5/src/nyckel/functions/classification/function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/functions/classification/image_classification.py` & `nyckel-0.4.5/src/nyckel/functions/classification/image_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/functions/classification/label_handler.py` & `nyckel-0.4.5/src/nyckel/functions/classification/label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/functions/classification/sample_handler.py` & `nyckel-0.4.5/src/nyckel/functions/classification/sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/functions/classification/tabular_classification.py` & `nyckel-0.4.5/src/nyckel/functions/classification/tabular_classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,41 +135,26 @@
         if len(samples) == 0:
             return []
 
         typed_samples = self._wrangle_post_samples_input(samples)
         typed_samples = self._strip_label_names(typed_samples)
         self._assert_fields_created(typed_samples)
         self._create_labels_as_needed(typed_samples)
-        typed_samples = self._switch_field_names_to_field_ids(typed_samples)
         return self._sample_handler.create_samples(typed_samples, self._get_image_field_transformer())
 
     def _get_image_field_transformer(self) -> Callable:
         fields = self.list_fields()
-        image_field_transformer = lambda x: x  # type: ignore  # noqa: E731
+        image_field_transformer = lambda x: x  # noqa: E731
         for field in fields:
             if field.type == "Image":
                 # There is only one image field (max) per function, so we can break here.
-                image_field_transformer = ImageFieldTransformer(field.id)  # type: ignore
+                image_field_transformer = ImageFieldTransformer(field.name)
                 break
         return image_field_transformer
 
-    def _switch_field_names_to_field_ids(
-        self, samples: List[TabularClassificationSample]
-    ) -> List[TabularClassificationSample]:
-
-        samples = copy.deepcopy(samples)  # Deep-copy so we don't modify the callers input.
-        fields = self.list_fields()
-        field_id_by_name = {field.name: field.id for field in fields}
-        for sample in samples:
-            field_names = list(sample.data.keys())
-            for field_name in field_names:
-                field_value = sample.data.pop(field_name)
-                sample.data[field_id_by_name[field_name]] = field_value  # type: ignore
-        return samples
-
     def list_samples(self) -> List[TabularClassificationSample]:  # type: ignore
         samples_dict_list = self._sample_handler.list_samples(self.sample_count)
         labels = self._label_handler.list_labels(None)
         fields = self.list_fields()
 
         label_name_by_id = {label.id: label.name for label in labels}
         field_name_by_id = {field.id: field.name for field in fields}  # type: ignore
```

### Comparing `nyckel-0.4.4/src/nyckel/functions/classification/text_classification.py` & `nyckel-0.4.5/src/nyckel/functions/classification/text_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/functions/tags/image_tags.py` & `nyckel-0.4.5/src/nyckel/functions/tags/image_tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/functions/tags/tabular_tags.py` & `nyckel-0.4.5/src/nyckel/functions/tags/tabular_tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,23 +199,28 @@
         if len(samples) == 0:
             return []
 
         typed_samples = self._wrangle_post_samples_input(samples)
         typed_samples = self._strip_label_names(typed_samples)
         self._assert_fields_created(typed_samples)
         self._create_labels_as_needed(typed_samples)
-        typed_samples = self._switch_field_names_to_field_ids(typed_samples)
         return self._sample_handler.create_samples(typed_samples, self._get_image_field_transformer())
 
     def _wrangle_post_samples_input(
         self, samples: Sequence[Union[TabularTagsSample, TabularSampleData]]
     ) -> List[TabularTagsSample]:
-        return [
-            sample if isinstance(sample, TabularTagsSample) else TabularTagsSample(data=sample) for sample in samples
-        ]
+        typed_samples: List[TabularTagsSample] = []
+        for sample in samples:
+            if isinstance(sample, TabularTagsSample):
+                typed_samples.append(sample)
+            elif isinstance(sample, dict):
+                typed_samples.append(TabularTagsSample(data=sample))
+            else:
+                raise ValueError(f"Sample {sample} has invalid type: {type(sample)}")
+        return typed_samples
 
     def _strip_label_names(self, samples: List[TabularTagsSample]) -> List[TabularTagsSample]:
         for sample in samples:
             if sample.annotation:
                 for entry in sample.annotation:
                     entry.label_name = entry.label_name.strip()
         return samples
@@ -235,32 +240,21 @@
             if sample.annotation:
                 new_label_names |= {annotation.label_name for annotation in sample.annotation}
         missing_label_names = new_label_names - existing_label_names
         missing_labels = [ClassificationLabel(name=label_name) for label_name in missing_label_names]
         if len(missing_labels) > 0:
             self._label_handler.create_labels(missing_labels)
 
-    def _switch_field_names_to_field_ids(self, samples: List[TabularTagsSample]) -> List[TabularTagsSample]:
-        samples = copy.deepcopy(samples)  # Deep-copy so we don't modify the callers input.
-        fields = self.list_fields()
-        field_id_by_name = {field.name: field.id for field in fields}
-        for sample in samples:
-            field_names = list(sample.data.keys())
-            for field_name in field_names:
-                field_value = sample.data.pop(field_name)
-                sample.data[field_id_by_name[field_name]] = field_value  # type: ignore
-        return samples
-
     def _get_image_field_transformer(self) -> Callable:
         fields = self.list_fields()
-        image_field_transformer = lambda x: x  # type: ignore  # noqa: E731
+        image_field_transformer = lambda x: x  # noqa: E731
         for field in fields:
             if field.type == "Image":
                 # There is only one image field (max) per function, so we can break here.
-                image_field_transformer = ImageFieldTransformer(field.id)  # type: ignore
+                image_field_transformer = ImageFieldTransformer(field.name)
                 break
         return image_field_transformer
 
     def list_samples(self) -> List[TabularTagsSample]:
         samples_dict_list = self._sample_handler.list_samples(self.sample_count)
         labels = self._label_handler.list_labels(None)
         fields = self.list_fields()
```

### Comparing `nyckel-0.4.4/src/nyckel/functions/tags/tags.py` & `nyckel-0.4.5/src/nyckel/functions/tags/tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from typing import List, Optional, Sequence
 
-from nyckel import NyckelId
+from nyckel.data_classes import NyckelId
 from nyckel.functions.classification.classification import (
     ClassificationPrediction,
     ImageSampleData,
     TabularSampleData,
     TextSampleData,
 )
```

### Comparing `nyckel-0.4.4/src/nyckel/functions/tags/tags_function_factory.py` & `nyckel-0.4.5/src/nyckel/functions/tags/tags_function_factory.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/functions/tags/tags_function_handler.py` & `nyckel-0.4.5/src/nyckel/functions/tags/tags_function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/functions/tags/tags_sample_handler.py` & `nyckel-0.4.5/src/nyckel/functions/tags/tags_sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/src/nyckel/functions/tags/text_tags.py` & `nyckel-0.4.5/src/nyckel/functions/tags/text_tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/tests/conftest.py` & `nyckel-0.4.5/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,29 @@
     ImageClassificationFunction,
     ImageClassificationSample,
     ImageEncoder,
     ImageTagsFunction,
     TabularClassificationFunction,
     TabularClassificationSample,
     TabularTagsFunction,
+    TabularTagsSample,
+    TagsAnnotation,
     TextClassificationFunction,
     TextClassificationSample,
     TextTagsFunction,
 )
 from nyckel.functions.classification.classification import TabularFunctionField
 from PIL import Image
 
+standard_tabular_test_fields = [
+    TabularFunctionField(name="name", type="Text"),
+    TabularFunctionField(name="age", type="Number"),
+    TabularFunctionField(name="mug", type="Image"),
+]
+
 
 def make_random_image(size: int = 100) -> str:
     imarray = np.random.rand(size, size, 3) * 255
     img = Image.fromarray(imarray.astype("uint8")).convert("RGB")
     return ImageEncoder().to_base64(img)
 
 
@@ -48,14 +56,20 @@
 def hold_until_list_samples_available(function: ClassificationFunction, expected_count: int) -> None:
     actual_count = 0
     while not actual_count == expected_count:
         actual_count = len(function.list_samples())
         time.sleep(0.25)
 
 
+def hold_until_function_trained(func: ClassificationFunction) -> None:
+    while not func.has_trained_model():
+        print("-> No trained model yet. Sleeping 1 sec...")
+        time.sleep(1)
+
+
 @pytest.fixture
 def auth_test_credentials() -> Iterator[Credentials]:
     credentials = get_test_credentials()
     assert_credentials_has_access(credentials)
     if not credentials_has_project(credentials):
         create_project_for_credentials(credentials)
     yield credentials
@@ -94,60 +108,43 @@
 def image_classification_function(auth_test_credentials: Credentials) -> Iterator[ImageClassificationFunction]:
     func = ImageClassificationFunction.create("PYTHON-SDK IMAGE TEST FUNCTION", auth_test_credentials)
     yield func
     func.delete()
 
 
 @pytest.fixture
-def image_classification_function_with_content(
-    auth_test_credentials: Credentials,
-) -> Iterator[ImageClassificationFunction]:
-    func = ImageClassificationFunction.create("PYTHON-SDK IMAGE TEST FUNCTION", auth_test_credentials)
-    labels_to_create = [ClassificationLabel(name="Nice"), ClassificationLabel(name="Boo")]
-    func.create_labels(labels_to_create)
-    nice = ClassificationAnnotation(label_name="Nice")
-    boo = ClassificationAnnotation(label_name="Boo")
-    samples = [
-        ImageClassificationSample(data=make_random_image(), external_id="1", annotation=nice),
-        ImageClassificationSample(data=make_random_image(), external_id="2", annotation=nice),
-        ImageClassificationSample(data=make_random_image(), external_id="3", annotation=boo),
-        ImageClassificationSample(data=make_random_image(), external_id="4", annotation=boo),
-        ImageClassificationSample(data=make_random_image(), external_id="5"),
-    ]
-    func.create_samples(samples)
-    hold_until_list_samples_available(func, len(samples))
+def tabular_classification_function(auth_test_credentials: Credentials) -> Iterator[TabularClassificationFunction]:
+    func = TabularClassificationFunction.create("PYTHON-SDK TABULAR TEST FUNCTION", auth_test_credentials)
     yield func
     func.delete()
 
 
 @pytest.fixture
-def tabular_classification_function(auth_test_credentials: Credentials) -> Iterator[TabularClassificationFunction]:
+def tabular_classification_function_with_fields(auth_test_credentials: Credentials) -> Iterator[ImageTagsFunction]:
     func = TabularClassificationFunction.create("PYTHON-SDK TABULAR TEST FUNCTION", auth_test_credentials)
+    func.create_fields(standard_tabular_test_fields)
     yield func
     func.delete()
 
 
 @pytest.fixture
-def tabular_classification_function_with_content(
+def trained_tabular_classification_function(
     auth_test_credentials: Credentials,
 ) -> Iterator[TabularClassificationFunction]:
     func = TabularClassificationFunction.create("PYTHON-SDK TABULAR TEST FUNCTION", auth_test_credentials)
-    labels_to_create = [ClassificationLabel(name="Nice"), ClassificationLabel(name="Boo")]
-    func.create_labels(labels_to_create)
-    nice = ClassificationAnnotation(label_name="Nice")
-    boo = ClassificationAnnotation(label_name="Boo")
+
+    func.create_fields(standard_tabular_test_fields)
     samples = [
-        TabularClassificationSample(data={"firstname": "Adam", "lastname": "Adams"}, external_id="1", annotation=nice),
-        TabularClassificationSample(data={"firstname": "Bo", "lastname": "Biden"}, external_id="2", annotation=nice),
-        TabularClassificationSample(data={"firstname": "Carl", "lastname": "Carrot"}, external_id="3", annotation=boo),
-        TabularClassificationSample(data={"firstname": "Dick", "lastname": "Denali"}, external_id="4", annotation=boo),
-        TabularClassificationSample(data={"firstname": "Erik", "lastname": "Elk"}, external_id="5"),
+        TabularClassificationSample(data=make_random_tabular(), annotation=ClassificationAnnotation(label_name="a")),
+        TabularClassificationSample(data=make_random_tabular(), annotation=ClassificationAnnotation(label_name="a")),
+        TabularClassificationSample(data=make_random_tabular(), annotation=ClassificationAnnotation(label_name="b")),
+        TabularClassificationSample(data=make_random_tabular(), annotation=ClassificationAnnotation(label_name="b")),
     ]
     func.create_samples(samples)
-    hold_until_list_samples_available(func, len(samples))
+    hold_until_function_trained(func)
     yield func
     func.delete()
 
 
 @pytest.fixture
 def text_tags_function(auth_test_credentials: Credentials) -> Iterator[TextTagsFunction]:
     func = TextTagsFunction.create("PYTHON-SDK TEXT TAGS TEST FUNCTION", auth_test_credentials)
@@ -159,29 +156,40 @@
 def image_tags_function(auth_test_credentials: Credentials) -> Iterator[ImageTagsFunction]:
     func = ImageTagsFunction.create("PYTHON-SDK IMAGE TAGS TEST FUNCTION", auth_test_credentials)
     yield func
     func.delete()
 
 
 @pytest.fixture
-def tabular_tags_function(auth_test_credentials: Credentials) -> Iterator[ImageTagsFunction]:
+def tabular_tags_function(auth_test_credentials: Credentials) -> Iterator[TabularTagsFunction]:
     func = TabularTagsFunction.create("PYTHON-SDK TABULAR TAGS TEST FUNCTION", auth_test_credentials)
     yield func
     func.delete()
 
 
 @pytest.fixture
-def tabular_tags_function_with_fields(auth_test_credentials: Credentials) -> Iterator[ImageTagsFunction]:
+def tabular_tags_function_with_fields(auth_test_credentials: Credentials) -> Iterator[TabularTagsFunction]:
     func = TabularTagsFunction.create("PYTHON-SDK TABULAR TAGS TEST FUNCTION", auth_test_credentials)
-    fields = [
-        TabularFunctionField(name="name", type="Text"),
-        TabularFunctionField(name="age", type="Number"),
-        TabularFunctionField(name="mug", type="Image"),
+    func.create_fields(standard_tabular_test_fields)
+    yield func
+    func.delete()
+
+
+@pytest.fixture
+def trained_tabular_tags_function(auth_test_credentials: Credentials) -> Iterator[TabularTagsFunction]:
+    func = TabularTagsFunction.create("PYTHON-SDK TABULAR TAGS TEST FUNCTION", auth_test_credentials)
+    func.create_fields(standard_tabular_test_fields)
+    samples = [
+        TabularTagsSample(data=make_random_tabular(), annotation=[TagsAnnotation(label_name="a")]),
+        TabularTagsSample(data=make_random_tabular(), annotation=[TagsAnnotation(label_name="a")]),
+        TabularTagsSample(data=make_random_tabular(), annotation=[TagsAnnotation(label_name="b")]),
+        TabularTagsSample(data=make_random_tabular(), annotation=[TagsAnnotation(label_name="b")]),
     ]
-    func.create_fields(fields)
+    func.create_samples(samples)
+    hold_until_function_trained(func)
     yield func
     func.delete()
 
 
 def get_test_credentials() -> Credentials:
     if "NYCKEL_PYTHON_SDK_CLIENT_SECRET" in os.environ:
         credentials = Credentials(
```

### Comparing `nyckel-0.4.4/tests/test_duplicates_handling.py` & `nyckel-0.4.5/tests/test_duplicates_handling.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/tests/test_field_handler.py` & `nyckel-0.4.5/tests/test_field_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/tests/test_image_classification_function.py` & `nyckel-0.4.5/tests/test_image_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/tests/test_image_decoder.py` & `nyckel-0.4.5/tests/test_image_decoder.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/tests/test_image_tags_function.py` & `nyckel-0.4.5/tests/test_image_tags_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/tests/test_label_handler.py` & `nyckel-0.4.5/tests/test_label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/tests/test_sample_handler.py` & `nyckel-0.4.5/tests/test_sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/tests/test_tabular_classification_function.py` & `nyckel-0.4.5/tests/test_tabular_classification_function.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import time
 import warnings
 from typing import Dict, Tuple, Union
 
 import pytest
+from conftest import make_random_image
 from nyckel import (
     ClassificationAnnotation,
     ClassificationLabel,
     ClassificationPrediction,
     ImageDecoder,
     TabularClassificationFunction,
     TabularClassificationSample,
@@ -133,7 +134,54 @@
     time.sleep(1)
     samples = tabular_classification_function.list_samples()
     assert isinstance(samples[0].data["mug"], str)
     img = ImageDecoder().to_image(samples[0].data["mug"])
 
     # The tabular filed uploader will resize the images to 384x384
     assert max(img.size) == 384
+
+
+local_image_file = os.path.abspath("tests/fixtures/flower.jpg")
+
+
+class TestImageFieldOverloading:
+    """Testing various way of giving the image field in the sample data."""
+
+    @pytest.mark.parametrize(
+        "sample",
+        [
+            TabularClassificationSample(data={"name": "Adam", "age": 32, "mug": "https://picsum.photos/40"}),
+            TabularClassificationSample(data={"name": "Adam", "age": 32, "mug": "https://picsum.photos/2000"}),
+            TabularClassificationSample(data={"name": "Adam", "age": 32, "mug": make_random_image()}),
+            TabularClassificationSample(data={"name": "Adam", "age": 32, "mug": local_image_file}),
+        ],
+    )
+    def test_post_sample(
+        self,
+        tabular_classification_function_with_fields: TabularClassificationFunction,
+        sample: TabularClassificationSample,
+    ) -> None:
+        func = tabular_classification_function_with_fields
+        func.create_samples([sample])
+        time.sleep(0.5)
+        assert func.sample_count == 1
+
+
+class TestInvokeFieldOverloading:
+
+    @pytest.mark.parametrize(
+        "sample",
+        [
+            TabularClassificationSample(data={"name": "Adam", "age": 32, "mug": "https://picsum.photos/40"}),
+            TabularClassificationSample(data={"name": "Adam", "age": 32, "mug": "https://picsum.photos/2000"}),
+            TabularClassificationSample(data={"name": "Adam", "age": 32, "mug": make_random_image()}),
+            TabularClassificationSample(data={"name": "Adam", "age": 32, "mug": local_image_file}),
+        ],
+    )
+    def test_invoke(
+        self,
+        trained_tabular_classification_function: TabularClassificationFunction,
+        sample: TabularClassificationSample,
+    ) -> None:
+        func = trained_tabular_classification_function
+        pred = func.invoke([sample.data])[0]
+        assert isinstance(pred, ClassificationPrediction)
```

### Comparing `nyckel-0.4.4/tests/test_tags_shared.py` & `nyckel-0.4.5/tests/test_tags_shared.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/tests/test_text_classification_function.py` & `nyckel-0.4.5/tests/test_text_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/tests/test_white_background.py` & `nyckel-0.4.5/tests/test_white_background.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/tests/fixtures/flower.jpg` & `nyckel-0.4.5/tests/fixtures/flower.jpg`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/tests/fixtures/mixed-alpha-background.png` & `nyckel-0.4.5/tests/fixtures/mixed-alpha-background.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/.gitignore` & `nyckel-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/LICENSE` & `nyckel-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/README.md` & `nyckel-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.4/pyproject.toml` & `nyckel-0.4.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/nyckel"]
 
 [project]
 name = "nyckel"
-version = "0.4.4"
+version = "0.4.5"
 authors = [{ name = "Oscar Beijbom", email = "oscar@nyckel.com" }]
 description = "Python package for the Nyckel API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `nyckel-0.4.4/PKG-INFO` & `nyckel-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nyckel
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python package for the Nyckel API
 Project-URL: Homepage, https://github.com/NyckelAI/python-sdk
 Author-email: Oscar Beijbom <oscar@nyckel.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

