# Comparing `tmp/OperationBattleshipCommonUtilities-0.4.1.tar.gz` & `tmp/operationbattleshipcommonutilities-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OperationBattleshipCommonUtilities-0.4.1.tar", last modified: Sun Apr  7 21:20:50 2024, max compression
+gzip compressed data, was "operationbattleshipcommonutilities-0.4.2.tar", last modified: Mon Apr 22 23:50:03 2024, max compression
```

## Comparing `OperationBattleshipCommonUtilities-0.4.1.tar` & `operationbattleshipcommonutilities-0.4.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 21:20:50.570362 OperationBattleshipCommonUtilities-0.4.1/
--rw-rw-rw-   0        0        0    11558 2024-03-23 16:54:02.000000 OperationBattleshipCommonUtilities-0.4.1/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-07 21:20:50.563144 OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/
--rw-rw-rw-   0        0        0     3177 2024-04-07 21:20:50.000000 OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1182 2024-04-07 21:20:50.000000 OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 21:20:50.000000 OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-07 21:20:50.000000 OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2024-04-07 21:20:50.000000 OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3177 2024-04-07 21:20:50.565142 OperationBattleshipCommonUtilities-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2571 2024-03-08 06:05:09.000000 OperationBattleshipCommonUtilities-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 21:20:50.561141 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/
--rw-rw-rw-   0        0        0     4577 2024-03-24 01:03:06.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/ApifyJobsCaller.py
--rw-rw-rw-   0        0        0     2601 2024-04-01 21:52:27.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/CandidateRequirementsDao.py
--rw-rw-rw-   0        0        0     6556 2024-04-01 21:51:05.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/CompanyDao.py
--rw-rw-rw-   0        0        0     3143 2024-04-01 21:48:50.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/FailureLogger.py
--rw-rw-rw-   0        0        0     1513 2024-04-01 23:24:18.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/GenaricDatabaseDao.py
--rw-rw-rw-   0        0        0     2219 2024-04-01 21:47:52.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/GeographyHelper.py
--rw-rw-rw-   0        0        0     3365 2024-04-01 21:47:37.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobKeyWordsDao.py
--rw-rw-rw-   0        0        0    18787 2024-04-07 21:12:06.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobPostingDao.py
--rw-rw-rw-   0        0        0     1706 2024-04-01 21:39:48.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobResponsibilitiesDao.py
--rw-rw-rw-   0        0        0     2848 2024-04-01 21:39:04.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobSkillsDao.py
--rw-rw-rw-   0        0        0     1830 2024-02-17 14:46:22.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobTitleCategoryClassifier.py
--rw-rw-rw-   0        0        0      613 2024-03-12 04:49:56.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/NomicAICaller.py
--rw-rw-rw-   0        0        0     1087 2024-02-15 03:50:23.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/OpenAICaller.py
--rw-rw-rw-   0        0        0     2758 2024-03-19 02:54:10.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/PineConeDatabaseCaller.py
--rw-rw-rw-   0        0        0        0 2024-01-26 02:28:14.000000 OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-07 21:20:50.571368 OperationBattleshipCommonUtilities-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      734 2024-04-07 21:13:34.000000 OperationBattleshipCommonUtilities-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 23:50:03.011697 operationbattleshipcommonutilities-0.4.2/
+-rw-rw-rw-   0        0        0    11558 2024-03-23 16:54:02.000000 operationbattleshipcommonutilities-0.4.2/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-22 23:50:03.011697 operationbattleshipcommonutilities-0.4.2/OperationBattleshipCommonUtilities.egg-info/
+-rw-rw-rw-   0        0        0     3177 2024-04-22 23:50:02.000000 operationbattleshipcommonutilities-0.4.2/OperationBattleshipCommonUtilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1182 2024-04-22 23:50:02.000000 operationbattleshipcommonutilities-0.4.2/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 23:50:02.000000 operationbattleshipcommonutilities-0.4.2/OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-22 23:50:02.000000 operationbattleshipcommonutilities-0.4.2/OperationBattleshipCommonUtilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2024-04-22 23:50:02.000000 operationbattleshipcommonutilities-0.4.2/OperationBattleshipCommonUtilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3177 2024-04-22 23:50:03.011697 operationbattleshipcommonutilities-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2571 2024-03-08 06:05:09.000000 operationbattleshipcommonutilities-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 23:50:02.996105 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/
+-rw-rw-rw-   0        0        0     4577 2024-03-24 01:03:06.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/ApifyJobsCaller.py
+-rw-rw-rw-   0        0        0     2601 2024-04-01 21:52:27.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/CandidateRequirementsDao.py
+-rw-rw-rw-   0        0        0     6556 2024-04-01 21:51:05.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/CompanyDao.py
+-rw-rw-rw-   0        0        0     3143 2024-04-01 21:48:50.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/FailureLogger.py
+-rw-rw-rw-   0        0        0     1513 2024-04-01 23:24:18.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/GenaricDatabaseDao.py
+-rw-rw-rw-   0        0        0     2219 2024-04-01 21:47:52.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/GeographyHelper.py
+-rw-rw-rw-   0        0        0     3365 2024-04-01 21:47:37.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/JobKeyWordsDao.py
+-rw-rw-rw-   0        0        0    18787 2024-04-07 21:12:06.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/JobPostingDao.py
+-rw-rw-rw-   0        0        0     1706 2024-04-01 21:39:48.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/JobResponsibilitiesDao.py
+-rw-rw-rw-   0        0        0     2848 2024-04-01 21:39:04.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/JobSkillsDao.py
+-rw-rw-rw-   0        0        0     1830 2024-02-17 14:46:22.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/JobTitleCategoryClassifier.py
+-rw-rw-rw-   0        0        0      613 2024-03-12 04:49:56.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/NomicAICaller.py
+-rw-rw-rw-   0        0        0     1087 2024-02-15 03:50:23.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/OpenAICaller.py
+-rw-rw-rw-   0        0        0     3595 2024-04-22 23:38:11.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/PineConeDatabaseCaller.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 02:28:14.000000 operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-22 23:50:03.011697 operationbattleshipcommonutilities-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      734 2024-04-22 23:47:47.000000 operationbattleshipcommonutilities-0.4.2/setup.py
```

### Comparing `OperationBattleshipCommonUtilities-0.4.1/LICENSE` & `operationbattleshipcommonutilities-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/PKG-INFO` & `operationbattleshipcommonutilities-0.4.2/OperationBattleshipCommonUtilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OperationBattleshipCommonUtilities
-Version: 0.4.1
+Version: 0.4.2
 Summary: Classes and Utilities that are shared in the Operation Battleship Application
 Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
 Author: Matthew Caraway
 Author-email: matthew@CarawayLabs.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `OperationBattleshipCommonUtilities-0.4.1/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt` & `operationbattleshipcommonutilities-0.4.2/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/PKG-INFO` & `operationbattleshipcommonutilities-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OperationBattleshipCommonUtilities
-Version: 0.4.1
+Version: 0.4.2
 Summary: Classes and Utilities that are shared in the Operation Battleship Application
 Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
 Author: Matthew Caraway
 Author-email: matthew@CarawayLabs.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `OperationBattleshipCommonUtilities-0.4.1/README.md` & `operationbattleshipcommonutilities-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/ApifyJobsCaller.py` & `operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/ApifyJobsCaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/CandidateRequirementsDao.py` & `operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/CandidateRequirementsDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/CompanyDao.py` & `operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/CompanyDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/FailureLogger.py` & `operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/FailureLogger.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/GenaricDatabaseDao.py` & `operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/GenaricDatabaseDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/GeographyHelper.py` & `operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/GeographyHelper.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobKeyWordsDao.py` & `operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/JobKeyWordsDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobPostingDao.py` & `operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/JobPostingDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobResponsibilitiesDao.py` & `operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/JobResponsibilitiesDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobSkillsDao.py` & `operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/JobSkillsDao.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/JobTitleCategoryClassifier.py` & `operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/JobTitleCategoryClassifier.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/NomicAICaller.py` & `operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/NomicAICaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/OpenAICaller.py` & `operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/OpenAICaller.py`

 * *Files identical despite different names*

### Comparing `OperationBattleshipCommonUtilities-0.4.1/operation_battleship_common_utilities/PineConeDatabaseCaller.py` & `operationbattleshipcommonutilities-0.4.2/operation_battleship_common_utilities/PineConeDatabaseCaller.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
+import datetime
 from dotenv import load_dotenv
