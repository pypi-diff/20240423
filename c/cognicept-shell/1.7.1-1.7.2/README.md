# Comparing `tmp/cognicept-shell-1.7.1.tar.gz` & `tmp/cognicept-shell-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognicept-shell-1.7.1.tar", last modified: Fri Dec 29 07:07:50 2023, max compression
+gzip compressed data, was "cognicept-shell-1.7.2.tar", last modified: Tue Apr 23 13:40:18 2024, max compression
```

## Comparing `cognicept-shell-1.7.1.tar` & `cognicept-shell-1.7.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-sr-x   0     1000     1000        0 2023-12-29 07:07:50.979423 cognicept-shell-1.7.1/
--rw-r--r--   0     1000     1000    11357 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/LICENSE.txt
--rw-r--r--   0     1000     1000    19785 2023-12-29 07:07:50.975423 cognicept-shell-1.7.1/PKG-INFO
--rw-r--r--   0     1000     1000    18921 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/README.md
-drwxr-sr-x   0     1000     1000        0 2023-12-29 07:07:50.975423 cognicept-shell-1.7.1/cognicept_shell.egg-info/
--rw-r--r--   0     1000     1000    19785 2023-12-29 07:07:50.000000 cognicept-shell-1.7.1/cognicept_shell.egg-info/PKG-INFO
--rw-r--r--   0     1000     1000      906 2023-12-29 07:07:50.000000 cognicept-shell-1.7.1/cognicept_shell.egg-info/SOURCES.txt
--rw-r--r--   0     1000     1000        1 2023-12-29 07:07:50.000000 cognicept-shell-1.7.1/cognicept_shell.egg-info/dependency_links.txt
--rw-r--r--   0     1000     1000       61 2023-12-29 07:07:50.000000 cognicept-shell-1.7.1/cognicept_shell.egg-info/entry_points.txt
--rw-r--r--   0     1000     1000      201 2023-12-29 07:07:50.000000 cognicept-shell-1.7.1/cognicept_shell.egg-info/requires.txt
--rw-r--r--   0     1000     1000       21 2023-12-29 07:07:50.000000 cognicept-shell-1.7.1/cognicept_shell.egg-info/top_level.txt
-drwxr-sr-x   0     1000     1000        0 2023-12-29 07:07:50.975423 cognicept-shell-1.7.1/cogniceptshell/
--rw-r--r--   0     1000     1000        0 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/cogniceptshell/__init__.py
--rw-r--r--   0     1000     1000    60991 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/cogniceptshell/agent_life_cycle.py
--rw-r--r--   0     1000     1000     2461 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/cogniceptshell/common.py
--rw-r--r--   0     1000     1000    30102 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/cogniceptshell/configuration.py
--rw-r--r--   0     1000     1000    10445 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/cogniceptshell/interface.py
--rw-r--r--   0     1000     1000    11482 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/cogniceptshell/pusher.py
--rw-r--r--   0     1000     1000    45142 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/cogniceptshell/robot_actions.py
--rw-r--r--   0     1000     1000    19344 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/cogniceptshell/rosbag_record.py
--rw-r--r--   0     1000     1000       38 2023-12-29 07:07:50.979423 cognicept-shell-1.7.1/setup.cfg
--rw-r--r--   0     1000     1000     1468 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/setup.py
-drwxr-sr-x   0     1000     1000        0 2023-12-29 07:07:50.975423 cognicept-shell-1.7.1/tests/
--rw-r--r--   0     1000     1000        0 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/tests/__init__.py
-drwxr-sr-x   0     1000     1000        0 2023-12-29 07:07:50.975423 cognicept-shell-1.7.1/tests/unit/
--rw-r--r--   0     1000     1000        0 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/tests/unit/__init__.py
--rw-r--r--   0     1000     1000     2414 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/tests/unit/mock_docker_client.py
--rw-r--r--   0     1000     1000     9247 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/tests/unit/test_config.py
--rw-r--r--   0     1000     1000      441 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/tests/unit/test_get_disk_space.py
--rw-r--r--   0     1000     1000     3203 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/tests/unit/test_get_robot_org_id.py
--rw-r--r--   0     1000     1000     3485 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/tests/unit/test_keyrotate.py
--rw-r--r--   0     1000     1000    34825 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/tests/unit/test_lifecycle.py
--rw-r--r--   0     1000     1000    34496 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/tests/unit/test_move.py
--rw-r--r--   0     1000     1000     4153 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/tests/unit/test_populate_config_files.py
--rw-r--r--   0     1000     1000     4134 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/tests/unit/test_pull_config_templates.py
--rw-r--r--   0     1000     1000     6978 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/tests/unit/test_update_event_log.py
--rwxr-xr-x   0     1000     1000     1543 2023-12-29 07:06:32.000000 cognicept-shell-1.7.1/tests/unit/test_version_update.py
+drwxr-sr-x   0     1000     1000        0 2024-04-23 13:40:18.928927 cognicept-shell-1.7.2/
+-rw-r--r--   0     1000     1000    11357 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/LICENSE.txt
+-rw-r--r--   0     1000     1000    20083 2024-04-23 13:40:18.928927 cognicept-shell-1.7.2/PKG-INFO
+-rw-r--r--   0     1000     1000    19219 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/README.md
+drwxr-sr-x   0     1000     1000        0 2024-04-23 13:40:18.924927 cognicept-shell-1.7.2/cognicept_shell.egg-info/
+-rw-r--r--   0     1000     1000    20083 2024-04-23 13:40:18.000000 cognicept-shell-1.7.2/cognicept_shell.egg-info/PKG-INFO
+-rw-r--r--   0     1000     1000      906 2024-04-23 13:40:18.000000 cognicept-shell-1.7.2/cognicept_shell.egg-info/SOURCES.txt
+-rw-r--r--   0     1000     1000        1 2024-04-23 13:40:18.000000 cognicept-shell-1.7.2/cognicept_shell.egg-info/dependency_links.txt
+-rw-r--r--   0     1000     1000       61 2024-04-23 13:40:18.000000 cognicept-shell-1.7.2/cognicept_shell.egg-info/entry_points.txt
+-rw-r--r--   0     1000     1000      201 2024-04-23 13:40:18.000000 cognicept-shell-1.7.2/cognicept_shell.egg-info/requires.txt
+-rw-r--r--   0     1000     1000       21 2024-04-23 13:40:18.000000 cognicept-shell-1.7.2/cognicept_shell.egg-info/top_level.txt
+drwxr-sr-x   0     1000     1000        0 2024-04-23 13:40:18.924927 cognicept-shell-1.7.2/cogniceptshell/
+-rw-r--r--   0     1000     1000        0 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/cogniceptshell/__init__.py
+-rw-r--r--   0     1000     1000    61610 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/cogniceptshell/agent_life_cycle.py
+-rw-r--r--   0     1000     1000     2461 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/cogniceptshell/common.py
+-rw-r--r--   0     1000     1000    30260 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/cogniceptshell/configuration.py
+-rw-r--r--   0     1000     1000    10622 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/cogniceptshell/interface.py
+-rw-r--r--   0     1000     1000    11482 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/cogniceptshell/pusher.py
+-rw-r--r--   0     1000     1000    43982 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/cogniceptshell/robot_actions.py
+-rw-r--r--   0     1000     1000    19344 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/cogniceptshell/rosbag_record.py
+-rw-r--r--   0     1000     1000       38 2024-04-23 13:40:18.928927 cognicept-shell-1.7.2/setup.cfg
+-rw-r--r--   0     1000     1000     1467 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/setup.py
+drwxr-sr-x   0     1000     1000        0 2024-04-23 13:40:18.928927 cognicept-shell-1.7.2/tests/
+-rw-r--r--   0     1000     1000        0 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/tests/__init__.py
+drwxr-sr-x   0     1000     1000        0 2024-04-23 13:40:18.928927 cognicept-shell-1.7.2/tests/unit/
+-rw-r--r--   0     1000     1000        0 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/tests/unit/__init__.py
+-rw-r--r--   0     1000     1000     2414 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/tests/unit/mock_docker_client.py
+-rw-r--r--   0     1000     1000     9247 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/tests/unit/test_config.py
+-rw-r--r--   0     1000     1000      441 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/tests/unit/test_get_disk_space.py
+-rw-r--r--   0     1000     1000     3203 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/tests/unit/test_get_robot_org_id.py
+-rw-r--r--   0     1000     1000     3485 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/tests/unit/test_keyrotate.py
+-rw-r--r--   0     1000     1000    35061 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/tests/unit/test_lifecycle.py
+-rw-r--r--   0     1000     1000    34498 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/tests/unit/test_move.py
+-rw-r--r--   0     1000     1000     4153 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/tests/unit/test_populate_config_files.py
+-rw-r--r--   0     1000     1000     4134 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/tests/unit/test_pull_config_templates.py
+-rw-r--r--   0     1000     1000     6978 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/tests/unit/test_update_event_log.py
+-rwxr-xr-x   0     1000     1000     2045 2024-04-23 13:40:00.000000 cognicept-shell-1.7.2/tests/unit/test_version_update.py
```

### Comparing `cognicept-shell-1.7.1/LICENSE.txt` & `cognicept-shell-1.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.7.1/PKG-INFO` & `cognicept-shell-1.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognicept-shell
-Version: 1.7.1
+Version: 1.7.2
 Summary: Shell utility to configure Cognicept tools.
 Home-page: https://kabam.ai
 Author: Jakub Tomasek
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -511,14 +511,21 @@
 
 * Feature branch: /feature/name-of-the-feature
 * Bug fix branch: /fix/name-of-the-bug
 * Release branch: /release/name-of-the-release
 
 
 ## Version history
