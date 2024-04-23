# Comparing `tmp/kurumii-1.4.8.1.tar.gz` & `tmp/kurumii-1.4.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kurumii-1.4.8.1.tar", last modified: Wed Apr 17 08:25:38 2024, max compression
+gzip compressed data, was "kurumii-1.4.8.2.tar", last modified: Tue Apr 23 14:41:06 2024, max compression
```

## Comparing `kurumii-1.4.8.1.tar` & `kurumii-1.4.8.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 08:25:38.005231 kurumii-1.4.8.1/
--rw-rw-rw-   0        0        0      309 2024-04-17 08:25:38.005231 kurumii-1.4.8.1/PKG-INFO
--rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 kurumii-1.4.8.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 08:25:37.971124 kurumii-1.4.8.1/kurumii/
--rw-rw-rw-   0        0        0     3885 2024-04-17 08:25:07.000000 kurumii-1.4.8.1/kurumii/__init__.py
--rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 kurumii-1.4.8.1/kurumii/additional_functions.py
--rw-rw-rw-   0        0        0    13965 2024-04-08 07:07:29.000000 kurumii-1.4.8.1/kurumii/ascii.py
--rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 kurumii-1.4.8.1/kurumii/data_manipulation.py
--rw-rw-rw-   0        0        0    38109 2024-04-17 08:20:32.000000 kurumii-1.4.8.1/kurumii/database.py
--rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 kurumii-1.4.8.1/kurumii/files.py
--rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 kurumii-1.4.8.1/kurumii/id.py
--rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 kurumii-1.4.8.1/kurumii/jsonify.py
--rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 kurumii-1.4.8.1/kurumii/keyboard.py
--rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 kurumii-1.4.8.1/kurumii/print_additions.py
--rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 kurumii-1.4.8.1/kurumii/profanities.py
--rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 kurumii-1.4.8.1/kurumii/youtube.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:25:38.000141 kurumii-1.4.8.1/kurumii.egg-info/
--rw-rw-rw-   0        0        0      309 2024-04-17 08:25:37.000000 kurumii-1.4.8.1/kurumii.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-04-17 08:25:37.000000 kurumii-1.4.8.1/kurumii.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 08:25:37.000000 kurumii-1.4.8.1/kurumii.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-17 08:25:37.000000 kurumii-1.4.8.1/kurumii.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 08:25:37.000000 kurumii-1.4.8.1/kurumii.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 08:25:38.008052 kurumii-1.4.8.1/setup.cfg
--rw-rw-rw-   0        0        0      388 2024-04-17 08:25:26.000000 kurumii-1.4.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:41:06.519311 kurumii-1.4.8.2/
+-rw-rw-rw-   0        0        0      309 2024-04-23 14:41:06.519311 kurumii-1.4.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 kurumii-1.4.8.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 14:41:06.502355 kurumii-1.4.8.2/kurumii/
+-rw-rw-rw-   0        0        0     3885 2024-04-17 08:25:07.000000 kurumii-1.4.8.2/kurumii/__init__.py
+-rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 kurumii-1.4.8.2/kurumii/additional_functions.py
+-rw-rw-rw-   0        0        0    15234 2024-04-23 14:40:29.000000 kurumii-1.4.8.2/kurumii/ascii.py
+-rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 kurumii-1.4.8.2/kurumii/data_manipulation.py
+-rw-rw-rw-   0        0        0    38183 2024-04-17 13:12:42.000000 kurumii-1.4.8.2/kurumii/database.py
+-rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 kurumii-1.4.8.2/kurumii/files.py
+-rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 kurumii-1.4.8.2/kurumii/id.py
+-rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 kurumii-1.4.8.2/kurumii/jsonify.py
+-rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 kurumii-1.4.8.2/kurumii/keyboard.py
+-rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 kurumii-1.4.8.2/kurumii/print_additions.py
+-rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 kurumii-1.4.8.2/kurumii/profanities.py
+-rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 kurumii-1.4.8.2/kurumii/youtube.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:41:06.516319 kurumii-1.4.8.2/kurumii.egg-info/
+-rw-rw-rw-   0        0        0      309 2024-04-23 14:41:06.000000 kurumii-1.4.8.2/kurumii.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2024-04-23 14:41:06.000000 kurumii-1.4.8.2/kurumii.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 14:41:06.000000 kurumii-1.4.8.2/kurumii.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-23 14:41:06.000000 kurumii-1.4.8.2/kurumii.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 14:41:06.000000 kurumii-1.4.8.2/kurumii.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 14:41:06.520309 kurumii-1.4.8.2/setup.cfg
+-rw-rw-rw-   0        0        0      388 2024-04-23 14:11:19.000000 kurumii-1.4.8.2/setup.py
```

### Comparing `kurumii-1.4.8.1/kurumii/__init__.py` & `kurumii-1.4.8.2/kurumii/__init__.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.1/kurumii/additional_functions.py` & `kurumii-1.4.8.2/kurumii/additional_functions.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.1/kurumii/ascii.py` & `kurumii-1.4.8.2/kurumii/ascii.py`

 * *Files 21% similar despite different names*

```diff
@@ -513,15 +513,159 @@
 " ___   ",
 "|__ \  ",
 "   ) | ",
 "  / /  ",
 " |_|   ",
 " (_)   ",
 "       "
