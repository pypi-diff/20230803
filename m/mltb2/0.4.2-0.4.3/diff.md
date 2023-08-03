# Comparing `tmp/mltb2-0.4.2.tar.gz` & `tmp/mltb2-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltb2-0.4.2.tar", last modified: Wed Aug  2 21:46:28 2023, max compression
+gzip compressed data, was "mltb2-0.4.3.tar", last modified: Thu Aug  3 07:01:03 2023, max compression
```

## Comparing `mltb2-0.4.2.tar` & `mltb2-0.4.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:46:28.700294 mltb2-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 21:46:16.000000 mltb2-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 21:46:16.000000 mltb2-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-02 21:46:28.700294 mltb2-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-02 21:46:16.000000 mltb2-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:46:28.696294 mltb2-0.4.2/mltb2/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-08-02 21:46:16.000000 mltb2-0.4.2/mltb2/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:46:28.696294 mltb2-0.4.2/mltb2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-02 21:46:28.000000 mltb2-0.4.2/mltb2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-02 21:46:28.000000 mltb2-0.4.2/mltb2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:46:28.000000 mltb2-0.4.2/mltb2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:46:28.000000 mltb2-0.4.2/mltb2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-02 21:46:28.000000 mltb2-0.4.2/mltb2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 21:46:28.000000 mltb2-0.4.2/mltb2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-02 21:46:16.000000 mltb2-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-02 21:46:28.700294 mltb2-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-08-02 21:46:16.000000 mltb2-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:46:28.700294 mltb2-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test_fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test_somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test_somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-02 21:46:16.000000 mltb2-0.4.2/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:01:03.939557 mltb2-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-03 07:00:49.000000 mltb2-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-03 07:00:49.000000 mltb2-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-03 07:01:03.939557 mltb2-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-03 07:00:49.000000 mltb2-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:01:03.935557 mltb2-0.4.3/mltb2/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-03 07:00:49.000000 mltb2-0.4.3/mltb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-08-03 07:00:49.000000 mltb2-0.4.3/mltb2/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-03 07:00:49.000000 mltb2-0.4.3/mltb2/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-03 07:00:49.000000 mltb2-0.4.3/mltb2/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-08-03 07:00:49.000000 mltb2-0.4.3/mltb2/optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-08-03 07:00:49.000000 mltb2-0.4.3/mltb2/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:00:49.000000 mltb2-0.4.3/mltb2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-08-03 07:00:49.000000 mltb2-0.4.3/mltb2/somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-08-03 07:00:49.000000 mltb2-0.4.3/mltb2/somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-08-03 07:00:49.000000 mltb2-0.4.3/mltb2/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:01:03.935557 mltb2-0.4.3/mltb2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-03 07:01:03.000000 mltb2-0.4.3/mltb2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-03 07:01:03.000000 mltb2-0.4.3/mltb2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:01:03.000000 mltb2-0.4.3/mltb2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:01:03.000000 mltb2-0.4.3/mltb2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-03 07:01:03.000000 mltb2-0.4.3/mltb2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 07:01:03.000000 mltb2-0.4.3/mltb2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-03 07:00:49.000000 mltb2-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-03 07:01:03.939557 mltb2-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-08-03 07:00:49.000000 mltb2-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:01:03.939557 mltb2-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-03 07:00:49.000000 mltb2-0.4.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-03 07:00:49.000000 mltb2-0.4.3/tests/test__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-03 07:00:49.000000 mltb2-0.4.3/tests/test_fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-03 07:00:49.000000 mltb2-0.4.3/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-03 07:00:49.000000 mltb2-0.4.3/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-03 07:00:49.000000 mltb2-0.4.3/tests/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-08-03 07:00:49.000000 mltb2-0.4.3/tests/test_somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-08-03 07:00:49.000000 mltb2-0.4.3/tests/test_somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-03 07:00:49.000000 mltb2-0.4.3/tests/test_transformers.py
```

### Comparing `mltb2-0.4.2/LICENSE` & `mltb2-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/PKG-INFO` & `mltb2-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.4.2
+Version: 0.4.3
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
```

### Comparing `mltb2-0.4.2/README.md` & `mltb2-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/mltb2/fasttext.py` & `mltb2-0.4.3/mltb2/fasttext.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/mltb2/files.py` & `mltb2-0.4.3/mltb2/files.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/mltb2/openai.py` & `mltb2-0.4.3/mltb2/openai.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/mltb2/optuna.py` & `mltb2-0.4.3/mltb2/optuna.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/mltb2/plot.py` & `mltb2-0.4.3/mltb2/plot.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/mltb2/somajo.py` & `mltb2-0.4.3/mltb2/somajo.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/mltb2/somajo_transformers.py` & `mltb2-0.4.3/mltb2/somajo_transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/mltb2/transformers.py` & `mltb2-0.4.3/mltb2/transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/mltb2.egg-info/PKG-INFO` & `mltb2-0.4.3/mltb2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.4.2
+Version: 0.4.3
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
```

### Comparing `mltb2-0.4.2/mltb2.egg-info/requires.txt` & `mltb2-0.4.3/mltb2.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 numpy
 scipy
 tqdm
 
 [all]
