# Comparing `tmp/odk_tools-0.1.0.tar.gz` & `tmp/odk_tools-0.1.1.tar.gz`

## Comparing `odk_tools-0.1.0.tar` & `odk_tools-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.1.0/src/odk_tools/__init__.py
--rw-r--r--   0        0        0    10987 2020-02-02 00:00:00.000000 odk_tools-0.1.0/src/odk_tools/classes.py
--rw-r--r--   0        0        0    20221 2020-02-02 00:00:00.000000 odk_tools-0.1.0/src/odk_tools/odk.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 odk_tools-0.1.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 odk_tools-0.1.0/LICENSE
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 odk_tools-0.1.0/README.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 odk_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 odk_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.1.1/src/odk_tools/__init__.py
+-rw-r--r--   0        0        0    20111 2020-02-02 00:00:00.000000 odk_tools-0.1.1/src/odk_tools/classes.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 odk_tools-0.1.1/src/odk_tools/functions.py
+-rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 odk_tools-0.1.1/src/odk_tools/odk.py
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 odk_tools-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 odk_tools-0.1.1/LICENSE
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 odk_tools-0.1.1/README.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 odk_tools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 odk_tools-0.1.1/PKG-INFO
```

### Comparing `odk_tools-0.1.0/src/odk_tools/odk.py` & `odk_tools-0.1.1/src/odk_tools/odk.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 import pandas as pd
 import numpy as np
 import requests
 import json
 from io import BytesIO
 import copy
-import datetime as dt
 import zipfile as zip
 import xlsxwriter
 import xml.etree.ElementTree as ET
 import uuid
 from types import FunctionType
 from .classes import Form
-from getpass import getpass
+
+#%% #@ Functions
 
 def save_to_excel(data, filename="output.xlsx", column_width=25, include_index=False, row_colours={0: "#D8E4BC", 1: "#C5D9F1"}, row_bold=[0], row_wrap=[1], autofilter=True, freeze_panes=True):
 
     workbook = xlsxwriter.Workbook(filename)
     worksheet = workbook.add_worksheet()
 
     for i in range(len(data.columns)):
@@ -47,46 +47,52 @@
         worksheet.autofilter(1, 0, len(data), len(data.columns)-1)
 
     if freeze_panes:
         worksheet.freeze_panes(2, 0)
 
     workbook.close()
 
+#%% #@ ODK Class
+
 class ODK():
 
     """
     The class is used to access the ODK server and download or upload data to projects.
     class parameters:
     url
 
     class functions:\n
-    connect: connects to the ODK server\n
+    connect: connects to the webserver by providing username and password\n
     set_target: defines the project and form to connect to\n
-    get_project\n
-    get_form\n
-    save_form\n
-    save_data\n
-    get_submissions\n
-    survey\n
-    choices\n
-    get_repeats\n
-    get_attachments\n
-    processing_submission\n
-    processing_repeats\n
-    save_main\n
-    save_repeat\n
-    listing_submissions\n
-    get_submission_metadata\n
-    get_submission_xml\n
-    put_submission\n
-    return_element\n
-    modify_xml\n
-    update_xml\n
-    change_submission\n
+    list_projects:\n
+    get_project:\n
+    list_forms:\n
+    get_form:\n
+    save_form:\n
+    save_data:\n
+    get_submissions:\n
+    survey:\n
+    choices:\n
+    get_repeats:\n
+    get_attachments:\n
+    processing_submission:\n
+    processing_repeats:\n
+    process_all:\n
+    save_main:\n
+    save_repeat:\n
+    listing_submissions:\n
+    get_submission_metadata:\n
+    get_submission_xml:\n
+    put_submission:\n
+    return_element:\n
+    modify_xml:\n
+    update_xml:\n
+    change_submission:\n
     """
+
     def __init__(self, url):
         self.url=url
 
     def connect(self, email, password):
 
         self.email = email
         self.password = password
@@ -109,32 +115,35 @@
     def get_project(self):
         req = requests.get(self.url+'/v1/projects', headers=self.headers)
         project = [req.json()[i]["id"] for i in range(len(req.json()))
                 if req.json()[i]["name"] == self.project_name][0]
     
         return project
 
-    def list_forms(self,project):
+    def list_forms(self,project=None):
         req = requests.get(self.url+'/v1/projects', headers=self.headers)
-        project = [req.json()[i]["id"] for i in range(len(req.json()))
-                   if req.json()[i]["name"] == project][0]
+        if project!=None:
+            project = [req.json()[i]["id"] for i in range(len(req.json())) if req.json()[i]["name"] == project][0]
+        else:
+            project = [req.json()[i]["id"] for i in range(
+                len(req.json())) if req.json()[i]["name"] == self.project_name][0]
         req = requests.get(self.url+'/v1/projects/' +
                            str(project)+"/forms", headers=self.headers)
         forms = [req.json()[i]["name"] for i in range(len(req.json()))]
         return forms
 
     def get_form(self):
 
         req = requests.get(self.url+'/v1/projects/' +
                            str(self.get_project())+"/forms", headers=self.headers)
         form = [req.json()[i]["xmlFormId"] for i in range(len(req.json())) if req.json()[i]["name"] == self.form_name][0]
 
         return form
 
-    def save_form(self, xlsx,path=""):
+    def save_form(self, xlsx="form",path=""):
         
         req = requests.get(self.url+'/v1/projects/'+str(self.get_project())+"/forms/"+self.get_form()+".xlsx", headers=self.headers).content
         
         version = str(pd.read_excel(BytesIO(req),
                     sheet_name="settings")["version"].iloc[0])
 
         file = open(path+xlsx+"_v"+version+".xlsx", "wb")
@@ -398,21 +407,21 @@
                 for i in survey["name"].loc[survey["type"] == "time"]:
                     if i in repeats[j].columns:
                         repeats[j][i] = pd.to_datetime(
                             repeats[j][i], format="%H:%M:%S.%f%z").dt.time
 
         return repeats
 
-    def process_all(self,form_name,variable='',time_variable='starttime'):
+    def process_all(self,variable='',time_variable='starttime'):
 
         submissions = self.processing_submission()
         survey = self.survey().dropna(how='all')
         choices = self.choices()
         repeats = self.processing_repeats()
-        survey_name = form_name
+        survey_name = self.form_name
         variable = variable
         time_variable = time_variable
 
         return Form(submissions,survey,choices,repeats,survey_name,variable,time_variable)
 
     def save_main(self,data=None,path=""):
 
@@ -538,8 +547,7 @@
             self.put_submission(id, self.update_xml(ff))
         else:
             self.set_target(project, form)
             c = self.get_submission_xml(id)
             for i in range(len(variable)):
                 c = self.modify_xml(c, variable[i], func[i])
             self.put_submission(id, self.update_xml(c))
-
```

### Comparing `odk_tools-0.1.0/LICENSE` & `odk_tools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `odk_tools-0.1.0/pyproject.toml` & `odk_tools-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "odk_tools"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Federico Lorenzetti", email="lorenzetti.federico@gmail.com" },
 ]
 description = "A collection of tools for interacting with an ODK server and uploading/downloading submissions"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `odk_tools-0.1.0/PKG-INFO` & `odk_tools-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: odk_tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of tools for interacting with an ODK server and uploading/downloading submissions
 Project-URL: Homepage, https://github.com/federlorenz/odk_tools
 Author-email: Federico Lorenzetti <lorenzetti.federico@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # odk-tools
 A collection of tools for interacting with an ODK server and uploading/downloading submissions.
 
 ## Installation
```

