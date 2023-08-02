# Comparing `tmp/VBBinaryLensing-3.6.0.tar.gz` & `tmp/VBBinaryLensing-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VBBinaryLensing-3.6.0.tar", last modified: Tue May 30 17:06:59 2023, max compression
+gzip compressed data, was "VBBinaryLensing-3.6.1.tar", last modified: Wed Aug  2 23:15:32 2023, max compression
```

## Comparing `VBBinaryLensing-3.6.0.tar` & `VBBinaryLensing-3.6.1.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-05-30 17:06:59.115445 VBBinaryLensing-3.6.0/
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)     7651 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/LICENSE
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)       59 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/MANIFEST.in
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)      399 2023-05-30 17:06:59.115445 VBBinaryLensing-3.6.0/PKG-INFO
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)     5143 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/README.md
-drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-05-30 17:06:59.111445 VBBinaryLensing-3.6.0/VBBinaryLensing/
-drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-05-30 17:06:59.115445 VBBinaryLensing-3.6.0/VBBinaryLensing/data/
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)   488032 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/data/ESPL.tbl
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)       18 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/data/OB151212coords.txt
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)        0 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/data/__init__.py
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)   110290 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/data/satellite1.txt
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)   112560 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/data/satellite2.txt
-drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-05-30 17:06:59.115445 VBBinaryLensing-3.6.0/VBBinaryLensing/lib/
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)   145025 2023-05-30 16:55:13.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)    11092 2023-05-30 16:55:13.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/lib/VBBinaryLensingLibrary.h
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)    30353 2023-05-30 16:02:34.000000 VBBinaryLensing-3.6.0/VBBinaryLensing/lib/python_bindings.cpp
-drwxrwxr-x   0 bachelet  (1000) bachelet  (1000)        0 2023-05-30 17:06:59.115445 VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)      399 2023-05-30 17:06:59.000000 VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/PKG-INFO
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)      587 2023-05-30 17:06:59.000000 VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/SOURCES.txt
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)        1 2023-05-30 17:06:59.000000 VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/dependency_links.txt
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)        1 2023-05-30 16:08:24.000000 VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/not-zip-safe
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)       14 2023-05-30 17:06:59.000000 VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/requires.txt
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)       16 2023-05-30 17:06:59.000000 VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/top_level.txt
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)      875 2023-05-30 17:06:59.115445 VBBinaryLensing-3.6.0/setup.cfg
--rw-rw-r--   0 bachelet  (1000) bachelet  (1000)     3696 2023-05-30 16:55:13.000000 VBBinaryLensing-3.6.0/setup.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:15:32.064952 VBBinaryLensing-3.6.1/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     7651 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/LICENSE
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       59 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/MANIFEST.in
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     6162 2023-08-02 23:15:32.064952 VBBinaryLensing-3.6.1/PKG-INFO
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     5143 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/README.md
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:15:32.060952 VBBinaryLensing-3.6.1/VBBinaryLensing/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       45 2023-08-02 23:09:57.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/__init__.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:15:32.064952 VBBinaryLensing-3.6.1/VBBinaryLensing/data/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)   488032 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/data/ESPL.tbl
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       18 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/data/OB151212coords.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/data/__init__.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)   110290 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/data/satellite1.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)   112560 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/data/satellite2.txt
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:15:32.064952 VBBinaryLensing-3.6.1/VBBinaryLensing/lib/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)   145042 2023-07-30 22:24:42.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    11092 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/lib/VBBinaryLensingLibrary.h
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    30353 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/lib/python_bindings.cpp
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:15:32.064952 VBBinaryLensing-3.6.1/VBBinaryLensing/tests/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1995 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/tests/test_all.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     7279 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/tests/test_magnification.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:15:32.064952 VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     6162 2023-08-02 23:15:32.000000 VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/PKG-INFO
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)      670 2023-08-02 23:15:32.000000 VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/SOURCES.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        1 2023-08-02 23:15:32.000000 VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/dependency_links.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       28 2023-08-02 23:15:32.000000 VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/requires.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       45 2023-08-02 23:15:32.000000 VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/top_level.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1322 2023-08-02 23:09:57.000000 VBBinaryLensing-3.6.1/pyproject.toml
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)      875 2023-08-02 23:15:32.068952 VBBinaryLensing-3.6.1/setup.cfg
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     2685 2023-08-02 23:09:57.000000 VBBinaryLensing-3.6.1/setup.py
```

### Comparing `VBBinaryLensing-3.6.0/LICENSE` & `VBBinaryLensing-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.0/README.md` & `VBBinaryLensing-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.0/VBBinaryLensing/data/ESPL.tbl` & `VBBinaryLensing-3.6.1/VBBinaryLensing/data/ESPL.tbl`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.0/VBBinaryLensing/data/satellite1.txt` & `VBBinaryLensing-3.6.1/VBBinaryLensing/data/satellite1.txt`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.0/VBBinaryLensing/data/satellite2.txt` & `VBBinaryLensing-3.6.1/VBBinaryLensing/data/satellite2.txt`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.0/VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp` & `VBBinaryLensing-3.6.1/VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2806,15 +2806,15 @@
 		}
 		else {
 			theta->errworst = abs(zr[worst1] - zr[worst2]);
 		}
 
 	} 
 	else { 
-		if (good[worst2]*dlmax > good[worst3] + 1.e-12) { // Dubious cases. Better exclude them
+		 if (good[worst2]*dlmax > good[worst3] + 1.e-12 && theta->th>=0) { // Dubious cases. Better exclude them
 			return Prov;
 		}
 		else {		// 5 good roots
 			f1 = 0;
 			for (int i = 0; i < 5; i++) {
 				Prov->append(zr[i].re, zr[i].im);
```