-scikit-learn
-optuna
-fasttext-wheel
-tiktoken
-sphinx
-numpy
-flake8
-SoMaJo
-packaging
+mdformat
 sphinx_copybutton
-mypy
-pydocstyle
-matplotlib
+torch
+pytest
+platformdirs
+flake8
+pylint
 transformers
+numpy
+tiktoken
+mypy
 sphinx_rtd_theme
+packaging
 isort
-platformdirs
-torch
+optuna
 pylintfileheader
+tqdm
+pydocstyle
+fasttext-wheel
 black
+matplotlib
 scipy
-mdformat
-tqdm
-pylint
-pytest
+scikit-learn
+sphinx
+SoMaJo
 
 [checking]
 black
 flake8
 isort
 mdformat
 pydocstyle
@@ -41,60 +41,60 @@
 
 [doc]
 sphinx
 sphinx_rtd_theme
 sphinx_copybutton
 
 [fasttext]
+scikit-learn
 fasttext-wheel
 platformdirs
-scikit-learn
 
 [files]
-platformdirs
 scikit-learn
+platformdirs
 
 [openai]
 tiktoken
 
 [optional]
-torch
-scikit-learn
-SoMaJo
-matplotlib
-tiktoken
+platformdirs
 transformers
-optuna
+matplotlib
 scipy
-fasttext-wheel
-platformdirs
+optuna
 numpy
 tqdm
+torch
+tiktoken
+scikit-learn
+fasttext-wheel
+SoMaJo
 
 [optuna]
-numpy
-optuna
 scipy
+optuna
+numpy
 
 [plot]
 matplotlib
 
 [somajo]
 tqdm
 SoMaJo
 
 [somajo_transformers]
-torch
 scikit-learn
+torch
 transformers
-SoMaJo
 tqdm
+SoMaJo
 
 [testing]
 pytest
 packaging
 
 [transformers]
-torch
-scikit-learn
 transformers
+scikit-learn
 tqdm
+torch
```

### Comparing `mltb2-0.4.2/pyproject.toml` & `mltb2-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/setup.py` & `mltb2-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         # "Code of Conduct": source_code + "/blob/main/CODE_OF_CONDUCT.md",
     },
     packages=setuptools.find_packages(),
     python_requires=">=3.8",
     install_requires=install_requires,
     extras_require=extras_require,
     zip_safe=False,
+    package_data={"mltb2": ["py.typed"]},
     keywords=keywords,
     classifiers=[
         "Development Status :: 3 - Alpha",
         # "Development Status :: 4 - Beta",
         # "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         # "Intended Audience :: Education",
```

### Comparing `mltb2-0.4.2/tests/test_fasttext.py` & `mltb2-0.4.3/tests/test_fasttext.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/tests/test_files.py` & `mltb2-0.4.3/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/tests/test_openai.py` & `mltb2-0.4.3/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/tests/test_optuna.py` & `mltb2-0.4.3/tests/test_optuna.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/tests/test_somajo.py` & `mltb2-0.4.3/tests/test_somajo.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/tests/test_somajo_transformers.py` & `mltb2-0.4.3/tests/test_somajo_transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.4.2/tests/test_transformers.py` & `mltb2-0.4.3/tests/test_transformers.py`

 * *Files identical despite different names*

