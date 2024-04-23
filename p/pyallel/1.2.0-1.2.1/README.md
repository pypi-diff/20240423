# Comparing `tmp/pyallel-1.2.0.tar.gz` & `tmp/pyallel-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyallel-1.2.0.tar", max compression
+gzip compressed data, was "pyallel-1.2.1.tar", max compression
```

## Comparing `pyallel-1.2.0.tar` & `pyallel-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-12-10 12:28:31.474872 pyallel-1.2.0/LICENSE
--rw-r--r--   0        0        0     4334 2024-04-20 11:06:03.145124 pyallel-1.2.0/README.md
--rw-r--r--   0        0        0     1047 2024-04-20 10:58:17.449054 pyallel-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-10 12:28:31.486873 pyallel-1.2.0/src/pyallel/__init__.py
--rw-r--r--   0        0        0      893 2024-04-13 11:42:32.468688 pyallel-1.2.0/src/pyallel/colours.py
--rw-r--r--   0        0        0      564 2024-04-20 09:08:17.203906 pyallel-1.2.0/src/pyallel/constants.py
--rw-r--r--   0        0        0      368 2023-12-10 16:41:29.922819 pyallel-1.2.0/src/pyallel/errors.py
--rw-r--r--   0        0        0     2190 2024-04-20 09:42:35.756227 pyallel-1.2.0/src/pyallel/main.py
--rw-r--r--   0        0        0     2799 2024-04-20 10:37:37.130827 pyallel-1.2.0/src/pyallel/parser.py
--rw-r--r--   0        0        0     1952 2024-04-20 09:15:53.499524 pyallel-1.2.0/src/pyallel/process.py
--rw-r--r--   0        0        0    10871 2024-04-20 09:16:13.527683 pyallel-1.2.0/src/pyallel/process_group.py
--rw-r--r--   0        0        0     2919 2024-04-20 10:15:27.504102 pyallel-1.2.0/src/pyallel/process_group_manager.py
--rw-r--r--   0        0        0        0 2023-12-10 12:28:32.010876 pyallel-1.2.0/src/pyallel/py.typed
--rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 pyallel-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-12-20 08:59:25.146414 pyallel-1.2.1/LICENSE
+-rw-r--r--   0        0        0     4983 2024-04-23 11:39:12.544453 pyallel-1.2.1/README.md
+-rw-r--r--   0        0        0     1047 2024-04-23 11:40:29.451691 pyallel-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-20 08:59:25.146880 pyallel-1.2.1/src/pyallel/__init__.py
+-rw-r--r--   0        0        0      893 2024-03-07 08:35:52.711592 pyallel-1.2.1/src/pyallel/colours.py
+-rw-r--r--   0        0        0      571 2024-04-23 11:33:30.180565 pyallel-1.2.1/src/pyallel/constants.py
+-rw-r--r--   0        0        0      368 2023-12-20 08:59:25.146977 pyallel-1.2.1/src/pyallel/errors.py
+-rw-r--r--   0        0        0     2190 2024-04-22 08:12:02.701958 pyallel-1.2.1/src/pyallel/main.py
+-rw-r--r--   0        0        0     2799 2024-04-22 08:12:02.702095 pyallel-1.2.1/src/pyallel/parser.py
+-rw-r--r--   0        0        0     1830 2024-04-22 08:12:02.702258 pyallel-1.2.1/src/pyallel/process.py
+-rw-r--r--   0        0        0    10864 2024-04-23 11:25:05.548244 pyallel-1.2.1/src/pyallel/process_group.py
+-rw-r--r--   0        0        0     2919 2024-04-22 08:12:02.702497 pyallel-1.2.1/src/pyallel/process_group_manager.py
+-rw-r--r--   0        0        0        0 2023-12-20 08:59:25.147305 pyallel-1.2.1/src/pyallel/py.typed
+-rw-r--r--   0        0        0     5891 1970-01-01 00:00:00.000000 pyallel-1.2.1/PKG-INFO
```

### Comparing `pyallel-1.2.0/LICENSE` & `pyallel-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyallel-1.2.0/README.md` & `pyallel-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -72,36 +72,60 @@
 
 You can also build an executable with the following (executables will be written to `./dist`):
 
 > [!NOTE]
 > The `arch=x86_64` values in the following code blocks can be replaced with `arch=aarch64` and
 > any other architecture that is supported by docker to build an executable for that given architecture
 
