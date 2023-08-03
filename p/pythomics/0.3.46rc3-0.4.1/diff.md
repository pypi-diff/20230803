# Comparing `tmp/pythomics-0.3.46rc3.tar.gz` & `tmp/pythomics-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pythomics-0.3.46rc3.tar", last modified: Wed Aug 25 17:47:17 2021, max compression
+gzip compressed data, was "dist/pythomics-0.4.1.tar", last modified: Thu Aug  3 16:04:53 2023, max compression
```

## Comparing `pythomics-0.3.46rc3.tar` & `pythomics-0.4.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:17.000000 pythomics-0.3.46rc3/
--rw-r--r--   0 runner    (1001) docker     (121)    35121 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-08-25 17:47:17.000000 pythomics-0.3.46rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      667 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:17.000000 pythomics-0.3.46rc3/pythomics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:17.000000 pythomics-0.3.46rc3/pythomics/genomics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/genomics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/genomics/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    16430 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/genomics/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)    22067 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/genomics/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:17.000000 pythomics-0.3.46rc3/pythomics/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/parsers/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7522 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/parsers/fasta.py
--rw-r--r--   0 runner    (1001) docker     (121)      301 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/parsers/fastq.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:17.000000 pythomics-0.3.46rc3/pythomics/proteomics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/proteomics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5821 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/proteomics/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1878 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/proteomics/digest.py
--rw-r--r--   0 runner    (1001) docker     (121)   105205 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/proteomics/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/proteomics/peptide.py
--rw-r--r--   0 runner    (1001) docker     (121)     4847 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/proteomics/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:17.000000 pythomics-0.3.46rc3/pythomics/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     8846 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:17.000000 pythomics-0.3.46rc3/pythomics/transcriptomics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/transcriptomics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:17.000000 pythomics-0.3.46rc3/pythomics/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     2293 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/pythomics/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:17.000000 pythomics-0.3.46rc3/pythomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-08-25 17:47:16.000000 pythomics-0.3.46rc3/pythomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-08-25 17:47:16.000000 pythomics-0.3.46rc3/pythomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-25 17:47:16.000000 pythomics-0.3.46rc3/pythomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-25 17:47:16.000000 pythomics-0.3.46rc3/pythomics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-08-25 17:47:16.000000 pythomics-0.3.46rc3/pythomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-08-25 17:47:16.000000 pythomics-0.3.46rc3/pythomics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-25 17:47:17.000000 pythomics-0.3.46rc3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)    10453 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/scripts/fastadigest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6389 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/scripts/fastadigeststats.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7370 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/scripts/fastxTrimmer.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6452 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/scripts/featureCollapser.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3293 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/scripts/fetchOrfs.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8806 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/scripts/incorporateGFF.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3304 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/scripts/incorporateVCF.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5242 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/scripts/intersectFiles.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3150 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/scripts/junctionalReads.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    38475 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/scripts/proteinInference.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8776 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/scripts/ptmSummary.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2021-08-25 17:47:17.000000 pythomics-0.3.46rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      900 2021-08-25 17:47:09.000000 pythomics-0.3.46rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:53.000000 pythomics-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-08-03 16:04:39.000000 pythomics-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 16:04:39.000000 pythomics-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-03 16:04:53.000000 pythomics-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-03 16:04:39.000000 pythomics-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:53.000000 pythomics-0.4.1/pythomics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:53.000000 pythomics-0.4.1/pythomics/genomics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/genomics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/genomics/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/genomics/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22000 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/genomics/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:53.000000 pythomics-0.4.1/pythomics/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/parsers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/parsers/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/parsers/fastq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:53.000000 pythomics-0.4.1/pythomics/proteomics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/proteomics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/proteomics/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/proteomics/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105203 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/proteomics/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/proteomics/peptide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/proteomics/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:53.000000 pythomics-0.4.1/pythomics/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:53.000000 pythomics-0.4.1/pythomics/transcriptomics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/transcriptomics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:53.000000 pythomics-0.4.1/pythomics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-03 16:04:39.000000 pythomics-0.4.1/pythomics/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:53.000000 pythomics-0.4.1/pythomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-03 16:04:53.000000 pythomics-0.4.1/pythomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 16:04:53.000000 pythomics-0.4.1/pythomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:04:53.000000 pythomics-0.4.1/pythomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:04:53.000000 pythomics-0.4.1/pythomics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 16:04:53.000000 pythomics-0.4.1/pythomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 16:04:53.000000 pythomics-0.4.1/pythomics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:04:53.000000 pythomics-0.4.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10453 2023-08-03 16:04:39.000000 pythomics-0.4.1/scripts/fastadigest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6389 2023-08-03 16:04:39.000000 pythomics-0.4.1/scripts/fastadigeststats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7371 2023-08-03 16:04:39.000000 pythomics-0.4.1/scripts/fastxTrimmer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6452 2023-08-03 16:04:39.000000 pythomics-0.4.1/scripts/featureCollapser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-08-03 16:04:39.000000 pythomics-0.4.1/scripts/fetchOrfs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8806 2023-08-03 16:04:39.000000 pythomics-0.4.1/scripts/incorporateGFF.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3304 2023-08-03 16:04:39.000000 pythomics-0.4.1/scripts/incorporateVCF.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5242 2023-08-03 16:04:39.000000 pythomics-0.4.1/scripts/intersectFiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3150 2023-08-03 16:04:39.000000 pythomics-0.4.1/scripts/junctionalReads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38476 2023-08-03 16:04:39.000000 pythomics-0.4.1/scripts/proteinInference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8776 2023-08-03 16:04:39.000000 pythomics-0.4.1/scripts/ptmSummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-03 16:04:53.000000 pythomics-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 16:04:39.000000 pythomics-0.4.1/setup.py
```

### Comparing `pythomics-0.3.46rc3/LICENSE` & `pythomics-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/README.md` & `pythomics-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/pythomics/genomics/parsers.py` & `pythomics-0.4.1/pythomics/genomics/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,18 @@
             return self.vcf_file.individuals.keys()
         return self.vcf_file.get_individual(individual=individual)
 
 
 class VCFIterator(templates.GenericIterator, VCFMixin):
     def __init__(self, filename, sample=None):
         """An iterator over the VCF file format
-        
+
         This reads VCF files and has been tested on VCF 4.0.
         The returned items are VCFEntry
-        
+
         """
         super(VCFIterator, self).__init__(filename)
         # process our meta information
         row = six.next(self.handle).decode().strip()
         self.vcf_file = structure.VCFFile(filename)
         self.inum = 0
         while row[:2] == "##":
