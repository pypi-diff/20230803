# Comparing `tmp/dataverse_utils-0.8.7.tar.gz` & `tmp/dataverse_utils-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse_utils-0.8.7.tar", last modified: Thu May 11 17:29:21 2023, max compression
+gzip compressed data, was "dataverse_utils-0.9.1.tar", last modified: Thu Aug  3 21:31:42 2023, max compression
```

## Comparing `dataverse_utils-0.8.7.tar` & `dataverse_utils-0.9.1.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.888426 dataverse_utils-0.8.7/
--rw-r--r--   0 paul       (501) staff       (20)      144 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/.gitignore
--rw-r--r--   0 paul       (501) staff       (20)     1103 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/LICENCE.md
--rw-r--r--   0 paul       (501) staff       (20)     2052 2023-05-11 17:29:21.887614 dataverse_utils-0.8.7/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)     1163 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/README.md
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.853564 dataverse_utils-0.8.7/docs/
--rw-r--r--   0 paul       (501) staff       (20)    10917 2022-04-26 15:29:23.000000 dataverse_utils-0.8.7/docs/api_ref.md
--rw-r--r--   0 paul       (501) staff       (20)      383 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/docs/credits.md
--rw-r--r--   0 paul       (501) staff       (20)     2932 2021-08-09 17:51:55.000000 dataverse_utils-0.8.7/docs/faq.md
--rw-r--r--   0 paul       (501) staff       (20)     5840 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/docs/index.md
--rw-r--r--   0 paul       (501) staff       (20)    18831 2023-05-11 15:44:20.000000 dataverse_utils-0.8.7/docs/scripts.md
--rw-r--r--   0 paul       (501) staff       (20)     5748 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/docs/windows.md
--rw-r--r--   0 paul       (501) staff       (20)      396 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/mkdocs.yml
--rw-r--r--   0 paul       (501) staff       (20)     2536 2023-05-11 15:42:55.000000 dataverse_utils-0.8.7/pyproject.toml
--rw-r--r--   0 paul       (501) staff       (20)      240 2023-05-11 15:55:17.000000 dataverse_utils-0.8.7/requirements.txt
--rw-r--r--   0 paul       (501) staff       (20)       38 2023-05-11 17:29:21.888603 dataverse_utils-0.8.7/setup.cfg
--rw-r--r--   0 paul       (501) staff       (20)       84 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/setup.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.841640 dataverse_utils-0.8.7/src/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.856538 dataverse_utils-0.8.7/src/dataverse_utils/
--rw-r--r--   0 paul       (501) staff       (20)      155 2023-05-11 15:54:33.000000 dataverse_utils-0.8.7/src/dataverse_utils/__init__.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.872144 dataverse_utils-0.8.7/src/dataverse_utils/data/
--rw-r--r--   0 paul       (501) staff       (20)     1545 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/data/LDC_EULA_general.md
--rw-r--r--   0 paul       (501) staff       (20)    17269 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/dataverse_utils.py
--rw-r--r--   0 paul       (501) staff       (20)    16047 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/ldc.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.881112 dataverse_utils-0.8.7/src/dataverse_utils/scripts/
--rw-r--r--   0 paul       (501) staff       (20)     4965 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_del.py
--rw-r--r--   0 paul       (501) staff       (20)     5348 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_ldc_uploader.py
--rw-r--r--   0 paul       (501) staff       (20)     5366 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_manifest_gen.py
--rw-r--r--   0 paul       (501) staff       (20)     9076 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_pg_facet_date.py
--rw-r--r--   0 paul       (501) staff       (20)     4349 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_record_copy.py
--rw-r--r--   0 paul       (501) staff       (20)     8071 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_release.py
--rw-r--r--   0 paul       (501) staff       (20)     4566 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_replace_licence.py
--rw-r--r--   0 paul       (501) staff       (20)     2975 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_upload_tsv.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.871100 dataverse_utils-0.8.7/src/dataverse_utils.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)     2052 2023-05-11 17:29:21.000000 dataverse_utils-0.8.7/src/dataverse_utils.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)     1022 2023-05-11 17:29:21.000000 dataverse_utils-0.8.7/src/dataverse_utils.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2023-05-11 17:29:21.000000 dataverse_utils-0.8.7/src/dataverse_utils.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)      574 2023-05-11 17:29:21.000000 dataverse_utils-0.8.7/src/dataverse_utils.egg-info/entry_points.txt
--rw-r--r--   0 paul       (501) staff       (20)      266 2023-05-11 17:29:21.000000 dataverse_utils-0.8.7/src/dataverse_utils.egg-info/requires.txt
--rw-r--r--   0 paul       (501) staff       (20)       16 2023-05-11 17:29:21.000000 dataverse_utils-0.8.7/src/dataverse_utils.egg-info/top_level.txt
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.882809 dataverse_utils-0.8.7/tests/
--rw-r--r--   0 paul       (501) staff       (20)        0 2021-08-09 17:51:55.000000 dataverse_utils-0.8.7/tests/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)     1124 2021-08-09 17:51:55.000000 dataverse_utils-0.8.7/tests/tests_dataverse_utils.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-11 17:29:21.886306 dataverse_utils-0.8.7/tmp/
--rw-r--r--   0 paul       (501) staff       (20)      324 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/tmp/requirements.txt
--rw-r--r--   0 paul       (501) staff       (20)     2493 2023-05-04 22:06:51.000000 dataverse_utils-0.8.7/tmp/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.118495 dataverse_utils-0.9.1/
+-rw-r--r--   0 paul       (501) staff       (20)      144 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/.gitignore
+-rw-r--r--   0 paul       (501) staff       (20)     1103 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/LICENCE.md
+-rw-r--r--   0 paul       (501) staff       (20)     2052 2023-08-03 21:31:42.117746 dataverse_utils-0.9.1/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)     1163 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/README.md
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.087225 dataverse_utils-0.9.1/docs/
+-rw-r--r--   0 paul       (501) staff       (20)    13561 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/docs/api_ref.md
+-rw-r--r--   0 paul       (501) staff       (20)      383 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/docs/credits.md
+-rw-r--r--   0 paul       (501) staff       (20)     2932 2021-08-09 17:51:55.000000 dataverse_utils-0.9.1/docs/faq.md
+-rw-r--r--   0 paul       (501) staff       (20)     5840 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/docs/index.md
+-rw-r--r--   0 paul       (501) staff       (20)    21852 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/docs/scripts.md
+-rw-r--r--   0 paul       (501) staff       (20)     5748 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/docs/windows.md
+-rw-r--r--   0 paul       (501) staff       (20)      396 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/mkdocs.yml
+-rw-r--r--   0 paul       (501) staff       (20)     2605 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/pyproject.toml
+-rw-r--r--   0 paul       (501) staff       (20)      240 2023-05-11 15:55:17.000000 dataverse_utils-0.9.1/requirements.txt
+-rw-r--r--   0 paul       (501) staff       (20)       38 2023-08-03 21:31:42.118665 dataverse_utils-0.9.1/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)       84 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.072110 dataverse_utils-0.9.1/src/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.092537 dataverse_utils-0.9.1/src/dataverse_utils/
+-rw-r--r--   0 paul       (501) staff       (20)      253 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/src/dataverse_utils/__init__.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.099070 dataverse_utils-0.9.1/src/dataverse_utils/data/
+-rw-r--r--   0 paul       (501) staff       (20)     1545 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/data/LDC_EULA_general.md
+-rw-r--r--   0 paul       (501) staff       (20)    17617 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/src/dataverse_utils/dataverse_utils.py
+-rw-r--r--   0 paul       (501) staff       (20)     7704 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/src/dataverse_utils/dvdata.py
+-rw-r--r--   0 paul       (501) staff       (20)    16047 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/ldc.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.109862 dataverse_utils-0.9.1/src/dataverse_utils/scripts/
+-rw-r--r--   0 paul       (501) staff       (20)     4965 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_del.py
+-rw-r--r--   0 paul       (501) staff       (20)     5348 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_ldc_uploader.py
+-rw-r--r--   0 paul       (501) staff       (20)     5366 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_manifest_gen.py
+-rw-r--r--   0 paul       (501) staff       (20)     9076 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_pg_facet_date.py
+-rw-r--r--   0 paul       (501) staff       (20)     4385 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_record_copy.py
+-rw-r--r--   0 paul       (501) staff       (20)     8071 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_release.py
+-rw-r--r--   0 paul       (501) staff       (20)     4566 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_replace_licence.py
+-rw-r--r--   0 paul       (501) staff       (20)     8782 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_study_migrator.py
+-rw-r--r--   0 paul       (501) staff       (20)     2975 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_upload_tsv.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.098008 dataverse_utils-0.9.1/src/dataverse_utils.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)     2052 2023-08-03 21:31:41.000000 dataverse_utils-0.9.1/src/dataverse_utils.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)     1101 2023-08-03 21:31:42.000000 dataverse_utils-0.9.1/src/dataverse_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-08-03 21:31:41.000000 dataverse_utils-0.9.1/src/dataverse_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)      641 2023-08-03 21:31:42.000000 dataverse_utils-0.9.1/src/dataverse_utils.egg-info/entry_points.txt
+-rw-r--r--   0 paul       (501) staff       (20)      266 2023-08-03 21:31:42.000000 dataverse_utils-0.9.1/src/dataverse_utils.egg-info/requires.txt
+-rw-r--r--   0 paul       (501) staff       (20)       16 2023-08-03 21:31:42.000000 dataverse_utils-0.9.1/src/dataverse_utils.egg-info/top_level.txt
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.111752 dataverse_utils-0.9.1/tests/
+-rw-r--r--   0 paul       (501) staff       (20)        0 2021-08-09 17:51:55.000000 dataverse_utils-0.9.1/tests/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)     1124 2021-08-09 17:51:55.000000 dataverse_utils-0.9.1/tests/tests_dataverse_utils.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.116236 dataverse_utils-0.9.1/tmp/
+-rw-r--r--   0 paul       (501) staff       (20)      324 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/tmp/requirements.txt
+-rw-r--r--   0 paul       (501) staff       (20)     2493 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/tmp/setup.py
```

### Comparing `dataverse_utils-0.8.7/LICENCE.md` & `dataverse_utils-0.9.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/PKG-INFO` & `dataverse_utils-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse_utils
-Version: 0.8.7
+Version: 0.9.1
 Summary: Utilities for the Dataverse data respository system
 Author-email: Paul Lesack <paul.lesack@ubc.ca>
 Project-URL: Homepage, https://ubc-library-rc.github.io/dataverse_utils
 Project-URL: Repository, https://github.com/ubc-library-rc/dataverse_utils.git
 Project-URL: Issue Tracker, https://github.com/ubc-library-rc/dataverse_utils/issues
 Keywords: Harvard Dataverse,Dataverse,research data management,data repository
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dataverse_utils-0.8.7/README.md` & `dataverse_utils-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/docs/api_ref.md` & `dataverse_utils-0.9.1/docs/api_ref.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 # API Reference
 
