# Comparing `tmp/monocleaner-1.6.tar.gz` & `tmp/monocleaner-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monocleaner-1.6.tar", last modified: Wed Jul 26 11:10:04 2023, max compression
+gzip compressed data, was "monocleaner-1.6.1.tar", last modified: Thu Aug  3 09:19:40 2023, max compression
```

## Comparing `monocleaner-1.6.tar` & `monocleaner-1.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 11:10:04.386776 monocleaner-1.6/
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-07-26 11:09:54.000000 monocleaner-1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    11218 2023-07-26 11:10:04.386776 monocleaner-1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10124 2023-07-26 11:09:54.000000 monocleaner-1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-07-26 11:09:54.000000 monocleaner-1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 11:10:04.382776 monocleaner-1.6/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1304 2023-07-26 11:09:54.000000 monocleaner-1.6/scripts/monocleaner-download
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-26 11:10:04.386776 monocleaner-1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 11:10:04.382776 monocleaner-1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 11:10:04.386776 monocleaner-1.6/src/monocleaner/
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14650 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/hardrules.py
--rw-r--r--   0 runner    (1001) docker     (122)    13458 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/lm.py
--rw-r--r--   0 runner    (1001) docker     (122)     6516 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/monocleaner.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/monocleaner_train.py
--rw-r--r--   0 runner    (1001) docker     (122)     6878 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/normalize.py
--rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 11:10:04.386776 monocleaner-1.6/src/monocleaner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11218 2023-07-26 11:10:04.000000 monocleaner-1.6/src/monocleaner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      526 2023-07-26 11:10:04.000000 monocleaner-1.6/src/monocleaner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 11:10:04.000000 monocleaner-1.6/src/monocleaner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-26 11:10:04.000000 monocleaner-1.6/src/monocleaner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-07-26 11:10:04.000000 monocleaner-1.6/src/monocleaner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-26 11:10:04.000000 monocleaner-1.6/src/monocleaner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:19:40.672168 monocleaner-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-08-03 09:19:27.000000 monocleaner-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    12571 2023-08-03 09:19:40.672168 monocleaner-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11475 2023-08-03 09:19:27.000000 monocleaner-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-08-03 09:19:27.000000 monocleaner-1.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:19:40.672168 monocleaner-1.6.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1304 2023-08-03 09:19:27.000000 monocleaner-1.6.1/scripts/monocleaner-download
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-03 09:19:40.672168 monocleaner-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:19:40.672168 monocleaner-1.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:19:40.672168 monocleaner-1.6.1/src/monocleaner/
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-08-03 09:19:27.000000 monocleaner-1.6.1/src/monocleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13893 2023-08-03 09:19:27.000000 monocleaner-1.6.1/src/monocleaner/hardrules.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13458 2023-08-03 09:19:27.000000 monocleaner-1.6.1/src/monocleaner/lm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7156 2023-08-03 09:19:27.000000 monocleaner-1.6.1/src/monocleaner/monocleaner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-08-03 09:19:27.000000 monocleaner-1.6.1/src/monocleaner/monocleaner_train.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6878 2023-08-03 09:19:27.000000 monocleaner-1.6.1/src/monocleaner/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-08-03 09:19:27.000000 monocleaner-1.6.1/src/monocleaner/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-08-03 09:19:27.000000 monocleaner-1.6.1/src/monocleaner/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:19:40.672168 monocleaner-1.6.1/src/monocleaner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    12571 2023-08-03 09:19:40.000000 monocleaner-1.6.1/src/monocleaner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-08-03 09:19:40.000000 monocleaner-1.6.1/src/monocleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 09:19:40.000000 monocleaner-1.6.1/src/monocleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-08-03 09:19:40.000000 monocleaner-1.6.1/src/monocleaner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-08-03 09:19:40.000000 monocleaner-1.6.1/src/monocleaner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-08-03 09:19:40.000000 monocleaner-1.6.1/src/monocleaner.egg-info/top_level.txt
```

### Comparing `monocleaner-1.6/LICENSE` & `monocleaner-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `monocleaner-1.6/PKG-INFO` & `monocleaner-1.6.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monocleaner
-Version: 1.6
+Version: 1.6.1
 Summary: Monolingual corpus fluency filter
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License: GNU General Public License v3.0
 Project-URL: Homepage, https://github.com/bitextor/monocleaner
 Project-URL: Monocleaner on GitHub, https://github.com/bitextor/monocleaner
 Project-URL: Prompsit Language Engineering, http://www.prompsit.com
@@ -97,21 +97,31 @@
             [--disable_hardrules]
             [--disable_minimal_length]
             [--disable_hbs]
             [--score_only]
             [--annotated_output]
             [--add_lang_ident]
             [--detect_script]
+            [--run_all_rules]
             [--debug]
             [-q]
             [-v]
             model_dir [input] [output]
 ```
 If input and output are omitted, it will read from stdin and write to stdout.
 
+The output file will contain the following columns which will appear in the strict order indicated below depending on the previous parameters:
+
+| Column | Value            | Parameters                    |
+| ------ | ---------------- | ----------------------------- | 
+|   1    | Sentence         | Disabled by --score_only      |
+|   2    | Score            |  -                            |
+|   3    | Language Code    | Enabled by --add_lang_ident   |
+|   4    | Hardrule Tag     | Enabled by --annotated_output |
+
 ### Parameters
 * Positional arguments:
   * `model_dir`: Directory where the model is stored.
   * `input`: Input text file, one sentence per line. When omitted jointly with output, it will read from stdin.
   * `output`: Output tab-separated text file adding monocleaner score. When omitted output will be written to stdout.
 * Optional arguments:
   * `--scol`: Sentence column (starting in 1) (default: 1)
@@ -119,14 +129,15 @@
   * `--disable_hardrules`: Disables the hardrules filtering (only monocleaner fluency scoring is applied) (default: False)
   * `--disable_minimal_length` : Don't apply minimal length rule (default: False).
   * `--disable_hbs`: Don't group Serbo-Croatian under 'hbs' tag. (default: False)
   * `--score_only`: Only output one column which is the monocleaner score (default: False)
   * `--annotated_output`: Add hardrules annotation for each sentence. (default: False)
   * `--add_lang_ident`: Add another column with the identified language if it's not disabled. (default: False)
   * `--detect_script`: Detect writing script with FastSpell (only Serbo-Croatian is supported) (default: False)
