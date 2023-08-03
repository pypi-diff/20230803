# Comparing `tmp/w3lib-2.1.1.tar.gz` & `tmp/w3lib-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3lib-2.1.1.tar", last modified: Fri Dec  9 11:09:23 2022, max compression
+gzip compressed data, was "w3lib-2.1.2.tar", last modified: Thu Aug  3 08:48:07 2023, max compression
```

## Comparing `w3lib-2.1.1.tar` & `w3lib-2.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:09:23.963288 w3lib-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2022-12-09 11:09:15.000000 w3lib-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      263 2022-12-09 11:09:15.000000 w3lib-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2022-12-09 11:09:15.000000 w3lib-2.1.1/NEWS
--rw-r--r--   0 runner    (1001) docker     (123)      939 2022-12-09 11:09:23.963288 w3lib-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      914 2022-12-09 11:09:15.000000 w3lib-2.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:09:23.959288 w3lib-2.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2022-12-09 11:09:15.000000 w3lib-2.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2022-12-09 11:09:15.000000 w3lib-2.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2022-12-09 11:09:15.000000 w3lib-2.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2022-12-09 11:09:15.000000 w3lib-2.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-09 11:09:15.000000 w3lib-2.1.1/docs/w3lib.rst
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-09 11:09:15.000000 w3lib-2.1.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-09 11:09:23.963288 w3lib-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2022-12-09 11:09:15.000000 w3lib-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:09:23.959288 w3lib-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 11:09:15.000000 w3lib-2.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12625 2022-12-09 11:09:15.000000 w3lib-2.1.1/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    24952 2022-12-09 11:09:15.000000 w3lib-2.1.1/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2022-12-09 11:09:15.000000 w3lib-2.1.1/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)    64003 2022-12-09 11:09:15.000000 w3lib-2.1.1/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2022-12-09 11:09:15.000000 w3lib-2.1.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2022-12-09 11:09:15.000000 w3lib-2.1.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:09:23.963288 w3lib-2.1.1/w3lib/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-09 11:09:15.000000 w3lib-2.1.1/w3lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-09 11:09:15.000000 w3lib-2.1.1/w3lib/_infra.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2022-12-09 11:09:15.000000 w3lib-2.1.1/w3lib/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2022-12-09 11:09:15.000000 w3lib-2.1.1/w3lib/_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    10426 2022-12-09 11:09:15.000000 w3lib-2.1.1/w3lib/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2022-12-09 11:09:15.000000 w3lib-2.1.1/w3lib/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2022-12-09 11:09:15.000000 w3lib-2.1.1/w3lib/http.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 11:09:15.000000 w3lib-2.1.1/w3lib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23930 2022-12-09 11:09:15.000000 w3lib-2.1.1/w3lib/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2022-12-09 11:09:15.000000 w3lib-2.1.1/w3lib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 11:09:23.963288 w3lib-2.1.1/w3lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2022-12-09 11:09:23.000000 w3lib-2.1.1/w3lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2022-12-09 11:09:23.000000 w3lib-2.1.1/w3lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 11:09:23.000000 w3lib-2.1.1/w3lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 11:09:23.000000 w3lib-2.1.1/w3lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-09 11:09:23.000000 w3lib-2.1.1/w3lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:07.089920 w3lib-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-03 08:47:51.000000 w3lib-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-03 08:47:51.000000 w3lib-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-08-03 08:47:51.000000 w3lib-2.1.2/NEWS
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 08:48:07.089920 w3lib-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-03 08:47:51.000000 w3lib-2.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:07.085919 w3lib-2.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-08-03 08:47:51.000000 w3lib-2.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-08-03 08:47:51.000000 w3lib-2.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-03 08:47:51.000000 w3lib-2.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-08-03 08:47:51.000000 w3lib-2.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-03 08:47:51.000000 w3lib-2.1.2/docs/w3lib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-03 08:47:51.000000 w3lib-2.1.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:48:07.089920 w3lib-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-03 08:47:51.000000 w3lib-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:07.089920 w3lib-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:47:51.000000 w3lib-2.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-08-03 08:47:51.000000 w3lib-2.1.2/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24952 2023-08-03 08:47:51.000000 w3lib-2.1.2/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-08-03 08:47:51.000000 w3lib-2.1.2/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64087 2023-08-03 08:47:51.000000 w3lib-2.1.2/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-03 08:47:51.000000 w3lib-2.1.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-03 08:47:51.000000 w3lib-2.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:07.089920 w3lib-2.1.2/w3lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-03 08:47:51.000000 w3lib-2.1.2/w3lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-03 08:47:51.000000 w3lib-2.1.2/w3lib/_infra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-03 08:47:51.000000 w3lib-2.1.2/w3lib/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-03 08:47:51.000000 w3lib-2.1.2/w3lib/_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-08-03 08:47:51.000000 w3lib-2.1.2/w3lib/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-08-03 08:47:51.000000 w3lib-2.1.2/w3lib/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-08-03 08:47:51.000000 w3lib-2.1.2/w3lib/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:47:51.000000 w3lib-2.1.2/w3lib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23930 2023-08-03 08:47:51.000000 w3lib-2.1.2/w3lib/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-03 08:47:51.000000 w3lib-2.1.2/w3lib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:48:07.089920 w3lib-2.1.2/w3lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 08:48:07.000000 w3lib-2.1.2/w3lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-03 08:48:07.000000 w3lib-2.1.2/w3lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:48:07.000000 w3lib-2.1.2/w3lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:48:07.000000 w3lib-2.1.2/w3lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 08:48:07.000000 w3lib-2.1.2/w3lib.egg-info/top_level.txt
```

### Comparing `w3lib-2.1.1/LICENSE` & `w3lib-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `w3lib-2.1.1/NEWS` & `w3lib-2.1.2/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 w3lib release notes
 ===================
 
+2.1.2 (2023-08-03)
+------------------
+
+- Fix test failures on Python 3.11.4+ (#212, #213).
+- Fix an incorrect type hint (#211).
+- Add project URLs to setup.py (#215).
+
 2.1.1 (2022-12-09)
 ------------------
 
 - :func:`~w3lib.url.safe_url_string`, :func:`~w3lib.url.safe_download_url`
   and :func:`~w3lib.url.canonicalize_url` now strip whitespace and control
   characters urls according to the URL living standard.
```

