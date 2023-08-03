# Comparing `tmp/hivemind_bus_client-0.0.3a2.tar.gz` & `tmp/hivemind_bus_client-0.0.4a4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivemind_bus_client-0.0.3a2.tar", last modified: Mon Nov 29 03:14:17 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

