# Comparing `tmp/miksiai-1.0.1-cp310-cp310-win_amd64.whl.zip` & `tmp/miksiai-1.0.2-cp310-cp310-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 1827195 bytes, number of entries: 16
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-22 05:43 miksiai/__init__.py
--rwxrwxr-x  2.0 unx   495680 b- defN 24-Apr-22 07:56 miksiai/agent.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx   446624 b- defN 24-Apr-22 07:56 miksiai/api.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx   220264 b- defN 24-Apr-22 07:56 miksiai/master.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx   319504 b- defN 24-Apr-22 07:56 miksiai/pythontool.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx   112888 b- defN 24-Apr-22 07:56 miksiai/settings.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx   751704 b- defN 24-Apr-22 07:56 miksiai/sqltool.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx   208264 b- defN 24-Apr-22 07:56 miksiai/utils.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx   440800 b- defN 24-Apr-22 07:56 miksiai/sql_graph/custom_sql.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx   407832 b- defN 24-Apr-22 07:56 miksiai/sql_graph/sql_graph.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx    79280 b- defN 24-Apr-22 07:56 miksiai/sql_graph/sql_graph_prompts.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx   955728 b- defN 24-Apr-22 07:56 miksiai/sql_graph/sql_runnables.cpython-310-x86_64-linux-gnu.so
--rw-rw-r--  2.0 unx     7595 b- defN 24-Apr-22 07:57 miksiai-1.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx      102 b- defN 24-Apr-22 07:57 miksiai-1.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 24-Apr-22 07:57 miksiai-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1592 b- defN 24-Apr-22 07:57 miksiai-1.0.1.dist-info/RECORD
-16 files, 4447865 bytes uncompressed, 1824517 bytes compressed:  59.0%
+Zip file size: 381140 bytes, number of entries: 16
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 15:56 miksiai/__init__.py
+-rwxr-xr-x  2.0 unx   136184 b- defN 24-Apr-23 12:34 miksiai/agent.cpython-310-darwin.so
+-rwxr-xr-x  2.0 unx   117142 b- defN 24-Apr-23 12:34 miksiai/api.cpython-310-darwin.so
+-rwxr-xr-x  2.0 unx    77353 b- defN 24-Apr-23 12:34 miksiai/master.cpython-310-darwin.so
+-rwxr-xr-x  2.0 unx   100653 b- defN 24-Apr-23 12:34 miksiai/pythontool.cpython-310-darwin.so
+-rwxr-xr-x  2.0 unx    75227 b- defN 24-Apr-23 12:34 miksiai/settings.cpython-310-darwin.so
+-rwxr-xr-x  2.0 unx   172602 b- defN 24-Apr-23 12:34 miksiai/sqltool.cpython-310-darwin.so
+-rwxr-xr-x  2.0 unx    78168 b- defN 24-Apr-23 12:34 miksiai/utils.cpython-310-darwin.so
+-rwxr-xr-x  2.0 unx   118093 b- defN 24-Apr-23 12:34 miksiai/sql_graph/custom_sql.cpython-310-darwin.so
+-rwxr-xr-x  2.0 unx   136972 b- defN 24-Apr-23 12:34 miksiai/sql_graph/sql_graph.cpython-310-darwin.so
+-rwxr-xr-x  2.0 unx    72260 b- defN 24-Apr-23 12:34 miksiai/sql_graph/sql_graph_prompts.cpython-310-darwin.so
+-rwxr-xr-x  2.0 unx   239248 b- defN 24-Apr-23 12:34 miksiai/sql_graph/sql_runnables.cpython-310-darwin.so
+-rw-r--r--  2.0 unx     7454 b- defN 24-Apr-23 12:42 miksiai-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-23 12:42 miksiai-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-23 12:42 miksiai-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1479 b- defN 24-Apr-23 12:42 miksiai-1.0.2.dist-info/RECORD
+16 files, 1332953 bytes uncompressed, 378682 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,49 +1,49 @@
 Filename: miksiai/__init__.py
 Comment: 
 
-Filename: miksiai/agent.cpython-310-x86_64-linux-gnu.so
+Filename: miksiai/agent.cpython-310-darwin.so
 Comment: 
 
-Filename: miksiai/api.cpython-310-x86_64-linux-gnu.so
+Filename: miksiai/api.cpython-310-darwin.so
 Comment: 
 
-Filename: miksiai/master.cpython-310-x86_64-linux-gnu.so
+Filename: miksiai/master.cpython-310-darwin.so
 Comment: 
 
-Filename: miksiai/pythontool.cpython-310-x86_64-linux-gnu.so
+Filename: miksiai/pythontool.cpython-310-darwin.so
 Comment: 
 