+  * `--run_all_rules`: Run all hardrules for each sentence instead of stopping at the first one discarded. (default: False)
 * Logging:
   * `--debug`: Debug logging mode (default: False)
   * `-q, --quiet`: Silent logging mode (default: False)
   * `-v, --version`: show version of this script and exit
 
 ### Example
 ```bash
@@ -137,47 +148,58 @@
 
 ## Monocleaner hard-rules
 `monocleaner-hardrules` is an optional pre-filtering step for obvious noise based on rules and incorrect language identified by [FastSpell](https://github.com/mbanon/fastspell). It can be used integrated into the `monocleaner` endpoint, or separately.
 
 ### Cleaning
 `monocleaner-hardrules` aims at detecting obvious noisey sentences in a monolingual corpus. Sentences that are considered noisy will be tagged with a `0` and the rest will be tagged with a `1`. By default, the input monolingual file must contain at least one column with the sentences needed to be cleaned. If more columns are present, the column index of the sentences desired to be cleaned can be customized via the `--scol` parameter.
 
-By default, the generated output file will contain the same lines and columns that the original input file has, however, an extra column containing the Monocleaner hard-rules score is added. The amount of newly inserted columns will vary depending on which parameters are enabled.
+By default, the generated output file will contain the same lines and columns that the original input file has, however, an extra column containing the Monocleaner hard-rules score is always added. The amount of newly inserted columns will vary depending on which parameters are enabled.
 
 This tool can be run with:
 ```bash
 monocleaner-hardrules [-h]
             [--scol SCOL]
             [--disable_lang_ident]
             [--disable_minimal_length]
             [--disable_hbs]
             [--score_only]
             [--add_lang_ident]
             [--detect_script]
             [--annotated_output]
+            [--run_all_rules]
             [--debug]
             [-q]
             [-v]
             language [input] [output]
 ```
 
+The output file will contain the following columns which will appear in the strict order indicated below depending on the previous parameters:
+
+| Column | Value            | Parameters                    |
+| ------ | ---------------- | ----------------------------- | 
+|   1    | Sentence         | Disabled by --score_only      |
+|   2    | Score            |  -                            |
+|   3    | Language Code    | Enabled by --add_lang_ident   |
+|   4    | Hardrule Tag     | Enabled by --annotated_output |
+
 ### Parameters
 * Positional arguments:
   * `language`: Language code of corpus in ISO 639-1 format (2-char code).
   * `input`: Input text file, one sentence per line. When omitted jointly with output, it will read from stdin.
   * `output`: Output tab-separated text file adding monocleaner score. When omitted output will be written to stdout.
 * Optional arguments:
   * `--scol`: Sentence column (starting in 1) (default: 1)
   * `--disable_lang_ident`: Disables language identification in hardrules. (default: False)
   * `--disable_minimal_length` : Don't apply minimal length rule (default: False).
   * `--disable_hbs`: Don't group Serbo-Croatian under 'hbs' tag. (default: False)
   * `--score_only`: Only output one column which is the monocleaner score (default: False)
   * `--add_lang_ident`: Add another column with the identified language if it's not disabled. (default: False)
   * `--detect_script`: Detect writing script with FastSpell (only Serbo-Croatian is supported) (default: False)
   * `--annotated_output`: Add hardrules annotation for each sentence. (default: False)
+  * `--run_all_rules`: Run all hardrules for each sentence instead of stopping at the first one discarded. (default: False)
 * Logging:
   * `--debug`: Debug logging mode (default: False)
   * `-q, --quiet`: Silent logging mode (default: False)
   * `-v, --version`: show version of this script and exit
 
 ### Example
 ```bash
```

### Comparing `monocleaner-1.6/README.md` & `monocleaner-1.6.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -73,21 +73,31 @@
             [--disable_hardrules]
             [--disable_minimal_length]
             [--disable_hbs]
             [--score_only]
             [--annotated_output]
             [--add_lang_ident]
             [--detect_script]
+            [--run_all_rules]
             [--debug]
             [-q]
             [-v]
             model_dir [input] [output]
 ```
 If input and output are omitted, it will read from stdin and write to stdout.
 
+The output file will contain the following columns which will appear in the strict order indicated below depending on the previous parameters:
+
+| Column | Value            | Parameters                    |
+| ------ | ---------------- | ----------------------------- | 
+|   1    | Sentence         | Disabled by --score_only      |
+|   2    | Score            |  -                            |
+|   3    | Language Code    | Enabled by --add_lang_ident   |
+|   4    | Hardrule Tag     | Enabled by --annotated_output |
+
 ### Parameters
 * Positional arguments:
   * `model_dir`: Directory where the model is stored.
   * `input`: Input text file, one sentence per line. When omitted jointly with output, it will read from stdin.
   * `output`: Output tab-separated text file adding monocleaner score. When omitted output will be written to stdout.
 * Optional arguments:
   * `--scol`: Sentence column (starting in 1) (default: 1)
@@ -95,14 +105,15 @@
   * `--disable_hardrules`: Disables the hardrules filtering (only monocleaner fluency scoring is applied) (default: False)
   * `--disable_minimal_length` : Don't apply minimal length rule (default: False).
   * `--disable_hbs`: Don't group Serbo-Croatian under 'hbs' tag. (default: False)
   * `--score_only`: Only output one column which is the monocleaner score (default: False)
   * `--annotated_output`: Add hardrules annotation for each sentence. (default: False)
   * `--add_lang_ident`: Add another column with the identified language if it's not disabled. (default: False)
   * `--detect_script`: Detect writing script with FastSpell (only Serbo-Croatian is supported) (default: False)
+  * `--run_all_rules`: Run all hardrules for each sentence instead of stopping at the first one discarded. (default: False)
 * Logging:
   * `--debug`: Debug logging mode (default: False)
   * `-q, --quiet`: Silent logging mode (default: False)
   * `-v, --version`: show version of this script and exit
 
 ### Example
 ```bash
