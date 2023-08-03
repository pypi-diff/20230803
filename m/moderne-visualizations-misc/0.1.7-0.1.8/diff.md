# Comparing `tmp/moderne_visualizations_misc-0.1.7.tar.gz` & `tmp/moderne_visualizations_misc-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moderne_visualizations_misc-0.1.7.tar", last modified: Wed Aug  2 01:07:28 2023, max compression
+gzip compressed data, was "moderne_visualizations_misc-0.1.8.tar", last modified: Wed Aug  2 22:24:34 2023, max compression
```

## Comparing `moderne_visualizations_misc-0.1.7.tar` & `moderne_visualizations_misc-0.1.8.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:07:28.175486 moderne_visualizations_misc-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-02 01:07:28.175486 moderne_visualizations_misc-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:07:28.171486 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/cobol_find_copy_book.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/dependency_vulnerabilities.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/find_methods.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:07:28.175486 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/images/
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/images/cobol_find_copy_book.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    31410 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/images/language_composition.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/images/parse_failure_analysis.300.png
--rw-r--r--   0 runner    (1001) docker     (123)    24871 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/images/sql_crud.300.png
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/language_composition.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/parse_failure_analysis.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:07:28.175486 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/specs/cobol_find_copy_book.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/specs/find_methods.yml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/specs/language_composition.yml
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/specs/parse_failure_analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/specs/sql_crud.yml
--rw-r--r--   0 runner    (1001) docker     (123)   152398 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/sql_crud.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:07:28.175486 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-02 01:07:28.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-02 01:07:28.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 01:07:28.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 01:07:28.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 01:07:28.000000 moderne_visualizations_misc-0.1.7/moderne_visualizations_misc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-08-02 01:07:09.000000 moderne_visualizations_misc-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 01:07:28.175486 moderne_visualizations_misc-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:24:34.891662 moderne_visualizations_misc-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-02 22:24:34.891662 moderne_visualizations_misc-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:24:34.887662 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/cobol_find_copy_book.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/dependency_vulnerabilities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/find_methods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    25481 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/find_source_files.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:24:34.891662 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/cobol_find_copy_book.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31410 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/language_composition.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/parse_failure_analysis.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24871 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/sql_crud.300.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/language_composition.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/parse_failure_analysis.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:24:34.891662 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/cobol_find_copy_book.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/find_methods.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/find_source_files.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/language_composition.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/parse_failure_analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/sql_crud.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   152398 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/sql_crud.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 22:24:34.891662 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-02 22:24:34.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-02 22:24:34.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 22:24:34.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-02 22:24:34.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 22:24:34.000000 moderne_visualizations_misc-0.1.8/moderne_visualizations_misc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-08-02 22:24:13.000000 moderne_visualizations_misc-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 22:24:34.891662 moderne_visualizations_misc-0.1.8/setup.cfg
```

### Comparing `moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/cobol_find_copy_book.ipynb` & `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/cobol_find_copy_book.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/dependency_vulnerabilities.ipynb` & `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/dependency_vulnerabilities.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.9.17'}}"}*

```diff
@@ -161,13 +161,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.17"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/find_methods.ipynb` & `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/find_methods.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.9.17'}}"}*

```diff
@@ -58,13 +58,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.17"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/images/cobol_find_copy_book.300.png` & `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/cobol_find_copy_book.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png` & `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/dependency_vulnerabilities.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/images/language_composition.300.png` & `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/language_composition.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/images/parse_failure_analysis.300.png` & `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/parse_failure_analysis.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/images/sql_crud.300.png` & `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/images/sql_crud.300.png`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/language_composition.ipynb` & `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/language_composition.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9915178571428571%*

 * *Differences: {"'cells'": "{2: {'execution_count': None, 'outputs': []}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.17'}}"}*

