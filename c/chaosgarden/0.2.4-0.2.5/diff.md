# Comparing `tmp/chaosgarden-0.2.4.tar.gz` & `tmp/chaosgarden-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaosgarden-0.2.4.tar", last modified: Fri Jul 21 12:36:01 2023, max compression
+gzip compressed data, was "chaosgarden-0.2.5.tar", last modified: Thu Aug  3 05:36:30 2023, max compression
```

## Comparing `chaosgarden-0.2.4.tar` & `chaosgarden-0.2.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.855718 chaosgarden-0.2.4/
--rw-r--r--   0 root         (0) root         (0)    10255 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-21 12:36:01.855718 chaosgarden-0.2.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.847718 chaosgarden-0.2.4/chaosgarden/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.847718 chaosgarden-0.2.4/chaosgarden/alicloud/
--rw-r--r--   0 root         (0) root         (0)    27059 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/alicloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16698 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/alicloud/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.847718 chaosgarden-0.2.4/chaosgarden/aws/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12486 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/aws/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.847718 chaosgarden-0.2.4/chaosgarden/azure/
--rw-r--r--   0 root         (0) root         (0)     7694 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/azure/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14897 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/azure/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/garden/
--rw-r--r--   0 root         (0) root         (0)      621 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/garden/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22179 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/garden/actions.py
--rw-r--r--   0 root         (0) root         (0)     4235 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/garden/probes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/gcp/
--rw-r--r--   0 root         (0) root         (0)     6984 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/gcp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15392 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/gcp/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/human/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/human/__init__.py
--rw-r--r--   0 root         (0) root         (0)      198 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/human/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/k8s/
--rw-r--r--   0 root         (0) root         (0)     6886 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4714 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/k8s/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3425 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/api/authenticators.py
--rw-r--r--   0 root         (0) root         (0)     7365 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/api/clients.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/api/cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/k8s/probe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11170 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2416 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/generate_resources.py
--rw-r--r--   0 root         (0) root         (0)    14856 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/probe_pod.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/suicidal_pod.py
--rw-r--r--   0 root         (0) root         (0)     8099 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/templated_resources.yaml
--rw-r--r--   0 root         (0) root         (0)     1943 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/thresholds.py
--rw-r--r--   0 root         (0) root         (0)    20971 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/metal/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/metal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/openstack/
--rw-r--r--   0 root         (0) root         (0)     4446 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/openstack/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13046 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/openstack/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.855718 chaosgarden-0.2.4/chaosgarden/util/
--rw-r--r--   0 root         (0) root         (0)      916 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1875 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/util/terminator.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/util/threading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.855718 chaosgarden-0.2.4/chaosgarden/vsphere/
--rw-r--r--   0 root         (0) root         (0)    11990 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/vsphere/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10486 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/vsphere/actions.py
--rw-r--r--   0 root         (0) root         (0)     4821 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/vsphere/pchelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.847718 chaosgarden-0.2.4/chaosgarden.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-21 12:36:01.000000 chaosgarden-0.2.4/chaosgarden.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1443 2023-07-21 12:36:01.000000 chaosgarden-0.2.4/chaosgarden.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 12:36:01.000000 chaosgarden-0.2.4/chaosgarden.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      436 2023-07-21 12:36:01.000000 chaosgarden-0.2.4/chaosgarden.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-21 12:36:01.000000 chaosgarden-0.2.4/chaosgarden.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 12:36:01.855718 chaosgarden-0.2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3331 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.994778 chaosgarden-0.2.5/
+-rw-r--r--   0 root         (0) root         (0)    10255 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-08-03 05:36:30.994778 chaosgarden-0.2.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.986778 chaosgarden-0.2.5/chaosgarden/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.986778 chaosgarden-0.2.5/chaosgarden/alicloud/
+-rw-r--r--   0 root         (0) root         (0)    27696 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/alicloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16695 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/alicloud/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.986778 chaosgarden-0.2.5/chaosgarden/aws/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12486 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/aws/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.986778 chaosgarden-0.2.5/chaosgarden/azure/
+-rw-r--r--   0 root         (0) root         (0)     7694 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/azure/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14897 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/azure/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.986778 chaosgarden-0.2.5/chaosgarden/garden/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/garden/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22179 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/garden/actions.py
+-rw-r--r--   0 root         (0) root         (0)     4235 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/garden/probes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.986778 chaosgarden-0.2.5/chaosgarden/gcp/
+-rw-r--r--   0 root         (0) root         (0)     6984 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/gcp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15392 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/gcp/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.990778 chaosgarden-0.2.5/chaosgarden/human/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/human/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      198 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/human/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.990778 chaosgarden-0.2.5/chaosgarden/k8s/
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4714 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.990778 chaosgarden-0.2.5/chaosgarden/k8s/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/api/authenticators.py
+-rw-r--r--   0 root         (0) root         (0)     7365 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/api/clients.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/api/cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.990778 chaosgarden-0.2.5/chaosgarden/k8s/probe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/probe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11170 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/probe/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.990778 chaosgarden-0.2.5/chaosgarden/k8s/probe/resources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/probe/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/probe/resources/generate_resources.py
+-rw-r--r--   0 root         (0) root         (0)    14856 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/probe/resources/probe_pod.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/probe/resources/suicidal_pod.py
+-rw-r--r--   0 root         (0) root         (0)     8099 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/probe/resources/templated_resources.yaml
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/probe/thresholds.py
+-rw-r--r--   0 root         (0) root         (0)    20971 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/k8s/probes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.990778 chaosgarden-0.2.5/chaosgarden/metal/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/metal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.990778 chaosgarden-0.2.5/chaosgarden/openstack/
+-rw-r--r--   0 root         (0) root         (0)     4446 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/openstack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13046 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/openstack/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.990778 chaosgarden-0.2.5/chaosgarden/util/
+-rw-r--r--   0 root         (0) root         (0)      916 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/util/terminator.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/util/threading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.994778 chaosgarden-0.2.5/chaosgarden/vsphere/
+-rw-r--r--   0 root         (0) root         (0)    11990 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/vsphere/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10486 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/vsphere/actions.py
+-rw-r--r--   0 root         (0) root         (0)     4821 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/chaosgarden/vsphere/pchelper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:36:30.986778 chaosgarden-0.2.5/chaosgarden.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-08-03 05:36:30.000000 chaosgarden-0.2.5/chaosgarden.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-08-03 05:36:30.000000 chaosgarden-0.2.5/chaosgarden.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 05:36:30.000000 chaosgarden-0.2.5/chaosgarden.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      436 2023-08-03 05:36:30.000000 chaosgarden-0.2.5/chaosgarden.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-03 05:36:30.000000 chaosgarden-0.2.5/chaosgarden.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 05:36:30.994778 chaosgarden-0.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3331 2023-08-03 05:35:38.000000 chaosgarden-0.2.5/setup.py
```

### Comparing `chaosgarden-0.2.4/LICENSE` & `chaosgarden-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/PKG-INFO` & `chaosgarden-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaosgarden
-Version: 0.2.4
+Version: 0.2.5
 Summary: Generic cloud provider zone outage and Kubernetes pod disruption simulations with specific support for Gardener
 Home-page: https://github.com/gardener/chaos-engineering
 Author: SAP SE
 License: License :: OSI Approved :: Apache Software License
 Keywords: chaostoolkit,kubernetes,gardener
 Platform: AWS
 Platform: Azure
