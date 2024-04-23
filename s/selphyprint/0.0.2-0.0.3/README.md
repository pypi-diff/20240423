# Comparing `tmp/selphyprint-0.0.2.tar.gz` & `tmp/selphyprint-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selphyprint-0.0.2.tar", last modified: Fri Apr 19 07:34:34 2024, max compression
+gzip compressed data, was "selphyprint-0.0.3.tar", last modified: Tue Apr 23 08:38:59 2024, max compression
```

## Comparing `selphyprint-0.0.2.tar` & `selphyprint-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:34:34.088353 selphyprint-0.0.2/
--rw-rw-rw-   0        0        0     1094 2024-04-19 05:54:19.000000 selphyprint-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1650 2024-04-19 07:34:34.088353 selphyprint-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-04-19 07:33:17.000000 selphyprint-0.0.2/README.md
--rw-rw-rw-   0        0        0      823 2024-04-19 07:33:42.000000 selphyprint-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-19 07:34:34.057103 selphyprint-0.0.2/selphyprint/
--rw-rw-rw-   0        0        0        0 2024-04-19 01:18:35.000000 selphyprint-0.0.2/selphyprint/__init__.py
--rw-rw-rw-   0        0        0     3005 2024-04-19 06:00:37.000000 selphyprint-0.0.2/selphyprint/main.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:34:34.072729 selphyprint-0.0.2/selphyprint.egg-info/
--rw-rw-rw-   0        0        0     1650 2024-04-19 07:34:34.000000 selphyprint-0.0.2/selphyprint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-04-19 07:34:34.000000 selphyprint-0.0.2/selphyprint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:34:34.000000 selphyprint-0.0.2/selphyprint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-19 07:34:34.000000 selphyprint-0.0.2/selphyprint.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-04-19 07:34:34.000000 selphyprint-0.0.2/selphyprint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-19 07:34:34.000000 selphyprint-0.0.2/selphyprint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 07:34:34.088353 selphyprint-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 08:38:59.535312 selphyprint-0.0.3/
+-rw-rw-rw-   0        0        0     1094 2024-04-19 05:54:19.000000 selphyprint-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1650 2024-04-23 08:38:59.532167 selphyprint-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-04-19 07:33:17.000000 selphyprint-0.0.3/README.md
+-rw-rw-rw-   0        0        0      823 2024-04-23 05:08:36.000000 selphyprint-0.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-23 08:38:59.479322 selphyprint-0.0.3/selphyprint/
+-rw-rw-rw-   0        0        0        0 2024-04-19 01:18:35.000000 selphyprint-0.0.3/selphyprint/__init__.py
+-rw-rw-rw-   0        0        0     3152 2024-04-23 08:35:46.000000 selphyprint-0.0.3/selphyprint/main.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:38:59.528963 selphyprint-0.0.3/selphyprint.egg-info/
+-rw-rw-rw-   0        0        0     1650 2024-04-23 08:38:59.000000 selphyprint-0.0.3/selphyprint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-04-23 08:38:59.000000 selphyprint-0.0.3/selphyprint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 08:38:59.000000 selphyprint-0.0.3/selphyprint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-23 08:38:59.000000 selphyprint-0.0.3/selphyprint.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-23 08:38:59.000000 selphyprint-0.0.3/selphyprint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-23 08:38:59.000000 selphyprint-0.0.3/selphyprint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 08:38:59.535839 selphyprint-0.0.3/setup.cfg
```

### Comparing `selphyprint-0.0.2/LICENSE` & `selphyprint-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `selphyprint-0.0.2/PKG-INFO` & `selphyprint-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selphyprint
-Version: 0.0.2
+Version: 0.0.3
 Summary: Prepare an image for printing on Canon Selphy printers without cropping
 Author-email: Roman <roman@kosobrodov.net>
 Project-URL: Homepage, https://github.com/RomanKosobrodov/selphy-print
 Project-URL: Bug Tracker, https://github.com/RomanKosobrodov/selphy-print
 Keywords: Canon Selphy crop bleeding
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `selphyprint-0.0.2/README.md` & `selphyprint-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `selphyprint-0.0.2/pyproject.toml` & `selphyprint-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "selphyprint"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Roman", email="roman@kosobrodov.net" },
 ]
 description = "Prepare an image for printing on Canon Selphy printers without cropping"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `selphyprint-0.0.2/selphyprint/main.py` & `selphyprint-0.0.3/selphyprint/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,47 +7,49 @@
 INCH = 25.4
 DPI = 300
 
 SPACING = 1
 STEPS = 10
 
 LEFT = 7 * SPACING
