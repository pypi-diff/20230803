# Comparing `tmp/robotchain_sdk-1.0.5.tar.gz` & `tmp/robotchain_sdk-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotchain_sdk-1.0.5.tar", last modified: Wed Aug  2 04:06:56 2023, max compression
+gzip compressed data, was "robotchain_sdk-1.0.6.tar", last modified: Thu Aug  3 02:31:28 2023, max compression
```

## Comparing `robotchain_sdk-1.0.5.tar` & `robotchain_sdk-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 04:06:56.498998 robotchain_sdk-1.0.5/
--rw-rw-rw-   0        0        0     1948 2023-08-02 04:06:56.498998 robotchain_sdk-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 04:06:56.473940 robotchain_sdk-1.0.5/robotchain_sdk/
--rw-rw-rw-   0        0        0      791 2023-08-02 03:25:23.000000 robotchain_sdk-1.0.5/robotchain_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:06:56.481005 robotchain_sdk-1.0.5/robotchain_sdk/board/
--rw-rw-rw-   0        0        0     2680 2023-08-02 03:57:53.000000 robotchain_sdk-1.0.5/robotchain_sdk/board/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:06:56.482005 robotchain_sdk-1.0.5/robotchain_sdk/ros/
--rw-rw-rw-   0        0        0     1353 2023-08-02 03:01:50.000000 robotchain_sdk-1.0.5/robotchain_sdk/ros/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:06:56.483005 robotchain_sdk-1.0.5/robotchain_sdk/utils/
--rw-rw-rw-   0        0        0      338 2023-08-02 04:06:08.000000 robotchain_sdk-1.0.5/robotchain_sdk/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:06:56.484003 robotchain_sdk-1.0.5/robotchain_sdk/utils/list/
--rw-rw-rw-   0        0        0      228 2023-08-02 04:05:36.000000 robotchain_sdk-1.0.5/robotchain_sdk/utils/list/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:06:56.496003 robotchain_sdk-1.0.5/robotchain_sdk/utils/loging/
--rw-rw-rw-   0        0        0     2849 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.5/robotchain_sdk/utils/loging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:06:56.497003 robotchain_sdk-1.0.5/robotchain_sdk/utils/random/
--rw-rw-rw-   0        0        0      445 2023-08-02 04:04:33.000000 robotchain_sdk-1.0.5/robotchain_sdk/utils/random/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:06:56.480006 robotchain_sdk-1.0.5/robotchain_sdk.egg-info/
--rw-rw-rw-   0        0        0     1948 2023-08-02 04:06:55.000000 robotchain_sdk-1.0.5/robotchain_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      402 2023-08-02 04:06:56.000000 robotchain_sdk-1.0.5/robotchain_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 04:06:55.000000 robotchain_sdk-1.0.5/robotchain_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-08-02 04:06:55.000000 robotchain_sdk-1.0.5/robotchain_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 04:06:56.499999 robotchain_sdk-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-08-02 04:06:48.000000 robotchain_sdk-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 02:31:28.116239 robotchain_sdk-1.0.6/
+-rw-rw-rw-   0        0        0     1948 2023-08-03 02:31:28.116239 robotchain_sdk-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 02:31:28.046259 robotchain_sdk-1.0.6/robotchain_sdk/
+-rw-rw-rw-   0        0        0      963 2023-08-03 02:30:01.000000 robotchain_sdk-1.0.6/robotchain_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 02:31:28.070251 robotchain_sdk-1.0.6/robotchain_sdk/board/
+-rw-rw-rw-   0        0        0     2680 2023-08-02 03:57:53.000000 robotchain_sdk-1.0.6/robotchain_sdk/board/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 02:31:28.079248 robotchain_sdk-1.0.6/robotchain_sdk/ros/
+-rw-rw-rw-   0        0        0     1353 2023-08-02 03:01:50.000000 robotchain_sdk-1.0.6/robotchain_sdk/ros/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 02:31:28.086245 robotchain_sdk-1.0.6/robotchain_sdk/utils/
+-rw-rw-rw-   0        0        0      338 2023-08-02 04:06:08.000000 robotchain_sdk-1.0.6/robotchain_sdk/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 02:31:28.093246 robotchain_sdk-1.0.6/robotchain_sdk/utils/list/
+-rw-rw-rw-   0        0        0      228 2023-08-02 04:05:36.000000 robotchain_sdk-1.0.6/robotchain_sdk/utils/list/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 02:31:28.107239 robotchain_sdk-1.0.6/robotchain_sdk/utils/loging/
+-rw-rw-rw-   0        0        0     2849 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.6/robotchain_sdk/utils/loging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 02:31:28.115236 robotchain_sdk-1.0.6/robotchain_sdk/utils/random/
+-rw-rw-rw-   0        0        0      445 2023-08-02 04:04:33.000000 robotchain_sdk-1.0.6/robotchain_sdk/utils/random/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 02:31:28.050259 robotchain_sdk-1.0.6/robotchain_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1948 2023-08-03 02:31:27.000000 robotchain_sdk-1.0.6/robotchain_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2023-08-03 02:31:27.000000 robotchain_sdk-1.0.6/robotchain_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 02:31:27.000000 robotchain_sdk-1.0.6/robotchain_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-08-03 02:31:27.000000 robotchain_sdk-1.0.6/robotchain_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 02:31:28.117235 robotchain_sdk-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      714 2023-08-03 02:30:57.000000 robotchain_sdk-1.0.6/setup.py
```

### Comparing `robotchain_sdk-1.0.5/PKG-INFO` & `robotchain_sdk-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotchain_sdk
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python development framework for robotchain.
 Home-page: https://github.com/geekros/python_framework_sdk
 Author: MakerYang
 Author-email: admin@wileho.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotchain_sdk-1.0.5/robotchain_sdk/__init__.py` & `robotchain_sdk-1.0.6/robotchain_sdk/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,18 @@
         self.utils = Utils(self)
         self.ros = ROS(self)
         self.setup()
 
     def setup(self):
         self.ros.client.run()
         self.utils.log.robot_start("Robot start.")
