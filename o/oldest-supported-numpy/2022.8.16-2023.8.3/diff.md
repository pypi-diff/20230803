# Comparing `tmp/oldest-supported-numpy-2022.8.16.tar.gz` & `tmp/oldest-supported-numpy-2023.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oldest-supported-numpy-2022.8.16.tar", last modified: Tue Aug 16 04:01:24 2022, max compression
+gzip compressed data, was "oldest-supported-numpy-2023.8.3.tar", last modified: Thu Aug  3 16:18:00 2023, max compression
```

## Comparing `oldest-supported-numpy-2022.8.16.tar` & `oldest-supported-numpy-2023.8.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 04:01:24.677741 oldest-supported-numpy-2022.8.16/
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-08-16 04:01:11.000000 oldest-supported-numpy-2022.8.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-08-16 04:01:11.000000 oldest-supported-numpy-2022.8.16/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-08-16 04:01:24.677741 oldest-supported-numpy-2022.8.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3624 2022-08-16 04:01:11.000000 oldest-supported-numpy-2022.8.16/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 04:01:24.677741 oldest-supported-numpy-2022.8.16/oldest_supported_numpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-08-16 04:01:24.000000 oldest-supported-numpy-2022.8.16/oldest_supported_numpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-08-16 04:01:24.000000 oldest-supported-numpy-2022.8.16/oldest_supported_numpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 04:01:24.000000 oldest-supported-numpy-2022.8.16/oldest_supported_numpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2660 2022-08-16 04:01:24.000000 oldest-supported-numpy-2022.8.16/oldest_supported_numpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 04:01:24.000000 oldest-supported-numpy-2022.8.16/oldest_supported_numpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3094 2022-08-16 04:01:24.677741 oldest-supported-numpy-2022.8.16/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)       37 2022-08-16 04:01:11.000000 oldest-supported-numpy-2022.8.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:18:00.282733 oldest-supported-numpy-2023.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-03 16:17:39.000000 oldest-supported-numpy-2023.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 16:17:39.000000 oldest-supported-numpy-2023.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-08-03 16:18:00.282733 oldest-supported-numpy-2023.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-08-03 16:17:39.000000 oldest-supported-numpy-2023.8.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:18:00.282733 oldest-supported-numpy-2023.8.3/oldest_supported_numpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-08-03 16:18:00.000000 oldest-supported-numpy-2023.8.3/oldest_supported_numpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-03 16:18:00.000000 oldest-supported-numpy-2023.8.3/oldest_supported_numpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:18:00.000000 oldest-supported-numpy-2023.8.3/oldest_supported_numpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-08-03 16:18:00.000000 oldest-supported-numpy-2023.8.3/oldest_supported_numpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:18:00.000000 oldest-supported-numpy-2023.8.3/oldest_supported_numpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-03 16:18:00.282733 oldest-supported-numpy-2023.8.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-08-03 16:17:39.000000 oldest-supported-numpy-2023.8.3/setup.py
```

### Comparing `oldest-supported-numpy-2022.8.16/LICENSE` & `oldest-supported-numpy-2023.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oldest-supported-numpy-2022.8.16/oldest_supported_numpy.egg-info/requires.txt` & `oldest-supported-numpy-2023.8.3/oldest_supported_numpy.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,63 @@
 
-[:platform_machine == "loongarch64" and python_version < "3.11"]
+[:platform_machine == "loongarch64" and python_version >= "3.8" and python_version < "3.11"]
 numpy==1.22.2
 
-[:python_version == "3.10" and platform_machine != "loongarch64" and platform_python_implementation != "PyPy"]
+[:python_version == "3.10" and platform_machine != "loongarch64"]
 numpy==1.21.6
 
-[:python_version == "3.11" and platform_python_implementation != "PyPy"]
+[:python_version == "3.11"]
 numpy==1.23.2
 
-[:python_version == "3.5" and platform_machine == "aarch64" and platform_python_implementation != "PyPy"]
-numpy==1.18.5
-
-[:python_version == "3.5" and platform_machine not in "aarch64|loongarch64" and platform_system != "AIX"]
-numpy==1.13.3
-
-[:python_version == "3.5" and platform_system == "AIX"]
-numpy==1.16.0
-
 [:python_version == "3.6" and platform_machine != "loongarch64" and platform_python_implementation == "PyPy"]
 numpy==1.19.0
 
