# Comparing `tmp/abstract_modules-0.0.1.3-py3-none-any.whl.zip` & `tmp/abstract_modules-0.0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 18467 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       40 b- defN 23-Aug-02 04:34 abstract_modules/__init__.py
 -rw-r--r--  2.0 unx    32997 b- defN 23-Aug-03 04:11 abstract_modules/create_module_folder.py
 -rw-r--r--  2.0 unx     1290 b- defN 23-Aug-02 04:34 abstract_modules/main.py
 -rw-r--r--  2.0 unx     3681 b- defN 23-Aug-02 08:02 abstract_modules/module_utils.py
 -rw-r--r--  2.0 unx    10684 b- defN 23-Aug-03 07:00 abstract_modules/upload_utils.py
--rw-r--r--  2.0 unx     3950 b- defN 23-Aug-03 08:43 abstract_modules-0.0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 08:43 abstract_modules-0.0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Aug-03 08:43 abstract_modules-0.0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      783 b- defN 23-Aug-03 08:43 abstract_modules-0.0.1.3.dist-info/RECORD
+-rw-r--r--  2.0 unx     3950 b- defN 23-Aug-03 08:44 abstract_modules-0.0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 08:44 abstract_modules-0.0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Aug-03 08:44 abstract_modules-0.0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      783 b- defN 23-Aug-03 08:44 abstract_modules-0.0.1.4.dist-info/RECORD
 9 files, 53534 bytes uncompressed, 17105 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: abstract_modules/module_utils.py
 Comment: 
 
 Filename: abstract_modules/upload_utils.py
 Comment: 
 
-Filename: abstract_modules-0.0.1.3.dist-info/METADATA
+Filename: abstract_modules-0.0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: abstract_modules-0.0.1.3.dist-info/WHEEL
+Filename: abstract_modules-0.0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: abstract_modules-0.0.1.3.dist-info/top_level.txt
+Filename: abstract_modules-0.0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: abstract_modules-0.0.1.3.dist-info/RECORD
+Filename: abstract_modules-0.0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `abstract_modules-0.0.1.3.dist-info/METADATA` & `abstract_modules-0.0.1.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-modules
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: abstract_modules allows you to easily upload your Python module to the Python Package Index (PyPI) using Twine. It automates several steps of the packaging and distribution process, making it easier to share your module with the Python community..
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_modules
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `abstract_modules-0.0.1.3.dist-info/RECORD` & `abstract_modules-0.0.1.4.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 abstract_modules/__init__.py,sha256=0LNjFqr-o-wHdm5LGqcJ2NyZGfe0l7_GunRKIl1PSvs,40
 abstract_modules/create_module_folder.py,sha256=Z1w1XX2beIfO2Hei4-0QKY6ROOw1kkWeOsYkZ2nQG3Y,32997
 abstract_modules/main.py,sha256=zrkeuBjXVoW_DfUx2uVV-mEWDUsnGgpwWPdkSYqhoT0,1290
 abstract_modules/module_utils.py,sha256=nJW5qU1RuVg8Irm7p-KFvFzALjSLwfXQ2pGA62rteJw,3681
 abstract_modules/upload_utils.py,sha256=b7aDrnDZXjxB7NyOAWKSvl64Ma0wMmOzIG8hH5qHiRc,10684
-abstract_modules-0.0.1.3.dist-info/METADATA,sha256=PM3Jc1cYt2T45RyudKsqxKQqm1ampxl6M5fEVlBx-GY,3950
-abstract_modules-0.0.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-abstract_modules-0.0.1.3.dist-info/top_level.txt,sha256=f9o4Vw5Mulr8ed3JeHE83u5oi5GQ3By2vY_v5nbAEMM,17
-abstract_modules-0.0.1.3.dist-info/RECORD,,
+abstract_modules-0.0.1.4.dist-info/METADATA,sha256=nLI_-lLRgfptzadKDojrKaEclTOa_5eS9kDpQXPy2M0,3950
+abstract_modules-0.0.1.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+abstract_modules-0.0.1.4.dist-info/top_level.txt,sha256=f9o4Vw5Mulr8ed3JeHE83u5oi5GQ3By2vY_v5nbAEMM,17
+abstract_modules-0.0.1.4.dist-info/RECORD,,
```

