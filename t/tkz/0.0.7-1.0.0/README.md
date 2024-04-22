# Comparing `tmp/tkz-0.0.7.tar.gz` & `tmp/tkz-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkz-0.0.7.tar", last modified: Tue Dec 19 22:19:52 2023, max compression
+gzip compressed data, was "tkz-1.0.0.tar", last modified: Mon Apr 22 22:41:54 2024, max compression
```

## Comparing `tkz-0.0.7.tar` & `tkz-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-19 22:19:52.523261 tkz-0.0.7/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1058 2023-12-11 21:28:06.000000 tkz-0.0.7/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     2016 2023-12-19 22:19:52.523212 tkz-0.0.7/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1570 2023-12-11 21:44:56.000000 tkz-0.0.7/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 tkz-0.0.7/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      568 2023-12-19 22:19:52.523457 tkz-0.0.7/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-19 22:19:52.521211 tkz-0.0.7/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-19 22:19:52.522290 tkz-0.0.7/src/tkz/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2023-12-11 22:09:38.000000 tkz-0.0.7/src/tkz/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    73116 2023-12-19 22:18:45.000000 tkz-0.0.7/src/tkz/tkz.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2023-12-19 22:19:52.523050 tkz-0.0.7/src/tkz.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     2016 2023-12-19 22:19:52.000000 tkz-0.0.7/src/tkz.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      235 2023-12-19 22:19:52.000000 tkz-0.0.7/src/tkz.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2023-12-19 22:19:52.000000 tkz-0.0.7/src/tkz.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2023-12-19 22:19:52.000000 tkz-0.0.7/src/tkz.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2023-12-19 22:19:52.000000 tkz-0.0.7/src/tkz.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 22:41:54.771881 tkz-1.0.0/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1058 2023-12-11 21:28:06.000000 tkz-1.0.0/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    15122 2024-04-22 22:41:54.771799 tkz-1.0.0/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    14676 2024-04-22 22:41:20.000000 tkz-1.0.0/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 tkz-1.0.0/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      568 2024-04-22 22:41:54.772097 tkz-1.0.0/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 22:41:54.769840 tkz-1.0.0/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 22:41:54.770759 tkz-1.0.0/src/tkz/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2023-12-11 22:09:38.000000 tkz-1.0.0/src/tkz/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    85841 2024-04-22 21:44:06.000000 tkz-1.0.0/src/tkz/tkz.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-22 22:41:54.771627 tkz-1.0.0/src/tkz.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    15122 2024-04-22 22:41:54.000000 tkz-1.0.0/src/tkz.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      235 2024-04-22 22:41:54.000000 tkz-1.0.0/src/tkz.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-22 22:41:54.000000 tkz-1.0.0/src/tkz.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-22 22:41:54.000000 tkz-1.0.0/src/tkz.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-22 22:41:54.000000 tkz-1.0.0/src/tkz.egg-info/top_level.txt
```

### Comparing `tkz-0.0.7/LICENSE.txt` & `tkz-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkz-0.0.7/setup.cfg` & `tkz-1.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tkz
-version = 0.0.7
+version = 1.0.0
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = TikZ Figure Generator
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/tkz
 classifiers =
