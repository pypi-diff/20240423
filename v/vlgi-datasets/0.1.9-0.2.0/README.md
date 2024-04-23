# Comparing `tmp/vlgi_datasets-0.1.9.tar.gz` & `tmp/vlgi_datasets-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlgi_datasets-0.1.9.tar", last modified: Mon Apr 22 18:35:51 2024, max compression
+gzip compressed data, was "vlgi_datasets-0.2.0.tar", last modified: Mon Apr 22 18:50:38 2024, max compression
```

## Comparing `vlgi_datasets-0.1.9.tar` & `vlgi_datasets-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 18:35:51.636818 vlgi_datasets-0.1.9/
--rw-rw-rw-   0        0        0     1259 2024-04-22 18:35:51.634816 vlgi_datasets-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      694 2024-04-12 14:03:49.000000 vlgi_datasets-0.1.9/README.md
--rw-rw-rw-   0        0        0      727 2024-04-22 18:35:04.000000 vlgi_datasets-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 18:35:51.636818 vlgi_datasets-0.1.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-22 18:35:51.620700 vlgi_datasets-0.1.9/vlgi_datasets/
--rw-rw-rw-   0        0        0      371 2024-04-12 14:03:49.000000 vlgi_datasets-0.1.9/vlgi_datasets/__init__.py
--rw-rw-rw-   0        0        0     1398 2024-04-11 11:53:01.000000 vlgi_datasets-0.1.9/vlgi_datasets/open_pyxl_dataset.py
--rw-rw-rw-   0        0        0     2727 2024-04-12 14:03:49.000000 vlgi_datasets-0.1.9/vlgi_datasets/pdf_dataset.py
--rw-rw-rw-   0        0        0     2090 2024-04-12 14:03:49.000000 vlgi_datasets-0.1.9/vlgi_datasets/postgres_soft_replace_dataset.py
--rw-rw-rw-   0        0        0     2566 2024-04-12 14:03:49.000000 vlgi_datasets-0.1.9/vlgi_datasets/postgres_upsert_table.py
--rw-rw-rw-   0        0        0     2475 2024-04-22 18:32:34.000000 vlgi_datasets-0.1.9/vlgi_datasets/sharepoint_excel_dataset.py
-drwxrwxrwx   0        0        0        0 2024-04-22 18:35:51.633816 vlgi_datasets-0.1.9/vlgi_datasets.egg-info/
--rw-rw-rw-   0        0        0     1259 2024-04-22 18:35:51.000000 vlgi_datasets-0.1.9/vlgi_datasets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2024-04-22 18:35:51.000000 vlgi_datasets-0.1.9/vlgi_datasets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 18:35:51.000000 vlgi_datasets-0.1.9/vlgi_datasets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-22 18:35:51.000000 vlgi_datasets-0.1.9/vlgi_datasets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-22 18:35:51.000000 vlgi_datasets-0.1.9/vlgi_datasets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 18:50:38.218025 vlgi_datasets-0.2.0/
+-rw-rw-rw-   0        0        0     1259 2024-04-22 18:50:38.216023 vlgi_datasets-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      694 2024-04-12 14:03:49.000000 vlgi_datasets-0.2.0/README.md
+-rw-rw-rw-   0        0        0      727 2024-04-22 18:50:05.000000 vlgi_datasets-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-22 18:50:38.218025 vlgi_datasets-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-22 18:50:38.200955 vlgi_datasets-0.2.0/vlgi_datasets/
+-rw-rw-rw-   0        0        0      453 2024-04-22 18:47:47.000000 vlgi_datasets-0.2.0/vlgi_datasets/__init__.py
+-rw-rw-rw-   0        0        0     1398 2024-04-11 11:53:01.000000 vlgi_datasets-0.2.0/vlgi_datasets/open_pyxl_dataset.py
+-rw-rw-rw-   0        0        0     2727 2024-04-12 14:03:49.000000 vlgi_datasets-0.2.0/vlgi_datasets/pdf_dataset.py
+-rw-rw-rw-   0        0        0     2090 2024-04-12 14:03:49.000000 vlgi_datasets-0.2.0/vlgi_datasets/postgres_soft_replace_dataset.py
+-rw-rw-rw-   0        0        0     2566 2024-04-12 14:03:49.000000 vlgi_datasets-0.2.0/vlgi_datasets/postgres_upsert_table.py
+-rw-rw-rw-   0        0        0     2475 2024-04-22 18:45:24.000000 vlgi_datasets-0.2.0/vlgi_datasets/sharepoint_excel_dataset.py
+drwxrwxrwx   0        0        0        0 2024-04-22 18:50:38.215026 vlgi_datasets-0.2.0/vlgi_datasets.egg-info/
+-rw-rw-rw-   0        0        0     1259 2024-04-22 18:50:38.000000 vlgi_datasets-0.2.0/vlgi_datasets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-04-22 18:50:38.000000 vlgi_datasets-0.2.0/vlgi_datasets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 18:50:38.000000 vlgi_datasets-0.2.0/vlgi_datasets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-22 18:50:38.000000 vlgi_datasets-0.2.0/vlgi_datasets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-22 18:50:38.000000 vlgi_datasets-0.2.0/vlgi_datasets.egg-info/top_level.txt
```

### Comparing `vlgi_datasets-0.1.9/PKG-INFO` & `vlgi_datasets-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlgi-datasets
-Version: 0.1.9
+Version: 0.2.0
 Summary: A package with custom kedro datasets for VLGI
 Author-email: Tecnologia Grupo Sozo <tecnologia@gruposozo.com.br>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `vlgi_datasets-0.1.9/README.md` & `vlgi_datasets-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vlgi_datasets-0.1.9/pyproject.toml` & `vlgi_datasets-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vlgi-datasets"
-version = "0.1.9"
+version = "0.2.0"
 description = "A package with custom kedro datasets for VLGI"
 authors = [
     { "name" = "Tecnologia Grupo Sozo", "email" = "tecnologia@gruposozo.com.br"}
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `vlgi_datasets-0.1.9/vlgi_datasets/open_pyxl_dataset.py` & `vlgi_datasets-0.2.0/vlgi_datasets/open_pyxl_dataset.py`

 * *Files identical despite different names*

### Comparing `vlgi_datasets-0.1.9/vlgi_datasets/pdf_dataset.py` & `vlgi_datasets-0.2.0/vlgi_datasets/pdf_dataset.py`

 * *Files identical despite different names*

### Comparing `vlgi_datasets-0.1.9/vlgi_datasets/postgres_soft_replace_dataset.py` & `vlgi_datasets-0.2.0/vlgi_datasets/postgres_soft_replace_dataset.py`

 * *Files identical despite different names*

### Comparing `vlgi_datasets-0.1.9/vlgi_datasets/postgres_upsert_table.py` & `vlgi_datasets-0.2.0/vlgi_datasets/postgres_upsert_table.py`

 * *Files identical despite different names*

### Comparing `vlgi_datasets-0.1.9/vlgi_datasets/sharepoint_excel_dataset.py` & `vlgi_datasets-0.2.0/vlgi_datasets/sharepoint_excel_dataset.py`

 * *Files identical despite different names*

### Comparing `vlgi_datasets-0.1.9/vlgi_datasets.egg-info/PKG-INFO` & `vlgi_datasets-0.2.0/vlgi_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlgi-datasets
-Version: 0.1.9
+Version: 0.2.0
 Summary: A package with custom kedro datasets for VLGI
 Author-email: Tecnologia Grupo Sozo <tecnologia@gruposozo.com.br>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

