# Comparing `tmp/r_lambda-1.0.1.tar.gz` & `tmp/r_lambda-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r_lambda-1.0.1.tar", last modified: Fri Jul 21 08:58:22 2023, max compression
+gzip compressed data, was "r_lambda-1.0.2.tar", last modified: Thu Aug  3 00:51:40 2023, max compression
```

## Comparing `r_lambda-1.0.1.tar` & `r_lambda-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 08:58:22.279514 r_lambda-1.0.1/
--rw-rw-rw-   0        0        0     1108 2023-07-21 07:56:32.000000 r_lambda-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2414 2023-07-21 08:58:22.279514 r_lambda-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2048 2023-07-21 08:22:15.000000 r_lambda-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 08:58:22.255519 r_lambda-1.0.1/r_lambda/
--rw-rw-rw-   0        0        0     1905 2023-07-21 08:27:22.000000 r_lambda-1.0.1/r_lambda/__init__.py
--rw-rw-rw-   0        0        0     1989 2023-07-21 08:49:39.000000 r_lambda-1.0.1/r_lambda/docker.py
--rw-rw-rw-   0        0        0     1426 2023-07-21 08:44:42.000000 r_lambda-1.0.1/r_lambda/r_env.py
--rw-rw-rw-   0        0        0     2685 2023-07-21 08:47:52.000000 r_lambda-1.0.1/r_lambda/shell.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:58:22.277520 r_lambda-1.0.1/r_lambda.egg-info/
--rw-rw-rw-   0        0        0     2414 2023-07-21 08:58:22.000000 r_lambda-1.0.1/r_lambda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-07-21 08:58:22.000000 r_lambda-1.0.1/r_lambda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 08:58:22.000000 r_lambda-1.0.1/r_lambda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 08:58:22.000000 r_lambda-1.0.1/r_lambda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 08:58:22.289188 r_lambda-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-07-21 08:57:57.000000 r_lambda-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:51:40.943306 r_lambda-1.0.2/
+-rw-rw-rw-   0        0        0     1108 2023-08-03 00:34:31.000000 r_lambda-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2430 2023-08-03 00:51:40.942307 r_lambda-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2066 2023-08-03 00:40:19.000000 r_lambda-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 00:51:40.917309 r_lambda-1.0.2/r_lambda/
+-rw-rw-rw-   0        0        0     1905 2023-08-03 00:34:31.000000 r_lambda-1.0.2/r_lambda/__init__.py
+-rw-rw-rw-   0        0        0     2011 2023-08-03 00:36:52.000000 r_lambda-1.0.2/r_lambda/docker.py
+-rw-rw-rw-   0        0        0     1426 2023-08-03 00:34:31.000000 r_lambda-1.0.2/r_lambda/r_env.py
+-rw-rw-rw-   0        0        0     2871 2023-08-03 00:39:20.000000 r_lambda-1.0.2/r_lambda/shell.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:51:40.941309 r_lambda-1.0.2/r_lambda.egg-info/
+-rw-rw-rw-   0        0        0     2430 2023-08-03 00:51:40.000000 r_lambda-1.0.2/r_lambda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-08-03 00:51:40.000000 r_lambda-1.0.2/r_lambda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 00:51:40.000000 r_lambda-1.0.2/r_lambda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-03 00:51:40.000000 r_lambda-1.0.2/r_lambda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 00:51:40.943306 r_lambda-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      900 2023-08-03 00:50:13.000000 r_lambda-1.0.2/setup.py
```

### Comparing `r_lambda-1.0.1/LICENSE` & `r_lambda-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `r_lambda-1.0.1/PKG-INFO` & `r_lambda-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r_lambda
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple commandline wrapper package for call a target R# function from commandline
 Home-page: https://github.com/rsharp-lang/IronR
 Author: xieguigang
 Author-email: xie.guigang@gcmodeller.org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -58,19 +58,18 @@
 
 ## Call R# lambda from a python workflow
 
 For call a R# lambda function from your python workflow, then you could use this python package function. Current package call the R# workflow function running in local machine or running in a docker container already been wrapped into function calls, so that you can call such hello world function in ``R#`` package in python, example like:
 
 ```py
 import r_lambda
-
-from r_lambda import docker
+from r_lambda.docker import docker_image
 
 r_lambda.call_lambda("demo::hello_world", 
 argv = {"str": "world"}, 
     options = None,
     workdir = "./",
-    docker = docker.docker_image(id = "example_image", 
-        volumn = ["/home"], name = "test"), 
+    docker = docker_image(id = "example_image", 
+        volumn = ["/home"], name = "test", tty = True), 
     run_debug = False
 )
 ```
```

