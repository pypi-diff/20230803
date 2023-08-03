# Comparing `tmp/Slpapy-0.4.4.tar.gz` & `tmp/Slpapy-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.4.4.tar", last modified: Thu Aug  3 01:03:47 2023, max compression
+gzip compressed data, was "Slpapy-0.4.5.tar", last modified: Thu Aug  3 05:51:40 2023, max compression
```

## Comparing `Slpapy-0.4.4.tar` & `Slpapy-0.4.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 01:03:47.453472 Slpapy-0.4.4/
--rw-rw-rw-   0        0        0      159 2023-08-03 01:03:47.452477 Slpapy-0.4.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-03 01:03:47.406598 Slpapy-0.4.4/Slpapy/
--rw-rw-rw-   0        0        0     3581 2023-06-16 07:08:20.000000 Slpapy-0.4.4/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.4.4/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-08-03 01:03:47.449483 Slpapy-0.4.4/Slpapy/Spatial_map_pic/
--rw-rw-rw-   0        0        0      645 2023-05-24 03:09:50.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/Spatial_map.py
--rw-rw-rw-   0        0        0       52 2023-05-10 02:09:04.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:24.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:24.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:24.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:24.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:24.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/readwrite.py
--rw-rw-rw-   0        0        0    43450 2023-05-24 03:01:38.000000 Slpapy-0.4.4/Slpapy/Spatial_map_pic/scatterplots.py
--rw-rw-rw-   0        0        0      263 2023-05-10 02:17:28.000000 Slpapy-0.4.4/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     7222 2023-08-02 10:20:51.000000 Slpapy-0.4.4/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-08-03 01:03:47.418566 Slpapy-0.4.4/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      159 2023-08-03 01:03:46.000000 Slpapy-0.4.4/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2023-08-03 01:03:47.000000 Slpapy-0.4.4/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 01:03:46.000000 Slpapy-0.4.4/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-08-03 01:03:46.000000 Slpapy-0.4.4/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-03 01:03:46.000000 Slpapy-0.4.4/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 01:03:47.453472 Slpapy-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-08-03 01:03:38.000000 Slpapy-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 05:51:40.199375 Slpapy-0.4.5/
+-rw-rw-rw-   0        0        0      159 2023-08-03 05:51:40.198376 Slpapy-0.4.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 05:51:40.150504 Slpapy-0.4.5/Slpapy/
+-rw-rw-rw-   0        0        0     3581 2023-06-16 07:08:20.000000 Slpapy-0.4.5/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.4.5/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-08-03 05:51:40.195384 Slpapy-0.4.5/Slpapy/Spatial_map_pic/
+-rw-rw-rw-   0        0        0      645 2023-05-24 03:09:50.000000 Slpapy-0.4.5/Slpapy/Spatial_map_pic/Spatial_map.py
+-rw-rw-rw-   0        0        0       52 2023-05-10 02:09:04.000000 Slpapy-0.4.5/Slpapy/Spatial_map_pic/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:24.000000 Slpapy-0.4.5/Slpapy/Spatial_map_pic/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:24.000000 Slpapy-0.4.5/Slpapy/Spatial_map_pic/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:24.000000 Slpapy-0.4.5/Slpapy/Spatial_map_pic/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.4.5/Slpapy/Spatial_map_pic/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.4.5/Slpapy/Spatial_map_pic/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.4.5/Slpapy/Spatial_map_pic/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:24.000000 Slpapy-0.4.5/Slpapy/Spatial_map_pic/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.4.5/Slpapy/Spatial_map_pic/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:24.000000 Slpapy-0.4.5/Slpapy/Spatial_map_pic/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.4.5/Slpapy/Spatial_map_pic/readwrite.py
+-rw-rw-rw-   0        0        0    43450 2023-05-24 03:01:38.000000 Slpapy-0.4.5/Slpapy/Spatial_map_pic/scatterplots.py
+-rw-rw-rw-   0        0        0      263 2023-05-10 02:17:28.000000 Slpapy-0.4.5/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     7409 2023-08-03 05:51:13.000000 Slpapy-0.4.5/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-08-03 05:51:40.162472 Slpapy-0.4.5/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-08-03 05:51:39.000000 Slpapy-0.4.5/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-08-03 05:51:39.000000 Slpapy-0.4.5/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 05:51:39.000000 Slpapy-0.4.5/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-08-03 05:51:39.000000 Slpapy-0.4.5/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-03 05:51:39.000000 Slpapy-0.4.5/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 05:51:40.199375 Slpapy-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-08-03 05:51:23.000000 Slpapy-0.4.5/setup.py
```

### Comparing `Slpapy-0.4.4/Slpapy/Data_reconstruction.py` & `Slpapy-0.4.5/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.4/Slpapy/MZ_ppm_match.py` & `Slpapy-0.4.5/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.4/Slpapy/Spatial_map_pic/Spatial_map.py` & `Slpapy-0.4.5/Slpapy/Spatial_map_pic/Spatial_map.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.4/Slpapy/Spatial_map_pic/_compat.py` & `Slpapy-0.4.5/Slpapy/Spatial_map_pic/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.4/Slpapy/Spatial_map_pic/_docs.py` & `Slpapy-0.4.5/Slpapy/Spatial_map_pic/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.4/Slpapy/Spatial_map_pic/_rcmod.py` & `Slpapy-0.4.5/Slpapy/Spatial_map_pic/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.4/Slpapy/Spatial_map_pic/_settings.py` & `Slpapy-0.4.5/Slpapy/Spatial_map_pic/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.4/Slpapy/Spatial_map_pic/_utils.py` & `Slpapy-0.4.5/Slpapy/Spatial_map_pic/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.4/Slpapy/Spatial_map_pic/beats.py` & `Slpapy-0.4.5/Slpapy/Spatial_map_pic/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.4/Slpapy/Spatial_map_pic/is_constant.py` & `Slpapy-0.4.5/Slpapy/Spatial_map_pic/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.4/Slpapy/Spatial_map_pic/logging.py` & `Slpapy-0.4.5/Slpapy/Spatial_map_pic/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.4/Slpapy/Spatial_map_pic/palettes.py` & `Slpapy-0.4.5/Slpapy/Spatial_map_pic/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.4/Slpapy/Spatial_map_pic/readwrite.py` & `Slpapy-0.4.5/Slpapy/Spatial_map_pic/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.4/Slpapy/Spatial_map_pic/scatterplots.py` & `Slpapy-0.4.5/Slpapy/Spatial_map_pic/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.4/Slpapy/processing_analyze.py` & `Slpapy-0.4.5/Slpapy/processing_analyze.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,22 +54,22 @@
     # 保存mz值
     mz = adata.var
     mz.to_csv('./mz.csv')
     adata.write('./pp_done.h5ad')
     return adata
 
 
