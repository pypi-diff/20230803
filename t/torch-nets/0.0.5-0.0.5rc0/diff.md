# Comparing `tmp/torch-nets-0.0.5.tar.gz` & `tmp/torch-nets-0.0.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-nets-0.0.5.tar", last modified: Thu Aug  3 03:10:57 2023, max compression
+gzip compressed data, was "torch-nets-0.0.5rc0.tar", last modified: Thu Aug  3 02:58:06 2023, max compression
```

## Comparing `torch-nets-0.0.5.tar` & `torch-nets-0.0.5rc0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:10:57.195332 torch-nets-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-08-03 03:10:47.000000 torch-nets-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-08-03 03:10:57.195332 torch-nets-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-03 03:10:47.000000 torch-nets-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 03:10:57.195332 torch-nets-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-03 03:10:47.000000 torch-nets-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:10:57.191332 torch-nets-0.0.5/torch_nets/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/_augmented_torch_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/_torch_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:10:57.191332 torch-nets-0.0.5/torch_nets/core/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/core/_layer_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/core/_power_space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:10:57.191332 torch-nets-0.0.5/torch_nets/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/core/config/_activation_function_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/core/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/core/config/_layer_wise_attributes_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/core/config/_network_structure_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:10:57.195332 torch-nets-0.0.5/torch_nets/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/plotting/_plot_weights_and_biases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:10:57.195332 torch-nets-0.0.5/torch_nets/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-08-03 03:10:47.000000 torch-nets-0.0.5/torch_nets/tools/_infer_network_architecture_from_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:10:57.191332 torch-nets-0.0.5/torch_nets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-08-03 03:10:57.000000 torch-nets-0.0.5/torch_nets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-03 03:10:57.000000 torch-nets-0.0.5/torch_nets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 03:10:57.000000 torch-nets-0.0.5/torch_nets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 03:10:57.000000 torch-nets-0.0.5/torch_nets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 03:10:57.000000 torch-nets-0.0.5/torch_nets.egg-info/top_level.txt
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

