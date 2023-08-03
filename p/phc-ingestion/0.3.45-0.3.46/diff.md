# Comparing `tmp/phc-ingestion-0.3.45.tar.gz` & `tmp/phc-ingestion-0.3.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.45.tar", last modified: Fri Jul 21 19:15:11 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.46.tar", last modified: Thu Aug  3 11:26:01 2023, max compression
```

## Comparing `phc-ingestion-0.3.45.tar` & `phc-ingestion-0.3.46.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       16 2023-07-21 19:14:47.718323 phc-ingestion-0.3.45/PYPI.md
--rw-r--r--   0        0        0        0 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1636 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      555 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4676 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21646 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     6933 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3142 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8742 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     5501 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3074 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     8522 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     3785 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     7341 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     2047 2023-07-21 19:14:47.730323 phc-ingestion-0.3.45/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-07-21 19:14:47.734323 phc-ingestion-0.3.45/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-07-21 19:14:47.734323 phc-ingestion-0.3.45/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2023-07-21 19:14:47.734323 phc-ingestion-0.3.45/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2023-07-21 19:14:47.734323 phc-ingestion-0.3.45/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2023-07-21 19:14:47.734323 phc-ingestion-0.3.45/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0     1029 2023-07-21 19:14:47.734323 phc-ingestion-0.3.45/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.45/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-08-03 11:25:26.745044 phc-ingestion-0.3.46/PYPI.md
+-rw-r--r--   0        0        0        0 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1636 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     5074 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21646 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     6933 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3142 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8742 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     5501 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3074 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8522 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     3785 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     7341 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2047 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-08-03 11:25:26.757044 phc-ingestion-0.3.46/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-08-03 11:25:26.761045 phc-ingestion-0.3.46/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2023-08-03 11:25:26.761045 phc-ingestion-0.3.46/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2023-08-03 11:25:26.761045 phc-ingestion-0.3.46/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2023-08-03 11:25:26.761045 phc-ingestion-0.3.46/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0     1029 2023-08-03 11:25:26.761045 phc-ingestion-0.3.46/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.46/PKG-INFO
```

### Comparing `phc-ingestion-0.3.45/ingestion/caris/process.py` & `phc-ingestion-0.3.46/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.46/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.46/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.46/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.46/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/caris/util/json.py` & `phc-ingestion-0.3.46/ingestion/caris/util/json.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,20 @@
     file_list = glob.glob("*")
     files = {}
 
     files["bam"] = []
     files["R1.fastq.gz"] = []
     files["R2.fastq.gz"] = []
 
+    # if file_list has more than one file that starts with DNA_ or RNA_ then we need to throw an error
+    if len([file for file in file_list if file.startswith("DNA_")]) > 1:
+        raise Exception(f"More than one DNA file found in {file_name}\n")
+    if len([file for file in file_list if file.startswith("RNA_")]) > 1:
+        raise Exception(f"More than one RNA file found in {file_name}\n")
+
     for file in file_list:
         extension = file.split(".")[1:]
         if not isinstance(extension, str):
             extension = ".".join(extension)
         # We can have multiple bam files (RNA and DNA)
         if extension == "bam" or "fastq" in extension:
             files[extension].append(file)
```

### Comparing `phc-ingestion-0.3.45/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.46/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.46/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.46/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.46/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/foundation/process.py` & `phc-ingestion-0.3.46/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.46/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.46/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.46/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.46/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/nextgen/process.py` & `phc-ingestion-0.3.46/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.3.46/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.46/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.46/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.46/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.3.46/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.46/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.46/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.3.46/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.3.46/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.45/pyproject.toml` & `phc-ingestion-0.3.46/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.45"
+version = "0.3.46"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

