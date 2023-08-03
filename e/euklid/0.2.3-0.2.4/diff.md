# Comparing `tmp/euklid-0.2.3.tar.gz` & `tmp/euklid-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\euklid-0.2.3.tar", last modified: Tue Mar  7 07:50:50 2023, max compression
+gzip compressed data, was "euklid-0.2.4.tar", last modified: Thu Aug  3 11:08:17 2023, max compression
```

## Comparing `euklid-0.2.3.tar` & `euklid-0.2.4.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 07:50:50.000000 euklid-0.2.3/
--rw-rw-rw-   0        0        0     1037 2023-03-07 07:50:50.000000 euklid-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-03-07 07:39:38.000000 euklid-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-07 07:50:50.000000 euklid-0.2.3/euklid.egg-info/
--rw-rw-rw-   0        0        0     1037 2023-03-07 07:50:50.000000 euklid-0.2.3/euklid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2023-03-07 07:50:50.000000 euklid-0.2.3/euklid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 07:50:50.000000 euklid-0.2.3/euklid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 07:50:50.000000 euklid-0.2.3/euklid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-07 07:50:50.000000 euklid-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     4502 2023-03-07 07:39:38.000000 euklid-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:08:17.307781 euklid-0.2.4/
+-rw-rw-rw-   0        0        0     1084 2023-08-03 10:52:47.000000 euklid-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      789 2023-08-03 11:08:17.307781 euklid-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2023-08-03 10:52:47.000000 euklid-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 11:08:17.307781 euklid-0.2.4/euklid.egg-info/
+-rw-rw-rw-   0        0        0      789 2023-08-03 11:08:17.000000 euklid-0.2.4/euklid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2023-08-03 11:08:17.000000 euklid-0.2.4/euklid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 11:08:17.000000 euklid-0.2.4/euklid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 11:08:17.000000 euklid-0.2.4/euklid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 11:08:17.307781 euklid-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     4392 2023-08-03 10:52:47.000000 euklid-0.2.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `euklid-0.2.3/PKG-INFO` & `euklid-0.2.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: euklid
-Version: 0.2.3
+Version: 0.2.4
 Summary: common vector operations [2D/3D]
 Home-page: http://github.com/airgproducts/euklid
 Author: airgproducts
-Author-email: UNKNOWN
 License: MIT
-Description: # Euklid [2D and 3D vector operations]
-        
-        [![PyPI version](https://badge.fury.io/py/euklid.svg)](https://badge.fury.io/py/euklid)
-        
-        A c++ library with bindings for python to help dealing with common CAD-like operations:
-        
-         * [Vectors](./src/vector/README.md)
-         * [PolyLines](./src/polyline/README.md)
-         * [Spline Curves](./src/spline/README.md)
-        
-        
-        ## Installation
-        
-        
-        ### install via pip:
-        
-        `pip install euklid`
-        
-        ### Compile from source:
-        
-        ``` bash
-        git clone https://github.com/airgproducts/euklid
-        cd euklid
-        git submodule init
-        git submodule update
-        pip install .
-        ```
-        
-Platform: UNKNOWN
+License-File: LICENSE
+
+# Euklid [2D and 3D vector operations]
+
+[![PyPI version](https://badge.fury.io/py/euklid.svg)](https://badge.fury.io/py/euklid)
+
+A c++ library with bindings for python to help dealing with common CAD-like operations:
+
+ * [Vectors](./src/vector/README.md)
+ * [PolyLines](./src/polyline/README.md)
+ * [Spline Curves](./src/spline/README.md)
+
+
+## Installation
+
+
+### install via pip:
+
+`pip install euklid`
+
+### Compile from source:
+
+``` bash
+git clone https://github.com/airgproducts/euklid
+cd euklid
+git submodule init
+git submodule update
+pip install .
+```
```

### Comparing `euklid-0.2.3/README.md` & `euklid-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `euklid-0.2.3/euklid.egg-info/PKG-INFO` & `euklid-0.2.4/euklid.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: euklid
-Version: 0.2.3
+Version: 0.2.4
 Summary: common vector operations [2D/3D]
 Home-page: http://github.com/airgproducts/euklid
 Author: airgproducts
-Author-email: UNKNOWN
 License: MIT
-Description: # Euklid [2D and 3D vector operations]
-        
-        [![PyPI version](https://badge.fury.io/py/euklid.svg)](https://badge.fury.io/py/euklid)
-        
-        A c++ library with bindings for python to help dealing with common CAD-like operations:
-        
-         * [Vectors](./src/vector/README.md)
-         * [PolyLines](./src/polyline/README.md)
-         * [Spline Curves](./src/spline/README.md)
-        
-        
-        ## Installation
-        
-        
-        ### install via pip:
-        
-        `pip install euklid`
-        
-        ### Compile from source:
-        
-        ``` bash
-        git clone https://github.com/airgproducts/euklid
-        cd euklid
-        git submodule init
-        git submodule update
-        pip install .
-        ```
-        
-Platform: UNKNOWN
+License-File: LICENSE
+
+# Euklid [2D and 3D vector operations]
+
+[![PyPI version](https://badge.fury.io/py/euklid.svg)](https://badge.fury.io/py/euklid)
+
+A c++ library with bindings for python to help dealing with common CAD-like operations:
+
+ * [Vectors](./src/vector/README.md)
+ * [PolyLines](./src/polyline/README.md)
+ * [Spline Curves](./src/spline/README.md)
+
+
+## Installation
+
+
+### install via pip:
+
+`pip install euklid`
+
+### Compile from source:
+
+``` bash
+git clone https://github.com/airgproducts/euklid
+cd euklid
+git submodule init
+git submodule update
+pip install .
+```
```

### Comparing `euklid-0.2.3/setup.py` & `euklid-0.2.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from distutils.core import setup
 import setuptools
 from setuptools.command.build_ext import build_ext
 from setuptools.command.install_lib import install_lib
 from setuptools.command.install import install
 
 
+version = "0.2.4"
+
 DEBUG = False
 if "--debug" in sys.argv:
     DEBUG = True
     sys.argv.remove("--debug")
 
 CONDA_BUILD = False
 if "--conda" in sys.argv:
@@ -107,27 +109,24 @@
             subprocess.check_call([sys.executable, 'stubs.py', stubgen_path])
         except subprocess.CalledProcessError:
             print("no mypy found")
 
 
         
 
-version = "-"
-with open("src/version.hpp") as version_file:
-    #print(version_file.read())
-    version = re.findall(r"version\s=\s['\"]([0-9\._]+)['\"]", version_file.read())[0]
 
 with open("README.md") as readme_file:
     long_description = readme_file.read()
 
 
 setup(
     name='euklid',
     version=version,
     description="common vector operations [2D/3D]",
+    package_data={"version": ["src/version.hpp"]},
     ext_modules=[CMakeExtension('.')],
     cmdclass={"build_ext": CMakeBuild, "install_lib": InstallStubs},
     license='MIT',
     long_description=long_description,
     author='airgproducts',
     url='http://github.com/airgproducts/euklid',
     test_suite="tests.test_suite",
```

