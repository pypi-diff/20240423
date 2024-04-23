# Comparing `tmp/time_tracker-0.4.1.tar.gz` & `tmp/time_tracker-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_tracker-0.4.1.tar", max compression
+gzip compressed data, was "time_tracker-0.5.0.tar", max compression
```

## Comparing `time_tracker-0.4.1.tar` & `time_tracker-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-04-21 16:00:56.633415 time_tracker-0.4.1/LICENSE
--rw-r--r--   0        0        0     1256 2023-04-21 16:00:56.633415 time_tracker-0.4.1/README.md
--rw-r--r--   0        0        0      638 2023-04-21 16:00:56.633415 time_tracker-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 16:00:56.633415 time_tracker-0.4.1/time_tracker/__init__.py
--rw-r--r--   0        0        0     2766 2023-04-21 16:00:56.633415 time_tracker-0.4.1/time_tracker/log.py
--rw-r--r--   0        0        0     5179 2023-04-21 16:00:56.633415 time_tracker-0.4.1/time_tracker/main.py
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 time_tracker-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-22 08:00:59.639340 time_tracker-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1256 2024-04-22 08:00:59.639414 time_tracker-0.5.0/README.md
+-rw-r--r--   0        0        0      638 2024-04-23 13:47:29.317816 time_tracker-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-22 08:00:59.640182 time_tracker-0.5.0/time_tracker/__init__.py
+-rw-r--r--   0        0        0     2829 2024-04-23 13:42:43.505217 time_tracker-0.5.0/time_tracker/log.py
+-rw-r--r--   0        0        0     5227 2024-04-23 13:41:50.606441 time_tracker-0.5.0/time_tracker/main.py
+-rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 time_tracker-0.5.0/PKG-INFO
```

### Comparing `time_tracker-0.4.1/LICENSE` & `time_tracker-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `time_tracker-0.4.1/README.md` & `time_tracker-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `time_tracker-0.4.1/pyproject.toml` & `time_tracker-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "time-tracker"
-version = "0.4.1"
+version = "0.5.0"
 description = "CLI to track time spent on tasks using pomodoro technique"
 authors = ["Jose Cabeda <jecabeda@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 tt = "time_tracker.main:app"
```

### Comparing `time_tracker-0.4.1/time_tracker/log.py` & `time_tracker-0.5.0/time_tracker/log.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,32 +14,38 @@
 
     def apply_configs(
         self, format: str = "%(asctime)-10s | %(levelname)s | %(message)s"
     ):
         self.log_folder = Path(os.getenv("TT_LOG_FOLDER", "."))
 
         self.log_file = self.log_folder / f"{(datetime.today()).strftime('%Y%m%d')}.log"
-        logging.basicConfig(filename=self.log_file, format=format, level=logging.INFO)
+        logging.basicConfig(filename=self.log_file, format=format, level=logging.WARN)
 
     def write_thought(self, message: str):
-        logger = logging.getLogger()  # Logger
-        logger_handler = logging.FileHandler(
-            filename=self.log_file
-        )  # Handler for the logger
-        logger.addHandler(logger_handler)
-        FORMAT = "thought: %(message)s"
-
-        # New formatter for the handler:
-        logger_handler.setFormatter(logging.Formatter(FORMAT))
-
-        logging.info(message)
-        logger.removeHandler(logger_handler)
+        # logger = logging.getLogger()  # Logger
+        # logger_handler = logging.FileHandler(
+        #     filename=self.log_file
+        # )  # Handler for the logger
+        # logger.addHandler(logger_handler)
+        # FORMAT = "thought: %(message)s"
+
+        # # New formatter for the handler:
+        # logger_handler.setFormatter(logging.Formatter(FORMAT))
+
+        # logging.info(message)
+        # logger.removeHandler(logger_handler)
+
+        # append the thought into the markdown file in the log folder
+        with open(
+            self.log_folder / f"{(datetime.today()).strftime('%Y-%m-%d')}.md", "a"
+        ) as file:
+            file.write(f"thought: {message}\n")
 
     def retrieve_thoughts(self):
-        list_of_files = list(self.log_folder.glob("*.log"))
+        list_of_files = list(self.log_folder.glob("*.md"))
 
         thoughts: list[str] = []
 
         for file in list_of_files:
             with open(file, "r") as file:
                 content = file.readlines()
                 filtered_logs = list(filter(self.is_thought_line, content))
@@ -53,15 +59,15 @@
         return thoughts
 
     def is_thought_line(self, message: str):
         return message.startswith("thought")
 
     def get_logs(self, last_log: bool, output: bool):
         if last_log:
-            list_of_files = list(self.log_folder.glob("*.log"))
+            list_of_files = list(self.log_folder.glob("*.md"))
             list_of_files_not_empty = list(
                 filter(lambda x: os.path.getsize(x) > 0, list_of_files)
             )  # Remove all empty files
 
             if list_of_files_not_empty == []:
                 print("No logs yet")
                 return None
@@ -78,17 +84,7 @@
             else:
                 os.system(f"open {latest_file}")  # Open directory
 
         else:
             os.system(f"open {self.log_folder}")
 
         return True
-
-    def info(self, data):
-        logging.info(data)
-
-    def warning(self, data):
-        logging.warn(data)
-
-    def error(self, data):
-        logging.error(data)
-        logging.error(data)
```

### Comparing `time_tracker-0.4.1/time_tracker/main.py` & `time_tracker-0.5.0/time_tracker/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,16 @@
 
 def runSession(time: int, shouldPrompt: bool, sessionType: SessionType):
     """Run individual session (supports work or break sessions)"""
 
     if sessionType == sessionType.workTime:
         workDescription: str = typer.prompt("What do you plan to do?")
 
-        logger.info(f"Work {time} min. TODO: {workDescription}")
+        # logger.info(f"Work {time} min. TODO: {workDescription}")
+        logger.write_thought(workDescription)
         countdown(time)
         notify("Session finished", "Ready for next?")
     else:
         logger.info(f"Started break session with {time} minutes.")
         countdown(time)
         notify("Session finished", "Ready for next?")
```

### Comparing `time_tracker-0.4.1/PKG-INFO` & `time_tracker-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: time-tracker
-Version: 0.4.1
+Version: 0.5.0
 Summary: CLI to track time spent on tasks using pomodoro technique
 Author: Jose Cabeda
 Author-email: jecabeda@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: python-dotenv (>=0.19.2,<0.20.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: typer (==0.7.0)
 Description-Content-Type: text/markdown
 
 # `time-tracker`
```

