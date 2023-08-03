# Comparing `tmp/cospgd-0.1.0.tar.gz` & `tmp/cospgd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cospgd-0.1.0.tar", last modified: Thu Aug  3 19:03:52 2023, max compression
+gzip compressed data, was "cospgd-0.1.1.tar", last modified: Thu Aug  3 19:45:19 2023, max compression
```

## Comparing `cospgd-0.1.0.tar` & `cospgd-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 shashank  (1000) shashank  (1000)        0 2023-08-03 19:03:52.119117 cospgd-0.1.0/
--rw-rw-r--   0 shashank  (1000) shashank  (1000)     1114 2023-08-03 16:40:23.000000 cospgd-0.1.0/LICENSE.md
--rw-rw-r--   0 shashank  (1000) shashank  (1000)     1010 2023-08-03 19:03:52.119117 cospgd-0.1.0/PKG-INFO
--rw-rw-r--   0 shashank  (1000) shashank  (1000)     1813 2023-08-03 16:23:45.000000 cospgd-0.1.0/README.md
-drwxrwxr-x   0 shashank  (1000) shashank  (1000)        0 2023-08-03 19:03:52.119117 cospgd-0.1.0/cospgd/
--rw-rw-r--   0 shashank  (1000) shashank  (1000)      470 2023-08-03 17:23:15.000000 cospgd-0.1.0/cospgd/__init__.py
--rw-rw-r--   0 shashank  (1000) shashank  (1000)    11604 2023-08-03 18:56:54.000000 cospgd-0.1.0/cospgd/attack_implementations.py
-drwxrwxr-x   0 shashank  (1000) shashank  (1000)        0 2023-08-03 19:03:52.119117 cospgd-0.1.0/cospgd.egg-info/
--rw-rw-r--   0 shashank  (1000) shashank  (1000)     1010 2023-08-03 19:03:52.000000 cospgd-0.1.0/cospgd.egg-info/PKG-INFO
--rw-rw-r--   0 shashank  (1000) shashank  (1000)      230 2023-08-03 19:03:52.000000 cospgd-0.1.0/cospgd.egg-info/SOURCES.txt
--rw-rw-r--   0 shashank  (1000) shashank  (1000)        1 2023-08-03 19:03:52.000000 cospgd-0.1.0/cospgd.egg-info/dependency_links.txt
--rw-rw-r--   0 shashank  (1000) shashank  (1000)       17 2023-08-03 19:03:52.000000 cospgd-0.1.0/cospgd.egg-info/requires.txt
--rw-rw-r--   0 shashank  (1000) shashank  (1000)        7 2023-08-03 19:03:52.000000 cospgd-0.1.0/cospgd.egg-info/top_level.txt
--rw-rw-r--   0 shashank  (1000) shashank  (1000)       38 2023-08-03 19:03:52.119117 cospgd-0.1.0/setup.cfg
--rw-rw-r--   0 shashank  (1000) shashank  (1000)     1207 2023-08-03 17:38:59.000000 cospgd-0.1.0/setup.py
+drwxrwxr-x   0 shashank  (1000) shashank  (1000)        0 2023-08-03 19:45:19.718332 cospgd-0.1.1/
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)     1114 2023-08-03 16:40:23.000000 cospgd-0.1.1/LICENSE.md
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)     1010 2023-08-03 19:45:19.718332 cospgd-0.1.1/PKG-INFO
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)     1813 2023-08-03 16:23:45.000000 cospgd-0.1.1/README.md
+drwxrwxr-x   0 shashank  (1000) shashank  (1000)        0 2023-08-03 19:45:19.718332 cospgd-0.1.1/cospgd/
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)      470 2023-08-03 17:23:15.000000 cospgd-0.1.1/cospgd/__init__.py
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)    11624 2023-08-03 19:37:49.000000 cospgd-0.1.1/cospgd/attack_implementations.py
+drwxrwxr-x   0 shashank  (1000) shashank  (1000)        0 2023-08-03 19:45:19.718332 cospgd-0.1.1/cospgd.egg-info/
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)     1010 2023-08-03 19:45:19.000000 cospgd-0.1.1/cospgd.egg-info/PKG-INFO
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)      230 2023-08-03 19:45:19.000000 cospgd-0.1.1/cospgd.egg-info/SOURCES.txt
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)        1 2023-08-03 19:45:19.000000 cospgd-0.1.1/cospgd.egg-info/dependency_links.txt
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)       17 2023-08-03 19:45:19.000000 cospgd-0.1.1/cospgd.egg-info/requires.txt
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)        7 2023-08-03 19:45:19.000000 cospgd-0.1.1/cospgd.egg-info/top_level.txt
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)       38 2023-08-03 19:45:19.718332 cospgd-0.1.1/setup.cfg
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)     1207 2023-08-03 19:44:17.000000 cospgd-0.1.1/setup.py
```

### Comparing `cospgd-0.1.0/LICENSE.md` & `cospgd-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cospgd-0.1.0/PKG-INFO` & `cospgd-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cospgd
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for benchmarking adversarial robustness of pixel-wise prediction tasks.
 Home-page: https://github.com/shashankskagnihotri/cospgd
 Author: Shashank Agnihotri, Steffen Jung, Prof. Dr. Margret Keuper
 Author-email: shashanksagnihotri@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cospgd-0.1.0/README.md` & `cospgd-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cospgd-0.1.0/cospgd/attack_implementations.py` & `cospgd-0.1.1/cospgd/attack_implementations.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         )
         images = images + noise
         images = images.clamp(clamp_min, clamp_max)
         return images
     
     
     """
-    Scaling of the loss as implemeted by: 
+    Scaling of the pixel-wise loss as proposed by: 
     Gu, Jindong, et al. "Segpgd: An effective and efficient adversarial attack for evaluating and boosting segmentation robustness." 
     European Conference on Computer Vision. Cham: Springer Nature Switzerland, 2022.
 
     predictions: Float tensor of shape [batch size, channel, (image spatial resolution)]: Predictions made by the model
     labels: The ground truth/target labels, for semantic segmentation index tensor of the shape: [batch size, channel, (image spatial resolution)].
                                      for pixel-wise regression tasks, same shape as predictions
     loss: Float tensor: The loss between the predictions and the ground truth/target
@@ -233,15 +233,15 @@
                     lambda_t*loss
                 )
             ) / (predictions.shape[-2]*predictions.shape[-1])
         return loss
     
     
     """
