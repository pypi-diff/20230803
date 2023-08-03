# Comparing `tmp/cobra_io-0.0.2-py3-none-any.whl.zip` & `tmp/cobra_io-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 17916 bytes, number of entries: 22
--rw-rw-r--  2.0 unx      149 b- defN 23-Jul-25 11:25 cobra/__init__.py
+Zip file size: 17904 bytes, number of entries: 22
+-rw-rw-r--  2.0 unx      149 b- defN 23-Aug-03 13:30 cobra/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-06 08:39 cobra/asset/__init__.py
 -rw-rw-r--  2.0 unx     1111 b- defN 23-Jul-13 12:05 cobra/asset/asset.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-06 08:39 cobra/robot/__init__.py
 -rw-rw-r--  2.0 unx     5226 b- defN 23-Jul-25 11:25 cobra/robot/robot.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-06 08:39 cobra/solution/__init__.py
 -rw-rw-r--  2.0 unx     9062 b- defN 23-Jul-25 11:25 cobra/solution/solution.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-06 08:39 cobra/task/__init__.py
 -rw-rw-r--  2.0 unx     6772 b- defN 23-Jul-25 11:25 cobra/task/task.py
 -rw-rw-r--  2.0 unx     1222 b- defN 23-Jul-13 12:05 cobra/user/user.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-06 08:39 cobra/utils/__init__.py
 -rw-rw-r--  2.0 unx      975 b- defN 23-Jul-13 12:05 cobra/utils/caches.py
--rw-rw-r--  2.0 unx     1069 b- defN 23-Jul-13 12:05 cobra/utils/cobra.config.sample
+-rw-rw-r--  2.0 unx     1026 b- defN 23-Aug-03 13:30 cobra/utils/cobra.config.sample
 -rw-rw-r--  2.0 unx     1252 b- defN 23-Jul-13 12:05 cobra/utils/configurations.py
 -rw-rw-r--  2.0 unx     3340 b- defN 23-Jul-13 12:05 cobra/utils/logging.py
 -rw-rw-r--  2.0 unx      335 b- defN 23-Jul-25 07:23 cobra/utils/urls.py
 -rw-rw-r--  2.0 unx     3800 b- defN 23-Jul-25 11:25 cobra/utils/utils.py
--rw-rw-r--  2.0 unx     1064 b- defN 23-Jul-25 11:26 cobra_io-0.0.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4441 b- defN 23-Jul-25 11:26 cobra_io-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 11:26 cobra_io-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-Jul-25 11:26 cobra_io-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1719 b- defN 23-Jul-25 11:26 cobra_io-0.0.2.dist-info/RECORD
-22 files, 41635 bytes uncompressed, 15138 bytes compressed:  63.6%
+-rw-rw-r--  2.0 unx     1064 b- defN 23-Aug-03 13:31 cobra_io-0.0.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4565 b- defN 23-Aug-03 13:31 cobra_io-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-03 13:31 cobra_io-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-Aug-03 13:31 cobra_io-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1719 b- defN 23-Aug-03 13:31 cobra_io-0.0.3.dist-info/RECORD
+22 files, 41716 bytes uncompressed, 15126 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: cobra/utils/urls.py
 Comment: 
 
 Filename: cobra/utils/utils.py
 Comment: 
 
-Filename: cobra_io-0.0.2.dist-info/LICENSE
+Filename: cobra_io-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: cobra_io-0.0.2.dist-info/METADATA
+Filename: cobra_io-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: cobra_io-0.0.2.dist-info/WHEEL
+Filename: cobra_io-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: cobra_io-0.0.2.dist-info/top_level.txt
+Filename: cobra_io-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: cobra_io-0.0.2.dist-info/RECORD
+Filename: cobra_io-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cobra/__init__.py

```diff
@@ -1,6 +1,6 @@
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 from .asset import asset
 from .robot import robot
 from .task import task
 from .solution import solution
 from .user import user
```

## cobra/utils/cobra.config.sample

```diff
@@ -14,10 +14,9 @@
 
 # This is where you can specify the location of the files CoBRA I/O caches for you.
 [FILE_LOCATIONS]
 cache = /tmp/cobra_cache
 
 # Configure which CoBRA API to use, e.g., for local development
 [API]
-# TODO Repalce by production URL once ready
-base_url = https://vmknoll79.in.tum.de/api/
+base_url = https://cobra.cps.cit.tum.de/api/
 version = 2022
```

## Comparing `cobra_io-0.0.2.dist-info/LICENSE` & `cobra_io-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cobra_io-0.0.2.dist-info/METADATA` & `cobra_io-0.0.3.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobra-io
-Version: 0.0.2
+Version: 0.0.3
 Summary: Composable Benchmark for Robotics Applications - Input/Output
 Author-email: Matthias Mayer <matthias.mayer@tum.de>
 License: MIT
 Project-URL: Source Code, https://gitlab.lrz.de/tum-cps/cobra-io
 Project-URL: Documentation, https://cobra-io.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://gitlab.lrz.de/tum-cps/cobra-io/-/issues
 Keywords: Modular Reconfigurable Robots,Robot Design,Model Generation,Simulation,Benchmark,Path Planning
