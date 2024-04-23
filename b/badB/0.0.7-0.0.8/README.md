# Comparing `tmp/badb-0.0.7.tar.gz` & `tmp/badb-0.0.8.tar.gz`

## Comparing `badb-0.0.7.tar` & `badb-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,10 @@
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 badb-0.0.7/badb.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 badb-0.0.7/requirements.txt
--rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 badb-0.0.7/my_first_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badb-0.0.7/my_first_app/Models/__init__.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 badb-0.0.7/my_first_app/Models/post.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 badb-0.0.7/my_first_app/Models/project.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 badb-0.0.7/my_first_app/Models/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badb-0.0.7/src/badb/__init__.py
--rw-r--r--   0        0        0    12229 2020-02-02 00:00:00.000000 badb-0.0.7/src/badb/__main__.py
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 badb-0.0.7/src/badb/questionnaire.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 badb-0.0.7/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 badb-0.0.7/LICENSE
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 badb-0.0.7/README.md
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 badb-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 badb-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 badb-0.0.8/badb.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 badb-0.0.8/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badb-0.0.8/src/badb/__init__.py
+-rw-r--r--   0        0        0    12229 2020-02-02 00:00:00.000000 badb-0.0.8/src/badb/__main__.py
+-rw-r--r--   0        0        0     6008 2020-02-02 00:00:00.000000 badb-0.0.8/src/badb/questionnaire.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 badb-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 badb-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 badb-0.0.8/README.md
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 badb-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 badb-0.0.8/PKG-INFO
```

### Comparing `badb-0.0.7/badb.json` & `badb-0.0.8/badb.json`

 * *Files identical despite different names*

### Comparing `badb-0.0.7/src/badb/__main__.py` & `badb-0.0.8/src/badb/__main__.py`

 * *Files identical despite different names*

### Comparing `badb-0.0.7/src/badb/questionnaire.py` & `badb-0.0.8/src/badb/questionnaire.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,106 @@
 import time
 from beaupy import confirm, prompt, select, select_multiple
 from beaupy.spinners import *
 from rich.console import Console
 from art import *
 import json
+import keyword
 
-def askQuestion():
-    data = {}
-    console = Console()
+data = {}
+console = Console()
 
-    tprint("BadB", font="swampland")
-    console.print("")
-    console.print("[bold blue]Welcome to the BADB[/bold blue]")
-    console.print("[bold blue]Create your Backend/API seamlessly[/bold blue]")
-    console.print("")
-    file_name = prompt("[green]Name your app [/green]", validator =lambda name: len(name) > 0)
-    console.print("[green]Initializing "+file_name+".json file...[/green]")
-    data['name'] = file_name
-    data['secret'] = "my_secret"
-    console.print("")
+def checkInputErrors(input):
+    keywords = keyword.kwlist
+    input = str(input).strip()
+    return True if (keywords.__contains__(input)) else False
+
+def getAppName():
+    while True:
+        try:
+            app_name = prompt("[green]Name your app [/green]", validator =lambda name: len(name) > 0)
+            if checkInputErrors(app_name):
+                console.print("[red]> Input cannot be pre-defined keywords!")
+                continue
+            else:
+                console.print("[green]> Initializing [bold]"+app_name+".json[/bold] file...[/green]")
+                console.print("")
+                return app_name
+                break
+        except:
+            console.print("[red]> Input cannot be empty!")
+
+def getAppSecret():
+    try:
+        secret = prompt("Enter the secret key for hashing passwords", validator= lambda pr: len(pr) > 0)
+    except: 
+        console.print("[red]> Input cannot be empty!")
+    return secret
+
+def getApiPrefix():
     prefix = None
     if(confirm("[green]Any prefix for api-endpoints ?[/green]")):
-        prefix = prompt("[green]Enter prefix for api-endpoints ?[/green]", validator = lambda pr: len(pr) > 0)
-        console.print("Adding prefix /"+prefix+" to api-endpoints...")
+        while True:
+            try:
+                prefix = prompt("[green]Enter prefix for api-endpoints ?[/green]", validator = lambda pr: len(pr) > 0)
+                if(checkInputErrors(prefix)):
+                    console.print("[red]> Input cannot be pre-defined keywords!")
+                    continue
+                else:
+                    console.print("[green]> Adding prefix [bold] /"+prefix+" [/bold] to api-endpoints...[/green]")
+                    console.print("")
+                    break
+            except:
+                console.print("[red]> Error while adding prefix !!!")
+                continue
+    return prefix
 
-    data['prefix'] = prefix
+def setupAppAuthentication():
+    if(confirm("[green]Want to add authentication functionality to the api ?[/green]")):
+        data['auth_config'] = {}
+        data["auth_config"]["auth"] = True
+        console.print("Adding auth functionality ...")
+        tables = list(data['schema'].keys())
+        console.print("[green]Select table of which variables will be used to verify credentials")
+        auth_table = select(options=tables, cursor="👉")
+        data["auth_config"]["table"] = auth_table
+        console.print(auth_table+" table selected...")
+        table_vars = list(data['schema'][auth_table].keys())
+        console.print("[green]Select variable to be used for verifying email/username")
+        auth_email = select(options=table_vars, cursor="👉")
+        data['auth_config']["email_field"] = auth_email
+        console.print(auth_email+" selected...")
+        console.print("[green]Select variable to be used for verifying password")
+        auth_pass = select(options=table_vars, cursor="👉")
+        data["auth_config"]['pass_field'] = auth_pass
+        console.print(auth_pass+" selected...")
+        all_routes = ["GET", "POST", "PUT", "DELETE"]
+        data["auth_config"]['auth_routes'] = {}
+        for i in tables:
+            data["auth_config"]['auth_routes'][i] = None
+            console.print("[green]Select all ROUTES to secure for "+i+" table[/green]")
+            selected_routes = select_multiple(options=all_routes, tick_character="✅")
+            str_selected_routes = ""
+            for val in selected_routes: str_selected_routes += val+", "
+            str_selected_routes = str_selected_routes[: len(str_selected_routes)-2]
+            data["auth_config"]['auth_routes'][i] = str_selected_routes
+            console.print(str(selected_routes)+" selected...")
+        data['secret'] = getAppSecret()
 
