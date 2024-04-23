# Comparing `tmp/sfmanager-0.1.7.tar.gz` & `tmp/sfmanager-0.1.8.tar.gz`

## Comparing `sfmanager-0.1.7.tar` & `sfmanager-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 sfmanager-0.1.7/update
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 sfmanager-0.1.7/version
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.7/sfmanager/__init__.py
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 sfmanager-0.1.7/sfmanager/app.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 sfmanager-0.1.7/sfmanager/utils.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.7/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.7/LICENSE
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 sfmanager-0.1.7/README.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 sfmanager-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 sfmanager-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 sfmanager-0.1.8/update
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 sfmanager-0.1.8/version
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.8/sfmanager/__init__.py
+-rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 sfmanager-0.1.8/sfmanager/app.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 sfmanager-0.1.8/sfmanager/utils.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.8/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.8/LICENSE
+-rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 sfmanager-0.1.8/README.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 sfmanager-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6209 2020-02-02 00:00:00.000000 sfmanager-0.1.8/PKG-INFO
```

### Comparing `sfmanager-0.1.7/sfmanager/app.py` & `sfmanager-0.1.8/sfmanager/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 	# Funcs for work with text files(.txt)
 
 	# Read line in text file
 
 	def readline(self, dst, use_wd=True):
 		if self.level >= 1:
 			try:
-				if use_wd == True:
+				if use_wd == True and "/" in self._dir:
 					with open(f"{self._dir}{dst}", "r") as f:
 						raw = f.readline()
 				else:
 					with open(f"{dst}", "r") as f:
 						raw = f.readline()
 				return raw
 			except FileNotFoundError:
@@ -163,15 +163,15 @@
 			print(f"Low access level! {self.level}, but need 1")
 
 	# Read lines in text file (as array)
 
 	def readlines(self, dst, use_wd=True):
 		if self.level >= 1:
 			try:
-				if use_wd == True:
+				if use_wd == True and "/" in self._dir:
 					with open(f"{self._dir}{dst}", "r") as f:
 						raw = f.readlines()
 				else:
 					with open(f"{dst}", "r") as f:
 						raw = f.readlines()
 				return raw
 			except FileNotFoundError:
@@ -180,15 +180,15 @@
 			print(f"Low access level! {self.level}, but need 1")
 
 	# Set content in text file
 
 	def set(self, dst, text, use_wd=True):
 		if self.level >= 3:
 			try:
-				if use_wd == True:
+				if use_wd == True and "/" in self._dir:
 					with open(f"{self._dir}{dst}", "w") as f:
 						f.write(text)
 						return 1
 				else:
 					with open(f"{dst}", "w") as f:
 						f.write(text)
 						return 1
@@ -198,15 +198,15 @@
 			print(f"Low access level! {self.level}, but need 3")
 
 	# Add content in text file with separator(default separator is empty)
 
 	def add(self, dst, text, sep="", use_wd=True):
 		if self.level >= 2:
 			try:
-				if use_wd == True:
+				if use_wd == True and "/" in self._dir:
 					with open(f"{self._dir}{dst}", "r") as f:
 						old = f.read()
 					with open(f"{self._dir}{dst}", "w") as f:
 						f.write(old + sep + text)
 						return 1
 				else:
 					with open(f"{dst}", "r") as f:
@@ -220,15 +220,15 @@
 			print(f"Low access level! {self.level}, but need 2")
 
 	# Replace certain content in text file
 
 	def replace(self, dst, _from, _to, use_wd=True):
 		if self.level >= 3:
 			try:
-				if use_wd == True:
+				if use_wd == True and "/" in self._dir:
 					with open(f"{dst}", "r") as f:
 						data = f.read().replace(_from, _to)
 					with open(f"{dst}", "w") as f:
 						f.write(data)
 				else:
 					with open(f"{dst}", "r") as f:
 						data = f.read().replace(_from, _to)
@@ -241,70 +241,70 @@
 
 	# Funcs for general work with files
 
 	# Create line
 
 	def create(self, dst, use_wd=True):
 		if self.level >= 2:
