# Comparing `tmp/memento-scorecard-1.3.2.tar.gz` & `tmp/memento-scorecard-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memento-scorecard-1.3.2.tar", last modified: Mon Jun 19 07:37:40 2023, max compression
+gzip compressed data, was "memento-scorecard-2.0.0.tar", last modified: Mon Apr 22 21:41:56 2024, max compression
```

## Comparing `memento-scorecard-1.3.2.tar` & `memento-scorecard-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 07:37:40.680210 memento-scorecard-1.3.2/
--rw-rw-rw-   0        0        0    11558 2023-06-07 21:33:58.000000 memento-scorecard-1.3.2/LICENSE
--rw-rw-rw-   0        0        0     1157 2023-06-19 07:37:40.677219 memento-scorecard-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       46 2023-06-07 21:33:58.000000 memento-scorecard-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 07:37:40.649291 memento-scorecard-1.3.2/memento/
--rw-rw-rw-   0        0        0     1384 2023-06-19 07:35:54.000000 memento-scorecard-1.3.2/memento/__init__.py
--rw-rw-rw-   0        0        0    28781 2023-06-19 07:35:26.000000 memento-scorecard-1.3.2/memento/bojack.py
--rw-rw-rw-   0        0        0     7582 2023-06-15 23:06:58.000000 memento-scorecard-1.3.2/memento/diane.py
--rw-rw-rw-   0        0        0    20641 2023-06-15 23:07:02.000000 memento-scorecard-1.3.2/memento/mr_peanutbutter.py
--rw-rw-rw-   0        0        0    23946 2023-06-15 23:07:00.000000 memento-scorecard-1.3.2/memento/princess_carolyn.py
--rw-rw-rw-   0        0        0     3243 2023-06-15 23:06:56.000000 memento-scorecard-1.3.2/memento/todd.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:37:40.673227 memento-scorecard-1.3.2/memento_scorecard.egg-info/
--rw-rw-rw-   0        0        0     1157 2023-06-19 07:37:40.000000 memento-scorecard-1.3.2/memento_scorecard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-06-19 07:37:40.000000 memento-scorecard-1.3.2/memento_scorecard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 07:37:40.000000 memento-scorecard-1.3.2/memento_scorecard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-19 07:37:40.000000 memento-scorecard-1.3.2/memento_scorecard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 07:37:40.680210 memento-scorecard-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-06-07 21:36:49.000000 memento-scorecard-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 21:41:56.295221 memento-scorecard-2.0.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-22 21:15:34.000000 memento-scorecard-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1132 2024-04-22 21:41:56.295221 memento-scorecard-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-04-22 21:15:34.000000 memento-scorecard-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 21:41:56.263956 memento-scorecard-2.0.0/memento/
+-rw-rw-rw-   0        0        0     1375 2024-04-22 21:41:48.000000 memento-scorecard-2.0.0/memento/__init__.py
+-rw-rw-rw-   0        0        0   105626 2024-04-22 21:41:22.000000 memento-scorecard-2.0.0/memento/memento.py
+drwxrwxrwx   0        0        0        0 2024-04-22 21:41:56.279611 memento-scorecard-2.0.0/memento_scorecard.egg-info/
+-rw-rw-rw-   0        0        0     1132 2024-04-22 21:41:56.000000 memento-scorecard-2.0.0/memento_scorecard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-04-22 21:41:56.000000 memento-scorecard-2.0.0/memento_scorecard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 21:41:56.000000 memento-scorecard-2.0.0/memento_scorecard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-22 21:41:56.000000 memento-scorecard-2.0.0/memento_scorecard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 21:41:56.295221 memento-scorecard-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1467 2024-04-22 21:41:32.000000 memento-scorecard-2.0.0/setup.py
```

### Comparing `memento-scorecard-1.3.2/LICENSE` & `memento-scorecard-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `memento-scorecard-1.3.2/PKG-INFO` & `memento-scorecard-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: memento-scorecard
-Version: 1.3.2
+Version: 2.0.0
 Summary: Scorecard development with Python
 Home-page: https://github.com/Guilliu/Memento
 Author: Guillermo Lizcano Villafáñez
 Author-email: guille.lv.97@gmail.com
 License: Apache License 2.0
 Keywords: python,scoring,rating,logistic,regression,scorecard,woe,credit-risk,autogrouping
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Memento - Scorecard development with Python
 
-**Memento** is a Python package with the aim of providing the necessary tools for:
+*Memento* is a Python package with the aim of providing the necessary tools for:
 
 - Grouping variables (both numerical and categorical) in an automatic and interactive way.
 - Development of customizable scorecards adaptable to the requirements of each user.
 
 ## Source code
 Check out the [GitHub](https://github.com/Guilliu/Memento) repository.
 
 ## Documentation
 You can find useful documentation [here](https://guilliu.github.io/).
-
-
```

