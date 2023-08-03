# Comparing `tmp/parameter-space-2d-0.1.3.tar.gz` & `tmp/parameter-space-2d-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parameter-space-2d-0.1.3.tar", last modified: Wed Apr 26 14:37:04 2023, max compression
+gzip compressed data, was "/home/runner/work/parameter-space-2d/parameter-space-2d/dist/.tmp-h6yh0a83/parameter-space-2d-0.1.4.tar", last modified: Thu Aug  3 11:07:11 2023, max compression
```

## Comparing `parameter-space-2d-0.1.3.tar` & `parameter-space-2d-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:37:04.386889 parameter-space-2d-0.1.3/
--rw-r--r--   0 blandt   (743162876) 1934034978    18650 2023-01-18 15:11:26.000000 parameter-space-2d-0.1.3/LICENSE
--rw-r--r--   0 blandt   (743162876) 1934034978     3004 2023-04-26 14:37:04.387287 parameter-space-2d-0.1.3/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978     2076 2023-01-24 10:19:29.000000 parameter-space-2d-0.1.3/README.md
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:37:04.301099 parameter-space-2d-0.1.3/parameter_space_2d.egg-info/
--rw-r--r--   0 blandt   (743162876) 1934034978     3004 2023-04-26 14:37:03.000000 parameter-space-2d-0.1.3/parameter_space_2d.egg-info/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978      297 2023-04-26 14:37:04.000000 parameter-space-2d-0.1.3/parameter_space_2d.egg-info/SOURCES.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-04-26 14:37:03.000000 parameter-space-2d-0.1.3/parameter_space_2d.egg-info/dependency_links.txt
--rw-r--r--   0 blandt   (743162876) 1934034978       17 2023-04-26 14:37:04.000000 parameter-space-2d-0.1.3/parameter_space_2d.egg-info/requires.txt
--rw-r--r--   0 blandt   (743162876) 1934034978       13 2023-04-26 14:37:04.000000 parameter-space-2d-0.1.3/parameter_space_2d.egg-info/top_level.txt
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:37:04.385649 parameter-space-2d-0.1.3/paramspace2d/
--rw-r--r--   0 blandt   (743162876) 1934034978       26 2023-01-23 16:34:38.000000 parameter-space-2d-0.1.3/paramspace2d/__init__.py
--rw-r--r--   0 blandt   (743162876) 1934034978    15422 2023-01-23 17:30:25.000000 parameter-space-2d-0.1.3/paramspace2d/paramspace.py
--rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-04-26 14:37:04.391010 parameter-space-2d-0.1.3/setup.cfg
--rw-r--r--   0 blandt   (743162876) 1934034978      705 2023-04-26 14:36:54.000000 parameter-space-2d-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:11.000000 parameter-space-2d-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-08-03 11:06:59.000000 parameter-space-2d-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-08-03 11:07:11.000000 parameter-space-2d-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-03 11:06:59.000000 parameter-space-2d-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:11.000000 parameter-space-2d-0.1.4/parameter_space_2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-08-03 11:07:11.000000 parameter-space-2d-0.1.4/parameter_space_2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-03 11:07:11.000000 parameter-space-2d-0.1.4/parameter_space_2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:07:11.000000 parameter-space-2d-0.1.4/parameter_space_2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 11:07:11.000000 parameter-space-2d-0.1.4/parameter_space_2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 11:07:11.000000 parameter-space-2d-0.1.4/parameter_space_2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:07:11.000000 parameter-space-2d-0.1.4/paramspace2d/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 11:06:59.000000 parameter-space-2d-0.1.4/paramspace2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-08-03 11:06:59.000000 parameter-space-2d-0.1.4/paramspace2d/paramspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 11:07:11.000000 parameter-space-2d-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-03 11:06:59.000000 parameter-space-2d-0.1.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `parameter-space-2d-0.1.3/LICENSE` & `parameter-space-2d-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `parameter-space-2d-0.1.3/README.md` & `parameter-space-2d-0.1.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # parameter-space-2d
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/parameter-space/HEAD?filepath=%2Fscripts/INDEX.ipynb)
 [![CC BY 4.0][cc-by-shield]][cc-by]
 [![PyPi version](https://badgen.net/pypi/v/parameter-space-2d/)](https://pypi.org/project/parameter-space-2d)
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/tsmbland/parameter-space-2d/master/docs/example_maps.png" width="100%" height="100%"/>
 </p>
 
@@ -25,36 +24,19 @@
 
 ## Installation
 
     pip install parameter-space-2d
 
 ## Instructions
 
-The repository contains a series of notebooks with instructions for performing analysis, using the Goehring et al. (2011) PAR polarity model as an example. 
+The repository contains a couple of notebooks with instructions for performing analysis, using the Goehring et al. (2011) PAR polarity model as an example. To run the notebooks interactively, click here:
 
-To run in the cloud, click 'launch binder' above.
+<a target="_blank" href="https://colab.research.google.com/github/tsmbland/parameter-space-2d/blob/master/scripts/INDEX.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" height=20/></a>
 
-To run on your local machine, follow these steps:
-
-&#8291;1. Clone the repository:
-
-    git clone https://github.com/tsmbland/parameter-space-2d.git
-    cd parameter-space-2d
-
-&#8291;2. Create conda environment:
-
-    conda env create -f environment.yml
-
-&#8291;3. Activate conda environment:
-
-    conda activate parameter-space-2d
-
-&#8291;4. Open jupyter notebooks:
-
-    jupyter notebook scripts/INDEX.ipynb
 
 
 ## License
 
 This work is licensed under a
 [Creative Commons Attribution 4.0 International License][cc-by].
```

### Comparing `parameter-space-2d-0.1.3/paramspace2d/paramspace.py` & `parameter-space-2d-0.1.4/paramspace2d/paramspace.py`

 * *Files identical despite different names*

### Comparing `parameter-space-2d-0.1.3/setup.py` & `parameter-space-2d-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='parameter-space-2d',
-    version='0.1.3',
+    version='0.1.4',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     install_requires=['numpy',
                       'matplotlib'],
     description='Tools for performing 2D parameter space analysis for deterministic models',
```