+* 1.7.2[23/04/2024]
+  * Fix pip dependency version issues
+  * Fix region name parameter issue
+  * Limit the log size with docker compose
+  * Fix latest version check on cognicept update
+  * Backward compatibility for `cognicept restart -d`
+  * Fix `cognicept move` fail to port robot and map issue
 * 1.7.1[24/11/2023]
   * Bug Fixed - templates directory blocking cognicept restart
   * cognicept prune to support only in attached mode
 * 1.7.0[25/10/2023]
   * `cognicept update` check for remaining disk space (in root directory) before pulling each image
   * `cognicept update -s` overrides check for disk space before pulling images
   * `cognicept update` will update the success or failure to S+ event logs
```

### Comparing `cognicept-shell-1.7.1/README.md` & `cognicept-shell-1.7.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -488,14 +488,21 @@
 
 * Feature branch: /feature/name-of-the-feature
 * Bug fix branch: /fix/name-of-the-bug
 * Release branch: /release/name-of-the-release
 
 
 ## Version history
+* 1.7.2[23/04/2024]
+  * Fix pip dependency version issues
+  * Fix region name parameter issue
+  * Limit the log size with docker compose
+  * Fix latest version check on cognicept update
+  * Backward compatibility for `cognicept restart -d`
+  * Fix `cognicept move` fail to port robot and map issue
 * 1.7.1[24/11/2023]
   * Bug Fixed - templates directory blocking cognicept restart
   * cognicept prune to support only in attached mode
 * 1.7.0[25/10/2023]
   * `cognicept update` check for remaining disk space (in root directory) before pulling each image
   * `cognicept update -s` overrides check for disk space before pulling images
   * `cognicept update` will update the success or failure to S+ event logs
