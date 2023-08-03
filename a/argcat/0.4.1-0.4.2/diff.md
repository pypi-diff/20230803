# Comparing `tmp/argcat-0.4.1.tar.gz` & `tmp/argcat-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argcat-0.4.1.tar", last modified: Sat Feb 18 11:09:52 2023, max compression
+gzip compressed data, was "argcat-0.4.2.tar", last modified: Thu Aug  3 01:41:04 2023, max compression
```

## Comparing `argcat-0.4.1.tar` & `argcat-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 chx1n      (501) staff       (20)        0 2023-02-18 11:09:52.155099 argcat-0.4.1/
--rw-r--r--   0 chx1n      (501) staff       (20)     1066 2022-12-04 13:58:38.000000 argcat-0.4.1/LICENSE
--rw-r--r--   0 chx1n      (501) staff       (20)     9822 2023-02-18 11:09:52.155162 argcat-0.4.1/PKG-INFO
--rw-r--r--   0 chx1n      (501) staff       (20)     9332 2022-12-04 13:58:38.000000 argcat-0.4.1/README.md
--rw-r--r--   0 chx1n      (501) staff       (20)      103 2022-12-04 14:03:46.000000 argcat-0.4.1/pyproject.toml
--rw-r--r--   0 chx1n      (501) staff       (20)      614 2023-02-18 11:09:52.155545 argcat-0.4.1/setup.cfg
-drwxr-xr-x   0 chx1n      (501) staff       (20)        0 2023-02-18 11:09:52.152327 argcat-0.4.1/src/
-drwxr-xr-x   0 chx1n      (501) staff       (20)        0 2023-02-18 11:09:52.153498 argcat-0.4.1/src/argcat/
--rw-r--r--   0 chx1n      (501) staff       (20)      160 2023-02-18 11:08:19.000000 argcat-0.4.1/src/argcat/__init__.py
--rw-r--r--   0 chx1n      (501) staff       (20)    39171 2023-02-18 10:55:27.000000 argcat-0.4.1/src/argcat/argcat.py
-drwxr-xr-x   0 chx1n      (501) staff       (20)        0 2023-02-18 11:09:52.154441 argcat-0.4.1/src/argcat.egg-info/
--rw-r--r--   0 chx1n      (501) staff       (20)     9822 2023-02-18 11:09:52.000000 argcat-0.4.1/src/argcat.egg-info/PKG-INFO
--rw-r--r--   0 chx1n      (501) staff       (20)      289 2023-02-18 11:09:52.000000 argcat-0.4.1/src/argcat.egg-info/SOURCES.txt
--rw-r--r--   0 chx1n      (501) staff       (20)        1 2023-02-18 11:09:52.000000 argcat-0.4.1/src/argcat.egg-info/dependency_links.txt
--rw-r--r--   0 chx1n      (501) staff       (20)        7 2023-02-18 11:09:52.000000 argcat-0.4.1/src/argcat.egg-info/top_level.txt
-drwxr-xr-x   0 chx1n      (501) staff       (20)        0 2023-02-18 11:09:52.154980 argcat-0.4.1/tests/
--rw-r--r--   0 chx1n      (501) staff       (20)    10011 2022-12-04 13:58:38.000000 argcat-0.4.1/tests/test_build.py
--rw-r--r--   0 chx1n      (501) staff       (20)     9509 2022-12-04 13:58:38.000000 argcat-0.4.1/tests/test_handler.py
--rw-r--r--   0 chx1n      (501) staff       (20)     9442 2022-12-04 13:58:38.000000 argcat-0.4.1/tests/test_parse_args.py
+drwxr-xr-x   0 chx1n      (501) staff       (20)        0 2023-08-03 01:41:04.789949 argcat-0.4.2/
+-rw-r--r--   0 chx1n      (501) staff       (20)     1066 2022-12-04 13:58:38.000000 argcat-0.4.2/LICENSE
+-rw-r--r--   0 chx1n      (501) staff       (20)     9822 2023-08-03 01:41:04.790013 argcat-0.4.2/PKG-INFO
+-rw-r--r--   0 chx1n      (501) staff       (20)     9332 2022-12-04 13:58:38.000000 argcat-0.4.2/README.md
+-rw-r--r--   0 chx1n      (501) staff       (20)      103 2022-12-04 14:03:46.000000 argcat-0.4.2/pyproject.toml
+-rw-r--r--   0 chx1n      (501) staff       (20)      614 2023-08-03 01:41:04.790247 argcat-0.4.2/setup.cfg
+drwxr-xr-x   0 chx1n      (501) staff       (20)        0 2023-08-03 01:41:04.787699 argcat-0.4.2/src/
+drwxr-xr-x   0 chx1n      (501) staff       (20)        0 2023-08-03 01:41:04.788685 argcat-0.4.2/src/argcat/
+-rw-r--r--   0 chx1n      (501) staff       (20)      160 2023-07-26 07:28:38.000000 argcat-0.4.2/src/argcat/__init__.py
+-rw-r--r--   0 chx1n      (501) staff       (20)    39716 2023-07-26 07:27:57.000000 argcat-0.4.2/src/argcat/argcat.py
+drwxr-xr-x   0 chx1n      (501) staff       (20)        0 2023-08-03 01:41:04.789128 argcat-0.4.2/src/argcat.egg-info/
+-rw-r--r--   0 chx1n      (501) staff       (20)     9822 2023-08-03 01:41:04.000000 argcat-0.4.2/src/argcat.egg-info/PKG-INFO
+-rw-r--r--   0 chx1n      (501) staff       (20)      289 2023-08-03 01:41:04.000000 argcat-0.4.2/src/argcat.egg-info/SOURCES.txt
+-rw-r--r--   0 chx1n      (501) staff       (20)        1 2023-08-03 01:41:04.000000 argcat-0.4.2/src/argcat.egg-info/dependency_links.txt
+-rw-r--r--   0 chx1n      (501) staff       (20)        7 2023-08-03 01:41:04.000000 argcat-0.4.2/src/argcat.egg-info/top_level.txt
+drwxr-xr-x   0 chx1n      (501) staff       (20)        0 2023-08-03 01:41:04.789822 argcat-0.4.2/tests/
+-rw-r--r--   0 chx1n      (501) staff       (20)    10011 2022-12-04 13:58:38.000000 argcat-0.4.2/tests/test_build.py
+-rw-r--r--   0 chx1n      (501) staff       (20)     9509 2022-12-04 13:58:38.000000 argcat-0.4.2/tests/test_handler.py
+-rw-r--r--   0 chx1n      (501) staff       (20)     9442 2022-12-04 13:58:38.000000 argcat-0.4.2/tests/test_parse_args.py
```

### Comparing `argcat-0.4.1/LICENSE` & `argcat-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `argcat-0.4.1/PKG-INFO` & `argcat-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argcat
-Version: 0.4.1
+Version: 0.4.2
 Summary: A cute helper for argparse in Python 3
 Home-page: https://github.com/dex1n/ArgCat
 Author: Chunxi Xin
 Author-email: chx1n.d@gmail.com
 Project-URL: Bug Tracker, https://github.com/dex1n/ArgCat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `argcat-0.4.1/README.md` & `argcat-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `argcat-0.4.1/setup.cfg` & `argcat-0.4.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = argcat
-version = 0.4.1
+version = 0.4.2
 author = Chunxi Xin
 author_email = chx1n.d@gmail.com
 description = A cute helper for argparse in Python 3
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/dex1n/ArgCat
 project_urls =
```

