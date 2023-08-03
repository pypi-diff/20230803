# Comparing `tmp/unigui-1.9.7.tar.gz` & `tmp/unigui-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.9.7.tar", last modified: Sun Jul 30 06:57:19 2023, max compression
+gzip compressed data, was "dist/unigui-1.9.8.tar", last modified: Mon Jul 31 08:24:20 2023, max compression
```

## Comparing `unigui-1.9.7.tar` & `unigui-1.9.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-30 06:57:19.000000 unigui-1.9.7/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-30 06:57:19.000000 unigui-1.9.7/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)     5550 2023-07-29 16:18:50.000000 unigui-1.9.7/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3531 2023-07-26 16:18:00.000000 unigui-1.9.7/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)     4181 2023-07-28 17:59:21.000000 unigui-1.9.7/unigui/tables.py
--rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-1.9.7/unigui/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)     7796 2023-07-29 16:08:30.000000 unigui-1.9.7/unigui/autotest.py
--rw-r--r--   0 george    (1000) george    (1000)     2642 2023-07-26 17:28:06.000000 unigui-1.9.7/unigui/utils.py
--rw-rw-r--   0 george    (1000) george    (1000)     5573 2023-07-26 17:26:38.000000 unigui-1.9.7/unigui/reloader.py
--rw-rw-r--   0 george    (1000) george    (1000)     8713 2023-07-26 09:11:50.000000 unigui-1.9.7/unigui/users.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-30 06:57:19.000000 unigui-1.9.7/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-30 06:57:19.000000 unigui-1.9.7/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)     2750 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/css/333.46a5102a.css
--rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/css/vendor.f747ec02.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-30 06:57:19.000000 unigui-1.9.7/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-30 06:57:19.000000 unigui-1.9.7/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-30 06:57:19.000000 unigui-1.9.7/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/js/app.38493c13.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)    50402 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/js/333.2f4fc18c.js
--rw-rw-r--   0 george    (1000) george    (1000)  1445576 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/js/vendor.8cb03aaa.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-30 06:54:09.000000 unigui-1.9.7/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.7/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      642 2023-07-30 04:57:21.000000 unigui-1.9.7/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    18773 2023-07-30 06:57:19.000000 unigui-1.9.7/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-30 06:57:19.000000 unigui-1.9.7/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18468 2023-07-30 04:54:06.000000 unigui-1.9.7/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.7/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-30 06:57:19.000000 unigui-1.9.7/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       63 2023-07-30 06:57:19.000000 unigui-1.9.7/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-30 06:57:19.000000 unigui-1.9.7/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    18773 2023-07-30 06:57:19.000000 unigui-1.9.7/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.7/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1258 2023-07-30 06:57:19.000000 unigui-1.9.7/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-30 06:57:19.000000 unigui-1.9.7/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     5345 2023-07-31 07:12:00.000000 unigui-1.9.8/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3531 2023-07-26 16:18:00.000000 unigui-1.9.8/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4181 2023-07-28 17:59:21.000000 unigui-1.9.8/unigui/tables.py
+-rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-1.9.8/unigui/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7796 2023-07-29 16:08:30.000000 unigui-1.9.8/unigui/autotest.py
+-rw-r--r--   0 george    (1000) george    (1000)     2669 2023-07-31 07:45:36.000000 unigui-1.9.8/unigui/utils.py
+-rw-rw-r--   0 george    (1000) george    (1000)     5573 2023-07-26 17:26:38.000000 unigui-1.9.8/unigui/reloader.py
+-rw-rw-r--   0 george    (1000) george    (1000)     8713 2023-07-26 09:11:50.000000 unigui-1.9.8/unigui/users.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)     2691 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/css/435.30396533.css
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/css/vendor.f747ec02.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)    50532 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/js/435.ced6eca8.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/js/app.353e1981.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1445576 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/js/vendor.8cb03aaa.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-31 08:13:49.000000 unigui-1.9.8/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.8/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      642 2023-07-31 08:24:03.000000 unigui-1.9.8/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    18773 2023-07-31 08:24:20.000000 unigui-1.9.8/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-31 08:24:20.000000 unigui-1.9.8/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18468 2023-07-30 04:54:06.000000 unigui-1.9.8/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.8/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       63 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    18773 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.8/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1258 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-31 08:24:20.000000 unigui-1.9.8/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.9.7/unigui/guielements.py` & `unigui-1.9.8/unigui/guielements.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,56 +62,52 @@
 def CameraButton(name, *args, **kwargs):    
     kwargs['type'] = 'camera'
     return Button(name, *args, **kwargs)
         
 def UploadImageButton(name, handler,**kwargs):    
     kwargs['type'] = 'image_uploader'
     if 'width' not in kwargs:
-        kwargs['width'] = 250.0              
-    if 'height' not in kwargs:
-        kwargs['height'] = 300.0         
+        kwargs['width'] = 250.0                  
     return Button(name, handler, **kwargs)
 
 UploadButton = UploadImageButton
 
 class Image(Gui):
     '''has to contain file parameter as name'''
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.type='image'
         if not hasattr(self,'width'):
             self.width = 500.0              
-        if not hasattr(self,'image'):
-            self.image = self.value if hasattr(self, 'value') else None
+        if not hasattr(self,'url'):
+            self.url = self.name
 
 class Video(Gui):
     '''has to contain src parameter'''
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.type='video'
         if not hasattr(self,'width'):
             self.width = 500.0              
-        if not hasattr(self,'src'):
-            raise "No video src reference!"
+        if not hasattr(self,'url'):
+            self.url = self.name
         if not hasattr(self,'ratio'):
-            self.ratio = "9/9"
+            self.ratio = None
 
 graph_default_value = {'nodes' : [], 'edges' : []}
 
 class Graph(Gui):
     '''has to contain nodes, edges, see Readme'''
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.type='graph'
         if not hasattr(self,'value'):
             self.value = graph_default_value
         if not hasattr(self,'minwidth'):
-            self.minwidth = 600.0              
-        if not hasattr(self,'minheight'):
-            self.minheight = 600.0              
+            self.minwidth = 600.0                      
         if not hasattr(self, 'nodes'):
             self.nodes = []
         if not hasattr(self, 'edges'):
             self.edges = []
 
 class Switch(Gui):
     def __init__(self, *args, **kwargs):
```

### Comparing `unigui-1.9.7/unigui/server.py` & `unigui-1.9.8/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/tables.py` & `unigui-1.9.8/unigui/tables.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/autotest.py` & `unigui-1.9.8/unigui/autotest.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/utils.py` & `unigui-1.9.8/unigui/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 def toJson(obj, indent, pretty):
     js = jsonpickle.encode(obj,unpicklable=False)
     return json.dumps(json.loads(js), indent=indent, sort_keys=pretty) if pretty else js
 
 def filename2url(fn):   
     if fn[0] == '/' or fn[1] == ':': #if full path
         fn = fn[len(app_dir):]   
-    return fn.replace(' ','%20')
+    if fn[0] == divpath:
+        fn = fn[1:]
+    return fn 
 
 def url2filepath(url):
     return url[url.find('/') + 1:].replace('%20',' ')   
 
 def url2filename(url):
     return url[url.rfind('/') + 1:].replace('%20',' ')
