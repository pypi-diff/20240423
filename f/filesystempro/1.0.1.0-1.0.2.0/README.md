# Comparing `tmp/filesystempro-1.0.1.0.tar.gz` & `tmp/filesystempro-1.0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/filesystempro-1.0.1.0.tar", last modified: Mon Dec 11 18:29:33 2023, max compression
+gzip compressed data, was "dist/filesystempro-1.0.2.0.tar", last modified: Tue Apr 23 19:16:49 2024, max compression
```

## Comparing `filesystempro-1.0.1.0.tar` & `filesystempro-1.0.2.0.tar`

### file list

```diff
@@ -1,16 +1,34 @@
-drwxr-xr-x   0 heitor     (501) staff       (20)        0 2023-12-11 18:29:33.000000 filesystempro-1.0.1.0/
--rw-r--r--   0 heitor     (501) staff       (20)    26321 2023-12-11 18:29:33.000000 filesystempro-1.0.1.0/PKG-INFO
-drwxr-xr-x   0 heitor     (501) staff       (20)        0 2023-12-11 18:29:33.000000 filesystempro-1.0.1.0/filesystem/
-drwxr-xr-x   0 heitor     (501) staff       (20)        0 2023-12-11 18:29:33.000000 filesystempro-1.0.1.0/filesystem/watcher/
--rw-r--r--   0 heitor     (501) staff       (20)     2287 2023-11-20 06:48:36.000000 filesystempro-1.0.1.0/filesystem/watcher/__init__.py
-drwxr-xr-x   0 heitor     (501) staff       (20)        0 2023-12-11 18:29:33.000000 filesystempro-1.0.1.0/filesystem/wrapper/
--rw-r--r--   0 heitor     (501) staff       (20)    12044 2023-12-11 17:30:22.000000 filesystempro-1.0.1.0/filesystem/wrapper/__init__.py
--rw-r--r--   0 heitor     (501) staff       (20)     5573 2023-12-09 16:57:46.000000 filesystempro-1.0.1.0/filesystem/__init__.py
--rw-r--r--   0 heitor     (501) staff       (20)    20530 2023-12-11 18:18:20.000000 filesystempro-1.0.1.0/README.md
--rw-r--r--   0 heitor     (501) staff       (20)     1611 2023-12-11 18:29:24.000000 filesystempro-1.0.1.0/setup.py
-drwxr-xr-x   0 heitor     (501) staff       (20)        0 2023-12-11 18:29:33.000000 filesystempro-1.0.1.0/filesystempro.egg-info/
--rw-r--r--   0 heitor     (501) staff       (20)    26321 2023-12-11 18:29:33.000000 filesystempro-1.0.1.0/filesystempro.egg-info/PKG-INFO
--rw-r--r--   0 heitor     (501) staff       (20)      251 2023-12-11 18:29:33.000000 filesystempro-1.0.1.0/filesystempro.egg-info/SOURCES.txt
--rw-r--r--   0 heitor     (501) staff       (20)       49 2023-12-11 18:29:33.000000 filesystempro-1.0.1.0/filesystempro.egg-info/top_level.txt
--rw-r--r--   0 heitor     (501) staff       (20)        1 2023-12-11 18:29:33.000000 filesystempro-1.0.1.0/filesystempro.egg-info/dependency_links.txt
--rw-r--r--   0 heitor     (501) staff       (20)       38 2023-12-11 18:29:33.000000 filesystempro-1.0.1.0/setup.cfg
+drwxr-xr-x   0 heitor     (501) staff       (20)        0 2024-04-23 19:16:49.000000 filesystempro-1.0.2.0/
+-rw-r--r--   0 heitor     (501) staff       (20)    33689 2024-04-23 19:16:49.000000 filesystempro-1.0.2.0/PKG-INFO
+drwxr-xr-x   0 heitor     (501) staff       (20)        0 2024-04-23 19:16:48.000000 filesystempro-1.0.2.0/filesystem/
+drwxr-xr-x   0 heitor     (501) staff       (20)        0 2024-04-23 19:16:48.000000 filesystempro-1.0.2.0/filesystem/__core__/
+-rw-r--r--   0 heitor     (501) staff       (20)     1445 2024-04-22 03:58:02.000000 filesystempro-1.0.2.0/filesystem/__core__/__init__.py
+drwxr-xr-x   0 heitor     (501) staff       (20)        0 2024-04-23 19:16:48.000000 filesystempro-1.0.2.0/filesystem/watcher/
+-rw-r--r--   0 heitor     (501) staff       (20)     2287 2023-11-20 06:48:36.000000 filesystempro-1.0.2.0/filesystem/watcher/__init__.py
+drwxr-xr-x   0 heitor     (501) staff       (20)        0 2024-04-23 19:16:48.000000 filesystempro-1.0.2.0/filesystem/wrapper/
+-rw-r--r--   0 heitor     (501) staff       (20)    12049 2024-04-20 01:51:07.000000 filesystempro-1.0.2.0/filesystem/wrapper/__init__.py
+-rw-r--r--   0 heitor     (501) staff       (20)     5738 2024-04-20 05:17:04.000000 filesystempro-1.0.2.0/filesystem/__init__.py
+drwxr-xr-x   0 heitor     (501) staff       (20)        0 2024-04-23 19:16:48.000000 filesystempro-1.0.2.0/filesystem/console/
+drwxr-xr-x   0 heitor     (501) staff       (20)        0 2024-04-23 19:16:48.000000 filesystempro-1.0.2.0/filesystem/console/tests/
+-rw-rw-r--   0 heitor     (501) staff       (20)     1866 2024-04-20 01:38:31.000000 filesystempro-1.0.2.0/filesystem/console/tests/isatty_test.py
+-rw-rw-r--   0 heitor     (501) staff       (20)     6730 2024-04-20 01:38:31.000000 filesystempro-1.0.2.0/filesystem/console/tests/initialise_test.py
+-rw-rw-r--   0 heitor     (501) staff       (20)       75 2024-04-20 01:38:31.000000 filesystempro-1.0.2.0/filesystem/console/tests/__init__.py
+-rw-r--r--   0 heitor     (501) staff       (20)     2839 2024-04-22 02:44:36.000000 filesystempro-1.0.2.0/filesystem/console/tests/ansi_test.py
+-rw-rw-r--   0 heitor     (501) staff       (20)     1079 2024-04-20 01:38:31.000000 filesystempro-1.0.2.0/filesystem/console/tests/utils.py
+-rw-r--r--   0 heitor     (501) staff       (20)     3705 2024-04-22 02:44:42.000000 filesystempro-1.0.2.0/filesystem/console/tests/winterm_test.py
+-rw-rw-r--   0 heitor     (501) staff       (20)    10659 2024-04-20 01:38:31.000000 filesystempro-1.0.2.0/filesystem/console/tests/ansitowin32_test.py
+-rw-rw-r--   0 heitor     (501) staff       (20)      356 2024-04-21 21:12:28.000000 filesystempro-1.0.2.0/filesystem/console/__init__.py
+-rw-rw-r--   0 heitor     (501) staff       (20)     6181 2024-04-20 01:38:31.000000 filesystempro-1.0.2.0/filesystem/console/win32.py
+-rw-rw-r--   0 heitor     (501) staff       (20)    11128 2024-04-20 04:00:59.000000 filesystempro-1.0.2.0/filesystem/console/ansitowin32.py
+-rw-rw-r--   0 heitor     (501) staff       (20)     2534 2024-04-21 21:12:10.000000 filesystempro-1.0.2.0/filesystem/console/ansi.py
+-rw-rw-r--   0 heitor     (501) staff       (20)     7168 2024-04-20 01:38:31.000000 filesystempro-1.0.2.0/filesystem/console/winterm.py
+-rw-rw-r--   0 heitor     (501) staff       (20)     3324 2024-04-20 01:38:31.000000 filesystempro-1.0.2.0/filesystem/console/initialise.py
+-rw-r--r--   0 heitor     (501) staff       (20)    26328 2024-04-22 20:36:10.000000 filesystempro-1.0.2.0/README.md
+-rw-r--r--   0 heitor     (501) staff       (20)     1592 2024-04-22 04:17:34.000000 filesystempro-1.0.2.0/setup.py
+drwxr-xr-x   0 heitor     (501) staff       (20)        0 2024-04-23 19:16:48.000000 filesystempro-1.0.2.0/filesystempro.egg-info/
+-rw-r--r--   0 heitor     (501) staff       (20)    33689 2024-04-23 19:16:48.000000 filesystempro-1.0.2.0/filesystempro.egg-info/PKG-INFO
+-rw-r--r--   0 heitor     (501) staff       (20)      781 2024-04-23 19:16:48.000000 filesystempro-1.0.2.0/filesystempro.egg-info/SOURCES.txt
+-rw-r--r--   0 heitor     (501) staff       (20)        9 2024-04-23 19:16:48.000000 filesystempro-1.0.2.0/filesystempro.egg-info/requires.txt
+-rw-r--r--   0 heitor     (501) staff       (20)       11 2024-04-23 19:16:48.000000 filesystempro-1.0.2.0/filesystempro.egg-info/top_level.txt
+-rw-r--r--   0 heitor     (501) staff       (20)        1 2024-04-23 19:16:48.000000 filesystempro-1.0.2.0/filesystempro.egg-info/dependency_links.txt
+-rw-r--r--   0 heitor     (501) staff       (20)       38 2024-04-23 19:16:49.000000 filesystempro-1.0.2.0/setup.cfg
```

### Comparing `filesystempro-1.0.1.0/PKG-INFO` & `filesystempro-1.0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,595 +1,763 @@
-Metadata-Version: 2.1
-Name: filesystempro
-Version: 1.0.1.0
-Summary: FileSystem Pro is designed to identify the operating system (OS) on which it`s running and define the paths to various user directories based on the OS.
-Home-page: https://github.com/hbisneto/FileSystemPro
-Author: Heitor Bisneto
-Author-email: heitor.bardemaker@live.com
-License: MIT License
-Description: # FileSystem Pro 
-        
-        FileSystem Pro is designed to identify the operating system (OS) on which it’s running and define the paths to various user directories based on the OS.
-        
-        ## Getting Started
-        
-        #### Recommendation
-        
-        It's recommended Python 3.8 or later to use **FileSystem Pro**. You can download the latest version of Python in [python.org](https://www.python.org/).
-        
-        #### Installation
-        
-        Don't forget to upgrade pip:
-        
-        ```sh
-        pip install --upgrade pip
-        ```
-        
-        And install **FileSystem Pro:**
-        
-        ```sh
-        pip install filesystempro
-        ```
-        
-        You can also clone this repo to your local machine using:
-        
-        ```sh
-        git clone https://github.com/hbisneto/FileSystemPro.git
-        ```
-        
-        ---
-        
-        ## Features
-        - **Cross-platform Compatibility:** The code is designed to work on multiple operating systems, including Linux, Mac, and Windows. This makes it versatile and adaptable to different environments.
-        - **Directory Path Identification:** The code identifies and defines the paths to several common user directories based on the operating system. This includes directories like Desktop, Documents, Downloads, Music, Pictures, Public, Videos, and others.
-        - **Current Working Directory:** The code uses `os.getcwd()` to get the current working directory.
-        - **String Formatting:** The code uses f-string formatting to create directory paths.
-        - **Monitoring System:** Wrapper acts as a monitoring system for the file system. It keeps track of all activities within the file system.
-        - **Change Tracking:** It records any changes made within the file system. This includes the creation of new files, modification of existing files, and deletion of files.
-        - **Real-Time Updates:** The Wrapper provides real-time updates on any changes made within the file system. This ensures that users have the most current information at all times.
-        - **Integrity Maintenance:** This feature is particularly useful in scenarios where maintaining the integrity and up-to-date status of the file system is crucial. By tracking all changes, the Wrapper helps ensure that the file system remains accurate and reliable.
-        
-        ---
-        
-        ## FileSystem
-        
-        ```py
-        import filesystem as fs
-        ```
-        
-        <details>
-        <summary>fs.CURRENT_LOCATION</summary>
-        
-        > Creates a string that represents the path to the current directory. (Where the application is running)
-        
-        ```py
-        print(fs.CURRENT_LOCATION)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.OS_SEPARATOR</summary>
-        
-        > prints the OS separator 
-        <br>'`/`' for macOS and Linux
-        <br>'`\\`' for Windows
-        
-        ```py
-        print(fs.OS_SEPARATOR)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.USER_NAME</summary>
-        
-        > Creates a string that represents the username of the user currently logged in to the system.
-        
-        ```py
-        print(fs.USER_NAME)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.user</summary>
-        
-        > Creates a string that represents the path to the current user's home directory.
-        
-        ```py
-        print(fs.user)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.desktop</summary>
-        
-        > Creates a string that represents the path to the current user's Desktop folder.
-        
-        ```py
-        print(fs.desktop)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.documents</summary>
-        
-        > Creates a string that represents the path to the current user's Documents folder.
-        
-        ```py
-        print(fs.documents)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.downloads</summary>
-        
-        > Creates a string that represents the path to the current user's Downloads folder.
-        
-        ```py
-        print(fs.downloads)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.music</summary>
-        
-        > Creates a string that represents the path to the current user's Music folder.
-        
-        ```py
-        print(fs.music)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.pictures</summary>
-        
-        > Creates a string that represents the path to the current user's Pictures folder.
-        
-        ```py
-        print(fs.pictures)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.public</summary>
-        
-        > Creates a string that represents the path to the current user's Public folder.
-        
-        ```py
-        print(fs.public)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.videos</summary>
-        
-        > Creates a string that represents the path to the current user's Videos folder.
-        
-        ```py
-        print(fs.videos)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.linux_templates</summary>
-        
-        > Creates a string that represents the path to the current user's Templates folder in Linux environment.
-        
-        ```py
-        print(fs.linux_templates)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.mac_applications</summary>
-        
-        > Creates a string that represents the path to the current user's Applications folder in macOS environment.
-        
-        ```py
-        print(fs.mac_applications)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.windows_applicationData</summary>
-        
-        > Creates a string that represents the path to the current user's Roaming folder inside AppData in Windows environment.
-        
-        ```py
-        print(fs.windows_applicationData)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.windows_favorites</summary>
-        
-        > Creates a string that represents the path to the current user's Favorites folder in Windows environment.
-        
-        ```py
-        print(fs.windows_favorites)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.windows_localappdata</summary>
-        
-        > Creates a string that represents the path to the current user's Local folder inside AppData in Windows environment.
-        
-        ```py
-        print(fs.windows_localappdata)
-        ```
-        
-        </details>
-        
-        <details>
-        <summary>fs.windows_temp</summary>
-        
-        > Creates a string that represents the path to the current user's Temp folder inside LocalAppData in Windows environment.
-        
-        ```py
-        print(fs.windows_temp)
-        ```
-        
-        </details>
-        
-        ## Sample Codes
-        
-        <details>
-        <summary>FileSystem: Reaching Desktop Folder</summary>
-        
-        The following example shows how to get the `Desktop` directory path
-        
-        ```py
-        import filesystem as fs
-        
-        desk = fs.desktop
-        
-        print(desk)
-        ```
-        
-        Output:
-        
-        ```sh
-        ## On Linux
-        /home/YOU/Desktop
-        
-        ## On macOS
-        /Users/YOU/Desktop
-        
-        ## On Windows
-        C:\Users\YOU\Desktop
-        ```
-        </details>
-        
-        ---
-        
-        # Wrapper
-        
-        ```py
-        from filesystem import wrapper as wra
-        ```
-        
-        Wrapper is a comprehensive toolkit that provides a set of utility functions specifically designed to facilitate file and directory operations. These operations may include creating, reading, updating, and deleting files or directories.
-        
-        <details>
-        <summary>combine(*args, paths=[]):</summary>
-        
-        ```py
-        wra.combine(*args, paths=[]):
-        ```
-        
-        This function is designed to combine file or directory paths. It takes any number of arguments `*args` and an optional parameter paths which is a list of paths. The function returns a combined path based on the inputs.
-        <br>If the paths list is provided, the function uses it to combine paths. It starts with the first path in the list and checks if it’s an absolute path. If it’s not, it raises a `ValueError` with a detailed error message. Then, it iterates over the rest of the paths in the list. If a path is absolute, it replaces the current result with this path. If a path is relative, it joins this path to the current result. Finally, it returns the combined path.
-        <br> If the paths list is not provided or is empty, the function uses the arguments passed `*args`. It starts with the first argument and checks if it’s an absolute path. If it’s not, it raises a `ValueError` with a detailed error message. Then, it iterates over the rest of the arguments. If an argument is an absolute path, it replaces the current result with this path. If an argument is a relative path and not an empty string, it adds this path to the current result. If the current result doesn’t end with a separator (os.sep), it adds one before adding the path. Finally, it returns the combined path.
-        <br><br> **Please note**: This function does not check if the paths exist or are valid, it only combines them based on the rules described. It’s up to the caller to ensure that the paths are valid and exist if necessary.
-        >This method is intended to concatenate individual strings into a single string that represents a file path. However, if an argument other than the first contains a rooted path, any previous path components are ignored, and the returned string begins with that rooted path component. As an alternative to the `combine` method, consider using the `join` method.
-        </details>
-        
-        <details>
-        <summary>create_directory(path, create_subdirs=True)</summary>
-        
-        ```py
-        wra.create_directory(path, create_subdirs=True)
-        ```
-        
-        This function is used to create a directory at the specified `path`. If `create_subdirs` is `True`, the function creates all intermediate-level directories needed to contain the leaf directory. If `create_subdirs` is `False`, the function will raise an error if the directory already exists or if any intermediate-level directories in the path do not exist. Default is **`True`**
-        <br>If the directories already exist, it does nothing.
-        </details>
-        
-        <details>
-        <summary>create_file(file_name, path, text, encoding="utf-8-sig"):</summary>
-        
-        ```py
-        wra.create_file(file_name, path, text, encoding="utf-8-sig")
-        ```
-        
-        The function attempts to open a file at the specified `path` with the given `file_name` (with extension), in write mode with the specified `encoding`. It then writes the provided `text` into the file.
-        </details>
-        
-        <details>
-        <summary>delete(path, recursive=False)</summary>
-        
-        ```py
-        wra.delete(path, recursive=False)
-        ```
-        
-        This function is designed to delete a directory at a given `path`.
-        <br>If `recursive` is set to `True`, the function will delete the directory and all its contents. If it’s `False`, the function will only delete the directory if it’s empty. Default is **`False`**.
-        </details>
-        
-        <details>
-        <summary>enumerate_files(path)</summary>
-        
-        ```py
-        wra.enumerate_files(path)
-        ```
-        
-        This function performs a depth-first traversal of the directory tree at the given path (after expanding any user home directory symbols). It returns a list of dictionaries containing the attributes of each file and directory in the tree.
-        </details>
-        
-        <details>
-        <summary>get_files(path):</summary>
-        
-        ```py
-        wra.get_files(path)
-        ```
-        
-        This function takes a path as input (which can include wildcards), expands any user home directory symbols (`~`), and returns a list of dictionaries containing the attributes of each file or directory that matches the path.
-        </details>
-        
-        <details>
-        <summary>get_object(path):</summary>
-        
-        ```py
-        wra.get_object(path)
-        ```
-        
-        This function takes a file or directory path as input and returns a dictionary containing various attributes of the file or directory. These attributes include the time of last modification, creation time, last access time, name, size, absolute path, parent directory, whether it's a directory or file or link, whether it exists, and its extension (if it's a file).
-        </details>
-        
-        <details>
-        <summary>join(path1='', path2='', path3='', path4='', paths=[]):</summary>
-        
-        ```py
-        wra.join(path1='', path2='', path3='', path4='', paths=[])
-        ```
-        
-        This function is designed to concatenate directory paths. It takes four optional string parameters `path1`, `path2`, `path3`, `path4` and an optional list of paths `paths`. The function returns a single string that represents the concatenated path.
-        <br> For each of the parameters `path1`, `path2`, `path3`, and `path4`, the function checks if the path ends with a separator. If it doesn’t, and the path is not an empty string, it adds a separator to the end of the path.
-        <br>If the paths list is provided and is not empty, the function iterates over each item in the list. For each item, it checks if the item ends with a separator. If it doesn’t, it adds a separator to the end of the item.
-        <br>Finally, the function returns the concatenated path.
-        <br><br> **Please note**: This function does not check if the paths exist or are valid, it only combines them based on the rules described. It’s up to the caller to ensure that the paths are valid and exist if necessary.
-        > Unlike the `combine` method, the `join` method does not attempt to root the returned path. (That is, if `path2` or `path3` or `path4` is an absolute path, the `join` method does not discard the previous paths as the `combine` method does.)
-        </details>
-        
-        <details>
-        <summary>list_directories(path):</summary>
-        
-        ```py
-        wra.list_directories(path)
-        ```
-        
-        This function returns a list of all the directories in a given directory.
-        </details>
-        
-        <details>
-        <summary>list_files(path):</summary>
-        
-        ```py
-        wra.list_files(path)
-        ```
-        
-        This function returns a list of all the files in a given directory.
-        </details>
-        
-        <details>
-        <summary>make_zip(source, destination):</summary>
-        
-        ```py
-        wra.make_zip(source, destination)
-        ```
-        
-        This function is used to create a zip archive of a given source directory and move it to a specified destination.
-        </details>
-        
-        ## Sample Codes
-        
-        <details>
-        <summary>Wrapper: Creating a Folder</summary>
-        
-        The following example shows how to create a new directory named `database` inside the `Documents` directory using **Wrapper**
-        
-        ```py
-        import filesystem as fs
-        from filesystem import wrapper as wra
-        
-        bd_folder = "database"
-        try:
-           wra.create_directory(f'{fs.documents}/{bd_folder}')
-        except:
-           print("Could`t create the folder")
-        ```
-        </details>
-        
-        <details>
-        <summary>Wrapper: Get Files</summary>
-        
-        1. **Get Files:**
-        
-        The following example shows how to get files information from **Downloads** folder.
-        
-        ```py
-        import filesystem as fs
-        from filesystem import wrapper as wra
-        
-        pointers = wra.get_files(f'{fs.downloads}/*')
-        print(pointers)
-        ```
-        
-        Output:
-        
-        ```py
-        [{'modified': 1695535334.1411633, 'created': 1697604128.7045012, 'access': 1697604129.781534, 'name': 'CLI.py', 'size': 3345, 'abspath': '/Users/YOU/Downloads/CLI.py', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'py'}, {'modified': 1697605101.6574, 'created': 1697683292.4821024, 'access': 1697683294.46923, 'name': 'Python_Logo.png', 'size': 747809, 'abspath': '/Users/YOU/Downloads/Python_Logo.png', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'png'}, {'modified': 1697681746.0940206, 'created': 1697682027.268841, 'access': 1697682292.5433743, 'name': 'Sample_File.py', 'size': 1031, 'abspath': '/Users/YOU/Downloads/Sample_File.py', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'py'}]
-        ```
-        
-        #
-        
-        2. **Filter Files by Extension:**
-        
-        The following example is using a list comprehension to filter out files with extension `.py` from the pointers list:
-        
-        ```py
-        py_files = [x for x in pointers if x["extension"] == "py"]
-        print(py_files)
-        ```
-        
-        ```py
-        [{'modified': 1695535334.1411633, 'created': 1697604128.7045012, 'access': 1697604129.781534, 'name': 'CLI.py', 'size': 3345, 'abspath': '/Users/YOU/Downloads/CLI.py', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'py'}, {'modified': 1697681746.0940206, 'created': 1697682027.268841, 'access': 1697681829.0075543, 'name': 'Sample_File.py', 'size': 1031, 'abspath': '/Users/YOU/Downloads/Sample_File.py', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'py'}]
-        ```
-        
-        #
-        
-        3. **Get File Names Inside the Filter:**
-        The following code is using a list comprehension that prints the names of all filtered files in the `py_files` list:
-        
-        ```py
-        print([x["name"] for x in py_files])
-        ```
-        
-        Output:
-        
-        ```sh
-        ['CLI.py', 'Sample_File.py']
-        ```
-        </details>
-        
-        <details>
-        <summary>Wrapper: Enumerate files (walk recursively) from a directory</summary>
-        
-        The following code is using a list comprehension to generate a list of all files in the **Downloads** directory:
-        
-        ```py
-        tree = [x for x in wra.enumerate_files(fs.downloads)]
-        print(tree)
-        ```
-        
-        Output:
-        
-        ```py
-        [{'modified': 1697683292.4821026, 'created': 1697683292.4821026, 'access': 1697683292.484029, 'name': 'Downloads', 'size': 224, 'abspath': '/Users/YOU/Downloads', 'dirname': '/Users/YOU', 'is_dir': True, 'is_file': False, 'is_link': False, 'exists': True, 'extension': ''}, {'modified': 1697683288.8639557, 'created': 1697683288.8639557, 'access': 1697602943.1846778, 'name': '.DS_Store', 'size': 6148, 'abspath': '/Users/YOU/Downloads/.DS_Store', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'DS_Store'}, {'modified': 1690685751.342114, 'created': 1690685751.4194765, 'access': 1690685751.342114, 'name': '.localized', 'size': 0, 'abspath': '/Users/YOU/Downloads/.localized', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'localized'}, {'modified': 1695535334.1411633, 'created': 1697604128.7045012, 'access': 1697604129.781534, 'name': 'CLI.py', 'size': 3345, 'abspath': '/Users/YOU/Downloads/CLI.py', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'py'}, {'modified': 1697605101.6574, 'created': 1697683292.4821024, 'access': 1697683294.46923, 'name': 'Python_Logo.png', 'size': 747809, 'abspath': '/Users/YOU/Downloads/Python_Logo.png', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'png'}, {'modified': 1697681746.0940206, 'created': 1697682027.268841, 'access': 1697682292.5433743, 'name': 'Sample_File.py', 'size': 1031, 'abspath': '/Users/YOU/Downloads/Sample_File.py', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'py'}]
-        ```
-        </details>
-        
-        ---
-        
-        # Watcher
-        
-        ```py
-        from filesystem import watcher as wat
-        ```
-        
-        Watcher serves as a monitoring system for the file system. It keeps track of any changes made within the file system, such as the creation of new files, modification of existing files, or deletion of files. This feature allows for real-time updates and can be particularly useful in scenarios where maintaining the integrity and up-to-date status of the file system is crucial.
-        
-        <details>
-        <summary>__init__(self, root):</summary>
-        
-        This is the constructor method that initializes the `Watcher` object with a root directory to watch. It also saves the current state of the file system in `self.saved_state`.
-        </details>
-        <details>
-        <summary>get_state(self, path):</summary>
-        
-        This method returns a dictionary where the keys are the absolute paths of all files in the given path and the values are file metadata obtained from the `wrapper.enumerate_files(path)` function.
-        </details>
-        <details>
-        <summary>diff(self):</summary>
-        
-        This method compares the current state of the file system with the saved state and identifies any changes (created, updated, or removed files). It returns a list of dictionaries where each dictionary contains the metadata of a changed file and an additional key "change" indicating the type of change.
-        </details>
-        <details>
-        <summary>__str__(self):</summary>
-        
-        This method returns a string representation of the `Watcher` object.
-        </details>
-        
-        <!-- <details>
-        <summary>List Of Functions </summary>
-        
-        Watcher is used to monitor changes in a file system.
-        
-        - `__init__(self, root)`: This is the constructor method that initializes the `Watcher` object with a root directory to watch. It also saves the current state of the file system in `self.saved_state`.
-        
-        - `get_state(self, path)`: This method returns a dictionary where the keys are the absolute paths of all files in the given path and the values are file metadata obtained from the `core.enumerate_files(path)` function.
-        
-        - `diff(self)`: This method compares the current state of the file system with the saved state and identifies any changes (created, updated, or removed files). It returns a list of dictionaries where each dictionary contains the metadata of a changed file and an additional key "change" indicating the type of change.
-        
-        - `__str__(self)`: This method returns a string representation of the `Watcher` object.
-        </details> -->
-        
-        This class could be useful in scenarios where you need to monitor changes to a file system, for example, in a backup system or a live syncing service.
-        
-        ## Sample Codes
-        
-        <details>
-        <summary>Watcher: Monitoring Documents Folder</summary>
-        
-        This Watcher example is designed to monitor changes in **Documents** directory and print out the changes as they occur.
-        
-        ```py
-        # Native library
-        import time
-        from datetime import datetime
-        
-        # FileSystemPro
-        import filesystem as fs
-        from filesystem import watcher as wat
-        
-        # Create a new instance of Watcher class
-        watcher = wat.Watcher(f'{fs.documents}')
-        
-        # Run `diff` method to get directory changes
-        while True:
-            changes = watcher.diff()
-            if changes:
-                print(f"Changes detected at: {datetime.now()}:")
-                for change in changes:
-                    print(f"{change['abspath']} was {change['change']}")
-            time.sleep(5)  # Awaits for 5 seconds before a new verification
-        ```
-        
-        </details>
-        
-        ---
-        
-        Copyright © 2023 Bisneto Inc. All rights reserved.
-Keywords: FileSystem,Linux,macOS,Windows,File,System
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Software Development :: Libraries
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+# FileSystem Pro 
+
+FileSystem Pro is designed to identify the operating system (OS) on which it’s running and define the paths to various user directories based on the OS.
+
+## Getting Started
+
+#### Recommendation
+
+It's recommended Python 3.8 or later to use **FileSystem Pro**. You can download the latest version of Python in [python.org](https://www.python.org/).
+
+#### Installation
+
+Don't forget to upgrade pip:
+
+```sh
+pip install --upgrade pip
+```
+
+And install **FileSystem Pro:**
+
+```sh
+pip install filesystempro
+```
+
+---
+
+#### To Developers / Contributors
+
+Clone this repository to your local machine using:
+
+```sh
+git clone https://github.com/hbisneto/FileSystemPro.git
+```
+
+Install setuptools
+
+```sh
+pip install setuptools
+```
+
+Upgrade setuptools
+
+```sh
+pip install --upgrade setuptools
+```
+> Note: FileSystem Pro requires setuptools 69.5.1 or later.
+><br> Python environment typically targets setuptools version 49.x.
+
+Install wheel
+
+```sh
+pip install wheel
+```
+
+Upgrade wheel
+
+```sh
+pip install --upgrade wheel
+```
+
+---
+
+## Features
+- **Cross-platform Compatibility:** The code is designed to work on multiple operating systems, including Linux, Mac, and Windows. This makes it versatile and adaptable to different environments.
+- **Directory Path Identification:** The code identifies and defines the paths to several common user directories based on the operating system. This includes directories like Desktop, Documents, Downloads, Music, Pictures, Public, Videos, and others.
+- **Current Working Directory:** The code uses `os.getcwd()` to get the current working directory.
+- **String Formatting:** The code uses f-string formatting to create directory paths.
+- **Monitoring System:** Watcher acts as a monitoring system for the file system. It keeps track of all activities within the file system.
+- **Change Tracking:** It records any changes made within the file system. This includes the creation of new files, modification of existing files, and deletion of files.
+- **Real-Time Updates:** The Watcher provides real-time updates on any changes made within the file system. This ensures that users have the most current information at all times.
+- **Integrity Maintenance:** This feature is particularly useful in scenarios where maintaining the integrity and up-to-date status of the file system is crucial. By tracking all changes, the Watcher helps ensure that the file system remains accurate and reliable.
+
+---
+
+## FileSystem
+
+```py
+import filesystem as fs
+```
+<table>
+  <tr>
+    <th>Method</th>
+    <th>Description</th>
+    <!-- <th>Code Sample</th> -->
+  </tr>
+  
+  <tr>
+    <td>
+    	CURRENT_LOCATION
+    </td>
+    <td>
+	    Creates a string that represents the path to the current directory. (Where the application is running)
+    </td>
+    <!-- <td>
+	    print(fs.CURRENT_LOCATION)
+    </td> -->
+  </tr>
+  
+  <tr>
+    <td>
+    	OS_SEPARATOR
+    </td>
+    <td>
+	    prints the OS separator
+		<br>'/' for macOS and Linux 
+		<br>'\\' for Windows
+    </td>
+    <!-- <td>
+	    print(fs.OS_SEPARATOR)
+    </td> -->
+  </tr>
+
+  <tr>
+    <td>
+    	USER_NAME
+    </td>
+    <td>
+	    Creates a string that represents the username of the user currently logged in to the system.
+    </td>
+    <!-- <td>
+	    print(fs.USER_NAME)
+    </td> -->
+  </tr>
+  
+  <tr>
+    <td>
+    	user
+    </td>
+    <td>
+	    Creates a string that represents the path to the current user's home directory.
+    </td>
+    <!-- <td>
+	    print(fs.user)
+    </td> -->
+  </tr>
+
+  <tr>
+    <td>
+    	desktop
+    </td>
+    <td>
+	    Creates a string that represents the path to the current user's Desktop folder.
+    </td>
+    <!-- <td>
+	    print(fs.desktop)
+    </td> -->
+  </tr>
+  
+  <tr>
+    <td>
+    	documents
+    </td>
+    <td>
+	    Creates a string that represents the path to the current user's Documents folder.
+    </td>
+    <!-- <td>
+	    print(fs.documents)
+    </td> -->
+  </tr>
+
+  <tr>
+    <td>
+    	downloads
+    </td>
+    <td>
+	    Creates a string that represents the path to the current user's Downloads folder.
+    </td>
+    <!-- <td>
+	    print(fs.downloads)
+    </td> -->
+  </tr>
+  
+  <tr>
+    <td>
+    	music
+    </td>
+    <td>
+	    Creates a string that represents the path to the current user's Music folder.
+    </td>
+    <!-- <td>
+	    print(fs.music)
+    </td> -->
+  </tr>
+
+  <tr>
+    <td>
+    	pictures
+    </td>
+    <td>
+	    Creates a string that represents the path to the current user's Pictures folder.
+    </td>
+    <!-- <td>
+	    print(fs.pictures)
+    </td> -->
+  </tr>
+  
+  <tr>
+    <td>
+    	public
+    </td>
+    <td>
+	    Creates a string that represents the path to the current user's Public folder.
+    </td>
+    <!-- <td>
+	    print(fs.public)
+    </td> -->
+  </tr>
+
+  <tr>
+    <td>
+    	videos
+    </td>
+    <td>
+	    Creates a string that represents the path to the current user's Videos folder.
+    </td>
+    <!-- <td>
+	    print(fs.videos)
+    </td> -->
+  </tr>
+  
+  <tr>
+    <td>
+    	linux_templates
+    </td>
+    <td>
+	    Creates a string that represents the path to the current user's Templates folder in Linux environment.
+    </td>
+    <!-- <td>
+	    print(fs.linux_templates)
+    </td> -->
+  </tr>
+
+  <tr>
+    <td>
+    	mac_applications
+    </td>
+    <td>
+	    Creates a string that represents the path to the current user's Applications folder in macOS environment.
+    </td>
+    <!-- <td>
+	    print(fs.mac_applications)
+    </td> -->
+  </tr>
+  
+  <tr>
+    <td>
+    	windows_applicationData
+    </td>
+    <td>
+	    Creates a string that represents the path to the current user's Roaming folder inside AppData in Windows environment.
+    </td>
+    <!-- <td>
+	    print(fs.windows_applicationData)
+    </td> -->
+  </tr>
+
+  <tr>
+    <td>
+    	windows_favorites
+    </td>
+    <td>
+	    Creates a string that represents the path to the current user's Favorites folder in Windows environment.
+    </td>
+    <!-- <td>
+	    print(fs.windows_favorites)
+    </td> -->
+  </tr>
+  
+  <tr>
+    <td>
+    	windows_localappdata
+    </td>
+    <td>
+	    Creates a string that represents the path to the current user's Local folder inside AppData in Windows environment.
+    </td>
+    <!-- <td>
+	    print(fs.windows_localappdata)
+    </td> -->
+  </tr>
+
+  <tr>
+    <td>
+    	windows_temp
+    </td>
+    <td>
+	    Creates a string that represents the path to the current user's Temp folder inside LocalAppData in Windows environment.
+    </td>
+    <!-- <td>
+	    print(fs.windows_temp)
+    </td> -->
+  </tr>
+
+</table>
+
+## Sample Codes
+
+<details>
+<summary>FileSystem: Reaching Desktop Folder</summary>
+
+The following example shows how to get the `Desktop` directory path
+
+```py
+import filesystem as fs
+
+desk = fs.desktop
+
+print(desk)
+```
+
+Output:
+
+```sh
+## On Linux
+/home/YOU/Desktop
+
+## On macOS
+/Users/YOU/Desktop
+
+## On Windows
+C:\Users\YOU\Desktop
+```
+</details>
+
+---
+
+# Wrapper
+
+```py
+from filesystem import wrapper as wra
+```
+
+Wrapper is a comprehensive toolkit that provides a set of utility functions specifically designed to facilitate file and directory operations. These operations may include creating, reading, updating, and deleting files or directories.
+
+<table>
+  <tr>
+    <th>Method</th>
+    <th>Description</th>
+  </tr>
+
+  <tr>
+    <td>combine(*args, paths=[])</td>
+    <td>
+      This function is designed to combine file or directory paths. It takes any number of arguments *args and an optional parameter paths which is a list of paths. The function returns a combined path based on the inputs.
+      If the paths list is provided, the function uses it to combine paths. It starts with the first path in the list and checks if it’s an absolute path. If it’s not, it raises a ValueError with a detailed error message. Then, it iterates over the rest of the paths in the list. If a path is absolute, it replaces the current result with this path. If a path is relative, it joins this path to the current result. Finally, it returns the combined path.
+      If the paths list is not provided or is empty, the function uses the arguments passed *args. It starts with the first argument and checks if it’s an absolute path. If it’s not, it raises a ValueError with a detailed error message. Then, it iterates over the rest of the arguments. If an argument is an absolute path, it replaces the current result with this path. If an argument is a relative path and not an empty string, it adds this path to the current result. If the current result doesn’t end with a separator (os.sep), it adds one before adding the path. Finally, it returns the combined path.
+      <br><br><strong>Please note:</strong> This function does not check if the paths exist or are valid, it only combines them based on the rules described. It’s up to the caller to ensure that the paths are valid and exist if necessary.
+      <br><br>This method is intended to concatenate individual strings into a single string that represents a file path. However, if an argument other than the first contains a rooted path, any previous path components are ignored, and the returned string begins with that rooted path component. As an alternative to the combine method, consider using the join method.
+    </td>
+  </tr>
+
+
+  <tr>
+    <td>
+      create_directory(path, create_subdirs=True)
+    </td>
+    <td>
+      This function is used to create a directory at the specified <strong>path</strong>. If <strong>create_subdirs</strong> is <strong>True</strong>, the function creates all intermediate-level directories needed to contain the leaf directory. If <strong>create_subdirs</strong> is <strong>False</strong>, the function will raise an error if the directory already exists or if any intermediate-level directories in the path do not exist. 
+      <br>Default is <strong>True</strong>
+      <br>If the directories already exist, it does nothing.
+    </td>
+  </tr>
+
+  <tr>
+    <td>
+      create_file(file_name, path, text, encoding="utf-8-sig")
+    </td>
+    <td>
+      The function attempts to open a file at the specified <strong>path</strong> with the given <strong>file_name</strong> (with extension), in write mode with the specified <strong>encoding</strong>. It then writes the provided <strong>text</strong> into the file.
+      <br>Finally, it calls Wrapper <strong>get_object</strong> with the full path to the newly created file and returns the resulting dictionary.
+    </td>
+  </tr>
+
+  <tr>
+    <td>
+      delete(path, recursive=False)
+    </td>
+    <td>
+      This function is designed to delete a directory at a given <strong>path</strong>.
+      If <strong>recursive</strong> is set to <strong>True</strong>, the function will delete the directory and all its contents. If it’s <strong>False</strong>, the function will only delete the directory if it’s empty. Default is <strong>False</strong>.
+    </td>
+  </tr>
+
+  <tr>
+    <td>
+      enumerate_files(path)
+    </td>
+    <td>
+      This function performs a depth-first traversal of the directory tree at the given path (after expanding any user home directory symbols). It returns a list of dictionaries containing the attributes of each file and directory in the tree.
+    </td>
+  </tr>
+
+  <tr>
+    <td>
+      get_files(path)
+    </td>
+    <td>
+      This function takes a path as input (which can include wildcards), expands any user home directory symbols (~), and returns a list of dictionaries containing the attributes of each file or directory that matches the path.
+    </td>
+  </tr>
+
+  <tr>
+    <td>
+      get_object(path)
+    </td>
+    <td>
+      This function takes a file or directory path as input and returns a dictionary containing various attributes of the file or directory. These attributes include the time of last modification, creation time, last access time, name, size, absolute path, parent directory, whether it's a directory or file or link, whether it exists, and its extension (if it's a file).
+    </td>
+  </tr>
+
+  <tr>
+    <td>
+      join(path1='', path2='', path3='', path4='', paths=[])
+    </td>
+    <td>
+      This function is designed to concatenate directory paths. It takes four optional string parameters <strong>path1</strong>, <strong>path2</strong>, <strong>path3</strong>, <strong>path4</strong> and an optional list of paths paths. The function returns a single string that represents the concatenated path.
+      <br>For each of the parameters <strong>path1</strong>, <strong>path2</strong>, <strong>path3</strong> and <strong>path4</strong>, the function checks if the path ends with a separator. If it doesn’t, and the path is not an empty string, it adds a separator to the end of the path.
+      If the paths list is provided and is not empty, the function iterates over each item in the list. For each item, it checks if the item ends with a separator. If it doesn’t, it adds a separator to the end of the item.
+      Finally, the function returns the concatenated path.
+      <br><br><strong>Please note:</strong> This function does not check if the paths exist or are valid, it only combines them based on the rules described. It’s up to the caller to ensure that the paths are valid and exist if necessary.
+      <br><br>Unlike the <strong>combine</strong> method, the <strong>join</strong> method does not attempt to root the returned path. (That is, if <strong>path2</strong> or <strong>path3</strong> or <strong>path4</strong> is an absolute path, the <strong>join</strong> method does not discard the previous paths as the <strong>combine</strong> method does).
+    </td>
+  </tr>
+
+  <tr>
+    <td>
+      list_directories(path)
+    </td>
+    <td>
+      This function returns a list of all the directories in a given directory.
+    </td>
+  </tr>
+
+  <tr>
+    <td>
+      list_files(path)
+    </td>
+    <td>
+      This function returns a list of all the files in a given directory.
+    </td>
+  </tr>
+
+  <tr>
+    <td>
+      make_zip(source, destination)
+    </td>
+    <td>
+      This function is used to create a zip archive of a given source directory and move it to a specified destination.
+    </td>
+  </tr>
+
+</table>
+
+## Sample Codes
+
+<details>
+<summary>Wrapper: Creating a Folder</summary>
+
+The following example shows how to create a new directory named `database` inside the `Documents` directory using **Wrapper**
+
+```py
+import filesystem as fs
+from filesystem import wrapper as wra
+
+bd_folder = "database"
+try:
+   wra.create_directory(f'{fs.documents}/{bd_folder}')
+except:
+   print("Could`t create the folder")
+```
+</details>
+
+<details>
+<summary>Wrapper: Get Files</summary>
+
+1. **Get Files:**
+
+The following example shows how to get files information from **Downloads** folder.
+
+```py
+import filesystem as fs
+from filesystem import wrapper as wra
+
+pointers = wra.get_files(f'{fs.downloads}/*')
+print(pointers)
+```
+
+Output:
+
+```sh
+[{'modified': 1695535334.1411633, 'created': 1697604128.7045012, 'access': 1697604129.781534, 'name': 'CLI.py', 'size': 3345, 'abspath': '/Users/YOU/Downloads/CLI.py', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'py'}, {'modified': 1697605101.6574, 'created': 1697683292.4821024, 'access': 1697683294.46923, 'name': 'Python_Logo.png', 'size': 747809, 'abspath': '/Users/YOU/Downloads/Python_Logo.png', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'png'}, {'modified': 1697681746.0940206, 'created': 1697682027.268841, 'access': 1697682292.5433743, 'name': 'Sample_File.py', 'size': 1031, 'abspath': '/Users/YOU/Downloads/Sample_File.py', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'py'}]
+```
+
+#
+
+2. **Filter Files by Extension:**
+
+The following example is using a list comprehension to filter out files with extension `.py` from the pointers list:
+
+```py
+py_files = [x for x in pointers if x["extension"] == "py"]
+print(py_files)
+```
+
+```sh
+[{'modified': 1695535334.1411633, 'created': 1697604128.7045012, 'access': 1697604129.781534, 'name': 'CLI.py', 'size': 3345, 'abspath': '/Users/YOU/Downloads/CLI.py', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'py'}, {'modified': 1697681746.0940206, 'created': 1697682027.268841, 'access': 1697681829.0075543, 'name': 'Sample_File.py', 'size': 1031, 'abspath': '/Users/YOU/Downloads/Sample_File.py', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'py'}]
+```
+
+#
+
+3. **Get File Names Inside the Filter:**
+The following code is using a list comprehension that prints the names of all filtered files in the `py_files` list:
+
+```py
+print([x["name"] for x in py_files])
+```
+
+Output:
+
+```sh
+['CLI.py', 'Sample_File.py']
+```
+</details>
+
+<details>
+<summary>Wrapper: Enumerate files (walk recursively) from a directory</summary>
+
+The following code is using a list comprehension to generate a list of all files in the **Downloads** directory:
+
+```py
+tree = [x for x in wra.enumerate_files(fs.downloads)]
+print(tree)
+```
+
+Output:
+
+```sh
+[{'modified': 1697683292.4821026, 'created': 1697683292.4821026, 'access': 1697683292.484029, 'name': 'Downloads', 'size': 224, 'abspath': '/Users/YOU/Downloads', 'dirname': '/Users/YOU', 'is_dir': True, 'is_file': False, 'is_link': False, 'exists': True, 'extension': ''}, {'modified': 1697683288.8639557, 'created': 1697683288.8639557, 'access': 1697602943.1846778, 'name': '.DS_Store', 'size': 6148, 'abspath': '/Users/YOU/Downloads/.DS_Store', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'DS_Store'}, {'modified': 1690685751.342114, 'created': 1690685751.4194765, 'access': 1690685751.342114, 'name': '.localized', 'size': 0, 'abspath': '/Users/YOU/Downloads/.localized', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'localized'}, {'modified': 1695535334.1411633, 'created': 1697604128.7045012, 'access': 1697604129.781534, 'name': 'CLI.py', 'size': 3345, 'abspath': '/Users/YOU/Downloads/CLI.py', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'py'}, {'modified': 1697605101.6574, 'created': 1697683292.4821024, 'access': 1697683294.46923, 'name': 'Python_Logo.png', 'size': 747809, 'abspath': '/Users/YOU/Downloads/Python_Logo.png', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'png'}, {'modified': 1697681746.0940206, 'created': 1697682027.268841, 'access': 1697682292.5433743, 'name': 'Sample_File.py', 'size': 1031, 'abspath': '/Users/YOU/Downloads/Sample_File.py', 'dirname': '/Users/YOU/Downloads', 'is_dir': False, 'is_file': True, 'is_link': False, 'exists': True, 'extension': 'py'}]
+```
+</details>
+
+---
+
+# Watcher
+
+```py
+from filesystem import watcher as wat
+```
+
+Watcher serves as a monitoring system for the file system. It keeps track of any changes made within the file system, such as the creation of new files, modification of existing files, or deletion of files. This feature allows for real-time updates and can be particularly useful in scenarios where maintaining the integrity and up-to-date status of the file system is crucial.
+
+<table>
+  <tr>
+    <th>Method</th>
+    <th>Description</th>
+  </tr>
+
+  <tr>
+    <td>init(self, root)</td>
+    <td>
+      This is the constructor method that initializes the Watcher object with a root directory to watch. It also saves the current state of the file system in <strong>self.saved_state</strong>.
+    </td>
+  </tr>
+
+  <tr>
+    <td>get_state(self, path):</td>
+    <td>
+      This method returns a dictionary where the keys are the absolute paths of all files in the given path and the values are file metadata obtained from the <strong>wrapper.enumerate_files(path)</strong> function.
+    </td>
+  </tr>
+
+  <tr>
+    <td>diff(self)</td>
+    <td>
+      This method compares the current state of the file system with the saved state and identifies any changes (created, updated, or removed files). It returns a list of dictionaries where each dictionary contains the metadata of a changed file and an additional key "change" indicating the type of change.
+    </td>
+  </tr>
+
+  <tr>
+    <td>str(self)</td>
+    <td>
+      This method returns a string representation of the <strong>Watcher</strong> object.
+    </td>
+  </tr>
+  
+</table>
+
+This class could be useful in scenarios where you need to monitor changes to a file system, for example, in a backup system or a live syncing service.
+
+## Sample Codes
+
+<details>
+<summary>Watcher: Monitoring Documents Folder</summary>
+
+This Watcher example is designed to monitor changes in **Documents** directory and print out the changes as they occur.
+
+```py
+# Native library
+import time
+from datetime import datetime
+
+# FileSystemPro
+import filesystem as fs
+from filesystem import watcher as wat
+
+# Create a new instance of Watcher class
+watcher = wat.Watcher(f'{fs.documents}')
+
+# Run `diff` method to get directory changes
+while True:
+    changes = watcher.diff()
+    if changes:
+        print(f"Changes detected at: {datetime.now()}:")
+        for change in changes:
+            print(f"{change['abspath']} was {change['change']}")
+    time.sleep(5)  # Awaits for 5 seconds before a new verification
+```
+
+</details>
+
+---
+
+# Console
+
+```
+from filesystem import console as fsconsole
+```
+
+Console is a robust library designed to enable ANSI escape character sequences, which are used for generating colored terminal text and cursor positioning.
+This library is a key addition to FileSystemPro as a third-party library, enhancing the toolkit for developers who require consistent terminal styling across different operating systems.
+
+## Features
+
+- **Universal Compatibility:** Console ensures that applications or libraries utilizing ANSI sequences for colored output on Unix or Macs can now operate identically on Windows systems.
+- **Simplified Integration:** With no dependencies other than the standard library, integrating Console into your projects is straightforward. It’s tested across multiple Python versions, ensuring reliability.
+- **Enhanced Terminal Experience:** By converting ANSI sequences into appropriate win32 calls, Console allows Windows terminals to emulate the behavior of Unix terminals, providing a consistent user experience.
+- **Effortless Transition:** For developers transitioning to FileSystemPro, incorporating Console into your workflow is effortless, enabling you to maintain the visual aspects of your terminal applications without platform constraints.
+
+<table>
+  <tr>
+    <th>Constants</th>
+    <th>Colors</th>
+  </tr>
+  
+  <tr>
+    <td>foreground</td>
+    <td>
+      BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE, RESET.
+    </td>
+  </tr>
+  
+  <tr>
+    <td>background</td>
+    <td>
+      BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE, RESET.
+    </td>
+  </tr>
+  
+  <tr>
+    <td>style</td>
+    <td>
+     DIM, NORMAL, BRIGHT, RESET_ALL
+  </td>
+  </tr>
+  
+</table>
+
+## Sample Codes
+
+> [!NOTE]
+> Please note that **GitHub (and PYPI) does not support colored text** in README files. This is due to the limitations of the markdown language used in GitHub (and PYPI) READMEs, which does not have built-in support for text color changes.
+
+<details>
+<summary>Console: Printing a red foreground text message</summary>
+
+The following example shows how to print some red foreground texts using **Console**
+
+```py
+from filesystem import console as fsconsole
+
+# This will print a spaced text to your print message
+print(fsconsole.foreground.RED, "This is a warn message")
+
+# This will print a no space text to your print message
+print(fsconsole.foreground.RED + "This is another warn message")
+
+# You can use f-string format to assign the color to your print
+print(f'{fsconsole.foreground.RED}This is a new warn message{fsconsole.foreground.RESET}')
+
+# This text will be printed without color (default)
+print("This is a normal text")
+```
+
+Output:
+
+<pre><code><span style="color: red;"> This is a warn message
+This is another warn message
+This is a new warn message</span>
+<span">This is a normal text</span></code></pre>
+
+</details>
+
+
+<details>
+<summary>Console: Printing a blue background text message</summary>
+
+The following example shows how to print some blue background texts using **Console**
+
+```py
+from filesystem import console as fsconsole
+
+# This will print a spaced text to your print message
+print(fsconsole.background.BLUE, 'This is a blue background message')
+
+# This will print a no space text to your print message
+print(fsconsole.background.BLUE + 'This is another blue background message')
+
+# You can use f-string format to assign the color to your print
+print(f'{fsconsole.background.BLUE}This is a new blue background message{fsconsole.background.RESET}')
+
+# This text will be printed without color (default)
+print('This is a normal text')
+```
+
+Output:
+
+<pre><code><span style="background-color: #ADD8E6;"> This is a blue background message
+This is another blue background warn message
+This is a new blue background message</span>
+<span">This is a normal text</span></code></pre>
+
+</details>
+
+<details>
+<summary>Console: Different foregrounds, backgrounds and styles</summary>
+
+The following example shows how to print some texts with different backgrounds, foregrounds and styles using **Console**
+
+```py
+# Prints a red foreground text
+print(f'{fsconsole.foreground.RED}Some red text')
+# Prints a red foreground text with a green background
+print(f'{fsconsole.background.GREEN}And with a green background{fsconsole.style.RESET_ALL}')
+# Prints a dim normal text with no background
+print(f'{fsconsole.style.DIM}And in dim text{fsconsole.style.RESET_ALL}')
+# Prints a normal text
+print('Back to normal color')
+```
+
+Output:
+
+<pre><code><span style="color: red;">Some red text</span>
+<span style="background-color: #90EE90; color: red">And with a green background</span>
+<span style="color: #A9A9A9">And in dim text</span>
+<span>Back to normal color</span>
+</code></pre>
+
+</details>
+
+Remember, for the color changes to work, your Terminal must support ANSI escape sequences, which are used to set the color. Not all Terminals do, so if you’re not seeing the colors as expected, that could be why. 
+
+---
+
+Copyright © 2023–2024 Bisneto Inc. All rights reserved.
```

