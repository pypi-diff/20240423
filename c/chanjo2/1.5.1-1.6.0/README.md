# Comparing `tmp/chanjo2-1.5.1.tar.gz` & `tmp/chanjo2-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chanjo2-1.5.1.tar", max compression
+gzip compressed data, was "chanjo2-1.6.0.tar", max compression
```

## Comparing `chanjo2-1.5.1.tar` & `chanjo2-1.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      759 2024-03-27 07:45:55.576772 chanjo2-1.5.1/pyproject.toml
--rw-r--r--   0        0        0       68 2024-03-27 07:45:55.576772 chanjo2-1.5.1/src/chanjo2/__init__.py
--rw-r--r--   0        0        0     3102 2024-03-27 07:45:55.576772 chanjo2-1.5.1/src/chanjo2/constants.py
--rw-r--r--   0        0        0     2640 2024-03-27 07:45:55.576772 chanjo2-1.5.1/src/chanjo2/crud/cases.py
--rw-r--r--   0        0        0     7002 2024-03-27 07:45:55.576772 chanjo2-1.5.1/src/chanjo2/crud/intervals.py
--rw-r--r--   0        0        0     3886 2024-03-27 07:45:55.576772 chanjo2-1.5.1/src/chanjo2/crud/samples.py
--rw-r--r--   0        0        0     1117 2024-03-27 07:45:55.576772 chanjo2-1.5.1/src/chanjo2/dbutil.py
--rw-r--r--   0        0        0      346 2024-03-27 07:45:55.576772 chanjo2-1.5.1/src/chanjo2/demo/109_green.bed
--rw-r--r--   0        0        0     1378 2024-03-27 07:45:55.576772 chanjo2-1.5.1/src/chanjo2/demo/__init__.py
--rw-r--r--   0        0        0   450444 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/demo/panelapp_109_example.d4
--rw-r--r--   0        0        0        0 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/endpoints/__init__.py
--rw-r--r--   0        0        0     1594 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/endpoints/cases.py
--rw-r--r--   0        0        0     8272 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/endpoints/coverage.py
--rw-r--r--   0        0        0     6109 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/endpoints/intervals.py
--rw-r--r--   0        0        0     3246 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/endpoints/overview.py
--rw-r--r--   0        0        0     2754 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/endpoints/report.py
--rw-r--r--   0        0        0     2024 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/endpoints/samples.py
--rw-r--r--   0        0        0     2150 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/main.py
--rw-r--r--   0        0        0        0 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/meta/__init__.py
--rw-r--r--   0        0        0     1249 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/meta/handle_bed.py
--rw-r--r--   0        0        0     2433 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/meta/handle_completeness_tasks.py
--rw-r--r--   0        0        0    12286 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/meta/handle_d4.py
--rw-r--r--   0        0        0     7608 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/meta/handle_load_intervals.py
--rw-r--r--   0        0        0     8760 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/meta/handle_report_contents.py
--rw-r--r--   0        0        0      335 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/models/__init__.py
--rw-r--r--   0        0        0     7695 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/models/pydantic_models.py
--rw-r--r--   0        0        0     4512 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/models/sql_models.py
--rw-r--r--   0        0        0     2552 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/populate_demo.py
--rw-r--r--   0        0        0      344 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/static/main.css
--rw-r--r--   0        0        0     1778 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/templates/base-layout.html
--rw-r--r--   0        0        0     1253 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/templates/gene-overview.html
--rw-r--r--   0        0        0     3901 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/templates/overview.html
--rw-r--r--   0        0        0     9969 2024-03-27 07:45:55.580772 chanjo2-1.5.1/src/chanjo2/templates/report.html
--rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 chanjo2-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      759 2024-04-23 10:55:14.717780 chanjo2-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2024-04-23 10:55:14.717780 chanjo2-1.6.0/src/chanjo2/__init__.py
+-rw-r--r--   0        0        0     3102 2024-04-23 10:55:14.717780 chanjo2-1.6.0/src/chanjo2/constants.py
+-rw-r--r--   0        0        0     2640 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/crud/cases.py
+-rw-r--r--   0        0        0     7002 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/crud/intervals.py
+-rw-r--r--   0        0        0     3886 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/crud/samples.py
+-rw-r--r--   0        0        0     1117 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/dbutil.py
+-rw-r--r--   0        0        0      346 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/demo/109_green.bed
+-rw-r--r--   0        0        0     2101 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/demo/__init__.py
+-rw-r--r--   0        0        0   450444 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/demo/panelapp_109_example.d4
+-rw-r--r--   0        0        0        0 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/endpoints/__init__.py
+-rw-r--r--   0        0        0     1594 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/endpoints/cases.py
+-rw-r--r--   0        0        0     8272 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/endpoints/coverage.py
+-rw-r--r--   0        0        0     6109 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/endpoints/intervals.py
+-rw-r--r--   0        0        0     3808 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/endpoints/overview.py
+-rw-r--r--   0        0        0     3247 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/endpoints/report.py
+-rw-r--r--   0        0        0     2024 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/endpoints/samples.py
+-rw-r--r--   0        0        0     2150 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/main.py
+-rw-r--r--   0        0        0        0 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/meta/__init__.py
+-rw-r--r--   0        0        0     1249 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/meta/handle_bed.py
+-rw-r--r--   0        0        0     2433 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/meta/handle_completeness_tasks.py
+-rw-r--r--   0        0        0    12286 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/meta/handle_d4.py
+-rw-r--r--   0        0        0     7608 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/meta/handle_load_intervals.py
+-rw-r--r--   0        0        0     8877 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/meta/handle_report_contents.py
+-rw-r--r--   0        0        0      335 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/models/__init__.py
+-rw-r--r--   0        0        0    10600 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/models/pydantic_models.py
+-rw-r--r--   0        0        0     4512 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/models/sql_models.py
+-rw-r--r--   0        0        0     2552 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/populate_demo.py
+-rw-r--r--   0        0        0      344 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/static/main.css
+-rw-r--r--   0        0        0     1778 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/templates/base-layout.html
+-rw-r--r--   0        0        0     1253 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/templates/gene-overview.html
+-rw-r--r--   0        0        0     3415 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/templates/overview.html
+-rw-r--r--   0        0        0     8274 2024-04-23 10:55:14.721781 chanjo2-1.6.0/src/chanjo2/templates/report.html
+-rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 chanjo2-1.6.0/PKG-INFO
```

### Comparing `chanjo2-1.5.1/pyproject.toml` & `chanjo2-1.6.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chanjo2"
-version = "1.5.1"
+version = "1.6.0"
 description = "Next generation coverage analysis"
 authors = ["northwestwitch <chiara.rasi@scilifelab.se>"]
 
 [tool.poetry_bumpversion.file."src/chanjo2/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `chanjo2-1.5.1/src/chanjo2/constants.py` & `chanjo2-1.6.0/src/chanjo2/constants.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/crud/cases.py` & `chanjo2-1.6.0/src/chanjo2/crud/cases.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/crud/intervals.py` & `chanjo2-1.6.0/src/chanjo2/crud/intervals.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/crud/samples.py` & `chanjo2-1.6.0/src/chanjo2/crud/samples.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/dbutil.py` & `chanjo2-1.6.0/src/chanjo2/dbutil.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/demo/__init__.py` & `chanjo2-1.6.0/src/chanjo2/demo/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict
 
 from importlib_resources import files
 
-from chanjo2.constants import BUILD_37
+from chanjo2.constants import BUILD_37, DEFAULT_COMPLETENESS_LEVELS
 
 BASE_PATH: str = "chanjo2.demo"
 
 GENE_PANEL_FILE: str = "109_green.bed"
 D4_DEMO_FILE: str = "panelapp_109_example.d4"
 
 # Paths
@@ -21,27 +21,44 @@
     "track_name": "ADM1059A2",
     "case_name": DEMO_CASE["name"],
     "coverage_file_path": d4_demo_path,
 }
 
 HTTP_SERVER_D4_file = "https://d4-format-testing.s3.us-west-1.amazonaws.com/hg002.d4"
 DEMO_HGNC_GENE_SYMBOLS = ["MTHFR", "DHFR", "FOLR1", "SLC46A1", "LAMA1", "PIPPI6"]
