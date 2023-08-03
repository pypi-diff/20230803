# Comparing `tmp/HiveMind-voice-sat-1.0.7.tar.gz` & `tmp/HiveMind_voice_sat-2.0.0a2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/HiveMind-voice-sat-1.0.7.tar", last modified: Fri Dec 18 11:12:28 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

