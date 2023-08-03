# Comparing `tmp/torch-nets-0.0.4rc0.tar.gz` & `tmp/torch-nets-0.0.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-nets-0.0.4rc0.tar", last modified: Thu Apr 13 19:09:08 2023, max compression
+gzip compressed data, was "torch-nets-0.0.5rc0.tar", last modified: Thu Aug  3 02:58:06 2023, max compression
```

## Comparing `torch-nets-0.0.4rc0.tar` & `torch-nets-0.0.5rc0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:08.396610 torch-nets-0.0.4rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-13 19:09:08.396610 torch-nets-0.0.4rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:09:08.396610 torch-nets-0.0.4rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:08.392610 torch-nets-0.0.4rc0/torch_nets/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/_augmented_torch_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/_torch_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:08.396610 torch-nets-0.0.4rc0/torch_nets/core/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/_layer_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/_power_space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:08.396610 torch-nets-0.0.4rc0/torch_nets/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/config/_activation_function_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/config/_layer_wise_attributes_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/core/config/_network_structure_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:08.396610 torch-nets-0.0.4rc0/torch_nets/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/plotting/_plot_weights_and_biases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:08.396610 torch-nets-0.0.4rc0/torch_nets/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-13 19:08:54.000000 torch-nets-0.0.4rc0/torch_nets/tools/_infer_network_architecture_from_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:09:08.392610 torch-nets-0.0.4rc0/torch_nets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-13 19:09:08.000000 torch-nets-0.0.4rc0/torch_nets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-13 19:09:08.000000 torch-nets-0.0.4rc0/torch_nets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:09:08.000000 torch-nets-0.0.4rc0/torch_nets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 19:09:08.000000 torch-nets-0.0.4rc0/torch_nets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 19:09:08.000000 torch-nets-0.0.4rc0/torch_nets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:58:06.368988 torch-nets-0.0.5rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-08-03 02:58:06.368988 torch-nets-0.0.5rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 02:58:06.368988 torch-nets-0.0.5rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:58:06.364988 torch-nets-0.0.5rc0/torch_nets/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/_augmented_torch_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/_torch_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:58:06.364988 torch-nets-0.0.5rc0/torch_nets/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/core/_layer_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/core/_power_space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:58:06.368988 torch-nets-0.0.5rc0/torch_nets/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/core/config/_activation_function_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/core/config/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/core/config/_layer_wise_attributes_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/core/config/_network_structure_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:58:06.368988 torch-nets-0.0.5rc0/torch_nets/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/plotting/_plot_weights_and_biases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:58:06.368988 torch-nets-0.0.5rc0/torch_nets/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-08-03 02:57:55.000000 torch-nets-0.0.5rc0/torch_nets/tools/_infer_network_architecture_from_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:58:06.364988 torch-nets-0.0.5rc0/torch_nets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-08-03 02:58:06.000000 torch-nets-0.0.5rc0/torch_nets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-03 02:58:06.000000 torch-nets-0.0.5rc0/torch_nets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 02:58:06.000000 torch-nets-0.0.5rc0/torch_nets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 02:58:06.000000 torch-nets-0.0.5rc0/torch_nets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 02:58:06.000000 torch-nets-0.0.5rc0/torch_nets.egg-info/top_level.txt
```

### Comparing `torch-nets-0.0.4rc0/LICENSE` & `torch-nets-0.0.5rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4rc0/PKG-INFO` & `torch-nets-0.0.5rc0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: torch-nets
-Version: 0.0.4rc0
+Version: 0.0.5rc0
 Summary: API to compose PyTorch neural networks on the fly.
