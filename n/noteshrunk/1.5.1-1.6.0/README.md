# Comparing `tmp/noteshrunk-1.5.1.tar.gz` & `tmp/noteshrunk-1.6.0.tar.gz`

## Comparing `noteshrunk-1.5.1.tar` & `noteshrunk-1.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 noteshrunk-1.5.1/CHANGELOG.md
--rwxr-xr-x   0        0        0    31003 2020-02-02 00:00:00.000000 noteshrunk-1.5.1/src/noteshrunk.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 noteshrunk-1.5.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 noteshrunk-1.5.1/LICENSE
--rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 noteshrunk-1.5.1/README.md
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 noteshrunk-1.5.1/pyproject.toml
--rw-r--r--   0        0        0    49283 2020-02-02 00:00:00.000000 noteshrunk-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 noteshrunk-1.6.0/CHANGELOG.md
+-rwxr-xr-x   0        0        0    32340 2020-02-02 00:00:00.000000 noteshrunk-1.6.0/src/noteshrunk.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 noteshrunk-1.6.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 noteshrunk-1.6.0/LICENSE
+-rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 noteshrunk-1.6.0/README.md
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 noteshrunk-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0    50112 2020-02-02 00:00:00.000000 noteshrunk-1.6.0/PKG-INFO
```

### Comparing `noteshrunk-1.5.1/CHANGELOG.md` & `noteshrunk-1.6.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.6] - 2024-04-23
+
+### Added
+
+- `--skip_empty`, `--threshold_empty`
+
 ## [1.5] - 2024-04-21
 
 ### Fixed
 
 - Processing of grayscale and black-and-white images.
 
 ### Changed
```

### Comparing `noteshrunk-1.5.1/src/noteshrunk.py` & `noteshrunk-1.6.0/src/noteshrunk.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
-VERSION = '1.5.1'
+VERSION = '1.6.0'
 
 import argparse
 from concurrent.futures import ThreadPoolExecutor
 import logging
 import os
 from pathlib import Path
 import random
@@ -87,14 +87,26 @@
     parser.add_argument(
         "-p",
         "--percentage",
         type=float,
         default=100,
         help="Percentage of pixels to sample from each image.")
     parser.add_argument(
+        '-e',
+        '--skip_empty',
+        action='store_true',
+        default=False,
+        help='Autoremove blank pages. Pages with a coverage (after removing about 6 % at the margin) below <-te> will be removed.')
+    parser.add_argument(
+        '-te',
+        '--threshold_empty',
+        type=lambda x: np.clip(x, a_min=0, a_max=None),
+        default=2,
+        help='Coverage in parts per thousand / permille below which a page should be discarded.')
+    parser.add_argument(
         "-j",
         "--jobs",
         type=int,
         default=os.cpu_count(),
         help="Number of processes to use (default: number of CPU cores)")
     parser.add_argument(
         '-y',
@@ -550,14 +562,24 @@
     else:
         foreground_mask = get_foreground_mask(
             image,
             background_color=color_palette[0],
             threshold_saturation=args.threshold_saturation,
             threshold_value=args.threshold_value)
 
+    if args.skip_empty:
+        Y, X = shape
+        # subtract a small safety margin
+        delta = int(round(X * .06, 0))
+        coverage = 1000 * foreground_mask.reshape(shape)[delta:Y-delta, delta:X-delta].mean()
+
+        if coverage <= args.threshold_empty:
+            logging.info('Removing page {} with coverage of {} (<= {}) ‰.'.format(idx, round(coverage, 1), args.threshold_empty))
+            return None
+
     # morphological opening of the binary foreground mask to remove e.g. dust speckles
     if args.denoise_opening:
         logging.info('Page {}: Applying opening ...'.format(idx))
         # disk(<1) results in id-operation or zero-matrix and is hence useless
         kernel = disk(
             args.opening_strength) if args.opening_strength >= 1 else square(2)
         foreground_mask = binary_opening(
@@ -785,36 +807,40 @@
     2. Creates a color palette for the image or uses a global palette if provided.
     3. Applies the color palette to the image, potentially with saturation maximization and denoising.
     4. Saves the processed image as a PDF file with the given output filename.
 
     Args:
         file (pathlib.Path): The path to the input image file.
         output_filename (pathlib.Path): The path to the output PDF file.
-        idx (int): The index of the image in the list of files being processed. Just used for the -v flag.
+        idx (int): The index of the image in the list of files being processed.
         args (argparse.Namespace): The command line arguments.
         global_palette (tuple, optional): A tuple containing the color palette and the fitted KMeans model,
                                           if using a global palette. Defaults to None.
 
     Returns:
-        None
+        tuple (idx, bool): idx: Same as input, bool: True: Success, False: Page is to be removed.
     """
     image = io.imread(file)
 
     processed_images = []
 
     logging.info('Processing image {}'.format(idx))
 
     if args.local_palette:
         color_palette, kmeans_model = create_palette(image, args, idx + 1)
     else:
         color_palette, kmeans_model = global_palette
 
     image = apply_color_palette(image, color_palette, kmeans_model, args, idx + 1)
 
-    save_as_pdf(image, output_filename, args, idx + 1)
+    if image is None:
+        return (idx, False)
+    else:
+        save_as_pdf(image, output_filename, args, idx + 1)
+        return (idx, True)
 
 
 def check_file_existence(files):
     """
     Checks if a file / a list of files exist and raises an error if any are missing.
 
     Args:
@@ -877,14 +903,15 @@
 
         if not args.local_palette:
             color_palette, kmeans_model = create_palette(file_paths, args, use_global_palette=True)
 
         with ThreadPoolExecutor(max_workers=args.jobs) as executor:
 
             threads = []
+            remove = []
             for idx, file in enumerate(file_paths):
 
                 output_filename = args.output.parent / temp_dir / Path(file.name).with_suffix('.pdf')
 
                 # E.g. the same input file multiple times
                 if output_filename in intermediate_pdf_paths or output_filename.exists():
                     output_filename = rename_with_random_string(output_filename)
@@ -893,15 +920,23 @@
                                  global_palette=(color_palette, kmeans_model) if not args.local_palette else None))
 
                 intermediate_pdf_paths.append(output_filename)
 
             executor.shutdown(wait=True)
             try:
                 for f in threads:
-                    f.result()  # This will raise a ValueError in case the thread crashed
+                    idx, result = f.result()  # This will raise a ValueError in case the thread crashed
+
+                    # Page is to be removed
+                    if result is False:
+                        remove.append(idx)
+
+                for idx in sorted(remove, reverse=True):
+                    intermediate_pdf_paths.pop(idx)
+
             except ValueError as e:
                 logging.critical(f"Caught an error: {e}")
                 sys.exit(1)
 
 
         if args.keep_intermediate:
             logging.info('Skipping the deletion of intermediate PDFs (folder {}).'.format(temp_dir))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `noteshrunk-1.5.1/.gitignore` & `noteshrunk-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.5.1/LICENSE` & `noteshrunk-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.5.1/README.md` & `noteshrunk-1.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 This is a complete and improved rewrite of [mzucker's](https://github.com/mzucker/noteshrink) noteshrink.
 
 ## Features
 
 * **Color Quantization:** Reduces the number of colors in the document using KMeans clustering, leading to smaller file sizes and higher contrast.
 * **Background Detection and Removal:** Identifies and removes the background color (replace with white), enhancing visual clarity.
+* **Autoremove empty pages**: Identifies and removes blank pages.
 * **Customizable Palette:** Allows you to specify the number of colors in the output palette, maximize saturation and choose between a global palette for all pages or individual palettes for each page.
 * **Denoising Options:** Provides [median filtering](https://en.wikipedia.org/wiki/Median_filter), [morphological opening](https://en.wikipedia.org/wiki/Opening_(morphology)) and [unsharp masking](https://en.wikipedia.org/wiki/Unsharp_masking) to reduce noise and improve image quality.
 * **Parallel processing:** Multi-threading for faster processing of multiple images.
 * **Low memory profile**: Trys to keep memory usage as small as possible. This is done by:
   * Each page is converted separately
   * The intermediate files are stored in the current working directory (so that you can choose between disk and RAM [e.g. `/tmp`])
   * The library functions and programs used are specifically chosen to have the smallest overhead
@@ -62,14 +63,29 @@
     <td><img src="https://github.com/suuuehgi/noteshrunk/blob/main/examples/example_2-unsharp.jpg?raw=True" alt="Unsharp Masking" width="970" height="217"/></td>
   </tr>
   <tr>
     <td><code>noteshrunk -w --unsharp_mask </code></td>
   </tr>
 </table>
 
+### Empty Pages
+
+
+<table>
+  <tr>
+    <td width="50%" valign="bottom">
+      This page has a coverage of about 0.1 ‰ within the blue rectangle and will be removed, if <code>-&#8288;-&#8288;skip_empty</code> is used.</br>
+      This is useful for duplex scanning.</br>
+      The margin width is 6% of the page width.
+    </td>
+    <td width="50%"><img src="https://github.com/suuuehgi/noteshrunk/blob/main/examples/empty.jpg?raw=True" alt="Processed Image" width="400" height="570"/></td>
+  </tr>
+</table>
+
+
 ### Advanced Example
 
 <table>
   <tr>
     <td width="50%"><img src="https://github.com/suuuehgi/noteshrunk/blob/main/examples/example_3-orig.jpg?raw=True" alt="Original Image" width="400" height="486"/></td>
     <td width="50%"><img src="https://github.com/suuuehgi/noteshrunk/blob/main/examples/example_3-advanced.jpg?raw=True" alt="Processed Image" width="400" height="486"/></td>
   </tr>
@@ -126,15 +142,15 @@
 pipx install noteshrunk
 ```
 
 ## Usage
 
 ```
 noteshrunk [-h] [-o OUTPUT] [-w] [-s] [-n N_COLORS] [-d DPI] [-q [1-100]] [-l]
-           [-p PERCENTAGE] [-j JOBS] [-y]
+           [-p PERCENTAGE] [-e] [-te THRESHOLD_EMPTY] [-j JOBS] [-y]
            [-ts THRESHOLD_SATURATION] [-tv THRESHOLD_VALUE]
            [--denoise_median] [--denoise_opening] [--unsharp_mask]
            [-ms MEDIAN_STRENGTH] [-cs CLOSING_STRENGTH] [-ua UNSHARP_AMOUNT] [-ur UNSHARP_RADIUS]
            [-k] [-v] [--version] files [files ...]
 ```
 
 ### Arguments
