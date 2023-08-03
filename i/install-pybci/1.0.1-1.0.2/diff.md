# Comparing `tmp/install-pybci-1.0.1.tar.gz` & `tmp/install-pybci-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-1.0.1.tar", last modified: Wed Jun 28 23:44:44 2023, max compression
+gzip compressed data, was "install-pybci-1.0.2.tar", last modified: Thu Aug  3 19:32:58 2023, max compression
```

## Comparing `install-pybci-1.0.1.tar` & `install-pybci-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:44:44.663317 install-pybci-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-28 23:44:06.000000 install-pybci-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-28 23:44:06.000000 install-pybci-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-06-28 23:44:44.663317 install-pybci-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-28 23:44:06.000000 install-pybci-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:44:44.659317 install-pybci-1.0.1/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-06-28 23:44:44.000000 install-pybci-1.0.1/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-28 23:44:44.000000 install-pybci-1.0.1/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 23:44:44.000000 install-pybci-1.0.1/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-28 23:44:44.000000 install-pybci-1.0.1/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-28 23:44:44.000000 install-pybci-1.0.1/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:44:44.659317 install-pybci-1.0.1/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:44:44.659317 install-pybci-1.0.1/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:44:44.663317 install-pybci-1.0.1/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/ThreadClasses/OptimisedDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 23:44:44.663317 install-pybci-1.0.1/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/Utils/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20072 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 23:44:06.000000 install-pybci-1.0.1/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 23:44:44.663317 install-pybci-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-06-28 23:44:06.000000 install-pybci-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:32:58.122005 install-pybci-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 19:32:22.000000 install-pybci-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 19:32:22.000000 install-pybci-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-08-03 19:32:58.122005 install-pybci-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-08-03 19:32:22.000000 install-pybci-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:32:58.118005 install-pybci-1.0.2/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-08-03 19:32:58.000000 install-pybci-1.0.2/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-03 19:32:58.000000 install-pybci-1.0.2/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:32:58.000000 install-pybci-1.0.2/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 19:32:58.000000 install-pybci-1.0.2/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 19:32:58.000000 install-pybci-1.0.2/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:32:58.118005 install-pybci-1.0.2/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:32:58.122005 install-pybci-1.0.2/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:32:58.122005 install-pybci-1.0.2/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/ThreadClasses/OptimisedDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:32:58.122005 install-pybci-1.0.2/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/Utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20072 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 19:32:22.000000 install-pybci-1.0.2/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 19:32:58.122005 install-pybci-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-08-03 19:32:22.000000 install-pybci-1.0.2/setup.py
```

### Comparing `install-pybci-1.0.1/LICENSE` & `install-pybci-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-1.0.1/PKG-INFO` & `install-pybci-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, Pytorch, SciKit-Learn and Tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine-learning tensorflow sklearn pytorch human-computer-interaction bci lsl brain-computer-interface labstreaminglayer
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,29 +28,46 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci) [![PyPI - version](https://img.shields.io/pypi/v/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create real-time Brain Computer Interfaces (BCI's). with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create real-time Brain Computer Interfaces (BCI's). Data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
-## Installation
+# Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
 
-(currently using install-pybci due to pybci having name too similar with another package on pypi)
+## Prerequisite for Non-Windows Users
+If you are not using windows then there is a prerequisite stipulated on the [pylsl repository](home/liam/.local/lib/python3.10/site-packages/pylsl/lib) to obtain a liblsl shared library. See the [liblsl repo documentation](https://github.com/sccn/liblsl) for more information. 
+Once the liblsl library has been downloaded ```pip install install-pybci``` should work.
+
+(currently using install-pybci due to pybci having name too similar with another package on pypi, [issue here.](https://github.com/pypi/support/issues/2840))
 
 [ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/)      [Examples found here!](https://github.com/LMBooth/pybci/tree/main/pybci/Examples)
 
 [Examples of supported LSL hardware here!](https://labstreaminglayer.readthedocs.io/info/supported_devices.html)
 
+## Python Package Dependencies Version Minimums
+The following package versions define the minimum supported by PyBCI, also defined in setup.py:
+
+    "pylsl>=1.16.1",
+    "scipy>=1.11.1",
+    "numpy>=1.24.3",
+    "antropy>=0.1.6",
+    "tensorflow>=2.13.0",
+    "scikit-learn>=1.3.0",
+    "torch>=2.0.1"
+    
+Earlier packages may work but are not guaranteed to be supported.
+
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
 bci = PyBCI() # set default epoch timing, looks for first available lsl marker stream and all data streams
 bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
@@ -72,14 +89,14 @@
         print("Current marker estimation: " + str(guess), end="\r")
         time.sleep(0.5)
 except KeyboardInterrupt: # allow user to break while loop
     pass
 ```
 
 ## Background Information
-PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
+PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing - as a rule of thumb it would be advised when testing a model to have a time window overlap >= 50% (Shannon-Nyquist criterion). [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable pytorch, sklearn or tensorflow classifier can be given to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy. If enough epochs are received or high enough accuracy is obtained TestMode() can be called. Once in test mode you can query what pybci estimates the current bci epoch is(typically baseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
-## Any issues, recommendations, pull-requests and suggestions are welcome and encouraged!
+## All issues, recommendations, pull-requests and suggestions are welcome and encouraged!
```

### Comparing `install-pybci-1.0.1/README.md` & `install-pybci-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci) [![PyPI - version](https://img.shields.io/pypi/v/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create real-time Brain Computer Interfaces (BCI's). with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create real-time Brain Computer Interfaces (BCI's). Data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
-## Installation
+# Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
 
-(currently using install-pybci due to pybci having name too similar with another package on pypi)
+## Prerequisite for Non-Windows Users
+If you are not using windows then there is a prerequisite stipulated on the [pylsl repository](home/liam/.local/lib/python3.10/site-packages/pylsl/lib) to obtain a liblsl shared library. See the [liblsl repo documentation](https://github.com/sccn/liblsl) for more information. 
+Once the liblsl library has been downloaded ```pip install install-pybci``` should work.
+
+(currently using install-pybci due to pybci having name too similar with another package on pypi, [issue here.](https://github.com/pypi/support/issues/2840))
 
 [ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/)      [Examples found here!](https://github.com/LMBooth/pybci/tree/main/pybci/Examples)
 
 [Examples of supported LSL hardware here!](https://labstreaminglayer.readthedocs.io/info/supported_devices.html)
 
+## Python Package Dependencies Version Minimums
+The following package versions define the minimum supported by PyBCI, also defined in setup.py:
+
+    "pylsl>=1.16.1",
+    "scipy>=1.11.1",
+    "numpy>=1.24.3",
+    "antropy>=0.1.6",
+    "tensorflow>=2.13.0",
+    "scikit-learn>=1.3.0",
+    "torch>=2.0.1"
+    
+Earlier packages may work but are not guaranteed to be supported.
+
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
 bci = PyBCI() # set default epoch timing, looks for first available lsl marker stream and all data streams
 bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
@@ -42,14 +59,14 @@
         print("Current marker estimation: " + str(guess), end="\r")
         time.sleep(0.5)
 except KeyboardInterrupt: # allow user to break while loop
     pass
 ```
 
 ## Background Information
-PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
+PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing - as a rule of thumb it would be advised when testing a model to have a time window overlap >= 50% (Shannon-Nyquist criterion). [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable pytorch, sklearn or tensorflow classifier can be given to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy. If enough epochs are received or high enough accuracy is obtained TestMode() can be called. Once in test mode you can query what pybci estimates the current bci epoch is(typically baseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
-## Any issues, recommendations, pull-requests and suggestions are welcome and encouraged!
+## All issues, recommendations, pull-requests and suggestions are welcome and encouraged!
```

### Comparing `install-pybci-1.0.1/install_pybci.egg-info/PKG-INFO` & `install-pybci-1.0.2/install_pybci.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, Pytorch, SciKit-Learn and Tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine-learning tensorflow sklearn pytorch human-computer-interaction bci lsl brain-computer-interface labstreaminglayer
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,29 +28,46 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci) [![PyPI - version](https://img.shields.io/pypi/v/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create real-time Brain Computer Interfaces (BCI's). with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create real-time Brain Computer Interfaces (BCI's). Data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
-## Installation
+# Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
 
-(currently using install-pybci due to pybci having name too similar with another package on pypi)
+## Prerequisite for Non-Windows Users
+If you are not using windows then there is a prerequisite stipulated on the [pylsl repository](home/liam/.local/lib/python3.10/site-packages/pylsl/lib) to obtain a liblsl shared library. See the [liblsl repo documentation](https://github.com/sccn/liblsl) for more information. 
+Once the liblsl library has been downloaded ```pip install install-pybci``` should work.
+
+(currently using install-pybci due to pybci having name too similar with another package on pypi, [issue here.](https://github.com/pypi/support/issues/2840))
 
 [ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/)      [Examples found here!](https://github.com/LMBooth/pybci/tree/main/pybci/Examples)
 
 [Examples of supported LSL hardware here!](https://labstreaminglayer.readthedocs.io/info/supported_devices.html)
 
+## Python Package Dependencies Version Minimums
+The following package versions define the minimum supported by PyBCI, also defined in setup.py:
+
+    "pylsl>=1.16.1",
+    "scipy>=1.11.1",
+    "numpy>=1.24.3",
+    "antropy>=0.1.6",
+    "tensorflow>=2.13.0",
+    "scikit-learn>=1.3.0",
+    "torch>=2.0.1"
+    
+Earlier packages may work but are not guaranteed to be supported.
+
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
 bci = PyBCI() # set default epoch timing, looks for first available lsl marker stream and all data streams
 bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
@@ -72,14 +89,14 @@
         print("Current marker estimation: " + str(guess), end="\r")
         time.sleep(0.5)
 except KeyboardInterrupt: # allow user to break while loop
     pass
 ```
 
 ## Background Information
-PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
+PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing - as a rule of thumb it would be advised when testing a model to have a time window overlap >= 50% (Shannon-Nyquist criterion). [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable pytorch, sklearn or tensorflow classifier can be given to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy. If enough epochs are received or high enough accuracy is obtained TestMode() can be called. Once in test mode you can query what pybci estimates the current bci epoch is(typically baseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
-## Any issues, recommendations, pull-requests and suggestions are welcome and encouraged!
+## All issues, recommendations, pull-requests and suggestions are welcome and encouraged!
```

### Comparing `install-pybci-1.0.1/install_pybci.egg-info/SOURCES.txt` & `install-pybci-1.0.2/install_pybci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `install-pybci-1.0.1/pybci/Configuration/EpochSettings.py` & `install-pybci-1.0.2/pybci/Configuration/EpochSettings.py`

 * *Files identical despite different names*

### Comparing `install-pybci-1.0.1/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-1.0.2/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-1.0.1/pybci/ThreadClasses/ClassifierThread.py` & `install-pybci-1.0.2/pybci/ThreadClasses/ClassifierThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-1.0.1/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-1.0.2/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-1.0.1/pybci/ThreadClasses/FeatureProcessorThread.py` & `install-pybci-1.0.2/pybci/ThreadClasses/FeatureProcessorThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-1.0.1/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-1.0.2/pybci/ThreadClasses/MarkerThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-1.0.1/pybci/ThreadClasses/OptimisedDataReceiverThread.py` & `install-pybci-1.0.2/pybci/ThreadClasses/OptimisedDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-1.0.1/pybci/Utils/Classifier.py` & `install-pybci-1.0.2/pybci/Utils/Classifier.py`

 * *Files identical despite different names*

### Comparing `install-pybci-1.0.1/pybci/Utils/FeatureExtractor.py` & `install-pybci-1.0.2/pybci/Utils/FeatureExtractor.py`

 * *Files identical despite different names*

### Comparing `install-pybci-1.0.1/pybci/Utils/LSLScanner.py` & `install-pybci-1.0.2/pybci/Utils/LSLScanner.py`

 * *Files identical despite different names*

### Comparing `install-pybci-1.0.1/pybci/Utils/Logger.py` & `install-pybci-1.0.2/pybci/Utils/Logger.py`

 * *Files identical despite different names*

### Comparing `install-pybci-1.0.1/pybci/pybci.py` & `install-pybci-1.0.2/pybci/pybci.py`

 * *Files identical despite different names*

### Comparing `install-pybci-1.0.1/setup.py` & `install-pybci-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,21 +95,21 @@
     keywords='machine-learning tensorflow sklearn pytorch human-computer-interaction bci lsl brain-computer-interface labstreaminglayer',
 
     cmdclass={
         'bdist_wheel': bdist_wheel
     },
 
     install_requires=[
-        "pylsl",
-        "scipy",
-        "numpy",
-        "antropy",
-        "tensorflow",
-        "scikit-learn",
-        "torch"
+        "pylsl>=1.16.1",
+        "scipy>=1.11.1",
+        "numpy>=1.24.3",
+        "antropy>=0.1.6",
+        "tensorflow>=2.13.0",
+        "scikit-learn>=1.3.0",
+        "torch>=2.0.1"
     ],
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     packages= find_packages(),#['pybci', 'pybci.examples'],
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
```