```

### Comparing `cognicept-shell-1.7.1/cognicept_shell.egg-info/PKG-INFO` & `cognicept-shell-1.7.2/cognicept_shell.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognicept-shell
-Version: 1.7.1
+Version: 1.7.2
 Summary: Shell utility to configure Cognicept tools.
 Home-page: https://kabam.ai
 Author: Jakub Tomasek
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -511,14 +511,21 @@
 
 * Feature branch: /feature/name-of-the-feature
 * Bug fix branch: /fix/name-of-the-bug
 * Release branch: /release/name-of-the-release
 
 
 ## Version history
+* 1.7.2[23/04/2024]
+  * Fix pip dependency version issues
+  * Fix region name parameter issue
+  * Limit the log size with docker compose
+  * Fix latest version check on cognicept update
+  * Backward compatibility for `cognicept restart -d`
+  * Fix `cognicept move` fail to port robot and map issue
 * 1.7.1[24/11/2023]
   * Bug Fixed - templates directory blocking cognicept restart
   * cognicept prune to support only in attached mode
 * 1.7.0[25/10/2023]
   * `cognicept update` check for remaining disk space (in root directory) before pulling each image
   * `cognicept update -s` overrides check for disk space before pulling images
   * `cognicept update` will update the success or failure to S+ event logs
```

### Comparing `cognicept-shell-1.7.1/cognicept_shell.egg-info/SOURCES.txt` & `cognicept-shell-1.7.2/cognicept_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.7.1/cogniceptshell/agent_life_cycle.py` & `cognicept-shell-1.7.2/cogniceptshell/agent_life_cycle.py`

 * *Files 1% similar despite different names*

```diff
@@ -824,28 +824,33 @@
         os.system("xhost -local:root")
 
     def cognicept_version_update(object,args):
         current_version = pkg_resources.require("cognicept-shell")[0].version
         package = 'cognicept-shell'
         response = requests.get(f'https://pypi.org/pypi/{package}/json')
         latest_version = response.json()['info']['version']
-        if latest_version != current_version:
+        if latest_version > current_version:
             if args.skip:
                 user_input = 'y'
             else:
-                user_input = input(f"New Cognicept Shell version {latest_version} is available! Proceed with update? ")
+                user_input = ""
+                while(user_input.lower() != "y" and user_input.lower() != "n"):
+                    user_input = input(f"New Cognicept Shell version {latest_version} is available! current version is {current_version}, proceed with update (y/n) ?  ")
 
