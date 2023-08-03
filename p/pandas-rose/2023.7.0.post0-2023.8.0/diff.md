# Comparing `tmp/pandas-rose-2023.7.0.post0.tar.gz` & `tmp/pandas-rose-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-rose-2023.7.0.post0.tar", last modified: Tue Aug  1 05:20:17 2023, max compression
+gzip compressed data, was "pandas-rose-2023.8.0.tar", last modified: Thu Aug  3 14:22:26 2023, max compression
```

## Comparing `pandas-rose-2023.7.0.post0.tar` & `pandas-rose-2023.8.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.859776 pandas-rose-2023.7.0.post0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.851776 pandas-rose-2023.7.0.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/.github/workflows/release-and-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/HOW_TO_RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   338948 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/images/
--rw-r--r--   0 runner    (1001) docker     (123)   532263 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/images/pandas-rose.png
--rw-r--r--   0 runner    (1001) docker     (123)    45880 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/images/sample_bar.png
--rw-r--r--   0 runner    (1001) docker     (123)    90999 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/images/sample_plot.png
--rw-r--r--   0 runner    (1001) docker     (123)    41538 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/images/sample_table.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/pandas_rose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-08-01 05:20:17.000000 pandas-rose-2023.7.0.post0/pandas_rose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-01 05:20:17.000000 pandas-rose-2023.7.0.post0/pandas_rose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 05:20:17.000000 pandas-rose-2023.7.0.post0/pandas_rose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 05:20:17.000000 pandas-rose-2023.7.0.post0/pandas_rose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 05:20:17.000000 pandas-rose-2023.7.0.post0/pandas_rose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/rose/
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/rose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 05:20:17.000000 pandas-rose-2023.7.0.post0/rose/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)   117589 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/sample_data/WBB.csv
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 05:20:17.859776 pandas-rose-2023.7.0.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:17.855775 pandas-rose-2023.7.0.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-01 05:20:02.000000 pandas-rose-2023.7.0.post0/tests/test_rose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:22:26.477612 pandas-rose-2023.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:22:26.473612 pandas-rose-2023.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:22:26.473612 pandas-rose-2023.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:22:26.473612 pandas-rose-2023.8.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/HOW_TO_RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-03 14:22:26.477612 pandas-rose-2023.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   338948 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:22:26.477612 pandas-rose-2023.8.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   532263 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/images/pandas-rose.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45880 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/images/sample_bar.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90999 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/images/sample_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41538 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/images/sample_table.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:22:26.477612 pandas-rose-2023.8.0/pandas_rose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-03 14:22:26.000000 pandas-rose-2023.8.0/pandas_rose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-03 14:22:26.000000 pandas-rose-2023.8.0/pandas_rose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:22:26.000000 pandas-rose-2023.8.0/pandas_rose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 14:22:26.000000 pandas-rose-2023.8.0/pandas_rose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 14:22:26.000000 pandas-rose-2023.8.0/pandas_rose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:22:26.477612 pandas-rose-2023.8.0/rose/
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/rose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-03 14:22:26.000000 pandas-rose-2023.8.0/rose/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/rose/snippets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:22:26.477612 pandas-rose-2023.8.0/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   117589 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/sample_data/WBB.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:22:26.477612 pandas-rose-2023.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:22:26.477612 pandas-rose-2023.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-03 14:22:12.000000 pandas-rose-2023.8.0/tests/test_rose.py
```

### Comparing `pandas-rose-2023.7.0.post0/LICENSE` & `pandas-rose-2023.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0.post0/PKG-INFO` & `pandas-rose-2023.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-rose
-Version: 2023.7.0.post0
+Version: 2023.8.0
 Summary: A simple Pandas accessor to make windrose plots.
 Author-email: Brian Blaylock <blaylockbk@gmail.com>
 Maintainer-email: Brian Blaylock <blaylockbk@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Brian K. Blaylock
         