-[:python_version == "3.6" and platform_machine == "aarch64" and platform_python_implementation != "PyPy"]
-numpy==1.19.2
-
-[:python_version == "3.6" and platform_machine not in "aarch64|loongarch64" and platform_system != "AIX" and platform_python_implementation != "PyPy"]
-numpy==1.13.3
-
-[:python_version == "3.6" and platform_system == "AIX"]
-numpy==1.16.0
-
 [:python_version == "3.7" and platform_machine != "loongarch64" and platform_python_implementation == "PyPy"]
 numpy==1.20.0
 
-[:python_version == "3.7" and platform_machine == "aarch64" and platform_python_implementation != "PyPy"]
+[:python_version == "3.7" and platform_machine == "aarch64" and platform_system != "AIX" and platform_python_implementation != "PyPy"]
 numpy==1.19.2
 
-[:python_version == "3.7" and platform_machine == "arm64" and platform_system == "Darwin"]
+[:python_version == "3.7" and platform_machine == "arm64" and platform_system == "Darwin" and platform_python_implementation != "PyPy"]
 numpy==1.21.0
 
+[:python_version == "3.7" and platform_machine == "arm64" and platform_system == "Windows" and platform_python_implementation != "PyPy"]
+numpy==1.14.5
+
 [:python_version == "3.7" and platform_machine not in "arm64|aarch64|loongarch64" and platform_system != "AIX" and platform_python_implementation != "PyPy"]
 numpy==1.14.5
 
-[:python_version == "3.7" and platform_system == "AIX"]
+[:python_version == "3.7" and platform_system == "AIX" and platform_machine != "loongarch64" and platform_python_implementation != "PyPy"]
 numpy==1.16.0
 
 [:python_version == "3.8" and platform_machine != "loongarch64" and platform_python_implementation == "PyPy"]
 numpy==1.22.2
 
 [:python_version == "3.8" and platform_machine == "aarch64" and platform_python_implementation != "PyPy"]
 numpy==1.19.2
 
-[:python_version == "3.8" and platform_machine == "arm64" and platform_system == "Darwin"]
+[:python_version == "3.8" and platform_machine == "arm64" and platform_system == "Darwin" and platform_python_implementation != "PyPy"]
 numpy==1.21.0
 
+[:python_version == "3.8" and platform_machine == "arm64" and platform_system == "Windows" and platform_python_implementation != "PyPy"]
+numpy==1.17.3
+
 [:python_version == "3.8" and platform_machine == "s390x" and platform_python_implementation != "PyPy"]
 numpy==1.17.5
 
 [:python_version == "3.8" and platform_machine not in "arm64|aarch64|s390x|loongarch64" and platform_python_implementation != "PyPy"]
 numpy==1.17.3
 
 [:python_version == "3.9" and platform_machine == "arm64" and platform_system == "Darwin"]
 numpy==1.21.0
 
-[:python_version == "3.9" and platform_machine not in "arm64|loongarch64" and platform_python_implementation != "PyPy"]
+[:python_version == "3.9" and platform_machine == "arm64" and platform_system == "Windows"]
 numpy==1.19.3
 
-[:python_version >= "3.12"]
-numpy
+[:python_version == "3.9" and platform_system == "OS400" and platform_machine != "loongarch64"]
+numpy==1.23.3
+
+[:python_version == "3.9" and platform_system not in "OS400" and platform_machine not in "arm64|loongarch64"]
+numpy==1.19.3
 
-[:python_version >= "3.9" and platform_python_implementation == "PyPy"]
+[:python_version >= "3.12"]
 numpy
```

### Comparing `oldest-supported-numpy-2022.8.16/setup.cfg` & `oldest-supported-numpy-2023.8.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -2,49 +2,48 @@
 name = oldest-supported-numpy
 description = Meta-package that provides the oldest NumPy that supports a given Python version and platform. If wheels for the platform became available on PyPI only for a more recent NumPy version, then that NumPy version is specified.
 long_description = file: README.rst
 author = Thomas Robitaille
 author_email = thomas.robitaille@gmail.com
 license = BSD
 url = https://github.com/scipy/oldest-supported-numpy
-version = 2022.8.16
+version = 2023.08.03
 
 [options]
-python_requires = >=3.5
+python_requires = >=3.7
 install_requires = 
 	
