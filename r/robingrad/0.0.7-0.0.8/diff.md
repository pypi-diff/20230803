# Comparing `tmp/robingrad-0.0.7.tar.gz` & `tmp/robingrad-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robingrad-0.0.7.tar", last modified: Fri Jul 28 16:36:28 2023, max compression
+gzip compressed data, was "robingrad-0.0.8.tar", last modified: Mon Jul 31 15:51:32 2023, max compression
```

## Comparing `robingrad-0.0.7.tar` & `robingrad-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-28 16:36:28.741640 robingrad-0.0.7/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-07-11 17:52:34.000000 robingrad-0.0.7/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2950 2023-07-28 16:36:28.741373 robingrad-0.0.7/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1289 2023-07-28 10:49:50.000000 robingrad-0.0.7/README.md
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      694 2023-07-28 10:49:39.000000 robingrad-0.0.7/pyproject.toml
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-28 16:36:28.736558 robingrad-0.0.7/robingrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-07-28 10:49:45.000000 robingrad-0.0.7/robingrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-07-12 20:52:44.000000 robingrad-0.0.7/robingrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     6324 2023-07-28 16:35:35.000000 robingrad-0.0.7/robingrad/lab.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-28 16:36:28.739935 robingrad-0.0.7/robingrad/nn/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      448 2023-07-24 22:02:33.000000 robingrad-0.0.7/robingrad/nn/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      244 2023-07-24 22:08:46.000000 robingrad-0.0.7/robingrad/nn/loss.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1564 2023-07-20 13:31:06.000000 robingrad-0.0.7/robingrad/optim.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1384 2023-07-15 12:31:49.000000 robingrad-0.0.7/robingrad/state.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11792 2023-07-28 16:35:53.000000 robingrad-0.0.7/robingrad/tensor.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-28 16:36:28.738452 robingrad-0.0.7/robingrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2950 2023-07-28 16:36:28.000000 robingrad-0.0.7/robingrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      379 2023-07-28 16:36:28.000000 robingrad-0.0.7/robingrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-07-28 16:36:28.000000 robingrad-0.0.7/robingrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       15 2023-07-28 16:36:28.000000 robingrad-0.0.7/robingrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       10 2023-07-28 16:36:28.000000 robingrad-0.0.7/robingrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-07-28 16:36:28.741718 robingrad-0.0.7/setup.cfg
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-28 16:36:28.740817 robingrad-0.0.7/tests/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9043 2023-07-28 13:50:02.000000 robingrad-0.0.7/tests/test_tensor.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-31 15:51:32.435145 robingrad-0.0.8/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-07-11 17:52:34.000000 robingrad-0.0.8/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2950 2023-07-31 15:51:32.434647 robingrad-0.0.8/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1289 2023-07-31 15:46:30.000000 robingrad-0.0.8/README.md
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      694 2023-07-31 15:46:24.000000 robingrad-0.0.8/pyproject.toml
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-31 15:51:32.429498 robingrad-0.0.8/robingrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-07-31 15:46:20.000000 robingrad-0.0.8/robingrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-07-12 20:52:44.000000 robingrad-0.0.8/robingrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     6339 2023-07-31 10:39:23.000000 robingrad-0.0.8/robingrad/lab.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-31 15:51:32.433450 robingrad-0.0.8/robingrad/nn/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      457 2023-07-31 15:51:19.000000 robingrad-0.0.8/robingrad/nn/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      477 2023-07-31 15:45:48.000000 robingrad-0.0.8/robingrad/nn/loss.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1564 2023-07-20 13:31:06.000000 robingrad-0.0.8/robingrad/optim.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1384 2023-07-15 12:31:49.000000 robingrad-0.0.8/robingrad/state.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11792 2023-07-28 16:35:53.000000 robingrad-0.0.8/robingrad/tensor.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-31 15:51:32.431912 robingrad-0.0.8/robingrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2950 2023-07-31 15:51:32.000000 robingrad-0.0.8/robingrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      379 2023-07-31 15:51:32.000000 robingrad-0.0.8/robingrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-07-31 15:51:32.000000 robingrad-0.0.8/robingrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       15 2023-07-31 15:51:32.000000 robingrad-0.0.8/robingrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       10 2023-07-31 15:51:32.000000 robingrad-0.0.8/robingrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-07-31 15:51:32.435321 robingrad-0.0.8/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-31 15:51:32.434018 robingrad-0.0.8/tests/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9043 2023-07-28 13:50:02.000000 robingrad-0.0.8/tests/test_tensor.py
```

### Comparing `robingrad-0.0.7/LICENSE` & `robingrad-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.7/PKG-INFO` & `robingrad-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robingrad
-Version: 0.0.7
+Version: 0.0.8
 Summary: Something between Tinygrad and Micrograd
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2023 Marco Salvalaggio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -32,15 +32,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.7
+pip install robingrad==0.0.8
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
```

### Comparing `robingrad-0.0.7/README.md` & `robingrad-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.7
+pip install robingrad==0.0.8
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
```

### Comparing `robingrad-0.0.7/pyproject.toml` & `robingrad-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robingrad"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Something between Tinygrad and Micrograd"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `robingrad-0.0.7/robingrad/graph.py` & `robingrad-0.0.8/robingrad/graph.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.7/robingrad/lab.py` & `robingrad-0.0.8/robingrad/lab.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,16 @@
 a = torch.full((5,1), 3., requires_grad=True)
 b = torch.ones((1,1), requires_grad=True)
 c = b * a
 loss = c.sum()
 loss.backward()
 print(a.grad)
 print(b.grad)
+print(c.grad)
 # res_torch_1 = a.grad.numpy().tolist()
 # res_torch_2 = b.grad.numpy().tolist()
 
 # print(res_robin_1)
 # print(res_robin_2)
 # print('\nTORCH')
 # print(res_torch_1)
-# print(res_torch_2)
+# print(res_torch_2)
```

### Comparing `robingrad-0.0.7/robingrad/optim.py` & `robingrad-0.0.8/robingrad/optim.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.7/robingrad/state.py` & `robingrad-0.0.8/robingrad/state.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.7/robingrad/tensor.py` & `robingrad-0.0.8/robingrad/tensor.py`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.7/robingrad.egg-info/PKG-INFO` & `robingrad-0.0.8/robingrad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robingrad
-Version: 0.0.7
+Version: 0.0.8
 Summary: Something between Tinygrad and Micrograd
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2023 Marco Salvalaggio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -32,15 +32,15 @@
 
 
 ## Installation
 
 To install the current release,
 
 ```console
-pip install robingrad==0.0.7
+pip install robingrad==0.0.8
 ```
 
 From source
 
 ```console
 git clone https://github.com/marcosalvalaggio/robingrad.git
 cd robingrad
```

### Comparing `robingrad-0.0.7/tests/test_tensor.py` & `robingrad-0.0.8/tests/test_tensor.py`

 * *Files identical despite different names*

