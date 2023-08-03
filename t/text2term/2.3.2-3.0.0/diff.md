# Comparing `tmp/text2term-2.3.2.tar.gz` & `tmp/text2term-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2term-2.3.2.tar", last modified: Fri May 12 15:13:00 2023, max compression
+gzip compressed data, was "text2term-3.0.0.tar", last modified: Thu Aug  3 17:13:37 2023, max compression
```

## Comparing `text2term-2.3.2.tar` & `text2term-3.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-12 15:13:00.790068 text2term-2.3.2/
--rw-r--r--   0 jason      (501) staff       (20)     1117 2022-08-03 13:24:07.000000 text2term-2.3.2/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)    14914 2023-05-12 15:13:00.789894 text2term-2.3.2/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)    14156 2023-05-04 15:09:10.000000 text2term-2.3.2/README.md
--rw-r--r--   0 jason      (501) staff       (20)       38 2023-05-12 15:13:00.790109 text2term-2.3.2/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1162 2023-03-27 17:45:54.000000 text2term-2.3.2/setup.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-12 15:13:00.785980 text2term-2.3.2/test/
--rw-r--r--   0 jason      (501) staff       (20)     1435 2023-04-25 18:43:12.000000 text2term-2.3.2/test/test-pypi.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-12 15:13:00.789025 text2term-2.3.2/text2term/
--rw-r--r--   0 jason      (501) staff       (20)      427 2023-05-04 15:09:10.000000 text2term-2.3.2/text2term/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     4540 2023-04-25 19:04:10.000000 text2term-2.3.2/text2term/__main__.py
--rw-r--r--   0 jason      (501) staff       (20)     4416 2023-05-10 15:07:50.000000 text2term-2.3.2/text2term/bioportal_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)       17 2023-05-12 15:12:28.000000 text2term-2.3.2/text2term/config.py
--rw-r--r--   0 jason      (501) staff       (20)      469 2022-09-26 14:42:08.000000 text2term-2.3.2/text2term/mapper.py
--rw-r--r--   0 jason      (501) staff       (20)     3735 2023-05-10 16:24:04.000000 text2term-2.3.2/text2term/onto_cache.py
--rw-r--r--   0 jason      (501) staff       (20)     6692 2023-03-27 17:45:54.000000 text2term-2.3.2/text2term/onto_utils.py
--rw-r--r--   0 jason      (501) staff       (20)     5540 2023-03-27 17:45:54.000000 text2term-2.3.2/text2term/preprocess.py
--rw-r--r--   0 jason      (501) staff       (20)     5403 2023-05-10 15:07:50.000000 text2term-2.3.2/text2term/syntactic_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)    12868 2023-05-12 15:12:28.000000 text2term-2.3.2/text2term/t2t.py
--rw-r--r--   0 jason      (501) staff       (20)      741 2023-02-24 16:05:08.000000 text2term-2.3.2/text2term/tagged_terms.py
--rw-r--r--   0 jason      (501) staff       (20)     2479 2023-04-18 15:25:34.000000 text2term-2.3.2/text2term/term.py
--rw-r--r--   0 jason      (501) staff       (20)    17050 2023-05-04 15:09:10.000000 text2term-2.3.2/text2term/term_collector.py
--rw-r--r--   0 jason      (501) staff       (20)     2697 2022-08-03 13:24:07.000000 text2term-2.3.2/text2term/term_graph.py
--rw-r--r--   0 jason      (501) staff       (20)     2991 2023-01-20 15:17:36.000000 text2term-2.3.2/text2term/term_graph_generator.py
--rw-r--r--   0 jason      (501) staff       (20)     2158 2023-04-11 13:56:32.000000 text2term-2.3.2/text2term/term_mapping.py
--rw-r--r--   0 jason      (501) staff       (20)     5108 2022-11-15 20:43:11.000000 text2term-2.3.2/text2term/tfidf_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)     4098 2023-05-10 15:07:50.000000 text2term-2.3.2/text2term/zooma_mapper.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-12 15:13:00.789692 text2term-2.3.2/text2term.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)    14914 2023-05-12 15:13:00.000000 text2term-2.3.2/text2term.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)      649 2023-05-12 15:13:00.000000 text2term-2.3.2/text2term.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2023-05-12 15:13:00.000000 text2term-2.3.2/text2term.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)      248 2023-05-12 15:13:00.000000 text2term-2.3.2/text2term.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)       10 2023-05-12 15:13:00.000000 text2term-2.3.2/text2term.egg-info/top_level.txt
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-08-03 17:13:37.605522 text2term-3.0.0/
+-rw-r--r--   0 jason      (501) staff       (20)     1117 2022-08-03 13:24:07.000000 text2term-3.0.0/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)    14880 2023-08-03 17:13:37.605330 text2term-3.0.0/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)    14122 2023-07-31 15:09:14.000000 text2term-3.0.0/README.md
+-rw-r--r--   0 jason      (501) staff       (20)       38 2023-08-03 17:13:37.605564 text2term-3.0.0/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1162 2023-03-27 17:45:54.000000 text2term-3.0.0/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-08-03 17:13:37.601668 text2term-3.0.0/test/
+-rw-r--r--   0 jason      (501) staff       (20)     1435 2023-04-25 18:43:12.000000 text2term-3.0.0/test/test-pypi.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-08-03 17:13:37.604175 text2term-3.0.0/text2term/
+-rw-r--r--   0 jason      (501) staff       (20)      327 2023-08-01 14:13:06.000000 text2term-3.0.0/text2term/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4540 2023-04-25 19:04:10.000000 text2term-3.0.0/text2term/__main__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4416 2023-05-10 15:07:50.000000 text2term-3.0.0/text2term/bioportal_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)       17 2023-08-03 17:10:54.000000 text2term-3.0.0/text2term/config.py
+-rw-r--r--   0 jason      (501) staff       (20)      469 2022-09-26 14:42:08.000000 text2term-3.0.0/text2term/mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)     3735 2023-05-10 16:24:04.000000 text2term-3.0.0/text2term/onto_cache.py
+-rw-r--r--   0 jason      (501) staff       (20)     6692 2023-03-27 17:45:54.000000 text2term-3.0.0/text2term/onto_utils.py
+-rw-r--r--   0 jason      (501) staff       (20)     4451 2023-08-03 14:05:17.000000 text2term-3.0.0/text2term/preprocess.py
+-rw-r--r--   0 jason      (501) staff       (20)     5403 2023-05-10 15:07:50.000000 text2term-3.0.0/text2term/syntactic_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)    12979 2023-08-03 14:29:26.000000 text2term-3.0.0/text2term/t2t.py
+-rw-r--r--   0 jason      (501) staff       (20)      837 2023-08-03 14:20:09.000000 text2term-3.0.0/text2term/tagged_terms.py
+-rw-r--r--   0 jason      (501) staff       (20)     2479 2023-04-18 15:25:34.000000 text2term-3.0.0/text2term/term.py
+-rw-r--r--   0 jason      (501) staff       (20)    17050 2023-05-04 15:09:10.000000 text2term-3.0.0/text2term/term_collector.py
+-rw-r--r--   0 jason      (501) staff       (20)     2697 2022-08-03 13:24:07.000000 text2term-3.0.0/text2term/term_graph.py
+-rw-r--r--   0 jason      (501) staff       (20)     2991 2023-01-20 15:17:36.000000 text2term-3.0.0/text2term/term_graph_generator.py
+-rw-r--r--   0 jason      (501) staff       (20)     2219 2023-08-03 13:37:32.000000 text2term-3.0.0/text2term/term_mapping.py
+-rw-r--r--   0 jason      (501) staff       (20)     5108 2022-11-15 20:43:11.000000 text2term-3.0.0/text2term/tfidf_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)     4098 2023-05-10 15:07:50.000000 text2term-3.0.0/text2term/zooma_mapper.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-08-03 17:13:37.605130 text2term-3.0.0/text2term.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)    14880 2023-08-03 17:13:37.000000 text2term-3.0.0/text2term.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)      649 2023-08-03 17:13:37.000000 text2term-3.0.0/text2term.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2023-08-03 17:13:37.000000 text2term-3.0.0/text2term.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)      248 2023-08-03 17:13:37.000000 text2term-3.0.0/text2term.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)       10 2023-08-03 17:13:37.000000 text2term-3.0.0/text2term.egg-info/top_level.txt
```

### Comparing `text2term-2.3.2/LICENSE` & `text2term-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `text2term-2.3.2/PKG-INFO` & `text2term-3.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2term
-Version: 2.3.2
+Version: 3.0.0
 Summary: A tool for mapping free-text descriptions of (biomedical) entities to controlled terms in ontologies
 Home-page: https://github.com/ccb-hms/ontology-mapper
 Author: Center for Computational Biomedicine, Harvard Medical School
 Author-email: rafael_goncalves@hms.harvard.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -28,21 +28,22 @@
 ```
 ## Examples
 ### Programmatic
 ```python
 import text2term
 import pandas
 
-df1 = text2term.map_file("test/unstruct_terms.txt", "http://www.ebi.ac.uk/efo/efo.owl")
+df1 = text2term.map_terms("test/unstruct_terms.txt", "http://www.ebi.ac.uk/efo/efo.owl")
 df2 = text2term.map_terms(["asthma", "acute bronchitis"], "http://www.ebi.ac.uk/efo/efo.owl")
+df3 = text2term.map_terms({"asthma":"disease", "acute bronchitis":["disease", "lungs"]}, "http://www.ebi.ac.uk/efo/efo.owl")
 ```
 Below is an example of caching, assuming the same imports as above:
 ```python
 text2term.cache_ontology("http://www.ebi.ac.uk/efo/efo.owl", "EFO")
-df1 = text2term.map_file("test/unstruct_terms.txt", "EFO", use_cache=True)
+df1 = text2term.map_terms("test/unstruct_terms.txt", "EFO", use_cache=True)
 df2 = text2term.map_terms(["asthma", "acute bronchitis"], "EFO", use_cache=True)
 text2term.clear_cache("EFO")
 ```
 
 ### Command Line
 The basic use of the tool requires a `source` file containing a list of terms to map to the given `target` ontology:  
 `python text2term -s test/unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl`