```

### Comparing `chaosgarden-0.2.4/chaosgarden/alicloud/__init__.py` & `chaosgarden-0.2.5/chaosgarden/alicloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 import time
 import json
-import uuid
-import copy
 
 from dataclasses import dataclass, field
 
 from aliyunsdkcore.client import AcsClient
 from aliyunsdkcore.acs_exception.exceptions import ClientException
 from aliyunsdkcore.acs_exception.exceptions import ServerException
+from aliyunsdkcore.request import AcsRequest
 
 from aliyunsdkecs.request.v20140526.DescribeInstancesRequest import DescribeInstancesRequest
 from aliyunsdkecs.request.v20140526.RebootInstanceRequest import RebootInstanceRequest
 from aliyunsdkecs.request.v20140526.DeleteInstanceRequest import DeleteInstanceRequest
 
 from aliyunsdkecs.request.v20140526.ListTagResourcesRequest import ListTagResourcesRequest as EcsListTagResourcesRequest
 
@@ -35,35 +34,50 @@
     if len(sorce_array) != len(dest_array):
         return False
     for idx in range(len(sorce_array)):
         if sorce_array[idx] != dest_array[idx]:
             return False
     return True
 
+def remove_dict_key(the_dict, key_name):
+    if the_dict and key_name in the_dict:
+        del the_dict[key_name]
+
 MAX_RETRY=5
 MAX_SIZE = 50
 @dataclass
 class AliyunBot:
     region: str
     access_key: str
     secret_key: str
     client: AcsClient = field(init=False)
 
     def __post_init__(self):    
         self.client = AcsClient(self.access_key, self.secret_key, self.region)
 