-<a name="dataverse_utils"></a>
+<a id="dataverse_utils"></a>
 
 ## dataverse\_utils
 
-Generalized dataverse utilities
+Generalized dataverse utilities. Note that
+`import dataverse_utils` is the equivalent of
+`import dataverse_utils.dataverse_utils`
 
-<a name="dataverse_utils.dataverse_utils"></a>
+<a id="dataverse_utils.dataverse_utils"></a>
 
 ## dataverse\_utils.dataverse\_utils
 
 A collection of Dataverse utilities for file and metadata
 manipulation
 
-<a name="dataverse_utils.dataverse_utils.DvGeneralUploadError"></a>
+<a id="dataverse_utils.dataverse_utils.DvGeneralUploadError"></a>
 
 ### DvGeneralUploadError Objects
 
 ```python
 class DvGeneralUploadError(Exception)
 ```
 
 Raised on non-200 URL response
 
-<a name="dataverse_utils.dataverse_utils.Md5Error"></a>
+<a id="dataverse_utils.dataverse_utils.Md5Error"></a>
 
 ### Md5Error Objects
 
 ```python
 class Md5Error(Exception)
 ```
 
 Raised on md5 mismatch
 
-<a name="dataverse_utils.dataverse_utils.make_tsv"></a>
+<a id="dataverse_utils.dataverse_utils.make_tsv"></a>
 
 ##### make\_tsv
 
 ```python
-make_tsv(start_dir, in_list=None, def_tag='Data', inc_header=True, mime=False, quotype=csv.QUOTE_MINIMAL) -> str
+def make_tsv(start_dir,
+             in_list=None,
+             def_tag='Data',
+             inc_header=True,
+             mime=False,
+             quotype=csv.QUOTE_MINIMAL) -> str
 ```
 
 Recurses the tree for files and produces tsv output with
 with headers 'file', 'description', 'tags'.
 
 The 'description' is the filename without an extension.
 
