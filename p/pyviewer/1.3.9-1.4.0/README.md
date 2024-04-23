# Comparing `tmp/pyviewer-1.3.9.tar.gz` & `tmp/pyviewer-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviewer-1.3.9.tar", last modified: Mon Feb 12 10:28:44 2024, max compression
+gzip compressed data, was "pyviewer-1.4.0.tar", last modified: Tue Apr 23 16:50:55 2024, max compression
```

## Comparing `pyviewer-1.3.9.tar` & `pyviewer-1.4.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:28:44.057263 pyviewer-1.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)    20879 2024-02-12 10:28:37.000000 pyviewer-1.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-12 10:28:44.053263 pyviewer-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-02-12 10:28:37.000000 pyviewer-1.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:28:44.053263 pyviewer-1.3.9/pyviewer/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:28:44.053263 pyviewer-1.3.9/pyviewer/custom_ops/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/custom_ops/cuda_gl_interop.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/custom_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/easy_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    25802 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/gl_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24300 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/imgui_themes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/single_image_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/toolbar_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20168 2024-02-12 10:28:37.000000 pyviewer-1.3.9/pyviewer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:28:44.053263 pyviewer-1.3.9/pyviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-12 10:28:44.000000 pyviewer-1.3.9/pyviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-12 10:28:44.000000 pyviewer-1.3.9/pyviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 10:28:44.000000 pyviewer-1.3.9/pyviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-12 10:28:44.000000 pyviewer-1.3.9/pyviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 10:28:44.000000 pyviewer-1.3.9/pyviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 10:28:44.057263 pyviewer-1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-12 10:28:37.000000 pyviewer-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:50:55.364974 pyviewer-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    20879 2024-04-23 16:50:41.000000 pyviewer-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-23 16:50:55.364974 pyviewer-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-23 16:50:41.000000 pyviewer-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:50:55.364974 pyviewer-1.4.0/pyviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)  3423528 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/MPLUSRounded1c-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:50:55.364974 pyviewer-1.4.0/pyviewer/custom_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/custom_ops/cuda_gl_interop.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/custom_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/easy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25971 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/gl_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24300 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/imgui_themes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71936 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/roboto_mono.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/single_image_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/toolbar_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20038 2024-04-23 16:50:42.000000 pyviewer-1.4.0/pyviewer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:50:55.364974 pyviewer-1.4.0/pyviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-23 16:50:55.000000 pyviewer-1.4.0/pyviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-23 16:50:55.000000 pyviewer-1.4.0/pyviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:50:55.000000 pyviewer-1.4.0/pyviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 16:50:55.000000 pyviewer-1.4.0/pyviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 16:50:55.000000 pyviewer-1.4.0/pyviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:50:55.364974 pyviewer-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-23 16:50:42.000000 pyviewer-1.4.0/setup.py
```

### Comparing `pyviewer-1.3.9/LICENSE` & `pyviewer-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.9/PKG-INFO` & `pyviewer-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviewer
-Version: 1.3.9
+Version: 1.4.0
 Summary: Interactyive python viewers
 Home-page: https://github.com/harskish/pyviewer
 Author: Erik Härkönen
 Author-email: erik.harkonen@hotmail.com
 License: CC BY-NC-SA 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyviewer-1.3.9/README.md` & `pyviewer-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.9/pyviewer/custom_ops/cuda_gl_interop.cpp` & `pyviewer-1.4.0/pyviewer/custom_ops/cuda_gl_interop.cpp`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.9/pyviewer/custom_ops.py` & `pyviewer-1.4.0/pyviewer/custom_ops.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,25 @@
 
 import os
 import torch
 import torch.utils.cpp_extension as cpp
 
 import importlib
 from functools import cache
+from typing import Union
 
 @cache
-def get_plugin(plugin_name: str, source_files: tuple or str, source_folder: str = '.', verbose=True):
-
+def get_plugin(
+    plugin_name: str,
+    source_files: Union[tuple, str],
+    source_folder: str = '.',
+    ldflags: tuple = None,
+    cuda: bool = True, # can turn off if not needed
+    verbose=True
+):
     # Make sure we can find the necessary compiler and libary binaries.
     if os.name == 'nt':
         lib_dir = os.path.dirname(__file__) + r"."
         def find_cl_path():
             import glob
             for maybe_x86 in ["", " (x86)"]:
                 for edition in ['Community', 'Enterprise', 'Professional', 'BuildTools']:
@@ -28,18 +35,18 @@
                 raise RuntimeError("Could not locate a supported Microsoft Visual C++ installation")
             os.environ['PATH'] += ';' + cl_path
 
 
     # Linker options.
     if os.name == 'posix':
         cflags = ['-O3', '-std=c++17']
-        ldflags = ['-lGL', '-lGLEW', '-lEGL']
+        ldflags = ['-lGL', '-lGLEW', '-lEGL'] if ldflags is None else ldflags
     elif os.name == 'nt':
         libs = ['user32', 'opengl32']
-        ldflags = ['/LIBPATH:' + lib_dir] + ['/DEFAULTLIB:' + x for x in libs]
+        ldflags = (['/LIBPATH:' + lib_dir] + ['/DEFAULTLIB:' + x for x in libs]) if ldflags is None else ldflags
         cflags = ['/O2', '/DWIN32', '/std:c++17','/permissive-', '/w']
 
 
     # Some containers set this to contain old architectures that won't compile. We only need the one installed in the machine.
     os.environ['TORCH_CUDA_ARCH_LIST'] = ''
 
     # Try to detect if a stray lock file is left in cache directory and show a warning. This sometimes happens on Windows if the build is interrupted at just the right moment.
@@ -51,11 +58,13 @@
                 os.remove(lock_fn)
         except:
             pass
     
     # Compile and load.
     original = os.getcwd()
     os.chdir(source_folder)
-
-    cpp.load(verbose=verbose, name=plugin_name, extra_cflags=cflags, extra_cuda_cflags=['-O2'], sources=source_files, extra_ldflags=ldflags, with_cuda=True)
-    os.chdir(original)
+    
+    try:
+        cpp.load(verbose=verbose, name=plugin_name, extra_cflags=cflags, extra_cuda_cflags=['-O2'], sources=source_files, extra_ldflags=ldflags, with_cuda=cuda)
+    finally:
+        os.chdir(original)
     return importlib.import_module(plugin_name)
```