+    def __clean_request(self, the_request: AcsRequest):
+        params = the_request.get_query_params()
+        remove_dict_key(params, 'Version')
+        remove_dict_key(params, 'Action')
+        remove_dict_key(params, 'Format')
+        remove_dict_key(params, 'RegionId')
+        remove_dict_key(params, 'AccessKeyId')
+        remove_dict_key(params, 'Timestamp')
+        remove_dict_key(params, 'SignatureMethod')
+        remove_dict_key(params, 'SignatureVersion')
+        remove_dict_key(params, 'SignatureNonce')
+        remove_dict_key(params, 'Signature')
+
     def __send_request(self, request):
-        
-        the_request = copy.deepcopy(request)
         try_count = 0
         while True:
             try:
                 try_count = try_count +1
-                the_request = copy.deepcopy(request)
-                return self.__call_request_action(the_request)
+                self.__clean_request(request)
+                return self.__call_request_action(request)
                 
             except ServerException as se:
                 
                 print(f'error info: {se}')
                 if se.get_error_code() in ['Throttling.User'] and try_count < MAX_RETRY:
                     sleep_time = 30 if try_count==1 else 3
                     time.sleep( sleep_time )
```

### Comparing `chaosgarden-0.2.4/chaosgarden/alicloud/actions.py` & `chaosgarden-0.2.5/chaosgarden/alicloud/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,15 +396,15 @@
     mode: str):
 
     logger.info(f'begin to unblock vpc {vpc_id} ')
 
     # get blocking ACL
     exists_block_acl = get_or_create_block_acl(alibot, vpc_id, mode)
     if exists_block_acl is None:
-        logger.warning(f'no exists alc for mode {mode} in vpc {vpc_id}, unblock exited!!')
+        logger.info(f'no exists alc for mode {mode} in vpc {vpc_id}, unblock exited!!')
         return
 
     blocking_acl_id = exists_block_acl['NetworkAclId']
     logger.info(f'got exists block acl {blocking_acl_id}')
 
 
     assocs_str = exists_block_acl['Tags'].get(ORIGINAL_NETWORK_ACL_ASSOCIATIONS_TAG_NAME)
```

### Comparing `chaosgarden-0.2.4/chaosgarden/aws/actions.py` & `chaosgarden-0.2.5/chaosgarden/aws/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/azure/__init__.py` & `chaosgarden-0.2.5/chaosgarden/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/azure/actions.py` & `chaosgarden-0.2.5/chaosgarden/azure/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/garden/__init__.py` & `chaosgarden-0.2.5/chaosgarden/garden/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/garden/actions.py` & `chaosgarden-0.2.5/chaosgarden/garden/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,32 +373,32 @@
     secret_binding  = Box(garden.client(API.CustomResources).get_namespaced_custom_object(name = shoot.spec.secretBindingName, namespace = project.spec.namespace, group = 'core.gardener.cloud', version = 'v1beta1', plural = 'secretbindings'))
     credentials     = Box(garden.client(API.CoreV1).read_namespaced_secret(name = secret_binding.secretRef.name, namespace = secret_binding.secretRef.namespace).data)
     cloud_profile   = Box(garden.client(API.CustomResources).get_cluster_custom_object(name = shoot.spec.cloudProfileName, group = 'core.gardener.cloud', version = 'v1beta1', plural = 'cloudprofiles'))
 
     # handle different cloud providers
     cloud_provider = shoot.spec.provider.type
     zone = resolve_zone(zone, resolve_zones(shoot.spec))
-    if cloud_provider == 'aws':
-        filters = {
-            'instances': [{'Name': 'tag-key', 'Values': [f'kubernetes.io/cluster/{shoot.status.technicalID}']}],
-            'vpcs': [{'Name': 'tag-key', 'Values': [f'kubernetes.io/cluster/{shoot.status.technicalID}']}]}
-        configuration = {
-            'aws_region': shoot.spec.region}
-        secrets = {}
-        b64decode_and_add(credentials, 'accessKeyID', secrets, 'aws_access_key_id')
-        b64decode_and_add(credentials, 'secretAccessKey', secrets, 'aws_secret_access_key')
-    elif cloud_provider == 'alicloud':
+    if cloud_provider == 'alicloud':
         filters = {
             'instances': {'Tag-key': f'kubernetes.io/cluster/{shoot.status.technicalID}'},
             'vpc': {'Name': f'shoot--{configuration.garden_project}--{configuration.garden_shoot}-vpc'}}
         configuration = {
             'ali_region': shoot.spec.region}
         secrets = {}
         b64decode_and_add(credentials, 'accessKeyID', secrets, 'ali_access_key')
         b64decode_and_add(credentials, 'accessKeySecret', secrets, 'ali_secret_key')
