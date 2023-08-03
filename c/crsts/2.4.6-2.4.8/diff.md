# Comparing `tmp/crsts-2.4.6.tar.gz` & `tmp/crsts-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crsts-2.4.6.tar", last modified: Thu Aug  3 05:51:37 2023, max compression
+gzip compressed data, was "dist/crsts-2.4.8.tar", last modified: Thu Aug  3 05:54:38 2023, max compression
```

## Comparing `crsts-2.4.6.tar` & `crsts-2.4.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bappy      (501) admin       (80)        0 2023-08-03 05:51:37.000000 crsts-2.4.6/
--rw-r--r--   0 bappy      (501) admin       (80)      376 2023-08-03 05:51:37.000000 crsts-2.4.6/PKG-INFO
-drwxr-xr-x   0 bappy      (501) admin       (80)        0 2023-08-03 05:51:37.000000 crsts-2.4.6/crsts/
--rw-r--r--   0 bappy      (501) admin       (80)       76 2021-08-30 02:59:14.000000 crsts-2.4.6/crsts/__init__.py
--rw-r--r--   0 bappy      (501) admin       (80)    23297 2023-08-03 05:51:30.000000 crsts-2.4.6/crsts/crsts.py
-drwxr-xr-x   0 bappy      (501) admin       (80)        0 2023-08-03 05:51:37.000000 crsts-2.4.6/crsts.egg-info/
--rw-r--r--   0 bappy      (501) admin       (80)      376 2023-08-03 05:51:37.000000 crsts-2.4.6/crsts.egg-info/PKG-INFO
--rw-r--r--   0 bappy      (501) admin       (80)      167 2023-08-03 05:51:37.000000 crsts-2.4.6/crsts.egg-info/SOURCES.txt
--rw-r--r--   0 bappy      (501) admin       (80)        6 2023-08-03 05:51:37.000000 crsts-2.4.6/crsts.egg-info/top_level.txt
--rw-r--r--   0 bappy      (501) admin       (80)        1 2023-08-03 05:51:37.000000 crsts-2.4.6/crsts.egg-info/dependency_links.txt
--rw-r--r--   0 bappy      (501) admin       (80)       48 2021-08-30 02:59:14.000000 crsts-2.4.6/README.md
--rw-r--r--   0 bappy      (501) admin       (80)      591 2023-08-03 05:51:30.000000 crsts-2.4.6/setup.py
--rw-r--r--   0 bappy      (501) admin       (80)       38 2023-08-03 05:51:37.000000 crsts-2.4.6/setup.cfg
+drwxr-xr-x   0 bappy      (501) admin       (80)        0 2023-08-03 05:54:38.000000 crsts-2.4.8/
+-rw-r--r--   0 bappy      (501) admin       (80)      376 2023-08-03 05:54:38.000000 crsts-2.4.8/PKG-INFO
+drwxr-xr-x   0 bappy      (501) admin       (80)        0 2023-08-03 05:54:38.000000 crsts-2.4.8/crsts/
+-rw-r--r--   0 bappy      (501) admin       (80)       76 2021-08-30 02:59:14.000000 crsts-2.4.8/crsts/__init__.py
+-rw-r--r--   0 bappy      (501) admin       (80)    23290 2023-08-03 05:54:35.000000 crsts-2.4.8/crsts/crsts.py
+drwxr-xr-x   0 bappy      (501) admin       (80)        0 2023-08-03 05:54:38.000000 crsts-2.4.8/crsts.egg-info/
+-rw-r--r--   0 bappy      (501) admin       (80)      376 2023-08-03 05:54:37.000000 crsts-2.4.8/crsts.egg-info/PKG-INFO
+-rw-r--r--   0 bappy      (501) admin       (80)      167 2023-08-03 05:54:37.000000 crsts-2.4.8/crsts.egg-info/SOURCES.txt
+-rw-r--r--   0 bappy      (501) admin       (80)        6 2023-08-03 05:54:37.000000 crsts-2.4.8/crsts.egg-info/top_level.txt
+-rw-r--r--   0 bappy      (501) admin       (80)        1 2023-08-03 05:54:37.000000 crsts-2.4.8/crsts.egg-info/dependency_links.txt
+-rw-r--r--   0 bappy      (501) admin       (80)       48 2021-08-30 02:59:14.000000 crsts-2.4.8/README.md
+-rw-r--r--   0 bappy      (501) admin       (80)      591 2023-08-03 05:54:35.000000 crsts-2.4.8/setup.py
+-rw-r--r--   0 bappy      (501) admin       (80)       38 2023-08-03 05:54:38.000000 crsts-2.4.8/setup.cfg
```

### Comparing `crsts-2.4.6/crsts/crsts.py` & `crsts-2.4.8/crsts/crsts.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,30 +75,30 @@
     cnt=[]
     for file_path in file_path_lst:
         cnt.extend(read_path(file_path))
     if shuffle:
         rand_shuffle(cnt)
     write2path(cnt,merge_file_path)
 
-def shuffle_pair_data(feat_path,label_path,new_file_suffix="shuffle"):
+def shuffle_pair_data(feat_path,label_path,new_file_suffix="_shuffle"):
     feat_data=read_path(feat_path)
     label_data=read_path(label_path)
     all_data=[]
     for index,f in enumerate(feat_data):
         all_data.append([f,label_data[index]])
     rand_shuffle(all_data)
 
     new_feat_data=[]
     new_label_data=[]
     for f in all_data:
         new_feat_data.append(f[0])
         new_label_data.append(f[1])
 
-    write2path(new_feat_data,feat_path+"_"+new_file_suffix)
-    write2path(new_label_data,label_path+"_"+new_file_suffix)
+    write2path(new_feat_data,feat_path+new_file_suffix)
+    write2path(new_label_data,label_path+new_file_suffix)
 
 def print_list(array,index=False,top_n=None):
     """ 打印list内容
             index - 是否打印索引
     """
     if not top_n:
         top_n=len(array)
```

### Comparing `crsts-2.4.6/setup.py` & `crsts-2.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="crsts",
-    version="2.4.6",
+    version="2.4.8",
     author="Chris Chen",
     author_email="wsywddr@163.com",
     description="This is my personal toolkit.",
     longe_description=long_description,
     longe_description_content_type="text/markdown",
     url="https://github.com/wsywddr",
     packages=setuptools.find_packages(),
```

