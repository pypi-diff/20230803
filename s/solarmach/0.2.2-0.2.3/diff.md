# Comparing `tmp/solarmach-0.2.2.tar.gz` & `tmp/solarmach-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarmach-0.2.2.tar", last modified: Fri May 26 10:24:46 2023, max compression
+gzip compressed data, was "solarmach-0.2.3.tar", last modified: Thu Aug  3 11:35:26 2023, max compression
```

## Comparing `solarmach-0.2.2.tar` & `solarmach-0.2.3.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-26 10:24:46.044977 solarmach-0.2.2/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.2.2/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-01-10 16:26:49.000000 solarmach-0.2.2/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6700 2023-05-26 10:24:46.044977 solarmach-0.2.2/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     5851 2023-05-25 11:54:23.000000 solarmach-0.2.2/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:50:45.000000 solarmach-0.2.2/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-26 10:24:46.032977 solarmach-0.2.2/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solarmach-0.2.2/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2300 2022-03-14 11:55:52.000000 solarmach-0.2.2/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      300 2022-03-14 11:56:45.000000 solarmach-0.2.2/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solarmach-0.2.2/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-26 10:24:46.036977 solarmach-0.2.2/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)  1915936 2023-04-27 13:41:04.000000 solarmach-0.2.2/examples/example.ipynb
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   348683 2022-03-14 16:09:27.000000 solarmach-0.2.2/examples/solarmach.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-26 10:24:46.040977 solarmach-0.2.2/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.2.2/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solarmach-0.2.2/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-01-10 16:26:49.000000 solarmach-0.2.2/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      106 2023-05-12 08:03:40.000000 solarmach-0.2.2/requirements.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2127 2023-05-26 10:24:46.044977 solarmach-0.2.2/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      660 2022-03-14 12:48:51.000000 solarmach-0.2.2/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-26 10:24:46.040977 solarmach-0.2.2/solarmach/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    53052 2023-05-26 09:06:15.000000 solarmach-0.2.2/solarmach/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    22465 2023-05-26 09:01:52.000000 solarmach-0.2.2/solarmach/pfss_utilities.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-26 10:24:46.044977 solarmach-0.2.2/solarmach/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solarmach-0.2.2/solarmach/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1695 2022-11-09 14:33:28.000000 solarmach-0.2.2/solarmach/tests/test.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-05-26 10:24:45.000000 solarmach-0.2.2/solarmach/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-26 10:24:46.044977 solarmach-0.2.2/solarmach.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6700 2023-05-26 10:24:45.000000 solarmach-0.2.2/solarmach.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      584 2023-05-26 10:24:46.000000 solarmach-0.2.2/solarmach.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-05-26 10:24:45.000000 solarmach-0.2.2/solarmach.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-03-17 17:20:48.000000 solarmach-0.2.2/solarmach.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      191 2023-05-26 10:24:45.000000 solarmach-0.2.2/solarmach.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       10 2023-05-26 10:24:45.000000 solarmach-0.2.2/solarmach.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1292 2022-03-14 12:48:29.000000 solarmach-0.2.2/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-08-03 11:35:26.099021 solarmach-0.2.3/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.2.3/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-01-10 16:26:49.000000 solarmach-0.2.3/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     7090 2023-08-03 11:35:26.099021 solarmach-0.2.3/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6241 2023-07-27 13:04:02.000000 solarmach-0.2.3/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:50:45.000000 solarmach-0.2.3/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-08-03 11:35:26.051050 solarmach-0.2.3/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2023-07-25 12:11:02.000000 solarmach-0.2.3/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1274 2023-08-03 10:58:27.000000 solarmach-0.2.3/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2038 2023-07-26 13:50:27.000000 solarmach-0.2.3/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      324 2023-07-25 14:25:17.000000 solarmach-0.2.3/docs/installation.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      800 2023-07-25 12:11:02.000000 solarmach-0.2.3/docs/make.bat
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       85 2023-07-26 13:33:43.000000 solarmach-0.2.3/docs/requirements.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      207 2023-08-03 11:23:14.000000 solarmach-0.2.3/docs/solarmach.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       43 2023-07-26 13:04:10.000000 solarmach-0.2.3/docs/usage.nblink
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-08-03 11:35:26.083031 solarmach-0.2.3/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)  4340086 2023-08-03 08:33:25.000000 solarmach-0.2.3/examples/example.ipynb
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   348683 2022-03-14 16:09:27.000000 solarmach-0.2.3/examples/solarmach.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-08-03 11:35:26.087028 solarmach-0.2.3/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.2.3/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solarmach-0.2.3/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      133 2023-07-25 15:09:54.000000 solarmach-0.2.3/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      121 2023-08-02 13:15:36.000000 solarmach-0.2.3/requirements.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2024 2023-08-03 11:35:26.103018 solarmach-0.2.3/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      660 2022-03-14 12:48:51.000000 solarmach-0.2.3/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-08-03 11:35:26.091026 solarmach-0.2.3/solarmach/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    69993 2023-08-03 11:32:12.000000 solarmach-0.2.3/solarmach/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    22579 2023-07-25 12:53:03.000000 solarmach-0.2.3/solarmach/pfss_utilities.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-08-03 11:35:26.099021 solarmach-0.2.3/solarmach/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solarmach-0.2.3/solarmach/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1801 2023-07-31 13:46:56.000000 solarmach-0.2.3/solarmach/tests/test.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-08-03 11:35:25.000000 solarmach-0.2.3/solarmach/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-08-03 11:35:26.099021 solarmach-0.2.3/solarmach.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     7090 2023-08-03 11:35:25.000000 solarmach-0.2.3/solarmach.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      665 2023-08-03 11:35:26.000000 solarmach-0.2.3/solarmach.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-08-03 11:35:25.000000 solarmach-0.2.3/solarmach.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-03-17 17:20:48.000000 solarmach-0.2.3/solarmach.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      232 2023-08-03 11:35:25.000000 solarmach-0.2.3/solarmach.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       10 2023-08-03 11:35:25.000000 solarmach-0.2.3/solarmach.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1292 2022-03-14 12:48:29.000000 solarmach-0.2.3/tox.ini
```

### Comparing `solarmach-0.2.2/LICENSE.rst` & `solarmach-0.2.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.2/PKG-INFO` & `solarmach-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarmach
-Version: 0.2.2
+Version: 0.2.3
 Summary: Multi-spacecraft longitudinal configuration plotter
 Home-page: https://github.com/jgieseler/solarmach
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -12,33 +12,37 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
 solarmach
 =========
 
-|pypi Version| |conda version| |license| |python version| |pytest| |zenodo|
+|pypi Version| |conda version| |python version| |pytest| |codecov| |docs| |license| |zenodo|
 
 .. |pypi Version| image:: https://img.shields.io/pypi/v/solarmach?style=flat&logo=pypi
    :target: https://pypi.org/project/solarmach/
 .. |conda version| image:: https://img.shields.io/conda/vn/conda-forge/solarmach?style=flat&logo=anaconda
    :target: https://anaconda.org/conda-forge/solarmach/
-.. |license| image:: https://img.shields.io/conda/l/conda-forge/solarmach?style=flat
-   :target: https://github.com/jgieseler/solarmach/blob/main/LICENSE.rst
 .. |python version| image:: https://img.shields.io/pypi/pyversions/solarmach?style=flat&logo=python
 .. |pytest| image:: https://github.com/jgieseler/solarmach/workflows/pytest/badge.svg
+.. |codecov| image:: https://codecov.io/gh/jgieseler/solarmach/branch/main/graph/badge.svg?token=CT2P8AQU3B
+   :target: https://codecov.io/gh/jgieseler/solarmach
+.. |docs| image:: https://readthedocs.org/projects/solarmach/badge/?version=latest
+   :target: https://solarmach.readthedocs.io/en/latest/?badge=latest
+.. |license| image:: https://img.shields.io/conda/l/conda-forge/solarmach?style=flat
+   :target: https://github.com/jgieseler/solarmach/blob/main/LICENSE.rst
 .. |zenodo| image:: https://zenodo.org/badge/469735286.svg
    :target: https://zenodo.org/badge/latestdoi/469735286
 
 
 
 The Solar MAgnetic Connection Haus (Solar-MACH) tool is a multi-spacecraft longitudinal configuration plotter. This is the repository of the pip/conda package of Solar-MACH, called **solarmach**. For the corresponding streamlit repository, which is used for `solar-mach.github.io <https://solar-mach.github.io>`_, see `github.com/jgieseler/Solar-MACH <https://github.com/jgieseler/Solar-MACH>`_.
 
@@ -104,15 +108,19 @@
    
    # obtain data as Pandas DataFrame
    display(sm.coord_table)
 
 .. image:: https://github.com/jgieseler/solarmach/raw/main/examples/solarmach.png
   :alt: Example output figure
   
-See example notebooks in next section for all options!
+
+Documentation
+-------------
+Full documentation for the package can be found at https://solarmach.readthedocs.io
+
   
 Example Notebooks
 -----------------
 
 **solarmach** can easily be run in a Jupyter Notebook. 
 
 - `Show simple example notebook <https://nbviewer.org/github/jgieseler/solarmach/blob/main/examples/example.ipynb>`_ |nbviewer1|
```

### Comparing `solarmach-0.2.2/README.rst` & `solarmach-0.2.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 solarmach
 =========
 
-|pypi Version| |conda version| |license| |python version| |pytest| |zenodo|
+|pypi Version| |conda version| |python version| |pytest| |codecov| |docs| |license| |zenodo|
 
 .. |pypi Version| image:: https://img.shields.io/pypi/v/solarmach?style=flat&logo=pypi
    :target: https://pypi.org/project/solarmach/
 .. |conda version| image:: https://img.shields.io/conda/vn/conda-forge/solarmach?style=flat&logo=anaconda
    :target: https://anaconda.org/conda-forge/solarmach/
-.. |license| image:: https://img.shields.io/conda/l/conda-forge/solarmach?style=flat
-   :target: https://github.com/jgieseler/solarmach/blob/main/LICENSE.rst
 .. |python version| image:: https://img.shields.io/pypi/pyversions/solarmach?style=flat&logo=python
 .. |pytest| image:: https://github.com/jgieseler/solarmach/workflows/pytest/badge.svg
