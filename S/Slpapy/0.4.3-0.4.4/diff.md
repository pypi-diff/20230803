# Comparing `tmp/Slpapy-0.4.3.tar.gz` & `tmp/Slpapy-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.4.3.tar", last modified: Mon Jul 10 02:12:52 2023, max compression
+gzip compressed data, was "Slpapy-0.4.4.tar", last modified: Thu Aug  3 01:03:47 2023, max compression
```

## Comparing `Slpapy-0.4.3.tar` & `Slpapy-0.4.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 02:12:52.220468 Slpapy-0.4.3/
--rw-rw-rw-   0        0        0      159 2023-07-10 02:12:52.219471 Slpapy-0.4.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-10 02:12:52.150656 Slpapy-0.4.3/Slpapy/
--rw-rw-rw-   0        0        0     3581 2023-06-16 07:08:20.000000 Slpapy-0.4.3/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.4.3/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-07-10 02:12:52.215482 Slpapy-0.4.3/Slpapy/Spatial_map_pic/
--rw-rw-rw-   0        0        0      645 2023-05-24 03:09:50.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/Spatial_map.py
--rw-rw-rw-   0        0        0       52 2023-05-10 02:09:04.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:24.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:24.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:24.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:24.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:24.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/readwrite.py
--rw-rw-rw-   0        0        0    43450 2023-05-24 03:01:38.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/scatterplots.py
--rw-rw-rw-   0        0        0      263 2023-05-10 02:17:28.000000 Slpapy-0.4.3/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     6880 2023-06-28 10:02:50.000000 Slpapy-0.4.3/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-07-10 02:12:52.167610 Slpapy-0.4.3/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      159 2023-07-10 02:12:51.000000 Slpapy-0.4.3/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2023-07-10 02:12:51.000000 Slpapy-0.4.3/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 02:12:51.000000 Slpapy-0.4.3/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-07-10 02:12:51.000000 Slpapy-0.4.3/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-10 02:12:51.000000 Slpapy-0.4.3/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 02:12:52.220468 Slpapy-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-07-10 02:12:42.000000 Slpapy-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:03:47.453472 Slpapy-0.4.4/
+-rw-rw-rw-   0        0        0      159 2023-08-03 01:03:47.452477 Slpapy-0.4.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 01:03:47.406598 Slpapy-0.4.4/Slpapy/
+-rw-rw-rw-   0        0        0     3581 2023-06-16 07:08:20.000000 Slpapy-0.4.4/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.4.4/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:03:47.449483 Slpapy-0.4.4/Slpapy/Spatial_map_pic/
+-rw-rw-rw-   0        0        0      645 2023-05-24 03:09:50.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/Spatial_map.py
+-rw-rw-rw-   0        0        0       52 2023-05-10 02:09:04.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:24.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:24.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:24.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:24.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:24.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/readwrite.py
+-rw-rw-rw-   0        0        0    43450 2023-05-24 03:01:38.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/scatterplots.py
+-rw-rw-rw-   0        0        0      263 2023-05-10 02:17:28.000000 Slpapy-0.4.4/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     7222 2023-08-02 10:20:51.000000 Slpapy-0.4.4/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:03:47.418566 Slpapy-0.4.4/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-08-03 01:03:46.000000 Slpapy-0.4.4/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-08-03 01:03:47.000000 Slpapy-0.4.4/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 01:03:46.000000 Slpapy-0.4.4/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-08-03 01:03:46.000000 Slpapy-0.4.4/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-03 01:03:46.000000 Slpapy-0.4.4/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 01:03:47.453472 Slpapy-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-08-03 01:03:38.000000 Slpapy-0.4.4/setup.py
```

### Comparing `Slpapy-0.4.3/Slpapy/Data_reconstruction.py` & `Slpapy-0.4.4/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.3/Slpapy/MZ_ppm_match.py` & `Slpapy-0.4.4/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.3/Slpapy/Spatial_map_pic/Spatial_map.py` & `Slpapy-0.4.4/Slpapy/Spatial_map_pic/Spatial_map.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.3/Slpapy/Spatial_map_pic/_compat.py` & `Slpapy-0.4.4/Slpapy/Spatial_map_pic/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.3/Slpapy/Spatial_map_pic/_docs.py` & `Slpapy-0.4.4/Slpapy/Spatial_map_pic/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.3/Slpapy/Spatial_map_pic/_rcmod.py` & `Slpapy-0.4.4/Slpapy/Spatial_map_pic/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.3/Slpapy/Spatial_map_pic/_settings.py` & `Slpapy-0.4.4/Slpapy/Spatial_map_pic/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.3/Slpapy/Spatial_map_pic/_utils.py` & `Slpapy-0.4.4/Slpapy/Spatial_map_pic/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.3/Slpapy/Spatial_map_pic/beats.py` & `Slpapy-0.4.4/Slpapy/Spatial_map_pic/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.3/Slpapy/Spatial_map_pic/is_constant.py` & `Slpapy-0.4.4/Slpapy/Spatial_map_pic/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.3/Slpapy/Spatial_map_pic/logging.py` & `Slpapy-0.4.4/Slpapy/Spatial_map_pic/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.3/Slpapy/Spatial_map_pic/palettes.py` & `Slpapy-0.4.4/Slpapy/Spatial_map_pic/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.3/Slpapy/Spatial_map_pic/readwrite.py` & `Slpapy-0.4.4/Slpapy/Spatial_map_pic/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.3/Slpapy/Spatial_map_pic/scatterplots.py` & `Slpapy-0.4.4/Slpapy/Spatial_map_pic/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.3/Slpapy/processing_analyze.py` & `Slpapy-0.4.4/Slpapy/processing_analyze.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import pandas as pd
 import scanpy as sc
 from scipy.sparse import csr_matrix
 from sklearn import preprocessing
 from sklearn.cluster import KMeans
 from .Spatial_map_pic import Spatial_map,Spatial_class_location
