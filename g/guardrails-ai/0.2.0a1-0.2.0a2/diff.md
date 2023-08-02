# Comparing `tmp/guardrails-ai-0.2.0a1.tar.gz` & `tmp/guardrails_ai-0.2.0a2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guardrails-ai-0.2.0a1.tar", last modified: Thu Jul 20 19:29:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