### Comparing `memento-scorecard-1.3.2/memento/__init__.py` & `memento-scorecard-2.0.0/memento/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-from memento.todd import (string_categories1, string_categories2, string_to_num,
-breakpoints_to_str, breakpoints_to_num, remapeo_missing, data_convert, adapt_data)
-from memento.diane import (compute_group_names, compute_table, transform_to_woes,
-calib_score, compute_scorecard, transform_to_points, apply_scorecard, compute_metrics)
-from memento.princess_carolyn import (compute_final_breakpoints,
-compute_info, features_selection, display_table_ng, reagrupa_var)
-from memento.mr_peanutbutter import (pretty_scorecard, parceling, cell_style,
-predict_pyspark, metrics_pyspark, compute_pyspark_ks, save_model,
-save_light_model, load_model, genera_punt_par, proc_freq)
-from memento.bojack import Scorecard, Autogrouping
+from memento.memento import (
+    string_categories1, string_categories2, string_to_num,
+    breakpoints_to_str, breakpoints_to_num, remapeo_missing, data_convert, adapt_data,
+    split, autogrouping,
+    compute_group_names, compute_table, transform_to_woes,
+    calib_score, compute_scorecard, transform_to_points, apply_scorecard, compute_metrics,
+    compute_final_breakpoints,
+    compute_info, features_selection, table_ng, reagrupa_var, interfaz_grafica,
+    pretty_scorecard, parceling, cell_style,
+    predict_pyspark, metrics_pyspark, compute_pyspark_ks, save_model,
+    save_light_model, load_model, genera_punt_par, proc_freq,
+    Scorecard, Autogrouping
+)
 
-__version__ = '1.3.2'
+__version__ = '2.0.0'
 
 __all__ = (
     string_categories1, string_categories2, string_to_num,
     breakpoints_to_str, breakpoints_to_num, remapeo_missing, data_convert, adapt_data,
+    split, autogrouping,
     compute_group_names, compute_table, transform_to_woes,
     calib_score, compute_scorecard, transform_to_points, apply_scorecard, compute_metrics,
     compute_final_breakpoints,
-    compute_info, features_selection, display_table_ng, reagrupa_var,
+    compute_info, features_selection, table_ng, reagrupa_var, interfaz_grafica,
     pretty_scorecard, parceling, cell_style,
     predict_pyspark, metrics_pyspark, compute_pyspark_ks, save_model,
     save_light_model, load_model, genera_punt_par, proc_freq,
     Scorecard, Autogrouping
 )
```

### Comparing `memento-scorecard-1.3.2/memento_scorecard.egg-info/PKG-INFO` & `memento-scorecard-2.0.0/memento_scorecard.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: memento-scorecard
-Version: 1.3.2
+Version: 2.0.0
 Summary: Scorecard development with Python
 Home-page: https://github.com/Guilliu/Memento
 Author: Guillermo Lizcano Villafáñez
 Author-email: guille.lv.97@gmail.com
 License: Apache License 2.0
 Keywords: python,scoring,rating,logistic,regression,scorecard,woe,credit-risk,autogrouping
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Memento - Scorecard development with Python
 
-**Memento** is a Python package with the aim of providing the necessary tools for:
+*Memento* is a Python package with the aim of providing the necessary tools for:
 
 - Grouping variables (both numerical and categorical) in an automatic and interactive way.
 - Development of customizable scorecards adaptable to the requirements of each user.
 
 ## Source code
 Check out the [GitHub](https://github.com/Guilliu/Memento) repository.
 
 ## Documentation
 You can find useful documentation [here](https://guilliu.github.io/).
-
-
```

### Comparing `memento-scorecard-1.3.2/setup.py` & `memento-scorecard-2.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-import re
-from setuptools import setup, find_packages
-
-with open('memento/__init__.py', encoding='utf-8') as f:
-    version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', f.read()).group(1)
-
-setup(
-    name='memento-scorecard',
-    version=version,
-    url='https://github.com/Guilliu/Memento',
-    author='Guillermo Lizcano Villafáñez',
-    author_email='guille.lv.97@gmail.com',
-    description='Scorecard development with Python',
-    license='Apache License 2.0',
-    packages=find_packages(),
-    keywords=['python', 'scoring', 'rating', 'logistic', 'regression',
-    'scorecard', 'woe', 'credit-risk', 'autogrouping'],
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: Apache Software License',
-        'Operating System :: OS Independent',
-        'Development Status :: 5 - Production/Stable'
-    ],
-    long_description_content_type='text/markdown',
-    long_description='''
-# Memento - Scorecard development with Python
-
-**Memento** is a Python package with the aim of providing the necessary tools for:
-
-- Grouping variables (both numerical and categorical) in an automatic and interactive way.
-- Development of customizable scorecards adaptable to the requirements of each user.
-
-## Source code
-Check out the [GitHub](https://github.com/Guilliu/Memento) repository.
-
-## Documentation
-You can find useful documentation [here](https://guilliu.github.io/).
-'''
-)
-
+import re
+from setuptools import setup, find_packages
+
+with open('memento/__init__.py', encoding='utf-8') as f:
+    version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', f.read()).group(1)
+
+setup(
+    name='memento-scorecard',
+    version=version,
+    url='https://github.com/Guilliu/Memento',
+    author='Guillermo Lizcano Villafáñez',
+    author_email='guille.lv.97@gmail.com',
+    description='Scorecard development with Python',
+    license='Apache License 2.0',
+    packages=find_packages(),
+    keywords=['python', 'scoring', 'rating', 'logistic', 'regression',
+    'scorecard', 'woe', 'credit-risk', 'autogrouping'],
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: Apache Software License',
+        'Operating System :: OS Independent',
+        'Development Status :: 5 - Production/Stable'
+    ],
+    long_description_content_type='text/markdown',
+    long_description='''
+# Memento - Scorecard development with Python
+
+*Memento* is a Python package with the aim of providing the necessary tools for:
+
+- Grouping variables (both numerical and categorical) in an automatic and interactive way.
+- Development of customizable scorecards adaptable to the requirements of each user.
+
+## Source code
+Check out the [GitHub](https://github.com/Guilliu/Memento) repository.
+
+## Documentation
+You can find useful documentation [here](https://guilliu.github.io/).
+'''
+)
```

