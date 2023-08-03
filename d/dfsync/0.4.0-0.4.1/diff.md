# Comparing `tmp/dfsync-0.4.0.tar.gz` & `tmp/dfsync-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfsync-0.4.0.tar", max compression
+gzip compressed data, was "dfsync-0.4.1.tar", max compression
```

## Comparing `dfsync-0.4.0.tar` & `dfsync-0.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0        0 2023-07-31 08:22:13.656849 dfsync-0.4.0/dfsync/__init__.py
--rw-r--r--   0        0        0       64 2021-04-06 10:05:47.000000 dfsync-0.4.0/dfsync/backends/__init__.py
--rw-r--r--   0        0        0    23995 2023-04-03 16:24:42.000000 dfsync-0.4.0/dfsync/backends/kube.py
--rwxr-xr-x   0        0        0     1928 2022-09-10 10:08:34.000000 dfsync-0.4.0/dfsync/backends/kube_exec.py
--rw-r--r--   0        0        0     5473 2023-07-31 21:29:22.099082 dfsync-0.4.0/dfsync/backends/rsync.py
--rw-r--r--   0        0        0     3617 2023-07-31 19:01:18.508583 dfsync-0.4.0/dfsync/char_ui.py
--rw-r--r--   0        0        0     1334 2022-10-21 04:03:26.000000 dfsync-0.4.0/dfsync/chcli.py
--rw-r--r--   0        0        0      582 2023-07-25 16:18:24.031315 dfsync-0.4.0/dfsync/check_dns.py
--rw-r--r--   0        0        0      148 2023-06-17 21:12:04.987300 dfsync-0.4.0/dfsync/cli.py
--rw-r--r--   0        0        0     2381 2023-06-19 07:28:44.923993 dfsync-0.4.0/dfsync/config.py
--rw-r--r--   0        0        0     2389 2023-07-31 22:35:43.410956 dfsync-0.4.0/dfsync/distribution.py
--rw-r--r--   0        0        0     3241 2021-03-30 12:50:07.000000 dfsync-0.4.0/dfsync/exp.py
--rw-r--r--   0        0        0     7025 2023-07-31 22:24:18.258289 dfsync-0.4.0/dfsync/filters.py
--rw-r--r--   0        0        0     1094 2023-05-20 11:19:56.000000 dfsync-0.4.0/dfsync/generate.py
--rw-r--r--   0        0        0     4543 2023-06-17 23:21:49.780512 dfsync-0.4.0/dfsync/kube_credentials.py
--rw-r--r--   0        0        0      679 2023-07-31 20:23:04.492784 dfsync-0.4.0/dfsync/lib.py
--rw-r--r--   0        0        0    10870 2023-07-31 20:25:25.957594 dfsync-0.4.0/dfsync/monitor.py
--rw-r--r--   0        0        0      725 2023-07-08 13:02:10.410286 dfsync-0.4.0/dfsync/pycode/__init__.py
--rw-r--r--   0        0        0     4421 2023-05-20 10:16:55.000000 dfsync-0.4.0/dfsync/pycode/bpe.py
--rw-r--r--   0        0        0     3641 2023-05-18 09:12:53.000000 dfsync-0.4.0/dfsync/pycode/generate_data.py
--rw-r--r--   0        0        0     2121 2023-05-20 11:12:31.000000 dfsync-0.4.0/dfsync/pycode/generate_docstring.py
--rw-r--r--   0        0        0     5869 2023-05-20 13:52:38.000000 dfsync-0.4.0/dfsync/pycode/generate_expansion.py
--rw-r--r--   0        0        0     3088 2023-05-20 11:12:48.000000 dfsync-0.4.0/dfsync/pycode/generate_func.py
--rw-r--r--   0        0        0      540 2023-05-16 17:24:44.000000 dfsync-0.4.0/dfsync/pycode/generate_pytest.py
--rw-r--r--   0        0        0     1822 2023-07-08 13:05:08.349161 dfsync-0.4.0/dfsync/pycode/oai.py
--rw-r--r--   0        0        0     2674 2023-06-02 11:17:40.000000 dfsync-0.4.0/dfsync/pycode/prompts.py
--rw-r--r--   0        0        0      212 2023-07-08 13:05:57.874746 dfsync-0.4.0/dfsync/pycode/search.py
--rw-r--r--   0        0        0     1830 2023-05-18 09:18:10.000000 dfsync-0.4.0/dfsync/pycode/test_generate_data.py
--rw-r--r--   0        0        0     4879 2023-05-20 08:26:16.000000 dfsync-0.4.0/dfsync/pycode/tokens.py
--rw-r--r--   0        0        0     3193 2023-05-20 11:11:17.000000 dfsync-0.4.0/dfsync/pycode/util.py
--rw-r--r--   0        0        0     4269 2023-07-26 02:24:53.086605 dfsync-0.4.0/dfsync/scrape_anm.py
--rw-r--r--   0        0        0      982 2023-07-26 01:41:23.893303 dfsync-0.4.0/dfsync/scrape_reord.py
--rw-r--r--   0        0        0     3350 2021-04-28 13:06:18.000000 dfsync-0.4.0/dfsync/transactions.py
--rw-r--r--   0        0        0      630 2023-07-31 22:31:34.135533 dfsync-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 dfsync-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 08:22:13.656849 dfsync-0.4.1/dfsync/__init__.py
+-rw-r--r--   0        0        0       64 2021-04-06 10:05:47.000000 dfsync-0.4.1/dfsync/backends/__init__.py
+-rw-r--r--   0        0        0    23995 2023-04-03 16:24:42.000000 dfsync-0.4.1/dfsync/backends/kube.py
+-rwxr-xr-x   0        0        0     1928 2022-09-10 10:08:34.000000 dfsync-0.4.1/dfsync/backends/kube_exec.py
+-rw-r--r--   0        0        0     5473 2023-07-31 21:29:22.099082 dfsync-0.4.1/dfsync/backends/rsync.py
+-rw-r--r--   0        0        0     3617 2023-07-31 19:01:18.508583 dfsync-0.4.1/dfsync/char_ui.py
+-rw-r--r--   0        0        0     1334 2022-10-21 04:03:26.000000 dfsync-0.4.1/dfsync/chcli.py
+-rw-r--r--   0        0        0      582 2023-07-25 16:18:24.031315 dfsync-0.4.1/dfsync/check_dns.py
+-rw-r--r--   0        0        0      148 2023-06-17 21:12:04.987300 dfsync-0.4.1/dfsync/cli.py
+-rw-r--r--   0        0        0     2381 2023-06-19 07:28:44.923993 dfsync-0.4.1/dfsync/config.py
+-rw-r--r--   0        0        0     2389 2023-07-31 22:35:43.410956 dfsync-0.4.1/dfsync/distribution.py
+-rw-r--r--   0        0        0     3241 2021-03-30 12:50:07.000000 dfsync-0.4.1/dfsync/exp.py
+-rw-r--r--   0        0        0     7155 2023-08-03 09:59:21.618826 dfsync-0.4.1/dfsync/filters.py
+-rw-r--r--   0        0        0     1094 2023-05-20 11:19:56.000000 dfsync-0.4.1/dfsync/generate.py
+-rw-r--r--   0        0        0     4543 2023-06-17 23:21:49.780512 dfsync-0.4.1/dfsync/kube_credentials.py
+-rw-r--r--   0        0        0      679 2023-07-31 20:23:04.492784 dfsync-0.4.1/dfsync/lib.py
+-rw-r--r--   0        0        0    10870 2023-07-31 20:25:25.957594 dfsync-0.4.1/dfsync/monitor.py
+-rw-r--r--   0        0        0      725 2023-07-08 13:02:10.410286 dfsync-0.4.1/dfsync/pycode/__init__.py
+-rw-r--r--   0        0        0     4421 2023-05-20 10:16:55.000000 dfsync-0.4.1/dfsync/pycode/bpe.py
+-rw-r--r--   0        0        0     3641 2023-05-18 09:12:53.000000 dfsync-0.4.1/dfsync/pycode/generate_data.py
+-rw-r--r--   0        0        0     2121 2023-05-20 11:12:31.000000 dfsync-0.4.1/dfsync/pycode/generate_docstring.py
+-rw-r--r--   0        0        0     5869 2023-05-20 13:52:38.000000 dfsync-0.4.1/dfsync/pycode/generate_expansion.py
+-rw-r--r--   0        0        0     3088 2023-05-20 11:12:48.000000 dfsync-0.4.1/dfsync/pycode/generate_func.py
+-rw-r--r--   0        0        0      540 2023-05-16 17:24:44.000000 dfsync-0.4.1/dfsync/pycode/generate_pytest.py
+-rw-r--r--   0        0        0     1822 2023-07-08 13:05:08.349161 dfsync-0.4.1/dfsync/pycode/oai.py
+-rw-r--r--   0        0        0     2674 2023-06-02 11:17:40.000000 dfsync-0.4.1/dfsync/pycode/prompts.py
+-rw-r--r--   0        0        0      212 2023-07-08 13:05:57.874746 dfsync-0.4.1/dfsync/pycode/search.py
+-rw-r--r--   0        0        0     1830 2023-05-18 09:18:10.000000 dfsync-0.4.1/dfsync/pycode/test_generate_data.py
+-rw-r--r--   0        0        0     4879 2023-05-20 08:26:16.000000 dfsync-0.4.1/dfsync/pycode/tokens.py
+-rw-r--r--   0        0        0     3193 2023-05-20 11:11:17.000000 dfsync-0.4.1/dfsync/pycode/util.py
+-rw-r--r--   0        0        0     4269 2023-07-26 02:24:53.086605 dfsync-0.4.1/dfsync/scrape_anm.py
+-rw-r--r--   0        0        0      982 2023-07-26 01:41:23.893303 dfsync-0.4.1/dfsync/scrape_reord.py
+-rw-r--r--   0        0        0     3350 2021-04-28 13:06:18.000000 dfsync-0.4.1/dfsync/transactions.py
+-rw-r--r--   0        0        0      630 2023-08-03 15:01:26.464929 dfsync-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 dfsync-0.4.1/PKG-INFO
```

### Comparing `dfsync-0.4.0/dfsync/backends/kube.py` & `dfsync-0.4.1/dfsync/backends/kube.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/backends/kube_exec.py` & `dfsync-0.4.1/dfsync/backends/kube_exec.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/backends/rsync.py` & `dfsync-0.4.1/dfsync/backends/rsync.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/char_ui.py` & `dfsync-0.4.1/dfsync/char_ui.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/chcli.py` & `dfsync-0.4.1/dfsync/chcli.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/check_dns.py` & `dfsync-0.4.1/dfsync/check_dns.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/config.py` & `dfsync-0.4.1/dfsync/config.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/distribution.py` & `dfsync-0.4.1/dfsync/distribution.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/exp.py` & `dfsync-0.4.1/dfsync/exp.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/filters.py` & `dfsync-0.4.1/dfsync/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,20 @@
     def _black_check(self, src_file_path):
         try:
             with open(src_file_path, "r") as f:
                 contents = f.read()
                 black.format_file_contents(contents, fast=False, mode=black.FileMode())
             return False
 
