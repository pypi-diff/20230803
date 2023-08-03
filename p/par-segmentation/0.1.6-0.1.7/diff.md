# Comparing `tmp/par_segmentation-0.1.6.tar.gz` & `tmp/par_segmentation-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/par-segmentation/par-segmentation/dist/.tmp-yphhugs8/par_segmentation-0.1.6.tar", last modified: Tue Aug  1 16:14:54 2023, max compression
+gzip compressed data, was "/home/runner/work/par-segmentation/par-segmentation/dist/.tmp-v4gdphlq/par_segmentation-0.1.7.tar", last modified: Thu Aug  3 13:18:38 2023, max compression
```

## Comparing `par_segmentation-0.1.6.tar` & `par_segmentation-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/par_segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18880 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/quantifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/roi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/par_segmentation/tgf_interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/par_segmentation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/par_segmentation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/par_segmentation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/par_segmentation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/par_segmentation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/par_segmentation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 16:14:54.000000 par_segmentation-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/tests/test_de_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/tests/test_de_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/tests/test_gd_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-01 16:14:40.000000 par_segmentation-0.1.6/tests/test_gd_correct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:18:38.000000 par_segmentation-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-08-03 13:18:38.000000 par_segmentation-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:18:38.000000 par_segmentation-0.1.7/par_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/par_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18880 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/par_segmentation/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/par_segmentation/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/par_segmentation/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/par_segmentation/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/par_segmentation/quantifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/par_segmentation/roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/par_segmentation/tgf_interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:18:38.000000 par_segmentation-0.1.7/par_segmentation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-08-03 13:18:38.000000 par_segmentation-0.1.7/par_segmentation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-03 13:18:38.000000 par_segmentation-0.1.7/par_segmentation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 13:18:38.000000 par_segmentation-0.1.7/par_segmentation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-03 13:18:38.000000 par_segmentation-0.1.7/par_segmentation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 13:18:38.000000 par_segmentation-0.1.7/par_segmentation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 13:18:38.000000 par_segmentation-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:18:38.000000 par_segmentation-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/tests/test_de_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/tests/test_de_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/tests/test_gd_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-03 13:18:25.000000 par_segmentation-0.1.7/tests/test_gd_correct.py
```

### Comparing `par_segmentation-0.1.6/LICENSE` & `par_segmentation-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.6/PKG-INFO` & `par_segmentation-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: par_segmentation
-Version: 0.1.6
+Version: 0.1.7
 Summary: Cell cortex segmentation in C. elegans PAR protein images
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
 Project-URL: Source Code, https://github.com/tsmbland/par-segmentation
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,27 +35,26 @@
 
 To run in the cloud using Binder, click here: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/par-segmentation/HEAD?filepath=%2Fscripts/Tutorial.ipynb)
 
 (Please note that it may take several minutes to open the notebook)
 
 #### Option 2: Docker
 
