# Comparing `tmp/poorman_handshake-0.2.0.tar.gz` & `tmp/poorman_handshake-0.2.2a3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/poorman_handshake-0.2.0.tar", last modified: Sun Feb 14 15:37:43 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