```

### Comparing `tkz-0.0.7/src/tkz/tkz.py` & `tkz-1.0.0/src/tkz/tkz.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,95 +15,100 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 --------------------------------------------------------------------------------
+This package is meant for the average Python user who does not necessarily know
+much of anything about the TikZ package. Its interface is meant to be similar to
+other packages like MatPlotLib, though perhaps more object-oriented in its use
+of object fields rather than functions (e.g., xlabel()). So, it does not require
+that the user know about the various names of predefined line widths or the
+names of line styles (e.g., "dashdotted"). However, it is meant to also be
+flexible enough for the user who is familiar with the options of the TikZ
+package. This is enabled through the "fmt" parameter.
 """
 
 __author__ = "David Woodburn"
 __license__ = "MIT"
-__date__ = "2023-12-19"
+__date__ = "2024-04-22"
 __maintainer__ = "David Woodburn"
 __email__ = "david.woodburn@icloud.com"
 __status__ = "Development"
 
 import os
 import warnings
-import math                 # about 5 to 10 times faster than NumPy for scalars
+import math                         # 5-10x faster than NumPy for scalars
 import numpy as np
 
-# TODO Add NaN immunity.
-# TODO Add cropping of data points outside the box.
-
 # Generic constants
 PT_PER_CM = 28.45274                # points per centimeter
 WIDTH = 8.636                       # default figure width (cm)
 TICK_SIZE = 0.1                     # default tick mark size (cm)
 LEGEND_RATIO = 0.03                 # of figure width (cm/cm)
 
-# Edge thicknesses
-ULTRA_THIN = 0.1                    # (pt)
-VERY_THIN = 0.2                     # (pt)
-THIN = 0.4                          # (pt)
-SEMI_THICK = 0.6                    # (pt)
-THICK = 0.8                         # (pt)
-VERY_THICK = 1.2                    # (pt)
-ULTRA_THICK = 1.6                   # (pt)
-
-# Display styles
-STYLE_LINE       = 0                # solid curve
-STYLE_CIRCLES    = 1                # scattered circles
-STYLE_DOTS       = 2                # scattered dots
-STYLE_FILLED     = 3                # fill area
-STYLE_FILLPAIRS  = 4                # fill between pairs of rows
-STYLE_HEXBIN     = 5                # hexagon bins
+# Predefined TikZ line styles
+SOLID           = 0                 # ----
+DASHDOTTED      = 1                 # -.-.
+DASHED          = 2                 # - -
+DENSELYDOTTED   = 3                 # ....
+DOTTED          = 4                 # . .
+LOOSELYDOTTED   = 5                 # .  .
+
+# Marker styles
+CIRCLES         = 0                 # o
+DOTS            = 1                 # .
+
+# Predefined TikZ edge thicknesses
+THINEST         = 0.05              # (pt)
+ULTRA_THIN      = 0.1               # (pt)
+VERY_THIN       = 0.2               # (pt)
+THIN            = 0.4               # (pt)
+SEMI_THICK      = 0.6               # (pt)
+THICK           = 0.8               # (pt)
+VERY_THICK      = 1.2               # (pt)
+ULTRA_THICK     = 1.6               # (pt)
+THICKEST        = 100.0             # (pt)
 
 # Key color values
-BLUE    = 0x0000ff                  #   0    0  255
-AZURE   = 0x0080ff                  #   0  128  255
-CYAN    = 0x00d1d1                  #   0  209  209
-GREEN   = 0x0fb400                  #  15  180    0
-LIME    = 0xa9cb00                  # 169  203    0
-YELLOW  = 0xffbf00                  # 255  191    0
-ORANGE  = 0xff8000                  # 255  128    0
-RED     = 0xff0000                  # 255    0    0
-MAGENTA = 0xff00ff                  # 255    0  255
-PURPLE  = 0x8000ff                  # 128    0  255
+BLUE            = 0x0000ff          #   0    0  255
+AZURE           = 0x0080ff          #   0  128  255
+CYAN            = 0x00d1d1          #   0  209  209
+GREEN           = 0x0fb400          #  15  180    0
+LIME            = 0xa9cb00          # 169  203    0
+YELLOW          = 0xffbf00          # 255  191    0
+ORANGE          = 0xff8000          # 255  128    0
+RED             = 0xff0000          # 255    0    0
+MAGENTA         = 0xff00ff          # 255    0  255
+PURPLE          = 0x8000ff          # 128    0  255
+
+# Color maps
+MAP_WHEEL = [BLUE, AZURE, CYAN, GREEN, LIME,
+        YELLOW, ORANGE, RED, MAGENTA, PURPLE]
 
 # Ratios of symbol widths to font size
 R_SIGN = 0.75                       # sign width as ratio of font size
 R_DIGIT = 0.5                       # digit width as ratio of font size
 R_DECIMAL = 0.28                    # decimal width as ratio of font size
 R_TIMES = 0.89                      # times width as ratio of font size
 R_POWER = 0.85                      # scaling factor for widths in powers
 
 
-# For scatter plots, "z" is used for the size of the markers and can be an
-# array. If it is a scalar, then all the markers will be the same size. The
-# "size" is for the thickness of the marker edges. For hexbin, "z" is unused and
-# "size" controls the distance from the center to an edge of a hexagon.
-class Set:
-    def __init__(self, x, y, z=None, color=None, opacity=1.0,
-            style=STYLE_LINE, size=THICK, label=None, fmt=None, simp=True):
-        self.x = x                  # array of x-axis values
-        self.y = y                  # array of y-axis values
-        self.z = z                  # array or list of z-axis values
-        self.color = color          # scalar color integer (0xRRGGBB)
-        self.opacity = opacity      # scalar opacity float [0, 1]
-        self.style = style          # fill, line, or marker style
-        self.size = size            # line size or hexagon max size (pt)
-        self.label = label          # set string label
-        self.fmt = fmt              # additional format string
-        self.simp = simp            # flag to simplify path
+# Library-wide attributes
+class config:
+    skip = False                    # flag to skip plotting
+    silent = True                   # flag to silence pdflatex output
+    directory = None                # directory for figure files
+    colormap = MAP_WHEEL            # main color map
 
 
-class Layout:
-    def __init__(self):
+class GraphLayout:
+    """ Settings for the layout of the graph. """
+    def __init__(self): # These are the internal, calculated settings.
         self.width = 0.0            # width of figure (cm)
         self.height = 0.0           # height of figure (cm)
         self.font_size = 0.0        # font size (pt)
         self.font_size_name = ""    # font size name ("tiny", "large", ...)
         self.x_min = 0.0            # x-axis min (units)
         self.x_max = 0.0            # x-axis max (units)
         self.y_min = 0.0            # y-axis min (units)
@@ -132,31 +137,66 @@
         self.legend_cols = 0        # number of legend columns
         self.legend_rows = 0        # number of legend rows
         self.H_legend_row = 0.0     # height of a legend row (cm)
         self.H_legend = 0.0         # height of the entire legend (cm)
         self.invisibles = False     # flag to show invisible boundaries
 
 
-class graph:
-    # Class-wide attributes
-    skip = False                    # flag to skip all subsequent plotting
-    silent = True                   # flag to silence pdflatex output
-    directory = None                # directory for all figures
+def append_to_fmt(fmt, opacity, width, pattern):
+    """ Add opacity, line width, and line pattern to the format string `fmt`.
+    Color is not included here because all colors will be predefined and then
+    referenced by short name in the path commands. """
+    if opacity is not None:
+        opacity = max(0.0, min(opacity, 1.0))
+        if opacity != 1:
+            opacity_str = f"opacity={opacity:0.3g}"
+            fmt = opacity_str if fmt is None else fmt + ", " + opacity_str
+    if (width is not None) and (width != THIN):
+        width = max(THINEST, min(width, THICKEST))
+        width_str = f"line width={width:0.3g}pt"
+        fmt = width_str if fmt is None else fmt + ", " + width_str
+    if pattern is not None:
+        pattern_list = ["solid", "dashdotted", "dashed",
+                "densely dotted", "dotted", "loosely dotted"]
+        pattern = max(0, min(pattern, len(pattern_list) - 1))
+        pattern_str = pattern_list[pattern]
+        if pattern_str != "solid":
+            fmt = pattern_str if fmt is None else fmt + ", " + pattern_str
+    return fmt
+
 
+class Set:
+    """ Settings for a curve in the graph. """
+    def __init__(self, x, y, z=None, zony=False, color=None, marker=None,
+            scaling=0, func=None, label=None, simp=True, fmt=None):
+        self.x = x                  # x axis, or y when y is None
+        self.y = y                  # y axis
+        self.z = z                  # second y array or radius (radii)
+        self.zony = zony            # flag to plot `z` on y axis
+        self.rows = None            # max rows of `x` and `y`
+        self.color = color          # scalar color integer (0xRRGGBB)
+        self.marker = marker        # marker type (circle, dot)
+        self.scaling = scaling      # scaling on the rendering of data
+        self.func = func            # plot, scatter, fill
+        self.label = label          # data set label string
+        self.simp = simp            # flag to simplify path
+        self.fmt = fmt              # additional format string
+
+
+class graph:
     def __init__(self, filename='fig', width=None, height=None,
             xmin=None, xmax=None, ymin=None, ymax=None,
             xpad=False, ypad=True, xlog=False, ylog=False,
             equal=False, fontsize=9, xlabel=None, ylabel=None,
             xaxis=True, yaxis=True, xgrid=True, ygrid=True,
             xsubgrid=True, ysubgrid=True, xtick=True, ytick=True,
             ticksize=TICK_SIZE, xout=False, yout=False,
             rowmajor=False, columns=None, preamble=None,
-            standalone=True, sets=None,
-            skip=None, silent=None, directory=None):
-        # Assign the settings.
+            standalone=True):
+        # Assign the settings. These are the user-facing options.
         self.filename = filename    # string of file without extension
         self.width = width          # width of pdf image in centimeters
         self.height = height        # height of pdf image in centimeters
         self.xmin = xmin            # x-axis minimum
         self.xmax = xmax            # x-axis maximum
         self.ymin = ymin            # y-axis minimum
         self.ymax = ymax            # y-axis maximum
@@ -179,249 +219,159 @@
         self.ticksize = ticksize    # size of tick marks (cm)
         self.xout = xout            # flag to put x-axis ticks outside
         self.yout = yout            # flag to put y-axis ticks outside
         self.rowmajor = rowmajor    # flag to layout legend row major
         self.columns = columns      # number of legend columns
         self.preamble = preamble    # added string of LaTeX code in preamble
         self.standalone = standalone# flag to create standalone LaTeX file
+        self.sets = []              # list of set objects
 
-        # Initialize the sets list.
-        if sets is None:
-            self.sets = []         # list of set objects
-        else:
-            if isinstance(sets, tuple):
-                self.sets = list(sets)
-            elif isinstance(sets, Set):
-                self.sets = [sets]
-
-        # Assign class-wide attributes.
-        if skip == False or skip == True:
-            graph.skip = skip
-        if silent == False or silent == True:
-            graph.silent = silent
-        if directory is not None:
-            graph.directory = directory
-
-    def set(self, x, y, z=None, color=None, opacity=1.0,
-            style=STYLE_LINE, size=THICK, label=None, fmt=None, simp=True):
-        p = Set(x=x, y=y, z=z, color=color, opacity=opacity,
-                style=style, size=size, label=label,
-                fmt=fmt, simp=simp)
-        self.sets.append(p)
-        return p
-
-    def solid(self, x, y=None, color=None, opacity=1.0,
-            width=THICK, label=None, fmt=None, simp=True):
-        if y is None:
-            y = x.copy()
-            K = x.shape[-1]
-            x = np.arange(K)
-        p = Set(x=x, y=y, z=None, color=color, opacity=opacity,
-                style=STYLE_LINE, size=width, label=label,
-                fmt=fmt, simp=simp)
-        self.sets.append(p)
-        return p
-
-    def dashed(self, x, y=None, color=None, opacity=1.0,
-            width=THICK, label=None, fmt=None, simp=True):
-        if y is None:
-            y = x.copy()
-            K = x.shape[-1]
-            x = np.arange(K)
-        fmt = "dashed" if fmt is None else fmt + ", dashed"
-        p = Set(x=x, y=y, z=None, color=color, opacity=opacity,
-                style=STYLE_LINE, size=width, label=label,
-                fmt=fmt, simp=simp)
-        self.sets.append(p)
-        return p
-
-    def dotted(self, x, y=None, color=None, opacity=1.0,
-            width=THICK, label=None, fmt=None, simp=True):
-        if y is None:
-            y = x.copy()
-            K = x.shape[-1]
-            x = np.arange(K)
-        fmt = "dotted" if fmt is None else fmt + ", dotted"
-        p = Set(x=x, y=y, z=None, color=color, opacity=opacity,
-                style=STYLE_LINE, size=width, label=label,
-                fmt=fmt, simp=simp)
+    def plot(self, x, y=None, color=None, opacity=1.0, width=THICK,
+            pattern=None, label=None, simp=True, fmt=None):
+        fmt = append_to_fmt(fmt, opacity, width, pattern)
+        p = Set(x=x, y=y, color=color,
+                func=plot_set, label=label, simp=simp, fmt=fmt)
         self.sets.append(p)
         return p
 
-    def dashdotted(self, x, y=None, color=None, opacity=1.0,
-            width=THICK, label=None, fmt=None, simp=True):
-        if y is None:
-            y = x.copy()
-            K = x.shape[-1]
-            x = np.arange(K)
-        fmt = "dashdotted" if fmt is None else fmt + ", dashdotted"
-        p = Set(x=x, y=y, z=None, color=color, opacity=opacity,
-                style=STYLE_LINE, size=width, label=label,
-                fmt=fmt, simp=simp)
+    def scatter(self, x, y=None, radius=0.03, color=None, opacity=1.0,
+            marker=CIRCLES, label=None, fmt=None):
+        # `radius` can be either a scalar or
+        # an array compatible with `x` and `y`.
+        fmt = append_to_fmt(fmt, opacity, None, None)
+        radius = 0.01 if radius is None else radius
+        p = Set(x=x, y=y, z=radius, color=color, marker=marker,
+                func=scatter_set, label=label, simp=False, fmt=fmt)
         self.sets.append(p)
         return p
 
-    def circles(self, x, y=None, radius=0.01, color=None, opacity=1.0,
-            width=THICK, label=None, fmt=None, simp=False):
-        if y is None:
-            y = x.copy()
-            K = x.shape[-1]
-            x = np.arange(K)
-        p = Set(x=x, y=y, z=radius, color=color, opacity=opacity,
-                style=STYLE_CIRCLES, size=width, label=label,
-                fmt=fmt, simp=simp)
+    def fill(self, x, y=None, z=None, color=None, opacity=1.0,
+            label=None, simp=True, fmt=None):
+        # If `y` and `z` are given, this becomes a fill-between.
+        fmt = append_to_fmt(fmt, opacity, None, None)
+        p = Set(x=x, y=y, z=z, zony=(z is not None), color=color,
+                func=fill_set, label=label, simp=simp, fmt=fmt)
         self.sets.append(p)
         return p
 
-    def dots(self, x, y=None, radius=0.01, color=None, opacity=1.0,
-            label=None, fmt=None, simp=False):
-        if y is None:
-            y = x.copy()
-            K = x.shape[-1]
-            x = np.arange(K)
-        p = Set(x=x, y=y, z=radius, color=color, opacity=opacity,
-                style=STYLE_DOTS, size=None, label=label,
-                fmt=fmt, simp=simp)
+    def hexbin(self, x, y=None, radius=0.2, color=None, opacity=1.0, scaling=0,
+            label=None, fmt=None):
+        # `radius` must be a scalar. A negative `radius` yields variable-size
+        # hexagons. `scaling` adjusts the weighting curve to the hexagonal
+        # shading (or sizing).
+        fmt = append_to_fmt(fmt, opacity, None, None)
+        p = Set(x=x, y=y, z=radius, color=color, scaling=scaling,
+                func=hexbin_set, label=label, simp=False, fmt=fmt)
         self.sets.append(p)
         return p
 
-    def filled(self, x, y=None, color=None, opacity=1.0,
-            label=None, fmt=None, simp=True):
-        if y is None:
-            y = x.copy()
-            K = x.shape[-1]
-            x = np.arange(K)
-        p = Set(x=x, y=y, z=None, color=color, opacity=opacity,
-                style=STYLE_FILLED, size=None, label=label,
-                fmt=fmt, simp=simp)
-        self.sets.append(p)
-        return p
-
-    def filledpairs(self, x, y=None, color=None, opacity=1.0,
-            label=None, fmt=None, simp=True):
-        if y is None:
-            y = x.copy()
-            K = x.shape[-1]
-            x = np.arange(K)
-        p = Set(x=x, y=y, z=None, color=color, opacity=opacity,
-                style=STYLE_FILLPAIRS, size=None, label=label,
-                fmt=fmt, simp=simp)
-        self.sets.append(p)
-        return p
-
-    def hexbin(self, x, y=None, color=None, opacity=1.0,
-            radius=0.2, label=None, fmt=None):
-        # A negative `radius` yields variable-size hexagons.
-        if y is None:
-            y = x.copy()
-            K = x.shape[-1]
-            x = np.arange(K)
-        p = Set(x=x, y=y, z=None, color=color, opacity=opacity,
-                style=STYLE_HEXBIN, size=radius, label=label,
-                fmt=fmt, simp=False)
-        self.sets.append(p)
-        return p
-
-    def render(self, sets=None):
+    def render(self):
         # Skip all the plotting code if the flag is set.
-        if graph.skip:
+        if config.skip:
             return
 
-        # Append additional sets to the list of sets.
-        if sets is not None:
-            # Ensure sets is a list.
-            if isinstance(sets, tuple):
-                sets = list(sets)
-            elif isinstance(sets, Set):
-                sets = [sets]
-            # Append to the list.
-            self.sets = self.sets + sets
-
-        # --------------------
-        # Plan out the figure.
-        # --------------------
+        # Ensure `x` and `y` are arrays with no more than 2 dimensions and
+        # are compatibly shaped. If `z` is defined, ensure it is a scalar or
+        # compatibly shaped with `x` and `y`.
+        check_shapes(self.sets)
+
+        # --------------------------------------------
+        # Plan the figure dimensions and data scaling.
+        # --------------------------------------------
 
         # Initialize the layout.
-        lay = Layout()
+        lay = GraphLayout()
 
-        # Get the viewing region. Find the mins and maxs and adjust for required
-        # padding.
-        get_view(self, self.sets, lay)
+        # Get the viewing region. Find the mins and maxs,
+        # ignoring nans and infs, and adjust for required padding.
+        get_data_view(self, self.sets, lay)
 
         # Get the size of the box and margins.
         get_layout(self, self.sets, lay)
 
         # Get the scaling factors and conditionally apply equal scaling. Equal
-        # scaling will alter the mins and maxs.
+        # scaling will alter the mins and maxs found in `get_data_view` and,
+        # consequently, will alter the scaling factors. Getting adjusted mins
+        # and maxs to satisfy equal scaling was also done by the `get_layout`
+        # function, but that was necessary to make guesses about the available
+        # drawing box size because of the potential impact of tick label
+        # placement. Once the box size has been set, however, the mins and maxs
+        # need to be recalculated if equal scaling is required.
         get_scaling(self, lay)
 
-        # Get grid line locations (in linear scaling).
+        # ------------------------------------------
+        # Position the grids, axes, and tick labels.
+        # ------------------------------------------
+
+        # Get grid line locations (in linear scaling). This step was already
+        # done once by the `get_layout` function, but that was only an
+        # approximation in order to determine the required sizes for the margins
+        # because of the placement of tick labels. Once the box size has been
+        # set, the mins and maxs were recalculated (to satisfy possible equal
+        # scaling) which requires that the grid placements be recalculated.
         if self.xlog:
             x_grids, x_sub_grids = grid_logarithmic(lay.x_min, lay.x_max)
         else:
             x_grids, x_sub_grids = grid_linear(lay.x_min, lay.x_max, lay.W_box,
                     max(lay.L_x_tick, lay.R_x_tick, lay.W_box/10))
         if self.ylog:
             y_grids, y_sub_grids = grid_logarithmic(lay.y_min, lay.y_max)
         else:
             y_grids, y_sub_grids = grid_linear(lay.y_min, lay.y_max, lay.H_box,
                     2*lay.font_size/PT_PER_CM)
 
-        # Determine where the x and y axes would be.
+        # Determine where the `x` and `y` axes would be in the drawing box. For
+        # log scale or outside axes, the position in the box is left and bottom.
+        # Otherwise, scale to centimeter units and bound within the box.
         if self.yout or self.xlog:
-            lay.X_axes = 0.0
+            lay.X_axes = 0.0 # bottom edge of drawing box
         else:
             lay.X_axes = to_scale(0, lay.x_min, lay.x_scale, self.xlog)
             lay.X_axes = max(0, min(lay.X_axes, lay.W_box))
         if self.xout or self.ylog:
-            lay.Y_axes = 0.0
+            lay.Y_axes = 0.0 # left edge of drawing box
         else:
             lay.Y_axes = to_scale(0, lay.y_min, lay.y_scale, self.ylog)
             lay.Y_axes = max(0, min(lay.Y_axes, lay.H_box))
 
-        # Determine what the tick format would be.
+        # Determine what the tick format should be.
         if self.xout or lay.Y_axes > lay.L_text:
             lay.x_tick_fmt = "below"
             lay.x_tick_shift = -lay.L_tick_shift
         else:
             lay.x_tick_fmt = "above"
             lay.x_tick_shift = lay.L_tick_shift
-        if not self.xout:
-            lay.x_tick_fmt += ", draw opacity=0.8"
         if self.yout or lay.X_axes > lay.W_box/2:
             lay.y_tick_fmt = "left"
             lay.y_tick_shift = -lay.L_tick_shift
         else:
             lay.y_tick_fmt = "right"
             lay.y_tick_shift = lay.L_tick_shift
-        if not self.yout:
-            lay.y_tick_fmt += ", draw opacity=0.8"
 
         # -----------------------
         # Write the data to file.
         # -----------------------
 
         # Open the output file.
-        if graph.directory is None:
-            fid = open(self.filename + ".tex", "w")
-        else:
-            fid = open(graph.directory + "/" + self.filename + ".tex", "w")
+        filepath = "" if config.directory is None else config.directory + "/"
+        filepath += self.filename + ".tex"
+        fid = open(filepath, "w")
 
         # Open the standalone TikZ script.
         if self.standalone:
             write_open(fid, self.preamble)
         elif self.preamble is not None:
-            print("Because this plot is not standalone, the additional "
-                    + "preamble will not be used.")
+            print("Because this plot is not standalone, "
+                    + "the additional preamble cannot be used.")
 
         # Define the font size.
         write_textstyle(fid, lay.font_size_name)
 
         # Define the colors.
-        write_colors(fid, self.sets)
+        write_color_definitions(fid, self.sets)
 
         # Reserve the full figure space: the box and margins.
         write_reserve(fid, lay)
 
         # Draw the sub-grids and grids.
         if self.xsubgrid:
             grids = to_scale(x_sub_grids, lay.x_min, lay.x_scale, self.xlog)
@@ -432,67 +382,33 @@
         if self.xgrid:
             grids = to_scale(x_grids, lay.x_min, lay.x_scale, self.xlog)
             write_xgrid(fid, grids, lay.H_box)
         if self.ygrid:
             grids = to_scale(y_grids, lay.y_min, lay.y_scale, self.ylog)
             write_ygrid(fid, grids, lay.W_box)
 
-        # Start a clip environment to contain the drawing.
-        write_begin_clip(fid, lay.W_box, lay.H_box)
+        # Begin a scope.
+        write_scope_begin(fid)
+
+        # Clip everything with this scope to the drawing box.
+        write_clip(fid, lay.W_box, lay.H_box)
 
         # Set line style to rounded.
         write_rounded(fid)
 
         # Draw the sets.
         for j in range(len(self.sets)):
             # Introduce this data set.
             write_comment(fid, f"Set {j}")
+            self.sets[j].func(fid, self.sets[j], lay.x_min, lay.y_min,
+                    lay.x_scale, lay.y_scale, self.xlog, self.ylog,
+                    lay.W_box, lay.H_box)
 
-            # Get the data set.
-            set_j = self.sets[j]
-            X = to_scale(set_j.x, lay.x_min, lay.x_scale, self.xlog)
-            Y = to_scale(set_j.y, lay.y_min, lay.y_scale, self.ylog)
-            Z = set_j.z
-            opacity = set_j.opacity
-            style = set_j.style
-            size = set_j.size
-            fmt = set_j.fmt
-            simp = set_j.simp
-
-            # Append color, opacity, and line width to the format specification.
-            pre = ""
-            if fmt is not None:
-                pre = ", "
-            else:
-                fmt = ""
-            if opacity != 1.0:
-                fmt += pre + f"opacity={opacity:0.3g}"
-                pre = ", "
-            if style in [STYLE_LINE, STYLE_CIRCLES] and size != THIN:
-                fmt += pre + f"line width={size:0.3g}pt"
-                pre = ", "
-            fmt += pre + f"C{j}"
-
-            # Draw the data.
-            if style == STYLE_LINE:
-                draw_set(fid, j, X, Y, fmt, simp, lay.W_box, lay.H_box)
-            elif style in [STYLE_CIRCLES, STYLE_DOTS]:
-                mark_set(fid, j, X, Y, Z, fmt, style, size,
-                        simp, lay.W_box, lay.H_box)
-            elif style == STYLE_FILLPAIRS:
-                fillpairs_set(fid, j, X, Y, fmt,
-                        simp, lay.W_box, lay.H_box)
-            elif style == STYLE_HEXBIN:
-                hex_set(fid, j, X, Y, fmt, size,
-                        simp, lay.W_box, lay.H_box)
-            else:
-                print(f"Unknown style for set {j}: {style}")
-
-        # End the clip environment.
-        write_end_clip(fid)
+        # End the scope.
+        write_scope_end(fid)
 
         # Draw the axes.
         write_comment(fid, "Draw axes.")
         if self.xaxis:
             write_line(fid, -self.ticksize/2, lay.Y_axes,
                     lay.W_box + self.ticksize, lay.Y_axes, "->")
         if self.yaxis:
@@ -506,84 +422,103 @@
 
             # Scale the grid lines to paper dimensions.
             X = to_scale(x_grids, lay.x_min, lay.x_scale, self.xlog)
 
             # Determine the form for the tick labels and their precision.
             format_func, precision = get_num_format(self.xlog, x_grids)
 
+            # Get the tick label strings and their widths.
+            tick_labels = []
+            tick_widths = []
+            tick_skip = [False for n in range(len(X))]
             for n in range(len(X)):
-                # Get the label string and its width.
                 txt, w_txt = format_func(x_grids[n], precision, lay.font_size)
-                W_txt = w_txt/PT_PER_CM
-
-                # Skip the tick labels too close to the axis.
+                tick_labels.append(txt)
+                tick_widths.append(w_txt/PT_PER_CM)
                 if not self.xout:
                     dist_to_axis = math.fabs(X[n] - lay.X_axes)
-                    if self.yaxis and dist_to_axis < W_txt/2:
-                        continue
+                    if self.yaxis and dist_to_axis < tick_widths[n]/2:
+                        tick_skip[n] = True
                     dist_to_edge = min(math.fabs(X[n]),
                             math.fabs(lay.W_box - X[n]))
-                    if dist_to_edge < W_txt/2:
-                        continue
+                    if dist_to_edge < tick_widths[n]/2:
+                        tick_skip[n] = True
 
-                # Draw the tick line.
+            # Write the tick marks.
+            for n in range(len(X)):
+                if tick_skip[n]:
+                    continue
                 write_line(fid, X[n], lay.Y_axes - self.ticksize/2,
                         X[n], lay.Y_axes + self.ticksize/2)
 
-                # Wrap the text string in math mode.
-                txt = "$" + txt + "$"
-
-                # Add a white contour.
-                if not self.xout:
-                    txt = f"\\contour{{white}}{{{txt}}}"
-
-                # Write the tick label.
+            # Write the tick labels.
+            if not self.xout:
+                write_scope_begin(fid, "opacity=0.8")
+                write_outline_style(fid)
+                for n in range(len(X)):
+                    if tick_skip[n]:
+                        continue
+                    write_text(fid, X[n], lay.Y_axes + lay.x_tick_shift,
+                            "$" + tick_labels[n] + "$\\strut", lay.x_tick_fmt)
+                write_scope_end(fid)
+            for n in range(len(X)):
+                if tick_skip[n]:
+                    continue
                 write_text(fid, X[n], lay.Y_axes + lay.x_tick_shift,
-                        txt + "\\strut", lay.x_tick_fmt)
+                        "$" + tick_labels[n] + "$\\strut", lay.x_tick_fmt)
 
         # Write the y-axis ticks and labels.
         if self.ytick and self.yaxis: # Ticks without an axis look weird.
             # Comment.
             write_comment(fid, "Draw y-axis ticks and labels.")
 
             # Scale the grid lines to paper dimensions.
             Y = to_scale(y_grids, lay.y_min, lay.y_scale, self.ylog)
 
             # Determine the form for the tick labels and their precision.
             format_func, precision = get_num_format(self.ylog, y_grids)
 
+            # Get the tick label strings and their widths.
+            tick_labels = []
+            tick_skip = [False for n in range(len(Y))]
             tol_to_axis = lay.font_size/(2*PT_PER_CM)
             for n in range(len(Y)):
-                # Get the label string.
                 txt, _ = format_func(y_grids[n], precision, lay.font_size)
-
-                # Skip the tick on the axis.
+                tick_labels.append(txt)
                 if not self.yout:
                     dist_to_axis = math.fabs(Y[n] - lay.Y_axes)
                     if self.xaxis and dist_to_axis < tol_to_axis:
-                        continue
+                        tick_skip[n] = True
                     dist_to_edge = min(math.fabs(Y[n]),
                             math.fabs(lay.H_box - Y[n]))
                     if dist_to_edge < tol_to_axis:
-                        continue
+                        tick_skip[n] = True
 
-                # Draw the tick line.
+            # Write the tick marks.
+            for n in range(len(Y)):
+                if tick_skip[n]:
+                    continue
                 write_line(fid, lay.X_axes - self.ticksize/2, Y[n],
                         lay.X_axes + self.ticksize/2, Y[n])
 
-                # Wrap the text string in math mode.
-                txt = "$" + txt + "$"
-
-                # Add a white contour.
-                if not self.yout:
-                    txt = f"\\contour{{white}}{{{txt}}}"
-
-                # Write the tick text.
+            # Write the tick labels.
+            if not self.yout:
+                write_scope_begin(fid, "opacity=0.8")
+                write_outline_style(fid)
+                for n in range(len(Y)):
+                    if tick_skip[n]:
+                        continue
+                    write_text(fid, lay.X_axes + lay.y_tick_shift, Y[n],
+                            "$" + tick_labels[n] + "$\\strut", lay.y_tick_fmt)
+                write_scope_end(fid)
+            for n in range(len(Y)):
+                if tick_skip[n]:
+                    continue
                 write_text(fid, lay.X_axes + lay.y_tick_shift, Y[n],
-                        txt + "\\strut", lay.y_tick_fmt)
+                        "$" + tick_labels[n] + "$\\strut", lay.y_tick_fmt)
 
         # Write the axis labels (inside the figure space).
         if self.xlabel is not None:
             write_comment(fid, "Write x-axis label.")
             write_text(fid, lay.W_box/2, -lay.B_margin,
                     self.xlabel + "\\strut", "above")
         if self.ylabel is not None:
@@ -635,29 +570,105 @@
         # -----------------
         # Compile the file.
         # -----------------
 
         # Compile the LaTeX file.
         if self.standalone:
             cmd = 'pdflatex'
-            if graph.silent:
+            if config.silent:
                 cmd = cmd + ' --interaction=batchmode'
-            if graph.directory is None:
+            if config.directory is None:
                 os.system(f'{cmd} {self.filename}.tex')
                 os.system(f'rm {self.filename}.aux')
                 os.system(f'rm {self.filename}.log')
             else:
                 pwd = os.getcwd()
-                cmd = f'{cmd} -output-directory="{pwd}/{graph.directory}"'
-                os.system(f'{cmd} "{graph.directory}/{self.filename}.tex"')
-                os.system(f'rm {graph.directory}/{self.filename}.aux')
-                os.system(f'rm {graph.directory}/{self.filename}.log')
+                cmd = f'{cmd} -output-directory="{pwd}/{config.directory}"'
+                os.system(f'{cmd} "{config.directory}/{self.filename}.tex"')
+                os.system(f'rm {config.directory}/{self.filename}.aux')
+                os.system(f'rm {config.directory}/{self.filename}.log')
+
+# ---------------------
+# Calculation Functions
+# ---------------------
 
+def check_shapes(sets):
+    # Cycle through each data set.
+    for j in range(len(sets)):
+        # Parse the x and y fields.
+        x = sets[j].x
+        y = sets[j].y
+        z = sets[j].z
 
-def get_view(fig, sets, lay):
+        # Convert scalars, lists, and tuples to arrays.
+        # None values will be unaffected.
+        if isinstance(x, (int, float)):
+            x = np.asarray([x], dtype=float)
+        elif isinstance(x, (list, tuple)):
+            x = np.asarray(x, dtype=float)
+        if isinstance(y, (int, float)):
+            y = np.asarray([y], dtype=float)
+        elif isinstance(y, (list, tuple)):
+            y = np.asarray(y, dtype=float)
+        if isinstance(z, int):
+            z = float(z) # Do not convert scalar z to array.
+        elif isinstance(z, (list, tuple)):
+            z = np.asarray(z, dtype=float)
+
+        # Ensure some data was defined.
+        if (x is None) and (y is None) and (z is None):
+            raise ValueError(f"No data was defined for data set {j}.")
+
+        # Handle undefined arrays.
+        if y is None:
+            if z is not None:
+                y = z
+                z = None
+            if x is not None:
+                y = x
+                x = None
+        if x is None:
+            x = np.arange(y.shape[-1])
+
+        # Check for too many dimensions. At this point,
+        # `x` and `y` are guaranteed to be arrays.
+        if x.ndim > 2:
+            raise ValueError(f"x in set {j} has too many dimensions.")
+        if y.ndim > 2:
+            raise ValueError(f"y in set {j} has too many dimensions.")
+        if (z is not None) and (np.ndim(z) > 2):
+            raise ValueError(f"z in set {j} has too many dimensions.")
+
+        # Check for incompatible dimensions.
+        xrows, xcols = (1, len(x)) if x.ndim == 1 else x.shape
+        yrows, ycols = (1, len(y)) if y.ndim == 1 else y.shape
+        if (xcols != ycols) or \
+                ((xrows > 1) and (yrows > 1) and (xrows != yrows)):
+            raise ValueError(f"x ({xrows},{xcols}) "
+                    + f"and y ({yrows},{ycols}) in set {j} "
+                    + "are incompatible")
+        rows = max(xrows, yrows)
+        if (z is not None) and (np.ndim(z) > 0):
+            zrows, zcols = (1, len(z)) if z.ndim == 1 else z.shape
+            if ((zcols > 1) and (zcols != xcols)) or \
+                    ((zrows > 1) and (rows > 1) and (zrows != rows)):
+                raise ValueError(f"x ({xrows},{xcols}) "
+                        + f"and y ({yrows},{ycols}) "
+                        + f"and z ({zrows},{zcols}) in set {j} "
+                        + "are incompatible")
+            rows = max(rows, zrows)
+
+        # Save to the data set.
+        sets[j].x = x
+        sets[j].y = y
+        sets[j].z = z
+        sets[j].rows = rows
+
+
+def get_data_view(fig, sets, lay):
     # Define constants.
     tol = 1e-45 # position tolerance
     pad_ratio = 0.1 # padding ratio of figure width
 
     # Initialize the minimums and maximums.
     lay.x_min = math.inf
     lay.x_max = -math.inf
@@ -665,101 +676,92 @@
     lay.y_max = -math.inf
 
     # Check the range of each set.
     for j in range(len(sets)):
         # Parse the x and y fields.
         x = sets[j].x
         y = sets[j].y
+        z = sets[j].z
+        zony = sets[j].zony
 
-        # Convert x and y to ndarrays.
-        if isinstance(x, (int, float)):
-            x = np.array([x], dtype=float)
-            sets[j].x = x
-        elif isinstance(x, (list, tuple)):
-            x = np.array(x)
-            sets[j].x = x
-        if isinstance(y, (int, float)):
-            y = np.array([y], dtype=float)
-            sets[j].y = y
-        elif isinstance(y, (list, tuple)):
-            y = np.array(y)
-            sets[j].y = y
-
-        # Check the dimensions.
-        if x.shape[-1] != y.shape[-1]:
-            raise ValueError("x and y do not have the same lengths "
-                    + f"in their last dimensions for set {j}.")
-
-        # Get extrema of this set, ignoring nans and infs.
-        x_valid = np.ma.masked_invalid(x)
-        y_valid = np.ma.masked_invalid(y)
-        x_min = x_valid.min()
-        x_max = x_valid.max()
-        y_min = y_valid.min()
-        y_max = y_valid.max()
-
-        # Enlarge minimums and maximums.
-        if x_min < lay.x_min:
-            lay.x_min = x_min
-        if x_max > lay.x_max:
-            lay.x_max = x_max
-        if y_min < lay.y_min:
-            lay.y_min = y_min
-        if y_max > lay.y_max:
-            lay.y_max = y_max
-
-    # Adjust for log scaling.
-    if fig.xlog and lay.x_min <= 0.0:
-        print("Negative values cannot be plotted in a log-scale x axis.")
-        lay.x_min = tol
-    if fig.ylog and lay.y_min <= 0.0:
-        print("Negative values cannot be plotted in a log-scale y axis.")
-        lay.y_min = tol
+        # Get the maximum number of rows.
+        rows = max(1, x.shape[0]*(x.ndim > 1), y.shape[0]*(y.ndim > 1))
+        if zony:
+            rows = max(rows, z.shape[0]*(z.ndim > 1))
+
+        # For each row in the data set,
+        for row in range(rows):
+            # Get the data for this row.
+            xr = x if x.ndim == 1 else x[row]
+            yr = y if y.ndim == 1 else y[row]
+            if zony:
+                zr = z if z.ndim == 1 else z[row]
+
+            # Find the valid points (not nan, inf, or negative (for log)).
+            nn = np.arange(len(xr))
+            xr_fin = np.isfinite(xr)
+            yr_fin = np.isfinite(yr)
+            nx_valid = nn[xr_fin & (xr > 0)] if fig.xlog else nn[xr_fin]
+            ny_valid = nn[yr_fin & (yr > 0)] if fig.ylog else nn[yr_fin]
+            nn_valid = np.intersect1d(nx_valid, ny_valid)
+            if zony:
+                zr_fin = np.isfinite(zr)
+                nz_valid = nn[zr_fin & (zr > 0)] if fig.ylog else nn[zr_fin]
+                nn_valid = np.intersect1d(nn_valid, nz_valid)
+
+            # Enlarge x extrema.
+            x_min = xr[nn_valid].min()
+            x_max = xr[nn_valid].max()
+            if x_min < lay.x_min:
+                lay.x_min = x_min
+            if x_max > lay.x_max:
+                lay.x_max = x_max
+
+            # Enlarge y extrema.
+            y_min = yr[nn_valid].min()
+            y_max = yr[nn_valid].max()
+            if y_min < lay.y_min:
+                lay.y_min = y_min
+            if y_max > lay.y_max:
+                lay.y_max = y_max
+
+            # Enlarge y extrema with z.
+            if zony:
+                z_min = zr[nn_valid].min()
+                z_max = zr[nn_valid].max()
+                if z_min < lay.y_min:
+                    lay.y_min = z_min
+                if z_max > lay.y_max:
+                    lay.y_max = z_max
 
     # Add x-axis padding if requested or needed.
-    if lay.x_max == lay.x_min:
-        # Add a very small padding.
-        lay.x_min -= tol
-        lay.x_max += tol
-    elif fig.xpad:
-        # Temporarily convert to logarithmic scaling.
-        if fig.xlog:
-            lay.x_min = math.log10(lay.x_min)
-            lay.x_max = math.log10(lay.x_max)
-
-        # Add padding.
-        w = lay.x_max - lay.x_min
-        lay.x_min -= w*pad_ratio/2
-        lay.x_max += w*pad_ratio/2
-
-        # Convert back to linear scaling.
-        if fig.xlog:
-            lay.x_min = 10.0**lay.x_min
-            lay.x_max = 10.0**lay.x_max
+    tol = 1e-45
+    if fig.xlog: # temporarily log scale
+        lay.x_min = math.log10(lay.x_min)
+        lay.x_max = math.log10(lay.x_max)
+        tol = 1.0
+    w = lay.x_max - lay.x_min
+    lay.x_min -= (w == 0)*tol + (fig.xpad)*w*pad_ratio/2
+    lay.x_max += (w == 0)*tol + (fig.xpad)*w*pad_ratio/2
+    if fig.xlog: # back to linear scale
+        lay.x_min = 10.0**lay.x_min
+        lay.x_max = 10.0**lay.x_max
 
     # Add y-axis padding if requested or needed.
-    if lay.y_max == lay.y_min:
-        # Add a very small padding.
-        lay.y_min -= tol
-        lay.y_max += tol
-    elif fig.ypad:
-        # Temporarily convert to logarithmic scaling.
-        if fig.ylog:
-            lay.y_min = math.log10(lay.y_min)
-            lay.y_max = math.log10(lay.y_max)
-
-        # Add padding.
-        h = lay.y_max - lay.y_min
-        lay.y_min -= h*pad_ratio/2
-        lay.y_max += h*pad_ratio/2
-
-        # Convert back to linear scaling.
-        if fig.ylog:
-            lay.y_min = 10.0**lay.y_min
-            lay.y_max = 10.0**lay.y_max
+    tol = 1e-45
+    if fig.ylog: # temporarily log scale
+        lay.y_min = math.log10(lay.y_min)
+        lay.y_max = math.log10(lay.y_max)
+        tol = 1.0
+    h = lay.y_max - lay.y_min
+    lay.y_min -= (h == 0)*tol + (fig.ypad)*h*pad_ratio/2
+    lay.y_max += (h == 0)*tol + (fig.ypad)*h*pad_ratio/2
+    if fig.ylog: # back to linear scale
+        lay.y_min = 10.0**lay.y_min
+        lay.y_max = 10.0**lay.y_max
 
     # Override for requested limits.
     if fig.xmin is not None:
         lay.x_min = fig.xmin
     if fig.xmax is not None:
         lay.x_max = fig.xmax
     if fig.ymin is not None:
@@ -853,15 +855,15 @@
     lay.legend_cols = 0
     lay.legend_rows = 0
     for j in range(len(sets)):
         if sets[j].label is not None:
             labeled += 1
     if labeled > 0:
         if fig.columns is None:
-            lay.legend_cols = round(lay.width/2.54)
+            lay.legend_cols = round(lay.width/2.0)
             if lay.legend_cols + 1 >= labeled:
                 lay.legend_cols = labeled
         else:
             lay.legend_cols = fig.columns
         lay.legend_rows = int(math.ceil(labeled/lay.legend_cols))
         if fig.xlabel:
             legend_buff = 0.25*lay.L_text
@@ -878,22 +880,22 @@
     x_min = lay.x_min
     x_max = lay.x_max
     y_min = lay.y_min
     y_max = lay.y_max
 
     # Get the tick-label dimensions, assuming the worst-case label widths.
     # This width is based on a number of the form "-m.mm x 10^(-eee)".
-    if fig.xtick and fig.xaxis and fig.xout:
+    if fig.xtick and fig.xaxis and fig.xout: # Ticks without an axis are weird.
         if fig.xlog:
             W_x_tick = 2.5*lay.font_size/PT_PER_CM
         else:
             W_x_tick = 6.0*lay.font_size/PT_PER_CM
     else:
         W_x_tick = 0.0
-    if fig.ytick and fig.yaxis and fig.yout:
+    if fig.ytick and fig.yaxis and fig.yout: # Ticks without an axis are weird.
         if fig.ylog:
             W_y_tick = 2.5*lay.font_size/PT_PER_CM
         else:
             W_y_tick = 6.0*lay.font_size/PT_PER_CM
     else:
         W_y_tick = 0.0
     H_y_tick = lay.L_text if fig.ytick and fig.yaxis else 0.0
@@ -906,15 +908,16 @@
     T_margin = max(fig.ticksize, H_y_tick/2)
 
     # Initialize the box size.
     W_box = lay.width - L_margin - R_margin
     H_box = lay.height - B_margin - T_margin - lay.H_legend
 
     # Adjust the limits for equal axis scaling. For equal axis scaling to affect
-    # anything, xlog must equal ylog.
+    # anything, xlog must equal ylog. This operation will be repeated by the
+    # `get_scaling` function once the drawing box size has been determined.
     if fig.equal and fig.xlog == fig.ylog:
         # Temporarily convert to logarithmic scaling.
         if fig.xlog and fig.ylog:
             x_min = math.log10(x_min)
             x_max = math.log10(x_max)
             y_min = math.log10(y_min)
             y_max = math.log10(y_max)
@@ -951,17 +954,17 @@
                 5*lay.font_size/PT_PER_CM)
     if fig.ylog:
         y_grids, _ = grid_logarithmic(y_min, y_max)
     else:
         y_grids, _ = grid_linear(y_min, y_max, H_box,
                 2*lay.font_size/PT_PER_CM)
 
-    # -------------------------------------
-    # Get the dimensions of the components.
-    # -------------------------------------
+    # --------------------------------------
+    # Get the dimensions of the tick labels.
+    # --------------------------------------
 
     # Get x-axis, tick-label margins.
     lay.L_x_tick = 0.0
     lay.R_x_tick = 0.0
     lay.H_x_tick = 0.0
     if fig.xtick and fig.xaxis: # Ticks without an axis look weird.
         # Height of tick label.
@@ -1255,14 +1258,37 @@
     """
     Simplify the u and v data path by replacement with a line that breaks when
     points are too far from the line. This algorithm works by setting a range of
     angles of tangent lines to a circle about the last pinned point. All future
     points must be between those tangent lines. This algorithm achieves a
     similar result to the Ramer-Douglas-Peucker algorithm, but with far fewer
     calculations.
