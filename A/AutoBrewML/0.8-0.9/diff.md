# Comparing `tmp/AutoBrewML-0.8-py3-none-any.whl.zip` & `tmp/AutoBrewML-0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10612 bytes, number of entries: 7
+Zip file size: 10626 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat    35109 b- defN 22-Aug-02 05:34 AutoBrewML/__init__.py
 -rw-rw-rw-  2.0 fat     6831 b- defN 22-Aug-01 14:48 AutoBrewML/test.py
--rw-rw-rw-  2.0 fat     1070 b- defN 22-Aug-02 05:46 AutoBrewML-0.8.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      672 b- defN 22-Aug-02 05:46 AutoBrewML-0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Aug-02 05:46 AutoBrewML-0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 22-Aug-02 05:46 AutoBrewML-0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      549 b- defN 22-Aug-02 05:46 AutoBrewML-0.8.dist-info/RECORD
-7 files, 44334 bytes uncompressed, 9642 bytes compressed:  78.3%
+-rw-rw-rw-  2.0 fat     1070 b- defN 22-Aug-02 05:54 AutoBrewML-0.9.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      682 b- defN 22-Aug-02 05:54 AutoBrewML-0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-Aug-02 05:54 AutoBrewML-0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 22-Aug-02 05:54 AutoBrewML-0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      549 b- defN 22-Aug-02 05:54 AutoBrewML-0.9.dist-info/RECORD
+7 files, 44344 bytes uncompressed, 9656 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: AutoBrewML/__init__.py
 Comment: 
 
 Filename: AutoBrewML/test.py
 Comment: 
 
-Filename: AutoBrewML-0.8.dist-info/LICENSE.txt
+Filename: AutoBrewML-0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: AutoBrewML-0.8.dist-info/METADATA
+Filename: AutoBrewML-0.9.dist-info/METADATA
 Comment: 
 
-Filename: AutoBrewML-0.8.dist-info/WHEEL
+Filename: AutoBrewML-0.9.dist-info/WHEEL
 Comment: 
 
-Filename: AutoBrewML-0.8.dist-info/top_level.txt
+Filename: AutoBrewML-0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: AutoBrewML-0.8.dist-info/RECORD
+Filename: AutoBrewML-0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `AutoBrewML-0.8.dist-info/LICENSE.txt` & `AutoBrewML-0.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `AutoBrewML-0.8.dist-info/METADATA` & `AutoBrewML-0.9.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: AutoBrewML
-Version: 0.8
+Version: 0.9
 Summary: With AutoBrewML Framework the time it takes to get production-ready ML models with great ease and efficiency highly accelerates.
 Home-page: UNKNOWN
 Author: Sreeja Deb
 Author-email: srde@microsoft.com
 License: UNKNOWN
 Project-URL: AutoBrewML GitHub, https://github.com/microsoft/AutoBrewML
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: sklearn
+Requires-Dist: sklearn (==1.0.2)
 Requires-Dist: pandas-profiling
 Requires-Dist: imblearn
 
 UNKNOWN
```