### Comparing `pyviewer-1.3.9/pyviewer/gl_viewer.py` & `pyviewer-1.4.0/pyviewer/gl_viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,32 +24,35 @@
 has_torch = False
 try:
     import torch
     has_torch = True
 except:
     pass
 
-cuda_synchronize = lambda : None
+torch_has_cuda = False
 if has_torch and torch.cuda.is_available():
-    cuda_synchronize = torch.cuda.synchronize
+    torch_has_cuda = True
+
+cuda_synchronize = torch.cuda.synchronize if torch_has_cuda else lambda : None
 
 has_pycuda = False
 try:
     import pycuda
     import pycuda.gl as cuda_gl
     import pycuda.tools
     has_pycuda = True
 except Exception:
     pass
 
 # CUDA-GL copy via PyTorch extension
 pt_plugin = None
 try:
     from . import custom_ops
-    pt_plugin = custom_ops.get_plugin('cuda_gl_interop', 'cuda_gl_interop.cpp', Path(__file__).parent / './custom_ops')
+    if torch_has_cuda:
+        pt_plugin = custom_ops.get_plugin('cuda_gl_interop', 'cuda_gl_interop.cpp', Path(__file__).parent / './custom_ops')
 except Exception:
     pass
 
 class PTExtMapper:
     tex: int
     resource: int # uint64_t
     
@@ -336,30 +339,32 @@
         self._imgui_context = imgui.create_context()
         self._implot_context = implot.create_context()
         implot.set_imgui_context(self._imgui_context)
         #implot.get_style().anti_aliased_lines = True # turn global AA on
 
         font = self.get_default_font()
 
