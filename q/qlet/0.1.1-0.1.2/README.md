# Comparing `tmp/qlet-0.1.1.tar.gz` & `tmp/qlet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlet-0.1.1.tar", last modified: Tue Jan 30 18:04:43 2024, max compression
+gzip compressed data, was "qlet-0.1.2.tar", last modified: Mon Apr 22 21:58:37 2024, max compression
```

## Comparing `qlet-0.1.1.tar` & `qlet-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2024-01-30 18:04:43.264002 qlet-0.1.1/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    11356 2024-01-30 16:20:34.000000 qlet-0.1.1/LICENSE
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    14560 2024-01-30 18:04:43.263497 qlet-0.1.1/PKG-INFO
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      468 2024-01-30 17:41:26.000000 qlet-0.1.1/README.md
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1211 2024-01-30 18:04:28.000000 qlet-0.1.1/pyproject.toml
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2024-01-30 18:04:43.258097 qlet-0.1.1/qlet/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      104 2024-01-30 18:04:31.000000 qlet-0.1.1/qlet/__init__.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2024-01-30 18:04:43.262276 qlet-0.1.1/qlet/comps/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2024-01-30 17:12:40.000000 qlet-0.1.1/qlet/comps/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      702 2024-01-30 17:12:16.000000 qlet-0.1.1/qlet/comps/qimage.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    13717 2024-01-30 18:03:17.000000 qlet-0.1.1/qlet/comps/qitem.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1139 2024-01-30 17:12:27.000000 qlet-0.1.1/qlet/comps/qrow.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1153 2024-01-30 17:12:31.000000 qlet-0.1.1/qlet/comps/qtext.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2024-01-30 18:04:43.262955 qlet-0.1.1/qlet.egg-info/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    14560 2024-01-30 18:04:43.000000 qlet-0.1.1/qlet.egg-info/PKG-INFO
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      291 2024-01-30 18:04:43.000000 qlet-0.1.1/qlet.egg-info/SOURCES.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        1 2024-01-30 18:04:43.000000 qlet-0.1.1/qlet.egg-info/dependency_links.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)       25 2024-01-30 18:04:43.000000 qlet-0.1.1/qlet.egg-info/requires.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        5 2024-01-30 18:04:43.000000 qlet-0.1.1/qlet.egg-info/top_level.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)       38 2024-01-30 18:04:43.264094 qlet-0.1.1/setup.cfg
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2024-04-22 21:58:37.211808 qlet-0.1.2/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    11356 2024-01-30 16:20:34.000000 qlet-0.1.2/LICENSE
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    14676 2024-04-22 21:58:37.210999 qlet-0.1.2/PKG-INFO
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      584 2024-02-01 14:02:19.000000 qlet-0.1.2/README.md
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1211 2024-04-22 21:57:08.000000 qlet-0.1.2/pyproject.toml
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2024-04-22 21:58:37.204804 qlet-0.1.2/qlet/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      104 2024-04-22 21:57:19.000000 qlet-0.1.2/qlet/__init__.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2024-04-22 21:58:37.209550 qlet-0.1.2/qlet/comps/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2024-01-30 17:12:40.000000 qlet-0.1.2/qlet/comps/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      700 2024-04-22 21:55:07.000000 qlet-0.1.2/qlet/comps/qimage.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    13689 2024-04-22 21:55:48.000000 qlet-0.1.2/qlet/comps/qitem.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1139 2024-01-30 17:12:27.000000 qlet-0.1.2/qlet/comps/qrow.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1151 2024-04-22 21:55:07.000000 qlet-0.1.2/qlet/comps/qtext.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2024-04-22 21:58:37.210256 qlet-0.1.2/qlet.egg-info/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    14676 2024-04-22 21:58:37.000000 qlet-0.1.2/qlet.egg-info/PKG-INFO
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      291 2024-04-22 21:58:37.000000 qlet-0.1.2/qlet.egg-info/SOURCES.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        1 2024-04-22 21:58:37.000000 qlet-0.1.2/qlet.egg-info/dependency_links.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)       25 2024-04-22 21:58:37.000000 qlet-0.1.2/qlet.egg-info/requires.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        5 2024-04-22 21:58:37.000000 qlet-0.1.2/qlet.egg-info/top_level.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)       38 2024-04-22 21:58:37.211966 qlet-0.1.2/setup.cfg
```

### Comparing `qlet-0.1.1/LICENSE` & `qlet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qlet-0.1.1/PKG-INFO` & `qlet-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qlet
-Version: 0.1.1
+Version: 0.1.2
 Summary: Provides Qt like api for flet components
 Author: Jarvis Yu
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -237,7 +237,13 @@
 that can auto-resize based on their `ref_parent`.
 
 ## Installation
 
 ```sh
 pip install qlet
 ```