```

### Comparing `pythomics-0.3.46rc3/pythomics/genomics/structures.py` & `pythomics-0.4.1/pythomics/genomics/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 
 GENOTYPE_SPLIT = re.compile(r"[\|/]")
 
 
 class VCFFile(object):
     def __init__(self, filename):
         """VCF File container
-        
+
         This class is designed to be somewhat consistent with the C++
         implementation of vcftools. It contains our higher level
         information such as metadata, samples, the format field,
         and can contain entries as well. Thus it can serve as a
         simple iterator or an in-memory VCF instance for rapid queries.
-        
+
         """
         self.filename = filename
         self.meta = VCFMeta()
         self.n_individuals = 0
         self.individuals = OrderedDict()  # maps individual name to index
         self.entries = {}
 
@@ -77,17 +77,15 @@
         """
         var_call = VCFEntry(self.individuals)
         var_call.parse_entry(row)
         self.entries[(var_call.chrom, var_call.pos)] = var_call
         return var_call
 
     def get_header(self, individual=-1):
-        """Returns the vcf header
-
-        """
+        """Returns the vcf header"""
         type_map = dict([(val, key) for key, val in self.meta.type_map.iteritems()])
         extra = "\n".join(["##{0}".format(i) for i in self.meta.extra])
         info = "\n".join(
             [
                 "##INFO=<ID={0},Number={1},Type={2},Description={3}>".format(
                     key,
                     val.get("num_entries", "."),
@@ -136,27 +134,26 @@
                         if v == individual:
                             individual = i
                             break
             header += "\t" + individual
         return "\n".join([extra, info, filter, format, alt, header])
 
     def get_individual(self, individual=None):
-        """Returns the index of the individual
-        """
+        """Returns the index of the individual"""
 
         return self.individuals.get(individual, None)
 
 
 class VCFMeta(object):
     def __init__(self):
         """VCF Metainfo Container
-        
+
         This contains information in the metainfo of a VCF File
         such as the format fields, ids, and filters.