```

### Comparing `unigui-1.9.7/unigui/reloader.py` & `unigui-1.9.8/unigui/reloader.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/users.py` & `unigui-1.9.8/unigui/users.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/favicon.ico` & `unigui-1.9.8/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/css/333.46a5102a.css` & `unigui-1.9.8/unigui/web/css/435.30396533.css`

 * *Files 13% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-thumb-hover:#2176d2;--scrollbar-thumb-dark:#2176d2;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.chart-container[data-v-981bab46]{height:400px;width:400px}body[data-v-b72ea538]{display:flex;justify-content:center}.custom-caption[data-v-b72ea538]{padding:5px!important}.web-camera-container[data-v-b72ea538]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-b72ea538]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-b72ea538]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-b72ea538]{opacity:1}.web-camera-container .camera-shoot[data-v-b72ea538]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-b72ea538]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-b72ea538]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-b72ea538]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-b72ea538]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-b72ea538]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-b72ea538]{animation:preload-b72ea538 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-b72ea538]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-b72ea538]:nth-child(3){animation-delay:.4s}@keyframes preload-b72ea538{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.q-tab__label{font-size:16px;font-weight:700}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-thumb-hover:#2176d2;--scrollbar-thumb-dark:#2176d2;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}body[data-v-d4b5cc5e]{display:flex;justify-content:center}.custom-caption[data-v-d4b5cc5e]{padding:5px!important}.web-camera-container[data-v-d4b5cc5e]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-d4b5cc5e]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-d4b5cc5e]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-d4b5cc5e]{opacity:1}.web-camera-container .camera-shoot[data-v-d4b5cc5e]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-d4b5cc5e]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-d4b5cc5e]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-d4b5cc5e]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-d4b5cc5e]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-d4b5cc5e]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-d4b5cc5e]{animation:preload-d4b5cc5e 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-d4b5cc5e]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-d4b5cc5e]:nth-child(3){animation-delay:.4s}@keyframes preload-d4b5cc5e{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.q-tab__label{font-size:16px;font-weight:700}
```

### Comparing `unigui-1.9.7/unigui/web/css/vendor.f747ec02.css` & `unigui-1.9.8/unigui/web/css/vendor.f747ec02.css`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/icons/favicon-96x96.png` & `unigui-1.9.8/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/icons/favicon-16x16.png` & `unigui-1.9.8/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/icons/favicon-32x32.png` & `unigui-1.9.8/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/icons/favicon-128x128.png` & `unigui-1.9.8/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `unigui-1.9.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.9.8/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.9.8/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.9.8/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.9.8/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/js/app.38493c13.js` & `unigui-1.9.8/unigui/web/js/app.353e1981.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(333)]).then(r.bind(r, 3333)),
+                        component: () => Promise.all([r.e(736), r.e(435)]).then(r.bind(r, 3435)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -163,24 +163,24 @@
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, o) => (r.f[o](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
-            333: "2f4fc18c",
-            430: "591e9a73"
+            430: "591e9a73",
+            435: "ced6eca8"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            333: "46a5102a",
+            435: "30396533",
             736: "f747ec02"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
@@ -264,15 +264,15 @@
                 e(o, l, n, a)
             })),
             n = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                333: 1
+                435: 1
             };
             n[e] ? t.push(n[e]) : 0 !== n[e] && r[e] && t.push(n[e] = o(e).then((() => {
                 n[e] = 0
             }), (t => {
                 throw delete n[e], t
             })))
         }