-			if use_wd == True:
+			if use_wd == True and "/" in self._dir:
 				f = open(f"{self._dir}{dst}")
 			else:
 				f = open(f"{dst}", "a")
 			f.close()
 		else:
 			print(f"Low access level! {self.level}, but need 2")
 
 	# Rename file(from self.filename to name)
 
 	def rename(self, dst, name, use_wd=True):
 		if self.level >= 4:
 			try:
-				if use_wd == True:
+				if use_wd == True and "/" in self._dir:
 					os.rename(f"{self._dir}{dst}")
 				else:
 					os.rename(f"{dst}", name)
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 4")
 
 	# Delete file
 
 	def delete(self, dst, use_wd=True):
 		if self.level == 5:
 			try:
-				if use_wd == True:
+				if use_wd == True and "/" in self._dir:
 					os.remove(f"{self._dir}{dst}")
 				else:
 					os.remove(f"{dst}")
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 5")
 
 	# Copy file
 
 	def copy(self, dst, new_dst, use_wd=True):
 		if self.level >= 4:
 			try:
-				if use_wd == True:
+				if use_wd == True and "/" in self._dir:
 					shutil.copy2(f"{self._dir}{dst}", f"{new_dst}")
 				else:
 					shutil.copy2(f"{dst}", f"{new_dst}")
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 4")
 
 	# Move file
 
 	def move(self, dst, new_dst, use_wd=True):
 		if self.level >= 4:
 			try:
-				if use_wd == True:
+				if use_wd == True and "/" in self._dir:
 					shutil.move(f"{self._dir}{dst}")
 				else:
 					shutil.move(f"{dst}", f"{new_dst}")
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 4")
```

### Comparing `sfmanager-0.1.7/sfmanager/utils.py` & `sfmanager-0.1.8/sfmanager/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 
 import pkg_resources
 import httpx
 import subprocess
 import sys
 import os
 
-logger.add("logs.log", level="DEBUG")
-
 def whatIsIt():
+	updates = httpx.get("https://raw.githubusercontent.com/GrandTheBest/sfmanager/main/update")
 	print("")
 	print("Hello dear user!")
 	sleep(1)
 	print("Thanks for download my library!")
 	sleep(2)
 	print("Homepage on github: https://github.com/GrandTheBest/sfmanager")
 	sleep(2)
@@ -26,14 +25,23 @@
 	print("Also you can create, copy, move, rename and remove any files.")
 	sleep(2)
 	print("That's all. Stay tuned!")
 	sleep(2)
 	print("Thanks for using! Good luck!")
 	sleep(1)
 
+	v = pkg_resources.get_distribution("sfmanager").version
+	print(f"\nv{v} stable-v1")
+	if updates.status_code == 200:
+		print(f"Whats new in v{v}?")
+		print(updates.text[0:])
+	print("Homepage on github: https://github.com/GrandTheBest/sfmanager")
+	print("Issues page on github: https://github.com/GrandTheBest/sfmanager/issues")
+	print("Documentation: https://github.com/GrandTheBest/sfmanager/blob/main/README.md")
+
 @logger.catch
 def checkUpdates():
 	logger.info("Checking for updates")
 
 	installed_v = pkg_resources.get_distribution("sfmanager").version
 	v = httpx.get("https://raw.githubusercontent.com/GrandTheBest/sfmanager/main/version")
 	updates = httpx.get("https://raw.githubusercontent.com/GrandTheBest/sfmanager/main/update")
@@ -47,11 +55,11 @@
 		else:
 			logger.info("Downloading an update using pip")
 
 			subprocess.check_call([sys.executable, "-m", "pip", "install", "sfmanager==" + value_v])
 			logger.success("sfmanager updated, changes will take effect after restart")
 
 			if updates.status_code == 200:
-				value_u = updates.text[0:]
-				print(f"{value_v}")
+				print(f"Whats new in v{value_v}?")
+				print(updates.text[0:])
 
 			os.chdir(os.path.join(pkg_resources.get_distribution("sfmanager").location, "sfmanager"))