+
+    Parameters
+    ----------
+    u : (N,) float np.ndarray
+        x-axis array of points.
+    v : (N,) float np.ndarray
+        y-axis array of points.
+    tol : float
+        Maximum allowable distance of points from fitting lines.
+
+    Returns
+    -------
+    nn : (M,) int np.ndarray
+        Array of indices to keep from original (u, v) path. (u[nn], v[nn])
+        defines the simplified path.
+
+    Notes
+    -----
+    A single tolerance assumes equal units and scaling between `u` and `v`. If
+    this is not the case, simply prescale the `u` or `v` values according to
+    preference.
+
+    This algorithm was developed by David Woodburn.
     """
 
     # Get the circle radius.
     h = tol/2
 
     # Initialize the pin index and array.
     N = len(u)
@@ -1360,76 +1386,335 @@
     nn = nn[:m + 1]
 
     # Return just the pinned points.
     return nn
 
 
 def simp_best(X, Y, W_box, H_box):
-    nn = simp_map(X, Y, 0.001)
-    tol = THIN/PT_PER_CM
+    tol = THINEST/PT_PER_CM
+    nn = simp_map(X, Y, tol)
     x_chunks = round(W_box/(tol/2))
     y_chunks = round(H_box/(tol/2))
     if len(nn) > 2*max(x_chunks, y_chunks):
         dX = np.diff(X)
         dY = np.diff(Y)
         if np.all(dX >= 0) or np.all(dX <= 0): # X is monotonic
             nn = simp_chunks(X, Y, x_chunks)
         elif np.all(dY >= 0) or np.all(dY <= 0): # Y is monotonic
             nn = simp_chunks(Y, X, y_chunks)
     return nn
 
+# ------------------
+# Plotting Functions
+# ------------------
+
+def plot_set(fid, setj, x_min, y_min, x_scale, y_scale,
+        x_log, y_log, W_box, H_box):
+    # Make a reusable index array.
+    nn = np.arange(setj.x.shape[-1])
+
+    # For each row of the data set,
+    for row in range(setj.rows):
+        # Get this row of data. `z` will be None.
+        x = setj.x.copy() if setj.x.ndim == 1 else setj.x[row].copy()
+        y = setj.y.copy() if setj.y.ndim == 1 else setj.y[row].copy()
+
+        # Find the valid points (not nan, inf, or negative (for log)).
+        x_fin = np.isfinite(x)
+        y_fin = np.isfinite(y)
+        nx_valid = nn[x_fin & (x > 0)] if x_log else nn[x_fin]
+        ny_valid = nn[y_fin & (y > 0)] if y_log else nn[y_fin]
+        nn_valid = np.intersect1d(nx_valid, ny_valid)
+
+        # Scale the data.
+        X = x; Y = y # aliases of copied rows
+        X[nn_valid] = np.log10(x[nn_valid]/x_min)*x_scale if x_log \
+                else (x[nn_valid] - x_min)*x_scale
+        Y[nn_valid] = np.log10(y[nn_valid]/y_min)*y_scale if y_log \
+                else (y[nn_valid] - y_min)*y_scale
+
+        # Split the indices of valid points into contiguous segments.
+        nn_segs = np.split(nn_valid, np.where(np.diff(nn_valid) != 1)[0] + 1)
+
+        # For each segment,
+        if setj.rows > 1:
+            write_comment(fid, f"Row {row}")
+        for m, nn_seg in enumerate(nn_segs):
+            # Get the points of this segment.
+            X_seg = X[nn_seg]
+            Y_seg = Y[nn_seg]
+
+            # Simplify the data if requested.
+            if setj.simp:
+                nn_simp = simp_best(X_seg, Y_seg, W_box, H_box)
+                X_seg = X_seg[nn_simp]
+                Y_seg = Y_seg[nn_simp]
+
+            # Ensure segment is at least partially within the viewing region.
+            if (X_seg.min() > W_box) or (X_seg.max() < 0) or \
+                    (Y_seg.min() > H_box) or (Y_seg.max() < 0):
+                continue
+
+            # Write the code for this segment.
+            if len(nn_segs) > 1:
+                write_comment(fid, f"Segment {m}")
+            write_draw(fid, setj.fmt, X_seg, Y_seg, W_box, H_box)
+
+
+def scatter_set(fid, setj, x_min, y_min, x_scale, y_scale,
+        x_log, y_log, W_box, H_box):
+    # Make a reusable index array.
+    nn = np.arange(setj.x.shape[-1])
+
+    # For each row of the data set,
+    for row in range(setj.rows):
+        # Get this row of data. `z` will not be None.
+        x = setj.x.copy() if setj.x.ndim == 1 else setj.x[row].copy()
+        y = setj.y.copy() if setj.y.ndim == 1 else setj.y[row].copy()
+        radius = math.fabs(setj.z) if np.ndim(setj.z) == 0 else setj.z.copy()
+        if np.ndim(radius) == 2:
+            radius = radius[row]
+
+        # Find the valid points (not nan, inf, or negative (for log)).
+        x_fin = np.isfinite(x)
+        y_fin = np.isfinite(y)
+        nx_valid = nn[x_fin & (x > 0)] if x_log else nn[x_fin]
+        ny_valid = nn[y_fin & (y > 0)] if y_log else nn[y_fin]
+        nn_valid = np.intersect1d(nx_valid, ny_valid)
+        if np.ndim(radius) > 0:
+            nr_valid = nn[np.isfinite(radius) & (radius > 0)]
+            nn_valid = np.intersect1d(nn_valid, nr_valid)
+
+        # Scale the `x` and `y` data.
+        X = x; Y = y; R = radius # aliases of copied rows
+        X[nn_valid] = np.log10(x[nn_valid]/x_min)*x_scale if x_log \
+                else (x[nn_valid] - x_min)*x_scale
+        Y[nn_valid] = np.log10(y[nn_valid]/y_min)*y_scale if y_log \
+                else (y[nn_valid] - y_min)*y_scale
+
+        # Split the indices of valid points into contiguous segments. Though
+        # continuity is not necessary for scatter plot points, it does simplify
+        # the filtering process during the write function.
+        nn_segs = np.split(nn_valid, np.where(np.diff(nn_valid) != 1)[0] + 1)
+
+        # For each segment,
+        if setj.rows > 1:
+            write_comment(fid, f"Row {row}")
+        for m, nn_seg in enumerate(nn_segs):
+            # Get the points of this segment.
+            X_seg = X[nn_seg]
+            Y_seg = Y[nn_seg]
+            R_seg = R if np.ndim(R) == 0 else R[nn_seg]
+
+            # The `simp` option will always be False.
+
+            # Ensure segment is at least partially within the viewing region.
+            if ((X_seg - R_seg).min() > W_box) or \
+                    ((X_seg + R_seg).max() < 0) or \
+                    ((Y_seg - R_seg).min() > H_box) or \
+                    ((Y_seg + R_seg).max() < 0):
+                continue
+
+            # Write the code for this segment.
+            if len(nn_segs) > 1:
+                write_comment(fid, f"Segment {m}")
+            write_mark(fid, setj.marker, setj.fmt,
+                    X_seg, Y_seg, R_seg, W_box, H_box)
+
+
+def fill_set(fid, setj, x_min, y_min, x_scale, y_scale,
+        x_log, y_log, W_box, H_box):
+    # Make a reusable index array.
+    nn = np.arange(setj.x.shape[-1])
+
+    # For each row of the data set,
+    for row in range(setj.rows):
+        # Get this row of data. `z` could be None or an array, not a scalar.
+        x = setj.x.copy() if setj.x.ndim == 1 else setj.x[row].copy()
+        y = setj.y.copy() if setj.y.ndim == 1 else setj.y[row].copy()
+        if setj.z is not None:
+            z = setj.z.copy() if setj.z.ndim == 1 else setj.z[row].copy()
+        else:
+            z = None
 
-def hex_to_rgb(color):
-    """
-    Convert 24-bit color values to red, green, blue values on the scale of 0
-    to 255.  This function can take an ndarray of colors.
-    """
-
-    B = np.bitwise_and(color, 0xFF)
-    RG = np.right_shift(color, 8)
-    G = np.bitwise_and(RG, 0xFF)
-    R = np.right_shift(RG, 8)
-    return R, G, B
-
+        # Find the valid points (not nan, inf, or negative (for log)).
+        x_fin = np.isfinite(x)
+        y_fin = np.isfinite(y)
+        nx_valid = nn[x_fin & (x > 0)] if x_log else nn[x_fin]
+        ny_valid = nn[y_fin & (y > 0)] if y_log else nn[y_fin]
+        nn_valid = np.intersect1d(nx_valid, ny_valid)
+        if z is not None:
+            z_fin = np.isfinite(z)
+            nz_valid = nn[z_fin & (z > 0)] if y_log else nn[z_fin]
+            nn_valid = np.intersect1d(nn_valid, nz_valid)
+
+        # Scale the `x` and `y` data.
+        X = x; Y = y; Z = z # aliases of copied rows
+        X[nn_valid] = np.log10(x[nn_valid]/x_min)*x_scale if x_log \
+                else (x[nn_valid] - x_min)*x_scale
+        Y[nn_valid] = np.log10(y[nn_valid]/y_min)*y_scale if y_log \
+                else (y[nn_valid] - y_min)*y_scale
+        if Z is not None:
+            Z[nn_valid] = np.log10(z[nn_valid]/y_min)*y_scale if y_log \
+                    else (z[nn_valid] - y_min)*y_scale
+
+        # Split the indices of valid points into contiguous segments. Each
+        # contiguous segment will be plotted as a separate fill.
+        nn_segs = np.split(nn_valid, np.where(np.diff(nn_valid) != 1)[0] + 1)
+
+        # For each segment,
+        if setj.rows > 1:
+            write_comment(fid, f"Row {row}")
+        for m, nn_seg in enumerate(nn_segs):
+            # Get the points of this segment.
+            X_seg = X[nn_seg]
+            Y_seg = Y[nn_seg]
+            if Z is not None: # Append Z segment in reverse order.
+                X_seg = np.concatenate((X_seg, np.flip(X_seg)))
+                Y_seg = np.concatenate((Y_seg, np.flip(Z[nn_seg])))
+
+            # Simplify the data if requested.
+            if setj.simp:
+                nn_simp = simp_best(X_seg, Y_seg, W_box, H_box)
+                X_seg = X_seg[nn_simp]
+                Y_seg = Y_seg[nn_simp]
+
+            # Ensure segment is at least partially within the viewing region.
+            if (X_seg.min() > W_box) or (X_seg.max() < 0) or \
+                    (Y_seg.min() > H_box) or (Y_seg.max() < 0):
+                continue
+
+            # Write the code for this segment.
+            if len(nn_segs) > 1:
+                write_comment(fid, f"Segment {m}")
+            write_fill(fid, setj.fmt, X_seg, Y_seg, W_box, H_box)
+
+
+class HexGrid:
+    def __init__(self, radius, W_box, H_box):
+        # Mark if the hexagons should vary in size.
+        self.radius = math.fabs(radius)
+        self.variable = (radius < 0)
+
+        # Build the rectangular grid.
+        SQ3 = math.sqrt(3)
+        self.W_rect = SQ3/2 * self.radius # width of each rectangle
+        self.H_rect = 3/2 * self.radius # height of each rectangle
+        self.C_rect = math.ceil(W_box/self.W_rect) # columns of rectangles
+        self.R_rect = math.ceil(H_box/self.H_rect) # rows of rectangles
+        self.dX_rect = (self.C_rect*self.W_rect - W_box)/2 # rect x-axis shift
+        self.dY_rect = (self.R_rect*self.H_rect - H_box)/2 # rect y-axis shift
+
+        # Build the hexagonal bin grid.
+        self.C_hex = 1 + self.C_rect//2 # columns of hexagons
+        self.R_hex = 1 + self.R_rect # rows of hexagons
+        self.hexs = np.zeros((self.R_hex, self.C_hex))
+
+        # Define the hexagon vertex arrays.
+        C_vert = 2*self.C_hex + 2 # columns of vertices
+        R_vert = 2*self.R_hex + 2 # rows of vertices
+        cc_vert = np.arange(C_vert) # vertex column indices
+        rr_vert = np.arange(R_vert//2) # vertex row indices
+        s = self.radius
+        self.X_vert = np.round(cc_vert*(s*SQ3/2) - s*SQ3/2 - self.dX_rect, 4)
+        self.Y_vert = np.zeros(R_vert)
+        self.Y_vert[::2] = np.round(rr_vert*(3*s/2) - s - self.dY_rect, 4)
+        self.Y_vert[1::2] = np.round(rr_vert*(3*s/2) - s/2 - self.dY_rect, 4)
+
+
+def hexbin_set(fid, setj, x_min, y_min, x_scale, y_scale,
+        x_log, y_log, W_box, H_box):
+    # Define the hexagonal grid.
+    hex_grid = HexGrid(setj.z, W_box, H_box)
+
+    # Make a reusable index array.
+    nn = np.arange(setj.x.shape[-1])
+
+    # For each row of the data set,
+    for row in range(setj.rows):
+        # Get this row of data. Each row is weighted independently.
+        x = setj.x.copy() if setj.x.ndim == 1 else setj.x[row].copy()
+        y = setj.y.copy() if setj.y.ndim == 1 else setj.y[row].copy()
+
+        # Find the valid points (not nan, inf, or negative (for log)).
+        x_fin = np.isfinite(x)
+        y_fin = np.isfinite(y)
+        nx_valid = nn[x_fin & (x > 0)] if x_log else nn[x_fin]
+        ny_valid = nn[y_fin & (y > 0)] if y_log else nn[y_fin]
+        nn_valid = np.intersect1d(nx_valid, ny_valid)
+
+        # Scale the `x` and `y` data.
+        X = x; Y = y # aliases of copied rows
+        X[nn_valid] = np.log10(x[nn_valid]/x_min)*x_scale if x_log \
+                else (x[nn_valid] - x_min)*x_scale
+        Y[nn_valid] = np.log10(y[nn_valid]/y_min)*y_scale if y_log \
+                else (y[nn_valid] - y_min)*y_scale
+
+        # Split the indices of valid points into contiguous segments. Though
+        # continuity is not necessary for hexagonal binning, it does simplify
+        # the filtering process during the write function.
+        nn_segs = np.split(nn_valid, np.where(np.diff(nn_valid) != 1)[0] + 1)
+
+        # For each segment,
+        for m, nn_seg in enumerate(nn_segs):
+            # Get the points of this segment.
+            X_seg = X[nn_seg]
+            Y_seg = Y[nn_seg]
+
+            # The `simp` option will always be False.
+
+            # Ensure segment is at least partially within the viewing region.
+            if (X_seg.min() > W_box) or (X_seg.max() < 0) or \
+                    (Y_seg.min() > H_box) or (Y_seg.max() < 0):
+                continue
 
-def rgb_to_hex(R, G, B):
-    """
-    Convert red, green, blue color values on the scale of 0 to 255 to 24-bit
-    color values.  This function can take ndarrays of `R`, `G`, and `B`.
-    """
+            # Add these points to the hexagonal bins.
+            hexbin_row(X_seg, Y_seg, hex_grid)
 
-    color = np.left_shift(R, 16) + np.left_shift(G, 8) + B
-    return color
+    # Write hexagons.
+    write_hexs(fid, hex_grid, setj.scaling, setj.fmt)
 
 
-def mix_rgb_colors(R0, G0, B0, R1, G1, B1, w):
-    """
-    Mix colors `R0,G0,B0` and `R1,G1,B1` using weight `w`. A weight of 0 makes
-    the output equal to `R0,G0,B0`, and a weight of 1 makes the output equal to
-    `R1,G1,B1`.
-    """
+def hexbin_row(X, Y, hex_grid):
+    # Rectangularly bin.
+    cr_rect = (X + hex_grid.dX_rect)/hex_grid.W_rect # real rect x-axis indices
+    rr_rect = (Y + hex_grid.dY_rect)/hex_grid.H_rect # real rect y-axis indices
+    nn_in = np.asarray((cr_rect >= 0) & (cr_rect < hex_grid.C_rect) \
+            & (rr_rect >= 0) & (rr_rect < hex_grid.R_rect)).nonzero()[0]
+    cr_rect = cr_rect[nn_in] # only points within bounds
+    rr_rect = rr_rect[nn_in] # only points within bounds
+    c_rect = np.floor(cr_rect).astype(int) # integer rectangle x-axis indices
+    r_rect = np.floor(rr_rect).astype(int) # integer rectangle y-axis indices
+    u = cr_rect - c_rect # normalized x-axis position within rectangle [0, 1)
+    v = rr_rect - r_rect # normalized y-axis position within rectangle [0, 1)
+
+    # Check which points are over or under the dividing line. Here, `vs` is the
+    # normalized y-axis position of the sloped dividing line within a rectangle.
+    # The `even_odd` array marks whether a point in on a black (True) or white
+    # (False) "chess board" position in this grid of rectangular bins.
+    even_odd = (c_rect % 2 == r_rect % 2)
+    vs = even_odd*(2.0/3 - u/3) + (~even_odd)*(1.0/3 + u/3)
+    over = (v >= vs) # over the dividing line
+    under = ~over # under the dividing line
 
-    R = int(math.sqrt(w*R1**2 + (1 - w)*R0**2))
-    G = int(math.sqrt(w*G1**2 + (1 - w)*G0**2))
-    B = int(math.sqrt(w*B1**2 + (1 - w)*B0**2))
-    return R, G, B
+    # Check if this is an even or odd row.
+    even_row = (r_rect % 2 == 0)
+    odd_row = ~even_row
 
+    # Get the indices of the left and right columns.
+    left_col = np.floor(c_rect/2)
+    right_col = np.floor((c_rect + 1)/2)
 
-def mix_hex_colors(C0, C1, w):
-    """
-    Mix colors `C0` and `C1` using weight `w`. A weight of 0 makes the output
-    equal to `C0`, and a weight of 1 makes the output equal to `C1`. The colors
-    are treated as 6-character hexadecimal values.
-    """
+    # Get the hexagon column and row indices.
+    c_hex = (even_row*(under*right_col + over*left_col)
+            + odd_row*(under*left_col + over*right_col)).astype(int)
+    r_hex = (over*(r_rect + 1) + under*r_rect).astype(int)
 
-    R0, G0, B0 = hex_to_rgb(C0)
-    R1, G1, B1 = hex_to_rgb(C1)
-    R, G, B = mix_rgb_colors(R0, G0, B0, R1, G1, B1, w)
-    C = rgb_to_hex(R, G, B)
-    return C
+    # Increment the appropriate hexagon bins.
+    np.add.at(hex_grid.hexs, (r_hex, c_hex), 1)
 
 
 def three_sigmas(y, Tf=None):
     """
     Create a probability-density contour plot of `y` as a function of `t`.
 
     Parameters