+        robot_start = "robot_start"
+        if robot_start in dir(app_file):
+            getattr(app_file, robot_start)(self)
+        self.sigint_handler(False, False)
 
     def sigint_handler(self, signum, frame):
         robot_exit = "robot_exit"
         if robot_exit in dir(app_file):
             getattr(app_file, robot_exit)(self)
         self.utils.log.robot_exit("Robot exit.")
         self.utils.time.sleep(.2)
```

### Comparing `robotchain_sdk-1.0.5/robotchain_sdk/board/__init__.py` & `robotchain_sdk-1.0.6/robotchain_sdk/board/__init__.py`

 * *Files identical despite different names*

### Comparing `robotchain_sdk-1.0.5/robotchain_sdk/ros/__init__.py` & `robotchain_sdk-1.0.6/robotchain_sdk/ros/__init__.py`

 * *Files identical despite different names*

### Comparing `robotchain_sdk-1.0.5/robotchain_sdk/utils/loging/__init__.py` & `robotchain_sdk-1.0.6/robotchain_sdk/utils/loging/__init__.py`

 * *Files identical despite different names*

### Comparing `robotchain_sdk-1.0.5/robotchain_sdk.egg-info/PKG-INFO` & `robotchain_sdk-1.0.6/robotchain_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotchain-sdk
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python development framework for robotchain.
 Home-page: https://github.com/geekros/python_framework_sdk
 Author: MakerYang
 Author-email: admin@wileho.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotchain_sdk-1.0.5/setup.py` & `robotchain_sdk-1.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="robotchain_sdk",
-    version="1.0.5",
+    version="1.0.6",
     author="MakerYang",
     author_email="admin@wileho.com",
     description="Python development framework for robotchain.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/geekros/python_framework_sdk",
     packages=find_packages(),
```

