# Comparing `tmp/shell_whiz-3.2.1.tar.gz` & `tmp/shell_whiz-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_whiz-3.2.1.tar", max compression
+gzip compressed data, was "shell_whiz-3.2.2.tar", max compression
```

## Comparing `shell_whiz-3.2.1.tar` & `shell_whiz-3.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2024-03-27 18:55:14.045580 shell_whiz-3.2.1/LICENSE
--rw-r--r--   0        0        0     3262 2024-03-27 18:55:14.045580 shell_whiz-3.2.1/README.md
--rw-r--r--   0        0        0      965 2024-03-27 18:55:14.045580 shell_whiz-3.2.1/pyproject.toml
--rw-r--r--   0        0        0      147 2024-03-27 18:55:14.045580 shell_whiz-3.2.1/shell_whiz/ai/__init__.py
--rw-r--r--   0        0        0     3811 2024-03-27 18:55:14.045580 shell_whiz-3.2.1/shell_whiz/ai/client.py
--rw-r--r--   0        0        0      158 2024-03-27 18:55:14.045580 shell_whiz-3.2.1/shell_whiz/ai/errors.py
--rw-r--r--   0        0        0      419 2024-03-27 18:55:14.049579 shell_whiz-3.2.1/shell_whiz/ai/prompts/edit_shell_command.yml
--rw-r--r--   0        0        0     2932 2024-03-27 18:55:14.049579 shell_whiz-3.2.1/shell_whiz/ai/prompts/explain_shell_command.yml
--rw-r--r--   0        0        0      750 2024-03-27 18:55:14.049579 shell_whiz-3.2.1/shell_whiz/ai/prompts/recognise_dangerous_command.yml
--rw-r--r--   0        0        0      446 2024-03-27 18:55:14.049579 shell_whiz-3.2.1/shell_whiz/ai/prompts/suggest_shell_command.yml
--rw-r--r--   0        0        0     1378 2024-03-27 18:55:14.049579 shell_whiz-3.2.1/shell_whiz/ai/providers/api.py
--rw-r--r--   0        0        0     5425 2024-03-27 18:55:14.049579 shell_whiz-3.2.1/shell_whiz/ai/providers/openai.py
--rw-r--r--   0        0        0      256 2024-03-27 18:55:14.049579 shell_whiz-3.2.1/shell_whiz/cli/__init__.py
--rw-r--r--   0        0        0     7472 2024-03-27 18:55:14.049579 shell_whiz-3.2.1/shell_whiz/cli/commands/ask.py
--rw-r--r--   0        0        0      904 2024-03-27 18:55:14.049579 shell_whiz-3.2.1/shell_whiz/cli/commands/config.py
--rw-r--r--   0        0        0     2047 2024-03-27 18:55:14.049579 shell_whiz-3.2.1/shell_whiz/cli/commands/explain.py
--rw-r--r--   0        0        0     1887 2024-03-27 18:55:14.049579 shell_whiz-3.2.1/shell_whiz/cli/core/shell_command.py
--rw-r--r--   0        0        0     4768 2024-03-27 18:55:14.049579 shell_whiz-3.2.1/shell_whiz/config.py
--rw-r--r--   0        0        0     2806 2024-03-27 18:55:14.049579 shell_whiz-3.2.1/shell_whiz/main.py
--rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 shell_whiz-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/LICENSE
+-rw-r--r--   0        0        0     3254 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/README.md
+-rw-r--r--   0        0        0      965 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/pyproject.toml
+-rw-r--r--   0        0        0      147 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/ai/__init__.py
+-rw-r--r--   0        0        0     3811 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/ai/client.py
+-rw-r--r--   0        0        0      158 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/ai/errors.py
+-rw-r--r--   0        0        0      419 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/ai/prompts/edit_shell_command.yml
+-rw-r--r--   0        0        0     2926 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/ai/prompts/explain_shell_command.yml
+-rw-r--r--   0        0        0      750 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/ai/prompts/recognise_dangerous_command.yml
+-rw-r--r--   0        0        0      446 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/ai/prompts/suggest_shell_command.yml
+-rw-r--r--   0        0        0     1378 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/ai/providers/api.py
+-rw-r--r--   0        0        0     5425 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/ai/providers/openai.py
+-rw-r--r--   0        0        0      256 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/cli/__init__.py
+-rw-r--r--   0        0        0     7464 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/cli/commands/ask.py
+-rw-r--r--   0        0        0     1198 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/cli/commands/config.py
+-rw-r--r--   0        0        0     2047 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/cli/commands/explain.py
+-rw-r--r--   0        0        0     1887 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/cli/core/shell_command.py
+-rw-r--r--   0        0        0     4768 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/config.py
+-rw-r--r--   0        0        0     2806 2024-04-23 10:17:17.839094 shell_whiz-3.2.2/shell_whiz/main.py
+-rw-r--r--   0        0        0     4347 1970-01-01 00:00:00.000000 shell_whiz-3.2.2/PKG-INFO
```

### Comparing `shell_whiz-3.2.1/LICENSE` & `shell_whiz-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_whiz-3.2.1/README.md` & `shell_whiz-3.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 PowerShell users can create a function in their [PowerShell profile](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_profiles).
 
 ```powershell
 function ?? {
   sw ask `
     -s (Get-Command powershell.exe).Source `
-    -m gpt-4-turbo-preview `
+    -m gpt-4-turbo `
     -p "I use PowerShell on a daily basis" `
     @Args
 }
 ```
 
 You can also create a function that allows you to save executed commands in history. Here are the functions for Bash and Zsh:
```