-    
+
         """
         self.info = OrderedDict()
         self.filter = OrderedDict()
         self.format = OrderedDict()
         self.alt = OrderedDict()
         self.extra = []
         self.type_map = {
@@ -297,17 +294,15 @@
         """Returns the VCF entry as it appears in the vcf file"""
         base = str(self)
         extra = self.get_sample_info(individual=individual)
         extra = [":".join([str(j) for j in i]) for i in zip(*extra.values())]
         return "\t".join([base, "\t".join(extra)])
 
     def get_sample_info(self, individual=-1):
-        """Returns the sample info of a given sample or all by default
-
-        """
+        """Returns the sample info of a given sample or all by default"""
         if isinstance(individual, str):
             individual = self.individuals[individual]
         extra = OrderedDict()
         for format_ in self.format:
             index = getattr(self, format_)
             if index != -1:
                 if format_ == "GT":
@@ -623,16 +618,14 @@
         """A dictionary of GFF features which are children of this feature
 
         :return: A dictionary of children GFF Features
         """
         return {} if not hasattr(self, "children") else self.children
 
     def parts(self):
-        """A generator consisting GFFObjects within this feature
-
-        """
+        """A generator consisting GFFObjects within this feature"""
         for i in self.features:
             yield i
 
     def __str__(self):
         rep = [str(i) for i in self.parts()]
         return "\n".join(rep)
```

### Comparing `pythomics-0.3.46rc3/pythomics/parsers/config.py` & `pythomics-0.4.1/pythomics/parsers/config.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/pythomics/parsers/fasta.py` & `pythomics-0.4.1/pythomics/parsers/fasta.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/pythomics/proteomics/config.py` & `pythomics-0.4.1/pythomics/proteomics/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,18 @@
     "S": ((-1 * MODIFICATION_MASSES["h2o"][0], ("b"), "-h2o"),),
     "T": ((-1 * MODIFICATION_MASSES["h2o"][0], ("b"), "-h2o"),),
     "D": ((-1 * MODIFICATION_MASSES["h2o"][0], ("b", "y"), "-h2o"),),
     "E": ((-1 * MODIFICATION_MASSES["h2o"][0], ("b", "y"), "-h2o"),),
 }
 
 LABEL_SCHEMES = {
-    "O18": {"O18": {4.008492: set(["]"])}, "O16": {0: set([])},},
+    "O18": {
+        "O18": {4.008492: set(["]"])},
+        "O16": {0: set([])},
+    },
     "N15": {
         "N15": {
             0.997035: set(["X"]),
             1.99407: set(["K", "Q", "N"]),
             2.991105: set(["H"]),
             3.98814: set(["R"]),
         },
```

### Comparing `pythomics-0.3.46rc3/pythomics/proteomics/digest.py` & `pythomics-0.4.1/pythomics/proteomics/digest.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/pythomics/proteomics/parsers.py` & `pythomics-0.4.1/pythomics/proteomics/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
     def build_index(self, file_obj):
         file_obj.seek(0)
         new_index = {}
         character_count = 0
         UNCONSUMED = ""
         while True:
-            i = UNCONSUMED + file_obj.read(2 ** 16)
+            i = UNCONSUMED + file_obj.read(2**16)
             UNCONSUMED = ""
             if i == "":
                 break
             while i:
                 start, end, tag = self.find_tags(i, "spectrum")
                 if start == -1:
                     start, end, tag = self.find_tags(i, "chromatogram")
```

### Comparing `pythomics-0.3.46rc3/pythomics/proteomics/peptide.py` & `pythomics-0.4.1/pythomics/proteomics/peptide.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/pythomics/proteomics/structures.py` & `pythomics-0.4.1/pythomics/proteomics/structures.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/pythomics/templates/__init__.py` & `pythomics-0.4.1/pythomics/templates/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,22 @@
 import six
 
 from ..proteomics import config as protein_config
 
 
 class GenericIterator(six.Iterator):
     gzip = False
-    CHUNK_SIZE = 2 ** 16
+    CHUNK_SIZE = 2**16
     UNCONSUMED = ""
     contents = []
 
     def __init__(self, filename, delimiter="\n", *args, **kwargs):
         self.delimiter = delimiter
         self.filename = filename
-        if (six.PY3 and isinstance(filename, IOBase)) or (
-            six.PY2 and isinstance(filename, file)
-        ):
+        if isinstance(filename, IOBase):
             self.filename = filename.name
             self._handle = filename
 
     @property
     def handle(self):
         handle = getattr(self, "_handle", None)
```

### Comparing `pythomics-0.3.46rc3/pythomics/utils/__init__.py` & `pythomics-0.4.1/pythomics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/pythomics.egg-info/SOURCES.txt` & `pythomics-0.4.1/pythomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/scripts/fastadigest.py` & `pythomics-0.4.1/scripts/fastadigest.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/scripts/fastadigeststats.py` & `pythomics-0.4.1/scripts/fastadigeststats.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/scripts/fastxTrimmer.py` & `pythomics-0.4.1/scripts/fastxTrimmer.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 global paired
 global read_min
 quality_min = 0
 quality_offset = 64
 paired = False
 read_min = 25
 
+
 # @profile
 def trim_read(entries):
     result = []
     for entry in entries:
         read_name, sequence = entry[:2]
         start_cut = start_trim.match(sequence)
         end_cut = end_trim.search(sequence)
```

### Comparing `pythomics-0.3.46rc3/scripts/featureCollapser.py` & `pythomics-0.4.1/scripts/featureCollapser.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/scripts/fetchOrfs.py` & `pythomics-0.4.1/scripts/fetchOrfs.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/scripts/incorporateGFF.py` & `pythomics-0.4.1/scripts/incorporateGFF.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/scripts/incorporateVCF.py` & `pythomics-0.4.1/scripts/incorporateVCF.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/scripts/intersectFiles.py` & `pythomics-0.4.1/scripts/intersectFiles.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/scripts/junctionalReads.py` & `pythomics-0.4.1/scripts/junctionalReads.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/scripts/proteinInference.py` & `pythomics-0.4.1/scripts/proteinInference.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,15 @@
     seen = set()
     return [x for x in l if x not in seen and not seen.add(x)]
     # return list(OrderedDict.fromkeys(l))
 
 
 # from profilestats import profile
 
+
 # @profile(print_stats=10, dump_stats=True)
 def mapper(peptides):
     # pep_format = r'(.+?)\t[^\n]+?({})'
     # pep_format = r'^([^\n]+)\t[^\n]+?({})'
     # matches = [{'peptide': i.group(2), 'peptide_start': i.start(2), 'accession': i.group(1)}
     #            for j in peptides
     #            for i in re.finditer(pep_format.format(j.upper().replace('L', '!').replace('!', '[IL]')), protein_sequences, re.M)]
```

### Comparing `pythomics-0.3.46rc3/scripts/ptmSummary.py` & `pythomics-0.4.1/scripts/ptmSummary.py`

 * *Files identical despite different names*

### Comparing `pythomics-0.3.46rc3/setup.cfg` & `pythomics-0.4.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.46rc3
+current_version = 0.4.1
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(rc(?P<rc>\d+))?
 serialize = 
 	{major}.{minor}.{patch}rc{rc}
 	{major}.{minor}.{patch}
 
@@ -15,13 +15,14 @@
 ignore = E111,E114,E121,E122,E124,E125,E126,E127,E128,E129,E131,E203,E231,E265,E501,E731,F841,W291,W293,W503,W504
 exclude = 
 	.git,
 	.tox,
 	__pycache__,
 	build,
 	dist,
+	scripts/*
 statistics = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pythomics-0.3.46rc3/setup.py` & `pythomics-0.4.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 from setuptools import find_packages, setup
 
 setup(
     name="pythomics",
-    version="0.3.46rc3",
+    version="0.4.1",
     description="A multi-omic python package",
     url="https://github.com/chris7/pythomics",
     author="Chris Mitchell",
     author_email="chris.mit7@gmail.com",
-    install_requires=["lxml", "six",],
-    extras_require={"all": ["matplotlib", "pandas", "pysam", "scipy",],},
+    install_requires=[
+        "lxml",
+        "six",
+    ],
+    extras_require={
+        "all": [
+            "matplotlib",
+            "pandas",
+            "pysam",
+            "scipy",
+        ],
+    },
     license="GPL3",
     packages=find_packages(),
     scripts=[
         "scripts/fastadigest.py",
         "scripts/fastadigeststats.py",
         "scripts/incorporateVCF.py",
         "scripts/fetchOrfs.py",
```