@@ -63,81 +64,54 @@
 
 Use the cache on the command line, first by flagging it, then in the future using the acronym:
 `python text2term -s test/unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl -c EFO`
 Then, after running this, the following command is equivalent:
 `python text2term -s test/unstruct_terms.txt -t EFO`
 
 ## Programmatic Usage
-The tool can be executed in Python with any of the three following functions:
+The tool can be executed in Python with the `map_terms` function:
 
 ```python
-text2term.map_file(input_file='/some/file.txt', 
+text2term.map_terms(source_terms, 
                    target_ontology='http://some.ontology/v1.owl',
                    base_iris=(),
                    csv_columns=(), 
                    excl_deprecated=False, 
                    max_mappings=3, 
                    mapper=Mapper.TFIDF,
                    min_score=0.3, 
                    output_file='', 
                    save_graphs=False, 
                    save_mappings=False, 
                    separator=',', 
                    use_cache=False,
-                   term_type='classes')
-```
-or
-```python
-text2term.map_terms(source_terms=['term one', 'term two'],
-                    target_ontology='http://some.ontology/v1.owl',
-                    base_iris=(),
-                    excl_deprecated=False,
-                    max_mappings=3,
-                    min_score=0.3,
-                    mapper=Mapper.TFIDF,
-                    output_file='',
-                    save_graphs=False,
-                    save_mappings=False,
-                    source_terms_ids=(),
-                    use_cache=False,
-                    term_type='classes')
-```
-or
-```python
-text2term.map_tagged_terms(tagged_terms_dict={'term one': ["tag 1", "tag 2"]},
-                    target_ontology='http://some.ontology/v1.owl',
-                    base_iris=(),
-                    excl_deprecated=False,
-                    max_mappings=3,
-                    min_score=0.3,
-                    mapper=Mapper.TFIDF,
-                    output_file='',
-                    save_graphs=False,
-                    save_mappings=False,
-                    source_terms_ids=(),
-                    use_cache=False,
-                    term_type='classes')
+                   term_type='classes',
+                   incl_unmapped=False)
+
 ```