```

### Comparing `unigui-1.9.7/unigui/web/js/430.591e9a73.js` & `unigui-1.9.8/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/js/333.2f4fc18c.js` & `unigui-1.9.8/unigui/web/js/435.ced6eca8.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [333], {
-        3333: (e, t, a) => {
+    [435], {
+        3435: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => la
+                default: () => sa
             });
             var s = a(3673),
                 l = a(2323);
             const i = (0, s._)("div", {
                     class: "q-pa-md"
                 }, null, -1),
                 n = (0, s._)("div", {
@@ -15,33 +15,33 @@
                 }, null, -1);
 
             function o(e, t, a, o, d, r) {
                 const c = (0, s.up)("q-item-label"),
                     h = (0, s.up)("element"),
                     u = (0, s.up)("q-tab"),
                     p = (0, s.up)("q-tabs"),
-                    g = (0, s.up)("q-space"),
-                    m = (0, s.up)("q-tooltip"),
-                    y = (0, s.up)("q-btn"),
-                    f = (0, s.up)("q-toolbar"),
+                    m = (0, s.up)("q-space"),
+                    g = (0, s.up)("q-tooltip"),
+                    f = (0, s.up)("q-btn"),
+                    y = (0, s.up)("q-toolbar"),
                     w = (0, s.up)("q-header"),
                     b = (0, s.up)("zone"),
                     k = (0, s.up)("q-page"),
                     v = (0, s.up)("q-page-container"),
                     x = (0, s.up)("q-layout");
                 return (0, s.wg)(), (0, s.j4)(x, {
                     view: "lHh Lpr lFf"
                 }, {
                     default: (0, s.w5)((() => [(0, s.Wm)(w, {
                         elevated: "",
                         class: (0, l.C_)({
                             "bg-deep-purple-9": e.Dark.isActive
                         })
                     }, {
-                        default: (0, s.w5)((() => [(0, s.Wm)(f, null, {
+                        default: (0, s.w5)((() => [(0, s.Wm)(y, null, {
                             default: (0, s.w5)((() => [(0, s.Wm)(c, {
                                 class: "text-h5"
                             }, {
                                 default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.screen.header ? e.screen.header : ""), 1)])),
                                 _: 1
                             }), i, ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.left_toolbar, (t => ((0, s.wg)(), (0, s.j4)(h, {
                                 class: (0, l.C_)(["q-ma-xs", {
@@ -74,31 +74,31 @@
                                     class: "justify-center text-white shadow-2",
                                     "no-caps": "",
                                     name: t.name,
                                     label: t.name,
                                     onClick: a => e.tabclick(t.name)
                                 }, null, 8, ["name", "label", "onClick"]))])))), 256))])),
                                 _: 1
-                            }, 8, ["modelValue"]), (0, s.Wm)(g), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.right_toolbar, (t => ((0, s.wg)(), (0, s.j4)(h, {
+                            }, 8, ["modelValue"]), (0, s.Wm)(m), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.right_toolbar, (t => ((0, s.wg)(), (0, s.j4)(h, {
                                 class: (0, l.C_)(["q-ma-xs", {
                                     "bg-blue-grey-7": e.Dark.isActive,
                                     "bg-blue-5": !e.Dark.isActive
                                 }]),
                                 data: t,
                                 pdata: e.tooldata
-                            }, null, 8, ["class", "data", "pdata"])))), 256)), (0, s.Wm)(y, {
+                            }, null, 8, ["class", "data", "pdata"])))), 256)), (0, s.Wm)(f, {
                                 class: (0, l.C_)(["q-ma-xs", {
                                     "bg-blue-grey-9": e.Dark.isActive
                                 }]),
                                 dense: "",
                                 round: "",
                                 icon: e.Dark.isActive ? "light_mode" : "dark_mode",
                                 onClick: e.switchTheme
                             }, {
-                                default: (0, s.w5)((() => [(0, s.Wm)(m, {
+                                default: (0, s.w5)((() => [(0, s.Wm)(g, {
                                     class: "text-body2"
                                 }, {
                                     default: (0, s.w5)((() => [(0, s.Uk)("Dark/Light mode")])),
                                     _: 1
                                 })])),
                                 _: 1
                             }, 8, ["class", "icon", "onClick"])])),
@@ -153,33 +153,33 @@
             }
             a(71);
             var r = a(698),
                 c = a(8603);
             let h = null,
                 u = {};
             var p;
-            const g = !1;
-            let m = g;
-            const y = ["graph", "textarea", "chart", "block"];
-            const f = window.location.host,
-                w = `${window.location.protocol}//${f}`;
+            const m = !1;
+            let g = m;
+            const f = ["graph", "textarea", "chart", "block"];
+            const y = window.location.host,
+                w = `${window.location.protocol}//${y}`;
             let b = {},
                 k = {},
                 v = {};
 
             function C(e) {
-                p = new WebSocket(g ? "ws://localhost:8000/ws" : `ws://${f}/ws`), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
-                    m && console.log("incoming message", t.data), h.designCycle = 0, e.processMessage(JSON.parse(t.data))
+                p = new WebSocket(m ? "ws://localhost:8000/ws" : `ws://${y}/ws`), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
+                    g && console.log("incoming message", t.data), h.designCycle = 0, e.processMessage(JSON.parse(t.data))
                 }, p.onerror = t => e.error(t), p.onclose = t => {
-                    t.wasClean ? e.info("Connection was finished by the server.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, m && console.info("close code : " + t.code + " reason: " + t.reason)
+                    t.wasClean ? e.info("Connection was finished by the server.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, g && console.info("close code : " + t.code + " reason: " + t.reason)
                 }, h = e
             }
 
             function _(e) {
-                m && console.log("sended", e), p.send(JSON.stringify(e))
+                g && console.log("sended", e), p.send(JSON.stringify(e))
             }
             let q = 0,
                 A = !0;
 
             function D(e) {
                 A = e, e || (v = {})
             }
@@ -231,15 +231,15 @@
                 for (let s of e) s instanceof Array ? t.push(s) : t.push([s]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
 
             function E(e = !1) {
                 for (let t of Object.values(k))
-                    if (t.expanding && (!e || y.includes(t.type))) {
+                    if (t.expanding && (!e || f.includes(t.type))) {
                         t.has_recalc = !0;
                         let e = t.$el;
                         if (e.getBoundingClientRect) {
                             let e = t.$el.getBoundingClientRect();
                             window.innerHeight < e.top + e.height && (t.styleSize = "")
                         }
                     }(0, s.Y3)((() => {
@@ -251,15 +251,15 @@
                             }))
                         }))
                     }))
             }
             let V = (0, c.debounce)(E, 100);
 
             function K(e) {
-                if (m && console.log(`------------------recalc design ${h.designCycle}`), h.designCycle >= 3) return;
+                if (g && console.log(`------------------recalc design ${h.designCycle}`), h.designCycle >= 3) return;
                 h.designCycle++;
                 const t = O(e),
                     a = H(e);
                 for (let [s, l] of Object.entries(t)) {
                     let t = k[s],
                         i = a[s];
                     const [n, o] = i || [0, 1];
@@ -277,19 +277,19 @@
                             }
                         } else if (e.name == t.data.name) {
                         d = t;
                         break
                     }
                     let p = n;
                     p /= o;
-                    let g = e || y.includes(t.type) || t.has_recalc,
-                        m = g ? `width:${Math.ceil(c.clientWidth+p)}px` : "",
-                        f = s.startsWith("_scroll@") ? r.inner.clientHeight : c.clientHeight;
-                    f < 0 && (f = 20);
-                    let w = `height: ${f+l}px; ${m}`;
+                    let m = e || f.includes(t.type) || t.has_recalc,
+                        g = m ? `width:${Math.ceil(c.clientWidth+p)}px` : "",
+                        y = s.startsWith("_scroll@") ? r.inner.clientHeight : c.clientHeight;
+                    y < 0 && (y = 20);
+                    let w = `height: ${y+l}px; ${g}`;
                     w != t.styleSize && (t.styleSize = w), t.has_recalc = !1
                 }
             }
 
             function O(e) {
                 const t = h.screen.blocks;
                 let a = window.innerHeight;
@@ -390,15 +390,15 @@
                     let t = Array.isArray(d) ? d[d.length - 1] : d,
                         a = b[t.name].$el.getBoundingClientRect().right;
                     t = Array.isArray(d) ? d[0] : d;
                     let l = b[t.name].$el.getBoundingClientRect().left,
                         i = s - a + l - 10;
                     const r = [];
                     for (let [s, n] of Object.entries(k))
-                        if (n.expanding_width && (n.fullname.startsWith("_scroll@") || e || y.includes(n.type))) {
+                        if (n.expanding_width && (n.fullname.startsWith("_scroll@") || e || f.includes(n.type))) {
                             let e = s.split("@")[1];
                             if (d.find((t => t.name == e))) {
                                 let e = !0,
                                     t = n.geom().left;
                                 for (let [a, s] of r.entries())
                                     if (s !== n && s.geom().left == t) {
                                         s.geom().scrollWidth < n.geom().scrollWidth ? (r[a] = n, o.set(s.fullname, n.fullname)) : o.set(n.fullname, s.fullname), e = !1;
@@ -587,78 +587,77 @@
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"]))], 8, se)))), 256))])),
                     _: 1
                 }, 8, ["style"])
             }
             var ne = a(8880);
-            const oe = e => ((0, s.dD)("data-v-b72ea538"), e = e(), (0, s.Cn)(), e),
+            const oe = e => ((0, s.dD)("data-v-d4b5cc5e"), e = e(), (0, s.Cn)(), e),
                 de = {
                     key: 4,
                     class: "{'bg-blue-grey-9': Dark.isActive}"
                 },
-                re = ["width", "height"],
-                ce = ["src"],
-                he = {
+                re = ["src"],
+                ce = {
                     key: 18,
                     class: "web-camera-container"
                 },
-                ue = {
+                he = {
                     class: "camera-button"
                 },
-                pe = {
+                ue = {
                     key: 0
                 },
-                ge = {
+                pe = {
                     key: 1
                 },
                 me = {
                     class: "camera-loading"
                 },
-                ye = oe((() => (0, s._)("ul", {
+                ge = oe((() => (0, s._)("ul", {
                     class: "loader-circle"
                 }, [(0, s._)("li"), (0, s._)("li"), (0, s._)("li")], -1))),
-                fe = [ye],
+                fe = [ge],
+                ye = ["height"],
                 we = ["height"],
-                be = ["height"],
-                ke = {
+                be = {
                     key: 1,
                     class: "camera-shoot"
                 },
-                ve = oe((() => (0, s._)("img", {
+                ke = oe((() => (0, s._)("img", {
                     src: "https://img.icons8.com/material-outlined/50/000000/camera--v2.png"
                 }, null, -1))),
-                xe = [ve],
-                Ce = {
+                ve = [ke],
+                xe = {
                     key: 2,
                     class: "camera-download"
                 };
 
-            function _e(e, t, a, i, n, o) {
+            function Ce(e, t, a, i, n, o) {
                 const d = (0, s.up)("q-icon"),
                     r = (0, s.up)("q-img"),
                     c = (0, s.up)("q-badge"),
                     h = (0, s.up)("q-select"),
                     u = (0, s.up)("q-checkbox"),
                     p = (0, s.up)("q-toggle"),
-                    g = (0, s.up)("q-btn"),
-                    m = (0, s.up)("q-btn-toggle"),
-                    y = (0, s.up)("utable"),
-                    f = (0, s.up)("linechart"),
+                    m = (0, s.up)("q-btn"),
+                    g = (0, s.up)("q-btn-toggle"),
+                    f = (0, s.up)("utable"),
+                    y = (0, s.up)("linechart"),
                     w = (0, s.up)("q-input"),
                     b = (0, s.up)("q-tree"),
                     k = (0, s.up)("q-scroll-area"),
                     v = (0, s.up)("q-separator"),
                     x = (0, s.up)("q-uploader"),
                     C = (0, s.up)("cgraph"),
                     _ = (0, s.up)("q-tooltip"),
                     q = (0, s.up)("q-spinner-ios");
                 return "image" == e.type ? ((0, s.wg)(), (0, s.j4)(r, {
                     key: 0,
-                    src: e.data.name,
+                    src: e.data.url,
                     "spinner-color": "blue",
                     onClick: (0, ne.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
                     style: (0, l.j5)(e.elemSize)
                 }, {
                     default: (0, s.w5)((() => [e.data.header ? ((0, s.wg)(), (0, s.iD)("div", {
                         key: 0,
@@ -707,38 +706,38 @@
                 }, null, 8, ["modelValue", "label"])) : "switch" == e.type ? ((0, s.wg)(), (0, s.j4)(p, {
                     key: 3,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[3] || (t[3] = t => e.value = t),
                     color: "primary",
                     label: e.nameLabel,
                     "left-label": ""
-                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, s.wg)(), (0, s.iD)("div", de, [e.showname ? ((0, s.wg)(), (0, s.j4)(g, {
+                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, s.wg)(), (0, s.iD)("div", de, [e.showname ? ((0, s.wg)(), (0, s.j4)(m, {
                     key: 0,
                     ripple: !1,
                     color: "indigo-10",
                     disable: "",
                     label: e.name,
                     "no-caps": ""
-                }, null, 8, ["label"])) : (0, s.kq)("", !0), (0, s.Wm)(m, {
+                }, null, 8, ["label"])) : (0, s.kq)("", !0), (0, s.Wm)(g, {
                     modelValue: e.value,
                     "onUpdate:modelValue": t[4] || (t[4] = t => e.value = t),
                     class: (0, l.C_)({
                         "bg-blue-grey-9": e.Dark.isActive
                     }),
                     "no-caps": "",
                     options: e.data.options.map((e => ({
                         label: e,
                         value: e
                     })))
-                }, null, 8, ["modelValue", "class", "options"])])) : "table" == e.type ? ((0, s.wg)(), (0, s.j4)(y, {
+                }, null, 8, ["modelValue", "class", "options"])])) : "table" == e.type ? ((0, s.wg)(), (0, s.j4)(f, {
                     key: 5,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.styleSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "chart" == e.type ? ((0, s.wg)(), (0, s.j4)(f, {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "chart" == e.type ? ((0, s.wg)(), (0, s.j4)(y, {
                     key: 6,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.styleSize
                 }, null, 8, ["data", "pdata", "styleSize"])) : "edit" == e.type ? ((0, s.wg)(), (0, s.j4)(w, {
                     key: 7,
                     modelValue: e.value,
@@ -814,22 +813,20 @@
                 })) : "text" == e.type ? ((0, s.wg)(), (0, s.iD)("p", {
                     key: 13,
                     class: (0, l.C_)(["q-ma-sm", {
                         white: e.Dark.isActive,
                         black: !e.Dark.isActive
                     }])
                 }, (0, l.zw)(e.value), 3)) : "video" == e.type ? ((0, s.wg)(), (0, s.iD)("video", {
-                    width: e.data.width,
-                    height: e.data.height,
-                    key: e.data.src,
+                    key: e.fullname,
                     controls: ""
                 }, [(0, s._)("source", {
-                    src: e.data.src,
+                    src: e.data.url,
                     type: "video/mp4"
-                }, null, 8, ce)], 8, re)) : "uploader" == e.type ? ((0, s.wg)(), (0, s.j4)(x, {
+                }, null, 8, re)])) : "uploader" == e.type ? ((0, s.wg)(), (0, s.j4)(x, {
                     key: 15,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: e.host_path,
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
@@ -854,22 +851,22 @@
                     }),
                     color: e.Dark.isActive ? "purple-10" : "blue"
                 }, null, 8, ["label", "url", "onUploaded", "onAdded", "class", "color"])) : "graph" == e.type ? ((0, s.wg)(), (0, s.j4)(C, {
                     key: 17,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.elemSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, s.wg)(), (0, s.iD)("div", he, [(0, s._)("div", ue, [(0, s._)("button", {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, s.wg)(), (0, s.iD)("div", ce, [(0, s._)("div", he, [(0, s._)("button", {
                     class: (0, l.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
                     }]),
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.toggleCamera && e.toggleCamera(...t))
-                }, [e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("span", ge, "Close Camera")) : ((0, s.wg)(), (0, s.iD)("span", pe, "Open Camera"))], 2)]), (0, s.wy)((0, s._)("div", me, fe, 512), [
+                }, [e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("span", pe, "Close Camera")) : ((0, s.wg)(), (0, s.iD)("span", ue, "Open Camera"))], 2)]), (0, s.wy)((0, s._)("div", me, fe, 512), [
                     [ne.F8, e.isCameraOpen && e.isLoading]
                 ]), e.isCameraOpen ? (0, s.wy)(((0, s.wg)(), (0, s.iD)("div", {
                     key: 0,
                     class: (0, l.C_)(["camera-box", {
                         flash: e.isShotPhoto
                     }])
                 }, [(0, s._)("div", {
@@ -877,33 +874,33 @@
                         flash: e.isShotPhoto
                     }])
                 }, null, 2), (0, s.wy)((0, s._)("video", {
                     ref: "camera",
                     width: 450,
                     height: 337.5,
                     autoplay: ""
-                }, null, 8, we), [
+                }, null, 8, ye), [
                     [ne.F8, !e.isPhotoTaken]
                 ]), (0, s.wy)((0, s._)("canvas", {
                     id: "photoTaken",
                     ref: "canvas",
                     width: 450,
                     height: 337.5
-                }, null, 8, be), [
+                }, null, 8, we), [
                     [ne.F8, e.isPhotoTaken]
                 ])], 2)), [
                     [ne.F8, !e.isLoading]
-                ]) : (0, s.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, s.wg)(), (0, s.iD)("div", ke, [(0, s._)("button", {
+                ]) : (0, s.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, s.wg)(), (0, s.iD)("div", be, [(0, s._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[12] || (t[12] = (...t) => e.takePhoto && e.takePhoto(...t))
-                }, xe)])) : (0, s.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("div", Ce, [(0, s.Wm)(g, {
+                }, ve)])) : (0, s.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("div", xe, [(0, s.Wm)(m, {
                     onClick: e.downloadImage,
                     label: "Send"
-                }, null, 8, ["onClick"])])) : (0, s.kq)("", !0)])) : "" != e.showname ? ((0, s.wg)(), (0, s.j4)(g, {
+                }, null, 8, ["onClick"])])) : (0, s.kq)("", !0)])) : "" != e.showname ? ((0, s.wg)(), (0, s.j4)(m, {
                     key: 19,
                     "no-caps": "",
                     class: (0, l.C_)({
                         "bg-blue-grey-8": e.Dark.isActive
                     }),
                     label: e.name,
                     icon: e.data.icon,
@@ -913,15 +910,15 @@
                         key: 0,
                         class: "text-body2"
                     }, {
                         default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, s.kq)("", !0)])),
                     _: 1
-                }, 8, ["class", "label", "icon", "onClick"])) : e.data.spinner ? ((0, s.wg)(), (0, s.j4)(g, {
+                }, 8, ["class", "label", "icon", "onClick"])) : e.data.spinner ? ((0, s.wg)(), (0, s.j4)(m, {
                     key: 21,
                     "no-caps": "",
                     dense: "",
                     round: "",
                     class: (0, l.C_)({
                         "bg-blue-grey-8": e.Dark.isActive
                     }),
@@ -933,15 +930,15 @@
                         key: 0,
                         class: "text-body2"
                     }, {
                         default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, s.kq)("", !0)])),
                     _: 1
-                }, 8, ["class", "onClick"])) : ((0, s.wg)(), (0, s.j4)(g, {
+                }, 8, ["class", "onClick"])) : ((0, s.wg)(), (0, s.j4)(m, {
                     key: 20,
                     "no-caps": "",
                     dense: "",
                     round: "",
                     class: (0, l.C_)({
                         "bg-blue-grey-8": e.Dark.isActive
                     }),
@@ -954,34 +951,34 @@
                     }, {
                         default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, s.kq)("", !0)])),
                     _: 1
                 }, 8, ["class", "icon", "onClick"]))
             }
-            const qe = {
+            const _e = {
                     key: 0
                 },
-                Ae = {
+                qe = {
                     class: "row"
                 },
-                De = ["onClick"];
+                Ae = ["onClick"];
 
-            function Se(e, t, a, i, n, o) {
+            function De(e, t, a, i, n, o) {
                 const d = (0, s.up)("q-icon"),
                     r = (0, s.up)("q-tooltip"),
                     c = (0, s.up)("q-input"),
                     h = (0, s.up)("q-btn"),
                     u = (0, s.up)("q-th"),
                     p = (0, s.up)("q-tr"),
-                    g = (0, s.up)("q-checkbox"),
-                    m = (0, s.up)("q-select"),
-                    y = (0, s.up)("q-td"),
-                    f = (0, s.up)("q-table");
-                return (0, s.wg)(), (0, s.j4)(f, {
+                    m = (0, s.up)("q-checkbox"),
+                    g = (0, s.up)("q-select"),
+                    f = (0, s.up)("q-td"),
+                    y = (0, s.up)("q-table");
+                return (0, s.wg)(), (0, s.j4)(y, {
                     "virtual-scroll": "",
                     dense: e.data.dense,
                     style: (0, l.j5)(e.styleSize),
                     flat: "",
                     filter: e.search,
                     ref: "table",
                     virtualScrollSliceSize: "100",
@@ -991,15 +988,15 @@
                     title: e.name,
                     rows: e.rows,
                     columns: e.columns,
                     selection: e.singleMode ? "single" : "multiple",
                     selected: e.selected,
                     "onUpdate:selected": t[2] || (t[2] = t => e.selected = t)
                 }, {
-                    "top-right": (0, s.w5)((() => [!1 !== e.data.tools ? ((0, s.wg)(), (0, s.iD)("div", qe, [(0, s._)("div", Ae, [(0, s.Wm)(c, {
+                    "top-right": (0, s.w5)((() => [!1 !== e.data.tools ? ((0, s.wg)(), (0, s.iD)("div", _e, [(0, s._)("div", qe, [(0, s.Wm)(c, {
                         modelValue: e.search,
                         "onUpdate:modelValue": t[1] || (t[1] = t => e.search = t),
                         label: "Search",
                         dense: "",
                         ref: "searchField"
                     }, (0, s.Nv)({
                         append: (0, s.w5)((() => ["" != e.search ? ((0, s.wg)(), (0, s.j4)(d, {
@@ -1168,25 +1165,25 @@
                         }, 1032, ["class", "props"])))), 128))])),
                         _: 2
                     }, 1032, ["props"])])),
                     body: (0, s.w5)((t => [(0, s.Wm)(p, {
                         props: t,
                         onClick: e => t.selected = !t.selected
                     }, {
-                        default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.columns, ((a, i) => ((0, s.wg)(), (0, s.j4)(y, {
+                        default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.columns, ((a, i) => ((0, s.wg)(), (0, s.j4)(f, {
                             key: a.name,
                             props: t
                         }, {
-                            default: (0, s.w5)((() => ["boolean" == typeof t.row[a.name] ? ((0, s.wg)(), (0, s.j4)(g, {
+                            default: (0, s.w5)((() => ["boolean" == typeof t.row[a.name] ? ((0, s.wg)(), (0, s.j4)(m, {
                                 key: 0,
                                 modelValue: t.row[a.name],
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, s => e.change_switcher(t.row, a.name, i)],
                                 dense: "",
                                 disable: !e.editMode
-                            }, null, 8, ["modelValue", "onUpdate:modelValue", "disable"])) : e.editMode && "complete" in e.data && i == e.cedit && e.redit == t.row.iiid ? ((0, s.wg)(), (0, s.j4)(m, {
+                            }, null, 8, ["modelValue", "onUpdate:modelValue", "disable"])) : e.editMode && "complete" in e.data && i == e.cedit && e.redit == t.row.iiid ? ((0, s.wg)(), (0, s.j4)(g, {
                                 key: 1,
                                 dense: "",
                                 "model-value": t.row[a.name],
                                 "use-input": "",
                                 "hide-selected": "",
                                 "fill-input": "",
                                 autofocus: "",
@@ -1204,35 +1201,35 @@
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, e.change],
                                 dense: "",
                                 onKeydown: e.keyInput,
                                 autofocus: ""
                             }, null, 8, ["modelValue", "onUpdate:modelValue", "onKeydown"])) : ((0, s.wg)(), (0, s.iD)("div", {
                                 key: 3,
                                 onClick: a => e.select(t.row.iiid, i)
-                            }, (0, l.zw)(t.row[a.name]), 9, De))])),
+                            }, (0, l.zw)(t.row[a.name]), 9, Ae))])),
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props", "onClick"])])),
                     _: 1
                 }, 8, ["dense", "style", "filter", "title", "rows", "columns", "selection", "selected"])
             }
-            var je = a(1959),
-                ze = a(9058);
+            var Se = a(1959),
+                je = a(9058);
 
-            function Ze(e, t) {
+            function ze(e, t) {
                 return e.length === t.length && e.every(((e, a) => t[a] && e.iiid == t[a].iiid))
             }
-            const $e = (0, s.aZ)({
+            const Ze = (0, s.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
-                    } = (0, je.BK)(e);
+                    } = (0, Se.BK)(e);
                     let l = (0, s.Fl)((() => {
                             let e = [],
                                 a = t.value;
                             const s = a.headers,
                                 l = s.length,
                                 i = a.rows,
                                 n = i.length;
@@ -1246,61 +1243,61 @@
                         })),
                         i = () => {
                             let e = t.value,
                                 a = null === e.value || 0 == l.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => l.value[e])) : [l.value[e.value]];
                             return a
                         },
                         n = i(),
-                        o = (0, je.iH)(n),
-                        d = (0, je.iH)(n),
-                        r = (0, je.iH)(!Array.isArray(t.value.value)),
+                        o = (0, Se.iH)(n),
+                        d = (0, Se.iH)(n),
+                        r = (0, Se.iH)(!Array.isArray(t.value.value)),
                         c = (e, s) => {
                             _([a.value.name, t.value.name, e, s])
                         },
                         h = (0, s.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
                         u = (0, s.Fl)((() => t.value.value));
                     return (0, s.YP)(l, ((e, t) => {
                         d.value = i(), o.value = d.value
                     })), (0, s.YP)(t, ((e, a) => {
-                        m && console.log("data update", a.name), d.value = i(), o.value = d.value, r.value = !Array.isArray(t.value.value)
+                        g && console.log("data update", a.name), d.value = i(), o.value = d.value, r.value = !Array.isArray(t.value.value)
                     })), {
                         rows: l,
                         value: h,
                         selected: d,
                         singleMode: r,
                         sendMessage: c,
                         datavalue: u,
                         updated: o
                     }
                 },
                 data() {
                     return {
-                        Dark: ze.Z,
+                        Dark: je.Z,
                         search: "",
                         editMode: !1,
                         options: [],
                         cedit: null
                     }
                 },
                 methods: {
                     select(e, t) {
-                        this.editMode && (this.cedit = t, m && console.log("selected", e, this.cedit))
+                        this.editMode && (this.cedit = t, g && console.log("selected", e, this.cedit))
                     },
                     change_switcher(e, t, a) {
                         if (console.log(e, t, a, e[t]), this.editMode) {
                             this.cedit = a;
                             const s = e.iiid;
                             let l = this.data.rows;
                             l[s][a] = e[t], this.sendMessage("modify", [e[t],
                                 [s, a]
                             ])
                         }
                     },
                     change(e) {
-                        if (m && console.log("changed", this.data.headers[this.cedit], e), this.editMode && this.selected.length) {
+                        if (g && console.log("changed", this.data.headers[this.cedit], e), this.editMode && this.selected.length) {
                             const t = this.selected[0].iiid;
                             let a = this.data.rows;
                             a[t][this.cedit] = e, this.sendMessage("modify", [e, [t, this.cedit]])
                         }
                     },
                     keyInput(e) {
                         if ("Control" == e.key) return;
@@ -1358,15 +1355,15 @@
                     },
                     append() {
                         let e = this.data.rows,
                             t = e.length,
                             a = this;
                         j(this, [t, this.search], (function(s) {
                             if (!Array.isArray(s)) return h.error(s);
-                            m && console.log("added row", s), a.search = "", e.push(s), setTimeout((() => {
+                            g && console.log("added row", s), a.search = "", e.push(s), setTimeout((() => {
                                 let e = a.rows;
                                 a.selected = [e[t]], a.showSelected(), a.editMode || a.switchEdit(), a.select(e[t], 0)
                             }), 100)
                         }), "append")
                     },
                     showSelected() {
                         let e = this.$refs.table;
@@ -1399,15 +1396,15 @@
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
                         const t = this.data;
-                        if (!Ze(this.updated, this.selected)) {
+                        if (!ze(this.updated, this.selected)) {
                             let e = this.selected.length;
                             t.value = this.singleMode ? 1 == e ? this.selected[0].iiid : null : this.selected.map((e => e.iiid)), this.sendMessage("changed", t.value), this.updated = this.selected
                         }
                         t.show && (this.showSelected(), t.show = !1)
                     }
                 },
                 computed: {
@@ -1432,52 +1429,52 @@
                 },
                 props: {
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
-            var Me = a(9267),
-                We = a(4842),
-                Ee = a(8870),
-                Ve = a(2165),
-                Ke = a(8186),
-                Oe = a(2414),
-                He = a(3884),
-                Qe = a(5735),
-                Ue = a(7208);
-            const Ne = (0, U.Z)($e, [
-                    ["render", Se]
+            var $e = a(9267),
+                Me = a(4842),
+                We = a(8870),
+                Ee = a(2165),
+                Ve = a(8186),
+                Ke = a(2414),
+                Oe = a(3884),
+                He = a(5735),
+                Qe = a(7208);
+            const Ue = (0, U.Z)(Ze, [
+                    ["render", De]
                 ]),
-                Pe = Ne;
-            R()($e, "components", {
-                QTable: Me.Z,
-                QInput: We.Z,
+                Ne = Ue;
+            R()(Ze, "components", {
+                QTable: $e.Z,
+                QInput: Me.Z,
                 QIcon: T.Z,
-                QTooltip: Ee.Z,
-                QBtn: Ve.Z,
-                QTr: Ke.Z,
-                QTh: Oe.Z,
-                QTd: He.Z,
-                QCheckbox: Qe.Z,
-                QSelect: Ue.Z
+                QTooltip: We.Z,
+                QBtn: Ee.Z,
+                QTr: Ve.Z,
+                QTh: Ke.Z,
+                QTd: Oe.Z,
+                QCheckbox: He.Z,
+                QSelect: Qe.Z
             });
-            const Te = ["nodes", "edges"];
+            const Pe = ["nodes", "edges"];
 
-            function Fe(e, t, a, i, n, o) {
+            function Te(e, t, a, i, n, o) {
                 return (0, s.wg)(), (0, s.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, l.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Te)
+                }, null, 12, Pe)
             }
-            var Ie = a(2393),
-                Re = a.n(Ie);
-            const Le = Re().stylesheet().selector("node").css({
+            var Fe = a(2393),
+                Ie = a.n(Fe);
+            const Re = Ie().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#26A69A",
                     "font-size": "14px"
                 }).selector(".selected").css({
                     "background-color": "#4286f4",
                     "border-color": "#ff5555",
                     "font-size": "14px"
@@ -1503,45 +1500,45 @@
                     label: "data(label)",
                     "text-rotation": "autorotate",
                     "text-margin-x": "-8px",
                     "text-margin-y": "-8px",
                     color: "#388E3C",
                     "font-size": "12px"
                 }),
-                Be = {
+                Le = {
                     animate: !0,
                     randomize: !0
                 };
 
-            function Ye(e, t) {
+            function Be(e, t) {
                 if (e.length != t.length) return !0;
                 for (let a = 0; a < e.length; a++)
                     if (e[a].id != t[a].id || e[a].label != t[a].label) return !0;
                 return !1
             }
-            const Xe = (0, s.aZ)({
+            const Ye = (0, s.aZ)({
                     name: "cgraph",
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
                         return {
                             cy: null,
-                            style: Le,
-                            layoutOptions: Be,
+                            style: Re,
+                            layoutOptions: Le,
                             selectedNodes: [],
                             selectedEdges: [],
                             oldNodes: [],
                             oldEdges: []
                         }
                     },
                     mounted() {
-                        let e = Re()({
+                        let e = Ie()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1657,15 +1654,15 @@
                                 for (let t of e) a.edges("[id='" + t + "']").addClass("highlighted")
                             }
                         },
                         data: {
                             handler(e, t) {
                                 let a = e.value,
                                     s = !1;
-                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Ye(e.nodes, this.oldNodes) && (s = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Ye(e.edges, this.oldEdges) && (s = !0, this.oldEdges = e.edges), s && null != this.cy) {
+                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Be(e.nodes, this.oldNodes) && (s = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Be(e.edges, this.oldEdges) && (s = !0, this.oldEdges = e.edges), s && null != this.cy) {
                                     this.cy.json({
                                         elements: {
                                             nodes: this.nodes,
                                             edges: this.edges
                                         }
                                     });
                                     let e = this.data.method;
@@ -1682,58 +1679,59 @@
                             this.cy.style(e)
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
-                Ge = (0, U.Z)(Xe, [
-                    ["render", Fe]
+                Xe = (0, U.Z)(Ye, [
+                    ["render", Te]
                 ]),
-                Je = Ge;
+                Ge = Xe;
 
-            function et(e, t, a, i, n, o) {
+            function Je(e, t, a, i, n, o) {
                 const d = (0, s.up)("v-chart");
                 return (0, s.wg)(), (0, s.j4)(d, {
                     ref: "chart",
                     "manual-update": !0,
                     onClick: o.clicked,
                     style: (0, l.j5)(a.styleSize ? a.styleSize : "width: 300px; height: 200px"),
                     autoresize: !0
                 }, null, 8, ["onClick", "style"])
             }
-            var tt = a(7559),
-                at = a(6938),
-                st = a(1006),
-                lt = a(6080),
-                it = a(3526),
-                nt = a(763),
-                ot = a(546),
-                dt = a(6902),
-                rt = a(2826),
-                ct = a(5256),
-                ht = a(3825),
-                ut = a(8825);
-            (0, nt.D)([at.N, st.N, it.N, lt.N]), (0, nt.D)([ot.N, dt.N, rt.N, ct.N, ht.N]);
-            let pt = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"];
-            const gt = {
+            var et = a(7559),
+                tt = a(6938),
+                at = a(1006),
+                st = a(6080),
+                lt = a(3526),
+                it = a(763),
+                nt = a(546),
+                ot = a(6902),
+                dt = a(2826),
+                rt = a(5256),
+                ct = a(3825),
+                ht = a(8825);
+            (0, it.D)([tt.N, at.N, lt.N, st.N]), (0, it.D)([nt.N, ot.N, dt.N, rt.N, ct.N]);
+            let ut = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"];
+            const pt = {
                     name: "linechart",
                     components: {
-                        VChart: tt.ZP
+                        VChart: et.ZP
                     },
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
-                        const e = (0, ut.Z)();
+                        const e = (0, ht.Z)();
                         return {
                             $q: e,
                             model: !1,
+                            animation: null,
                             markPoint: null,
                             options: {
                                 responsive: !0,
                                 maintainAspectRatio: !1,
                                 legend: {
                                     data: [],
                                     bottom: 10,
@@ -1797,17 +1795,19 @@
                             }))
                         },
                         clicked(e) {
                             let t = [e.dataIndex, this.options.series[e.seriesIndex].data[e.dataIndex]];
                             this.processCoord(t, this.markPoint.data, h.shiftKey);
                             let a = this.markPoint.data.map((e => e.coord[0])),
                                 s = this.data;
-                            s.value = Array.isArray(s.value) || a.length > 1 ? a : a.length ? a[0] : null, this.$refs.chart.setOption(this.options, {
-                                replaceMerge: "markPoint"
-                            }), _([this.pdata.name, this.data.name, "changed", this.data.value])
+                            if (s.value = Array.isArray(s.value) || a.length > 1 ? a : a.length ? a[0] : null, this.animation) {
+                                let e = this.options.dataZoom;
+                                e[0].start = this.animation.start, e[1].start = this.animation.start, e[0].end = this.animation.end, e[1].end = this.animation.end
+                            }
+                            this.setOptions(), _([this.pdata.name, this.data.name, "changed", this.data.value])
                         },
                         calcSeries() {
                             this.options.toolbox.feature.mySwitcher = {
                                 show: !0,
                                 title: "Switch view to the table",
                                 icon: "image:M0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V2zm15 2h-4v3h4V4zm0 4h-4v3h4V8zm0 4h-4v3h3a1 1 0 0 0 1-1v-2zm-5 3v-3H6v3h4zm-5 0v-3H1v2a1 1 0 0 0 1 1h3zm-4-4h4V8H1v3zm0-4h4V4H1v3zm5-3v3h4V4H6zm4 4H6v3h4V8z",
                                 onclick: () => {
@@ -1825,15 +1825,15 @@
                             for (let n = 0; n < s.length; n++) s[n] = "i" == s[n] ? -1 : parseInt(s[n]), l.push([]), n && (this.options.series.push({
                                 name: t[s[n]],
                                 type: "line",
                                 symbol: "circle",
                                 symbolSize: 10,
                                 sampling: "lttb",
                                 itemStyle: {
-                                    color: pt[n]
+                                    color: ut[n]
                                 },
                                 data: l[n]
                             }), this.options.legend.data.push(t[s[n]]));
                             this.options.xAxis.data = l[0];
                             let i = this.data.rows;
                             for (let n = 0; n < i.length; n++)
                                 for (let e = 0; e < s.length; e++) l[e].push(-1 == s[e] ? n : i[n][s[e]]);
@@ -1856,37 +1856,40 @@
                                     data: e
                                 }, this.options.series[1].markPoint = this.markPoint
                             }
                             this.setOptions()
                         }
                     },
                     mounted() {
-                        this.calcSeries()
+                        this.calcSeries();
+                        let e = this;
+                        this.$refs.chart.chart.on("datazoom", (function(t) {
+                            (t.start || t.end) && (e.animation = t)
+                        }))
                     }
                 },
-                mt = (0, U.Z)(gt, [
-                    ["render", et],
-                    ["__scopeId", "data-v-981bab46"]
+                mt = (0, U.Z)(pt, [
+                    ["render", Je]
                 ]),
-                yt = mt;
+                gt = mt;
 
             function ft(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
                 a.open("POST", w, !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const wt = (0, s.aZ)({
+            const yt = (0, s.aZ)({
                 name: "element",
                 components: {
-                    utable: Pe,
-                    cgraph: Je,
-                    linechart: yt
+                    utable: Ne,
+                    cgraph: Ge,
+                    linechart: gt
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
                         0 !== e.length && (0 !== this.fileArr.length ? (this.$refs.uploaderRef.removeFile(this.fileArr[0]), this.fileArr.splice(0, 1, e[0])) : this.fileArr.push(e[0]))
@@ -1979,15 +1982,15 @@
                     k[this.fullname] = this
                 },
                 mounted() {
                     k[this.fullname] = this, this.data.focus && this.$refs.inputRef.$el.focus()
                 },
                 data() {
                     return {
-                        Dark: ze.Z,
+                        Dark: je.Z,
                         value: this.data.value,
                         styleSize: h.visibility ? S(this) : null,
                         has_recalc: !0,
                         host_path: w,
                         options: [],
                         expandedKeys: [],
                         thumbStyle: {
@@ -2100,58 +2103,58 @@
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
                         this.styleSize || (this.styleSize = ""), this.value = this.data.value, this.updated = this.value, k[this.fullname] = this
                     }
                 }
             });
-            var bt = a(4027),
-                kt = a(9721),
-                vt = a(8886),
-                xt = a(8761),
-                Ct = a(1232),
-                _t = a(5551),
-                qt = a(5869),
-                At = a(1745),
-                Dt = a(8506);
-            const St = (0, U.Z)(wt, [
-                    ["render", _e],
-                    ["__scopeId", "data-v-b72ea538"]
+            var wt = a(4027),
+                bt = a(9721),
+                kt = a(8886),
+                vt = a(8761),
+                xt = a(1232),
+                Ct = a(5551),
+                _t = a(5869),
+                qt = a(1745),
+                At = a(8506);
+            const Dt = (0, U.Z)(yt, [
+                    ["render", Ce],
+                    ["__scopeId", "data-v-d4b5cc5e"]
                 ]),
-                jt = St;
+                St = Dt;
 
-            function zt(e) {
+            function jt(e) {
                 let t = e.type;
                 return "tree" == t || "table" == t || "list" == t || "textarea" == t || "graph" == t || "chart" == t
             }
-            R()(wt, "components", {
-                QImg: bt.Z,
+            R()(yt, "components", {
+                QImg: wt.Z,
                 QIcon: T.Z,
-                QSelect: Ue.Z,
-                QBadge: kt.Z,
-                QCheckbox: Qe.Z,
-                QToggle: vt.Z,
-                QBtn: Ve.Z,
-                QBtnToggle: xt.Z,
-                QInput: We.Z,
-                QScrollArea: Ct.Z,
-                QTree: _t.Z,
-                QSeparator: qt.Z,
-                QUploader: At.Z,
-                QTooltip: Ee.Z,
-                QSpinnerIos: Dt.Z
+                QSelect: Qe.Z,
+                QBadge: bt.Z,
+                QCheckbox: He.Z,
+                QToggle: kt.Z,
+                QBtn: Ee.Z,
+                QBtnToggle: vt.Z,
+                QInput: Me.Z,
+                QScrollArea: xt.Z,
+                QTree: Ct.Z,
+                QSeparator: _t.Z,
+                QUploader: qt.Z,
+                QTooltip: We.Z,
+                QSpinnerIos: At.Z
             });
-            const Zt = (0, s.aZ)({
+            const zt = (0, s.aZ)({
                 name: "block",
                 components: {
-                    element: jt
+                    element: St
                 },
                 data() {
                     return {
-                        Dark: ze.Z,
+                        Dark: je.Z,
                         styleSize: "",
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
                             opacity: .75
@@ -2208,16 +2211,16 @@
                         return this.expanding
                     },
                     only_fixed_elems() {
                         if (this.data.scroll) return !1;
                         for (let e of this.data.value)
                             if (Array.isArray(e)) {
                                 for (let t of e)
-                                    if (zt(t)) return !1
-                            } else if (zt(e)) return !1;
+                                    if (jt(t)) return !1
+                            } else if (jt(e)) return !1;
                         return !0
                     },
                     expanding_height() {
                         return !this.data.height && (this.expanding || this.only_fixed_elems)
                     },
                     tops() {
                         let e = this.data.value;
@@ -2228,25 +2231,25 @@
                     data: {
                         type: Object,
                         required: !0
                     }
                 },
                 watch: {
                     data(e) {
-                        m && console.log("data update", this.name), b[this.name] = this, this.expanding && (this.styleSize = h.visibility ? S(this) : "", k[this.fullname] = this)
+                        g && console.log("data update", this.name), b[this.name] = this, this.expanding && (this.styleSize = h.visibility ? S(this) : "", k[this.fullname] = this)
                     }
                 }
             });
-            var $t = a(151);
-            const Mt = (0, U.Z)(Zt, [
+            var Zt = a(151);
+            const $t = (0, U.Z)(zt, [
                     ["render", ie]
                 ]),
-                Wt = Mt;
+                Mt = $t;
 
-            function Et() {
+            function Wt() {
                 console.log();
                 let e = A && k.size == v.size;
                 if (e)
                     for (let [t, a] of Object.entries(k))
                         if (!v[t]) {
                             e = !1;
                             break
@@ -2254,44 +2257,44 @@
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
                             h.visible(!0)
                         }))
                     }))
                 })))
             }
-            R()(Zt, "components", {
-                QCard: $t.Z,
+            R()(zt, "components", {
+                QCard: Zt.Z,
                 QIcon: T.Z,
-                QScrollArea: Ct.Z
+                QScrollArea: xt.Z
             });
-            const Vt = (0, s.aZ)({
+            const Et = (0, s.aZ)({
                     name: "zone",
                     components: {
-                        block: Wt
+                        block: Mt
                     },
                     props: {
                         data: Object
                     },
                     updated(e) {
                         (0, s.Y3)((() => {
                             requestAnimationFrame((() => {
-                                requestAnimationFrame(Et)
+                                requestAnimationFrame(Wt)
                             }))
                         }))
                     }
                 }),
-                Kt = (0, U.Z)(Vt, [
+                Vt = (0, U.Z)(Et, [
                     ["render", J]
                 ]),
-                Ot = Kt,
-                Ht = {
+                Kt = Vt,
+                Ot = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function Qt(e, t, a, i, n, o) {
+            function Ht(e, t, a, i, n, o) {
                 const d = (0, s.up)("block"),
                     r = (0, s.up)("q-item-label"),
                     c = (0, s.up)("q-space"),
                     h = (0, s.up)("q-btn"),
                     u = (0, s.up)("q-card"),
                     p = (0, s.up)("q-dialog");
                 return (0, s.wg)(), (0, s.j4)(p, {
@@ -2308,33 +2311,33 @@
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, s.kq)("", !0), (0, s.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, s._)("div", Ht, [(0, s.Wm)(c), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(a.buttons, (e => ((0, s.wg)(), (0, s.j4)(h, {
+                        }), (0, s._)("div", Ot, [(0, s.Wm)(c), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(a.buttons, (e => ((0, s.wg)(), (0, s.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             "no-caps": "",
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => o.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
                 }, 8, ["onHide", "onKeyup"])
             }
-            const Ut = {
+            const Qt = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
-                    block: Wt
+                    block: Mt
                 },
                 emits: ["ok", "hide"],
                 methods: {
                     show() {
                         this.$refs.dialog.show()
                     },
                     sendMessage(e) {
@@ -2353,39 +2356,39 @@
                         this.$emit("ok"), this.hide()
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
-            var Nt = a(5926),
-                Pt = a(2025);
-            const Tt = (0, U.Z)(Ut, [
-                    ["render", Qt]
+            var Ut = a(5926),
+                Nt = a(2025);
+            const Pt = (0, U.Z)(Qt, [
+                    ["render", Ht]
                 ]),
-                Ft = Tt;
-            R()(Ut, "components", {
-                QDialog: Nt.Z,
-                QCard: $t.Z,
+                Tt = Pt;
+            R()(Qt, "components", {
+                QDialog: Ut.Z,
+                QCard: Zt.Z,
                 QItemLabel: F.Z,
-                QSpace: Pt.Z,
-                QBtn: Ve.Z
+                QSpace: Nt.Z,
+                QBtn: Ee.Z
             });
-            var It = a(589);
-            let Rt = "theme";
+            var Ft = a(589);
+            let It = "theme";
             try {
-                ze.Z.set(It.Z.getItem(Rt))
-            } catch (ia) {}
-            let Lt = null;
-            const Bt = (0, s.aZ)({
+                je.Z.set(Ft.Z.getItem(It))
+            } catch (la) {}
+            let Rt = null;
+            const Lt = (0, s.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
-                        Dark: ze.Z,
+                        Dark: je.Z,
                         menu: [],
                         tab: "",
                         tooldata: {
                             name: "toolbar"
                         },
                         localServer: !0,
                         statusConnect: !1,
@@ -2396,16 +2399,16 @@
                         visibility: !0,
                         designCycle: 0,
                         shiftKey: !1
                     }
                 },
                 components: {
                     menubar: B,
-                    zone: Ot,
-                    element: jt
+                    zone: Kt,
+                    element: St
                 },
                 created() {
                     C(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
@@ -2415,15 +2418,15 @@
                     },
                     right_toolbar() {
                         return this.screen.toolbar.filter((e => e.right))
                     }
                 },
                 methods: {
                     switchTheme() {
-                        ze.Z.set(!ze.Z.isActive), It.Z.set(Rt, ze.Z.isActive)
+                        je.Z.set(!je.Z.isActive), Ft.Z.set(It, je.Z.isActive)
                     },
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
                         _(["root", e])
                     },
@@ -2433,23 +2436,23 @@
                     handleKeyDown(e) {
                         "Shift" == e.key && (this.shiftKey = !0)
                     },
                     handleKeyUp(e) {
                         "Shift" == e.key && (this.shiftKey = !1)
                     },
                     onResize(e) {
-                        m && console.log("window has been resized", window.innerHeight, window.innerWidth), this.designCycle = 0, V()
+                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), this.designCycle = 0, V()
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: Ft
+                                component: Tt
                             },
                             {
                                 height: a,
                                 ...s
                             } = e;
                         s.width = 750;
                         let l = {
@@ -2468,57 +2471,57 @@
                         let a = t,
                             s = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == Lt ? (s = {
+                        "progress" == t ? null == Rt ? (s = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, Lt = this.$q.notify(s)) : null == e ? (Lt(), Lt = null) : (s = {
+                        }, Rt = this.$q.notify(s)) : null == e ? (Rt(), Rt = null) : (s = {
                             caption: e
-                        }, Lt(s)) : ("error" == t && s.type, this.$q.notify(s))
+                        }, Rt(s)) : ("error" == t && s.type, this.$q.notify(s))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if ("screen" == e.type) z(), this.screen.name != e.name && (D(!1), m || this.visible(!1)), this.screen = e, this.menu = e.menu.map((e => ({
+                        if ("screen" == e.type) z(), this.screen.name != e.name && (D(!1), g || this.visible(!1)), this.screen = e, this.menu = e.menu.map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
                         }))), this.tab = this.screen.name;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = Ft, t.componentProps = {
+                            t.component = Tt, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
                         } else if ("answer" == e.type) M(e);
                         else {
                             let t = e.updates && e.updates.length;
                             t && $(e.updates);
                             let a = !1;
                             ["error", "progress", "warning", "info"].includes(e.type) && (this.notify(e.value, e.type), a = !0), a || t || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        Lt && "progress" != e.type && this.notify(null, "progress")
+                        Rt && "progress" != e.type && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     window.addEventListener("resize", this.onResize);
                     const e = new ResizeObserver((e => {
                         let t = document.documentElement.scrollWidth > window.innerWidth || document.documentElement.scrollHeight > window.innerHeight;
                         t && E(!0)
@@ -2526,34 +2529,34 @@
                     let t = this.$refs.page.$el;
                     e.observe(t), window.addEventListener("keydown", this.handleKeyDown), window.addEventListener("keyup", this.handleKeyUp)
                 },
                 beforeUnmount() {
                     window.removeEventListener("keydown", this.handleKeyDown), window.removeEventListener("keyup", this.handleKeyUp)
                 }
             });
-            var Yt = a(9214),
-                Xt = a(3812),
-                Gt = a(9570),
-                Jt = a(7547),
-                ea = a(3269),
-                ta = a(2652),
-                aa = a(4379);
-            const sa = (0, U.Z)(Bt, [
+            var Bt = a(9214),
+                Yt = a(3812),
+                Xt = a(9570),
+                Gt = a(7547),
+                Jt = a(3269),
+                ea = a(2652),
+                ta = a(4379);
+            const aa = (0, U.Z)(Lt, [
                     ["render", o]
                 ]),
-                la = sa;
-            R()(Bt, "components", {
-                QLayout: Yt.Z,
-                QHeader: Xt.Z,
-                QToolbar: Gt.Z,
-                QBtn: Ve.Z,
+                sa = aa;
+            R()(Lt, "components", {
+                QLayout: Bt.Z,
+                QHeader: Yt.Z,
+                QToolbar: Xt.Z,
+                QBtn: Ee.Z,
                 QItemLabel: F.Z,
-                QTabs: Jt.Z,
-                QTab: ea.Z,
-                QSpace: Pt.Z,
-                QTooltip: Ee.Z,
-                QPageContainer: ta.Z,
-                QPage: aa.Z
+                QTabs: Gt.Z,
+                QTab: Jt.Z,
+                QSpace: Nt.Z,
+                QTooltip: We.Z,
+                QPageContainer: ea.Z,
+                QPage: ta.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.9.7/unigui/web/js/vendor.8cb03aaa.js` & `unigui-1.9.8/unigui/web/js/vendor.8cb03aaa.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/js/193.283445be.js` & `unigui-1.9.8/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui/web/index.html` & `unigui-1.9.8/unigui/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.8cb03aaa.js></script><script defer src=js/app.38493c13.js></script><link href=css/vendor.f747ec02.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.8cb03aaa.js></script><script defer src=js/app.353e1981.js></script><link href=css/vendor.f747ec02.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.9.7/LICENSE` & `unigui-1.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/setup.py` & `unigui-1.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.9.7',      
+      version='1.9.8',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.9.7/PKG-INFO` & `unigui-1.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.7
+Version: 1.9.8
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.9.7/README.md` & `unigui-1.9.8/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.9.7/unigui.egg-info/PKG-INFO` & `unigui-1.9.8/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.7
+Version: 1.9.8
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.9.7/unigui.egg-info/SOURCES.txt` & `unigui-1.9.8/unigui.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/333.46a5102a.css
+unigui/web/css/435.30396533.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.f747ec02.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -30,11 +30,11 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
-unigui/web/js/333.2f4fc18c.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/app.38493c13.js
+unigui/web/js/435.ced6eca8.js
+unigui/web/js/app.353e1981.js
 unigui/web/js/vendor.8cb03aaa.js
```