@@ -1558,122 +1843,143 @@
     for k in range(K-1, -1, -1):
         E = y[:, k] - D0*EOld
         y[:, k] = N1*E + N0*EOld
         EOld = E
 
     return y
 
+# --------------------------
+# LaTeX Code Write Functions
+# --------------------------
 
 def write_open(fid, preamble=None):
     fid.write("% Preamble")
     fid.write("\n\\batchmode")
     fid.write("\n\\documentclass{standalone}")
+    fid.write("\n\\usepackage{bm}")
     fid.write("\n\\usepackage{tikz}")
-    fid.write("\n\\usepackage[pdftex, outline]{contour}")
-    fid.write("\n\\usetikzlibrary{plotmarks}")
-    fid.write("\n\\contourlength{0.8pt}")
+    fid.write("\n\\usepackage{pdfrender}")
     fid.write("\n\\newcommand{\\ul}[1] % vectors")
     fid.write("\n    {{}\\mkern1mu\\underline")
     fid.write("{\\mkern-1mu#1\\mkern-1mu}\\mkern1mu}")
-    fid.write("\n\\newcommand{\\micro}")
-    fid.write("\n    {{\\fontencoding{U}\\fontfamily{eur}")
-    fid.write("\\selectfont\\char22}}")
     fid.write("\n\\DeclareSymbolFont{euler}{U}{eur}{m}{n}")
     fid.write("\n\\DeclareMathSymbol{\\PI}{\\mathord}{euler}{25}")
     if preamble is not None:
         fid.write("\n\\errorstopmode")
         fid.write("\n%s" % preamble)
         fid.write("\n\\batchmode")
     fid.write("\n% Document contents")
     fid.write("\n\\begin{document}")
     fid.write("\n\\begin{tikzpicture}")
     fid.write("\n\\errorstopmode")
 
 
