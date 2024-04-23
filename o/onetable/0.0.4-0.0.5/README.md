# Comparing `tmp/onetable-0.0.4.tar.gz` & `tmp/onetable-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onetable-0.0.4.tar", last modified: Wed May 27 07:38:00 2020, max compression
+gzip compressed data, was "dist/onetable-0.0.5.tar", last modified: Tue Apr 23 02:18:51 2024, max compression
```

## Comparing `onetable-0.0.4.tar` & `onetable-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2020-05-27 07:38:00.000000 onetable-0.0.4/
--rw-r--r--   0 Robin      (501) staff       (20)     1440 2020-05-27 07:38:00.000000 onetable-0.0.4/PKG-INFO
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2020-05-27 07:38:00.000000 onetable-0.0.4/onetable/
--rw-r--r--   0 Robin      (501) staff       (20)    27172 2020-05-27 07:31:56.000000 onetable-0.0.4/onetable/__init__.py
-drwxr-xr-x   0 Robin      (501) staff       (20)        0 2020-05-27 07:38:00.000000 onetable-0.0.4/onetable.egg-info/
--rw-r--r--   0 Robin      (501) staff       (20)     1440 2020-05-27 07:37:59.000000 onetable-0.0.4/onetable.egg-info/PKG-INFO
--rw-r--r--   0 Robin      (501) staff       (20)        1 2019-06-22 09:24:07.000000 onetable-0.0.4/onetable.egg-info/not-zip-safe
--rw-r--r--   0 Robin      (501) staff       (20)      221 2020-05-27 07:37:59.000000 onetable-0.0.4/onetable.egg-info/SOURCES.txt
--rw-r--r--   0 Robin      (501) staff       (20)        9 2020-05-27 07:37:59.000000 onetable-0.0.4/onetable.egg-info/top_level.txt
--rw-r--r--   0 Robin      (501) staff       (20)        1 2020-05-27 07:37:59.000000 onetable-0.0.4/onetable.egg-info/dependency_links.txt
--rw-r--r--   0 Robin      (501) staff       (20)       12 2020-03-11 15:15:12.000000 onetable-0.0.4/MANIFEST.in
--rw-r--r--   0 Robin      (501) staff       (20)      723 2020-05-27 07:31:03.000000 onetable-0.0.4/README.md
--rwxr-xr-x   0 Robin      (501) staff       (20)      757 2019-06-22 09:22:53.000000 onetable-0.0.4/setup.py
--rw-r--r--   0 Robin      (501) staff       (20)       67 2019-06-22 09:45:21.000000 onetable-0.0.4/CHANGES.md
--rw-r--r--   0 Robin      (501) staff       (20)       38 2020-05-27 07:38:00.000000 onetable-0.0.4/setup.cfg
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2024-04-23 02:18:51.000000 onetable-0.0.5/
+-rw-r--r--   0 Robin      (501) staff       (20)     1506 2024-04-23 02:18:51.000000 onetable-0.0.5/PKG-INFO
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2024-04-23 02:18:51.000000 onetable-0.0.5/onetable/
+-rw-r--r--   0 Robin      (501) staff       (20)    27416 2024-04-23 02:16:41.000000 onetable-0.0.5/onetable/__init__.py
+drwxr-xr-x   0 Robin      (501) staff       (20)        0 2024-04-23 02:18:51.000000 onetable-0.0.5/onetable.egg-info/
+-rw-r--r--   0 Robin      (501) staff       (20)     1506 2024-04-23 02:18:51.000000 onetable-0.0.5/onetable.egg-info/PKG-INFO
+-rw-r--r--   0 Robin      (501) staff       (20)        1 2019-06-22 09:24:07.000000 onetable-0.0.5/onetable.egg-info/not-zip-safe
+-rw-r--r--   0 Robin      (501) staff       (20)      221 2024-04-23 02:18:51.000000 onetable-0.0.5/onetable.egg-info/SOURCES.txt
+-rw-r--r--   0 Robin      (501) staff       (20)        9 2024-04-23 02:18:51.000000 onetable-0.0.5/onetable.egg-info/top_level.txt
+-rw-r--r--   0 Robin      (501) staff       (20)        1 2024-04-23 02:18:51.000000 onetable-0.0.5/onetable.egg-info/dependency_links.txt
+-rw-r--r--   0 Robin      (501) staff       (20)       12 2020-03-11 15:15:12.000000 onetable-0.0.5/MANIFEST.in
+-rw-r--r--   0 Robin      (501) staff       (20)      724 2022-04-09 12:52:40.000000 onetable-0.0.5/README.md
+-rwxr-xr-x   0 Robin      (501) staff       (20)      757 2019-06-22 09:22:53.000000 onetable-0.0.5/setup.py
+-rw-r--r--   0 Robin      (501) staff       (20)      100 2024-04-23 02:17:02.000000 onetable-0.0.5/CHANGES.md
+-rw-r--r--   0 Robin      (501) staff       (20)       38 2024-04-23 02:18:51.000000 onetable-0.0.5/setup.cfg
```

### Comparing `onetable-0.0.4/PKG-INFO` & `onetable-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetable
-Version: 0.0.4
+Version: 0.0.5
 Summary: Once defined, multiple ways to export table.
 Home-page: https://github.com/sintrb/onetable/
 Author: trb
 Author-email: sintrb@gmail.com
 License: UNKNOWN
 Description: onetable
         ===============