-Filename: miksiai/settings.cpython-310-x86_64-linux-gnu.so
+Filename: miksiai/settings.cpython-310-darwin.so
 Comment: 
 
-Filename: miksiai/sqltool.cpython-310-x86_64-linux-gnu.so
+Filename: miksiai/sqltool.cpython-310-darwin.so
 Comment: 
 
-Filename: miksiai/utils.cpython-310-x86_64-linux-gnu.so
+Filename: miksiai/utils.cpython-310-darwin.so
 Comment: 
 
-Filename: miksiai/sql_graph/custom_sql.cpython-310-x86_64-linux-gnu.so
+Filename: miksiai/sql_graph/custom_sql.cpython-310-darwin.so
 Comment: 
 
-Filename: miksiai/sql_graph/sql_graph.cpython-310-x86_64-linux-gnu.so
+Filename: miksiai/sql_graph/sql_graph.cpython-310-darwin.so
 Comment: 
 
-Filename: miksiai/sql_graph/sql_graph_prompts.cpython-310-x86_64-linux-gnu.so
+Filename: miksiai/sql_graph/sql_graph_prompts.cpython-310-darwin.so
 Comment: 
 
-Filename: miksiai/sql_graph/sql_runnables.cpython-310-x86_64-linux-gnu.so
+Filename: miksiai/sql_graph/sql_runnables.cpython-310-darwin.so
 Comment: 
 
