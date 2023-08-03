# Comparing `tmp/sheCry-0.0.8.tar.gz` & `tmp/sheCry-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheCry-0.0.8.tar", last modified: Tue Aug  1 08:43:02 2023, max compression
+gzip compressed data, was "sheCry-0.0.9.tar", last modified: Tue Aug  1 08:59:19 2023, max compression
```

## Comparing `sheCry-0.0.8.tar` & `sheCry-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:43:02.083583 sheCry-0.0.8/
--rw-rw-rw-   0        0        0    35821 2023-07-31 18:14:15.000000 sheCry-0.0.8/LICENSE.md
--rw-rw-rw-   0        0        0    10131 2023-08-01 08:43:02.077584 sheCry-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     9484 2023-08-01 08:42:37.000000 sheCry-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 08:43:02.083583 sheCry-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      909 2023-08-01 08:42:56.000000 sheCry-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:43:02.075585 sheCry-0.0.8/sheCry.egg-info/
--rw-rw-rw-   0        0        0    10131 2023-08-01 08:43:01.000000 sheCry-0.0.8/sheCry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-08-01 08:43:01.000000 sheCry-0.0.8/sheCry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:43:01.000000 sheCry-0.0.8/sheCry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:43:01.000000 sheCry-0.0.8/sheCry.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 08:59:19.130486 sheCry-0.0.9/
+-rw-rw-rw-   0        0        0    35821 2023-07-31 18:14:15.000000 sheCry-0.0.9/LICENSE.md
+-rw-rw-rw-   0        0        0    10137 2023-08-01 08:59:19.122485 sheCry-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9490 2023-08-01 08:58:17.000000 sheCry-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 08:59:19.131485 sheCry-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-08-01 08:58:38.000000 sheCry-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 08:59:19.120484 sheCry-0.0.9/sheCry.egg-info/
+-rw-rw-rw-   0        0        0    10137 2023-08-01 08:59:18.000000 sheCry-0.0.9/sheCry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-08-01 08:59:18.000000 sheCry-0.0.9/sheCry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:59:18.000000 sheCry-0.0.9/sheCry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 08:59:18.000000 sheCry-0.0.9/sheCry.egg-info/top_level.txt
```

### Comparing `sheCry-0.0.8/LICENSE.md` & `sheCry-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sheCry-0.0.8/PKG-INFO` & `sheCry-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheCry
-Version: 0.0.8
+Version: 0.0.9
 Summary: SHE Cryptography is architectured by Tahsin Ahmed.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,SHE,SHE cryptography,Symmetric Hybrid Encryption,Symmetric Hybrid Encryption cryptography,sheCry
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
@@ -62,14 +62,15 @@
 **Usage / Example**
 ----------------------------
 This is an example how you can write your code so that it runs successfully.
 
     from sheCry import crypto
     
     sharedKey = int(input("Key length for shared key value: "))
+    
     privatedKey = int(input("Key length for private key: "))
         
     message = input("Enter message: ")
     
     she = crypto()
     
     she.key(sharedKey, privatedKey)
```

### Comparing `sheCry-0.0.8/README.md` & `sheCry-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 **Usage / Example**
 ----------------------------
 This is an example how you can write your code so that it runs successfully.
 
     from sheCry import crypto
     
     sharedKey = int(input("Key length for shared key value: "))
+    
     privatedKey = int(input("Key length for private key: "))
         
     message = input("Enter message: ")
     
     she = crypto()
     
     she.key(sharedKey, privatedKey)
```

### Comparing `sheCry-0.0.8/setup.py` & `sheCry-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "sheCry",
 
-    version = "0.0.8",
+    version = "0.0.9",
     
     author = "Tahsin Ahmed",
 
     description = "SHE Cryptography is architectured by Tahsin Ahmed.",
 
     long_description = open("README.md", encoding="utf-8").read(),
```

### Comparing `sheCry-0.0.8/sheCry.egg-info/PKG-INFO` & `sheCry-0.0.9/sheCry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheCry
-Version: 0.0.8
+Version: 0.0.9
 Summary: SHE Cryptography is architectured by Tahsin Ahmed.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,SHE,SHE cryptography,Symmetric Hybrid Encryption,Symmetric Hybrid Encryption cryptography,sheCry
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
@@ -62,14 +62,15 @@
 **Usage / Example**
 ----------------------------
 This is an example how you can write your code so that it runs successfully.
 
     from sheCry import crypto
     
     sharedKey = int(input("Key length for shared key value: "))
+    
     privatedKey = int(input("Key length for private key: "))
         
     message = input("Enter message: ")
     
     she = crypto()
     
     she.key(sharedKey, privatedKey)
```