@@ -22,42 +22,41 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.dev/blaylockbk/pandas-rose
-Project-URL: Documentation, https://github.dev/blaylockbk/pandas-rose
-Project-URL: Repository, https://github.dev/blaylockbk/pandas-rose
-Project-URL: Changelog, https://github.dev/blaylockbk/pandas-rose/releases
+Project-URL: Homepage, https://github.com/blaylockbk/pandas-rose
+Project-URL: Documentation, https://github.com/blaylockbk/pandas-rose
+Project-URL: Repository, https://github.com/blaylockbk/pandas-rose
+Project-URL: Changelog, https://github.com/blaylockbk/pandas-rose/releases
+Project-URL: Bug Tracker, https://github.com/blaylockbk/pandas-rose/issues
 Keywords: weather,meteorology,wind
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 <div align=center>
 
-<img src="images/pandas-rose.png" title="Bing Image Creator: Cartoon chunky panda hugging rose in the wind pixel art " width=200>
+<img src="https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/pandas-rose.png" title="Bing Image Creator: Cartoon chunky panda hugging rose in the wind pixel art " width=200>
 
 </div>
 
 # Pandas Rose
 
 This python package adds a custom Pandas accessor to generate polar wind rose plots from a Pandas dataframe.
 
 I don't mean to compete with the wonderful [windrose](https://github.com/python-windrose/windrose) package already available, but that package has a little too much complexity for what I wanted. This package is meant to provide a minimal, simple interface to making wind rose plots. This is done by using Pandas methods `pd.cut` and `df.groupby` and using Matplotlib regular polar axes.
 
 # Install
 
-> ## TODO: Publish and Upload to PyPI
-
 Install with pip. The requirements are only pandas, numpy, and matplotlib.
 
 ```bash
 pip install pandas-rose
 ```
 
 # Usage
