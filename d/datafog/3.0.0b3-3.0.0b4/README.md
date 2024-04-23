# Comparing `tmp/datafog-3.0.0b3.tar.gz` & `tmp/datafog-3.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.0.0b3.tar", last modified: Mon Apr 22 19:01:09 2024, max compression
+gzip compressed data, was "datafog-3.0.0b4.tar", last modified: Tue Apr 23 04:29:35 2024, max compression
```

## Comparing `datafog-3.0.0b3.tar` & `datafog-3.0.0b4.tar`

### file list

```diff
@@ -1,24 +1,12 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 19:01:09.874369 datafog-3.0.0b3/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-04-21 22:55:54.000000 datafog-3.0.0b3/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     7705 2024-04-22 19:01:09.874126 datafog-3.0.0b3/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     6353 2024-04-21 22:55:54.000000 datafog-3.0.0b3/README.md
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-04-22 19:01:09.874419 datafog-3.0.0b3/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1679 2024-04-22 19:00:14.000000 datafog-3.0.0b3/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 19:01:09.871244 datafog-3.0.0b3/src/
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 19:01:09.872166 datafog-3.0.0b3/src/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       29 2024-04-22 19:00:06.000000 datafog-3.0.0b3/src/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1929 2024-04-22 18:52:58.000000 datafog-3.0.0b3/src/datafog/__init__.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 19:01:09.873304 datafog-3.0.0b3/src/datafog/image_processors/
--rw-r--r--   0 sidmohan   (501) staff       (20)       46 2024-04-22 17:55:38.000000 datafog-3.0.0b3/src/datafog/image_processors/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     4216 2024-04-22 18:57:45.000000 datafog-3.0.0b3/src/datafog/image_processors/donut_model.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2101 2024-04-21 23:54:11.000000 datafog-3.0.0b3/src/datafog/models.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      318 2024-04-21 23:54:42.000000 datafog-3.0.0b3/src/datafog/utils.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 19:01:09.873752 datafog-3.0.0b3/src/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     7705 2024-04-22 19:01:09.000000 datafog-3.0.0b3/src/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      411 2024-04-22 19:01:09.000000 datafog-3.0.0b3/src/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-04-22 19:01:09.000000 datafog-3.0.0b3/src/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       76 2024-04-22 19:01:09.000000 datafog-3.0.0b3/src/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       13 2024-04-22 19:01:09.000000 datafog-3.0.0b3/src/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)     2044 2024-04-22 18:55:04.000000 datafog-3.0.0b3/src/test.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-22 19:01:09.873532 datafog-3.0.0b3/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)      934 2024-04-21 23:54:11.000000 datafog-3.0.0b3/tests/test_datafog.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-23 04:29:35.325180 datafog-3.0.0b4/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-04-23 03:14:56.000000 datafog-3.0.0b4/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7574 2024-04-23 04:29:35.325063 datafog-3.0.0b4/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6353 2024-04-23 03:14:56.000000 datafog-3.0.0b4/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-23 04:29:35.324871 datafog-3.0.0b4/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7574 2024-04-23 04:29:35.000000 datafog-3.0.0b4/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      180 2024-04-23 04:29:35.000000 datafog-3.0.0b4/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-04-23 04:29:35.000000 datafog-3.0.0b4/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      172 2024-04-23 04:29:35.000000 datafog-3.0.0b4/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-04-23 04:29:35.000000 datafog-3.0.0b4/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-04-23 04:29:35.325223 datafog-3.0.0b4/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1766 2024-04-23 03:30:35.000000 datafog-3.0.0b4/setup.py
```

### Comparing `datafog-3.0.0b3/LICENSE` & `datafog-3.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.0.0b3/PKG-INFO` & `datafog-3.0.0b4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.0.0b3
+Version: 3.0.0b4
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
 Project-URL: Homepage, https://datafog.ai
 Project-URL: Documentation, https://docs.datafog.ai
 Project-URL: Discord, https://discord.gg/bzDth394R4
 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python
 Keywords: pii,redaction,nlp,rag,retrieval augmented generation
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: tox
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas==2.2.2
-Requires-Dist: pytest==8.0.2
-Requires-Dist: Requests==2.31.0
-Requires-Dist: spacy==3.4.4
-Requires-Dist: en_spacy_pii_fast
 
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
@@ -166,7 +162,9 @@
 
 ```
 
 ## License
 
 This software is published under the [MIT
 license](https://en.wikipedia.org/wiki/MIT_License).
+
+
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.0.0b3 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.0.0b4 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
-pii,redaction,nlp,rag,retrieval augmented generation Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Framework :: tox Classifier: Framework :: Pytest
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Science/Research Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pandas==2.2.2 Requires-Dist: pytest==8.0.2 Requires-Dist: Requests==2.31.0
-Requires-Dist: spacy==3.4.4 Requires-Dist: en_spacy_pii_fast
+pii,redaction,nlp,rag,retrieval augmented generation Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Framework :: tox
+Classifier: Framework :: Pytest Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: Information Technology Classifier: Intended Audience :: System
+Administrators Requires-Python: >=3.10 Description-Content-Type: text/markdown
+License-File: LICENSE
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
```

### Comparing `datafog-3.0.0b3/README.md` & `datafog-3.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.0.0b3/setup.py` & `datafog-3.0.0b4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.0.0-beta.3"
+    return "3.0.0-beta.4"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
@@ -23,19 +23,24 @@
     version=__version__(),
     author="DataFog",
     author_email="hi@datafog.ai",
     description="Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
-        "pandas==2.2.2",
-        "pytest==8.0.2",
-        "Requests==2.31.0",
-        "spacy==3.4.4",
-        "en_spacy_pii_fast",
+"en_spacy_pii_fast==0.0.0",
+"pandas==2.2.2",
+"Pillow==10.3.0",
+"pydantic==1.10.8",
+"pytest==8.0.2",
+"Requests==2.31.0",
+"setuptools==58.1.0",
+"torch==2.2.2",
+        "transformers==4.40.0",
+        "protobuf==5.26.1",
     ],
     python_requires=">=3.10",
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `datafog-3.0.0b3/src/datafog.egg-info/PKG-INFO` & `datafog-3.0.0b4/datafog.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.0.0b3
+Version: 3.0.0b4
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
 Project-URL: Homepage, https://datafog.ai
 Project-URL: Documentation, https://docs.datafog.ai
 Project-URL: Discord, https://discord.gg/bzDth394R4
 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python
 Keywords: pii,redaction,nlp,rag,retrieval augmented generation
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: tox
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas==2.2.2
-Requires-Dist: pytest==8.0.2
-Requires-Dist: Requests==2.31.0
-Requires-Dist: spacy==3.4.4
-Requires-Dist: en_spacy_pii_fast
 
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
@@ -166,7 +162,9 @@
 
 ```
 
 ## License
 
 This software is published under the [MIT
 license](https://en.wikipedia.org/wiki/MIT_License).
+
+
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.0.0b3 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.0.0b4 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
-pii,redaction,nlp,rag,retrieval augmented generation Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Framework :: tox Classifier: Framework :: Pytest
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Science/Research Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pandas==2.2.2 Requires-Dist: pytest==8.0.2 Requires-Dist: Requests==2.31.0
-Requires-Dist: spacy==3.4.4 Requires-Dist: en_spacy_pii_fast
+pii,redaction,nlp,rag,retrieval augmented generation Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Framework :: tox
+Classifier: Framework :: Pytest Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: Information Technology Classifier: Intended Audience :: System
+Administrators Requires-Python: >=3.10 Description-Content-Type: text/markdown
+License-File: LICENSE
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
```