+ANALYSIS_DATE = "2023-04-23T10:20:30.400+02:30"
 
-# Data for generating a demo coverage report
+# JSON Data for generating a demo coverage report
 DEMO_COVERAGE_QUERY_DATA = {
     "build": BUILD_37,
     "samples": [
         {
             "name": DEMO_SAMPLE["name"],
             "case_name": DEMO_CASE["name"],
             "coverage_file_path": d4_demo_path,
-            "analysis_date": "2023-04-23T10:20:30.400+02:30",
+            "analysis_date": ANALYSIS_DATE,
         }
     ],
     "case_display_name": "643594",
     "gene_panel": "A test Panel 1.0",
     "interval_type": "transcripts",
     "ensembl_gene_ids": [],
     "hgnc_gene_ids": [],
     "hgnc_gene_symbols": DEMO_HGNC_GENE_SYMBOLS,
     "default_level": 20,
 }
+
+# HTTP FORM-like data for generating a demo coverage report
+DEMO_COVERAGE_QUERY_FORM = {
+    "build": BUILD_37,
+    "samples": f"[{{'name': '{DEMO_SAMPLE['name']}', 'coverage_file_path': '{d4_demo_path}', 'case_name': '{DEMO_CASE['name']}', 'analysis_date': '{ANALYSIS_DATE}'}}]",
+    "case_display_name": DEMO_CASE["name"],
+    "gene_panel": "A test Panel 1.0",
+    "interval_type": "transcripts",
+    "ensembl_gene_ids": [],
+    "hgnc_gene_ids": [],
+    "hgnc_gene_symbols": ",".join(DEMO_HGNC_GENE_SYMBOLS),
+    "default_level": "20",
+    "completeness_thresholds": ",".join(
+        [str(threshold) for threshold in DEFAULT_COMPLETENESS_LEVELS]
+    ),
+}
```

### Comparing `chanjo2-1.5.1/src/chanjo2/demo/panelapp_109_example.d4` & `chanjo2-1.6.0/src/chanjo2/demo/panelapp_109_example.d4`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/endpoints/cases.py` & `chanjo2-1.6.0/src/chanjo2/endpoints/cases.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/endpoints/coverage.py` & `chanjo2-1.6.0/src/chanjo2/endpoints/coverage.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/endpoints/intervals.py` & `chanjo2-1.6.0/src/chanjo2/endpoints/intervals.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/endpoints/overview.py` & `chanjo2-1.6.0/src/chanjo2/endpoints/overview.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from os import path
 
-from fastapi import APIRouter, Depends, Request
+from fastapi import APIRouter, Depends, HTTPException, Request, status
 from fastapi.encoders import jsonable_encoder
 from fastapi.responses import HTMLResponse
 from fastapi.templating import Jinja2Templates
+from pydantic_core._pydantic_core import ValidationError
 from sqlalchemy.orm import Session
 from starlette.datastructures import FormData
 
 from chanjo2.dbutil import get_session
 from chanjo2.demo import DEMO_COVERAGE_QUERY_DATA
 from chanjo2.meta.handle_report_contents import (
     get_gene_overview_coverage_stats,
@@ -30,33 +31,50 @@
 
 
 @router.get("/overview/demo", response_class=HTMLResponse)
 async def demo_overview(request: Request, db: Session = Depends(get_session)):
     """Return a demo genes overview page over a list of genes for a list of samples."""
 
     overview_query = ReportQuery(**DEMO_COVERAGE_QUERY_DATA)
-    overview_content: dict = get_report_data(query=overview_query, session=db)
+    overview_content: dict = get_report_data(
+        query=overview_query, session=db, is_overview=True
+    )
     return templates.TemplateResponse(
         "overview.html",
         {
             "request": request,
             "extras": overview_content["extras"],
             "levels": overview_content["levels"],
             "incomplete_coverage_rows": overview_content["incomplete_coverage_rows"],
         },
     )
 
 
 @router.post("/overview", response_class=HTMLResponse)
 async def overview(
-    request: Request, report_query: ReportQuery, db: Session = Depends(get_session)
+    request: Request,
+    db: Session = Depends(get_session),
 ):
     """Return the genes overview page over a list of genes for a list of samples."""
+    request_headers: str = request.headers.get("Content-Type")
+    try:
+        if request_headers == "application/json":
+            overview_query = ReportQuery(**await request.json())
+        else:
+            overview_query = ReportQuery.as_form(await request.form())
+
+    except ValidationError as ve:
+        raise HTTPException(
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=ve.json(),
+        )
 
-    overview_content: dict = get_report_data(query=report_query, session=db)
+    overview_content: dict = get_report_data(
+        query=overview_query, session=db, is_overview=True
+    )
     return templates.TemplateResponse(
         "overview.html",
         {
             "request": request,
             "extras": overview_content["extras"],
             "levels": overview_content["levels"],
             "incomplete_coverage_rows": overview_content["incomplete_coverage_rows"],
```

