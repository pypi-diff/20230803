# Comparing `tmp/piqp-0.2.0.tar.gz` & `tmp/piqp-0.2.1-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piqp-0.2.0.tar", last modified: Fri Jul 28 14:17:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

