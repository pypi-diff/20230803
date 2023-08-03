# Comparing `tmp/packg-0.2.24.tar.gz` & `tmp/packg-0.2.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packg-0.2.24.tar", last modified: Fri Jul 14 12:43:23 2023, max compression
+gzip compressed data, was "packg-0.2.25.tar", last modified: Thu Aug  3 07:25:43 2023, max compression
```

## Comparing `packg-0.2.24.tar` & `packg-0.2.25.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:43:23.518693 packg-0.2.24/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.24/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-14 12:43:23.518693 packg-0.2.24/PKG-INFO
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-07-14 12:42:57.000000 packg-0.2.24/README.md
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2337 2023-07-06 08:44:58.000000 packg-0.2.24/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-14 12:42:57.000000 packg-0.2.24/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-07-14 12:43:23.518693 packg-0.2.24/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:43:23.430691 packg-0.2.24/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:43:23.474692 packg-0.2.24/src/packg/
--rw-------   0 gings    (14999) lmb-mit   (1061)      129 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/__init__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      120 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/__main__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3097 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/caching.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5871 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/constclass.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      544 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/debugging.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/dtime.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     8439 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/import_from_source.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:43:23.510693 packg-0.2.24/src/packg/iotools/
--rw-------   0 gings    (14999) lmb-mit   (1061)      794 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/iotools/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/iotools/compressed.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      457 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/iotools/gitmatcher.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     6252 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/iotools/jsonext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    10990 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/iotools/jsonext_encoder.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4027 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/iotools/misc.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4890 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/iotools/yamlext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5948 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/log.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/misc.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2394 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/packaging.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2698 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/paths.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:43:23.514693 packg-0.2.24/src/packg/run/
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3626 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/run/syncjupytext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5507 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/strings.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1968 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/system.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1407 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/tensors.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/typext.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:43:23.494692 packg-0.2.24/src/packg.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-14 12:43:23.000000 packg-0.2.24/src/packg.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      808 2023-07-14 12:43:23.000000 packg-0.2.24/src/packg.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-07-14 12:43:23.000000 packg-0.2.24/src/packg.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-14 12:43:23.000000 packg-0.2.24/src/packg.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-07-14 12:43:23.000000 packg-0.2.24/src/packg.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.24/src/packg.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 07:25:43.306107 packg-0.2.25/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.25/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-08-03 07:25:43.302107 packg-0.2.25/PKG-INFO
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-08-03 07:24:35.000000 packg-0.2.25/README.md
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2337 2023-07-06 08:44:58.000000 packg-0.2.25/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-08-03 07:24:35.000000 packg-0.2.25/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-08-03 07:25:43.306107 packg-0.2.25/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 07:25:43.098103 packg-0.2.25/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 07:25:43.210105 packg-0.2.25/src/packg/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      129 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/__init__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      120 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/__main__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3097 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/caching.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5871 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/constclass.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      544 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/debugging.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/dtime.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     8439 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/import_from_source.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 07:25:43.270106 packg-0.2.25/src/packg/iotools/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      794 2023-08-03 07:24:35.000000 packg-0.2.25/src/packg/iotools/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-08-03 07:24:35.000000 packg-0.2.25/src/packg/iotools/compressed.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      457 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/iotools/gitmatcher.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     6252 2023-08-03 07:24:35.000000 packg-0.2.25/src/packg/iotools/jsonext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    10990 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/iotools/jsonext_encoder.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4027 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/iotools/misc.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4890 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/iotools/yamlext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5959 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/log.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/misc.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2394 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/packaging.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2698 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/paths.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 07:25:43.282106 packg-0.2.25/src/packg/run/
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3626 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/run/syncjupytext.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 07:25:43.298107 packg-0.2.25/src/packg/strings/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      284 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/strings/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4842 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/strings/abbreviations.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1933 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/strings/base64utils.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      623 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/strings/quote_urlparse.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1968 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/system.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1407 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/tensors.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-08-03 07:24:34.000000 packg-0.2.25/src/packg/typext.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-08-03 07:25:43.234105 packg-0.2.25/src/packg.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-08-03 07:25:43.000000 packg-0.2.25/src/packg.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      921 2023-08-03 07:25:43.000000 packg-0.2.25/src/packg.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-08-03 07:25:43.000000 packg-0.2.25/src/packg.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-08-03 07:25:43.000000 packg-0.2.25/src/packg.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-08-03 07:25:43.000000 packg-0.2.25/src/packg.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.25/src/packg.egg-info/zip-safe
```

### Comparing `packg-0.2.24/LICENSE` & `packg-0.2.25/LICENSE`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/PKG-INFO` & `packg-0.2.25/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.24
+Version: 0.2.25
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.24 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.25 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.24/README.md` & `packg-0.2.25/README.md`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/pyproject.toml` & `packg-0.2.25/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/caching.py` & `packg-0.2.25/src/packg/caching.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/constclass.py` & `packg-0.2.25/src/packg/constclass.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/debugging.py` & `packg-0.2.25/src/packg/debugging.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/import_from_source.py` & `packg-0.2.25/src/packg/import_from_source.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/iotools/__init__.py` & `packg-0.2.25/src/packg/iotools/__init__.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/iotools/jsonext.py` & `packg-0.2.25/src/packg/iotools/jsonext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/iotools/jsonext_encoder.py` & `packg-0.2.25/src/packg/iotools/jsonext_encoder.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/iotools/misc.py` & `packg-0.2.25/src/packg/iotools/misc.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/iotools/yamlext.py` & `packg-0.2.25/src/packg/iotools/yamlext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/log.py` & `packg-0.2.25/src/packg/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     logger_config = {"handlers": handlers, **kwargs}
     logger.configure(**logger_config)
     global global_logger_config
     global_logger_config = logger_config
     return logger_config
 
 
