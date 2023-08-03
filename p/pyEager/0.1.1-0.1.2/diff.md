# Comparing `tmp/pyEager-0.1.1.tar.gz` & `tmp/pyEager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEager-0.1.1.tar", last modified: Wed Aug  2 15:14:07 2023, max compression
+gzip compressed data, was "pyEager-0.1.2.tar", last modified: Thu Aug  3 13:03:41 2023, max compression
```

## Comparing `pyEager-0.1.1.tar` & `pyEager-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-08-02 15:14:07.528261 pyEager-0.1.1/
--rw-r--r--   0 lamnidis   (506) staff       (20)     1071 2023-08-02 14:15:47.000000 pyEager-0.1.1/LICENSE.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)     2623 2023-08-02 15:14:07.528512 pyEager-0.1.1/PKG-INFO
--rw-r--r--   0 lamnidis   (506) staff       (20)     1736 2023-08-02 14:42:34.000000 pyEager-0.1.1/README.md
-drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-08-02 15:14:07.524883 pyEager-0.1.1/pyEager/
--rw-r--r--   0 lamnidis   (506) staff       (20)      313 2023-08-02 13:55:17.000000 pyEager-0.1.1/pyEager/__init__.py
--rw-r--r--   0 lamnidis   (506) staff       (20)     4455 2023-08-02 14:07:28.000000 pyEager-0.1.1/pyEager/parsers.py
--rw-r--r--   0 lamnidis   (506) staff       (20)     2929 2023-08-02 12:59:57.000000 pyEager-0.1.1/pyEager/wrappers.py
-drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-08-02 15:14:07.527595 pyEager-0.1.1/pyEager.egg-info/
--rw-r--r--   0 lamnidis   (506) staff       (20)     2623 2023-08-02 15:14:07.000000 pyEager-0.1.1/pyEager.egg-info/PKG-INFO
--rw-r--r--   0 lamnidis   (506) staff       (20)      253 2023-08-02 15:14:07.000000 pyEager-0.1.1/pyEager.egg-info/SOURCES.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)        1 2023-08-02 15:14:07.000000 pyEager-0.1.1/pyEager.egg-info/dependency_links.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)        7 2023-08-02 15:14:07.000000 pyEager-0.1.1/pyEager.egg-info/requires.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)        8 2023-08-02 15:14:07.000000 pyEager-0.1.1/pyEager.egg-info/top_level.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)       79 2023-08-02 15:14:07.529126 pyEager-0.1.1/setup.cfg
--rw-r--r--   0 lamnidis   (506) staff       (20)     1171 2023-08-02 15:12:34.000000 pyEager-0.1.1/setup.py
+drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-08-03 13:03:41.438827 pyEager-0.1.2/
+-rw-r--r--   0 lamnidis   (506) staff       (20)     1071 2023-08-02 14:15:47.000000 pyEager-0.1.2/LICENSE.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)     2724 2023-08-03 13:03:41.439050 pyEager-0.1.2/PKG-INFO
+-rw-r--r--   0 lamnidis   (506) staff       (20)     1837 2023-08-03 13:02:36.000000 pyEager-0.1.2/README.md
+drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-08-03 13:03:41.435754 pyEager-0.1.2/pyEager/
+-rw-r--r--   0 lamnidis   (506) staff       (20)      340 2023-08-03 12:59:11.000000 pyEager-0.1.2/pyEager/__init__.py
+-rw-r--r--   0 lamnidis   (506) staff       (20)     4863 2023-08-03 12:58:24.000000 pyEager-0.1.2/pyEager/parsers.py
+-rw-r--r--   0 lamnidis   (506) staff       (20)     2929 2023-08-03 12:59:09.000000 pyEager-0.1.2/pyEager/wrappers.py
+drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-08-03 13:03:41.438436 pyEager-0.1.2/pyEager.egg-info/
+-rw-r--r--   0 lamnidis   (506) staff       (20)     2724 2023-08-03 13:03:40.000000 pyEager-0.1.2/pyEager.egg-info/PKG-INFO
+-rw-r--r--   0 lamnidis   (506) staff       (20)      253 2023-08-03 13:03:41.000000 pyEager-0.1.2/pyEager.egg-info/SOURCES.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)        1 2023-08-03 13:03:41.000000 pyEager-0.1.2/pyEager.egg-info/dependency_links.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)        7 2023-08-03 13:03:41.000000 pyEager-0.1.2/pyEager.egg-info/requires.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)        8 2023-08-03 13:03:41.000000 pyEager-0.1.2/pyEager.egg-info/top_level.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)       79 2023-08-03 13:03:41.439694 pyEager-0.1.2/setup.cfg
+-rw-r--r--   0 lamnidis   (506) staff       (20)     1171 2023-08-03 12:59:02.000000 pyEager-0.1.2/setup.py
```

### Comparing `pyEager-0.1.1/LICENSE.txt` & `pyEager-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyEager-0.1.1/PKG-INFO` & `pyEager-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyEager
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple package to read in eager results.
 Home-page: https://github.com/TCLamnidis/pyEager
