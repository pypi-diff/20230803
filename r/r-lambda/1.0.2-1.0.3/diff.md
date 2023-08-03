# Comparing `tmp/r_lambda-1.0.2.tar.gz` & `tmp/r_lambda-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r_lambda-1.0.2.tar", last modified: Thu Aug  3 00:51:40 2023, max compression
+gzip compressed data, was "r_lambda-1.0.3.tar", last modified: Thu Aug  3 03:12:06 2023, max compression
```

## Comparing `r_lambda-1.0.2.tar` & `r_lambda-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 00:51:40.943306 r_lambda-1.0.2/
--rw-rw-rw-   0        0        0     1108 2023-08-03 00:34:31.000000 r_lambda-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2430 2023-08-03 00:51:40.942307 r_lambda-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2066 2023-08-03 00:40:19.000000 r_lambda-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 00:51:40.917309 r_lambda-1.0.2/r_lambda/
--rw-rw-rw-   0        0        0     1905 2023-08-03 00:34:31.000000 r_lambda-1.0.2/r_lambda/__init__.py
--rw-rw-rw-   0        0        0     2011 2023-08-03 00:36:52.000000 r_lambda-1.0.2/r_lambda/docker.py
--rw-rw-rw-   0        0        0     1426 2023-08-03 00:34:31.000000 r_lambda-1.0.2/r_lambda/r_env.py
--rw-rw-rw-   0        0        0     2871 2023-08-03 00:39:20.000000 r_lambda-1.0.2/r_lambda/shell.py
-drwxrwxrwx   0        0        0        0 2023-08-03 00:51:40.941309 r_lambda-1.0.2/r_lambda.egg-info/
--rw-rw-rw-   0        0        0     2430 2023-08-03 00:51:40.000000 r_lambda-1.0.2/r_lambda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-08-03 00:51:40.000000 r_lambda-1.0.2/r_lambda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 00:51:40.000000 r_lambda-1.0.2/r_lambda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-03 00:51:40.000000 r_lambda-1.0.2/r_lambda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 00:51:40.943306 r_lambda-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      900 2023-08-03 00:50:13.000000 r_lambda-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:12:06.659327 r_lambda-1.0.3/
+-rw-rw-rw-   0        0        0     1108 2023-08-03 00:34:31.000000 r_lambda-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2430 2023-08-03 03:12:06.659327 r_lambda-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2066 2023-08-03 00:40:19.000000 r_lambda-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 03:12:06.652317 r_lambda-1.0.3/r_lambda/
+-rw-rw-rw-   0        0        0     1905 2023-08-03 00:34:31.000000 r_lambda-1.0.3/r_lambda/__init__.py
+-rw-rw-rw-   0        0        0     2013 2023-08-03 03:09:09.000000 r_lambda-1.0.3/r_lambda/docker.py
+-rw-rw-rw-   0        0        0     1426 2023-08-03 00:34:31.000000 r_lambda-1.0.3/r_lambda/r_env.py
+-rw-rw-rw-   0        0        0     2871 2023-08-03 00:39:20.000000 r_lambda-1.0.3/r_lambda/shell.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:12:06.658319 r_lambda-1.0.3/r_lambda.egg-info/
+-rw-rw-rw-   0        0        0     2430 2023-08-03 03:12:06.000000 r_lambda-1.0.3/r_lambda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-08-03 03:12:06.000000 r_lambda-1.0.3/r_lambda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 03:12:06.000000 r_lambda-1.0.3/r_lambda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-03 03:12:06.000000 r_lambda-1.0.3/r_lambda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 03:12:06.660318 r_lambda-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      900 2023-08-03 03:11:46.000000 r_lambda-1.0.3/setup.py
```

### Comparing `r_lambda-1.0.2/LICENSE` & `r_lambda-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `r_lambda-1.0.2/PKG-INFO` & `r_lambda-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r_lambda
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple commandline wrapper package for call a target R# function from commandline
 Home-page: https://github.com/rsharp-lang/IronR
 Author: xieguigang
 Author-email: xie.guigang@gcmodeller.org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `r_lambda-1.0.2/README.md` & `r_lambda-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `r_lambda-1.0.2/r_lambda/__init__.py` & `r_lambda-1.0.3/r_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `r_lambda-1.0.2/r_lambda/docker.py` & `r_lambda-1.0.3/r_lambda/docker.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     id -- required, the docker image id to run the application
     volumn -- optional, the volumn names to mapping from the physical file system to
         the docker internal file system
     name -- optional, the name that specific to the running container,
         default value none means no name was specific.
     """
 
-    return {"image": id, "volumn": volumn, "name": name, tty: tty}
+    return {"image": id, "volumn": volumn, "name": name, "tty": tty}
 
 
 def mount_volumn(docker_run, argv, workdir, docker_config):
     """Create the docker volumn mount argument
 
     + argv -- the target R# function parameters
     + docker -- the docker argument object for create docker run, this argument
```

### Comparing `r_lambda-1.0.2/r_lambda/r_env.py` & `r_lambda-1.0.3/r_lambda/r_env.py`

 * *Files identical despite different names*

### Comparing `r_lambda-1.0.2/r_lambda/shell.py` & `r_lambda-1.0.3/r_lambda/shell.py`

 * *Files identical despite different names*

### Comparing `r_lambda-1.0.2/r_lambda.egg-info/PKG-INFO` & `r_lambda-1.0.3/r_lambda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r-lambda
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple commandline wrapper package for call a target R# function from commandline
 Home-page: https://github.com/rsharp-lang/IronR
 Author: xieguigang
 Author-email: xie.guigang@gcmodeller.org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `r_lambda-1.0.2/setup.py` & `r_lambda-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # from r_lambda.docker import docker_image
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setuptools.setup(
     name="r_lambda",
-    version="1.0.2",
+    version="1.0.3",
     author="xieguigang",
     author_email="xie.guigang@gcmodeller.org",
     packages=["r_lambda"],
     description="A simple commandline wrapper package for call a target R# function from commandline",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/rsharp-lang/IronR",
```

