# Comparing `tmp/roff-0.1.0.tar.gz` & `tmp/roff-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roff-0.1.0.tar", last modified: Mon Apr 22 09:21:50 2024, max compression
+gzip compressed data, was "roff-0.2.0.tar", last modified: Tue Apr 23 11:36:40 2024, max compression
```

## Comparing `roff-0.1.0.tar` & `roff-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-22 09:21:50.844196 roff-0.1.0/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1072 2024-04-21 09:37:21.000000 roff-0.1.0/LICENSE
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     2616 2024-04-22 09:21:50.844196 roff-0.1.0/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1367 2024-04-22 09:20:48.000000 roff-0.1.0/README.md
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-22 09:21:50.844196 roff-0.1.0/docs/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      973 2024-04-22 09:12:46.000000 roff-0.1.0/docs/roff.1
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-21 09:38:29.000000 roff-0.1.0/pyproject.toml
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-04-22 09:21:50.844196 roff-0.1.0/setup.cfg
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1940 2024-04-22 09:19:03.000000 roff-0.1.0/setup.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-22 09:21:50.844196 roff-0.1.0/src/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-22 09:21:50.844196 roff-0.1.0/src/roff/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-22 09:21:50.844196 roff-0.1.0/src/roff/__cli__/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       78 2024-04-21 12:02:06.000000 roff-0.1.0/src/roff/__cli__/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      513 2024-04-21 12:31:53.000000 roff-0.1.0/src/roff/__cli__/convert.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      632 2024-04-21 10:35:06.000000 roff-0.1.0/src/roff/__cli__/template.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1508 2024-04-22 09:17:21.000000 roff-0.1.0/src/roff/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1239 2024-04-22 09:05:54.000000 roff-0.1.0/src/roff/__main__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     5727 2024-04-22 09:12:39.000000 roff-0.1.0/src/roff/convert.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-22 09:21:50.844196 roff-0.1.0/src/roff.egg-info/
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     2616 2024-04-22 09:21:50.000000 roff-0.1.0/src/roff.egg-info/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      395 2024-04-22 09:21:50.000000 roff-0.1.0/src/roff.egg-info/SOURCES.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-04-22 09:21:50.000000 roff-0.1.0/src/roff.egg-info/dependency_links.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       44 2024-04-22 09:21:50.000000 roff-0.1.0/src/roff.egg-info/entry_points.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       15 2024-04-22 09:21:50.000000 roff-0.1.0/src/roff.egg-info/requires.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        5 2024-04-22 09:21:50.000000 roff-0.1.0/src/roff.egg-info/top_level.txt
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-23 11:36:40.850998 roff-0.2.0/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1072 2024-04-23 10:39:23.000000 roff-0.2.0/LICENSE
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     2759 2024-04-23 11:36:40.850998 roff-0.2.0/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1510 2024-04-23 10:39:23.000000 roff-0.2.0/README.md
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-23 11:36:40.846997 roff-0.2.0/docs/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1354 2024-04-23 11:36:29.000000 roff-0.2.0/docs/roff.1
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-23 10:39:23.000000 roff-0.2.0/pyproject.toml
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-04-23 11:36:40.850998 roff-0.2.0/setup.cfg
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1940 2024-04-23 10:39:23.000000 roff-0.2.0/setup.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-23 11:36:40.846997 roff-0.2.0/src/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-23 11:36:40.846997 roff-0.2.0/src/roff/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-23 11:36:40.850998 roff-0.2.0/src/roff/__cli__/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       78 2024-04-23 10:39:23.000000 roff-0.2.0/src/roff/__cli__/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      513 2024-04-23 10:39:23.000000 roff-0.2.0/src/roff/__cli__/convert.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      950 2024-04-23 10:56:38.000000 roff-0.2.0/src/roff/__cli__/template.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1508 2024-04-23 11:36:18.000000 roff-0.2.0/src/roff/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1457 2024-04-23 10:54:12.000000 roff-0.2.0/src/roff/__main__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     6732 2024-04-23 11:33:32.000000 roff-0.2.0/src/roff/convert.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-23 11:36:40.850998 roff-0.2.0/src/roff.egg-info/
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     2759 2024-04-23 11:36:40.000000 roff-0.2.0/src/roff.egg-info/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      395 2024-04-23 11:36:40.000000 roff-0.2.0/src/roff.egg-info/SOURCES.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-04-23 11:36:40.000000 roff-0.2.0/src/roff.egg-info/dependency_links.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       44 2024-04-23 11:36:40.000000 roff-0.2.0/src/roff.egg-info/entry_points.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       15 2024-04-23 11:36:40.000000 roff-0.2.0/src/roff.egg-info/requires.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        5 2024-04-23 11:36:40.000000 roff-0.2.0/src/roff.egg-info/top_level.txt
```

### Comparing `roff-0.1.0/LICENSE` & `roff-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roff-0.1.0/PKG-INFO` & `roff-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roff
-Version: 0.1.0
+Version: 0.2.0
 Summary: python-based cli to convert markdown to the roff (man-pages) format
 Home-page: https://github.com/utility-toolbox/roff
 Author: PlayerG9
 License: MIT
 Project-URL: Organisation Github, https://github.com/utility-toolbox
 Project-URL: Homepage, https://github.com/utility-toolbox/roff/
 Project-URL: Bug Tracker, https://github.com/utility-toolbox/roff/issues