-Filename: miksiai-1.0.1.dist-info/METADATA
+Filename: miksiai-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: miksiai-1.0.1.dist-info/WHEEL
+Filename: miksiai-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: miksiai-1.0.1.dist-info/top_level.txt
+Filename: miksiai-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: miksiai-1.0.1.dist-info/RECORD
+Filename: miksiai-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `miksiai-1.0.1.dist-info/METADATA` & `miksiai-1.0.2.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,84 @@
 Metadata-Version: 2.1
 Name: miksiai
-Version: 1.0.1
+Version: 1.0.2
 Summary: Miksi-AI empowers your BI
 Home-page: https://github.com/Miksi-io/Custom-Agent
 Author: RichardKaranuMbuti
 Author-email: officialforrichardk@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: Cython (==3.0.9)
-Requires-Dist: PyMySQL (==1.1.0)
-Requires-Dist: PyYAML (==6.0.1)
-Requires-Dist: SQLAlchemy (==2.0.27)
-Requires-Dist: aiohttp (==3.9.3)
-Requires-Dist: aiosignal (==1.3.1)
-Requires-Dist: annotated-types (==0.6.0)
-Requires-Dist: anyio (==4.3.0)
-Requires-Dist: attrs (==23.2.0)
-Requires-Dist: certifi (==2024.2.2)
-Requires-Dist: charset-normalizer (==3.3.2)
-Requires-Dist: dataclasses-json (==0.6.4)
-Requires-Dist: distro (==1.9.0)
-Requires-Dist: frozenlist (==1.4.1)
-Requires-Dist: greenlet (==3.0.3)
-Requires-Dist: h11 (==0.14.0)
-Requires-Dist: httpcore (==1.0.4)
-Requires-Dist: httpx (==0.27.0)
-Requires-Dist: idna (==3.6)
-Requires-Dist: jinja2
-Requires-Dist: jsonpatch (==1.33)
-Requires-Dist: jsonpointer (==2.4)
-Requires-Dist: langchain-community (==0.0.25)
-Requires-Dist: langchain-core (==0.1.38)
-Requires-Dist: langchain-openai (==0.0.8)
-Requires-Dist: langchain-text-splitters (==0.0.1)
-Requires-Dist: langchain (==0.1.10)
-Requires-Dist: langgraph (==0.0.31)
-Requires-Dist: langsmith (==0.1.13)
-Requires-Dist: loguru (==0.7.2)
-Requires-Dist: marshmallow (==3.21.0)
+Requires-Dist: aiohttp ==3.9.3
+Requires-Dist: aiosignal ==1.3.1
+Requires-Dist: annotated-types ==0.6.0
+Requires-Dist: anyio ==4.3.0
+Requires-Dist: attrs ==23.2.0
+Requires-Dist: certifi ==2024.2.2
+Requires-Dist: charset-normalizer ==3.3.2
+Requires-Dist: Cython ==3.0.9
+Requires-Dist: dataclasses-json ==0.6.4
+Requires-Dist: distro ==1.9.0
+Requires-Dist: frozenlist ==1.4.1
+Requires-Dist: greenlet ==3.0.3
+Requires-Dist: h11 ==0.14.0
+Requires-Dist: httpcore ==1.0.4
+Requires-Dist: httpx ==0.27.0
+Requires-Dist: idna ==3.6
+Requires-Dist: jsonpatch ==1.33
+Requires-Dist: jsonpointer ==2.4
+Requires-Dist: langchain ==0.1.10
+Requires-Dist: langchain-community ==0.0.25
+Requires-Dist: langchain-core ==0.1.38
+Requires-Dist: langchain-openai ==0.0.8
+Requires-Dist: langchain-text-splitters ==0.0.1
+Requires-Dist: langsmith ==0.1.13
+Requires-Dist: marshmallow ==3.21.0
+Requires-Dist: multidict ==6.0.5
+Requires-Dist: mypy-extensions ==1.0.0
+Requires-Dist: numpy ==1.26.4
+Requires-Dist: openai ==1.13.3
+Requires-Dist: orjson ==3.9.15
+Requires-Dist: packaging ==23.2
+Requires-Dist: psycopg2-binary ==2.9.9
+Requires-Dist: pydantic ==1.10.13
+Requires-Dist: pydantic-core ==2.16.3
+Requires-Dist: PyMySQL ==1.1.0
+Requires-Dist: pyodbc ==5.1.0
+Requires-Dist: python-dotenv ==1.0.1
+Requires-Dist: PyYAML ==6.0.1
+Requires-Dist: regex ==2023.12.25
+Requires-Dist: requests ==2.31.0
+Requires-Dist: sniffio ==1.3.1
+Requires-Dist: SQLAlchemy ==2.0.27
+Requires-Dist: tenacity ==8.2.3
+Requires-Dist: tiktoken ==0.6.0
+Requires-Dist: tqdm ==4.66.2
+Requires-Dist: typing-inspect ==0.9.0
+Requires-Dist: typing-extensions ==4.10.0
+Requires-Dist: urllib3 ==2.2.1
+Requires-Dist: yarl ==1.9.4
+Requires-Dist: langgraph ==0.0.31
+Requires-Dist: loguru ==0.7.2
 Requires-Dist: matplotlib
-Requires-Dist: multidict (==6.0.5)
-Requires-Dist: mypy-extensions (==1.0.0)
-Requires-Dist: mysql-connector-python (==8.3.0)
+Requires-Dist: scikit-learn
 Requires-Dist: numpy
-Requires-Dist: numpy (==1.26.4)
-Requires-Dist: openai (==1.13.3)
-Requires-Dist: orjson (==3.9.15)
-Requires-Dist: packaging (==23.2)
 Requires-Dist: pandas
-Requires-Dist: psycopg2-binary (==2.9.9)
-Requires-Dist: pydantic (==1.10.13)
-Requires-Dist: pydantic-core (==2.16.3)
-Requires-Dist: pyodbc (==5.1.0)
-Requires-Dist: python-dotenv (==1.0.1)
-Requires-Dist: regex (==2023.12.25)
-Requires-Dist: requests (==2.31.0)
-Requires-Dist: scikit-learn
 Requires-Dist: scipy
-Requires-Dist: sniffio (==1.3.1)
-Requires-Dist: tenacity (==8.2.3)
-Requires-Dist: tiktoken (==0.6.0)
-Requires-Dist: tqdm (==4.66.2)
-Requires-Dist: typing-inspect (==0.9.0)
-Requires-Dist: typing-extensions (==4.10.0)
-Requires-Dist: urllib3 (==2.2.1)
-Requires-Dist: yarl (==1.9.4)
+Requires-Dist: mysql-connector-python ==8.3.0
+Requires-Dist: jinja2
 
 # Intro
 
 Miksi AI agent works with a couple of tools to give you the final value. Mostly, it's an interchange between a tool that executes SQL queries and the one that executes the python code to generate graphs.
 
 While the agent is instructed strictly not to execute code that writes/modifies the data, we advise you to provide a database user with only read permission to the agent.
 
@@ -188,9 +186,7 @@
 
 query = "your query here"
 answer = run_agent(agent, query, media_path)
 ```
 
 
 