-        # MPLUSRounded1c-Medium.tff: no content for sizes >35
+        # MPLUSRounded1c-Medium.ttf: no content for sizes >35
         # Apple M1, WSL have have low texture count limits
         font_sizes = range(8, 36, 1) if 'win32' in platform else range(8, 36, 2)
         font_sizes = [int(s) for s in font_sizes]
         handle = imgui.get_io().fonts
         self._imgui_fonts = {
             size: handle.add_font_from_file_ttf(font, size,
                 glyph_ranges=handle.get_glyph_ranges_chinese_full()) for size in font_sizes
         }
 
         self._context_lock = mp.Lock()
         self._context_tid = None # id of thread in critical section
         self.set_ui_scale(self.ui_scale)
 
     def get_default_font(self):
-        return str(Path(__file__).parent / 'MPLUSRounded1c-Medium.ttf')
+        font = Path(__file__).parent / 'MPLUSRounded1c-Medium.ttf'
+        assert font.is_file(), f'Font file missing: "{font.resolve()}"'
+        return str(font)
     
     def push_context(self):
         if has_pycuda:
             self._cuda_context.push()
     
     def pop_context(self):
         if has_pycuda:
```

### Comparing `pyviewer-1.3.9/pyviewer/imgui_themes.py` & `pyviewer-1.4.0/pyviewer/imgui_themes.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.9/pyviewer/params.py` & `pyviewer-1.4.0/pyviewer/params.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,15 +104,14 @@
         if not self.overlap:
             return slider_range_float(*self.value, self.min, self.max, title=self.label)
         else:
             return imgui.slider_float2(self.label, *self.value, self.min, self.max)
     
 ##########################################
 # Container that exposes raw values
-
 @strict_dataclass
 class ParamContainer:
     def __iter__(self):
         for attr, _ in self.__dataclass_fields__.items():
             yield attr, super().__getattribute__(attr)
     
     def __getattribute__(self, __name: str):
@@ -123,8 +122,17 @@
             return obj
     
     def __setattr__(self, __name: str, __value) -> None:
         obj = super().__getattribute__(__name)
         if isinstance(obj, Param) and not isinstance(__value, Param):
             obj.value = __value
         else:
-            super().__setattr__(__name, __value)
+            super().__setattr__(__name, __value)
+            
+    def __todict__(self):
+        ret = {}
+        for attr, _ in self.__dataclass_fields__.items():
+            ret[attr] = self.__getattribute__(attr)
+        return ret
+
+    def __str__(self):
+        return str(self.__todict__())
```

### Comparing `pyviewer-1.3.9/pyviewer/single_image_viewer.py` & `pyviewer-1.4.0/pyviewer/single_image_viewer.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.9/pyviewer/toolbar_viewer.py` & `pyviewer-1.4.0/pyviewer/toolbar_viewer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import imgui
 import glfw
 import threading
 import random
 import string
 import numpy as np
 import time
+from pathlib import Path
+from functools import partial
 
 from . import gl_viewer
 from .utils import imgui_item_width, begin_inline, PannableArea
 from .easy_dict import EasyDict
 from .params import ParamContainer, Param
 
 #----------------------------------------------------------------------------
 # Helper class for UIs with toolbar on the left and output image on the right
 
+def file_drop_callback_wrapper(window, paths, callback: callable):
+    return callback([Path(p) for p in paths])
+
 class ToolbarViewer:
     def __init__(self, name, pad_bottom=0, hidden=False, batch_mode=False):
         self.output_key = ''.join(random.choices(string.ascii_letters, k=20))
         self._user_pad_bottom = pad_bottom
         self.v = gl_viewer.viewer(name, hidden=hidden or batch_mode, swap_interval=1)
         self.menu_bar_height = self.v.font_size + 2*imgui.get_style().frame_padding.y
 
