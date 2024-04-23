# Comparing `tmp/cytomine-python-client-2.4.1.tar.gz` & `tmp/cytomine-python-client-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cytomine-python-client-2.4.1.tar", last modified: Wed Apr  3 08:03:29 2024, max compression
+gzip compressed data, was "cytomine-python-client-3.0.0.tar", last modified: Tue Apr 23 13:59:43 2024, max compression
```

## Comparing `cytomine-python-client-2.4.1.tar` & `cytomine-python-client-3.0.0.tar`

### file list

```diff
@@ -1,45 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:03:29.873130 cytomine-python-client-2.4.1/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2296 2024-04-03 08:03:29.873130 cytomine-python-client-2.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1684 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:03:29.869130 cytomine-python-client-2.4.1/cytomine/
--rwxrwxrwx   0 root         (0) root         (0)     1016 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    53983 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/cytomine.py
--rw-rw-rw-   0 root         (0) root         (0)    13962 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/cytomine_job.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:03:29.869130 cytomine-python-client-2.4.1/cytomine/models/
--rwxrwxrwx   0 root         (0) root         (0)     2739 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:03:29.873130 cytomine-python-client-2.4.1/cytomine/models/_utilities/
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/_utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/_utilities/dump.py
--rw-rw-rw-   0 root         (0) root         (0)     4425 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/_utilities/parallel.py
--rw-rw-rw-   0 root         (0) root         (0)     1527 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/_utilities/pattern_matching.py
--rw-rw-rw-   0 root         (0) root         (0)    16521 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)    11155 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/collection.py
--rwxrwxrwx   0 root         (0) root         (0)    23887 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/image.py
--rwxrwxrwx   0 root         (0) root         (0)     4644 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/model.py
--rwxrwxrwx   0 root         (0) root         (0)     3624 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/ontology.py
--rwxrwxrwx   0 root         (0) root         (0)     3502 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/project.py
--rw-rw-rw-   0 root         (0) root         (0)     7958 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/property.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/social.py
--rwxrwxrwx   0 root         (0) root         (0)    12863 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/software.py
--rw-rw-rw-   0 root         (0) root         (0)     3300 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/storage.py
--rw-rw-rw-   0 root         (0) root         (0)     2994 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/track.py
--rwxrwxrwx   0 root         (0) root         (0)     8394 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:03:29.873130 cytomine-python-client-2.4.1/cytomine/utilities/
--rw-rw-rw-   0 root         (0) root         (0)      972 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/utilities/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     5646 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/utilities/descriptor_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     3527 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/utilities/geometry.py
--rwxrwxrwx   0 root         (0) root         (0)    11203 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/utilities/reader.py
--rw-rw-rw-   0 root         (0) root         (0)     4621 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/utilities/software.py
--rwxrwxrwx   0 root         (0) root         (0)     4412 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/utilities/wholeslide.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:03:29.873130 cytomine-python-client-2.4.1/cytomine_python_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2296 2024-04-03 08:03:29.000000 cytomine-python-client-2.4.1/cytomine_python_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1102 2024-04-03 08:03:29.000000 cytomine-python-client-2.4.1/cytomine_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:03:29.000000 cytomine-python-client-2.4.1/cytomine_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-03 08:03:29.000000 cytomine-python-client-2.4.1/cytomine_python_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-03 08:03:29.000000 cytomine-python-client-2.4.1/cytomine_python_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      973 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/requirements-py2.7.txt
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 08:03:29.873130 cytomine-python-client-2.4.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2299 2024-04-03 08:03:29.000000 cytomine-python-client-2.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:59:43.901433 cytomine-python-client-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2024-04-03 08:01:55.000000 cytomine-python-client-3.0.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      558 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2011 2024-04-23 13:59:43.901433 cytomine-python-client-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:59:43.901433 cytomine-python-client-3.0.0/cytomine/
+-rwxrwxrwx   0 root         (0) root         (0)      769 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28038 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/cytomine.py
+-rw-rw-rw-   0 root         (0) root         (0)    13716 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/cytomine_job.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:59:43.901433 cytomine-python-client-3.0.0/cytomine/models/
+-rwxrwxrwx   0 root         (0) root         (0)     2492 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:59:43.901433 cytomine-python-client-3.0.0/cytomine/models/_utilities/
+-rw-rw-rw-   0 root         (0) root         (0)      817 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/_utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2989 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/_utilities/dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     5077 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/_utilities/parallel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2179 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/_utilities/pattern_matching.py
+-rw-rw-rw-   0 root         (0) root         (0)    12447 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)    10908 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/collection.py
+-rwxrwxrwx   0 root         (0) root         (0)    22835 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/image.py
+-rwxrwxrwx   0 root         (0) root         (0)     4397 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/model.py
+-rwxrwxrwx   0 root         (0) root         (0)     3377 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/ontology.py
+-rwxrwxrwx   0 root         (0) root         (0)     3255 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     7603 2024-04-08 14:26:12.000000 cytomine-python-client-3.0.0/cytomine/models/property.py
+-rw-rw-rw-   0 root         (0) root         (0)     6869 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/social.py
+-rwxrwxrwx   0 root         (0) root         (0)    12616 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/software.py
+-rw-rw-rw-   0 root         (0) root         (0)     3053 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2747 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/track.py
+-rwxrwxrwx   0 root         (0) root         (0)     8147 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:59:43.901433 cytomine-python-client-3.0.0/cytomine/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)      653 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2024-04-03 08:01:55.000000 cytomine-python-client-3.0.0/cytomine/utilities/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5598 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/cytomine/utilities/descriptor_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     4621 2024-04-03 08:01:55.000000 cytomine-python-client-3.0.0/cytomine/utilities/software.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 13:59:43.901433 cytomine-python-client-3.0.0/cytomine_python_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2011 2024-04-23 13:59:43.000000 cytomine-python-client-3.0.0/cytomine_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-23 13:59:43.000000 cytomine-python-client-3.0.0/cytomine_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 13:59:43.000000 cytomine-python-client-3.0.0/cytomine_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2024-04-23 13:59:43.000000 cytomine-python-client-3.0.0/cytomine_python_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-23 13:59:43.000000 cytomine-python-client-3.0.0/cytomine_python_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      781 2024-04-08 14:24:50.000000 cytomine-python-client-3.0.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 13:59:43.901433 cytomine-python-client-3.0.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1989 2024-04-23 13:59:43.000000 cytomine-python-client-3.0.0/setup.py
```

### Comparing `cytomine-python-client-2.4.1/LICENSE` & `cytomine-python-client-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.1/PKG-INFO` & `cytomine-python-client-3.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 Metadata-Version: 2.1
 Name: cytomine-python-client