@@ -75,15 +74,15 @@
     "wind_direction":[20, 10, 190,300]
 })
 
 # Display a polar wind plot of the data
 df.rose.plot()
 ```
 
-![Alt text](images/sample_plot.png)
+![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_plot.png)
 
 You can specify the pandas column to use for wind direction and wind speed. You may also change the number of sectors to bin the wind direction .
 
 ```python
 df.rose.plot(
     var_column="A",    # name of variable column
     dir_column="B",    # name of direction column
@@ -97,15 +96,15 @@
 There are two other accessors that give some information.
 
 ```python
 # Display a dataframe of the binned values
 df.rose.table(sectors=8)
 ```
 
-![Alt text](images/sample_table.png)
+![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_table.png)
 
 ```python
 # Display the binned data as bar graph on regular axes.
 df.rose.bar()
 ```
 
-![Alt text](images/sample_bar.png)
+![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_bar.png)
```

### Comparing `pandas-rose-2023.7.0.post0/README.md` & `pandas-rose-2023.8.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 <div align=center>
 
-<img src="images/pandas-rose.png" title="Bing Image Creator: Cartoon chunky panda hugging rose in the wind pixel art " width=200>
+<img src="https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/pandas-rose.png" title="Bing Image Creator: Cartoon chunky panda hugging rose in the wind pixel art " width=200>
 
 </div>
 
 # Pandas Rose
 
 This python package adds a custom Pandas accessor to generate polar wind rose plots from a Pandas dataframe.
 
 I don't mean to compete with the wonderful [windrose](https://github.com/python-windrose/windrose) package already available, but that package has a little too much complexity for what I wanted. This package is meant to provide a minimal, simple interface to making wind rose plots. This is done by using Pandas methods `pd.cut` and `df.groupby` and using Matplotlib regular polar axes.
 
 # Install
 
-> ## TODO: Publish and Upload to PyPI
-
 Install with pip. The requirements are only pandas, numpy, and matplotlib.
 
 ```bash
 pip install pandas-rose
 ```
 
 # Usage
@@ -35,15 +33,15 @@
     "wind_direction":[20, 10, 190,300]
 })
 
 # Display a polar wind plot of the data
 df.rose.plot()
 ```
 
-![Alt text](images/sample_plot.png)
+![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_plot.png)
 
 You can specify the pandas column to use for wind direction and wind speed. You may also change the number of sectors to bin the wind direction .
 
 ```python
 df.rose.plot(
     var_column="A",    # name of variable column
     dir_column="B",    # name of direction column
@@ -57,15 +55,15 @@
 There are two other accessors that give some information.
 
 ```python
 # Display a dataframe of the binned values
 df.rose.table(sectors=8)
 ```
 
-![Alt text](images/sample_table.png)
+![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_table.png)
 
 ```python
 # Display the binned data as bar graph on regular axes.
 df.rose.bar()
 ```
 
-![Alt text](images/sample_bar.png)
+![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_bar.png)
```

### Comparing `pandas-rose-2023.7.0.post0/demo.ipynb` & `pandas-rose-2023.8.0/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0.post0/images/pandas-rose.png` & `pandas-rose-2023.8.0/images/pandas-rose.png`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0.post0/images/sample_bar.png` & `pandas-rose-2023.8.0/images/sample_bar.png`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0.post0/images/sample_plot.png` & `pandas-rose-2023.8.0/images/sample_plot.png`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0.post0/images/sample_table.png` & `pandas-rose-2023.8.0/images/sample_table.png`

 * *Files identical despite different names*

### Comparing `pandas-rose-2023.7.0.post0/pandas_rose.egg-info/PKG-INFO` & `pandas-rose-2023.8.0/pandas_rose.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-rose
-Version: 2023.7.0.post0
+Version: 2023.8.0
 Summary: A simple Pandas accessor to make windrose plots.
 Author-email: Brian Blaylock <blaylockbk@gmail.com>
 Maintainer-email: Brian Blaylock <blaylockbk@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Brian K. Blaylock
         
@@ -22,42 +22,41 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.dev/blaylockbk/pandas-rose
-Project-URL: Documentation, https://github.dev/blaylockbk/pandas-rose
-Project-URL: Repository, https://github.dev/blaylockbk/pandas-rose
-Project-URL: Changelog, https://github.dev/blaylockbk/pandas-rose/releases
+Project-URL: Homepage, https://github.com/blaylockbk/pandas-rose
+Project-URL: Documentation, https://github.com/blaylockbk/pandas-rose
+Project-URL: Repository, https://github.com/blaylockbk/pandas-rose
+Project-URL: Changelog, https://github.com/blaylockbk/pandas-rose/releases
+Project-URL: Bug Tracker, https://github.com/blaylockbk/pandas-rose/issues
 Keywords: weather,meteorology,wind
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 <div align=center>
 
-<img src="images/pandas-rose.png" title="Bing Image Creator: Cartoon chunky panda hugging rose in the wind pixel art " width=200>
+<img src="https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/pandas-rose.png" title="Bing Image Creator: Cartoon chunky panda hugging rose in the wind pixel art " width=200>
 
 </div>
 
 # Pandas Rose
 
 This python package adds a custom Pandas accessor to generate polar wind rose plots from a Pandas dataframe.
 
 I don't mean to compete with the wonderful [windrose](https://github.com/python-windrose/windrose) package already available, but that package has a little too much complexity for what I wanted. This package is meant to provide a minimal, simple interface to making wind rose plots. This is done by using Pandas methods `pd.cut` and `df.groupby` and using Matplotlib regular polar axes.
 
 # Install
 
-> ## TODO: Publish and Upload to PyPI
-
 Install with pip. The requirements are only pandas, numpy, and matplotlib.
 
 ```bash
 pip install pandas-rose
 ```
 
 # Usage
@@ -75,15 +74,15 @@
     "wind_direction":[20, 10, 190,300]
 })
 
 # Display a polar wind plot of the data
 df.rose.plot()
 ```
 
-![Alt text](images/sample_plot.png)
+![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_plot.png)
 
 You can specify the pandas column to use for wind direction and wind speed. You may also change the number of sectors to bin the wind direction .
 
 ```python
 df.rose.plot(
     var_column="A",    # name of variable column
     dir_column="B",    # name of direction column
@@ -97,15 +96,15 @@
 There are two other accessors that give some information.
 
 ```python
 # Display a dataframe of the binned values
 df.rose.table(sectors=8)
 ```
 
-![Alt text](images/sample_table.png)
+![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_table.png)
 
 ```python
 # Display the binned data as bar graph on regular axes.
 df.rose.bar()
 ```
 
-![Alt text](images/sample_bar.png)
+![Alt text](https://raw.githubusercontent.com/blaylockbk/pandas-rose/main/images/sample_bar.png)
```

### Comparing `pandas-rose-2023.7.0.post0/pyproject.toml` & `pandas-rose-2023.8.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 maintainers = [{ name = "Brian Blaylock", email = "blaylockbk@gmail.com" }]
 classifiers = ["Programming Language :: Python"]
 keywords = ["weather", "meteorology", "wind"]
 dependencies = ["matplotlib", "numpy", "pandas"]
 dynamic = ["version"]
 
 [project.urls]
-Homepage = "https://github.dev/blaylockbk/pandas-rose"
-Documentation = "https://github.dev/blaylockbk/pandas-rose"
-Repository = "https://github.dev/blaylockbk/pandas-rose"
-Changelog = "https://github.dev/blaylockbk/pandas-rose/releases"
+"Homepage" = "https://github.com/blaylockbk/pandas-rose"
+"Documentation" = "https://github.com/blaylockbk/pandas-rose"
+"Repository" = "https://github.com/blaylockbk/pandas-rose"
+"Changelog" = "https://github.com/blaylockbk/pandas-rose/releases"
+"Bug Tracker" = "https://github.com/blaylockbk/pandas-rose/issues"
 
 [project.optional-dependencies]
 docs = ["mkdocs-material"]
 test = ["pytest", "black"]
 
 [build-system]
 requires = ["setuptools>=42", "wheel", "setuptools_scm[toml]>=3.4"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
-py-modules = ["rose"]
+packages = ["rose"]
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
 local_scheme = "no-local-version"
 write_to = "rose/_version.py"
 
 [tool.isort]
```

### Comparing `pandas-rose-2023.7.0.post0/rose/__init__.py` & `pandas-rose-2023.8.0/rose/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         plt.xlabel("Wind Direction bins (degrees)")
         plt.ylabel("Frequency")
 
         ax.grid(ls="--", alpha=0.5)
 
         return ax
 
-    def plot(self, spacing=3, figsize=(7, 6), colors="viridis", **kwargs):
+    def plot(self, ax=None, spacing=3, figsize=(7, 6), colors="viridis", **kwargs):
         """Plot the binned data as a windrose
 
         Parameters
         ----------
         dir_column, var_columns: str
             The name of the column representing the wind direction and
             the variable (i.e., wind speed)
@@ -117,16 +117,18 @@
         kwarg_list = list(kwargs)
         table_kwargs = {d: kwargs.pop(d) for d in kwarg_list if d in table_parms}
 
         table = self._obj.rose.table(**table_kwargs)
         nsectors, nbins = table.shape
         radian_locs = np.arange(0, np.pi * 2, np.pi * 2 / len(table))
 
-        fig = plt.figure(figsize=figsize)
-        ax = plt.subplot(projection="polar")
+        if ax is None:
+            fig = plt.figure(figsize=figsize)
+            ax = plt.subplot(projection="polar")
+
         ax.set_theta_zero_location("N")  # theta=0 at the top
         ax.set_theta_direction(-1)  # theta increasing clockwise
 
         kwargs.setdefault("edgecolor", "k")
         kwargs.setdefault("linewidth", 0.5)
         kwargs.setdefault("zorder", 1)
         kwargs.setdefault("alpha", 1)
```

### Comparing `pandas-rose-2023.7.0.post0/sample_data/WBB.csv` & `pandas-rose-2023.8.0/sample_data/WBB.csv`

 * *Files identical despite different names*