### Comparing `filesystempro-1.0.1.0/filesystem/watcher/__init__.py` & `filesystempro-1.0.2.0/filesystem/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `filesystempro-1.0.1.0/filesystem/wrapper/__init__.py` & `filesystempro-1.0.2.0/filesystem/wrapper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,21 +175,20 @@
     If `recursive` is set to `True`, the function will delete the directory and all its contents. 
     
     If `recursive` is set to `False`, the function will only delete the directory if it's empty. 
     
     Default is `False`.
     """
     if not os.path.exists(path):
-        print(f'\n\n>> The directory "{path}" does not exist.')
-        return
+        raise Exception(f'\n\n>> The directory "{path}" does not exist.')
 
     if not os.listdir(path) or recursive:
         shutil.rmtree(path)
     else:
-        print(f'\n\n>> The directory "{path}" is not empty.\n>> Use delete(path, True) to remove anyway.')
+        raise Exception(f'\n\n>> The directory "{path}" is not empty.\n>> Use delete(path, True) to remove anyway.')
 
 def enumerate_files(path):
     """
     This function performs a depth-first traversal of the directory tree at the given path 
     (after expanding any user home directory symbols).
     
     It returns a list of dictionaries containing the attributes of each file and directory in the tree.
```

### Comparing `filesystempro-1.0.1.0/filesystem/__init__.py` & `filesystempro-1.0.2.0/filesystem/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import getpass
 import os
 from sys import platform as PLATFORM
 