+NOTE: As of 3.0.0, the former three functions (`map_file`, `map_terms`, `map_tagged_terms`) have been condensed into one function. Users can now change the name of any function in old code to `map_terms` and it reads the input context to maintain the functionality of each one.
 
 ### Arguments
-For `map_file`, the first argument 'input_file' specifies a path to a file containing the terms to be mapped. It also has a `csv_column` argument that allows the user to specify a column to map if a csv is passed in as the input file. 
-For `map_terms`, the first argument 'source_terms' takes in a list of the terms to be mapped.
-For `map_tagged_terms`, everything is the same as `map_terms` except the first argument is either a dictionary of terms to a list of tags, or a list of TaggedTerm objects (see below). Currently, the tags do not affect the mapping in any way, but they are added to the output dataframe at the end of the process.
+For `map_terms`, the first argument can be any of the following: 1) a string that specifies a path to a file containing the terms to be mapped, 2) a list of the terms to be mapped, or 3)dictionary of terms to a list of tags, or a list of TaggedTerm objects (see below). 
+Currently, the tags do not affect the mapping in any way, but they are added to the output dataframe at the end of the process. The exception is the Ignore tag, which causes the term to not be mapped at all, but still be outputted in the results if the incl_unmapped argument is True (see below).
 
 All other arguments are the same, and have the same functionality:
 
 `target_ontology` : str
     Path or URL of 'target' ontology to map the source terms to. When the chosen mapper is BioPortal or Zooma,
     provide a comma-separated list of ontology acronyms (eg 'EFO,HPO') or write 'all' to search all ontologies
     As of version 2.3.0, passing a recognized acronym to `target_ontology` will generate the download link automatically. This is done using the `bioregistry` python package.
 
 `base_iris` : tuple
     Map only to ontology terms whose IRIs start with one of the strings given in this tuple, for example:
     ('http://www.ebi.ac.uk/efo','http://purl.obolibrary.org/obo/HP')
 
+`csv_column` : tuple 
+    Allows the user to specify a column to map if a csv is passed in as the input file. Ignored if the input is not a file path.
+
 `source_terms_ids` : tuple
     Collection of identifiers for the given source terms
     WARNING: While this is still available for the tagged term function, it is worth noting that dictionaries do not necessarily preserve order, so it is not recommended. If using the TaggedTerm object, the source terms can be attached there to guarantee order.
 
 `excl_deprecated` : bool
     Exclude ontology terms stated as deprecated via `owl:deprecated true`
 
@@ -156,20 +130,26 @@
 
 `save_graphs` : bool
     Save vis.js graphs representing the neighborhood of each ontology term
 
 `save_mappings` : bool
     Save the generated mappings to a file (specified by `output_file`) 
 
+`seperator` : str
+    Character that seperates the source term values if a file input is given. Ignored if the input is not a file path.
+
 `use_cache` : bool
     Use the cache for the ontology. More details are below.
 
 `term_type` : str
     Determines whether the ontology should be parsed for its classes (ThingClass), properties (PropertyClass), or both. Possible values are ['classes', 'properties', 'both']. If it does not match one of these values, the program will throw a ValueError.
 
+`incl_unmapped` : bool
+    Include all unmapped terms in the output. If something has been tagged Ignore (see below) or falls below the `min_score` threshold, it is included without a mapped term at the end of the output. 
+
 All default values, if they exist, can be seen above.
 
 ### Return Value
 Both functions return the same value:
 
 `df` : Data frame containing the generated ontology mappings
 
@@ -200,47 +180,53 @@
 Finally, `cache_exists(ontology_acronym='')` is a simple function that returns `True` if the given acronym exists in the cache, and `False` otherwise. It is worth noting that while ontology URLs can repeat, acronyms must be distinct in a given environment.
 
 ### Input Preprocessing
 As of version 1.2.0, text2term includes regex-based preprocessing functionality for input terms. Specifically, these functions take the input terms and a collection of (user-defined) regular expressions, then match each term to each regular expression to simplify the input term.
 
 Like the "map" functions above, the two functions differ on whether the input is a file or a list of strings:
 ```python
-preprocess_file(file_path, template_path, output_file='', blocklist_path='', blocklist_char='', rem_duplicates=False)
-```
-```python
 preprocess_terms(terms, template_path, output_file='', blocklist_path='', blocklist_char='', rem_duplicates=False)
 ``` 
 ```python
 preprocess_tagged_terms(file_path, template_path='', blocklist_path='', blocklist_char='', rem_duplicates=False, separator=';:;')
 ```
 
 In all cases, the regex templates and blocklist must be stored in a newline-separated file. If an output file is specified, the preprocessed strings are written to that file and the list of preprocessed strings is returned.
 
 The blocklist functionality allows the user to specify another regex file. If any terms match any regex in blocklist, they are removed from the terms, or, if a blocklist character is specified, replaced with that character for placeholding. 
 NOTE: As of version 2.1.0, the arguments were changed to "blocklist" from "blacklist". Backwards compatibility is currently supported, but will likely be discontinued at the next major release.
 
 The Remove Duplicates `rem_duplicates` functionality will remove all duplicate terms after processing, if set to `True`. 
 WARNING: Removing duplicates at any point does not guarantee which original term is kept. This is particularly important if original terms have different tags, so user caution is advised.
 
-The functions `preprocess_file()` and `preprocess_terms()` both return a dictionary where the keys are the original terms and the values are the preprocessed terms.
+The function `preprocess_terms()` returns a dictionary where the keys are the original terms and the values are the preprocessed terms.
 The `preprocess_tagged_terms()` function returns a list of TaggedTerm items with the following function contracts:
 ```python
 def __init__(self, term=None, tags=[], original_term=None, source_term_id=None)
 def add_tags(self, new_tags)
 def update_term(self, term)
 def update_source_term_id(self, source_term_id)
 def get_original_term(self)
 def get_term(self)
 def get_tags(self)
 def get_source_term_id(self)
 ```