-Author: Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital
-Author-email: mvinyard@broadinstitute.org
+Author: Michael E. Vinyard
+Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >3.7.0
+Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Torch-Nets
+# ![logo](./docs/imgs/torch-nets.logo.png)
+<!-- # Torch-Nets -->
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-nets.svg)](https://pypi.python.org/pypi/torch-nets/)
 [![PyPI version](https://badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
-<a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a>
+<!-- <a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a> -->
 
 Compose PyTorch neural networks with ease.
 
 ### Installation
 
-From PYPI (current version: [`v0.0.4rc0`](https://pypi.org/project/torch-nets))
+From PYPI (current version: [`v0.0.5`](https://pypi.org/project/torch-nets))
 ```python
 pip install torch-nets
 ```
 
 Alternatively, install the development version from GitHub:
 ```shell
 git clone https://github.com/mvinyard/torch-nets.git;
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: torch-nets Version: 0.0.4rc0 Summary: API to
-compose PyTorch neural networks on the fly. Author: Michael E. Vinyard -
-Harvard University - Broad Institute of MIT and Harvard - Massachussetts
-General Hospital Author-email: mvinyard@broadinstitute.org License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha Classifier: Programming
-Language :: Python :: 3.7 Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Requires-Python:
->3.7.0 Description-Content-Type: text/markdown License-File: LICENSE # Torch-
-Nets [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-
-nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version](https://
-badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets) [![Code
-style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
-(https://github.com/psf/black) [ol-reliable-spongebob] Compose PyTorch neural
-networks with ease. ### Installation From PYPI (current version: [`v0.0.4rc0`]
-(https://pypi.org/project/torch-nets)) ```python pip install torch-nets ```
+Metadata-Version: 2.1 Name: torch-nets Version: 0.0.5rc0 Summary: API to
+compose PyTorch neural networks on the fly. Author: Michael E. Vinyard Author-
+email: mvinyard.ai@gmail.com License: MIT Classifier: Development Status :: 2 -
+Pre-Alpha Classifier: Programming Language :: Python :: 3.9 Classifier:
+Intended Audience :: Science/Research Classifier: Topic :: Scientific/
+Engineering :: Bio-Informatics Requires-Python: >3.9.0 Description-Content-
+Type: text/markdown License-File: LICENSE # ![logo](./docs/imgs/torch-
+nets.logo.png)  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/
+torch-nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version]
+(https://badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg)](https://github.com/psf/black)  Compose PyTorch neural networks
+with ease. ### Installation From PYPI (current version: [`v0.0.5`](https://
+pypi.org/project/torch-nets)) ```python pip install torch-nets ```
 Alternatively, install the development version from GitHub: ```shell git clone
 https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -e . ```
 ### Example API use-cases ```python from torch_nets import TorchNet ``` ####
 Create a feed-forward neural network The only required arguments are
 `in_features` and `out_features`. The network can be made as simple or complex
 as you want through optional parameters. ```python net = TorchNet
 ( in_features=50, out_features=50, hidden=[400, 400], activation="LeakyReLU",
```

### Comparing `torch-nets-0.0.4rc0/README.md` & `torch-nets-0.0.5rc0/torch_nets.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,37 @@
-# Torch-Nets
+Metadata-Version: 2.1
+Name: torch-nets
+Version: 0.0.5rc0
+Summary: API to compose PyTorch neural networks on the fly.
+Author: Michael E. Vinyard
+Author-email: mvinyard.ai@gmail.com
+License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >3.9.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ![logo](./docs/imgs/torch-nets.logo.png)
+<!-- # Torch-Nets -->
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-nets.svg)](https://pypi.python.org/pypi/torch-nets/)
 [![PyPI version](https://badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
-<a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a>
+<!-- <a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a> -->
 
 Compose PyTorch neural networks with ease.
 
 ### Installation
 
-From PYPI (current version: [`v0.0.4rc0`](https://pypi.org/project/torch-nets))
+From PYPI (current version: [`v0.0.5`](https://pypi.org/project/torch-nets))
 ```python
 pip install torch-nets
 ```
 
 Alternatively, install the development version from GitHub:
 ```shell
 git clone https://github.com/mvinyard/torch-nets.git;
```

#### html2text {}

```diff
@@ -1,14 +1,21 @@
-# Torch-Nets [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-
-nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version](https://
-badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets) [![Code
-style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
-(https://github.com/psf/black) [ol-reliable-spongebob] Compose PyTorch neural
-networks with ease. ### Installation From PYPI (current version: [`v0.0.4rc0`]
-(https://pypi.org/project/torch-nets)) ```python pip install torch-nets ```
+Metadata-Version: 2.1 Name: torch-nets Version: 0.0.5rc0 Summary: API to
+compose PyTorch neural networks on the fly. Author: Michael E. Vinyard Author-
+email: mvinyard.ai@gmail.com License: MIT Classifier: Development Status :: 2 -
+Pre-Alpha Classifier: Programming Language :: Python :: 3.9 Classifier:
+Intended Audience :: Science/Research Classifier: Topic :: Scientific/
+Engineering :: Bio-Informatics Requires-Python: >3.9.0 Description-Content-
+Type: text/markdown License-File: LICENSE # ![logo](./docs/imgs/torch-
+nets.logo.png)  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/
+torch-nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version]
+(https://badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg)](https://github.com/psf/black)  Compose PyTorch neural networks
+with ease. ### Installation From PYPI (current version: [`v0.0.5`](https://
+pypi.org/project/torch-nets)) ```python pip install torch-nets ```
 Alternatively, install the development version from GitHub: ```shell git clone
 https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -e . ```
 ### Example API use-cases ```python from torch_nets import TorchNet ``` ####
 Create a feed-forward neural network The only required arguments are
 `in_features` and `out_features`. The network can be made as simple or complex
 as you want through optional parameters. ```python net = TorchNet
 ( in_features=50, out_features=50, hidden=[400, 400], activation="LeakyReLU",
```

### Comparing `torch-nets-0.0.4rc0/setup.py` & `torch-nets-0.0.5rc0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import re
 import os
 import sys
 
 
 setuptools.setup(
     name="torch-nets",
-    version="0.0.4rc0",
-    python_requires=">3.7.0",
-    author="Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital",
-    author_email="mvinyard@broadinstitute.org",
+    version="0.0.5rc0",
+    python_requires=">3.9.0",
+    author="Michael E. Vinyard",
+    author_email="mvinyard.ai@gmail.com",
     url=None,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="API to compose PyTorch neural networks on the fly.",
     packages=setuptools.find_packages(),
     install_requires=[
         "torch>=2.0.0",
-        "ABCParse>=0.0.3",
+        "ABCParse>=0.0.6",
         "vinplots>=0.0.75",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.9",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     license="MIT",
 )
```

### Comparing `torch-nets-0.0.4rc0/torch_nets/__init__.py` & `torch-nets-0.0.5rc0/torch_nets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 __module_name__ = "__init__.py"
 __doc__ = """Main API __init__.py module."""
 __author__ = ", ".join(["Michael E. Vinyard"])
 __email__ = ", ".join(["vinyard@g.harvard.edu",])
-__version__ = "0.0.4rc0"
+__version__ = "0.0.5rc0"
 
 
 # -- import network modules: -------------------------------------------------------------
 from ._torch_net import TorchNet
 from ._encoder import Encoder
 from ._decoder import Decoder
 from ._augmented_torch_net import AugmentedTorchNet
```

### Comparing `torch-nets-0.0.4rc0/torch_nets/_augmented_torch_net.py` & `torch-nets-0.0.5rc0/torch_nets/_augmented_torch_net.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         Notes:
         ------
         -> updates self.in_features
         -> updates self.out_features
         
         """
         
-        super(AugmentedTorchNet, self).__init__()
+        super().__init__()
 
         self.__parse__(locals())
         
         self._in_features_orig = in_features
         self._out_features_orig = out_features
         
         in_features += n_augment
```

### Comparing `torch-nets-0.0.4rc0/torch_nets/_decoder.py` & `torch-nets-0.0.5rc0/torch_nets/_decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             params than necessary are passed, they will go unused.
         """
 
         hidden = power_space(
             start=latent_dim, stop=data_dim, n=n_hidden + 2, power=power
         )[1:-1].tolist()
 
-        super(Decoder, self).__init__(
+        super().__init__(
             in_features=latent_dim,
             out_features=data_dim,
             hidden=hidden,
             activation=activation,
             dropout=dropout,
             bias=bias,
             output_bias=output_bias,
```

### Comparing `torch-nets-0.0.4rc0/torch_nets/_encoder.py` & `torch-nets-0.0.5rc0/torch_nets/_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             params than necessary are passed, they will go unused.
         """
         
         hidden = power_space(
             start=data_dim, stop=latent_dim, n=n_hidden + 2, power=power
         )[1:-1].tolist()
 
-        super(Encoder, self).__init__(
+        super().__init__(
             in_features=data_dim,
             out_features=latent_dim,
             hidden=hidden,
             activation=activation,
             dropout=dropout,
             bias=bias,
             output_bias=output_bias,
```

### Comparing `torch-nets-0.0.4rc0/torch_nets/_torch_net.py` & `torch-nets-0.0.5rc0/torch_nets/_torch_net.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,21 +44,21 @@
         self.config = Config(
             in_features=in_features,
             out_features=out_features,
             hidden=hidden,
         )
 
         self.names, layers = [], []
-        _net = self.__build__()
+        _net = self._build_net()
 
         for i, (_name, _layer) in enumerate(_net.items()):
             layers.append(_layer)
             self.names.append(_name)
 
-        super(TorchNet, self).__init__(*layers)
+        super().__init__(*layers)
         self._rename_nn_sequential_inplace(self, self.names)
 
     def _rename_nn_sequential_inplace(
         self, sequential: torch.nn.Sequential, names: List[str]
     ) -> None:
         new_modules = OrderedDict()
         for i, (k, v) in enumerate(sequential._modules.items()):
@@ -93,15 +93,15 @@
     def _build_output_layer(self, in_dim, out_dim):
         return LayerBuilder()(
             in_features=in_dim,
             out_features=out_dim,
             bias=self.output_bias,
         )
 
-    def __build__(self):
+    def _build_net(self):
         self.stack()
 
         TorchNetDict = {}
 
         for n, (layer_name, (in_dim, out_dim)) in enumerate(
             self.config.network_structure.items()
         ):
```

### Comparing `torch-nets-0.0.4rc0/torch_nets/core/_layer_builder.py` & `torch-nets-0.0.5rc0/torch_nets/core/_layer_builder.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4rc0/torch_nets/core/_power_space.py` & `torch-nets-0.0.5rc0/torch_nets/core/_power_space.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4rc0/torch_nets/core/config/_activation_function_config.py` & `torch-nets-0.0.5rc0/torch_nets/core/config/_activation_function_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4rc0/torch_nets/core/config/_config.py` & `torch-nets-0.0.5rc0/torch_nets/core/config/_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4rc0/torch_nets/core/config/_layer_wise_attributes_config.py` & `torch-nets-0.0.5rc0/torch_nets/core/config/_layer_wise_attributes_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4rc0/torch_nets/core/config/_network_structure_config.py` & `torch-nets-0.0.5rc0/torch_nets/core/config/_network_structure_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4rc0/torch_nets/plotting/_plot_weights_and_biases.py` & `torch-nets-0.0.5rc0/torch_nets/plotting/_plot_weights_and_biases.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4rc0/torch_nets/tools/_infer_network_architecture_from_state.py` & `torch-nets-0.0.5rc0/torch_nets/tools/_infer_network_architecture_from_state.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.4rc0/torch_nets.egg-info/PKG-INFO` & `torch-nets-0.0.5rc0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,22 @@
-Metadata-Version: 2.1
-Name: torch-nets
-Version: 0.0.4rc0
-Summary: API to compose PyTorch neural networks on the fly.
-Author: Michael E. Vinyard - Harvard University - Broad Institute of MIT and Harvard - Massachussetts General Hospital
-Author-email: mvinyard@broadinstitute.org
-License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Torch-Nets
+# ![logo](./docs/imgs/torch-nets.logo.png)
+<!-- # Torch-Nets -->
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-nets.svg)](https://pypi.python.org/pypi/torch-nets/)
 [![PyPI version](https://badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
-<a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a>
+<!-- <a href="https://github.com/mvinyard/torch-nets/"><img src="/docs/imgs/ol-reliable-spongebob.gif" alt="ol-reliable-spongebob" width="400"/></a> -->
 
 Compose PyTorch neural networks with ease.
 
 ### Installation
 
-From PYPI (current version: [`v0.0.4rc0`](https://pypi.org/project/torch-nets))
+From PYPI (current version: [`v0.0.5`](https://pypi.org/project/torch-nets))
 ```python
 pip install torch-nets
 ```
 
 Alternatively, install the development version from GitHub:
 ```shell
 git clone https://github.com/mvinyard/torch-nets.git;
```

#### html2text {}

```diff
@@ -1,30 +1,23 @@
-Metadata-Version: 2.1 Name: torch-nets Version: 0.0.4rc0 Summary: API to
-compose PyTorch neural networks on the fly. Author: Michael E. Vinyard -
-Harvard University - Broad Institute of MIT and Harvard - Massachussetts
-General Hospital Author-email: mvinyard@broadinstitute.org License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha Classifier: Programming
-Language :: Python :: 3.7 Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Requires-Python:
->3.7.0 Description-Content-Type: text/markdown License-File: LICENSE # Torch-
-Nets [![PyPI pyversions](https://img.shields.io/pypi/pyversions/torch-
-nets.svg)](https://pypi.python.org/pypi/torch-nets/) [![PyPI version](https://
-badge.fury.io/py/torch-nets.svg)](https://badge.fury.io/py/torch-nets) [![Code
-style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
-(https://github.com/psf/black) [ol-reliable-spongebob] Compose PyTorch neural
-networks with ease. ### Installation From PYPI (current version: [`v0.0.4rc0`]
-(https://pypi.org/project/torch-nets)) ```python pip install torch-nets ```
-Alternatively, install the development version from GitHub: ```shell git clone
-https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -e . ```
-### Example API use-cases ```python from torch_nets import TorchNet ``` ####
-Create a feed-forward neural network The only required arguments are
-`in_features` and `out_features`. The network can be made as simple or complex
-as you want through optional parameters. ```python net = TorchNet
-( in_features=50, out_features=50, hidden=[400, 400], activation="LeakyReLU",
-dropout=0.2, bias=True, output_bias=True, ) ```  See output
+# ![logo](./docs/imgs/torch-nets.logo.png)  [![PyPI pyversions](https://
+img.shields.io/pypi/pyversions/torch-nets.svg)](https://pypi.python.org/pypi/
+torch-nets/) [![PyPI version](https://badge.fury.io/py/torch-nets.svg)](https:/
+/badge.fury.io/py/torch-nets) [![Code style: black](https://img.shields.io/
+badge/code%20style-black-000000.svg)](https://github.com/psf/black)  Compose
+PyTorch neural networks with ease. ### Installation From PYPI (current version:
+[`v0.0.5`](https://pypi.org/project/torch-nets)) ```python pip install torch-
+nets ``` Alternatively, install the development version from GitHub: ```shell
+git clone https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip
+install -e . ``` ### Example API use-cases ```python from torch_nets import
+TorchNet ``` #### Create a feed-forward neural network The only required
+arguments are `in_features` and `out_features`. The network can be made as
+simple or complex as you want through optional parameters. ```python net =
+TorchNet( in_features=50, out_features=50, hidden=[400, 400],
+activation="LeakyReLU", dropout=0.2, bias=True, output_bias=True, ) ```  See
+output
 ``` TorchNet( (hidden_1): Sequential( (linear): Linear(in_features=50,
 out_features=400, bias=True) (dropout): Dropout(p=0.2, inplace=False)
 (activation): LeakyReLU(negative_slope=0.01) ) (hidden_2): Sequential(
 (linear): Linear(in_features=400, out_features=400, bias=True) (dropout):
 Dropout(p=0.2, inplace=False) (activation): LeakyReLU(negative_slope=0.01) )
 (output): Sequential( (linear): Linear(in_features=400, out_features=50,
 bias=True) ) ) ```  ### Documentation For more information, including examples
```

### Comparing `torch-nets-0.0.4rc0/torch_nets.egg-info/SOURCES.txt` & `torch-nets-0.0.5rc0/torch_nets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

