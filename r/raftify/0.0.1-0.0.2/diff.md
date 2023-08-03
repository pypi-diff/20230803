# Comparing `tmp/raftify-0.0.1.tar.gz` & `tmp/raftify-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raftify-0.0.1.tar", last modified: Thu Aug  3 08:05:20 2023, max compression
+gzip compressed data, was "raftify-0.0.2.tar", last modified: Thu Aug  3 08:15:03 2023, max compression
```

## Comparing `raftify-0.0.1.tar` & `raftify-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 jopemachine   (501) staff       (20)        0 2023-08-03 08:05:20.116851 raftify-0.0.1/
--rw-r--r--   0 jopemachine   (501) staff       (20)    10349 2023-07-31 06:47:59.000000 raftify-0.0.1/LICENSE
--rw-r--r--   0 jopemachine   (501) staff       (20)      355 2023-08-03 08:05:20.116690 raftify-0.0.1/PKG-INFO
--rw-r--r--   0 jopemachine   (501) staff       (20)     4467 2023-08-03 04:04:47.000000 raftify-0.0.1/README.md
--rw-r--r--   0 jopemachine   (501) staff       (20)      203 2023-08-03 04:04:47.000000 raftify-0.0.1/pyproject.toml
-drwxr-xr-x   0 jopemachine   (501) staff       (20)        0 2023-08-03 08:05:20.114384 raftify-0.0.1/raftify/
--rw-r--r--   0 jopemachine   (501) staff       (20)        6 2023-07-31 06:54:36.000000 raftify-0.0.1/raftify/VERSION
--rw-r--r--   0 jopemachine   (501) staff       (20)      679 2023-07-31 06:54:36.000000 raftify-0.0.1/raftify/__init__.py
--rw-r--r--   0 jopemachine   (501) staff       (20)       86 2023-07-31 06:54:36.000000 raftify-0.0.1/raftify/error.py
--rw-r--r--   0 jopemachine   (501) staff       (20)      368 2023-07-31 06:54:36.000000 raftify-0.0.1/raftify/fsm.py
--rw-r--r--   0 jopemachine   (501) staff       (20)    10934 2023-07-31 06:54:36.000000 raftify-0.0.1/raftify/lmdb.py
--rw-r--r--   0 jopemachine   (501) staff       (20)     2828 2023-07-31 07:10:41.000000 raftify-0.0.1/raftify/mailbox.py
--rw-r--r--   0 jopemachine   (501) staff       (20)     1408 2023-08-03 04:08:50.000000 raftify-0.0.1/raftify/message_sender.py
--rw-r--r--   0 jopemachine   (501) staff       (20)     7907 2023-07-31 06:55:11.000000 raftify-0.0.1/raftify/pb_adapter.py
-drwxr-xr-x   0 jopemachine   (501) staff       (20)        0 2023-08-03 08:05:20.116339 raftify-0.0.1/raftify/protos/
--rw-r--r--   0 jopemachine   (501) staff       (20)     5208 2023-07-31 06:54:36.000000 raftify-0.0.1/raftify/protos/eraftpb_pb2.py
--rw-r--r--   0 jopemachine   (501) staff       (20)      173 2023-07-31 06:54:36.000000 raftify-0.0.1/raftify/protos/eraftpb_pb2_grpc.py
--rw-r--r--   0 jopemachine   (501) staff       (20)     2859 2023-07-31 06:54:36.000000 raftify-0.0.1/raftify/protos/raft_service_pb2.py
--rw-r--r--   0 jopemachine   (501) staff       (20)     7331 2023-07-31 06:54:36.000000 raftify-0.0.1/raftify/protos/raft_service_pb2_grpc.py
--rw-r--r--   0 jopemachine   (501) staff       (20)     2551 2023-07-31 06:55:04.000000 raftify-0.0.1/raftify/raft_client.py
--rw-r--r--   0 jopemachine   (501) staff       (20)     4693 2023-08-03 04:04:47.000000 raftify-0.0.1/raftify/raft_facade.py
--rw-r--r--   0 jopemachine   (501) staff       (20)    14379 2023-08-03 06:39:02.000000 raftify-0.0.1/raftify/raft_node.py
--rw-r--r--   0 jopemachine   (501) staff       (20)     1425 2023-07-31 06:55:16.000000 raftify-0.0.1/raftify/raft_server.py
--rw-r--r--   0 jopemachine   (501) staff       (20)     3621 2023-07-31 06:55:21.000000 raftify-0.0.1/raftify/raft_service.py
--rw-r--r--   0 jopemachine   (501) staff       (20)      985 2023-07-31 06:55:19.000000 raftify-0.0.1/raftify/request_message.py
--rw-r--r--   0 jopemachine   (501) staff       (20)      753 2023-07-31 06:55:20.000000 raftify-0.0.1/raftify/response_message.py
--rw-r--r--   0 jopemachine   (501) staff       (20)     1503 2023-07-31 06:54:36.000000 raftify-0.0.1/raftify/utils.py
-drwxr-xr-x   0 jopemachine   (501) staff       (20)        0 2023-08-03 08:05:20.115509 raftify-0.0.1/raftify.egg-info/
--rw-r--r--   0 jopemachine   (501) staff       (20)      355 2023-08-03 08:05:20.000000 raftify-0.0.1/raftify.egg-info/PKG-INFO
--rw-r--r--   0 jopemachine   (501) staff       (20)      702 2023-08-03 08:05:20.000000 raftify-0.0.1/raftify.egg-info/SOURCES.txt
--rw-r--r--   0 jopemachine   (501) staff       (20)        1 2023-08-03 08:05:20.000000 raftify-0.0.1/raftify.egg-info/dependency_links.txt
--rw-r--r--   0 jopemachine   (501) staff       (20)        1 2023-07-31 06:50:22.000000 raftify-0.0.1/raftify.egg-info/not-zip-safe
--rw-r--r--   0 jopemachine   (501) staff       (20)      413 2023-08-03 08:05:20.000000 raftify-0.0.1/raftify.egg-info/requires.txt
--rw-r--r--   0 jopemachine   (501) staff       (20)        8 2023-08-03 08:05:20.000000 raftify-0.0.1/raftify.egg-info/top_level.txt
--rw-r--r--   0 jopemachine   (501) staff       (20)       38 2023-08-03 08:05:20.116894 raftify-0.0.1/setup.cfg
--rw-r--r--   0 jopemachine   (501) staff       (20)     1205 2023-08-03 08:04:35.000000 raftify-0.0.1/setup.py
+drwxr-xr-x   0 jopemachine   (501) staff       (20)        0 2023-08-03 08:15:03.498960 raftify-0.0.2/
+-rw-r--r--   0 jopemachine   (501) staff       (20)    10349 2023-07-31 06:47:59.000000 raftify-0.0.2/LICENSE
+-rw-r--r--   0 jopemachine   (501) staff       (20)     4797 2023-08-03 08:15:03.498823 raftify-0.0.2/PKG-INFO
+-rw-r--r--   0 jopemachine   (501) staff       (20)     4467 2023-08-03 04:04:47.000000 raftify-0.0.2/README.md
+-rw-r--r--   0 jopemachine   (501) staff       (20)      203 2023-08-03 04:04:47.000000 raftify-0.0.2/pyproject.toml
+drwxr-xr-x   0 jopemachine   (501) staff       (20)        0 2023-08-03 08:15:03.495096 raftify-0.0.2/raftify/
+-rw-r--r--   0 jopemachine   (501) staff       (20)        6 2023-08-03 08:10:21.000000 raftify-0.0.2/raftify/VERSION
+-rw-r--r--   0 jopemachine   (501) staff       (20)      679 2023-07-31 06:54:36.000000 raftify-0.0.2/raftify/__init__.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)       86 2023-07-31 06:54:36.000000 raftify-0.0.2/raftify/error.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)      368 2023-07-31 06:54:36.000000 raftify-0.0.2/raftify/fsm.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)    10934 2023-07-31 06:54:36.000000 raftify-0.0.2/raftify/lmdb.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)     2828 2023-07-31 07:10:41.000000 raftify-0.0.2/raftify/mailbox.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)     1408 2023-08-03 04:08:50.000000 raftify-0.0.2/raftify/message_sender.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)     7907 2023-07-31 06:55:11.000000 raftify-0.0.2/raftify/pb_adapter.py
+drwxr-xr-x   0 jopemachine   (501) staff       (20)        0 2023-08-03 08:15:03.498259 raftify-0.0.2/raftify/protos/
+-rw-r--r--   0 jopemachine   (501) staff       (20)     5208 2023-07-31 06:54:36.000000 raftify-0.0.2/raftify/protos/eraftpb_pb2.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)      173 2023-07-31 06:54:36.000000 raftify-0.0.2/raftify/protos/eraftpb_pb2_grpc.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)     2859 2023-07-31 06:54:36.000000 raftify-0.0.2/raftify/protos/raft_service_pb2.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)     7331 2023-07-31 06:54:36.000000 raftify-0.0.2/raftify/protos/raft_service_pb2_grpc.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)     2551 2023-07-31 06:55:04.000000 raftify-0.0.2/raftify/raft_client.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)     4693 2023-08-03 04:04:47.000000 raftify-0.0.2/raftify/raft_facade.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)    14379 2023-08-03 06:39:02.000000 raftify-0.0.2/raftify/raft_node.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)     1425 2023-07-31 06:55:16.000000 raftify-0.0.2/raftify/raft_server.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)     3621 2023-07-31 06:55:21.000000 raftify-0.0.2/raftify/raft_service.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)      985 2023-07-31 06:55:19.000000 raftify-0.0.2/raftify/request_message.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)      753 2023-07-31 06:55:20.000000 raftify-0.0.2/raftify/response_message.py
+-rw-r--r--   0 jopemachine   (501) staff       (20)     1503 2023-07-31 06:54:36.000000 raftify-0.0.2/raftify/utils.py
+drwxr-xr-x   0 jopemachine   (501) staff       (20)        0 2023-08-03 08:15:03.495913 raftify-0.0.2/raftify.egg-info/
+-rw-r--r--   0 jopemachine   (501) staff       (20)     4797 2023-08-03 08:15:03.000000 raftify-0.0.2/raftify.egg-info/PKG-INFO
+-rw-r--r--   0 jopemachine   (501) staff       (20)      702 2023-08-03 08:15:03.000000 raftify-0.0.2/raftify.egg-info/SOURCES.txt
+-rw-r--r--   0 jopemachine   (501) staff       (20)        1 2023-08-03 08:15:03.000000 raftify-0.0.2/raftify.egg-info/dependency_links.txt
+-rw-r--r--   0 jopemachine   (501) staff       (20)        1 2023-07-31 06:50:22.000000 raftify-0.0.2/raftify.egg-info/not-zip-safe
+-rw-r--r--   0 jopemachine   (501) staff       (20)      413 2023-08-03 08:15:03.000000 raftify-0.0.2/raftify.egg-info/requires.txt
+-rw-r--r--   0 jopemachine   (501) staff       (20)        8 2023-08-03 08:15:03.000000 raftify-0.0.2/raftify.egg-info/top_level.txt
+-rw-r--r--   0 jopemachine   (501) staff       (20)       38 2023-08-03 08:15:03.499003 raftify-0.0.2/setup.cfg
+-rw-r--r--   0 jopemachine   (501) staff       (20)     1242 2023-08-03 08:14:02.000000 raftify-0.0.2/setup.py
```

### Comparing `raftify-0.0.1/LICENSE` & `raftify-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/README.md` & `raftify-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/__init__.py` & `raftify-0.0.2/raftify/__init__.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/lmdb.py` & `raftify-0.0.2/raftify/lmdb.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/mailbox.py` & `raftify-0.0.2/raftify/mailbox.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/message_sender.py` & `raftify-0.0.2/raftify/message_sender.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/pb_adapter.py` & `raftify-0.0.2/raftify/pb_adapter.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/protos/eraftpb_pb2.py` & `raftify-0.0.2/raftify/protos/eraftpb_pb2.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/protos/raft_service_pb2.py` & `raftify-0.0.2/raftify/protos/raft_service_pb2.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/protos/raft_service_pb2_grpc.py` & `raftify-0.0.2/raftify/protos/raft_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/raft_client.py` & `raftify-0.0.2/raftify/raft_client.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/raft_facade.py` & `raftify-0.0.2/raftify/raft_facade.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/raft_node.py` & `raftify-0.0.2/raftify/raft_node.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/raft_server.py` & `raftify-0.0.2/raftify/raft_server.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/raft_service.py` & `raftify-0.0.2/raftify/raft_service.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/request_message.py` & `raftify-0.0.2/raftify/request_message.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/response_message.py` & `raftify-0.0.2/raftify/response_message.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify/utils.py` & `raftify-0.0.2/raftify/utils.py`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/raftify.egg-info/SOURCES.txt` & `raftify-0.0.2/raftify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raftify-0.0.1/setup.py` & `raftify-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import os
 from pathlib import Path
 
 from setuptools import setup
 
 ROOT_PATH = os.path.abspath(os.path.dirname(__file__))
 VERSION = (Path(__file__).parent / "raftify" / "VERSION").read_text().strip()
-description = (
-    "A raft framework, for regular people. Written in Python."
-)
+README = (Path(__file__).parent / "README.md").read_text().strip()
 
 
 def get_requirements(env: str = None):
     requirements = "requirements"
     if env is not None:
         requirements = f"{requirements}-{env}"
     with open(f"{requirements}.txt".format(env)) as fp:
@@ -22,15 +20,16 @@
 dev_requires = get_requirements("dev")
 build_requires = get_requirements("build")
 
 
 setup(
     name="raftify",
     version=VERSION,
-    description=description,
+    long_description=README,
+    long_description_content_type='text/markdown',
     author="Lablup Inc.",
     maintainer="jopemachine",
     maintainer_email="gbl@lablup.com",
     url="https://github.com/lablup/raftify",
     license="Apache License 2.0",
     package_dir={"raftify": "raftify"},
     package_data={"": ["VERSION"]},
```