-As mentioned in the mapping section above, this can then be passed directly to map_tagged_terms(), allowing for easy programmatic usage. Note that this allows multiple of the same preprocessed term with different tags. 
+As mentioned in the mapping section above, this can then be passed directly to `map_terms`, allowing for easy programmatic usage. Note that this allows multiple of the same preprocessed term with different tags. 
 
 **Note on NA values in input**: As of v2.0.3, when the input to text2term is a table file, any rows that contain `NA` values in the specified term column, or in the term ID column (if provided), will be ignored.
 
+### Tag Usage
+As of 3.0.0, some tags have additional functionality that is added when attached to a term:
+
+IGNORE:
+    If an ignore tag is added to a term, that term will not be mapped to any terms in the ontology. It will only be included in the output if the `incl_unmapped` argument is True. Here are the following values that count as ignore tags:
+```python
+    IGNORE_TAGS = ["ignore", "Ignore", "ignore ", "Ignore "]
+```
+
 ## Command Line Usage
 
 After installation, execute the tool from a command line as follows:
 
 `python text2term -s SOURCE -t TARGET [-o OUTPUT] [-m MAPPER] [-csv CSV_INPUT] [-top TOP_MAPPINGS] [-min MIN_SCORE] [-iris BASE_IRIS] [-d EXCL_DEPRECATED] [-g SAVE_TERM_GRAPHS]`
 
 To display a help message with descriptions of tool arguments do:
```

### Comparing `text2term-2.3.2/README.md` & `text2term-3.0.0/text2term.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: text2term
+Version: 3.0.0
+Summary: A tool for mapping free-text descriptions of (biomedical) entities to controlled terms in ontologies
+Home-page: https://github.com/ccb-hms/ontology-mapper
+Author: Center for Computational Biomedicine, Harvard Medical School
+Author-email: rafael_goncalves@hms.harvard.edu
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # *text2term* ontology mapper
 A tool for mapping free-text descriptions of (biomedical) entities to controlled terms in ontologies. 
 
 ## Installation
 Install package using **pip**:
 
 ```
@@ -9,21 +28,22 @@
 ```
 ## Examples
 ### Programmatic
 ```python
 import text2term
 import pandas
 
-df1 = text2term.map_file("test/unstruct_terms.txt", "http://www.ebi.ac.uk/efo/efo.owl")
+df1 = text2term.map_terms("test/unstruct_terms.txt", "http://www.ebi.ac.uk/efo/efo.owl")
 df2 = text2term.map_terms(["asthma", "acute bronchitis"], "http://www.ebi.ac.uk/efo/efo.owl")
+df3 = text2term.map_terms({"asthma":"disease", "acute bronchitis":["disease", "lungs"]}, "http://www.ebi.ac.uk/efo/efo.owl")
 ```
 Below is an example of caching, assuming the same imports as above:
 ```python
 text2term.cache_ontology("http://www.ebi.ac.uk/efo/efo.owl", "EFO")
-df1 = text2term.map_file("test/unstruct_terms.txt", "EFO", use_cache=True)
+df1 = text2term.map_terms("test/unstruct_terms.txt", "EFO", use_cache=True)
 df2 = text2term.map_terms(["asthma", "acute bronchitis"], "EFO", use_cache=True)
 text2term.clear_cache("EFO")
 ```
 
 ### Command Line
 The basic use of the tool requires a `source` file containing a list of terms to map to the given `target` ontology:  
 `python text2term -s test/unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl`
@@ -44,81 +64,54 @@
 
 Use the cache on the command line, first by flagging it, then in the future using the acronym:
 `python text2term -s test/unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl -c EFO`
 Then, after running this, the following command is equivalent:
 `python text2term -s test/unstruct_terms.txt -t EFO`
 
 ## Programmatic Usage
-The tool can be executed in Python with any of the three following functions:
+The tool can be executed in Python with the `map_terms` function:
 
 ```python
-text2term.map_file(input_file='/some/file.txt', 
+text2term.map_terms(source_terms, 
                    target_ontology='http://some.ontology/v1.owl',
                    base_iris=(),
                    csv_columns=(), 
                    excl_deprecated=False, 
                    max_mappings=3, 
                    mapper=Mapper.TFIDF,
                    min_score=0.3, 
                    output_file='', 
                    save_graphs=False, 
                    save_mappings=False, 
                    separator=',', 
                    use_cache=False,
-                   term_type='classes')
-```
-or
-```python
-text2term.map_terms(source_terms=['term one', 'term two'],
-                    target_ontology='http://some.ontology/v1.owl',
-                    base_iris=(),
-                    excl_deprecated=False,
-                    max_mappings=3,
-                    min_score=0.3,
-                    mapper=Mapper.TFIDF,
-                    output_file='',
-                    save_graphs=False,
-                    save_mappings=False,
-                    source_terms_ids=(),
-                    use_cache=False,
-                    term_type='classes')
-```
-or
-```python
-text2term.map_tagged_terms(tagged_terms_dict={'term one': ["tag 1", "tag 2"]},
-                    target_ontology='http://some.ontology/v1.owl',
-                    base_iris=(),
-                    excl_deprecated=False,
-                    max_mappings=3,
-                    min_score=0.3,
-                    mapper=Mapper.TFIDF,
-                    output_file='',
-                    save_graphs=False,
-                    save_mappings=False,
-                    source_terms_ids=(),
-                    use_cache=False,
-                    term_type='classes')
+                   term_type='classes',
+                   incl_unmapped=False)
+
 ```
+NOTE: As of 3.0.0, the former three functions (`map_file`, `map_terms`, `map_tagged_terms`) have been condensed into one function. Users can now change the name of any function in old code to `map_terms` and it reads the input context to maintain the functionality of each one.
 
 ### Arguments