@@ -50,14 +55,16 @@
         # Batch mode: handle compute loop manually, don't start UI
         if not batch_mode:
             self.start_UI()
 
     def start_UI(self):
         compute_thread = threading.Thread(target=self._compute_loop, args=[])
         def init_callbacks(window):
+            glfw.set_drop_callback(window,
+                partial(file_drop_callback_wrapper, callback=self.drag_and_drop_callback))
             self.setup_callbacks(window)
             self.pan_handler.set_callbacks(window)
         self.v.start(self._ui_main, (compute_thread), init_callbacks)
 
     # Extra user content below image
     @property
     def pad_bottom(self):
@@ -81,15 +88,15 @@
 
     @property
     def mouse_pos_abs(self):
         return np.array(imgui.get_mouse_pos())
 
     @property
     def mouse_pos_content_norm(self):
-        return (self.mouse_pos_abs - self.output_area_tl) / self.content_size
+        return (self.mouse_pos_abs - self.output_pos_tl) / self.content_size
     
     @property
     def mouse_pos_img_norm(self):
         dims = self.output_pos_br - self.output_pos_tl
         if any(dims == 0):
             return np.array([-1, -1], dtype=np.float32) # no valid content
         return (self.mouse_pos_abs - self.output_pos_tl) / dims
@@ -268,18 +275,21 @@
     def compute(self):
         pass
 
     # Program state init
     def setup_state(self):
         pass
 
-    # GLFW callbacks
+    # Manual GLFW callbacks
+    # Overrides the ones below
     def setup_callbacks(self, window):
         pass
 
+    def drag_and_drop_callback(self, paths: list[Path]):
+        pass
 
 #----------------------------------------------
 # Version that creates UI widgets automatically
 
 class AutoUIViewer(ToolbarViewer):
     def draw_toolbar_autoUI(self):
         if not isinstance(self.state, ParamContainer):
```

### Comparing `pyviewer-1.3.9/pyviewer/utils.py` & `pyviewer-1.4.0/pyviewer/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
 import imgui
 import contextlib
 from io import BytesIO
 from pathlib import Path
+from functools import partial
+import shutil
 import os
 import glfw
 import random
 import string
 from textwrap import dedent
 
 import OpenGL.GL as gl
@@ -473,61 +475,52 @@
         rng = np.random.RandomState(seed)
         latents[i] = rng.standard_normal(n_dims)
     
     return latents
 
 # File copy with progress bar
 # For slow network drives etc.
-def copy_with_progress(pth_from, pth_to):
-    from tqdm import tqdm
+def copy_with_progress(pth_from: Path, pth_to: Path):
     os.makedirs(pth_to.parent, exist_ok=True)
-    size = int(os.path.getsize(pth_from))
-    fin = open(pth_from, 'rb')
-    fout = open(pth_to, 'ab')
-
-    try:
-        with tqdm(ncols=80, total=size, bar_format=pth_from.name + ' {l_bar}{bar} | Remaining: {remaining}') as pbar:
-            while True:
-                buf = fin.read(4*2**20) # 4 MiB
-                if len(buf) == 0:
-                    break
-                fout.write(buf)
-                pbar.update(len(buf))
-    except Exception as e:
-        print(f'File copy failed: {e}')
-    finally:
-        fin.close()
-        fout.close()
+    return shutil.copyfileobj(open_prog(pth_from, 'rb', pth_to.name), open(pth_to, 'ab'))
 
 # File open with progress bar
 # For slow network drives etc.
 # Supports context manager
-def open_prog(pth, mode):
+def open_prog(pth, mode, name=None):
     from tqdm import tqdm
-    size = int(os.path.getsize(pth))
-    fin = open(pth, 'rb')
-
-    assert mode == 'rb', 'Only rb supported'
-    fout = BytesIO()
 
