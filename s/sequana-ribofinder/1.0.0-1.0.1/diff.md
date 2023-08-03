# Comparing `tmp/sequana_ribofinder-1.0.0.tar.gz` & `tmp/sequana_ribofinder-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_ribofinder-1.0.0.tar", last modified: Mon May 22 14:22:12 2023, max compression
+gzip compressed data, was "dist/sequana_ribofinder-1.0.1.tar", last modified: Thu Aug  3 12:57:11 2023, max compression
```

## Comparing `sequana_ribofinder-1.0.0.tar` & `sequana_ribofinder-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:22:12.000000 sequana_ribofinder-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6890 2023-05-22 14:22:12.000000 sequana_ribofinder-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4626 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:22:12.000000 sequana_ribofinder-1.0.0/sequana_pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:22:12.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3128 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    20253 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/dag.png
--rwxr-xr-x   0 runner    (1001) docker     (122)     5506 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4586 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/multiqc_config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)    12017 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/ribofinder.rules
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:22:12.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6890 2023-05-22 14:22:11.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-22 14:22:11.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 14:22:11.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-22 14:22:11.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 14:22:11.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-22 14:22:11.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-22 14:22:11.000000 sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-05-22 14:22:12.000000 sequana_ribofinder-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:22:12.000000 sequana_ribofinder-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)     1797 2023-05-22 14:22:07.000000 sequana_ribofinder-1.0.0/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:57:11.000000 sequana_ribofinder-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-08-03 12:57:03.000000 sequana_ribofinder-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6954 2023-08-03 12:57:11.000000 sequana_ribofinder-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4682 2023-08-03 12:57:03.000000 sequana_ribofinder-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-08-03 12:57:03.000000 sequana_ribofinder-1.0.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:57:11.000000 sequana_ribofinder-1.0.1/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:57:11.000000 sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-08-03 12:57:03.000000 sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-08-03 12:57:03.000000 sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    20253 2023-08-03 12:57:03.000000 sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/dag.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5506 2023-08-03 12:57:03.000000 sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4586 2023-08-03 12:57:03.000000 sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/multiqc_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-08-03 12:57:03.000000 sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    11913 2023-08-03 12:57:03.000000 sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/ribofinder.rules
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-08-03 12:57:03.000000 sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:57:11.000000 sequana_ribofinder-1.0.1/sequana_ribofinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6954 2023-08-03 12:57:10.000000 sequana_ribofinder-1.0.1/sequana_ribofinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-08-03 12:57:11.000000 sequana_ribofinder-1.0.1/sequana_ribofinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 12:57:10.000000 sequana_ribofinder-1.0.1/sequana_ribofinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-08-03 12:57:10.000000 sequana_ribofinder-1.0.1/sequana_ribofinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 12:57:10.000000 sequana_ribofinder-1.0.1/sequana_ribofinder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-08-03 12:57:10.000000 sequana_ribofinder-1.0.1/sequana_ribofinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-08-03 12:57:10.000000 sequana_ribofinder-1.0.1/sequana_ribofinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-08-03 12:57:11.000000 sequana_ribofinder-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-08-03 12:57:03.000000 sequana_ribofinder-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:57:11.000000 sequana_ribofinder-1.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     1797 2023-08-03 12:57:03.000000 sequana_ribofinder-1.0.1/test/test_main.py
```

### Comparing `sequana_ribofinder-1.0.0/PKG-INFO` & `sequana_ribofinder-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sequana_ribofinder
-Version: 1.0.0
+Version: 1.0.1
 Summary: NGS, ribosomal, rRNA, snakemake, sequana
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -115,14 +115,15 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
+        1.0.1     * add sequana_wrappers in the config/pipeline
         1.0.0     * use graphviz apptainer and latest wrappers
         0.13.0    * add  final apptainers and update CI actions
         0.12.0    * set singularity containers
         0.11.1    * Fix config file (removing hard-coded path)
         0.11.0    * Fix multiqc plot using same fix as in sequna_rnaseq pipelines
                   * add utility plot to check rate of  ribosomal per sequence and also
                     the corresponding  RPKM.
```

### Comparing `sequana_ribofinder-1.0.0/README.rst` & `sequana_ribofinder-1.0.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 
 Changelog
 ~~~~~~~~~
 
 ========= ====================================================================
 Version   Description
 ========= ====================================================================
+1.0.1     * add sequana_wrappers in the config/pipeline
 1.0.0     * use graphviz apptainer and latest wrappers
 0.13.0    * add  final apptainers and update CI actions
 0.12.0    * set singularity containers
 0.11.1    * Fix config file (removing hard-coded path)
 0.11.0    * Fix multiqc plot using same fix as in sequna_rnaseq pipelines
           * add utility plot to check rate of  ribosomal per sequence and also
             the corresponding  RPKM.
```

### Comparing `sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/config.yaml` & `sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 # ==================[ Sections for the users ]================================
 #
 # One of input_directory, input_pattern and input_samples must be provided
 # If input_directory provided, use it otherwise if input_pattern provided,
 # use it, otherwise use input_samples.
 # ============================================================================
+sequana_wrappers: "v0.15.1"
 input_directory:
 input_readtag: _R[12]_
 input_pattern: '*fastq.gz'
 # =========================================== Sections for the users
 
 #############################################################################
 # Genome section:
```

### Comparing `sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/dag.png` & `sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/dag.png`

 * *Files identical despite different names*

### Comparing `sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/main.py` & `sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/main.py`

 * *Files identical despite different names*

### Comparing `sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/multiqc_config.yaml` & `sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/multiqc_config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/ribofinder.rules` & `sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/ribofinder.rules`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,20 @@
 """Ribofinder pipeline"""
 import shutil
 import os
 from collections import Counter
 
 
 from sequana_pipetools import PipelineManager
-from sequana_pipetools import snaketools as sm
-from sequana import logger as log
-
 from sequana.gff3 import GFF3
+from sequana import logger as log
 
 configfile: "config.yaml"
 
 manager = PipelineManager("ribofinder", config)
-sequana_wrapper_branch = "main"
 
 
 rule pipeline:
     input:
         ".sequana/rulegraph.svg",
         "outputs/proportions.png",
         "outputs/RPKM.png",
@@ -131,15 +128,15 @@
     params:
         options=""
     threads:
         2
     container:
         config['apptainers']['sequana_ribofinder']
     wrapper:
-        f"{sequana_wrapper_branch}/wrappers/bowtie1/build"
+        f"{manager.wrappers}/wrappers/bowtie1/build"
 
 
 
 """With paired data, alignement on rRNA leads to 0% alignment if we use R1 and
 R2. If we use R1 only, the percentage is >0. First reason is that reads are not
 trimmed properly. In truth, bowtie2 supports local alignments which means it can
 soft-clip non-matching (=adapter) content while still align the local part of
@@ -173,15 +170,15 @@
     params:
         options=""
     threads:
         config['bowtie1_mapping_rna']['threads']
     container:
         config['apptainers']['sequana_ribofinder']
     wrapper:
-        f"{sequana_wrapper_branch}/wrappers/bowtie1/align"
+        f"{manager.wrappers}/wrappers/bowtie1/align"
 
 
 # ======================================================== Fix bowtie log
 # This fix_bowtie1_log is used to fix a bug in multiqc showing 0% match in all samples.
 # Note: same rule as in rnaseq pipeline.
 rule fix_bowtie1_log:
     input:
@@ -288,27 +285,27 @@
         options=config['multiqc']['options'],
         input_directory=config['multiqc']['input_directory'],
         config_file=config['multiqc']['config_file'],
         modules=config['multiqc']['modules']
     log:
         "multiqc/multiqc.log"
     wrapper:
-       f"{sequana_wrapper_branch}/wrappers/multiqc"
+       f"{manager.wrappers}/wrappers/multiqc"
 
 
 # ========================================================== rulegraph
 rule rulegraph:
     input: str(manager.snakefile)
     output:
         svg = "rulegraph/rulegraph.dot"
     params:
         mapper = {"multiqc": "../multiqc/multiqc_report.html"},
         configname = "config.yaml"
     wrapper:
-        f"{sequana_wrapper_branch}/wrappers/rulegraph"
+        f"{manager.wrappers}/wrappers/rulegraph"
 
 
 rule dot2svg:
     input:
         "rulegraph/rulegraph.dot"
     output:
         ".sequana/rulegraph.svg"
```

### Comparing `sequana_ribofinder-1.0.0/sequana_pipelines/ribofinder/schema.yaml` & `sequana_ribofinder-1.0.1/sequana_pipelines/ribofinder/schema.yaml`

 * *Files identical despite different names*

### Comparing `sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/PKG-INFO` & `sequana_ribofinder-1.0.1/sequana_ribofinder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sequana-ribofinder
-Version: 1.0.0
+Version: 1.0.1
 Summary: NGS, ribosomal, rRNA, snakemake, sequana
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -115,14 +115,15 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
+        1.0.1     * add sequana_wrappers in the config/pipeline
         1.0.0     * use graphviz apptainer and latest wrappers
         0.13.0    * add  final apptainers and update CI actions
         0.12.0    * set singularity containers
         0.11.1    * Fix config file (removing hard-coded path)
         0.11.0    * Fix multiqc plot using same fix as in sequna_rnaseq pipelines
                   * add utility plot to check rate of  ribosomal per sequence and also
                     the corresponding  RPKM.
```

### Comparing `sequana_ribofinder-1.0.0/sequana_ribofinder.egg-info/SOURCES.txt` & `sequana_ribofinder-1.0.1/sequana_ribofinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sequana_ribofinder-1.0.0/setup.py` & `sequana_ribofinder-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_namespace_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 import subprocess
 
 _MAJOR               = 1
 _MINOR               = 0
-_MICRO               = 0
+_MICRO               = 1
 version              = '%d.%d.%d' % (_MAJOR, _MINOR, _MICRO)
 release              = '%d.%d' % (_MAJOR, _MINOR)
 
 metainfo = {
     'authors': {"main": ("thomas cokelaer", "thomas.cokelaer@pasteur.fr")},
     'version': version,
     'license' : 'new BSD',
```

### Comparing `sequana_ribofinder-1.0.0/test/test_main.py` & `sequana_ribofinder-1.0.1/test/test_main.py`

 * *Files identical despite different names*