-__version__ = "1.0.1.0"
+## VERIFY IF THE LIBRARY HAS SOME AVAILABLE UPDATE
+from filesystem import __core__
+__core__.__checkupdates__("Hbisneto","FileSystemPro")
+## VERIFY IF THE LIBRARY HAS SOME AVAILABLE UPDATE
+
 CURRENT_LOCATION = os.getcwd()
 """
 Creates a string that represents the path to the current directory. (Where the application is running)
 """
 OS_SEPARATOR = os.sep
 """
 The os.sep is an attribute in the os module in Python. It represents the character that is used by the operating system to separate pathname components, and it varies between different operating systems.
```

### Comparing `filesystempro-1.0.1.0/setup.py` & `filesystempro-1.0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from setuptools import setup
+from setuptools import setup, Extension, find_packages
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(
     name = 'filesystempro',
-    version = '1.0.1.0',
+    version = '1.0.2.0',
     url = 'https://github.com/hbisneto/FileSystemPro',
     license = 'MIT License',
     
     author = 'Heitor Bisneto',
     author_email = 'heitor.bardemaker@live.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
@@ -25,19 +25,17 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     description = u'FileSystem Pro is designed to identify the operating system (OS) on which it`s running and define the paths to various user directories based on the OS.',
-    install_requires = [''],
+    install_requires = [
+        'requests',
+    ],
     long_description = readme,
     long_description_content_type = "text/markdown",
-    keywords = ['FileSystem', 'Linux', 'macOS', 'Windows', 'File', 'System'],
-    packages = [
-        'filesystem', 
-        'filesystem/watcher',
-        'filesystem/wrapper',
-        ],
+    keywords = ['FileSystem', 'Linux', 'macOS', 'Windows', 'File', 'System', 'Terminals'],
+    packages=find_packages(),
     platforms = 'any',
     python_requires= '>=3.8',
 )
```