+> [!NOTE]
+> To build aarch64 binaries on an x86_64 host machine, you will need to run the following
+> commands to setup qemu to allow this to work
+
+```bash
+sudo apt-get install qemu binfmt-support qemu-user-static && \
+docker run --rm --privileged multiarch/qemu-user-static --reset -p yes
+```
+
 #### Build for generic linux
 
 ```bash
-docker build --tag pyallel --build-arg 'arch=x86_64' . && docker run -e 'arch=x86_64' --rm --volume "$(pwd):/src" pyallel
+docker build --tag pyallel --build-arg 'arch=x86_64' --build-arg "uid=$(id -u)" . && \
+    docker run -e 'arch=x86_64' --rm --volume "$(pwd):/src" pyallel
 ```
 
 #### Build for alpine linux
 
 ```bash
-docker build --tag pyallel-alpine --build-arg 'arch=x86_64' --file Dockerfile.alpine . && docker run -e 'arch=x86_64' --rm --volume "$(pwd):/src" pyallel-alpine
+docker build --tag pyallel-alpine --build-arg 'arch=x86_64' --build-arg "uid=$(id -u)" --file Dockerfile.alpine . && \
+    docker run -e 'arch=x86_64' --rm --volume "$(pwd):/src" pyallel-alpine
 ```
 
 #### Build locally
 
 ```bash
-python -m venv .venv && source .venv/bin/activate && pip install . -r requirements_build.txt && ./build.sh
+python -m venv .venv && \
+  source .venv/bin/activate && \
+  pip install . -r requirements_build.txt && \
+  ./build.sh
+```
+
+#### Build all
+
+```bash
+./build_all.sh
 ```
 
 ## TODOs
 
 - [x] Add support to have commands depend on other commands (some commands must complete
       before a given command can start)
+- [ ] Add a debug mode that logs debug information to a log file
+- [ ] Fix wrapping of long commands in the command status line
+- [ ] Fix wrapping of very long lines in command output that pushes other commands off the
+      screen
 - [ ] Add support to state how many lines a command can use for it's output in interactive mode
 - [ ] Maybe add support to allow the user to provide stdin for commands that request it
       (such as a REPL)
 - [ ] Add custom parsing of command output to support filtering for errors (like vim's
       `errorformat`)
 - [ ] Allow list of files to be provided to supply as input arguments to each command
 - [ ] Allow input to be piped into `pyallel` via stdin to supply as standard input to each
```

### Comparing `pyallel-1.2.0/pyproject.toml` & `pyallel-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyallel"
-version = "1.2.0"
+version = "1.2.1"
 description = "Run and handle the output of multiple executables in pyallel (as in parallel)"
 authors = ["Daniel Black <danielcrblack@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Danthewaann/pyallel"
 repository = "https://github.com/Danthewaann/pyallel"
 keywords = ["parallel", "command", "runner", "executable", "shell", "terminal"]
```

### Comparing `pyallel-1.2.0/src/pyallel/colours.py` & `pyallel-1.2.1/src/pyallel/colours.py`

 * *Files identical despite different names*

### Comparing `pyallel-1.2.0/src/pyallel/constants.py` & `pyallel-1.2.1/src/pyallel/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import re
 import sys
 
 IN_TTY = sys.stdout.isatty()
 CLEAR_LINE = "\033[2K"
 UP_LINE = "\033[1F"
-ANSI_ESCAPE = re.compile(r"(\x9B|\x1B\[)[0-?]*[ -\/]*[@-~]")
+ANSI_ESCAPE = re.compile(r"(\x9B|\x1B\[|\x1B\()[0-?]*[ -\/]*[@-~]")
 
 if IN_TTY:
 
     def COLUMNS() -> int:
         return os.get_terminal_size().columns
 
     def LINES() -> int:
```

### Comparing `pyallel-1.2.0/src/pyallel/main.py` & `pyallel-1.2.1/src/pyallel/main.py`

 * *Files identical despite different names*

### Comparing `pyallel-1.2.0/src/pyallel/parser.py` & `pyallel-1.2.1/src/pyallel/parser.py`

 * *Files identical despite different names*

### Comparing `pyallel-1.2.0/src/pyallel/process.py` & `pyallel-1.2.1/src/pyallel/process.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,11 +66,7 @@
         if self._process:
             self._process.send_signal(signal.SIGKILL)
 
     def wait(self) -> int:
         if self._process:
             return self._process.wait()
         return -1
-
-    @classmethod
-    def from_command(cls, id: int, command: str) -> Process:
-        return cls(id=id, command=command)
```

### Comparing `pyallel-1.2.0/src/pyallel/process_group.py` & `pyallel-1.2.1/src/pyallel/process_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     completed_processes: set[int] = field(default_factory=set)
     exit_code: int = 0
     interrupt_count: int = 0
     passed: bool = True
     icon: int = 0
     colours: Colours = field(default_factory=Colours)
 
+    def __post_init__(self) -> None:
+        self.process_lines = [0 for _ in self.processes]
+
     def stream(self) -> int:
         for process in self.processes:
             process.run()
 
         if not self.interactive:
             return self.stream_non_interactive()
 
@@ -223,15 +226,15 @@
     ) -> ProcessGroup:
         colours = colours or Colours()
         processes: list[Process] = []
         errors: list[InvalidExecutableError] = []
 
         for i, command in enumerate(commands):
             try:
-                processes.append(Process.from_command(i + 1, command))
+                processes.append(Process(i + 1, command))
             except InvalidExecutableError as e:
                 errors.append(e)
 
         if errors:
             raise InvalidExecutableErrors(*errors)
 
         process_group = cls(
@@ -239,26 +242,21 @@
             interactive=interactive,
             timer=timer,
             colours=colours,
         )
 
         return process_group
 
-    def complete_output(self, tail: int = 20, all: bool = False) -> str:
+    def complete_output(self, all: bool = False) -> str:
         num_processes = len(self.processes)
         lines = constants.LINES() - (2 * num_processes)
         remainder = lines % num_processes
         tail = lines // num_processes
-
-        if self.process_lines:
-            self.process_lines = []
-
-        for process in self.processes:
-            self.process_lines.append(tail)
-
+        for i in range(num_processes):
+            self.process_lines[i] = tail
         if remainder:
             self.process_lines[-1] += remainder - 2
         else:
             self.process_lines[-1] -= 2
 
         output = ""
         for i, process in enumerate(self.processes, start=1):
```

### Comparing `pyallel-1.2.0/src/pyallel/process_group_manager.py` & `pyallel-1.2.1/src/pyallel/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `pyallel-1.2.0/PKG-INFO` & `pyallel-1.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyallel
-Version: 1.2.0
+Version: 1.2.1
 Summary: Run and handle the output of multiple executables in pyallel (as in parallel)
 Home-page: https://github.com/Danthewaann/pyallel
 License: MIT
 Keywords: parallel,command,runner,executable,shell,terminal
 Author: Daniel Black
 Author-email: danielcrblack@gmail.com
 Requires-Python: >=3.8,<3.13
@@ -94,36 +94,60 @@
 
 You can also build an executable with the following (executables will be written to `./dist`):
 
 > [!NOTE]
 > The `arch=x86_64` values in the following code blocks can be replaced with `arch=aarch64` and
 > any other architecture that is supported by docker to build an executable for that given architecture
 
+> [!NOTE]
+> To build aarch64 binaries on an x86_64 host machine, you will need to run the following
+> commands to setup qemu to allow this to work
+
+```bash
+sudo apt-get install qemu binfmt-support qemu-user-static && \
+docker run --rm --privileged multiarch/qemu-user-static --reset -p yes
+```
+
 #### Build for generic linux
 
 ```bash
-docker build --tag pyallel --build-arg 'arch=x86_64' . && docker run -e 'arch=x86_64' --rm --volume "$(pwd):/src" pyallel
+docker build --tag pyallel --build-arg 'arch=x86_64' --build-arg "uid=$(id -u)" . && \
+    docker run -e 'arch=x86_64' --rm --volume "$(pwd):/src" pyallel
 ```
 
 #### Build for alpine linux
 
 ```bash
-docker build --tag pyallel-alpine --build-arg 'arch=x86_64' --file Dockerfile.alpine . && docker run -e 'arch=x86_64' --rm --volume "$(pwd):/src" pyallel-alpine
+docker build --tag pyallel-alpine --build-arg 'arch=x86_64' --build-arg "uid=$(id -u)" --file Dockerfile.alpine . && \
+    docker run -e 'arch=x86_64' --rm --volume "$(pwd):/src" pyallel-alpine
 ```
 
 #### Build locally
 
 ```bash
-python -m venv .venv && source .venv/bin/activate && pip install . -r requirements_build.txt && ./build.sh
+python -m venv .venv && \
+  source .venv/bin/activate && \
+  pip install . -r requirements_build.txt && \
+  ./build.sh
+```
+
+#### Build all
+
+```bash
+./build_all.sh
 ```
 
 ## TODOs
 
 - [x] Add support to have commands depend on other commands (some commands must complete
       before a given command can start)
+- [ ] Add a debug mode that logs debug information to a log file
+- [ ] Fix wrapping of long commands in the command status line
+- [ ] Fix wrapping of very long lines in command output that pushes other commands off the
+      screen
 - [ ] Add support to state how many lines a command can use for it's output in interactive mode
 - [ ] Maybe add support to allow the user to provide stdin for commands that request it
       (such as a REPL)
 - [ ] Add custom parsing of command output to support filtering for errors (like vim's
       `errorformat`)
 - [ ] Allow list of files to be provided to supply as input arguments to each command
 - [ ] Allow input to be piped into `pyallel` via stdin to supply as standard input to each
```

