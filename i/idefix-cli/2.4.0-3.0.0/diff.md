# Comparing `tmp/idefix_cli-2.4.0.tar.gz` & `tmp/idefix_cli-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idefix_cli-2.4.0.tar", last modified: Sat Jul 29 16:55:02 2023, max compression
+gzip compressed data, was "idefix_cli-3.0.0.tar", last modified: Wed Aug  2 16:05:56 2023, max compression
```

## Comparing `idefix_cli-2.4.0.tar` & `idefix_cli-3.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:55:02.340545 idefix_cli-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-29 16:55:02.340545 idefix_cli-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 16:55:02.340545 idefix_cli-2.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:55:02.336545 idefix_cli-2.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:55:02.336545 idefix_cli-2.4.0/src/idefix_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:55:02.340545 idefix_cli-2.4.0/src/idefix_cli/_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/read.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_commands/write.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/src/idefix_cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:55:02.340545 idefix_cli-2.4.0/src/idefix_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-29 16:55:02.000000 idefix_cli-2.4.0/src/idefix_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-29 16:55:02.000000 idefix_cli-2.4.0/src/idefix_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:55:02.000000 idefix_cli-2.4.0/src/idefix_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-29 16:55:02.000000 idefix_cli-2.4.0/src/idefix_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-29 16:55:02.000000 idefix_cli-2.4.0/src/idefix_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 16:55:02.000000 idefix_cli-2.4.0/src/idefix_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:55:02.340545 idefix_cli-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_app_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-29 16:54:52.000000 idefix_cli-2.4.0/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:56.092379 idefix_cli-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-02 16:05:56.092379 idefix_cli-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:05:56.092379 idefix_cli-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:56.088379 idefix_cli-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:56.088379 idefix_cli-3.0.0/src/idefix_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:56.092379 idefix_cli-3.0.0/src/idefix_cli/_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_commands/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/src/idefix_cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:56.088379 idefix_cli-3.0.0/src/idefix_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-02 16:05:56.000000 idefix_cli-3.0.0/src/idefix_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-02 16:05:56.000000 idefix_cli-3.0.0/src/idefix_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:05:56.000000 idefix_cli-3.0.0/src/idefix_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-02 16:05:56.000000 idefix_cli-3.0.0/src/idefix_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-02 16:05:56.000000 idefix_cli-3.0.0/src/idefix_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 16:05:56.000000 idefix_cli-3.0.0/src/idefix_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:56.092379 idefix_cli-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_app_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-08-02 16:05:46.000000 idefix_cli-3.0.0/tests/test_write.py
```

### Comparing `idefix_cli-2.4.0/LICENSE` & `idefix_cli-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/PKG-INFO` & `idefix_cli-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix_cli
-Version: 2.4.0
+Version: 3.0.0
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
```

### Comparing `idefix_cli-2.4.0/README.md` & `idefix_cli-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/pyproject.toml` & `idefix_cli-3.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/src/idefix_cli/__main__.py` & `idefix_cli-3.0.0/src/idefix_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/src/idefix_cli/_backports.py` & `idefix_cli-3.0.0/src/idefix_cli/_backports.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/src/idefix_cli/_commands/clean.py` & `idefix_cli-3.0.0/src/idefix_cli/_commands/clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/src/idefix_cli/_commands/clone.py` & `idefix_cli-3.0.0/src/idefix_cli/_commands/clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/src/idefix_cli/_commands/conf.py` & `idefix_cli-3.0.0/src/idefix_cli/_commands/conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/src/idefix_cli/_commands/read.py` & `idefix_cli-3.0.0/src/idefix_cli/_commands/read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/src/idefix_cli/_commands/run.py` & `idefix_cli-3.0.0/src/idefix_cli/_commands/run.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/src/idefix_cli/_commands/stamp.py` & `idefix_cli-3.0.0/src/idefix_cli/_commands/stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/src/idefix_cli/_commands/switch.py` & `idefix_cli-3.0.0/src/idefix_cli/_commands/switch.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/src/idefix_cli/_commands/write.py` & `idefix_cli-3.0.0/src/idefix_cli/_commands/write.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/src/idefix_cli/lib.py` & `idefix_cli-3.0.0/src/idefix_cli/lib.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/src/idefix_cli.egg-info/PKG-INFO` & `idefix_cli-3.0.0/src/idefix_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix-cli
-Version: 2.4.0
+Version: 3.0.0
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
```

### Comparing `idefix_cli-2.4.0/src/idefix_cli.egg-info/SOURCES.txt` & `idefix_cli-3.0.0/src/idefix_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/tests/test_app_structure.py` & `idefix_cli-3.0.0/tests/test_app_structure.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/tests/test_clean.py` & `idefix_cli-3.0.0/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/tests/test_clone.py` & `idefix_cli-3.0.0/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/tests/test_commons.py` & `idefix_cli-3.0.0/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/tests/test_conf.py` & `idefix_cli-3.0.0/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/tests/test_digest.py` & `idefix_cli-3.0.0/tests/test_digest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
 import re
 import sys
 from pathlib import Path
 
+import pytest
+
 from idefix_cli.__main__ import main
 from idefix_cli._commands.digest import command as digest
 
 if sys.version_info >= (3, 11):
     from contextlib import chdir
 else:
     from idefix_cli.lib import chdir
@@ -19,30 +21,51 @@
         ret = main(["digest"])
     out, err = capsys.readouterr()
     assert ret == 0
     json.loads(out)  # validate output
     assert err == ""
 
 
-def test_digest_dir(capsys):
-    ret = main(["digest", "--dir", str(BASE_SETUP.absolute())])
+@pytest.mark.parametrize("supp_args", [(), ("--all",)])
+def test_digest_dir(capsys, supp_args):
+    ret = main(["digest", "--dir", str(BASE_SETUP.absolute()), *supp_args])
     out, err = capsys.readouterr()
     assert ret == 0
     json.loads(out)  # validate output
     assert err == ""
 
 
+@pytest.mark.parametrize("supp_args", [(), ("--all",)])
+def test_output(capsys, tmp_path, supp_args):
+    output_file = tmp_path / "out.json"
+    ret = main(
+        [
+            "digest",
+            "--dir",
+            str(BASE_SETUP.absolute()),
+            "--output",
+            str(output_file),
+            *supp_args,
+        ]
+    )
+    out, err = capsys.readouterr()
+    assert ret == 0
+    assert out == ""
+    assert err == ""
+    json.loads(output_file.read_text())
+
+
 def test_timer(capsys):
     with chdir(BASE_SETUP):
         ret = main(["digest", "--timeit"])
     out, err = capsys.readouterr()
     assert ret == 0
     json.loads(out)  # validate output
 
-    assert re.fullmatch(r"took \d\.\d\d\d ms\n", err)
+    assert re.fullmatch(r"took \d+\.\d\d\d ms\n", err)
 
 
 def test_invalid_dir(tmp_path, capsys):
     path = str((tmp_path / "nope").resolve())
     ret = main(["digest", "--dir", path])
     out, err = capsys.readouterr()
     assert ret != 0
```

### Comparing `idefix_cli-2.4.0/tests/test_read.py` & `idefix_cli-3.0.0/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/tests/test_run.py` & `idefix_cli-3.0.0/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/tests/test_stamp.py` & `idefix_cli-3.0.0/tests/test_stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/tests/test_ux.py` & `idefix_cli-3.0.0/tests/test_ux.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.4.0/tests/test_write.py` & `idefix_cli-3.0.0/tests/test_write.py`

 * *Files identical despite different names*

