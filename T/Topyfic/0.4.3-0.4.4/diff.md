# Comparing `tmp/Topyfic-0.4.3.tar.gz` & `tmp/Topyfic-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Topyfic-0.4.3.tar", last modified: Wed Jul 26 22:28:12 2023, max compression
+gzip compressed data, was "Topyfic-0.4.4.tar", last modified: Wed Aug  2 23:22:22 2023, max compression
```

## Comparing `Topyfic-0.4.3.tar` & `Topyfic-0.4.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-07-26 22:28:12.410627 Topyfic-0.4.3/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.4.3/LICENSE.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-07-26 22:28:12.410703 Topyfic-0.4.3/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.4.3/README.md
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-07-26 22:28:12.409497 Topyfic-0.4.3/Topyfic/
--rw-rw-r--   0 nargesrezaie   (501) staff       (20)      197 2023-06-01 18:15:16.000000 Topyfic-0.4.3/Topyfic/__init__.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    45223 2023-07-26 22:27:24.000000 Topyfic-0.4.3/Topyfic/analysis.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     4087 2023-06-01 18:15:16.000000 Topyfic-0.4.3/Topyfic/main.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    13776 2023-06-05 22:53:45.000000 Topyfic-0.4.3/Topyfic/topModel.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     8982 2023-06-01 18:15:16.000000 Topyfic-0.4.3/Topyfic/topic.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    10440 2023-05-31 22:59:19.000000 Topyfic-0.4.3/Topyfic/train.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    19189 2023-07-14 01:34:33.000000 Topyfic-0.4.3/Topyfic/utilsAnalyseModel.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    21560 2023-07-25 22:29:44.000000 Topyfic-0.4.3/Topyfic/utilsMakeModel.py
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-07-26 22:28:12.410495 Topyfic-0.4.3/Topyfic.egg-info/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-07-26 22:28:12.000000 Topyfic-0.4.3/Topyfic.egg-info/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      359 2023-07-26 22:28:12.000000 Topyfic-0.4.3/Topyfic.egg-info/SOURCES.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-07-26 22:28:12.000000 Topyfic-0.4.3/Topyfic.egg-info/dependency_links.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      280 2023-07-26 22:28:12.000000 Topyfic-0.4.3/Topyfic.egg-info/requires.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-07-26 22:28:12.000000 Topyfic-0.4.3/Topyfic.egg-info/top_level.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-07-26 22:28:12.410968 Topyfic-0.4.3/setup.cfg
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     2018 2023-07-26 22:27:50.000000 Topyfic-0.4.3/setup.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-08-02 23:22:22.333002 Topyfic-0.4.4/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.4.4/LICENSE.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-08-02 23:22:22.333093 Topyfic-0.4.4/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.4.4/README.md
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-08-02 23:22:22.331805 Topyfic-0.4.4/Topyfic/
+-rw-rw-r--   0 nargesrezaie   (501) staff       (20)      197 2023-06-01 18:15:16.000000 Topyfic-0.4.4/Topyfic/__init__.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    45223 2023-07-26 22:27:24.000000 Topyfic-0.4.4/Topyfic/analysis.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     4087 2023-06-01 18:15:16.000000 Topyfic-0.4.4/Topyfic/main.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    13776 2023-06-05 22:53:45.000000 Topyfic-0.4.4/Topyfic/topModel.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     8982 2023-06-01 18:15:16.000000 Topyfic-0.4.4/Topyfic/topic.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    10440 2023-05-31 22:59:19.000000 Topyfic-0.4.4/Topyfic/train.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    19277 2023-08-02 23:12:10.000000 Topyfic-0.4.4/Topyfic/utilsAnalyseModel.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    21648 2023-08-01 19:47:14.000000 Topyfic-0.4.4/Topyfic/utilsMakeModel.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-08-02 23:22:22.332850 Topyfic-0.4.4/Topyfic.egg-info/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-08-02 23:22:22.000000 Topyfic-0.4.4/Topyfic.egg-info/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      359 2023-08-02 23:22:22.000000 Topyfic-0.4.4/Topyfic.egg-info/SOURCES.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-08-02 23:22:22.000000 Topyfic-0.4.4/Topyfic.egg-info/dependency_links.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      280 2023-08-02 23:22:22.000000 Topyfic-0.4.4/Topyfic.egg-info/requires.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-08-02 23:22:22.000000 Topyfic-0.4.4/Topyfic.egg-info/top_level.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-08-02 23:22:22.333356 Topyfic-0.4.4/setup.cfg
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     2018 2023-08-02 23:21:15.000000 Topyfic-0.4.4/setup.py
```

### Comparing `Topyfic-0.4.3/LICENSE.txt` & `Topyfic-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Topyfic-0.4.3/PKG-INFO` & `Topyfic-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.4.3
+Version: 0.4.4
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.3.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.4.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
 Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network,Topic Modeling,single-nucleus RNA-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `Topyfic-0.4.3/README.md` & `Topyfic-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `Topyfic-0.4.3/Topyfic/analysis.py` & `Topyfic-0.4.4/Topyfic/analysis.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.4.3/Topyfic/main.py` & `Topyfic-0.4.4/Topyfic/main.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.4.3/Topyfic/topModel.py` & `Topyfic-0.4.4/Topyfic/topModel.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.4.3/Topyfic/topic.py` & `Topyfic-0.4.4/Topyfic/topic.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.4.3/Topyfic/train.py` & `Topyfic-0.4.4/Topyfic/train.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.4.3/Topyfic/utilsAnalyseModel.py` & `Topyfic-0.4.4/Topyfic/utilsAnalyseModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,18 @@
                                          nodePos,
                                          edge_labels=edge_labels,
                                          font_size=7,
                                          ax=ax)
 
             i += 1
 
