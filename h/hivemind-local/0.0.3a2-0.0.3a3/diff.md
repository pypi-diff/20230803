# Comparing `tmp/hivemind-local-0.0.3a2.tar.gz` & `tmp/hivemind_local-0.0.3a3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivemind-local-0.0.3a2.tar", last modified: Thu Aug  3 19:00:03 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