+    elif cloud_provider == 'aws':
+        filters = {
+            'instances': [{'Name': 'tag-key', 'Values': [f'kubernetes.io/cluster/{shoot.status.technicalID}']}],
+            'vpcs': [{'Name': 'tag-key', 'Values': [f'kubernetes.io/cluster/{shoot.status.technicalID}']}]}
+        configuration = {
+            'aws_region': shoot.spec.region}
+        secrets = {}
+        b64decode_and_add(credentials, 'accessKeyID', secrets, 'aws_access_key_id')
+        b64decode_and_add(credentials, 'secretAccessKey', secrets, 'aws_secret_access_key')
     elif cloud_provider == 'azure':
         cloud = configuration.get('azure_cloud', 'AZURE_PUBLIC_CLOUD')
         filters = {
             'virtual_machines': f'where tags contains "kubernetes.io-cluster-{shoot.status.technicalID}"'}
         configuration = {
             'azure_region': shoot.spec.region,
             'azure_resource_group': shoot.spec.provider.infrastructureConfig.resourceGroup.name if 'resourceGroup' in shoot.spec.provider.infrastructureConfig else shoot.status.technicalID}
```

### Comparing `chaosgarden-0.2.4/chaosgarden/garden/probes.py` & `chaosgarden-0.2.5/chaosgarden/garden/probes.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/gcp/__init__.py` & `chaosgarden-0.2.5/chaosgarden/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/gcp/actions.py` & `chaosgarden-0.2.5/chaosgarden/gcp/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/k8s/__init__.py` & `chaosgarden-0.2.5/chaosgarden/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/k8s/actions.py` & `chaosgarden-0.2.5/chaosgarden/k8s/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/k8s/api/authenticators.py` & `chaosgarden-0.2.5/chaosgarden/k8s/api/authenticators.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/k8s/api/clients.py` & `chaosgarden-0.2.5/chaosgarden/k8s/api/clients.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/k8s/api/cluster.py` & `chaosgarden-0.2.5/chaosgarden/k8s/api/cluster.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/k8s/probe/metrics.py` & `chaosgarden-0.2.5/chaosgarden/k8s/probe/metrics.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/generate_resources.py` & `chaosgarden-0.2.5/chaosgarden/k8s/probe/resources/generate_resources.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/probe_pod.py` & `chaosgarden-0.2.5/chaosgarden/k8s/probe/resources/probe_pod.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/suicidal_pod.py` & `chaosgarden-0.2.5/chaosgarden/k8s/probe/resources/suicidal_pod.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/templated_resources.yaml` & `chaosgarden-0.2.5/chaosgarden/k8s/probe/resources/templated_resources.yaml`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/k8s/probe/thresholds.py` & `chaosgarden-0.2.5/chaosgarden/k8s/probe/thresholds.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/k8s/probes.py` & `chaosgarden-0.2.5/chaosgarden/k8s/probes.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/openstack/__init__.py` & `chaosgarden-0.2.5/chaosgarden/openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/openstack/actions.py` & `chaosgarden-0.2.5/chaosgarden/openstack/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/util/__init__.py` & `chaosgarden-0.2.5/chaosgarden/util/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/util/terminator.py` & `chaosgarden-0.2.5/chaosgarden/util/terminator.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/util/threading.py` & `chaosgarden-0.2.5/chaosgarden/util/threading.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/vsphere/__init__.py` & `chaosgarden-0.2.5/chaosgarden/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/vsphere/actions.py` & `chaosgarden-0.2.5/chaosgarden/vsphere/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden/vsphere/pchelper.py` & `chaosgarden-0.2.5/chaosgarden/vsphere/pchelper.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/chaosgarden.egg-info/PKG-INFO` & `chaosgarden-0.2.5/chaosgarden.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaosgarden
-Version: 0.2.4
+Version: 0.2.5
 Summary: Generic cloud provider zone outage and Kubernetes pod disruption simulations with specific support for Gardener
 Home-page: https://github.com/gardener/chaos-engineering
 Author: SAP SE
 License: License :: OSI Approved :: Apache Software License
 Keywords: chaostoolkit,kubernetes,gardener
 Platform: AWS
 Platform: Azure
```

### Comparing `chaosgarden-0.2.4/chaosgarden.egg-info/SOURCES.txt` & `chaosgarden-0.2.5/chaosgarden.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.4/setup.py` & `chaosgarden-0.2.5/setup.py`

 * *Files identical despite different names*

