# Comparing `tmp/urlfetch-2.0.0.tar.gz` & `tmp/urlfetch-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/urlfetch-2.0.0.tar", last modified: Sat Jul 29 15:41:01 2023, max compression
+gzip compressed data, was "dist/urlfetch-2.0.1.tar", last modified: Thu Aug  3 16:35:56 2023, max compression
```

## Comparing `urlfetch-2.0.0.tar` & `urlfetch-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 duyue      (501) staff       (20)        0 2023-07-29 15:41:01.599151 urlfetch-2.0.0/
--rw-r--r--   0 duyue      (501) staff       (20)     1313 2020-04-29 08:16:55.000000 urlfetch-2.0.0/LICENSE
--rw-r--r--   0 duyue      (501) staff       (20)       68 2013-11-09 02:41:08.000000 urlfetch-2.0.0/MANIFEST.in
--rw-r--r--   0 duyue      (501) staff       (20)     3802 2023-07-29 15:41:01.599362 urlfetch-2.0.0/PKG-INFO
--rw-r--r--   0 duyue      (501) staff       (20)     2255 2023-07-29 15:10:56.000000 urlfetch-2.0.0/README.rst
--rw-r--r--   0 duyue      (501) staff       (20)       97 2023-07-29 15:41:01.599961 urlfetch-2.0.0/setup.cfg
--rw-r--r--   0 duyue      (501) staff       (20)     1176 2023-07-29 15:26:47.000000 urlfetch-2.0.0/setup.py
-drwxr-xr-x   0 duyue      (501) staff       (20)        0 2023-07-29 15:41:01.598774 urlfetch-2.0.0/urlfetch.egg-info/
--rw-r--r--   0 duyue      (501) staff       (20)     3802 2023-07-29 15:41:01.000000 urlfetch-2.0.0/urlfetch.egg-info/PKG-INFO
--rw-r--r--   0 duyue      (501) staff       (20)      214 2023-07-29 15:41:01.000000 urlfetch-2.0.0/urlfetch.egg-info/SOURCES.txt
--rw-r--r--   0 duyue      (501) staff       (20)        1 2023-07-29 15:41:01.000000 urlfetch-2.0.0/urlfetch.egg-info/dependency_links.txt
--rw-r--r--   0 duyue      (501) staff       (20)        9 2023-07-29 15:41:01.000000 urlfetch-2.0.0/urlfetch.egg-info/top_level.txt
--rw-r--r--   0 duyue      (501) staff       (20)    34668 2023-07-29 15:32:59.000000 urlfetch-2.0.0/urlfetch.py
--rw-r--r--   0 duyue      (501) staff       (20)   587726 2019-10-11 04:58:26.000000 urlfetch-2.0.0/urlfetch.useragents.list
+drwxr-xr-x   0 duyue      (501) staff       (20)        0 2023-08-03 16:35:56.256994 urlfetch-2.0.1/
+-rw-r--r--   0 duyue      (501) staff       (20)     1313 2020-04-29 08:16:55.000000 urlfetch-2.0.1/LICENSE
+-rw-r--r--   0 duyue      (501) staff       (20)       68 2013-11-09 02:41:08.000000 urlfetch-2.0.1/MANIFEST.in
+-rw-r--r--   0 duyue      (501) staff       (20)     3825 2023-08-03 16:35:56.257248 urlfetch-2.0.1/PKG-INFO
+-rw-r--r--   0 duyue      (501) staff       (20)     2255 2023-07-29 15:10:56.000000 urlfetch-2.0.1/README.rst
+-rw-r--r--   0 duyue      (501) staff       (20)       97 2023-08-03 16:35:56.257962 urlfetch-2.0.1/setup.cfg
+-rw-r--r--   0 duyue      (501) staff       (20)     1205 2023-07-31 13:26:04.000000 urlfetch-2.0.1/setup.py
+drwxr-xr-x   0 duyue      (501) staff       (20)        0 2023-08-03 16:35:56.256450 urlfetch-2.0.1/urlfetch.egg-info/
+-rw-r--r--   0 duyue      (501) staff       (20)     3825 2023-08-03 16:35:56.000000 urlfetch-2.0.1/urlfetch.egg-info/PKG-INFO
+-rw-r--r--   0 duyue      (501) staff       (20)      214 2023-08-03 16:35:56.000000 urlfetch-2.0.1/urlfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 duyue      (501) staff       (20)        1 2023-08-03 16:35:56.000000 urlfetch-2.0.1/urlfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 duyue      (501) staff       (20)        9 2023-08-03 16:35:56.000000 urlfetch-2.0.1/urlfetch.egg-info/top_level.txt
+-rw-r--r--   0 duyue      (501) staff       (20)    34680 2023-08-03 16:32:36.000000 urlfetch-2.0.1/urlfetch.py
+-rw-r--r--   0 duyue      (501) staff       (20)   587726 2019-10-11 04:58:26.000000 urlfetch-2.0.1/urlfetch.useragents.list
```

### Comparing `urlfetch-2.0.0/LICENSE` & `urlfetch-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `urlfetch-2.0.0/PKG-INFO` & `urlfetch-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: urlfetch
-Version: 2.0.0
+Version: 2.0.1
 Summary: An easy to use HTTP client
 Home-page: https://github.com/ifduyue/urlfetch
 Author: Yue Du
 Author-email: ifduyue@gmail.com
 License: BSD
 Description: urlfetch |github-actions-badge| |furyio-badge|
         ==========================================================
@@ -99,7 +99,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.5
```

