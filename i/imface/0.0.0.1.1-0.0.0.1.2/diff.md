# Comparing `tmp/imface-0.0.0.1.1.tar.gz` & `tmp/imface-0.0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imface-0.0.0.1.1.tar", last modified: Thu Jul 27 15:21:11 2023, max compression
+gzip compressed data, was "imface-0.0.0.1.2.tar", last modified: Thu Aug  3 15:50:43 2023, max compression
```

## Comparing `imface-0.0.0.1.1.tar` & `imface-0.0.0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2023-07-27 15:21:11.502335 imface-0.0.0.1.1/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1066 2023-07-26 07:46:02.000000 imface-0.0.0.1.1/LICENSE
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       25 2023-07-27 15:17:32.000000 imface-0.0.0.1.1/MANIFEST.in
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      874 2023-07-27 15:21:11.502335 imface-0.0.0.1.1/PKG-INFO
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      616 2023-07-27 13:09:52.000000 imface-0.0.0.1.1/README.md
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2023-07-27 15:21:11.494336 imface-0.0.0.1.1/imface/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2023-07-26 06:03:13.000000 imface-0.0.0.1.1/imface/__init__.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       61 2023-07-26 06:30:47.000000 imface-0.0.0.1.1/imface/__main__.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2751 2023-07-27 15:19:28.000000 imface-0.0.0.1.1/imface/main.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2023-07-27 15:21:11.502335 imface-0.0.0.1.1/imface/utils/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      889 2023-07-26 08:16:23.000000 imface-0.0.0.1.1/imface/utils/deepface_util.py
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1922 2023-07-26 06:05:02.000000 imface-0.0.0.1.1/imface/utils/distance.py
-drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2023-07-27 15:21:11.498335 imface-0.0.0.1.1/imface.egg-info/
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      874 2023-07-27 15:21:11.000000 imface-0.0.0.1.1/imface.egg-info/PKG-INFO
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      328 2023-07-27 15:21:11.000000 imface-0.0.0.1.1/imface.egg-info/SOURCES.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        1 2023-07-27 15:21:11.000000 imface-0.0.0.1.1/imface.egg-info/dependency_links.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       44 2023-07-27 15:21:11.000000 imface-0.0.0.1.1/imface.egg-info/entry_points.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        9 2023-07-27 15:21:11.000000 imface-0.0.0.1.1/imface.egg-info/requires.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        7 2023-07-27 15:21:11.000000 imface-0.0.0.1.1/imface.egg-info/top_level.txt
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       38 2023-07-27 15:21:11.502335 imface-0.0.0.1.1/setup.cfg
--rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1708 2023-07-27 15:19:21.000000 imface-0.0.0.1.1/setup.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2023-08-03 15:50:43.311118 imface-0.0.0.1.2/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1066 2023-07-26 07:46:02.000000 imface-0.0.0.1.2/LICENSE
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       25 2023-07-27 15:17:32.000000 imface-0.0.0.1.2/MANIFEST.in
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      874 2023-08-03 15:50:43.311118 imface-0.0.0.1.2/PKG-INFO
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      616 2023-07-27 13:09:52.000000 imface-0.0.0.1.2/README.md
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2023-08-03 15:50:43.291118 imface-0.0.0.1.2/imface/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        0 2023-07-26 06:03:13.000000 imface-0.0.0.1.2/imface/__init__.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       61 2023-07-26 06:30:47.000000 imface-0.0.0.1.2/imface/__main__.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2851 2023-08-02 03:56:56.000000 imface-0.0.0.1.2/imface/main.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2023-08-03 15:50:43.307118 imface-0.0.0.1.2/imface/utils/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      889 2023-07-26 08:16:23.000000 imface-0.0.0.1.2/imface/utils/deepface_util.py
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     1922 2023-07-26 06:05:02.000000 imface-0.0.0.1.2/imface/utils/distance.py
+drwxrwxr-x   0 alfazari  (1000) alfazari  (1000)        0 2023-08-03 15:50:43.303118 imface-0.0.0.1.2/imface.egg-info/
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      874 2023-08-03 15:50:43.000000 imface-0.0.0.1.2/imface.egg-info/PKG-INFO
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)      328 2023-08-03 15:50:43.000000 imface-0.0.0.1.2/imface.egg-info/SOURCES.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        1 2023-08-03 15:50:43.000000 imface-0.0.0.1.2/imface.egg-info/dependency_links.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       44 2023-08-03 15:50:43.000000 imface-0.0.0.1.2/imface.egg-info/entry_points.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        9 2023-08-03 15:50:43.000000 imface-0.0.0.1.2/imface.egg-info/requires.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)        7 2023-08-03 15:50:43.000000 imface-0.0.0.1.2/imface.egg-info/top_level.txt
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)       38 2023-08-03 15:50:43.311118 imface-0.0.0.1.2/setup.cfg
+-rw-rw-r--   0 alfazari  (1000) alfazari  (1000)     2546 2023-08-03 15:50:11.000000 imface-0.0.0.1.2/setup.py
```

### Comparing `imface-0.0.0.1.1/LICENSE` & `imface-0.0.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imface-0.0.0.1.1/PKG-INFO` & `imface-0.0.0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imface
-Version: 0.0.0.1.1
+Version: 0.0.0.1.2
 Author: Achmad Alfazari
 License: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `imface-0.0.0.1.1/README.md` & `imface-0.0.0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `imface-0.0.0.1.1/imface/main.py` & `imface-0.0.0.1.2/imface/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,29 +33,32 @@
             print("image not exist")
             raise SystemExit(1)
         try:
             embed = utils.getEmbeddingVector(str(target_image))
             print(embed)
         except Exception as e:
             print("error " + repr(e))