-        [axi.axis('off') for axi in axs.ravel()]
+        if len(connected_components) == 1:
+            ax.axis('off')
+        else:
+            [axi.axis('off') for axi in axs.ravel()]
         plt.tight_layout()
         if save:
             plt.savefig(f"{file_name}.{plot_format}")
         if plot_show:
             plt.show()
         else:
             plt.close()
```

### Comparing `Topyfic-0.4.3/Topyfic/utilsMakeModel.py` & `Topyfic-0.4.4/Topyfic/utilsMakeModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     return data
 
 
 def calculate_leiden_clustering(trains,
                                 data,
                                 n_top_genes=50,
                                 resolution=1,
+                                max_iter_harmony=10,
                                 min_cell_participation=None,
                                 file_format="pdf"):
     """
     Do leiden clustering w/o harmony base on number of assays you have and then remove low participation topics
 
     :param trains: list of train class
     :type trains: list of Train
@@ -208,15 +209,15 @@
 
     else:
         adata = anndata.AnnData(all_components)
         adata.obs['assays'] = all_batches
         sc.pp.log1p(adata)
         sc.pp.highly_variable_genes(adata, n_top_genes=n_top_genes)
         sc.pp.neighbors(adata)
-        sce.pp.harmony_integrate(adata, 'assays')
+        sce.pp.harmony_integrate(adata, 'assays', max_iter_harmony=max_iter_harmony)
         adata.obsm['X_pca'] = adata.obsm['X_pca_harmony']
         sc.pp.neighbors(adata)
         sc.tl.umap(adata)
         sc.tl.leiden(adata, resolution=resolution)
         adata.obs["topics"] = adata.obs["leiden"].astype(int) + 1
         adata.obs["topics"] = "Topic_" + adata.obs["topics"].astype(str)
         sc.pl.umap(adata, color=['topics'],
```

### Comparing `Topyfic-0.4.3/Topyfic.egg-info/PKG-INFO` & `Topyfic-0.4.4/Topyfic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.4.3
+Version: 0.4.4
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.3.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.4.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
 Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network,Topic Modeling,single-nucleus RNA-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `Topyfic-0.4.3/setup.py` & `Topyfic-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name='Topyfic',  # the name of your package
     packages=['Topyfic'],  # same as above
-    version='v0.4.3',  # version number
+    version='v0.4.4',  # version number
     license='MIT',  # license type
     description='Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) '
                 'using leiden clustering and harmony for single cell epigenomics data',
     # short description
     author='Narges Rezaie',  # your name
     author_email='nargesrezaie80@gmail.com',  # your email
     url='https://github.com/mortazavilab/Topyfic',  # url to your git repo
-    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.3.tar.gz',  # link to the tar.gz file associated with this release
+    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.4.tar.gz',  # link to the tar.gz file associated with this release
     keywords=['Cellular Programs', 'Latent Dirichlet allocation', 'single-cell multiome', 'single-cell RNA-seq',
               'gene regulatory network', 'Topic Modeling', 'single-nucleus RNA-seq'],  #
     python_requires='>=3.8',
     install_requires=[  # these can also include >, <, == to enforce version compatibility
         'pandas>=1.4.4',  # make sure the packages you put here are those NOT included in the base python distribution
         'scikit-learn>=0.24.2',
         'pytest',
```