### Comparing `r_lambda-1.0.1/README.md` & `r_lambda-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,19 +46,18 @@
 
 ## Call R# lambda from a python workflow
 
 For call a R# lambda function from your python workflow, then you could use this python package function. Current package call the R# workflow function running in local machine or running in a docker container already been wrapped into function calls, so that you can call such hello world function in ``R#`` package in python, example like:
 
 ```py
 import r_lambda
-
-from r_lambda import docker
+from r_lambda.docker import docker_image
 
 r_lambda.call_lambda("demo::hello_world", 
 argv = {"str": "world"}, 
     options = None,
     workdir = "./",
-    docker = docker.docker_image(id = "example_image", 
-        volumn = ["/home"], name = "test"), 
+    docker = docker_image(id = "example_image", 
+        volumn = ["/home"], name = "test", tty = True), 
     run_debug = False
 )
-```
+```
```

### Comparing `r_lambda-1.0.1/r_lambda/__init__.py` & `r_lambda-1.0.2/r_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `r_lambda-1.0.1/r_lambda/docker.py` & `r_lambda-1.0.2/r_lambda/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import platform
 
-def docker_image(id, volumn=[], name=None):
+def docker_image(id, volumn=[], tty = True, name=None):
     """A helper function for create the docker argument
 
     Keyword arguments:
     id -- required, the docker image id to run the application
     volumn -- optional, the volumn names to mapping from the physical file system to
         the docker internal file system
     name -- optional, the name that specific to the running container,
         default value none means no name was specific.
     """
 
-    return {"image": id, "volumn": volumn, "name": name}
+    return {"image": id, "volumn": volumn, "name": name, tty: tty}
 
 
 def mount_volumn(docker_run, argv, workdir, docker_config):
     """Create the docker volumn mount argument
 
     + argv -- the target R# function parameters
     + docker -- the docker argument object for create docker run, this argument
```

### Comparing `r_lambda-1.0.1/r_lambda/r_env.py` & `r_lambda-1.0.2/r_lambda/r_env.py`

 * *Files identical despite different names*

### Comparing `r_lambda-1.0.1/r_lambda/shell.py` & `r_lambda-1.0.2/r_lambda/shell.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,15 +72,21 @@
 
         super().__init__(argv, options, workdir)
 
     def commandline(self, func):
         image_id = self.docker["image"]
 
         run_pipeline = []
-        run_pipeline.append("docker run -it --rm -e WINEDEBUG=-all")
+        run_pipeline.append("docker run")
+
+        # handling tty device for sbatch task
+        if not self.docker["tty"] is None and self.docker["tty"]:
+            run_pipeline.append("-it")
+
+        run_pipeline.append("--rm -e WINEDEBUG=-all")
 
         if not self.docker["name"] is None:
             run_pipeline.append('--name "{}"'.format(self.docker["name"]))
 
         run_pipeline = docker.mount_volumn(
             docker_run=run_pipeline,
             argv=self.argv,
```

### Comparing `r_lambda-1.0.1/r_lambda.egg-info/PKG-INFO` & `r_lambda-1.0.2/r_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r-lambda
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple commandline wrapper package for call a target R# function from commandline
 Home-page: https://github.com/rsharp-lang/IronR
 Author: xieguigang
 Author-email: xie.guigang@gcmodeller.org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -58,19 +58,18 @@
 
 ## Call R# lambda from a python workflow
 
 For call a R# lambda function from your python workflow, then you could use this python package function. Current package call the R# workflow function running in local machine or running in a docker container already been wrapped into function calls, so that you can call such hello world function in ``R#`` package in python, example like:
 
 ```py
 import r_lambda
-
-from r_lambda import docker
+from r_lambda.docker import docker_image
 
 r_lambda.call_lambda("demo::hello_world", 
 argv = {"str": "world"}, 
     options = None,
     workdir = "./",
-    docker = docker.docker_image(id = "example_image", 
-        volumn = ["/home"], name = "test"), 
+    docker = docker_image(id = "example_image", 
+        volumn = ["/home"], name = "test", tty = True), 
     run_debug = False
 )
 ```
```

### Comparing `r_lambda-1.0.1/setup.py` & `r_lambda-1.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import setuptools
 
+# install tools for build package
 # pip3 install setuptools wheel
+
+# then create the package
 # python3 setup.py sdist bdist_wheel
 
 # upload package to repository
 # pip3 install twine
 # twine upload --repository pypi dist/*
 
 # pip install test-package
@@ -13,15 +16,15 @@
 # from r_lambda.docker import docker_image
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setuptools.setup(
     name="r_lambda",
-    version="1.0.1",
+    version="1.0.2",
     author="xieguigang",
     author_email="xie.guigang@gcmodeller.org",
     packages=["r_lambda"],
     description="A simple commandline wrapper package for call a target R# function from commandline",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/rsharp-lang/IronR",
```

