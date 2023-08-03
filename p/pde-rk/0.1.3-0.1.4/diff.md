# Comparing `tmp/pde-rk-0.1.3.tar.gz` & `tmp/pde-rk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pde-rk-0.1.3.tar", last modified: Wed Apr 26 14:22:21 2023, max compression
+gzip compressed data, was "/home/runner/work/pde-rk/pde-rk/dist/.tmp-fpa2zcge/pde-rk-0.1.4.tar", last modified: Thu Aug  3 11:11:42 2023, max compression
```

## Comparing `pde-rk-0.1.3.tar` & `pde-rk-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:22:21.794171 pde-rk-0.1.3/
--rw-r--r--   0 blandt   (743162876) 1934034978    18650 2023-01-18 15:11:26.000000 pde-rk-0.1.3/LICENSE
--rw-r--r--   0 blandt   (743162876) 1934034978     2076 2023-04-26 14:22:21.794451 pde-rk-0.1.3/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978     1303 2023-01-24 10:06:48.000000 pde-rk-0.1.3/README.md
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:22:21.778601 pde-rk-0.1.3/pde_rk/
--rw-r--r--   0 blandt   (743162876) 1934034978       19 2023-01-23 17:09:04.000000 pde-rk-0.1.3/pde_rk/__init__.py
--rw-r--r--   0 blandt   (743162876) 1934034978     6824 2023-01-23 17:09:04.000000 pde-rk-0.1.3/pde_rk/pde.py
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:22:21.793128 pde-rk-0.1.3/pde_rk.egg-info/
--rw-r--r--   0 blandt   (743162876) 1934034978     2076 2023-04-26 14:22:19.000000 pde-rk-0.1.3/pde_rk.egg-info/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978      218 2023-04-26 14:22:20.000000 pde-rk-0.1.3/pde_rk.egg-info/SOURCES.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-04-26 14:22:19.000000 pde-rk-0.1.3/pde_rk.egg-info/dependency_links.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        6 2023-04-26 14:22:19.000000 pde-rk-0.1.3/pde_rk.egg-info/requires.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        7 2023-04-26 14:22:19.000000 pde-rk-0.1.3/pde_rk.egg-info/top_level.txt
--rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-04-26 14:22:21.797444 pde-rk-0.1.3/setup.cfg
--rw-r--r--   0 blandt   (743162876) 1934034978      666 2023-04-26 14:21:31.000000 pde-rk-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:11:42.000000 pde-rk-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-08-03 11:11:29.000000 pde-rk-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-03 11:11:42.000000 pde-rk-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-03 11:11:29.000000 pde-rk-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:11:42.000000 pde-rk-0.1.4/pde_rk/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 11:11:29.000000 pde-rk-0.1.4/pde_rk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-08-03 11:11:29.000000 pde-rk-0.1.4/pde_rk/pde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:11:42.000000 pde-rk-0.1.4/pde_rk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-03 11:11:42.000000 pde-rk-0.1.4/pde_rk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-03 11:11:42.000000 pde-rk-0.1.4/pde_rk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:11:42.000000 pde-rk-0.1.4/pde_rk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 11:11:42.000000 pde-rk-0.1.4/pde_rk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 11:11:42.000000 pde-rk-0.1.4/pde_rk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 11:11:42.000000 pde-rk-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-03 11:11:29.000000 pde-rk-0.1.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pde-rk-0.1.3/LICENSE` & `pde-rk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pde-rk-0.1.3/README.md` & `pde-rk-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,38 @@
+Metadata-Version: 2.1
+Name: pde-rk
+Version: 0.1.4
+Summary: Package for simulating one-dimensional PDE models with and adaptive Runge-Kutta scheme
+Author: Tom Bland
+Author-email: tom_bland@hotmail.co.uk
+License: CC BY 4.0
+Project-URL: Source Code, https://github.com/tsmbland/pde-rk
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pde-rk
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/pde-rk/HEAD?filepath=%2Fscripts/simulate_par.ipynb)
 [![CC BY 4.0][cc-by-shield]][cc-by]
 [![PyPi version](https://badgen.net/pypi/v/pde-rk/)](https://pypi.org/project/pde-rk)
 
 Functions for simulating PDE models with an adaptive Runge-Kutta scheme
 
 ## Installation
 
     pip install pde-rk
 
 ## Instructions
 
-The repository contains an example notebook that demonstrates the method using the PAR polarity model (Goehring et al., 2011)
-
-To run in the cloud, click 'launch binder' above.
-
-To run on your local machine, follow these steps:
-
-&#8291;1. Clone the repository:
-
-    git clone https://github.com/tsmbland/pde-rk.git
-    cd pde-rk
-
-&#8291;2. Create conda environment:
-
-    conda env create -f environment.yml
-
-&#8291;3. Activate conda environment:
+The repository contains an example notebook that demonstrates the method using the PAR polarity model (Goehring et al., 2011).
+To run the notebook in Colab, click here: 
 
-    conda activate pde-rk
+<a target="_blank" href="https://colab.research.google.com/github/tsmbland/pde-rk/blob/master/scripts/simulate_par.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" height=20/></a>
 
-&#8291;4. Open jupyter notebook:
 
-    jupyter notebook scripts/simulate_par.ipynb
 
 ## License
 
 This work is licensed under a
 [Creative Commons Attribution 4.0 International License][cc-by].
 
 [![CC BY 4.0][cc-by-image]][cc-by]
```

### Comparing `pde-rk-0.1.3/pde_rk/pde.py` & `pde-rk-0.1.4/pde_rk/pde.py`

 * *Files identical despite different names*

### Comparing `pde-rk-0.1.3/setup.py` & `pde-rk-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pde-rk',
-    version='0.1.3',
+    version='0.1.4',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     install_requires=['numpy'],
     description='Package for simulating one-dimensional PDE models with and adaptive Runge-Kutta scheme',
     long_description=long_description,
     long_description_content_type='text/markdown',
     project_urls={
-            "Source Code": "https://github.com/tsmbland/pde-rk",
-        }
+        "Source Code": "https://github.com/tsmbland/pde-rk",
+    }
 )
```

