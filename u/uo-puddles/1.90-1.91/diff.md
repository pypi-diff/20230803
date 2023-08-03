# Comparing `tmp/uo_puddles-1.90.tar.gz` & `tmp/uo_puddles-1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uo_puddles-1.90.tar", last modified: Tue Aug  1 21:00:19 2023, max compression
+gzip compressed data, was "uo_puddles-1.91.tar", last modified: Thu Aug  3 19:06:03 2023, max compression
```

## Comparing `uo_puddles-1.90.tar` & `uo_puddles-1.91.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:00:19.908265 uo_puddles-1.90/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-01 21:00:09.000000 uo_puddles-1.90/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 21:00:19.908265 uo_puddles-1.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 21:00:09.000000 uo_puddles-1.90/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-01 21:00:09.000000 uo_puddles-1.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 21:00:19.908265 uo_puddles-1.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-01 21:00:09.000000 uo_puddles-1.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:00:19.908265 uo_puddles-1.90/uo_puddles/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-01 21:00:09.000000 uo_puddles-1.90/uo_puddles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-08-01 21:00:09.000000 uo_puddles-1.90/uo_puddles/cis423.py
--rw-r--r--   0 runner    (1001) docker     (123)    26639 2023-08-01 21:00:09.000000 uo_puddles-1.90/uo_puddles/good_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-08-01 21:00:09.000000 uo_puddles-1.90/uo_puddles/good_ai_22.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-08-01 21:00:09.000000 uo_puddles-1.90/uo_puddles/gremcat_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-08-01 21:00:09.000000 uo_puddles-1.90/uo_puddles/gremcat_oo.py
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-08-01 21:00:09.000000 uo_puddles-1.90/uo_puddles/mlops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:00:19.908265 uo_puddles-1.90/uo_puddles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 21:00:19.000000 uo_puddles-1.90/uo_puddles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-01 21:00:19.000000 uo_puddles-1.90/uo_puddles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:00:19.000000 uo_puddles-1.90/uo_puddles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 21:00:19.000000 uo_puddles-1.90/uo_puddles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:06:03.313794 uo_puddles-1.91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-03 19:05:52.000000 uo_puddles-1.91/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-03 19:06:03.313794 uo_puddles-1.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 19:05:52.000000 uo_puddles-1.91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-03 19:05:52.000000 uo_puddles-1.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 19:06:03.313794 uo_puddles-1.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-03 19:05:52.000000 uo_puddles-1.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:06:03.313794 uo_puddles-1.91/uo_puddles/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-03 19:05:52.000000 uo_puddles-1.91/uo_puddles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-08-03 19:05:52.000000 uo_puddles-1.91/uo_puddles/cis423.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26639 2023-08-03 19:05:52.000000 uo_puddles-1.91/uo_puddles/good_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-08-03 19:05:52.000000 uo_puddles-1.91/uo_puddles/good_ai_22.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-08-03 19:05:52.000000 uo_puddles-1.91/uo_puddles/gremcat_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-08-03 19:05:52.000000 uo_puddles-1.91/uo_puddles/gremcat_oo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21492 2023-08-03 19:05:52.000000 uo_puddles-1.91/uo_puddles/mlops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:06:03.313794 uo_puddles-1.91/uo_puddles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-03 19:06:03.000000 uo_puddles-1.91/uo_puddles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-03 19:06:03.000000 uo_puddles-1.91/uo_puddles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:06:03.000000 uo_puddles-1.91/uo_puddles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 19:06:03.000000 uo_puddles-1.91/uo_puddles.egg-info/top_level.txt
```

### Comparing `uo_puddles-1.90/LICENSE.txt` & `uo_puddles-1.91/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.90/setup.py` & `uo_puddles-1.91/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="uo_puddles",
-    version="1.90",    #also change pypi_version variable at top of library
+    version="1.91",    #also change pypi_version variable at top of library
     author="Stephen Fickas",
     author_email="stephenfickas@gmail.com",
     description="for cis423 class",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `uo_puddles-1.90/uo_puddles/cis423.py` & `uo_puddles-1.91/uo_puddles/cis423.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.90/uo_puddles/good_ai.py` & `uo_puddles-1.91/uo_puddles/good_ai.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.90/uo_puddles/good_ai_22.py` & `uo_puddles-1.91/uo_puddles/good_ai_22.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.90/uo_puddles/gremcat_df.py` & `uo_puddles-1.91/uo_puddles/gremcat_df.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.90/uo_puddles/gremcat_oo.py` & `uo_puddles-1.91/uo_puddles/gremcat_oo.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.90/uo_puddles/mlops.py` & `uo_puddles-1.91/uo_puddles/mlops.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,56 +37,28 @@
     new_f = types.FunctionType(f.__code__, globals=new_globals, argdefs=f.__defaults__)
     new_f.__annotations__ = f.__annotations__ # for some reason annotations aren't copied over
     return new_f
 
   return wrap
 
 #drop by removing or keeping
-class DropColumnsTransformer(BaseEstimator, TransformerMixin):
-  def __init__(self, column_list, action='drop'):
-    assert action in ['keep', 'drop'], f'DropColumnsTransformer action {action} not in ["keep", "drop"]'
-    assert isinstance(column_list, list), f'DropColumnsTransformer expected list but saw {type(column_list)}'
-    self.column_list = column_list
-    self.action = action
 
-  #fill in rest below
-  def fit(self, X, y = None):
-    print(f"Warning: {self.__class__.__name__}.fit does nothing.")
-    return X
-
-  def transform(self, X):
-    assert isinstance(X, pd.core.frame.DataFrame), f'{self.__class__.__name__}.transform expected Dataframe but got {type(X)} instead.'
-    remaining_set = set(self.column_list) - set(X.columns)
-
-    X_ = X.copy()
-    if self.action=='drop':
-      if remaining_set:
-        print(f"\nWarning: {self.__class__.__name__} does not contain these columns to drop: {remaining_set}.")
-      X_ = X_.drop(columns=self.column_list, errors='ignore')
-    else:
-      assert not remaining_set, f'{self.__class__.__name__}.transform unknown columns to keep: {remaining_set}'
-      X_ = X_[self.column_list]
-    return X_
-
-  def fit_transform(self, X, y = None):
-    result = self.transform(X)
-    return result
   
 #This class maps values in a column, numeric or categorical.
 #Importantly, it does not change NaNs, leaving that for the imputer step.
-class MappingTransformer(BaseEstimator, TransformerMixin):
+class CustomMappingTransformer(BaseEstimator, TransformerMixin):
   
   def __init__(self, mapping_column, mapping_dict:dict):
     assert isinstance(mapping_dict, dict), f'{self.__class__.__name__} constructor expected dictionary but got {type(mapping_dict)} instead.'
     self.mapping_dict = mapping_dict
     self.mapping_column = mapping_column  #column to focus on
 
   def fit(self, X, y = None):
     print(f"\nWarning: {self.__class__.__name__}.fit does nothing.\n")
-    return X
+    return self
 
   def transform(self, X):
     assert isinstance(X, pd.core.frame.DataFrame), f'{self.__class__.__name__}.transform expected Dataframe but got {type(X)} instead.'
     assert self.mapping_column in X.columns.to_list(), f'{self.__class__.__name__}.transform unknown column "{self.mapping_column}"'  #column legit?
     
     #now check to see if all keys are contained in column
     column_set = set(X[self.mapping_column])
@@ -100,123 +72,167 @@
       print(f"\nWarning: {self.__class__.__name__}[{self.mapping_column}] these values in the column do not contain corresponing mapping keys: {keys_absent}\n")
 
     X_ = X.copy()
     X_[self.mapping_column].replace(self.mapping_dict, inplace=True)
     return X_
 
   def fit_transform(self, X, y = None):
+    #self.fit(X,y)
     result = self.transform(X)
     return result
     
 
-class OHETransformer(BaseEstimator, TransformerMixin):
+class CustomOHETransformer(BaseEstimator, TransformerMixin):
   def __init__(self, target_column, dummy_na=False, drop_first=False):  #False because worried about mismatched columns after splitting. Easier to add missing column.
     self.target_column = target_column
     self.dummy_na = dummy_na
     self.drop_first = drop_first
  
   def fit(self, X, y = None):
     print(f"Warning: {self.__class__.__name__}.fit does nothing.")
-    return X
+    return self
 
   def transform(self, X):
     assert isinstance(X, pd.core.frame.DataFrame), f'{self.__class__.__name__}.transform expected Dataframe but got {type(X)} instead.'
     assert self.target_column in X.columns.to_list(), f'{self.__class__.__name__}.transform unknown column {self.target_column}'
     X_ = X.copy()
     X_ = pd.get_dummies(X_, columns=[self.target_column],
                         dummy_na=self.dummy_na,
                         drop_first = self.drop_first)
     return X_
 
   def fit_transform(self, X, y = None):
+    #self.fit(X,y)
     result = self.transform(X)
     return result
   
 #This class will rename one or more columns.
-class RenamingTransformer(BaseEstimator, TransformerMixin):
+class CustomRenamingTransformer(BaseEstimator, TransformerMixin):
   #your __init__ method below
 
   def __init__(self, mapping_dict:dict):
     assert isinstance(mapping_dict, dict), f'{self.__class__.__name__} constructor expected dictionary but got {type(mapping_dict)} instead.' 
     self.mapping_dict = mapping_dict
 
+  def fit(self, X, y = None):
+    print(f"Warning: {self.__class__.__name__}.fit does nothing.")
+    return self
+
   #write the transform method without asserts. Again, maybe copy and paste from MappingTransformer and fix up.   
   def transform(self, X):
     assert isinstance(X, pd.core.frame.DataFrame), f'RenamingTransformer.transform expected Dataframe but got {type(X)} instead.'
     #your assert code below
 
     column_set = set(X.columns)
     not_found = set(self.mapping_dict.keys()) - column_set
     assert not not_found, f"Columns {not_found}, are not in the data table"
 
     X_ = X.copy()
     return X_.rename(columns=self.mapping_dict)
+
+  def fit_transform(self, X, y = None):
+    #self.fit(X,y)
+    result = self.transform(X)
+    return result
+
+class CustomPearsonTransformer(BaseEstimator, TransformerMixin):
+  def __init__(self, threshold):
+    self.threshold = threshold
+    self.correlated_columns = None
+
+  #define methods below
+
+  def fit(self, X, y = None):
+    df_corr = X.corr(method='pearson')
+    masked_df = df_corr.abs() > self.threshold
+    upper_mask = np.triu(masked_df, k=1)
+    self.correlated_columns = [c for i,c in enumerate(df_corr.columns) if upper_mask[:,i].any()]
+    return self
+
+  def transform(self, X):
+    assert isinstance(X, pd.core.frame.DataFrame), f'{self.__class__.__name__}.transform expected Dataframe but got {type(X)} instead.'
+    assert isinstance(self.correlated_columns, list), f'NotFittedError: This {self.__class__.__name__} instance is not fitted yet. Call "fit" with appropriate arguments before using this estimator.'
+
+    X_ = X.drop(columns=self.correlated_columns)
+    return X_
+
+  def fit_transform(self, X, y = None):
+    self.fit(X, y)
+    result = self.transform(X)
+    return result
   
 #chapter 4 asks for 2 new transformers
 
-class Sigma3Transformer(BaseEstimator, TransformerMixin):
-  def __init__(self, target_column):  
+class CustomSigma3Transformer(BaseEstimator, TransformerMixin):
+  def __init__(self, target_column):
     self.target_column = target_column
-    
+    self.high_wall = None
+    self.low_wall = None
+
   def fit(self, X, y = None):
-    print(f"Warning: {self.__class__.__name__}.fit does nothing.")
+    assert isinstance(X, pd.core.frame.DataFrame), f'{self.__class__.__name__}.fit expected Dataframe but got {type(X)} instead.'
+    assert self.target_column in X.columns.to_list(), f'{self.__class__.__name__}.fit unrecognizable column {self.target_column}.'
+    mean = X[self.target_column].mean()
+    sigma = X[self.target_column].std()
+    self.high_wall = float(mean + 3.0*sigma)
+    self.low_wall = mean - 3.0*sigma
     return self
 
   def transform(self, X):
     assert isinstance(X, pd.core.frame.DataFrame), f'{self.__class__.__name__}.transform expected Dataframe but got {type(X)} instead.'
+    assert isinstance(self.high_wall, float), f'{self.__class__.__name__}.transform appears no fit was called prior.'
+    assert self.target_column in X.columns.to_list(), f'{self.__class__.__name__}.transform unrecognizable column {self.target_column}.'
+
     X_ = X.copy()
-    mean = X_[self.target_column].mean()
-    sigma = X_[self.target_column].std()
-    high_wall = mean + 3*sigma
-    low_wall = mean - 3*sigma
-    #print(f'{self.__class__.__name__} mean, sigma, low_wall, high_wall: {round(mean, 2)}, {round(sigma, 2)}, {round(low_wall, 2)}, {round(high_wall, 2)}')
-    X_[self.target_column] = X_[self.target_column].clip(lower=low_wall, upper=high_wall)
+    X_[self.target_column] = X_[self.target_column].clip(lower=self.low_wall, upper=self.high_wall)
     return X_
 
   def fit_transform(self, X, y = None):
+    self.fit(X,y)
     result = self.transform(X)
     return result
 
-class TukeyTransformer(BaseEstimator, TransformerMixin):
+class CustomTukeyTransformer(BaseEstimator, TransformerMixin):
   def __init__(self, target_column, fence='outer'):
     assert fence in ['inner', 'outer']
     self.target_column = target_column
     self.fence = fence
-    
+    self.inner_low = None
+    self.outer_low = None
+    self.inner_high = None
+    self.outer_high = None
+
   def fit(self, X, y = None):
-    print(f"Warning: {self.__class__.__name__}.fit does nothing.")
+    assert isinstance(X, pd.core.frame.DataFrame), f'{self.__class__.__name__}.fit expected Dataframe but got {type(X)} instead.'
+    assert self.target_column in X.columns.to_list(), f'{self.__class__.__name__}.fit unrecognizable column {self.target_column}.'
+    q1 = X[self.target_column].quantile(0.25)
+    q3 = X[self.target_column].quantile(0.75)
+    iqr = q3-q1
+    self.inner_low = q1-1.5*iqr
+    self.outer_low = q1-3.0*iqr
+    self.inner_high = q3+1.5*iqr
+    self.outer_high = q3+3.0*iqr
     return self
 
   def transform(self, X):
     assert isinstance(X, pd.core.frame.DataFrame), f'{self.__class__.__name__}.transform expected Dataframe but got {type(X)} instead.'
-    if len(set(X[self.target_column]))<20:
-      print(f'{self.__class__.__name__} warning: {self.target_column} has less than 20 unique values. Consider it as categorical?')
-      
+    assert isinstance(self.inner_low, float), f'{self.__class__.__name__}.transform appears no fit was called prior.'
+    assert self.target_column in X.columns.to_list(), f'{self.__class__.__name__}.transform unrecognizable column {self.target_column}.'
+
     X_ = X.copy()
-    q1 = X_[self.target_column].quantile(0.25)
-    q3 = X_[self.target_column].quantile(0.75)
-    iqr = q3-q1
-    inner_low = q1-1.5*iqr
-    outer_low = q1-3*iqr
-    inner_high = q3+1.5*iqr
-    outer_high = q3+3*iqr
-    #print(f'{self.__class__.__name__} inner_low, inner_high, outer_low, outer_high: {round(inner_low, 2)}, {round(outer_low, 2)}, {round(inner_high, 2)}, {round(outer_high, 2)}')
     if self.fence=='inner':
-      X_[self.target_column] = X_[self.target_column].clip(lower=inner_low, upper=inner_high)
+      X_[self.target_column] = X_[self.target_column].clip(lower=self.inner_low, upper=self.inner_high)
     elif self.fence=='outer':
-      X_[self.target_column] = X_[self.target_column].clip(lower=outer_low, upper=outer_high)
+      X_[self.target_column] = X_[self.target_column].clip(lower=self.outer_low, upper=self.outer_high)
     else:
       assert False, f"fence has unrecognized value {self.fence}"
-      
-    if len(set(X_[self.target_column]))<5:
-      print(f'{self.__class__.__name__} warning: {self.target_column} has less than 5 unique values after clipping.')
-      
     return X_
 
   def fit_transform(self, X, y = None):
+    self.fit(X,y)
     result = self.transform(X)
     return result
 
 #chapter 5 asks for 1 new transformer
 
 class MinMaxTransformer(BaseEstimator, TransformerMixin):
   def __init__(self):
@@ -276,14 +292,43 @@
     return X_
 
   def fit_transform(self, X, y = None):
     self.fit(X,y)
     result = self.transform(X)
     return result
 
+class CustomRobustTransformer(BaseEstimator, TransformerMixin):
+  def __init__(self, column):
+    #fill in rest below
+    self.target_column = column
+    self.iqr = None
+    self.med = None
+
+  def fit(self, X, y = None):
+    assert isinstance(X, pd.core.frame.DataFrame), f'{self.__class__.__name__}.fit expected Dataframe but got {type(X)} instead.'
+    assert self.target_column in X.columns.to_list(), f'{self.__class__.__name__}.fit unrecognizable column {self.target_column}.'
+    self.iqr = float(X[self.target_column].quantile(.75) - X[self.target_column].quantile(.25))
+    self.med = X[self.target_column].median()
+    return self
+
+  def transform(self, X):
+    assert isinstance(X, pd.core.frame.DataFrame), f'{self.__class__.__name__}.transform expected Dataframe but got {type(X)} instead.'
+    assert isinstance(self.iqr, float), f'NotFittedError: This {self.__class__.__name__} instance is not fitted yet. Call "fit" with appropriate arguments before using this estimator.'
+    assert self.target_column in X.columns.to_list(), f'{self.__class__.__name__}.transform unrecognizable column {self.target_column}.'
+
+    X_ = X.copy()
+    X_[self.target_column] -= med
+    X_[self.target_column] /= iqr
+    return X_
+
+  def fit_transform(self, X, y = None):
+    self.fit(X,y)
+    result = self.transform(X)
+    return result
+
 ##added in chapter 6
 
 class KNNTransformer(BaseEstimator, TransformerMixin):
   def __init__(self,n_neighbors=5, weights="uniform"):
     #your code
     self.n_neighbors = n_neighbors
     self.weights=weights
```