-	numpy==1.16.0; python_version=='3.5' and platform_system=='AIX'
-	numpy==1.16.0; python_version=='3.6' and platform_system=='AIX'
-	numpy==1.16.0; python_version=='3.7' and platform_system=='AIX'
-	
-	numpy==1.18.5; python_version=='3.5' and platform_machine=='aarch64' and platform_python_implementation != 'PyPy'
-	numpy==1.19.2; python_version=='3.6' and platform_machine=='aarch64' and platform_python_implementation != 'PyPy'
-	numpy==1.19.2; python_version=='3.7' and platform_machine=='aarch64' and platform_python_implementation != 'PyPy'
+	numpy==1.16.0; python_version=='3.7' and platform_system=='AIX' and platform_machine!='loongarch64' and platform_python_implementation != 'PyPy'
+	
+	numpy==1.23.3; python_version=='3.9' and platform_system=='OS400' and platform_machine!='loongarch64'
+	
+	numpy==1.19.2; python_version=='3.7' and platform_machine=='aarch64' and platform_system!='AIX' and platform_python_implementation != 'PyPy'
 	numpy==1.19.2; python_version=='3.8' and platform_machine=='aarch64' and platform_python_implementation != 'PyPy'
 	
-	numpy==1.21.0; python_version=='3.7' and platform_machine=='arm64' and platform_system=='Darwin'
-	numpy==1.21.0; python_version=='3.8' and platform_machine=='arm64' and platform_system=='Darwin'
+	numpy==1.21.0; python_version=='3.7' and platform_machine=='arm64' and platform_system=='Darwin' and platform_python_implementation!='PyPy'
+	numpy==1.21.0; python_version=='3.8' and platform_machine=='arm64' and platform_system=='Darwin' and platform_python_implementation!='PyPy'
 	numpy==1.21.0; python_version=='3.9' and platform_machine=='arm64' and platform_system=='Darwin'
 	
 	numpy==1.17.5; python_version=='3.8' and platform_machine=='s390x' and platform_python_implementation != 'PyPy'
 	
-	numpy==1.22.2; platform_machine=='loongarch64' and python_version<'3.11'
+	numpy==1.22.2; platform_machine=='loongarch64' and python_version>='3.8' and python_version<'3.11'
+	
+	numpy==1.14.5; python_version=='3.7' and platform_machine=='arm64' and platform_system=='Windows' and platform_python_implementation != 'PyPy'
+	numpy==1.17.3; python_version=='3.8' and platform_machine=='arm64' and platform_system=='Windows' and platform_python_implementation != 'PyPy'
+	numpy==1.19.3; python_version=='3.9' and platform_machine=='arm64' and platform_system=='Windows'
 	
-	numpy==1.13.3; python_version=='3.5' and platform_machine not in 'aarch64|loongarch64' and platform_system!='AIX'
-	numpy==1.13.3; python_version=='3.6' and platform_machine not in 'aarch64|loongarch64' and platform_system!='AIX' and platform_python_implementation != 'PyPy'
 	numpy==1.14.5; python_version=='3.7' and platform_machine not in 'arm64|aarch64|loongarch64' and platform_system!='AIX' and platform_python_implementation != 'PyPy'
 	numpy==1.17.3; python_version=='3.8' and platform_machine not in 'arm64|aarch64|s390x|loongarch64' and platform_python_implementation != 'PyPy'
-	numpy==1.19.3; python_version=='3.9' and platform_machine not in 'arm64|loongarch64' and platform_python_implementation != 'PyPy'
-	numpy==1.21.6; python_version=='3.10' and platform_machine!='loongarch64' and platform_python_implementation != 'PyPy'
-	numpy==1.23.2; python_version=='3.11' and platform_python_implementation != 'PyPy'
+	numpy==1.19.3; python_version=='3.9' and platform_system not in 'OS400' and platform_machine not in 'arm64|loongarch64'
+	numpy==1.21.6; python_version=='3.10' and platform_machine!='loongarch64'
+	numpy==1.23.2; python_version=='3.11'
 	
 	numpy==1.19.0; python_version=='3.6' and platform_machine!='loongarch64' and platform_python_implementation=='PyPy'
 	numpy==1.20.0; python_version=='3.7' and platform_machine!='loongarch64' and platform_python_implementation=='PyPy'
 	numpy==1.22.2; python_version=='3.8' and platform_machine!='loongarch64' and platform_python_implementation=='PyPy'
 	
 	numpy; python_version>='3.12'
-	numpy; python_version>='3.9' and platform_python_implementation=='PyPy'
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

