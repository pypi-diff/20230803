# Comparing `tmp/xaitk-saliency-demo-2.2.3.tar.gz` & `tmp/xaitk-saliency-demo-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xaitk-saliency-demo-2.2.3.tar", last modified: Fri Jul 21 16:41:17 2023, max compression
+gzip compressed data, was "xaitk-saliency-demo-2.3.0.tar", last modified: Thu Aug  3 19:51:37 2023, max compression
```

## Comparing `xaitk-saliency-demo-2.2.3.tar` & `xaitk-saliency-demo-2.3.0.tar`

### file list

```diff
@@ -1,37 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:41:17.772419 xaitk-saliency-demo-2.2.3/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2724 2023-07-21 16:41:17.772419 xaitk-saliency-demo-2.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1942 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/README.rst
--rw-r--r--   0 root         (0) root         (0)     1380 2023-07-21 16:41:17.772419 xaitk-saliency-demo-2.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:41:17.764418 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:41:17.768418 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/__init__.py
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:41:17.772419 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/
--rw-r--r--   0 root         (0) root         (0)      197 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:41:17.772419 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/assets/
--rw-r--r--   0 root         (0) root         (0)      498 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10472 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt
--rw-r--r--   0 root         (0) root         (0)     1974 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/main.py
--rw-r--r--   0 root         (0) root         (0)     9702 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/ml_models.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/ml_xai.py
--rw-r--r--   0 root         (0) root         (0)     2443 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/options.py
--rw-r--r--   0 root         (0) root         (0)     5323 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/trame_exec.py
--rw-r--r--   0 root         (0) root         (0)     4031 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/trame_state.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/jupyter.py
--rw-r--r--   0 root         (0) root         (0)      747 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:41:17.772419 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/ui/
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4188 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/ui/main.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/ui/options.py
--rw-r--r--   0 root         (0) root         (0)    16375 2023-07-21 16:41:14.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/ui/ui_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:41:17.768418 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2724 2023-07-21 16:41:17.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1041 2023-07-21 16:41:17.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 16:41:17.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-21 16:41:17.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      352 2023-07-21 16:41:17.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-21 16:41:17.000000 xaitk-saliency-demo-2.2.3/xaitk_saliency_demo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:51:37.494473 xaitk-saliency-demo-2.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2724 2023-08-03 19:51:37.494473 xaitk-saliency-demo-2.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-08-03 19:51:37.494473 xaitk-saliency-demo-2.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:51:37.490473 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:51:37.494473 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       62 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     3742 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/config.py
+-rw-r--r--   0 root         (0) root         (0)    13426 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/core.py
+-rw-r--r--   0 root         (0) root         (0)      756 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:51:37.494473 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/ml/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/ml/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:51:37.494473 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/ml/assets/
+-rw-r--r--   0 root         (0) root         (0)      498 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/ml/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10472 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/ml/assets/imagenet_classes.txt
+-rw-r--r--   0 root         (0) root         (0)     9702 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/ml/models.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/ml/xai.py
+-rw-r--r--   0 root         (0) root         (0)    18586 2023-08-03 19:51:34.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/xaitk_widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:51:37.494473 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2724 2023-08-03 19:51:37.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      798 2023-08-03 19:51:37.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 19:51:37.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-08-03 19:51:37.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      359 2023-08-03 19:51:37.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-03 19:51:37.000000 xaitk-saliency-demo-2.3.0/xaitk_saliency_demo.egg-info/top_level.txt
```

### Comparing `xaitk-saliency-demo-2.2.3/LICENSE` & `xaitk-saliency-demo-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.3/PKG-INFO` & `xaitk-saliency-demo-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xaitk-saliency-demo
-Version: 2.2.3
+Version: 2.3.0
 Summary: Web application demonstrating XAITK Saliency functionality
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `xaitk-saliency-demo-2.2.3/README.rst` & `xaitk-saliency-demo-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.3/setup.cfg` & `xaitk-saliency-demo-2.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xaitk-saliency-demo
-version = 2.2.3
+version = 2.3.0
 description = Web application demonstrating XAITK Saliency functionality
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = BSD License
 classifiers = 
 	Development Status :: 5 - Production/Stable
@@ -40,16 +40,16 @@
 	smqtk-descriptors==0.19.0
 	smqtk-detection[torch,centernet]==0.20.0
 	smqtk-image-io==0.17.1
 	
 	xaitk-saliency==0.7.0
 	ubelt==1.3.2
 	
-	torch==1.10.2
-	torchvision==0.11.3
+	torch>=1.9.0,!=2.0.1
+	torchvision>=0.10.0
 	
 	scikit-learn==1.3.0
 	scikit-image==0.21.0
 
 [options.entry_points]
 console_scripts = 
 	xaitk-saliency-demo = xaitk_saliency_demo:main
```

### Comparing `xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt` & `xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/ml/assets/imagenet_classes.txt`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/ml_models.py` & `xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/ml/models.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/ml_xai.py` & `xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/ml/xai.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/engine/options.py` & `xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -71,7 +71,54 @@
     "seed": int,
     "threads": int,
     "proximity_metric": str,
     "debiased": bool,
 }
 
 SALINECY_PARAM_REMAP = {"s": "s_tuple"}