-            if user_input == 'Y' or user_input == 'y':
+            if user_input.lower() == "y":
                 print(f"{package} current version {current_version} - Installing Version {latest_version}")
-                os.system(f'pip3 install -q {package}=={latest_version}')
-                print(f'Installation {package} to version {latest_version}:'+bcolors.OKBLUE + " DONE" + bcolors.ENDC)
+                updation_result = os.system(f'pip3 install -q {package}=={latest_version}')
+                if updation_result == 0: # Process exited with success   
+                    print(f'Updating {package} to version {latest_version}:'+bcolors.OKGREEN + " SUCCESS" + bcolors.ENDC + "\n")
+                else:
+                    print(f'Updating {package} to version {latest_version}:'+bcolors.FAIL + " FAILED" + bcolors.ENDC + "\n")
             else:
                 print(f"{package} was not updated. Current version: {current_version}")
         else:
-            print(f"{package} already in latest version={latest_version}")
+            print(f"{package} already on latest version={latest_version}")
 
     def pull_image(object,image_name,N,i):
         """
         Pulls a Docker image and displays a progress bar.
 
             Parameters:
                 image_name : The name of the Docker image to pull.
@@ -954,15 +959,15 @@
                         raise OSError
 
             except docker.errors.NotFound:
                 try:
                     object.pull_image(image_name,N=N, i=i)
                     
                 except docker.errors.NotFound:
-                    print(bcolors.FAIL + "Error: " + bcolors.ENDC + f"Image {image_name_short} can’t be accessed in ECR or Docker Hub.")
+                    print(bcolors.FAIL + "Error: " + bcolors.ENDC + f"Image {image_name_short} can't be accessed in ECR or Docker Hub.")
                     print("[" + str(i) + "/" + str(N) + "] " + image_name_short +
                         " - " + bcolors.FAIL + "FAILED" + bcolors.ENDC + "\033[K")
                     success_flag = False
                     
                 except DockerException as ex:
                     print("[" + str(i) + "/" + str(N) + "] " + image_name_short +
                         " - " + bcolors.FAIL + "FAILED" + bcolors.ENDC + "\033[K")
@@ -1259,15 +1264,15 @@
         if (image_data[1] == 'latest') and ('ecr' in image_uri):
             repo_name = image_data[0].split('/')[1]
             registry_id = image_uri.split('.')[0]
             image_digest = object.get_image_digest(':'.join(image_data))
             
             try:
                 if image_digest:
-                    ecr_client = boto3.client('ecr')
+                    ecr_client = boto3.client('ecr', region_name='ap-southeast-1')
                     response = ecr_client.describe_images(
                         registryId=registry_id,
                         repositoryName=repo_name,
                         imageIds=[
                             {
                                 "imageDigest":image_digest    
                             }
@@ -1287,14 +1292,17 @@
                 else:
                     return None
             
             except boto3.exceptions.Boto3Error as e:
                 print(f"Error occurred while querying ECR: {e}")
                 return None
             
+            except botocore.exceptions.NoCredentialsError as e:
+                return None
+            
             except Exception as e:
                 print("Error: " + str(e))
                 return None    
         
     def display_version(object, args):
         """
         Display Cognicept-Shell version and docker images version
@@ -1339,12 +1347,14 @@
                 "--abort-on-container-exit": False,
                 "--remove-orphans": False,
                 "--force-recreate": False,
                 "--build": False,
                 "--no-build": True,
                 "--scale": [f'{container_name}=1'],
                 "--quiet-pull": True,
+                "--log-driver": "json-file",
+                "--log-opt": "max-size=5m"
                 }
         project = project_from_options(object._compose_dir,option)
         compose_cmd = TopLevelCommand(project)
         compose_cmd.up(option)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cognicept-shell-1.7.1/cogniceptshell/common.py` & `cognicept-shell-1.7.2/cogniceptshell/common.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.7.1/cogniceptshell/configuration.py` & `cognicept-shell-1.7.2/cogniceptshell/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                     " Aborting saving runtime configuration: " + ex.strerror + bcolors.ENDC)
         
         # If backup is success, try to save it
         if backup_success:
             try:
                 with open(object.env_path, 'w') as file:
                     for key, value in object.config.items():
