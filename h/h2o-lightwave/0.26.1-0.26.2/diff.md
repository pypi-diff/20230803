# Comparing `tmp/h2o_lightwave-0.26.1-py3-none-any.whl.zip` & `tmp/h2o_lightwave-0.26.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 121155 bytes, number of entries: 15
--rw-r--r--  2.0 unx     1132 b- defN 23-Jul-03 09:53 h2o_lightwave/__init__.py
--rw-r--r--  2.0 unx    14374 b- defN 23-Jul-03 09:53 h2o_lightwave/core.py
--rw-r--r--  2.0 unx    25866 b- defN 23-Jul-03 09:53 h2o_lightwave/graphics.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 09:53 h2o_lightwave/py.typed
--rw-r--r--  2.0 unx     7889 b- defN 23-Jul-03 09:53 h2o_lightwave/routing.py
--rw-r--r--  2.0 unx     3850 b- defN 23-Jul-03 09:53 h2o_lightwave/server.py
--rw-r--r--  2.0 unx   635848 b- defN 23-Jul-03 09:53 h2o_lightwave/types.py
--rw-r--r--  2.0 unx   166206 b- defN 23-Jul-03 09:53 h2o_lightwave/ui.py
--rw-r--r--  2.0 unx     2325 b- defN 23-Jul-03 09:53 h2o_lightwave/ui_ext.py
--rw-r--r--  2.0 unx       23 b- defN 23-Jul-03 09:53 h2o_lightwave/version.py
--rw-r--r--  2.0 unx       53 b- defN 23-Jul-03 10:12 h2o_lightwave-0.26.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6185 b- defN 23-Jul-03 10:12 h2o_lightwave-0.26.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 10:12 h2o_lightwave-0.26.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jul-03 10:12 h2o_lightwave-0.26.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1218 b- defN 23-Jul-03 10:12 h2o_lightwave-0.26.1.dist-info/RECORD
-15 files, 865075 bytes uncompressed, 119149 bytes compressed:  86.2%
+Zip file size: 121154 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     1132 b- defN 23-Aug-03 12:38 h2o_lightwave/__init__.py
+-rw-r--r--  2.0 unx    14374 b- defN 23-Aug-03 12:38 h2o_lightwave/core.py
+-rw-r--r--  2.0 unx    25866 b- defN 23-Aug-03 12:38 h2o_lightwave/graphics.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-03 12:38 h2o_lightwave/py.typed
+-rw-r--r--  2.0 unx     7889 b- defN 23-Aug-03 12:38 h2o_lightwave/routing.py
+-rw-r--r--  2.0 unx     3850 b- defN 23-Aug-03 12:38 h2o_lightwave/server.py
+-rw-r--r--  2.0 unx   635848 b- defN 23-Aug-03 12:38 h2o_lightwave/types.py
+-rw-r--r--  2.0 unx   166206 b- defN 23-Aug-03 12:38 h2o_lightwave/ui.py
+-rw-r--r--  2.0 unx     2325 b- defN 23-Aug-03 12:38 h2o_lightwave/ui_ext.py
+-rw-r--r--  2.0 unx       23 b- defN 23-Aug-03 12:38 h2o_lightwave/version.py
+-rw-r--r--  2.0 unx       53 b- defN 23-Aug-03 12:45 h2o_lightwave-0.26.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6185 b- defN 23-Aug-03 12:45 h2o_lightwave-0.26.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 12:45 h2o_lightwave-0.26.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Aug-03 12:45 h2o_lightwave-0.26.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1218 b- defN 23-Aug-03 12:45 h2o_lightwave-0.26.2.dist-info/RECORD
+15 files, 865075 bytes uncompressed, 119148 bytes compressed:  86.2%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: h2o_lightwave/ui_ext.py
 Comment: 
 
 Filename: h2o_lightwave/version.py
 Comment: 
 
-Filename: h2o_lightwave-0.26.1.dist-info/LICENSE
+Filename: h2o_lightwave-0.26.2.dist-info/LICENSE
 Comment: 
 
-Filename: h2o_lightwave-0.26.1.dist-info/METADATA
+Filename: h2o_lightwave-0.26.2.dist-info/METADATA
 Comment: 
 