+
+TASKS = [
+    {"text": "Image Similarity", "value": "similarity"},
+    {"text": "Object Detection", "value": "detection"},
+    {"text": "Image Classification", "value": "classification"},
+]
+
+PROXIMITY_METRIC_AVAILABLE = [
+    "braycurtis",
+    "canberra",
+    "chebyshev",
+    "cityblock",
+    "correlation",
+    "cosine",
+    "dice",
+    "euclidean",
+    "hamming",
+    "jaccard",
+    "jensenshannon",
+    "kulsinski",
+    "mahalanobis",
+    "matching",
+    "minkowski",
+    "rogerstanimoto",
+    "russellrao",
+    "seuclidean",
+    "sokalmichener",
+    "sokalsneath",
+    "sqeuclidean",
+    "wminkowski",
+    "yule",
+]
+
+# https://github.com/Kitware/trame-components/blob/master/vue-components/src/components/XaiHeatMap/script.js#L47-L78
+HEAT_MAP_MODES = [
+    ("full", "mdi-arrow-left-right", "true"),
+    ("maxSym", "mdi-arrow-expand-horizontal", "true"),
+    ("minSym", "mdi-arrow-collapse-horizontal", "full_range[0] < 0"),
+    ("negative", "mdi-ray-end-arrow", "full_range[0] < 0"),
+    ("positive", "mdi-ray-start-arrow", "full_range[1] > 0"),
+    ("custom", "mdi-account", "true"),
+]
+
+# Common css style
+STYLE_COMPACT = dict(hide_details=True, dense=True)
+STYLE_SELECT = dict(style="max-width: 200px", classes="mx-2")
+STYLE_ROW = dict(style="min-width: 0;", classes="d-flex flex-shrink-1")
```

### Comparing `xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/main.py` & `xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 from trame.app import get_server
-from . import engine, ui
-from .engine.ml_models import update_ml_device
+from .core import XaitkSaliency
+from .ml.models import update_ml_device
 
 
 def main(server=None, **kwargs):
     # Get or create server
     if server is None:
         server = get_server()
 
     if isinstance(server, str):
         server = get_server(server)
 
-    # Fix version of vue
-    server.client_type = "vue2"
-
     # CLI
     server.cli.add_argument(
         "--cpu",
         help="Force usage of CPU even if a GPU is available",
         dest="cpu",
         action="store_true",
     )
     update_ml_device(server.cli.parse_known_args()[0].cpu)
 
     # Init application
