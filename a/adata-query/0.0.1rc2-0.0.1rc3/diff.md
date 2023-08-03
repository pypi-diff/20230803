# Comparing `tmp/adata_query-0.0.1rc2.tar.gz` & `tmp/adata_query-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adata_query-0.0.1rc2.tar", last modified: Thu Aug  3 14:33:41 2023, max compression
+gzip compressed data, was "adata_query-0.0.1rc3.tar", last modified: Thu Aug  3 15:24:52 2023, max compression
```

## Comparing `adata_query-0.0.1rc2.tar` & `adata_query-0.0.1rc3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:33:41.084382 adata_query-0.0.1rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 14:33:41.084382 adata_query-0.0.1rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:33:41.080381 adata_query-0.0.1rc2/adata_query/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/adata_query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:33:41.084382 adata_query-0.0.1rc2/adata_query/_core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/adata_query/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/adata_query/_core/_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/adata_query/_core/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/adata_query/_core/_locator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:33:41.084382 adata_query-0.0.1rc2/adata_query/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/adata_query/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/adata_query/_utils/_info_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:33:41.084382 adata_query-0.0.1rc2/adata_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 14:33:41.000000 adata_query-0.0.1rc2/adata_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-03 14:33:41.000000 adata_query-0.0.1rc2/adata_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:33:41.000000 adata_query-0.0.1rc2/adata_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 14:33:41.000000 adata_query-0.0.1rc2/adata_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 14:33:41.000000 adata_query-0.0.1rc2/adata_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:33:41.084382 adata_query-0.0.1rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:24:52.955311 adata_query-0.0.1rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 15:24:52.955311 adata_query-0.0.1rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:24:52.955311 adata_query-0.0.1rc3/adata_query/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/adata_query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:24:52.955311 adata_query-0.0.1rc3/adata_query/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/adata_query/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/adata_query/_core/_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/adata_query/_core/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/adata_query/_core/_locator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:24:52.955311 adata_query-0.0.1rc3/adata_query/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/adata_query/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/adata_query/_utils/_info_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:24:52.955311 adata_query-0.0.1rc3/adata_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 15:24:52.000000 adata_query-0.0.1rc3/adata_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-03 15:24:52.000000 adata_query-0.0.1rc3/adata_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:24:52.000000 adata_query-0.0.1rc3/adata_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 15:24:52.000000 adata_query-0.0.1rc3/adata_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 15:24:52.000000 adata_query-0.0.1rc3/adata_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:24:52.955311 adata_query-0.0.1rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/setup.py
```

### Comparing `adata_query-0.0.1rc2/LICENSE` & `adata_query-0.0.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc2/PKG-INFO` & `adata_query-0.0.1rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata_query
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: Fetch and format data matrices from AnnData.
 Home-page: https://github.com/mvinyard/AnnDataQuery
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `adata_query-0.0.1rc2/README.md` & `adata_query-0.0.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc2/adata_query/_core/_fetcher.py` & `adata_query-0.0.1rc3/adata_query/_core/_fetcher.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 
 # -- import packages: ----------------------------------------------------------
 import ABCParse
 import autodevice
 import anndata
 import torch as _torch
+import numpy as np
 
 
 # -- import local dependencies: ------------------------------------------------
 from ._locator import locate
 from ._formatter import format_data
 
 
 # -- set typing: ---------------------------------------------------------------
-from typing import Optional
+from typing import Dict, List, Optional, Union
 
 
 # -- operational class: --------------------------------------------------------
 class AnnDataFetcher(ABCParse.ABCParse):
     """Operational class powering the fetch function."""
     def __init__(self, *args, **kwargs):
 
@@ -27,90 +28,125 @@
         return self._adata.obs.groupby(self._groupby)
 
     def _forward(self, adata, key):
         data = getattr(adata, locate(adata, key))[key]
         return format_data(data=data, torch = self._torch, device = self._device)
 
     def _grouped_subroutine(self, adata, key):
-        for group, group_df in self._GROUPED:
-            yield self._forward(adata[group_df.index], key)
+        if self._as_dict:
+            for group, group_df in self._GROUPED:
+                yield group, self._forward(adata[group_df.index], key)
+        else:
+            for group, group_df in self._GROUPED:
+                yield self._forward(adata[group_df.index], key)
 
     def __call__(
         self,
         adata: anndata.AnnData,
         key: str,
         groupby: Optional[str] = None,
         torch: bool = False,
         device: _torch.device = autodevice.AutoDevice(),
+        as_dict: bool = True,
     ):
         """
-        adata: anndata.AnnData [required]
+        adata: anndata.AnnData [ required ]
+            Annotated single-cell data object.
         
-        key: str [required]
+        key: str [ required ]
+            Key to access a matrix in adata. For example, if you wanted to access
+            adata.obsm['X_pca'], you would pass: "X_pca".
         
         groupby: Optional[str], default = None
-        
+            Optionally, one may choose to group data according to a cell-specific
+            annotation in adata.obs. This would invoke returning data as List
+            
         torch: bool, default = False
-        
+            Boolean indicator of whether data should be formatted as torch.Tensor. If
+            False (default), data is formatted as np.ndarray.device (torch.device) =
+            autodevice.AutoDevice(). Should torch=True, the device ("cpu", "cuda:N", 
+            "mps:N") may be set. The default value, autodevice.AutoDevice() will 
+            indicate the use of GPU, if available.
+
         device: torch.device, default = autodevice.AutoDevice()
+            
+    
+        as_dict: bool, default = True
+            Only relevant when `groupby` is not None. Boolean indicator to return
+            data in a Dict where the key for each value corresponds to the respective
+            `groupby` value. If False, returns List.
         """
 
         self.__update__(locals(), public=[None])
 
         if hasattr(self, "_groupby"):
+            if self._as_dict:
+                return dict(self._grouped_subroutine(adata, key))
             return list(self._grouped_subroutine(adata, key))
         return self._forward(adata, key)
 
 def fetch(
     adata: anndata.AnnData,
     key: str,
     groupby: Optional[str] = None,
     torch: bool = False,
     device: _torch.device = autodevice.AutoDevice(),
+    as_dict: bool = True,
     *args,
     **kwargs,
-):
+) -> Union[
+    _torch.Tensor,
+    np.ndarray,
+    List[Union[_torch.Tensor, np.ndarray]],
+    Dict[Union[str, int], Union[_torch.Tensor, np.ndarray]],
+]:
     """
     Given, adata and a key that points to a specific matrix stored in adata,
     return the data, formatted either as np.ndarray or torch.Tensor. If formatted
     as torch.Tensor, device may be specified based on available devices.
-    
+
     Parameters
     ----------
     adata: anndata.AnnData [ required ]
         Annotated single-cell data object.
-        
+
     key: str [ required ]
         Key to access a matrix in adata. For example, if you wanted to access
         adata.obsm['X_pca'], you would pass: "X_pca".
-    
+
     groupby: Optional[str], default = None
         Optionally, one may choose to group data according to a cell-specific
         annotation in adata.obs. This would invoke returning data as List
-        
+
     torch: bool, default = False
         Boolean indicator of whether data should be formatted as torch.Tensor. If
         False (default), data is formatted as np.ndarray.device (torch.device) =
-        autodevice.AutoDevice(). Should torch=True, the device ("cpu", "cuda:N", 
-        "mps:N") may be set. The default value, autodevice.AutoDevice() will 
+        autodevice.AutoDevice(). Should torch=True, the device ("cpu", "cuda:N",
+        "mps:N") may be set. The default value, autodevice.AutoDevice() will
         indicate the use of GPU, if available.
-    
+
+    as_dict: bool, default = True
+        Only relevant when `groupby` is not None. Boolean indicator to return
+        data in a Dict where the key for each value corresponds to the respective
+        `groupby` value. If False, returns List.
+
     Returns
     -------
-    data: Union[torch.Tensor, np.ndarray, List[torch.Tensor], List[np.ndarray]
+    data: Union[torch.Tensor, np.ndarray, List[Union[torch.Tensor, np.ndarray]], Dict[Union[str, int], Union[torch.Tensor, np.ndarray]]
         Formatted data as np.ndarray or torch.Tensor. If torch=True the torch.Tensor
-        is allocated to the device indicated by the device argument. If groupby is passed,
-        returned as a List[np.ndarray] or List[torch.Tensor]
+        is allocated to the device indicated by the device argument. If `groupby` is passed,
+        returned as Dict[np.ndarray] or Dict[torch.Tensor]. If groupby is passed and `as_dict`
+        = False, returns List[np.ndarray] or List[torch.Tensor].
     """
-    
-    
+
     fetcher = AnnDataFetcher()
-    
+
     return fetcher(
-        adata = adata,
-        key = key,
-        groupby = groupby,
-        torch = torch,
-        device = device,
+        adata=adata,
+        key=key,
+        groupby=groupby,
+        torch=torch,
+        device=device,
+        as_dict=as_dict,
         *args,
         **kwargs,
-    )
+    )
```

### Comparing `adata_query-0.0.1rc2/adata_query/_core/_formatter.py` & `adata_query-0.0.1rc3/adata_query/_core/_formatter.py`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc2/adata_query/_core/_locator.py` & `adata_query-0.0.1rc3/adata_query/_core/_locator.py`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc2/adata_query/_utils/_info_message.py` & `adata_query-0.0.1rc3/adata_query/_utils/_info_message.py`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc2/adata_query.egg-info/PKG-INFO` & `adata_query-0.0.1rc3/adata_query.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata-query
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: Fetch and format data matrices from AnnData.
 Home-page: https://github.com/mvinyard/AnnDataQuery
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `adata_query-0.0.1rc2/setup.py` & `adata_query-0.0.1rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import sys
 
 
 # -- run setup: ----------------------------------------------------------------
 setuptools.setup(
     name="adata_query",
-    version="0.0.1rc2",
+    version="0.0.1rc3",
     python_requires=">3.9.0",
     author="Michael E. Vinyard",
     author_email="mvinyard.ai@gmail.com",
     url="https://github.com/mvinyard/AnnDataQuery",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="Fetch and format data matrices from AnnData.",
```