@@ -75,20 +82,20 @@
   Default = csv.QUOTE_MINIMAL
   Acceptable values:
   csv.QUOTE_MINIMAL / 0
   csv.QUOTE_ALL / 1
   csv.QUOTE_NONNUMERIC / 2
   csv.QUOTE_NONE / 3
 
-<a name="dataverse_utils.dataverse_utils.dump_tsv"></a>
+<a id="dataverse_utils.dataverse_utils.dump_tsv"></a>
 
 ##### dump\_tsv
 
 ```python
-dump_tsv(start_dir, filename, in_list=None, **kwargs)
+def dump_tsv(start_dir, filename, in_list=None, **kwargs)
 ```
 
 Dumps output of make_tsv manifest to a file.
 
 ------------------------------------------
 
 **Arguments**:
@@ -118,20 +125,20 @@
   Default : csv.QUOTE_MINIMAL
   Acceptable values:
   csv.QUOTE_MINIMAL / 0
   csv.QUOTE_ALL / 1
   csv.QUOTE_NONNUMERIC / 2
   csv.QUOTE_NONE / 3
 
-<a name="dataverse_utils.dataverse_utils.file_path"></a>
+<a id="dataverse_utils.dataverse_utils.file_path"></a>
 
 ##### file\_path
 
 ```python
-file_path(fpath, trunc='') -> str
+def file_path(fpath, trunc='') -> str
 ```
 
 Create relative file path from full path string
 
 >>> file_path('/tmp/Data/2011/excelfile.xlsx', '/tmp/')
 'Data/2011'
 >>> file_path('/tmp/Data/2011/excelfile.xlsx', '/tmp')
@@ -144,20 +151,20 @@
   
   fpath : str
   File location (ie, complete path)
   
   trunc : str
   Leftmost portion of path to remove
 
-<a name="dataverse_utils.dataverse_utils.check_lock"></a>
+<a id="dataverse_utils.dataverse_utils.check_lock"></a>
 
 ##### check\_lock
 
 ```python
-check_lock(dv_url, study, apikey) -> bool
+def check_lock(dv_url, study, apikey) -> bool
 ```
 
 Checks study lock status; returns True if locked.
 
 ----------------------------------------
 
 **Arguments**:
@@ -168,20 +175,20 @@
   
 - `study` - str
   Persistent ID of study
   
   apikey : str
   API key for user
 
-<a name="dataverse_utils.dataverse_utils.force_notab_unlock"></a>
+<a id="dataverse_utils.dataverse_utils.force_notab_unlock"></a>
 
 ##### force\_notab\_unlock
 
 ```python
-force_notab_unlock(study, dv_url, fid, apikey, try_uningest=True) -> int
+def force_notab_unlock(study, dv_url, fid, apikey, try_uningest=True) -> int
 ```
 
 Forcibly unlocks and uningests
 to prevent tabular file processing. Required if mime and filename
 spoofing is not sufficient.
 
 Returns 0 if unlocked, file id if locked (and then unlocked).
@@ -203,20 +210,20 @@
   apikey : str
   API key for user
   
   try_uningest : bool
   Try to uningest the file that was locked.
 - `Default` - True
 
-<a name="dataverse_utils.dataverse_utils.uningest_file"></a>
+<a id="dataverse_utils.dataverse_utils.uningest_file"></a>
 
 ##### uningest\_file
 
 ```python
-uningest_file(dv_url, fid, apikey, study='n/a')
+def uningest_file(dv_url, fid, apikey, study='n/a')
 ```
 
 Tries to uningest a file that has been ingested.
 Requires superuser API key.
 
 ----------------------------------------
 
@@ -231,20 +238,20 @@
   
   apikey : str
   API key for superuser
   
   study : str
   Optional handle parameter for log messages
 
-<a name="dataverse_utils.dataverse_utils.upload_file"></a>
+<a id="dataverse_utils.dataverse_utils.upload_file"></a>
 
 ##### upload\_file
 
 ```python
-upload_file(fpath, hdl, **kwargs)
+def upload_file(fpath, hdl, **kwargs)
 ```
 
 Uploads file to Dataverse study and sets file metadata and tags.
 
 ----------------------------------------
 
 **Arguments**:
@@ -300,21 +307,27 @@
   Restrict file. Defaults to false unless True supplied
   
   mimetype : str
   OPTIONAL
   Mimetype of file. Useful if using File Previewers. Mimetype for zip files
   (application/zip) will be ignored to circumvent Dataverse's automatic
   unzipping function.
+  label : str
+  OPTIONAL
+  If included in kwargs, this value will be used for the label
+  timeout = int
+  OPTIONAL
+  Timeout in seconds
 
