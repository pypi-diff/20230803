# Comparing `tmp/WeiboBot-0.3.7.tar.gz` & `tmp/WeiboBot-0.4.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WeiboBot-0.3.7.tar", last modified: Thu Oct 27 15:10:15 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

