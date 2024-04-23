# Comparing `tmp/dockipy-0.0.6.tar.gz` & `tmp/dockipy-0.0.7.tar.gz`

## Comparing `dockipy-0.0.6.tar` & `dockipy-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 dockipy-0.0.6/requirements.txt
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 dockipy-0.0.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dockipy-0.0.6/src/dockipy/__about__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 dockipy-0.0.6/src/dockipy/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dockipy-0.0.6/src/dockipy/hello_world.py
--rw-r--r--   0        0        0    15502 2020-02-02 00:00:00.000000 dockipy-0.0.6/src/dockipy/main.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 dockipy-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dockipy-0.0.6/tests/init_test.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dockipy-0.0.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dockipy-0.0.6/LICENSE
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 dockipy-0.0.6/README.md
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 dockipy-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 dockipy-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 dockipy-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 dockipy-0.0.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dockipy-0.0.7/src/dockipy/__about__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 dockipy-0.0.7/src/dockipy/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dockipy-0.0.7/src/dockipy/hello_world.py
+-rw-r--r--   0        0        0    15404 2020-02-02 00:00:00.000000 dockipy-0.0.7/src/dockipy/main.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 dockipy-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dockipy-0.0.7/tests/init_test.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dockipy-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dockipy-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 dockipy-0.0.7/README.md
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 dockipy-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 dockipy-0.0.7/PKG-INFO
```

### Comparing `dockipy-0.0.6/.github/workflows/publish.yml` & `dockipy-0.0.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dockipy-0.0.6/src/dockipy/main.py` & `dockipy-0.0.7/src/dockipy/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,14 @@
 
 
         runtime = get_runtime(base_image)
         setup_venv(project_root, target_root, client, image, python_dep, docki_content, runtime, user, volumes)
        
         # Run a container from the image
         command = " ".join(command)
-        print(f"Running the command: {command}")
         container = client.containers.run(image, 
                                             f'{target_root}/venv/bin/python3 {command}',
                                             stdout=True,
                                             stderr=True,
                                             tty = True,
                                             # remove=True,
                                             shm_size=shm_size,
@@ -362,16 +361,15 @@
     password = docki_config.get("notebook_password", "docki")
     
     print(f"Building the Docker image based on {base_image}...")
     image, client = build_docker_image(base_image, system_dep, project_root, tag)
     command = f"{target_root}/venv/bin/jupyter notebook --no-browser --ServerApp.allow_origin='*' "+\
     f" --ServerApp.token='{token}'"+\
     f" --ServerApp.password='{password}'"+\
-    f" --ServerApp.root_dir='{work_dir}/'"+\
-    f" --ServerApp.runtime_dir ='{work_dir}/'"
+    f" --ServerApp.root_dir='{work_dir}/'"
 
     try:
         if platform.system() == "Linux":
             volumes = {project_root: {"bind": target_root, "mode": "rw"}, "mnt": {"bind": "/mnt", "mode": "rw"}}
             user = f"{os.getuid()}:{os.getgid()}"
         else:
             volumes = {project_root: {"bind": target_root, "mode": "rw"}}
```

### Comparing `dockipy-0.0.6/LICENSE` & `dockipy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dockipy-0.0.6/README.md` & `dockipy-0.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -93,12 +93,15 @@
     - python3-dev
     - python3-venv
 python_dep:
     file: ./requirements.txt
 notebook_token: docki
 notebook_password: docki
 ```
-
+## TODO
+- [ ] Add support Windows Notebooks
+- [ ] Add support Windows Shell
+- [ ] Add support for Docker GPU driver installation on WLS2
 
 ## License
 
 `dockipy` is like that cool friend who always lets you borrow their stuff without any fuss. It's distributed under the terms of the [apache-2.0](https://choosealicense.com/licenses/apache-2.0/) license. So go ahead, have some fun with it! 🎉
```

### Comparing `dockipy-0.0.6/pyproject.toml` & `dockipy-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dockipy-0.0.6/PKG-INFO` & `dockipy-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dockipy
-Version: 0.0.6
+Version: 0.0.7
 Project-URL: Documentation, https://github.com/Arty-Facts/dockipy#readme
 Project-URL: Issues, https://github.com/Arty-Facts/dockipy/issues
 Project-URL: Source, https://github.com/Arty-Facts/dockipy
 Author-email: Arturas Aleksandraus <arturas@aleksandraus.se>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -116,12 +116,15 @@
     - python3-dev
     - python3-venv
 python_dep:
     file: ./requirements.txt
 notebook_token: docki
 notebook_password: docki
 ```
-
+## TODO
+- [ ] Add support Windows Notebooks
+- [ ] Add support Windows Shell
+- [ ] Add support for Docker GPU driver installation on WLS2
 
 ## License
 
 `dockipy` is like that cool friend who always lets you borrow their stuff without any fuss. It's distributed under the terms of the [apache-2.0](https://choosealicense.com/licenses/apache-2.0/) license. So go ahead, have some fun with it! 🎉
```