-
 from pinecone import Pinecone, ServerlessSpec
 
 load_dotenv('.env')
 
 
 class PineConeDatabaseCaller:
 
@@ -54,21 +54,35 @@
             vectors.append({
                 'id': id,
                 'values': embedding,
                 'metadata': data['metadata']
             })
         upsert_response = index.upsert(vectors, namespace=namespace)
         return upsert_response
-    
-    def query(self, embeddedResume, numberOfNeighbors, indexName, namsSpace):
+        
+    def query(self, embeddedResume, numberOfNeighbors, indexName, namespace, numberOfDays=45):
+        # Calculate the date to filter job postings
+        job_posting_date_cutoff = self.getIntegerValueForDayFilter(numberOfDays)
 
         index = self.pc.Index(indexName)
 
+        # Applying the job_posting_date filter
         result = index.query(
-            namespace = namsSpace,
-            vector = embeddedResume,
-            top_k = numberOfNeighbors,
-            include_metadata = True
-            )
+            namespace=namespace,
+            vector=embeddedResume,
+            filter={"job_posting_date": {"$gte": job_posting_date_cutoff}},  # Adjust this filter as per your requirements
+            top_k=numberOfNeighbors,
+            include_metadata=True
+        )
 
         return result
 
+    def getIntegerValueForDayFilter(self, numberOfDays):
+        """
+        Calculate the number of days since the Unix epoch for the date numberOfDays ago.
+        """
+        today = datetime.date.today()
+        cutoff_date = today - datetime.timedelta(days=numberOfDays)
+        epoch_start = datetime.date(1970, 1, 1)
+        days_since_epoch = (cutoff_date - epoch_start).days
+        logging.info(f"Computed days since epoch for cutoff: {days_since_epoch}")
+        return days_since_epoch
```

### Comparing `OperationBattleshipCommonUtilities-0.4.1/setup.py` & `operationbattleshipcommonutilities-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='OperationBattleshipCommonUtilities',
-    version='0.4.1',
+    version='0.4.2',
     packages=find_packages(),
     license='Apache-2.0 license',
     description='Classes and Utilities that are shared in the Operation Battleship Application',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Matthew Caraway',
     author_email='matthew@CarawayLabs.com',
```