### Comparing `urlfetch-2.0.0/README.rst` & `urlfetch-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `urlfetch-2.0.0/setup.py` & `urlfetch-2.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     url=urlfetch.__url__,
     description="An easy to use HTTP client",
     long_description=open('README.rst').read(),
     license="BSD",
     keywords="httpclient urlfetch",
     py_modules=['urlfetch'],
     data_files=[('', ['urlfetch.useragents.list'])],
+    python_requires=">=3.5",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `urlfetch-2.0.0/urlfetch.egg-info/PKG-INFO` & `urlfetch-2.0.1/urlfetch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: urlfetch
-Version: 2.0.0
+Version: 2.0.1
 Summary: An easy to use HTTP client
 Home-page: https://github.com/ifduyue/urlfetch
 Author: Yue Du
 Author-email: ifduyue@gmail.com
 License: BSD
 Description: urlfetch |github-actions-badge| |furyio-badge|
         ==========================================================
@@ -99,7 +99,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.5
```

### Comparing `urlfetch-2.0.0/urlfetch.py` & `urlfetch-2.0.1/urlfetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 
 An easy to use HTTP client based on httplib.
 
 :copyright: (c) 2011-2020 by Yue Du.
 :license: BSD 2-clause License, see LICENSE for more details.
 """
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __author__ = "Yue Du <ifduyue@gmail.com>"
 __url__ = "https://github.com/ifduyue/urlfetch"
 __license__ = "BSD 2-Clause License"
 
+import zlib
 import os, sys, base64, codecs, uuid, stat, time, socket
 import ssl
 from os.path import basename, dirname, abspath, join as pathjoin
 from functools import partial
 from io import BytesIO
 import re
 
 try:
     import simplejson as json
 except ImportError:
     import json
 
 from http.client import HTTPConnection, HTTPSConnection
-from urllib.parse import urlencode
-import urllib.parse as urlparse
+from urllib.parse import parse_qs, urlencode, urlsplit, urljoin
 import http.cookies as Cookie
 
 basestring = (str, bytes)
 unicode = str
 b = lambda s: s.encode("latin-1")
 u = lambda s: s
 
@@ -220,15 +220,15 @@
         self.getheader = r.getheader
         self.getheaders = r.getheaders
 
         self._content_encoding = self.getheader("content-encoding", None)
         self._decoder = None
 
         try:
-            self.length_limit = int(kwargs.get("length_limit"))
+            self.length_limit = int(kwargs.get("length_limit", 0)) or None
         except:
             self.length_limit = None
 
         # if content (length) size is more than length_limit, skip
         content_length = int(self.getheader("Content-Length", 0))
         if self.length_limit and content_length > self.length_limit:
             self.close()
@@ -255,16 +255,14 @@
                 return chunk
             else:
                 raise StopIteration
         else:
             ce = self._content_encoding
             if ce in ("gzip", "deflate"):
                 if not self._decoder:
-                    import zlib
-
                     if ce == "gzip":
                         self._decoder = zlib.decompressobj(16 + zlib.MAX_WBITS)
                     else:
                         self._decoder = zlib.decompressobj()
                         try:
                             return self._decoder.decompress(chunk)
                         except zlib.error:
@@ -663,14 +661,16 @@
         "Host": parsed_url["http_host"],
     }
 
     # Proxy support
     scheme = parsed_url["scheme"]
     if proxies is None and trust_env:
         proxies = PROXIES
+    if not proxies:
+        proxies = {}
 
     ignore_hosts = PROXY_IGNORE_HOSTS
     if trust_env:
         no_proxy = os.getenv("no_proxy") or os.getenv("NO_PROXY")
         if no_proxy:
             ignore_hosts = no_proxy.split(",")
 
@@ -751,15 +751,15 @@
             raise TooManyRedirects("max_redirects exceeded")
 
         method = method if response.status == 307 else "GET"
         location = response.headers["location"]
         if location[:2] == "//":
             url = parsed_url["scheme"] + ":" + location
         else:
-            url = urlparse.urljoin(url, location)
+            url = urljoin(url, location)
         parsed_url = parse_url(url)
 
         reqheaders["Host"] = parsed_url["http_host"]
         reqheaders["Referer"] = response.url
 
         # Proxy
         scheme = parsed_url["scheme"]
@@ -863,15 +863,15 @@
         pass
 
     if "://" in url:
         scheme, url = url.split("://", 1)
     else:
         scheme = "http"
     url = "http://" + url
-    parsed = urlparse.urlsplit(url)
+    parsed = urlsplit(url)
     r = ObjectDict()
     r["scheme"] = scheme
     r["netloc"] = parsed.netloc
     r["path"] = parsed.path
     r["query"] = parsed.query
     r["fragment"] = parsed.fragment
     r["uri"] = parsed.path
@@ -990,20 +990,20 @@
     """
     if not args:
         return url
 
     if keep_existing:
         if url[-1] not in ("?", "&"):
             url += "&" if ("?" in url) else "?"
-        return url + urlencode(args, 1)
+        return url + urlencode(args, True)
     else:
         url, seq, query = url.partition("?")
-        query = urlparse.parse_qs(query, True)
+        query = parse_qs(query, True)
         query.update(args)
-        return url + "?" + urlencode(query, 1)
+        return url + "?" + urlencode(query, True)
 
 
 def choose_boundary():
     """Generate a multipart boundry.
 
     :returns: A boundary string
     """
@@ -1077,15 +1077,15 @@
             writer(body).write(
                 'Content-Disposition: form-data; name="%s"; '
                 'filename="%s"\r\n' % (fieldname, filename)
             )
             body.write(b"Content-Type: application/octet-stream\r\n\r\n")
         else:
             writer(body).write(
-                'Content-Disposition: form-data; name="%s"' "\r\n" % name
+                'Content-Disposition: form-data; name="%s"' "\r\n" % fieldname
             )
             body.write(b"Content-Type: text/plain\r\n\r\n")
 
         if isinstance(value, str):
             writer(body).write(value)
         else:
             body.write(value)
```

### Comparing `urlfetch-2.0.0/urlfetch.useragents.list` & `urlfetch-2.0.1/urlfetch.useragents.list`

 * *Files identical despite different names*