@@ -21,14 +21,17 @@
 Requires-Dist: flake8 (>=5.0) ; extra == 'dev'
 Requires-Dist: coverage (>=6.3) ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
 Requires-Dist: pip-tools ; extra == 'dev'
 Requires-Dist: pytest (>=6.0) ; extra == 'dev'
 Requires-Dist: setuptools (>=61.0.0) ; extra == 'dev'
 Requires-Dist: timor-python ; extra == 'dev'
+Requires-Dist: nb-clean ; extra == 'dev'
+Requires-Dist: nbconvert ; extra == 'dev'
+Requires-Dist: nbformat ; extra == 'dev'
 Provides-Extra: full
 Requires-Dist: cobra-io[dev] ; extra == 'full'
 Requires-Dist: notebook ; extra == 'full'
 
 CoBRA I/O
 =========
```

## Comparing `cobra_io-0.0.2.dist-info/RECORD` & `cobra_io-0.0.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-cobra/__init__.py,sha256=Nt8ftFxzNvSnCTTHHKiL1UwZjO1cL-4wfecO8otBDoM,149
+cobra/__init__.py,sha256=9lJNhtLd2MhM6sKKunP3h7ytz6rzyFMI5uqf9dXwb08,149
 cobra/asset/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cobra/asset/asset.py,sha256=UOlmjLkRkqdUuP4MvDMVMMadYRnEQNpGgsuKnGv6swc,1111
 cobra/robot/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cobra/robot/robot.py,sha256=pVp8VWgFFx5pcqA1tUhH7VCCh7GllH5dWGclKXzGSqs,5226
 cobra/solution/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cobra/solution/solution.py,sha256=nk-Wxn4xI0k_eLRS1K-u8UBXxYMdaFgNnXJK-YuVAeg,9062
 cobra/task/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cobra/task/task.py,sha256=xqcGijDHzx9xUPnHbARzbKIEd3bOGOVeYHelv0SyB2Q,6772
 cobra/user/user.py,sha256=SvGKuMDJ1qJ2d6a8oehVe1wBoZKtF1KDiq3MJc5tZ7c,1222
 cobra/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cobra/utils/caches.py,sha256=v-wVaQGmXY69flLxfYaySDJwaZ8Chy9ljQb0MuzLnLk,975
-cobra/utils/cobra.config.sample,sha256=rEL3Jt8RE0iNDSRDhOEscpS3lSezhQWQ83QCPUKjHmc,1069
+cobra/utils/cobra.config.sample,sha256=7_xNB0SkKiY6HB-LvQ17-oG4K1s09LTL3u5a4j88e5k,1026
 cobra/utils/configurations.py,sha256=zSGFsc_RTitjRs7vC_hP-wxbxvyPWYBayLbWrHJI-08,1252
 cobra/utils/logging.py,sha256=_zABBV3S4einE7UT19WY4vJ7T7fgOWqKoeM5jznC6dk,3340
 cobra/utils/urls.py,sha256=JamfmH3UgXgc2e_7o66eTTP-fWS6rNiu-rcf1clTgxo,335
 cobra/utils/utils.py,sha256=LtnJfTMsivp4rDIj71GctsP9BNoQmuPdHYmJYOo79c8,3800
-cobra_io-0.0.2.dist-info/LICENSE,sha256=HkUglOilukiAaKStefgjNm645flvvv1UwNYFj2E1dE4,1064
-cobra_io-0.0.2.dist-info/METADATA,sha256=pAkbsefHUWedfD1wDe3F9cbZbfrj0Q0D120jtPDyjsg,4441
-cobra_io-0.0.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-cobra_io-0.0.2.dist-info/top_level.txt,sha256=LeT4BKKqEqFNqc-EGNWRSpdtIvqG4eLt-Qn3Rf1EmG8,6
-cobra_io-0.0.2.dist-info/RECORD,,
+cobra_io-0.0.3.dist-info/LICENSE,sha256=HkUglOilukiAaKStefgjNm645flvvv1UwNYFj2E1dE4,1064
+cobra_io-0.0.3.dist-info/METADATA,sha256=Y3wNufdLCHxn4tmyOl-VmYxPnd2Bm45CFELoJVkFvR4,4565
+cobra_io-0.0.3.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+cobra_io-0.0.3.dist-info/top_level.txt,sha256=LeT4BKKqEqFNqc-EGNWRSpdtIvqG4eLt-Qn3Rf1EmG8,6
+cobra_io-0.0.3.dist-info/RECORD,,
```