-
+from .Spatial_map_pic.scatterplots import embedding
 sc.settings.verbosity = 3  # 设置日志等级: errors (0), warnings (1), info (2), hints (3)
 sc.logging.print_header()
 sc.settings.set_figure_params(dpi=720, facecolor='white')
 
 
 def XYadata(adata):
     df = preprocessing.normalize(np.c_[np.array(adata.obs['X']), np.array(adata.obs['Y'])])
@@ -132,26 +132,36 @@
         Spatial_map(adata, 'leiden')
 
     Spatial_class_location(adata, 'leiden')
     adata.write('./analyze_done.h5ad')
     return adata
 
 
-#选择上方函数返回的adata数据中obs,根据选择筛选后进行比较
-def cluster_compare(
+def significant_feature_pic(
         adata: ad.AnnData,
-        list1: list,
-        list2: list,
-) -> Optional[ad.AnnData]:
-    #选择上方函数返回的adata数据中obs,根据选择筛选后进行比较
-    bdata = adata[adata.obs['leiden'].isin(list1 + list2), :]
-    #对于bdata中的list1和list2在bdata.obs['leidens']进行重新编号
-    bdata.obs['leidens'] = bdata.obs['leiden'].cat.rename_categories(
-        {i: 'list1' for i in list1} | {i: 'list2' for i in list2})
-    Spatial_map(bdata, 'leidens')
-    sc.pl.rank_genes_groups(bdata, n_genes=25, sharey=False, save='_Wilcoxon.png')
-    sc.pl.rank_genes_groups_dotplot(bdata, n_genes=10, save='_dotplot_Wilcoxon.png')
-    return bdata
+        names: str = None,
+        n_genes: int = 5,
+        ):
+    result = adata.uns['rank_genes_groups']
+
+    if names == None:
+        #结束本函数
+        return print("Please input the name of the cluster")
+    if names not in result['names'].dtype.names:
+        return print("Please input the right name of the cluster")
 
 
+    result = adata.uns['rank_genes_groups']
+    res = pd.DataFrame({key: result[key][names] for key in
+                        ['names', 'pvals', 'logfoldchanges', 'pvals_adj', 'scores']})
+    # 查找res中scores最大的前n_genes个基因的名字形成列表
+    res = res.sort_values(by='scores', ascending=False)
+    res = res.iloc[:n_genes, :]
+    # 在adata.var['m/z']中查找res中的基因名字对应的m/z值
+    res['m/z'] = [adata.var.loc[i, 'm/z'] for i in res['names']]
+    for i in res.index:
+        embedding(adata, basis='X_spacial', color=f"{res.loc[i, 'names']}",
+                     frameon=False, save=f"{res.loc[i, 'm/z']}.png")
+
+    return
```

### Comparing `Slpapy-0.4.3/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.4.4/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

