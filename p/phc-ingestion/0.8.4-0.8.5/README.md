# Comparing `tmp/phc-ingestion-0.8.4.tar.gz` & `tmp/phc-ingestion-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.8.4.tar", last modified: Fri Apr 19 09:07:23 2024, max compression
+gzip compressed data, was "phc-ingestion-0.8.5.tar", last modified: Tue Apr 23 09:22:50 2024, max compression
```

## Comparing `phc-ingestion-0.8.4.tar` & `phc-ingestion-0.8.5.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0       16 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/PYPI.md
--rw-r--r--   0        0        0        0 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1257 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4441 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1640 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      507 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      770 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/hla.py
--rw-r--r--   0        0        0    12312 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/ihc.py
--rw-r--r--   0        0        0      555 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4706 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/json.py
--rw-r--r--   0        0        0     9536 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     2051 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/specimen_details.py
--rw-r--r--   0        0        0     4599 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0      372 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/tests.py
--rw-r--r--   0        0        0     1027 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/tmb.py
--rw-r--r--   0        0        0     1595 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     3440 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3151 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0    10987 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     2163 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0        0 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/generic/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/generic/process.py
--rw-r--r--   0        0        0     2814 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/generic/utils.py
--rw-r--r--   0        0        0       46 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3074 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     8522 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     5563 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     7341 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     2047 2024-04-19 09:07:01.761364 phc-ingestion-0.8.4/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0      162 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/ingestion/shared_util/open_maybe_gzipped.py
--rw-r--r--   0        0        0       68 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/ingestion/shared_util/types.py
--rw-r--r--   0        0        0     5398 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/ingestion/vcf_standardization/Variant.py
--rw-r--r--   0        0        0        0 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/ingestion/vcf_standardization/__init__.py
--rw-r--r--   0        0        0     2289 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/ingestion/vcf_standardization/standardize.py
--rw-r--r--   0        0        0        0 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/ingestion/vcf_standardization/util/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/ingestion/vcf_standardization/util/af_helpers.py
--rw-r--r--   0        0        0      823 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/ingestion/vcf_standardization/util/dp_helpers.py
--rw-r--r--   0        0        0     2471 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/ingestion/vcf_standardization/util/read_write.py
--rw-r--r--   0        0        0     1010 2024-04-19 09:07:01.765364 phc-ingestion-0.8.4/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/PYPI.md
+-rw-r--r--   0        0        0        0 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1257 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4441 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1640 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      507 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      770 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/hla.py
+-rw-r--r--   0        0        0    12312 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/ihc.py
+-rw-r--r--   0        0        0      555 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4706 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0     9536 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     2051 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/specimen_details.py
+-rw-r--r--   0        0        0     4599 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0      372 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/tests.py
+-rw-r--r--   0        0        0     1027 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/tmb.py
+-rw-r--r--   0        0        0     1595 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     3440 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3151 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0    10987 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     2163 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0        0 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/generic/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/generic/process.py
+-rw-r--r--   0        0        0     2814 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/generic/utils.py
+-rw-r--r--   0        0        0       46 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3074 2024-04-23 09:22:26.234705 phc-ingestion-0.8.5/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0      741 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/nextgen/util/manifest_helpers.py
+-rw-r--r--   0        0        0     2284 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8133 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     5563 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     7341 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2047 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0      162 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/shared_util/open_maybe_gzipped.py
+-rw-r--r--   0        0        0       68 2024-04-23 09:22:26.238705 phc-ingestion-0.8.5/ingestion/shared_util/types.py
+-rw-r--r--   0        0        0     5398 2024-04-23 09:22:26.242704 phc-ingestion-0.8.5/ingestion/vcf_standardization/Variant.py
+-rw-r--r--   0        0        0        0 2024-04-23 09:22:26.242704 phc-ingestion-0.8.5/ingestion/vcf_standardization/__init__.py
+-rw-r--r--   0        0        0     2289 2024-04-23 09:22:26.242704 phc-ingestion-0.8.5/ingestion/vcf_standardization/standardize.py
+-rw-r--r--   0        0        0        0 2024-04-23 09:22:26.242704 phc-ingestion-0.8.5/ingestion/vcf_standardization/util/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-23 09:22:26.242704 phc-ingestion-0.8.5/ingestion/vcf_standardization/util/af_helpers.py
+-rw-r--r--   0        0        0      823 2024-04-23 09:22:26.242704 phc-ingestion-0.8.5/ingestion/vcf_standardization/util/dp_helpers.py
+-rw-r--r--   0        0        0     2471 2024-04-23 09:22:26.242704 phc-ingestion-0.8.5/ingestion/vcf_standardization/util/read_write.py
+-rw-r--r--   0        0        0     1009 2024-04-23 09:22:26.242704 phc-ingestion-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.8.5/PKG-INFO
```

### Comparing `phc-ingestion-0.8.4/ingestion/caris/process.py` & `phc-ingestion-0.8.5/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/caris/util/cnv.py` & `phc-ingestion-0.8.5/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.8.5/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/caris/util/hla.py` & `phc-ingestion-0.8.5/ingestion/caris/util/hla.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/caris/util/ihc.py` & `phc-ingestion-0.8.5/ingestion/caris/util/ihc.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.8.5/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/caris/util/json.py` & `phc-ingestion-0.8.5/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/caris/util/metadata.py` & `phc-ingestion-0.8.5/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/caris/util/specimen_details.py` & `phc-ingestion-0.8.5/ingestion/caris/util/specimen_details.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/caris/util/structural.py` & `phc-ingestion-0.8.5/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/caris/util/tmb.py` & `phc-ingestion-0.8.5/ingestion/caris/util/tmb.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/caris/util/tsv.py` & `phc-ingestion-0.8.5/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/caris/util/vcf.py` & `phc-ingestion-0.8.5/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/foundation/process.py` & `phc-ingestion-0.8.5/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.8.5/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.8.5/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.8.5/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.8.5/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/generic/process.py` & `phc-ingestion-0.8.5/ingestion/generic/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/generic/utils.py` & `phc-ingestion-0.8.5/ingestion/generic/utils.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/nextgen/process.py` & `phc-ingestion-0.8.5/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.8.5/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.8.5/ingestion/nextgen/util/process_manifest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
-from ruamel.yaml import YAML
 from logging import Logger
 