```diff
@@ -12,29 +12,17 @@
             "metadata": {},
             "source": [
                 "This report shows the different languages that are used in the projects."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "ename": "ModuleNotFoundError",
-                    "evalue": "No module named 'plotly'",
-                    "output_type": "error",
-                    "traceback": [
-                        "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
-                        "\u001b[1;31mModuleNotFoundError\u001b[0m                       Traceback (most recent call last)",
-                        "Cell \u001b[1;32mIn[1], line 1\u001b[0m\n\u001b[1;32m----> 1\u001b[0m \u001b[38;5;28;01mimport\u001b[39;00m \u001b[38;5;21;01mplotly\u001b[39;00m\u001b[38;5;21;01m.\u001b[39;00m\u001b[38;5;21;01mexpress\u001b[39;00m \u001b[38;5;28;01mas\u001b[39;00m \u001b[38;5;21;01mpx\u001b[39;00m\n\u001b[0;32m      2\u001b[0m \u001b[38;5;28;01mimport\u001b[39;00m \u001b[38;5;21;01mpandas\u001b[39;00m \u001b[38;5;28;01mas\u001b[39;00m \u001b[38;5;21;01mpd\u001b[39;00m\n\u001b[0;32m      3\u001b[0m \u001b[38;5;28;01mimport\u001b[39;00m \u001b[38;5;21;01mwarnings\u001b[39;00m\n",
-                        "\u001b[1;31mModuleNotFoundError\u001b[0m: No module named 'plotly'"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "import plotly.express as px\n",
                 "import pandas as pd\n",
                 "import warnings\n",
                 "import moderne_pkg.helpers as helpers\n",
                 "\n",
                 "warnings.simplefilter(\"ignore\")\n",
@@ -144,13 +132,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.4"
+            "version": "3.9.17"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/parse_failure_analysis.ipynb` & `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/parse_failure_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml` & `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/dependency_vulnerabilities.yml`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/specs/parse_failure_analysis.yml` & `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/specs/parse_failure_analysis.yml`

 * *Files identical despite different names*

### Comparing `moderne_visualizations_misc-0.1.7/moderne_visualizations_misc/sql_crud.ipynb` & `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc/sql_crud.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.9.17'}}"}*

```diff
@@ -995,13 +995,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.17"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `moderne_visualizations_misc-0.1.7/moderne_visualizations_misc.egg-info/SOURCES.txt` & `moderne_visualizations_misc-0.1.8/moderne_visualizations_misc.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MANIFEST.in
 README.rst
 pyproject.toml
 moderne_visualizations_misc/__init__.py
 moderne_visualizations_misc/cobol_find_copy_book.ipynb
 moderne_visualizations_misc/dependency_vulnerabilities.ipynb
 moderne_visualizations_misc/find_methods.ipynb
+moderne_visualizations_misc/find_source_files.ipynb
 moderne_visualizations_misc/language_composition.ipynb
 moderne_visualizations_misc/parse_failure_analysis.ipynb
 moderne_visualizations_misc/sql_crud.ipynb
 moderne_visualizations_misc.egg-info/PKG-INFO
 moderne_visualizations_misc.egg-info/SOURCES.txt
 moderne_visualizations_misc.egg-info/dependency_links.txt
 moderne_visualizations_misc.egg-info/requires.txt
@@ -17,10 +18,11 @@
 moderne_visualizations_misc/images/dependency_vulnerabilities.300.png
 moderne_visualizations_misc/images/language_composition.300.png
 moderne_visualizations_misc/images/parse_failure_analysis.300.png
 moderne_visualizations_misc/images/sql_crud.300.png
 moderne_visualizations_misc/specs/cobol_find_copy_book.yml
 moderne_visualizations_misc/specs/dependency_vulnerabilities.yml
 moderne_visualizations_misc/specs/find_methods.yml
+moderne_visualizations_misc/specs/find_source_files.yml
 moderne_visualizations_misc/specs/language_composition.yml
 moderne_visualizations_misc/specs/parse_failure_analysis.yml
 moderne_visualizations_misc/specs/sql_crud.yml
```

### Comparing `moderne_visualizations_misc-0.1.7/pyproject.toml` & `moderne_visualizations_misc-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @see https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "moderne_visualizations_misc"
-version = "0.1.7"
+version = "0.1.8"
 description = "Miscellaneous visualizations for the Moderne platform"
 authors = [
     { name = "Jonathan Schneider", email = "jonathan@moderne.io" },
     { name = "Kyle Scully", email = "kyle@moderne.io" }
 ]
 license = { text = "Apache-2.0" }
 dependencies = [
```

