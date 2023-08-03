# Comparing `tmp/multicallable-5.1.1.tar.gz` & `tmp/multicallable-5.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/hassan/Documents/codes/deusfinance/multicallable/dist/tmp32ay2ygs/multicallable-5.1.1.tar", last modified: Mon May 29 08:30:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