+
+## Examples
+
+***WIP***
+
+The repo owner is busy recently, but this section should be filled by the end of Feb 2024.
```

### Comparing `qlet-0.1.1/pyproject.toml` & `qlet-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qlet"
-version = "0.1.1"
+version = "0.1.2"
 license = {file = "LICENSE"}
 
 description = "Provides Qt like api for flet components"
 authors = [{ name="Jarvis Yu" }]
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
```

### Comparing `qlet-0.1.1/qlet/comps/qimage.py` & `qlet-0.1.2/qlet/comps/qimage.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,11 +14,11 @@
         ):
         self._image = ft.Image(src=src, border_radius=border_radius, fit=fit)
         super().__init__(border_radius=border_radius, **kwargs)
         self._image.width = self.width
         self._image.height = self.height
         self.add_flet_comp(self._image)
     
-    def __on_resized(self) -> None:
+    def _on_resized(self) -> None:
         self._image.width = self.width
         self._image.height = self.height
-        super().__on_resized()
+        super()._on_resized()
```

### Comparing `qlet-0.1.1/qlet/comps/qitem.py` & `qlet-0.1.2/qlet/comps/qitem.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,54 +135,54 @@
 
         self._frame = ft.Stack(
             expand=True,
             clip_behavior=self.clip,
         )
 
         if self.parent is not None:
-            self.__init_according_to_parent()
+            self._init_according_to_parent()
         elif self.ref_parent is not None:
-            self.__init_according_to_ref_parent()
+            self._init_according_to_ref_parent()
 
         self.add_flet_comp(flets)
 
-    def __init_by_parent(self, parent: Self) -> None:
+    def _init_by_parent(self, parent: Self) -> None:
         """ Called by parent if this item is added as a child """
         assert self.inited is False
         assert self.parent is None
         self.parent = parent
         self.ref_parent = parent if self.ref_parent is None else self.ref_parent
-        self.__init_according_to_parent()
+        self._init_according_to_parent()
 
-    def __init_according_to_parent(self) -> None:
+    def _init_according_to_parent(self) -> None:
         """ Init this item according to its parent """
         assert self.inited is False
         assert self.parent is not None
         assert self.ref_parent is not None
-        self.__recalc_size()
-        self.__init_internal_container()
-        self.parent.__add_child_item(self)
+        self._recalc_size()
+        self._init_internal_container()
+        self.parent._add_child_item(self)
         self.inited = True
         for child in self.children:
             if child.inited:
                 continue
-            child.__init_by_parent(self)
+            child._init_by_parent(self)
 
-    def __init_according_to_ref_parent(self) -> None:
+    def _init_according_to_ref_parent(self) -> None:
         assert self.inited is False
         assert self.parent is None
         assert self.ref_parent is not None
-        self.__recalc_size()
-        self.__init_internal_container()
-        self.ref_parent.__add_ref_child_item(self)
+        self._recalc_size()
+        self._init_internal_container()
+        self.ref_parent._add_ref_child_item(self)
         self.inited = True
         for child in self.children:
-            child.__init_by_parent(self)
+            child._init_by_parent(self)
 
-    def __init_internal_container(self) -> None:
+    def _init_internal_container(self) -> None:
         """ Init the internal container """
         if self.expand:
             self._container = ft.Container(
                 content=self._frame,
                 bgcolor=self.colour,
                 expand=True,
             )
@@ -231,15 +231,15 @@
                 width=self.width,
                 height=self.height,
             )
         self._container.border = self.border
         self._container.rotate = self.rotate
         self._container.border_radius = self.border_radius
 
-    def __update_internal_container_on_size(self) -> None:
+    def _update_internal_container_on_size(self) -> None:
         """ Update the internal container on size change """
         if self.expand:
             return
 
         if self.parent is None:
             assert self.ref_parent is not None
             self.root_component.width = self.width
@@ -256,15 +256,15 @@
         )
         internal_container.alignment = self.align
         top_trans_container = internal_container.content
         assert isinstance(top_trans_container, ft.TransparentPointer)
         top_trans_container.width = self.width
         top_trans_container.height = self.height
 