-<a name="dataverse_utils.dataverse_utils.restrict_file"></a>
+<a id="dataverse_utils.dataverse_utils.restrict_file"></a>
 
 ##### restrict\_file
 
 ```python
-restrict_file(**kwargs)
+def restrict_file(**kwargs)
 ```
 
 Restrict file in Dataverse study.
 
 ----------------------------------------
 
 **Arguments**:
@@ -340,20 +353,20 @@
   apikey : str
   REQUIRED
   API key for user
   
   rest : bool
   On True, restrict. Default True
 
-<a name="dataverse_utils.dataverse_utils.upload_from_tsv"></a>
+<a id="dataverse_utils.dataverse_utils.upload_from_tsv"></a>
 
 ##### upload\_from\_tsv
 
 ```python
-upload_from_tsv(fil, hdl, **kwargs)
+def upload_from_tsv(fil, hdl, **kwargs)
 ```
 
 Utility for bulk uploading. Assumes fil is formatted
 as tsv with headers 'file', 'description', 'tags'.
 
 'tags' field will be split on commas.
 
@@ -387,182 +400,187 @@
   apikey : str
   REQUIRED
   API key for user
   
   rest : bool
   On True, restrict access. Default False
 
-<a name="dataverse_utils.ldc"></a>
+<a id="dataverse_utils.ldc"></a>
 
 ## dataverse\_utils.ldc
 
 Creates dataverse JSON from Linguistic Data Consortium
 website page.
 
-<a name="dataverse_utils.ldc.Ldc"></a>
+<a id="dataverse_utils.ldc.Ldc"></a>
 
 ### Ldc Objects
 
 ```python
 class Ldc(ds.Serializer)
 ```
 
 An LDC item (eg, LDC2021T01)
 