-def write_textstyle(fid, fsname):
+def write_textstyle(fid, font_size_name):
     txt = "\n% Set the style of all text."
     txt += "\n\\tikzset{every node/.style={inner sep=0pt"
-    if fsname != "normalsize":
-        txt += ", font=\\" + fsname
+    if font_size_name != "normalsize":
+        txt += ", font=\\" + font_size_name
     txt += "}}"
     fid.write(txt)
 
 
-def write_colors(fid, sets):
-    color_map = [BLUE, AZURE, CYAN, GREEN, LIME,
-            YELLOW, ORANGE, RED, MAGENTA, PURPLE]
-    J = len(sets)
+# FIXME Calculating missing colors and writing them should be separated.
+def write_color_definitions(fid, sets):
+    def hex_to_rgb(color):
+        B = np.bitwise_and(color, 0xFF)
+        RG = np.right_shift(color, 8)
+        G = np.bitwise_and(RG, 0xFF)
+        R = np.right_shift(RG, 8)
+        return R, G, B
+
+    # Get the scaling factor from set index to color map index.
+    J = len(sets);  L = len(config.colormap)
+    scale = L/max(J, L/3) if J < 5 else L/max(J, L/2)
+
     fid.write("\n% Define the plot colors.")
     for j in range(J):
+        # Pick a color using the `colormap`.
         if sets[j].color is None:
-            if J < 5:
-                R, G, B = hex_to_rgb(color_map[3*j])
-            elif J == 5:
-                R, G, B = hex_to_rgb(color_map[2*j])
-            elif J <= 10:
-                R, G, B = hex_to_rgb(color_map[j])
-            else:
-                r = (len(color_map) - 1)*(j/(J - 1.0)) # real weight
-                n = int(r) # integer weight
-                w = r - n # fractional weight
-                if n == len(color_map) - 1: # end of map
-                    C = color_map[n]
-                    R, G, B = hex_to_rgb(C)
-                else: # not at end of map
-                    C0 = color_map[n]
-                    C1 = color_map[n + 1]
-                    R0, G0, B0 = hex_to_rgb(C0)
-                    R1, G1, B1 = hex_to_rgb(C1)
-                    R, G, B = mix_rgb_colors(R0, G0, B0, R1, G1, B1, w)
-        else:
-            C = int(sets[j].color)
-            R = ((C & 0xff0000) >> 16)
-            G = ((C & 0x00ff00) >> 8)
-            B = (C & 0x0000ff)
-        fid.write(f"\n\definecolor{{C{j}}}{{RGB}}{{{R},{G},{B}}}")
+            # Get the weight and integer map index.
+            r = j*scale # real weight
+            n = int(r) # integer weight
+            w = r - n # fractional weight
+
+            if n >= len(config.colormap) - 1: # end of map
+                # Get the last color.
+                color = config.colormap[-1]
+            else: # not at end of map
+                # Get the two nearest-neighbor map colors.
+                C0, C1 = config.colormap[n:n + 2]
+                R0, G0, B0 = hex_to_rgb(C0)
+                R1, G1, B1 = hex_to_rgb(C1)
+
+                # Mix the colors in square space using the weight.
+                R = int(math.sqrt(w*R1**2 + (1 - w)*R0**2))
+                G = int(math.sqrt(w*G1**2 + (1 - w)*G0**2))
+                B = int(math.sqrt(w*B1**2 + (1 - w)*B0**2))
+
+                # Convert color back to hex value.
+                color = np.left_shift(R, 16) + np.left_shift(G, 8) + B
+        else: # Get the color.
+            color = sets[j].color
+
+        # Write color definition.
+        fid.write("\n\\definecolor{C" + str(j) + "}{HTML}{"
+                + f"{color:06x}" + "}")
+
+        # Append color to the format specifier.
+        fmt = sets[j].fmt
+        sets[j].fmt = f"C{j}" if fmt is None else fmt + f", C{j}"
 
 
 def write_reserve(fid, lay):
     # Calculate dimensions.
-    xa = lay.W_box + lay.R_margin - lay.width
-    ya = lay.H_box + lay.T_margin - lay.height
     xb = lay.W_box + lay.R_margin
     yb = lay.H_box + lay.T_margin
+    xa = xb - lay.width
+    ya = yb - lay.height
 
     # Comment.
     fid.write("\n% Reserve the full figure space.")
 
     # Draw the sets.
     if lay.invisibles:
         # Outer figure box
         fid.write(f"\n\\draw[ultra thin, red] ({xa:0.4f},{ya:0.4f}) rectangle "
                 + f"({xb:0.4f},{yb:0.4f});")
         # Margins
         xc = -lay.L_margin
         yc = -lay.B_margin