+        except black.report.NothingChanged as e:
+            return False
+
         except Exception as e:
-            echo(f"Rejected {src_file_path}, {e}")
+            message = str(e) or type(e).__name__
+            echo(f"Rejected {src_file_path}, {message}")
             return True
 
 
 class UntrackedGitFilesFilter(LoggingFilter):
     def __init__(self):
         super().__init__()
         self._repos = {}
```

### Comparing `dfsync-0.4.0/dfsync/generate.py` & `dfsync-0.4.1/dfsync/generate.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/kube_credentials.py` & `dfsync-0.4.1/dfsync/kube_credentials.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/lib.py` & `dfsync-0.4.1/dfsync/lib.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/monitor.py` & `dfsync-0.4.1/dfsync/monitor.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/pycode/__init__.py` & `dfsync-0.4.1/dfsync/pycode/__init__.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/pycode/bpe.py` & `dfsync-0.4.1/dfsync/pycode/bpe.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/pycode/generate_data.py` & `dfsync-0.4.1/dfsync/pycode/generate_data.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/pycode/generate_docstring.py` & `dfsync-0.4.1/dfsync/pycode/generate_docstring.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/pycode/generate_expansion.py` & `dfsync-0.4.1/dfsync/pycode/generate_expansion.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/pycode/generate_func.py` & `dfsync-0.4.1/dfsync/pycode/generate_func.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/pycode/generate_pytest.py` & `dfsync-0.4.1/dfsync/pycode/generate_pytest.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/pycode/oai.py` & `dfsync-0.4.1/dfsync/pycode/oai.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/pycode/prompts.py` & `dfsync-0.4.1/dfsync/pycode/prompts.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/pycode/test_generate_data.py` & `dfsync-0.4.1/dfsync/pycode/test_generate_data.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/pycode/tokens.py` & `dfsync-0.4.1/dfsync/pycode/tokens.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/pycode/util.py` & `dfsync-0.4.1/dfsync/pycode/util.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/scrape_anm.py` & `dfsync-0.4.1/dfsync/scrape_anm.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/scrape_reord.py` & `dfsync-0.4.1/dfsync/scrape_reord.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/dfsync/transactions.py` & `dfsync-0.4.1/dfsync/transactions.py`

 * *Files identical despite different names*

### Comparing `dfsync-0.4.0/pyproject.toml` & `dfsync-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dfsync"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["Mihai Balint <balint.mihai@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 watchdog = "^2.0.2"
 gitpython = "^3.1.14"
```

### Comparing `dfsync-0.4.0/PKG-INFO` & `dfsync-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfsync
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: Mihai Balint
 Author-email: balint.mihai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