-For `map_file`, the first argument 'input_file' specifies a path to a file containing the terms to be mapped. It also has a `csv_column` argument that allows the user to specify a column to map if a csv is passed in as the input file. 
-For `map_terms`, the first argument 'source_terms' takes in a list of the terms to be mapped.
-For `map_tagged_terms`, everything is the same as `map_terms` except the first argument is either a dictionary of terms to a list of tags, or a list of TaggedTerm objects (see below). Currently, the tags do not affect the mapping in any way, but they are added to the output dataframe at the end of the process.
+For `map_terms`, the first argument can be any of the following: 1) a string that specifies a path to a file containing the terms to be mapped, 2) a list of the terms to be mapped, or 3)dictionary of terms to a list of tags, or a list of TaggedTerm objects (see below). 
+Currently, the tags do not affect the mapping in any way, but they are added to the output dataframe at the end of the process. The exception is the Ignore tag, which causes the term to not be mapped at all, but still be outputted in the results if the incl_unmapped argument is True (see below).
 
 All other arguments are the same, and have the same functionality:
 
 `target_ontology` : str
     Path or URL of 'target' ontology to map the source terms to. When the chosen mapper is BioPortal or Zooma,
     provide a comma-separated list of ontology acronyms (eg 'EFO,HPO') or write 'all' to search all ontologies
     As of version 2.3.0, passing a recognized acronym to `target_ontology` will generate the download link automatically. This is done using the `bioregistry` python package.
 
 `base_iris` : tuple
     Map only to ontology terms whose IRIs start with one of the strings given in this tuple, for example:
     ('http://www.ebi.ac.uk/efo','http://purl.obolibrary.org/obo/HP')
 
+`csv_column` : tuple 
+    Allows the user to specify a column to map if a csv is passed in as the input file. Ignored if the input is not a file path.
+
 `source_terms_ids` : tuple
     Collection of identifiers for the given source terms
     WARNING: While this is still available for the tagged term function, it is worth noting that dictionaries do not necessarily preserve order, so it is not recommended. If using the TaggedTerm object, the source terms can be attached there to guarantee order.
 
 `excl_deprecated` : bool
     Exclude ontology terms stated as deprecated via `owl:deprecated true`
 
@@ -137,20 +130,26 @@
 
 `save_graphs` : bool
     Save vis.js graphs representing the neighborhood of each ontology term
 
 `save_mappings` : bool
     Save the generated mappings to a file (specified by `output_file`) 
 
+`seperator` : str
+    Character that seperates the source term values if a file input is given. Ignored if the input is not a file path.
+
 `use_cache` : bool
     Use the cache for the ontology. More details are below.
 
 `term_type` : str
     Determines whether the ontology should be parsed for its classes (ThingClass), properties (PropertyClass), or both. Possible values are ['classes', 'properties', 'both']. If it does not match one of these values, the program will throw a ValueError.
 
+`incl_unmapped` : bool
+    Include all unmapped terms in the output. If something has been tagged Ignore (see below) or falls below the `min_score` threshold, it is included without a mapped term at the end of the output. 
+
 All default values, if they exist, can be seen above.
 
 ### Return Value
 Both functions return the same value:
 
 `df` : Data frame containing the generated ontology mappings
 
@@ -181,47 +180,53 @@
 Finally, `cache_exists(ontology_acronym='')` is a simple function that returns `True` if the given acronym exists in the cache, and `False` otherwise. It is worth noting that while ontology URLs can repeat, acronyms must be distinct in a given environment.
 
 ### Input Preprocessing
 As of version 1.2.0, text2term includes regex-based preprocessing functionality for input terms. Specifically, these functions take the input terms and a collection of (user-defined) regular expressions, then match each term to each regular expression to simplify the input term.
 
 Like the "map" functions above, the two functions differ on whether the input is a file or a list of strings:
 ```python
-preprocess_file(file_path, template_path, output_file='', blocklist_path='', blocklist_char='', rem_duplicates=False)
-```
-```python
 preprocess_terms(terms, template_path, output_file='', blocklist_path='', blocklist_char='', rem_duplicates=False)
 ``` 
 ```python
 preprocess_tagged_terms(file_path, template_path='', blocklist_path='', blocklist_char='', rem_duplicates=False, separator=';:;')
 ```
 
 In all cases, the regex templates and blocklist must be stored in a newline-separated file. If an output file is specified, the preprocessed strings are written to that file and the list of preprocessed strings is returned.
 
 The blocklist functionality allows the user to specify another regex file. If any terms match any regex in blocklist, they are removed from the terms, or, if a blocklist character is specified, replaced with that character for placeholding. 
 NOTE: As of version 2.1.0, the arguments were changed to "blocklist" from "blacklist". Backwards compatibility is currently supported, but will likely be discontinued at the next major release.
 
 The Remove Duplicates `rem_duplicates` functionality will remove all duplicate terms after processing, if set to `True`. 
 WARNING: Removing duplicates at any point does not guarantee which original term is kept. This is particularly important if original terms have different tags, so user caution is advised.
 
-The functions `preprocess_file()` and `preprocess_terms()` both return a dictionary where the keys are the original terms and the values are the preprocessed terms.
+The function `preprocess_terms()` returns a dictionary where the keys are the original terms and the values are the preprocessed terms.
 The `preprocess_tagged_terms()` function returns a list of TaggedTerm items with the following function contracts:
 ```python
 def __init__(self, term=None, tags=[], original_term=None, source_term_id=None)
 def add_tags(self, new_tags)
 def update_term(self, term)
 def update_source_term_id(self, source_term_id)
 def get_original_term(self)
 def get_term(self)
 def get_tags(self)
 def get_source_term_id(self)
 ```
-As mentioned in the mapping section above, this can then be passed directly to map_tagged_terms(), allowing for easy programmatic usage. Note that this allows multiple of the same preprocessed term with different tags. 
+As mentioned in the mapping section above, this can then be passed directly to `map_terms`, allowing for easy programmatic usage. Note that this allows multiple of the same preprocessed term with different tags. 
 
 **Note on NA values in input**: As of v2.0.3, when the input to text2term is a table file, any rows that contain `NA` values in the specified term column, or in the term ID column (if provided), will be ignored.
 
