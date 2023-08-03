# Comparing `tmp/jianglab-0.7.3.tar.gz` & `tmp/jianglab-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.7.3.tar", last modified: Fri Jul 28 00:13:06 2023, max compression
+gzip compressed data, was "jianglab-0.7.4.tar", last modified: Thu Aug  3 15:10:33 2023, max compression
```

## Comparing `jianglab-0.7.3.tar` & `jianglab-0.7.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-28 00:13:06.458008 jianglab-0.7.3/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-28 00:13:06.457648 jianglab-0.7.3/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.7.3/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-28 00:13:06.453956 jianglab-0.7.3/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.7.3/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    48868 2023-07-28 00:12:46.000000 jianglab-0.7.3/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.7.3/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-28 00:13:06.456848 jianglab-0.7.3/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-28 00:13:06.000000 jianglab-0.7.3/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-28 00:13:06.000000 jianglab-0.7.3/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-28 00:13:06.000000 jianglab-0.7.3/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      158 2023-07-28 00:13:06.000000 jianglab-0.7.3/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-28 00:13:06.000000 jianglab-0.7.3/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-28 00:13:06.458137 jianglab-0.7.3/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1141 2023-07-28 00:12:53.000000 jianglab-0.7.3/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-03 15:10:33.706579 jianglab-0.7.4/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-03 15:10:33.706189 jianglab-0.7.4/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.7.4/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-03 15:10:33.702057 jianglab-0.7.4/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.7.4/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    49302 2023-08-03 15:09:59.000000 jianglab-0.7.4/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.7.4/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-08-03 15:10:33.705545 jianglab-0.7.4/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-08-03 15:10:33.000000 jianglab-0.7.4/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-08-03 15:10:33.000000 jianglab-0.7.4/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-08-03 15:10:33.000000 jianglab-0.7.4/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      173 2023-08-03 15:10:33.000000 jianglab-0.7.4/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-08-03 15:10:33.000000 jianglab-0.7.4/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-08-03 15:10:33.706718 jianglab-0.7.4/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1177 2023-08-03 15:10:08.000000 jianglab-0.7.4/setup.py
```

### Comparing `jianglab-0.7.3/PKG-INFO` & `jianglab-0.7.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.7.3
+Version: 0.7.4
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.7.3/README.md` & `jianglab-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.7.3/jianglab/common_functions.py` & `jianglab-0.7.4/jianglab/common_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from sklearn.cluster import AgglomerativeClustering 
 
 from scipy.cluster import hierarchy 
 from scipy.spatial import distance_matrix 
 import umap
 
 import warnings
+import glob
 
 
 
 
 
 def frame_ref_to_onset(frame_ref, first_onset_index = 184, visualize_window = (250_000,350_000), stimulus_interval = 60, on_duration = 30, sampling_rate = 20000,overlay_split_num = 5):
     '''
@@ -1199,8 +1200,18 @@
     scaled_data = StandardScaler().fit_transform(data)
     embedding = reducer.fit_transform(scaled_data)
     
     plot_data = pd.DataFrame(embedding, columns=['umap1', 'umap2'])
     plot_data['Labels'] = X['Labels'].values
     sns.scatterplot(x='umap1', y='umap2', hue='Labels', data=plot_data)
 
-    return plot_data
+    return plot_data
+
+def search_file_in_location(location, keyword, recursive=True):
+    """Search for a file in a given location. 
+    If recursive is True, the search will be recursive.
+    search files that contain the keyword in their name."""
+    if recursive:
+        file_list = glob.glob(location + '/**/*' + keyword + '*', recursive=True)
+    else:
+        file_list = glob.glob(location + '/*' + keyword + '*')
+    return file_list
```

### Comparing `jianglab-0.7.3/jianglab.egg-info/PKG-INFO` & `jianglab-0.7.4/jianglab.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.7.3
+Version: 0.7.4
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.7.3/setup.py` & `jianglab-0.7.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.7.3',
+    version='0.7.4',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
@@ -18,14 +18,16 @@
         "opencv-python",
         "ipython",
         "seaborn",
         "optuna",
         "xgboost",
         "scikit-learn",
         "umap-learn",
+        "missingno",
+        "glob"
 
     ],
     author = "Jiang Zheng",
     author_email = "zjiang314@gmail.com",
     description = "A package for Jiang lab",
     url = "https://github.com/jiang-lab-retina/jianglab.git",
     classifiers=[
```

