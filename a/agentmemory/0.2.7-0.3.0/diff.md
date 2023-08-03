# Comparing `tmp/agentmemory-0.2.7.tar.gz` & `tmp/agentmemory-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentmemory-0.2.7.tar", last modified: Tue Jul 18 13:44:27 2023, max compression
+gzip compressed data, was "agentmemory-0.3.0.tar", last modified: Thu Aug  3 07:36:11 2023, max compression
```

## Comparing `agentmemory-0.2.7.tar` & `agentmemory-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-18 13:44:27.321830 agentmemory-0.2.7/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.2.7/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)    11200 2023-07-18 13:44:27.321605 agentmemory-0.2.7/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)    10642 2023-07-18 13:18:07.000000 agentmemory-0.2.7/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-18 13:44:27.318996 agentmemory-0.2.7/agentmemory/
--rw-r--r--   0 shawwalters   (501) staff       (20)      881 2023-07-18 13:44:19.000000 agentmemory-0.2.7/agentmemory/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)    24359 2023-07-18 13:20:57.000000 agentmemory-0.2.7/agentmemory/main.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-18 13:44:27.321296 agentmemory-0.2.7/agentmemory.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)    11200 2023-07-18 13:44:27.000000 agentmemory-0.2.7/agentmemory.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      244 2023-07-18 13:44:27.000000 agentmemory-0.2.7/agentmemory.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-18 13:44:27.000000 agentmemory-0.2.7/agentmemory.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-18 13:44:27.000000 agentmemory-0.2.7/agentmemory.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-18 13:44:27.000000 agentmemory-0.2.7/agentmemory.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-18 13:44:27.321878 agentmemory-0.2.7/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1267 2023-07-18 13:44:19.000000 agentmemory-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:36:11.034008 agentmemory-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 07:35:56.000000 agentmemory-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-08-03 07:36:11.034008 agentmemory-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14750 2023-08-03 07:35:56.000000 agentmemory-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:36:11.034008 agentmemory-0.3.0/agentmemory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-03 07:35:56.000000 agentmemory-0.3.0/agentmemory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-03 07:35:56.000000 agentmemory-0.3.0/agentmemory/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-08-03 07:35:56.000000 agentmemory-0.3.0/agentmemory/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-08-03 07:35:56.000000 agentmemory-0.3.0/agentmemory/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-08-03 07:35:56.000000 agentmemory-0.3.0/agentmemory/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-08-03 07:35:56.000000 agentmemory-0.3.0/agentmemory/persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:36:11.034008 agentmemory-0.3.0/agentmemory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-08-03 07:36:11.000000 agentmemory-0.3.0/agentmemory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-03 07:36:11.000000 agentmemory-0.3.0/agentmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:36:11.000000 agentmemory-0.3.0/agentmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 07:36:11.000000 agentmemory-0.3.0/agentmemory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 07:36:11.000000 agentmemory-0.3.0/agentmemory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:36:11.034008 agentmemory-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-03 07:35:56.000000 agentmemory-0.3.0/setup.py
```

### Comparing `agentmemory-0.2.7/LICENSE` & `agentmemory-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agentmemory-0.2.7/setup.py` & `agentmemory-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,27 +9,27 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='agentmemory',
-    version='0.2.7',
+    version='0.3.0',
     description='Easy-to-use agent memory, powered by chromadb',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
-    url='https://github.com/lalalune/agentmemory',
+    url='https://github.com/AutonomousResearchGroup/agentmemory',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
     packages=['agentmemory'],
-    install_requires=['chromadb'],
+    install_requires=['chromadb', 'agentlogger'],
     readme = "README.md",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',  
         'Operating System :: POSIX :: Linux',        
         'Programming Language :: Python :: 3',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows'
     ],
```