@@ -33,20 +33,24 @@
         table.writeNextRowCols([1, 2, 3])
         table.writeNextRowCols([3, 2, 1, 1], style='red')
         with open('test.xls', 'wb') as out:
             XlsRender().save(tab=table, out=out)
         ```
         
         
+        
         CHANGES
         ===============
         0.0.1
         
         - first version
         
         0.0.2
         
         - add usage
         
+        0.0.5
+        
+        - add background for xlsx
 Keywords: onetable,excel,csv,table,export
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `onetable-0.0.4/onetable/__init__.py` & `onetable-0.0.5/onetable/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: UTF-8 -*
 '''
 Created on 2019/06/22
 
 @author: Robin
 '''
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 
 
 class UniTable(object):
     defaultValue = ''
     defaultStyle = ''
 
     def __init__(self):
@@ -501,14 +501,15 @@
             'blue': 'FF0000FF',
             'green': 'FF00FF00',
             'white': 'FFFFFFFF',
             'lavender': 'FFC572DA',
             'lime': 'FF63C544',
             'light_orange': 'FFF49638',
             'coral': 'FFFB4D50',
+            'lightpink': 'FFB6C1',
         }
 
         def transcolor(c):
             return colormap.get(c)
 
         for name, style in tab.styles.items():
             border = None if 'border' in style and style['border'] == None else defaultborder
@@ -522,25 +523,29 @@
                         color=transcolor(style.get('color', 'FF000000')))
             alignment = Alignment(horizontal=style.get('align', 'left'),
                                   vertical='center',
                                   text_rotation=0,
                                   wrap_text=True,
                                   shrink_to_fit=True,
                                   indent=0)
+            fill = PatternFill(patternType='solid',
+                               fgColor=transcolor(style.get('background', 'white')))
             styled = {
                 'border': border,
                 'font': font,
-                'alignment': alignment
+                'alignment': alignment,
+                'fill': fill,
             }
             stylemap[name] = styled
 
         def applystyled(cs, styled):
             cs.border = styled.get('border')
             cs.font = styled.get('font')
             cs.alignment = styled.get('alignment')
+            cs.fill = styled.get('fill')
 
         for r in range(tab.maxRow + 1):
             for c in range(tab.maxCol + 1):
                 cell = tab.getCellByRowCol(r, c) or {}
                 if cell and cell.get('span'):
                     continue
                 value = tab.getValue(cell)  # cell.get('value')
```

### Comparing `onetable-0.0.4/onetable.egg-info/PKG-INFO` & `onetable-0.0.5/onetable.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetable
-Version: 0.0.4
+Version: 0.0.5
 Summary: Once defined, multiple ways to export table.
 Home-page: https://github.com/sintrb/onetable/
 Author: trb
 Author-email: sintrb@gmail.com
 License: UNKNOWN
 Description: onetable
         ===============
@@ -33,20 +33,24 @@
         table.writeNextRowCols([1, 2, 3])
         table.writeNextRowCols([3, 2, 1, 1], style='red')
         with open('test.xls', 'wb') as out:
             XlsRender().save(tab=table, out=out)
         ```
         
         
+        
         CHANGES
         ===============
         0.0.1
         
         - first version
         
         0.0.2
         
         - add usage
         
+        0.0.5
+        
+        - add background for xlsx
 Keywords: onetable,excel,csv,table,export
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `onetable-0.0.4/README.md` & `onetable-0.0.5/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 table.writeNextRowCols([('Title1', 3, 'title')])
 table.pushStatus()
 table.popStatus()
 table.writeNextRowCols([1, 2, 3])
 table.writeNextRowCols([3, 2, 1, 1], style='red')
 with open('test.xls', 'wb') as out:
     XlsRender().save(tab=table, out=out)
-```
+```
```

### Comparing `onetable-0.0.4/setup.py` & `onetable-0.0.5/setup.py`

 * *Files identical despite different names*