### Comparing `argcat-0.4.1/src/argcat/argcat.py` & `argcat-0.4.2/src/argcat/argcat.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 import functools
 from copy import deepcopy
 from pydoc import locate
 from enum import Enum, unique
 from argparse import ArgumentParser, Namespace, _ArgumentGroup, _MutuallyExclusiveGroup, _SubParsersAction, Action
 from typing import ClassVar, List, Dict, Optional, Callable, Tuple, Any, Union
-
+import traceback
 
 # May not be the best solution for the constants, but it's fine for now.
 # And we don't need ClassVar[str] here because I think all constants' type are pretty clear.
 class _ManifestConstants:
     META = "meta"
     METAVAR = "metavar"
     PROG = "prog"
@@ -578,17 +578,18 @@
                 result = parser.handler_func(**parameters)
             # Catch all exception to print the actual exception raised in the handler besides
             # TypeError. If we are only capturing TypeError, the actual error would be "covered" by the TypeError, which
             # means all error would be raised as TypeError. This could be very confusing.
             except Exception as exc:
                 func_sig = inspect.signature(parser.handler_func)
                 input_sig = str(tuple(parameters)).replace('\'','')
-                error_msg = "Handling function Exception: \"{}\", with function sig: {} and received parameters: {}."\
-                    .format(exc, func_sig, input_sig)
+                error_msg = "Handling function sig: `{}` and received parameters: `{}`.".format(func_sig, input_sig)
                 _ArgCatPrinter.print(error_msg, level=_ArgCatPrintLevel.ERROR, indent=1)
