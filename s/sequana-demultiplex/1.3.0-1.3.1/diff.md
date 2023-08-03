# Comparing `tmp/sequana_demultiplex-1.3.0.tar.gz` & `tmp/sequana_demultiplex-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_demultiplex-1.3.0.tar", last modified: Wed May 17 12:04:29 2023, max compression
+gzip compressed data, was "dist/sequana_demultiplex-1.3.1.tar", last modified: Thu Aug  3 13:00:18 2023, max compression
```

## Comparing `sequana_demultiplex-1.3.0.tar` & `sequana_demultiplex-1.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    12131 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9282 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    12131 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      745 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    17354 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/dag.png
--rw-r--r--   0 runner    (1001) docker     (122)     7372 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/demultiplex.rules
--rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/logo.png
--rwxr-xr-x   0 runner    (1001) docker     (122)     8427 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/main.py
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:04:29.000000 sequana_demultiplex-1.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/test/test_check_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-17 12:04:26.000000 sequana_demultiplex-1.3.0/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:00:18.000000 sequana_demultiplex-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-08-03 13:00:13.000000 sequana_demultiplex-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    12199 2023-08-03 13:00:18.000000 sequana_demultiplex-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9342 2023-08-03 13:00:13.000000 sequana_demultiplex-1.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-08-03 13:00:13.000000 sequana_demultiplex-1.3.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:00:18.000000 sequana_demultiplex-1.3.1/sequana_demultiplex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    12199 2023-08-03 13:00:18.000000 sequana_demultiplex-1.3.1/sequana_demultiplex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      745 2023-08-03 13:00:18.000000 sequana_demultiplex-1.3.1/sequana_demultiplex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 13:00:18.000000 sequana_demultiplex-1.3.1/sequana_demultiplex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-08-03 13:00:18.000000 sequana_demultiplex-1.3.1/sequana_demultiplex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 13:00:18.000000 sequana_demultiplex-1.3.1/sequana_demultiplex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-08-03 13:00:18.000000 sequana_demultiplex-1.3.1/sequana_demultiplex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-08-03 13:00:18.000000 sequana_demultiplex-1.3.1/sequana_demultiplex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:00:18.000000 sequana_demultiplex-1.3.1/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:00:18.000000 sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-08-03 13:00:13.000000 sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-08-03 13:00:13.000000 sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    17354 2023-08-03 13:00:13.000000 sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/dag.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7453 2023-08-03 13:00:13.000000 sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/demultiplex.rules
+-rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-08-03 13:00:13.000000 sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/logo.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8427 2023-08-03 13:00:13.000000 sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-08-03 13:00:13.000000 sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-08-03 13:00:13.000000 sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-08-03 13:00:18.000000 sequana_demultiplex-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-08-03 13:00:13.000000 sequana_demultiplex-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:00:18.000000 sequana_demultiplex-1.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-08-03 13:00:13.000000 sequana_demultiplex-1.3.1/test/test_check_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-08-03 13:00:13.000000 sequana_demultiplex-1.3.1/test/test_main.py
```

### Comparing `sequana_demultiplex-1.3.0/PKG-INFO` & `sequana_demultiplex-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sequana_demultiplex
-Version: 1.3.0
+Version: 1.3.1
 Summary: Pipeline that runs bcl2fastq and creates additional plots within a Snakemake workflow
 Home-page: https://github.com/sequana/
 Author: cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -122,14 +122,15 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= =======================================================================
         Version   Description
         ========= =======================================================================
+        1.3.1     * use sequana_wrappers version in the config file
         1.3.0     * use latest sequana-wrappers to benefit and graphivz apptainer
         1.2.1     * Update CI action and use new sequana_pipetools v0.9.0
         1.2.0     * stable release with cleanup of the setup and README
         1.1.3     * add the --mars-seq option that fills the config automatically
         1.1.2     * fix the none_and_force merging strategy option
         1.1.1     * fix a regression bug
         1.1.0     * Uses new sequana-wrappers repository
```

### Comparing `sequana_demultiplex-1.3.0/README.rst` & `sequana_demultiplex-1.3.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 
 Changelog
 ~~~~~~~~~
 
 ========= =======================================================================
 Version   Description
 ========= =======================================================================
+1.3.1     * use sequana_wrappers version in the config file
 1.3.0     * use latest sequana-wrappers to benefit and graphivz apptainer
 1.2.1     * Update CI action and use new sequana_pipetools v0.9.0
 1.2.0     * stable release with cleanup of the setup and README
 1.1.3     * add the --mars-seq option that fills the config automatically
 1.1.2     * fix the none_and_force merging strategy option
 1.1.1     * fix a regression bug
 1.1.0     * Uses new sequana-wrappers repository
