# Comparing `tmp/ripemd-hash-1.0.0.tar.gz` & `tmp/ripemd-hash-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ripemd-hash-1.0.0.tar", last modified: Fri Aug 26 12:13:09 2022, max compression
+gzip compressed data, was "ripemd-hash-1.0.1.tar", last modified: Thu Aug  3 10:53:31 2023, max compression
```

## Comparing `ripemd-hash-1.0.0.tar` & `ripemd-hash-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 12:13:10.082359 ripemd-hash-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     2926 2022-08-25 18:40:23.000000 ripemd-hash-1.0.0/LICENSE.rst
--rw-r--r--   0 root         (0) root         (0)       16 2022-08-26 11:49:11.000000 ripemd-hash-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1749 2022-08-26 12:13:10.079806 ripemd-hash-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      612 2022-08-25 18:43:25.000000 ripemd-hash-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 12:13:09.871352 ripemd-hash-1.0.0/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 12:13:09.948891 ripemd-hash-1.0.0/lib/ripemd/
--rw-r--r--   0 root         (0) root         (0)      108 2022-08-25 15:04:51.000000 ripemd-hash-1.0.0/lib/ripemd/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10439 2022-08-25 15:04:42.000000 ripemd-hash-1.0.0/lib/ripemd/_raw_api.py
--rw-r--r--   0 root         (0) root         (0)     6210 2022-08-25 15:10:22.000000 ripemd-hash-1.0.0/lib/ripemd/ripemd160.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 12:13:10.021922 ripemd-hash-1.0.0/lib/ripemd_hash.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1749 2022-08-26 12:13:09.000000 ripemd-hash-1.0.0/lib/ripemd_hash.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      364 2022-08-26 12:13:09.000000 ripemd-hash-1.0.0/lib/ripemd_hash.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 12:13:09.000000 ripemd-hash-1.0.0/lib/ripemd_hash.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 11:43:42.000000 ripemd-hash-1.0.0/lib/ripemd_hash.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        7 2022-08-26 12:13:09.000000 ripemd-hash-1.0.0/lib/ripemd_hash.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-26 12:13:10.082869 ripemd-hash-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    11727 2022-08-26 11:51:56.000000 ripemd-hash-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 12:13:10.067251 ripemd-hash-1.0.0/src/
--rw-r--r--   0 root         (0) root         (0)     4864 2022-08-25 14:26:31.000000 ripemd-hash-1.0.0/src/common.h
--rw-r--r--   0 root         (0) root         (0)     7524 2022-08-25 14:28:15.000000 ripemd-hash-1.0.0/src/endianess.h
--rw-r--r--   0 root         (0) root         (0)      712 2022-08-25 14:27:30.000000 ripemd-hash-1.0.0/src/errors.h
--rw-r--r--   0 root         (0) root         (0)    11887 2022-08-25 14:25:43.000000 ripemd-hash-1.0.0/src/ripemd160.c
+drwxrwxrwx   0        0        0        0 2023-08-03 10:53:31.908273 ripemd-hash-1.0.1/
+-rw-rw-rw-   0        0        0     2926 2022-08-25 18:40:23.000000 ripemd-hash-1.0.1/LICENSE.rst
+-rw-rw-rw-   0        0        0       16 2022-08-26 11:49:11.000000 ripemd-hash-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1769 2023-08-03 10:53:31.908273 ripemd-hash-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2022-08-25 18:43:25.000000 ripemd-hash-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 10:53:31.893273 ripemd-hash-1.0.1/lib/
+drwxrwxrwx   0        0        0        0 2023-08-03 10:53:31.899273 ripemd-hash-1.0.1/lib/ripemd/
+-rw-rw-rw-   0        0        0      108 2023-08-02 11:01:08.000000 ripemd-hash-1.0.1/lib/ripemd/__init__.py
+-rw-rw-rw-   0        0        0    10439 2022-08-25 15:04:42.000000 ripemd-hash-1.0.1/lib/ripemd/_raw_api.py
+-rw-rw-rw-   0        0        0     6210 2022-08-25 15:10:22.000000 ripemd-hash-1.0.1/lib/ripemd/ripemd160.py
+drwxrwxrwx   0        0        0        0 2023-08-03 10:53:31.904273 ripemd-hash-1.0.1/lib/ripemd_hash.egg-info/
+-rw-rw-rw-   0        0        0     1769 2023-08-03 10:53:31.000000 ripemd-hash-1.0.1/lib/ripemd_hash.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-08-03 10:53:31.000000 ripemd-hash-1.0.1/lib/ripemd_hash.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 10:53:31.000000 ripemd-hash-1.0.1/lib/ripemd_hash.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2022-08-26 11:43:42.000000 ripemd-hash-1.0.1/lib/ripemd_hash.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-08-03 10:53:31.000000 ripemd-hash-1.0.1/lib/ripemd_hash.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 10:53:31.909273 ripemd-hash-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0    11557 2023-08-03 10:46:10.000000 ripemd-hash-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 10:53:31.907273 ripemd-hash-1.0.1/src/
+-rw-rw-rw-   0        0        0     4864 2023-08-03 10:40:36.000000 ripemd-hash-1.0.1/src/common.h
+-rw-rw-rw-   0        0        0     7524 2022-08-25 14:28:15.000000 ripemd-hash-1.0.1/src/endianess.h
+-rw-rw-rw-   0        0        0      712 2022-08-25 14:27:30.000000 ripemd-hash-1.0.1/src/errors.h
+-rw-rw-rw-   0        0        0    11887 2023-08-03 10:40:50.000000 ripemd-hash-1.0.1/src/ripemd160.c
```

### Comparing `ripemd-hash-1.0.0/LICENSE.rst` & `ripemd-hash-1.0.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ripemd-hash-1.0.0/PKG-INFO` & `ripemd-hash-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,47 @@
-Metadata-Version: 2.1
-Name: ripemd-hash
-Version: 1.0.0
-Summary: Ripemd library for Python
-Home-page: https://github.com/symbol/ripemd
-Author: Symbol Contributors
-Author-email: contributors@symbol.dev
-License: BSD, Public Domain
-Platform: Posix; MacOS X; Windows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: License :: Public Domain
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Topic :: Security :: Cryptography
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
-Ripemd
-======
-
-Given headache openssl devs gave to everyone, this is tiny ripemd module for python 3. Shamelessly ~~stolen~~ extracted from [pycryptodome](https://github.com/Legrandin/pycryptodome).
-
-### Usage
-
-Single call:
-```py
-from ripemd.ripemd160 import ripemd160  # import function
-
-ripemd160(b'abc').hex() == '8eb208f7e05d987a9b044a8e98c6b087f15a0bfc'
-ripemd160(b'a' * 1000000).hex() == '52783243c1697bdbe16d37f97f68f08325dc1528'
-```
-
-Update mode:
-```py
-from ripemd import ripemd160  # import module
-
-h = ripemd160.new()
-h.update(b'abc')
-h.digest().hex() == '8eb208f7e05d987a9b044a8e98c6b087f15a0bfc'
-```
+Metadata-Version: 2.1
+Name: ripemd-hash
+Version: 1.0.1
+Summary: Ripemd library for Python
+Home-page: https://github.com/symbol/ripemd
+Author: Symbol Contributors
+Author-email: contributors@symbol.dev
+License: BSD, Public Domain
+Description: Ripemd
+        ======
+        
+        Given headache openssl devs gave to everyone, this is tiny ripemd module for python 3. Shamelessly ~~stolen~~ extracted from [pycryptodome](https://github.com/Legrandin/pycryptodome).
+        
+        ### Usage
+        
+        Single call:
+        ```py
+        from ripemd.ripemd160 import ripemd160  # import function
+        
+        ripemd160(b'abc').hex() == '8eb208f7e05d987a9b044a8e98c6b087f15a0bfc'
+        ripemd160(b'a' * 1000000).hex() == '52783243c1697bdbe16d37f97f68f08325dc1528'
+        ```
+        
+        Update mode:
+        ```py
+        from ripemd import ripemd160  # import module
+        
+        h = ripemd160.new()
+        h.update(b'abc')
+        h.digest().hex() == '8eb208f7e05d987a9b044a8e98c6b087f15a0bfc'
+        ```
+        
+Platform: Posix; MacOS X; Windows
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Public Domain
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Topic :: Security :: Cryptography
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
```

### Comparing `ripemd-hash-1.0.0/README.md` & `ripemd-hash-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ripemd-hash-1.0.0/lib/ripemd/_raw_api.py` & `ripemd-hash-1.0.1/lib/ripemd/_raw_api.py`

 * *Files identical despite different names*

### Comparing `ripemd-hash-1.0.0/lib/ripemd/ripemd160.py` & `ripemd-hash-1.0.1/lib/ripemd/ripemd160.py`

 * *Files identical despite different names*

### Comparing `ripemd-hash-1.0.0/lib/ripemd_hash.egg-info/PKG-INFO` & `ripemd-hash-1.0.1/lib/ripemd_hash.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,47 @@
-Metadata-Version: 2.1
-Name: ripemd-hash
-Version: 1.0.0
-Summary: Ripemd library for Python
-Home-page: https://github.com/symbol/ripemd
-Author: Symbol Contributors
-Author-email: contributors@symbol.dev
-License: BSD, Public Domain
-Platform: Posix; MacOS X; Windows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: License :: Public Domain
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Topic :: Security :: Cryptography
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
-Ripemd
-======
-
-Given headache openssl devs gave to everyone, this is tiny ripemd module for python 3. Shamelessly ~~stolen~~ extracted from [pycryptodome](https://github.com/Legrandin/pycryptodome).
-
-### Usage
-
-Single call:
-```py
-from ripemd.ripemd160 import ripemd160  # import function
-
-ripemd160(b'abc').hex() == '8eb208f7e05d987a9b044a8e98c6b087f15a0bfc'
-ripemd160(b'a' * 1000000).hex() == '52783243c1697bdbe16d37f97f68f08325dc1528'
-```
-
-Update mode:
-```py
-from ripemd import ripemd160  # import module
-
-h = ripemd160.new()
-h.update(b'abc')
-h.digest().hex() == '8eb208f7e05d987a9b044a8e98c6b087f15a0bfc'
-```
+Metadata-Version: 2.1
+Name: ripemd-hash
+Version: 1.0.1
+Summary: Ripemd library for Python
+Home-page: https://github.com/symbol/ripemd
+Author: Symbol Contributors
+Author-email: contributors@symbol.dev
+License: BSD, Public Domain
+Description: Ripemd
+        ======
+        
+        Given headache openssl devs gave to everyone, this is tiny ripemd module for python 3. Shamelessly ~~stolen~~ extracted from [pycryptodome](https://github.com/Legrandin/pycryptodome).
+        
+        ### Usage
+        
+        Single call:
+        ```py
+        from ripemd.ripemd160 import ripemd160  # import function
+        
+        ripemd160(b'abc').hex() == '8eb208f7e05d987a9b044a8e98c6b087f15a0bfc'
+        ripemd160(b'a' * 1000000).hex() == '52783243c1697bdbe16d37f97f68f08325dc1528'
+        ```
+        
+        Update mode:
+        ```py
+        from ripemd import ripemd160  # import module
+        
+        h = ripemd160.new()
+        h.update(b'abc')
+        h.digest().hex() == '8eb208f7e05d987a9b044a8e98c6b087f15a0bfc'
+        ```
+        
+Platform: Posix; MacOS X; Windows
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Public Domain
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Topic :: Security :: Cryptography
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
```

### Comparing `ripemd-hash-1.0.0/setup.py` & `ripemd-hash-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,29 +427,25 @@
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	author="Symbol Contributors",
 	author_email="contributors@symbol.dev",
 	url="https://github.com/symbol/ripemd",
 	platforms='Posix; MacOS X; Windows',
 	zip_safe=False,
-	python_requires='>=3.5',
+	python_requires='>=3.8',
 	classifiers=[
 		'Development Status :: 5 - Production/Stable',
 		'License :: OSI Approved :: BSD License',
 		'License :: OSI Approved :: Apache Software License',
 		'License :: Public Domain',
 		'Intended Audience :: Developers',
 		'Operating System :: Unix',
 		'Operating System :: Microsoft :: Windows',
 		'Operating System :: MacOS :: MacOS X',
 		'Topic :: Security :: Cryptography',
-		'Programming Language :: Python :: 3',
-		'Programming Language :: Python :: 3.5',
-		'Programming Language :: Python :: 3.6',
-		'Programming Language :: Python :: 3.7',
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 	],
 	license="BSD, Public Domain",
 	packages=packages,
 	package_dir={"": "lib"},
```

### Comparing `ripemd-hash-1.0.0/src/common.h` & `ripemd-hash-1.0.1/src/common.h`

 * *Files identical despite different names*

### Comparing `ripemd-hash-1.0.0/src/endianess.h` & `ripemd-hash-1.0.1/src/endianess.h`

 * *Files identical despite different names*

### Comparing `ripemd-hash-1.0.0/src/errors.h` & `ripemd-hash-1.0.1/src/errors.h`

 * *Files identical despite different names*

### Comparing `ripemd-hash-1.0.0/src/ripemd160.c` & `ripemd-hash-1.0.1/src/ripemd160.c`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
  * According to http://www.users.zetnet.co.uk/hopwood/crypto/scan/md.html:
  *   "RIPEMD-160 is big-bit-endian, little-byte-endian, and left-justified."
  */
 
 #include "common.h"
 #include "endianess.h"
 
-FAKE_INIT(RIPEMD160)
+FAKE_INIT(ripemd160)
 
 #define RIPEMD160_DIGEST_SIZE 20
 
 typedef struct {
     uint32_t h[5];      /* The current hash state */
     uint64_t length;    /* Total number of _bits_ (not bytes) added to the
                            hash.  This includes bits that have been buffered
```