+.. |codecov| image:: https://codecov.io/gh/jgieseler/solarmach/branch/main/graph/badge.svg?token=CT2P8AQU3B
+   :target: https://codecov.io/gh/jgieseler/solarmach
+.. |docs| image:: https://readthedocs.org/projects/solarmach/badge/?version=latest
+   :target: https://solarmach.readthedocs.io/en/latest/?badge=latest
+.. |license| image:: https://img.shields.io/conda/l/conda-forge/solarmach?style=flat
+   :target: https://github.com/jgieseler/solarmach/blob/main/LICENSE.rst
 .. |zenodo| image:: https://zenodo.org/badge/469735286.svg
    :target: https://zenodo.org/badge/latestdoi/469735286
 
 
 
 The Solar MAgnetic Connection Haus (Solar-MACH) tool is a multi-spacecraft longitudinal configuration plotter. This is the repository of the pip/conda package of Solar-MACH, called **solarmach**. For the corresponding streamlit repository, which is used for `solar-mach.github.io <https://solar-mach.github.io>`_, see `github.com/jgieseler/Solar-MACH <https://github.com/jgieseler/Solar-MACH>`_.
 
@@ -80,15 +84,19 @@
    
    # obtain data as Pandas DataFrame
    display(sm.coord_table)
 
 .. image:: https://github.com/jgieseler/solarmach/raw/main/examples/solarmach.png
   :alt: Example output figure
   
-See example notebooks in next section for all options!
+
+Documentation
+-------------
+Full documentation for the package can be found at https://solarmach.readthedocs.io
+
   
 Example Notebooks
 -----------------
 
 **solarmach** can easily be run in a Jupyter Notebook. 
 
 - `Show simple example notebook <https://nbviewer.org/github/jgieseler/solarmach/blob/main/examples/example.ipynb>`_ |nbviewer1|
```

### Comparing `solarmach-0.2.2/code_of_conduct.md` & `solarmach-0.2.3/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.2/docs/Makefile` & `solarmach-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.2/examples/solarmach.png` & `solarmach-0.2.3/examples/solarmach.png`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.2/licenses/LICENSE.rst` & `solarmach-0.2.3/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.2/licenses/TEMPLATE_LICENSE.rst` & `solarmach-0.2.3/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.2/setup.cfg` & `solarmach-0.2.3/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -19,68 +19,66 @@
 	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 zip_safe = False
 packages = find:
 include_package_data = True
-python_requires = >=3.6
+python_requires = >=3.7
 setup_requires = setuptools_scm
 install_requires = 
 	astropy
 	astroquery
 	cmasher
 	drms
+	imageio
 	Jinja2
 	lxml
 	matplotlib==3.5.3
 	numpy
 	pandas
 	pfsspy
 	plotly
 	scipy
+	speasy
 	sunpy
 	zeep
 
 [options.extras_require]
 all = 
 test = 
 	pytest
 	pytest-doctestplus
 	pytest-cov
 docs = 
 	sphinx
 	sphinx-automodapi
+	numpydoc
+	sphinx_rtd_theme
 
 [tool:pytest]
 testpaths = "solarmach" "docs"
 doctest_plus = enabled
 text_file_format = rst
 addopts = --doctest-rst
 python_files = 
 	test_*.py
 	*_test.py
 	test.py
 	tests.py
 
 [coverage:run]
 omit = 
-	solarmach/__init*
-	solarmach/conftest.py
-	solarmach/*setup_package*
+	solarmach/setup*
 	solarmach/tests/*
 	solarmach/*/tests/*
-	solarmach/extern/*
 	solarmach/version*
-	*/solarmach/__init*
-	*/solarmach/conftest.py
-	*/solarmach/*setup_package*
+	*/solarmach/setup*
 	*/solarmach/tests/*
 	*/solarmach/*/tests/*
-	*/solarmach/extern/*
 	*/solarmach/version*
 
 [coverage:report]
 exclude_lines = 
 	pragma: no cover
 	except ImportError
 	raise AssertionError
```

### Comparing `solarmach-0.2.2/setup.py` & `solarmach-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.2/solarmach/__init__.py` & `solarmach-0.2.3/solarmach/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 
 from pkg_resources import get_distribution, DistributionNotFound
 try:
     __version__ = get_distribution(__name__).version
 except DistributionNotFound:
     pass  # package is not installed
 
+import copy
+import dateutil.parser
 import math
-from copy import deepcopy
 
 import astropy.constants as aconst
 import astropy.units as u
+import datetime as dt
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import matplotlib.text
 import numpy as np
 import pandas as pd
 import scipy.constants as const
+import speasy as spz
 from astropy.coordinates import SkyCoord
 from matplotlib.legend_handler import HandlerPatch
 from sunpy import log
 from sunpy.coordinates import frames, get_horizons_coord
 
 from solarmach.pfss_utilities import calculate_pfss_solution, get_field_line_coords, get_gong_map, multicolorline, sphere, spheric2cartesian, vary_flines
 
@@ -28,95 +31,174 @@
 # pd.options.display.float_format = '{:.1f}'.format
 # if needed, rather use the following to have the desired display:
 """
 with pd.option_context('display.float_format', '{:0.2f}'.format):
     display(df)
 """
 
-
 # initialize the body dictionary
-body_dict = dict.fromkeys(['Mercury', 199], [199, 'Mercury', 'darkturquoise'])
-body_dict.update(dict.fromkeys(['Venus', 299], [299, 'Venus', 'darkorchid']))
-body_dict.update(dict.fromkeys(['Earth', 'EARTH', 'earth', 399], [399, 'Earth', 'green']))
-body_dict.update(dict.fromkeys(['Mars', 499], [499, 'Mars', 'maroon']))
+body_dict = dict.fromkeys(['Earth', 'EARTH', 'earth', 399], [399, 'Earth', 'green'])
+body_dict.update(dict.fromkeys(['ACE', 'ace', 'Advanced Composition Explorer', -92], [-92, 'ACE', 'dimgrey']))
+body_dict.update(dict.fromkeys(['BepiColombo', 'Bepi Colombo', 'Bepi', 'MPO', -121], [-121, 'BepiColombo', 'orange']))
+body_dict.update(dict.fromkeys(['Cassini', -82], [-82, 'Cassini', 'mediumvioletred']))
+body_dict.update(dict.fromkeys(['JUICE', 'Juice', -28], [-28, 'JUICE', 'violet']))
+body_dict.update(dict.fromkeys(['Juno', 'JUNO', -61], [-61, 'Juno', 'orangered']))
 body_dict.update(dict.fromkeys(['Jupiter', 599], [599, 'Jupiter', 'navy']))
-
 body_dict.update(dict.fromkeys(['L1', 31], [31, 'SEMB-L1', 'black']))
-body_dict.update(dict.fromkeys(['ACE', 'Advanced Composition Explorer', -92], [-92, 'ACE', 'dimgrey']))
-
-body_dict.update(dict.fromkeys(['STEREO B', 'STEREO-B', 'STB', 'stb', -235], [-235, 'STEREO B', 'b']))
-body_dict.update(dict.fromkeys(['STEREO A', 'STEREO-A', 'STA', 'sta', -234], [-234, 'STEREO A', 'red']))
-body_dict.update(dict.fromkeys(['SOHO', 'soho', -21], [-21, 'SOHO', 'darkgreen']))
-body_dict.update(dict.fromkeys(['Solar Orbiter', 'SolO', 'solarorbiter', 'SolarOrbiter', -144], [-144, 'Solar Orbiter', 'dodgerblue']))
-body_dict.update(dict.fromkeys(['PSP', 'Parker Solar Probe', 'parkersolarprobe', 'ParkerSolarProbe', -96], [-96, 'Parker Solar Probe', 'purple']))
-body_dict.update(dict.fromkeys(['BepiColombo', 'Bepi Colombo', 'Bepi', 'MPO', -121], [-121, 'BepiColombo', 'orange']))
-body_dict.update(dict.fromkeys(['MAVEN', -202], [-202, 'MAVEN', 'brown']))
+body_dict.update(dict.fromkeys(['Mars', 499], [499, 'Mars', 'maroon']))
 body_dict.update(dict.fromkeys(['Mars Express', -41], [-41, 'Mars Express', 'darkorange']))
-body_dict.update(dict.fromkeys(['MESSENGER', -236], [-236, 'MESSENGER', 'olivedrab']))
-body_dict.update(dict.fromkeys(['JUICE', -28], [-28, 'JUICE', 'violet']))
-body_dict.update(dict.fromkeys(['Juno', -61], [-61, 'Juno', 'orangered']))
-body_dict.update(dict.fromkeys(['Cassini', -82], [-82, 'Cassini', 'mediumvioletred']))
+body_dict.update(dict.fromkeys(['MAVEN', 'Maven', -202], [-202, 'MAVEN', 'brown']))
+body_dict.update(dict.fromkeys(['Mercury', 199], [199, 'Mercury', 'darkturquoise']))
+body_dict.update(dict.fromkeys(['MESSENGER', 'Messenger', -236], [-236, 'MESSENGER', 'olivedrab']))
+body_dict.update(dict.fromkeys(['PSP', 'Parker Solar Probe', 'parkersolarprobe', 'ParkerSolarProbe', -96], [-96, 'Parker Solar Probe', 'purple']))
+body_dict.update(dict.fromkeys(['Pioneer10', 'Pioneer 10', -23], [-23, 'Pioneer 10', 'teal']))
+body_dict.update(dict.fromkeys(['Pioneer11', 'Pioneer 11', -24], [-24, 'Pioneer 11', 'darkblue']))
 body_dict.update(dict.fromkeys(['Rosetta', -226], [-226, 'Rosetta', 'blueviolet']))
-body_dict.update(dict.fromkeys(['Pioneer10', -23], [-23, 'Pioneer 10', 'teal']))
-body_dict.update(dict.fromkeys(['Pioneer11', -24], [-24, 'Pioneer 11', 'darkblue']))
+body_dict.update(dict.fromkeys(['SOHO', 'soho', 'SoHO', -21], [-21, 'SOHO', 'darkgreen']))
+body_dict.update(dict.fromkeys(['Solar Orbiter', 'SolO', 'solo', 'SOLO', 'solarorbiter', 'SolarOrbiter', -144], [-144, 'Solar Orbiter', 'dodgerblue']))
+body_dict.update(dict.fromkeys(['STEREO B', 'STEREO-B', 'STB', 'stb', -235], [-235, 'STEREO B', 'blue']))
+body_dict.update(dict.fromkeys(['STEREO A', 'STEREO-A', 'STA', 'sta', -234], [-234, 'STEREO A', 'red']))
 body_dict.update(dict.fromkeys(['Ulysses', -55], [-55, 'Ulysses', 'dimgray']))