-<a name="dataverse_utils.ldc.Ldc.__init__"></a>
+<a id="dataverse_utils.ldc.Ldc.__init__"></a>
 
 ##### \_\_init\_\_
 
 ```python
- | __init__(ldc)
+def __init__(ldc, cert=None)
 ```
 
 Returns a dict with keys created from an LDC catalogue web
 page.
 
 ----------------------------------------
 
 **Arguments**:
 
   
   ldc : str
   Linguistic Consortium Catalogue Number (eg. 'LDC2015T05'.
   This is what forms the last part of the LDC catalogue URL.
+  cert : str
+  Path to certificate chain; LDC has had a problem
+  with intermediate certificates, so you can
+  download the chain with a browser and supply a
+  path to the .pem with this parameter
 
-<a name="dataverse_utils.ldc.Ldc.ldcJson"></a>
+<a id="dataverse_utils.ldc.Ldc.ldcJson"></a>
 
 ##### ldcJson
 
 ```python
- | @property
- | ldcJson()
+@property
+def ldcJson()
 ```
 
 Returns a JSON based on the LDC web page scraping
 
-<a name="dataverse_utils.ldc.Ldc.dryadJson"></a>
+<a id="dataverse_utils.ldc.Ldc.dryadJson"></a>
 
 ##### dryadJson
 
 ```python
- | @property
- | dryadJson()
+@property
+def dryadJson()
 ```
 
 LDC metadata in Dryad JSON format
 
-<a name="dataverse_utils.ldc.Ldc.dvJson"></a>
+<a id="dataverse_utils.ldc.Ldc.dvJson"></a>
 
 ##### dvJson
 
 ```python
- | @property
- | dvJson()
+@property
+def dvJson()
 ```
 
 LDC metadata in Dataverse JSON format
 
-<a name="dataverse_utils.ldc.Ldc.embargo"></a>
+<a id="dataverse_utils.ldc.Ldc.embargo"></a>
 
 ##### embargo
 
 ```python
- | @property
- | embargo()
+@property
+def embargo()
 ```
 
 Boolean indicating embargo status
 
-<a name="dataverse_utils.ldc.Ldc.fileJson"></a>
+<a id="dataverse_utils.ldc.Ldc.fileJson"></a>
 
 ##### fileJson
 
 ```python
- | @property
- | fileJson(timeout=45)
+@property
+def fileJson(timeout=45)
 ```
 
 Returns False: No attached files possible at LDC
 
-<a name="dataverse_utils.ldc.Ldc.files"></a>
+<a id="dataverse_utils.ldc.Ldc.files"></a>
 
 ##### files
 
 ```python
- | @property
- | files()
+@property
+def files()
 ```
 
 Returns None. No files possible
 
-<a name="dataverse_utils.ldc.Ldc.fetch_record"></a>
+<a id="dataverse_utils.ldc.Ldc.fetch_record"></a>
 
 ##### fetch\_record
 
 ```python
- | fetch_record(url=None, timeout=45)
+def fetch_record(url=None, timeout=45)
 ```
 
 Downloads record from LDC website
 
-<a name="dataverse_utils.ldc.Ldc.make_ldc_json"></a>
+<a id="dataverse_utils.ldc.Ldc.make_ldc_json"></a>
 
 ##### make\_ldc\_json
 
 ```python
- | make_ldc_json()
+def make_ldc_json()
 ```
 
 Returns a dict with keys created from an LDC catalogue web
 page.
 
-<a name="dataverse_utils.ldc.Ldc.name_parser"></a>
+<a id="dataverse_utils.ldc.Ldc.name_parser"></a>
 
 ##### name\_parser
 
 ```python
- | @staticmethod
- | name_parser(name)
+@staticmethod
+def name_parser(name)
 ```
 
 Returns lastName/firstName JSON snippet from name
 
 ----------------------------------------
 
 **Arguments**:
 
   
   name : str
   A name
 
-<a name="dataverse_utils.ldc.Ldc.make_dryad_json"></a>
+<a id="dataverse_utils.ldc.Ldc.make_dryad_json"></a>
 
 ##### make\_dryad\_json
 
 ```python
- | make_dryad_json(ldc=None)
+def make_dryad_json(ldc=None)
 ```
 
 Creates a Dryad-style dict from an LDC dictionary
 
 ----------------------------------------
 
 **Arguments**:
 
   
   ldc : dict
   Dictionary containing LDC data. Defaults to self.ldcJson
 
-<a name="dataverse_utils.ldc.Ldc.find_block_index"></a>
+<a id="dataverse_utils.ldc.Ldc.find_block_index"></a>
 
 ##### find\_block\_index
 
 ```python
- | @staticmethod
- | find_block_index(dvjson, key)
+@staticmethod
+def find_block_index(dvjson, key)
 ```
 
 Finds the index number of an item in Dataverse's idiotic JSON list
 
 ----------------------------------------
 
 **Arguments**:
@@ -570,38 +588,38 @@
   
   dvjson : dict
   Dataverse JSON
   
   key : str
   key for which to find list index
 
-<a name="dataverse_utils.ldc.Ldc.make_dv_json"></a>
+<a id="dataverse_utils.ldc.Ldc.make_dv_json"></a>
 
 ##### make\_dv\_json
 
 ```python
- | make_dv_json(ldc=None)
+def make_dv_json(ldc=None)
 ```
 
 Returns complete Dataverse JSON
 
 ----------------------------------------
 
 **Arguments**:
 
   
   ldc : dict
   LDC dictionary. Defaults to self.ldcJson
 
-<a name="dataverse_utils.ldc.Ldc.upload_metadata"></a>
+<a id="dataverse_utils.ldc.Ldc.upload_metadata"></a>
 
 ##### upload\_metadata
 
 ```python
- | upload_metadata(**kwargs) -> dict
+def upload_metadata(**kwargs) -> dict
 ```
 
 Uploads metadata to dataverse
 
 Returns json from connection attempt.
 
 ----------------------------------------
@@ -616,7 +634,122 @@
   
   key : str
   api key
   
   dv : str
   Dataverse to which it is being uploaded
 
+<a id="dataverse_utils.dvdata"></a>
+
+## dataverse\_utils.dvdata
+
+Dataverse studies and files
+
+<a id="dataverse_utils.dvdata.Study"></a>
+
+### Study Objects
+
+```python
+class Study(dict)
+```
+
+Dataverse record. Dataverse study records are pure metadata so this
+is represented with a dictionary.
+
+<a id="dataverse_utils.dvdata.Study.__init__"></a>
+
+##### \_\_init\_\_
+
+```python
+def __init__(pid: str, url: str, key: str, **kwargs)
+```
+
+pid : str
+    Record persistent identifier: hdl or doi
+url : str
+    Base URL to host Dataverse instance
+key : str
+    Dataverse API key with downloader privileges
+
+<a id="dataverse_utils.dvdata.File"></a>
+
+### File Objects
+
+```python
+class File(dict)
+```
+
+Class representing a file on a Dataverse instance
+
+<a id="dataverse_utils.dvdata.File.__init__"></a>
+
+##### \_\_init\_\_
+
+```python
+def __init__(url: str, key: str, **kwargs)
+```
+
+url : str
+    Base URL to host Dataverse instance
+key : str
+    Dataverse API key with downloader privileges
+id : int or str
+    File identifier; can be a file ID or PID
+args : list
+kwargs : dict
+
+To initialize correctly, pass a value from Study['file_info'].
+
+Eg: File('https://test.invalid', 'ABC123', **Study_instance['file_info'][0])
+
+<a id="dataverse_utils.dvdata.File.download_file"></a>
+
+##### download\_file
+
+```python
+def download_file()
+```
+
+Downloads the file to a temporary location. Data will be in the ORIGINAL format,
+not Dataverse-processed TSVs
+
+<a id="dataverse_utils.dvdata.File.del_tempfile"></a>
+
+##### del\_tempfile
+
+```python
+def del_tempfile()
+```
+
+Delete tempfile if it exists
+
+<a id="dataverse_utils.dvdata.File.produce_digest"></a>
+
+##### produce\_digest
+
+```python
+def produce_digest(prot: str = 'md5', blocksize: int = 2**16) -> str
+```
+
+Returns hex digest for object
+
+    fname : str
+       Path to a file object
+
+    prot : str
+       Hash type. Supported hashes: 'sha1', 'sha224', 'sha256',
+          'sha384', 'sha512', 'blake2b', 'blake2s', 'md5'.
+          Default: 'md5'
+
+    blocksize : int
+       Read block size in bytes
+
+<a id="dataverse_utils.dvdata.File.verify"></a>
+
+##### verify
+
+```python
+def verify() -> None
+```
+
+Compares checksum with stated checksum
+
```

### Comparing `dataverse_utils-0.8.7/docs/faq.md` & `dataverse_utils-0.9.1/docs/faq.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/docs/index.md` & `dataverse_utils-0.9.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/docs/scripts.md` & `dataverse_utils-0.9.1/docs/scripts.md`

 * *Files 10% similar despite different names*

```diff
@@ -265,14 +265,65 @@
   -u URL, --url URL     Base URL of Dataverse installation. Defaults to "https://abacus.library.ubc.ca"
   -l LIC, --licence LIC
                         Licence file in Markdown format
   -k KEY, --key KEY     Dataverse API key
   -r, --republish       Republish study without incrementing version
   --version             Show version number and exit
 ``` 
+## dv_study_migrator
+
+If for some reason you need to copy everything from a Dataverse record to a different Dataverse installation or a different collection, this utility will do it for you. Metadata, file names, paths, restrictions etc will all be copied. There are some limitations, though, as only the most recent version will be copied and date handling is done on the target server. The utility will either copy records specifice with a persistent identifer (PID) to a target collection on the same or another server, or replace records with an existing PID.
+
+```nohighlight
+usage: dv_study_migrator [-h] -s SOURCE_URL -a SOURCE_KEY -t TARGET_URL -b TARGET_KEY [-o TIMEOUT] (-c COLLECTION | -r REPLACE [REPLACE ...]) [-v] pids [pids ...]
+
+Record migrator for Dataverse.
+
+This utility will take the most recent version of a study
+from one Dataverse installation and copy the metadata
+and records to another, completely separate dataverse installation.
+
+You could also use it to copy records from one collection to another.
+
+positional arguments:
+  pids                  PID(s) of original Dataverse record(s) in source Dataverse
+                        separated by spaces. eg. "hdl:11272.1/AB2/JEG5RH
+                        doi:11272.1/AB2/JEG5RH".
+                        Case is ignored.
+
+options:
+  -h, --help            show this help message and exit
+  -s SOURCE_URL, --source_url SOURCE_URL
+                        Source Dataverse installation base URL.
+  -a SOURCE_KEY, --source_key SOURCE_KEY
+                        API key for source Dataverse installation.
+  -t TARGET_URL, --target_url TARGET_URL
+                        Source Dataverse installation base URL.
+  -b TARGET_KEY, --target_key TARGET_KEY
+                        API key for target Dataverse installation.
+  -o TIMEOUT, --timeout TIMEOUT
+                        Request timeout in seconds. Default 100.
+  -c COLLECTION, --collection COLLECTION
+                        Short name of target Dataverse collection (eg: dli).
+  -r REPLACE [REPLACE ...], --replace REPLACE [REPLACE ...]
+                        Replace data in these target PIDs with data from the
+                        source PIDS. Number of PIDs listed here must match
+                        the number of PID arguments to follow. That is, the number
+                        of records must be equal. Records will be matched on a
+                        1-1 basis in order. For example:
+                        [rest of command] -r doi:123.34/etc hdl:12323/AB/SOMETHI
+                        will replace the record with identifier 'doi' with the data from 'hdl'.
+                        
+                        Make sure you don't use this as the penultimate switch, because 
+                        then it's not possible to disambiguate PIDS from this argument
+                        and positional arguments.
+                        ie, something like dv_study_migrator -r blah blah -s http//test.invalid etc.
+  -v, --version         Show version number and exit
+```
+
 
 ## dv_upload_tsv
 
 Now that you have a tsv full of nicely described data, you can easily upload it to an existing study if you know the persistent ID and have an API key.
 
 For the best metadata, you should probably edit it manually to add correct descriptive metadata, notably the "Description" and "Tags". Tags are split separated by commas, so it's possible to have multiple tags for each data item, like "Data, SPSS, June 2021".
```

#### html2text {}

```diff
@@ -190,20 +190,52 @@
 required for republishing as the version is not incremented. This software
 requires the Dataverse installation to be running Dataverse software version >=
 5.6. positional arguments: studies Persistent IDs of studies options: -h, --
 help show this help message and exit -u URL, --url URL Base URL of Dataverse
 installation. Defaults to "https://abacus.library.ubc.ca" -l LIC, --licence LIC
 Licence file in Markdown format -k KEY, --key KEY Dataverse API key -r, --
 republish Republish study without incrementing version --version Show version
-number and exit ``` ## dv_upload_tsv Now that you have a tsv full of nicely
-described data, you can easily upload it to an existing study if you know the
-persistent ID and have an API key. For the best metadata, you should probably
-edit it manually to add correct descriptive metadata, notably the "Description"
-and "Tags". Tags are split separated by commas, so it's possible to have
-multiple tags for each data item, like "Data, SPSS, June 2021". File paths are
+number and exit ``` ## dv_study_migrator If for some reason you need to copy
+everything from a Dataverse record to a different Dataverse installation or a
+different collection, this utility will do it for you. Metadata, file names,
+paths, restrictions etc will all be copied. There are some limitations, though,
+as only the most recent version will be copied and date handling is done on the
+target server. The utility will either copy records specifice with a persistent
+identifer (PID) to a target collection on the same or another server, or
+replace records with an existing PID. ```nohighlight usage: dv_study_migrator
+[-h] -s SOURCE_URL -a SOURCE_KEY -t TARGET_URL -b TARGET_KEY [-o TIMEOUT] (-
+c COLLECTION | -r REPLACE [REPLACE ...]) [-v] pids [pids ...] Record migrator
+for Dataverse. This utility will take the most recent version of a study from
+one Dataverse installation and copy the metadata and records to another,
+completely separate dataverse installation. You could also use it to copy
+records from one collection to another. positional arguments: pids PID(s) of
+original Dataverse record(s) in source Dataverse separated by spaces. eg. "hdl:
+11272.1/AB2/JEG5RH doi:11272.1/AB2/JEG5RH". Case is ignored. options: -h, --
+help show this help message and exit -s SOURCE_URL, --source_url SOURCE_URL
+Source Dataverse installation base URL. -a SOURCE_KEY, --source_key SOURCE_KEY
+API key for source Dataverse installation. -t TARGET_URL, --target_url
+TARGET_URL Source Dataverse installation base URL. -b TARGET_KEY, --target_key
+TARGET_KEY API key for target Dataverse installation. -o TIMEOUT, --timeout
+TIMEOUT Request timeout in seconds. Default 100. -c COLLECTION, --collection
+COLLECTION Short name of target Dataverse collection (eg: dli). -r REPLACE
+[REPLACE ...], --replace REPLACE [REPLACE ...] Replace data in these target
+PIDs with data from the source PIDS. Number of PIDs listed here must match the
+number of PID arguments to follow. That is, the number of records must be
+equal. Records will be matched on a 1-1 basis in order. For example: [rest of
+command] -r doi:123.34/etc hdl:12323/AB/SOMETHI will replace the record with
+identifier 'doi' with the data from 'hdl'. Make sure you don't use this as the
+penultimate switch, because then it's not possible to disambiguate PIDS from
+this argument and positional arguments. ie, something like dv_study_migrator -
+r blah blah -s http//test.invalid etc. -v, --version Show version number and
+exit ``` ## dv_upload_tsv Now that you have a tsv full of nicely described
+data, you can easily upload it to an existing study if you know the persistent
+ID and have an API key. For the best metadata, you should probably edit it
+manually to add correct descriptive metadata, notably the "Description" and
+"Tags". Tags are split separated by commas, so it's possible to have multiple
+tags for each data item, like "Data, SPSS, June 2021". File paths are
 automatically generated from the "file" column. Because of this, you should
 probably use relative paths rather than absolute paths unless you want to have
 a lengthy path string in Dataverse. If uploading a tsv which includes
 mimetypes, be aware that mimetypes for zip files will be ignored to circumvent
 Dataverse's automatic unzipping feature. The rationale for manually specifiying
 mimetypes is to enable the use of previews which require a specific mimetype to
 function, but Dataverse does not correctly detect the type. For example, the
```

### Comparing `dataverse_utils-0.8.7/docs/windows.md` & `dataverse_utils-0.9.1/docs/windows.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/pyproject.toml` & `dataverse_utils-0.9.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -52,8 +52,9 @@
 dv_ldc_uploader = 'dataverse_utils.scripts.dv_ldc_uploader:main'
 dv_manifest_gen = 'dataverse_utils.scripts.dv_manifest_gen:main'
 dv_pg_facet_date = 'dataverse_utils.scripts.dv_pg_facet_date:main [server]'
 dv_record_copy = 'dataverse_utils.scripts.dv_record_copy:main'
 dv_release = 'dataverse_utils.scripts.dv_release:main'
 dv_replace_licence = 'dataverse_utils.scripts.dv_replace_licence:main'
 dv_replace_license = 'dataverse_utils.scripts.dv_replace_licence:main'
+dv_study_migrator = 'dataverse_utils.scripts.dv_study_migrator:main'
 dv_upload_tsv = 'dataverse_utils.scripts.dv_upload_tsv:main'
```

### Comparing `dataverse_utils-0.8.7/src/dataverse_utils/data/LDC_EULA_general.md` & `dataverse_utils-0.9.1/src/dataverse_utils/data/LDC_EULA_general.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/src/dataverse_utils/dataverse_utils.py` & `dataverse_utils-0.9.1/src/dataverse_utils/dataverse_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     '''
     if dv_url.endswith('/'):
         dv_url = dv_url[:-1]
     headers = {'X-Dataverse-key': apikey}
     params = {'persistentId': study}
     return (dv_url, headers, params)
 
-def make_tsv(start_dir, in_list=None, def_tag='Data',
+def make_tsv(start_dir, in_list=None, def_tag='Data', # pylint: disable=too-many-arguments
              inc_header=True,
              mime=False,
              quotype=csv.QUOTE_MINIMAL) -> str:
     '''
     Recurses the tree for files and produces tsv output with
     with headers 'file', 'description', 'tags'.
 
@@ -168,15 +168,15 @@
 
     def_tag= kwargs.get('def_tag', 'Data')
     inc_header =kwargs.get('inc_header', True)
     mime = kwargs.get('mime', False)
     quotype = kwargs.get('quotype', csv.QUOTE_MINIMAL)
 
     dumper = make_tsv(start_dir, in_list, def_tag, inc_header, mime, quotype)
-    with open(filename, 'w', newline='') as tsvfile:
+    with open(filename, 'w', newline='', encoding='utf-8') as tsvfile:
         tsvfile.write(dumper)
 
 def file_path(fpath, trunc='') -> str:
     '''
     Create relative file path from full path string
 
     >>> file_path('/tmp/Data/2011/excelfile.xlsx', '/tmp/')
@@ -367,14 +367,20 @@
             Restrict file. Defaults to false unless True supplied
 
         mimetype : str
             OPTIONAL
             Mimetype of file. Useful if using File Previewers. Mimetype for zip files
             (application/zip) will be ignored to circumvent Dataverse's automatic
             unzipping function.
+        label : str
+            OPTIONAL
+            If included in kwargs, this value will be used for the label
+        timeout = int
+            OPTIONAL
+            Timeout in seconds
     '''
     #Why are SPSS files getting processed anyway?
     #Does SPSS detection happen *after* upload
     #Does the file need to be renamed post hoc?
     #I don't think this can be fixed. Goddamitsomuch.
     dvurl = kwargs['dv'].strip('\\ /')
     if os.path.splitext(fpath)[1].lower() in NOTAB:
@@ -391,33 +397,33 @@
     mime = mimetypes.guess_type(fpath)[0]
     if kwargs.get('mimetype'):
         mime = kwargs['mimetype']
     if file_name.endswith('.NOPROCESS') or mime == 'application/zip':
         mime = 'application/octet-stream'
 
     #create file metadata in nice, simple, chunks
-    dv4_meta = {'label' : file_name_clean,
+    dv4_meta = {'label' : kwargs.get('label', file_name_clean),
                 'description' : kwargs.get('descr', ''),
                 'directoryLabel': kwargs.get('dirlabel', ''),
                 'categories': kwargs.get('tags', [])}
     fpath = os.path.abspath(fpath)
-    fields = {'file': (file_name, open(fpath, 'rb'), mime)}
+    fields = {'file': (file_name, open(fpath, 'rb'), mime)}#pylint: disable=consider-using-with
     #fields.update({'jsonData' : f'{dv4_meta}'})
     fields.update({'jsonData' : json.dumps(dv4_meta)})
     multi = MultipartEncoder(fields=fields) # use multipart streaming for large files
     headers = {'X-Dataverse-key' : kwargs.get('apikey'),
                'Content-type' : multi.content_type}
     params = {'persistentId' : hdl}
 
-    print(multi)
+    #print(multi)
 
     LOGGER.info('Uploading %s to %s', fpath, hdl)
     upload = requests.post(f"{dvurl}/api/datasets/:persistentId/add",
                            params=params, headers=headers, data=multi,
-                           timeout=1000)#timeout hardcoded. Bad idea?
+                           timeout=kwargs.get('timeout',1000))
     try:
         print(upload.json())
     except json.decoder.JSONDecodeError:
         #This can happend when Glassfish crashes
         LOGGER.critical(upload.text)
         print(upload.text)
         err = ('It\'s possible Glassfish may have crashed. '
@@ -486,18 +492,19 @@
     else:
         rest= 'false'
     if kwargs.get('pid'):
         params={'persistentId':kwargs['pid']}
         rest = requests.put(f'{kwargs["dv"]}/api/files/:persistentId/restrict',
                             headers=headers,
                             params=params,
-                            data=rest)
+                            data=rest,
+                            timeout=300)
     elif kwargs.get('fid'):
         rest = requests.put(f'{kwargs["dv"]}/api/files/{kwargs["fid"]}/restrict',
-                            headers=headers, data=rest)
+                            headers=headers, data=rest, timeout=300)
     else:
         LOGGER.error('No file ID/PID supplied for file restriction')
         raise KeyError('One of persistentId (pid) or database ID'
                        '(fid) is required for file restriction')
 
 def upload_from_tsv(fil, hdl, **kwargs):
     '''
```

### Comparing `dataverse_utils-0.8.7/src/dataverse_utils/ldc.py` & `dataverse_utils-0.9.1/src/dataverse_utils/ldc.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_del.py` & `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_del.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_ldc_uploader.py` & `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_ldc_uploader.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_manifest_gen.py` & `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_manifest_gen.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_pg_facet_date.py` & `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_pg_facet_date.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_record_copy.py` & `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_record_copy.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 is edit a few fields in the GUI instead of
 painfully editing JSON or painfully using the
 Dataverse GUI.
 '''
 import argparse
 import requests
 
