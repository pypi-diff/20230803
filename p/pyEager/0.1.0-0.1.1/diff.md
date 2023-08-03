# Comparing `tmp/pyEager-0.1.0.tar.gz` & `tmp/pyEager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEager-0.1.0.tar", last modified: Wed Aug  2 14:53:40 2023, max compression
+gzip compressed data, was "pyEager-0.1.1.tar", last modified: Wed Aug  2 15:14:07 2023, max compression
```

## Comparing `pyEager-0.1.0.tar` & `pyEager-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-08-02 14:53:40.669780 pyEager-0.1.0/
--rw-r--r--   0 lamnidis   (506) staff       (20)     1071 2023-08-02 14:15:47.000000 pyEager-0.1.0/LICENSE.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)      894 2023-08-02 14:53:40.670049 pyEager-0.1.0/PKG-INFO
--rw-r--r--   0 lamnidis   (506) staff       (20)     1736 2023-08-02 14:42:34.000000 pyEager-0.1.0/README.md
-drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-08-02 14:53:40.666041 pyEager-0.1.0/pyEager/
--rw-r--r--   0 lamnidis   (506) staff       (20)      313 2023-08-02 13:55:17.000000 pyEager-0.1.0/pyEager/__init__.py
--rw-r--r--   0 lamnidis   (506) staff       (20)     4455 2023-08-02 14:07:28.000000 pyEager-0.1.0/pyEager/parsers.py
--rw-r--r--   0 lamnidis   (506) staff       (20)     2929 2023-08-02 12:59:57.000000 pyEager-0.1.0/pyEager/wrappers.py
-drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-08-02 14:53:40.669068 pyEager-0.1.0/pyEager.egg-info/
--rw-r--r--   0 lamnidis   (506) staff       (20)      894 2023-08-02 14:53:40.000000 pyEager-0.1.0/pyEager.egg-info/PKG-INFO
--rw-r--r--   0 lamnidis   (506) staff       (20)      253 2023-08-02 14:53:40.000000 pyEager-0.1.0/pyEager.egg-info/SOURCES.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)        1 2023-08-02 14:53:40.000000 pyEager-0.1.0/pyEager.egg-info/dependency_links.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)       12 2023-08-02 14:53:40.000000 pyEager-0.1.0/pyEager.egg-info/requires.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)        8 2023-08-02 14:53:40.000000 pyEager-0.1.0/pyEager.egg-info/top_level.txt
--rw-r--r--   0 lamnidis   (506) staff       (20)       79 2023-08-02 14:53:40.670793 pyEager-0.1.0/setup.cfg
--rw-r--r--   0 lamnidis   (506) staff       (20)     1144 2023-08-02 14:52:02.000000 pyEager-0.1.0/setup.py
+drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-08-02 15:14:07.528261 pyEager-0.1.1/
+-rw-r--r--   0 lamnidis   (506) staff       (20)     1071 2023-08-02 14:15:47.000000 pyEager-0.1.1/LICENSE.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)     2623 2023-08-02 15:14:07.528512 pyEager-0.1.1/PKG-INFO
+-rw-r--r--   0 lamnidis   (506) staff       (20)     1736 2023-08-02 14:42:34.000000 pyEager-0.1.1/README.md
+drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-08-02 15:14:07.524883 pyEager-0.1.1/pyEager/
+-rw-r--r--   0 lamnidis   (506) staff       (20)      313 2023-08-02 13:55:17.000000 pyEager-0.1.1/pyEager/__init__.py
+-rw-r--r--   0 lamnidis   (506) staff       (20)     4455 2023-08-02 14:07:28.000000 pyEager-0.1.1/pyEager/parsers.py
+-rw-r--r--   0 lamnidis   (506) staff       (20)     2929 2023-08-02 12:59:57.000000 pyEager-0.1.1/pyEager/wrappers.py
+drwxr-xr-x   0 lamnidis   (506) staff       (20)        0 2023-08-02 15:14:07.527595 pyEager-0.1.1/pyEager.egg-info/
+-rw-r--r--   0 lamnidis   (506) staff       (20)     2623 2023-08-02 15:14:07.000000 pyEager-0.1.1/pyEager.egg-info/PKG-INFO
+-rw-r--r--   0 lamnidis   (506) staff       (20)      253 2023-08-02 15:14:07.000000 pyEager-0.1.1/pyEager.egg-info/SOURCES.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)        1 2023-08-02 15:14:07.000000 pyEager-0.1.1/pyEager.egg-info/dependency_links.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)        7 2023-08-02 15:14:07.000000 pyEager-0.1.1/pyEager.egg-info/requires.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)        8 2023-08-02 15:14:07.000000 pyEager-0.1.1/pyEager.egg-info/top_level.txt
+-rw-r--r--   0 lamnidis   (506) staff       (20)       79 2023-08-02 15:14:07.529126 pyEager-0.1.1/setup.cfg
+-rw-r--r--   0 lamnidis   (506) staff       (20)     1171 2023-08-02 15:12:34.000000 pyEager-0.1.1/setup.py
```

### Comparing `pyEager-0.1.0/LICENSE.txt` & `pyEager-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyEager-0.1.0/README.md` & `pyEager-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyEager-0.1.0/pyEager/parsers.py` & `pyEager-0.1.1/pyEager/parsers.py`

 * *Files identical despite different names*

### Comparing `pyEager-0.1.0/pyEager/wrappers.py` & `pyEager-0.1.1/pyEager/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyEager-0.1.0/setup.py` & `pyEager-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from distutils.core import setup
 setup(
   name = 'pyEager',
   packages = ['pyEager'],
-  version = '0.1.0',
+  version = '0.1.1',
   license='MIT',
   description = 'A simple package to read in eager results.',
+  long_description=open('README.md').read(),
   author = 'Thiseas C. Lamnidis',
   author_email = 'thisseass@gmail.com',
   url = 'https://github.com/TCLamnidis/pyEager',
-  download_url = 'https://github.com/TCLamnidis/pyEager/archive/refs/tags/0.1.0.tar.gz',
+  download_url = 'https://github.com/TCLamnidis/pyEager/archive/refs/tags/0.1.1.tar.gz',
   keywords = ['python', 'pandas', 'nf-core', 'eager', 'nf-core/eager', 'ancient DNA' ],
   python_requires=">=3.6",
   install_requires=[
           'pandas',
-          'json',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     # 'Intended Audience :: Developers',      # Define that your audience are developers
     # 'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
```

