# Comparing `tmp/docprompt-0.2.8.tar.gz` & `tmp/docprompt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docprompt-0.2.8.tar", max compression
+gzip compressed data, was "docprompt-0.3.0.tar", max compression
```

## Comparing `docprompt-0.2.8.tar` & `docprompt-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.2.8/LICENSE
--rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.2.8/README.md
--rw-r--r--   0        0        0      674 2024-04-14 18:41:33.996277 docprompt-0.2.8/docprompt/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.2.8/docprompt/_exec/__init__.py
--rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.2.8/docprompt/_exec/ghostscript.py
--rw-r--r--   0        0        0        0 2024-03-18 23:40:35.967506 docprompt-0.2.8/docprompt/provenance/__init__.py
--rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.2.8/docprompt/provenance/search.py
--rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.2.8/docprompt/provenance/source.py
--rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.2.8/docprompt/provenance/util.py
--rw-r--r--   0        0        0     5560 2024-04-14 18:42:33.400748 docprompt-0.2.8/docprompt/rasterize.py
--rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.2.8/docprompt/schema/__init__.py
--rw-r--r--   0        0        0     9704 2024-04-14 18:42:33.400748 docprompt-0.2.8/docprompt/schema/document.py
--rw-r--r--   0        0        0     6649 2024-04-13 03:18:18.370507 docprompt-0.2.8/docprompt/schema/layout.py
--rw-r--r--   0        0        0     3764 2024-04-05 21:39:58.248888 docprompt-0.2.8/docprompt/schema/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.2.8/docprompt/tasks/__init__.py
--rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.2.8/docprompt/tasks/base.py
--rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.2.8/docprompt/tasks/classification/__init__.py
--rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.2.8/docprompt/tasks/message.py
--rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.2.8/docprompt/tasks/ocr/__init__.py
--rw-r--r--   0        0        0    18558 2024-04-13 03:18:18.370507 docprompt-0.2.8/docprompt/tasks/ocr/gcp.py
--rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.2.8/docprompt/tasks/ocr/result.py
--rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.2.8/docprompt/tasks/table_extraction/__init__.py
--rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.2.8/docprompt/tasks/table_extraction/base.py
--rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.2.8/docprompt/tasks/table_extraction/providers/__init__.py
--rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.2.8/docprompt/tasks/table_extraction/providers/claude.py
--rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.2.8/docprompt/tasks/table_extraction/result.py
--rw-r--r--   0        0        0      351 2024-03-14 21:45:48.927780 docprompt-0.2.8/docprompt/utils/__init__.py
--rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.2.8/docprompt/utils/compressor.py
--rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.2.8/docprompt/utils/date_extraction.py
--rw-r--r--   0        0        0        0 2024-03-18 15:46:16.978297 docprompt-0.2.8/docprompt/utils/raster.py
--rw-r--r--   0        0        0     4015 2024-04-13 03:01:14.714377 docprompt-0.2.8/docprompt/utils/splitter.py
--rw-r--r--   0        0        0     3994 2024-04-05 21:52:56.007611 docprompt-0.2.8/docprompt/utils/util.py
--rw-r--r--   0        0        0     4131 2024-04-14 18:42:28.484709 docprompt-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.2.8/tests/fixtures/1.pdf
--rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.2.8/tests/fixtures/1_ocr.json
--rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.2.8/tests/fixtures.py
--rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.2.8/tests/test_date_extraction.py
--rw-r--r--   0        0        0     3656 2024-04-14 18:42:33.400748 docprompt-0.2.8/tests/test_document.py
--rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.2.8/tests/test_layout_models.py
--rw-r--r--   0        0        0     1227 2024-04-09 01:36:21.595068 docprompt-0.2.8/tests/test_search.py
--rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.2.8/tests/test_threadpool.py
--rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.2.8/tests/util.py
--rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 docprompt-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      585 2024-04-18 22:55:47.915108 docprompt-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4917 2024-04-18 22:55:47.915108 docprompt-0.3.0/README.md
+-rw-r--r--   0        0        0      674 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/_exec/__init__.py
+-rw-r--r--   0        0        0     2395 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/_exec/ghostscript.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/provenance/__init__.py
+-rw-r--r--   0        0        0     9850 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/provenance/search.py
+-rw-r--r--   0        0        0     1357 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/provenance/source.py
+-rw-r--r--   0        0        0     6054 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/provenance/util.py
+-rw-r--r--   0        0        0     7095 2024-04-23 00:28:28.294162 docprompt-0.3.0/docprompt/rasterize.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/schema/__init__.py
+-rw-r--r--   0        0        0     8981 2024-04-23 00:27:13.953736 docprompt-0.3.0/docprompt/schema/document.py
+-rw-r--r--   0        0        0     6649 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/schema/layout.py
+-rw-r--r--   0        0        0     8448 2024-04-23 00:27:13.953736 docprompt-0.3.0/docprompt/schema/pipeline.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/tasks/__init__.py
+-rw-r--r--   0        0        0     5103 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/tasks/classification/__init__.py
+-rw-r--r--   0        0        0     2522 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/tasks/message.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/tasks/ocr/__init__.py
+-rw-r--r--   0        0        0    18558 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/tasks/ocr/gcp.py
+-rw-r--r--   0        0        0     1170 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/tasks/ocr/result.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/tasks/table_extraction/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/tasks/table_extraction/base.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/tasks/table_extraction/providers/__init__.py
+-rw-r--r--   0        0        0     3420 2024-04-18 22:55:47.915108 docprompt-0.3.0/docprompt/tasks/table_extraction/providers/claude.py
+-rw-r--r--   0        0        0      783 2024-04-18 22:55:47.919108 docprompt-0.3.0/docprompt/tasks/table_extraction/result.py
+-rw-r--r--   0        0        0      351 2024-04-18 22:55:47.919108 docprompt-0.3.0/docprompt/utils/__init__.py
+-rw-r--r--   0        0        0      421 2024-04-18 22:55:47.919108 docprompt-0.3.0/docprompt/utils/compressor.py
+-rw-r--r--   0        0        0     4915 2024-04-18 22:55:47.919108 docprompt-0.3.0/docprompt/utils/date_extraction.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.919108 docprompt-0.3.0/docprompt/utils/masking/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-18 22:55:47.919108 docprompt-0.3.0/docprompt/utils/masking/image.py
+-rw-r--r--   0        0        0     4015 2024-04-18 22:55:47.919108 docprompt-0.3.0/docprompt/utils/splitter.py
+-rw-r--r--   0        0        0     3994 2024-04-18 22:55:47.919108 docprompt-0.3.0/docprompt/utils/util.py
+-rw-r--r--   0        0        0     4131 2024-04-23 00:28:36.802211 docprompt-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-04-18 22:55:47.935108 docprompt-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0   123638 2024-04-18 22:55:47.935108 docprompt-0.3.0/tests/fixtures/1.pdf
+-rw-r--r--   0        0        0  2788655 2024-04-18 22:55:47.943108 docprompt-0.3.0/tests/fixtures/1_ocr.json
+-rw-r--r--   0        0        0      202 2024-04-18 22:55:47.935108 docprompt-0.3.0/tests/fixtures.py
+-rw-r--r--   0        0        0      830 2024-04-18 22:55:47.943108 docprompt-0.3.0/tests/test_date_extraction.py
+-rw-r--r--   0        0        0     3656 2024-04-18 22:55:47.943108 docprompt-0.3.0/tests/test_document.py
+-rw-r--r--   0        0        0      590 2024-04-23 00:27:13.937736 docprompt-0.3.0/tests/test_documentnode.py
+-rw-r--r--   0        0        0     1361 2024-04-18 22:55:47.943108 docprompt-0.3.0/tests/test_layout_models.py
+-rw-r--r--   0        0        0     1227 2024-04-18 22:55:47.943108 docprompt-0.3.0/tests/test_search.py
+-rw-r--r--   0        0        0      878 2024-04-18 22:55:47.943108 docprompt-0.3.0/tests/test_threadpool.py
+-rw-r--r--   0        0        0     1003 2024-04-18 22:55:47.943108 docprompt-0.3.0/tests/util.py
+-rw-r--r--   0        0        0     7726 1970-01-01 00:00:00.000000 docprompt-0.3.0/PKG-INFO
```

### Comparing `docprompt-0.2.8/LICENSE` & `docprompt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/README.md` & `docprompt-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/__init__.py` & `docprompt-0.3.0/docprompt/__init__.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/_exec/ghostscript.py` & `docprompt-0.3.0/docprompt/_exec/ghostscript.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/provenance/search.py` & `docprompt-0.3.0/docprompt/provenance/search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/provenance/source.py` & `docprompt-0.3.0/docprompt/provenance/source.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/provenance/util.py` & `docprompt-0.3.0/docprompt/provenance/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/schema/document.py` & `docprompt-0.3.0/docprompt/schema/document.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from pydantic import Field
 
 import magic
 import pypdfium2 as pdfium
 from pydantic import (
     BaseModel,
     PositiveInt,
-    PrivateAttr,
     computed_field,
     field_serializer,
     field_validator,
 )
 
 from docprompt._exec.ghostscript import (
     compress_pdf_to_bytes,
@@ -58,16 +57,14 @@
     Represents a PDF document
     """
 
     name: str = Field(description="The name of the document")
     file_bytes: bytes = Field(description="The bytes of the document", repr=False)
     file_path: Optional[str] = None
 
-    _raster_cache: Dict[int, Dict[int, bytes]] = PrivateAttr(default_factory=dict)
-
     def __len__(self):
         return self.num_pages
 
     def __hash__(self):
         return hash(self.document_hash)
 
     @computed_field
@@ -162,47 +159,36 @@
         page_number: int,
         *,
         dpi: int = DEFAULT_DPI,
         downscale_size: Optional[Tuple[int, int]] = None,
         resize_mode: ResizeModes = "thumbnail",
         max_file_size_bytes: Optional[int] = None,
         resize_aspect_ratios: Optional[Iterable[AspectRatioRule]] = None,
-        use_cache: bool = True,
         do_convert: bool = False,
         image_covert_mode: str = "L",
         do_quantize: bool = False,
         quantize_color_count: int = 8,
     ) -> bytes:
         """
         Rasterizes a page of the document using Pdfium
         """
-        generated_image = False
 
         if page_number < 0 or page_number > self.num_pages:
             raise ValueError(f"Page number must be between 0 and {self.num_pages}")
 
-        if use_cache and self._raster_cache.get(dpi, {}).get(page_number):
-            rastered = self._raster_cache[dpi][page_number]
-        else:
-            pdf = pdfium.PdfDocument(BytesIO(self.file_bytes))
-            page = pdf[page_number - 1]
-
-            bitmap = page.render(scale=(1 / 72) * dpi)
-
-            pil = bitmap.to_pil().convert("RGB")
+        pdf = pdfium.PdfDocument(BytesIO(self.file_bytes))
+        page = pdf[page_number - 1]
 
-            img_bytes = BytesIO()
-            pil.save(img_bytes, format="PNG")
-            rastered = img_bytes.getvalue()
+        bitmap = page.render(scale=(1 / 72) * dpi)
 
-            generated_image = True
+        pil = bitmap.to_pil().convert("RGB")
 
-        if use_cache and generated_image:
-            self._raster_cache.setdefault(dpi, {})
-            self._raster_cache[dpi][page_number] = rastered
+        img_bytes = BytesIO()
+        pil.save(img_bytes, format="PNG")
+        rastered = img_bytes.getvalue()
 
         rastered = process_raster_image(
             rastered,
             resize_width=downscale_size[0] if downscale_size else None,
             resize_height=downscale_size[1] if downscale_size else None,
             resize_mode=resize_mode,
             resize_aspect_ratios=resize_aspect_ratios,
@@ -248,36 +234,30 @@
             resize_aspect_ratios=resize_aspect_ratios,
         )
         return f"data:image/png;base64,{base64.b64encode(image_bytes).decode('utf-8')}"
 
     def rasterize_pdf(
         self,
         dpi: int = DEFAULT_DPI,
-        use_cache: bool = True,
+        max_file_size_bytes: Optional[int] = None,
     ) -> Dict[int, bytes]:
         """
         Rasterizes the entire document using Pdfium
         """
-        if (
-            use_cache
-            and self._raster_cache.get(dpi)
-            and len(self._raster_cache[dpi]) == self.num_pages
-        ):
-            return self._raster_cache[dpi]
 
         result = {}
 
         for page_number in range(1, self.num_pages + 1):
             result[page_number] = self.rasterize_page(
-                page_number, dpi=dpi, use_cache=False
+                page_number,
+                dpi=dpi,
+                use_cache=False,
+                max_file_size_bytes=max_file_size_bytes,
             )
 
-        if use_cache:
-            self._raster_cache[dpi] = result.copy()  # Shallow copy should be OK
-
         return result
 
     def split(self, start: Optional[int] = None, stop: Optional[int] = None):
         """
         Splits a document into multiple documents
         """
         if start is None and stop is None:
```

### Comparing `docprompt-0.2.8/docprompt/schema/layout.py` & `docprompt-0.3.0/docprompt/schema/layout.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/tasks/base.py` & `docprompt-0.3.0/docprompt/tasks/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/tasks/message.py` & `docprompt-0.3.0/docprompt/tasks/message.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/tasks/ocr/gcp.py` & `docprompt-0.3.0/docprompt/tasks/ocr/gcp.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/tasks/ocr/result.py` & `docprompt-0.3.0/docprompt/tasks/ocr/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/tasks/table_extraction/base.py` & `docprompt-0.3.0/docprompt/tasks/table_extraction/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/tasks/table_extraction/providers/claude.py` & `docprompt-0.3.0/docprompt/tasks/table_extraction/providers/claude.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/tasks/table_extraction/result.py` & `docprompt-0.3.0/docprompt/tasks/table_extraction/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/utils/date_extraction.py` & `docprompt-0.3.0/docprompt/utils/date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/utils/splitter.py` & `docprompt-0.3.0/docprompt/utils/splitter.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/docprompt/utils/util.py` & `docprompt-0.3.0/docprompt/utils/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/pyproject.toml` & `docprompt-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "docprompt"
-version = "0.2.8"
+version = "0.3.0"
 homepage = "https://github.com/Page-Leaf/docprompt"
 description = "Documents and large language models."
 authors = ["Frankie Colson <frank@pageleaf.io>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `docprompt-0.2.8/tests/fixtures/1.pdf` & `docprompt-0.3.0/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/tests/fixtures/1_ocr.json` & `docprompt-0.3.0/tests/fixtures/1_ocr.json`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/tests/test_date_extraction.py` & `docprompt-0.3.0/tests/test_date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/tests/test_document.py` & `docprompt-0.3.0/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/tests/test_layout_models.py` & `docprompt-0.3.0/tests/test_layout_models.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/tests/test_search.py` & `docprompt-0.3.0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/tests/test_threadpool.py` & `docprompt-0.3.0/tests/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/tests/util.py` & `docprompt-0.3.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.8/PKG-INFO` & `docprompt-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: docprompt
-Version: 0.2.8
+Version: 0.3.0
 Summary: Documents and large language models.
 Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0
 Author: Frankie Colson
 Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: azure
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: google
 Provides-Extra: search
 Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,51 +1,51 @@
-Metadata-Version: 2.1 Name: docprompt Version: 0.2.8 Summary: Documents and
+Metadata-Version: 2.1 Name: docprompt Version: 0.3.0 Summary: Documents and
 large language models. Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0 Author: Frankie Colson Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.8 Provides-Extra: azure Provides-Extra: dev Provides-Extra: doc
-Provides-Extra: google Provides-Extra: search Provides-Extra: test Requires-
-Dist: azure-ai-formrecognizer (>=3.3.0) ; extra == "azure" Requires-Dist:
-bump2version (>=1.0.1,<2.0.0) ; extra == "dev" Requires-Dist: flake8
-(>=6.1.0,<7.0.0) ; extra == "test" Requires-Dist: flake8-docstrings
-(>=1.7.0,<2.0.0) ; extra == "test" Requires-Dist: fsspec (>=2022.11.0)
-Requires-Dist: google-cloud-documentai (>=2.20.0) ; extra == "google" Requires-
-Dist: isort (>=5.12.0,<6.0.0) ; extra == "test" Requires-Dist: mkdocs
-(>=1.1.2,<2.0.0) ; extra == "doc" Requires-Dist: mkdocs-autorefs
-(>=0.2.1,<0.3.0) ; extra == "doc" Requires-Dist: mkdocs-include-markdown-plugin
-(>=1.0.0,<2.0.0) ; extra == "doc" Requires-Dist: mkdocs-material
-(>=6.1.7,<7.0.0) ; extra == "doc" Requires-Dist: mkdocs-material-extensions
-(>=1.0.1,<2.0.0) Requires-Dist: mkdocstrings (>=0.15.2,<0.16.0) ; extra ==
-"doc" Requires-Dist: mypy (>=1.6.1,<2.0.0) ; extra == "test" Requires-Dist:
-networkx (>=2.8.8) ; extra == "search" Requires-Dist: numpy (>=1.20.3,<2.0.0)
-Requires-Dist: pillow (>=9.0.1) Requires-Dist: pip (>=20.3.1,<21.0.0) ; extra
-== "dev" Requires-Dist: pre-commit (>=2.12.0,<3.0.0) ; extra == "dev" Requires-
-Dist: pydantic (>=2.1.0) Requires-Dist: pypdfium2 (>=4.28.0,<5.0.0) Requires-
-Dist: pytest (>=7.4.2,<8.0.0) ; extra == "test" Requires-Dist: pytest-cov
-(>=4.1.0,<5.0.0) ; extra == "test" Requires-Dist: python-dateutil
-(>=2.8.2,<3.0.0) Requires-Dist: python-magic (>=0.4.24) Requires-Dist:
-rapidfuzz (>=3.0.0) Requires-Dist: rtree (>=1.2.0,<2.0.0) ; extra == "search"
-Requires-Dist: ruff (>=0.3.3,<0.4.0) ; extra == "test" Requires-Dist: tantivy
-(>=0.21.0,<0.22.0) ; extra == "search" Requires-Dist: tenacity (>=7.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev" Requires-Dist: tox
-(>=3.20.1,<4.0.0) ; extra == "dev" Requires-Dist: tqdm (>=4.61.0) Requires-
-Dist: twine (>=3.3.0,<4.0.0) ; extra == "dev" Requires-Dist: virtualenv
-(>=20.2.2,<21.0.0) ; extra == "dev" Description-Content-Type: text/markdown [!
-[pypi](https://img.shields.io/pypi/v/docprompt.svg)](https://pypi.org/project/
-docprompt/) [![python](https://img.shields.io/pypi/pyversions/docprompt.svg)]
-(https://pypi.org/project/docprompt/) [![Build Status](https://github.com/Page-
-Leaf/Docprompt/actions/workflows/dev.yml/badge.svg)](https://github.com/Page-
-Leaf/docprompt/actions/workflows/dev.yml) [![codecov](https://codecov.io/gh/
-Page-Leaf/Docprompt/branch/main/graphs/badge.svg)](https://codecov.io/github/
-Page-Leaf/Docprompt)
+Python :: 3.12 Classifier: Programming Language :: Python :: 3.8 Provides-
+Extra: azure Provides-Extra: dev Provides-Extra: doc Provides-Extra: google
+Provides-Extra: search Provides-Extra: test Requires-Dist: azure-ai-
+formrecognizer (>=3.3.0) ; extra == "azure" Requires-Dist: bump2version
+(>=1.0.1,<2.0.0) ; extra == "dev" Requires-Dist: flake8 (>=6.1.0,<7.0.0) ;
+extra == "test" Requires-Dist: flake8-docstrings (>=1.7.0,<2.0.0) ; extra ==
+"test" Requires-Dist: fsspec (>=2022.11.0) Requires-Dist: google-cloud-
+documentai (>=2.20.0) ; extra == "google" Requires-Dist: isort
+(>=5.12.0,<6.0.0) ; extra == "test" Requires-Dist: mkdocs (>=1.1.2,<2.0.0) ;
+extra == "doc" Requires-Dist: mkdocs-autorefs (>=0.2.1,<0.3.0) ; extra == "doc"
+Requires-Dist: mkdocs-include-markdown-plugin (>=1.0.0,<2.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-material (>=6.1.7,<7.0.0) ; extra == "doc" Requires-Dist:
+mkdocs-material-extensions (>=1.0.1,<2.0.0) Requires-Dist: mkdocstrings
+(>=0.15.2,<0.16.0) ; extra == "doc" Requires-Dist: mypy (>=1.6.1,<2.0.0) ;
+extra == "test" Requires-Dist: networkx (>=2.8.8) ; extra == "search" Requires-
+Dist: numpy (>=1.20.3,<2.0.0) Requires-Dist: pillow (>=9.0.1) Requires-Dist:
+pip (>=20.3.1,<21.0.0) ; extra == "dev" Requires-Dist: pre-commit
+(>=2.12.0,<3.0.0) ; extra == "dev" Requires-Dist: pydantic (>=2.1.0) Requires-
+Dist: pypdfium2 (>=4.28.0,<5.0.0) Requires-Dist: pytest (>=7.4.2,<8.0.0) ;
+extra == "test" Requires-Dist: pytest-cov (>=4.1.0,<5.0.0) ; extra == "test"
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: python-magic
+(>=0.4.24) Requires-Dist: rapidfuzz (>=3.0.0) Requires-Dist: rtree
+(>=1.2.0,<2.0.0) ; extra == "search" Requires-Dist: ruff (>=0.3.3,<0.4.0) ;
+extra == "test" Requires-Dist: tantivy (>=0.21.0,<0.22.0) ; extra == "search"
+Requires-Dist: tenacity (>=7.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0) ;
+extra == "dev" Requires-Dist: tox (>=3.20.1,<4.0.0) ; extra == "dev" Requires-
+Dist: tqdm (>=4.61.0) Requires-Dist: twine (>=3.3.0,<4.0.0) ; extra == "dev"
+Requires-Dist: virtualenv (>=20.2.2,<21.0.0) ; extra == "dev" Description-
+Content-Type: text/markdown [![pypi](https://img.shields.io/pypi/v/
+docprompt.svg)](https://pypi.org/project/docprompt/) [![python](https://
+img.shields.io/pypi/pyversions/docprompt.svg)](https://pypi.org/project/
+docprompt/) [![Build Status](https://github.com/Page-Leaf/Docprompt/actions/
+workflows/dev.yml/badge.svg)](https://github.com/Page-Leaf/docprompt/actions/
+workflows/dev.yml) [![codecov](https://codecov.io/gh/Page-Leaf/Docprompt/
+branch/main/graphs/badge.svg)](https://codecov.io/github/Page-Leaf/Docprompt)
                                     _[_L_o_g_o_]
                               ******** DDooccpprroommpptt ********
                         Document AI, powered by LLM's
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                        Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 # About Docprompt is a library for Document AI. It aims to make enterprise-
```