+import ingestion.nextgen.util.manifest_helpers as manifest_helpers
+
 
 def transform_date(date: str):
     """mm/dd/yyyy -> yyyy-mm-dd"""
     date_list = date.split("/")
     new_date = f"{date_list[2]}-{date_list[0]}-{date_list[1]}"
     return new_date
 
@@ -136,31 +137,25 @@
             manifest["collDate"] = transform_date(coll_date)
 
         if "receivedDate" not in manifest and "Received" in line:
             recArray = line.split(" ")
             rec_date = search_and_grab(recArray, "Received", 1)
             manifest["receivedDate"] = transform_date(rec_date)
 
-        if "reportID" not in manifest and "Accession" in line:
-            reportArray = line.split(" ")
-            report_id = search_and_grab(reportArray, "Accession", 2)
-            manifest["reportID"] = report_id
+        if "reportID" not in manifest and "Accession #" in line:
+            manifest["reportID"] = manifest_helpers.parse_report_id(line)
+
+        if "sampleNumber" not in manifest and "Specimen #" in line:
+            manifest["sampleNumber"] = manifest_helpers.parse_sample_number(line)
 
         if "orderingMDName" not in manifest and "Physician Name:" in line:
-            physArray = line.split(" ")
-            phys_last = search_and_grab(physArray, "Name:", 1)
-            phys_first = search_and_grab(physArray, "Name:", 2)
-            manifest["orderingMDName"] = f"{phys_last} {phys_first}"
+            manifest["orderingMDName"] = manifest_helpers.parse_ordering_md(line)
 
         if "indication" not in manifest and "Reason for Referral" in line:
-            indicationArray = line.split(" ")
-            indication = search_and_grab(indicationArray, "Referral", 1)
-            # Accounting for two-word indication
-            if "</" not in search_and_grab(indicationArray, "Referral", 2):
-                indication = f'{indication} {search_and_grab(indicationArray, "Referral", 2)}'
+            indication = manifest_helpers.parse_indication(line)
             manifest["indication"] = indication
             manifest["indicationDisplay"] = indication
 
         if "bodySite" not in manifest and "Specimen:" in line:
             bodySiteArray = line.split(" ")
             body_site_one = search_and_grab(bodySiteArray, "Specimen:", 1)
             body_site_two = search_and_grab(bodySiteArray, "Specimen:", 2)
@@ -184,17 +179,15 @@
     test_text = extract_xml_text(xml_in_file)
     interpretation_text = extract_interpretation_text(xml_in_file)
     manifest = extract_test_data(test_text, interpretation_text)
     manifest.update(extract_patient_data(test_text))
 
     manifest["reportFile"] = f".lifeomic/nextgen/{prefix}/{prefix}.pdf"
     manifest["sourceFileId"] = source_file_id
-    manifest["resources"] = [
-        {"fileName": f".lifeomic/nextgen/{prefix}/{prefix}.pdf"},
-    ]
+    manifest["resources"] = []
 
     manifest["files"] = [
         {
             "fileName": f".lifeomic/nextgen/{prefix}/{prefix}.copynumber.csv",
             "sequenceType": "somatic",
             "type": "copyNumberVariant",
         },
```

### Comparing `phc-ingestion-0.8.4/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.8.5/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.8.5/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.8.5/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.8.5/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.8.5/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.8.5/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.8.5/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/vcf_standardization/Variant.py` & `phc-ingestion-0.8.5/ingestion/vcf_standardization/Variant.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/vcf_standardization/standardize.py` & `phc-ingestion-0.8.5/ingestion/vcf_standardization/standardize.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/vcf_standardization/util/af_helpers.py` & `phc-ingestion-0.8.5/ingestion/vcf_standardization/util/af_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/vcf_standardization/util/dp_helpers.py` & `phc-ingestion-0.8.5/ingestion/vcf_standardization/util/dp_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/ingestion/vcf_standardization/util/read_write.py` & `phc-ingestion-0.8.5/ingestion/vcf_standardization/util/read_write.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.4/pyproject.toml` & `phc-ingestion-0.8.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.8.4"
+version = "0.8.5"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
@@ -28,18 +28,18 @@
 build-backend = "pdm.pep517.api"
 
 [tool.black]
 line-length = 100
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "black==24.3.0",
-    "pytest==7.1.2",
-    "pytest-cov==2.10.1",
-    "coverage==6.4.1",
+    "black==24.4.0",
+    "pytest==8.1.1",
+    "pytest-cov==5.0.0",
+    "coverage==7.4.4",
 ]
 
 [tool.pdm.build]
 excludes = [
     "tests/",
 ]
```