### Comparing `w3lib-2.1.1/PKG-INFO` & `w3lib-2.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: w3lib
-Version: 2.1.1
+Version: 2.1.2
 Summary: Library of web-related functions
 Home-page: https://github.com/scrapy/w3lib
 Author: Scrapy project
 Author-email: info@scrapy.org
 License: BSD
+Project-URL: Documentation, https://w3lib.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/scrapy/w3lib
+Project-URL: Issue Tracker, https://github.com/scrapy/w3lib/issues
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `w3lib-2.1.1/README.rst` & `w3lib-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `w3lib-2.1.1/docs/Makefile` & `w3lib-2.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `w3lib-2.1.1/docs/conf.py` & `w3lib-2.1.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 copyright = '2014, w3lib developers'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = '2.1.1'
+release = '2.1.2'
 # The short X.Y version.
 version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
```

### Comparing `w3lib-2.1.1/docs/index.rst` & `w3lib-2.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `w3lib-2.1.1/docs/make.bat` & `w3lib-2.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `w3lib-2.1.1/setup.py` & `w3lib-2.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="w3lib",
-    version="2.1.1",
+    version="2.1.2",
     license="BSD",
     description="Library of web-related functions",
     author="Scrapy project",
     author_email="info@scrapy.org",
     url="https://github.com/scrapy/w3lib",
+    project_urls={
+        "Documentation": "https://w3lib.readthedocs.io/en/latest/",
+        "Source Code": "https://github.com/scrapy/w3lib",
+        "Issue Tracker": "https://github.com/scrapy/w3lib/issues",
+    },
     packages=find_packages(exclude=("tests", "tests.*")),
     package_data={
         "w3lib": ["py.typed"],
     },
     include_package_data=True,
     zip_safe=False,
     platforms=["Any"],