```

### Comparing `sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/PKG-INFO` & `sequana_demultiplex-1.3.1/sequana_demultiplex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sequana-demultiplex
-Version: 1.3.0
+Version: 1.3.1
 Summary: Pipeline that runs bcl2fastq and creates additional plots within a Snakemake workflow
 Home-page: https://github.com/sequana/
 Author: cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -122,14 +122,15 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= =======================================================================
         Version   Description
         ========= =======================================================================
+        1.3.1     * use sequana_wrappers version in the config file
         1.3.0     * use latest sequana-wrappers to benefit and graphivz apptainer
         1.2.1     * Update CI action and use new sequana_pipetools v0.9.0
         1.2.0     * stable release with cleanup of the setup and README
         1.1.3     * add the --mars-seq option that fills the config automatically
         1.1.2     * fix the none_and_force merging strategy option
         1.1.1     * fix a regression bug
         1.1.0     * Uses new sequana-wrappers repository
```

### Comparing `sequana_demultiplex-1.3.0/sequana_demultiplex.egg-info/SOURCES.txt` & `sequana_demultiplex-1.3.1/sequana_demultiplex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/config.yaml` & `sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #  The full license is in the LICENSE file, distributed with this software.
 #
 #  website: https://github.com/sequana/sequana
 #  documentation: http://sequana.readthedocs.io
 #
 ##############################################################################
 
-
+sequana_wrappers: "v0.15.1"
 
 #################################################################
 # bcl2fastq
 #
 # :Parameters:
 #
 #   intensities are expected to be found in input_directory/Data/Intensities
```

### Comparing `sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/dag.png` & `sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/dag.png`

 * *Files identical despite different names*

### Comparing `sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/demultiplex.rules` & `sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/demultiplex.rules`

 * *Files 3% similar despite different names*

```diff
@@ -29,20 +29,22 @@
 
 # do not overwrite the snakemake logger !
 from sequana import logger as log
 
 # This must be defined before the include
 configfile: "config.yaml"
 
-sequana_wrapper_branch = "main"
 
 
 # A convenient manager
 manager = PipelineManagerDirectory("demultiplex", config)
 
+# should be part of PipelineManagerDirectory
+manager.wrappers = config.get("sequana_wrappers", "main")
+
 
 samplesheet = config['bcl2fastq']['samplesheet_file'].strip()
 
 
 if samplesheet.strip() != "":
     if os.path.exists(samplesheet) is False:
         log.error(f"Sample sheet {samplesheet} does not exist")
@@ -116,15 +118,15 @@
         no_bgzf_compression=config['bcl2fastq']['no_bgzf_compression'],
         merge_all_lanes=config['bcl2fastq']['merge_all_lanes'],
         options=config['bcl2fastq']['options']
     threads: config['bcl2fastq']['threads']
     resources:
        **config['bcl2fastq']['resources']
     wrapper:
-        "main/wrappers/bcl2fastq"
+        f"{manager.wrappers}/wrappers/bcl2fastq"
 
 
 rule plot_barplot_samples:
     input:  "Stats/Stats.json"
     output:
         barplot="samples.png"
     run:
@@ -151,15 +153,15 @@
         workflow.snakefile
     output:
         "rulegraph/rulegraph.dot"
     params:
         mapper = {},
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

### Comparing `sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/logo.png` & `sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/logo.png`

 * *Files identical despite different names*

### Comparing `sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/main.py` & `sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/main.py`

 * *Files identical despite different names*

### Comparing `sequana_demultiplex-1.3.0/sequana_pipelines/demultiplex/schema.yaml` & `sequana_demultiplex-1.3.1/sequana_pipelines/demultiplex/schema.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,18 @@
   "general":
       type: map
       mapping:
           "input_directory":
              type: str
              required: False
 
+  "apptainers":
+        type: any
+
+
   "bcl2fastq":
         type: map
         mapping:
             "threads":
                 type: int
             "barcode_mismatch": 
                 type: int
```

### Comparing `sequana_demultiplex-1.3.0/setup.py` & `sequana_demultiplex-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_namespace_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 
 _MAJOR               = 1
 _MINOR               = 3
-_MICRO               = 0
+_MICRO               = 1
 version              = '%d.%d.%d' % (_MAJOR, _MINOR, _MICRO)
 release              = '%d.%d' % (_MAJOR, _MINOR)
 
 metainfo = {
     'authors': {"main": ("cokelaer", "thomas.cokelaer@pasteur.fr")},
     'version': version,
     'license' : 'new BSD',
```

### Comparing `sequana_demultiplex-1.3.0/test/test_check_samplesheet.py` & `sequana_demultiplex-1.3.1/test/test_check_samplesheet.py`

 * *Files identical despite different names*

### Comparing `sequana_demultiplex-1.3.0/test/test_main.py` & `sequana_demultiplex-1.3.1/test/test_main.py`

 * *Files identical despite different names*