-    engine.initialize(server)
-    ui.initialize(server)
+    XaitkSaliency(server)
 
     # Start server
     server.start(**kwargs)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `xaitk-saliency-demo-2.2.3/xaitk_saliency_demo/app/ui/ui_helper.py` & `xaitk-saliency-demo-2.3.0/xaitk_saliency_demo/app/xaitk_widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,477 +1,485 @@
 from trame.widgets import html, vuetify, plotly, trame
-
-from . import options
+from xaitk_saliency_demo.app import config
 
 import multiprocessing
 
 NB_THREADS = int(multiprocessing.cpu_count() / 2 + 0.5)
 
 # -----------------------------------------------------------------------------
-# Global properties
-# -----------------------------------------------------------------------------
-
-compact_styles = {
-    "hide_details": True,
-    "dense": True,
-}
-
-combo_styles = {
-    "style": "max-width: 200px",
-    "classes": "mx-2",
-}
-
-row_style = {
-    "classes": "d-flex flex-shrink-1",
-    "style": "min-width: 0;",
-}
-
-# -----------------------------------------------------------------------------
 # Component builders
 # -----------------------------------------------------------------------------
 
 
-def create_btn_icon(__icon, **kwargs):
-    kwargs.setdefault("icon", True)
-    btn = vuetify.VBtn(**kwargs)
-    with btn:
-        vuetify.VIcon(__icon)
-    return btn
+class IconButton(vuetify.VBtn):
+    def __init__(self, icon, **kwargs):
+        kwargs.setdefault("icon", True)
+        super().__init__(**kwargs)
+        with self:
+            vuetify.VIcon(icon)
+
+
+class CardContainer(vuetify.VCard):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        with self:
+            self.header = vuetify.VCardTitle()
+            vuetify.VDivider()
+            self.content = vuetify.VCardText()
+
+
+class InputImage(html.Div):
+    def __init__(self, input, **kwargs):
+        _img_url = f"{input}_img_url"
+        _name = f"{input}_name"
+        super().__init__(style="position: relative;", v_show=(_img_url,))
+        with self:
+            vuetify.VImg(
+                aspect_ratio=1,
+                src=(_img_url, None),
+                classes="elevation-2 ma-2",
+                max_height="200px",
+                max_width="200px",
+                min_height="200px",
+                min_width="200px",
+                **kwargs,
+            )
+            IconButton(
+                "mdi-close-thick",
+                absolute=True,
+                style="top: -2px; right: -2px; background: white;",
+                outlined=True,
+                x_small=True,
+                click=f"{_img_url} = null",
+                **kwargs,
+            )
+            html.Div(
+                f"{{{{ {_name} }}}}",
+                classes="text-center text-caption",
+                v_show=("task_active == 'similarity'",),
+            )
 
 
 def create_card_container(**kwargs):
     with vuetify.VCard(**kwargs) as _card:
         _header = vuetify.VCardTitle()
         vuetify.VDivider()
         _content = vuetify.VCardText()
 
     return _card, _header, _content
 
 
 # -----------------------------------------------------------------------------
 # Section builders
 #
-# +--------------------------------------------------------------------+
-# | toolbar                                                            |
-# +---------------------------------+----------------------------------+
-# | create_section_input()          | create_section_model_execution() |
-# +---------------------------------+----------------------------------+
-# | create_section_xai_parameters() | create_section_xai_execution()   |
-# +---------------------------------+----------------------------------+
+# +---------------------------------------------------+
+# | Toolbar()                                           |
+# +-------------------------+-------------------------+
+# | InputSection()          | ModelExecutionSection() |
+# +-------------------------+-------------------------+
+# | XaiParametersSection()  | XaiExecutionSection()   |
+# +-------------------------+-------------------------+
 #
 # -----------------------------------------------------------------------------
 
 
-def create_section_input():
-    _card, _header, _content = create_card_container(
-        classes="ma-4",
-        style=("{ width: `${2 * 216 + 8}px`}",),
-    )
-    _content.style = "min-height: 224px;"
-
-    with _header:
-        _header.add_child("Data Selection")
+class Toolbar:
+    def __init__(self):
         vuetify.VSpacer()
-        create_btn_icon(
-            "mdi-image-plus",
-            small=True,
-            v_show=("input_needed", True),
-            click="input_file=null; $refs.file_form.reset(); $refs.input_file.click()",
+        vuetify.VSelect(
+            label="Task",
+            v_model=("task_active", "classification"),
+            items=("task_available", config.TASKS),
+            **config.STYLE_COMPACT,
+            **config.STYLE_SELECT,
         )
-
-    with _content:
-        with vuetify.VRow():
-            create_input_image("input_1")
-            create_input_image("input_2")
-        with html.Form(ref="file_form", classes="d-none"):
-            html.Input(
-                ref="input_file",
-                type="file",
-                change="input_file=$event.target.files[0]",
-                __events=["change"],
-            )
-
-    return _card
-
-
-def create_input_image(input, **kwargs):
-    _img_url = f"{input}_img_url"
-    _name = f"{input}_name"
-    _container = html.Div(style="position: relative;", v_show=(_img_url,))
-
-    with _container:
-        vuetify.VImg(
-            aspect_ratio=1,
-            src=(_img_url, None),
-            classes="elevation-2 ma-2",
-            max_height="200px",
-            max_width="200px",
-            min_height="200px",
-            min_width="200px",
-            **kwargs,
+        vuetify.VSelect(
+            label="Model",
+            v_model=("model_active", ""),
+            items=("model_available", []),
+            **config.STYLE_COMPACT,
+            **config.STYLE_SELECT,
         )
-        create_btn_icon(
-            "mdi-close-thick",
-            absolute=True,
-            style="top: -2px; right: -2px; background: white;",
-            outlined=True,
-            x_small=True,
-            click=f"{_img_url} = null",
-            **kwargs,
+        vuetify.VSelect(
+            label="Saliency Algorithm",
+            v_show="saliency_available.length > 1",
+            v_model=("saliency_active", ""),
+            items=("saliency_available", []),
+            **config.STYLE_COMPACT,
+            **config.STYLE_SELECT,
         )
-        html.Div(
-            f"{{{{ {_name} }}}}",
-            classes="text-center text-caption",
-            v_show=("task_active == 'similarity'",),
+        vuetify.VSelect(
+            v_show=("['classification', 'detection'].includes(task_active)",),
+            label="Top classes",
+            v_model=("TOP_K", 5),
+            items=("TOP_K_available", list(range(5, 11))),
+            **config.STYLE_COMPACT,
+            style="max-width: 70px",
+        )
+        vuetify.VProgressLinear(
+            indeterminate=True,
+            absolute=True,
+            bottom=True,
+            active=("trame__busy",),
         )
 
-    return _container
 
+class InputSection(CardContainer):
+    def __init__(self):
+        super().__init__(classes="ma-4", style=f"width: {2 * 216 + 8}px;")
+        self.content.style = "min-height: 224px;"
+        with self.header:
+            self.header.add_child("Data Selection")
+            vuetify.VSpacer()
+            IconButton(
+                "mdi-image-plus",
+                small=True,
+                v_show=("input_needed", True),
+                click="input_file=null; $refs.file_form.reset(); $refs.input_file.click()",
+            )
 
-# -----------------------------------------------------------------------------
+        with self.content:
+            with vuetify.VRow():
+                InputImage("input_1")
+                InputImage("input_2")
+            with html.Form(ref="file_form", classes="d-none"):
+                html.Input(
+                    ref="input_file",
+                    type="file",
+                    change="input_file=$event.target.files[0]",
+                    __events=["change"],
+                )
 
 
-def create_section_model_execution(ctrl):
-    _card, _header, _content = create_card_container(
-        classes="ma-4 flex-sm-grow-1",
-        style="width: calc(100% - 504px);",
-    )
-    _content.style = "min-height: 224px"
-    _content.classes = "d-flex flex-shrink-1"
-
-    with _header:
-        create_btn_icon(
-            "mdi-run-fast",
-            small=True,
-            disabled=("input_needed",),
-            classes="mr-2",
-            click=ctrl.run_model,
-        )
-        _header.add_child("Model execution")
+class ModelExecutionSection(CardContainer):
+    def __init__(self, run=None):
+        super().__init__(
+            classes="ma-4 flex-sm-grow-1", style="width: calc(100% - 504px);"
+        )
+        ctrl = self.server.controller
+
+        with self.header as header:
+            IconButton(
+                "mdi-run-fast",
+                small=True,
+                disabled=("input_needed",),
+                classes="mr-2",
+                click=run,
+            )
+            header.add_child("Model execution")
 
-    with _content:
-        # classes UI
-        _chart = plotly.Figure(
-            style="width: 100%; height: 100%;",
-            v_show=("task_active === 'classification'",),
-            display_mode_bar=False,
-        )
-        ctrl.classification_chart_update = _chart.update
+        with self.content as content:
+            content.style = "min-height: 224px"
+            content.classes = "d-flex flex-shrink-1"
+            # classes UI
+            _chart = plotly.Figure(
+                style="width: 100%; height: 100%;",
+                v_show=("task_active === 'classification'",),
+                display_mode_bar=False,
+            )
+            ctrl.classification_chart_update = _chart.update
 
-        # similarity UI
-        vuetify.VProgressCircular(
-            "{{ Math.round(model_viz_similarity) }} %",
-            v_show=("task_active === 'similarity'",),
-            size=192,
-            width=15,
-            color="teal",
-            value=("model_viz_similarity", 0),
-        )
+            # similarity UI
+            vuetify.VProgressCircular(
+                "{{ Math.round(model_viz_similarity) }} %",
+                v_show=("task_active === 'similarity'",),
+                size=192,
+                width=15,
+                color="teal",
+                value=("model_viz_similarity", 0),
+            )
 
-        # object detection UI
-        with vuetify.VRow(v_show=("task_active === 'detection'",), align="center"):
-            trame.XaiImage(
-                classes="ma-2",
-                src=("input_1_img_url",),
-                areas=("model_viz_detection_areas", []),
-                area_selected=("model_viz_detection_area_actives", []),
-                area_opacity=0.25,
-                area_selected_opacity=1,
-                area_key="id",
-                max_height=216,
-                area_style=("{ 'stroke-width': 3, rx: 10 }",),
-            )
-            with vuetify.VRow(
-                classes="d-flex flex-shrink-1 align-content-start flex-wrap no-gutters",
-                style="width: 25px; height: 100%;",
-            ):
-                with vuetify.VSheet(
-                    v_for=("item, idx in model_viz_detection_areas",),
-                    key="idx",
+            # object detection UI
+            with vuetify.VRow(v_show=("task_active === 'detection'",), align="center"):
+                trame.XaiImage(
                     classes="ma-2",
-                    style="cursor: pointer",
-                    elevation=4,
-                    width=125,
-                    height=40,
-                    rounded=True,
-                    mouseenter="model_viz_detection_area_actives = [idx + 1]",
-                    mouseleave="model_viz_detection_area_actives = []",
+                    src=("input_1_img_url",),
+                    areas=("model_viz_detection_areas", []),
+                    area_selected=("model_viz_detection_area_actives", []),
+                    area_opacity=0.25,
+                    area_selected_opacity=1,
+                    area_key="id",
+                    max_height=216,
+                    area_style=("{ 'stroke-width': 3, rx: 10 }",),
+                )
+                with vuetify.VRow(
+                    classes="d-flex flex-shrink-1 align-content-start flex-wrap no-gutters",
+                    style="width: 25px; height: 100%;",
                 ):
-                    with vuetify.VContainer(classes="fill-height"):
-                        with vuetify.VRow(
-                            classes="px-3",
-                            align_self="center",
-                            align_content="center",
-                            justify="space-between",
-                        ):
-                            html.Div("{{ item.class }}", classes="text-capitalize")
-                            html.Div("{{ item.probability }}%")
-
-
-# -----------------------------------------------------------------------------
-
+                    with vuetify.VSheet(
+                        v_for=("item, idx in model_viz_detection_areas",),
+                        key="idx",
+                        classes="ma-2",
+                        style="cursor: pointer",
+                        elevation=4,
+                        width=125,
+                        height=40,
+                        rounded=True,
+                        mouseenter="model_viz_detection_area_actives = [idx + 1]",
+                        mouseleave="model_viz_detection_area_actives = []",
+                    ):
+                        with vuetify.VContainer(classes="fill-height"):
+                            with vuetify.VRow(
+                                classes="px-3",
+                                align_self="center",
+                                align_content="center",
+                                justify="space-between",
+                            ):
+                                html.Div("{{ item.class }}", classes="text-capitalize")
+                                html.Div("{{ item.probability }}%")
+
+
+class XaiParametersSection(CardContainer):
+    def __init__(self):
+        super().__init__(classes="ma-4", style="width: 440px;")
+        self.header.add_child("XAI parameters")
+        with self.content:
+            with vuetify.VRow(v_show=("xai_params_to_show.includes('window_size')",)):
+                vuetify.VTextField(
+                    label="Window Size (Height)",
+                    v_model=("xai_param__window_size[0]",),
+                    type="number",
+                    classes="mx-2",
+                    change="flushState('xai_param__window_size')",
+                )
+                vuetify.VTextField(
+                    label="Window Size (Width)",
+                    v_model=("xai_param__window_size[1]",),
+                    type="number",
+                    classes="mx-2",
+                    change="flushState('xai_param__window_size')",
+                )
 
-def create_section_xai_parameters():
-    _card, _header, _content = create_card_container(
-        classes="ma-4",
-        style="width: 440px;",
-    )
-    _header.add_child("XAI parameters")
-    with _content:
-        with vuetify.VRow(v_show=("xai_params_to_show.includes('window_size')",)):
+            with vuetify.VRow(v_show=("xai_params_to_show.includes('stride')",)):
+                vuetify.VTextField(
+                    label="Stride Size (Height step)",
+                    v_model=("xai_param__stride[0]",),
+                    type="number",
+                    classes="mx-2",
+                    change="flushState('xai_param__stride')",
+                )
+                vuetify.VTextField(
+                    label="Stride Size (Width step)",
+                    v_model=("xai_param__stride[1]",),
+                    type="number",
+                    classes="mx-2",
+                    change="flushState('xai_param__stride')",
+                )
             vuetify.VTextField(
-                label="Window Size (Height)",
-                v_model=("xai_param__window_size[0]",),
+                label="Number of random masks used in the algorithm",
+                v_show=("xai_params_to_show.includes('n')",),
+                v_model=("xai_param__n", 1000),
                 type="number",
-                classes="mx-2",
-                change="flushState('xai_param__window_size')",
             )
             vuetify.VTextField(
-                label="Window Size (Width)",
-                v_model=("xai_param__window_size[1]",),
+                label="Spatial resolution of the small masking grid",
+                v_show=("xai_params_to_show.includes('s')",),
+                v_model=("xai_param__s", 8),
                 type="number",
-                classes="mx-2",
-                change="flushState('xai_param__window_size')",
             )
-
-        with vuetify.VRow(v_show=("xai_params_to_show.includes('stride')",)):
-            vuetify.VTextField(
-                label="Stride Size (Height step)",
-                v_model=("xai_param__stride[0]",),
-                type="number",
-                classes="mx-2",
-                change="flushState('xai_param__stride')",
+            with vuetify.VCol(v_show=("xai_params_to_show.includes('s_tuple')",)):
+                vuetify.VRow(
+                    "Spatial resolution of the small masking grid (x, y)",
+                    classes="text-caption text--secondary",
+                    style="line-height: 20px; height: 20px; letter-spacing: normal !important;",
+                )
+                with vuetify.VRow(classes="mt-0 pt-0"):
+                    vuetify.VTextField(
+                        v_model_number=("xai_param__s_tuple[0]",),
+                        change="flushState('xai_param__s_tuple')",
+                        type="number",
+                        classes="mr-1 pt-1",
+                    )
+                    vuetify.VTextField(
+                        v_model_number=("xai_param__s_tuple[1]",),
+                        change="flushState('xai_param__s_tuple')",
+                        type="number",
+                        classes="ml-1 pt-1",
+                    )
+            vuetify.VSlider(
+                label="P1",
+                persistent_hint=True,
+                hint="Probability of the grid cell being set to 1 (otherwise 0). This should be a float value in the [0, 1] range.",
+                v_show=("xai_params_to_show.includes('p1')",),
+                v_model=("xai_param__p1", 0.5),
+                min="0",
+                max="1",
+                step="0.01",
+                thumb_size="24",
+                thumb_label="always",
+                classes="my-4",
             )
             vuetify.VTextField(
-                label="Stride Size (Width step)",
-                v_model=("xai_param__stride[1]",),
+                label="Seed",
+                v_show=("xai_params_to_show.includes('seed')",),
+                v_model=("xai_param__seed", 1234),
                 type="number",
-                classes="mx-2",
-                change="flushState('xai_param__stride')",
+                hint="A seed to pass into the constructed random number generator to allow for reproducibility",
+                persistent_hint=True,
+                classes="my-4",
             )
-        vuetify.VTextField(
-            label="Number of random masks used in the algorithm",
-            v_show=("xai_params_to_show.includes('n')",),
-            v_model=("xai_param__n", 1000),
-            type="number",
-        )
-        vuetify.VTextField(
-            label="Spatial resolution of the small masking grid",
-            v_show=("xai_params_to_show.includes('s')",),
-            v_model=("xai_param__s", 8),
-            type="number",
-        )
-        with vuetify.VCol(v_show=("xai_params_to_show.includes('s_tuple')",)):
-            vuetify.VRow(
-                "Spatial resolution of the small masking grid (x, y)",
-                classes="text-caption text--secondary",
-                style="line-height: 20px; height: 20px; letter-spacing: normal !important;",
+            vuetify.VSlider(
+                label="Threads",
+                v_show=("xai_params_to_show.includes('threads')",),
+                v_model=("xai_param__threads", NB_THREADS),
+                min="0",
+                max="32",
+                hint="The number of threads to utilize when generating masks. If this is <=0 or None, no threading is used and processing is performed in-line serially.",
+                persistent_hint=True,
+                thumb_size="24",
+                thumb_label="always",
+                classes="my-6",
+            )
+            vuetify.VSelect(
+                label="Proximity Metric",
+                v_show=("xai_params_to_show.includes('proximity_metric')",),
+                v_model=("xai_param__proximity_metric", "euclidean"),
+                items=(
+                    "xai_param__proximity_metric_available",
+                    config.PROXIMITY_METRIC_AVAILABLE,
+                ),
+            )
+            vuetify.VSwitch(
+                label="Debiased",
+                v_show=("xai_params_to_show.includes('debiased')",),
+                v_model=("xai_param__debiased", False),
             )
-            with vuetify.VRow(classes="mt-0 pt-0"):
-                vuetify.VTextField(
-                    v_model_number=("xai_param__s_tuple[0]",),
-                    change="flushState('xai_param__s_tuple')",
-                    type="number",
-                    classes="mr-1 pt-1",
-                )
-                vuetify.VTextField(
-                    v_model_number=("xai_param__s_tuple[1]",),
-                    change="flushState('xai_param__s_tuple')",
-                    type="number",
-                    classes="ml-1 pt-1",
-                )
-        vuetify.VSlider(
-            label="P1",
-            persistent_hint=True,
-            hint="Probability of the grid cell being set to 1 (otherwise 0). This should be a float value in the [0, 1] range.",
-            v_show=("xai_params_to_show.includes('p1')",),
-            v_model=("xai_param__p1", 0.5),
-            min="0",
-            max="1",
-            step="0.01",
-            thumb_size="24",
-            thumb_label="always",
-            classes="my-4",
-        )
-        vuetify.VTextField(
-            label="Seed",
-            v_show=("xai_params_to_show.includes('seed')",),
-            v_model=("xai_param__seed", 1234),
-            type="number",
-            hint="A seed to pass into the constructed random number generator to allow for reproducibility",
-            persistent_hint=True,
-            classes="my-4",
-        )
-        vuetify.VSlider(
-            label="Threads",
-            v_show=("xai_params_to_show.includes('threads')",),
-            v_model=("xai_param__threads", NB_THREADS),
-            min="0",
-            max="32",
-            hint="The number of threads to utilize when generating masks. If this is <=0 or None, no threading is used and processing is performed in-line serially.",
-            persistent_hint=True,
-            thumb_size="24",
-            thumb_label="always",
-            classes="my-6",
-        )
-        vuetify.VSelect(
-            label="Proximity Metric",
-            v_show=("xai_params_to_show.includes('proximity_metric')",),
-            v_model=("xai_param__proximity_metric", "euclidean"),
-            items=(
-                "xai_param__proximity_metric_available",
-                options.PROXIMITY_METRIC_AVAILABLE,
-            ),
-        )
-        vuetify.VSwitch(
-            label="Debiased",
-            v_show=("xai_params_to_show.includes('debiased')",),
-            v_model=("xai_param__debiased", False),
-        )
-
-    return _card
-
-
-# -----------------------------------------------------------------------------
 
 
-def create_section_xai_execution(ctrl):
-    _card, _header, _content = create_card_container(
-        classes="ma-4 flex-sm-grow-1",
-        style="width: calc(100% - 504px);",
-    )
-
-    with _header:
-        create_btn_icon(
-            "mdi-run-fast",
-            small=True,
-            classes="mr-2",
-            click=ctrl.run_saliency,
-        )
-        _header.add_child("XAI")
-        vuetify.VSpacer()
-        vuetify.VTextField(
-            label="Min",
-            v_model=("xai_viz_color_min", -1),
-            **compact_styles,
-            style="max-width: 75px",
-            classes="mx-1",
-            disabled=("xai_viz_heatmap_color_mode !== 'custom'",),
-        )
-        vuetify.VTextField(
-            label="Max",
-            v_model=("xai_viz_color_max", 1),
-            **compact_styles,
-            style="max-width: 75px",
-            classes="mx-1",
-            disabled=("xai_viz_heatmap_color_mode !== 'custom'",),
+class XaiExecutionSection(CardContainer):
+    def __init__(self, run=None):
+        super().__init__(
+            classes="ma-4 flex-sm-grow-1",
+            style="width: calc(100% - 504px);",
         )
-        vuetify.VSlider(
-            v_model=("xai_viz_heatmap_opacity", 0.5),
-            min=0,
-            max=1,
-            step=0.05,
-            **compact_styles,
-            style="max-width: 300px",
-        )
-        with vuetify.VBtnToggle(
-            v_model=("xai_viz_heatmap_color_mode", "full"),
-            mandatory=True,
-            classes="mx-2",
-            **compact_styles,
-        ):
-            for value, icon, show in options.HEAT_MAP_MODES:
-                with vuetify.VBtn(
-                    v_show=show,
-                    icon=True,
-                    value=value,
-                    small=True,
-                    **compact_styles,
-                ):
-                    vuetify.VIcon(icon, small=True)
-
-    with _content:
-        create_xai_classification()
-        create_xai_similarity()
-        create_xai_detection()
-
-    return _card
 
+        with self.header:
+            IconButton(
+                "mdi-run-fast",
+                small=True,
+                classes="mr-2",
+                click=run,
+            )
+            self.header.add_child("XAI")
+            vuetify.VSpacer()
+            vuetify.VTextField(
+                label="Min",
+                v_model=("xai_viz_color_min", -1),
+                **config.STYLE_COMPACT,
+                style="max-width: 75px",
+                classes="mx-1",
+                disabled=("xai_viz_heatmap_color_mode !== 'custom'",),
+            )
+            vuetify.VTextField(
+                label="Max",
+                v_model=("xai_viz_color_max", 1),
+                **config.STYLE_COMPACT,
+                style="max-width: 75px",
+                classes="mx-1",
+                disabled=("xai_viz_heatmap_color_mode !== 'custom'",),
+            )
+            vuetify.VSlider(
+                v_model=("xai_viz_heatmap_opacity", 0.5),
+                min=0,
+                max=1,
+                step=0.05,
+                **config.STYLE_COMPACT,
+                style="max-width: 300px",
+            )
+            with vuetify.VBtnToggle(
+                v_model=("xai_viz_heatmap_color_mode", "full"),
+                mandatory=True,
+                classes="mx-2",
+                **config.STYLE_COMPACT,
+            ):
+                for value, icon, show in config.HEAT_MAP_MODES:
+                    with vuetify.VBtn(
+                        v_show=show,
+                        icon=True,
+                        value=value,
+                        small=True,
+                        **config.STYLE_COMPACT,
+                    ):
+                        vuetify.VIcon(icon, small=True)
+
+        with self.content:
+            XaiClassificationResults()
+            XaiSimilarityResults()
+            XaiDetectionResults()
+
+
+class XaiClassificationResults(html.Div):
+    def __init__(self):
+        super().__init__(
+            v_if=("xai_viz_type == 'classification'",),
+            classes="d-flex flex-column",
+        )
+        with self:
+            vuetify.VSelect(
+                v_model=("xai_viz_classification_selected",),
+                items=("xai_viz_classification_selected_available", []),
+                **config.STYLE_COMPACT,
+                classes="mb-2",
+            )
+            trame.XaiImage(
+                v_if=("input_1_img_url",),
+                src=("input_1_img_url",),
+                max_height=400,
+                areas=("[]",),
+                heatmaps=("xai_viz_classification_heatmaps", {}),
+                heatmap_opacity=("xai_viz_heatmap_opacity",),
+                heatmap_color_preset="BuRd",
+                heatmap_color_range=("xai_viz_heatmap_color_range", [-1, 1]),
+                heatmap_color_mode=("xai_viz_heatmap_color_mode",),
+                heatmap_active=("xai_viz_classification_selected", "heatmap_0"),
+                color_range="[xai_viz_color_min, xai_viz_color_max] = $event",
+                full_range="full_range = $event",
+            )
 
-def create_xai_classification():
-    container = html.Div(
-        v_if=("xai_viz_type == 'classification'",), classes="d-flex flex-column"
-    )
-    with container:
-        vuetify.VSelect(
-            v_model=("xai_viz_classification_selected",),
-            items=("xai_viz_classification_selected_available", []),
-            **compact_styles,
-            classes="mb-2",
-        )
-        trame.XaiImage(
-            v_if=("input_1_img_url",),
-            src=("input_1_img_url",),
-            max_height=400,
-            areas=("[]",),
-            heatmaps=("xai_viz_classification_heatmaps", {}),
-            heatmap_opacity=("xai_viz_heatmap_opacity",),
-            heatmap_color_preset="BuRd",
-            heatmap_color_range=("xai_viz_heatmap_color_range", [-1, 1]),
-            heatmap_color_mode=("xai_viz_heatmap_color_mode",),
-            heatmap_active=("xai_viz_classification_selected", "heatmap_0"),
-            color_range="[xai_viz_color_min, xai_viz_color_max] = $event",
-            full_range="full_range = $event",
-        )
-
-    return container
-
-
-def create_xai_similarity():
-    container = html.Div(v_if=("xai_viz_type == 'similarity'",))
-    with container:
-        trame.XaiImage(
-            v_if=("input_2_img_url",),
-            src=("input_1_img_url",),
-            max_height=400,
-            areas=("[]",),
-            heatmaps=("xai_viz_similarity_heatmaps", {}),
-            heatmap_opacity=("xai_viz_heatmap_opacity",),
-            heatmap_color_preset="BuRd",
-            heatmap_color_range=("xai_viz_heatmap_color_range", [-1, 1]),
-            heatmap_color_mode=("xai_viz_heatmap_color_mode",),
-            heatmap_active="heatmap_0",
-            color_range="[xai_viz_color_min, xai_viz_color_max] = $event",
-            full_range="full_range = $event",
-        )
-
-    return container
 
+class XaiSimilarityResults(html.Div):
+    def __init__(self):
+        super().__init__(v_if=("xai_viz_type == 'similarity'",))
+        with self:
+            trame.XaiImage(
+                v_if=("input_2_img_url",),
+                src=("input_1_img_url",),
+                max_height=400,
+                areas=("[]",),
+                heatmaps=("xai_viz_similarity_heatmaps", {}),
+                heatmap_opacity=("xai_viz_heatmap_opacity",),
+                heatmap_color_preset="BuRd",
+                heatmap_color_range=("xai_viz_heatmap_color_range", [-1, 1]),
+                heatmap_color_mode=("xai_viz_heatmap_color_mode",),
+                heatmap_active="heatmap_0",
+                color_range="[xai_viz_color_min, xai_viz_color_max] = $event",
+                full_range="full_range = $event",
+            )
 
-def create_xai_detection():
-    container = html.Div(
-        v_if=("xai_viz_type == 'detection'",), classes="d-flex flex-column"
-    )
-    with container:
-        vuetify.VSelect(
-            v_model=("xai_viz_detection_selected",),
-            items=("model_viz_detection_areas", []),
-            change="model_viz_detection_area_actives = [1 + Number(xai_viz_detection_selected.split('_')[1])]",
-            **compact_styles,
-            classes="mb-2",
-        )
-        trame.XaiImage(
-            v_if=("input_1_img_url",),
-            src=("input_1_img_url",),
-            max_height=400,
-            areas=("[]",),
-            heatmaps=("xai_viz_detection_heatmaps", {}),
-            heatmap_color_preset="BuRd",
-            heatmap_color_range=("xai_viz_heatmap_color_range", [-1, 1]),
-            heatmap_color_mode=("xai_viz_heatmap_color_mode",),
-            heatmap_opacity=("xai_viz_heatmap_opacity",),
-            heatmap_active=("xai_viz_detection_selected", "heatmap_0"),
-            color_range="[xai_viz_color_min, xai_viz_color_max] = $event",
-            full_range="full_range = $event",
-        )
 
-    return container
+class XaiDetectionResults(html.Div):
+    def __init__(self):
+        super().__init__(
+            v_if=("xai_viz_type == 'detection'",), classes="d-flex flex-column"
+        )
+        with self:
+            vuetify.VSelect(
+                v_model=("xai_viz_detection_selected",),
+                items=("model_viz_detection_areas", []),
+                change="model_viz_detection_area_actives = [1 + Number(xai_viz_detection_selected.split('_')[1])]",
+                **config.STYLE_COMPACT,
+                classes="mb-2",
+            )
+            trame.XaiImage(
+                v_if=("input_1_img_url",),
+                src=("input_1_img_url",),
+                max_height=400,
+                areas=("[]",),
+                heatmaps=("xai_viz_detection_heatmaps", {}),
+                heatmap_color_preset="BuRd",
+                heatmap_color_range=("xai_viz_heatmap_color_range", [-1, 1]),
+                heatmap_color_mode=("xai_viz_heatmap_color_mode",),
+                heatmap_opacity=("xai_viz_heatmap_opacity",),
+                heatmap_active=("xai_viz_detection_selected", "heatmap_0"),
+                color_range="[xai_viz_color_min, xai_viz_color_max] = $event",
+                full_range="full_range = $event",
+            )
```