-def se_analyze(adata, n_neighbors, n_pcs, resolution):
+def se_analyze(adata, n_neighbors, n_pcs, resolution,min_dist, alpha, spread):
     # 将每个脂质缩放到单位方差。阈值超过标准偏差 10。，如非高斯分布，则不建议使用
     # sc.pp.scale(adata, max_value=10)
     # 绘制 PCA 图降维
     sc.tl.pca(adata, svd_solver='arpack')  #
     # Neighborhood graph使用数据矩阵的 PCA 表示来计算细胞的邻域图
     sc.pp.neighbors(adata, n_neighbors=n_neighbors, n_pcs=n_pcs, )
-    sc.tl.umap(adata, min_dist=0.01, alpha=1, spread=2)  #
+    sc.tl.umap(adata, min_dist=min_dist, alpha=alpha, spread=spread)  #
     # Leiden 图聚类
     # 计算
     sc.tl.leiden(adata, resolution=resolution)
     return adata
 
 
 def third_analyze(adata):
@@ -93,26 +93,28 @@
         adata: ad.AnnData,
         *,
         use_spacial: bool = False,
         orgknn: bool = False,
         onlyhighly: bool = False,
         n_neighbors: int = 20,
         n_pcs: int = 30,
-        resolution: int = 0.8
-
+        resolution: int = 0.8,
+        min_dist: int =0.01,
+        alpha: int =1,
+        spread: int =2,
 ) -> Optional[ad.AnnData]:
     adata = pp_analyze(adata, onlyhighly)
     if use_spacial == True:
         adata = XYadata(adata)
-        adata = se_analyze(adata, n_neighbors, n_pcs, resolution)
+        adata = se_analyze(adata, n_neighbors, n_pcs, resolution,min_dist, alpha, spread)
         adata = third_analyze(adata)
         adata.obs['leidenXY'] = adata.obs['leiden']
         Spatial_map(adata, 'leidenXY')
     elif orgknn == True:
-        adata = se_analyze(adata, n_neighbors, n_pcs, resolution)
+        adata = se_analyze(adata, n_neighbors, n_pcs, resolution,min_dist, alpha, spread)
         estimator = KMeans(n_clusters=adata.obs['leiden'].values.codes.max() + 1)  # 构造聚类器
         estimator.fit(
             np.c_[adata.X, preprocessing.normalize(np.c_[np.array(adata.obs['X']), np.array(adata.obs['Y'])])])
         label_pred = estimator.labels_  # 获取聚类标签
         adata.obs['KNNlableXY'] = label_pred.T
         adata.obs['KNNlableXY'] = adata.obs['KNNlableXY'].astype('category')
         sc.tl.rank_genes_groups(adata, 'KNNlableXY', method='wilcoxon')
@@ -123,15 +125,15 @@
         res = pd.DataFrame({group + '_' + key: result[key][group] for group in groups for key in
                             ['names', 'pvals', 'logfoldchanges', 'pvals_adj', 'scores']})
         res.to_csv("dif.csv")
         sc.pl.pca_variance_ratio(adata, log=True, save='_KXY.png')
         sc.pl.umap(adata, color=['KNNlableXY'], save='_KXY.png')
         Spatial_map(adata, 'KNNlableXY')
     else:
-        adata = se_analyze(adata, n_neighbors, n_pcs, resolution)
+        adata = se_analyze(adata, n_neighbors, n_pcs, resolution,min_dist, alpha, spread)
         adata = third_analyze(adata)
         Spatial_map(adata, 'leiden')
 
     Spatial_class_location(adata, 'leiden')
     adata.write('./analyze_done.h5ad')
     return adata
```

### Comparing `Slpapy-0.4.4/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.4.5/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