-                        file.write(key + '=' + value + '\n')
+                        file.write(key + '=' + ("" if value is None else value) + '\n')
             except OSError:
                 print(bcolors.FAIL + "Could not write into `" + object.env_path +
                     "`. Please check write permission or run with `sudo`." + bcolors.ENDC)        
 
     def get_cognicept_credentials(object):
         """
         Checks and returns `COGNICEPT_ACCESS_KEY` from configuration.
@@ -473,15 +473,15 @@
                 "AccessKeyId"]
             object.config["AWS_SECRET_ACCESS_KEY"] = response[
                 "SecretAccessKey"]
             object.config["AWS_SESSION_TOKEN"] = response[
                 "SessionToken"]
             object.config["AWS_TOKEN_EXPIRATION"] = response[
                 "Expiration"]
-            print("Cloud access keys rotated successfully!")
+            print(bcolors.OKGREEN+"Cloud access keys rotated successfully!"+bcolors.ENDC)
         except requests.exceptions.Timeout:
             print("Cognicept REST API error: time out.")
             return False
         except requests.exceptions.TooManyRedirects:
             print("Cognicept REST API error: Wrong endpoint.")
             return False
         except Exception as e:
@@ -515,18 +515,18 @@
                 template_key = template['Key']
                 template_filename = os.path.basename(template_key)
                 
                 if template_filename.endswith(('.yaml', '.yml')):
                     destination_path = os.path.join(templates_folder, template_filename)
                     s3.download_file(bucket_name,template_key,destination_path)
 
-            print('All robot configuration templates have been successfully downloaded.')
+            print(bcolors.OKGREEN+'All robot configuration templates have been successfully downloaded.'+bcolors.ENDC)
 
         except Exception:
-            print("Failed to retrieve template config files")
+            print(bcolors.WARNING +"Warning: Failed to retrieve template config files" + bcolors.ENDC)
             return False
 
     def check_user_api_version(object, api_uri):
         if 'v1' in api_uri:
             print("WARNING: COGNICEPT_USER_API is 'v1'. Initializing robot with robot_code and org_code will fail!")
             init_endpoint = "spinup/config/"
         else:
@@ -656,15 +656,15 @@
                 r.raise_for_status()
                 j = r.json()
                 if j:
                     for key in j:
                         object.config[key] = j[key]
                     object.save_config()
                     object.pull_config_templates(args)
-                    print("Successfully initialized configuration for the robot `" + robot_id + "`. To start agents run `cognicept start`")
+                    print(bcolors.OKGREEN + "Successfully initialized configuration for the robot `" + robot_id + "`. To start agents run `cognicept start`"+ bcolors.ENDC)
                     return True
                 else:
                     print("Failed to initialize the robot: ID `" + robot_id + "` in organization `" + org_id + "` not found")
                     return False
                 
         except requests.exceptions.Timeout:
             print("Cognicept REST API error: time out.")
```

### Comparing `cognicept-shell-1.7.1/cogniceptshell/interface.py` & `cognicept-shell-1.7.2/cogniceptshell/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,16 @@
 
 parser_lastevent.add_argument(
     '--path', help='Cognicept configuration directory (default: `' + DEFAULT_PATH + '`)', default=DEFAULT_PATH)
 
 
 parser_restart.add_argument('-a', '--attach', action='store_true',
                             help='sets restart to be run in a attached manner. Progress will be printed')
+parser_restart.add_argument('-d', '--detach', action='store_true',
+                            help='sets restart to be run in a detached. By default restart in detached mode')
 parser_restart.add_argument(
     '--path', help='Cognicept configuration directory (default: `' + DEFAULT_PATH + '`)', default=DEFAULT_PATH)
 parser_restart.add_argument(
     'list', help='List of agents to restart, leave empty to restart all agents', metavar='list', type=str, nargs='*',choices=container_names)
 parser_restart.add_argument('--prune', action='store_true',
                             help='Clears the logs of in kriya_logs and agent logs, only attached mode restart is supported with this argument')
```

### Comparing `cognicept-shell-1.7.1/cogniceptshell/pusher.py` & `cognicept-shell-1.7.2/cogniceptshell/pusher.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.7.1/cogniceptshell/robot_actions.py` & `cognicept-shell-1.7.2/cogniceptshell/robot_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,19 +260,14 @@
             image_file = io.BytesIO(get_map_resp.content)
             image_data = image_file.read()
             b64_string = base64.b64encode(image_data).decode('utf-8')
         except Exception as err:
             print("Failed to decode image file")
             raise SystemExit(1)
         
-        # remove padding
-        last_index = len(b64_string) - 1
-        while b64_string[last_index] == "=":
-            b64_string = b64_string[:-1]
-            last_index -= 1
         return b64_string
     
     def get_maps_from_robot_id(self, robot_id, headers):
         map_base_uri = self.api_uri + "map/"
         get_map_uri = map_base_uri + '?filter={{"robot_id":"{robot_id}"}}'.format(robot_id=robot_id)
         get_map_resp = requests.get(get_map_uri, headers=headers, timeout=5)
         if get_map_resp.status_code != 200:
@@ -594,56 +589,34 @@
         headers['Authorization'] = 'Bearer ' + new_access_token
         
         newly_created_data = {}
 
         try:
             #### Create property in new organization - if required ####
             if new_property_id is None:
-                old_property_data.pop('created_at', None)
-                old_property_data.pop('modified_at', None)
-                old_property_data.pop('is_default', None)
-                old_property_data.pop('property_id', None)
-                old_property_data.pop('is_deleted', None)
+                new_property_data = {
+                    "property_code": old_property_data['property_code'],
+                    "property_name": old_property_data['property_name'],
+                    "status": "Active",
+                    "zendesk_id": old_property_data['zendesk_id']
+                }
             
-                new_property_id = self.create_property(property_details=old_property_data, headers=headers)
+                new_property_id = self.create_property(property_details=new_property_data, headers=headers)
                 newly_created_data['property_id'] = new_property_id
 
-            #### Create robot in new organization ####
-            # Modify the data to create the robot in the new organization
-            old_robot_data.pop("robot_id", None)
-            old_robot_data.pop("pilot_config", None)
-            old_robot_data.pop("robot_code", None)
-            old_robot_data.pop("modified_at", None)
-            old_robot_data.pop("robot_url", None)
-            old_robot_data.pop("is_deleted", None)
-            old_robot_data.pop("last_heartbeat_at", None)
-            old_robot_data.pop("last_health_update", None)
-            old_robot_data.pop("model_code", None)
-            old_robot_data.pop("organization_id", None)
-            old_robot_data.pop("status_details", None)
-            old_robot_data.pop("adapter_url", None)
-            old_robot_data.pop("aws_role_id", None)
-            old_robot_data.pop("aws_channel_arn", None)
-            
-            old_robot_data['status'] = "Offline"
-            old_robot_data['property_id'] = new_property_id
-
-            # Remove any keys in robot data with value as None #
-            delete_keys = []
-            for key, value in old_robot_data.items():
-                if value is None or value == 'None':
-                    delete_keys.append(key)
-            for key in delete_keys:
-                old_robot_data.pop(key)
-            
-            # oem_id is required even tho it is null
-            if old_robot_data.get('oem_id', None) is None: 
-                old_robot_data['oem_id'] = None
+            new_robot_data = {
+                "model_id": old_robot_data['model_id'],
+                "nick_name": old_robot_data['nick_name'],
+                "oem_id": old_robot_data['oem_id'],
+                "property_id": new_property_id,
+                "status": "Offline",
+                "zendesk_id": old_robot_data['zendesk_id']
+            }
 
-            new_robot_id = self.create_robot(robot_details=old_robot_data, headers=headers)
+            new_robot_id = self.create_robot(robot_details=new_robot_data, headers=headers)
             newly_created_data['robot'] = {
                 "robot_id": new_robot_id,
                 "organization_id": args.new_org_id
             }
             
             print(bcolors.OKBLUE + "Porting over robot details..." + bcolors.ENDC)
 
@@ -676,15 +649,17 @@
                 old_waypoint_id = waypoint_data.pop('waypoint_id', None)
                 to_delete_waypoint_id.append(old_waypoint_id)
 
                 old_map_id = waypoint_data.pop('map_id', None)
                 waypoint_data['map_id'] = old_to_new_map_dict[old_map_id]
                 waypoint_data.pop('map', None)
                 waypoint_data['waypoint_name'] = waypoint_data.get('name', '')
-
+                waypoint_data.pop('name', None)
+                if waypoint_data['tag'] == None:
+                    waypoint_data['tag'] = []
                 new_waypoint_id = self.create_waypoint(waypoint_details=waypoint_data, headers=headers)
                 waypoint_count += 1
                 
                 created_waypoints = newly_created_data.get('waypoints', [])
                 created_waypoints.append(new_waypoint_id)
                 newly_created_data['waypoints'] = created_waypoints
 
@@ -847,8 +822,8 @@
                 'Authorization': 'Bearer ' + access_token
             }
             self.delete_robot(robot_id=args.robot_id, organization_id=args.old_org_id, headers=headers)
             for mission_id in old_mission_ids:
                 if mission_id:
                     self.delete_mission(mission_id=mission_id, headers=headers)
             for map_id in to_delete_map_id:
-                self.delete_map(map_id, headers=headers)
+                self.delete_map(map_id, headers=headers)
```

### Comparing `cognicept-shell-1.7.1/cogniceptshell/rosbag_record.py` & `cognicept-shell-1.7.2/cogniceptshell/rosbag_record.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.7.1/setup.py` & `cognicept-shell-1.7.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 import ast
 
 from setuptools import setup, find_packages
 
 
 requires = ['python-dotenv>=0.13.0', 'boto3>=1.14.0', 'docker>=5.0.0',  'PyCryptodome >=3.9.8', 'argcomplete>=1.12.3', 'tabulate', 'ping3', 'docker-compose==1.29.2', 'PyJWT==1.7.1', 'websocket-client==0.59.0', 'paramiko>=2.4.2', 'psutil', 'ruamel.yaml']
 
-with open('README.md') as readme_file:
+with open("README.md") as readme_file:
     README = readme_file.read()
 
 setup(
-    name='cognicept-shell',
-    version='1.7.1',
-    description='Shell utility to configure Cognicept tools.',
+    name="cognicept-shell",
+    version="1.7.2",
+    description="Shell utility to configure Cognicept tools.",
     long_description_content_type="text/markdown",
     long_description=README,
-    author='Jakub Tomasek',
-    url='https://kabam.ai',
+    author="Jakub Tomasek",
+    url="https://kabam.ai",
     packages=find_packages(),
     install_requires=requires,
     license="Apache License 2.0",
-    entry_points = {
-        'console_scripts': ['cognicept=cogniceptshell.interface:main'],
+    entry_points={
+        "console_scripts": ["cognicept=cogniceptshell.interface:main"],
     },
     classifiers=(
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'Intended Audience :: System Administrators',
-        'Natural Language :: English',
-        'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.8'
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Intended Audience :: System Administrators",
+        "Natural Language :: English",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.8",
     ),
 )
```

### Comparing `cognicept-shell-1.7.1/tests/unit/mock_docker_client.py` & `cognicept-shell-1.7.2/tests/unit/mock_docker_client.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.7.1/tests/unit/test_config.py` & `cognicept-shell-1.7.2/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.7.1/tests/unit/test_get_robot_org_id.py` & `cognicept-shell-1.7.2/tests/unit/test_get_robot_org_id.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.7.1/tests/unit/test_keyrotate.py` & `cognicept-shell-1.7.2/tests/unit/test_keyrotate.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.7.1/tests/unit/test_lifecycle.py` & `cognicept-shell-1.7.2/tests/unit/test_lifecycle.py`

 * *Files 0% similar despite different names*

```diff
@@ -770,15 +770,15 @@
                 # Call the function
                 agent_lifecycle = AgentLifeCycle()
                 result = agent_lifecycle.get_version_tag_from_latest(image_data)
 
                 # Assert the result
                 assert result == expected_tag
                 mock_get_image_digest.assert_called_with(':'.join(image_data))
-                mock_client.assert_called_with('ecr')
+                mock_client.assert_called_with('ecr', region_name='ap-southeast-1')
                 mock_describe_images.assert_called_with(
                     registryId="412284733352",
                     repositoryName='repo1',
                     imageIds=[{"imageDigest": image_digest}]
                 )
 def test_get_version_tag_failure():
     image_data = ['412284733352.dkr.ecr.ap-southeast-1.amazonaws.com/repo1','latest']
@@ -792,15 +792,15 @@
             # Call the function
             agent_lifecycle = AgentLifeCycle()
             result = agent_lifecycle.get_version_tag_from_latest(image_data)
 
             # Assert the result is None
             assert result is None
             mock_get_image_digest.assert_called_with(':'.join(image_data))
-            mock_client.assert_called_with('ecr')
+            mock_client.assert_called_with('ecr', region_name='ap-southeast-1')
             # Since an exception is raised in the mocked client, no further calls will be made.
             mock_client.assert_called_once()
 
 def test_display_version(tmpdir, monkeypatch, capsys):
     args = type('', (), {})()
     args.path = str(tmpdir) + "/"
 
@@ -847,28 +847,32 @@
                 "--abort-on-container-exit": False,
                 "--remove-orphans": False,
                 "--force-recreate": False,
                 "--build": False,
                 "--no-build": True,
                 "--scale": ["camera_top=1"],
                 "--quiet-pull": True,
+                "--log-driver": "json-file",
+                "--log-opt": "max-size=5m"
                 })
     top_level_command_mock.up.assert_called_with({"--detach": True, 
                 "SERVICE": ["camera_top"],
                 "--no-deps": "",
                 "--no-color": True,
                 "--no-recreate": True,
                 "--always-recreate-deps": "",
                 "--abort-on-container-exit": False,
                 "--remove-orphans": False,
                 "--force-recreate": False,
                 "--build": False,
                 "--no-build": True,
                 "--scale": ["camera_top=1"],
                 "--quiet-pull": True,
+                "--log-driver": "json-file",
+                "--log-opt": "max-size=5m"
                 })    
 
 def test_clear_logs(tmpdir):
 
     def mock_check_sudo_password(cmd, capture_output, input, encoding):
         return True
```

### Comparing `cognicept-shell-1.7.1/tests/unit/test_move.py` & `cognicept-shell-1.7.2/tests/unit/test_move.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     robot_code = 'DoNotMove'
     robot_details = { "robot_name": "Test" }
     wrong_robot_id = '9d834f2a-5993-4a84-99b4-943d2b4cce22'
     wrong_robot_code = 'This_is_wrong'
 
     # map details
     map_ids = ['f2dae02a-8f73-460a-989d-2540598b3a1a']
-    map_image = 'iVBORw0KGgoAAAANSUhEUg'
+    map_image = 'iVBORw0KGgoAAAANSUhEUg=='
     map_details = {"map_image": "asdasd"}
     b64_encoded_map_image = b'\x89PNG\r\n\x1a\n\x00\x00\x00\rIHDR'
 
     waypoint_id = '2af2cbeb-7b50-40d1-8692-559eda719e74'
 
     # mission details
     mission_id = 'fe23e302-209d-4bf5-a669-6ecf441511cd'
```

### Comparing `cognicept-shell-1.7.1/tests/unit/test_populate_config_files.py` & `cognicept-shell-1.7.2/tests/unit/test_populate_config_files.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.7.1/tests/unit/test_pull_config_templates.py` & `cognicept-shell-1.7.2/tests/unit/test_pull_config_templates.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.7.1/tests/unit/test_update_event_log.py` & `cognicept-shell-1.7.2/tests/unit/test_update_event_log.py`

 * *Files identical despite different names*

### Comparing `cognicept-shell-1.7.1/tests/unit/test_version_update.py` & `cognicept-shell-1.7.2/tests/unit/test_version_update.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from unittest.mock import patch, MagicMock
 from cogniceptshell.agent_life_cycle import AgentLifeCycle as agent
 
 @pytest.fixture
 def mock_response():
     response = MagicMock()
-    response.json.return_value = {'info': {'version': '1.2.3'}}
+    response.json.return_value = {'info': {'version': '1.3.2'}}
     return response
 
 @pytest.fixture
 def mock_requests_get(mock_response):
     with patch('requests.get') as mock_get:
         mock_get.return_value = mock_response
         yield mock_get
@@ -20,26 +20,39 @@
         yield
 
 @pytest.fixture
 def mock_input_no():
     with patch('builtins.input', return_value='n'):
         yield
 
-def test_version_update_skip_true(mock_requests_get, mock_input_yes, capsys):
+@pytest.fixture
+def mock_pkg_resources():
+    mock_distribution = MagicMock()
+    mock_distribution.version = "1.0.2"
+    with patch('pkg_resources.require', return_value=[mock_distribution]):
+        yield
+
+@pytest.fixture
+def mock_os_system():
+    with patch('os.system', return_value=0):
+        # Set the return value of the mocked os.system to simulate success (0 exit code)
+        yield
+
+def test_version_update_skip_true(mock_pkg_resources, mock_requests_get, mock_os_system, mock_input_yes, capsys):
     args = MagicMock(skip=True)
     agent.cognicept_version_update(None, args)
     captured = capsys.readouterr()
     assert "cognicept-shell current version" in captured.out
-    assert "Installing Version 1.2.3" in captured.out
+    assert "Installing Version 1.3.2" in captured.out
 
-def test_version_update_skip_false_input_yes(mock_requests_get, mock_input_yes, capsys):
+def test_version_update_skip_false_input_yes(mock_pkg_resources, mock_requests_get, mock_os_system, mock_input_yes, capsys):
     args = MagicMock(skip=False)
     agent.cognicept_version_update(None, args)
     captured = capsys.readouterr()
     assert "cognicept-shell current version" in captured.out
-    assert "Installing Version 1.2.3" in captured.out
+    assert "Installing Version 1.3.2" in captured.out
 
-def test_version_update_skip_false_input_no(mock_requests_get, mock_input_no, capsys):
+def test_version_update_skip_false_input_no(mock_pkg_resources, mock_requests_get,mock_os_system, mock_input_no, capsys):
     args = MagicMock(skip=False)
     agent.cognicept_version_update(None, args)
     captured = capsys.readouterr()
     assert "cognicept-shell was not updated" in captured.out
```