+                # v0.4.2-feat: Add Traceback for error details.
+                traceback.print_exc()
             else:
                 return result
         else:
             _ArgCatPrinter.print("Parser `{}` does not have any handler.".format(parser.name), 
             level=_ArgCatPrintLevel.ERROR, indent=1)
         return None
         
@@ -608,16 +609,19 @@
         def on_build_done(manifest_data):
             self._manifest_data = manifest_data
             self._create_parsers()
             self._is_building = False
             _ArgCatPrinter.print("Building DONE. Use print_xx functions for more information.")
         
         return _ArgCatBuilder(on_build_done)
-        
-    def parse_args(self, args: Optional[List[str]]=None, namespace: Optional[Namespace]=None) -> Dict:
+    
+    # v0.4.2-feat: subparser_ignore_main is added to deal with the case in which user would like to not trigger the main 
+    # parser's handler if any subparser handler is called. 
+    def parse_args(self, subparser_ignore_main: bool = False, args: Optional[List[str]]=None, 
+                   namespace: Optional[Namespace]=None) -> Dict:
         """Start to parse args.
 
         This method is pretty much the same as the original `parse_args()` of ArgumentParser, which means
         you can use it the same way as you use ArgumentParser's before.
 
         Returns result from handler. This is the only difference from the ArgumentParser's parse_args.
         The latter one returns a Namespace, but ArgCat returns the result from handler since 
@@ -628,16 +632,18 @@
         subparser_name, subparser_parsed_arguments_dict, main_parser_parsed_arguments_dict = \
         self._arg_parsers[_ManifestConstants.MAIN].parse_args(args=args, namespace=namespace)
         
         ret_result = {}
         
         # The main parser's handler should be called for two cases: 
         # 1. no subparser called or 
-        # 2. subparser called but main parser has arguments.
-        if subparser_name is None or main_parser_parsed_arguments_dict:
+        # 2. subparser called but subparser_ignore_main is not true and main parser has arguments.
+        # v0.4.2-bug: Only if any element of main_parser_parsed_arguments_dict is not None, 
+        # main_parser_parsed_arguments_dict can be considered as not None.
+        if not subparser_name or (not subparser_ignore_main and any(main_parser_parsed_arguments_dict.values())):
             ret_result['main'] = self._call_parser_handler(parser=self._arg_parsers[_ManifestConstants.MAIN], 
                                                            parameters=main_parser_parsed_arguments_dict)
         
         # Only need to check subparser_name because subparser_parsed_arguments_dict can be None when a subparser 
         # is called without any arguments.
         if subparser_name:
             subparser = self._arg_parsers[subparser_name]
```

### Comparing `argcat-0.4.1/src/argcat.egg-info/PKG-INFO` & `argcat-0.4.2/src/argcat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argcat
-Version: 0.4.1
+Version: 0.4.2
 Summary: A cute helper for argparse in Python 3
 Home-page: https://github.com/dex1n/ArgCat
 Author: Chunxi Xin
 Author-email: chx1n.d@gmail.com
 Project-URL: Bug Tracker, https://github.com/dex1n/ArgCat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `argcat-0.4.1/tests/test_build.py` & `argcat-0.4.2/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `argcat-0.4.1/tests/test_handler.py` & `argcat-0.4.2/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `argcat-0.4.1/tests/test_parse_args.py` & `argcat-0.4.2/tests/test_parse_args.py`

 * *Files identical despite different names*

