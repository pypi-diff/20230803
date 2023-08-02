# Comparing `tmp/CellNeighborEX-0.0.3.tar.gz` & `tmp/CellNeighborEX-0.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CellNeighborEX-0.0.3.tar", last modified: Mon Jul 24 10:15:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