-        fid.write(f"\n\draw[ultra thin, red] ({xc:0.4f},{yc:0.4f}) rectangle "
+        fid.write(f"\n\\draw[ultra thin, red] ({xc:0.4f},{yc:0.4f}) rectangle "
                 + f"({xb:0.4f},{yb:0.4f});")
         # Legend
         yd = -lay.H_legend - lay.B_margin
         for row in range(lay.legend_rows):
             yd += lay.H_legend_row
             fid.write(f"\n\\draw[ultra thin, red] "
                     + f"({xa:0.4f},{yd:0.4f}) -- ({xb:0.4f},{yd:0.4f});")
     else:
         fid.write(f"\n\\path ({xa:0.4f},{ya:0.4f}) rectangle "
                 + f"({xb:0.4f},{yb:0.4f});")
 
 
-def write_begin_clip(fid, W_box, H_box):
-    fid.write("\n% Draw the plot contents, clipping it to the box area.")
-    fid.write("\n\\begin{scope}")
+def write_clip(fid, W_box, H_box):
     fid.write(f"\n\\clip (0,0) rectangle ({W_box:0.4f},{H_box:0.4f});")
 
 
-def write_end_clip(fid):
+def write_scope_begin(fid, opts=None):
+    fid.write("\n% Draw the plot contents, clipping it to the box area.")
+    if opts is None:
+        fid.write("\n\\begin{scope}")
+    else:
+        fid.write("\n\\begin{scope}" + f"[{opts}]")
+
+
+def write_scope_end(fid):
     fid.write("\n\\end{scope}")
 
 
 def write_comment(fid, txt):
     fid.write(f"\n% {txt}")
 
 
@@ -1711,237 +2017,137 @@
 
 def write_rounded(fid):
     fid.write("\n% Round every subsequent path until the end of the clip.")
     fid.write("\n\\tikzset{every path/.style="
             + "{line cap=round, line join=round}}")
 
 
-def draw_set(fid, j, X, Y, fmt, simp, W_box, H_box):
-    if X.ndim == 1 and Y.ndim == 1:
-        write_draw(fid, X, Y, fmt, simp, W_box, H_box)
-    elif X.ndim == 1 and Y.ndim == 2:
-        for row in range(Y.shape[0]):
-            write_draw(fid, X, Y[row, :], fmt, simp, W_box, H_box)
-    elif X.ndim == 2 and Y.ndim == 1:
-        for row in range(X.shape[0]):
-            write_draw(fid, X[row, :], Y, fmt, simp, W_box, H_box)
-    elif X.ndim == 2 and Y.ndim == 2:
-        for row in range(X.shape[0]):
-            write_draw(fid, X[row, :], Y[row, :], fmt, simp, W_box, H_box)
-    else:
-        print(f"x and y for set {j} are not 1 or 2D arrays.")
-
-
-def mark_set(fid, j, X, Y, Z, fmt, style, size, simp, W_box, H_box):
-    if X.ndim == 1 and Y.ndim == 1:
-        write_mark(fid, X, Y, Z,
-                fmt, style, size, simp, W_box, H_box)
-    elif X.ndim == 1 and Y.ndim == 2:
-        for row in range(Y.shape[0]):
-            write_mark(fid, X, Y[row, :], Z[row, :],
-                    fmt, style, size, simp, W_box, H_box)
-    elif X.ndim == 2 and Y.ndim == 1:
-        for row in range(X.shape[0]):
-            write_mark(fid, X[row, :], Y, Z[row, :],
-                    fmt, style, size, simp, W_box, H_box)
-    elif X.ndim == 2 and Y.ndim == 2:
-        for row in range(X.shape[0]):
-            write_mark(fid, X[row, :], Y[row, :], Z[row, :],
-                    fmt, style, size, simp, W_box, H_box)
-    else:
-        print(f"x and y for set {j} are not 1 or 2D arrays.")
-
-
-def fillpairs_set(fid, j, X, Y, fmt, simp, W_box, H_box):
-    if X.ndim == 1 and Y.ndim == 2:
-        for row in range(1, Y.shape[0], 2):
-            x = np.concatenate((X, X[::-1]))
-            y = np.concatenate((Y[row - 1, :], Y[row, ::-1]))
-            write_fill(fid, x, y, fmt, simp, W_box, H_box)
-        if Y.shape[0] % 2 != 0:
-            print(f"y for set {j} should have an even number of rows.")
-    elif X.ndim == 2 and Y.ndim == 1:
-        for row in range(1, X.shape[0], 2):
-            x = np.concatenate((X[row - 1, :], X[row, ::-1]))
-            y = np.concatenate((Y, Y[::-1]))
-            write_fill(fid, x, y, fmt, simp, W_box, H_box)
-        if X.shape[0] % 2 != 0:
-            print(f"x for set {j} should have an even number of rows.")
-    elif X.ndim == 2 and Y.ndim == 2:
-        for row in range(1, X.shape[0], 2):
-            x = np.concatenate((X[row - 1, :], X[row, ::-1]))
-            y = np.concatenate((Y[row - 1, :], Y[row, ::-1]))
-            write_fill(fid, x, y, fmt, simp, W_box, H_box)
-        if X.shape[0] % 2 != 0 or Y.shape[0] % 2 != 0:
-            print(f"x and y for set {j} should have an even number of rows.")
-    else:
-        print(f"x and y for set {j} should both be 1 or 2D arrays, "
-                + "and at least one must be a 2D array.")
-
-
-def hex_bin_1D(X, Y, hexs, s, DX, DY):
-    # Define the rectangular grid.
-    SQ3 = math.sqrt(3)
-    DXr = s*SQ3/2 # width of rectangles
-    DYr = 3*s/2 # height of rectangles
-    BX = math.ceil(DX/DXr) # number of rectangles horizontally
-    BY = math.ceil(DY/DYr) # number of rectangles vertically
-    dXr = (BX*DXr - DX)/2 # x-axis shift to rectangles
-    dYr = (BY*DYr - DY)/2 # y-axis shift to rectangles
-
-    # Rectangularly bin.
-    rX = (X + dXr)/DXr
-    rY = (Y + dYr)/DYr
-    bX = np.floor(rX).astype(int)
-    bY = np.floor(rY).astype(int)
-    ur = rX - bX # normalized x-axis position within rectangle [0, 1)
-    vr = rY - bY # normalized y-axis position within rectangle [0, 1)
-
-    # Filter out points outside bounds.
-    nn = np.arange(len(bX))
-    nn_horz = nn[(bX >= 0) & (bX < BX)]
-    nn_vert = nn[(bY >= 0) & (bY < BY)]
-    nn_in = np.intersect1d(nn_horz, nn_vert)
-    bX = bX[nn_in]
-    bY = bY[nn_in]
-    ur = ur[nn_in]
-    vr = vr[nn_in]
-
-    # Check if point within rectangle is over or under the dividing line.
-    even_odd = (bX % 2 == bY % 2)
-    vs = even_odd*(2.0/3 - ur/3) + (~even_odd)*(1.0/3 + ur/3)
-    over = (vr > vs)
-    under = (vr <= vs)
-
-    # Check if this is an even or odd row.
-    even_row = (bY % 2 == 0)
-    odd_row = (bY % 2 == 1)
-
-    # Get the indices of the left and right columns.
-    left_col = np.floor(bX/2)
-    right_col = np.floor((bX + 1)/2)
-
-    # Get the hexagon indices.
-    hX = (even_row*(under*right_col + over*left_col)
-            + odd_row*(under*left_col + over*right_col)).astype(int)
-    hY = (over*(bY + 1) + under*bY).astype(int)
-
-    # Increment the appropriate hexagon bins.
-    np.add.at(hexs, (hY, hX), 1)
-
-
-def hex_set(fid, j, X, Y, fmt, s, simp, DX, DY):
-    # Define the rectangular grid.
-    SQ3 = math.sqrt(3)
-    DXr = s*SQ3/2 # width of rectangles
-    DYr = 3*s/2 # height of rectangles
-    BX = math.ceil(DX/DXr) # number of rectangles horizontally
-    BY = math.ceil(DY/DYr) # number of rectangles vertically
-    dXr = (BX*DXr - DX)/2 # x-axis shift to rectangles
-    dYr = (BY*DYr - DY)/2 # y-axis shift to rectangles
-
-    # Build the hexagon grid.
-    HX = math.floor((BX + 2)/2)
-    HY = BY + 1
-    hexs = np.zeros((HY, HX))
-
-    # Bin values into hexagonal storage.
-    if X.ndim == 1 and Y.ndim == 1:
-        hex_bin_1D(X, Y, hexs, s, DX, DY)
-    elif X.ndim == 1 and Y.ndim == 2:
-        for row in range(Y.shape[0]):
-            hex_bin_1D(X, Y[row, :], hexs, s, DX, DY)
-    elif X.ndim == 2 and Y.ndim == 1:
-        for row in range(X.shape[0]):
-            hex_bin_1D(X[row, :], Y, hexs, s, DX, DY)
-    elif X.ndim == 2 and Y.ndim == 2:
-        for row in range(X.shape[0]):
-            hex_bin_1D(X[row, :], Y[row, :], hexs, s, DX, DY)
-    else:
-        print(f"x and y for set {j} are not 1 or 2D arrays.")
-
-    # Write hexagons.
-    write_hexs(fid, hexs, fmt, s, dXr, dYr)
-
-
-def write_draw(fid, X, Y, fmt, simp, W_box, H_box):
-    # Simplify the data set.
-    if simp:
-        nn = simp_best(X, Y, W_box, H_box)
-        X = X[nn]
-        Y = Y[nn]
-
-    # Write the drawing command.
+def write_draw(fid, fmt, X, Y, W_box, H_box):
+    # Start the drawing command.
     fid.write("\n\\draw")
     if fmt is not None:
-        fid.write(f"[{fmt}]")
-    fid.write(f"\n    ({X[0]:0.4f},{Y[0]:0.4f})")
-    for k in range(1, len(X)):
-        if k % 3 == 0:
-            fid.write("\n   ")
-        fid.write(f" -- ({X[k]:0.4f},{Y[k]:0.4f})")
-    fid.write(";")
+        fid.write(f"[{fmt}]\n   ")
 
+    # Run state machine.
+    path_visible = False
+    points_on_line = 0
+    for k in range(len(X)):
+        # Check if this point is in the box.
+        in_box = (X[k] >= 0) and (X[k] <= W_box) \
+                and (Y[k] >= 0) and (Y[k] <= H_box)
+
+        # Continue a path or start it depending on
+        # if the path was visible and if it is in the box.
+        if path_visible:
+            if points_on_line == 3:
+                fid.write("\n   ")
+                points_on_line = 0
+            fid.write(f" -- ({X[k]:0.4f},{Y[k]:0.4f})")
+            points_on_line += 1
+            if not in_box:
+                path_visible = False
+        elif in_box:
+            if points_on_line == 3:
+                fid.write("\n   ")
+                points_on_line = 0
+            if k == 0:
+                fid.write(f" ({X[k]:0.4f},{Y[k]:0.4f})")
+                points_on_line += 1
+            else:
+                fid.write(f" ({X[k-1]:0.4f},{Y[k-1]:0.4f})")
+                fid.write(f" -- ({X[k]:0.4f},{Y[k]:0.4f})")
+                points_on_line += 2
+            path_visible = True
 
-def write_fill(fid, X, Y, fmt, simp, W_box, H_box):
-    # Simplify the data set.
-    if simp:
-        nn = simp_best(X, Y, W_box, H_box)
-        X = X[nn];      Y = Y[nn]
-
-    # Write the drawing command.
-    fid.write("\n\\fill")
-    if fmt is not None:
-        fid.write(f"[{fmt}]")
-    fid.write(f"\n    ({X[0]:0.4f},{Y[0]:0.4f})")
-    for k in range(1, len(X)):
-        if k % 3 == 0:
-            fid.write("\n   ")
-        fid.write(f" -- ({X[k]:0.4f},{Y[k]:0.4f})")
+    # Close the drawing command.
     fid.write(";")
 
 
-def write_mark(fid, X, Y, Z, fmt, style, size, simp, W_box, H_box):
-    # Simplify the data set.
-    if simp:
-        nn = simp_best(X, Y, W_box, H_box)
-        X = X[nn];      Y = Y[nn];      Z = Z[nn]
-
+def write_mark(fid, marker, fmt, X, Y, R, W_box, H_box):
     # Build the beginning of the command.
-    if style == STYLE_CIRCLES:
+    if marker == CIRCLES:
         cmd = "\n\\draw"
-    elif style == STYLE_DOTS:
+    elif marker == DOTS:
         cmd = "\n\\fill"
     if fmt is not None:
         cmd += f"[{fmt}]"
 
     # Write the drawing commands.
-    if isinstance(Z, (np.ndarray, list, tuple)):
-        for k in range(len(X)):
-            if k % 32 == 0:
-                if k == 0:
-                    fid.write(f"{cmd}")
-                else:
-                    fid.write(f";{cmd}")
-            fid.write(f"\n     ({X[k]:0.4f},{Y[k]:0.4f})"
-                    + f" circle ({math.fabs(Z[k]):0.4f})")
-        fid.write(";")
-    else:
-        for k in range(len(X)):
-            if k % 32 == 0:
-                if k == 0:
-                    fid.write(f"{cmd}")
-                else:
-                    fid.write(f";{cmd}")
-            fid.write(f"\n     ({X[k]:0.4f},{Y[k]:0.4f})"
-                    + f" circle ({math.fabs(Z):0.4f})")
+    scalar_R = (np.ndim(R) == 0)
+    points_in_cmd = 0
+    for k in range(len(X)):
+        # Get the radius of this point.
+        r = R if scalar_R else R[k]
+
+        # Skip if this point is not in the box.
+        in_box = (X[k] + r >= 0) and (X[k] - r <= W_box) \
+                and (Y[k] + r >= 0) and (Y[k] - r <= H_box)
+        if not in_box:
+            continue
+
+        # Restart the drawing command periodically.
+        if points_in_cmd == 0:
+            fid.write(f"{cmd}")
+
+        # Write the symbol.
+        fid.write(f"\n     ({X[k]:0.4f},{Y[k]:0.4f})"
+                + f" circle ({r:0.4f})")
+        points_in_cmd += 1
+
+        if points_in_cmd == 32:
+            fid.write(";")
+            points_in_cmd = 0
+
+    # Close the last drawing command.
+    if points_in_cmd != 0:
         fid.write(";")
 
 
-def write_hexs(fid, hexs, fmt, s, dXr, dYr):
+def write_fill(fid, fmt, X, Y, W_box, H_box):
+    # Start the drawing command.
+    fid.write("\n\\fill")
+    if fmt is not None:
+        fid.write(f"[{fmt}]\n   ")
+
+    # Run state machine.
+    path_visible = False
+    points_on_line = 0
+    for k in range(len(X)):
+        # Check if this point is in the box.
+        in_box = (X[k] >= 0) and (X[k] <= W_box) \
+                and (Y[k] >= 0) and (Y[k] <= H_box)
+
+        # Continue a path or start it depending on
+        # if the path was visible and if it is in the box.
+        if path_visible:
+            if points_on_line == 3:
+                fid.write("\n   ")
+                points_on_line = 0
+            fid.write(f" -- ({X[k]:0.4f},{Y[k]:0.4f})")
+            points_on_line += 1
+            if not in_box:
+                path_visible = False
+        elif in_box:
+            if points_on_line == 3:
+                fid.write("\n   ")
+                points_on_line = 0
+            if k == 0:
+                fid.write(f" ({X[k]:0.4f},{Y[k]:0.4f})")
+                points_on_line += 1
+            else:
+                fid.write(f" ({X[k-1]:0.4f},{Y[k-1]:0.4f})")
+                fid.write(f" -- ({X[k]:0.4f},{Y[k]:0.4f})")
+                points_on_line += 2
+            path_visible = True
+
+    # Close the drawing command.
+    fid.write(";")
+
+
+def write_hexs(fid, hex_grid, scaling, fmt):
     def split_hex(U):
         U1a = U[::2, ::3].flatten()
         U1b = U[1::2, 1::3].flatten()
         U2a = U[::2, 1::3].flatten()
         U2b = U[1::2, 2::3].flatten()
         U3a = U[::2, 2::3].flatten()
         U3b = U[1::2, ::3].flatten()
@@ -1953,77 +2159,93 @@
     def sort_hex(X, Y, P):
         nn = np.argsort(P)
         P = P[nn]
         X = X[nn]
         Y = Y[nn]
         return X, Y, P
 
-    # Get the shape of the hexagon grid.
-    HY, HX = hexs.shape
-
-    # Define the vertex arrays.
-    SQ3 = math.sqrt(3)
-    VX = 2*HX + 2
-    VY = 2*HY + 2
-    vX = np.arange(VX)
-    vY = np.arange(VY//2)
-    Xv = np.round(vX*(s*SQ3/2) - s*SQ3/2 - dXr, 4)
-    Yv = np.zeros(VY)
-    Yv[::2] = np.round(vY*(3*s/2) - s - dYr, 4)
-    Yv[1::2] = np.round(vY*(3*s/2) - s/2 - dYr, 4)
-
     # FIXME Compensate for partially-visible hexagons.
-    # Normalize the hexagon counts and build matrices of indices.
-    pps = np.round(99*hexs/np.max(hexs) + 1).astype(int) # point scaling
-    hhx = np.outer(np.ones(HY), np.arange(HX)).astype(int)
-    hhy = np.outer(np.arange(HY), np.ones(HX)).astype(int)
+    # FIXME Scale each row of the data set independently.
+    # Normalize the hexagon counts and build matrices of indices. Testing was
+    # done to show that there is no higher color mixing precision than integer
+    # percentages. In other words, 100 variations is the maximum and rounding pp
+    # to integers from 0 to 100 is fine.
+    pp = hex_grid.hexs/np.max(hex_grid.hexs)
+    if scaling != 0:
+        pp = np.sqrt(scaling*(2*pp - 1) + scaling**2 + 1/4)/scaling \
+                - pp - 1/(2*scaling) + 1
+    pp = np.round(99*pp + 1).astype(int) # point scaling
+    cc = np.outer(np.ones(hex_grid.R_hex),
+            np.arange(hex_grid.C_hex)).astype(int)
+    rr = np.outer(np.arange(hex_grid.R_hex),
+            np.ones(hex_grid.C_hex)).astype(int)
 
     # Split and flatten the matrices into three sets.
-    P1, P2, P3 = split_hex(pps)
-    X1, X2, X3 = split_hex(hhx)
-    Y1, Y2, Y3 = split_hex(hhy)
+    pp1, pp2, pp3 = split_hex(pp)
+    cc1, cc2, cc3 = split_hex(cc)
+    rr1, rr2, rr3 = split_hex(rr)
 
     # Sort within each set by the scaling.
-    X1, Y1, P1 = sort_hex(X1, Y1, P1)
-    X2, Y2, P2 = sort_hex(X2, Y2, P2)
-    X3, Y3, P3 = sort_hex(X3, Y3, P3)
+    cc1, rr1, pp1 = sort_hex(cc1, rr1, pp1)
+    cc2, rr2, pp2 = sort_hex(cc2, rr2, pp2)
+    cc3, rr3, pp3 = sort_hex(cc3, rr3, pp3)
 
     # Concatenate the sets.
-    pps = np.concatenate((P1, P2, P3))
-    hhx = np.concatenate((X1, X2, X3))
-    hhy = np.concatenate((Y1, Y2, Y3))
+    pp = np.concatenate((pp1, pp2, pp3))
+    cc = np.concatenate((cc1, cc2, cc3))
+    rr = np.concatenate((rr1, rr2, rr3))
 
     # Write the hexagons.
-    ps_last = None
-    for n in range(len(pps)):
-        # Define the center of the hexagon.
-        ps = pps[n]
-        if (ps <= 1):
+    p_last = None # last percentage
+    tol = 100.0*(ULTRA_THIN/PT_PER_CM)/hex_grid.radius
+    p_smallest = 1 if not hex_grid.variable else tol
+    for n in range(len(pp)):
+        # Get this percentage.
+        p = pp[n]
+        if p <= p_smallest:
             continue
-        hx = hhx[n]
-        hy = hhy[n]
 
         # Start a new fill command.
-        if ps_last is None:
-            fid.write("\n\\fill[%s!%d]" % (fmt, int(ps)))
-            ps_last = ps
-        elif ps != ps_last:
-            fid.write(";\n\\fill[%s!%d]" % (fmt, int(ps)))
-            ps_last = ps
+        if p != p_last:
+            if p_last is not None:
+                fid.write(";")
+            if hex_grid.variable:
+                fid.write(f"\n\\fill[{fmt}]")
+                s = (1.0 - p*0.01)*hex_grid.radius/2 # short-side shrink
+                l = math.sqrt(3.0)*s # long-side shrink
+            else:
+                fid.write(f"\n\\fill[{fmt}!{p}]")
+            p_last = p
+
+        # Column of left vertex and row of bottom vertex
+        cv = 2*cc[n] + int(rr[n] % 2) # column
+        rv = 2*rr[n] # row
+
+        # Coordinates of bottom half vertices, left to right
+        Xa = hex_grid.X_vert[cv + 0];    Ya = hex_grid.Y_vert[rv + 1]
+        Xb = hex_grid.X_vert[cv + 1];    Yb = hex_grid.Y_vert[rv + 0]
+        Xc = hex_grid.X_vert[cv + 2];    Yc = hex_grid.Y_vert[rv + 1]
+        # Coordinates of top half vertices, right to left
+        Xd = hex_grid.X_vert[cv + 2];    Yd = hex_grid.Y_vert[rv + 2]
+        Xe = hex_grid.X_vert[cv + 1];    Ye = hex_grid.Y_vert[rv + 3]
+        Xf = hex_grid.X_vert[cv + 0];    Yf = hex_grid.Y_vert[rv + 2]
+        # Adjust size of hexagon in variable radius mode.
+        if hex_grid.variable:
+            Xa += l;    Ya += s;    Yb += 2*s;  Xc -= l;    Yc += s
+            Xd -= l;    Yd -= s;    Ye -= 2*s;  Xf += l;    Yf -= s
 
         # Write the hexagon vertices.
-        odd = int(hy % 2)
         fid.write("\n") # bottom half, left to right
-        fid.write("    (%.4g,%.4g)" % (Xv[2*hx + 0 + odd], Yv[2*hy + 1]))
-        fid.write(" -- (%.4g,%.4g)" % (Xv[2*hx + 1 + odd], Yv[2*hy + 0]))
-        fid.write(" -- (%.4g,%.4g)" % (Xv[2*hx + 2 + odd], Yv[2*hy + 1]))
+        fid.write("    (%.4g,%.4g)" % (Xa, Ya))
+        fid.write(" -- (%.4g,%.4g)" % (Xb, Yb))
+        fid.write(" -- (%.4g,%.4g)" % (Xc, Yc))
         fid.write("\n   ") # top half, right to left
-        fid.write(" -- (%.4g,%.4g)" % (Xv[2*hx + 2 + odd], Yv[2*hy + 2]))
-        fid.write(" -- (%.4g,%.4g)" % (Xv[2*hx + 1 + odd], Yv[2*hy + 3]))
-        fid.write(" -- (%.4g,%.4g)" % (Xv[2*hx + 0 + odd], Yv[2*hy + 2]))
+        fid.write(" -- (%.4g,%.4g)" % (Xd, Yd))
+        fid.write(" -- (%.4g,%.4g)" % (Xe, Ye))
+        fid.write(" -- (%.4g,%.4g)" % (Xf, Yf))
 
     # Write the closing and close the file.
     fid.write(";")
 
 
 def write_line(fid, xa, ya, xb, yb, fmt=None):
     # Draw the line.
@@ -2031,15 +2253,20 @@
     if fmt is not None:
         fid.write(f"[{fmt}]")
     fid.write(f" ({xa:0.4f},{ya:0.4f}) -- ({xb:0.4f},{yb:0.4f});")
 
 
 def write_text(fid, x, y, txt, fmt=None):
     if fmt is None:
-        fid.write(f"\n\\node at ({x:0.4f},{y:0.4f})\n    {{{txt}}};")
+        fid.write(f"\n\\node at ({x:0.4f},{y:0.4f}) {{{txt}}};")
     else:
-        fid.write(f"\n\\node[{fmt}] at ({x:0.4f},{y:0.4f})\n    {{{txt}}};")
+        fid.write(f"\n\\node[{fmt}] at ({x:0.4f},{y:0.4f}) {{{txt}}};")
+
+
+def write_outline_style(fid):
+    fid.write("\n\\pdfrender{TextRenderingMode=1, LineWidth=1.2pt,\n"
+            + "        LineCapStyle=1, LineJoinStyle=1}\\color{white}")
 
 
 def write_close(fid):
     fid.write("\n\\end{tikzpicture}")
     fid.write("\n\\end{document}")
```