-Version: 2.4.1
+Version: 3.0.0
 Summary: Python client to interact with Cytomine.
 Home-page: https://www.cytomine.org
 License: LICENSE
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: NOTICE
 
 # Cytomine-python-client
 
-When using our software, we kindly ask you to cite our website url and related publications in all your work (publications, studies, oral presentations,...). In particular, we recommend to cite (Marée et al., Bioinformatics 2016) paper, and to use our logo when appropriate. See our license files for additional details.
+All data available from the Cytomine graphical interface can be manipulated programmatically from your computer. This page introduces the key concepts on how to interact with Cytomine without this graphical interface. Cytomine is a RESTful application. 
+It means that the data stored and managed by Cytomine can be obtained through specific URLs. Contrary to the graphical interface, these URLs only provide relevant information data.
 
-- URL: http://www.cytomine.org
-- Logo: http://www.cytomine.org/sites/default/files/inline-images/logo-300-org.png
-- Scientific paper: Raphaël Marée, Loïc Rollus, Benjamin Stévens, Renaud Hoyoux, Gilles Louppe, Rémy Vandaele, Jean-Michel Begon, Philipp Kainz, Pierre Geurts and Louis Wehenkel. Collaborative analysis of multi-gigapixel imaging data using Cytomine, Bioinformatics, DOI: 10.1093/bioinformatics/btw013, 2016. https://doi.org/10.1093/bioinformatics/btw013
+To ease interaction with Cytomine, the **Cytomine API client for Python** encapsulates all the technical details relative to the HTTP API so that you can manipulate Cytomine resources without complexity.
 
+## Install
 