### Comparing `VBBinaryLensing-3.6.0/VBBinaryLensing/lib/VBBinaryLensingLibrary.h` & `VBBinaryLensing-3.6.1/VBBinaryLensing/lib/VBBinaryLensingLibrary.h`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.0/VBBinaryLensing/lib/python_bindings.cpp` & `VBBinaryLensing-3.6.1/VBBinaryLensing/lib/python_bindings.cpp`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.0/VBBinaryLensing.egg-info/SOURCES.txt` & `VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
+VBBinaryLensing/__init__.py
 VBBinaryLensing.egg-info/PKG-INFO
 VBBinaryLensing.egg-info/SOURCES.txt
 VBBinaryLensing.egg-info/dependency_links.txt
-VBBinaryLensing.egg-info/not-zip-safe
 VBBinaryLensing.egg-info/requires.txt
 VBBinaryLensing.egg-info/top_level.txt
 VBBinaryLensing/data/ESPL.tbl
 VBBinaryLensing/data/OB151212coords.txt
 VBBinaryLensing/data/__init__.py
 VBBinaryLensing/data/satellite1.txt
 VBBinaryLensing/data/satellite2.txt
 VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp
 VBBinaryLensing/lib/VBBinaryLensingLibrary.h
-VBBinaryLensing/lib/python_bindings.cpp
+VBBinaryLensing/lib/python_bindings.cpp
+VBBinaryLensing/tests/test_all.py
+VBBinaryLensing/tests/test_magnification.py
```

### Comparing `VBBinaryLensing-3.6.0/setup.cfg` & `VBBinaryLensing-3.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.0/setup.py` & `VBBinaryLensing-3.6.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,27 @@
-from setuptools import setup, Extension, find_packages
-from setuptools.command.build_ext import build_ext
 import sys
-import setuptools
-import os
-
-__version__ = '3.6.0'
-
-
-class get_pybind_include(object):
-    """Helper class to determine the pybind11 include path
-
-    The purpose of this class is to postpone importing pybind11
-    until it is actually installed, so that the ``get_include()``
-    method can be invoked. """
-
-    def __init__(self, user=False):
-        self.user = user
-
-    def __str__(self):
-        import pybind11
-        return pybind11.get_include(self.user)
 
+import setuptools
+from pybind11.setup_helpers import Pybind11Extension
+from setuptools import setup
+from setuptools.command.build_ext import build_ext
 
 ext_modules = [
-    Extension(
-        'VBBinaryLensing',
-        ['VBBinaryLensing/lib/python_bindings.cpp', 'VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp'],
-        include_dirs=[
-            # Path to pybind11 headers
-            get_pybind_include(),
-            get_pybind_include(user=True)
+    Pybind11Extension(
+        # Import package name
+        name="VBBinaryLensing.VBBinaryLensing",
+
+        # List of C++ source code
+        sources=[
+            'VBBinaryLensing/lib/python_bindings.cpp',
+            'VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp'
         ],
-        language='c++'
+
+        # Path to dir of C++ headers
+        include_dirs=["VBBinaryLensing/lib/"],
     ),
 ]
 
 
 # As of Python 3.6, CCompiler has a `has_flag` method.
 # cf http://bugs.python.org/issue26689
 def has_flag(compiler, flagname):
@@ -62,16 +48,14 @@
     for flag in flags:
         if has_flag(compiler, flag): return flag
 
     raise RuntimeError('Unsupported compiler -- at least C++11 support '
                        'is needed!')
 
 
-
-
 class BuildExt(build_ext):
     """A custom build extension for adding compiler-specific options."""
     c_opts = {
         'msvc': ['/EHsc'],
         'unix': [],
     }
     l_opts = {
@@ -97,26 +81,10 @@
             opts.append('/DVERSION_INFO=\\"%s\\"' % self.distribution.get_version())
         for ext in self.extensions:
             ext.extra_compile_args = opts
             ext.extra_link_args = link_opts
         build_ext.build_extensions(self)
 
 setup(
-    name='VBBinaryLensing',
-    version=__version__,
-    author='Valerio Bozza, Fran Bartolic, Etienne Bachelet',
-    author_email='valboz@sa.infn.it, fb90@st-andrews.ac.uk, etibachelet@gmail.com',
-    url='https://github.com/valboz/VBBinaryLensing',
-    description='Python wrapper of the VBBinaryLensing code for \
-            computing microlensing light curves.',
-    long_description='',
     ext_modules=ext_modules,
-    install_requires=['pybind11>=2.3'],
-    setup_requires=['pybind11>=2.3'],
     cmdclass={'build_ext': BuildExt},
-    zip_safe=False,
-    include_package_data=True,
-    packages=['VBBinaryLensing.data'],
-    package_data={'VBBinaryLensing.data': ['data/*',]},
-               
-    
 )
```