### Comparing `shell_whiz-3.2.1/pyproject.toml` & `shell_whiz-3.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.poetry]
 name = "shell-whiz"
-version = "3.2.1"
+version = "3.2.2"
 description = "AI assistant for command line"
 license = "GPL-3.0-only"
 authors = ["Tamerlan Beyimjan <beyimjan@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/beyimjan/shell-whiz"
 packages = [{include = "shell_whiz"}]
```

### Comparing `shell_whiz-3.2.1/shell_whiz/ai/client.py` & `shell_whiz-3.2.2/shell_whiz/ai/client.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-3.2.1/shell_whiz/ai/prompts/explain_shell_command.yml` & `shell_whiz-3.2.2/shell_whiz/ai/prompts/explain_shell_command.yml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   - role: user
     content: "dd if=/dev/urandom of=/tmp/tmp.iH7K0TMOU9 bs=1M count=4096"
   - role: assistant
     content: |
       - `dd` is a command for copying and converting files.
         - `if=/dev/urandom` specifies the input file as the random device.
         - `of=...` specifies the output file.
-        - `bs=1M` sets the block size to 1 megabyte.
+        - `bs=1M` sets the block size to 1 MB.
         - `count=4096` sets the number of blocks to be copied.
   - role: user
     content: "ps aux --sort=-%mem"
   - role: assistant
     content: |
       - `ps` reports a snapshot of the current processes.
         - `a` displays processes from all users.
```

### Comparing `shell_whiz-3.2.1/shell_whiz/ai/prompts/recognise_dangerous_command.yml` & `shell_whiz-3.2.2/shell_whiz/ai/prompts/recognise_dangerous_command.yml`

 * *Files identical despite different names*

### Comparing `shell_whiz-3.2.1/shell_whiz/ai/providers/api.py` & `shell_whiz-3.2.2/shell_whiz/ai/providers/api.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-3.2.1/shell_whiz/ai/providers/openai.py` & `shell_whiz-3.2.2/shell_whiz/ai/providers/openai.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-3.2.1/shell_whiz/cli/commands/ask.py` & `shell_whiz-3.2.2/shell_whiz/cli/commands/ask.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                 coro=ai.get_explanation_of_shell_command(shell_command.args),
             )
         elif action == "Explain using GPT-4":
             print()
             await _explain_shell_command(
                 ai=ai,
                 coro=ai.get_explanation_of_shell_command(
-                    shell_command.args, model="gpt-4-turbo-preview"
+                    shell_command.args, model="gpt-4-turbo"
                 ),
             )
         elif action == "Revise query":
             await _edit_shell_command(ai=ai, shell_command=shell_command)
             return
         elif action == "Edit manually":
             await shell_command.edit_manually()
```

### Comparing `shell_whiz-3.2.1/shell_whiz/cli/commands/config.py` & `shell_whiz-3.2.2/shell_whiz/cli/commands/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,30 @@
 
 def config() -> None:
     """Set up OpenAI API key"""
 
     rich.print(
         "Visit https://platform.openai.com/api-keys to get your API key."
     )
+    openai_api_key = questionary.text(
+        "OpenAI API key",
+        default=os.environ.get("OPENAI_API_KEY", ""),
+        validate=lambda text: len(text) > 0,
+    ).unsafe_ask()
+
+    rich.print(
+        "\n[bold italic](Optional)[/] Leave blank if you are not a member of multiple organizations."
+    )
+    openai_org_id = questionary.text(
+        "Organization ID", default=os.environ.get("OPENAI_ORG_ID", "")
+    ).unsafe_ask()
 
     try:
         config = ConfigModel(
-            openai_api_key=questionary.text(
-                "OpenAI API key",
-                default=os.environ.get("OPENAI_API_KEY", ""),
-                validate=lambda text: len(text) > 0,
-            ).unsafe_ask()
+            openai_api_key=openai_api_key, openai_org_id=openai_org_id or None
         )
     except pydantic.ValidationError:
         rich.print(
             "[bold yellow]Error[/]: Something went wrong.", file=sys.stderr
         )
         raise typer.Exit(1)
```

### Comparing `shell_whiz-3.2.1/shell_whiz/cli/commands/explain.py` & `shell_whiz-3.2.2/shell_whiz/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-3.2.1/shell_whiz/cli/core/shell_command.py` & `shell_whiz-3.2.2/shell_whiz/cli/core/shell_command.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-3.2.1/shell_whiz/config.py` & `shell_whiz-3.2.2/shell_whiz/config.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-3.2.1/shell_whiz/main.py` & `shell_whiz-3.2.2/shell_whiz/main.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-3.2.1/PKG-INFO` & `shell_whiz-3.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-whiz
-Version: 3.2.1
+Version: 3.2.2
 Summary: AI assistant for command line
 Home-page: https://github.com/beyimjan/shell-whiz
 License: GPL-3.0-only
 Author: Tamerlan Beyimjan
 Author-email: beyimjan@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -64,15 +64,15 @@
 
 PowerShell users can create a function in their [PowerShell profile](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_profiles).
 
 ```powershell
 function ?? {
   sw ask `
     -s (Get-Command powershell.exe).Source `
-    -m gpt-4-turbo-preview `
+    -m gpt-4-turbo `
     -p "I use PowerShell on a daily basis" `
     @Args
 }
 ```
 
 You can also create a function that allows you to save executed commands in history. Here are the functions for Bash and Zsh:
```