-def reroute_logger(new_sink, logger_config=None, handler_num: int = 0) -> None:
+def reroute_logger(new_sink=sys.stderr, logger_config=None, handler_num: int = 0) -> None:
     """
     Reroute a sink from one target to another. Useful for proper logging inside
     a tqdm progressbar without having to recreate the entire logger.
 
     Args:
         new_sink: new target
         logger_config: config created by configure_logger() function above.
```

### Comparing `packg-0.2.24/src/packg/packaging.py` & `packg-0.2.25/src/packg/packaging.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/paths.py` & `packg-0.2.25/src/packg/paths.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/run/syncjupytext.py` & `packg-0.2.25/src/packg/run/syncjupytext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/strings.py` & `packg-0.2.25/src/packg/strings/abbreviations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,13 @@
-import urllib.parse
 from collections import defaultdict
 from copy import deepcopy
 from typing import List, Dict, Tuple
 
 
-def quote_with_urlparse(sentence: str, prefix="q") -> str:
-    """
-    Quote the input s.t. it is safe for using in a URL.
-    Useful also for e.g. using the input
-    as file names.
-
-    Args:
-        sentence: input string
-        prefix: prefix to add to the quoted string, useful to avoid the empty result
-
-    Returns:
-        quoted string
-    """
-
-    quoted = urllib.parse.quote(sentence, safe="")
-    return f"{prefix}{quoted}"
-
-
-def unquote_with_urlparse(sentence: str, prefix="q") -> str:
-    sentence_no_prefix = sentence[len(prefix) :]
-    return urllib.parse.unquote(sentence_no_prefix)
-
-
-def create_unique_abbreviations(
-    input_strings: List[str], seps=("_", ".")
-) -> Dict[str, str]:
+def create_unique_abbreviations(input_strings: List[str], seps=("_", ".")) -> Dict[str, str]:
     """
 
     Old version, splits input strings at "_" and "." and takes first letter of each word.
 
     lg         run.list_gpus
     pcbs       run.packaging.create_build_scripts
 
@@ -62,17 +36,15 @@
                     abbreviation = new_abbreviation
                     break
                 i += 1
         abbreviations[abbreviation] = name
     return abbreviations
 
 
-def create_nested_abbreviations(
-    input_strings: List[str], sep_dir="."
-) -> Dict[str, str]:
+def create_nested_abbreviations(input_strings: List[str], sep_dir=".") -> Dict[str, str]:
     """
     New version, keep the directory nesting and use minimal amount of letters
 
     l          run.list_gpus
     p.c        run.packaging.create_build_scripts
 
     Args:
@@ -145,15 +117,13 @@
             sub_stem_short = f"{stem_short}.{short_key}"
             sub_stem_long = f"{stem_long}.{long_key}"
             if key_is_leaf[long_key]:
                 # leaf node, return the short and long total stems
                 return_strs.append((sub_stem_short, sub_stem_long))
                 continue
             # non-leaf node, recurse
-            sub_strs = _recursive_shortcuts(
-                dct_in[long_key], sub_stem_short, sub_stem_long
-            )
+            sub_strs = _recursive_shortcuts(dct_in[long_key], sub_stem_short, sub_stem_long)
             return_strs.extend(sub_strs)
         return return_strs
 
     # finally cut the first "." and return the dict
     return {s[1:]: l[1:] for s, l in _recursive_shortcuts(dct)}
```

### Comparing `packg-0.2.24/src/packg/system.py` & `packg-0.2.25/src/packg/system.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/tensors.py` & `packg-0.2.25/src/packg/tensors.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg/typext.py` & `packg-0.2.25/src/packg/typext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.24/src/packg.egg-info/PKG-INFO` & `packg-0.2.25/src/packg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.24
+Version: 0.2.25
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.24 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.25 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.24/src/packg.egg-info/SOURCES.txt` & `packg-0.2.25/src/packg.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 src/packg/debugging.py
 src/packg/dtime.py
 src/packg/import_from_source.py
 src/packg/log.py
 src/packg/misc.py
 src/packg/packaging.py
 src/packg/paths.py
-src/packg/strings.py
 src/packg/system.py
 src/packg/tensors.py
 src/packg/typext.py
 src/packg.egg-info/PKG-INFO
 src/packg.egg-info/SOURCES.txt
 src/packg.egg-info/dependency_links.txt
 src/packg.egg-info/requires.txt
@@ -26,8 +25,12 @@
 src/packg/iotools/__init__.py
 src/packg/iotools/compressed.py
 src/packg/iotools/gitmatcher.py
 src/packg/iotools/jsonext.py
 src/packg/iotools/jsonext_encoder.py
 src/packg/iotools/misc.py
 src/packg/iotools/yamlext.py
-src/packg/run/syncjupytext.py
+src/packg/run/syncjupytext.py
+src/packg/strings/__init__.py
+src/packg/strings/abbreviations.py
+src/packg/strings/base64utils.py
+src/packg/strings/quote_urlparse.py
```