@@ -43,22 +43,23 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/roff)
 ](https://pypi.org/project/roff/)
 
 ```shell
 pip install roff
 ```
 
-> Tip: after the installation you should be able to see roff's manpage with `man roff` 
+> Tip: after the installation you should be able to see [roff's manpage](https://github.com/utility-toolbox/roff/blob/main/docs/roff.1.md) with `man roff` 
 
 ## Usage/Execution
 
 ```shell
 roff --help
 roff template command.1.md
 roff convert command.1.md
+man ./command.1
 ```
 
 ## Example
 
 ````markdown
 roff(1) -- python-based cli to convert markdown to the roff (man-pages) format
 =============================================
@@ -109,8 +110,8 @@
 https://github.com/PlayerG9
 
 ## SEE ALSO
 
 https://github.com/utility-toolbox/roff
 ````
 
-![example-manpage](README.assets/example-manpage.png)
+![example-manpage](https://github.com/utility-toolbox/roff/blob/main/README.assets/example-manpage.png?raw=true)
```

### Comparing `roff-0.1.0/README.md` & `roff-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/roff)
 ](https://pypi.org/project/roff/)
 
 ```shell
 pip install roff
 ```
 
-> Tip: after the installation you should be able to see roff's manpage with `man roff` 
+> Tip: after the installation you should be able to see [roff's manpage](https://github.com/utility-toolbox/roff/blob/main/docs/roff.1.md) with `man roff` 
 
 ## Usage/Execution
 
 ```shell
 roff --help
 roff template command.1.md
 roff convert command.1.md
+man ./command.1
 ```
 
 ## Example
 
 ````markdown
 roff(1) -- python-based cli to convert markdown to the roff (man-pages) format
 =============================================
@@ -79,8 +80,8 @@
 https://github.com/PlayerG9
 
 ## SEE ALSO
 
 https://github.com/utility-toolbox/roff
 ````
 
-![example-manpage](README.assets/example-manpage.png)
+![example-manpage](https://github.com/utility-toolbox/roff/blob/main/README.assets/example-manpage.png?raw=true)
```

### Comparing `roff-0.1.0/docs/roff.1` & `roff-0.2.0/docs/roff.1`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,89 @@
-.\" generated with roff/v0.1.0
-.\" https://pypi.org/project/roff/0.1.0
+.\" generated with roff/v0.2.0
+.\" https://pypi.org/project/roff/0.2.0
 .\" https://github.com/utility-toolbox/roff/
 .\"
-.TH "ROFF" "1" "22 April 2024" "github.com/utility-toolbox/roff"
+.TH "ROFF" "1" "23 April 2024" "github.com/utility-toolbox/roff"
 .SH "NAME"
 \fBroff\fP \- python-based cli to convert markdown to the roff (man-pages) format
 .SH "SYNOPSIS"
-.TP
+.br
+*
+.RS 2
 \fBroff [-h] [-v] {convert,template} ...\fP
-.TP
+.RE
+*
+.RS 2
 \fBroff convert [-h] source [dest]\fP
-.TP
+.RE
+*
+.RS 2
 \fBroff template [-h] dest\fP
+.RE
+.br
 .SH "DESCRIPTION"
 python-based cli to convert markdown to the roff (man-pages) format\.
+Supported Markdown Features:
+.br
+*
+.RS 2
+heading (h2-h4) (h1 is reserved for the head)
+.RE
+*
+.RS 2
+Flat Lists
+.RE
+*
+.RS 2
+code-blocks
+.RE
+*
+.RS 2
+inline-code
+.RE
+*
+.RS 2
+inline-bold
+.RE
+*
+.RS 2
+inline-italic
+.RE
+.br
 .SH "OPTIONS"
 .SS "\fBconvert\fP"
 .sp
 .RS 2
 Converts markdown to roff
 .RE
 .sp
-.TP
+.sp
 \fBsource\fP:
 .br
 Markdown file that should be parsed
-.TP
+.sp
 \fB[dest]\fP:
 .br
 Manpage file
 .SS "\fBtemplate\fP"
 .sp
 .RS 2
 Generates a Markdown file that you can fill
 .RE
 .sp
-.TP
+.sp
+\fB-y\fP, \fB--yes\fP:
+.br
+Overwrite file if it exists
+.sp
 \fBdest\fP:
 .br
 Target file that should be generated
 .SH "BUGS"
 https://github\.com/utility-toolbox/roff/issues
 .SH "AUTHOR"
 https://github\.com/PlayerG9
 .SH "SEE ALSO"
+.SS "Organisation:"
+https://github\.com/utility-toolbox
+.SS "Repository:"
 https://github\.com/utility-toolbox/roff
```

### Comparing `roff-0.1.0/setup.py` & `roff-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `roff-0.1.0/src/roff/__cli__/convert.py` & `roff-0.2.0/src/roff/__cli__/convert.py`

 * *Files identical despite different names*

### Comparing `roff-0.1.0/src/roff/__cli__/template.py` & `roff-0.2.0/src/roff/__cli__/template.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,34 +4,45 @@
 """
 from pathlib import Path
 
 
 __all__ = ['__cmd__']
 
 
-def __cmd__(dest: str) -> None:
+def __cmd__(dest: str, *, yes: bool) -> None:
     dest = Path(dest)
     if not dest.parent.is_dir():
         raise NotADirectoryError(f"parent directory '{dest.parent!s}' does not exist")
+    if dest.is_file() and not yes:
+        response = input(f"'{dest!s}' already exists. Do you want to overwrite it? [Y/n] ")
+        if response.lower() not in {'y', 'yes'}:
+            exit(0)
 
     command = dest.name.split('.', 1)[0]
     manpage_area = next((int(sfx[1]) for sfx in dest.suffixes if sfx[1:].isdigit() and len(sfx) == 2), 1)
 
     with open(dest, 'w') as f:
         f.write(fr"""{command}({manpage_area}) -- @DESCRIPTION
 =============================================
 
 ## SYNOPSIS
 
+- `{command} [-h]`
 
 ## DESCRIPTION
 
 
 ## OPTIONS
 
+<!--
+### `{command} <SUBCOMMAND>`
+-->
+
+* `-h`, `--help`:
+show the help message and exits
 
 ## BUGS
 
 
 ## AUTHOR
```

### Comparing `roff-0.1.0/src/roff/__init__.py` & `roff-0.2.0/src/roff/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 __copyright__ = "Copyright 2024, utility-toolbox"
 __credits__ = ["PlayerG9"]
 __license__ = "MIT"
 __maintainer__ = "PlayerG9"
 __email__ = None
 __status__ = "Prototype"  # Prototype, Development, Production
 __description__ = "python-based cli to convert markdown to the roff (man-pages) format"
-__version_info__ = (0, 1, 0)
+__version_info__ = (0, 2, 0)
 __version__ = '.'.join(str(_) for _ in __version_info__)
```

### Comparing `roff-0.1.0/src/roff/__main__.py` & `roff-0.2.0/src/roff/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding=utf-8 -*-
 r"""
-
+python-based cli to convert markdown to the roff (man-pages) format
 """
 import argparse as ap
 from . import __version__, __cli__
 
 
-parser = ap.ArgumentParser(prog='roff', formatter_class=ap.ArgumentDefaultsHelpFormatter)
+parser = ap.ArgumentParser(prog='roff', formatter_class=ap.ArgumentDefaultsHelpFormatter, description=__doc__)
 parser.set_defaults(__cmd__=parser.print_help)
 parser.add_argument('-v', '--version', action='version', version='{}'.format(__version__))
 subparsers = parser.add_subparsers()
 
 
 convert_parser = subparsers.add_parser('convert',
                                        help="Converts markdown to roff")
@@ -20,14 +20,16 @@
 convert_parser.add_argument('dest', nargs=ap.OPTIONAL,
                             help="Manpage file that should be generated")
 
 
 template_parser = subparsers.add_parser('template',
                                         help="Generates a Markdown file that you can fill")
 template_parser.set_defaults(__cmd__=__cli__.template.__cmd__)
+template_parser.add_argument('-y', '--yes', action='store_true',
+                             help="Overwrite file if it exists")
 template_parser.add_argument('dest',
                              help="Target file that should be generated")
 
 
 def main():
     args = vars(parser.parse_args())
     cmd = args.pop('__cmd__')
```

### Comparing `roff-0.1.0/src/roff/convert.py` & `roff-0.2.0/src/roff/convert.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,27 +22,34 @@
     :param source: markdown file content
     :return: roff file content
     """
     return Converter(source).getvalue()
 
 
 class Converter:
+    _stream: io.StringIO
+    _had_head: bool
+    manpage_area: int
+
     def __init__(self, source: str) -> None:
         self._stream = io.StringIO()
+        self._had_head = False
 
         self.manpage_area = 1  # default. should be overwritten
 
         parser = markdown_it.MarkdownIt()
 
         tokens = parser.parse(src=source)
         root_node = markdown_it.tree.SyntaxTreeNode(tokens=tokens, create_root=True)
 
         self._add_head()
         # print(root_node.pretty(show_text=True))
         self._parse_children(children=root_node.children)
+        if not self._had_head:
+            raise SyntaxError("Missing head")
 
     def getvalue(self) -> str:
         return self._stream.getvalue()
 
     def _add_head(self):
         self._stream.write(f".\\\" generated with roff/v{__version__}\n")
         self._stream.write(f".\\\" https://pypi.org/project/roff/{__version__}\n")
@@ -50,14 +57,16 @@
         self._stream.write(f".\\\"\n")
 
     def _parse_children(self, children: t.List[markdown_it.tree.SyntaxTreeNode]) -> None:
         for child in children:
             self._parse_node(node=child)
 
     def _parse_node(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
+        if not self._had_head and node.tag != 'h1':
+            raise SyntaxError("First element in the document should be the header")
         parser = getattr(self, f"_parse_{node.tag}", None)
         if parser is None:
             warnings.warn(f"Unsupported node tag '{node.tag}' of type '{node.type}'", RuntimeWarning)
             return
         parser(node=node)
 
     def _parse_inline(self, node: markdown_it.tree.SyntaxTreeNode) -> str:
@@ -88,14 +97,19 @@
             else:
                 warnings.warn(f"Unsupported inline node tag '{child.tag}' of type '{child.type}'", RuntimeWarning)
 
         return ''.join(chunks)
 
     def _parse_h1(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         from datetime import date
+
+        if self._had_head:
+            raise SyntaxError("Duplicate Head detected")
+        self._had_head = True
+
         head_re = re.compile(r'^(?P<command>\w+)\\?\((?P<manpage_area>\d)\\?\) \\?-\\?- (?P<description>.+)$')
         content = self._parse_inline(node=node.children[0])
         match = head_re.search(content)
         if match is None:
             raise SyntaxError("Unsupported format of head. (expected 'command(1) -- description')")
 
         command = match.group('command')
@@ -110,28 +124,41 @@
 
     def _parse_h2(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         self._stream.write(f'.SH "{self._parse_inline(node=node.children[0])}"\n')
 
     def _parse_h3(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         self._stream.write(f'.SS "{self._parse_inline(node=node.children[0])}"\n')
 
+    def _parse_h4(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
+        self._stream.write(f'.sp\n{self._parse_inline(node=node.children[0])}\n.br\n')
+
     def _parse_p(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         content = self._parse_inline(node=node.children[0])
         if not content.strip():
             return
         content = re.sub(r'\n{2,}', '\n.\n', content)
         self._stream.write(f'{content}\n')
 
     def _parse_ul(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
-        self._parse_children(children=node.children)
-
-    def _parse_li(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
+        r""" unordered list """
+        self._stream.write('.br\n')
         for child in node.children:
-            self._stream.write('.TP\n')
-            self._parse_node(node=child)
+            self._stream.write(f'*\n.RS 2\n')
+            self._parse_children(children=child.children)
+            self._stream.write(f'.RE\n')
+        self._stream.write('.br\n')
+
+    def _parse_ol(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
+        r""" ordered list """
+        self._stream.write('.br\n')
+        for i, child in enumerate(node.children):
+            self._stream.write(f'{i+1}.\n.RS 2\n')
+            self._parse_children(children=child.children)
+            self._stream.write(f'.RE\n')
+        self._stream.write('.br\n')
 
     def _parse_blockquote(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         self._stream.write(f'.sp\n.RS 2\n')
         self._parse_children(children=node.children)
         self._stream.write(f'.RE\n.sp\n')
 
     def _parse_code(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
```

### Comparing `roff-0.1.0/src/roff.egg-info/PKG-INFO` & `roff-0.2.0/src/roff.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roff
-Version: 0.1.0
+Version: 0.2.0
 Summary: python-based cli to convert markdown to the roff (man-pages) format
 Home-page: https://github.com/utility-toolbox/roff
 Author: PlayerG9
 License: MIT
 Project-URL: Organisation Github, https://github.com/utility-toolbox
 Project-URL: Homepage, https://github.com/utility-toolbox/roff/
 Project-URL: Bug Tracker, https://github.com/utility-toolbox/roff/issues
@@ -43,22 +43,23 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/roff)
 ](https://pypi.org/project/roff/)
 
 ```shell
 pip install roff
 ```
 
-> Tip: after the installation you should be able to see roff's manpage with `man roff` 
+> Tip: after the installation you should be able to see [roff's manpage](https://github.com/utility-toolbox/roff/blob/main/docs/roff.1.md) with `man roff` 
 
 ## Usage/Execution
 
 ```shell
 roff --help
 roff template command.1.md
 roff convert command.1.md
+man ./command.1
 ```
 
 ## Example
 
 ````markdown
 roff(1) -- python-based cli to convert markdown to the roff (man-pages) format
 =============================================
@@ -109,8 +110,8 @@
 https://github.com/PlayerG9
 
 ## SEE ALSO
 
 https://github.com/utility-toolbox/roff
 ````
 
-![example-manpage](README.assets/example-manpage.png)
+![example-manpage](https://github.com/utility-toolbox/roff/blob/main/README.assets/example-manpage.png?raw=true)
```