### Comparing `xaitk-saliency-demo-2.2.3/xaitk_saliency_demo.egg-info/PKG-INFO` & `xaitk-saliency-demo-2.3.0/xaitk_saliency_demo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xaitk-saliency-demo
-Version: 2.2.3
+Version: 2.3.0
 Summary: Web application demonstrating XAITK Saliency functionality
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `xaitk-saliency-demo-2.2.3/xaitk_saliency_demo.egg-info/SOURCES.txt` & `xaitk-saliency-demo-2.3.0/xaitk_saliency_demo.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,22 +8,17 @@
 xaitk_saliency_demo.egg-info/SOURCES.txt
 xaitk_saliency_demo.egg-info/dependency_links.txt
 xaitk_saliency_demo.egg-info/entry_points.txt
 xaitk_saliency_demo.egg-info/requires.txt
 xaitk_saliency_demo.egg-info/top_level.txt
 xaitk_saliency_demo/app/__init__.py
 xaitk_saliency_demo/app/__main__.py
+xaitk_saliency_demo/app/config.py
+xaitk_saliency_demo/app/core.py
 xaitk_saliency_demo/app/jupyter.py
 xaitk_saliency_demo/app/main.py
-xaitk_saliency_demo/app/engine/__init__.py
-xaitk_saliency_demo/app/engine/main.py
-xaitk_saliency_demo/app/engine/ml_models.py
-xaitk_saliency_demo/app/engine/ml_xai.py
-xaitk_saliency_demo/app/engine/options.py
-xaitk_saliency_demo/app/engine/trame_exec.py
-xaitk_saliency_demo/app/engine/trame_state.py
-xaitk_saliency_demo/app/engine/assets/__init__.py
-xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt
-xaitk_saliency_demo/app/ui/__init__.py
-xaitk_saliency_demo/app/ui/main.py
-xaitk_saliency_demo/app/ui/options.py
-xaitk_saliency_demo/app/ui/ui_helper.py
+xaitk_saliency_demo/app/xaitk_widgets.py
+xaitk_saliency_demo/app/ml/__init__.py
+xaitk_saliency_demo/app/ml/models.py
+xaitk_saliency_demo/app/ml/xai.py
+xaitk_saliency_demo/app/ml/assets/__init__.py
+xaitk_saliency_demo/app/ml/assets/imagenet_classes.txt
```