-Cytomine (http://doc.cytomine.org) client and utilities in Python.
+```
+pip install cytomine-python-client
+```
 
-Cytomine client contains functions to import/export data (projects, ontologies, images, users, annotations, softwares, ... ) from/to Cytomine core server based on the RESTful API.
+For versions lower than `2.3.4`, refer to [manual installation guide](https://doc.cytomine.com/dev-guide/clients/python/installation).
 
-Cytomine utilities contains various functions including ones to access whole slide images (tiles, ...) and basic image processing tools.
+## Documentation
+* [How to interact with Cytomine programmatically introduction](https://doc.cytomine.com/dev-guide/api/)
+* [How to use the API client for Python](https://doc.cytomine.com/dev-guide/clients/python/usage)
 
-See examples in https://github.com/cytomine/Cytomine-python-client/tree/master/client/examples and https://github.com/cytomine/Cytomine-python-client/tree/master/utilities/examples
+## Examples
+* [Detailed examples detailed step by step](https://doc.cytomine.com/dev-guide/clients/python/examples)
+* [Examples source code](https://github.com/cytomine/Cytomine-python-client/tree/master/client/examples)
 
-The client is automatically installed with the Docker/Bootstrap procedure, however it is possible to install it independently on remote computers. See installation instructions here : [https://doc.cytomine.org/Python-client](https://doc.cytomine.org/Python-client?structure=DataScientists)
 
+# More about Cytomine
+* [Cytomine Corporation SA](https://cytomine.com)
+* [Cytomine documentation](https://doc.cytomine.com)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/README.md` & `cytomine-python-client-3.0.0/cytomine_python_client.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,46 @@
+Metadata-Version: 2.1
+Name: cytomine-python-client
+Version: 3.0.0
+Summary: Python client to interact with Cytomine.
+Home-page: https://www.cytomine.org
+License: LICENSE
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+
 # Cytomine-python-client
 
-When using our software, we kindly ask you to cite our website url and related publications in all your work (publications, studies, oral presentations,...). In particular, we recommend to cite (Marée et al., Bioinformatics 2016) paper, and to use our logo when appropriate. See our license files for additional details.
+All data available from the Cytomine graphical interface can be manipulated programmatically from your computer. This page introduces the key concepts on how to interact with Cytomine without this graphical interface. Cytomine is a RESTful application. 
+It means that the data stored and managed by Cytomine can be obtained through specific URLs. Contrary to the graphical interface, these URLs only provide relevant information data.
+
+To ease interaction with Cytomine, the **Cytomine API client for Python** encapsulates all the technical details relative to the HTTP API so that you can manipulate Cytomine resources without complexity.
+
+## Install
 
-- URL: http://www.cytomine.org
-- Logo: http://www.cytomine.org/sites/default/files/inline-images/logo-300-org.png
-- Scientific paper: Raphaël Marée, Loïc Rollus, Benjamin Stévens, Renaud Hoyoux, Gilles Louppe, Rémy Vandaele, Jean-Michel Begon, Philipp Kainz, Pierre Geurts and Louis Wehenkel. Collaborative analysis of multi-gigapixel imaging data using Cytomine, Bioinformatics, DOI: 10.1093/bioinformatics/btw013, 2016. https://doi.org/10.1093/bioinformatics/btw013
+```
+pip install cytomine-python-client
+```
 
+For versions lower than `2.3.4`, refer to [manual installation guide](https://doc.cytomine.com/dev-guide/clients/python/installation).
 
-Cytomine (http://doc.cytomine.org) client and utilities in Python.
+## Documentation
+* [How to interact with Cytomine programmatically introduction](https://doc.cytomine.com/dev-guide/api/)
+* [How to use the API client for Python](https://doc.cytomine.com/dev-guide/clients/python/usage)
 
-Cytomine client contains functions to import/export data (projects, ontologies, images, users, annotations, softwares, ... ) from/to Cytomine core server based on the RESTful API.
+## Examples
+* [Detailed examples detailed step by step](https://doc.cytomine.com/dev-guide/clients/python/examples)
+* [Examples source code](https://github.com/cytomine/Cytomine-python-client/tree/master/client/examples)
 
-Cytomine utilities contains various functions including ones to access whole slide images (tiles, ...) and basic image processing tools.
 
-See examples in https://github.com/cytomine/Cytomine-python-client/tree/master/client/examples and https://github.com/cytomine/Cytomine-python-client/tree/master/utilities/examples
+# More about Cytomine
+* [Cytomine Corporation SA](https://cytomine.com)
+* [Cytomine documentation](https://doc.cytomine.com)
 
-The client is automatically installed with the Docker/Bootstrap procedure, however it is possible to install it independently on remote computers. See installation instructions here : [https://doc.cytomine.org/Python-client](https://doc.cytomine.org/Python-client?structure=DataScientists)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/cytomine/cytomine_job.py` & `cytomine-python-client-3.0.0/cytomine/cytomine_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
@@ -23,18 +23,14 @@
 import logging
 
 from cytomine.cytomine import Cytomine, _cytomine_parameter_name_synonyms
 from cytomine.models.project import Project
 from cytomine.models.software import Software, Job, JobParameter, SoftwareParameterCollection
 from cytomine.models.user import User
 
-__author__ = "Begon Jean-Michel <jm.begon@gmail.com>"
-__contributors = ["Mormont Romain <romainmormont@gmail.com", "Rubens Ulysse <urubens@uliege.be>"]
-__copyright__ = "Copyright 2010-2022 University of Liège, Belgium, http://www.cytomine.be/"
-
 
 def _inferred_number_type(v):
     """Return the inferred type for the given string. The string must contain either an interger or a float.
     """
     try:
         return int(v)
     except ValueError:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/cytomine/models/__init__.py` & `cytomine-python-client-3.0.0/cytomine/models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
 # * Unless required by applicable law or agreed to in writing, software
 # * distributed under the License is distributed on an "AS IS" BASIS,
 # * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # * See the License for the specific language governing permissions and
 # * limitations under the License.
 
-__author__ = "Rubens Ulysse <urubens@uliege.be>"
-__contributors__ = ["Marée Raphaël <raphael.maree@uliege.be>", "Mormont Romain <r.mormont@uliege.be>"]
-__copyright__ = "Copyright 2010-2022 University of Liège, Belgium, http://www.cytomine.be/"
 
 from .model import Model, DomainModel
 from .collection import Collection, DomainCollection
 from .annotation import Annotation, AnnotationCollection, AnnotationTerm, AlgoAnnotationTerm
 from .image import AbstractImage, AbstractImageCollection, AbstractSlice, AbstractSliceCollection,\
     ImageInstance, ImageInstanceCollection, SliceInstance, SliceInstanceCollection, \
     ImageServer, ImageServerCollection
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/cytomine/models/_utilities/dump.py` & `cytomine-python-client-3.0.0/cytomine/models/_utilities/dump.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# -*- coding: utf-8 -*-
+
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
+# *
+# * Licensed under the Apache License, Version 2.0 (the "License");
+# * you may not use this file except in compliance with the License.
+# * You may obtain a copy of the License at
+# *
+# *      http://www.apache.org/licenses/LICENSE-2.0
+# *
+# * Unless required by applicable law or agreed to in writing, software
+# * distributed under the License is distributed on an "AS IS" BASIS,
+# * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# * See the License for the specific language governing permissions and
+# * limitations under the License.
+
 import os
 from shutil import copyfile
 
 from .parallel import makedirs
 from .pattern_matching import resolve_pattern
```

### Comparing `cytomine-python-client-2.4.1/cytomine/models/_utilities/parallel.py` & `cytomine-python-client-3.0.0/cytomine/models/_utilities/parallel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# -*- coding: utf-8 -*-
+
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
+# *
+# * Licensed under the Apache License, Version 2.0 (the "License");
+# * you may not use this file except in compliance with the License.
+# * You may obtain a copy of the License at
+# *
+# *      http://www.apache.org/licenses/LICENSE-2.0
+# *
+# * Unless required by applicable law or agreed to in writing, software
+# * distributed under the License is distributed on an "AS IS" BASIS,
+# * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# * See the License for the specific language governing permissions and
+# * limitations under the License.
+
 import errno
 import os
 
 try:
     import queue as queue
 except ImportError:
     import Queue as queue
```

### Comparing `cytomine-python-client-2.4.1/cytomine/models/collection.py` & `cytomine-python-client-3.0.0/cytomine/models/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
@@ -15,17 +15,14 @@
 # * limitations under the License.
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
-__author__ = "Rubens Ulysse <urubens@uliege.be>"
-__contributors__ = ["Marée Raphaël <raphael.maree@uliege.be>", "Mormont Romain <r.mormont@uliege.be>"]
-__copyright__ = "Copyright 2010-2022 University of Liège, Belgium, http://www.cytomine.be/"
 
 # Importing collections.abc objects from collections is deprecated
 # since python 3.3. 
 from sys import version_info
 if version_info.major < 3 or \
         (version_info.major == 3 and version_info.minor < 3):
     from collections import MutableSequence
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/cytomine/models/image.py` & `cytomine-python-client-3.0.0/cytomine/models/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
@@ -15,17 +15,14 @@
 # * limitations under the License.
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
-__author__ = "Rubens Ulysse <urubens@uliege.be>"
-__contributors__ = ["Marée Raphaël <raphael.maree@uliege.be>", "Mormont Romain <r.mormont@uliege.be>"]
-__copyright__ = "Copyright 2010-2022 University of Liège, Belgium, http://www.cytomine.be/"
 
 import re
 import os
 
 from cytomine.cytomine import Cytomine, deprecated
 from cytomine.models.collection import Collection
 from cytomine.models.model import Model
@@ -283,35 +280,14 @@
 
         files = generic_image_dump(dest_pattern, self, dump_url_fn, override=override, check_extension=False)
         return len(files) > 0
 
     def __str__(self):
         return "[{}] {} : {}".format(self.callback_identifier, self.id, self.instanceFilename)
 
-    def profile(self, x, y, width=None, height=None):
-        import numpy as np
-        from shapely.geometry import Point, box
-
-        geometry = box(x, y, x + width, y + height) if (width and height) else Point(x, y)
-
-        uri = "{}/{}/profile.json".format(self.callback_identifier, self.id)
-        data = Cytomine.get_instance().get(uri, {"geometry": geometry})
-
-        if width and height:
-            data = data["collection"]
-            depth = len(data[0]["profile"])
-            profile = np.empty((height, width, depth), dtype=np.uint)
-            for p in data:
-                row = p["point"][1] - y
-                col = p["point"][0] - x
-                profile[row, col, :] = p["profile"]
-            return profile
-        else:
-            return np.asarray([[data["profile"]]])
-
     def window(self, x, y, w, h, dest_pattern="{id}-{x}-{y}-{w}-{h}.jpg", override=True, mask=None, alpha=None,
                bits=8, annotations=None, terms=None, users=None, reviewed=None, complete=True, projection=None,
                max_size=None, zoom=None):
         """
         Extract a window (rectangle) from an image and download it.
 
         Parameters
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/cytomine/models/model.py` & `cytomine-python-client-3.0.0/cytomine/models/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
@@ -15,17 +15,14 @@
 # * limitations under the License.
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
-__author__ = "Rubens Ulysse <urubens@uliege.be>"
-__contributors__ = ["Marée Raphaël <raphael.maree@uliege.be>", "Mormont Romain <r.mormont@uliege.be>"]
-__copyright__ = "Copyright 2010-2022 University of Liège, Belgium, http://www.cytomine.be/"
 
 import six
 import json
 
 from cytomine.cytomine import Cytomine
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/cytomine/models/ontology.py` & `cytomine-python-client-3.0.0/cytomine/models/ontology.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
@@ -17,17 +17,14 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
 from cytomine.cytomine import Cytomine
 
-__author__ = "Rubens Ulysse <urubens@uliege.be>"
-__contributors__ = ["Marée Raphaël <raphael.maree@uliege.be>", "Mormont Romain <r.mormont@uliege.be>"]
-__copyright__ = "Copyright 2010-2022 University of Liège, Belgium, http://www.cytomine.be/"
 
 from cytomine.models.collection import Collection
 from cytomine.models.model import Model
 
 
 class Ontology(Model):
     def __init__(self, name=None, **attributes):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/cytomine/models/project.py` & `cytomine-python-client-3.0.0/cytomine/models/storage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
@@ -15,79 +15,83 @@
 # * limitations under the License.
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
-from cytomine import Cytomine
-
-__author__ = "Rubens Ulysse <urubens@uliege.be>"
-__contributors__ = ["Marée Raphaël <raphael.maree@uliege.be>", "Mormont Romain <r.mormont@uliege.be>"]
-__copyright__ = "Copyright 2010-2022 University of Liège, Belgium, http://www.cytomine.be/"
 
 from cytomine.models.collection import Collection
 from cytomine.models.model import Model
 
 
-class Project(Model):
-    def __init__(self, name=None, id_ontology=None, **attributes):
-        super(Project, self).__init__()
+class Storage(Model):
+    def __init__(self, name=None, id_user=None, **attributes):
+        super(Storage, self).__init__()
         self.name = name
-        self.ontology = id_ontology
-        self.ontologyName = None
-        self.discipline = None
-        self.blindMode = None
-        self.disciplineName = None
-        self.numberOfSlides = None
-        self.numberOfImages = None
-        self.numberOfAnnotations = None
-        self.numberOfJobAnnotations = None
-        self.retrievalProjects = None
-        self.numberOfReviewedAnnotations = None
-        self.retrievalDisable = None
-        self.retrievalAllOntology = None
-        self.isClosed = None
-        self.isReadOnly = None
-        self.hideUsersLayers = None
-        self.hideAdminsLayers = None
-
-        self.admins = None
-        self.users = None
-        self.mode = None
+        self.user = id_user
         self.populate(attributes)
 
-    def add_user(self, id_user, admin=False):
-        if admin:
-            return Cytomine.get_instance().post("project/{}/user/{}/admin.json".format(self.id, id_user))
-        else:
-            return Cytomine.get_instance().post("project/{}/user/{}.json".format(self.id, id_user))
-
-    def delete_user(self, id_user, admin=False):
-        if admin:
-            return Cytomine.get_instance().delete("project/{}/user/{}/admin.json".format(self.id, id_user))
-        else:
-            return Cytomine.get_instance().delete("project/{}/user/{}.json".format(self.id, id_user))
-
 
-class ProjectCollection(Collection):
+class StorageCollection(Collection):
     def __init__(self, filters=None, max=0, offset=0, **parameters):
-        super(ProjectCollection, self).__init__(Project, filters, max, offset)
-        self._allowed_filters = [None, "user", "software", "ontology"]
-        self.set_parameters(parameters)
+        super(StorageCollection, self).__init__(Storage, filters, max, offset)
+        self._allowed_filters = [None]
 
-    def save(self, *args, **kwargs):
-        raise NotImplementedError("Cannot save a project collection by client.")
+        self.all = None
+        self.set_parameters(parameters)
 
 
-class Discipline(Model):
-    def __init__(self, name=None, **attributes):
-        super(Discipline, self).__init__()
-        self.name = name
+class UploadedFile(Model):
+    # Old codes
+    UPLOADED = 0
+    CONVERTED = 1
+    DEPLOYED = 2
+    ERROR_FORMAT = 3
+    ERROR_CONVERT = 4
+    UNCOMPRESSED = 5
+    TO_DEPLOY = 6
+    # --
+
+    DETECTING_FORMAT = 10
+    ERROR_FORMAT = 11
+    EXTRACTING_DATA = 20
+    ERROR_EXTRACTION = 21
+    CONVERTING = 30
+    ERROR_CONVERSION = 31
+    DEPLOYING = 40
+    ERROR_DEPLOYMENT = 41
+    DEPLOYED = 100
+    EXTRACTED = 102
+    CONVERTED = 104
+
+    def __init__(self, original_filename=None, filename=None, size=None, ext=None, content_type=None,
+                 id_projects=None, id_storage=None, id_user=None, id_image_server=None, status=None, id_parent=None, **attributes):
+        super(UploadedFile, self).__init__()
+        self.originalFilename = original_filename
+        self.filename = filename
+        self.path = None
+        self.size = size
+        self.ext = ext
+        self.contentType = content_type
+        self.projects = id_projects
+        self.storage = id_storage
+        self.imageServer = id_image_server
+        self.user = id_user
+        self.status = status
+        self.statusText = None
+        self.parent = id_parent
         self.populate(attributes)
 
+    def __str__(self):
+        return "[{}] {} : {}".format(self.callback_identifier, self.id, self.filename)
 
-class DisciplineCollection(Collection):
+
+class UploadedFileCollection(Collection):
     def __init__(self, filters=None, max=0, offset=0, **parameters):
-        super(DisciplineCollection, self).__init__(Discipline, filters, max, offset)
+        super(UploadedFileCollection, self).__init__(UploadedFile, filters, max, offset)
         self._allowed_filters = [None]
+
+        self.all = None
+        self.parent = None
+        self.onlyRoots = None
         self.set_parameters(parameters)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/cytomine/models/property.py` & `cytomine-python-client-3.0.0/cytomine/models/property.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
@@ -17,17 +17,14 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
 import re
 
-__author__ = "Rubens Ulysse <urubens@uliege.be>"
-__contributors__ = ["Marée Raphaël <raphael.maree@uliege.be>", "Mormont Romain <r.mormont@uliege.be>"]
-__copyright__ = "Copyright 2010-2022 University of Liège, Belgium, http://www.cytomine.be/"
 
 from cytomine.cytomine import Cytomine
 from cytomine.models.annotation import Annotation
 from cytomine.models.collection import Collection, DomainCollection
 from cytomine.models.model import Model, DomainModel
 
 
@@ -42,18 +39,15 @@
     @property
     def obj(self):
         return self._object
 
     @obj.setter
     def obj(self, value):
         self._object = value
-        if isinstance(value, Annotation):
-            self.domainClassName = "annotation"
-        else:
-            self.domainClassName = value.class_
+        self.domainClassName = value.class_
         self.domainIdent = value.id
 
     def uri(self):
         if self._by_key and self.domainClassName and self.domainIdent and self.key:
             uri = "domain/{}/{}/key/{}/property.json".format(self.domainClassName, self.domainIdent, self.key)
         else:
             uri = super(Property, self).uri()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/cytomine/models/social.py` & `cytomine-python-client-3.0.0/cytomine/models/social.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
@@ -15,17 +15,14 @@
 # * limitations under the License.
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
-__author__ = "Rubens Ulysse <urubens@uliege.be>"
-__contributors__ = ["Marée Raphaël <raphael.maree@uliege.be>", "Mormont Romain <r.mormont@uliege.be>"]
-__copyright__ = "Copyright 2010-2022 University of Liège, Belgium, http://www.cytomine.be/"
 
 from cytomine.models.collection import Collection
 from cytomine.models.model import Model
 
 
 class Position(Model):
     def __init__(self):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/cytomine/models/software.py` & `cytomine-python-client-3.0.0/cytomine/models/software.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
@@ -19,17 +19,14 @@
 from __future__ import print_function
 from __future__ import unicode_literals
 
 import re
 
 import os
 
-__author__ = "Rubens Ulysse <urubens@uliege.be>"
-__contributors__ = ["Marée Raphaël <raphael.maree@uliege.be>", "Mormont Romain <r.mormont@uliege.be>"]
-__copyright__ = "Copyright 2010-2022 University of Liège, Belgium, http://www.cytomine.be/"
 
 from cytomine.cytomine import Cytomine
 from cytomine.models.collection import Collection
 from cytomine.models.model import Model
 
 
 class Software(Model):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/cytomine/models/track.py` & `cytomine-python-client-3.0.0/cytomine/models/track.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
@@ -15,17 +15,14 @@
 # * limitations under the License.
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
-__author__ = "Rubens Ulysse <urubens@uliege.be>"
-__contributors__ = ["Marée Raphaël <raphael.maree@uliege.be>", "Mormont Romain <r.mormont@uliege.be>"]
-__copyright__ = "Copyright 2010-2022 University of Liège, Belgium, http://www.cytomine.be/"
 
 from cytomine.cytomine import Cytomine
 from cytomine.models.collection import Collection
 from cytomine.models.model import Model
 
 
 class Track(Model):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/cytomine/models/user.py` & `cytomine-python-client-3.0.0/cytomine/models/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
@@ -15,17 +15,14 @@
 # * limitations under the License.
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 from __future__ import unicode_literals
 
-__author__ = "Rubens Ulysse <urubens@uliege.be>"
-__contributors__ = ["Marée Raphaël <raphael.maree@uliege.be>", "Mormont Romain <r.mormont@uliege.be>"]
-__copyright__ = "Copyright 2010-2022 University of Liège, Belgium, http://www.cytomine.be/"
 
 from cytomine.cytomine import Cytomine
 from cytomine.models.collection import Collection
 from cytomine.models.model import Model
 
 
 class CytomineUser:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/cytomine/utilities/__init__.py` & `cytomine-python-client-3.0.0/cytomine/models/_utilities/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
 # * Unless required by applicable law or agreed to in writing, software
 # * distributed under the License is distributed on an "AS IS" BASIS,
 # * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # * See the License for the specific language governing permissions and
 # * limitations under the License.
 
-__author__ = "Rubens Ulysse <urubens@uliege.be>"
-__contributors__ = ["Marée Raphaël <raphael.maree@uliege.be>", "Mormont Romain <r.mormont@uliege.be>"]
-__copyright__ = "Copyright 2010-2022 University of Liège, Belgium, http://www.cytomine.be/"
-
-from .geometry import *
-from .reader import *
-from .wholeslide import *
+from .parallel import generic_download, makedirs, is_false
+from .dump import generic_image_dump, DumpError
+from .pattern_matching import resolve_pattern, is_iterable
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cytomine-python-client-2.4.1/cytomine/utilities/annotations.py` & `cytomine-python-client-3.0.0/cytomine/utilities/annotations.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.1/cytomine/utilities/descriptor_reader.py` & `cytomine-python-client-3.0.0/cytomine/utilities/descriptor_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
@@ -20,15 +20,15 @@
 from __future__ import unicode_literals
 
 import json
 
 
 from cytomine.models import Software, SoftwareParameter, SoftwareCollection, SoftwareParameterCollection
 
-__author__ = "Rubens Ulysse <urubens@uliege.be>"
+
 
 
 def _format_type(type):
     if type.lower() == "listdomain":
         return "ListDomain"
     else:
         return type.lower().capitalize()
```

### Comparing `cytomine-python-client-2.4.1/cytomine/utilities/software.py` & `cytomine-python-client-3.0.0/cytomine/utilities/software.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.1/cytomine_python_client.egg-info/SOURCES.txt` & `cytomine-python-client-3.0.0/cytomine_python_client.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
+NOTICE
 README.md
-requirements-py2.7.txt
 requirements.txt
 setup.py
 cytomine/__init__.py
 cytomine/cytomine.py
 cytomine/cytomine_job.py
 cytomine/models/__init__.py
 cytomine/models/annotation.py
@@ -22,16 +22,13 @@
 cytomine/models/_utilities/__init__.py
 cytomine/models/_utilities/dump.py
 cytomine/models/_utilities/parallel.py
 cytomine/models/_utilities/pattern_matching.py
 cytomine/utilities/__init__.py
 cytomine/utilities/annotations.py
 cytomine/utilities/descriptor_reader.py
-cytomine/utilities/geometry.py
-cytomine/utilities/reader.py
 cytomine/utilities/software.py
-cytomine/utilities/wholeslide.py
 cytomine_python_client.egg-info/PKG-INFO
 cytomine_python_client.egg-info/SOURCES.txt
 cytomine_python_client.egg-info/dependency_links.txt
 cytomine_python_client.egg-info/requires.txt
 cytomine_python_client.egg-info/top_level.txt
```

### Comparing `cytomine-python-client-2.4.1/requirements-py2.7.txt` & `cytomine-python-client-3.0.0/requirements.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 #
-# This file is autogenerated by pip-compile
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
-#    pip-compile --output-file=requirements-py2.7.txt setup.py
+#    pip-compile setup.py
 #
-cachecontrol==0.12.6
-    # via Cytomine-Python-Client (setup.py)
+cachecontrol==0.12.10
+    # via cytomine-python-client (setup.py)
 certifi==2021.5.30
     # via requests
-chardet==4.0.0
+charset-normalizer==2.0.12
     # via requests
 future==0.18.2
-    # via Cytomine-Python-Client (setup.py)
-idna==2.10
+    # via cytomine-python-client (setup.py)
+idna==3.2
     # via requests
 msgpack==1.0.2
     # via cachecontrol
-numpy==1.16.6
-    # via Cytomine-Python-Client (setup.py)
-opencv-python-headless==4.2.0.32
-    # via Cytomine-Python-Client (setup.py)
-pillow==6.2.2
-    # via Cytomine-Python-Client (setup.py)
-requests-toolbelt==0.9.1
-    # via Cytomine-Python-Client (setup.py)
-requests==2.26.0
+requests==2.27.1
     # via
-    #   Cytomine-Python-Client (setup.py)
     #   cachecontrol
+    #   cytomine-python-client (setup.py)
     #   requests-toolbelt
+requests-toolbelt==0.9.1
+    # via cytomine-python-client (setup.py)
 shapely==1.7.1
-    # via Cytomine-Python-Client (setup.py)
+    # via cytomine-python-client (setup.py)
 six==1.16.0
-    # via Cytomine-Python-Client (setup.py)
+    # via cytomine-python-client (setup.py)
 urllib3==1.26.6
     # via
-    #   Cytomine-Python-Client (setup.py)
+    #   cytomine-python-client (setup.py)
     #   requests
```

### Comparing `cytomine-python-client-2.4.1/setup.py` & `cytomine-python-client-3.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# * Copyright (c) 2009-2022. Authors: see NOTICE file.
+# * Copyright (c) 2009-2024. Authors: see NOTICE file.
 # *
 # * Licensed under the Apache License, Version 2.0 (the "License");
 # * you may not use this file except in compliance with the License.
 # * You may obtain a copy of the License at
 # *
 # *      http://www.apache.org/licenses/LICENSE-2.0
 # *
@@ -17,44 +17,39 @@
 
 from setuptools import setup
 from io import open
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
-pillow_version_constraint = ',<7.0.0' if sys.version_info.major < 3 else ''
 
 setup(
     name='cytomine-python-client',
-    version='2.4.1',
+    version='3.0.0',
     description='Python client to interact with Cytomine.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['cytomine', 'cytomine.models', 'cytomine.models._utilities', 'cytomine.utilities'],
     url='https://www.cytomine.org',
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Operating System :: OS Independent'
     ],
     install_requires=['requests-toolbelt>=0.8.0',
                       'CacheControl>=0.12.10',
-                      'numpy>=1.15.4',
                       'Shapely>=1.6.4',
                       'six>=1.11.0',
                       'future>=0.17.1',
-                      'opencv-python-headless>=3.4.3',
-                      'Pillow>=5.3.0{}'.format(pillow_version_constraint),
                       'requests>=2.27.1',
                       'urllib3>=1.25.2'],
     setup_requires=['pytest-runner'],
     extra_requires={
         "test": ['pytest']
     },
     test_suite='cytomine.tests',
     license='LICENSE',
-    data_files=[('', ['LICENSE', 'requirements.txt', 'requirements-py2.7.txt'])]
+    data_files=[('', ['LICENSE', 'NOTICE', 'requirements.txt'])]
 )
```