### Comparing `chanjo2-1.5.1/src/chanjo2/endpoints/report.py` & `chanjo2-1.6.0/src/chanjo2/endpoints/report.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 import time
 from os import path
 from typing import Dict
 
-from fastapi import APIRouter, Depends, Request
+from fastapi import APIRouter, Depends, HTTPException, Request, status
 from fastapi.responses import HTMLResponse
 from fastapi.templating import Jinja2Templates
+from pydantic_core._pydantic_core import ValidationError
 from sqlalchemy.orm import Session
 
 from chanjo2.dbutil import get_session
 from chanjo2.demo import DEMO_COVERAGE_QUERY_DATA
 from chanjo2.meta.handle_report_contents import get_report_data
 from chanjo2.models.pydantic_models import ReportQuery
 
@@ -46,19 +47,33 @@
             "errors": report_content["errors"],
         },
     )
 
 
 @router.post("/report", response_class=HTMLResponse)
 async def report(
-    request: Request, report_query: ReportQuery, db: Session = Depends(get_session)
+    request: Request,
+    db: Session = Depends(get_session),
 ):
     """Return a coverage report over a list of genes for a list of samples."""
 
     start_time = time.time()
+    request_headers: str = request.headers.get("Content-Type")
+
+    try:
+        if request_headers == "application/json":
+            report_query = ReportQuery(**await request.json())
+        else:
+            report_query = ReportQuery.as_form(await request.form())
+    except ValidationError as ve:
+        raise HTTPException(
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=ve.json(),
+        )
+
     report_content: dict = get_report_data(query=report_query, session=db)
     LOG.debug(f"Time to compute stats: {time.time() - start_time} seconds.")
     return templates.TemplateResponse(
         "report.html",
         {
             "request": request,
             "levels": report_content["levels"],
```

### Comparing `chanjo2-1.5.1/src/chanjo2/endpoints/samples.py` & `chanjo2-1.6.0/src/chanjo2/endpoints/samples.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/main.py` & `chanjo2-1.6.0/src/chanjo2/main.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/meta/handle_bed.py` & `chanjo2-1.6.0/src/chanjo2/meta/handle_bed.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/meta/handle_completeness_tasks.py` & `chanjo2-1.6.0/src/chanjo2/meta/handle_completeness_tasks.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/meta/handle_d4.py` & `chanjo2-1.6.0/src/chanjo2/meta/handle_d4.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/meta/handle_load_intervals.py` & `chanjo2-1.6.0/src/chanjo2/meta/handle_load_intervals.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/meta/handle_report_contents.py` & `chanjo2-1.6.0/src/chanjo2/meta/handle_report_contents.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,17 @@
         "name": sample.name,
         "case_name": sample.case_name,
         "coverage_file_path": sample.coverage_file_path,
         "analysis_date": str(sample.analysis_date),
     }
 
 
-def get_report_data(query: ReportQuery, session: Session) -> Dict:
+def get_report_data(
+    query: ReportQuery, session: Session, is_overview: Optional[bool] = False
+) -> Dict:
     """Return the information that will be displayed in the coverage report or in the genes overview report.."""
 
     set_samples_coverage_files(session=session, samples=query.samples)
 
     genes: List[SQLGene] = get_genes(
         db=session,
         build=query.build,
@@ -129,15 +131,17 @@
     for sample in query.samples:
         get_report_sample_interval_coverage(
             d4_file_path=sample.coverage_file_path,
             sample_name=sample.name,
             gene_ids_mapping=gene_ids_mapping,
             sql_intervals=sql_intervals,
             intervals_coords=intervals_coords,
-            completeness_thresholds=query.completeness_thresholds,
+            completeness_thresholds=(
+                [query.default_level] if is_overview else query.completeness_thresholds
+            ),
             default_threshold=query.default_level,
             report_data=data,
         )
     return data
 
 
 #### Functions used to create coverage report data
```

### Comparing `chanjo2-1.5.1/src/chanjo2/models/pydantic_models.py` & `chanjo2-1.6.0/src/chanjo2/models/pydantic_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 import json
 import logging
+import os
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 import validators
 from pydantic import BaseModel, Field, field_validator, model_validator
 from pydantic_settings import SettingsConfigDict
+from starlette.datastructures import FormData
 
 from chanjo2.constants import (
     AMBIGUOUS_SAMPLES_INPUT,
     DEFAULT_COMPLETENESS_LEVELS,
     GENE_LISTS_NOT_SUPPORTED_MSG,
     WRONG_COVERAGE_FILE_MSG,
 )
 
 LOG = logging.getLogger("uvicorn.access")
 
 
+def default_report_coverage_levels() -> List[int]:
+    """Sets the coverage thresholds to be used for report metrics whenever a request doesn't contain 'completeness_thresholds' values."""
+    if os.getenv("REPORT_COVERAGE_LEVELS"):
+        return json.loads(os.getenv("REPORT_COVERAGE_LEVELS"))
+    return DEFAULT_COMPLETENESS_LEVELS
+
+
 class Builds(str, Enum):
     build_37 = "GRCh37"
     build_38 = "GRCh38"
 
     @staticmethod
     def get_enum_values() -> List[str]:
         """Returns the values of the available genome builds."""
@@ -218,24 +227,81 @@
     coverage_file_path: Optional[str] = None
     case_name: Optional[str] = None
     analysis_date: Optional[datetime] = datetime.now()
 
 
 class ReportQuery(BaseModel):
     build: Builds
-    completeness_thresholds: Optional[List[int]] = DEFAULT_COMPLETENESS_LEVELS
+    completeness_thresholds: Optional[List[int]] = default_report_coverage_levels()
     ensembl_gene_ids: Optional[List[str]] = None
     hgnc_gene_ids: Optional[List[int]] = None
     hgnc_gene_symbols: Optional[List[str]] = None
     interval_type: IntervalType
     default_level: int = 10
     panel_name: Optional[str] = "Custom panel"
     case_display_name: Optional[str] = None
     samples: List[ReportQuerySample]
 
+    @staticmethod
+    def comma_sep_values_to_list(
+        comma_sep_values: Optional[str], items_format: Union[str, int]
+    ) -> Optional[List[Union[str, int]]]:
+        """Helper function that formats list of strings or integers passed by a form as comma separated values."""
+        if comma_sep_values is None:
+            return
+        if items_format == str:
+            return [item.strip() for item in comma_sep_values.split(",")]
+        else:
+            return [int(item.strip()) for item in comma_sep_values.split(",")]
+
+    @staticmethod
+    def set_query_genes(form_data: FormData):
+        """Helper function that collects form data from report page requests and sets the right gene IDs/values in the query."""
+        query_genes = {
+            "ensembl_gene_ids": [],
+            "hgnc_gene_ids": [],
+            "hgnc_gene_symbols": [],
+        }
+
+        for gene_ids_key in query_genes.keys():
+            if bool(form_data.get(gene_ids_key)) is False:
+                continue
+            id_values: List[Union[str, int]] = [
+                item.strip() for item in form_data.get(gene_ids_key).split(",")
+            ]
+            for value in id_values:
+                if value.isdigit():
+                    query_genes["hgnc_gene_ids"].append(value)
+                elif value.startswith("ENSG"):
+                    query_genes["ensembl_gene_ids"].append(value)
+                else:
+                    query_genes["hgnc_gene_symbols"].append(value)
+        return query_genes
+
+    @classmethod
+    def as_form(cls, form_data: FormData) -> "ReportQuery":
+        query_genes: dict = cls.set_query_genes(form_data)
+        report_query: dict = {
+            "build": form_data.get("build"),
+            "completeness_thresholds": cls.comma_sep_values_to_list(
+                comma_sep_values=form_data.get("completeness_thresholds"),
+                items_format=int,
+            )
+            or default_report_coverage_levels(),
+            "ensembl_gene_ids": query_genes["ensembl_gene_ids"],
+            "hgnc_gene_ids": query_genes["hgnc_gene_ids"],
+            "hgnc_gene_symbols": query_genes["hgnc_gene_symbols"],
+            "interval_type": form_data.get("interval_type"),
+            "default_level": form_data.get("default_level"),
+            "panel_name": form_data.get("panel_name"),
+            "case_display_name": form_data.get("case_display_name"),
+            "samples": form_data.get("samples"),
+        }
+        return cls(**report_query)
+
     @field_validator("samples", mode="before")
     def samples_validator(cls, sample_list):
         if isinstance(sample_list, str):
             return json.loads(sample_list.replace("'", '"'))
         return sample_list
 
     @model_validator(mode="before")
@@ -251,15 +317,15 @@
         if nr_provided_gene_lists != 1:
             raise ValueError(GENE_LISTS_NOT_SUPPORTED_MSG)
         return values
 
 
 class GeneReportForm(BaseModel):
     build: Builds
-    completeness_thresholds: Optional[List[int]] = DEFAULT_COMPLETENESS_LEVELS
+    completeness_thresholds: Optional[List[int]] = default_report_coverage_levels()
     hgnc_gene_id: int
     default_level: int = 10
     samples: List[ReportQuerySample]
     interval_type: IntervalType
 
     @field_validator("samples", mode="before")
     def samples_validator(cls, sample_list):
```

### Comparing `chanjo2-1.5.1/src/chanjo2/models/sql_models.py` & `chanjo2-1.6.0/src/chanjo2/models/sql_models.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/populate_demo.py` & `chanjo2-1.6.0/src/chanjo2/populate_demo.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/templates/base-layout.html` & `chanjo2-1.6.0/src/chanjo2/templates/base-layout.html`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/templates/gene-overview.html` & `chanjo2-1.6.0/src/chanjo2/templates/gene-overview.html`

 * *Files identical despite different names*

### Comparing `chanjo2-1.5.1/src/chanjo2/templates/overview.html` & `chanjo2-1.6.0/src/chanjo2/templates/overview.html`

 * *Files 25% similar despite different names*

```diff
@@ -7,30 +7,33 @@
 {% macro completeness_cutoffs() %}
 <!-- Grey with black text -->
 <nav class="navbar navbar-expand-lg navbar-light bg-light">
   <div class="container-fluid">
     <ul class="navbar-nav">
 		{% for level_id, _ in levels.items() %}
 			<li class="nav-item">
-				<a class="nav-link {% if level_id == extras.default_level %}active{% endif %}" href="#" onclick="updateOverview({{level_id}});">Completeness {{ level_id }}x</a>
+				<a class="nav-link {% if level_id == extras.default_level %}active{% endif %}" href="#" onclick="return updateOverview({{level_id}});">Completeness {{ level_id }}x</a>
 			</li>
 		{% endfor%}
     </ul>
   </div>
 </nav>
 {% endmacro %}
 
 
 {% macro incompletely_covered_intervals(active_level) %}
  <form id="geneStatsForm" action="{{url_for('gene_overview')}}" method="post">
 	 <input type="hidden" name="build" value="{{extras.build}}"/>
-	 <input type="hidden" name="default_level" value="{{extras.default_level}}"/>
+	 <input type="hidden" name="default_level" id="defaultLevel" value="{{extras.default_level}}"/>
 	 <input type="hidden" name="completeness_thresholds" value="{{extras.completeness_thresholds|join(',')}}"/>
 	 <input type="hidden" name="samples" value="{{extras.samples|safe}}"/>
 	 <input type="hidden" name="interval_type" value="{{extras.interval_type}}"/>
+	 {% if extras.hgnc_gene_ids %} <!-- genes should be loaded in database -->
+	 	<input type="hidden" name="hgnc_gene_ids" value="{{extras.hgnc_gene_ids|join(',')}}"/>
+	 {% endif %}
 </form>
 	<div class="row">
 		<div class="col-md-12">
 			<table class="table table-bordered">
 			<caption>Incompletely covered {{ extras.interval_type }}</caption>
 				<thead>
 					<tr>
@@ -96,53 +99,26 @@
 
 {% endblock %}
 
 
 {% block js_code %}
 	{{ super() }}
 	<script>
-
-		// Extracts the content of the body element of an HTML page as a string
-		function updatedReportBody(html)
-		{
-			return /<body.*?>([\s\S]*)<\/body>/.exec(html)[1];
-		}
+		let theForm = document.getElementById("geneStatsForm");
 
 		function updateOverview(customLevel)
 		{
-			let formDict = {
-				'build' : '{{ extras.build }}',
-				'completeness_thresholds' : {{ extras.completeness_thresholds }},
-				'hgnc_gene_ids' : {{ extras.hgnc_gene_ids }},
-				'interval_type' : '{{ extras.interval_type }}',
-				'default_level' : customLevel,
-				'samples' : {{ extras.samples|safe }},
-			}
-
-			fetch('/overview', {
-					method: 'POST',
-					headers: {
-						'Content-Type': 'application/json'
-					},
-					body: JSON.stringify(formDict)
-				})
-				.then(resp => resp.text())
-				.then(html => {
-					document.body.innerHTML = updatedReportBody(html);
-				})
-				.catch(error => {
-					console.error(error);
-			});
+			document.getElementById("defaultLevel").value = customLevel;
+			theForm.action = '/overview';
+			theForm.submit();
 		}
 
-
 		function getGeneStatsPage(hgncId)
 		{
 			event.preventDefault();
-			var theForm = document.getElementById("geneStatsForm");
 			var geneInput = document.createElement("input");
 			geneInput.setAttribute("type", "hidden");
 			geneInput.setAttribute("name", "hgnc_gene_id");
 			geneInput.setAttribute("value", hgncId);
 			theForm.appendChild(geneInput);
 			theForm.submit();
 		}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends "base-layout.html" %} {% block css %} {{ super() }} {% endblock %}
 {% macro completeness_cutoffs() %}
     * {% for level_id, _ in levels.items() %}
     * _C_o_m_p_l_e_t_e_n_e_s_s_ _{_{_ _l_e_v_e_l___i_d_ _}_}_x
     * {% endfor%}
 {% endmacro %} {% macro incompletely_covered_intervals(active_level) %}
+{% if extras.hgnc_gene_ids %} {% endif %}
                IInnccoommpplleetteellyy ccoovveerreedd {{{{ eexxttrraass..iinntteerrvvaall__ttyyppee }}}}
                                                    CCoommpplleetteenneessss {{
 GGeennee       {{{{ eexxttrraass..iinntteerrvvaall__ttyyppee }}}} SSaammppllee       {{ eexxttrraass..ddeeffaauulltt__lleevveell }}}}xx
                                                    [[%%]]
 _{_{_r_o_w_[_0_]_}_} {{ row[2] }}               {{ row[3] }} {{ row[4] }}
 No intervals found..
 {{samples_coverage_stats}} {% endmacro %} {% block title %}
```

### Comparing `chanjo2-1.5.1/src/chanjo2/templates/report.html` & `chanjo2-1.6.0/src/chanjo2/templates/report.html`

 * *Files 15% similar despite different names*

```diff
@@ -19,50 +19,47 @@
       <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#flush-collapseOne" aria-expanded="false" aria-controls="flush-collapseOne">
        Customize
       </button>
     </h2>
     <div id="flush-collapseOne" class="accordion-collapse collapse" aria-labelledby="flush-headingOne" data-bs-parent="#accordionFlushExample">
 		<div class="accordion-body">
 			<!-- hidden fields passed from previous query -->
+			<form name="customizeForm" action="{{url_for('report')}}" method="post">
 			<input type="hidden" id="build" name="build" value="{{extras.build}}">
 			<input type="hidden" id="interval_type" name="interval_type" value="{{extras.interval_type}}">
+			<input type="hidden" name="samples" value="{{extras.samples|safe}}"/>
 			  <div>
 				<div class="form-group">
 				  <div class="row" {% if hidden %}hidden{% endif %}>
 					<div class="col-6">
 					  <label class="form-label">Completeness cutoff</label>
 					  <select class="form-control" name="default_level" id="default_level">
 						{% for level, _ in levels.items() %}
-						  <option value="{{ level }}" {% if level == extras.level %} selected {% endif %}>{{ level }}x</option>
+						  <option value="{{ level }}" {% if level == extras.default_level %} selected {% endif %}>{{ level }}x</option>
 						{% endfor %}
 					  </select>
 					</div>
 
 				<div class="col-6">
 				  <label class="form-label">Gene panel name to display</label>
 				  <input class="form-control" id="panel_name" type="text" placeholder="Skeletal dysplasia 3.2" value="{{ extras.panel_name or '' }}">
 				</div>
 			  </div>
 			</div>
 
 			<div class="row">
 				<div class="col-7">
-				  <label class="form-label">Included genes (Comma separated list of Ensembl IDs, HGNC IDs or HGNC symbols)</label>
-				  <div><input class="form-control" type="text" name="gene_ids" id ="gene_ids" value="{{ extras.hgnc_gene_ids|join(', ') }}" placeholder="ADK,GIT"></div>
+				  <label class="form-label">Included genes (Comma separated list HGNC IDs, HGNC symbols or Ensembl IDs)</label>
+				  <div><input class="form-control" type="text" name="hgnc_gene_ids" value="{{ extras.hgnc_gene_ids|join(', ') }}" placeholder="17284, 21022,.."></div>
 				</div>
 				<div class="col-4 offset-1 mt-2">
-				  <button class="btn btn-primary mt-4" type="button" onclick="submitAsJson();">Update</button>
+				  <button class="btn btn-primary mt-4" type="submit">Update</button>
 				</div>
 			</div>
-
-			{% for sample_id in sample_ids %}
-			  <input type="text" name="sample_id" value="{{ sample_id }}" hidden>
-			{% endfor %}
-
-			</div>
+			</form>
 		</div>
 	</div>
   </div>
 </div>
 {% endmacro %}
 
 {% macro sex_rows_block() %}
@@ -259,66 +256,10 @@
 					e.style.display = 'none';
 				}
 				else {
 					e.style.display = 'block';
 				}
 			}
 		}
-
-		// Extracts the content of the body element of an HTML page as a string
-		function updatedReportBody(html)
-		{
-			return /<body.*?>([\s\S]*)<\/body>/.exec(html)[1];
-		}
-
-		// Returns the list of HGNC genes present in the user query as a sring as a list of integers
-		function getFormGeneIDsAsList()
-		{
-			let geneIdsTypes = [null, null, null]; // [Ensembl_ids_list, HGNC_ids_list, HGNC_symbols_list];
-			let formGeneIds = document.getElementById('gene_ids').value.replace(/\s/g, '').split(",");
-			if (!isNaN(formGeneIds[0])) {
-				geneIdsTypes[1] = formGeneIds.map(Number);
-			}
-			else if (formGeneIds[0].startsWith('ENSG')){
-				geneIdsTypes[0] = formGeneIds;
-			}
-			else{
-				geneIdsTypes[2] = formGeneIds;
-			}
-			return geneIdsTypes;
-		}
-
-		function submitAsJson()
-		{
-			event.preventDefault();
-			let geneIds = getFormGeneIDsAsList();
-			let formDict = {
-				'build' : '{{ extras.build }}',
-				'completeness_thresholds' : {{ extras.completeness_thresholds }},
-				'ensembl_gene_ids': geneIds[0],
-				'hgnc_gene_ids' : geneIds[1],
-				'hgnc_gene_symbols' : geneIds[2],
-				'interval_type' : '{{ extras.interval_type }}',
-				'panel_name' : document.getElementById("panel_name").value,
-				'default_level' : document.getElementById("default_level").value,
-				'case_display_name' : '{{ extras.case_name }}',
-				'samples' : {{ extras.samples|safe }},
-			}
-
-			fetch('/report', {
-					method: 'POST',
-					headers: {
-						'Content-Type': 'application/json'
-					},
-					body: JSON.stringify(formDict)
-				})
-				.then(resp => resp.text())
-				.then(html => {
-					document.body.innerHTML = updatedReportBody(html);
-				})
-				.catch(error => {
-					console.error(error);
-			});
-		}
 	</script>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -2,21 +2,20 @@
 {% macro errors_block() %} {% for error_description, error_content in errors %}
 {% if error_content %}
 {{error_description}}: {{error_content|join(", ")}}
 {% endif %} {% endfor %} {% endmacro %} {% macro report_filters() %}
 ********** CCuussttoommiizzee **********
 % if hidden %}hidden{% endif %}>
 {% for level, _ in levels.items() %}
-% if level == extras.level %} selected {% endif %}>{{ level }}x
+% if level == extras.default_level %} selected {% endif %}>{{ level }}x
 {% endfor %}
 Gene panel name to display[{{ extras.panel_name or '' }}]
-Included genes (Comma separated list of Ensembl IDs, HGNC IDs or HGNC symbols)
+Included genes (Comma separated list HGNC IDs, HGNC symbols or Ensembl IDs)
 [{{ extras.hgnc_gene_ids|join(', ') }}]
 Update
-{% for sample_id in sample_ids %} [{{ sample_id }}     ]{% endfor %}
 {% endmacro %} {% macro sex_rows_block() %}
                                        SSeexx mmeettrriiccss ffrroomm sseeqquueenncciinngg ddaattaa
 SSaammppllee        GGrroouupp       AAnnaallyyzzeedd aatt               SSeexx aaccccoorrddiinngg ttoo        AAvveerraaggee ccoovveerraaggee [[xx]]
                                                     sseeqquueennccee ddaattaa           CChhrroommoossoommee XX      CChhrroommoossoommee YY
 {             {           {                                                 {                 {
 {             {           {                         {                       {                 {
 sample.sample sample.case sample.analysis_date.date {sample.predicted_sex}} sample.x_coverage sample.y_coverage
```

### Comparing `chanjo2-1.5.1/PKG-INFO` & `chanjo2-1.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chanjo2
-Version: 1.5.1
+Version: 1.6.0
 Summary: Next generation coverage analysis
 Author: northwestwitch
 Author-email: chiara.rasi@scilifelab.se
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

