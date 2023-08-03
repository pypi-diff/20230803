# Comparing `tmp/AlgDiff-2.1.tar.gz` & `tmp/AlgDiff-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgDiff-2.1.tar", last modified: Thu Jun 15 19:47:41 2023, max compression
+gzip compressed data, was "AlgDiff-2.1.1.tar", last modified: Thu Aug  3 09:05:50 2023, max compression
```

## Comparing `AlgDiff-2.1.tar` & `AlgDiff-2.1.1.tar`

### file list

```diff
@@ -1,16 +1,7 @@
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 19:47:41.138824 AlgDiff-2.1/
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 19:47:41.138824 AlgDiff-2.1/AlgDiff/
--rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)       68 2023-06-15 14:57:11.000000 AlgDiff-2.1/AlgDiff/__init__.py
--rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)    41507 2023-06-15 19:36:33.000000 AlgDiff-2.1/AlgDiff/algebraicDifferentiator.py
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 19:47:41.138824 AlgDiff-2.1/AlgDiff.egg-info/
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    14532 2023-06-15 19:47:41.000000 AlgDiff-2.1/AlgDiff.egg-info/PKG-INFO
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      260 2023-06-15 19:47:41.000000 AlgDiff-2.1/AlgDiff.egg-info/SOURCES.txt
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)        1 2023-06-15 19:47:41.000000 AlgDiff-2.1/AlgDiff.egg-info/dependency_links.txt
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       19 2023-06-15 19:47:41.000000 AlgDiff-2.1/AlgDiff.egg-info/requires.txt
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)        8 2023-06-15 19:47:41.000000 AlgDiff-2.1/AlgDiff.egg-info/top_level.txt
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1458 2023-06-06 12:55:23.000000 AlgDiff-2.1/LICENSE
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    14532 2023-06-15 19:47:41.138824 AlgDiff-2.1/PKG-INFO
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    12074 2023-06-15 16:15:25.000000 AlgDiff-2.1/README.md
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      871 2023-06-15 19:36:33.000000 AlgDiff-2.1/pyproject.toml
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       79 2023-06-15 19:47:41.138824 AlgDiff-2.1/setup.cfg
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1154 2023-06-15 19:36:33.000000 AlgDiff-2.1/setup.py
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-08-03 09:05:50.104585 AlgDiff-2.1.1/
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-08-03 09:05:50.104585 AlgDiff-2.1.1/AlgDiff/
+-rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)       68 2023-06-15 14:57:11.438138 AlgDiff-2.1.1/AlgDiff/__init__.py
+-rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)    41484 2023-08-03 08:24:37.404719 AlgDiff-2.1.1/AlgDiff/algebraicDifferentiator.py
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     2632 2023-08-03 09:05:50.104585 AlgDiff-2.1.1/PKG-INFO
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       40 2023-06-15 19:08:47.507484 AlgDiff-2.1.1/setup.cfg
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1158 2023-08-03 09:05:17.772752 AlgDiff-2.1.1/setup.py
```

### Comparing `AlgDiff-2.1/AlgDiff/algebraicDifferentiator.py` & `AlgDiff-2.1.1/AlgDiff/algebraicDifferentiator.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,14 @@
             out[0] = p[0]
             for i in range(1,L-1):
                 if i%order==0:
                     out[i] = p[0]+p[-1]
                 else:
                     out[i] = p[i%order]
             out[-1] = p[-1]
-            print(out)
             return out
 
                 
         if redFilLength:
             tau1,tau2,_,_,_ = self.reduceFilterLength(der,tol=redTol)
             theta0 = tau1/self.__ts
             L0 = int((tau2-tau1)/self.__ts)+1
```

### Comparing `AlgDiff-2.1/setup.py` & `AlgDiff-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "docs/source/usage.rst").read_text()
 
 setup(
   name = 'AlgDiff',
   packages = ['AlgDiff'],
-  version = '2.1',
+  version = '2.1.1',
   license='bsd-3-clause',
   description = 'AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.',
   
   long_description = long_description,
   long_description_content_type='text/x-rst',
   
   author = 'Amine Othmane',
   author_email = 'amine.othmane@uni-saarland.de',
   url = 'https://github.com/aothmane-control/Algebraic-differentiators',
-  download_url = 'https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.1',
+  download_url = 'https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.1.1',
   keywords = ['numerical-differentiation ', 'fir-filters', 'orthogonal-polynomials', 'numerical-methods '],
   install_requires=[            # I get to this in a second
           'scipy',
           'mpmath',
           'numpy',
       ],
   classifiers=[
```

