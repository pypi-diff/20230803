# Comparing `tmp/symbal-0.0.8.tar.gz` & `tmp/symbal-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbal-0.0.8.tar", last modified: Wed Jul 12 18:33:43 2023, max compression
+gzip compressed data, was "symbal-0.0.9.tar", last modified: Wed Jul 12 18:43:04 2023, max compression
```

## Comparing `symbal-0.0.8.tar` & `symbal-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 18:33:43.794968 symbal-0.0.8/
--rw-rw-rw-   0        0        0     1090 2023-07-09 21:31:44.000000 symbal-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       32 2023-07-09 21:31:44.000000 symbal-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      666 2023-07-12 18:33:43.793970 symbal-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       84 2023-07-09 21:31:44.000000 symbal-0.0.8/README.md
--rw-rw-rw-   0        0        0      111 2023-07-09 21:31:44.000000 symbal-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 18:33:43.794968 symbal-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      842 2023-07-12 18:33:37.000000 symbal-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 18:33:43.786989 symbal-0.0.8/symbal/
--rw-rw-rw-   0        0        0      353 2023-07-12 18:33:37.000000 symbal-0.0.8/symbal/__init__.py
--rw-rw-rw-   0        0        0     3493 2023-07-12 18:33:37.000000 symbal-0.0.8/symbal/main.py
--rw-rw-rw-   0        0        0      408 2023-07-09 21:41:09.000000 symbal-0.0.8/symbal/penalties.py
--rw-rw-rw-   0        0        0     6364 2023-07-10 15:33:20.000000 symbal-0.0.8/symbal/test_function.py
--rw-rw-rw-   0        0        0     2579 2023-07-11 21:28:25.000000 symbal-0.0.8/symbal/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 18:33:43.792973 symbal-0.0.8/symbal.egg-info/
--rw-rw-rw-   0        0        0      666 2023-07-12 18:33:43.000000 symbal-0.0.8/symbal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-12 18:33:43.000000 symbal-0.0.8/symbal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 18:33:43.000000 symbal-0.0.8/symbal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 18:33:43.000000 symbal-0.0.8/symbal.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 18:43:04.977270 symbal-0.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-07-09 21:31:44.000000 symbal-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-07-09 21:31:44.000000 symbal-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      666 2023-07-12 18:43:04.977270 symbal-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2023-07-09 21:31:44.000000 symbal-0.0.9/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-09 21:31:44.000000 symbal-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 18:43:04.977270 symbal-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-07-12 18:42:58.000000 symbal-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:43:04.969291 symbal-0.0.9/symbal/
+-rw-rw-rw-   0        0        0      353 2023-07-12 18:42:58.000000 symbal-0.0.9/symbal/__init__.py
+-rw-rw-rw-   0        0        0     3496 2023-07-12 18:42:58.000000 symbal-0.0.9/symbal/main.py
+-rw-rw-rw-   0        0        0      408 2023-07-09 21:41:09.000000 symbal-0.0.9/symbal/penalties.py
+-rw-rw-rw-   0        0        0     6364 2023-07-10 15:33:20.000000 symbal-0.0.9/symbal/test_function.py
+-rw-rw-rw-   0        0        0     2579 2023-07-11 21:28:25.000000 symbal-0.0.9/symbal/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:43:04.975275 symbal-0.0.9/symbal.egg-info/
+-rw-rw-rw-   0        0        0      666 2023-07-12 18:43:04.000000 symbal-0.0.9/symbal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-12 18:43:04.000000 symbal-0.0.9/symbal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 18:43:04.000000 symbal-0.0.9/symbal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 18:43:04.000000 symbal-0.0.9/symbal.egg-info/top_level.txt
```

### Comparing `symbal-0.0.8/LICENSE` & `symbal-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `symbal-0.0.8/PKG-INFO` & `symbal-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbal
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package for batch adaptive sampling with symbolic regression
 Home-page: https://github.com/ajsummers/symbal
 Author: Alex Summers
 Author-email: ajs0201@auburn.edu
 License: UNKNOWN
 Project-URL: Issues, https://github.com/ajsummers/symbal/issues
 Platform: UNKNOWN
```

### Comparing `symbal-0.0.8/setup.py` & `symbal-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='symbal',
-    version='0.0.8',
+    version='0.0.9',
     author='Alex Summers',
     author_email='ajs0201@auburn.edu',
     description='A Python package for batch adaptive sampling with symbolic regression',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ajsummers/symbal',
     project_urls={
```

### Comparing `symbal-0.0.8/symbal/main.py` & `symbal-0.0.9/symbal/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,17 @@
             selected_indices, captured_penalties = bs(np.array(x_cand), batch_size=batch_size, **batch_config)
             captured_penalties = captured_penalties.rename(columns={
                 column: f'{i+1}-{column}' for column in list(captured_penalties.columns)
             })
             self.captured_penalties = pd.concat([self.captured_penalties, captured_penalties], axis=1)
             self.selected_indices.append(selected_indices)
 
-            logging.debug('Selected indices: ', selected_indices)
-            logging.debug('tf.candidates shape: ', tf.candidates.shape)
-            logging.debug('x_cand shape: ', x_cand.shape)
+            logging.debug(f'Selected indices: {selected_indices}')
+            logging.debug(f'tf.candidates shape: {tf.candidates.shape}')
+            logging.debug(f'x_cand shape: {x_cand.shape}')
 
             tf.initial_set = pd.concat([tf.initial_set, tf.candidates.loc[selected_indices, :]], axis=0)
             tf.candidates = tf.candidates.drop(selected_indices, axis=0)
 
         scores_dict = {
             'equation': equations,
             'extrap': extrap_scores,
```

### Comparing `symbal-0.0.8/symbal/test_function.py` & `symbal-0.0.9/symbal/test_function.py`

 * *Files identical despite different names*

### Comparing `symbal-0.0.8/symbal/utils.py` & `symbal-0.0.9/symbal/utils.py`

 * *Files identical despite different names*

### Comparing `symbal-0.0.8/symbal.egg-info/PKG-INFO` & `symbal-0.0.9/symbal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbal
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package for batch adaptive sampling with symbolic regression
 Home-page: https://github.com/ajsummers/symbal
 Author: Alex Summers
 Author-email: ajs0201@auburn.edu
 License: UNKNOWN
 Project-URL: Issues, https://github.com/ajsummers/symbal/issues
 Platform: UNKNOWN
```