-    if(confirm("🥱 [green]Want to add schema info ?[/green]")):
-        data['schema'] = {}
-        add_more_table = False
-        while(True):
-            s_name = prompt("[green]Enter table name ?[/green]", validator = lambda pr: len(pr) > 0)
+def setupAppSchema():
+    console.print("> [green]Let's add [bold]Schema[/bold] info ...[/green]")
+    console.print("")
+    data['schema'] = {}
+    add_more_table = False
+    while(True):
+        try:
+            s_name = prompt("> [green]Enter table name ?[/green]", validator = lambda pr: len(pr) > 0)
+            if (checkInputErrors(s_name)):
+                console.print("[red]> Input cannot be pre-defined keywords!")
+                continue
             data['schema'][s_name] = {}
             console.print("Added table "+s_name)
             add_more_var = False
             while(True):
                 s_var = prompt("Add variable name (Enter) and select datatype")
                 data['schema'][s_name][s_var] = "NULL"
                 # console.print("Select datatype for variable")
@@ -49,61 +115,29 @@
                     console.print("Adding variables to schema "+s_name+" ...")
                     break
             add_more_table = confirm("Want to add more tables to project ?")
             if add_more_table:
                 continue
             else:
                 break
+        except:
+            console.print("[red]> Input cannot be empty!")
 
-        if(confirm("[green]Want to add authentication functionality to the api ?[/green]")):
-            data['auth_config'] = {}
-            data["auth_config"]["auth"] = True
-            console.print("Adding auth functionality ...")
-            tables = list(data['schema'].keys())
-            console.print("[green]Select table of which variables will be used to verify credentials")
-            auth_table = select(options=tables, cursor="👉")
-            data["auth_config"]["table"] = auth_table
-            console.print(auth_table+" table selected...")
-            table_vars = list(data['schema'][auth_table].keys())
-            console.print("[green]Select variable to be used for verifying email/username")
-            auth_email = select(options=table_vars, cursor="👉")
-            data['auth_config']["email_field"] = auth_email
-            console.print(auth_email+" selected...")
-            console.print("[green]Select variable to be used for verifying password")
-            auth_pass = select(options=table_vars, cursor="👉")
-            data["auth_config"]['pass_field'] = auth_pass
-            console.print(auth_pass+" selected...")
-            all_routes = ["GET", "POST", "PUT", "DELETE"]
-            data["auth_config"]['auth_routes'] = {}
-            for i in tables:
-                data["auth_config"]['auth_routes'][i] = None
-                console.print("[green]Select all ROUTES to secure for "+i+" table[/green]")
-                selected_routes = select_multiple(options=all_routes, tick_character="✅")
-                str_selected_routes = ""
-                for val in selected_routes: str_selected_routes += val+", "
-                str_selected_routes = str_selected_routes[: len(str_selected_routes)-2]
-                data["auth_config"]['auth_routes'][i] = str_selected_routes
-                console.print(str(selected_routes)+" selected...")
-            secret = prompt("Enter the secret key for hashing passwords", validator= lambda pr: len(pr) > 0)
-            data['secret'] = secret
-
-    # if(confirm("[green]Want to add any custom routes ?[/green]")):
-    #     console.print("Adding custom routes functionality ...")
-    #     route_name = prompt("Enter custom route name:", validator= lambda name: len(name) > 0)
-    #     console.print("Enter custom route name: [bold]"+route_name+"[/bold]")
-    #     console.print("Choose route method:")
-    #     route_method = select(options=all_routes, cursor="👉")
-    #     console.print(route_method+" selected...")
-    #     require_auth = confirm("[green]Do require authentication for this route ?")
-    #     if require_auth: console.print("Adding authentication...")
-    #     console.print("Select table required by the route")
-    #     route_table = select(options=tables, cursor="👉")
-    #     console.print(route_table+" selected...")
+def askQuestion():
 
+    tprint("BadB", font="swampland")
+    console.print("")
+    console.print("[bold blue]Welcome to the BADB[/bold blue]")
+    console.print("[bold blue]Create your Backend/API seamlessly[/bold blue]")
+    console.print("")
+    data['name'] = getAppName()
+    data['secret'] = "my_secret"
+    data['prefix'] = getApiPrefix()
+    setupAppSchema()
+    setupAppAuthentication()
 
     with open(data['name']+'.json', 'w', encoding='utf-8') as f:
         json.dump(data, f, ensure_ascii=False, indent=4)
 
-    console.print("[green bold]Run following command to create api-endpoints :[/green bold] python -m badb [cyan bold]"+file_name+".json[/cyan bold]")
-    # console.print("\t[bold] badb "+file_name+".json [/bold]")
+    console.print("[green bold]Run following command to create api-endpoints :[/green bold] badb-create-app [cyan bold]"+data['name']+".json[/cyan bold]")
```

### Comparing `badb-0.0.7/.gitignore` & `badb-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `badb-0.0.7/LICENSE` & `badb-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `badb-0.0.7/pyproject.toml` & `badb-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "badB"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Akash Srivastava", email="sriakash.dev@gmail.com" },
 ]
 description = "A pip package to create Flask RESTful-api seamlessly with customizations"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