-Download-URL: https://github.com/TCLamnidis/pyEager/archive/refs/tags/0.1.1.tar.gz
+Download-URL: https://github.com/TCLamnidis/pyEager/archive/refs/tags/0.1.2.tar.gz
 Author: Thiseas C. Lamnidis
 Author-email: thisseass@gmail.com
 License: MIT
 Keywords: python,pandas,nf-core,eager,nf-core/eager,ancient DNA
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -33,14 +33,15 @@
     - `collect_damageprofiler_results()`: Collects the results from multiple damageprofiler JSON output files into a large dictionary containing all the results for each sample. This function wraps `parse_damageprofiler_json` across all provided JSON files.
     - `parse_damageprofiler_json()`: Read in the information in a single damageprofiler JSON output file. 
  - `compile_snp_coverage_table()`: Creates a compiled table of SNP coverage results from the list of JSON files provided. Wraps `parse_snp_coverage_json` across all provided JSON files
     - `parse_snp_coverage_json()`: Read in the information in a single SNP coverage JSON file.
  - `parse_sexdeterrmine_json()`: Reads in the Sexdeterrmine output JSON into a dataframe.
  - `parse_nuclear_contamination_json()`: Reads in the nuclear contamination output JSON into a dataframe.
  - `parse_eager_tsv()`: Reads in the eager input TSV into a dataframe.
+ - `parse_general_stats_table`: Reads in the general stats table output of MultiQC into a dataframe.
 
 ## Installation
 
 <!-- TODO Add installation instructions -->
 
 ## Usage
```

### Comparing `pyEager-0.1.1/README.md` & `pyEager-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     - `collect_damageprofiler_results()`: Collects the results from multiple damageprofiler JSON output files into a large dictionary containing all the results for each sample. This function wraps `parse_damageprofiler_json` across all provided JSON files.
     - `parse_damageprofiler_json()`: Read in the information in a single damageprofiler JSON output file. 
  - `compile_snp_coverage_table()`: Creates a compiled table of SNP coverage results from the list of JSON files provided. Wraps `parse_snp_coverage_json` across all provided JSON files
     - `parse_snp_coverage_json()`: Read in the information in a single SNP coverage JSON file.
  - `parse_sexdeterrmine_json()`: Reads in the Sexdeterrmine output JSON into a dataframe.
  - `parse_nuclear_contamination_json()`: Reads in the nuclear contamination output JSON into a dataframe.
  - `parse_eager_tsv()`: Reads in the eager input TSV into a dataframe.
+ - `parse_general_stats_table`: Reads in the general stats table output of MultiQC into a dataframe.
 
 ## Installation
 
 <!-- TODO Add installation instructions -->
 
 ## Usage
```

### Comparing `pyEager-0.1.1/pyEager/parsers.py` & `pyEager-0.1.2/pyEager/parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,8 +121,22 @@
   Returns:
       pandas.DataFrame: A data frame containing the data of the TSV.
   """
   ## TODO Eventually, could add renaming of columns here to keep output consistent between eager 2.* and 3.*
   with open(tsv_path) as f:
     data=pd.read_table(f, sep="\t")
   
+  return data
+
+def parse_general_stats_table(general_stats_path):
+  """Parse the general_stats_table.txt output of MultiQC into a pandas DataFrame.
+
+  Args:
+      general_stats_path (string): The path to the `general_stats_table.txt` TSV file.
+
+  Returns:
+      pandas.DataFrame: A data frame containing the data of the TSV.
+  """
+  with open(general_stats_path) as f:
+    data=pd.read_table(f, sep="\t")
+  
   return data
```

### Comparing `pyEager-0.1.1/pyEager/wrappers.py` & `pyEager-0.1.2/pyEager/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyEager-0.1.1/pyEager.egg-info/PKG-INFO` & `pyEager-0.1.2/pyEager.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyEager
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple package to read in eager results.
 Home-page: https://github.com/TCLamnidis/pyEager
-Download-URL: https://github.com/TCLamnidis/pyEager/archive/refs/tags/0.1.1.tar.gz
+Download-URL: https://github.com/TCLamnidis/pyEager/archive/refs/tags/0.1.2.tar.gz
 Author: Thiseas C. Lamnidis
 Author-email: thisseass@gmail.com
 License: MIT
 Keywords: python,pandas,nf-core,eager,nf-core/eager,ancient DNA
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -33,14 +33,15 @@
     - `collect_damageprofiler_results()`: Collects the results from multiple damageprofiler JSON output files into a large dictionary containing all the results for each sample. This function wraps `parse_damageprofiler_json` across all provided JSON files.
     - `parse_damageprofiler_json()`: Read in the information in a single damageprofiler JSON output file. 
  - `compile_snp_coverage_table()`: Creates a compiled table of SNP coverage results from the list of JSON files provided. Wraps `parse_snp_coverage_json` across all provided JSON files
     - `parse_snp_coverage_json()`: Read in the information in a single SNP coverage JSON file.
  - `parse_sexdeterrmine_json()`: Reads in the Sexdeterrmine output JSON into a dataframe.
  - `parse_nuclear_contamination_json()`: Reads in the nuclear contamination output JSON into a dataframe.
  - `parse_eager_tsv()`: Reads in the eager input TSV into a dataframe.
+ - `parse_general_stats_table`: Reads in the general stats table output of MultiQC into a dataframe.
 
 ## Installation
 
 <!-- TODO Add installation instructions -->
 
 ## Usage
```

### Comparing `pyEager-0.1.1/setup.py` & `pyEager-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 setup(
   name = 'pyEager',
   packages = ['pyEager'],
-  version = '0.1.1',
+  version = '0.1.2',
   license='MIT',
   description = 'A simple package to read in eager results.',
   long_description=open('README.md').read(),
   author = 'Thiseas C. Lamnidis',
   author_email = 'thisseass@gmail.com',
   url = 'https://github.com/TCLamnidis/pyEager',
-  download_url = 'https://github.com/TCLamnidis/pyEager/archive/refs/tags/0.1.1.tar.gz',
+  download_url = 'https://github.com/TCLamnidis/pyEager/archive/refs/tags/0.1.2.tar.gz',
   keywords = ['python', 'pandas', 'nf-core', 'eager', 'nf-core/eager', 'ancient DNA' ],
   python_requires=">=3.6",
   install_requires=[
           'pandas',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

