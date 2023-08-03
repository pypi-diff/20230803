# Comparing `tmp/HiveMind_presence-0.0.2a2.tar.gz` & `tmp/HiveMind_presence-0.0.2a4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HiveMind_presence-0.0.2a2.tar", last modified: Wed Dec  8 16:34:50 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