### Comparing `torch-nets-0.0.5/LICENSE` & `torch-nets-0.0.5rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.5/PKG-INFO` & `torch-nets-0.0.5rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-nets
-Version: 0.0.5
+Version: 0.0.5rc0
 Summary: API to compose PyTorch neural networks on the fly.
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: torch-nets Version: 0.0.5 Summary: API to compose
-PyTorch neural networks on the fly. Author: Michael E. Vinyard Author-email:
-mvinyard.ai@gmail.com License: MIT Classifier: Development Status :: 2 - Pre-
-Alpha Classifier: Programming Language :: Python :: 3.9 Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
-Bio-Informatics Requires-Python: >3.9.0 Description-Content-Type: text/markdown
-License-File: LICENSE # ![logo](./docs/imgs/torch-nets.logo.png)  [![PyPI
-pyversions](https://img.shields.io/pypi/pyversions/torch-nets.svg)](https://
-pypi.python.org/pypi/torch-nets/) [![PyPI version](https://badge.fury.io/py/
-torch-nets.svg)](https://badge.fury.io/py/torch-nets) [![Code style: black]
-(https://img.shields.io/badge/code%20style-black-000000.svg)](https://
-github.com/psf/black)  Compose PyTorch neural networks with ease. ###
-Installation From PYPI (current version: [`v0.0.5`](https://pypi.org/project/
-torch-nets)) ```python pip install torch-nets ``` Alternatively, install the
-development version from GitHub: ```shell git clone https://github.com/
-mvinyard/torch-nets.git; cd torch-nets; pip install -e . ``` ### Example API
-use-cases ```python from torch_nets import TorchNet ``` #### Create a feed-
-forward neural network The only required arguments are `in_features` and
-`out_features`. The network can be made as simple or complex as you want
-through optional parameters. ```python net = TorchNet( in_features=50,
-out_features=50, hidden=[400, 400], activation="LeakyReLU", dropout=0.2,
-bias=True, output_bias=True, ) ```  See output
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
+Alternatively, install the development version from GitHub: ```shell git clone
+https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -e . ```
+### Example API use-cases ```python from torch_nets import TorchNet ``` ####
+Create a feed-forward neural network The only required arguments are
+`in_features` and `out_features`. The network can be made as simple or complex
+as you want through optional parameters. ```python net = TorchNet
+( in_features=50, out_features=50, hidden=[400, 400], activation="LeakyReLU",
+dropout=0.2, bias=True, output_bias=True, ) ```  See output
 ``` TorchNet( (hidden_1): Sequential( (linear): Linear(in_features=50,
 out_features=400, bias=True) (dropout): Dropout(p=0.2, inplace=False)
 (activation): LeakyReLU(negative_slope=0.01) ) (hidden_2): Sequential(
 (linear): Linear(in_features=400, out_features=400, bias=True) (dropout):
 Dropout(p=0.2, inplace=False) (activation): LeakyReLU(negative_slope=0.01) )
 (output): Sequential( (linear): Linear(in_features=400, out_features=50,
 bias=True) ) ) ```  ### Documentation For more information, including examples
```

### Comparing `torch-nets-0.0.5/README.md` & `torch-nets-0.0.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.5/setup.py` & `torch-nets-0.0.5rc0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import os
 import sys
 
 
 setuptools.setup(
     name="torch-nets",
-    version="0.0.5",
+    version="0.0.5rc0",
     python_requires=">3.9.0",
     author="Michael E. Vinyard",
     author_email="mvinyard.ai@gmail.com",
     url=None,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="API to compose PyTorch neural networks on the fly.",
```

### Comparing `torch-nets-0.0.5/torch_nets/__init__.py` & `torch-nets-0.0.5rc0/torch_nets/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 __module_name__ = "__init__.py"
 __doc__ = """Main API __init__.py module."""
 __author__ = ", ".join(["Michael E. Vinyard"])
 __email__ = ", ".join(["vinyard@g.harvard.edu",])
-__version__ = "0.0.5"
+__version__ = "0.0.5rc0"
 
 
 # -- import network modules: -------------------------------------------------------------
 from ._torch_net import TorchNet
 from ._encoder import Encoder
 from ._decoder import Decoder
 from ._augmented_torch_net import AugmentedTorchNet
```

### Comparing `torch-nets-0.0.5/torch_nets/_augmented_torch_net.py` & `torch-nets-0.0.5rc0/torch_nets/_augmented_torch_net.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.5/torch_nets/_decoder.py` & `torch-nets-0.0.5rc0/torch_nets/_decoder.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.5/torch_nets/_encoder.py` & `torch-nets-0.0.5rc0/torch_nets/_encoder.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.5/torch_nets/_torch_net.py` & `torch-nets-0.0.5rc0/torch_nets/_torch_net.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.5/torch_nets/core/_layer_builder.py` & `torch-nets-0.0.5rc0/torch_nets/core/_layer_builder.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.5/torch_nets/core/_power_space.py` & `torch-nets-0.0.5rc0/torch_nets/core/_power_space.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.5/torch_nets/core/config/_activation_function_config.py` & `torch-nets-0.0.5rc0/torch_nets/core/config/_activation_function_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.5/torch_nets/core/config/_config.py` & `torch-nets-0.0.5rc0/torch_nets/core/config/_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.5/torch_nets/core/config/_layer_wise_attributes_config.py` & `torch-nets-0.0.5rc0/torch_nets/core/config/_layer_wise_attributes_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.5/torch_nets/core/config/_network_structure_config.py` & `torch-nets-0.0.5rc0/torch_nets/core/config/_network_structure_config.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.5/torch_nets/plotting/_plot_weights_and_biases.py` & `torch-nets-0.0.5rc0/torch_nets/plotting/_plot_weights_and_biases.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.5/torch_nets/tools/_infer_network_architecture_from_state.py` & `torch-nets-0.0.5rc0/torch_nets/tools/_infer_network_architecture_from_state.py`

 * *Files identical despite different names*

### Comparing `torch-nets-0.0.5/torch_nets.egg-info/PKG-INFO` & `torch-nets-0.0.5rc0/torch_nets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-nets
-Version: 0.0.5
+Version: 0.0.5rc0
 Summary: API to compose PyTorch neural networks on the fly.
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: torch-nets Version: 0.0.5 Summary: API to compose
-PyTorch neural networks on the fly. Author: Michael E. Vinyard Author-email:
-mvinyard.ai@gmail.com License: MIT Classifier: Development Status :: 2 - Pre-
-Alpha Classifier: Programming Language :: Python :: 3.9 Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
-Bio-Informatics Requires-Python: >3.9.0 Description-Content-Type: text/markdown
-License-File: LICENSE # ![logo](./docs/imgs/torch-nets.logo.png)  [![PyPI
-pyversions](https://img.shields.io/pypi/pyversions/torch-nets.svg)](https://
-pypi.python.org/pypi/torch-nets/) [![PyPI version](https://badge.fury.io/py/
-torch-nets.svg)](https://badge.fury.io/py/torch-nets) [![Code style: black]
-(https://img.shields.io/badge/code%20style-black-000000.svg)](https://
-github.com/psf/black)  Compose PyTorch neural networks with ease. ###
-Installation From PYPI (current version: [`v0.0.5`](https://pypi.org/project/
-torch-nets)) ```python pip install torch-nets ``` Alternatively, install the
-development version from GitHub: ```shell git clone https://github.com/
-mvinyard/torch-nets.git; cd torch-nets; pip install -e . ``` ### Example API
-use-cases ```python from torch_nets import TorchNet ``` #### Create a feed-
-forward neural network The only required arguments are `in_features` and
-`out_features`. The network can be made as simple or complex as you want
-through optional parameters. ```python net = TorchNet( in_features=50,
-out_features=50, hidden=[400, 400], activation="LeakyReLU", dropout=0.2,
-bias=True, output_bias=True, ) ```  See output
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
+Alternatively, install the development version from GitHub: ```shell git clone
+https://github.com/mvinyard/torch-nets.git; cd torch-nets; pip install -e . ```
+### Example API use-cases ```python from torch_nets import TorchNet ``` ####
+Create a feed-forward neural network The only required arguments are
+`in_features` and `out_features`. The network can be made as simple or complex
+as you want through optional parameters. ```python net = TorchNet
+( in_features=50, out_features=50, hidden=[400, 400], activation="LeakyReLU",
+dropout=0.2, bias=True, output_bias=True, ) ```  See output
 ``` TorchNet( (hidden_1): Sequential( (linear): Linear(in_features=50,
 out_features=400, bias=True) (dropout): Dropout(p=0.2, inplace=False)
 (activation): LeakyReLU(negative_slope=0.01) ) (hidden_2): Sequential(
 (linear): Linear(in_features=400, out_features=400, bias=True) (dropout):
 Dropout(p=0.2, inplace=False) (activation): LeakyReLU(negative_slope=0.01) )
 (output): Sequential( (linear): Linear(in_features=400, out_features=50,
 bias=True) ) ) ```  ### Documentation For more information, including examples
```

### Comparing `torch-nets-0.0.5/torch_nets.egg-info/SOURCES.txt` & `torch-nets-0.0.5rc0/torch_nets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