-Filename: h2o_lightwave-0.26.1.dist-info/WHEEL
+Filename: h2o_lightwave-0.26.2.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_lightwave-0.26.1.dist-info/top_level.txt
+Filename: h2o_lightwave-0.26.2.dist-info/top_level.txt
 Comment: 
 
-Filename: h2o_lightwave-0.26.1.dist-info/RECORD
+Filename: h2o_lightwave-0.26.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_lightwave/version.py

```diff
@@ -1 +1 @@
-__version__ = '0.26.1'
+__version__ = '0.26.2'
```

## Comparing `h2o_lightwave-0.26.1.dist-info/METADATA` & `h2o_lightwave-0.26.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h2o-lightwave
-Version: 0.26.1
+Version: 0.26.2
 Summary: H2O Wave Python driver for integration with arbitrary python web frameworks.
 Home-page: https://h2o.ai/products/h2o-wave
 Author: Martin Turoci
 Author-email: martin.turoci@h2o.ai
 License: UNKNOWN
 Project-URL: Documentation, https://wave.h2o.ai/
 Project-URL: Source, https://github.com/h2oai/wave
@@ -22,15 +22,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 Provides-Extra: web
-Requires-Dist: h2o-lightwave-web (==0.26.1) ; extra == 'web'
+Requires-Dist: h2o-lightwave-web (==0.26.2) ; extra == 'web'
 
 # H2O Lightwave
 
 H2O Lightwave is a lightweight, pure-Python version of [H2O Wave](https://wave.h2o.ai/) that can be embedded in popular async web frameworks like FastAPI, Starlette, etc.
 
 In other words, H2O Lightwave works without the Wave server.
```

## Comparing `h2o_lightwave-0.26.1.dist-info/RECORD` & `h2o_lightwave-0.26.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 h2o_lightwave/graphics.py,sha256=HLYrX-lwsMKbyLmy2ClG5L46DA2_hSCEPTsv0gPVoyg,25866
 h2o_lightwave/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 h2o_lightwave/routing.py,sha256=5aNgnVjhYU3Yih--rC2THfsNZpVWBHmzY9ju64KtyB4,7889
 h2o_lightwave/server.py,sha256=g0qj5W0NLesG9ghZlgwTOI74OgHY8XErw1BQWuljumI,3850
 h2o_lightwave/types.py,sha256=DO-z92m6oAxPUhN1144vdZ4Ug8jII8YAGlHYu239P4E,635848
 h2o_lightwave/ui.py,sha256=u41t97teUgPOB3IJ8TxIkd4qp8AW_Y9Dskcaq78iRww,166206
 h2o_lightwave/ui_ext.py,sha256=zx_2Ec2-p_ztm8brfVaVF0fTQWVDrb_YxcGfVb-wA10,2325
-h2o_lightwave/version.py,sha256=ETW1KUvXcKPocfR8oqFVOl2UoxVGnBdqQHPWngZJk_g,23
-h2o_lightwave-0.26.1.dist-info/LICENSE,sha256=hpuFayniDwysSKD0tHGELH2KJDVyhUrKS29torRIpqY,53
-h2o_lightwave-0.26.1.dist-info/METADATA,sha256=-BqQJAD2d3DbFU_Y1tVQTAVsVi80ly2FViprBDzGYWg,6185
-h2o_lightwave-0.26.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-h2o_lightwave-0.26.1.dist-info/top_level.txt,sha256=1ZH7jcWsnca5BnX2d9scu4t0ohD50aeA2ceYXY8M2c8,14
-h2o_lightwave-0.26.1.dist-info/RECORD,,
+h2o_lightwave/version.py,sha256=IJFEoLY0s48Q1zpqv88QrvXA_m6iYTmujuwk8Gd0uus,23
+h2o_lightwave-0.26.2.dist-info/LICENSE,sha256=hpuFayniDwysSKD0tHGELH2KJDVyhUrKS29torRIpqY,53
+h2o_lightwave-0.26.2.dist-info/METADATA,sha256=AVOm3ubkRWZLS-wIVUAO1wL2eC6bDcdqdKAzunxNtJU,6185
+h2o_lightwave-0.26.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+h2o_lightwave-0.26.2.dist-info/top_level.txt,sha256=1ZH7jcWsnca5BnX2d9scu4t0ohD50aeA2ceYXY8M2c8,14
+h2o_lightwave-0.26.2.dist-info/RECORD,,
```