+            raise SystemExit(1)
 
     elif args.extract:
         target_image = Path(args.extract)
 
         if not target_image.exists():
             print("image not exist")
             raise SystemExit(1)
         try:
             data = utils.extractFace(str(target_image))
             if len(data) > 1:
                 print("error only allowed one face")
             else:
                 print(data[0]['embedding'])
+                raise SystemExit(1)
         except Exception as e:
             print("error" + repr(e))
+            raise SystemExit(1)
 
     elif args.command == "distance":
         if args.source and args.target:
             # Convert the string representation of vectors to lists of floats
             source_vector = ast.literal_eval(args.source)
             target_vector = ast.literal_eval(args.target)
```

### Comparing `imface-0.0.0.1.1/imface/utils/deepface_util.py` & `imface-0.0.0.1.2/imface/utils/deepface_util.py`

 * *Files identical despite different names*

### Comparing `imface-0.0.0.1.1/imface/utils/distance.py` & `imface-0.0.0.1.2/imface/utils/distance.py`

 * *Files identical despite different names*

### Comparing `imface-0.0.0.1.1/imface.egg-info/PKG-INFO` & `imface-0.0.0.1.2/imface.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imface
-Version: 0.0.0.1.1
+Version: 0.0.0.1.2
 Author: Achmad Alfazari
 License: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `imface-0.0.0.1.1/setup.py` & `imface-0.0.0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,42 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from pathlib import Path
 import gdown
 import os
 
-home_dir = Path.home()
+
+def initialize_folder():
+    """Initialize the folder for storing weights and models.
+
+    Raises:
+        OSError: if the folder cannot be created.
+    """
+    home = get_deepface_home()
+    deepFaceHomePath = home + "/.deepface"
+    weightsPath = deepFaceHomePath + "/weights"
+
+    if not os.path.exists(deepFaceHomePath):
+        os.makedirs(deepFaceHomePath, exist_ok=True)
+        print("Directory ", home, "/.deepface created")
+
+    if not os.path.exists(weightsPath):
+        os.makedirs(weightsPath, exist_ok=True)
+        print("Directory ", home, "/.deepface/weights created")
+
+
+def get_deepface_home():
+    """Get the home directory for storing weights and models.
+
+    Returns:
+        str: the home directory.
+    """
+    return str(os.getenv("DEEPFACE_HOME", default=str(Path.home())))
+
+home_dir = get_deepface_home()
 def downloadWeights():
     facenet512_url = "https://github.com/serengil/deepface_models/releases/download/v1.0/facenet512_weights.h5"
     retinaface_url = "https://github.com/serengil/deepface_models/releases/download/v1.0/retinaface.h5"
     if os.path.isfile(str(home_dir) + "/.deepface/weights/facenet512_weights.h5") != True:
         print("facenet512_weights.h5 will be downloaded...")
 
         output = str(home_dir) + "/.deepface/weights/facenet512_weights.h5"
@@ -18,24 +46,25 @@
 
         output = str(home_dir) + "/.deepface/weights/retinaface.h5"
         gdown.download(retinaface_url, output, quiet=False)
 
 class CustomInstallCommand(install):
     def run(self):
         install.run(self)
+        initialize_folder()
         downloadWeights()
 
 with open("README.md", "r") as file:
     description = file.read()
 
 requirements = ["deepface"]
 
 setup(
     name='imface',
-    version='0.0.0.1.1',
+    version='0.0.0.1.2',
     install_requires=requirements,
     packages=find_packages(),
     include_package_data=True,
     entry_points={"console_scripts": ["imface=imface.main:main"]},
     author="Achmad Alfazari",
     license="License :: OSI Approved :: MIT License",
     classifiers=[
```

