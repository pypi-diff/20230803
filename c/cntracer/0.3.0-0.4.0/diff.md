# Comparing `tmp/cntracer-0.3.0-cp39-cp39-win_amd64.whl.zip` & `tmp/cntracer-0.4.0-cp39-cp39-musllinux_1_1_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,12 @@
-Zip file size: 79738 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   176640 b- defN 23-Aug-03 08:10 cntracer.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2182 b- defN 23-Aug-03 08:10 cntracer-0.3.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      233 b- defN 23-Aug-03 08:10 cntracer-0.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-03 08:10 cntracer-0.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Aug-03 08:10 cntracer-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      476 b- defN 23-Aug-03 08:10 cntracer-0.3.0.dist-info/RECORD
-6 files, 179640 bytes uncompressed, 78878 bytes compressed:  56.1%
+Zip file size: 619861 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 08:58 cntracer-0.4.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 08:58 cntracer.libs/
+-rwxr-xr-x  2.0 unx   337161 b- defN 23-Aug-03 08:58 cntracer.cpython-39-aarch64-linux-gnu.so
+-rw-r--r--  2.0 unx      222 b- defN 23-Aug-03 08:58 cntracer-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      112 b- defN 23-Aug-03 08:58 cntracer-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx     2182 b- defN 23-Aug-03 08:58 cntracer-0.4.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      694 b- defN 23-Aug-03 08:58 cntracer-0.4.0.dist-info/RECORD
+-rw-r--r--  2.0 unx        9 b- defN 23-Aug-03 08:58 cntracer-0.4.0.dist-info/top_level.txt
+-rwxr-xr-x  2.0 unx  2599041 b- defN 23-Aug-03 08:58 cntracer.libs/libstdc++-fd9f4683.so.6.0.28
+-rw-r--r--  2.0 unx   134393 b- defN 23-Aug-03 08:58 cntracer.libs/libgcc_s-4e37474d.so.1
+10 files, 3073814 bytes uncompressed, 618437 bytes compressed:  79.9%
```

## zipnote {}

```diff
@@ -1,19 +1,31 @@
-Filename: cntracer.cp39-win_amd64.pyd
+Filename: cntracer-0.4.0.dist-info/
 Comment: 
 
-Filename: cntracer-0.3.0.dist-info/LICENSE
+Filename: cntracer.libs/
 Comment: 
 
-Filename: cntracer-0.3.0.dist-info/METADATA
+Filename: cntracer.cpython-39-aarch64-linux-gnu.so
 Comment: 
 
-Filename: cntracer-0.3.0.dist-info/WHEEL
+Filename: cntracer-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: cntracer-0.3.0.dist-info/top_level.txt
+Filename: cntracer-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: cntracer-0.3.0.dist-info/RECORD
+Filename: cntracer-0.4.0.dist-info/LICENSE
+Comment: 
+
+Filename: cntracer-0.4.0.dist-info/RECORD
+Comment: 
+
+Filename: cntracer-0.4.0.dist-info/top_level.txt
+Comment: 
+
+Filename: cntracer.libs/libstdc++-fd9f4683.so.6.0.28
+Comment: 
+
+Filename: cntracer.libs/libgcc_s-4e37474d.so.1
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `cntracer-0.3.0.dist-info/LICENSE` & `cntracer-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