-RIGHT = 6 * SPACING
+RIGHT = 7 * SPACING
 TOP = 4 * SPACING
 BOTTOM = 4 * SPACING
 
 WIDTH_PX = int(WIDTH / INCH * DPI)
 HEIGHT_PX = int(HEIGHT / INCH * DPI)
 
+MAX_BORDER = 30
+
 X0 = int(LEFT / INCH * DPI)
 X1 = int(RIGHT / INCH * DPI)
 Y0 = int(TOP / INCH * DPI)
 Y1 = int(BOTTOM / INCH * DPI)
 W = WIDTH_PX - X1 - X0
 H = HEIGHT_PX - Y1 - Y0
 
 
 def process_image(input_filename, border_pixels, output_filename):
     background = Image.new(mode="RGB", size=(WIDTH_PX, HEIGHT_PX), color=(255, 255, 255))
     try:
         with Image.open(input_filename, "r") as im:
             if im.height > im.width:
                 im = im.rotate(angle=90)
-            scale_x = W / im.width
-            scale_y = H / im.height
+            scale_x = (W - 2 * border_pixels) / im.width
+            scale_y = (H - 2 * border_pixels) / im.height
             scale = min(scale_x, scale_y)
-            w = int(scale * im.width - border_pixels)
-            h = int(scale * im.height - border_pixels)
-            im = im.resize(size=(w, h), resample=Image.Resampling.NEAREST)
+            w = int(scale * im.width)
+            h = int(scale * im.height)
             offset_x = int((WIDTH_PX - w) / 2)
             offset_y = int((HEIGHT_PX - h) / 2)
+            im = im.resize(size=(w, h), resample=Image.Resampling.NEAREST)
             background.paste(im, box=(offset_x, offset_y))
             background.save(output_filename, dpi=(DPI, DPI))
     except UnidentifiedImageError:
-        print(f"Unsupported image file \"{args.input}\"")
+        print(f"Unsupported image file \"{input_filename}\"")
 
 
 def main():
     parser = argparse.ArgumentParser(description="Adjust image to print on Canon Selphy without cropping")
     parser.add_argument("--input", "-i",
                         help="Input image or directory with multiple images",
                         type=str,
@@ -60,22 +62,26 @@
     parser.add_argument("--output", "-o",
                         help="Output image or directory",
                         type=str,
                         required=True)
     args = parser.parse_args()
 
     if not os.path.exists(args.input):
-        print(f"Input path \"{args.input}\" does not exist")
+        print(f"Input path \"{args.input}\" does not exist.")
         exit(1)
 
     output_parent = os.path.dirname(args.output)
     if not os.path.isdir(output_parent):
-        print(f"Parent directory \"{output_parent}\" must exist")
+        print(f"Parent directory \"{output_parent}\" must exist.")
         exit(2)
 
+    if args.border > MAX_BORDER:
+        print(f"Border cannot exceed {MAX_BORDER} mm.")
+        exit(3)
+
     border_px = int(args.border / INCH * DPI)
 
     if os.path.isfile(args.input):
         process_image(args.input, border_px, args.output)
     else:
         root, subdirectory, files = next(os.walk(args.input))
         for filename in files:
```

### Comparing `selphyprint-0.0.2/selphyprint.egg-info/PKG-INFO` & `selphyprint-0.0.3/selphyprint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selphyprint
-Version: 0.0.2
+Version: 0.0.3
 Summary: Prepare an image for printing on Canon Selphy printers without cropping
 Author-email: Roman <roman@kosobrodov.net>
 Project-URL: Homepage, https://github.com/RomanKosobrodov/selphy-print
 Project-URL: Bug Tracker, https://github.com/RomanKosobrodov/selphy-print
 Keywords: Canon Selphy crop bleeding
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