+### Tag Usage
+As of 3.0.0, some tags have additional functionality that is added when attached to a term:
+
+IGNORE:
+    If an ignore tag is added to a term, that term will not be mapped to any terms in the ontology. It will only be included in the output if the `incl_unmapped` argument is True. Here are the following values that count as ignore tags:
+```python
+    IGNORE_TAGS = ["ignore", "Ignore", "ignore ", "Ignore "]
+```
+
 ## Command Line Usage
 
 After installation, execute the tool from a command line as follows:
 
 `python text2term -s SOURCE -t TARGET [-o OUTPUT] [-m MAPPER] [-csv CSV_INPUT] [-top TOP_MAPPINGS] [-min MIN_SCORE] [-iris BASE_IRIS] [-d EXCL_DEPRECATED] [-g SAVE_TERM_GRAPHS]`
 
 To display a help message with descriptions of tool arguments do:
```

### Comparing `text2term-2.3.2/setup.py` & `text2term-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.2/test/test-pypi.py` & `text2term-3.0.0/test/test-pypi.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.2/text2term/__main__.py` & `text2term-3.0.0/text2term/__main__.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.2/text2term/bioportal_mapper.py` & `text2term-3.0.0/text2term/bioportal_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.2/text2term/onto_cache.py` & `text2term-3.0.0/text2term/onto_cache.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.2/text2term/onto_utils.py` & `text2term-3.0.0/text2term/onto_utils.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.2/text2term/preprocess.py` & `text2term-3.0.0/text2term/preprocess.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,17 @@
 import re
 import os
 from enum import Enum
 from .tagged_terms import TaggedTerm
 
-def preprocess_file(file_path, template_path, output_file="", blocklist_path="", \
-	                blocklist_char='', blacklist_path="", blacklist_char='', \
-	                rem_duplicates=False):
-	# Allows backwards compatibility to blacklist. Will eventually be deleted
-	if blocklist_char == '':
-		blocklist_char = blacklist_char
-	if blocklist_path == "":
-		blocklist_path = blacklist_path
-	terms = _get_values(file_path)
-	processed_terms = preprocess_terms(terms, template_path, output_file=output_file, \
-					blocklist_path=blocklist_path, blocklist_char=blocklist_char, \
-					rem_duplicates=rem_duplicates)
-
-	return processed_terms
-
 ## Tags should be stored with their terms in the same line, delineated by ";:;" 
 ##		ex: Age when diagnosed with (.*) ;:; age,diagnosis
 ##		"Age when diagnosed with cancer" becomes: {"cancer", ["age", "diagnosis"]}
 def preprocess_tagged_terms(file_path, template_path="", blocklist_path="", \
-	                 		blocklist_char='', blacklist_path="", blacklist_char='', \
-	                 		rem_duplicates=False, separator=";:;"):
-	# Allows backwards compatibility to blacklist. Will eventually be deleted
-	if blocklist_char == '':
-		blocklist_char = blacklist_char
-	if blocklist_path == "":
-		blocklist_path = blacklist_path
+	                 		blocklist_char='', rem_duplicates=False, separator=";:;"):
 	# Seperate tags from the terms, put in TaggedTerm and add to list
 	raw_terms = _get_values(file_path)
 	terms = []
 	for raw_term in raw_terms:
 		seperated = raw_term.split(separator)
 		try:
 			tags = seperated[1].split(",")
@@ -76,21 +55,17 @@
 
 	if rem_duplicates:
 		processed_terms = _remove_duplicates(processed_terms)
 
 	return processed_terms
 
 def preprocess_terms(terms, template_path, output_file="", blocklist_path="", \
-	                 blocklist_char='', blacklist_path="", blacklist_char='', \
-	                 rem_duplicates=False):
-	# Allows backwards compatibility to blacklist. Will eventually be deleted
-	if blocklist_char == '':
-		blocklist_char = blacklist_char
-	if blocklist_path == "":
-		blocklist_path = blacklist_path
+	                 blocklist_char='', rem_duplicates=False):
+	if isinstance(terms, str):
+		terms = _get_values(file_path)
 	# Form the templates as regular expressions
 	template_strings = []
 	if template_path != "":
 		template_strings = _get_values(template_path)
 	template_strings.append("(.*)")
 	templates = _make_regex_list(template_strings)
```

### Comparing `text2term-2.3.2/text2term/syntactic_mapper.py` & `text2term-3.0.0/text2term/syntactic_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.2/text2term/tagged_terms.py` & `text2term-3.0.0/text2term/tagged_terms.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,19 +14,25 @@
 
 	def update_term(self, term):
 		self.term = term
 
 	def update_source_term_id(self, source_term_id):
 		self.source_term_id = source_term_id
 
+	def has_tag(self, tag):
+		return tag in self.tags
+
 	def get_original_term(self):
 		return self.original_term
 
 	def get_term(self):
 		return self.term
 
 	def get_tags(self):
 		return self.tags
 
 	def get_source_term_id(self):
 		return self.source_term_id
+
+	def to_dict(self):
+		return {term : tags}
```

### Comparing `text2term-2.3.2/text2term/term.py` & `text2term-3.0.0/text2term/term.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.2/text2term/term_collector.py` & `text2term-3.0.0/text2term/term_collector.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.2/text2term/term_graph.py` & `text2term-3.0.0/text2term/term_graph.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.2/text2term/term_graph_generator.py` & `text2term-3.0.0/text2term/term_graph_generator.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.2/text2term/term_mapping.py` & `text2term-3.0.0/text2term/term_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 
     @property
     def mapped_term_iri(self):
         return self._mapped_term_iri
 
     @property
     def mapped_term_curie(self):
+        if self.mapped_term_iri == "":
+            return ""
         return onto_utils.curie_from_iri(self.mapped_term_iri)
 
     @property
     def mapping_score(self):
         return self._mapping_score
 
     def to_dict(self):