-body_dict.update(dict.fromkeys(['Voyager1', -31], [-31, 'Voyager 1', 'darkred']))
-body_dict.update(dict.fromkeys(['Voyager2', -32], [-32, 'Voyager 2', 'midnightblue']))
+body_dict.update(dict.fromkeys(['Venus', 299], [299, 'Venus', 'darkorchid']))
+body_dict.update(dict.fromkeys(['Voyager1', 'Voyager 1', -31], [-31, 'Voyager 1', 'darkred']))
+body_dict.update(dict.fromkeys(['Voyager2', 'Voyager 2', -32], [-32, 'Voyager 2', 'midnightblue']))
+body_dict.update(dict.fromkeys(['WIND', 'Wind', 'wind', -8], [-8, 'Wind', 'slategray']))
 
 
 def print_body_list():
     """
-    prints a selection of body keys and the corresponding body names which may be provided to the
-    SolarMACH class
+    Prints a selection of body keys and the corresponding body names which may
+    be provided to the SolarMACH class.
+    Visit https://ssd.jpl.nasa.gov/horizons/app.html for a complete list of
+    available bodies.
     """
-    # print('Please visit https://ssd.jpl.nasa.gov/horizons.cgi?s_target=1#top for a complete list of available bodies')
     data = pd.DataFrame\
         .from_dict(body_dict, orient='index', columns=['ID', 'Body', 'Color'])\
         .drop(columns=['ID', 'Color'])\
         .drop_duplicates()
     data.index.name = 'Key'
     return data
 
 
+def get_sw_speed(body, dtime, trange=1, default_vsw=400.0):
+    """
+    Obtains measured solar wind bulk speed. Downloads solar wind speed
+    measurements for "body" from "trange" hours before "dtime" until "trange"
+    hours after "dtime", then calculates 1-hour mean values, and finally
+    returns that 1-hour mean measurements that is closest to "dtime".
+
+    Parameters
+    ----------
+    body : str
+        Name of body, e.g., planet or spacecraft
+    dtime : datetime object or datetime-compatible str
+        Date and time of measurement
+    trange : int of float
+        Timedelta for which measurements are obtainted before and after "dtime",
+        i.e. dtime +- trange (in hours). Default value 2.
+    default_vsw : float
+        Default solar wind bulk speed in km/s that is returned if no
+        measurements can be obtained. Default value 400.0
+
+    Returns
+    -------
+    float
+        solar wind bulk speed in km/s
+    """
+    try:
+        # standardize body name (e.g. 'PSP' => 'Parker Solar Probe')
+        body = body_dict[body][1]
+    except KeyError:
+        pass
+
+    amda_tree = spz.inventories.data_tree.amda
+    cda_tree = spz.inventories.data_tree.cda
+
+    dataset = dict(ACE=cda_tree.ACE.SWE.AC_K1_SWE.Vp)  # https://cdaweb.gsfc.nasa.gov/misc/NotesA.html#AC_K1_SWE
+    dataset['SOHO'] = cda_tree.SOHO.CELIAS_PM.SOHO_CELIAS_PM_5MIN.V_p
+    dataset['Parker Solar Probe'] = amda_tree.Parameters.PSP.SWEAP_SPC.psp_spc_mom.psp_spc_vp_mom_nrm
+    dataset['Solar Orbiter'] = amda_tree.Parameters.SolarOrbiter.PAS.L2.so_pas_momgr1.pas_momgr1_v_rtn_tot
+    dataset['STEREO A'] = amda_tree.Parameters.STEREO.STEREO_A.PLASTIC.sta_l2_pla.vpbulk_sta
+    dataset['STEREO B'] = amda_tree.Parameters.STEREO.STEREO_B.PLASTIC.stb_l2_pla.vpbulk_stb
+    dataset['Wind'] = amda_tree.Parameters.Wind.SWE.wnd_swe_kp.wnd_swe_vmag
+
+    sw_key = dict(ACE='SW Bulk Speed')  # Solar Wind Bulk Speed [Vp]
+    sw_key['Parker Solar Probe'] = 'psp_spc_vp_mom_nrm'  # Velocity vector magnitude
+    sw_key['SOHO'] = 'Proton V' # Proton speed, scalar
+    sw_key['Solar Orbiter'] = 'pas_momgr1_v_rtn_tot'  # Velocity magnitude in RTN frame
+    sw_key['STEREO A'] = 'vpbulk_sta'  # Scalar magnitude of the velocity in km/s
+    sw_key['STEREO B'] = 'vpbulk_stb'  # Scalar magnitude of the velocity in km/s
+    sw_key['Wind'] = 'wnd_swe_vmag'  # |v|
+
+    if body in ['Earth', 'SEMB-L1']:
+        print(f"Using 'ACE' measurements for '{body}'.")
+        body = 'ACE'
+    elif body not in dataset.keys():
+        print(f"Body '{body}' not supported, assuming default Vsw value of 400 km/s.")
+        return default_vsw
+
+    if type(dtime) == str:
+        try:
+            dtime = dateutil.parser.parse(dtime)
+        except dateutil.parser.ParserError:
+            print(f"Unable to extract datetime from '{dtime}'. Assuming default Vsw value of 400 km/s.")
+            return default_vsw
+
+    try:
+        df = spz.get_data(dataset[body], dtime-dt.timedelta(hours=trange), dtime+dt.timedelta(hours=trange)).to_dataframe()
+        df = df[sw_key[body]].resample('1H').mean()
+        if len(df) > 0:
+            idx = df[df.index.get_indexer([dtime], method='nearest')]
+            return idx.values[0]
+        else:
+            print(f"No Vsw data found for '{body}' on {dtime}, assuming default Vsw value of 400 km/s.")
+            return default_vsw
+    except AttributeError:
+        print(f"No Vsw data found for '{body}' on {dtime}, assuming default Vsw value of 400 km/s.")
+        return default_vsw
+
+
 class SolarMACH():
     """
-    Class which handles the selected bodies
+    Class handling selected bodies
 
     Parameters
     ----------
     date: str
     body_list: list
         list of body keys to be used. Keys can be string of int.
     vsw_list: list, optional
-        list of solar wind speeds at the position of the different bodies. Must have the same length as body_list.
-        Default is an epmty list leading to vsw=400km/s used for every body.
+        list of solar wind bulk speeds in km/s at the position of the different bodies. Must have the same length as body_list.
+        If empty list, obtaining actual measurements is tried. If this is not successful, a default value defined by default_vsw is used.
+    default_vsw: int or float, optional
+        Solar wind bulk speed in km/s to be used if vsw_list is not defined and no vsw measurements could be obtained. By default 400.0.
     coord_sys: string, optional
         Defines the coordinate system used: 'Carrington' (default) or 'Stonyhurst'
     reference_long: float, optional
         Longitute of reference position at the Sun
     reference_lat: float, optional
         Latitude of referene position at the Sun
     """
 
-    def __init__(self, date, body_list, vsw_list=[], reference_long=None, reference_lat=None, coord_sys='Carrington', **kwargs):
+    def __init__(self, date, body_list, vsw_list=[], reference_long=None, reference_lat=None, coord_sys='Carrington', default_vsw=400.0, **kwargs):
         if 'diff_rot' in kwargs.keys():
             self.diff_rot = kwargs['diff_rot']
         else:
             self.diff_rot = True
         if 'target_solar_radius' in kwargs.keys():
             self.target_solar_radius = kwargs['target_solar_radius']
         else:
             self.target_solar_radius = 1
 
         # get initial sunpy logging level and disable unnecessary logging
         initial_log_level = log.getEffectiveLevel()
         log.setLevel('WARNING')
 
         body_list = list(dict.fromkeys(body_list))
-        bodies = deepcopy(body_dict)
+        bodies = copy.deepcopy(body_dict)
 
         if coord_sys.lower().startswith('car'):
             coord_sys = 'Carrington'
         if coord_sys.lower().startswith('sto') or coord_sys.lower() == 'Earth':
             coord_sys = 'Stonyhurst'
 
         self.date = date
@@ -126,16 +208,22 @@
 
         pos_E = get_horizons_coord(399, self.date, None)  # (lon, lat, radius) in (deg, deg, AU)
         if coord_sys=='Carrington':
             self.pos_E = pos_E.transform_to(frames.HeliographicCarrington(observer='Sun'))
         elif coord_sys=='Stonyhurst':
             self.pos_E = pos_E
 
-        if len(vsw_list) == 0:
-            vsw_list = np.zeros(len(body_list)) + 400
+        # make deep copy of vsw_list bc. otherwise it doesn't get reset in a new init:
+        vsw_list2 = copy.deepcopy(vsw_list)
+
+        if len(vsw_list2) == 0:
+            print('No solar wind speeds defined, trying to obtain measurements...')
+            for body in body_list:
+                vsw_list2.append(get_sw_speed(body, date, default_vsw))
+            # vsw_list = np.zeros(len(body_list)) + 400
 
         random_cols = ['forestgreen', 'mediumblue', 'm', 'saddlebrown', 'tomato', 'olive', 'steelblue', 'darkmagenta',
                        'c', 'darkslategray', 'yellow', 'darkolivegreen']
         body_lon_list = []
         body_lat_list = []
         body_dist_list = []
         longsep_E_list = []
@@ -159,30 +247,30 @@
                 bodies.update(dict.fromkeys([body_id], [body_id, body_lab, body_color]))
 
             try:
                 pos = get_horizons_coord(body_id, date, None)  # (lon, lat, radius) in (deg, deg, AU)
                 if coord_sys=='Carrington':
                     pos = pos.transform_to(frames.HeliographicCarrington(observer='Sun'))
                 bodies[body_id].append(pos)
-                bodies[body_id].append(vsw_list[i])
+                bodies[body_id].append(vsw_list2[i])
 
                 longsep_E = pos.lon.value - self.pos_E.lon.value
                 if longsep_E > 180:
                     longsep_E = longsep_E - 360.
                 latsep_E = pos.lat.value - self.pos_E.lat.value
 
                 body_lon_list.append(pos.lon.value)
                 body_lat_list.append(pos.lat.value)
                 body_dist_list.append(pos.radius.value)
                 longsep_E_list.append(longsep_E)
                 latsep_E_list.append(latsep_E)
 
-                body_vsw_list.append(vsw_list[i])
+                body_vsw_list.append(vsw_list2[i])
 