@@ -113,47 +124,58 @@
 
 ## Monocleaner hard-rules
 `monocleaner-hardrules` is an optional pre-filtering step for obvious noise based on rules and incorrect language identified by [FastSpell](https://github.com/mbanon/fastspell). It can be used integrated into the `monocleaner` endpoint, or separately.
 
 ### Cleaning
 `monocleaner-hardrules` aims at detecting obvious noisey sentences in a monolingual corpus. Sentences that are considered noisy will be tagged with a `0` and the rest will be tagged with a `1`. By default, the input monolingual file must contain at least one column with the sentences needed to be cleaned. If more columns are present, the column index of the sentences desired to be cleaned can be customized via the `--scol` parameter.
 
-By default, the generated output file will contain the same lines and columns that the original input file has, however, an extra column containing the Monocleaner hard-rules score is added. The amount of newly inserted columns will vary depending on which parameters are enabled.
+By default, the generated output file will contain the same lines and columns that the original input file has, however, an extra column containing the Monocleaner hard-rules score is always added. The amount of newly inserted columns will vary depending on which parameters are enabled.
 
 This tool can be run with:
 ```bash
 monocleaner-hardrules [-h]
             [--scol SCOL]
             [--disable_lang_ident]
             [--disable_minimal_length]
             [--disable_hbs]
             [--score_only]
             [--add_lang_ident]
             [--detect_script]
             [--annotated_output]
+            [--run_all_rules]
             [--debug]
             [-q]
             [-v]
             language [input] [output]
 ```
 
+The output file will contain the following columns which will appear in the strict order indicated below depending on the previous parameters:
+
+| Column | Value            | Parameters                    |
+| ------ | ---------------- | ----------------------------- | 
+|   1    | Sentence         | Disabled by --score_only      |
+|   2    | Score            |  -                            |
+|   3    | Language Code    | Enabled by --add_lang_ident   |
+|   4    | Hardrule Tag     | Enabled by --annotated_output |
+
 ### Parameters
 * Positional arguments:
   * `language`: Language code of corpus in ISO 639-1 format (2-char code).
   * `input`: Input text file, one sentence per line. When omitted jointly with output, it will read from stdin.
   * `output`: Output tab-separated text file adding monocleaner score. When omitted output will be written to stdout.
 * Optional arguments:
   * `--scol`: Sentence column (starting in 1) (default: 1)
   * `--disable_lang_ident`: Disables language identification in hardrules. (default: False)
   * `--disable_minimal_length` : Don't apply minimal length rule (default: False).
   * `--disable_hbs`: Don't group Serbo-Croatian under 'hbs' tag. (default: False)
   * `--score_only`: Only output one column which is the monocleaner score (default: False)
   * `--add_lang_ident`: Add another column with the identified language if it's not disabled. (default: False)
   * `--detect_script`: Detect writing script with FastSpell (only Serbo-Croatian is supported) (default: False)
   * `--annotated_output`: Add hardrules annotation for each sentence. (default: False)
+  * `--run_all_rules`: Run all hardrules for each sentence instead of stopping at the first one discarded. (default: False)
 * Logging:
   * `--debug`: Debug logging mode (default: False)
   * `-q, --quiet`: Silent logging mode (default: False)
   * `-v, --version`: show version of this script and exit
 
 ### Example
 ```bash
```

### Comparing `monocleaner-1.6/pyproject.toml` & `monocleaner-1.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "monocleaner"
-version = "1.6"
+version = "1.6.1"
 requires-python = ">=3.8"
 authors = [
     { name = "Prompsit Language Engineering", email = "info@prompsit.com" },
 ]
 maintainers = [
     { name = "Jaume Zaragoza", email = "jzaragoza@prompsit.com" },
 ]
```

### Comparing `monocleaner-1.6/scripts/monocleaner-download` & `monocleaner-1.6.1/scripts/monocleaner-download`

 * *Files identical despite different names*

### Comparing `monocleaner-1.6/src/monocleaner/hardrules.py` & `monocleaner-1.6.1/src/monocleaner/hardrules.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from unicodedata import category as cat
 from timeit import default_timer
 from fastspell import FastSpell
+from inspect import getmembers
 import unicodedata
 import argparse
 import logging
 import regex
 import sys
 import re
 import os
@@ -40,278 +41,193 @@
 
 #similar_pairs = [{"es","ca"}, {"es","gl"}, {"pt","gl"}, {"no","nn"}, {"no", "da"}]
 atilde_langs = {"pt"}
 acumflex_langs = {"cy", "fr", "fa", "it", "pt", "tr", "vi",}
 CJK = {"zh", "ja", "ko"}
 
 
-def c_no_empty(args, sentence):
-    return sentence != ""
+class Hardrules():
 
-def c_no_titles(args, sentence):    
-    return not len(sentence.strip().split(" ")) > 1
+    def __init__(self, args):
+        self.language = args.language
+        self.disable_minimal_length = args.disable_minimal_length
+        self.fastspell = args.fastspell
+        self.detect_script = args.detect_script
+        self.disable_lang_ident = args.disable_lang_ident
 
-def c_not_too_long(args, sentence):
-    return len(sentence) < 1024
+        # Get all rule names to be called in a loop as functions
+        self.rules = {n: f for n, f in getmembers(self) if n.startswith('c_')}
 
-def c_not_too_short(args, sentence):
-    if args.disable_minimal_length:
-        return True
+    def c_no_empty(self, sentence):
+        return sentence != ""
 
-    # for Chinese, Japanese and Korean characters rather than words are used
-    if args.language in CJK:
-        return len(sentence) >= 3
-
-    """ Counts number of whitespace, requires >= 2 (3 words) """
-    return len(regex_blank.findall(sentence)) >= 2
-
-def c_lang_id(args, sentence):
-    if not args.disable_lang_ident:
-        # Obtain fastspell prediction, lowercasing helps in small langs
-        langid = args.fastspell.getlang(sentence.lower())
-
-        # Separate langid from the detected script (only Serbo-Croatian is supported)
-        if args.detect_script:
-            langid_no_suffix = langid.split('_')[0]
-        else:
-            langid_no_suffix = langid
-            
-        # Return language identified, else, return args.language
-        if langid_no_suffix != args.language:
-            return langid_no_suffix, False
-    return args.language, True
-
-def c_no_bad_encoding(args, sentence):
-    if args.language not in atilde_langs and 'Ã' in sentence:
-        return False
-    if args.language not in acumflex_langs and 'Â' in sentence:
-        return False
-    return True
-
-def c_no_only_symbols(args, sentence):
-    return len(regex_alpha.findall(sentence)) / len(sentence) > 0.1
-
-def c_no_only_numbers(args, sentence):
-    threshold = 0.5
-    if args.language in CJK:
-        threshold = 0.7
-    return len(regex_numbers.findall(sentence)) / len(sentence) < threshold
-
-def c_no_urls(args, sentence):
-    return len(regex_url.findall(sentence)) == 0
-
-def c_no_breadcrumbs(args, sentence):
-    return len(regex_breadcrumbs1.findall(sentence)) < 3 \
-            or len(regex_breadcrumbs2.findall(sentence)) < 2
-
-def c_no_unicode_noise(args, sentence):
-    # Icelandic can have words with three or four high unicode values like 'þýðir'
-    # Finish sometimes too
-    if args.language in ('is', 'fi'):
-        return len(regex_unicode_noise_relaxed.findall(sentence)) == 0
-    else:
-        return len(regex_unicode_noise.findall(sentence)) == 0
+    def c_no_titles(self, sentence):    
+        return len(sentence.strip().split(" ")) > 1
 
-def c_no_space_noise(args, sentence):
-    return len(regex_spaces_noise.findall(sentence)) == 0
+    def c_not_too_long(self, sentence):
+        return len(sentence) < 1024
 
-def c_no_paren(args, sentence):
-    if len(re.findall(regex_paren, sentence)): #there are parentheses
-        char_count = {i: sentence.count(i) for i in set(sentence)}
-        
-        if (((char_count.get("[") or 0) + (char_count.get("]") or 0)) > 6 ) or (char_count.get("[") or 0) != (char_count.get("]") or 0): #max 6 [ or ], having the same [ and ] 
-            return False            
-        if (((char_count.get("{") or 0) + (char_count.get("}") or 0)) > 6 ) or (char_count.get("{") or 0) != (char_count.get("}") or 0): #max than 6 { or }, having the same { and }
-            return False           
-        if (((char_count.get("⟨") or 0) + (char_count.get("⟩") or 0)) > 6 ) or (char_count.get("⟨") or 0) != (char_count.get("⟩") or 0): #max than 6 ⟨ or ⟩, having the same ⟨ and ⟩            
-            return False
-        
-        opening_paren = char_count.get("(") or 0
-        closing_paren = char_count.get(")") or 0
-        if opening_paren == closing_paren: #any amount of  () is allowed, as long as there are the same amount of  ( and )
+    def c_not_too_short(self, sentence):
+        if self.disable_minimal_length:
             return True
-        else:
-            return False
-    return True    
 
-def c_no_literals(args, sentence):
-    return not any(l in sentence for l in ["Re:","{{", "%s", "}}", "+++", "***", '=\"'])
+        # for Chinese, Japanese and Korean characters rather than words are used
+        if self.language in CJK:
+            return len(sentence) >= 3
 
-def c_no_escaped_unicode(args, sentence):
-    return len(regex_escaped_unicode.findall(sentence)) == 0
+        """ Counts number of whitespace, requires >= 2 (3 words) """
+        return len(regex_blank.findall(sentence)) >= 2
 
-def c_no_glued_words(args, sentence):
-    return regex_glued_words.search(sentence) == None
-
-def c_no_repeated_words(args, sentence):
-    our_regex = regex_repeated_without_words
-    if args.language in safe_noise_detection_langs:
-        our_regex = regex_repeated_words
-
-    min_chars = 7
-    if args.language in CJK:
-        min_chars = 4
-
-    count = 0
-    for match_obj in regex.finditer(our_regex, sentence):
-        matching = match_obj.group().strip()
-        # if match does not have a minimum length continue without discarding
-        if len(matching) > min_chars:
-            r2 = regex.search("[[:alpha:]]", matching)
-            if r2:
-                # if a certain count of repeated patterns has been reached, then return False
-                count += 1
-                if count >= 1:
-                    return False
+    def c_no_bad_encoding(self, sentence):
+        if self.language not in atilde_langs and 'Ã' in sentence:
+            return False
+        if self.language not in acumflex_langs and 'Â' in sentence:
+            return False
+        return True
 
-    return True
+    def c_no_only_symbols(self, sentence):
+        return len(regex_alpha.findall(sentence)) / len(sentence) > 0.1
 
-'''
-def c_different_language(left, right, left_lang, right_lang):
-    if left_lang =="nb":
-        left_lang="no"
+    def c_no_only_numbers(self, sentence):
+        threshold = 0.5
+        if self.language in CJK:
+            threshold = 0.7
+        return len(regex_numbers.findall(sentence)) / len(sentence) < threshold
+
+    def c_no_urls(self, sentence):
+        return len(regex_url.findall(sentence)) == 0
+
+    def c_no_breadcrumbs(self, sentence):
+        return len(regex_breadcrumbs1.findall(sentence)) < 3 \
+                or len(regex_breadcrumbs2.findall(sentence)) < 2
+
+    def c_no_unicode_noise(self, sentence):
+        # Icelandic can have words with three or four high unicode values like 'þýðir'
+        # Finish sometimes too
+        if self.language in ('is', 'fi'):
+            return len(regex_unicode_noise_relaxed.findall(sentence)) == 0
+        else:
+            return len(regex_unicode_noise.findall(sentence)) == 0
 
-    if right_lang=="nb":
-        right_lang="no"
-        
+    def c_no_space_noise(self, sentence):
+        return len(regex_spaces_noise.findall(sentence)) == 0
+
+    def c_no_paren(self, sentence):
+        if len(re.findall(regex_paren, sentence)): #there are parentheses
+            char_count = {i: sentence.count(i) for i in set(sentence)}
+            
+            if (((char_count.get("[") or 0) + (char_count.get("]") or 0)) > 6 ) or (char_count.get("[") or 0) != (char_count.get("]") or 0): #max 6 [ or ], having the same [ and ] 
+                return False            
+            if (((char_count.get("{") or 0) + (char_count.get("}") or 0)) > 6 ) or (char_count.get("{") or 0) != (char_count.get("}") or 0): #max than 6 { or }, having the same { and }
+                return False           
+            if (((char_count.get("⟨") or 0) + (char_count.get("⟩") or 0)) > 6 ) or (char_count.get("⟨") or 0) != (char_count.get("⟩") or 0): #max than 6 ⟨ or ⟩, having the same ⟨ and ⟩            
+                return False
+            
+            opening_paren = char_count.get("(") or 0
+            closing_paren = char_count.get(")") or 0
+            if opening_paren == closing_paren: #any amount of  () is allowed, as long as there are the same amount of  ( and )
+                return True
+            else:
+                return False
+        return True    
+
+    def c_no_literals(self, sentence):
+        return not any(l in sentence for l in ["Re:","{{", "%s", "}}", "+++", "***", '=\"'])
+
+    def c_no_escaped_unicode(self, sentence):
+        return len(regex_escaped_unicode.findall(sentence)) == 0
+
+    def c_no_glued_words(self, sentence):
+        return regex_glued_words.search(sentence) == None
+
+    def c_no_repeated_words(self, sentence):
+        our_regex = regex_repeated_without_words
+        if self.language in safe_noise_detection_langs:
+            our_regex = regex_repeated_words
+
+        min_chars = 7
+        if self.language in CJK:
+            min_chars = 4
+
+        count = 0
+        for match_obj in regex.finditer(our_regex, sentence):
+            matching = match_obj.group().strip()
+            # if match does not have a minimum length continue without discarding
+            if len(matching) > min_chars:
+                r2 = regex.search("[[:alpha:]]", matching)
+                if r2:
+                    # if a certain count of repeated patterns has been reached, then return False
+                    count += 1
+                    if count >= 1:
+                        return False
 
-    l_reliable = False
-    l_bytes = 0
-    l_details = ()
- 
-    try:
-        l_reliable, l_bytes, l_details = pycld2.detect(left)
-    except:
-        return False # encoding error -> noise
-
-    r_reliable = False
-    r_bytes = 0
-    r_details = ()
-
-    try:
-        r_reliable, r_bytes, r_details = pycld2.detect(right)
-    except:
-        return False # encoding error -> noise
-        
-    if l_reliable and r_reliable and l_details[0][1] != r_details[0][1]:    
-        return True
-    elif not l_reliable or not r_reliable:
-        return True
-    else:
-        #both langs are reliable at this point, and the identified language is the same for left and right
-        identified = l_details[0][1]
-        if (identified in [left_lang, right_lang]  and {left_lang, right_lang} in similar_pairs):
-            return True
-        else:    
-            return False
-'''
-'''        
-def c_reliable_long_language(sentence, language):
-    if language=="nb":
-        language = "no"
-        
-    reliable = False
-    bytes = 0
-    details = ()
-    
-    try:
-        reliable, bytes, details = pycld2.detect(sentence)
-    except:
-        return True # encoding error -> noise
-    
-    if len(sentence) > 30 and reliable and details[0][1] != language:
-        if {language, details[0][1]} in similar_pairs:
-            return True
-        else:
-            return False
-    else:
         return True
-'''
+
+    def z_no_wrong_language(self, sentence):
+        if not self.disable_lang_ident:
+            # Obtain fastspell prediction, lowercasing helps in small langs
+            langid = self.fastspell.getlang(sentence.lower())
+
+            # Separate langid from the detected script (only Serbo-Croatian is supported)
+            if self.detect_script:
+                langid_no_suffix = langid.split('_')[0]
+            else:
+                langid_no_suffix = langid
+                
+            # Return language identified, else, return self.language
+            if langid_no_suffix != self.language:
+                return langid_no_suffix, False
+        return self.language, True
+
+    def wrong_segment(self, args, sentence):
+        if args.disable_hardrules:
+            return 'keep'
+
+        discarded = []
+
+        for rule_name in self.rules:
+            rule = getattr(self, rule_name)
+            result = rule(sentence)
+
+            # If rule applied fails, then only add the rule name to discarded
+            if not result:
+                discarded.append(rule_name.replace('c_', '', 1))
+            
+            # If user doesn't want to run all rules, stop after the first one that fails
+            if not result and not args.run_all_rules:
+                return ''.join(discarded)
+
+        if discarded == []:
+            return 'keep'
+        return '+'.join(discarded)
 
 '''
 def c_unwanted(sentence):
     return len(regex_unwanted.findall(sentence)) < 5
 
 def c_inconditional(sentence):
     return len(regex_inconditional.findall(sentence)) < 1
 
 '''
 
 
-def wrong_segment(sentence, args, hardrules_call = False):
-    '''
-    elif not c_unwanted(sent):
-        return "c_unwanted"
-    elif not c_inconditional(sent):
-        return "c_inconditional"
-    '''
-    
-    if args.disable_hardrules:
-        return "keep"
-
-    if not c_no_empty(args, sentence):
-        return 'no_empty'
-    elif c_no_titles(args, sentence):
-        return 'no_titles'
-    elif not c_not_too_long(args, sentence):
-        return 'not_too_long'
-    elif not c_not_too_short(args, sentence):
-        return 'not_too_short'
-    elif not c_no_bad_encoding(args, sentence):
-        return 'no_bad_encoding'
-    elif not c_no_only_symbols(args, sentence):
-        return 'no_only_symbols'
-    elif not c_no_only_numbers(args, sentence):
-        return 'no_only_numbers'
-    elif not c_no_urls(args, sentence):
-        return 'no_urls'
-    elif not c_no_breadcrumbs(args, sentence):
-        return 'no_breadcrumbs'
-    elif not c_no_unicode_noise(args, sentence):
-        return 'no_unicode_noise'
-    elif not c_no_space_noise(args, sentence):
-        return 'no_space_noise'
-    elif not c_no_paren(args, sentence):
-        return 'no_paren'
-    elif not c_no_literals(args, sentence):
-        return 'no_literals'
-    elif not c_no_escaped_unicode(args, sentence):
-        return 'no_escaped_unicode'
-    elif not c_no_glued_words(args, sentence):
-        return 'no_glued_words'
-    elif not c_no_repeated_words(args, sentence):
-        return 'no_repeated_words'
-
-    # Language identification is done only if it is enabled and 
-    # the call is being made from the hardrules endpoint
-    if hardrules_call and not args.disable_lang_ident:
-        langid, fails_lang = c_lang_id(args, sentence)
-        if not fails_lang:
-            return langid, 'c_wrong_language'
-
-    return "keep"
-
-
-
-
-
-
 def initialization():
     parser = argparse.ArgumentParser()
     parser.add_argument("language", type=str, help="Language code of corpus in ISO 639-1 format (2-char code).")
     parser.add_argument("input", type=argparse.FileType('r'), nargs='?', help="Input file. If omitted, read from 'stdin'.")
     parser.add_argument("output", type=argparse.FileType('w'), nargs='?', help="Output tab-separated text file adding monocleaner score. When omitted output will be written to stdout.")
     parser.add_argument("--scol", default=1, type=check_positive, help ="Sentence column (starting in 1)")
     parser.add_argument("--disable_lang_ident", action='store_true', help="Disables language identification in hardrules")
     parser.add_argument("--disable_minimal_length", action='store_true', help="Don't apply minimal length (3 words) rule")
     parser.add_argument("--disable_hbs", action='store_true', help="Don't group Serbo-Croatian under 'hbs' tag")
     parser.add_argument("--score_only", action='store_true', help="Only print the score for each sentence, omit all fields")
     parser.add_argument("--add_lang_ident", action='store_true', help="Add another column with the identified language if it's not disabled")
     parser.add_argument("--detect_script", action='store_true', help="Detect writing script with FastSpell (only Serbo-Croatian is supported)")
     parser.add_argument("--annotated_output", action='store_true', help="Add hardrules annotation for each sentence")
+    parser.add_argument("--run_all_rules", action='store_true', help="Run all hardrules for each sentence instead of stopping at the first one discarded")
     parser.add_argument("--debug", action='store_true')
     parser.add_argument("-q", "--quiet", action='store_true')
     parser.add_argument('-v', '--version', action='version', version="%(prog)s " + __version__, help="show version of this script and exit")
 
     args = parser.parse_args()
 
     if args.output == None:
@@ -324,65 +240,85 @@
     
     if args.disable_lang_ident:
         args.fastspell = None
     else:
         args.fastspell = FastSpell(args.language, mode="aggr",
                                     hbs=not args.disable_hbs,
                                     script=args.detect_script)
+        
+    # Language identification sanity checks
+    if args.disable_lang_ident:
+        args.add_lang_ident = False
+    else:
+        if args.add_lang_ident:
+            args.disable_lang_ident = False
     
     # This is just to skip over the disable_hardrules parameter
-    # that can be enabled from the monocleaner endpoint
+    # which can be enabled only from the monocleaner endpoint
     args.disable_hardrules = False
     
     return args
 
 def main():
     args = initialization()
     
     time_start = default_timer()
     logging.info("Start hardruling text")
     
+    # TODO: add wrong_segment as method in hardrules
+    hardrules = Hardrules(args)
+    
     nline = 0
     for line in args.input:
         nline += 1
         parts = line.rstrip("\n").split("\t")
 
         if len(parts) >= args.scol:
             sentence = parts[args.scol-1]
         else:
             logging.error(f" scol ({args.scol}) index above column number ({len(parts)}) on line {nline}")
             continue
         
-        hr_result = wrong_segment(line, args, hardrules_call = True)
-        langid = args.language
+        hr_result = hardrules.wrong_segment(args, sentence)
         tag = hr_result
+        langid = args.language
         
-        # Language identification output
-        if type(hr_result) is tuple:
-            langid = hr_result[0]
-            tag = hr_result[1]
-        
-        #print("{} - {} - {}".format(type(hr_result), langid, tag))
+        # Language identification rule and output
+        if not args.disable_lang_ident:
+            # If run all rules is enabled, run the identification method.
+            # If it doesn't pass, then set the tag accordingly if other hardrules have failed.
+            if args.run_all_rules:
+                langid, res = hardrules.z_no_wrong_language(line)
+
+                if not res:
+                    if tag == 'keep':
+                        tag = 'no_wrong_language'
+                    else:
+                        tag += '+no_wrong_language'
+            else:
+                # If run all rules is disabled, then only run identification method when all other hardrules have passed
+                if tag == 'keep':
+                    langid, res = hardrules.z_no_wrong_language(line)
+                    
+                    if not res:
+                        tag = 'no_wrong_language'
         
         score = 1
         if tag != "keep":
             score = 0
         
-        # print score
         # print sentence when no score_only
-        # print hardrule annotation if requested
+        # print score
         # print identified language if requested
+        # print hardrule annotation if requested
         if not args.score_only:
             args.output.write(line.rstrip("\n") + '\t')
-        if tag != "keep":
-            args.output.write(f"{score}")
+        args.output.write("{0}".format(score))
         if args.add_lang_ident:
             args.output.write('\t' + langid)
-        else:
-            args.output.write(f"{score:.3f}")
         if args.annotated_output:
             args.output.write('\t' + tag)
         args.output.write("\n")
         
     # Print elapsed time and avg speed
     logging.info("Finished")
     elapsed_time = default_timer() - time_start
```

### Comparing `monocleaner-1.6/src/monocleaner/lm.py` & `monocleaner-1.6.1/src/monocleaner/lm.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.6/src/monocleaner/monocleaner.py` & `monocleaner-1.6.1/src/monocleaner/monocleaner.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 import sys
 import os
 
 try:
     from . import __version__
     from .lm import *
     from .util import logging_setup, check_if_folder, check_positive
-    from .hardrules import wrong_segment
+    from .hardrules import Hardrules
 except (SystemError, ImportError):
     from monocleaner import __version__
     from lm import *
     from util import logging_setup, check_if_folder, check_positive
-    from hardrules import wrong_segment
+    from hardrules import Hardrules
 
 def initialization():
     parser = ArgumentParser()
     parser.add_argument("model_dir", type=check_if_folder, help="Model directory to store LM file and metadata.")
     parser.add_argument("input", type=argparse.FileType('r'), nargs='?', help="Input file. If omitted, read from 'stdin'.")
     parser.add_argument("output", type=argparse.FileType('w'), nargs='?', help="Output tab-separated text file adding monocleaner score. When omitted output will be written to stdout.")
     parser.add_argument("--scol", default=1, type=check_positive, help ="Sentence column (starting in 1)")
@@ -27,25 +27,33 @@
     parser.add_argument("--disable_hardrules", action='store_true', help='Disables the hardrules filtering (only monocleaner fluency scoring is applied)')
     parser.add_argument("--disable_minimal_length", action='store_true', help="Don't apply minimal length (3 words) rule")
     parser.add_argument("--disable_hbs", action='store_true', help="Don't group Serbo-Croatian under 'hbs' tag")
     parser.add_argument("--score_only", action='store_true', help="Only print the score for each sentence, omit all fields")
     parser.add_argument("--add_lang_ident", action='store_true', help="Add another column with the identified language if it's not disabled")
     parser.add_argument("--detect_script", action='store_true', help="Detect writing script with FastSpell (only Serbo-Croatian is supported)")
     parser.add_argument("--annotated_output", action='store_true', help="Add hardrules annotation for each sentence")
+    parser.add_argument("--run_all_rules", action='store_true', help="Run all hardrules for each sentence instead of stopping at the first one discarded")
     parser.add_argument("--debug", action='store_true')
     parser.add_argument("-q", "--quiet", action='store_true')
     parser.add_argument('-v', '--version', action='version', version="%(prog)s " + __version__, help="show version of this script and exit")
 
     args = parser.parse_args()
 
     args.metadata = args.model_dir + '/metadata.yaml'
     if args.output == None:
         args.output = sys.stdout
     if args.input == None:
         args.input = sys.stdin
+        
+    # Language identification sanity checks
+    if args.disable_lang_ident:
+        args.add_lang_ident = False
+    else:
+        if args.add_lang_ident:
+            args.disable_lang_ident = False
 
     logging_setup(args)
     load_model(args)
     logging.debug(args)
     return args
 
 def load_model(args):
@@ -76,26 +84,29 @@
 
 def perform_scoring(args):
     time_start = default_timer()
     logging.info("Start scoring text")
 
     nline = 0
     langid = None
+    
+    hardrules = Hardrules(args)
+    
     for line in args.input:
         nline += 1
         parts = line.rstrip("\n").split("\t")
 
         if len(parts) >= args.scol:
             sentence = parts[args.scol-1]
         else:
             logging.error(f" scol ({args.scol}) index above column number ({len(parts)}) on line {nline}")
             continue
 
         # Obtain hardrules tag
-        tag = wrong_segment(sentence, args)
+        tag = hardrules.wrong_segment(args, sentence)
 
         # Language identification
         # Only run if not disabled or not discarded or if it's requested in the output
         if not args.disable_lang_ident and (args.add_lang_ident or tag == 'keep'):
             # Obtain fastspell prediction, lowercasing helps in small langs
             langid = args.fastspell.getlang(sentence.lower())
 
@@ -104,36 +115,42 @@
                 langid_no_suffix = langid.split('_')[0]
             else:
                 langid_no_suffix = langid
 
             # Hardrule of langident here, to avoid calling fastspell two times
             # have the language prediction available to print it
             if not args.disable_hardrules \
-                    and tag == "keep" \
                     and langid_no_suffix != args.language:
-                tag = 'c_wrong_language'
+                if args.run_all_rules:
+                    if tag == 'keep':
+                        tag = 'no_wrong_language'
+                    else:
+                        tag += '+no_wrong_language'
+                else:
+                    if tag == 'keep':
+                        tag = 'no_wrong_language'
 
         # Score with lm non discarded sentences
         if tag == "keep":
             score = args.ff.score(sentence)
         else:
             score = 0
 
-        # always print score
         # print sentence when no score_only
-        # print hardrule annotation if requested
+        # always print score
         # print identified language if requested
+        # print hardrule annotation if requested
         if not args.score_only:
             args.output.write(line.rstrip("\n") + '\t')
-        if args.add_lang_ident:
-            args.output.write(langid + '\t')
         if tag != "keep":
             args.output.write(f"{score}")
         else:
             args.output.write(f"{score:.3f}")
+        if args.add_lang_ident:
+            args.output.write('\t' + langid)
         if args.annotated_output:
             args.output.write('\t' + tag)
         args.output.write("\n")
 
     # Print elapsed time and avg speed
     logging.info("Finished")
     elapsed_time = default_timer() - time_start
```

### Comparing `monocleaner-1.6/src/monocleaner/monocleaner_train.py` & `monocleaner-1.6.1/src/monocleaner/monocleaner_train.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.6/src/monocleaner/normalize.py` & `monocleaner-1.6.1/src/monocleaner/normalize.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.6/src/monocleaner/tokenizer.py` & `monocleaner-1.6.1/src/monocleaner/tokenizer.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.6/src/monocleaner/util.py` & `monocleaner-1.6.1/src/monocleaner/util.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.6/src/monocleaner.egg-info/PKG-INFO` & `monocleaner-1.6.1/src/monocleaner.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monocleaner
-Version: 1.6
+Version: 1.6.1
 Summary: Monolingual corpus fluency filter
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License: GNU General Public License v3.0
 Project-URL: Homepage, https://github.com/bitextor/monocleaner
 Project-URL: Monocleaner on GitHub, https://github.com/bitextor/monocleaner
 Project-URL: Prompsit Language Engineering, http://www.prompsit.com
@@ -97,21 +97,31 @@
             [--disable_hardrules]
             [--disable_minimal_length]
             [--disable_hbs]
             [--score_only]
             [--annotated_output]
             [--add_lang_ident]
             [--detect_script]
+            [--run_all_rules]
             [--debug]
             [-q]
             [-v]
             model_dir [input] [output]
 ```
 If input and output are omitted, it will read from stdin and write to stdout.
 
+The output file will contain the following columns which will appear in the strict order indicated below depending on the previous parameters:
+
+| Column | Value            | Parameters                    |
+| ------ | ---------------- | ----------------------------- | 
+|   1    | Sentence         | Disabled by --score_only      |
+|   2    | Score            |  -                            |
+|   3    | Language Code    | Enabled by --add_lang_ident   |
+|   4    | Hardrule Tag     | Enabled by --annotated_output |
+
 ### Parameters
 * Positional arguments:
   * `model_dir`: Directory where the model is stored.
   * `input`: Input text file, one sentence per line. When omitted jointly with output, it will read from stdin.
   * `output`: Output tab-separated text file adding monocleaner score. When omitted output will be written to stdout.
 * Optional arguments:
   * `--scol`: Sentence column (starting in 1) (default: 1)
@@ -119,14 +129,15 @@
   * `--disable_hardrules`: Disables the hardrules filtering (only monocleaner fluency scoring is applied) (default: False)
   * `--disable_minimal_length` : Don't apply minimal length rule (default: False).
   * `--disable_hbs`: Don't group Serbo-Croatian under 'hbs' tag. (default: False)
   * `--score_only`: Only output one column which is the monocleaner score (default: False)
   * `--annotated_output`: Add hardrules annotation for each sentence. (default: False)
   * `--add_lang_ident`: Add another column with the identified language if it's not disabled. (default: False)
   * `--detect_script`: Detect writing script with FastSpell (only Serbo-Croatian is supported) (default: False)
+  * `--run_all_rules`: Run all hardrules for each sentence instead of stopping at the first one discarded. (default: False)
 * Logging:
   * `--debug`: Debug logging mode (default: False)
   * `-q, --quiet`: Silent logging mode (default: False)
   * `-v, --version`: show version of this script and exit
 
 ### Example
 ```bash
@@ -137,47 +148,58 @@
 
 ## Monocleaner hard-rules
 `monocleaner-hardrules` is an optional pre-filtering step for obvious noise based on rules and incorrect language identified by [FastSpell](https://github.com/mbanon/fastspell). It can be used integrated into the `monocleaner` endpoint, or separately.
 
 ### Cleaning
 `monocleaner-hardrules` aims at detecting obvious noisey sentences in a monolingual corpus. Sentences that are considered noisy will be tagged with a `0` and the rest will be tagged with a `1`. By default, the input monolingual file must contain at least one column with the sentences needed to be cleaned. If more columns are present, the column index of the sentences desired to be cleaned can be customized via the `--scol` parameter.
 
-By default, the generated output file will contain the same lines and columns that the original input file has, however, an extra column containing the Monocleaner hard-rules score is added. The amount of newly inserted columns will vary depending on which parameters are enabled.
+By default, the generated output file will contain the same lines and columns that the original input file has, however, an extra column containing the Monocleaner hard-rules score is always added. The amount of newly inserted columns will vary depending on which parameters are enabled.
 
 This tool can be run with:
 ```bash
 monocleaner-hardrules [-h]
             [--scol SCOL]
             [--disable_lang_ident]
             [--disable_minimal_length]
             [--disable_hbs]
             [--score_only]
             [--add_lang_ident]
             [--detect_script]
             [--annotated_output]
+            [--run_all_rules]
             [--debug]
             [-q]
             [-v]
             language [input] [output]
 ```
 
+The output file will contain the following columns which will appear in the strict order indicated below depending on the previous parameters:
+
+| Column | Value            | Parameters                    |
+| ------ | ---------------- | ----------------------------- | 
+|   1    | Sentence         | Disabled by --score_only      |
+|   2    | Score            |  -                            |
+|   3    | Language Code    | Enabled by --add_lang_ident   |
+|   4    | Hardrule Tag     | Enabled by --annotated_output |
+
 ### Parameters
 * Positional arguments:
   * `language`: Language code of corpus in ISO 639-1 format (2-char code).
   * `input`: Input text file, one sentence per line. When omitted jointly with output, it will read from stdin.
   * `output`: Output tab-separated text file adding monocleaner score. When omitted output will be written to stdout.
 * Optional arguments:
   * `--scol`: Sentence column (starting in 1) (default: 1)
   * `--disable_lang_ident`: Disables language identification in hardrules. (default: False)
   * `--disable_minimal_length` : Don't apply minimal length rule (default: False).
   * `--disable_hbs`: Don't group Serbo-Croatian under 'hbs' tag. (default: False)
   * `--score_only`: Only output one column which is the monocleaner score (default: False)
   * `--add_lang_ident`: Add another column with the identified language if it's not disabled. (default: False)
   * `--detect_script`: Detect writing script with FastSpell (only Serbo-Croatian is supported) (default: False)
   * `--annotated_output`: Add hardrules annotation for each sentence. (default: False)
+  * `--run_all_rules`: Run all hardrules for each sentence instead of stopping at the first one discarded. (default: False)
 * Logging:
   * `--debug`: Debug logging mode (default: False)
   * `-q, --quiet`: Silent logging mode (default: False)
   * `-v, --version`: show version of this script and exit
 
 ### Example
 ```bash
```

### Comparing `monocleaner-1.6/src/monocleaner.egg-info/SOURCES.txt` & `monocleaner-1.6.1/src/monocleaner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