```

### Comparing `text2term-2.3.2/text2term/tfidf_mapper.py` & `text2term-3.0.0/text2term/tfidf_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.2/text2term/zooma_mapper.py` & `text2term-3.0.0/text2term/zooma_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.2/text2term.egg-info/PKG-INFO` & `text2term-3.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: text2term
-Version: 2.3.2
-Summary: A tool for mapping free-text descriptions of (biomedical) entities to controlled terms in ontologies
-Home-page: https://github.com/ccb-hms/ontology-mapper
-Author: Center for Computational Biomedicine, Harvard Medical School
-Author-email: rafael_goncalves@hms.harvard.edu
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # *text2term* ontology mapper
 A tool for mapping free-text descriptions of (biomedical) entities to controlled terms in ontologies. 
 
 ## Installation
 Install package using **pip**:
 
 ```
@@ -28,21 +9,22 @@
 ```
 ## Examples
 ### Programmatic
 ```python
 import text2term
 import pandas
 
-df1 = text2term.map_file("test/unstruct_terms.txt", "http://www.ebi.ac.uk/efo/efo.owl")
+df1 = text2term.map_terms("test/unstruct_terms.txt", "http://www.ebi.ac.uk/efo/efo.owl")
 df2 = text2term.map_terms(["asthma", "acute bronchitis"], "http://www.ebi.ac.uk/efo/efo.owl")
+df3 = text2term.map_terms({"asthma":"disease", "acute bronchitis":["disease", "lungs"]}, "http://www.ebi.ac.uk/efo/efo.owl")
 ```
 Below is an example of caching, assuming the same imports as above:
 ```python
 text2term.cache_ontology("http://www.ebi.ac.uk/efo/efo.owl", "EFO")
-df1 = text2term.map_file("test/unstruct_terms.txt", "EFO", use_cache=True)
+df1 = text2term.map_terms("test/unstruct_terms.txt", "EFO", use_cache=True)
 df2 = text2term.map_terms(["asthma", "acute bronchitis"], "EFO", use_cache=True)
 text2term.clear_cache("EFO")
 ```
 
 ### Command Line
 The basic use of the tool requires a `source` file containing a list of terms to map to the given `target` ontology:  
 `python text2term -s test/unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl`
@@ -63,81 +45,54 @@
 
 Use the cache on the command line, first by flagging it, then in the future using the acronym:
 `python text2term -s test/unstruct_terms.txt -t http://www.ebi.ac.uk/efo/efo.owl -c EFO`
 Then, after running this, the following command is equivalent:
 `python text2term -s test/unstruct_terms.txt -t EFO`
 
 ## Programmatic Usage
-The tool can be executed in Python with any of the three following functions:
+The tool can be executed in Python with the `map_terms` function:
 
 ```python
-text2term.map_file(input_file='/some/file.txt', 
+text2term.map_terms(source_terms, 
                    target_ontology='http://some.ontology/v1.owl',
                    base_iris=(),
                    csv_columns=(), 
                    excl_deprecated=False, 
                    max_mappings=3, 
                    mapper=Mapper.TFIDF,
                    min_score=0.3, 
                    output_file='', 
                    save_graphs=False, 
                    save_mappings=False, 
                    separator=',', 
                    use_cache=False,
-                   term_type='classes')
-```
-or
-```python
-text2term.map_terms(source_terms=['term one', 'term two'],
-                    target_ontology='http://some.ontology/v1.owl',
-                    base_iris=(),
-                    excl_deprecated=False,
-                    max_mappings=3,
-                    min_score=0.3,
-                    mapper=Mapper.TFIDF,
-                    output_file='',
-                    save_graphs=False,
-                    save_mappings=False,
-                    source_terms_ids=(),
-                    use_cache=False,
-                    term_type='classes')
-```
-or
-```python
-text2term.map_tagged_terms(tagged_terms_dict={'term one': ["tag 1", "tag 2"]},
-                    target_ontology='http://some.ontology/v1.owl',
-                    base_iris=(),
-                    excl_deprecated=False,
-                    max_mappings=3,
-                    min_score=0.3,
-                    mapper=Mapper.TFIDF,
-                    output_file='',
-                    save_graphs=False,
-                    save_mappings=False,
-                    source_terms_ids=(),
-                    use_cache=False,
-                    term_type='classes')
+                   term_type='classes',
+                   incl_unmapped=False)
+
 ```
+NOTE: As of 3.0.0, the former three functions (`map_file`, `map_terms`, `map_tagged_terms`) have been condensed into one function. Users can now change the name of any function in old code to `map_terms` and it reads the input context to maintain the functionality of each one.
 
 ### Arguments
-For `map_file`, the first argument 'input_file' specifies a path to a file containing the terms to be mapped. It also has a `csv_column` argument that allows the user to specify a column to map if a csv is passed in as the input file. 
-For `map_terms`, the first argument 'source_terms' takes in a list of the terms to be mapped.
-For `map_tagged_terms`, everything is the same as `map_terms` except the first argument is either a dictionary of terms to a list of tags, or a list of TaggedTerm objects (see below). Currently, the tags do not affect the mapping in any way, but they are added to the output dataframe at the end of the process.
+For `map_terms`, the first argument can be any of the following: 1) a string that specifies a path to a file containing the terms to be mapped, 2) a list of the terms to be mapped, or 3)dictionary of terms to a list of tags, or a list of TaggedTerm objects (see below). 
+Currently, the tags do not affect the mapping in any way, but they are added to the output dataframe at the end of the process. The exception is the Ignore tag, which causes the term to not be mapped at all, but still be outputted in the results if the incl_unmapped argument is True (see below).
 
 All other arguments are the same, and have the same functionality:
 
 `target_ontology` : str
     Path or URL of 'target' ontology to map the source terms to. When the chosen mapper is BioPortal or Zooma,
     provide a comma-separated list of ontology acronyms (eg 'EFO,HPO') or write 'all' to search all ontologies
     As of version 2.3.0, passing a recognized acronym to `target_ontology` will generate the download link automatically. This is done using the `bioregistry` python package.
 
 `base_iris` : tuple
     Map only to ontology terms whose IRIs start with one of the strings given in this tuple, for example:
     ('http://www.ebi.ac.uk/efo','http://purl.obolibrary.org/obo/HP')
 