@@ -144,14 +160,16 @@
 * `-w`, `--white_background`: Use white background instead of dominant color.
 * `-s`, `--saturate`: Maximize saturation in the output image.
 * `-n`, `--n_colors`: Number of colors in the palette (default: 8).
 * `-d`, `--dpi`: DPI value of the input images (default: 300).
 * `-q`, `--quality`: JPEG quality of the images embedded in the PDF (1-100, default: 75).
 * `-l`, `--local_palette`: Create an individual color palette for each image (by sampling a -p percentage of the pixels of that image) instead of a global palette (by sampling a -p percentage of the pixels of each input image).
 * `-p`, `--percentage`: Percentage of pixels to sample from each input image for color palette creation (default: 10).
+* `-e`, `--skip_empty`: Pages with a coverage (after removing about 6 % at the margin) below `-te` will be removed.
+* `-te`, `--threshold_empty`: Coverage in parts per thousand / permille below which a page should be discarded.
 * `-j`, `--jobs`: Number of threads to use for multi-threading (default: number of CPU cores).
 * `-y`, `--overwrite`: Overwrite existing files without asking.
 * `-ts`, `--threshold_saturation`: HSV saturation threshold (in percent) used for background detection (default: 15).
 * `-tv`, `--threshold_value`: HSV value threshold (in percent) used for background detection (default: 25).
 * `--denoise_median`: Apply median denoising on the output image with strength `-ms`.
 * `-ms`, `--median_strength`: Strength of median filtering (default: 3).
 * `--denoise_opening`: Apply morphological opening on the background mask with strength `-os`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -10,19 +10,20 @@
 > color) to the color space of the image with the largest color space. For
 saving black-and-white images, I recommend having libtiff installed, otherwise
 it will fall back to using embedded jpeg. This is a complete and improved
 rewrite of [mzucker's](https://github.com/mzucker/noteshrink) noteshrink. ##
 Features * **Color Quantization:** Reduces the number of colors in the document
 using KMeans clustering, leading to smaller file sizes and higher contrast. *
 **Background Detection and Removal:** Identifies and removes the background
-color (replace with white), enhancing visual clarity. * **Customizable Palette:
-** Allows you to specify the number of colors in the output palette, maximize
-saturation and choose between a global palette for all pages or individual
-palettes for each page. * **Denoising Options:** Provides [median filtering]
-(https://en.wikipedia.org/wiki/Median_filter), [morphological opening](https://
+color (replace with white), enhancing visual clarity. * **Autoremove empty
+pages**: Identifies and removes blank pages. * **Customizable Palette:** Allows
+you to specify the number of colors in the output palette, maximize saturation
+and choose between a global palette for all pages or individual palettes for
+each page. * **Denoising Options:** Provides [median filtering](https://
+en.wikipedia.org/wiki/Median_filter), [morphological opening](https://
 en.wikipedia.org/wiki/Opening_(morphology)) and [unsharp masking](https://
 en.wikipedia.org/wiki/Unsharp_masking) to reduce noise and improve image
 quality. * **Parallel processing:** Multi-threading for faster processing of
 multiple images. * **Low memory profile**: Trys to keep memory usage as small
 as possible. This is done by: * Each page is converted separately * The
 intermediate files are stored in the current working directory (so that you can
 choose between disk and RAM [e.g. `/tmp`]) * The library functions and programs
@@ -36,14 +37,19 @@
 swallows fine structures, but unsharp masking helps preserve them.
 [Original Image]
 Original Image (own)
 [Morphological Opening]
 noteshrunk -w --denoise_opening -os .9
 [Unsharp Masking]
 noteshrunk -w --unsharp_mask
+### Empty Pages
+This page has a coverage of about 0.1 â° within the blue
+rectangle and will be removed, if -⁠-⁠skip_empty is used.     [Processed Image]
+This is useful for duplex scanning. The margin width is 6% of
+the page width.
 ### Advanced Example
 [Original Image] [Processed Image]
 Original Image   noteshrunk -w -s -tv 30 --denoise_opening -os 1.6 -n 6 -p 100
                  example_3-orig.jpg
 Image Source: https://github.com/mzucker/noteshrink/blob/master/https://
 github.com/suuuehgi/noteshrunk/blob/main/examples/notesA1.jpg ### Further
 Examples 1. Compress a single image with default settings: ```bash noteshrunk
@@ -52,43 +58,45 @@
 images using a local color palette and keep intermediate files while disabling
 multi-threading: ```bash noteshrunk -l -j 1 -k *.jpg ``` ## Requirements ###
 Python Packages - argcomplete - NumPy - Pillow (PIL Fork) - Python 3 - scikit-
 image - scikit-learn - SciPy ### Other - Ghostscript (executable `gs` in PATH -
 for PDF merging) ### Optional Dependencies - `libtiff` for much smaller file
 sizes on black-and-white images. ## Installation ```bash pipx install
 noteshrunk ``` ## Usage ``` noteshrunk [-h] [-o OUTPUT] [-w] [-s] [-n N_COLORS]
-[-d DPI] [-q [1-100]] [-l] [-p PERCENTAGE] [-j JOBS] [-y] [-ts
-THRESHOLD_SATURATION] [-tv THRESHOLD_VALUE] [--denoise_median] [--
+[-d DPI] [-q [1-100]] [-l] [-p PERCENTAGE] [-e] [-te THRESHOLD_EMPTY] [-j JOBS]
+[-y] [-ts THRESHOLD_SATURATION] [-tv THRESHOLD_VALUE] [--denoise_median] [--
 denoise_opening] [--unsharp_mask] [-ms MEDIAN_STRENGTH] [-cs CLOSING_STRENGTH]
 [-ua UNSHARP_AMOUNT] [-ur UNSHARP_RADIUS] [-k] [-v] [--version] files [files
 ...] ``` ### Arguments * `files`: A list of paths to the input image files. *
 `-o`, `--output`: Path to the output PDF file (default: `output.pdf`). * `-w`,
 `--white_background`: Use white background instead of dominant color. * `-s`,
 `--saturate`: Maximize saturation in the output image. * `-n`, `--n_colors`:
 Number of colors in the palette (default: 8). * `-d`, `--dpi`: DPI value of the
 input images (default: 300). * `-q`, `--quality`: JPEG quality of the images
 embedded in the PDF (1-100, default: 75). * `-l`, `--local_palette`: Create an
 individual color palette for each image (by sampling a -p percentage of the
 pixels of that image) instead of a global palette (by sampling a -p percentage
 of the pixels of each input image). * `-p`, `--percentage`: Percentage of
 pixels to sample from each input image for color palette creation (default:
-10). * `-j`, `--jobs`: Number of threads to use for multi-threading (default:
-number of CPU cores). * `-y`, `--overwrite`: Overwrite existing files without
-asking. * `-ts`, `--threshold_saturation`: HSV saturation threshold (in
-percent) used for background detection (default: 15). * `-tv`, `--
-threshold_value`: HSV value threshold (in percent) used for background
-detection (default: 25). * `--denoise_median`: Apply median denoising on the
-output image with strength `-ms`. * `-ms`, `--median_strength`: Strength of
-median filtering (default: 3). * `--denoise_opening`: Apply morphological
-opening on the background mask with strength `-os`. * `-os`, `--
-opening_strength`: Strength of opening filtering / radius of the structuring
-element (disk, default: 3). * `--unsharp_mask`: Apply unsharp masking on the
-final image with radius `-ur` and amount `-ua`. * `-ur`, `-ua`: Radius and
-Amount used for unsharp masking. * `-k`, `--keep_intermediate`: Keep the
-intermediate single-page PDFs. * `-v`, `--verbose`: Verbose output. * `--
-version`: Show program version and exit. ## Contributing Contributions are
-welcome! Please feel free to submit issues or pull requests on the GitHub
-repository. ## Acknowledgements This project utilizes open-source software from
-the Python community. Special thanks to the developers and maintainers of the
-required libraries as well as [mzucker's](https://github.com/mzucker/
-noteshrink) initial program. ## License This project is licensed under the MIT
-License. See the `LICENSE` file for details.
+10). * `-e`, `--skip_empty`: Pages with a coverage (after removing about 6 % at
+the margin) below `-te` will be removed. * `-te`, `--threshold_empty`: Coverage
+in parts per thousand / permille below which a page should be discarded. * `-
+j`, `--jobs`: Number of threads to use for multi-threading (default: number of
+CPU cores). * `-y`, `--overwrite`: Overwrite existing files without asking. *
+`-ts`, `--threshold_saturation`: HSV saturation threshold (in percent) used for
+background detection (default: 15). * `-tv`, `--threshold_value`: HSV value
+threshold (in percent) used for background detection (default: 25). * `--
+denoise_median`: Apply median denoising on the output image with strength `-
+ms`. * `-ms`, `--median_strength`: Strength of median filtering (default: 3). *
+`--denoise_opening`: Apply morphological opening on the background mask with
+strength `-os`. * `-os`, `--opening_strength`: Strength of opening filtering /
+radius of the structuring element (disk, default: 3). * `--unsharp_mask`: Apply
+unsharp masking on the final image with radius `-ur` and amount `-ua`. * `-ur`,
+`-ua`: Radius and Amount used for unsharp masking. * `-k`, `--
+keep_intermediate`: Keep the intermediate single-page PDFs. * `-v`, `--
+verbose`: Verbose output. * `--version`: Show program version and exit. ##
+Contributing Contributions are welcome! Please feel free to submit issues or
+pull requests on the GitHub repository. ## Acknowledgements This project
+utilizes open-source software from the Python community. Special thanks to the
+developers and maintainers of the required libraries as well as [mzucker's]
+(https://github.com/mzucker/noteshrink) initial program. ## License This
+project is licensed under the MIT License. See the `LICENSE` file for details.
```

### Comparing `noteshrunk-1.5.1/pyproject.toml` & `noteshrunk-1.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "noteshrunk"
-version = "1.5.1"
+version = "1.6.0"
 description = "Document Color Palette Compression"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "suuuehgi"}
 ]
```

### Comparing `noteshrunk-1.5.1/PKG-INFO` & `noteshrunk-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: noteshrunk
-Version: 1.5.1
+Version: 1.6.0
 Summary: Document Color Palette Compression
 Project-URL: Homepage, https://github.com/suuuehgi/noteshrunk
 Project-URL: Issues, https://github.com/suuuehgi/noteshrunk/issues
 Author: suuuehgi
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -705,14 +705,15 @@
 
 This is a complete and improved rewrite of [mzucker's](https://github.com/mzucker/noteshrink) noteshrink.
 
 ## Features
 
 * **Color Quantization:** Reduces the number of colors in the document using KMeans clustering, leading to smaller file sizes and higher contrast.
 * **Background Detection and Removal:** Identifies and removes the background color (replace with white), enhancing visual clarity.
+* **Autoremove empty pages**: Identifies and removes blank pages.
 * **Customizable Palette:** Allows you to specify the number of colors in the output palette, maximize saturation and choose between a global palette for all pages or individual palettes for each page.
 * **Denoising Options:** Provides [median filtering](https://en.wikipedia.org/wiki/Median_filter), [morphological opening](https://en.wikipedia.org/wiki/Opening_(morphology)) and [unsharp masking](https://en.wikipedia.org/wiki/Unsharp_masking) to reduce noise and improve image quality.
 * **Parallel processing:** Multi-threading for faster processing of multiple images.
 * **Low memory profile**: Trys to keep memory usage as small as possible. This is done by:
   * Each page is converted separately
   * The intermediate files are stored in the current working directory (so that you can choose between disk and RAM [e.g. `/tmp`])
   * The library functions and programs used are specifically chosen to have the smallest overhead
@@ -756,14 +757,29 @@
     <td><img src="https://github.com/suuuehgi/noteshrunk/blob/main/examples/example_2-unsharp.jpg?raw=True" alt="Unsharp Masking" width="970" height="217"/></td>
   </tr>
   <tr>
     <td><code>noteshrunk -w --unsharp_mask </code></td>
   </tr>
 </table>
 
+### Empty Pages
+
+
+<table>
+  <tr>
+    <td width="50%" valign="bottom">
+      This page has a coverage of about 0.1 ‰ within the blue rectangle and will be removed, if <code>-&#8288;-&#8288;skip_empty</code> is used.</br>
+      This is useful for duplex scanning.</br>
+      The margin width is 6% of the page width.
+    </td>
+    <td width="50%"><img src="https://github.com/suuuehgi/noteshrunk/blob/main/examples/empty.jpg?raw=True" alt="Processed Image" width="400" height="570"/></td>
+  </tr>
+</table>
+
+
 ### Advanced Example
 
 <table>
   <tr>
     <td width="50%"><img src="https://github.com/suuuehgi/noteshrunk/blob/main/examples/example_3-orig.jpg?raw=True" alt="Original Image" width="400" height="486"/></td>
     <td width="50%"><img src="https://github.com/suuuehgi/noteshrunk/blob/main/examples/example_3-advanced.jpg?raw=True" alt="Processed Image" width="400" height="486"/></td>
   </tr>
@@ -820,15 +836,15 @@
 pipx install noteshrunk
 ```
 
 ## Usage
 
 ```
 noteshrunk [-h] [-o OUTPUT] [-w] [-s] [-n N_COLORS] [-d DPI] [-q [1-100]] [-l]
-           [-p PERCENTAGE] [-j JOBS] [-y]
+           [-p PERCENTAGE] [-e] [-te THRESHOLD_EMPTY] [-j JOBS] [-y]
            [-ts THRESHOLD_SATURATION] [-tv THRESHOLD_VALUE]
            [--denoise_median] [--denoise_opening] [--unsharp_mask]
            [-ms MEDIAN_STRENGTH] [-cs CLOSING_STRENGTH] [-ua UNSHARP_AMOUNT] [-ur UNSHARP_RADIUS]
            [-k] [-v] [--version] files [files ...]
 ```
 
 ### Arguments
@@ -838,14 +854,16 @@
 * `-w`, `--white_background`: Use white background instead of dominant color.
 * `-s`, `--saturate`: Maximize saturation in the output image.
 * `-n`, `--n_colors`: Number of colors in the palette (default: 8).
 * `-d`, `--dpi`: DPI value of the input images (default: 300).
 * `-q`, `--quality`: JPEG quality of the images embedded in the PDF (1-100, default: 75).
 * `-l`, `--local_palette`: Create an individual color palette for each image (by sampling a -p percentage of the pixels of that image) instead of a global palette (by sampling a -p percentage of the pixels of each input image).
 * `-p`, `--percentage`: Percentage of pixels to sample from each input image for color palette creation (default: 10).
+* `-e`, `--skip_empty`: Pages with a coverage (after removing about 6 % at the margin) below `-te` will be removed.
+* `-te`, `--threshold_empty`: Coverage in parts per thousand / permille below which a page should be discarded.
 * `-j`, `--jobs`: Number of threads to use for multi-threading (default: number of CPU cores).
 * `-y`, `--overwrite`: Overwrite existing files without asking.
 * `-ts`, `--threshold_saturation`: HSV saturation threshold (in percent) used for background detection (default: 15).
 * `-tv`, `--threshold_value`: HSV value threshold (in percent) used for background detection (default: 25).
 * `--denoise_median`: Apply median denoising on the output image with strength `-ms`.
 * `-ms`, `--median_strength`: Strength of median filtering (default: 3).
 * `--denoise_opening`: Apply morphological opening on the background mask with strength `-os`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