```

### Comparing `sfmanager-0.1.7/.gitignore` & `sfmanager-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.7/LICENSE` & `sfmanager-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.7/README.md` & `sfmanager-0.1.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # SFManager 
 
 [![PyPI version](https://img.shields.io/pypi/v/sfmanager)](https://pypi.org/project/sfmanager/)
-
-## What new in 0.1.6?
-> - Added the abillity to work with any files independently of each other
-> - Added check updates on command `sfmanager`
-> - Added method `cd` for set work directory
-> - Added method `create` - for create files
-> - Added print "What new in v...?" in command sfmanager after update sfmanager
+[![Distribution](https://img.shields.io/badge/Distribution-Stable%20V1-green)](https://pypi.org/project/sfmanager/)
+[![Distribution](https://img.shields.io/badge/Release-v0.1.8%20stable-blue)](https://github.com/GrandTheBest/sfmanager/releases/tag/v0.1.8-stable)
+[![Distribution](https://img.shields.io/github/license/GrandTheBest/sfmanager.svg)](https://github.com/GrandTheBest/sfmanager?tab=GPL-3.0-1-ov-file)
+
+## What new in 0.1.8?
+> - Fixed bug with empty directory
+> - Removed log file and save logs in log file(temporarily)
+> - Modified `sfmanager` command
 
 ## This library is not that useful. Perhaps someday it will become great.
 
 ## Python super filemanager
 
 SFManager - this is library for work with files!
```

### Comparing `sfmanager-0.1.7/pyproject.toml` & `sfmanager-0.1.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "sfmanager"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
 	{name="GrandTheBest", email="grandinfo-cm@gmail.com"},
 ]
 description = "This library is not that useful. Perhaps someday it will become great."
 readme = "README.md"
 requires-python = ">=3.10.0"
 dependencies = [
 	"Pillow>=9.0.1",
    "loguru>=0.7.2"
 ]
 classifiers = [
    "Programming Language :: Python :: 3",
-   "License :: OSI Approved :: MIT License",
+   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
    "Operating System :: OS Independent",
 ]
 [project.scripts]
 sfmanager = "sfmanager:checkUpdates"
 [project.urls]
 Homepage = "https://github.com/GrandTheBest/sfmanager"
 Issues = "https://github.com/GrandTheBest/sfmanager/issues"
```

### Comparing `sfmanager-0.1.7/PKG-INFO` & `sfmanager-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.3
 Name: sfmanager
-Version: 0.1.7
+Version: 0.1.8
 Summary: This library is not that useful. Perhaps someday it will become great.
 Project-URL: Homepage, https://github.com/GrandTheBest/sfmanager
 Project-URL: Issues, https://github.com/GrandTheBest/sfmanager/issues
 Author-email: GrandTheBest <grandinfo-cm@gmail.com>
 License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.0
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: pillow>=9.0.1
 Description-Content-Type: text/markdown
 
 # SFManager 
 
 [![PyPI version](https://img.shields.io/pypi/v/sfmanager)](https://pypi.org/project/sfmanager/)
-
-## What new in 0.1.6?
-> - Added the abillity to work with any files independently of each other
-> - Added check updates on command `sfmanager`
-> - Added method `cd` for set work directory
-> - Added method `create` - for create files
-> - Added print "What new in v...?" in command sfmanager after update sfmanager
+[![Distribution](https://img.shields.io/badge/Distribution-Stable%20V1-green)](https://pypi.org/project/sfmanager/)
+[![Distribution](https://img.shields.io/badge/Release-v0.1.8%20stable-blue)](https://github.com/GrandTheBest/sfmanager/releases/tag/v0.1.8-stable)
+[![Distribution](https://img.shields.io/github/license/GrandTheBest/sfmanager.svg)](https://github.com/GrandTheBest/sfmanager?tab=GPL-3.0-1-ov-file)
+
+## What new in 0.1.8?
+> - Fixed bug with empty directory
+> - Removed log file and save logs in log file(temporarily)
+> - Modified `sfmanager` command
 
 ## This library is not that useful. Perhaps someday it will become great.
 
 ## Python super filemanager
 
 SFManager - this is library for work with files!
```

