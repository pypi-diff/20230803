# Comparing `tmp/dustmaps-1.0.8.tar.gz` & `tmp/dustmaps-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dustmaps-1.0.8.tar", last modified: Thu Apr 22 09:17:18 2021, max compression
+gzip compressed data, was "dist/dustmaps-1.0.9.tar", last modified: Mon Aug 16 13:22:15 2021, max compression
```

## Comparing `dustmaps-1.0.8.tar` & `dustmaps-1.0.9.tar`

### file list

```diff
@@ -1,44 +1,42 @@
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2021-04-22 09:17:18.000000 dustmaps-1.0.8/
--rw-rw-r--   0 greg      (1000) greg      (1000)     5298 2021-04-22 09:13:35.000000 dustmaps-1.0.8/setup.py
--rw-r--r--   0 greg      (1000) greg      (1000)      108 2018-08-21 20:32:11.000000 dustmaps-1.0.8/MANIFEST.in
--rw-r--r--   0 greg      (1000) greg      (1000)    14931 2018-08-21 20:32:11.000000 dustmaps-1.0.8/LICENSE.txt
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2021-04-22 09:17:18.000000 dustmaps-1.0.8/dustmaps/
--rw-r--r--   0 greg      (1000) greg      (1000)     3656 2018-10-22 20:11:48.000000 dustmaps-1.0.8/dustmaps/pg2010.py
--rw-r--r--   0 greg      (1000) greg      (1000)     4476 2019-05-08 00:58:47.000000 dustmaps-1.0.8/dustmaps/leike_ensslin_2019.py
--rw-r--r--   0 greg      (1000) greg      (1000)    11786 2018-10-22 20:11:48.000000 dustmaps-1.0.8/dustmaps/json_serializers.py
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2021-04-22 09:17:18.000000 dustmaps-1.0.8/dustmaps/tests/
--rw-r--r--   0 greg      (1000) greg      (1000)     1290 2018-08-21 20:32:11.000000 dustmaps-1.0.8/dustmaps/tests/ned_output.json
--rw-r--r--   0 greg      (1000) greg      (1000)    13729 2019-05-08 00:58:47.000000 dustmaps-1.0.8/dustmaps/equirectangular_map.py
--rw-r--r--   0 greg      (1000) greg      (1000)    10094 2018-10-22 20:11:48.000000 dustmaps-1.0.8/dustmaps/chen2014.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1593 2018-08-21 20:32:11.000000 dustmaps-1.0.8/dustmaps/dustexceptions.py
--rw-r--r--   0 greg      (1000) greg      (1000)     5298 2020-10-05 14:22:59.000000 dustmaps-1.0.8/dustmaps/leike2020.py
--rw-r--r--   0 greg      (1000) greg      (1000)    13830 2019-02-21 23:12:36.000000 dustmaps-1.0.8/dustmaps/iphas.py
--rw-r--r--   0 greg      (1000) greg      (1000)     3128 2018-10-22 20:11:48.000000 dustmaps-1.0.8/dustmaps/lenz2017.py
--rw-r--r--   0 greg      (1000) greg      (1000)    12870 2018-10-22 20:11:48.000000 dustmaps-1.0.8/dustmaps/marshall.py
--rw-r--r--   0 greg      (1000) greg      (1000)     4673 2018-10-22 20:11:48.000000 dustmaps-1.0.8/dustmaps/unstructured_map.py
--rw-r--r--   0 greg      (1000) greg      (1000)    14866 2019-05-08 00:58:47.000000 dustmaps-1.0.8/dustmaps/fetch_utils.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     8939 2021-04-22 09:11:26.000000 dustmaps-1.0.8/dustmaps/planck.py
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2021-04-22 09:17:18.000000 dustmaps-1.0.8/dustmaps/data/
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2021-04-22 09:17:18.000000 dustmaps-1.0.8/dustmaps/data/bh/
--rw-r--r--   0 greg      (1000) greg      (1000)   396117 2018-08-21 20:32:11.000000 dustmaps-1.0.8/dustmaps/data/bh/bh.h5
--rw-r--r--   0 greg      (1000) greg      (1000)      848 2018-08-21 20:32:11.000000 dustmaps-1.0.8/dustmaps/__init__.py
--rw-r--r--   0 greg      (1000) greg      (1000)     5684 2018-10-22 14:26:04.000000 dustmaps-1.0.8/dustmaps/sfd.py
--rwxr-xr-x   0 greg      (1000) greg      (1000)    19981 2020-11-10 20:16:44.000000 dustmaps-1.0.8/dustmaps/map_base.py
--rw-r--r--   0 greg      (1000) greg      (1000)     5992 2021-01-25 13:13:32.000000 dustmaps-1.0.8/dustmaps/config.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1831 2021-01-25 13:13:32.000000 dustmaps-1.0.8/dustmaps/std_paths.py
--rw-r--r--   0 greg      (1000) greg      (1000)     3921 2019-05-08 00:58:47.000000 dustmaps-1.0.8/dustmaps/chen2018.py
--rw-r--r--   0 greg      (1000) greg      (1000)    26747 2020-11-10 12:39:24.000000 dustmaps-1.0.8/dustmaps/bayestar.py
--rw-r--r--   0 greg      (1000) greg      (1000)    13723 2019-02-28 00:11:15.000000 dustmaps-1.0.8/dustmaps/cartesian_map.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     4829 2021-04-22 09:11:26.000000 dustmaps-1.0.8/dustmaps/healpix_map.py
--rw-r--r--   0 greg      (1000) greg      (1000)     4508 2020-10-05 10:07:04.000000 dustmaps-1.0.8/dustmaps/leike_ensslin.py
--rw-r--r--   0 greg      (1000) greg      (1000)     7287 2018-08-21 20:32:11.000000 dustmaps-1.0.8/dustmaps/bh.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     4871 2021-04-22 09:11:26.000000 dustmaps-1.0.8/README.md
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2021-04-22 09:17:18.000000 dustmaps-1.0.8/dustmaps.egg-info/
--rw-r--r--   0 greg      (1000) greg      (1000)        1 2018-10-22 20:17:37.000000 dustmaps-1.0.8/dustmaps.egg-info/not-zip-safe
--rw-r--r--   0 greg      (1000) greg      (1000)       58 2021-04-22 09:17:17.000000 dustmaps-1.0.8/dustmaps.egg-info/requires.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      831 2021-04-22 09:17:17.000000 dustmaps-1.0.8/dustmaps.egg-info/SOURCES.txt
--rw-r--r--   0 greg      (1000) greg      (1000)     6543 2021-04-22 09:17:17.000000 dustmaps-1.0.8/dustmaps.egg-info/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)        1 2021-04-22 09:17:17.000000 dustmaps-1.0.8/dustmaps.egg-info/dependency_links.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        9 2021-04-22 09:17:17.000000 dustmaps-1.0.8/dustmaps.egg-info/top_level.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)     6543 2021-04-22 09:17:18.000000 dustmaps-1.0.8/PKG-INFO
--rw-rw-r--   0 greg      (1000) greg      (1000)       38 2021-04-22 09:17:18.000000 dustmaps-1.0.8/setup.cfg
+drwxrwxr-x   0 green    (10369) green    (10369)        0 2021-08-16 13:22:15.000000 dustmaps-1.0.9/
+-rw-rw-r--   0 green    (10369) green    (10369)       38 2021-08-16 13:22:15.000000 dustmaps-1.0.9/setup.cfg
+-rw-rw-r--   0 green    (10369) green    (10369)     5270 2021-08-16 13:22:15.000000 dustmaps-1.0.9/PKG-INFO
+drwxrwxr-x   0 green    (10369) green    (10369)        0 2021-08-16 13:22:15.000000 dustmaps-1.0.9/dustmaps/
+-rw-rw-r--   0 green    (10369) green    (10369)     3921 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/chen2018.py
+-rw-rw-r--   0 green    (10369) green    (10369)     1593 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/dustexceptions.py
+-rw-rw-r--   0 green    (10369) green    (10369)    12870 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/marshall.py
+-rw-rw-r--   0 green    (10369) green    (10369)      848 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/__init__.py
+-rw-rw-r--   0 green    (10369) green    (10369)    26747 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/bayestar.py
+-rw-rw-r--   0 green    (10369) green    (10369)     4476 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/leike_ensslin_2019.py
+-rw-rw-r--   0 green    (10369) green    (10369)     7287 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/bh.py
+-rw-rw-r--   0 green    (10369) green    (10369)     4829 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/healpix_map.py
+-rw-rw-r--   0 green    (10369) green    (10369)    14866 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/fetch_utils.py
+-rw-rw-r--   0 green    (10369) green    (10369)     5298 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/leike2020.py
+-rw-rw-r--   0 green    (10369) green    (10369)     5992 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/config.py
+-rw-rw-r--   0 green    (10369) green    (10369)     1831 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/std_paths.py
+-rw-rw-r--   0 green    (10369) green    (10369)     5684 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/sfd.py
+drwxrwxr-x   0 green    (10369) green    (10369)        0 2021-08-16 13:22:15.000000 dustmaps-1.0.9/dustmaps/tests/
+-rw-rw-r--   0 green    (10369) green    (10369)     1290 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/tests/ned_output.json
+-rw-rw-r--   0 green    (10369) green    (10369)    13729 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/equirectangular_map.py
+-rw-rw-r--   0 green    (10369) green    (10369)     8939 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/planck.py
+-rw-rw-r--   0 green    (10369) green    (10369)     3128 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/lenz2017.py
+-rw-rw-r--   0 green    (10369) green    (10369)    13830 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/iphas.py
+drwxrwxr-x   0 green    (10369) green    (10369)        0 2021-08-16 13:22:15.000000 dustmaps-1.0.9/dustmaps/data/
+drwxrwxr-x   0 green    (10369) green    (10369)        0 2021-08-16 13:22:15.000000 dustmaps-1.0.9/dustmaps/data/bh/
+-rw-rw-r--   0 green    (10369) green    (10369)   396117 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/data/bh/bh.h5
+-rw-rw-r--   0 green    (10369) green    (10369)    11786 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/json_serializers.py
+-rw-rw-r--   0 green    (10369) green    (10369)    10076 2021-08-16 13:19:24.000000 dustmaps-1.0.9/dustmaps/chen2014.py
+-rw-rw-r--   0 green    (10369) green    (10369)     4673 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/unstructured_map.py
+-rwxrwxr-x   0 green    (10369) green    (10369)    19981 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/map_base.py
+-rw-rw-r--   0 green    (10369) green    (10369)     3656 2021-07-17 19:48:43.000000 dustmaps-1.0.9/dustmaps/pg2010.py
+-rw-rw-r--   0 green    (10369) green    (10369)     5298 2021-08-16 13:19:24.000000 dustmaps-1.0.9/setup.py
+drwxrwxr-x   0 green    (10369) green    (10369)        0 2021-08-16 13:22:15.000000 dustmaps-1.0.9/dustmaps.egg-info/
+-rw-rw-r--   0 green    (10369) green    (10369)     5270 2021-08-16 13:22:15.000000 dustmaps-1.0.9/dustmaps.egg-info/PKG-INFO
+-rw-rw-r--   0 green    (10369) green    (10369)      779 2021-08-16 13:22:15.000000 dustmaps-1.0.9/dustmaps.egg-info/SOURCES.txt
+-rw-rw-r--   0 green    (10369) green    (10369)        9 2021-08-16 13:22:15.000000 dustmaps-1.0.9/dustmaps.egg-info/top_level.txt
+-rw-rw-r--   0 green    (10369) green    (10369)       58 2021-08-16 13:22:15.000000 dustmaps-1.0.9/dustmaps.egg-info/requires.txt
+-rw-rw-r--   0 green    (10369) green    (10369)        1 2021-08-16 13:22:15.000000 dustmaps-1.0.9/dustmaps.egg-info/not-zip-safe
+-rw-rw-r--   0 green    (10369) green    (10369)        1 2021-08-16 13:22:15.000000 dustmaps-1.0.9/dustmaps.egg-info/dependency_links.txt
+-rw-rw-r--   0 green    (10369) green    (10369)    14931 2021-07-17 19:48:43.000000 dustmaps-1.0.9/LICENSE.txt
+-rw-rw-r--   0 green    (10369) green    (10369)     4871 2021-07-17 19:48:43.000000 dustmaps-1.0.9/README.md
+-rw-rw-r--   0 green    (10369) green    (10369)      108 2021-07-17 19:48:43.000000 dustmaps-1.0.9/MANIFEST.in
```

### Comparing `dustmaps-1.0.8/setup.py` & `dustmaps-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,20 +149,20 @@
 def readme():
     with io.open('README.md', mode='r', encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='dustmaps',
-    version='1.0.8',
+    version='1.0.9',
     description='Uniform interface for multiple dust reddening maps.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/gregreen/dustmaps',
-    download_url='https://github.com/gregreen/dustmaps/archive/v1.0.8.tar.gz',
+    download_url='https://github.com/gregreen/dustmaps/archive/v1.0.9.tar.gz',
     author='Gregory M. Green',
     author_email='gregorymgreen@gmail.com',
     license='GPLv2',
     packages=['dustmaps'],
     install_requires=[
         'numpy',
         'scipy',
```

### Comparing `dustmaps-1.0.8/LICENSE.txt` & `dustmaps-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/pg2010.py` & `dustmaps-1.0.9/dustmaps/pg2010.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/leike_ensslin_2019.py` & `dustmaps-1.0.9/dustmaps/leike_ensslin_2019.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/json_serializers.py` & `dustmaps-1.0.9/dustmaps/json_serializers.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/tests/ned_output.json` & `dustmaps-1.0.9/dustmaps/tests/ned_output.json`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/equirectangular_map.py` & `dustmaps-1.0.9/dustmaps/equirectangular_map.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/chen2014.py` & `dustmaps-1.0.9/dustmaps/chen2014.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,15 @@
             overwritten, even if it appears to match. If ``False`` (the
             default), :obj:`fetch()` will attempt to determine if the dataset
             already exists. This determination is not 100\% robust against data
             corruption.
     """
 
     dest_dir = fname_pattern = os.path.join(data_dir(), 'chen2014')
-    url = 'http://lamost973.pku.edu.cn/site/Photometric-Extinctions-and-Distances/table2.dat'
+    url = 'https://paperdata.china-vo.org/diskec/extinmaps/chen2014map.dat'
     dat_fname = os.path.join(dest_dir, 'chen2014.dat')
     h5_fname = os.path.join(dest_dir, 'chen2014.h5')
     md5 = 'f8a2bc46d411c57ca4c76dc344e291f1'
 
     # Check if file already exists
     if not clobber:
         h5_size = 52768768 # Guess, in Bytes
```

### Comparing `dustmaps-1.0.8/dustmaps/dustexceptions.py` & `dustmaps-1.0.9/dustmaps/dustexceptions.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/leike2020.py` & `dustmaps-1.0.9/dustmaps/leike2020.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/iphas.py` & `dustmaps-1.0.9/dustmaps/iphas.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/lenz2017.py` & `dustmaps-1.0.9/dustmaps/lenz2017.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/marshall.py` & `dustmaps-1.0.9/dustmaps/marshall.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/unstructured_map.py` & `dustmaps-1.0.9/dustmaps/unstructured_map.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/fetch_utils.py` & `dustmaps-1.0.9/dustmaps/fetch_utils.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/planck.py` & `dustmaps-1.0.9/dustmaps/planck.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/data/bh/bh.h5` & `dustmaps-1.0.9/dustmaps/data/bh/bh.h5`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/__init__.py` & `dustmaps-1.0.9/dustmaps/__init__.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/sfd.py` & `dustmaps-1.0.9/dustmaps/sfd.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/map_base.py` & `dustmaps-1.0.9/dustmaps/map_base.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/config.py` & `dustmaps-1.0.9/dustmaps/config.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/std_paths.py` & `dustmaps-1.0.9/dustmaps/std_paths.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/chen2018.py` & `dustmaps-1.0.9/dustmaps/chen2018.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/bayestar.py` & `dustmaps-1.0.9/dustmaps/bayestar.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/healpix_map.py` & `dustmaps-1.0.9/dustmaps/healpix_map.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps/bh.py` & `dustmaps-1.0.9/dustmaps/bh.py`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/README.md` & `dustmaps-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dustmaps-1.0.8/dustmaps.egg-info/SOURCES.txt` & `dustmaps-1.0.9/dustmaps.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
 dustmaps/__init__.py
 dustmaps/bayestar.py
 dustmaps/bh.py
-dustmaps/cartesian_map.py
 dustmaps/chen2014.py
 dustmaps/chen2018.py
 dustmaps/config.py
 dustmaps/dustexceptions.py
 dustmaps/equirectangular_map.py
 dustmaps/fetch_utils.py
 dustmaps/healpix_map.py
 dustmaps/iphas.py
 dustmaps/json_serializers.py
 dustmaps/leike2020.py
-dustmaps/leike_ensslin.py
 dustmaps/leike_ensslin_2019.py
 dustmaps/lenz2017.py
 dustmaps/map_base.py
 dustmaps/marshall.py
 dustmaps/pg2010.py
 dustmaps/planck.py
 dustmaps/sfd.py
```

### Comparing `dustmaps-1.0.8/dustmaps.egg-info/PKG-INFO` & `dustmaps-1.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,173 +1,176 @@
 Metadata-Version: 2.1
 Name: dustmaps
-Version: 1.0.8
+Version: 1.0.9
 Summary: Uniform interface for multiple dust reddening maps.
 Home-page: https://github.com/gregreen/dustmaps
 Author: Gregory M. Green
 Author-email: gregorymgreen@gmail.com
 License: GPLv2
-Download-URL: https://github.com/gregreen/dustmaps/archive/v1.0.8.tar.gz
-Description: [![DOI](http://joss.theoj.org/papers/10.21105/joss.00695/status.svg)](https://doi.org/10.21105/joss.00695) [![DOI](https://zenodo.org/badge/59614814.svg)](https://zenodo.org/badge/latestdoi/59614814)
-        
-        dustmaps
-        ========
-        
-        The ``dustmaps`` package provides a uniform interface for dealing with a number
-        of 2D and 3D maps of interstellar dust reddening/extinction.
-        
-        Supported Dust Maps
-        -------------------
-        
-        The currently supported dust maps are:
-        
-        1. Burstein & Heiles (1982; BH'82)
-        2. Chen et al. (2014)
-        3. Green, Schlafly, Finkbeiner et al. (2015,2018,2019; Bayestar)
-        4. Marshall et al. (2006)
-        5. Planck Collaboration (2013)
-        6. Planck Collaboration (2016; GNILC)
-        7. Sale et al. (2014; IPHAS)
-        8. Schlegel, Finkbeiner & Davis (1998; SFD'98)
-        9. Lenz, Hensley & Doré (2017)
-        10. Peek & Graves (2010)
-        11. Leike & Enßlin (2019)
-        12. Leike, Glatzle & Enßlin (2020)
-        
-        To request addition of another dust map in this package, [file an issue on
-        GitHub](https://github.com/gregreen/dustmaps/issues), or submit a pull request.
-        
-        
-        Installation
-        ------------
-        
-        Download the repository from [GitHub](https://github.com/gregreen/dustmaps) and
-        then run:
-        
-            python setup.py install --large-data-dir=/path/where/you/want/large/data/files/stored
-        
-        Alternatively, you can use the Python package manager `pip`:
-        
-            pip install dustmaps
-        
-        
-        Getting the Data
-        ----------------
-        
-        To fetch the data for the SFD dust map, run:
-        
-            python setup.py fetch --map-name=sfd
-        
-        You can download the other dust maps by changing "sfd" to "planck",
-        "planckGNILC", "bayestar", "iphas", "marshall", "chen2014", "lenz2017",
-        "pg2010", "leikeensslin2019", "leike2020" or "bh".
-        
-        Alternatively, if you have used `pip` to install `dustmaps`, then you can
-        configure the data directory and download the data by opening up a python
-        interpreter and running:
-        
-            >>> from dustmaps.config import config
-            >>> config['data_dir'] = '/path/where/you/want/large/data/files/stored'
-            >>>
-            >>> import dustmaps.sfd
-            >>> dustmaps.sfd.fetch()
-            >>>
-            >>> import dustmaps.planck
-            >>> dustmaps.planck.fetch()
-            >>>
-            >>> import dustmaps.planck
-            >>> dustmaps.planck.fetch(which='GNILC')
-            >>>
-            >>> import dustmaps.bayestar
-            >>> dustmaps.bayestar.fetch()
-            >>>
-            >>> import dustmaps.iphas
-            >>> dustmaps.iphas.fetch()
-            >>>
-            >>> import dustmaps.marshall
-            >>> dustmaps.marshall.fetch()
-            >>>
-            >>> import dustmaps.chen2014
-            >>> dustmaps.chen2014.fetch()
-            >>>
-            >>> import dustmaps.lenz2017
-            >>> dustmaps.lenz2017.fetch()
-            >>>
-            >>> import dustmaps.pg2010
-            >>> dustmaps.pg2010.fetch()
-            >>>
-            >>> import dustmaps.leike_ensslin_2019
-            >>> dustmaps.leike_ensslin_2019.fetch()
-            >>>
-            >>> import dustmaps.leike2020
-            >>> dustmaps.leike2020.fetch()
-        
-        
-        Querying the Maps
-        -----------------
-        
-        Maps are queried using
-        [`astropy.coordinates.SkyCoord`](http://docs.astropy.org/en/stable/api/astropy.coordinates.SkyCoord.html#astropy.coordinates.SkyCoord)
-        objects. This means that any coordinate system supported by `astropy` can be
-        used as input. For example, we can query SFD'98 as follows:
-        
-            >>> from dustmaps.sfd import SFDQuery
-            >>> from astropy.coordinates import SkyCoord
-            >>>
-            >>> sfd = SFDQuery()
-            >>>
-            >>> c = SkyCoord(
-                    '05h00m00.00000s',
-                    '+30d00m00.0000s',
-                    frame='icrs')
-            >>> print sfd(c)
-            0.483961
-        
-        Above, we have used the ICRS coordinate system (the inputs are RA and Dec). We
-        can use other coordinate systems, such as Galactic coordinates, and we can
-        provide coordinate arrays. The following example uses both features:
-        
-            >>> c = SkyCoord(
-                    [75.00000000, 130.00000000],
-                    [-89.00000000, 10.00000000],
-                    frame='galactic',
-                    unit='deg')
-            >>> print sfd(c)
-            [ 0.0146584   0.97695869]
-        
-        
-        Documentation
-        -------------
-        
-        Read the full documentation at http://dustmaps.readthedocs.io/en/latest/.
-        
-        
-        Citation
-        --------
-        
-        If you make use of this software in a publication, please cite
-        [Green (2018) in The Journal of Open Source Software](https://doi.org/10.21105/joss.00695):
-        
-            @ARTICLE{2018JOSS....3..695M,
-                   author = {{Green}, {Gregory M.}},
-                    title = "{dustmaps: A Python interface for maps of interstellar dust}",
-                  journal = {The Journal of Open Source Software},
-                     year = "2018",
-                    month = "Jun",
-                   volume = {3},
-                   number = {26},
-                    pages = {695},
-                      doi = {10.21105/joss.00695},
-                   adsurl = {https://ui.adsabs.harvard.edu/abs/2018JOSS....3..695M},
-                  adsnote = {Provided by the SAO/NASA Astrophysics Data System}
-            }
-        
-        
-        Development
-        -----------
-        
-        Development of `dustmaps` takes place on GitHub, at
-        https://github.com/gregreen/dustmaps. Any bugs, feature requests, pull requests,
-        or other issues can be filed there. Contributions to the software are welcome.
-        
+Download-URL: https://github.com/gregreen/dustmaps/archive/v1.0.9.tar.gz
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![DOI](http://joss.theoj.org/papers/10.21105/joss.00695/status.svg)](https://doi.org/10.21105/joss.00695) [![DOI](https://zenodo.org/badge/59614814.svg)](https://zenodo.org/badge/latestdoi/59614814)
+
+dustmaps
+========
+
+The ``dustmaps`` package provides a uniform interface for dealing with a number
+of 2D and 3D maps of interstellar dust reddening/extinction.
+
+Supported Dust Maps
+-------------------
+
+The currently supported dust maps are:
+
+1. Burstein & Heiles (1982; BH'82)
+2. Chen et al. (2014)
+3. Green, Schlafly, Finkbeiner et al. (2015,2018,2019; Bayestar)
+4. Marshall et al. (2006)
+5. Planck Collaboration (2013)
+6. Planck Collaboration (2016; GNILC)
+7. Sale et al. (2014; IPHAS)
+8. Schlegel, Finkbeiner & Davis (1998; SFD'98)
+9. Lenz, Hensley & Doré (2017)
+10. Peek & Graves (2010)
+11. Leike & Enßlin (2019)
+12. Leike, Glatzle & Enßlin (2020)
+
+To request addition of another dust map in this package, [file an issue on
+GitHub](https://github.com/gregreen/dustmaps/issues), or submit a pull request.
+
+
+Installation
+------------
+
+Download the repository from [GitHub](https://github.com/gregreen/dustmaps) and
+then run:
+
+    python setup.py install --large-data-dir=/path/where/you/want/large/data/files/stored
+
+Alternatively, you can use the Python package manager `pip`:
+
+    pip install dustmaps
+
+
+Getting the Data
+----------------
+
+To fetch the data for the SFD dust map, run:
+
+    python setup.py fetch --map-name=sfd
+
+You can download the other dust maps by changing "sfd" to "planck",
+"planckGNILC", "bayestar", "iphas", "marshall", "chen2014", "lenz2017",
+"pg2010", "leikeensslin2019", "leike2020" or "bh".
+
+Alternatively, if you have used `pip` to install `dustmaps`, then you can
+configure the data directory and download the data by opening up a python
+interpreter and running:
+
+    >>> from dustmaps.config import config
+    >>> config['data_dir'] = '/path/where/you/want/large/data/files/stored'
+    >>>
+    >>> import dustmaps.sfd
+    >>> dustmaps.sfd.fetch()
+    >>>
+    >>> import dustmaps.planck
+    >>> dustmaps.planck.fetch()
+    >>>
+    >>> import dustmaps.planck
+    >>> dustmaps.planck.fetch(which='GNILC')
+    >>>
+    >>> import dustmaps.bayestar
+    >>> dustmaps.bayestar.fetch()
+    >>>
+    >>> import dustmaps.iphas
+    >>> dustmaps.iphas.fetch()
+    >>>
+    >>> import dustmaps.marshall
+    >>> dustmaps.marshall.fetch()
+    >>>
+    >>> import dustmaps.chen2014
+    >>> dustmaps.chen2014.fetch()
+    >>>
+    >>> import dustmaps.lenz2017
+    >>> dustmaps.lenz2017.fetch()
+    >>>
+    >>> import dustmaps.pg2010
+    >>> dustmaps.pg2010.fetch()
+    >>>
+    >>> import dustmaps.leike_ensslin_2019
+    >>> dustmaps.leike_ensslin_2019.fetch()
+    >>>
+    >>> import dustmaps.leike2020
+    >>> dustmaps.leike2020.fetch()
+
+
+Querying the Maps
+-----------------
+
+Maps are queried using
+[`astropy.coordinates.SkyCoord`](http://docs.astropy.org/en/stable/api/astropy.coordinates.SkyCoord.html#astropy.coordinates.SkyCoord)
+objects. This means that any coordinate system supported by `astropy` can be
+used as input. For example, we can query SFD'98 as follows:
+
+    >>> from dustmaps.sfd import SFDQuery
+    >>> from astropy.coordinates import SkyCoord
+    >>>
+    >>> sfd = SFDQuery()
+    >>>
+    >>> c = SkyCoord(
+            '05h00m00.00000s',
+            '+30d00m00.0000s',
+            frame='icrs')
+    >>> print sfd(c)
+    0.483961
+
+Above, we have used the ICRS coordinate system (the inputs are RA and Dec). We
+can use other coordinate systems, such as Galactic coordinates, and we can
+provide coordinate arrays. The following example uses both features:
+
+    >>> c = SkyCoord(
+            [75.00000000, 130.00000000],
+            [-89.00000000, 10.00000000],
+            frame='galactic',
+            unit='deg')
+    >>> print sfd(c)
+    [ 0.0146584   0.97695869]
+
+
+Documentation
+-------------
+
+Read the full documentation at http://dustmaps.readthedocs.io/en/latest/.
+
+
+Citation
+--------
+
+If you make use of this software in a publication, please cite
+[Green (2018) in The Journal of Open Source Software](https://doi.org/10.21105/joss.00695):
+
+    @ARTICLE{2018JOSS....3..695M,
+           author = {{Green}, {Gregory M.}},
+            title = "{dustmaps: A Python interface for maps of interstellar dust}",
+          journal = {The Journal of Open Source Software},
+             year = "2018",
+            month = "Jun",
+           volume = {3},
+           number = {26},
+            pages = {695},
+              doi = {10.21105/joss.00695},
+           adsurl = {https://ui.adsabs.harvard.edu/abs/2018JOSS....3..695M},
+          adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+    }
+
+
+Development
+-----------
+
+Development of `dustmaps` takes place on GitHub, at
+https://github.com/gregreen/dustmaps. Any bugs, feature requests, pull requests,
+or other issues can be filed there. Contributions to the software are welcome.
+
+
```

### Comparing `dustmaps-1.0.8/PKG-INFO` & `dustmaps-1.0.9/dustmaps.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,173 +1,176 @@
 Metadata-Version: 2.1
 Name: dustmaps
-Version: 1.0.8
+Version: 1.0.9
 Summary: Uniform interface for multiple dust reddening maps.
 Home-page: https://github.com/gregreen/dustmaps
 Author: Gregory M. Green
 Author-email: gregorymgreen@gmail.com
 License: GPLv2
-Download-URL: https://github.com/gregreen/dustmaps/archive/v1.0.8.tar.gz
-Description: [![DOI](http://joss.theoj.org/papers/10.21105/joss.00695/status.svg)](https://doi.org/10.21105/joss.00695) [![DOI](https://zenodo.org/badge/59614814.svg)](https://zenodo.org/badge/latestdoi/59614814)
-        
-        dustmaps
-        ========
-        
-        The ``dustmaps`` package provides a uniform interface for dealing with a number
-        of 2D and 3D maps of interstellar dust reddening/extinction.
-        
-        Supported Dust Maps
-        -------------------
-        
-        The currently supported dust maps are:
-        
-        1. Burstein & Heiles (1982; BH'82)
-        2. Chen et al. (2014)
-        3. Green, Schlafly, Finkbeiner et al. (2015,2018,2019; Bayestar)
-        4. Marshall et al. (2006)
-        5. Planck Collaboration (2013)
-        6. Planck Collaboration (2016; GNILC)
-        7. Sale et al. (2014; IPHAS)
-        8. Schlegel, Finkbeiner & Davis (1998; SFD'98)
-        9. Lenz, Hensley & Doré (2017)
-        10. Peek & Graves (2010)
-        11. Leike & Enßlin (2019)
-        12. Leike, Glatzle & Enßlin (2020)
-        
-        To request addition of another dust map in this package, [file an issue on
-        GitHub](https://github.com/gregreen/dustmaps/issues), or submit a pull request.
-        
-        
-        Installation
-        ------------
-        
-        Download the repository from [GitHub](https://github.com/gregreen/dustmaps) and
-        then run:
-        
-            python setup.py install --large-data-dir=/path/where/you/want/large/data/files/stored
-        
-        Alternatively, you can use the Python package manager `pip`:
-        
-            pip install dustmaps
-        
-        
-        Getting the Data
-        ----------------
-        
-        To fetch the data for the SFD dust map, run:
-        
-            python setup.py fetch --map-name=sfd
-        
-        You can download the other dust maps by changing "sfd" to "planck",
-        "planckGNILC", "bayestar", "iphas", "marshall", "chen2014", "lenz2017",
-        "pg2010", "leikeensslin2019", "leike2020" or "bh".
-        
-        Alternatively, if you have used `pip` to install `dustmaps`, then you can
-        configure the data directory and download the data by opening up a python
-        interpreter and running:
-        
-            >>> from dustmaps.config import config
-            >>> config['data_dir'] = '/path/where/you/want/large/data/files/stored'
-            >>>
-            >>> import dustmaps.sfd
-            >>> dustmaps.sfd.fetch()
-            >>>
-            >>> import dustmaps.planck
-            >>> dustmaps.planck.fetch()
-            >>>
-            >>> import dustmaps.planck
-            >>> dustmaps.planck.fetch(which='GNILC')
-            >>>
-            >>> import dustmaps.bayestar
-            >>> dustmaps.bayestar.fetch()
-            >>>
-            >>> import dustmaps.iphas
-            >>> dustmaps.iphas.fetch()
-            >>>
-            >>> import dustmaps.marshall
-            >>> dustmaps.marshall.fetch()
-            >>>
-            >>> import dustmaps.chen2014
-            >>> dustmaps.chen2014.fetch()
-            >>>
-            >>> import dustmaps.lenz2017
-            >>> dustmaps.lenz2017.fetch()
-            >>>
-            >>> import dustmaps.pg2010
-            >>> dustmaps.pg2010.fetch()
-            >>>
-            >>> import dustmaps.leike_ensslin_2019
-            >>> dustmaps.leike_ensslin_2019.fetch()
-            >>>
-            >>> import dustmaps.leike2020
-            >>> dustmaps.leike2020.fetch()
-        
-        
-        Querying the Maps
-        -----------------
-        
-        Maps are queried using
-        [`astropy.coordinates.SkyCoord`](http://docs.astropy.org/en/stable/api/astropy.coordinates.SkyCoord.html#astropy.coordinates.SkyCoord)
-        objects. This means that any coordinate system supported by `astropy` can be
-        used as input. For example, we can query SFD'98 as follows:
-        
-            >>> from dustmaps.sfd import SFDQuery
-            >>> from astropy.coordinates import SkyCoord
-            >>>
-            >>> sfd = SFDQuery()
-            >>>
-            >>> c = SkyCoord(
-                    '05h00m00.00000s',
-                    '+30d00m00.0000s',
-                    frame='icrs')
-            >>> print sfd(c)
-            0.483961
-        
-        Above, we have used the ICRS coordinate system (the inputs are RA and Dec). We
-        can use other coordinate systems, such as Galactic coordinates, and we can
-        provide coordinate arrays. The following example uses both features:
-        
-            >>> c = SkyCoord(
-                    [75.00000000, 130.00000000],
-                    [-89.00000000, 10.00000000],
-                    frame='galactic',
-                    unit='deg')
-            >>> print sfd(c)
-            [ 0.0146584   0.97695869]
-        
-        
-        Documentation
-        -------------
-        
-        Read the full documentation at http://dustmaps.readthedocs.io/en/latest/.
-        
-        
-        Citation
-        --------
-        
-        If you make use of this software in a publication, please cite
-        [Green (2018) in The Journal of Open Source Software](https://doi.org/10.21105/joss.00695):
-        
-            @ARTICLE{2018JOSS....3..695M,
-                   author = {{Green}, {Gregory M.}},
-                    title = "{dustmaps: A Python interface for maps of interstellar dust}",
-                  journal = {The Journal of Open Source Software},
-                     year = "2018",
-                    month = "Jun",
-                   volume = {3},
-                   number = {26},
-                    pages = {695},
-                      doi = {10.21105/joss.00695},
-                   adsurl = {https://ui.adsabs.harvard.edu/abs/2018JOSS....3..695M},
-                  adsnote = {Provided by the SAO/NASA Astrophysics Data System}
-            }
-        
-        
-        Development
-        -----------
-        
-        Development of `dustmaps` takes place on GitHub, at
-        https://github.com/gregreen/dustmaps. Any bugs, feature requests, pull requests,
-        or other issues can be filed there. Contributions to the software are welcome.
-        
+Download-URL: https://github.com/gregreen/dustmaps/archive/v1.0.9.tar.gz
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![DOI](http://joss.theoj.org/papers/10.21105/joss.00695/status.svg)](https://doi.org/10.21105/joss.00695) [![DOI](https://zenodo.org/badge/59614814.svg)](https://zenodo.org/badge/latestdoi/59614814)
+
+dustmaps
+========
+
+The ``dustmaps`` package provides a uniform interface for dealing with a number
+of 2D and 3D maps of interstellar dust reddening/extinction.
+
+Supported Dust Maps
+-------------------
+
+The currently supported dust maps are:
+
+1. Burstein & Heiles (1982; BH'82)
+2. Chen et al. (2014)
+3. Green, Schlafly, Finkbeiner et al. (2015,2018,2019; Bayestar)
+4. Marshall et al. (2006)
+5. Planck Collaboration (2013)
+6. Planck Collaboration (2016; GNILC)
+7. Sale et al. (2014; IPHAS)
+8. Schlegel, Finkbeiner & Davis (1998; SFD'98)
+9. Lenz, Hensley & Doré (2017)
+10. Peek & Graves (2010)
+11. Leike & Enßlin (2019)
+12. Leike, Glatzle & Enßlin (2020)
+
+To request addition of another dust map in this package, [file an issue on
+GitHub](https://github.com/gregreen/dustmaps/issues), or submit a pull request.
+
+
+Installation
+------------
+
+Download the repository from [GitHub](https://github.com/gregreen/dustmaps) and
+then run:
+
+    python setup.py install --large-data-dir=/path/where/you/want/large/data/files/stored
+
+Alternatively, you can use the Python package manager `pip`:
+
+    pip install dustmaps
+
+
+Getting the Data
+----------------
+
+To fetch the data for the SFD dust map, run:
+
+    python setup.py fetch --map-name=sfd
+
+You can download the other dust maps by changing "sfd" to "planck",
+"planckGNILC", "bayestar", "iphas", "marshall", "chen2014", "lenz2017",
+"pg2010", "leikeensslin2019", "leike2020" or "bh".
+
+Alternatively, if you have used `pip` to install `dustmaps`, then you can
+configure the data directory and download the data by opening up a python
+interpreter and running:
+
+    >>> from dustmaps.config import config
+    >>> config['data_dir'] = '/path/where/you/want/large/data/files/stored'
+    >>>
+    >>> import dustmaps.sfd
+    >>> dustmaps.sfd.fetch()
+    >>>
+    >>> import dustmaps.planck
+    >>> dustmaps.planck.fetch()
+    >>>
+    >>> import dustmaps.planck
+    >>> dustmaps.planck.fetch(which='GNILC')
+    >>>
+    >>> import dustmaps.bayestar
+    >>> dustmaps.bayestar.fetch()
+    >>>
+    >>> import dustmaps.iphas
+    >>> dustmaps.iphas.fetch()
+    >>>
+    >>> import dustmaps.marshall
+    >>> dustmaps.marshall.fetch()
+    >>>
+    >>> import dustmaps.chen2014
+    >>> dustmaps.chen2014.fetch()
+    >>>
+    >>> import dustmaps.lenz2017
+    >>> dustmaps.lenz2017.fetch()
+    >>>
+    >>> import dustmaps.pg2010
+    >>> dustmaps.pg2010.fetch()
+    >>>
+    >>> import dustmaps.leike_ensslin_2019
+    >>> dustmaps.leike_ensslin_2019.fetch()
+    >>>
+    >>> import dustmaps.leike2020
+    >>> dustmaps.leike2020.fetch()
+
+
+Querying the Maps
+-----------------
+
+Maps are queried using
+[`astropy.coordinates.SkyCoord`](http://docs.astropy.org/en/stable/api/astropy.coordinates.SkyCoord.html#astropy.coordinates.SkyCoord)
+objects. This means that any coordinate system supported by `astropy` can be
+used as input. For example, we can query SFD'98 as follows:
+
+    >>> from dustmaps.sfd import SFDQuery
+    >>> from astropy.coordinates import SkyCoord
+    >>>
+    >>> sfd = SFDQuery()
+    >>>
+    >>> c = SkyCoord(
+            '05h00m00.00000s',
+            '+30d00m00.0000s',
+            frame='icrs')
+    >>> print sfd(c)
+    0.483961
+
+Above, we have used the ICRS coordinate system (the inputs are RA and Dec). We
+can use other coordinate systems, such as Galactic coordinates, and we can
+provide coordinate arrays. The following example uses both features:
+
+    >>> c = SkyCoord(
+            [75.00000000, 130.00000000],
+            [-89.00000000, 10.00000000],
+            frame='galactic',
+            unit='deg')
+    >>> print sfd(c)
+    [ 0.0146584   0.97695869]
+
+
+Documentation
+-------------
+
+Read the full documentation at http://dustmaps.readthedocs.io/en/latest/.
+
+
+Citation
+--------
+
+If you make use of this software in a publication, please cite
+[Green (2018) in The Journal of Open Source Software](https://doi.org/10.21105/joss.00695):
+
+    @ARTICLE{2018JOSS....3..695M,
+           author = {{Green}, {Gregory M.}},
+            title = "{dustmaps: A Python interface for maps of interstellar dust}",
+          journal = {The Journal of Open Source Software},
+             year = "2018",
+            month = "Jun",
+           volume = {3},
+           number = {26},
+            pages = {695},
+              doi = {10.21105/joss.00695},
+           adsurl = {https://ui.adsabs.harvard.edu/abs/2018JOSS....3..695M},
+          adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+    }
+
+
+Development
+-----------
+
+Development of `dustmaps` takes place on GitHub, at
+https://github.com/gregreen/dustmaps. Any bugs, feature requests, pull requests,
+or other issues can be filed there. Contributions to the software are welcome.
+
+
```