-
-
```

## Comparing `miksiai-1.0.1.dist-info/RECORD` & `miksiai-1.0.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 miksiai/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-miksiai/agent.cpython-310-x86_64-linux-gnu.so,sha256=Y_Fzp9zWy2DScFbCbOFm00vy45lwdqV30XY4b8mHhFI,495680
-miksiai/api.cpython-310-x86_64-linux-gnu.so,sha256=k6dKbL3fLmIhT05D8AcTrd0V1WH4ylnLQ0QIUHOYYd0,446624
-miksiai/master.cpython-310-x86_64-linux-gnu.so,sha256=_R9gS0NCH3og4lwzfLrjevWWFm3kxFYM16Um3mDfB4A,220264
-miksiai/pythontool.cpython-310-x86_64-linux-gnu.so,sha256=KOt354NS7YhWKObaZ2EWQrPML9m5TV1Nk6qVcAmxFgg,319504
-miksiai/settings.cpython-310-x86_64-linux-gnu.so,sha256=LiWeTIsifXH_5QmrpgluKAyHvlWKuovNWqVdQpd_Mkc,112888
-miksiai/sqltool.cpython-310-x86_64-linux-gnu.so,sha256=llO9dGRupv4dNmmA8cW05Cwiowpr9LzJmbwlwdfrnrQ,751704
-miksiai/utils.cpython-310-x86_64-linux-gnu.so,sha256=Kt95E28TwirziFUpY_LI5QpKAsTUUoFi02kH2hEYmtg,208264
-miksiai/sql_graph/custom_sql.cpython-310-x86_64-linux-gnu.so,sha256=_GngbtJmXwyVOPXcYWGj5vjcxL0xCC12XzehCgY2JFA,440800
-miksiai/sql_graph/sql_graph.cpython-310-x86_64-linux-gnu.so,sha256=OQ9-URiKo_4Fj6CquYfoSRYE98eC1sY2aOCAcFsFwM8,407832
-miksiai/sql_graph/sql_graph_prompts.cpython-310-x86_64-linux-gnu.so,sha256=NPTgcEHhmCBz9FsiU-fhbFp84OB2Wq04ObWWdJchUwo,79280
-miksiai/sql_graph/sql_runnables.cpython-310-x86_64-linux-gnu.so,sha256=_tN--XjTHB5BpYj64zzkTcK0L5Pyd8ggMYUXsU499nk,955728
-miksiai-1.0.1.dist-info/METADATA,sha256=3M9bBpSV4loocVqueMTItLvbALHjN3_fQ8wps4uYPlg,7595
-miksiai-1.0.1.dist-info/WHEEL,sha256=W26pYN7HLsBT1jrDSL9udgf_mdNKJmYmL23sIP-FcgM,102
-miksiai-1.0.1.dist-info/top_level.txt,sha256=ZFs4wEgKwJOgH1c2Yw9pkvibLpluMlWlMeBx9YztSFI,8
-miksiai-1.0.1.dist-info/RECORD,,
+miksiai/agent.cpython-310-darwin.so,sha256=CxUVGBkMqTPk8rr0J31fKLfeOlkhPMjBrItQGcYTrxQ,136184
+miksiai/api.cpython-310-darwin.so,sha256=rFwRZtgdqgdlNkvbhjP7mjb-__8NFfx8_xbAQtte0VI,117142
+miksiai/master.cpython-310-darwin.so,sha256=OBqG7uSDOCA50xVRPkRfqo73oriAlrAPKqf37aM6Thg,77353
+miksiai/pythontool.cpython-310-darwin.so,sha256=nOi_eXBlkSb-fFZlHJqSBK20lqzVMvnAkl5_CQxN7ZY,100653
+miksiai/settings.cpython-310-darwin.so,sha256=lxgn4A5o0gm-co9UDBveRzOzirguPwJ6-S3i_q5vgE4,75227
+miksiai/sqltool.cpython-310-darwin.so,sha256=AhTJbq3nhqq9tYK2azQqTgkfvzxG8fmEjNr3lT8l2XE,172602
+miksiai/utils.cpython-310-darwin.so,sha256=HfCX5rtdAlc-ApvOEl31aykQVKyA4O0UeWGq4ss45cA,78168
+miksiai/sql_graph/custom_sql.cpython-310-darwin.so,sha256=7VBcfA0gVlyXtcQgZRoL8lRGgKa3F_yii4MmegFkFmM,118093
+miksiai/sql_graph/sql_graph.cpython-310-darwin.so,sha256=1WmRzSjJUloSxgx_V-i4irSuFW6R5mcNuIDxXBVR-T4,136972
+miksiai/sql_graph/sql_graph_prompts.cpython-310-darwin.so,sha256=TaX5tUGdjfdr0kJnprsWFJ_CYCIJqlEHB9bFKtQJpNQ,72260
+miksiai/sql_graph/sql_runnables.cpython-310-darwin.so,sha256=VUgwdHHY8g-Wv02wqz-K8MAWvXGWrxQn9C9aUuRZqQQ,239248
+miksiai-1.0.2.dist-info/METADATA,sha256=4chQCUxSkgEboINTuRXNxlWWV2zDPbqMJZUnvlLYAck,7454
+miksiai-1.0.2.dist-info/WHEEL,sha256=ReeDLt7JoWNv8uQs9jcofmiBOX-MvocIgD8kJPMfr7M,110
+miksiai-1.0.2.dist-info/top_level.txt,sha256=ZFs4wEgKwJOgH1c2Yw9pkvibLpluMlWlMeBx9YztSFI,8
+miksiai-1.0.2.dist-info/RECORD,,
```

