# Comparing `tmp/usersgenerator-2.2.0.tar.gz` & `tmp/usersgenerator-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usersgenerator-2.2.0.tar", last modified: Tue Jan  4 12:49:59 2022, max compression
+gzip compressed data, was "usersgenerator-2.2.1.tar", last modified: Thu Aug  3 00:21:38 2023, max compression
```

## Comparing `usersgenerator-2.2.0.tar` & `usersgenerator-2.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 abeljm    (1000) abeljm    (1000)        0 2022-01-04 12:49:59.000000 usersgenerator-2.2.0/
--rwxrwxrwx   0 abeljm    (1000) abeljm    (1000)      985 2022-01-04 12:49:59.000000 usersgenerator-2.2.0/PKG-INFO
--rwxrwxrwx   0 abeljm    (1000) abeljm    (1000)      348 2022-01-03 21:15:05.000000 usersgenerator-2.2.0/README.md
--rwxrwxrwx   0 abeljm    (1000) abeljm    (1000)       38 2022-01-04 12:49:59.000000 usersgenerator-2.2.0/setup.cfg
--rwxrwxrwx   0 abeljm    (1000) abeljm    (1000)      997 2022-01-04 12:48:58.000000 usersgenerator-2.2.0/setup.py
-drwxrwxrwx   0 abeljm    (1000) abeljm    (1000)        0 2022-01-04 12:49:59.000000 usersgenerator-2.2.0/usersgenerator/
--rwxrwxrwx   0 abeljm    (1000) abeljm    (1000)       61 2022-01-04 12:48:52.000000 usersgenerator-2.2.0/usersgenerator/__init__.py
--rwxrwxrwx   0 abeljm    (1000) abeljm    (1000)     3318 2022-01-04 12:48:40.000000 usersgenerator-2.2.0/usersgenerator/usersgenerator.py
-drwxrwxrwx   0 abeljm    (1000) abeljm    (1000)        0 2022-01-04 12:49:59.000000 usersgenerator-2.2.0/usersgenerator.egg-info/
--rwxrwxrwx   0 abeljm    (1000) abeljm    (1000)      985 2022-01-04 12:49:59.000000 usersgenerator-2.2.0/usersgenerator.egg-info/PKG-INFO
--rwxrwxrwx   0 abeljm    (1000) abeljm    (1000)      308 2022-01-04 12:49:59.000000 usersgenerator-2.2.0/usersgenerator.egg-info/SOURCES.txt
--rwxrwxrwx   0 abeljm    (1000) abeljm    (1000)        1 2022-01-04 12:49:59.000000 usersgenerator-2.2.0/usersgenerator.egg-info/dependency_links.txt
--rwxrwxrwx   0 abeljm    (1000) abeljm    (1000)       71 2022-01-04 12:49:59.000000 usersgenerator-2.2.0/usersgenerator.egg-info/entry_points.txt
--rwxrwxrwx   0 abeljm    (1000) abeljm    (1000)        9 2022-01-04 12:49:59.000000 usersgenerator-2.2.0/usersgenerator.egg-info/requires.txt
--rwxrwxrwx   0 abeljm    (1000) abeljm    (1000)       15 2022-01-04 12:49:59.000000 usersgenerator-2.2.0/usersgenerator.egg-info/top_level.txt
+drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-08-03 00:21:38.180357 usersgenerator-2.2.1/
+-rwxrwxrwx   0 abel      (1000) abel      (1000)      985 2023-08-03 00:21:38.179927 usersgenerator-2.2.1/PKG-INFO
+-rwxrwxrwx   0 abel      (1000) abel      (1000)      348 2023-08-02 02:10:51.000000 usersgenerator-2.2.1/README.md
+-rwxrwxrwx   0 abel      (1000) abel      (1000)       38 2023-08-03 00:21:38.180419 usersgenerator-2.2.1/setup.cfg
+-rwxrwxrwx   0 abel      (1000) abel      (1000)      997 2023-08-03 00:20:46.000000 usersgenerator-2.2.1/setup.py
+drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-08-03 00:21:38.177475 usersgenerator-2.2.1/usersgenerator/
+-rwxrwxrwx   0 abel      (1000) abel      (1000)       61 2023-08-03 00:20:40.000000 usersgenerator-2.2.1/usersgenerator/__init__.py
+-rwxrwxrwx   0 abel      (1000) abel      (1000)     5314 2023-08-03 00:14:19.000000 usersgenerator-2.2.1/usersgenerator/usersgenerator.py
+drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-08-03 00:21:38.179500 usersgenerator-2.2.1/usersgenerator.egg-info/
+-rwxrwxrwx   0 abel      (1000) abel      (1000)      985 2023-08-03 00:21:37.000000 usersgenerator-2.2.1/usersgenerator.egg-info/PKG-INFO
+-rwxrwxrwx   0 abel      (1000) abel      (1000)      308 2023-08-03 00:21:37.000000 usersgenerator-2.2.1/usersgenerator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 abel      (1000) abel      (1000)        1 2023-08-03 00:21:37.000000 usersgenerator-2.2.1/usersgenerator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 abel      (1000) abel      (1000)       71 2023-08-03 00:21:37.000000 usersgenerator-2.2.1/usersgenerator.egg-info/entry_points.txt
+-rwxrwxrwx   0 abel      (1000) abel      (1000)        9 2023-08-03 00:21:37.000000 usersgenerator-2.2.1/usersgenerator.egg-info/requires.txt
+-rwxrwxrwx   0 abel      (1000) abel      (1000)       15 2023-08-03 00:21:37.000000 usersgenerator-2.2.1/usersgenerator.egg-info/top_level.txt
```

### Comparing `usersgenerator-2.2.0/PKG-INFO` & `usersgenerator-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usersgenerator
-Version: 2.2.0
+Version: 2.2.1
 Summary: Generate possible users of an organization from some names
 Home-page: https://github.com/abeljm/UsersGenerator
 Author: Avelino Navarro
 Author-email: abeljm2017@gmail.com
 License: UNKNOWN
 Description: # Users Generator
```

### Comparing `usersgenerator-2.2.0/setup.py` & `usersgenerator-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="usersgenerator",
-    version="2.2.0",
+    version="2.2.1",
     description="Generate possible users of an organization from some names",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/abeljm/UsersGenerator",
     author="Avelino Navarro",
     author_email="abeljm2017@gmail.com",
     classifiers=[
```

### Comparing `usersgenerator-2.2.0/usersgenerator.egg-info/PKG-INFO` & `usersgenerator-2.2.1/usersgenerator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usersgenerator
-Version: 2.2.0
+Version: 2.2.1
 Summary: Generate possible users of an organization from some names
 Home-page: https://github.com/abeljm/UsersGenerator
 Author: Avelino Navarro
 Author-email: abeljm2017@gmail.com
 License: UNKNOWN
 Description: # Users Generator
```