```

### Comparing `w3lib-2.1.1/tests/test_encoding.py` & `w3lib-2.1.2/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `w3lib-2.1.1/tests/test_html.py` & `w3lib-2.1.2/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `w3lib-2.1.1/tests/test_http.py` & `w3lib-2.1.2/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `w3lib-2.1.1/tests/test_url.py` & `w3lib-2.1.2/tests/test_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import os
 import unittest
 from inspect import isclass
 from typing import Optional, Union, Type, Callable, Tuple, List
 from urllib.parse import urlparse
 
 import pytest
@@ -98,15 +99,15 @@
 USERINFO_SAFE = _ASCII_ALPHANUMERIC + "-_.!~*'()" + "&+$,"
 USERNAME_TO_ENCODE = "".join(
     chr(value)
     for value in range(0x80)
     if (
         chr(value) not in _C0_CONTROL_OR_SPACE
         and chr(value) not in USERINFO_SAFE
-        and chr(value) not in ":/?#\\"
+        and chr(value) not in ":/?#\\[]"
     )
 )
 USERNAME_ENCODED = "".join(f"%{ord(char):02X}" for char in USERNAME_TO_ENCODE)
 PASSWORD_TO_ENCODE = USERNAME_TO_ENCODE + ":"
 PASSWORD_ENCODED = "".join(f"%{ord(char):02X}" for char in PASSWORD_TO_ENCODE)
 
 # Path characters that do not need escaping.
@@ -382,15 +383,14 @@
     # are not escaped.
     "https://@\\example.com",  # Invalid URL
     "https://\x80.example",  # Invalid domain name (non-visible character)
     "https://%80.example",  # Invalid domain name (non-visible character)
     "http://192.168.0.256",  # Invalid IP address
     "http://192.168.0.0.0",  # Invalid IP address / domain name
     "http://[2a01:5cc0:1:2::4]",  # https://github.com/scrapy/w3lib/issues/193
-    "http://[2a01:5cc0:1:2:3:4]",  # Invalid IPv6
     "https://example.com:",  # Removes the :
     # Does not convert \ to /
     "https://example.com\\a",
     "https://example.com\\a\\b",
     # Encodes \ and / after the first one in the path
     "https://example.com/a/b",
     "https://example.com/a\\b",
@@ -414,14 +414,16 @@
     "https://example.com/#",
     "https://example.com?#",
     "https://example.com/?#",
     # Some fragment characters that RFC 2396 and RFC 3986 require escaping
     # (%) are not escaped.
     f"a://example.com#{FRAGMENT_TO_ENCODE}",
 }
+if sys.version_info < (3, 11, 4):
+    KNOWN_SAFE_URL_STRING_URL_ISSUES.add("http://[2a01:5cc0:1:2:3:4]")  # Invalid IPv6
 
 
 @pytest.mark.parametrize(
     "url,output",
     tuple(
         case
         if case[0] not in KNOWN_SAFE_URL_STRING_URL_ISSUES
```

### Comparing `w3lib-2.1.1/tests/test_util.py` & `w3lib-2.1.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `w3lib-2.1.1/tox.ini` & `w3lib-2.1.2/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     bandit -r -c .bandit.yml {posargs:w3lib}
 
 [testenv:typing]
 basepython = python3
 deps =
     # mypy would error if pytest (or its sub) not found
     pytest
-    mypy==0.991
+    mypy==1.0.0
 commands =
-    mypy --strict --show-error-codes {posargs: w3lib tests}
+    mypy --strict {posargs: w3lib tests}
 
 [testenv:flake8]
 basepython = python3
 deps =
     flake8
 commands =
     flake8 \
```

### Comparing `w3lib-2.1.1/w3lib/encoding.py` & `w3lib-2.1.2/w3lib/encoding.py`

 * *Files identical despite different names*

### Comparing `w3lib-2.1.1/w3lib/html.py` & `w3lib-2.1.2/w3lib/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,16 +324,16 @@
 
 
 def get_meta_refresh(
     text: AnyStr,
     baseurl: str = "",
     encoding: str = "utf-8",
     ignore_tags: Iterable[str] = ("script", "noscript"),
-) -> Tuple[Optional[float], Optional[str]]:
-    """Return  the http-equiv parameter of the HTML meta element from the given
+) -> Union[Tuple[None, None], Tuple[float, str]]:
+    """Return the http-equiv parameter of the HTML meta element from the given
     HTML text and return a tuple ``(interval, url)`` where interval is an integer
     containing the delay in seconds (or zero if not present) and url is a
     string with the absolute url to redirect.
 
     If no meta redirect is found, ``(None, None)`` is returned.
 
     """
```

### Comparing `w3lib-2.1.1/w3lib/http.py` & `w3lib-2.1.2/w3lib/http.py`

 * *Files identical despite different names*

### Comparing `w3lib-2.1.1/w3lib/url.py` & `w3lib-2.1.2/w3lib/url.py`

 * *Files identical despite different names*

### Comparing `w3lib-2.1.1/w3lib/util.py` & `w3lib-2.1.2/w3lib/util.py`

 * *Files identical despite different names*

### Comparing `w3lib-2.1.1/w3lib.egg-info/PKG-INFO` & `w3lib-2.1.2/w3lib.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: w3lib
-Version: 2.1.1
+Version: 2.1.2
 Summary: Library of web-related functions
 Home-page: https://github.com/scrapy/w3lib
 Author: Scrapy project
 Author-email: info@scrapy.org
 License: BSD
+Project-URL: Documentation, https://w3lib.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/scrapy/w3lib
+Project-URL: Issue Tracker, https://github.com/scrapy/w3lib/issues
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `w3lib-2.1.1/w3lib.egg-info/SOURCES.txt` & `w3lib-2.1.2/w3lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