-                sep, alpha = self.backmapping(pos, reference_long, target_solar_radius=self.target_solar_radius, vsw=vsw_list[i])
+                sep, alpha = self.backmapping(pos, reference_long, target_solar_radius=self.target_solar_radius, vsw=vsw_list2[i])
                 bodies[body_id].append(sep)
 
                 body_footp_long = pos.lon.value + alpha
                 if body_footp_long > 360:
                     body_footp_long = body_footp_long - 360
                 footp_long_list.append(body_footp_long)
 
@@ -226,28 +314,29 @@
         self.coord_table.style.set_properties(**{'text-align': 'left'})
 
         # reset sunpy log level to initial state
         log.setLevel(initial_log_level)
 
     def backmapping(self, body_pos, reference_long, target_solar_radius=1, vsw=400):
         """
-        Determine the longitudinal separation angle of a given spacecraft and a given reference longitude
+        Determine the longitudinal separation angle of a given body and a given reference longitude
 
         Parameters
         ----------
         body_pos : astropy.coordinates.sky_coordinate.SkyCoord
             coordinates of the body
         reference_long: float
             Longitude of reference point at Sun to which we determine the longitudinal separation
         target_solar_radius: float
             Target solar radius to which to be backmapped. 0 corresponds to Sun's center, 1 to 1 solar radius, and e.g. 2.5 to the source surface.
         vsw: float
              solar wind speed (km/s) used to determine the position of the magnetic footpoint of the body. Default is 400.
 
-        out:
+        Returns
+        -------
             sep: float
                 longitudinal separation of body magnetic footpoint and reference longitude in degrees
             alpha: float
                 backmapping angle
         """
         # AU = const.au / 1000  # km
 
@@ -309,15 +398,22 @@
              long_offset=270,
              outfile='',
              figsize=(12, 8),
              dpi=200,
              long_sector=None,
              long_sector_vsw=None,
              long_sector_color='red',
-             background_spirals=None):
+             long_sector_alpha=0.5,
+             background_spirals=None,
+             test_plotly=False,
+             test_plotly_template='plotly',
+             # x_offset=0.0,  # TODO: remove this option.
+             # y_offset=0.0, # TODO: remove this option.
+             test_plotly_legend=(1.0, 1.0),
+             test_plotly_logo=(1.0, 0.0)):
         """
         Make a polar plot showing the Sun in the center (view from North) and the positions of the selected bodies
 
         Parameters
         ----------
         plot_spirals: bool
             if True, the magnetic field lines connecting the bodies with the Sun are plotted
@@ -339,14 +435,16 @@
             if provided, the plot is saved with outfile as filename
         long_sector: list of 2 numbers, optional
             Start and stop longitude of a shaded area; e.g. [350, 20] to get a cone from 350 to 20 degree longitude (for long_sector_vsw=None).
         long_sector_vsw: list of 2 numbers, optional
             Solar wind speed used to calculate Parker spirals (at start and stop longitude provided by long_sector) between which a reference cone should be drawn; e.g. [400, 400] to assume for both edges of the fill area a Parker spiral produced by solar wind speeds of 400 km/s. If None, instead of Parker spirals straight lines are used, i.e. a simple cone wil be plotted. By default None.
         long_sector_color: string, optional
             String defining the matplotlib color used for the shading defined by long_sector. By default 'red'.
+        long_sector_alpha: float, optional
+            Float between 0.0 and 1.0, defining the matplotlib alpha used for the shading defined by long_sector. By default 0.5.W
         background_spirals: list of 2 numbers (and 3 optional strings), optional
             If defined, plot evenly distributed Parker spirals over 360°. background_spirals[0] defines the number of spirals, background_spirals[1] the solar wind speed in km/s used for their calculation. background_spirals[2], background_spirals[3], and background_spirals[4] optionally change the plotting line style, color, and alpha setting, respectively (default values ':', 'grey', and 0.1). Full example that plots 12 spirals (i.e., every 30°) using a solar wind speed of 400 km/s with solid red lines with alpha=0.2: background_spirals=[12, 400, '-', 'red', 0.2]
         """
         hide_logo = False  # optional later keyword to hide logo on figure
         AU = const.au / 1000  # km
 
         # save inital rcParams and update some of them:
@@ -361,14 +459,18 @@
         # build array of values for radius (in spherical coordinates!) given in AU!
         r_array = np.arange(0.007, (self.max_dist+0.1)/np.cos(np.deg2rad(self.max_dist_lat)) + 3.0, 0.001)
         # take into account solar differential rotation wrt. latitude. Thus move calculation of omega to the per-body section below
         # omega = np.radians(360. / (25.38 * 24 * 60 * 60))  # solar rot-angle in rad/sec, sidereal period
 
         E_long = self.pos_E.lon.value
 
+        if test_plotly:
+            import plotly.graph_objects as go
+            pfig = go.Figure()
+
         for i, body_id in enumerate(self.body_dict):
             body_lab = self.body_dict[body_id][1]
             body_color = self.body_dict[body_id][2]
             body_vsw = self.body_dict[body_id][4]
             body_pos = self.body_dict[body_id][3]
 
             pos = body_pos
@@ -399,14 +501,53 @@
             if plot_spirals:
                 # tt = dist_body * AU / body_vsw
                 # alpha = np.degrees(omega * tt)
                 # alpha_body = np.deg2rad(body_long) + omega / (body_vsw / AU) * (dist_body - r_array)
                 alpha_body = np.deg2rad(body_long) + omega / (body_vsw / AU) * (dist_body - r_array) * np.cos(np.deg2rad(body_lat))
                 ax.plot(alpha_body, r_array * np.cos(np.deg2rad(body_lat)), color=body_color)
 
+            if test_plotly:
+                if plot_spirals:
+                    pfig.add_trace(go.Scatterpolar(
+                        r=r_array * np.cos(np.deg2rad(body_lat)),
+                        theta=alpha_body,
+                        mode='lines',
+                        name=f'{body_id} magnetic field line',
+                        showlegend=False,
+                        line=dict(color=body_dict[body_id][2]),
+                        thetaunit="radians"))
+
+                if plot_sun_body_line:
+                    pfig.add_trace(go.Scatterpolar(
+                        r=[0.01, dist_body*np.cos(np.deg2rad(body_lat))],
+                        theta=[np.deg2rad(body_long), np.deg2rad(body_long)],
+                        mode='lines',
+                        name=f'{body_id} direct line',
+                        showlegend=False,
+                        line=dict(color=body_dict[body_id][2], dash='dot'),
+                        thetaunit="radians"))
+
+                if numbered_markers:
+                    str_number = f'<b>{i+1}</b>'
+                else:
+                    str_number = None
+
+                pfig.add_trace(go.Scatterpolar(
+                    r=[dist_body*np.cos(np.deg2rad(body_lat))],
+                    theta=[np.deg2rad(body_long)],
+                    mode='markers+text',
+                    name=body_id,
+                    marker=dict(size=16, color=body_dict[body_id][2]),
+                    # text=[f'<b>{body_id}</b>'],
+                    # textposition="top center",
+                    text=[str_number],
+                    textfont=dict(color="white", size=14),
+                    textposition="middle center",
+                    thetaunit="radians"))
+
         if self.reference_long is not None:
             delta_ref = self.reference_long
             if delta_ref < 0.:
                 delta_ref = delta_ref + 360.
             if self.reference_lat is None:
                 ref_lat = 0.
             else:
@@ -424,24 +565,101 @@
             # ref_arr = plt.arrow(alpha_ref[0], 0.01, 0, arrow_dist, head_width=0.12, head_length=0.11, edgecolor='black',
             #                     facecolor='black', lw=2, zorder=5, overhang=0.2)
             arrow_dist = min([self.max_dist/3.2, 2.])
             # ref_arr = plt.arrow(alpha_ref[0], 0.01, 0, arrow_dist, head_width=0.2, head_length=0.07, edgecolor='black',
             #                     facecolor='black', lw=1.8, zorder=5, overhang=0.2)
             ref_arr = plt.arrow(np.deg2rad(delta_ref), 0.01, 0, arrow_dist, head_width=0.2, head_length=0.07, edgecolor='black',
                                 facecolor='black', lw=1.8, zorder=5, overhang=0.2)
-
+            if test_plotly:
+                if test_plotly_template=="plotly_dark":
+                    reference_color = "white"
+                else:
+                    reference_color = "black"
+                pfig.add_trace(go.Scatterpolar(
+                    r=[0.0, arrow_dist],
+                    theta=[np.deg2rad(delta_ref), np.deg2rad(delta_ref)],
+                    mode='lines+markers',
+                    marker=dict(symbol="arrow", size=15, angleref="previous", color=reference_color),
+                    name='reference long.',
+                    showlegend=True,
+                    line=dict(color=reference_color),
+                    thetaunit="radians"))
             if plot_spirals:
                 ax.plot(alpha_ref, r_array * np.cos(np.deg2rad(ref_lat)), '--k', label=f'field line connecting to\nref. long. (vsw={reference_vsw} km/s)')