-Step 1: With [Docker](https://www.docker.com/products/docker-desktop/) open on your machine,  pull the image (copy and paste into the terminal)
+Step 1: Make sure [Docker](https://www.docker.com/products/docker-desktop/) is installed and open on your machine 
 
-    docker pull tsmbland/par-segmentation
+Step 2: Download and run the Docker container: 
 
-Step 2: Run the docker container (copy and paste into the terminal)
+    docker run --rm -p 8888:8888 tsmbland/par-segmentation
 
-    docker run -p 8888:8888 tsmbland/par-segmentation
+Once the Docker image has finished downloading, this will print two URLs at the bottom for you to copy and paste into your web browser to open up Jupyter (please try both)
 
-This will print a URL at the bottom for you to copy and paste into your web browser to open up Jupyter
+Step 3: Navigate to _scripts/Tutorial.ipynb_ to run the notebook
+
+Step 4: When finished, delete the image:
 
-Step 3: When finished, delete the container and image
-    
-    docker container prune -f
     docker image rm tsmbland/par-segmentation
 
 #### Option 3: Conda
 
 You can use the environment.yml file to set up a [Conda](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html) environment on your machine from which the notebook can be run
 
     conda env create -f environment.yml
@@ -64,14 +63,15 @@
 
 
 ## Installation
 
 To explore further and incorporate into your own analysis pipelines, you can install the package using pip:
 
     pip install par-segmentation
+    pip install tensorflow
 
 ## Methods
 
 Starting with an initial rough manual ROI of the cell edge, the cortex of the image is straightened (Step 1).
 The program then attempts to mimic this straightened image by differentiable simulation (Step 2).
 In doing so, it learns the position of the cortex, which enables the ROI to be adjusted (Step 3) and the cortex re-straightened.
```

### Comparing `par_segmentation-0.1.6/README.md` & `par_segmentation-0.1.7/par_segmentation.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: par-segmentation
+Version: 0.1.7
+Summary: Cell cortex segmentation in C. elegans PAR protein images
+Author: Tom Bland
+Author-email: tom_bland@hotmail.co.uk
+License: CC BY 4.0
+Project-URL: Source Code, https://github.com/tsmbland/par-segmentation
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PAR Segmentation
 
 [![CC BY 4.0][cc-by-shield]][cc-by]
 ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
 [![PyPi version](https://badgen.net/pypi/v/par-segmentation/)](https://pypi.org/project/par-segmentation)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/par-segmentation/HEAD?filepath=%2Fscripts/Tutorial.ipynb)
 [![run with docker](https://img.shields.io/badge/run%20with-docker-0db7ed?logo=docker)](https://www.docker.com/)
@@ -24,27 +35,26 @@
 
 To run in the cloud using Binder, click here: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/par-segmentation/HEAD?filepath=%2Fscripts/Tutorial.ipynb)
 
 (Please note that it may take several minutes to open the notebook)
 
 #### Option 2: Docker
 
-Step 1: With [Docker](https://www.docker.com/products/docker-desktop/) open on your machine,  pull the image (copy and paste into the terminal)
+Step 1: Make sure [Docker](https://www.docker.com/products/docker-desktop/) is installed and open on your machine 
+
+Step 2: Download and run the Docker container: 
 
-    docker pull tsmbland/par-segmentation
+    docker run --rm -p 8888:8888 tsmbland/par-segmentation
 
-Step 2: Run the docker container (copy and paste into the terminal)
+Once the Docker image has finished downloading, this will print two URLs at the bottom for you to copy and paste into your web browser to open up Jupyter (please try both)
 
-    docker run -p 8888:8888 tsmbland/par-segmentation
+Step 3: Navigate to _scripts/Tutorial.ipynb_ to run the notebook
 
-This will print a URL at the bottom for you to copy and paste into your web browser to open up Jupyter
+Step 4: When finished, delete the image:
 
-Step 3: When finished, delete the container and image
-    
-    docker container prune -f
     docker image rm tsmbland/par-segmentation
 
 #### Option 3: Conda
 
 You can use the environment.yml file to set up a [Conda](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html) environment on your machine from which the notebook can be run
 
     conda env create -f environment.yml
@@ -53,14 +63,15 @@
 
 
 ## Installation
 
 To explore further and incorporate into your own analysis pipelines, you can install the package using pip:
 
     pip install par-segmentation
+    pip install tensorflow
 
 ## Methods
 
 Starting with an initial rough manual ROI of the cell edge, the cortex of the image is straightened (Step 1).
 The program then attempts to mimic this straightened image by differentiable simulation (Step 2).
 In doing so, it learns the position of the cortex, which enables the ROI to be adjusted (Step 3) and the cortex re-straightened.
```

### Comparing `par_segmentation-0.1.6/par_segmentation/funcs.py` & `par_segmentation-0.1.7/par_segmentation/funcs.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.6/par_segmentation/interactive.py` & `par_segmentation-0.1.7/par_segmentation/interactive.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.6/par_segmentation/legacy.py` & `par_segmentation-0.1.7/par_segmentation/legacy.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.6/par_segmentation/model.py` & `par_segmentation-0.1.7/par_segmentation/model.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.6/par_segmentation/quantifier.py` & `par_segmentation-0.1.7/par_segmentation/quantifier.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.6/par_segmentation/roi.py` & `par_segmentation-0.1.7/par_segmentation/roi.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.6/par_segmentation/tgf_interpolate.py` & `par_segmentation-0.1.7/par_segmentation/tgf_interpolate.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.6/par_segmentation.egg-info/PKG-INFO` & `par_segmentation-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: par-segmentation
-Version: 0.1.6
-Summary: Cell cortex segmentation in C. elegans PAR protein images
-Author: Tom Bland
-Author-email: tom_bland@hotmail.co.uk
-License: CC BY 4.0
-Project-URL: Source Code, https://github.com/tsmbland/par-segmentation
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PAR Segmentation
 
 [![CC BY 4.0][cc-by-shield]][cc-by]
 ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
 [![PyPi version](https://badgen.net/pypi/v/par-segmentation/)](https://pypi.org/project/par-segmentation)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/par-segmentation/HEAD?filepath=%2Fscripts/Tutorial.ipynb)
 [![run with docker](https://img.shields.io/badge/run%20with-docker-0db7ed?logo=docker)](https://www.docker.com/)
@@ -35,27 +24,26 @@
 
 To run in the cloud using Binder, click here: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/par-segmentation/HEAD?filepath=%2Fscripts/Tutorial.ipynb)
 
 (Please note that it may take several minutes to open the notebook)
 
 #### Option 2: Docker
 
-Step 1: With [Docker](https://www.docker.com/products/docker-desktop/) open on your machine,  pull the image (copy and paste into the terminal)
+Step 1: Make sure [Docker](https://www.docker.com/products/docker-desktop/) is installed and open on your machine 
+
+Step 2: Download and run the Docker container: 
 
-    docker pull tsmbland/par-segmentation
+    docker run --rm -p 8888:8888 tsmbland/par-segmentation
 
-Step 2: Run the docker container (copy and paste into the terminal)
+Once the Docker image has finished downloading, this will print two URLs at the bottom for you to copy and paste into your web browser to open up Jupyter (please try both)
 
-    docker run -p 8888:8888 tsmbland/par-segmentation
+Step 3: Navigate to _scripts/Tutorial.ipynb_ to run the notebook
 
-This will print a URL at the bottom for you to copy and paste into your web browser to open up Jupyter
+Step 4: When finished, delete the image:
 
-Step 3: When finished, delete the container and image
-    
-    docker container prune -f
     docker image rm tsmbland/par-segmentation
 
 #### Option 3: Conda
 
 You can use the environment.yml file to set up a [Conda](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html) environment on your machine from which the notebook can be run
 
     conda env create -f environment.yml
@@ -64,14 +52,15 @@
 
 
 ## Installation
 
 To explore further and incorporate into your own analysis pipelines, you can install the package using pip:
 
     pip install par-segmentation
+    pip install tensorflow
 
 ## Methods
 
 Starting with an initial rough manual ROI of the cell edge, the cortex of the image is straightened (Step 1).
 The program then attempts to mimic this straightened image by differentiable simulation (Step 2).
 In doing so, it learns the position of the cortex, which enables the ROI to be adjusted (Step 3) and the cortex re-straightened.
```

### Comparing `par_segmentation-0.1.6/par_segmentation.egg-info/SOURCES.txt` & `par_segmentation-0.1.7/par_segmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.6/setup.py` & `par_segmentation-0.1.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='par_segmentation',
-    version='0.1.6',
+    version='0.1.7',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     install_requires=['numpy',
                       'matplotlib',
                       'scipy',
                       'ipywidgets',
                       'scikit-image',
                       'jupyter',
                       'opencv-python',
                       'joblib',
-                      'tensorflow>=2.9.1',
                       'tqdm',
                       'pandas',
                       'absl-py'],
     description='Cell cortex segmentation in C. elegans PAR protein images',
     long_description=long_description,
     long_description_content_type='text/markdown',
     project_urls={
```

### Comparing `par_segmentation-0.1.6/tests/test_de_completion.py` & `par_segmentation-0.1.7/tests/test_de_completion.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.6/tests/test_de_correct.py` & `par_segmentation-0.1.7/tests/test_de_correct.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.6/tests/test_gd_completion.py` & `par_segmentation-0.1.7/tests/test_gd_completion.py`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.6/tests/test_gd_correct.py` & `par_segmentation-0.1.7/tests/test_gd_correct.py`

 * *Files identical despite different names*

