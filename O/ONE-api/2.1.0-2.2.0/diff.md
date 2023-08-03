# Comparing `tmp/ONE-api-2.1.0.tar.gz` & `tmp/ONE-api-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ONE-api-2.1.0.tar", last modified: Fri Jun 16 10:42:32 2023, max compression
+gzip compressed data, was "ONE-api-2.2.0.tar", last modified: Thu Aug  3 18:15:01 2023, max compression
```

## Comparing `ONE-api-2.1.0.tar` & `ONE-api-2.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.292338 ONE-api-2.1.0/
--rw-rw-rw-   0        0        0       26 2021-05-11 13:53:45.000000 ONE-api-2.1.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.216002 ONE-api-2.1.0/ONE_api.egg-info/
--rw-rw-rw-   0        0        0     4464 2023-06-16 10:42:31.000000 ONE-api-2.1.0/ONE_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1380 2023-06-16 10:42:31.000000 ONE-api-2.1.0/ONE_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 10:42:31.000000 ONE-api-2.1.0/ONE_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-06-16 10:42:31.000000 ONE-api-2.1.0/ONE_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-16 10:42:31.000000 ONE-api-2.1.0/ONE_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4464 2023-06-16 10:42:32.288348 ONE-api-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3453 2023-05-12 08:59:29.000000 ONE-api-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.232519 ONE-api-2.1.0/one/
--rw-rw-rw-   0        0        0       77 2023-06-16 09:54:18.000000 ONE-api-2.1.0/one/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.243882 ONE-api-2.1.0/one/alf/
--rw-rw-rw-   0        0        0       70 2021-09-13 19:50:22.000000 ONE-api-2.1.0/one/alf/__init__.py
--rw-rw-rw-   0        0        0    11896 2023-06-16 08:46:55.000000 ONE-api-2.1.0/one/alf/cache.py
--rw-rw-rw-   0        0        0     3186 2023-06-16 09:25:42.000000 ONE-api-2.1.0/one/alf/exceptions.py
--rw-rw-rw-   0        0        0    14801 2023-05-12 08:59:29.000000 ONE-api-2.1.0/one/alf/files.py
--rw-rw-rw-   0        0        0    28696 2023-06-16 09:54:18.000000 ONE-api-2.1.0/one/alf/io.py
--rw-rw-rw-   0        0        0    18659 2023-06-16 09:54:18.000000 ONE-api-2.1.0/one/alf/spec.py
--rw-rw-rw-   0        0        0   118319 2023-06-16 09:25:42.000000 ONE-api-2.1.0/one/api.py
--rw-rw-rw-   0        0        0    26479 2023-05-12 08:59:29.000000 ONE-api-2.1.0/one/converters.py
--rw-rw-rw-   0        0        0    13362 2023-02-28 15:23:52.000000 ONE-api-2.1.0/one/params.py
--rw-rw-rw-   0        0        0    33596 2023-05-12 08:59:29.000000 ONE-api-2.1.0/one/registration.py
-drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.253463 ONE-api-2.1.0/one/remote/
--rw-rw-rw-   0        0        0       40 2022-11-09 13:45:11.000000 ONE-api-2.1.0/one/remote/__init__.py
--rw-rw-rw-   0        0        0     8957 2023-04-21 11:35:55.000000 ONE-api-2.1.0/one/remote/aws.py
--rw-rw-rw-   0        0        0     4566 2023-01-20 12:25:51.000000 ONE-api-2.1.0/one/remote/base.py
--rw-rw-rw-   0        0        0    21865 2023-05-12 08:59:29.000000 ONE-api-2.1.0/one/remote/globus.py
-drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.199498 ONE-api-2.1.0/one/tests/
-drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.263268 ONE-api-2.1.0/one/tests/fixtures/
--rw-rw-rw-   0        0        0    29918 2021-05-13 19:38:01.000000 ONE-api-2.1.0/one/tests/fixtures/datasets.pqt
-drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.269251 ONE-api-2.1.0/one/tests/fixtures/params/
--rw-rw-rw-   0        0        0      140 2021-09-13 19:50:22.000000 ONE-api-2.1.0/one/tests/fixtures/params/.caches
--rw-rw-rw-   0        0        0      276 2022-04-25 08:39:47.000000 ONE-api-2.1.0/one/tests/fixtures/params/.test.alyx.internationalbrainlab.org
-drwxrwxrwx   0        0        0        0 2023-06-16 10:42:32.286354 ONE-api-2.1.0/one/tests/fixtures/rest_responses/
--rw-rw-rw-   0        0        0      283 2021-09-13 19:50:22.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/1f187d80fd59677b395fcdb18e68e4401bfa1cc9
--rw-rw-rw-   0        0        0      427 2022-11-09 13:45:11.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/3f51aa2e0baa42438467906f56a457c91a221898
--rw-rw-rw-   0        0        0     1370 2021-09-13 19:50:22.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/47893cf67c985e6361cdee009334963f49fb0746
--rw-rw-rw-   0        0        0     1451 2021-09-13 19:50:22.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/535d0e9a1e2c1efbdeba0d673b131e00361a2edb
--rw-rw-rw-   0        0        0      313 2022-11-09 13:45:11.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/5618bea3484a52cd893616f07903f0e49e023ba1
--rw-rw-rw-   0        0        0     8066 2022-11-09 13:45:11.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/6dc96f7e9bcc6ac2e7581489b9580a6cd3f28293
--rw-rw-rw-   0        0        0      210 2021-09-13 19:50:22.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/db1731fb8df0208944ae85f76718430813a8bf50
--rw-rw-rw-   0        0        0      417 2022-11-09 13:45:11.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/dcce48259bb929661f60a02a48563f70aa6185b3
--rw-rw-rw-   0        0        0    22531 2021-05-12 14:50:16.000000 ONE-api-2.1.0/one/tests/fixtures/rest_responses/f530d6022f61cdc9e38cc66beb3cb71f3003c9a1
--rw-rw-rw-   0        0        0     6916 2021-05-13 19:38:01.000000 ONE-api-2.1.0/one/tests/fixtures/sessions.pqt
--rw-rw-rw-   0        0        0      324 2021-09-16 15:52:39.000000 ONE-api-2.1.0/one/tests/fixtures/test_dbs.json
--rw-rw-rw-   0        0        0   828598 2021-09-13 19:50:22.000000 ONE-api-2.1.0/one/tests/fixtures/test_img.png
--rw-rw-rw-   0        0        0    21620 2023-05-12 08:59:29.000000 ONE-api-2.1.0/one/util.py
--rw-rw-rw-   0        0        0    47614 2023-05-12 08:59:29.000000 ONE-api-2.1.0/one/webclient.py
--rw-rw-rw-   0        0        0       42 2023-06-16 10:42:32.292338 ONE-api-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1679 2022-11-09 13:45:11.000000 ONE-api-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 18:15:01.806842 ONE-api-2.2.0/
+-rw-rw-rw-   0        0        0       26 2021-05-11 13:53:45.000000 ONE-api-2.2.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-08-03 18:15:01.410394 ONE-api-2.2.0/ONE_api.egg-info/
+-rw-rw-rw-   0        0        0     4464 2023-08-03 18:15:01.000000 ONE-api-2.2.0/ONE_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1380 2023-08-03 18:15:01.000000 ONE-api-2.2.0/ONE_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 18:15:01.000000 ONE-api-2.2.0/ONE_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-08-03 18:15:01.000000 ONE-api-2.2.0/ONE_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-03 18:15:01.000000 ONE-api-2.2.0/ONE_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4464 2023-08-03 18:15:01.805843 ONE-api-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3453 2023-05-12 08:59:29.000000 ONE-api-2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 18:15:01.432335 ONE-api-2.2.0/one/
+-rw-rw-rw-   0        0        0       78 2023-08-02 11:38:15.000000 ONE-api-2.2.0/one/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 18:15:01.448136 ONE-api-2.2.0/one/alf/
+-rw-rw-rw-   0        0        0       70 2021-09-13 19:50:22.000000 ONE-api-2.2.0/one/alf/__init__.py
+-rw-rw-rw-   0        0        0    11896 2023-06-16 08:46:55.000000 ONE-api-2.2.0/one/alf/cache.py
+-rw-rw-rw-   0        0        0     3190 2023-08-02 11:38:15.000000 ONE-api-2.2.0/one/alf/exceptions.py
+-rw-rw-rw-   0        0        0    14794 2023-08-02 11:38:15.000000 ONE-api-2.2.0/one/alf/files.py
+-rw-rw-rw-   0        0        0    28687 2023-08-02 11:38:15.000000 ONE-api-2.2.0/one/alf/io.py
+-rw-rw-rw-   0        0        0    18951 2023-08-02 11:38:15.000000 ONE-api-2.2.0/one/alf/spec.py
+-rw-rw-rw-   0        0        0   121489 2023-08-02 11:38:15.000000 ONE-api-2.2.0/one/api.py
+-rw-rw-rw-   0        0        0    26515 2023-08-02 11:38:15.000000 ONE-api-2.2.0/one/converters.py
+-rw-rw-rw-   0        0        0    13367 2023-08-02 11:38:15.000000 ONE-api-2.2.0/one/params.py
+-rw-rw-rw-   0        0        0    33598 2023-08-02 11:38:15.000000 ONE-api-2.2.0/one/registration.py
+drwxrwxrwx   0        0        0        0 2023-08-03 18:15:01.457112 ONE-api-2.2.0/one/remote/
+-rw-rw-rw-   0        0        0       40 2022-11-09 13:45:11.000000 ONE-api-2.2.0/one/remote/__init__.py
+-rw-rw-rw-   0        0        0     8959 2023-08-02 11:38:15.000000 ONE-api-2.2.0/one/remote/aws.py
+-rw-rw-rw-   0        0        0     4550 2023-08-02 11:38:25.000000 ONE-api-2.2.0/one/remote/base.py
+-rw-rw-rw-   0        0        0    34889 2023-08-03 11:15:39.000000 ONE-api-2.2.0/one/remote/globus.py
+drwxrwxrwx   0        0        0        0 2023-08-03 18:15:01.393440 ONE-api-2.2.0/one/tests/
+drwxrwxrwx   0        0        0        0 2023-08-03 18:15:01.772579 ONE-api-2.2.0/one/tests/fixtures/
+-rw-rw-rw-   0        0        0    29918 2021-05-13 19:38:01.000000 ONE-api-2.2.0/one/tests/fixtures/datasets.pqt
+drwxrwxrwx   0        0        0        0 2023-08-03 18:15:01.780557 ONE-api-2.2.0/one/tests/fixtures/params/
+-rw-rw-rw-   0        0        0      140 2021-09-13 19:50:22.000000 ONE-api-2.2.0/one/tests/fixtures/params/.caches
+-rw-rw-rw-   0        0        0      276 2022-04-25 08:39:47.000000 ONE-api-2.2.0/one/tests/fixtures/params/.test.alyx.internationalbrainlab.org
+drwxrwxrwx   0        0        0        0 2023-08-03 18:15:01.802621 ONE-api-2.2.0/one/tests/fixtures/rest_responses/
+-rw-rw-rw-   0        0        0      283 2021-09-13 19:50:22.000000 ONE-api-2.2.0/one/tests/fixtures/rest_responses/1f187d80fd59677b395fcdb18e68e4401bfa1cc9
+-rw-rw-rw-   0        0        0      427 2022-11-09 13:45:11.000000 ONE-api-2.2.0/one/tests/fixtures/rest_responses/3f51aa2e0baa42438467906f56a457c91a221898
+-rw-rw-rw-   0        0        0     1370 2021-09-13 19:50:22.000000 ONE-api-2.2.0/one/tests/fixtures/rest_responses/47893cf67c985e6361cdee009334963f49fb0746
+-rw-rw-rw-   0        0        0     1451 2021-09-13 19:50:22.000000 ONE-api-2.2.0/one/tests/fixtures/rest_responses/535d0e9a1e2c1efbdeba0d673b131e00361a2edb
+-rw-rw-rw-   0        0        0      313 2022-11-09 13:45:11.000000 ONE-api-2.2.0/one/tests/fixtures/rest_responses/5618bea3484a52cd893616f07903f0e49e023ba1
+-rw-rw-rw-   0        0        0     8066 2022-11-09 13:45:11.000000 ONE-api-2.2.0/one/tests/fixtures/rest_responses/6dc96f7e9bcc6ac2e7581489b9580a6cd3f28293
+-rw-rw-rw-   0        0        0      210 2021-09-13 19:50:22.000000 ONE-api-2.2.0/one/tests/fixtures/rest_responses/db1731fb8df0208944ae85f76718430813a8bf50
+-rw-rw-rw-   0        0        0      417 2022-11-09 13:45:11.000000 ONE-api-2.2.0/one/tests/fixtures/rest_responses/dcce48259bb929661f60a02a48563f70aa6185b3
+-rw-rw-rw-   0        0        0    22531 2021-05-12 14:50:16.000000 ONE-api-2.2.0/one/tests/fixtures/rest_responses/f530d6022f61cdc9e38cc66beb3cb71f3003c9a1
+-rw-rw-rw-   0        0        0     6916 2021-05-13 19:38:01.000000 ONE-api-2.2.0/one/tests/fixtures/sessions.pqt
+-rw-rw-rw-   0        0        0      324 2021-09-16 15:52:39.000000 ONE-api-2.2.0/one/tests/fixtures/test_dbs.json
+-rw-rw-rw-   0        0        0   828598 2021-09-13 19:50:22.000000 ONE-api-2.2.0/one/tests/fixtures/test_img.png
+-rw-rw-rw-   0        0        0    21624 2023-08-02 11:38:15.000000 ONE-api-2.2.0/one/util.py
+-rw-rw-rw-   0        0        0    48394 2023-08-02 11:38:15.000000 ONE-api-2.2.0/one/webclient.py
+-rw-rw-rw-   0        0        0       42 2023-08-03 18:15:01.807837 ONE-api-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1679 2022-11-09 13:45:11.000000 ONE-api-2.2.0/setup.py
```

### Comparing `ONE-api-2.1.0/ONE_api.egg-info/PKG-INFO` & `ONE-api-2.2.0/ONE_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ONE-api
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Neurophysiology Environment
 Home-page: https://github.com/int-brain-lab/ONE
 Author: IBL Staff
 License: MIT
 Description: # Open Neurophysiology Environment
         [![Coverage Status](https://coveralls.io/repos/github/int-brain-lab/ONE/badge.svg?branch=main)](https://coveralls.io/github/int-brain-lab/ONE?branch=main)
         ![CI workflow](https://github.com/int-brain-lab/ONE/actions/workflows/main.yaml/badge.svg?branch=main)
```

### Comparing `ONE-api-2.1.0/ONE_api.egg-info/SOURCES.txt` & `ONE-api-2.2.0/ONE_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ONE-api-2.1.0/PKG-INFO` & `ONE-api-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ONE-api
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Neurophysiology Environment
 Home-page: https://github.com/int-brain-lab/ONE
 Author: IBL Staff
 License: MIT
 Description: # Open Neurophysiology Environment
         [![Coverage Status](https://coveralls.io/repos/github/int-brain-lab/ONE/badge.svg?branch=main)](https://coveralls.io/github/int-brain-lab/ONE?branch=main)
         ![CI workflow](https://github.com/int-brain-lab/ONE/actions/workflows/main.yaml/badge.svg?branch=main)
```

### Comparing `ONE-api-2.1.0/README.md` & `ONE-api-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ONE-api-2.1.0/one/alf/cache.py` & `ONE-api-2.2.0/one/alf/cache.py`

 * *Files identical despite different names*

### Comparing `ONE-api-2.1.0/one/alf/exceptions.py` & `ONE-api-2.2.0/one/alf/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 
 A set of Alyx and ALF related error classes which provide a more verbose description of the raised
 issues.
 """
 
 
 class ALFError(Exception):
-    """A base class for ALF-related errors
+    """A base class for ALF-related errors.
 
     Attributes
     ----------
     explanation : str
         An optional, verbose but general explanation of the error class.  All errors will display
         the same explanation.
     """
     explanation = ''
 
     def __init__(self, *args, terse=False):
-        """A base ALF exception
+        """A base ALF exception.
 
         Parameters
         ----------
         args : str, any
-            A specific error message to display or items to include in message
+            A specific error message to display or items to include in message.
         terse : bool
-            If True, the explanation string is not included in exception message
+            If True, the explanation string is not included in exception message.
 
         Examples
         --------
         >>> raise ALFError("ALF directory doesn't exist")
         one.alf.exceptions.ALFError: ALF directory doesn't exist
 
         >>> raise ALFError('invalid/path/one', 'invalid/path/two')
```

### Comparing `ONE-api-2.1.0/one/alf/files.py` & `ONE-api-2.2.0/one/alf/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,20 @@
 
 An ALF file has the following components (those in brackets are optional):
     (_namespace_)object.attribute(_timescale)(.extra.parts).ext
 
 Note the following:
     Object attributes may not contain an underscore unless followed by 'times' or 'intervals'.
     A namespace must not contain extra underscores (i.e. `name_space` and `__namespace__` are not
-    valid)
-    ALF files must always have an extension
+    valid).
+    ALF files must always have an extension.
 
 For more information, see the following documentation:
     https://int-brain-lab.github.io/ONE/alf_intro.html
 
-Created on Tue Sep 11 18:06:21 2018
-
-@author: Miles
 """
 from collections import OrderedDict
 from datetime import datetime
 from typing import Union, Optional
 from pathlib import Path
 import logging
 
@@ -34,26 +31,26 @@
 
     A relative path follows the pattern
         (collection/)(#revision#/)_namespace_object.attribute_timescale.extra.extension
 
     Parameters
     ----------
     rel_path : str, pathlib.Path
-        A relative path string
+        A relative path string.
     as_dict : bool
         If true, an OrderedDict of parts are returned with the keys ('lab', 'subject', 'date',
-        'number'), otherwise a tuple of values are returned
+        'number'), otherwise a tuple of values are returned.
     assert_valid : bool
         If true a ValueError is raised when the session cannot be parsed, otherwise an empty
-        dict of tuple of Nones is returned
+        dict of tuple of Nones is returned.
 
     Returns
     -------
     OrderedDict, tuple
-        A dict if as_dict is true, or a tuple of parsed values
+        A dict if as_dict is true, or a tuple of parsed values.
     """
     return _path_parts(rel_path, REL_PATH_SPEC, True, as_dict, assert_valid)
 
 
 def session_path_parts(session_path, as_dict=False, assert_valid=True):
     """Parse a session path into the relevant parts.
 
@@ -62,58 +59,58 @@
         - subject
         - date
         - number
 
     Parameters
     ----------
     session_path : str, pathlib.Path
-        A session path string
+        A session path string.
     as_dict : bool
         If true, an OrderedDict of parts are returned with the keys ('lab', 'subject', 'date',
-        'number'), otherwise a tuple of values are returned
+        'number'), otherwise a tuple of values are returned.
     assert_valid : bool
         If true a ValueError is raised when the session cannot be parsed, otherwise an empty
-        dict of tuple of Nones is returned
+        dict of tuple of Nones is returned.
 
     Returns
     -------
     OrderedDict, tuple
-        A dict if as_dict is true, or a tuple of parsed values
+        A dict if as_dict is true, or a tuple of parsed values.
 
     Raises
     ------
     ValueError
-        Invalid ALF session path (assert_valid is True)
+        Invalid ALF session path (assert_valid is True).
     """
     return _path_parts(session_path, SESSION_SPEC, False, as_dict, assert_valid)
 
 
 def _path_parts(path, spec_str, match=True, as_dict=False, assert_valid=True):
-    """Given a ALF and a spec string, parse into parts
+    """Given a ALF and a spec string, parse into parts.
 
     Parameters
     ----------
     path : str, pathlib.Path
-        An ALF path or dataset
+        An ALF path or dataset.
     match : bool
-        If True, string must match exactly, otherwise search for expression within path
+        If True, string must match exactly, otherwise search for expression within path.
     as_dict : bool
-        When true a dict of matches is returned
+        When true a dict of matches is returned.
     assert_valid : bool
-        When true an exception is raised when the filename cannot be parsed
+        When true an exception is raised when the filename cannot be parsed.
 
     Returns
     -------
     OrderedDict, tuple
-        A dict if as_dict is true, or a tuple of parsed values
+        A dict if as_dict is true, or a tuple of parsed values.
 
     Raises
     ------
     ValueError
-        Invalid ALF path (assert_valid is True)
+        Invalid ALF path (assert_valid is True).
     """
     if hasattr(path, 'as_posix'):
         path = path.as_posix()
     pattern = spec.regex(spec_str)
     empty = OrderedDict.fromkeys(pattern.groupindex.keys())
     parsed = (pattern.match if match else pattern.search)(path)
     if parsed:  # py3.8
@@ -128,34 +125,34 @@
 def filename_parts(filename, as_dict=False, assert_valid=True) -> Union[dict, tuple]:
     """
     Return the parsed elements of a given ALF filename.
 
     Parameters
     ----------
     filename : str
-        The name of the file
+        The name of the file.
     as_dict : bool
-        When true a dict of matches is returned
+        When true a dict of matches is returned.
     assert_valid : bool
-        When true an exception is raised when the filename cannot be parsed
+        When true an exception is raised when the filename cannot be parsed.
 
     Returns
     -------
     namespace : str
-        The _namespace_ or None if not present
+        The _namespace_ or None if not present.
     object : str
-        ALF object
+        ALF object.
     attribute : str
-        The ALF attribute
+        The ALF attribute.
     timescale : str
-        The ALF _timescale or None if not present
+        The ALF _timescale or None if not present.
     extra : str
-        Any extra parts to the filename, or None if not present
+        Any extra parts to the filename, or None if not present.
     extension : str
-        The file extension
+        The file extension.
 
     Examples
     --------
     >>> filename_parts('_namespace_obj.times_timescale.extra.foo.ext')
     ('namespace', 'obj', 'times', 'timescale', 'extra.foo', 'ext')
     >>> filename_parts('spikes.clusters.npy', as_dict=True)
     {'namespace': None,
@@ -174,35 +171,35 @@
     ('spikeglx', 'ephysData_g0_t0', 'imec0', None, 'lf', 'bin')
     >>> filename_parts('_ibl_trials.goCue_times_bpod.csv')
     ('ibl', 'trials', 'goCue_times', 'bpod', None, 'csv')
 
     Raises
     ------
     ValueError
-        Invalid ALF dataset (assert_valid is True)
+        Invalid ALF dataset (assert_valid is True).
     """
     return _path_parts(filename, FILE_SPEC, True, as_dict, assert_valid)
 
 
 def full_path_parts(path, as_dict=False, assert_valid=True) -> Union[dict, tuple]:
     """Parse all filename and folder parts.
 
     Parameters
     ----------
-    path : str, pathlib.Path
+    path : str, pathlib.Path.
         The ALF path
     as_dict : bool
-        When true a dict of matches is returned
+        When true a dict of matches is returned.
     assert_valid : bool
-        When true an exception is raised when the filename cannot be parsed
+        When true an exception is raised when the filename cannot be parsed.
 
     Returns
     -------
     OrderedDict, tuple
-        A dict if as_dict is true, or a tuple of parsed values
+        A dict if as_dict is true, or a tuple of parsed values.
 
     Examples
     --------
     >>> full_path_parts(
     ...    'lab/Subjects/subject/2020-01-01/001/collection/#revision#/'
     ...    '_namespace_obj.times_timescale.extra.foo.ext')
     ('lab', 'subject', '2020-01-01', '001', 'collection', 'revision',
@@ -220,15 +217,15 @@
      'timescale': None,
      'extra': None,
      'extension': 'npy'}
 
     Raises
     ------
     ValueError
-        Invalid ALF path (assert_valid is True)
+        Invalid ALF path (assert_valid is True).
     """
     path = Path(path)
     # NB We try to determine whether we have a folder or filename path.  Filenames contain at
     # least two periods, however it is currently permitted to have any number of periods in a
     # collection, making the ALF path ambiguous.
     if sum(x == '.' for x in path.name) < 2:  # folder only
         folders = folder_parts(path, as_dict, assert_valid)
@@ -247,24 +244,24 @@
 
 def folder_parts(folder_path, as_dict=False, assert_valid=True) -> Union[dict, tuple]:
     """Parse all folder parts, including session, collection and revision.
 
     Parameters
     ----------
     folder_path : str, pathlib.Path
-        The ALF folder path
+        The ALF folder path.
     as_dict : bool
-        When true a dict of matches is returned
+        When true a dict of matches is returned.
     assert_valid : bool
-        When true an exception is raised when the filename cannot be parsed
+        When true an exception is raised when the filename cannot be parsed.
 
     Returns
     -------
     OrderedDict, tuple
-        A dict if as_dict is true, or a tuple of parsed values
+        A dict if as_dict is true, or a tuple of parsed values.
 
     Examples
     --------
     >>> folder_parts('lab/Subjects/subject/2020-01-01/001/collection/#revision#')
     ('lab', 'subject', '2020-01-01', '001', 'collection', 'revision')
     >>> folder_parts(Path('lab/Subjects/subject/2020-01-01/001'), as_dict=True)
     {'lab': 'lab',
@@ -273,37 +270,37 @@
      'number': '001',
      'collection': None,
      'revision': None}
 
     Raises
     ------
     ValueError
-        Invalid ALF path (assert_valid is True)
+        Invalid ALF path (assert_valid is True).
     """
     if hasattr(folder_path, 'as_posix'):
         folder_path = folder_path.as_posix()
     if folder_path and folder_path[-1] != '/':  # Slash required for regex pattern
         folder_path = folder_path + '/'
     spec_str = f'{SESSION_SPEC}/{COLLECTION_SPEC}'
     return _path_parts(folder_path, spec_str, False, as_dict, assert_valid)
 
 
 def _isdatetime(s: str) -> bool:
-    """Returns True if input is valid ISO date string"""
+    """Returns True if input is valid ISO date string."""
     try:
         datetime.strptime(s, '%Y-%m-%d')
         return True
     except ValueError:
         return False
 
 
 def get_session_path(path: Union[str, Path]) -> Optional[Path]:
     """
     Returns the session path from any filepath if the date/number pattern is found,
-    including the root directory
+    including the root directory.
 
     Returns
     -------
     pathlib.Path
         The session path part of the input path or None if path invalid.
 
     Examples
@@ -331,20 +328,20 @@
     Attempts to return the first valid part of the path, first searching for a session path,
     then relative path (collection/revision/filename), then just the filename.  If all invalid,
     None is returned.
 
     Parameters
     ----------
     path : str, pathlib.Path
-        A path to parse
+        A path to parse.
 
     Returns
     -------
     str
-        A string containing the full ALF path, session path, relative path or filename
+        A string containing the full ALF path, session path, relative path or filename.
 
     Examples
     --------
     >>> get_alf_path('etc/etc/lab/Subjects/subj/2021-01-21/001')
     'lab/Subjects/subj/2021-01-21/001/collection/file.attr.ext'
 
     >>> get_alf_path('etc/etc/subj/2021-01-21/001/collection/file.attr.ext')
@@ -396,15 +393,15 @@
     Raises
     ------
     ValueError
         `uuid` must be a valid hyphen-separated hexadecimal UUID.
 
     See Also
     --------
-    one.alf.io.remove_uuid_string
+    one.alf.files.remove_uuid_string
     one.alf.spec.is_uuid
     """
     if isinstance(uuid, str) and not spec.is_uuid_string(uuid):
         raise ValueError('Should provide a valid UUID v4')
     uuid = str(uuid)
     # NB: Only instantiate as Path if not already a Path, otherwise we risk changing the class
     if isinstance(file_path, str):
@@ -436,15 +433,15 @@
     Path('/path/to/trials.intervals.npy')
 
     >>> add_uuid_string('/path/to/trials.intervals.npy')
     Path('/path/to/trials.intervals.npy')
 
     See Also
     --------
-    one.alf.io.add_uuid_string
+    one.alf.files.add_uuid_string
     """
     if isinstance(file_path, str):
         file_path = Path(file_path)
     name_parts = file_path.stem.split('.')
 
     if spec.is_uuid_string(name_parts[-1]):
         file_path = file_path.with_name('.'.join(name_parts[:-1]) + file_path.suffix)
```

### Comparing `ONE-api-2.1.0/one/alf/io.py` & `ONE-api-2.2.0/one/alf/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,15 +334,15 @@
     ----------
     alfpath : str, pathlib.Path
         The folder to list
     object : str, list
         An ALF object name to filter by
     wildcards : bool
         If true uses unix shell style pattern matching, otherwise uses regular expressions
-    kwargs : dict
+    **kwargs
         Other ALF parts to filter, including namespace, attribute, etc.
 
     Returns
     -------
     list
         A list of ALF paths
     tuple
@@ -425,15 +425,15 @@
         The folder to look into
     object : str
         ALF object name
     attributes : str, list
         Wanted attributes
     wildcards : bool
         If true uses unix shell style pattern matching, otherwise uses regular expressions
-    kwargs : dict
+    **kwargs
         Other ALF parts to filter by
 
     Returns
     -------
     bool
         For multiple attributes, returns True only if all attributes are found
     """
@@ -465,31 +465,31 @@
     Full Reference here: https://int-brain-lab.github.io/ONE/alf_intro.html
 
     Simplified example: _namespace_object.attribute_timescale.part1.part2.extension
 
     Parameters
     ----------
     alfpath : str, pathlib.Path, list
-        Any ALF path pertaining to the object OR directory containing ALFs OR list of paths
+        Any ALF path pertaining to the object OR directory containing ALFs OR list of paths.
     object : str, list, None
         The ALF object(s) to filter by.  If a directory is provided and object is None, all valid
-        ALF files returned
+        ALF files returned.
     short_keys : bool
         By default, the output dictionary keys will be compounds of attributes, timescale and
         any eventual parts separated by a dot. Use True to shorten the keys to the attribute
-        and timescale
+        and timescale.
     wildcards : bool
-        If true uses unix shell style pattern matching, otherwise uses regular expressions
-    kwargs : dict
-        Other ALF parts to filter by
+        If true uses unix shell style pattern matching, otherwise uses regular expressions.
+    **kwargs
+        Other ALF parts to filter by.
 
     Returns
     -------
     AlfBunch
-        An ALFBunch (dict-like) of all attributes pertaining to the object
+        An ALFBunch (dict-like) of all attributes pertaining to the object.
 
     Examples
     --------
         Load 'spikes' object
 
         >>> spikes = load_object('full/path/to/my/alffolder/', 'spikes')
```

### Comparing `ONE-api-2.1.0/one/alf/spec.py` & `ONE-api-2.2.0/one/alf/spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,15 @@
         The ALF object name
     attribute : str
         The ALF object attribute name
     extension : str
         The file extension
     namespace : str
         An optional namespace
-    timescale : str
+    timescale : str, tuple
         An optional timescale
     extra : str, tuple
         One or more optional extra ALF attributes
 
     Returns
     -------
     str
@@ -356,14 +356,16 @@
     --------
     >>> to_alf('spikes', 'times', 'ssv')
     'spikes.times.ssv'
     >>> to_alf('spikes', 'times', 'ssv', namespace='ibl')
     '_ibl_spikes.times.ssv'
     >>> to_alf('spikes', 'times', 'ssv', namespace='ibl', timescale='ephysClock')
     '_ibl_spikes.times_ephysClock.ssv'
+    >>> to_alf('spikes', 'times', 'ssv', namespace='ibl', timescale=('ephys clock', 'minutes'))
+    '_ibl_spikes.times_ephysClock_minutes.ssv'
     >>> to_alf('spikes', 'times', 'npy', namespace='ibl', timescale='ephysClock', extra='raw')
     '_ibl_spikes.times_ephysClock.raw.npy'
     >>> to_alf('wheel', 'timestamps', 'npy', 'ibl', 'bpod', ('raw', 'v12'))
     '_ibl_wheel.timestamps_bpod.raw.v12.npy'
     """
     # Validate inputs
     if not extension:
@@ -376,15 +378,18 @@
            (object, attribute, namespace, extension, timescale)):
         raise ValueError('ALF parts must not contain a period (`.`)')
     if '_' in (namespace or ''):
         raise ValueError('Namespace must not contain extra underscores')
     if object[0] == '_':
         raise ValueError('Objects must not contain underscores; use namespace arg instead')
     # Ensure parts are camel case (converts whitespace and snake case)
-    object, timescale = map(_dromedary, (object, timescale))
+    if timescale:
+        timescale = filter(None, [timescale] if isinstance(timescale, str) else timescale)
+        timescale = '_'.join(map(_dromedary, timescale))
+    object = _dromedary(object)
 
     # Optional extras may be provided as string or tuple of strings
     if not extra:
         extra = ()
     elif isinstance(extra, str):
         extra = extra.split('.')
```

### Comparing `ONE-api-2.1.0/one/api.py` & `ONE-api-2.2.0/one/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Classes for searching, listing and (down)loading ALyx Files."""
 import collections.abc
 import urllib.parse
 import warnings
 import logging
-import packaging.version
 from datetime import datetime, timedelta
 from functools import lru_cache, partial
 from inspect import unwrap
 from pathlib import Path, PurePosixPath
 from typing import Any, Union, Optional, List
 from uuid import UUID
 from urllib.error import URLError
 import time
 import threading
 
 import pandas as pd
 import numpy as np
 import requests.exceptions
+import packaging.version
 
 from iblutil.io import parquet, hashfile
 from iblutil.util import Bunch, flatten
 
 import one.params
 import one.webclient as wc
 import one.alf.io as alfio
@@ -378,19 +378,21 @@
         """
         Searches sessions matching the given criteria and returns a list of matching eids
 
         For a list of search terms, use the method
 
             one.search_terms()
 
-        For all of the search parameters, a single value or list may be provided.  For dataset,
+        For all of the search parameters, a single value or list may be provided.  For `dataset`,
         the sessions returned will contain all listed datasets.  For the other parameters,
-        the session must contain at least one of the entries. NB: Wildcards are not permitted,
-        however if wildcards property is False, regular expressions may be used for all but
-        number and date_range.
+        the session must contain at least one of the entries.
+
+        For all but `date_range` and `number`, any field that contains the search string is
+        returned.  Wildcards are not permitted, however if wildcards property is True, regular
+        expressions may be used (see notes and examples).
 
         Parameters
         ----------
         dataset : str, list
             One or more dataset names. Returns sessions containing all these datasets.
             A dataset matches if it contains the search string e.g. 'wheel.position' matches
             '_ibl_wheel.position.npy'.
@@ -417,14 +419,44 @@
         Returns
         -------
         list
             A list of eids.
         (list)
             (If details is True) a list of dictionaries, each entry corresponding to a matching
             session.
+
+        Examples
+        --------
+        Search for sessions with 'training' in the task protocol.
+
+        >>> eids = one.search(task='training')
+
+        Search for sessions by subject 'MFD_04'.
+
+        >>> eids = one.search(subject='MFD_04')
+
+        Do an exact search for sessions by subject 'FD_04'.
+
+        >>> assert one.wildcards is True, 'the wildcards flag must be True for regex expressions'
+        >>> eids = one.search(subject='^FD_04$')
+
+        Search for sessions on a given date, in a given lab, containing trials and spike data.
+
+        >>> eids = one.search(date='2023-01-01', lab='churchlandlab', dataset=['trials', 'spikes'])
+
+        Notes
+        -----
+        - In default and local mode, most queries are case-sensitive partial matches. When lists
+          are provided, the search is a logical OR, except for `datasets`, which is a logical AND.
+        - All search terms are true for a session to be returned, i.e. subject matches AND project
+          matches, etc.
+        - In remote mode most queries are case-insensitive partial matches.
+        - In default and local mode, when the one.wildcards flag is True (default), queries are
+          interpreted as regular expressions. To turn this off set one.wildcards to False.
+        - In remote mode regular expressions are only supported using the `django` argument.
         """
 
         def all_present(x, dsets, exists=True):
             """Returns true if all datasets present in Series"""
             return all(any(x.str.contains(y, regex=self.wildcards) & exists) for y in dsets)
 
         # Iterate over search filters, reducing the sessions table
@@ -1079,21 +1111,21 @@
             A list of data (or file paths) the length of datasets
         list
             A list of meta data Bunches. If assert_present is False, missing data will be None
 
         Notes
         -----
         - There are three ways the datasets may be formatted: the object.attribute; the file name
-         (including namespace and extension); the ALF components as a dict; the dataset path,
-         relative to the session path, e.g. collection/object.attribute.ext.
+          (including namespace and extension); the ALF components as a dict; the dataset path,
+          relative to the session path, e.g. collection/object.attribute.ext.
         - When relative paths are provided (e.g. 'collection/#revision#/object.attribute.ext'),
-         wildcards/regular expressions must not be used. To use wildcards, pass the collection and
-         revision as separate keyword arguments.
+          wildcards/regular expressions must not be used. To use wildcards, pass the collection and
+          revision as separate keyword arguments.
         - To ensure you are loading the correct revision, use the revisions kwarg instead of
-         relative paths.
+          relative paths.
 
         Raises
         ------
         ValueError
             When a relative paths is provided (e.g. 'collection/#revision#/object.attribute.ext'),
             the collection and revision keyword arguments must be None.
         ValueError
@@ -1973,35 +2005,39 @@
         """
         Searches sessions matching the given criteria and returns a list of matching eids.
 
         For a list of search terms, use the method
 
             one.search_terms(query_type='remote')
 
-        For all of the search parameters, a single value or list may be provided.  For dataset,
+        For all of the search parameters, a single value or list may be provided.  For `dataset`,
         the sessions returned will contain all listed datasets.  For the other parameters,
-        the session must contain at least one of the entries. NB: Wildcards are not permitted,
-        however if wildcards property is False, regular expressions may be used for all but
-        number and date_range.
+        the session must contain at least one of the entries.
+
+        For all but `date_range` and `number`, any field that contains the search string is
+        returned.  Wildcards are not permitted, however if wildcards property is True, regular
+        expressions may be used (see notes and examples).
 
         Parameters
         ----------
         dataset : str
             A (partial) dataset name. Returns sessions containing matching datasets.
             A dataset matches if it contains the search string e.g. 'wheel.position' matches
             '_ibl_wheel.position.npy'. C.f. `datasets` argument.
         date_range : str, list, datetime.datetime, datetime.date, pandas.timestamp
             A single date to search or a list of 2 dates that define the range (inclusive).  To
             define only the upper or lower date bound, set the other element to None.
         lab : str, list
-            A str or list of lab names, returns sessions from any of these labs.
+            A str or list of lab names, returns sessions from any of these labs (can be partial,
+            i.e. any task protocol containing that str will be found).
         number : str, int
             Number of session to be returned, i.e. number in sequence for a given date.
         subject : str, list
-            A list of subject nicknames, returns sessions for any of these subjects.
+            A list of subject nicknames, returns sessions for any of these subjects (can be
+            partial, i.e. any task protocol containing that str will be found).
         task_protocol : str, list
             The task protocol name (can be partial, i.e. any task protocol containing that str
             will be found).
         project(s) : str, list
             The project name (can be partial, i.e. any task protocol containing that str
             will be found).
         performance_lte / performance_gte : float
@@ -2026,14 +2062,44 @@
         Returns
         -------
         list
             List of eids.
         (list of dicts)
             If details is True, also returns a list of dictionaries, each entry corresponding to a
             matching session.
+
+        Examples
+        --------
+        Search for sessions with 'training' in the task protocol.
+
+        >>> eids = one.search(task='training')
+
+        Search for sessions by subject 'MFD_04'.
+
+        >>> eids = one.search(subject='MFD_04')
+
+        Do an exact search for sessions by subject 'FD_04'.
+
+        >>> assert one.wildcards is True, 'the wildcards flag must be True for regex expressions'
+        >>> eids = one.search(subject='^FD_04$', query_type='local')
+
+        Search for sessions on a given date, in a given lab, containing trials and spike data.
+
+        >>> eids = one.search(date='2023-01-01', lab='churchlandlab', dataset=['trials', 'spikes'])
+
+        Notes
+        -----
+        - In default and local mode, most queries are case-sensitive partial matches. When lists
+          are provided, the search is a logical OR, except for `datasets`, which is a logical AND.
+        - All search terms are true for a session to be returned, i.e. subject matches AND project
+          matches, etc.
+        - In remote mode most queries are case-insensitive partial matches.
+        - In default and local mode, when the one.wildcards flag is True (default), queries are
+          interpreted as regular expressions. To turn this off set one.wildcards to False.
+        - In remote mode regular expressions are only supported using the `django` argument.
         """
         query_type = query_type or self.mode
         if query_type != 'remote':
             return super(OneAlyx, self).search(details=details, query_type=query_type, **kwargs)
 
         # loop over input arguments and build the url
         search_terms = self.search_terms(query_type=query_type)
@@ -2569,40 +2635,40 @@
             if rel_path.endswith(dset_name):
                 return idx[-1]  # (eid, did)
         raise ValueError(f'Dataset {dset_name} not found in cache')
 
     @util.refresh
     @util.parse_id
     def get_details(self, eid: str, full: bool = False, query_type=None):
-        """Return session details for a given session
+        """Return session details for a given session.
 
         Parameters
         ----------
         eid : str, UUID, pathlib.Path, dict, list
             Experiment session identifier; may be a UUID, URL, experiment reference string
             details dict or Path.
         full : bool
-            If True, returns a DataFrame of session and dataset info
+            If True, returns a DataFrame of session and dataset info.
         query_type : {'local', 'refresh', 'auto', 'remote'}
             The query mode - if 'local' the details are taken from the cache tables; if 'remote'
             the details are returned from the sessions REST endpoint; if 'auto' uses whichever
             mode ONE is in; if 'refresh' reloads the cache before querying.
 
         Returns
         -------
         pd.Series, pd.DataFrame, dict
             in local mode - a session record or full DataFrame with dataset information if full is
-            True; in remote mode - a full or partial session dict
+            True; in remote mode - a full or partial session dict.
 
         Raises
         ------
         ValueError
-            Invalid experiment ID (failed to parse into eid string)
+            Invalid experiment ID (failed to parse into eid string).
         requests.exceptions.HTTPError
-            [Errno 404] Remote session not found on Alyx
+            [Errno 404] Remote session not found on Alyx.
         """
         if (query_type or self.mode) == 'local':
             return super().get_details(eid, full=full)
         # If eid is a list of eIDs recurse through list and return the results
         if isinstance(eid, list):
             details_list = []
             for p in eid:
```

### Comparing `ONE-api-2.1.0/one/converters.py` & `ONE-api-2.2.0/one/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,20 @@
     given the latter, a list is returned.  This decorator is intended to work on class methods,
     therefore the first arg is assumed to be the object.  Maps and pandas objects are not
     iterated over.
 
     Parameters
     ----------
     func : function
-        A method to decorate
+        A method to decorate.
 
     Returns
     -------
     function
-        The decorated method
+        The decorated method.
     """
     @functools.wraps(func)
     def wrapper_decorator(*args, **kwargs):
         if len(args) <= 1:
             return func(*args, **kwargs)
         obj, first = args[:2]
         exclude = (str, Mapping, pd.Series, pd.DataFrame)
@@ -342,31 +342,31 @@
         file = Path(self.cache_dir, session_path, rel_path)
         return file  # files[0] if len(datasets) == 1 else files
 
     @recurse
     def eid2ref(self, eid: Union[str, Iter], as_dict=True, parse=True) \
             -> Union[str, Mapping, List]:
         """
-        Get human-readable session ref from path
+        Get human-readable session ref from path.
 
         Parameters
         ----------
         eid : str, uuid.UUID
-            The experiment uuid to find reference for
+            The experiment uuid to find reference for.
         as_dict : bool
-            If false a string is returned in the form 'subject_sequence_yyyy-mm-dd'
+            If false a string is returned in the form 'subject_sequence_yyyy-mm-dd'.
         parse : bool
             If true, the reference date and sequence are parsed from strings to their respective
-            data types
+            data types.
 
         Returns
         -------
         dict, str, list
             One or more objects with keys ('subject', 'date', 'sequence'), or strings with the
-            form yyyy-mm-dd_n_subject
+            form yyyy-mm-dd_n_subject.
 
         Examples
         --------
         >>> eid = '4e0b3320-47b7-416e-b842-c34dc9004cf8'
         >>> one.eid2ref(eid)
         {'subject': 'flowers', 'date': datetime.date(2018, 7, 13), 'sequence': 1}
         >>> one.eid2ref(eid, parse=False)
@@ -389,26 +389,26 @@
             }
             format_str = '{date:s}_{sequence:s}_{subject:s}'
         return Bunch(ref) if as_dict else format_str.format(**ref)
 
     @recurse
     def ref2eid(self, ref: Union[Mapping, str, Iter]) -> Union[str, List]:
         """
-        Returns experiment uuid, given one or more experiment references
+        Returns experiment uuid, given one or more experiment references.
 
         Parameters
         ----------
         ref : str, dict, list
             One or more objects with keys ('subject', 'date', 'sequence'), or strings with
-            the form yyyy-mm-dd_n_subject
+            the form yyyy-mm-dd_n_subject.
 
         Returns
         -------
         str, list
-            One or more experiment uuid strings
+            One or more experiment uuid strings.
 
         Examples
         --------
         >>> base = 'https://test.alyx.internationalbrainlab.org'
         >>> one = ONE(username='test_user', password='TapetesBloc18', base_url=base)
         Connected to...
         >>> ref = {'date': datetime(2018, 7, 13).date(), 'sequence': 1, 'subject': 'flowers'}
@@ -425,26 +425,26 @@
             number=ref['sequence'])
         assert len(session) == 1, 'session not found'
         return session[0]
 
     @recurse
     def ref2path(self, ref):
         """
-        Convert one or more experiment references to session path(s)
+        Convert one or more experiment references to session path(s).
 
         Parameters
         ----------
         ref : str, dict, list
             One or more objects with keys ('subject', 'date', 'sequence'), or strings with
-            the form yyyy-mm-dd_n_subject
+            the form yyyy-mm-dd_n_subject.
 
         Returns
         -------
         pathlib.Path
-            Path object(s) for the experiment session(s)
+            Path object(s) for the experiment session(s).
 
         Examples
         --------
         >>> base = 'https://test.alyx.internationalbrainlab.org'
         >>> one = ONE(username='test_user', password='TapetesBloc18', base_url=base)
         Connected to...
         >>> ref = {'subject': 'flowers', 'date': datetime(2018, 7, 13).date(), 'sequence': 1}
@@ -464,22 +464,22 @@
         """
         Returns a human readable experiment reference, given a session path.
         The path need not exist.
 
         Parameters
         ----------
         path_str : str
-            A path to a given session
+            A path to a given session.
         as_dict : bool
-            If True a Bunch is returned, otherwise a string
+            If True a Bunch is returned, otherwise a string.
 
         Returns
         -------
         dict, str, list
-            One or more objects with keys ('subject', 'date', 'sequence')
+            One or more objects with keys ('subject', 'date', 'sequence').
 
         Examples
         --------
         >>> path_str = Path('E:/FlatIron/Subjects/zadorlab/flowers/2018-07-13/001')
         >>> path2ref(path_str)
         {'subject': 'flowers', 'date': datetime.date(2018, 7, 13), 'sequence': 1}
         >>> path2ref(path_str, parse=False)
@@ -496,26 +496,26 @@
         if match:
             ref = match.groupdict()
             return Bunch(ref) if as_dict else '{date:s}_{sequence:s}_{subject:s}'.format(**ref)
 
     @staticmethod
     def is_exp_ref(ref: Union[str, Mapping, Iter]) -> Union[bool, List[bool]]:
         """
-        Returns True is ref is a valid experiment reference
+        Returns True is ref is a valid experiment reference.
 
         Parameters
         ----------
         ref : str, dict, list
             One or more objects with keys ('subject', 'date', 'sequence'), or strings with
-            the form yyyy-mm-dd_n_subject
+            the form yyyy-mm-dd_n_subject.
 
         Returns
         -------
         bool
-            True if ref is valid
+            True if ref is valid.
 
         Examples
         --------
         >>> ref = {'date': datetime(2018, 7, 13).date(), 'sequence': 1, 'subject': 'flowers'}
         >>> is_exp_ref(ref)
         True
         >>> is_exp_ref('2018-07-13_001_flowers')
@@ -533,25 +533,25 @@
             return False
         return re.compile(r'\d{4}(-\d{2}){2}_(\d{1}|\d{3})_\w+').match(ref) is not None
 
     @staticmethod
     @parse_values
     def ref2dict(ref: Union[str, Mapping, Iter]) -> Union[Bunch, List]:
         """
-        Returns a Bunch (dict-like) from a reference string (or list thereof)
+        Returns a Bunch (dict-like) from a reference string (or list thereof).
 
         Parameters
         ----------
         ref : str, list
-            One or more experiment reference strings
+            One or more experiment reference strings.
 
         Returns
         -------
         iblutil.util.Bunch
-            A Bunch in with keys ('subject', 'sequence', 'date')
+            A Bunch in with keys ('subject', 'sequence', 'date').
 
         Examples
         --------
         >>> ref2dict('2018-07-13_1_flowers')
         {'date': datetime.date(2018, 7, 13), 'sequence': 1, 'subject': 'flowers'}
         >>> ref2dict('2018-07-13_001_flowers', parse=False)
         {'date': '2018-07-13', 'sequence': '001', 'subject': 'flowers'}
@@ -570,20 +570,20 @@
     def dict2ref(ref_dict) -> Union[str, List]:
         """
         Convert an experiment reference dict to a string in the format yyyy-mm-dd_n_subject.
 
         Parameters
         ----------
         ref_dict : dict, Bunch, list, tuple
-            A map with the keys ('subject', 'date', 'sequence')
+            A map with the keys ('subject', 'date', 'sequence').
 
         Returns
         -------
         str, list:
-            An experiment reference string, or list thereof
+            An experiment reference string, or list thereof.
         """
         if isinstance(ref_dict, (list, tuple)):
             return [ConversionMixin.dict2ref(x) for x in ref_dict]
         if not ref_dict:
             return
         parsed = any(not isinstance(k, str) for k in ref_dict.values())
         format_str = ('{date:%Y-%m-%d}_{sequence:d}_{subject:s}'
@@ -596,47 +596,47 @@
     """
     Returns local one file path from a dset record or a list of dsets records from REST.
     Unlike `to_eid`, this function does not require ONE, and the dataset may not exist.
 
     Parameters
     ----------
     dset : dict, list
-        Dataset dictionary or list of dictionaries from Alyx rest endpoint
+        Dataset dictionary or list of dictionaries from Alyx rest endpoint.
     one_cache : str, pathlib.Path, pathlib.PurePath
-        The local ONE data cache directory
+        The local ONE data cache directory.
 
     Returns
     -------
     pathlib.Path
-        The local path for a given dataset
+        The local path for a given dataset.
     """
     return path_from_dataset(dset, root_path=one_cache, uuid=False)
 
 
 def path_from_dataset(dset, root_path=PurePosixPath('/'), repository=None, uuid=False):
     """
     Returns the local file path from a dset record from a REST query.
     Unlike `to_eid`, this function does not require ONE, and the dataset may not exist.
 
     Parameters
     ----------
     dset : dict, list
-        Dataset dictionary or list of dictionaries from Alyx rest endpoint
+        Dataset dictionary or list of dictionaries from Alyx rest endpoint.
     root_path : str, pathlib.Path, pathlib.PurePath
-        The prefix path such as the ONE download directory or remote http server root
+        The prefix path such as the ONE download directory or remote http server root.
     repository : str, None
         Which data repository to use from the file_records list, defaults to first online
-        repository
+        repository.
     uuid : bool
-        If True, the file path will contain the dataset UUID
+        If True, the file path will contain the dataset UUID.
 
     Returns
     -------
     pathlib.Path, list
-        File path or list of paths
+        File path or list of paths.
     """
     if isinstance(dset, list):
         return [path_from_dataset(d) for d in dset]
     if repository:
         fr = next((fr for fr in dset['file_records'] if fr['data_repository'] == repository))
     else:
         fr = next((fr for fr in dset['file_records'] if fr['data_url']))
@@ -649,24 +649,24 @@
     Returns a data file Path constructed from an Alyx file record.  The Path type returned
     depends on the type of root_path: If root_path is a string a Path object is returned,
     otherwise if the root_path is a PurePath, the same path type is returned.
 
     Parameters
     ----------
     fr : dict
-        An Alyx file record dict
+        An Alyx file record dict.
     root_path : str, pathlib.Path
-        An optional root path
+        An optional root path.
     uuid : str, uuid.UUID
-        An optional dataset UUID to add to the file name
+        An optional dataset UUID to add to the file name.
 
     Returns
     -------
     pathlib.Path
-        A filepath as a pathlib object
+        A filepath as a pathlib object.
     """
     if isinstance(fr, list):
         return [path_from_filerecord(f) for f in fr]
     repo_path = (p := fr['data_repository_path'])[p[0] == '/':]  # Remove slash at start, if any
     file_path = PurePosixPath(repo_path, fr['relative_path'])
     if root_path:
         # NB: By checking for string we won't cast any PurePaths
```

### Comparing `ONE-api-2.1.0/one/params.py` & `ONE-api-2.2.0/one/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,22 +38,22 @@
 def _get_current_par(k, par_current):
     """
     Return the current parameter value or the default.
 
     Parameters
     ----------
     k : str
-        The parameter key lookup
+        The parameter key lookup.
     par_current : IBLParams
-        The current parameter set
+        The current parameter set.
 
     Returns
     -------
     any
-        The current parameter value or default if None or not set
+        The current parameter value or default if None or not set.
     """
     cpar = getattr(par_current, k, None)
     if cpar is None:
         cpar = getattr(default(), k, None)
     return cpar
 
 
@@ -61,20 +61,20 @@
     """
     Convert a URL str to one valid for use as a file name or dict key.  URL Protocols are
     removed entirely.  The returned string will have characters in the set [a-zA-Z.-_].
 
     Parameters
     ----------
     url : str
-        A URL string
+        A URL string.
 
     Returns
     -------
     str
-        A filename-safe string
+        A filename-safe string.
 
     Example
     -------
     >>> url = _key_from_url('http://test.alyx.internationalbrainlab.org/')
    'test.alyx.internationalbrainlab.org'
     """
     url = unicodedata.normalize('NFKC', url)  # Ensure ASCII
```

### Comparing `ONE-api-2.1.0/one/registration.py` & `ONE-api-2.2.0/one/registration.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,18 +428,18 @@
         -------
         list of dicts, dict
             A list of newly created Alyx dataset records or the registration data if dry.
 
         Notes
         -----
         - The registered files may be automatically moved to new revision folders if they are
-         protected on Alyx, therefore it's important to check the relative paths of the output.
+          protected on Alyx, therefore it's important to check the relative paths of the output.
         - Protected datasets are not checked in dry mode.
         - In most circumstances a new revision will be added automatically, however if this fails
-         a 403 HTTP status may be returned.
+          a 403 HTTP status may be returned.
 
         Raises
         ------
         requests.exceptions.HTTPError
             Submitted data not valid (400 status code)
             Server side database error (500 status code)
             Revision protected (403 status code)
```

### Comparing `ONE-api-2.1.0/one/remote/aws.py` & `ONE-api-2.2.0/one/remote/aws.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,17 +160,17 @@
         An S3 ServiceResource instance with the provided.
     str
         The name of the S3 bucket.
 
     Notes
     -----
     - If no credentials are present in the database, boto3 will use environment config or default
-     AWS profile settings instead.
+      AWS profile settings instead.
     - If there are no credentials for the bucket and the bucket has 'public' in the name, the
-     returned resource will use an unsigned signature.
+      returned resource will use an unsigned signature.
     """
     session_keys, bucket_name = get_aws_access_keys(alyx, repo_name)
     no_creds = not any(filter(None, (v for k, v in session_keys.items() if 'key' in k.lower())))
     session = boto3.Session(**session_keys)
     if no_creds and 'public' in bucket_name.lower():
         config = Config(signature_version=UNSIGNED)
     else:
```

### Comparing `ONE-api-2.1.0/one/remote/base.py` & `ONE-api-2.2.0/one/remote/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 Includes the DownloadClient superclass.
 
 TODO Currently record2url assumes all data are stored on a single HTTP data server. Data repos
  are not stored in the cache tables so should by default use HTTP data server but could get
  address by precedence.  NB: OneAlyx._download_dataset uses record2url then calls
  AlyxClient.download_file.
 TODO Could have .one/.params file that stores ONE state, including whether files are distributed?
-TODO Release changes to alyx repo first
 """
 from abc import abstractmethod
 import logging
 
 from iblutil.io import params as iopar
 
 from one.params import _PAR_ID_STR
@@ -52,17 +51,17 @@
     -------
     IBLParams, None
         Download client parameters or None if assert_present is False and no parameters found.
 
     Raises
     ------
     FileNotFoundError
-        No one/remote JSON file found
+        No one/remote JSON file found.
     AttributeError
-        Provided client key not present in one/remote params
+        Provided client key not present in one/remote params.
 
     Examples
     --------
     Load all remote parameters
 
     >>> pars = load_client_params()
 
@@ -91,50 +90,50 @@
     """
     Save parameters into the remote params file.  If a client key is provided, parameters are
     saved into this field.
 
     Parameters
     ----------
     new_pars : dict, IBLParams
-        A set or subset or parameters to save
+        A set or subset or parameters to save.
     client_key : str
         An optional, specific client whose parameters to save.
 
     Raises
     ------
     ValueError
-        If client_key is None, all parameter fields must hold dicts
+        If client_key is None, all parameter fields must hold dicts.
     """
     if not client_key:
         if not all(isinstance(x, dict) for x in iopar.as_dict(new_pars).values()):
             raise ValueError('Not all parameter fields contain dicts')
         return iopar.write(PAR_ID_STR, new_pars)  # Save all parameters
     # Save parameters into client key field
     pars = iopar.as_dict(iopar.read(PAR_ID_STR, {}) or {})
     pars[client_key] = iopar.as_dict(new_pars)
     iopar.write(PAR_ID_STR, pars)
 
 
 class DownloadClient:
-    """Data download handler base class"""
+    """Data download handler base class."""
     def __init__(self):
         pass
 
     @abstractmethod
     def to_address(self, data_path, *args, **kwargs):
-        """Returns the remote data URL for a given ALF path"""
+        """Returns the remote data URL for a given ALF path."""
         pass  # pragma: no cover
 
     @abstractmethod
-    def download_file(self, file_address):
-        """Download an ALF dataset given its address"""
+    def download_file(self, file_address, *args, **kwargs):
+        """Download an ALF dataset given its address."""
         pass  # pragma: no cover
 
     @staticmethod
     @abstractmethod
     def setup(*args, **kwargs):
         pass  # pragma: no cover
 
     @staticmethod
     def repo_from_alyx(name, alyx):
-        """Return the data repository information for a given data repository"""
+        """Return the data repository information for a given data repository."""
         return alyx.rest('data-repository', 'read', id=name)
```

### Comparing `ONE-api-2.1.0/one/remote/globus.py` & `ONE-api-2.2.0/one/remote/globus.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,62 @@
-"""A module for handling file operations through the Globus SDK"""
+"""A module for handling file operations through the Globus SDK.
+
+Setup
+-----
+
+To set up Globus simply instantiate the `Globus` class for the first time and follow the prompts.
+Providing a client name string to the constructor allows one to set up multiple Globus clients
+(i.e. when switching between different Globus client IDs).
+
+Examples
+--------
+
+Asynchronously transfer data between Alyx repositories
+
+>>> alyx = AlyxClient()
+>>> glo = Globus('admin')
+>>> glo.add_endpoint('flatiron_cortexlab', alyx=alyx)
+>>> glo.add_endpoint('cortex_lab_SR', alyx=alyx)
+>>> task_id = glo.transfer_data('path/to/file', 'flatiron_cortexlab', 'cortex_lab_SR')
+
+Synchronously transfer data to an alternate local location
+
+>>> from functools import partial
+>>> root_path = '/path/to/new/location'
+>>> glo.add_endpoint(get_local_endpoint_id(), label='alternate_local', root_path=root_path)
+>>> folder = 'camera/ZFM-01867/2021-03-23/002'  # An example folder to download
+>>> task = partial(glo.transfer_data, folder, 'integration', 'integration_local',
+...                label='alternate data', recursive=True)
+>>> task_id = glo.run_task(task)  # Submit task to Globus and await completion
+
+Temporarily change local data root path and synchronously download file
+
+>>> glo.endpoints['local']['root_path'] = '/path/to/new/location'
+>>> file = glo.download_file('path/to/file.ext', 'source_endpoint')
+Path('/path/to/new/location/path/to/file.ext')
+"""
 import os
 import re
 import sys
 import logging
+from uuid import UUID
 from pathlib import Path, PurePosixPath, PurePath, PureWindowsPath
 import warnings
+from functools import partial
 
 import globus_sdk
 from globus_sdk import TransferAPIError, GlobusAPIError, NetworkError, GlobusTimeoutError, \
     GlobusConnectionError, GlobusConnectionTimeoutError
 from iblutil.io import params as iopar
 
 from one.alf.spec import is_uuid
 from one.alf.files import remove_uuid_string
 import one.params
 from one.webclient import AlyxClient
+from one.util import ensure_list
 from .base import DownloadClient, load_client_params, save_client_params
 
 _logger = logging.getLogger(__name__)
 CLIENT_KEY = 'globus'
 DEFAULT_PAR = {'GLOBUS_CLIENT_ID': None, 'local_endpoint': None, 'local_path': None}
 
 
@@ -70,16 +108,16 @@
         message += f' (default: {default_endpoint})'
     except AssertionError:
         default_endpoint = ''
         warnings.warn(
             'Cannot find local endpoint ID. Beware that this might mean that Globus Connect '
             'is not set up properly.')
     pars['local_endpoint'] = input(message + ':').strip() or default_endpoint
-    if not pars['local_endpoint']:
-        raise ValueError('Globus local endpoint ID is a required field')
+    if not is_uuid(pars['local_endpoint'], (1, 2)):
+        raise ValueError('Globus local endpoint ID must be a UUID version 1 or 2')
 
     # Check for local path
     message = 'Please enter the local endpoint path'
     local_path = pars['local_path'] or one.params.get(silent=True).CACHE_DIR
     message += f' (default: {local_path})'
     pars['local_path'] = input(message + ':').strip() or local_path
 
@@ -130,30 +168,30 @@
 
 def get_local_endpoint_id():
     """
     Extracts the ID of the local Globus Connect endpoint.
 
     Returns
     -------
-    str
+    uuid.UUID
         The local Globus endpoint ID
     """
     msg = ('Cannot find local endpoint ID, check if Globus Connect is set up correctly, '
            '{} exists and contains a UUID.')
     if sys.platform in ('win32', 'cygwin'):
         id_path = Path(os.environ['LOCALAPPDATA']).joinpath('Globus Connect')
     else:
         id_path = Path.home().joinpath('.globusonline', 'lta')
 
     id_file = id_path.joinpath('client-id.txt')
     assert id_file.exists(), msg.format(id_file)
     local_id = id_file.read_text().strip()
     assert isinstance(local_id, str), msg.format(id_file)
     print(f'Found local endpoint ID in Globus Connect settings {local_id}')
-    return local_id
+    return UUID(local_id)
 
 
 def get_local_endpoint_paths():
     """
     Extracts the local endpoint paths accessible by Globus Connect.  NB: This is only supported
     on Linux.
 
@@ -210,41 +248,46 @@
 def as_globus_path(path):
     """
     Convert a path into one suitable for the Globus TransferClient.
 
     Parameters
     ----------
     path : pathlib.Path, pathlib.PurePath, str
-        A path to convert to a Globus-complient path string
+        A path to convert to a Globus-complient path string.
 
     Returns
     -------
     str
-        A formatted path string
+        A formatted path string.
 
     Notes
     -----
     - If using tilda in path, the home folder of your Globus Connect instance must be the same as
       the OS home dir.
     - If validating a path for another system ensure the input path is a PurePath, in particular,
-    on a Linux computer a remote Windows should first be made into a PureWindowsPath.
+      on a Linux computer a remote Windows should first be made into a PureWindowsPath.
 
     Examples
     --------
-    A Windows path
+    A Windows path (on Windows OS)
 
     >>> as_globus_path('E:\\FlatIron\\integration')
     '/E/FlatIron/integration'
 
-    A relative POSIX path
+    When explicitly a POSIX path, remains unchanged
+
+    >>> as_globus_path(PurePosixPath('E:\\FlatIron\\integration'))
+    'E:\\FlatIron\\integration'
+
+    A relative POSIX path (on *nix OS)
 
     >>> as_globus_path('../data/integration')
     '/mnt/data/integration'
 
-    A globus path
+    A valid Globus path remains unchanged
 
     >>> as_globus_path('/E/FlatIron/integration')
     '/E/FlatIron/integration'
     """
     is_pure_path = isinstance(path, PurePath)
     is_win = sys.platform in ('win32', 'cygwin') or isinstance(path, PureWindowsPath)
     if isinstance(path, str):
@@ -261,32 +304,170 @@
         path = '/' + str(path.as_posix().replace(':', '', 1))
     return str(path)
 
 
 class Globus(DownloadClient):
     """Wrapper for managing files on Globus endpoints."""
     def __init__(self, client_name='default'):
+        """
+        Wrapper for managing files on Globus endpoints.
+
+        Parameters
+        ----------
+        client_name : str
+            Parameter profile name to load e.g. 'default', 'admin'.
+        """
         # Setting up transfer client
         super().__init__()
         self.client = create_globus_client(client_name=client_name)
         self.pars = load_client_params(f'{CLIENT_KEY}.{client_name}')
         # Try adding local endpoint
-        self.endpoints = {'local': {'id': self.pars.local_endpoint}}
+        self.endpoints = {'local': {'id': UUID(self.pars.local_endpoint)}}
         _logger.info('Adding local endpoint.')
         self.endpoints['local']['root_path'] = self.pars.local_path
 
+    def fetch_endpoints_from_alyx(self, alyx=None, overwrite=False):
+        """
+        Update endpoints property with Alyx Globus data repositories.
+
+        Parameters
+        ----------
+        alyx : one.webclient.AlyxClient
+            An optional AlyxClient.
+        overwrite : bool
+            Whether existing endpoint with the same label should be replaced.
+
+        Returns
+        -------
+        dict
+            The endpoints added from Alyx.
+        """
+        alyx = alyx or AlyxClient()
+        alyx_endpoints = alyx.rest('data-repository', 'list')
+        for endpoint in alyx_endpoints:
+            if not endpoint['globus_endpoint_id']:
+                continue
+            uid = UUID(endpoint['globus_endpoint_id'])
+            self.add_endpoint(
+                uid, label=endpoint['name'], root_path=endpoint['globus_path'], overwrite=overwrite
+            )
+        endpoint_names = {e['name'] for e in alyx_endpoints}
+        return {k: v for k, v in self.endpoints.items() if k in endpoint_names}
+
     def to_address(self, data_path, endpoint):
-        pass  # pragma: no cover
+        """
+        Get full path for a given endpoint.
 
-    def download_file(self, file_address):
-        pass  # pragma: no cover
+        Parameters
+        ----------
+        data_path : Path, PurePath, str
+            An absolute or relative POSIX path
+        endpoint : str, uuid.UUID
+            An endpoint label or UUID.
+
+        Returns
+        -------
+        str
+            A complete path string formatted for Globus.
+
+        Examples
+        --------
+        >>> glo = Globus()
+        >>> glo.add_endpoint('0ec47586-3a19-11eb-b173-0ee0d5d9299f',
+        ...                  label='foobar', root_path='/foo')
+        >>> glo.to_address('bar/baz.ext', 'foobar')
+        '/foo/bar/baz.ext'
+        """
+        _, root_path = self._endpoint_id_root(endpoint)
+        return self._endpoint_path(data_path, root_path)
+
+    def download_file(self, file_address, source_endpoint, recursive=False, **kwargs):
+        """
+        Download one or more files via Globus.
+
+        Parameters
+        ----------
+        file_address : str, list of str
+            One or more relative POSIX paths to download.
+        source_endpoint : str, uuid.UUID
+            The source endpoint name or uuid.
+        recursive : bool
+            If true, transfer the contents of nested directories (NB: all data_paths must be
+            directories).
+        **kwargs
+            See Globus.transfer_data.
+
+        Returns
+        -------
+        pathlib.Path, list of pathlib.Path
+            The downloaded file path(s). If recursive is True, a list is always returned.
+
+        Notes
+        -----
+        - Assumes that the local endpoint root path is NOT POSIX style on Windows.
+
+        TODO Return None for failed files
+
+        Examples
+        --------
+        Download a single file
+
+        >>> file = Globus().download_file('path/to/file', '0ec47586-3a19-11eb-b173-0ee0d5d9299f')
+
+        Download multiple files and verify checksum
+
+        >>> files = ['relative/file/path.ext', 'foo.bar']
+        >>> files = Globus().download_file(files, 'source_endpoint_name', verify_checksum=True)
+
+        Download a folder
+
+        >>> files = Globus().download_file('folder/path', 'source_endpoint_name', recursive=True)
+        """
+        return_single = isinstance(file_address, str) and recursive is False
+        kwargs['label'] = kwargs.get('label', 'ONE download')
+        task = partial(self.transfer_data, file_address, source_endpoint, 'local',
+                       sync_level='mtime', recursive=recursive, **kwargs)
+        task_id = self.run_task(task)
+        files = []
+        root = Path(self.endpoints['local']['root_path'])
+        idx = len(self._endpoint_path(PurePosixPath(as_globus_path(root))))
+        for info in self.client.task_successful_transfers(task_id):
+            files.append(info['destination_path'][idx:].strip('/'))
+
+        if return_single:
+            file = root / files[0]
+            assert file.exists()
+            return file
+
+        # Order files by input
+        def _best_match(x):
+            """Return the index of the input file that best matches downloaded file."""
+            spans = [len(frag) / len(x) if frag in x else 0 for frag in ensure_list(file_address)]
+            return spans.index(max(spans))
+        files = list(map(root.joinpath, sorted(files, key=_best_match)))
+        assert all(map(Path.exists, filter(None, files)))
+        return files
 
     @staticmethod
-    def setup(*args, **kwargs):
-        pass  # pragma: no cover
+    def setup(client_name='default'):
+        """
+        Setup a Globus client.
+
+        Parameters
+        ----------
+        client_name : str
+            Parameter profile name to set up e.g. 'default', 'admin'.
+
+        Returns
+        -------
+        Globus
+            A new Globus client object.
+        """
+        setup(client_name)
+        return Globus(client_name)
 
     def add_endpoint(self, endpoint, label=None, root_path=None, overwrite=False, alyx=None):
         """
         Add an endpoint to the Globus instance to be used by other functions.
 
         Parameters
         ----------
@@ -295,38 +476,39 @@
         label : str
             Label to access the endpoint. If endpoint is UUID this has to be set, otherwise is
             optional.
         root_path : str, pathlib.Path, pathlib.PurePath
             File path to be accessed by Globus on the endpoint.
         overwrite : bool
             Whether existing endpoint with the same label should be replaced.
-        alyx : webclient.AlyxClient
+        alyx : one.webclient.AlyxClient
             An AlyxClient instance for looking up repository information.
         """
-        if is_uuid(endpoint, versions=(1,)):  # MAC address UUID
+        if is_uuid(endpoint, versions=(1, 2)):  # MAC address UUID
             if label is None:
                 raise ValueError('If "endpoint" is a UUID, "label" cannot be None.')
-            endpoint_id = str(endpoint)
+            endpoint_id = self._ensure_uuid(endpoint)
         else:
             repo = self.repo_from_alyx(endpoint, alyx=alyx)
-            endpoint_id = repo['globus_endpoint_id']
+            endpoint_id = UUID(repo['globus_endpoint_id'])
             root_path = root_path or repo['globus_path']
             label = label or endpoint
         if label in self.endpoints.keys() and overwrite is False:
             _logger.error(f'An endpoint called "{label}" already exists. Choose a different label '
                           'or set overwrite=True')
         else:
             self.endpoints[label] = {'id': endpoint_id}
             if root_path:
                 self.endpoints[label]['root_path'] = root_path
 
     @staticmethod
     def _endpoint_path(path, root_path=None):
         """
         Given an absolute path or relative path with a root path, return a Globus path str.
+
         Note: Paths must be POSIX or Globus-compliant paths.  In other words for Windows systems
         the input root_path or absolute path must be passed through `as_globus_path` before
         calling this method.
 
         TODO include globus_path_from_dataset
 
         Parameters
@@ -355,29 +537,186 @@
             path = PurePosixPath(path)
         if root_path and not str(path).startswith(str(root_path)):
             path = PurePosixPath(root_path) / path
         if not path.is_absolute():
             raise ValueError(f'{path} is relative and no root_path defined')
         return as_globus_path(path)
 
+    @staticmethod
+    def _ensure_uuid(uid):
+        """
+        Ensures UUID object returned.
+
+        Parameters
+        ----------
+        uid : str, uuid.UUID
+            A UUID to cast to UUID object.
+
+        Returns
+        -------
+        uuid.UUID
+            A UUID object.
+        """
+        return UUID(uid) if not isinstance(uid, UUID) else uid
+
     def _endpoint_id_root(self, endpoint):
+        """
+        Return endpoint UUID and root path from a given endpoint identifier.
+
+        Parameters
+        ----------
+        endpoint : str, uuid.UUID
+            An endpoint label or UUID.
+
+        Returns
+        -------
+        uuid.UUID
+            The endpoint UUID.
+        str, None
+            The POSIX-style endpoint root path (if defined).
+
+        Warnings
+        --------
+        UserWarning
+            If endpoint UUID is associated with multiple root paths, it is better to provide the
+            endpoint label to avoid this warning and to ensure the intended root path is returned.
+
+        See Also
+        --------
+        Globus._sanitize_local
+        """
         root_path = None
         if endpoint in self.endpoints.keys():
             endpoint_id = self.endpoints[endpoint]['id']
             if 'root_path' in self.endpoints[endpoint].keys():
-                root_path = str(self.endpoints[endpoint]['root_path'])
-            return endpoint_id, root_path
+                root_path = self.endpoints[endpoint]['root_path']
+            return self._sanitize_local(endpoint_id, root_path)
         elif is_uuid(endpoint, range(1, 5)):
-            endpoint_id = endpoint
-            return endpoint_id, None
+            # If a UUID was provided, find the first endpoint with a root path with the UUID
+            endpoint_id = self._ensure_uuid(endpoint)
+            matching = (
+                k for k, v in self.endpoints.items() if v['id'] == endpoint_id and 'root_path' in v
+            )
+            if name := next(matching, None):
+                # Warn of ambiguity if multiple endpoints share a UUID
+                if next(matching, None) is not None:
+                    warnings.warn(
+                        f'Multiple endpoints added with the same UUID, '
+                        f'using root path from "{name}"')
+                root_path = self.endpoints[name]['root_path']
+            else:
+                root_path = None
+            return self._sanitize_local(endpoint_id, root_path)
         else:
             raise ValueError(
                 '"endpoint" must be a UUID or the label of an endpoint registered in this '
                 'Globus instance. You can add endpoints via the add_endpoints method')
 
+    def _sanitize_local(self, endpoint_id, root_path):
+        """
+        Ensure local root path on Windows is POSIX-style.
+
+        Parameters
+        ----------
+        endpoint_id : uuid.UUID
+            The endpoint UUID to determine if root path is local.
+        root_path : pathlib.Path, str, None
+            The root path to sanitize.
+
+        Returns
+        -------
+        endpoint_id : uuid.UUID
+            The endpoint UUID, returned unchanged to match `Globus._endpoint_id_root` signature.
+        str, None
+            The root path as a POSIX style string, or None if root_path is None.
+
+        Examples
+        --------
+        Providing a local root path on Windows
+
+        >>> glo = Globus()
+        >>> uid = glo.endpoints['local']['id']
+        >>> glo._sanitize_local(uid, 'C:\\Data')
+        UUID('50282ed5-3124-11ee-b977-482ae33bf6ca'), '/C/Data'
+
+        Path left unchanged on *nix systems or when endpoint ID is not local
+
+        >>> uid = UUID('c7c46cec-3124-11ee-bf50-482ae33bf6ca')
+        >>> glo._sanitize_local(uid, 'C:\\Data')
+        UUID('c7c46cec-3124-11ee-bf50-482ae33bf6ca'), 'C:\\Data'
+        """
+        if not root_path:
+            return endpoint_id, None
+        # If the local root path is not explicitly a Windows Path and we're on windows, make sure
+        # it's converted correctly to a POSIX style path
+        if isinstance(root_path, str):
+            is_win = sys.platform in ('win32', 'cygwin')
+            if endpoint_id == self.endpoints['local']['id'] and is_win:
+                root_path = PureWindowsPath(root_path)
+            else:
+                root_path = PurePosixPath(root_path)
+        return endpoint_id, as_globus_path(root_path)
+
+    def transfer_data(self, data_path, source_endpoint, destination_endpoint,
+                      recursive=False, **kwargs):
+        """
+        Transfer one or more paths between endpoints.
+
+        At least one of the endpoints must be a server endpoint.  Both file and directory paths may
+        be provided, however if recursive is true, all paths must be directories.
+
+        Parameters
+        ----------
+        data_path : str, list of str
+            One or more data paths, relative to the endpoint root path.
+        source_endpoint : str, uuid.UUID
+            The name or UUID of the source endpoint.
+        destination_endpoint : str, uuid.UUID
+            The name or UUID of the destination endpoint.
+        recursive : bool
+            If true, transfer the contents of nested directories (NB: all data_paths must be
+            directories).
+        **kwargs
+            See globus_sdk.TransferData.
+
+        Returns
+        -------
+        uuid.UUID
+            The Globus transfer ID.
+
+        Examples
+        --------
+        Transfer two files (asynchronous)
+
+        >>> glo = Globus()
+        >>> files = ['file.ext', 'foo.bar']
+        >>> task_id = glo.transfer_data(files, 'source_endpoint', 'destination_endpoint')
+
+        Transfer a folder (asynchronous)
+
+        >>> folder = 'path/to/folder'
+        >>> task_id = glo.transfer_data(
+        ...    folder, 'source_endpoint', 'destination_endpoint', recursive=True)
+        """
+        kwargs['source_endpoint'] = (source_endpoint
+                                     if is_uuid(source_endpoint, versions=(1,))
+                                     else self.endpoints.get(source_endpoint)['id'])
+        kwargs['destination_endpoint'] = (destination_endpoint
+                                          if is_uuid(destination_endpoint, versions=(1,))
+                                          else self.endpoints.get(destination_endpoint)['id'])
+        transfer_object = globus_sdk.TransferData(self.client, **kwargs)
+
+        # add any number of items to the submission data
+        for path in ensure_list(data_path):
+            src = self._endpoint_path(path, self._endpoint_id_root(source_endpoint)[1])
+            dst = self._endpoint_path(path, self._endpoint_id_root(destination_endpoint)[1])
+            transfer_object.add_item(src, dst, recursive=recursive)
+        response = self.client.submit_transfer(transfer_object)
+        return UUID(response.data['task_id'])
+
     def ls(self, endpoint, path, remove_uuid=False, return_size=False, max_retries=1):
         """
         Return the list of (filename, filesize) in a given endpoint directory.
         NB: If you're using ls routinely when transferring or deleting files you're probably doing
         something wrong!
 
         Parameters
@@ -444,15 +783,15 @@
         timeout : int
             Maximum time in seconds to wait for the task to complete.
         kwargs
             Optional arguments for globus_sdk.TransferData.
 
         Returns
         -------
-        int
+        uuid.UUID
             A Globus task ID.
         """
         source_endpoint, source_root = self._endpoint_id_root(source_endpoint)
         target_endpoint, target_root = self._endpoint_id_root(target_endpoint)
         source_paths = [str(self._endpoint_path(path, source_root)) for path in source_paths]
         target_paths = [str(self._endpoint_path(path, target_root)) for path in target_paths]
 
@@ -471,36 +810,38 @@
         return self.run_task(wrapper, timeout=timeout)
 
     def run_task(self, globus_func, retries=3, timeout=None):
         """
         Block until a Globus task finishes and retry upon Network or REST Errors.
         globus_func needs to submit a task to the client and return a task_id.
 
-
         Parameters
         ----------
-        globus_func : function
+        globus_func : function, Callable
             A function that returns a Globus task ID, typically it will submit a transfer.
         retries : int
             The number of times to call globus_func if it raises a Globus error.
         timeout : int
             Maximum time in seconds to wait for the task to complete.
 
         Returns
         -------
-        int
+        uuid.UUID
             Globus task ID.
 
         Raises
         ------
         IOError
             Timed out waiting for task to complete.
+
+        TODO Add a quick fail option that returns when files missing, etc.
         """
         try:
             task_id = globus_func()
+            assert is_uuid(task_id, versions=(1, 2)), 'invalid UUID returned'
             print(f'Waiting for Globus task {task_id} to complete')
             # While the task with task is active, print a dot every second. Timeout after timeout
             i = 0
             while not self.client.task_wait(task_id, timeout=5, polling_interval=1):
                 print('.', end='')
                 i += 1
                 if timeout and i >= timeout:
@@ -520,15 +861,15 @@
                     for info in successful:
                         _logger.debug(f'{info["source_path"]} -> {info["destination_path"]}')
                 except TransferAPIError:
                     _logger.warning(f'\nGlobus task {task_id} SUCCEEDED but querying transfers was'
                                     f'unsuccessful')
             else:
                 raise IOError(f'Globus task finished unsuccessfully with status {task["status"]}')
-            return task_id
+            return self._ensure_uuid(task_id)
         except (GlobusAPIError, NetworkError, GlobusTimeoutError, GlobusConnectionError,
                 GlobusConnectionTimeoutError) as e:
             if retries < 1:
                 _logger.error('\nMax retries exceeded.')
                 raise e
             else:
                 _logger.debug('\nGlobus experienced a network error', exc_info=True)
```

### Comparing `ONE-api-2.1.0/one/tests/fixtures/datasets.pqt` & `ONE-api-2.2.0/one/tests/fixtures/datasets.pqt`

 * *Files identical despite different names*

### Comparing `ONE-api-2.1.0/one/tests/fixtures/rest_responses/47893cf67c985e6361cdee009334963f49fb0746` & `ONE-api-2.2.0/one/tests/fixtures/rest_responses/47893cf67c985e6361cdee009334963f49fb0746`

 * *Files identical despite different names*

### Comparing `ONE-api-2.1.0/one/tests/fixtures/rest_responses/535d0e9a1e2c1efbdeba0d673b131e00361a2edb` & `ONE-api-2.2.0/one/tests/fixtures/rest_responses/535d0e9a1e2c1efbdeba0d673b131e00361a2edb`

 * *Files identical despite different names*

### Comparing `ONE-api-2.1.0/one/tests/fixtures/rest_responses/6dc96f7e9bcc6ac2e7581489b9580a6cd3f28293` & `ONE-api-2.2.0/one/tests/fixtures/rest_responses/6dc96f7e9bcc6ac2e7581489b9580a6cd3f28293`

 * *Files identical despite different names*

### Comparing `ONE-api-2.1.0/one/tests/fixtures/rest_responses/f530d6022f61cdc9e38cc66beb3cb71f3003c9a1` & `ONE-api-2.2.0/one/tests/fixtures/rest_responses/f530d6022f61cdc9e38cc66beb3cb71f3003c9a1`

 * *Files identical despite different names*

### Comparing `ONE-api-2.1.0/one/tests/fixtures/sessions.pqt` & `ONE-api-2.2.0/one/tests/fixtures/sessions.pqt`

 * *Files identical despite different names*

### Comparing `ONE-api-2.1.0/one/tests/fixtures/test_img.png` & `ONE-api-2.2.0/one/tests/fixtures/test_img.png`

 * *Files identical despite different names*

### Comparing `ONE-api-2.1.0/one/util.py` & `ONE-api-2.2.0/one/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Decorators and small standalone functions for api module"""
+"""Decorators and small standalone functions for api module."""
 import logging
 import urllib.parse
 from functools import wraps
 from typing import Sequence, Union, Iterable, Optional, List
 from collections.abc import Mapping
 import fnmatch
 from datetime import datetime
@@ -16,15 +16,15 @@
 from one.alf.files import rel_path_parts, get_session_path, get_alf_path, remove_uuid_string
 from one.alf.spec import FILE_SPEC, regex as alf_regex
 
 logger = logging.getLogger(__name__)
 
 
 def Listable(t):
-    """Return a typing.Union if the input and sequence of input"""
+    """Return a typing.Union if the input and sequence of input."""
     return Union[t, Sequence[t]]
 
 
 def ses2records(ses: dict):
     """Extract session cache record and datasets cache from a remote session data record.
 
     Parameters
@@ -333,16 +333,16 @@
     Filter by filename parts
 
     >>> datasets = filter_datasets(all_datasets, dict(object='spikes', attribute='times'))
 
     Notes
     -----
     - It is not possible to match datasets that are in a given collection OR NOT in ANY collection.
-     e.g. filter_datasets(dsets, collection=['alf', '']) will not match the latter. For this you
-     must use two separate queries.
+      e.g. filter_datasets(dsets, collection=['alf', '']) will not match the latter. For this you
+      must use two separate queries.
     """
     # Create a regular expression string to match relative path against
     filename = filename or {}
     regex_args = {'collection': collection}
     spec_str = _collection_spec(collection, None if revision_last_before else revision)
 
     if isinstance(filename, dict):
```

### Comparing `ONE-api-2.1.0/one/webclient.py` & `ONE-api-2.2.0/one/webclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""API for interacting with a remote Alyx instance through REST
+"""API for interacting with a remote Alyx instance through REST.
 The AlyxClient class contains methods for making remote Alyx REST queries and downloading remote
 files through Alyx.
 
 Examples
 --------
 >>> alyx = AlyxClient(
 ...     username='test_user', password='TapetesBloc18',
@@ -56,53 +56,53 @@
 from iblutil.io.params import set_hidden
 from one.util import ensure_list
 import concurrent.futures
 _logger = logging.getLogger(__name__)
 
 
 def _cache_response(method):
-    """Decorator for the generic request method
+    """Decorator for the generic request method.
 
     Caches the result of the query and on subsequent calls, returns cache instead of hitting the
-    database
+    database.
 
     Parameters
     ----------
     method : function
-        Function to wrap (i.e. AlyxClient._generic_request)
+        Function to wrap (i.e. AlyxClient._generic_request).
 
     Returns
     -------
     function
-        Handle to wrapped method
+        Handle to wrapped method.
     """
 
     @functools.wraps(method)
     def wrapper_decorator(alyx_client, *args, expires=None, clobber=False, **kwargs):
         """
-        REST caching wrapper
+        REST caching wrapper.
 
         Parameters
         ----------
         alyx_client : AlyxClient
-            An instance of the AlyxClient class
+            An instance of the AlyxClient class.
         args : any
-            Positional arguments for applying to wrapped function
+            Positional arguments for applying to wrapped function.
         expires : bool
             An optional timedelta for how long cached response is valid.  If True, the cached
             response will not be used on subsequent calls.  If None, the default expiry is applied.
         clobber : bool
-            If True any existing cached response is overwritten
-        kwargs : any
-            Keyword arguments for applying to wrapped function
+            If True any existing cached response is overwritten.
+        **kwargs
+            Keyword arguments for applying to wrapped function.
 
         Returns
         -------
         dict
-            The REST response JSON either from cached file or directly from remote
+            The REST response JSON either from cached file or directly from remote.
         """
         expires = expires or alyx_client.default_expiry
         mode = (alyx_client.cache_mode or '').lower()
         if args[0].__name__ != mode and mode != '*':
             return method(alyx_client, *args, **kwargs)
         # Check cache
         rest_cache = alyx_client.cache_dir.joinpath('.rest')
@@ -275,17 +275,17 @@
     Downloads a list of files from a remote HTTP server from a list of links.
     Generates up to 4 separate threads to handle downloads.
     Same options behaviour as http_download_file.
 
     Parameters
     ----------
     links_to_file_list : list
-        List of http links to files
-    kwargs
-        Optional arguments to pass to http_download_file
+        List of http links to files.
+    **kwargs
+        Optional arguments to pass to http_download_file.
 
     Returns
     -------
     list of pathlib.Path
         A list of the local full path of the downloaded files.
     """
     links_to_file_list = list(links_to_file_list)  # In case generator was passed
@@ -475,27 +475,27 @@
         Create a client instance that allows to GET and POST to the Alyx server.
         For One, constructor attempts to authenticate with credentials in params.py.
         For standalone cases, AlyxClient(username='', password='', base_url='').
 
         Parameters
         ----------
         base_url : str
-            Alyx server address, including port and protocol
+            Alyx server address, including port and protocol.
         username : str
-            Alyx database user
+            Alyx database user.
         password : str
-            Alyx database password
+            Alyx database password.
         cache_dir : str, pathlib.Path
-            The default root download location
+            The default root download location.
         silent : bool
-            If true, user prompts and progress bars are suppressed
+            If true, user prompts and progress bars are suppressed.
         cache_rest : str
-            Which type of http method to apply cache to; if '*', all requests are cached
+            Which type of http method to apply cache to; if '*', all requests are cached.
         stay_logged_in : bool
-            If true, auth token is cached
+            If true, auth token is cached.
         """
         self.silent = silent
         self._par = one.params.get(client=base_url, silent=self.silent, username=username)
         self.base_url = base_url or self._par.ALYX_URL
         self._par = self._par.set('CACHE_DIR', cache_dir or self._par.CACHE_DIR)
         if username or password:
             self.authenticate(username, password)
@@ -508,34 +508,34 @@
         # turned off.
         self.default_expiry = timedelta(days=1)
         self.cache_mode = cache_rest
         self._obj_id = id(self)
 
     @property
     def rest_schemes(self):
-        """dict: The REST endpoints and their parameters"""
+        """dict: The REST endpoints and their parameters."""
         # Delayed fetch of rest schemes speeds up instantiation
         if not self._rest_schemes:
             self._rest_schemes = self.get('/docs', expires=timedelta(weeks=1))
         return self._rest_schemes
 
     @property
     def cache_dir(self):
-        """pathlib.Path: The location of the downloaded file cache"""
+        """pathlib.Path: The location of the downloaded file cache."""
         return Path(self._par.CACHE_DIR)
 
     @cache_dir.setter
     def cache_dir(self, cache_dir):
         cache_dir = Path(cache_dir)
         cache_dir.mkdir(parents=True, exist_ok=True)
         self._par = self._par.set('CACHE_DIR', cache_dir)
 
     @property
     def is_logged_in(self):
-        """bool: Check if user logged into Alyx database; True if user is authenticated"""
+        """bool: Check if user logged into Alyx database; True if user is authenticated."""
         return bool(self.user and self._token and 'Authorization' in self._headers)
 
     def list_endpoints(self):
         """
         Return a list of available REST endpoints.
 
         Returns
@@ -719,43 +719,43 @@
         """
         Sends a DELETE request to the Alyx server. Will raise an exception on any status_code
         other than 200, 201.
 
         Parameters
         ----------
         rest_query : str
-            A REST query string either as a relative URL path complete URL
+            A REST query string either as a relative URL path complete URL.
 
         Returns
         -------
-        JSON interpreted dictionary from response
+        JSON interpreted dictionary from response.
 
         Examples
         --------
         >>> AlyxClient.delete('/weighings/c617562d-c107-432e-a8ee-682c17f9e698')
         >>> AlyxClient.delete(
         ...     'https://alyx.example.com/endpoint/c617562d-c107-432e-a8ee-682c17f9e698')
         """
         return self._generic_request(requests.delete, rest_query)
 
     def download_file(self, url, **kwargs):
         """
         Downloads a single file or list of files on the Alyx server from a
-        file record REST field URL
+        file record REST field URL.
 
         Parameters
         ----------
         url : str, list
-            Full url(s) of the file(s)
-        kwargs : Any
-            WebClient.http_download_file parameters
+            Full url(s) of the file(s).
+        **kwargs
+            WebClient.http_download_file parameters.
 
         Returns
         -------
-        Local path(s) of downloaded file(s)
+        Local path(s) of downloaded file(s).
         """
         if isinstance(url, str):
             url = self._validate_file_url(url)
             download_fcn = http_download_file
         else:
             url = (self._validate_file_url(x) for x in url)
             download_fcn = http_download_file_list
@@ -772,15 +772,15 @@
             if ex.code == 401:
                 ex.msg += (' - please check your HTTP_DATA_SERVER_LOGIN and '
                            'HTTP_DATA_SERVER_PWD ONE params, or username/password kwargs')
             raise ex
         return files
 
     def download_cache_tables(self, source=None, destination=None):
-        """Downloads the Alyx cache tables to the local data cache directory
+        """Downloads the Alyx cache tables to the local data cache directory.
 
         Parameters
         ----------
         source : str, pathlib.Path
             The remote HTTP directory of the cache table (excluding the filename).
             Default: AlyxClient.base_url.
         destination : str, pathlib.Path
@@ -813,19 +813,19 @@
         """Asserts that URL matches HTTP_DATA_SERVER parameter.
         Currently only one remote HTTP server is supported for a given AlyxClient instance.  If
         the URL contains only the relative path part, the full URL is returned.
 
         Parameters
         ----------
         url : str
-            The full or partial URL to validate
+            The full or partial URL to validate.
 
         Returns
         -------
-            The complete URL
+            The complete URL.
 
         Examples
         --------
         >>> url = self._validate_file_url('https://webserver.net/path/to/file')
         'https://webserver.net/path/to/file'
         >>> url = self._validate_file_url('path/to/file')
         'https://webserver.net/path/to/file'
@@ -841,19 +841,19 @@
     def rel_path2url(self, path):
         """Given a relative file path, return the remote HTTP server URL.
         It is expected that the remote HTTP server has the same file tree as the local system.
 
         Parameters
         ----------
         path : str, pathlib.Path
-            A relative ALF path (subject/date/number/etc.)
+            A relative ALF path (subject/date/number/etc.).
 
         Returns
         -------
-            A URL string
+            A URL string.
         """
         path = str(path).strip('/')
         assert not path.startswith('http')
         return f'{self._par.HTTP_DATA_SERVER}/{path}'
 
     def get(self, rest_query, **kwargs):
         """
@@ -861,21 +861,21 @@
         other than 200, 201.
         For the dictionary contents and list of endpoints, refer to:
         https://openalyx.internationalbrainlab.org/docs
 
         Parameters
         ----------
         rest_query : str
-            A REST URL path, e.g. '/sessions?user=Hamish'
-        kwargs : any
-            Optional arguments to pass to _generic_request and _cache_response decorator
+            A REST URL path, e.g. '/sessions?user=Hamish'.
+        **kwargs
+            Optional arguments to pass to _generic_request and _cache_response decorator.
 
         Returns
         -------
-        JSON interpreted dictionary from response
+        JSON interpreted dictionary from response.
         """
         rep = self._generic_request(requests.get, rest_query, **kwargs)
         if isinstance(rep, dict) and list(rep.keys()) == ['count', 'next', 'previous', 'results']:
             if len(rep['results']) < rep['count']:
                 cache_args = {k: v for k, v in kwargs.items() if k in ('clobber', 'expires')}
                 rep = _PaginatedResponse(self, rep, cache_args)
             else:
@@ -887,66 +887,66 @@
         Sends a PATCH request to the Alyx server.
         For the dictionary contents, refer to:
         https://openalyx.internationalbrainlab.org/docs
 
         Parameters
         ----------
         rest_query : str
-            The endpoint as full or relative URL
+            The endpoint as full or relative URL.
         data : dict, str
-            JSON encoded string or dictionary (c.f. requests)
+            JSON encoded string or dictionary (c.f. requests).
         files : dict, tuple
-            Files to attach (c.f. requests)
+            Files to attach (c.f. requests).
 
         Returns
         -------
-        Response object
+        Response object.
         """
         return self._generic_request(requests.patch, rest_query, data=data, files=files)
 
     def post(self, rest_query, data=None, files=None):
         """
         Sends a POST request to the Alyx server.
         For the dictionary contents, refer to:
         https://openalyx.internationalbrainlab.org/docs
 
         Parameters
         ----------
         rest_query : str
-            The endpoint as full or relative URL
+            The endpoint as full or relative URL.
         data : dict, str
-            JSON encoded string or dictionary (c.f. requests)
+            JSON encoded string or dictionary (c.f. requests).
         files : dict, tuple
-            Files to attach (c.f. requests)
+            Files to attach (c.f. requests).
 
         Returns
         -------
-        Response object
+        Response object.
         """
         return self._generic_request(requests.post, rest_query, data=data, files=files)
 
     def put(self, rest_query, data=None, files=None):
         """
         Sends a PUT request to the Alyx server.
         For the dictionary contents, refer to:
         https://openalyx.internationalbrainlab.org/docs
 
         Parameters
         ----------
         rest_query : str
-            The endpoint as full or relative URL
+            The endpoint as full or relative URL.
         data : dict, str
-            JSON encoded string or dictionary (c.f. requests)
+            JSON encoded string or dictionary (c.f. requests).
         files : dict, tuple
-            Files to attach (c.f. requests)
+            Files to attach (c.f. requests).
 
         Returns
         -------
         requests.Response
-            Response object
+            Response object.
         """
         return self._generic_request(requests.put, rest_query, data=data, files=files)
 
     def rest(self, url=None, action=None, id=None, data=None, files=None,
              no_cache=False, **kwargs):
         """
         alyx_client.rest(): lists endpoints
@@ -964,33 +964,33 @@
         >>> client.rest('subjects', 'partial_update', id='nickname', data=sub_dict)
         >>> client.rest('subjects', 'delete', id='nickname')
         >>> client.rest('notes', 'create', data=nd, files={'image': open(image_file, 'rb')})
 
         Parameters
         ----------
         url : str
-            Endpoint name
+            Endpoint name.
         action : str
-            One of 'list', 'create', 'read', 'update', 'partial_update', 'delete'
+            One of 'list', 'create', 'read', 'update', 'partial_update', 'delete'.
         id : str
-            Lookup string for actions 'read', 'update', 'partial_update', and 'delete'
+            Lookup string for actions 'read', 'update', 'partial_update', and 'delete'.
         data : dict
-            Data dictionary for actions 'update', 'partial_update' and 'create'
+            Data dictionary for actions 'update', 'partial_update' and 'create'.
         files : dict, tuple
-            Option file(s) to upload
+            Option file(s) to upload.
         no_cache : bool
-            If true the `list` and `read` actions are performed without returning the cache
-        kwargs
+            If true the `list` and `read` actions are performed without returning the cache.
+        **kwargs
             Filters as per the Alyx REST documentation
             cf. https://openalyx.internationalbrainlab.org/docs/
 
         Returns
         -------
         list, dict
-            List of queried dicts ('list') or dict (other actions)
+            List of queried dicts ('list') or dict (other actions).
         """
         # if endpoint is None, list available endpoints
         if not url:
             pprint(self.list_endpoints())
             return
         # remove beginning slash if any
         if url.startswith('/'):
@@ -1018,15 +1018,16 @@
                              '\n       ' + '\n       '.join(endpoint_scheme.keys()))
         # the actions below require an id in the URL, warn and help the user
         if action in ['read', 'update', 'partial_update', 'delete'] and not id:
             _logger.warning('REST action "' + action + '" requires an ID in the URL: ' +
                             endpoint_scheme[action]['url'])
             return
         # the actions below require a data dictionary, warn and help the user with fields list
-        if action in ['create', 'update', 'partial_update'] and not data:
+        data_required = 'fields' in endpoint_scheme[action]
+        if action in ['create', 'update', 'partial_update'] and data_required and not data:
             pprint(endpoint_scheme[action]['fields'])
             for act in endpoint_scheme[action]['fields']:
                 print("'" + act['name'] + "': ...,")
             _logger.warning('REST action "' + action + '" requires a data dict with above keys')
             return
 
         # clobber=True means remote request always made, expires=True means response is not cached
@@ -1085,26 +1086,26 @@
         """
         Write data to JSON field.  WILL NOT CHECK IF DATA EXISTS
         NOTE: Destructive write!
 
         Parameters
         ----------
         endpoint : str, None
-            Valid alyx endpoint, defaults to None
+            Valid alyx endpoint, defaults to None.
         uuid : str, uuid.UUID, None
-            UUID or lookup name for endpoint
+            UUID or lookup name for endpoint.
         field_name : str, None
-            Valid json field name, defaults to None
+            Valid json field name, defaults to None.
         data : dict, None
-            Data to write to json field, defaults to None
+            Data to write to json field, defaults to None.
 
         Returns
         -------
         dict
-            Written data dict
+            Written data dict.
         """
         self._check_inputs(endpoint)
         # Prepare data to patch
         patch_dict = {field_name: data}
         # Upload new extended_qc to session
         ret = self.rest(endpoint, "partial_update", id=uuid, data=patch_dict)
         return ret[field_name]
@@ -1113,34 +1114,35 @@
             self,
             endpoint: str = None,
             uuid: str = None,
             field_name: str = 'json',
             data: dict = None
     ) -> dict:
         """
-        Non-destructive update of JSON field of endpoint for object
+        Non-destructive update of JSON field of endpoint for object.
+
         Will update the field_name of the object with pk = uuid of given endpoint
         If data has keys with the same name of existing keys it will squash the old
         values (uses the dict.update() method).
 
         Parameters
         ----------
         endpoint : str
-            Alyx REST endpoint to hit
+            Alyx REST endpoint to hit.
         uuid : str, uuid.UUID
-            UUID or lookup name of object
+            UUID or lookup name of object.
         field_name : str
-            Name of the json field
+            Name of the json field.
         data : dict
-            A dictionary with fields to be updated
+            A dictionary with fields to be updated.
 
         Returns
         -------
         dict
-            New patched json field contents as dict
+            New patched json field contents as dict.
 
         Examples
         --------
         >>> client = AlyxClient()
         >>> client.json_field_update('sessions', 'eid_str', 'extended_qc', {'key': 'value'})
         """
         self._check_inputs(endpoint)
@@ -1168,31 +1170,32 @@
             endpoint: str = None,
             uuid: str = None,
             field_name: str = 'json',
             key: str = None
     ) -> Optional[dict]:
         """
         Remove inputted key from JSON field dict and re-upload it to Alyx.
-        Needs endpoint, uuid and json field name
+
+        Needs endpoint, UUID and json field name.
 
         Parameters
         ----------
         endpoint : str
-            Endpoint to hit, defaults to None
-        uuid : str
-            UUID or lookup name for endpoint
+            Endpoint to hit, defaults to None.
+        uuid : str, uuid.UUID
+            UUID or lookup name for endpoint.
         field_name : str
-            JSON field name of object, defaults to None
+            JSON field name of object, defaults to None.
         key : str
-            Key name of dictionary inside object, defaults to None
+            Key name of dictionary inside object, defaults to None.
 
         Returns
         -------
         dict
-            New content of json field
+            New content of json field.
         """
         self._check_inputs(endpoint)
         current = self.rest(endpoint, 'read', id=uuid)[field_name]
         # If no contents, cannot remove key, return
         if current is None:
             return current
         # if contents are not dict, cannot remove key, return contents
@@ -1212,15 +1215,35 @@
             endpoint=endpoint, uuid=uuid, field_name=field_name, data=current
         )
         return written
 
     def json_field_delete(
             self, endpoint: str = None, uuid: str = None, field_name: str = None
     ) -> None:
+        """
+        Set an entire field to null.
+
+        Note that this deletes all data from a given field. To delete only a single key from a
+        given JSON field, use `json_field_remove_key`.
+
+        Parameters
+        ----------
+        endpoint : str
+            Endpoint to hit, defaults to None.
+        uuid : str, uuid.UUID
+            UUID or lookup name for endpoint.
+        field_name : str
+            The field name of object (e.g. 'json', 'name', 'extended_qc'), defaults to None.
+
+        Returns
+        -------
+        None
+            New content of json field.
+        """
         self._check_inputs(endpoint)
         _ = self.rest(endpoint, 'partial_update', id=uuid, data={field_name: None})
         return _[field_name]
 
     def clear_rest_cache(self):
-        """Clear all REST response cache files for the base url"""
+        """Clear all REST response cache files for the base url."""
         for file in self.cache_dir.joinpath('.rest').glob('*'):
             file.unlink()
```

### Comparing `ONE-api-2.1.0/setup.py` & `ONE-api-2.2.0/setup.py`

 * *Files identical despite different names*