+                if test_plotly:
+                    pfig.add_trace(go.Scatterpolar(
+                        r=r_array * np.cos(np.deg2rad(ref_lat)),
+                        theta=alpha_ref,
+                        mode='lines',
+                        name=f'field line connecting to<br>ref. long. (vsw={reference_vsw} km/s)',
+                        showlegend=True,
+                        line=dict(color=reference_color, dash="dash"),
+                        thetaunit="radians"))
+
+        if test_plotly:
+            if numbered_markers:
+                for i, body_id in enumerate(self.body_dict):
+                    if self.reference_long is not None:
+                        x_offset_ref = -0.035  # 0.004
+                        y_offset_ref = 0.081
+                        y_offset_per_i = -0.051
+                    else:
+                        x_offset_ref = 0.0
+                        y_offset_ref = 0.0
+                        y_offset_per_i = -0.0475
+                    x_offset = -0.11  # 0.05
+                    y_offset = 0.124  # -0.0064
+                    pfig.add_annotation(text=f'<b>{i+1}</b>', xref="paper", yref="paper", xanchor="center", yanchor="top",
+                                        x=test_plotly_legend[0]+x_offset+x_offset_ref, y=test_plotly_legend[1]+y_offset+y_offset_ref+y_offset_per_i*i,
+                                        showarrow=False, font=dict(color="white", size=14))
+
+            pfig.add_annotation(text='Solar-MACH', xref="paper", yref="paper",  # xanchor="center", yanchor="middle",
+                                x=test_plotly_logo[0], y=test_plotly_logo[1]+0.05,
+                                showarrow=False, font=dict(color="black", size=28, family='DejaVu Serif'), align="right")
+            pfig.add_annotation(text='https://solar-mach.github.io', xref="paper", yref="paper",  # xanchor="center", yanchor="middle",
+                                x=test_plotly_logo[0], y=test_plotly_logo[1],
+                                showarrow=False, font=dict(color="black", size=18, family='DejaVu Serif'), align="right")
+
+            # for template in ["plotly", "plotly_white", "plotly_dark", "ggplot2", "seaborn", "simple_white", "none"]:
+            if not test_plotly_template:
+                test_plotly_template = "plotly"
+            polar_rotation = (long_offset - E_long)
+            pfig.update_layout(template=test_plotly_template,
+                               polar=dict(radialaxis_range=[0, self.max_dist + 0.3], angularaxis_rotation=polar_rotation),
+                               modebar_add=["v1hovermode"],
+                               modebar_remove=["select2d", "lasso2d"],
+                               margin=dict(l=100, r=100, b=0, t=50),
+                               # paper_bgcolor="LightSteelBlue",
+                               legend=dict(yanchor="middle", y=test_plotly_legend[1], xanchor="center", x=test_plotly_legend[0]))
+            # fig.show()
+            # if using streamlit, send plot to streamlit output, else call plt.show()
+            if _isstreamlit():
+                import streamlit as st
+                # st.plotly_chart(pfig, theme="streamlit")
+                st.components.v1.html(pfig.to_html(include_mathjax='cdn'), height=500)
+            else:
+                pfig.show()
 
         if long_sector is not None:
-            if type(long_sector) == list and len(long_sector)==2:
-                delta_ref1 = long_sector[0]
+            if type(long_sector) == list and np.array(long_sector).ndim==1:
+                long_sector = [long_sector]
+                long_sector_vsw = [long_sector_vsw]
+                long_sector_color = [long_sector_color]
+                long_sector_alpha = [long_sector_alpha]
+            else:
+                print("Non-standard 'long_sector'. It should be a 2-element list defining the start and end longitude of the cone in degrees; e.g. 'long_sector=[15,45]'. 'long_sector_XXX' options have to follow accordingly.")
+            for i in range(len(long_sector)):
+                t_long_sector = long_sector[i]
+                t_long_sector_vsw = long_sector_vsw[i]
+                t_long_sector_color = long_sector_color[i]
+                t_long_sector_alpha = long_sector_alpha[i]
+                delta_ref1 = t_long_sector[0]
                 if delta_ref1 < 0.:
                     delta_ref1 = delta_ref1 + 360.
-                delta_ref2 = long_sector[1]
+                delta_ref2 = t_long_sector[1]
                 if delta_ref2 < 0.:
                     delta_ref2 = delta_ref2 + 360.
 
                 # Check that we are considering the same rotation
                 if delta_ref2 < delta_ref1:
                     delta_ref2 += 360
 
@@ -449,60 +667,58 @@
                 # take into account solar differential rotation wrt. latitude
                 omega_ref1 = self.solar_diff_rot(long_sector_lat[0])
                 omega_ref2 = self.solar_diff_rot(long_sector_lat[1])
 
                 # Build an r_array for the second spiral for while loop to iterate forwards
                 r_array2 = np.copy(r_array)
 
-                if long_sector_vsw is not None:
+                if t_long_sector_vsw is not None:
                     # Calculate the first spiral's angles along r
-                    alpha_ref1 = np.deg2rad(delta_ref1) + omega_ref1 / (long_sector_vsw[0] / AU) * (self.target_solar_radius*aconst.R_sun.to(u.AU).value - r_array) * np.cos(np.deg2rad(long_sector_lat[0]))
-                    alpha_ref2 = np.deg2rad(delta_ref2) + omega_ref2 / (long_sector_vsw[1] / AU) * (self.target_solar_radius*aconst.R_sun.to(u.AU).value - r_array2) * np.cos(np.deg2rad(long_sector_lat[1]))
+                    alpha_ref1 = np.deg2rad(delta_ref1) + omega_ref1 / (t_long_sector_vsw[0] / AU) * (self.target_solar_radius*aconst.R_sun.to(u.AU).value - r_array) * np.cos(np.deg2rad(long_sector_lat[0]))
+                    alpha_ref2 = np.deg2rad(delta_ref2) + omega_ref2 / (t_long_sector_vsw[1] / AU) * (self.target_solar_radius*aconst.R_sun.to(u.AU).value - r_array2) * np.cos(np.deg2rad(long_sector_lat[1]))
 
                     # Save the last angle as a starting point for reference for the while loop
                     alpha_init = alpha_ref2[-1]
 
                     # Check that reference angle of the first loop is ahead
                     if alpha_ref1[-1] > alpha_ref2[-1]:
                         alpha_ref1_comp = alpha_ref1[-1] - 2*np.pi
                     else:
                         alpha_ref1_comp = alpha_ref1[-1]
 
                     # While the second spiral is behind the first spiral in angle, extend the second spiral
                     while alpha_ref2[-1] > alpha_ref1_comp:
                         r_array2 = np.append(r_array2, r_array2[-1] + 0.1)
-                        alpha_ref2 = np.append(alpha_ref2, np.deg2rad(delta_ref2) + omega_ref2 / (long_sector_vsw[1] / AU) * (self.target_solar_radius*aconst.R_sun.to(u.AU).value - r_array2[-1]) * np.cos(np.deg2rad(long_sector_lat[1])))
+                        alpha_ref2 = np.append(alpha_ref2, np.deg2rad(delta_ref2) + omega_ref2 / (t_long_sector_vsw[1] / AU) * (self.target_solar_radius*aconst.R_sun.to(u.AU).value - r_array2[-1]) * np.cos(np.deg2rad(long_sector_lat[1])))
 
                     # Interpolate the first spiral's angles to the coarser second spiral's angles (outside the plot)
                     alpha_ref1 = np.interp(r_array2, r_array, alpha_ref1)
 
                 else:
                     # if no solar wind speeds for Parker spirals are provided, use straight lines:
                     alpha_ref1 = np.array([np.deg2rad(delta_ref1)] * len(r_array))
                     alpha_ref2 = np.array([np.deg2rad(delta_ref2)] * len(r_array))
 
-                c1 = plt.polar(alpha_ref1, r_array2 * np.cos(np.deg2rad(long_sector_lat[0])), lw=0, color=long_sector_color, alpha=0.5)[0]
+                c1 = plt.polar(alpha_ref1, r_array2 * np.cos(np.deg2rad(long_sector_lat[0])), lw=0, color=t_long_sector_color, alpha=t_long_sector_alpha)[0]
                 x1 = c1.get_xdata()
                 y1 = c1.get_ydata()
-                c2 = plt.polar(alpha_ref2, r_array2 * np.cos(np.deg2rad(long_sector_lat[1])), lw=0, color=long_sector_color, alpha=0.5)[0]
+                c2 = plt.polar(alpha_ref2, r_array2 * np.cos(np.deg2rad(long_sector_lat[1])), lw=0, color=t_long_sector_color, alpha=t_long_sector_alpha)[0]
                 x2 = c2.get_xdata()
                 y2 = c2.get_ydata()
 
                 # Check that plotted are is between the two spirals, and do not fill after potential crossing
                 clause1 = x1 < x2
                 clause2 = alpha_ref1[clause1] < alpha_ref2[clause1]
 
                 # Take only the points that fill the above clauses
                 y1_fill = y1[clause1][clause2]
                 x1_fill = x1[clause1][clause2]
                 x2_fill = x2[clause1][clause2]
 
-                plt.fill_betweenx(y1_fill, x1_fill, x2_fill, lw=0, color=long_sector_color, alpha=0.5)
-            else:
-                print("Ill-defined 'long_sector'. It should be a 2-element list defining the start and end longitude of the cone in degrees; e.g. 'long_sector=[15,45]'")
+                plt.fill_betweenx(y1_fill, x1_fill, x2_fill, lw=0, color=t_long_sector_color, alpha=t_long_sector_alpha)
 
         if background_spirals is not None:
             if type(background_spirals) == list and len(background_spirals)>=2:
                 # maybe later add option to have a non-zero latitude, so that the field lines are out of the ecliptic
                 background_spirals_lat = 0
                 # take into account solar differential rotation wrt. latitude
                 omega_ref = self.solar_diff_rot(background_spirals_lat)
@@ -617,15 +833,19 @@
         if _isstreamlit():
             import streamlit as st
             st.pyplot(fig)  # , dpi=200)
         else:
             plt.show()
 
         if return_plot_object:
-            return fig, ax
+            # TODO: not really straightforward; change in future
+            if not test_plotly:
+                return fig, ax
+            else:
+                return pfig
 
     def _polar_twin(self, ax, E_long, position, long_offset):
         """
         add an additional axes which is needed to plot additional longitudinal tickmarks with Earth at longitude 0
         not used any more!
         """
         ax2 = ax.figure.add_axes(position, projection='polar',
@@ -642,29 +862,29 @@
         ax2.set_theta_offset(np.deg2rad(long_offset - E_long))
         gridlines = ax2.xaxis.get_gridlines()
         for xax in gridlines:
             xax.set_color('darkgreen')
 
         return ax2
 
-    def plot_pfss(self,
+    def plot_pfss(self, 
                   rss=2.5,
-                  pfss_solution=None,
-                  figsize=(15, 10),
-                  dpi=200,
-                  return_plot_object=False,
+                  pfss_solution = None,
+                  figsize = (15,10),
+                  dpi = 200,
+                  return_plot_object = False,
                   vary=False, n_varies=1,
-                  long_offset=270,
-                  reference_vsw=400.,
-                  numbered_markers=False,
-                  plot_spirals=True,
-                  long_sector=None,
-                  long_sector_vsw=None,
-                  long_sector_color=None,
-                  hide_logo=False):
+                  long_offset = 270,
+                  reference_vsw = 400.,
+                  numbered_markers = False,
+                  plot_spirals = True,
+                  long_sector = None,
+                  long_sector_vsw = None,
+                  long_sector_color = None,
+                  hide_logo = False):
         """
         Produces a figure of the heliosphere in polar coordinates with logarithmic r-axis outside the pfss.
         Also tracks an open field line down to photosphere given a point on the pfss.
 
         rss : float
                 source surface height of the potential field in solar radii. default 2.5
         pfss_solution : .fits
@@ -673,17 +893,17 @@
                 draws an arrow pointing radially outward, input in degrees
 
         """
 
         if not pfss_solution:
             raise Exception("A PFSS solution is required for solar magnetic field extrapolation!")
 
-        # Constants
+        # Constants 
         AU = const.au / 1000  # km
-        sun_radius = aconst.R_sun.value  # meters
+        sun_radius = aconst.R_sun.value # meters
 
         # r_scaler scales distances from astronomical units to solar radii. unit = [solar radii / AU]
         r_scaler = (AU*1000)/sun_radius
 
         # carrington longitude of the Earth
         E_long = self.pos_E.lon.value
 
@@ -693,40 +913,36 @@
         plt.rcParams['font.size'] = 15
         plt.rcParams['agg.path.chunksize'] = 20000
 
         # init the figure and axes
         fig, ax = plt.subplots(subplot_kw=dict(projection='polar'), figsize=figsize, dpi=dpi)
 
         # maximum distance anything will be plotted
-        r_max = r_scaler * 5  # 5 AU in units of solar radii
+        r_max = r_scaler * 5 # 5 AU = 1075 in units of solar radii
 
         # setting the title
         ax.set_title(self.date + '\n', pad=30, fontsize=26)
 
         # Plot the source_surface and solar surface
         full_circle_radians = 2*np.pi*np.linspace(0, 1, 200)
         ax.plot(full_circle_radians, np.ones(200)*rss, c='k', ls='--', zorder=3)
         ax.plot(full_circle_radians, np.ones(200), c='darkorange', lw=2.5, zorder=1)
 
         # Plot the 30 and 60 deg lines on the Sun
-        ax.plot(full_circle_radians, np.ones(len(full_circle_radians))*0.866, c='darkgray', lw=1.5, ls=":", zorder=3)  # cos(30deg) = 0.866(O)
-        ax.plot(full_circle_radians, np.ones(len(full_circle_radians))*0.500, c='darkgray', lw=1.5, ls=":", zorder=3)  # cos(60deg) = 0.5(0)
+        ax.plot(full_circle_radians, np.ones(len(full_circle_radians))*0.866, c='darkgray', lw=1.5, ls=":", zorder=3) #cos(30deg) = 0.866(O)
+        ax.plot(full_circle_radians, np.ones(len(full_circle_radians))*0.500, c='darkgray', lw=1.5, ls=":", zorder=3) #cos(60deg) = 0.5(0)
 
         # Gather field line objects, photospheric footpoints and magnetic polarities in these lists
         # fieldlines is a class attribute, so that the field lines can be neasily 3D plotted with another method
         self.fieldlines = []
         photospheric_footpoints = []
         fieldline_polarities = []
 
-        # The radial coordinates for reference parker spiral
-        reference_array = np.linspace(r_max, rss, 1000)
-
-        #
-        # reference_array for cones -> normalize their parker spiral math
-        #
+        # The radial coordinates for reference parker spiral (plot even outside the figure boundaries to avert visual bugs)
+        reference_array = np.linspace(rss, r_max+200, int(1e3))
 
         for i, body_id in enumerate(self.body_dict):
 
             body_lab = self.body_dict[body_id][1]
             body_color = self.body_dict[body_id][2]
             body_vsw = self.body_dict[body_id][4]
             body_pos = self.body_dict[body_id][3]
@@ -735,15 +951,15 @@
             dist_body = pos.radius.value
 
             body_long = pos.lon.value
             body_lat = pos.lat.value
 
             # take into account solar differential rotation wrt. latitude
             omega = self.solar_diff_rot(body_lat)
-
+ 
             # The radial coordinates (outside source surface) for each object
             r_array = np.linspace(r_scaler*dist_body*np.cos(np.deg2rad(body_lat)), rss, 1000)
 
             # plot body positions
             if numbered_markers:
                 ax.plot(np.deg2rad(body_long), r_scaler*dist_body*np.cos(np.deg2rad(body_lat)), 'o', ms=15, color=body_color, label=body_lab)
                 ax.annotate(i+1, xy=(np.deg2rad(body_long), r_scaler*dist_body*np.cos(np.deg2rad(body_lat))), color='white',
@@ -757,19 +973,19 @@
             if plot_spirals:
 
                 # The angular coordinates are calculated here
                 # alpha = longitude + (omega)*(distance-r)/sw
                 alpha_body = np.deg2rad(body_long) + omega / (1000*body_vsw / sun_radius) * (r_scaler*dist_body - r_array) * np.cos(np.deg2rad(body_lat))
                 ax.plot(alpha_body, r_array * np.cos(np.deg2rad(body_lat)), color=body_color)
 
-            # acquire an array of (r,lon,lat) coordinates of the open field lines under the pfss
+            # Acquire an array of (r,lon,lat) coordinates of the open field lines under the pfss
             # based on the footpoint(s) of the sc
             if vary:
 
-                # Triplets contain 35 tuples of (r,lon,lat)
+                # Triplets contain 35 tuples of (r,lon,lat) 
                 fline_triplets, fline_objects, varyfline_triplets, varyfline_objects = vary_flines(alpha_body[-1], np.deg2rad(body_lat), pfss_solution, n_varies, rss)
 
                 # Collect field line objects to a list
                 self.fieldlines.append(fline_objects[0])
                 for varyfline in varyfline_objects:
                     self.fieldlines.append(varyfline)
 
@@ -779,15 +995,15 @@
                     v_fl_lon = triplet[1]
                     v_fl_lat = triplet[2]
 
                     fieldline = multicolorline(np.deg2rad(v_fl_lon), np.cos(np.deg2rad(v_fl_lat))*v_fl_r, ax=ax, cvals=v_fl_lat, vmin=-90, vmax=90)
 
             else:
                 # If no varying, then just get one field line from get_field_line_coords()
-                # Note that even in the case of a singular fieldline object, this function returns a list
+                # Note that even in the case of a singular fieldline object, this function returns a list 
                 fline_triplets, fline_objects = get_field_line_coords(alpha_body[-1], np.deg2rad(body_lat), pfss_solution, rss)
 
                 # Collect field line objects to a list
                 self.fieldlines.append(fline_objects[0])
 
             # The middlemost field lines are always plotted regardless if varying or no
             fl_r   = fline_triplets[0][0]
@@ -797,42 +1013,88 @@
             # Plot the color coded field line
             fieldline = multicolorline(np.deg2rad(fl_lon), np.cos(np.deg2rad(fl_lat))*fl_r, ax=ax, cvals=fl_lat, vmin=-90, vmax=90)
 
             # Finally, save the photospheric footpoint of the middlemost field lines as a tuple and magnetic polarity as +1/-1
             photospheric_footpoints.append((fl_lon[0], fl_lat[0]))
             fieldline_polarities.append(int(fline_objects[0].polarity))
 
+
         # Reference longitude and corresponding parker spiral arm
         if self.reference_long:
             delta_ref = self.reference_long
             if delta_ref < 0.:
                 delta_ref = delta_ref + 360.
             if self.reference_lat is None:
                 ref_lat = 0.
             else:
                 ref_lat = self.reference_lat
 
             # take into account solar differential rotation wrt. latitude
             omega_ref = self.solar_diff_rot(ref_lat)
 
-            # old eq. for alpha_ref contained redundant dist_e variable:
-            # alpha_ref = np.deg2rad(delta_ref) + omega_ref / (1000*reference_vsw / sun_radius) * (r_scaler*self.target_solar_radius*aconst.R_sun.to(u.AU).value - reference_array) * np.cos(np.deg2rad(ref_lat))
-            alpha_ref = np.deg2rad(delta_ref) + omega_ref / (1000*reference_vsw / sun_radius) * (rss - reference_array) * np.cos(np.deg2rad(ref_lat))
+            # Track up from the reference point a fluxtube
+            # Start tracking from the height of 0.1 solar radii
+            ref_triplets, ref_objects, varyref_triplets, varyref_objects = vary_flines(np.deg2rad(delta_ref), np.deg2rad(ref_lat), pfss_solution, n_varies, 1.1)
 
-            # old arrow style:
-            arrow_dist = rss-1
-            ref_arr = plt.arrow(np.deg2rad(delta_ref), 1, 0, arrow_dist, head_width=0.1, head_length=0.4, edgecolor='black',
-                                facecolor='black', lw=2.0, zorder=5, overhang=0.2)
+            # Plot the color coded field line
+            fieldline = multicolorline(np.deg2rad(ref_triplets[0][1]), np.cos(np.deg2rad(ref_triplets[0][2]))*ref_triplets[0][0], ax=ax, cvals=ref_triplets[0][2], vmin=-90, vmax=90)
+
+            # ... And also plot the color coded flux tube
+            for triplet in varyref_triplets:
+                v_fl_r   = triplet[0]
+                v_fl_lon = triplet[1]
+                v_fl_lat = triplet[2]
+
+                fieldline = multicolorline(np.deg2rad(v_fl_lon), np.cos(np.deg2rad(v_fl_lat))*v_fl_r, ax=ax, cvals=v_fl_lat, vmin=-90, vmax=90)
+
+            # Collect reference flux tube to their own list of fieldlines
+            self.reference_fieldlines = []
+            self.reference_fieldlines.append(ref_objects[0])
+
+            # Also init extreme values for the longitudinal span of the uptracked flux tube
+            reference_long_min, reference_long_max = 360, 0
+
+            # Loop the fieldlines, collect them to the list and find the extreme values of longitude at the ss
+            for ref_vary in varyref_objects:
+                self.reference_fieldlines.append(ref_vary)
+
+                # Check the orientation of the field line; is the first index at the photosphere or the last?
+                idx = 0 if ref_vary.coords.radius.value[0] > ref_vary.coords.radius.value[-1] else -1
+
+                # Collect the longitudinal extreme values from the uptracked fluxtube at the source surface height
+                if ref_vary.coords.lon.value[idx] < reference_long_min:
+                    reference_long_min = ref_vary.coords.lon.value[idx]
+                if ref_vary.coords.lon.value[idx] > reference_long_max:
+                    reference_long_max = ref_vary.coords.lon.value[idx]
+
+            arrow_dist = rss-0.80
+            ref_arr = plt.arrow(np.deg2rad(reference_long_min), 1, 0, arrow_dist, head_width=0.05, head_length=0.2, edgecolor='black',
+                               facecolor='black', lw=0, zorder=7, overhang=0.1)
+            ref_arr = plt.arrow(np.deg2rad(reference_long_max), 1, 0, arrow_dist, head_width=0.05, head_length=0.2, edgecolor='black',
+                               facecolor='black', lw=0, zorder=7, overhang=0.1)
 
             if plot_spirals:
-                ax.plot(alpha_ref, reference_array * np.cos(np.deg2rad(ref_lat)), ls='--', lw=1.8, color='k',
-                        label=f'field line connecting to\nref. long. (vsw={reference_vsw} km/s)', zorder=1)
+
+                # Calculate spirals for the flux tube boundaries
+                alpha_ref_min = np.deg2rad(reference_long_min) + omega_ref / (1000*reference_vsw / sun_radius) * (rss - reference_array) * np.cos(np.deg2rad(ref_lat))
+                alpha_ref_max = np.deg2rad(reference_long_max) + omega_ref / (1000*reference_vsw / sun_radius) * (rss - reference_array) * np.cos(np.deg2rad(ref_lat))
+
+                # Plot the spirals
+                min_edge = plt.polar(alpha_ref_min, reference_array * np.cos(np.deg2rad(ref_lat)), lw=0.7, color="grey", alpha=0.45)[0]
+                max_edge = plt.polar(alpha_ref_max, reference_array * np.cos(np.deg2rad(ref_lat)), lw=0.7, color="grey", alpha=0.45)[0]
+
+                # Extract 'x' and 'y' values
+                x1 = min_edge.get_xdata()
+                y1 = min_edge.get_ydata()
+                x2 = max_edge.get_xdata()
+
+                plt.fill_betweenx(y1, x1, x2, lw=0, color="grey", alpha=0.35)
 
         if long_sector is not None:
-            if type(long_sector) == list and len(long_sector)==2:
+            if isinstance(long_sector, (list,tuple)) and len(long_sector)==2:
 
                 delta_ref1 = long_sector[0]
                 if delta_ref1 < 0.:
                     delta_ref1 = delta_ref1 + 360.
                 delta_ref2 = long_sector[1]
                 if delta_ref2 < 0.:
                     delta_ref2 = delta_ref2 + 360.
@@ -841,29 +1103,76 @@
                 long_sector_lat = [0, 0]
 
                 # take into account solar differential rotation wrt. latitude
                 omega_ref1 = self.solar_diff_rot(long_sector_lat[0])
                 omega_ref2 = self.solar_diff_rot(long_sector_lat[1])
 
                 if long_sector_vsw is not None:
-                    alpha_ref1 = np.deg2rad(delta_ref1) + omega_ref1 / (long_sector_vsw[0] / AU) * (self.target_solar_radius*aconst.R_sun.to(u.AU).value - reference_array) * np.cos(np.deg2rad(long_sector_lat[0]))
-                    alpha_ref2 = np.deg2rad(delta_ref2) + omega_ref2 / (long_sector_vsw[1] / AU) * (self.target_solar_radius*aconst.R_sun.to(u.AU).value - reference_array) * np.cos(np.deg2rad(long_sector_lat[1]))
+
+                    # Calculate the spirals' angles along r
+                    alpha_ref1 = np.deg2rad(delta_ref1) + omega_ref1 / (1000*long_sector_vsw[0] / sun_radius) * (rss - reference_array) * np.cos(np.deg2rad(long_sector_lat[0]))
+                    alpha_ref2 = np.deg2rad(delta_ref2) + omega_ref2 / (1000*long_sector_vsw[1] / sun_radius) * (rss - reference_array) * np.cos(np.deg2rad(long_sector_lat[1]))
+
+                    # Construct a second r_array for the second spiral for while loop to iterate forwards.
+                    # This copy of an array will be used to plot both spiral later.
+                    reference_array2 = np.copy(reference_array)
+
+                    # Check that reference angle of the first loop is ahead
+                    if alpha_ref1[-1] > alpha_ref2[-1]:
+                      alpha_ref1_comp = alpha_ref1[-1] - 2*np.pi
+                    else:
+                      alpha_ref1_comp = alpha_ref1[-1]
+
+                    # While the second spiral is behind the first spiral in angle, extend the second spiral
+                    while alpha_ref2[-1] > alpha_ref1_comp:
+                      reference_array2 = np.append(reference_array2, reference_array2[-1] + 1)
+                      alpha_ref2 = np.append(alpha_ref2, np.deg2rad(delta_ref2) + omega_ref2 / (1000*long_sector_vsw[1] / sun_radius) * (rss - reference_array2[-1]) * np.cos(np.deg2rad(long_sector_lat[1])))
+
+                    # Finally interpolate the first spiral's angles to the coarser second spiral's angles (outside the plot)
+                    alpha_ref1 = np.interp(reference_array2, reference_array, alpha_ref1)
+
+                    # Introduce r axis to plot that is common between these if and else blocks
+                    r_to_plot = reference_array2
+
                 else:
                     # if no solar wind speeds for Parker spirals are provided, use straight lines:
-                    alpha_ref1 = [np.deg2rad(delta_ref1)] * len(reference_array)
-                    alpha_ref2 = [np.deg2rad(delta_ref2)] * len(reference_array)
+                    #alpha_ref1 = [np.deg2rad(delta_ref1)] * len(reference_array)
+                    #alpha_ref2 = [np.deg2rad(delta_ref2)] * len(reference_array)
 
-                c1 = plt.polar(alpha_ref1, reference_array * np.cos(np.deg2rad(long_sector_lat[0])), lw=0, color=long_sector_color, alpha=0.5)[0]
+                    # Vectorize the previous implementation for added performance
+                    alpha_ref1 = np.ones(shape=len(reference_array)) * np.deg2rad(delta_ref1)
+                    alpha_ref2 = np.ones(shape=len(reference_array)) * np.deg2rad(delta_ref2)
+
+                    # Another reference to r_array to unify this if/else -block's output
+                    r_to_plot = reference_array
+
+
+                c1 = plt.polar(alpha_ref1, r_to_plot * np.cos(np.deg2rad(long_sector_lat[0])), lw=0, color=long_sector_color, alpha=0)[0]
                 x1 = c1.get_xdata()
                 y1 = c1.get_ydata()
-                c2 = plt.polar(alpha_ref2, reference_array * np.cos(np.deg2rad(long_sector_lat[1])), lw=0, color=long_sector_color, alpha=0.5)[0]
+                c2 = plt.polar(alpha_ref2, r_to_plot * np.cos(np.deg2rad(long_sector_lat[1])), lw=0, color=long_sector_color, alpha=0)[0]
                 x2 = c2.get_xdata()
                 y2 = c2.get_ydata()
 
-                plt.fill_betweenx(y1, x1, x2, lw=0, color=long_sector_color, alpha=0.5)
+                # Check that plotted are is between the two spirals, and do not fill after potential crossing
+                if long_sector_vsw:
+                    clause1 = x1 < x2 
+                    clause2 = alpha_ref1[clause1] < alpha_ref2[clause1]
+
+                    # Take as a selection only the points that fill the above clauses
+                    y1_fill = y1[clause1][clause2]
+                    x1_fill = x1[clause1][clause2]
+                    x2_fill = x2[clause1][clause2]
+                else:
+                    y1_fill = y1
+                    x1_fill = x1
+                    x2_fill = x2
+
+                plt.fill_betweenx(y1_fill, x1_fill, x2_fill, lw=0, color=long_sector_color, alpha=0.40)
+
             else:
                 print("Ill-defined 'long_sector'. It should be a 2-element list defining the start and end longitude of the cone in degrees; e.g. 'long_sector=[15,45]'")
 
         leg1 = ax.legend(loc=(1.05, 0.8), fontsize=13)
 
         if numbered_markers:
             offset = matplotlib.text.OffsetFrom(leg1, (0.0, 1.0))
@@ -894,25 +1203,38 @@
         # if self.coord_sys=='Stonyhurst':
         #     ax.set_xticks(np.pi/180. * np.linspace(180, -180, 8, endpoint=False))
         #     ax.set_thetalim(-np.pi, np.pi)
 
         # Spin the angular coordinate so that earth is at 6 o'clock
         ax.set_theta_offset(np.deg2rad(long_offset - E_long))
 
-        # For some reason we need to specify 'ylim' here
-        ax.set_ylim(0, r_max)
+        # For some reason we need to specify 'ylim' here 
+        ax.set_ylim(0,r_max)
         ax.set_rscale('symlog', linthresh=rss)
         ax.set_rmax(r_max)
         ax.set_rticks([1.0, rss, 10.0, 100.0])
         ax.set_rlabel_position(-22.5)  # Move radial labels away from plotted line
         ax.tick_params(which='major', labelsize=22,)
 
         rlabels = ['1', str(rss), r'$10^1$', r'$10^2$']
         ax.set_yticklabels(rlabels)
 
+        # Drawing a circle around the plot, because sometimes for unkown reason the plot boundary is not drawn.
+        # Here circle_radius corresponds to the boundary of the plot, and it was empirically found.
+        circle_radius = 9.35
+
+        circle = plt.Circle((0., 0.),
+                            circle_radius,
+                            transform=ax.transData._b,
+                            edgecolor="k",
+                            facecolor=None,
+                            fill=False, lw=2)
+        ax.add_patch(circle)
+
+        # Cut off unnecessary margins from the plot
         plt.tight_layout()
 
         if not hide_logo:
             txt_x_begin, txt_y_begin = 0.98, 0.16
             ax.text(txt_x_begin, txt_y_begin, 'Solar-MACH',
                     fontfamily='DejaVu Serif', fontsize=28,
                     ha='right', va='bottom', transform=fig.transFigure)
```

### Comparing `solarmach-0.2.2/solarmach/pfss_utilities.py` & `solarmach-0.2.3/solarmach/pfss_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
     params
     -------
     longitude: int/float
             Carrington longitude of the seeding point for the FieldLine tracing
     latitude: int/float
             Carrington latitude of the seeding point for the FieldLine tracing
     hmimap: hmi_synoptic_map object
+            hmimap
     seedheight: float
             Heliocentric height of the seeding point
 
     returns
     -------
     coordlist: list[list[float,float,float]]
             The list of lists  of all coordinate triplets that correspond to the FieldLine objects traced
@@ -220,119 +221,120 @@
         triplet = [fl_r, fl_lon, fl_lat]
         coordlist.append(triplet)
         flinelist.append(fline)
 
     return coordlist, flinelist
 
 
-def vary_flines(lon, lat, hmimap, n_varies, rss):
+def vary_flines(lon, lat, hmimap, n_varies, seedheight):
     """
     Finds a set of sub-pfss fieldlines connected to or very near a single footpoint on the pfss.
-
+    
     lon: longitude of the footpoint [rad]
     lat: latitude of the footpoint [rad]
-
+    
     n_varies:   tuple that holds the amount of circles and the number of dummy flines per circle
-                if type(n_varies)=int, consider that as the amount of circles, and set the
+                if type(n_varies)=int, consider that as the amount of circles, and set the 
                 amount of dummy flines per circle to 16
 
     params
     -------
     lon: int/float
             The longitude of the footpoint in radians
     lat: int/float
             The latitude of the footpoint in radians
     hmimap: hmi_synoptic_map object
             The pfss-solution used to calculate the field lines
-    n_varies: list[int,int] or int
+    n_varies: list[int,int] or int 
             A list that holds the amount of circles and the number of dummy flines per circle
             if type(n_varies)=int, consider that as the amount of circles, and set the
             amount of dummy flines per circle to 16
-    rss: float
-            Heliocentric height of the source surface
+    seedheight: float
+            Heliocentric height of the tracing starting point
 
     returns
     -------
     coordlist: list[float,float,float]
             List of coordinate triplets of the original field lines (lon,lat,height)
     flinelist: list[FieldLine-object]
             List of Fieldline objects of the original field lines
     varycoords: list[float,float,float]
             List of coordinate triplets of the varied field lines
     varyflines: list[FieldLine-object]
             List of Fieldline objects of the varied field lines
     """
 
     # Field lines per n_circles (circle)
-    if isinstance(n_varies, list):
+    if isinstance(n_varies,(list,tuple)):
+        print(f"n_varies: {n_varies}")
         n_circles = n_varies[0]
         n_flines = n_varies[1]
     else:
         n_circles = n_varies
         n_flines = 16
 
     # First produce new points around the given lonlat_pair
     lons, lats= np.array([lon]), np.array([lat])
     increments = np.array([0.03, 0.05, 0.07, 0.09, 0.11, 0.13, 0.15, 0.17, 0.19, 0.21, 0.23, 0.25, 0.27, 0.29])
     for circle in range(n_circles):
 
-        newlons, newlats = circle_around(lon, lat, n_flines, r=increments[circle])
-        lons, lats = np.append(lons, newlons), np.append(lats, newlats)
+        newlons, newlats = circle_around(lon,lat,n_flines,r=increments[circle])
+        lons, lats = np.append(lons,newlons), np.append(lats,newlats)
 
     pointlist = np.array([lons, lats])
 
     # Trace fieldlines from all of these points
-    varycoords, varyflines = get_field_line_coords(pointlist[0], pointlist[1], hmimap, rss)
+    varycoords, varyflines = get_field_line_coords(pointlist[0],pointlist[1],hmimap, seedheight)
 
     # Because the original fieldlines and the varied ones are all in the same arrays,
     # Extract the varied ones to their own arrays
     coordlist, flinelist = [], []
 
     # Total amount of flines = 1 + (circles) * (fieldlines_per_circle)
     total_per_fp = n_flines*n_circles+1
     erased_indices = []
     for i in range(len(varycoords)):
         # n_flines*n_circles = the amount of extra field lines between each "original" field line
         if i%(total_per_fp)==0:
             erased_indices.append(i)
             # pop(i) removes the ith element from the list and returns it
             # -> we append it to the list of original footpoint fieldlines
-            coordlist.append(varycoords[i])  # .pop(i)
+            coordlist.append(varycoords[i]) #.pop(i)
             flinelist.append(varyflines[i])
 
     # Really ugly quick fix to erase values from varycoords and varyflines
     for increment, index in enumerate(erased_indices):
         varycoords.pop(index-increment)
         varyflines.pop(index-increment)
 
     return coordlist, flinelist, varycoords, varyflines
 
 
 def trace_field_line(lon0, lat0, hmimap, seedheight, rad=True):
-    '''
+    """
     Traces a single open magnetic field line at coordinates (lon0,lat0) on the pfss down
     to the photosphere
 
     Parameters:
     -----------
     lon0, lat0: float
             Longitude and latitude of the seedpoint
     hmimap: hmimap-object
-
+            hmimap
     seedheight: float
             The height at which field line tracing is started (in solar radii)
     rad: bool, (default True)
             Wether or not input coordinates are in radians. If False, consider them degrees
 
     Returns:
     --------
     field_lines: FieldLine or list[FieldLine]
             A FieldLine object, or a list of them, if input coordinates were a list
 
-    '''
+    """
     from pfsspy import tracing
 
     # if lat0 and lon0 are given in deg for some reason, transform them to rad
     if not rad:
         lat0 = np.deg2rad(lat0)
         lon0 = np.deg2rad(lon0)
 
@@ -376,15 +378,15 @@
     returns
     -----------
     lon, lat: float
             new coordinate pair
     """
 
     # In radians, 1 rad \approx 57.3 deg
-    step = 0.01
+    step = 0.005
 
     # Keeps track of how many steps until it's time to turn
     steps_until_corner, steps_moved = corner_tracker[0], corner_tracker[1]
 
     if turn=='lon':
 
         lon = lon + step*sign_switch
```

### Comparing `solarmach-0.2.2/solarmach/tests/test.py` & `solarmach-0.2.3/solarmach/tests/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def test_solarmach_initialize():
     body_list = ['STEREO-A']
     vsw_list = [400]
     date = '2021-10-28 15:15:00'
     reference_long = 273
     reference_lat = 9
 
-    sm = SolarMACH(date, body_list, vsw_list, reference_long, reference_lat)
+    sm = SolarMACH(date=date, body_list=body_list, vsw_list=vsw_list, reference_long=reference_long, reference_lat=reference_lat)
 
     assert sm.date == date
     assert sm.reference_lat == reference_lat
     assert sm.reference_long == reference_long
     assert np.round(sm.max_dist, 3) == 0.958
 
     assert isinstance(sm.pos_E, astropy.coordinates.sky_coordinate.SkyCoord)
@@ -39,14 +39,14 @@
     vsw_list = [400]
     date = '2021-10-28 15:15:00'
     reference_long = 273
     reference_lat = 9
     reference_vsw = 400
     filename = 'test.png'
 
-    sm = SolarMACH(date, body_list, vsw_list, reference_long, reference_lat)
+    sm = SolarMACH(date=date, body_list=body_list, vsw_list=vsw_list, reference_long=reference_long, reference_lat=reference_lat)
     sm.plot(plot_spirals=True, plot_sun_body_line=True,
             reference_vsw=reference_vsw, transparent=False,
             show_earth_centered_coord=False, numbered_markers=True,
             outfile=filename)
 
     assert os.path.exists(os.getcwd()+os.sep+filename)
```

### Comparing `solarmach-0.2.2/solarmach.egg-info/PKG-INFO` & `solarmach-0.2.3/solarmach.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarmach
-Version: 0.2.2
+Version: 0.2.3
 Summary: Multi-spacecraft longitudinal configuration plotter
 Home-page: https://github.com/jgieseler/solarmach
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -12,33 +12,37 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
 solarmach
 =========
 
-|pypi Version| |conda version| |license| |python version| |pytest| |zenodo|
+|pypi Version| |conda version| |python version| |pytest| |codecov| |docs| |license| |zenodo|
 
 .. |pypi Version| image:: https://img.shields.io/pypi/v/solarmach?style=flat&logo=pypi
    :target: https://pypi.org/project/solarmach/
 .. |conda version| image:: https://img.shields.io/conda/vn/conda-forge/solarmach?style=flat&logo=anaconda
    :target: https://anaconda.org/conda-forge/solarmach/
-.. |license| image:: https://img.shields.io/conda/l/conda-forge/solarmach?style=flat
-   :target: https://github.com/jgieseler/solarmach/blob/main/LICENSE.rst
 .. |python version| image:: https://img.shields.io/pypi/pyversions/solarmach?style=flat&logo=python
 .. |pytest| image:: https://github.com/jgieseler/solarmach/workflows/pytest/badge.svg
+.. |codecov| image:: https://codecov.io/gh/jgieseler/solarmach/branch/main/graph/badge.svg?token=CT2P8AQU3B
+   :target: https://codecov.io/gh/jgieseler/solarmach
+.. |docs| image:: https://readthedocs.org/projects/solarmach/badge/?version=latest
+   :target: https://solarmach.readthedocs.io/en/latest/?badge=latest
+.. |license| image:: https://img.shields.io/conda/l/conda-forge/solarmach?style=flat
+   :target: https://github.com/jgieseler/solarmach/blob/main/LICENSE.rst
 .. |zenodo| image:: https://zenodo.org/badge/469735286.svg
    :target: https://zenodo.org/badge/latestdoi/469735286
 
 
 
 The Solar MAgnetic Connection Haus (Solar-MACH) tool is a multi-spacecraft longitudinal configuration plotter. This is the repository of the pip/conda package of Solar-MACH, called **solarmach**. For the corresponding streamlit repository, which is used for `solar-mach.github.io <https://solar-mach.github.io>`_, see `github.com/jgieseler/Solar-MACH <https://github.com/jgieseler/Solar-MACH>`_.
 
@@ -104,15 +108,19 @@
    
    # obtain data as Pandas DataFrame
    display(sm.coord_table)
 
 .. image:: https://github.com/jgieseler/solarmach/raw/main/examples/solarmach.png
   :alt: Example output figure
   
-See example notebooks in next section for all options!
+
+Documentation
+-------------
+Full documentation for the package can be found at https://solarmach.readthedocs.io
+
   
 Example Notebooks
 -----------------
 
 **solarmach** can easily be run in a Jupyter Notebook. 
 
 - `Show simple example notebook <https://nbviewer.org/github/jgieseler/solarmach/blob/main/examples/example.ipynb>`_ |nbviewer1|
```

### Comparing `solarmach-0.2.2/solarmach.egg-info/SOURCES.txt` & `solarmach-0.2.3/solarmach.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/conf.py
 docs/index.rst
+docs/installation.rst
 docs/make.bat
+docs/requirements.txt
+docs/solarmach.rst
+docs/usage.nblink
 examples/example.ipynb
 examples/solarmach.png
 licenses/LICENSE.rst
 licenses/TEMPLATE_LICENSE.rst
 solarmach/__init__.py
 solarmach/pfss_utilities.py
 solarmach/version.py
```

### Comparing `solarmach-0.2.2/tox.ini` & `solarmach-0.2.3/tox.ini`

 * *Files identical despite different names*

