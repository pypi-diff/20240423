# Comparing `tmp/mkdocs-table-of-figures-0.2.0.tar.gz` & `tmp/mkdocs-table-of-figures-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-table-of-figures-0.2.0.tar", last modified: Fri Apr 19 12:15:57 2024, max compression
+gzip compressed data, was "mkdocs-table-of-figures-0.2.2.tar", last modified: Tue Apr 23 13:14:14 2024, max compression
```

## Comparing `mkdocs-table-of-figures-0.2.0.tar` & `mkdocs-table-of-figures-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-19 12:15:57.909587 mkdocs-table-of-figures-0.2.0/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2023-05-09 09:20:19.000000 mkdocs-table-of-figures-0.2.0/MANIFEST.in
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     6813 2024-04-19 12:15:57.909587 mkdocs-table-of-figures-0.2.0/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1288 2024-04-17 13:51:56.000000 mkdocs-table-of-figures-0.2.0/changelog.md
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2023-04-28 08:21:37.000000 mkdocs-table-of-figures-0.2.0/license
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-19 12:15:57.797205 mkdocs-table-of-figures-0.2.0/mkdocs_table_of_figures/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-02 06:14:09.000000 mkdocs-table-of-figures-0.2.0/mkdocs_table_of_figures/__init__.py
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     8581 2024-04-19 12:14:17.000000 mkdocs-table-of-figures-0.2.0/mkdocs_table_of_figures/plugin.py
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-19 12:15:57.892988 mkdocs-table-of-figures-0.2.0/mkdocs_table_of_figures.egg-info/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     6813 2024-04-19 12:15:57.000000 mkdocs-table-of-figures-0.2.0/mkdocs_table_of_figures.egg-info/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      417 2024-04-19 12:15:57.000000 mkdocs-table-of-figures-0.2.0/mkdocs_table_of_figures.egg-info/SOURCES.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2024-04-19 12:15:57.000000 mkdocs-table-of-figures-0.2.0/mkdocs_table_of_figures.egg-info/dependency_links.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       83 2024-04-19 12:15:57.000000 mkdocs-table-of-figures-0.2.0/mkdocs_table_of_figures.egg-info/entry_points.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       14 2024-04-19 12:15:57.000000 mkdocs-table-of-figures-0.2.0/mkdocs_table_of_figures.egg-info/requires.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       24 2024-04-19 12:15:57.000000 mkdocs-table-of-figures-0.2.0/mkdocs_table_of_figures.egg-info/top_level.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     5204 2024-04-19 12:05:39.000000 mkdocs-table-of-figures-0.2.0/readme.md
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2024-04-19 12:15:57.916175 mkdocs-table-of-figures-0.2.0/setup.cfg
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1135 2024-04-18 09:31:56.000000 mkdocs-table-of-figures-0.2.0/setup.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-23 13:14:14.898038 mkdocs-table-of-figures-0.2.2/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.2.2/MANIFEST.in
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     5928 2024-04-23 13:14:14.892710 mkdocs-table-of-figures-0.2.2/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1742 2024-04-23 13:06:41.000000 mkdocs-table-of-figures-0.2.2/changelog.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.2.2/license
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-23 13:14:14.801363 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures/__init__.py
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)    11367 2024-04-23 13:03:08.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures/plugin.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-23 13:14:14.877189 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     5928 2024-04-23 13:14:14.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      417 2024-04-23 13:14:14.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2024-04-23 13:14:14.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       83 2024-04-23 13:14:14.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/entry_points.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       14 2024-04-23 13:14:14.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/requires.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       24 2024-04-23 13:14:14.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/top_level.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     5389 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.2.2/readme.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2024-04-23 13:14:14.899039 mkdocs-table-of-figures-0.2.2/setup.cfg
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1135 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.2.2/setup.py
```

### Comparing `mkdocs-table-of-figures-0.2.0/PKG-INFO` & `mkdocs-table-of-figures-0.2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,151 +1,156 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.2.0
+Version: 0.2.2
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
-Description: # mkdocs-table-of-figures
-        
-        This is a plugin that creates a `figcaption` with elements `alt` attribute or title and lists all figures in files into a table of figures to be integrated in `Markdown` pages for MkDocs.
-        
-        ## Setup
-        
-        ### Installing using pip:
-        
-        `pip install mkdocs-table-of-figures`
-        
-        ## Config
-        
-        You need to activate the plugin in `mkdocs.yml`:
-        
-        ``` yaml
-        plugins:
-          - table-of-figures:
-              title_label: "Table of figures of the documentation" # Optional --> Default : Table of Figures
-              figure_label: "Figure N°" # Optional --> Default : Figure
-              description_label: "Description of the figures" # Optional --> Default : Description
-        
-              temp_dir: "folder_name" # Optional --> Default : temp_figures
-              file: "file_name" # Optional --> Default : figures.md
-              
-              on_mermaid: true # Optional --> Default : false
-              on_codeblock: true # Optional --> Default : false
-              on_table: true # Optional --> Default : false
-        ```
-        
-        As you can see, every option is optional, but if you want to generate a table of figures in another language than English, you will need to set up label options.
-        
-        - `title_label` - This is the title (heading 1) given to the page that will contain the table of figures.
-        - `figure_label` - This is the name given to every figure right before the auto-incremented number.
-        - `description_label` - This is the label given to the column containing the description of each figure (alt text).
-        - `temp_dir` - The temporary directory used to store the table of figures `Markdown` file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
-        - `file` - The name of the `Markdown` file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
-        - `on_mermaid` - To enable `mermaid` diagrams support, need to use of `md_in_html` `Markdown` extension
-        - `on_codeblock` - To enable code blocks support, need to use of `md_in_html` `Markdown` extension
-        - `on_table` - To enable tables support, need to use of `md_in_html` `Markdown` extension
-        
-        ## Usage
-        
-        The plugin will only look for `Markdown` image composed of alt text. If you don't set any alt text for the `Markdown` image it will be ignored.
-        
-        There is two way of correctly rendering image stored within the docs:
-        
-        - Using url from base: this mean that you give the full path from the docs directory starting with `/` like this `/path/to/image/from/docs/image.png`
-        - With the help of `md_in_html`: there is a `Markdown` extension that you can set in `mkdocs.yml` that allow the plugin to place `Markdown` in `HTML` which allow this plugin to let `MkDocs` set relative link in src attribute properly during `HTML` rendering
-        
-        Concerning external images nothing change.
-        
-        You can set the `md_in_html` option like so :
-        
-        ``` yaml
-        markdown_extensions:
-          - md_in_html
-        ```
-        
-        Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
-        
-        ## Support
-        
-        This plugin currently supports markdown images, `mermaid` diagrams, code blocks and table.
-        
-        To make a `mermaid` diagram, code block or table detectable by this plugin, you need to give it a title at the line just below it like this:
-        
-        ``` markdown
-            ``` php
-            <?php
-              $var = 42;
-            ?>
-            ```
-            The title of the code block go here
-        ```
-        
-        ``` markdown
-            ``` mermaid
-            sequenceDiagram
-                participant Alice
-                participant Bob
-                Alice->>John: Hello John, how are you?
-                loop Healthcheck
-                    John->>John: Fight against hypochondria
-                end
-                Note right of John: Rational thoughts <br/>prevail!
-                John-->>Alice: Great!
-                John->>Bob: How about you?
-                Bob-->>John: Jolly good!
-            ```
-            The title of the mermaid diagram go here
-        ```
-        
-        ``` markdown
-            | Table   | Right | Center  | Left  |
-            | ------- | ----: | :-----: | :---- |
-            | A table |  With | Content | in it |
-            The title of the table go here
-        ```
-        
-        It will not work if there is a line between the element and the title.
-        
-        I highly recommend using `mkdocs-material` to use `mermaid` diagrams. For more info about `mermaid` diagrams, I invite you to check `mkdocs-material` and `mermaid`'s official documentation.
-        
-        I also recommend to add this stylesheet to prevent mermaid size from being reduced or code blocks from having code centered by mkdocs-material.
-        
-        ``` css
-        figure.figure-mermaid {
-            margin: 0 1em;
-            width: 100%;
-        }
-        
-        figure.figure-codeblock code {
-            text-align: initial;
-        }
-        ```
-        
-        You can place the stylesheet in your `mkdocs.yml` at extra-css option
-        
-        ``` yml
-        extra_css:
-          - fix-mermaid-figure.css
-        ```
-        
-        ## License
-        
-        This project is under MIT license. See the `license` file for more details.
-        
-        ## See Also
-        
-        - [GitLab Repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-table-of-figures/)
-        - [MkDocs Website](http://www.mkdocs.org/)
-        - [MkDocs-Material Documentation](https://squidfunk.github.io/mkdocs-material/)
-        - [Mermaid Documentation](https://mermaid.org/intro/)
 Keywords: mkdocs
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+
+# mkdocs-table-of-figures
+
+This is a plugin that creates a `figcaption` with elements `alt` attribute or title and lists all figures in files into a table of figures to be integrated in `Markdown` pages for MkDocs.
+
+## Setup
+
+### Installing using pip:
+
+`pip install mkdocs-table-of-figures`
+
+## Config
+
+You need to activate the plugin in `mkdocs.yml`:
+
+``` yaml
+plugins:
+  - table-of-figures:
+      title_label: "Table of figures of the documentation" # Optional --> Default : Table of Figures
+      figure_label: "Figure N°" # Optional --> Default : Figure
+      description_label: "Description of the figures" # Optional --> Default : Description
+
+      temp_dir: "folder_name" # Optional --> Default : temp_figures
+      file: "file_name" # Optional --> Default : figures.md
+
+      follow_nav_structure: true # Optional --> Default : true
+      
+      on_mermaid: true # Optional --> Default : false
+      on_codeblock: true # Optional --> Default : false
+      on_table: true # Optional --> Default : false
+```
+
+As you can see, every option is optional, but if you want to generate a table of figures in another language than English, you will need to set up label options.
+
+- `title_label` - This is the title (heading 1) given to the page that will contain the table of figures.
+- `figure_label` - This is the name given to every figure right before the auto-incremented number.
+- `description_label` - This is the label given to the column containing the description of each figure (alt text).
+- `temp_dir` - The temporary directory used to store the table of figures `Markdown` file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
+- `file` - The name of the `Markdown` file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
+- `follow_nav_structure` - To order the figures in function of the navigation instead of alphabetical files order.
+- `on_mermaid` - To enable `mermaid` diagrams support, need to use of `md_in_html` `Markdown` extension.
+- `on_codeblock` - To enable code blocks support, need to use of `md_in_html` `Markdown` extension.
+- `on_table` - To enable tables support, need to use of `md_in_html` `Markdown` extension.
+
+## Usage
+
+The plugin will only look for `Markdown` image composed of alt text. If you don't set any alt text for the `Markdown` image it will be ignored.
+
+There is two way of correctly rendering image stored within the docs:
+
+- Using url from base: this mean that you give the full path from the docs directory starting with `/` like this `/path/to/image/from/docs/image.png`
+- With the help of `md_in_html`: there is a `Markdown` extension that you can set in `mkdocs.yml` that allow the plugin to place `Markdown` in `HTML` which allow this plugin to let `MkDocs` set relative link in src attribute properly during `HTML` rendering
+
+Concerning external images nothing change.
+
+You can set the `md_in_html` option like so :
+
+``` yaml
+markdown_extensions:
+  - md_in_html
+```
+
+Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
+
+## Support
+
+This plugin currently supports markdown images, `mermaid` diagrams, code blocks and table.
+
+To make a `mermaid` diagram, code block or table detectable by this plugin, you need to give it a title at the line just below it like this:
+
+``` markdown
+    ``` php
+    <?php
+      $var = 42;
+    ?>
+    ```
+    The title of the code block go here
+```
+
+``` markdown
+    ``` mermaid
+    sequenceDiagram
+        participant Alice
+        participant Bob
+        Alice->>John: Hello John, how are you?
+        loop Healthcheck
+            John->>John: Fight against hypochondria
+        end
+        Note right of John: Rational thoughts <br/>prevail!
+        John-->>Alice: Great!
+        John->>Bob: How about you?
+        Bob-->>John: Jolly good!
+    ```
+    The title of the mermaid diagram go here
+```
+
+``` markdown
+    | Table   | Right | Center  | Left  |
+    | ------- | ----: | :-----: | :---- |
+    | A table |  With | Content | in it |
+    The title of the table go here
+```
+
+It will not work if there is a line between the element and the title.
+
+I highly recommend using `mkdocs-material` to use `mermaid` diagrams. For more info about `mermaid` diagrams, I invite you to check `mkdocs-material` and `mermaid`'s official documentation.
+
+I also recommend to add this stylesheet to prevent mermaid size from being reduced or code blocks from having code centered by mkdocs-material.
+
+``` css
+figure.figure-mermaid {
+    margin: 0 1em;
+    width: 100%;
+}
+
+figure.figure-codeblock code {
+    text-align: initial;
+}
+```
+
+You can place the stylesheet in your `mkdocs.yml` at extra-css option
+
+``` yml
+extra_css:
+  - fix-mermaid-figure.css
+```
+
+## License
+
+This project is under MIT license. See the `license` file for more details.
+
+## See Also
+
+- [GitLab Repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-table-of-figures/)
+- [MkDocs Website](http://www.mkdocs.org/)
+- [MkDocs-Material Documentation](https://squidfunk.github.io/mkdocs-material/)
+- [Mermaid Documentation](https://mermaid.org/intro/)
+
```

### Comparing `mkdocs-table-of-figures-0.2.0/changelog.md` & `mkdocs-table-of-figures-0.2.2/changelog.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,33 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on Keep a Changelog, and this project adheres to Semantic Versioning.
 
+## [0.2.2] - 2024-04-23
+
+### Fixed
+
+- removed the gap in the indexing jump for navigation order created by ignored elements (elements without alt text or caption)
+
+## [0.2.1] - 2024-04-19
+
+### Added
+
+- options to enable/disable navigation order for the number of each figures
+
+## [0.2.0] - 2024-04-19
+
+### Added
+
+- support for code blocks
+- support for tables
+- options to enable/disable supports for mermaid, code blocks and tables
+
 ## [0.1.7] - 2024-04-17
 
 ### Added
 
 - specific class to mermaid figure to let user fix width if needed in `plugin.py`
 
 ## [0.1.6] - 2024-04-15
```

### Comparing `mkdocs-table-of-figures-0.2.0/license` & `mkdocs-table-of-figures-0.2.2/license`

 * *Files identical despite different names*

### Comparing `mkdocs-table-of-figures-0.2.0/mkdocs_table_of_figures/plugin.py` & `mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 File: mkdocs_table_of_figures/plugin.py
 Desc: This file contain the plugin used by mkdocs create the table of figures
 Author: Thibaud Briard - BRT, <thibaud.brrd@eduge.ch>
 Version: 0.1.4 - 2023-05-10
 """
 # Imports...
 import os, shutil # used to create folder and file in documentation
+import subprocess # used to call mermaid cli to prerender diagrams
 import re # used to recognize markdown figure pattern
 import logging # used to log warning and errors for MkDocs among other things
 
 from mkdocs.config.base import Config as base_config # used to create an MkDocs config class derived from MkDocs config base
 from mkdocs.plugins import BasePlugin as base_plugin # used to create an MkDocs plugin class derived from MkDocs plugin base
 from mkdocs.config import config_options as c # used for config schema type safety
 from mkdocs.structure.files import File # used to create File in documentation
@@ -17,14 +18,15 @@
 # The plugin config options
 class TableOfFiguresConfig(base_config):
     temp_dir = c.Type(str, default='temp_figures')
     file = c.Type(str, default='figures.md')
     title_label = c.Type(str, default='Table of Figures')
     figure_label = c.Type(str, default='Figure')
     description_label = c.Type(str, default='Description')
+    follow_nav_structure = c.Type(bool, default=True)
     on_mermaid = c.Type(bool, default=False)
     on_codeblock = c.Type(bool, default=False)
     on_table = c.Type(bool, default=False)
 
 # The plugin itself
 class TableOfFigures(base_plugin[TableOfFiguresConfig]):
     def __init__(self):
@@ -35,23 +37,31 @@
         self.total_time = 0
 
         self.counter = 1
         self.figures = []
         self.file_directories_count = 0
         self.file_relative_path = ''
         self.page = None
+        self.nav_structure = None
+        self.docs_dir = None
+        #self.mermaid_dir ='assets/mermaids/'
         self.keep_md_format = False
         self.listening = True
 
     def on_config(self, config):
         self.file_directories_count = self.config.file.count('/')
         self.file_relative_path = '../' * self.file_directories_count
+        self.docs_dir = config.docs_dir
         if 'markdown_extensions' in config and 'md_in_html' in config.markdown_extensions:
             self.keep_md_format = True
         return config
+    
+    def on_nav(self, nav, config, files):
+        self.nav_structure = nav
+        return
 
     def on_files(self, files, config):
         tof = os.path.join(self.config.temp_dir, self.config.file)
 
         # Create directory if it don't exist
         if not os.path.exists(os.path.dirname(tof)):
             os.makedirs(os.path.dirname(tof))
@@ -62,73 +72,116 @@
         
         # Add the tof file to the mkdocs files list
         self.page = File(self.config.file, src_dir=self.config.temp_dir, dest_dir=config.site_dir, use_directory_urls=config.use_directory_urls)
         files.append(self.page)
 
         return files
     
+    def count_previous_figures(self, page, nav_structure, depth=0):
+        found = False
+        counter = 0
+        depth_range = ''
+        for i in range(depth):
+            depth_range += '\t'
+        
+        for index, nav_item in enumerate(nav_structure):
+            addon = 0
+            if nav_item.is_page:
+                if nav_item == page:
+                    found = True
+                elif os.path.exists(os.path.join(self.docs_dir, nav_item.file.src_uri)):
+                    with open(os.path.join(self.docs_dir, nav_item.file.src_uri), 'r') as file:
+                        markdown = file.read()
+
+                    pattern_img = r'!\[([^\]]+?)\]\((.+?)\)'
+                    pattern_mermaid = r'^(``` ?(mermaid)\r?\n(.*?)```)$\r?\n^([^\n]+?)$'
+                    pattern_codeblock = r'^(``` ?([^\r\n]*)\r?\n(.*?)```)$\r?\n^([^\n]+?)$'
+                    pattern_table = r'^((?:\|[^|\r\n]*)+\|\r?\n(?:\|[-: ]*)+\|(?:\r?\n(?:\|[^|\r\n]*)+\|)*)\r?\n^([^|\n]+?)$'
+                    
+                    matches = []
+                    matches.extend(re.finditer(pattern_img, markdown, flags= re.IGNORECASE))
+                    matches.extend(re.finditer(pattern_mermaid, markdown, flags= re.MULTILINE | re.DOTALL)) if self.config.on_mermaid and not self.config.on_codeblock else None
+                    matches.extend(re.finditer(pattern_codeblock, markdown, flags= re.MULTILINE | re.DOTALL)) if self.config.on_codeblock else None
+                    matches.extend(re.finditer(pattern_table, markdown, flags= re.MULTILINE | re.DOTALL)) if self.config.on_table else None
+
+                    addon = len(matches)
+            elif nav_item.is_section:
+                found, addon = self.count_previous_figures(page, nav_item.children, depth + 1)
+            
+            counter += addon
+            if found:
+                break
+        return found, counter
+
     def on_page_markdown(self, markdown, page, config, files):
         if self.listening:
             if self.page == page.file:
-                self._logger.info(f'Populating table of figure file {self.config.file} with {self.counter} figure{"s" if self.counter else ""} ')
+                self._logger.info(f'Populating table of figure file {self.config.file} with {len(self.figures)} figure{"s" if self.counter else ""} ')
                 markdown += f'| {self.config.figure_label} | {self.config.description_label} |\n'
                 markdown += f'| -------------------------- | ------------------------------- |\n'
-                for figure in self.figures:
+                figures = sorted(self.figures, key=lambda figure: figure["number"])
+                for figure in figures:
                     markdown += f'| [{self.config.figure_label} {figure["number"]}]({figure["link"]}) | {figure["description"]} |\n'
                 
                 self.listening = False
             else:
+                if self.config.follow_nav_structure and self.nav_structure:
+                    found, counter = self.count_previous_figures(page, self.nav_structure)
+                    if found:
+                        self.counter = counter + 1
+
                 original = markdown
                 try:
                     pattern_img = r'!\[(.*?)\]\((.+?)\)'
-                    pattern_mermaid = r'^(``` ?(mermaid)\r?\n.*?```)$\r?\n^(.*?)$'
-                    pattern_codeblock = r'^(``` ?([^\r\n]*)\r?\n.*?```)$\r?\n^(.*?)$'
+                    pattern_mermaid = r'^(``` ?(mermaid)\r?\n(.*?)```)$\r?\n^(.*?)$'
+                    pattern_codeblock = r'^(``` ?([^\r\n]*)\r?\n(.*?)```)$\r?\n^(.*?)$'
                     pattern_table = r'^((?:\|[^|\r\n]*)+\|\r?\n(?:\|[-: ]*)+\|(?:\r?\n(?:\|[^|\r\n]*)+\|)*)\r?\n^([^|]*?)$'
                     
                     matches = []
                     matches.extend(re.finditer(pattern_img, markdown, flags= re.IGNORECASE))
                     matches.extend(re.finditer(pattern_mermaid, markdown, flags= re.MULTILINE | re.DOTALL)) if self.config.on_mermaid and not self.config.on_codeblock else None
                     matches.extend(re.finditer(pattern_codeblock, markdown, flags= re.MULTILINE | re.DOTALL)) if self.config.on_codeblock else None
                     matches.extend(re.finditer(pattern_table, markdown, flags= re.MULTILINE | re.DOTALL)) if self.config.on_table else None
-
                     matches = sorted(matches, key=lambda x: x.start())
 
                     position_offset = 0
                     for match in matches:
                         checkpoint = markdown
 
                         try:
                             link = f'{self.file_relative_path}{page.file.src_uri}#figure-{self.counter}'
                             replacement = match.group(0)
                             if match.re.pattern == pattern_img and match.group(1):
                                 self.figures.append({"number": self.counter, "description": match.group(1), "link": link})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n  <img src="{config.site_url + match.group(2) if match.group(2).startswith("/") else match.group(2)}" alt="{match.group(1)}">\n  <figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
                                 if self.keep_md_format:
-                                    replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n  ![{match.group(1)}]({match.group(2)})\n  <figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
-                            elif (match.re.pattern == pattern_mermaid and match.group(3)) or (self.config.on_mermaid and match.re.pattern == pattern_codeblock and match.group(2) == 'mermaid' and match.group(3)):
-                                self.figures.append({"number": self.counter, "description": match.group(3), "link": link})
-                                replacement = f'<figure id="figure-{self.counter}" class="figure-mermaid" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(3)}</figcaption>\n</figure>'
-                            elif match.re.pattern == pattern_codeblock and match.group(2) != 'mermaid' and match.group(3):
-                                self.figures.append({"number": self.counter, "description": match.group(3), "link": link})
-                                replacement = f'<figure id="figure-{self.counter}" class="figure-codeblock" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(3)}</figcaption>\n</figure>'
+                                    replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n![{match.group(1)}]({match.group(2)})\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
+                            elif (match.re.pattern == pattern_mermaid and match.group(4)) or (self.config.on_mermaid and match.re.pattern == pattern_codeblock and match.group(2) == 'mermaid' and match.group(4)):
+                                self.figures.append({"number": self.counter, "description": match.group(4), "link": link})
+                                replacement = f'<figure id="figure-{self.counter}" class="figure-mermaid" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(4)}</figcaption>\n</figure>'
+                            elif match.re.pattern == pattern_codeblock and match.group(2) != 'mermaid' and match.group(4):
+                                self.figures.append({"number": self.counter, "description": match.group(4), "link": link})
+                                replacement = f'<figure id="figure-{self.counter}" class="figure-codeblock" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(4)}</figcaption>\n</figure>'
                             elif match.re.pattern == pattern_table and match.group(2):
                                 self.figures.append({"number": self.counter, "description": match.group(2), "link": link})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-table" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(2)}</figcaption>\n</figure>'
                             
                             if replacement == match.group(0):
                                 self._logger.debug(f'Ignoring image/diagram at {self.file_relative_path}{page.file.src_uri}')
                             else:
                                 self._logger.debug(f'Formating image/diagram as figure at {self.file_relative_path}{page.file.src_uri}')
                                 self.counter += 1
                                 markdown = markdown[:match.start() + position_offset] + replacement + markdown[match.end() + position_offset:]
                                 position_offset += len(replacement) - len(match.group(0))
-                        except:
+                        except Exception as error:
+                            self._logger.warning(error)
                             markdown = checkpoint
                             
-                except:
+                except Exception as error:
+                    self._logger.warning(error)
                     markdown = original
 
         return markdown
     
     
     def on_post_build(self, config):
         # Removing temp_dir directory
```

### Comparing `mkdocs-table-of-figures-0.2.0/mkdocs_table_of_figures.egg-info/PKG-INFO` & `mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,151 +1,156 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.2.0
+Version: 0.2.2
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
-Description: # mkdocs-table-of-figures
-        
-        This is a plugin that creates a `figcaption` with elements `alt` attribute or title and lists all figures in files into a table of figures to be integrated in `Markdown` pages for MkDocs.
-        
-        ## Setup
-        
-        ### Installing using pip:
-        
-        `pip install mkdocs-table-of-figures`
-        
-        ## Config
-        
-        You need to activate the plugin in `mkdocs.yml`:
-        
-        ``` yaml
-        plugins:
-          - table-of-figures:
-              title_label: "Table of figures of the documentation" # Optional --> Default : Table of Figures
-              figure_label: "Figure N°" # Optional --> Default : Figure
-              description_label: "Description of the figures" # Optional --> Default : Description
-        
-              temp_dir: "folder_name" # Optional --> Default : temp_figures
-              file: "file_name" # Optional --> Default : figures.md
-              
-              on_mermaid: true # Optional --> Default : false
-              on_codeblock: true # Optional --> Default : false
-              on_table: true # Optional --> Default : false
-        ```
-        
-        As you can see, every option is optional, but if you want to generate a table of figures in another language than English, you will need to set up label options.
-        
-        - `title_label` - This is the title (heading 1) given to the page that will contain the table of figures.
-        - `figure_label` - This is the name given to every figure right before the auto-incremented number.
-        - `description_label` - This is the label given to the column containing the description of each figure (alt text).
-        - `temp_dir` - The temporary directory used to store the table of figures `Markdown` file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
-        - `file` - The name of the `Markdown` file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
-        - `on_mermaid` - To enable `mermaid` diagrams support, need to use of `md_in_html` `Markdown` extension
-        - `on_codeblock` - To enable code blocks support, need to use of `md_in_html` `Markdown` extension
-        - `on_table` - To enable tables support, need to use of `md_in_html` `Markdown` extension
-        
-        ## Usage
-        
-        The plugin will only look for `Markdown` image composed of alt text. If you don't set any alt text for the `Markdown` image it will be ignored.
-        
-        There is two way of correctly rendering image stored within the docs:
-        
-        - Using url from base: this mean that you give the full path from the docs directory starting with `/` like this `/path/to/image/from/docs/image.png`
-        - With the help of `md_in_html`: there is a `Markdown` extension that you can set in `mkdocs.yml` that allow the plugin to place `Markdown` in `HTML` which allow this plugin to let `MkDocs` set relative link in src attribute properly during `HTML` rendering
-        
-        Concerning external images nothing change.
-        
-        You can set the `md_in_html` option like so :
-        
-        ``` yaml
-        markdown_extensions:
-          - md_in_html
-        ```
-        
-        Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
-        
-        ## Support
-        
-        This plugin currently supports markdown images, `mermaid` diagrams, code blocks and table.
-        
-        To make a `mermaid` diagram, code block or table detectable by this plugin, you need to give it a title at the line just below it like this:
-        
-        ``` markdown
-            ``` php
-            <?php
-              $var = 42;
-            ?>
-            ```
-            The title of the code block go here
-        ```
-        
-        ``` markdown
-            ``` mermaid
-            sequenceDiagram
-                participant Alice
-                participant Bob
-                Alice->>John: Hello John, how are you?
-                loop Healthcheck
-                    John->>John: Fight against hypochondria
-                end
-                Note right of John: Rational thoughts <br/>prevail!
-                John-->>Alice: Great!
-                John->>Bob: How about you?
-                Bob-->>John: Jolly good!
-            ```
-            The title of the mermaid diagram go here
-        ```
-        
-        ``` markdown
-            | Table   | Right | Center  | Left  |
-            | ------- | ----: | :-----: | :---- |
-            | A table |  With | Content | in it |
-            The title of the table go here
-        ```
-        
-        It will not work if there is a line between the element and the title.
-        
-        I highly recommend using `mkdocs-material` to use `mermaid` diagrams. For more info about `mermaid` diagrams, I invite you to check `mkdocs-material` and `mermaid`'s official documentation.
-        
-        I also recommend to add this stylesheet to prevent mermaid size from being reduced or code blocks from having code centered by mkdocs-material.
-        
-        ``` css
-        figure.figure-mermaid {
-            margin: 0 1em;
-            width: 100%;
-        }
-        
-        figure.figure-codeblock code {
-            text-align: initial;
-        }
-        ```
-        
-        You can place the stylesheet in your `mkdocs.yml` at extra-css option
-        
-        ``` yml
-        extra_css:
-          - fix-mermaid-figure.css
-        ```
-        
-        ## License
-        
-        This project is under MIT license. See the `license` file for more details.
-        
-        ## See Also
-        
-        - [GitLab Repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-table-of-figures/)
-        - [MkDocs Website](http://www.mkdocs.org/)
-        - [MkDocs-Material Documentation](https://squidfunk.github.io/mkdocs-material/)
-        - [Mermaid Documentation](https://mermaid.org/intro/)
 Keywords: mkdocs
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+
+# mkdocs-table-of-figures
+
+This is a plugin that creates a `figcaption` with elements `alt` attribute or title and lists all figures in files into a table of figures to be integrated in `Markdown` pages for MkDocs.
+
+## Setup
+
+### Installing using pip:
+
+`pip install mkdocs-table-of-figures`
+
+## Config
+
+You need to activate the plugin in `mkdocs.yml`:
+
+``` yaml
+plugins:
+  - table-of-figures:
+      title_label: "Table of figures of the documentation" # Optional --> Default : Table of Figures
+      figure_label: "Figure N°" # Optional --> Default : Figure
+      description_label: "Description of the figures" # Optional --> Default : Description
+
+      temp_dir: "folder_name" # Optional --> Default : temp_figures
+      file: "file_name" # Optional --> Default : figures.md
+
+      follow_nav_structure: true # Optional --> Default : true
+      
+      on_mermaid: true # Optional --> Default : false
+      on_codeblock: true # Optional --> Default : false
+      on_table: true # Optional --> Default : false
+```
+
+As you can see, every option is optional, but if you want to generate a table of figures in another language than English, you will need to set up label options.
+
+- `title_label` - This is the title (heading 1) given to the page that will contain the table of figures.
+- `figure_label` - This is the name given to every figure right before the auto-incremented number.
+- `description_label` - This is the label given to the column containing the description of each figure (alt text).
+- `temp_dir` - The temporary directory used to store the table of figures `Markdown` file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
+- `file` - The name of the `Markdown` file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
+- `follow_nav_structure` - To order the figures in function of the navigation instead of alphabetical files order.
+- `on_mermaid` - To enable `mermaid` diagrams support, need to use of `md_in_html` `Markdown` extension.
+- `on_codeblock` - To enable code blocks support, need to use of `md_in_html` `Markdown` extension.
+- `on_table` - To enable tables support, need to use of `md_in_html` `Markdown` extension.
+
+## Usage
+
+The plugin will only look for `Markdown` image composed of alt text. If you don't set any alt text for the `Markdown` image it will be ignored.
+
+There is two way of correctly rendering image stored within the docs:
+
+- Using url from base: this mean that you give the full path from the docs directory starting with `/` like this `/path/to/image/from/docs/image.png`
+- With the help of `md_in_html`: there is a `Markdown` extension that you can set in `mkdocs.yml` that allow the plugin to place `Markdown` in `HTML` which allow this plugin to let `MkDocs` set relative link in src attribute properly during `HTML` rendering
+
+Concerning external images nothing change.
+
+You can set the `md_in_html` option like so :
+
+``` yaml
+markdown_extensions:
+  - md_in_html
+```
+
+Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
+
+## Support
+
+This plugin currently supports markdown images, `mermaid` diagrams, code blocks and table.
+
+To make a `mermaid` diagram, code block or table detectable by this plugin, you need to give it a title at the line just below it like this:
+
+``` markdown
+    ``` php
+    <?php
+      $var = 42;
+    ?>
+    ```
+    The title of the code block go here
+```
+
+``` markdown
+    ``` mermaid
+    sequenceDiagram
+        participant Alice
+        participant Bob
+        Alice->>John: Hello John, how are you?
+        loop Healthcheck
+            John->>John: Fight against hypochondria
+        end
+        Note right of John: Rational thoughts <br/>prevail!
+        John-->>Alice: Great!
+        John->>Bob: How about you?
+        Bob-->>John: Jolly good!
+    ```
+    The title of the mermaid diagram go here
+```
+
+``` markdown
+    | Table   | Right | Center  | Left  |
+    | ------- | ----: | :-----: | :---- |
+    | A table |  With | Content | in it |
+    The title of the table go here
+```
+
+It will not work if there is a line between the element and the title.
+
+I highly recommend using `mkdocs-material` to use `mermaid` diagrams. For more info about `mermaid` diagrams, I invite you to check `mkdocs-material` and `mermaid`'s official documentation.
+
+I also recommend to add this stylesheet to prevent mermaid size from being reduced or code blocks from having code centered by mkdocs-material.
+
+``` css
+figure.figure-mermaid {
+    margin: 0 1em;
+    width: 100%;
+}
+
+figure.figure-codeblock code {
+    text-align: initial;
+}
+```
+
+You can place the stylesheet in your `mkdocs.yml` at extra-css option
+
+``` yml
+extra_css:
+  - fix-mermaid-figure.css
+```
+
+## License
+
+This project is under MIT license. See the `license` file for more details.
+
+## See Also
+
+- [GitLab Repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-table-of-figures/)
+- [MkDocs Website](http://www.mkdocs.org/)
+- [MkDocs-Material Documentation](https://squidfunk.github.io/mkdocs-material/)
+- [Mermaid Documentation](https://mermaid.org/intro/)
+
```

### Comparing `mkdocs-table-of-figures-0.2.0/readme.md` & `mkdocs-table-of-figures-0.2.2/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,30 +17,33 @@
   - table-of-figures:
       title_label: "Table of figures of the documentation" # Optional --> Default : Table of Figures
       figure_label: "Figure N°" # Optional --> Default : Figure
       description_label: "Description of the figures" # Optional --> Default : Description
 
       temp_dir: "folder_name" # Optional --> Default : temp_figures
       file: "file_name" # Optional --> Default : figures.md
+
+      follow_nav_structure: true # Optional --> Default : true
       
       on_mermaid: true # Optional --> Default : false
       on_codeblock: true # Optional --> Default : false
       on_table: true # Optional --> Default : false
 ```
 
 As you can see, every option is optional, but if you want to generate a table of figures in another language than English, you will need to set up label options.
 
 - `title_label` - This is the title (heading 1) given to the page that will contain the table of figures.
 - `figure_label` - This is the name given to every figure right before the auto-incremented number.
 - `description_label` - This is the label given to the column containing the description of each figure (alt text).
 - `temp_dir` - The temporary directory used to store the table of figures `Markdown` file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
 - `file` - The name of the `Markdown` file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
-- `on_mermaid` - To enable `mermaid` diagrams support, need to use of `md_in_html` `Markdown` extension
-- `on_codeblock` - To enable code blocks support, need to use of `md_in_html` `Markdown` extension
-- `on_table` - To enable tables support, need to use of `md_in_html` `Markdown` extension
+- `follow_nav_structure` - To order the figures in function of the navigation instead of alphabetical files order.
+- `on_mermaid` - To enable `mermaid` diagrams support, need to use of `md_in_html` `Markdown` extension.
+- `on_codeblock` - To enable code blocks support, need to use of `md_in_html` `Markdown` extension.
+- `on_table` - To enable tables support, need to use of `md_in_html` `Markdown` extension.
 
 ## Usage
 
 The plugin will only look for `Markdown` image composed of alt text. If you don't set any alt text for the `Markdown` image it will be ignored.
 
 There is two way of correctly rendering image stored within the docs:
```

### Comparing `mkdocs-table-of-figures-0.2.0/setup.py` & `mkdocs-table-of-figures-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-table-of-figures',
-    version='0.2.0',
+    version='0.2.2',
     description='A MkDocs plugin listing all figures to create a table of figures page',
     long_description=io.open('readme.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
```

