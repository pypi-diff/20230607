# Comparing `tmp/phc-ingestion-0.3.34.tar.gz` & `tmp/phc-ingestion-0.3.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.34.tar", last modified: Tue Jun  6 16:50:14 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.35.tar", last modified: Wed Jun  7 14:39:07 2023, max compression
```

## Comparing `phc-ingestion-0.3.34.tar` & `phc-ingestion-0.3.35.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       16 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/PYPI.md
--rw-r--r--   0        0        0        0 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1603 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      555 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4636 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21500 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     5010 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3127 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8876 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     3187 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     7409 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     3785 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     5664 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     1913 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2023-06-06 16:49:46.543448 phc-ingestion-0.3.34/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0     1029 2023-06-06 16:49:46.547448 phc-ingestion-0.3.34/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.34/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/PYPI.md
+-rw-r--r--   0        0        0        0 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1603 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4636 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21500 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     5010 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3127 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8876 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     3187 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     2976 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     7368 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     3785 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     5664 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     1913 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-06-07 14:38:43.227614 phc-ingestion-0.3.35/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-06-07 14:38:43.227614 phc-ingestion-0.3.35/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2023-06-07 14:38:43.227614 phc-ingestion-0.3.35/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2023-06-07 14:38:43.227614 phc-ingestion-0.3.35/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2023-06-07 14:38:43.227614 phc-ingestion-0.3.35/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0     1029 2023-06-07 14:38:43.227614 phc-ingestion-0.3.35/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.35/PKG-INFO
```

### Comparing `phc-ingestion-0.3.34/ingestion/caris/process.py` & `phc-ingestion-0.3.35/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.35/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.35/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.35/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.35/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/caris/util/json.py` & `phc-ingestion-0.3.35/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.35/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.35/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.35/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.35/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/foundation/process.py` & `phc-ingestion-0.3.35/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.35/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.35/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.35/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.35/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/nextgen/process.py` & `phc-ingestion-0.3.35/ingestion/nextgen/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,18 @@
         structural_path_name, structural_status = process_structural(
             xml_in_file=vendor_files["xmlFile"],
             sv_in_file=vendor_files["somaticSvVcfFile"],
             root_path=local_output_dir,
             prefix=prefix,
             log=log,
         )
-        xml_pdf_prefix = vendor_files["pdfFile"].split("/")[-1].split(".")[0]
         manifest = process_manifest(
             xml_in_file=vendor_files["xmlFile"],
             source_file_id=source_file_id,
             prefix=prefix,
-            xml_pdf_prefix=xml_pdf_prefix,
             structural_status=structural_status,
             log=log,
         )
         somatic_vcf_meta_data = process_vcf(
             vcf_in_file=vendor_files["somaticVcfFile"],
             root_path=local_output_dir,
             prefix=prefix,
```

### Comparing `phc-ingestion-0.3.34/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.3.35/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.35/ingestion/nextgen/util/process_manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,26 +141,25 @@
     return manifest
 
 
 def process_manifest(
     xml_in_file: str,
     source_file_id: str,
     prefix: str,
-    xml_pdf_prefix: str,
     structural_status: bool,
     log: Logger,
 ):
     xml_text = extract_xml_text(xml_in_file)
     manifest = extract_test_data(xml_text)
     manifest.update(extract_patient_data(xml_text))
 
-    manifest["reportFile"] = f".lifeomic/nextgen/{prefix}/{xml_pdf_prefix}.pdf"
+    manifest["reportFile"] = f".lifeomic/nextgen/{prefix}/{prefix}.pdf"
     manifest["sourceFileId"] = source_file_id
     manifest["resources"] = [
-        {"fileName": f".lifeomic/nextgen/{prefix}/{xml_pdf_prefix}.pdf"},
+        {"fileName": f".lifeomic/nextgen/{prefix}/{prefix}.pdf"},
     ]
 
     manifest["files"] = [
         {
             "fileName": f".lifeomic/nextgen/{prefix}/{prefix}.copynumber.csv",
             "sequenceType": "somatic",
             "type": "copyNumberVariant",
```

### Comparing `phc-ingestion-0.3.34/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.35/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.35/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.3.35/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.35/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.35/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.3.35/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.3.35/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.34/pyproject.toml` & `phc-ingestion-0.3.35/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.34"
+version = "0.3.35"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