+`csv_column` : tuple 
+    Allows the user to specify a column to map if a csv is passed in as the input file. Ignored if the input is not a file path.
+
 `source_terms_ids` : tuple
     Collection of identifiers for the given source terms
     WARNING: While this is still available for the tagged term function, it is worth noting that dictionaries do not necessarily preserve order, so it is not recommended. If using the TaggedTerm object, the source terms can be attached there to guarantee order.
 
 `excl_deprecated` : bool
     Exclude ontology terms stated as deprecated via `owl:deprecated true`
 
@@ -156,20 +111,26 @@
 
 `save_graphs` : bool
     Save vis.js graphs representing the neighborhood of each ontology term
 
 `save_mappings` : bool
     Save the generated mappings to a file (specified by `output_file`) 
 
+`seperator` : str
+    Character that seperates the source term values if a file input is given. Ignored if the input is not a file path.
+
 `use_cache` : bool
     Use the cache for the ontology. More details are below.
 
 `term_type` : str
     Determines whether the ontology should be parsed for its classes (ThingClass), properties (PropertyClass), or both. Possible values are ['classes', 'properties', 'both']. If it does not match one of these values, the program will throw a ValueError.
 
+`incl_unmapped` : bool
+    Include all unmapped terms in the output. If something has been tagged Ignore (see below) or falls below the `min_score` threshold, it is included without a mapped term at the end of the output. 
+
 All default values, if they exist, can be seen above.
 
 ### Return Value
 Both functions return the same value:
 
 `df` : Data frame containing the generated ontology mappings
 
@@ -200,47 +161,53 @@
 Finally, `cache_exists(ontology_acronym='')` is a simple function that returns `True` if the given acronym exists in the cache, and `False` otherwise. It is worth noting that while ontology URLs can repeat, acronyms must be distinct in a given environment.
 
 ### Input Preprocessing
 As of version 1.2.0, text2term includes regex-based preprocessing functionality for input terms. Specifically, these functions take the input terms and a collection of (user-defined) regular expressions, then match each term to each regular expression to simplify the input term.
 
 Like the "map" functions above, the two functions differ on whether the input is a file or a list of strings:
 ```python
-preprocess_file(file_path, template_path, output_file='', blocklist_path='', blocklist_char='', rem_duplicates=False)
-```
-```python
 preprocess_terms(terms, template_path, output_file='', blocklist_path='', blocklist_char='', rem_duplicates=False)
 ``` 
 ```python
 preprocess_tagged_terms(file_path, template_path='', blocklist_path='', blocklist_char='', rem_duplicates=False, separator=';:;')
 ```
 
 In all cases, the regex templates and blocklist must be stored in a newline-separated file. If an output file is specified, the preprocessed strings are written to that file and the list of preprocessed strings is returned.
 
 The blocklist functionality allows the user to specify another regex file. If any terms match any regex in blocklist, they are removed from the terms, or, if a blocklist character is specified, replaced with that character for placeholding. 
 NOTE: As of version 2.1.0, the arguments were changed to "blocklist" from "blacklist". Backwards compatibility is currently supported, but will likely be discontinued at the next major release.
 
 The Remove Duplicates `rem_duplicates` functionality will remove all duplicate terms after processing, if set to `True`. 
 WARNING: Removing duplicates at any point does not guarantee which original term is kept. This is particularly important if original terms have different tags, so user caution is advised.
 
-The functions `preprocess_file()` and `preprocess_terms()` both return a dictionary where the keys are the original terms and the values are the preprocessed terms.
+The function `preprocess_terms()` returns a dictionary where the keys are the original terms and the values are the preprocessed terms.
 The `preprocess_tagged_terms()` function returns a list of TaggedTerm items with the following function contracts:
 ```python
 def __init__(self, term=None, tags=[], original_term=None, source_term_id=None)
 def add_tags(self, new_tags)
 def update_term(self, term)
 def update_source_term_id(self, source_term_id)
 def get_original_term(self)
 def get_term(self)
 def get_tags(self)
 def get_source_term_id(self)
 ```
-As mentioned in the mapping section above, this can then be passed directly to map_tagged_terms(), allowing for easy programmatic usage. Note that this allows multiple of the same preprocessed term with different tags. 
+As mentioned in the mapping section above, this can then be passed directly to `map_terms`, allowing for easy programmatic usage. Note that this allows multiple of the same preprocessed term with different tags. 
 
 **Note on NA values in input**: As of v2.0.3, when the input to text2term is a table file, any rows that contain `NA` values in the specified term column, or in the term ID column (if provided), will be ignored.
 
+### Tag Usage
+As of 3.0.0, some tags have additional functionality that is added when attached to a term:
+
+IGNORE:
+    If an ignore tag is added to a term, that term will not be mapped to any terms in the ontology. It will only be included in the output if the `incl_unmapped` argument is True. Here are the following values that count as ignore tags:
+```python
+    IGNORE_TAGS = ["ignore", "Ignore", "ignore ", "Ignore "]
+```
+
 ## Command Line Usage
 
 After installation, execute the tool from a command line as follows:
 
 `python text2term -s SOURCE -t TARGET [-o OUTPUT] [-m MAPPER] [-csv CSV_INPUT] [-top TOP_MAPPINGS] [-min MIN_SCORE] [-iris BASE_IRIS] [-d EXCL_DEPRECATED] [-g SAVE_TERM_GRAPHS]`
 
 To display a help message with descriptions of tool arguments do:
```

### Comparing `text2term-2.3.2/text2term.egg-info/SOURCES.txt` & `text2term-3.0.0/text2term.egg-info/SOURCES.txt`

 * *Files identical despite different names*