-    Scaling of the loss as implemeted by: 
+    Scaling of the pixel-wise loss as implemeted by: 
     Agnihotri, Shashank, et al. "CosPGD: a unified white-box adversarial attack for pixel-wise prediction tasks." 
     arXiv preprint arXiv:2302.02213 (2023).
 
     predictions: Float tensor of shape [batch size, channel, (image spatial resolution)]: Predictions made by the model
     labels: The ground truth/target labels, for semantic segmentation index tensor of the shape: [batch size, channel, (image spatial resolution)].
                                      for pixel-wise regression tasks, same shape as predictions
     loss: Float tensor: The loss between the predictions and the ground truth/target
```

### Comparing `cospgd-0.1.0/cospgd.egg-info/PKG-INFO` & `cospgd-0.1.1/cospgd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cospgd
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for benchmarking adversarial robustness of pixel-wise prediction tasks.
 Home-page: https://github.com/shashankskagnihotri/cospgd
 Author: Shashank Agnihotri, Steffen Jung, Prof. Dr. Margret Keuper
 Author-email: shashanksagnihotri@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cospgd-0.1.0/setup.py` & `cospgd-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='cospgd',
-    version='0.1.0',    
+    version='0.1.1',    
     description='A tool for benchmarking adversarial robustness of pixel-wise prediction tasks.',
     url='https://github.com/shashankskagnihotri/cospgd',
     author='Shashank Agnihotri, Steffen Jung, Prof. Dr. Margret Keuper',
     author_email='shashanksagnihotri@gmail.com',
     license='MIT',
     packages=['cospgd'],
     install_requires=['torch>=1.7',
```