-    def __recalc_size(self) -> None:
+    def _recalc_size(self) -> None:
         """ Recalculate or init the size of this item """
         ref_parent_width = self.ref_parent.width if self.ref_parent.width is not None else 0
         ref_parent_height = self.ref_parent.height if self.ref_parent.height is not None else 0
 
         if self.width_pct is not None:
             self.width = ref_parent_width * self.width_pct
             if self.height_width_pct is not None:
@@ -306,83 +306,83 @@
                 align.y_pct = self.anchor.bottom - height_pct / 2
             self.align = align.to_flet()
 
         if self.expand:
             self.width = ref_parent_width
             self.height = ref_parent_height
 
-        self.__on_resized()
+        self._on_resized()
 
-    def __add_child_item(self, item: Self) -> None:
+    def _add_child_item(self, item: Self) -> None:
         if item not in self.children:
             self.children.append(item)
         if item.root_component not in self._frame.controls:
             self._frame.controls.append(item.root_component)
 
-    def __add_ref_child_item(self, item: Self) -> None:
+    def _add_ref_child_item(self, item: Self) -> None:
         if item not in self.children:
             self.children.append(item)
 
     def clear(self) -> None:
         self._frame.controls.clear()
         self.children.clear()
 
     def add_children(self, children: Sequence[Self] | Self) -> None:
         children = children if isinstance(children, Sequence) else (children,)
         if self.inited:
             for child in children:
-                child.__init_by_parent(self)
+                child._init_by_parent(self)
         else:
             if isinstance(children, Sequence):
                 self.children.extend(children)
             else:
                 self.children.append(children)
 
     def add_flet_comp(self, comp: Sequence[Self] | ft.Control) -> None:
         if isinstance(comp, ft.Control):
             self._frame.controls.append(comp)
         else:
             self._frame.controls.extend(comp)
 
-    def __add_to_page(self, page: ft.Page) -> None:
+    def _add_to_page(self, page: ft.Page) -> None:
         self.width = page.width - page.padding * 2
         self.height = page.height - page.padding * 2
-        self.__init_internal_container()
+        self._init_internal_container()
         page.bgcolor = self.colour
         page.controls.append(ft.SafeArea(
             content=self.root_component,
             expand=True,
         ))
 
         def on_resize(_: ft.ControlEvent) -> None:
             self.width = page.width - page.padding * 2
             self.height = page.height - page.padding * 2
-            self.__on_resized()
+            self._on_resized()
             page.update()
 
         page.on_resize = on_resize
 
-    def __on_resized(self) -> None:
+    def _on_resized(self) -> None:
         for child in self.children:
             if not child.inited:
                 continue
             child.update_size()
 
     def update_size(self) -> None:
         """ Recalculate and update the size of this item. """
-        self.__recalc_size()
-        self.__update_internal_container_on_size()
+        self._recalc_size()
+        self._update_internal_container_on_size()
 
     @classmethod
     def init_page(
             cls,
             page: ft.Page,
             colour: str = ft.colors.with_opacity(0, "#FFFFFF"),
     ) -> Self:
         """
         Puts an item on the page that expands to fill the page.
         Returns the item.
         """
         root_item = QItem(expand=True, colour=colour)
-        root_item.__add_to_page(page)
+        root_item._add_to_page(page)
         root_item.inited = True
         return root_item
```

### Comparing `qlet-0.1.1/qlet/comps/qrow.py` & `qlet-0.1.2/qlet/comps/qrow.py`

 * *Files identical despite different names*

### Comparing `qlet-0.1.1/qlet/comps/qtext.py` & `qlet-0.1.2/qlet/comps/qtext.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,13 +22,13 @@
             self.add_flet_comp(ft.TransparentPointer(
                 content=ft.Container(
                     content=self._text,
                     alignment=text_alignment,
                 ),
             ))
 
-    def __on_resized(self) -> None:
+    def _on_resized(self) -> None:
         if self._size_rel_height is not None:
             self._text.size = self.height * self._size_rel_height
         elif self._size_rel_width is not None:
             self._text.size = self.width * self._size_rel_width
-        super().__on_resized()
+        super()._on_resized()
```

### Comparing `qlet-0.1.1/qlet.egg-info/PKG-INFO` & `qlet-0.1.2/qlet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qlet
-Version: 0.1.1
+Version: 0.1.2
 Summary: Provides Qt like api for flet components
 Author: Jarvis Yu
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -237,7 +237,13 @@
 that can auto-resize based on their `ref_parent`.
 
 ## Installation
 
 ```sh
 pip install qlet
 ```
+
+## Examples
+
+***WIP***
+
+The repo owner is busy recently, but this section should be filled by the end of Feb 2024.
```