-    try:
-        with tqdm(ncols=80, total=size, bar_format=Path(pth).name + ' {l_bar}{bar}| Remaining: {remaining}') as pbar:
-            while True:
-                buf = fin.read(4*2**20) # 4 MiB
-                if len(buf) == 0:
-                    break
-                fout.write(buf)
-                pbar.update(len(buf))
-    except Exception as e:
-        print(f'File copy failed: {e}')
-    finally:
-        fin.close()
-        fout.seek(0)
-
-    return fout
+    assert mode in ['r', 'rb'], 'Only r and rb supported'
+    total_size = int(os.path.getsize(pth))
+    label = Path(pth).name if name is None else name
+    pbar = tqdm(ncols=80, total=total_size, bar_format=f'{label} {{l_bar}}{{bar}}| {{elapsed}}<{{remaining}}')
+    handle = open(pth, mode)
+
+    def update(size):
+        pbar.update(size)
+        if pbar.n == pbar.total:
+            pbar.refresh()
+            pbar.close()
+
+    def read(size, orig=None):
+        update(size)
+        return orig(size)
+    handle.read = partial(read, orig=handle.read)
+
+    def readinto(memory, orig=None):
+        update(memory.nbytes)
+        return orig(memory)
+    handle.readinto = partial(readinto, orig=handle.readinto)
+
+    def close(orig=None):
+        update(pbar.total - pbar.n) # set to 100%
+        return orig()
+    handle.close = partial(close, orig=handle.close)
+    
+    return handle
 
 # Convert input image to valid range for showing
 # Output converted to target dtype *after* scaling
 #   => should not affect quality that much
 def normalize_image_data(img_hwc, target_dtype='uint8'):    
     is_np = isinstance(img_hwc, np.ndarray)
     is_fp = (img_hwc.dtype.kind == 'f') if is_np else img_hwc.dtype.is_floating_point
```

### Comparing `pyviewer-1.3.9/pyviewer.egg-info/PKG-INFO` & `pyviewer-1.4.0/pyviewer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviewer
-Version: 1.3.9
+Version: 1.4.0
 Summary: Interactyive python viewers
 Home-page: https://github.com/harskish/pyviewer
 Author: Erik Härkönen
 Author-email: erik.harkonen@hotmail.com
 License: CC BY-NC-SA 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyviewer-1.3.9/setup.py` & `pyviewer-1.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,30 @@
 from pathlib import Path
 
 import sys
 if 'develop' in sys.argv:
     print("WARNING: 'python setup.py develop' won't install \
         dependencies correctly, please use 'pip install -e .' instead.")
 
-# Workflow:
+# Version bump workflow:
 # Increment version number (together with other changes)
 # git commit
 # git tag -a "vX.X.X" -m "vX.X.X"  (only annotated tags show up in GitHub)
 # git push --follow-tags
+    
+# In case of mistake:
+# git tag --delete tagname
+# git push --delete origin tagname
+
+# Test package_data changes by manually starting
+# the publish workflow and checking the "Print whl contents" step,
+# or with: `rm -r build\ && pip wheel . && unzip -l pyviewer-*.whl`
+# (not same environment, but good first step)
 setup(name='pyviewer',
-    version='1.3.9',
+    version='1.4.0',
     description='Interactyive python viewers',
     author='Erik Härkönen',
     author_email='erik.harkonen@hotmail.com',
     url='https://github.com/harskish/pyviewer',
     packages=['pyviewer'], # name of importable thing
     setup_requires=['wheel'],
     install_requires=[
@@ -27,15 +36,17 @@
         'pyopengl>3.0.0',
         'pyplotgui',  # custom imgui+implot package
         'light-process==0.0.7',
         'ninja', # for custom OP
     ],
     include_package_data=True,
     package_data={
-        '': ['*.ttf'], # embedded fonts
-        '': ['custom_ops/*.cpp'], # custom CUDA op
+        'pyviewer': [
+            '*.ttf',            # embedded fonts
+            'custom_ops/*.cpp', # custom CUDA op
+        ],
     },
     long_description=Path('README.md').read_text()
         .replace('docs/screenshot.jpg', 'https://github.com/harskish/pyviewer/raw/master/docs/screenshot.jpg'),
     long_description_content_type="text/markdown",
     license='CC BY-NC-SA 4.0',
 )
```