-VERSION = (0, 1, 0)
+VERSION = (0, 1, 1)
 __version__ = '.'.join([str(x) for x in VERSION])
 TIMEOUT = 100
 
 def parsley() -> argparse.ArgumentParser():
     '''
     Parses the arguments from the command line.
 
@@ -27,16 +27,16 @@
                    'Please note that this utility was built with the Abacus '
                    'repository (https://abacus.library.ubc.ca) in mind, '
                    'so many of the defaults are specific to that Dataverse '
                    'installation.')
     parser = argparse.ArgumentParser(description=description)
     parser.add_argument('pid',
                         help=('PID of original dataverse record'
-                              'separated by spaces. eg. "LDC2012T19 LDC2011T07". '
-                              'Case is ignored, so "ldc2012T19" will also work.'))
+                              'separated by spaces. eg. "hdl:11272.1/AB2/NOMATH hdl:11272.1/AB2/HANDLE". '
+                              'Case is ignored, so "hdl:11272.1/ab2/handle" will also work.'))
     parser.add_argument('-u', '--url', default='https://abacus.library.ubc.ca',
                         help=('Dataverse installation base URL. '
                               'Defaults to "https://abacus.library.ubc.ca"'))
     parser.add_argument('-k', '--key', required=True,
                         help='API key')
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument('-c', '--collection',
```

### Comparing `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_release.py` & `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_release.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_replace_licence.py` & `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_replace_licence.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/src/dataverse_utils/scripts/dv_upload_tsv.py` & `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_upload_tsv.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/src/dataverse_utils.egg-info/PKG-INFO` & `dataverse_utils-0.9.1/src/dataverse_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-utils
-Version: 0.8.7
+Version: 0.9.1
 Summary: Utilities for the Dataverse data respository system
 Author-email: Paul Lesack <paul.lesack@ubc.ca>
 Project-URL: Homepage, https://ubc-library-rc.github.io/dataverse_utils
 Project-URL: Repository, https://github.com/ubc-library-rc/dataverse_utils.git
 Project-URL: Issue Tracker, https://github.com/ubc-library-rc/dataverse_utils/issues
 Keywords: Harvard Dataverse,Dataverse,research data management,data repository
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dataverse_utils-0.8.7/src/dataverse_utils.egg-info/SOURCES.txt` & `dataverse_utils-0.9.1/src/dataverse_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 docs/credits.md
 docs/faq.md
 docs/index.md
 docs/scripts.md
 docs/windows.md
 src/dataverse_utils/__init__.py
 src/dataverse_utils/dataverse_utils.py
+src/dataverse_utils/dvdata.py
 src/dataverse_utils/ldc.py
 src/dataverse_utils.egg-info/PKG-INFO
 src/dataverse_utils.egg-info/SOURCES.txt
 src/dataverse_utils.egg-info/dependency_links.txt
 src/dataverse_utils.egg-info/entry_points.txt
 src/dataverse_utils.egg-info/requires.txt
 src/dataverse_utils.egg-info/top_level.txt
@@ -24,12 +25,13 @@
 src/dataverse_utils/scripts/dv_del.py
 src/dataverse_utils/scripts/dv_ldc_uploader.py
 src/dataverse_utils/scripts/dv_manifest_gen.py
 src/dataverse_utils/scripts/dv_pg_facet_date.py
 src/dataverse_utils/scripts/dv_record_copy.py
 src/dataverse_utils/scripts/dv_release.py
 src/dataverse_utils/scripts/dv_replace_licence.py
+src/dataverse_utils/scripts/dv_study_migrator.py
 src/dataverse_utils/scripts/dv_upload_tsv.py
 tests/__init__.py
 tests/tests_dataverse_utils.py
 tmp/requirements.txt
 tmp/setup.py
```

### Comparing `dataverse_utils-0.8.7/tests/tests_dataverse_utils.py` & `dataverse_utils-0.9.1/tests/tests_dataverse_utils.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.8.7/tmp/setup.py` & `dataverse_utils-0.9.1/tmp/setup.py`

 * *Files identical despite different names*