+],
+"-":[
+"         ",   
+"         ",
+" ______  ",
+"|______| ",
+"         ",     
+"         ",
+"         "
+         
+         
+
+],
+"_":[ 
+"         ",
+"         ",
+"         ",
+"         ",
+" ______  ",
+"|______| ",
+"         "
+],
+"1":[   
+" __  ",
+"/_ | ",
+" | | ",
+" | | ",
+" | | ",
+" |_| ",
+"     "
+],
+"2":[
+" ___   ",
+"|__ \  ",
+"   ) | ",
+"  / /  ",
+" / /_  ",
+"|____| ",
+"       "
+],
+"3":[      
+" ____   ",
+"|___ \  ",
+"  __) | ",
+" |__ <  ",
+" ___) | ",
+"|____/  ",
+"        "
+],
+"4":[
+    
+" _  _    ",
+"| || |   ",
+"| || |_  ",
+"|__   _| ",
+"   | |   ",
+"   |_|   ",
+"         "
+         
+
+],
+"5":[
+" _____  ",
+"| ____| ",
+"| |__   ",
+"|___ \  ",
+" ___) | ",
+"|____/  ",
+"        "
+],
+"6":[
+    
+"   __   ",
+"  / /   ",
+" / /_   ",
+"| '_ \  ",
+"| (_) | ",
+" \___/  ",
+"        "
+],
+"7":[
+" ______  ",
+"|____  | ",
+"    / /  ",
+"   / /   ",
+"  / /    ",
+" /_/     ",
+"         "
+],
+"8":[   
+"  ___   ",
+" / _ \  ",
+"| (_) | ",
+" > _ <  ",
+"| (_) | ",
+" \___/  ",
+"        "
+],
+"9":[
+"  ___   ",
+" / _ \  ",
+"| (_) | ",
+" \__, | ",
+"   / /  ",
+"  /_/   ",
+"        "
+],
+"0":[
+    
+"  ___   ",
+" / _ \  ",
+"| | | | ",
+"| | | | ",
+"| |_| | ",
+" \___/  ",
+"        "
+],
+"+":[
+    
+"        ",
+"   _    ",
+" _| |_  ",
+"|_   _| ",
+"  |_|   ",
+"        ",
+"        "
+        
+        
+        
+
+],
+"=":[
+    
+"         ",   
+" ______  ",
+"|______| ",
+" ______  ",
+"|______| ",
+"         ",
+"         "
+         
+         
+
 ]
+
 }
 
 def print_ascii(text):
 
     combined_art = ""
     for line_num in range(len(ascii_art_['A'])):
         for char in text:
@@ -558,20 +702,20 @@
 
     print(combined_art)
 
 def print_ascii_colored(text, hex_color):
     """
     Print the text in the specified color.
     
-    :param text: The text to be printed.
-    :param color: The color in which the text should be printed.
-                  Options: 'green', 'red', 'yellow', 'blue', 'magenta', 'cyan', 'white', 'black', 'gray', 
-                           'lightgray', 'darkgray', 'lightblue', 'lightgreen', 'lightcyan', 'lightred', 'pink'
-                  Optionally, the color can be specified as a hexadecimal string.
-                  Optional: False
+    - Args:
+        - text (str): The text that should be printed
+        - hex_color: The color in hex
+    
+    - Returns:
+        - None
     """
     color_codes = {
         "green": "0;255;0",
         "red": "255;0;0",
         "yellow": "255;255;0",
         "blue": "0;0;255",
         "magenta": "255;0;255",
```

### Comparing `kurumii-1.4.8.1/kurumii/data_manipulation.py` & `kurumii-1.4.8.2/kurumii/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.1/kurumii/database.py` & `kurumii-1.4.8.2/kurumii/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 def create_sqlite_database(filename:str,path:str=".\\db",overwrite=False, logging=False):
     """
     Create an empty SQLite database file.
 
     Args:
         - path (str, optional): The path where the database file should be created. Defaults to current directory.
-        - filename (str, optional): The name of the database file. Defaults to "example.db".
+        - filename (str): The name of the database file.
         - overwrite (bool, optional): Whether to overwrite the existing file if it already exists. 
                                     Defaults to False.
         - logging (bool, optional): Whether to log success or failure messages. Defaults to False.
     
     Returns:
         - tuple: 
             - A tuple containing a boolean indicating whether the database file was created successfully
@@ -144,23 +144,24 @@
             print(f"Empty database file '{filename}' created successfully in '{file_path}'.")
         return True, file_path
     except Exception as e:
         if logging:
             print(f"Error occurred while creating database file: {e}")
         return False, file_path
     
-def create_table(table_name, columns, filepath, primary_key, overwrite=False, logging=False):
+def create_table(columns, filepath, primary_key, table_name="data", overwrite=False, logging=False):
     """
     Add a table to an SQLite database.
 
     Args:
-        - table_name (str): The name of the table to be added.
         - columns (str): A string representing the columns of the table in SQLite syntax.
         - filepath (str): The path to the SQLite database file.
         - primary_key (str): The primary key of the table.
+        - table_name (str, optional): The name of the table to be added.
+                                     Defaults to 'data'
         - overwrite (bool, optional): Whether to overwrite the existing table if it already exists. 
                                      Defaults to False.
         - logging (bool, optional): Whether to log success or failure messages. Defaults to False.
     
     Returns:
         - bool: A boolean indicating whether the table was added successfully (True) or not (False).
     
@@ -222,21 +223,21 @@
                 print(f"Error creating table '{table_name}': {str(e)}")
             return(False)
     else:
         if logging:
             print(f"The file '{filepath}' does not exist")
         return(False)
 
-def remove_table(table_name, filepath, confirm=False, logging=False):
+def remove_table(filepath, table_name="data", confirm=False, logging=False):
     """
     Remove a table from an SQLite database.
 
     Args:
-        - table_name (str): The name of the table to be deleted.
         - filepath (str): The path to the SQLite database file.
+        - table_name (str, optional): The name of the table to be deleted. Defaults to 'data'
         - confirm (bool, optional): Whether to prompt the user for confirmation before deletion. Defaults to False.
         - logging (bool, optional): Whether to log success or failure messages. Defaults to False.
     
     Returns:
         - bool: A boolean indicating whether the table was deleted successfully (True) or not (False).
     
     Raises:
```

### Comparing `kurumii-1.4.8.1/kurumii/files.py` & `kurumii-1.4.8.2/kurumii/files.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.1/kurumii/id.py` & `kurumii-1.4.8.2/kurumii/id.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.1/kurumii/jsonify.py` & `kurumii-1.4.8.2/kurumii/jsonify.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.1/kurumii/keyboard.py` & `kurumii-1.4.8.2/kurumii/keyboard.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.1/kurumii/print_additions.py` & `kurumii-1.4.8.2/kurumii/print_additions.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.1/kurumii/profanities.py` & `kurumii-1.4.8.2/kurumii/profanities.py`

 * *Files identical despite different names*

### Comparing `kurumii-1.4.8.1/kurumii/youtube.py` & `kurumii-1.4.8.2/kurumii/youtube.py`

 * *Files identical despite different names*

