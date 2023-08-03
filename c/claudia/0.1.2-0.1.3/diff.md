# Comparing `tmp/claudia-0.1.2.tar.gz` & `tmp/claudia-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claudia-0.1.2.tar", last modified: Fri Jul 21 01:53:22 2023, max compression
+gzip compressed data, was "claudia-0.1.3.tar", last modified: Thu Aug  3 00:36:22 2023, max compression
```

## Comparing `claudia-0.1.2.tar` & `claudia-0.1.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.919436 claudia-0.1.2/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1074 2023-05-25 22:01:40.000000 claudia-0.1.2/LICENSE
--rw-r--r--   0 ksaxena    (502) staff       (20)    11120 2023-07-21 01:53:22.918224 claudia-0.1.2/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)      402 2023-06-22 00:52:56.000000 claudia-0.1.2/README.md
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.879432 claudia-0.1.2/claudia.egg-info/
--rw-r--r--   0 ksaxena    (502) staff       (20)    11120 2023-07-21 01:53:22.000000 claudia-0.1.2/claudia.egg-info/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)     2759 2023-07-21 01:53:22.000000 claudia-0.1.2/claudia.egg-info/SOURCES.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-07-21 01:53:22.000000 claudia-0.1.2/claudia.egg-info/dependency_links.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-07-21 01:53:22.000000 claudia-0.1.2/claudia.egg-info/entry_points.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)      109 2023-07-21 01:53:22.000000 claudia-0.1.2/claudia.egg-info/requires.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-07-21 01:53:22.000000 claudia-0.1.2/claudia.egg-info/top_level.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-07-21 01:53:22.919555 claudia-0.1.2/setup.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)     1478 2023-07-20 20:52:54.000000 claudia-0.1.2/setup.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.870006 claudia-0.1.2/src/
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.881323 claudia-0.1.2/src/claudia/
--rw-r--r--   0 ksaxena    (502) staff       (20)    10771 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/README.md
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    40220 2023-07-20 20:52:46.000000 claudia-0.1.2/src/claudia/claudia.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.883072 claudia-0.1.2/src/claudia/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/features/nft_burn_mint.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-07-12 21:19:51.000000 claudia-0.1.2/src/claudia/features/payments.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/features/trustline.feature
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.887083 claudia-0.1.2/src/claudia/javascript/
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/cleanup
--rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/cucumber.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.887728 claudia-0.1.2/src/claudia/javascript/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1227 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/features/context.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.888195 claudia-0.1.2/src/claudia/javascript/features/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)     2107 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/features/lib/ObjFactory.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.891077 claudia-0.1.2/src/claudia/javascript/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    38941 2023-07-21 01:52:20.000000 claudia-0.1.2/src/claudia/javascript/features/steps/common.js
--rw-r--r--   0 ksaxena    (502) staff       (20)      303 2023-06-05 20:21:20.000000 claudia-0.1.2/src/claudia/javascript/features/steps/constants.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/features/steps/nft_mint_burn.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/features/steps/payments.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/features/steps/trustline.js
--rw-r--r--   0 ksaxena    (502) staff       (20)   130175 2023-07-21 01:52:20.000000 claudia-0.1.2/src/claudia/javascript/package-lock.json
--rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-07-21 01:52:20.000000 claudia-0.1.2/src/claudia/javascript/package.json
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      870 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/javascript/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     5028 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/javascript/runTest
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.892833 claudia-0.1.2/src/claudia/network_setup/
--rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/Dockerfile.rippled_build
--rw-r--r--   0 ksaxena    (502) staff       (20)      714 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/Dockerfile.rippled_install
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.872612 claudia-0.1.2/src/claudia/network_setup/configs/
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.873464 claudia-0.1.2/src/claudia/network_setup/configs/rippled/
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.893956 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_1/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1809 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_1/rippled.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_1/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.894953 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_2/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1851 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_2/rippled.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_2/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.895897 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_3/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1851 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_3/rippled.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_3/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.896779 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_4/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1850 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_4/rippled.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_4/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.900560 claudia-0.1.2/src/claudia/network_setup/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1775 2023-07-21 01:52:09.000000 claudia-0.1.2/src/claudia/network_setup/lib/build.sh
--rw-r--r--   0 ksaxena    (502) staff       (20)     1268 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/lib/rippled_network.yml
--rw-r--r--   0 ksaxena    (502) staff       (20)    27463 2023-07-21 01:52:09.000000 claudia-0.1.2/src/claudia/network_setup/lib/setup_helper.sh
--rw-r--r--   0 ksaxena    (502) staff       (20)     1268 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/lib/sidechain_network.yml
--rw-r--r--   0 ksaxena    (502) staff       (20)     5442 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/network_setup/lib/validate_network.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     4013 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/network_setup/lib/witness_action.sh
--rw-r--r--   0 ksaxena    (502) staff       (20)    16916 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/network_setup/lib/xchain_bridge_create.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     7323 2023-07-20 20:52:46.000000 claudia-0.1.2/src/claudia/network_setup/setup.sh
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.903987 claudia-0.1.2/src/claudia/python/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/python/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/python/behave.ini
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/python/cleanup
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.905575 claudia-0.1.2/src/claudia/python/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/python/features/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     3217 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/python/features/environment.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.911637 claudia-0.1.2/src/claudia/python/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    65962 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/python/features/steps/nft_mint_burn.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    21692 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/python/features/steps/payments.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    54433 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/python/features/steps/trustline.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.912630 claudia-0.1.2/src/claudia/python/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/python/lib/__init__.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.914209 claudia-0.1.2/src/claudia/python/lib/exceptions/
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/python/lib/exceptions/InvalidInputException.py
--rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/python/lib/exceptions/UnconfiguredEnvironmentException.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-07-21 01:53:22.917277 claudia-0.1.2/src/claudia/python/lib/framework/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/python/lib/framework/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    26242 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/python/lib/framework/common.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      252 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/python/lib/framework/constants.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     9148 2023-07-20 20:52:54.000000 claudia-0.1.2/src/claudia/python/lib/framework/object_factory.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    22326 2023-07-19 20:08:15.000000 claudia-0.1.2/src/claudia/python/lib/framework/workflow_helper.py
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     1382 2023-05-30 20:36:34.000000 claudia-0.1.2/src/claudia/python/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     6158 2023-07-12 21:19:51.000000 claudia-0.1.2/src/claudia/python/runTest
--rw-r--r--   0 ksaxena    (502) staff       (20)      109 2023-06-22 00:52:56.000000 claudia-0.1.2/src/claudia/requirements.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.976202 claudia-0.1.3/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1074 2023-05-25 22:01:40.000000 claudia-0.1.3/LICENSE
+-rw-r--r--   0 ksaxena    (502) staff       (20)    11120 2023-08-03 00:36:22.975952 claudia-0.1.3/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)      402 2023-06-22 00:52:56.000000 claudia-0.1.3/README.md
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.952781 claudia-0.1.3/claudia.egg-info/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    11120 2023-08-03 00:36:22.000000 claudia-0.1.3/claudia.egg-info/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2759 2023-08-03 00:36:22.000000 claudia-0.1.3/claudia.egg-info/SOURCES.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-08-03 00:36:22.000000 claudia-0.1.3/claudia.egg-info/dependency_links.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-08-03 00:36:22.000000 claudia-0.1.3/claudia.egg-info/entry_points.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)      109 2023-08-03 00:36:22.000000 claudia-0.1.3/claudia.egg-info/requires.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-08-03 00:36:22.000000 claudia-0.1.3/claudia.egg-info/top_level.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-08-03 00:36:22.976253 claudia-0.1.3/setup.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1478 2023-08-03 00:31:55.000000 claudia-0.1.3/setup.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.945928 claudia-0.1.3/src/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.954151 claudia-0.1.3/src/claudia/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    10771 2023-06-22 00:52:56.000000 claudia-0.1.3/src/claudia/README.md
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    40220 2023-08-03 00:31:04.000000 claudia-0.1.3/src/claudia/claudia.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.955685 claudia-0.1.3/src/claudia/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/features/nft_burn_mint.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-07-12 21:19:51.000000 claudia-0.1.3/src/claudia/features/payments.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/features/trustline.feature
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.958788 claudia-0.1.3/src/claudia/javascript/
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/javascript/cleanup
+-rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/javascript/cucumber.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.959298 claudia-0.1.3/src/claudia/javascript/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1227 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/javascript/features/context.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.959592 claudia-0.1.3/src/claudia/javascript/features/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2107 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/javascript/features/lib/ObjFactory.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.961773 claudia-0.1.3/src/claudia/javascript/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    38941 2023-07-27 23:10:41.000000 claudia-0.1.3/src/claudia/javascript/features/steps/common.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)      303 2023-06-05 20:21:20.000000 claudia-0.1.3/src/claudia/javascript/features/steps/constants.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/javascript/features/steps/nft_mint_burn.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/javascript/features/steps/payments.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/javascript/features/steps/trustline.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)   130175 2023-07-27 23:10:41.000000 claudia-0.1.3/src/claudia/javascript/package-lock.json
+-rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-07-27 23:10:41.000000 claudia-0.1.3/src/claudia/javascript/package.json
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      870 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/javascript/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     5028 2023-06-22 00:52:56.000000 claudia-0.1.3/src/claudia/javascript/runTest
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.963186 claudia-0.1.3/src/claudia/network_setup/
+-rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-06-22 00:52:56.000000 claudia-0.1.3/src/claudia/network_setup/Dockerfile.rippled_build
+-rw-r--r--   0 ksaxena    (502) staff       (20)      714 2023-06-22 00:52:56.000000 claudia-0.1.3/src/claudia/network_setup/Dockerfile.rippled_install
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.947679 claudia-0.1.3/src/claudia/network_setup/configs/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.948350 claudia-0.1.3/src/claudia/network_setup/configs/rippled/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.963979 claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_1/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1809 2023-07-20 20:52:54.000000 claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_1/rippled.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_1/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.964731 claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_2/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1851 2023-07-20 20:52:54.000000 claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_2/rippled.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_2/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.965345 claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_3/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1851 2023-07-20 20:52:54.000000 claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_3/rippled.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_3/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.965889 claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_4/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1850 2023-07-20 20:52:54.000000 claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_4/rippled.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-22 00:52:56.000000 claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_4/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.968384 claudia-0.1.3/src/claudia/network_setup/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1775 2023-08-01 17:19:11.000000 claudia-0.1.3/src/claudia/network_setup/lib/build.sh
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1268 2023-06-22 00:52:56.000000 claudia-0.1.3/src/claudia/network_setup/lib/rippled_network.yml
+-rw-r--r--   0 ksaxena    (502) staff       (20)    27464 2023-08-03 00:31:19.000000 claudia-0.1.3/src/claudia/network_setup/lib/setup_helper.sh
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1268 2023-06-22 00:52:56.000000 claudia-0.1.3/src/claudia/network_setup/lib/sidechain_network.yml
+-rw-r--r--   0 ksaxena    (502) staff       (20)     5442 2023-06-22 00:52:56.000000 claudia-0.1.3/src/claudia/network_setup/lib/validate_network.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     4013 2023-07-19 20:08:15.000000 claudia-0.1.3/src/claudia/network_setup/lib/witness_action.sh
+-rw-r--r--   0 ksaxena    (502) staff       (20)    16916 2023-08-01 17:19:11.000000 claudia-0.1.3/src/claudia/network_setup/lib/xchain_bridge_create.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     7221 2023-08-03 00:31:19.000000 claudia-0.1.3/src/claudia/network_setup/setup.sh
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.970627 claudia-0.1.3/src/claudia/python/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/python/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/python/behave.ini
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/python/cleanup
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.971224 claudia-0.1.3/src/claudia/python/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/python/features/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     3217 2023-07-19 20:08:15.000000 claudia-0.1.3/src/claudia/python/features/environment.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.972793 claudia-0.1.3/src/claudia/python/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    65962 2023-07-20 20:52:54.000000 claudia-0.1.3/src/claudia/python/features/steps/nft_mint_burn.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    21692 2023-07-20 20:52:54.000000 claudia-0.1.3/src/claudia/python/features/steps/payments.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    54433 2023-07-20 20:52:54.000000 claudia-0.1.3/src/claudia/python/features/steps/trustline.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.973271 claudia-0.1.3/src/claudia/python/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-07-19 20:08:15.000000 claudia-0.1.3/src/claudia/python/lib/__init__.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.974058 claudia-0.1.3/src/claudia/python/lib/exceptions/
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-07-19 20:08:15.000000 claudia-0.1.3/src/claudia/python/lib/exceptions/InvalidInputException.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-07-19 20:08:15.000000 claudia-0.1.3/src/claudia/python/lib/exceptions/UnconfiguredEnvironmentException.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-08-03 00:36:22.975574 claudia-0.1.3/src/claudia/python/lib/framework/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-07-19 20:08:15.000000 claudia-0.1.3/src/claudia/python/lib/framework/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    26242 2023-07-20 20:52:54.000000 claudia-0.1.3/src/claudia/python/lib/framework/common.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      252 2023-07-19 20:08:15.000000 claudia-0.1.3/src/claudia/python/lib/framework/constants.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     9148 2023-07-20 20:52:54.000000 claudia-0.1.3/src/claudia/python/lib/framework/object_factory.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    22326 2023-08-01 17:19:11.000000 claudia-0.1.3/src/claudia/python/lib/framework/workflow_helper.py
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     1382 2023-05-30 20:36:34.000000 claudia-0.1.3/src/claudia/python/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     6158 2023-07-12 21:19:51.000000 claudia-0.1.3/src/claudia/python/runTest
+-rw-r--r--   0 ksaxena    (502) staff       (20)      109 2023-08-03 00:31:04.000000 claudia-0.1.3/src/claudia/requirements.txt
```

### Comparing `claudia-0.1.2/LICENSE` & `claudia-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/PKG-INFO` & `claudia-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claudia
-Version: 0.1.2
+Version: 0.1.3
 Summary: Run XRPL Automated Tests
 Home-page: https://xrpl.org/
 Download-URL: https://gitlab.ops.ripple.com/xrpledger/xrpl-nocode-automation
 Author: Kausty Saxena
 Author-email: ksaxena@ripple.com
 Keywords: ripple xrpl python javascript
 Description-Content-Type: text/markdown
```

### Comparing `claudia-0.1.2/claudia.egg-info/PKG-INFO` & `claudia-0.1.3/claudia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claudia
-Version: 0.1.2
+Version: 0.1.3
 Summary: Run XRPL Automated Tests
 Home-page: https://xrpl.org/
 Download-URL: https://gitlab.ops.ripple.com/xrpledger/xrpl-nocode-automation
 Author: Kausty Saxena
 Author-email: ksaxena@ripple.com
 Keywords: ripple xrpl python javascript
 Description-Content-Type: text/markdown
```

### Comparing `claudia-0.1.2/claudia.egg-info/SOURCES.txt` & `claudia-0.1.3/claudia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/setup.py` & `claudia-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         requirements = content.split('\n')
 
     return requirements
 
 
 setup(
     name='claudia',
-    version='0.1.2',
+    version='0.1.3',
     description='Run XRPL Automated Tests',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     author="Kausty Saxena",
     author_email="ksaxena@ripple.com",
     keywords="ripple xrpl python javascript",
     url='https://xrpl.org/',
```

### Comparing `claudia-0.1.2/src/claudia/README.md` & `claudia-0.1.3/src/claudia/README.md`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/claudia.py` & `claudia-0.1.3/src/claudia/claudia.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/features/nft_burn_mint.feature` & `claudia-0.1.3/src/claudia/features/nft_burn_mint.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/features/payments.feature` & `claudia-0.1.3/src/claudia/features/payments.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/features/trustline.feature` & `claudia-0.1.3/src/claudia/features/trustline.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/javascript/features/context.js` & `claudia-0.1.3/src/claudia/javascript/features/context.js`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/javascript/features/lib/ObjFactory.js` & `claudia-0.1.3/src/claudia/javascript/features/lib/ObjFactory.js`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/javascript/features/steps/common.js` & `claudia-0.1.3/src/claudia/javascript/features/steps/common.js`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/javascript/features/steps/nft_mint_burn.js` & `claudia-0.1.3/src/claudia/javascript/features/steps/nft_mint_burn.js`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/javascript/features/steps/payments.js` & `claudia-0.1.3/src/claudia/javascript/features/steps/payments.js`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/javascript/features/steps/trustline.js` & `claudia-0.1.3/src/claudia/javascript/features/steps/trustline.js`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/javascript/package-lock.json` & `claudia-0.1.3/src/claudia/javascript/package-lock.json`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/javascript/runSetup` & `claudia-0.1.3/src/claudia/javascript/runSetup`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/javascript/runTest` & `claudia-0.1.3/src/claudia/javascript/runTest`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/network_setup/Dockerfile.rippled_install` & `claudia-0.1.3/src/claudia/network_setup/Dockerfile.rippled_install`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_1/rippled.cfg` & `claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_1/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_2/rippled.cfg` & `claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_2/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_3/rippled.cfg` & `claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_3/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/network_setup/configs/rippled/rippled_4/rippled.cfg` & `claudia-0.1.3/src/claudia/network_setup/configs/rippled/rippled_4/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/network_setup/lib/build.sh` & `claudia-0.1.3/src/claudia/network_setup/lib/build.sh`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/network_setup/lib/rippled_network.yml` & `claudia-0.1.3/src/claudia/network_setup/lib/rippled_network.yml`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/network_setup/lib/setup_helper.sh` & `claudia-0.1.3/src/claudia/network_setup/lib/setup_helper.sh`

 * *Files 0% similar despite different names*

```diff
@@ -714,15 +714,15 @@
   if [ "${l_disable_feature_opt}" = "true" ]; then
     if [ -n "${feature}" ]; then
       for config_file in ${host_script_dir}/${RIPPLED_CONFIGS_FILE}
       do
         feature_configured=$(grep -w "${feature}" "${config_file}")
         if [ -n "${feature_configured}" ]; then
           feature_string=""
-          sed -i '' "/${feature}/d" "${config_file}"
+          sed -i.bak "/${feature}/d" "${config_file}"
           feature_disabled=true
         fi
       done
 
       if [ "${feature_disabled}" = "true" ]; then
         echo "- Feature '${feature}' disabled"
         stop_all_networks
```

### Comparing `claudia-0.1.2/src/claudia/network_setup/lib/sidechain_network.yml` & `claudia-0.1.3/src/claudia/network_setup/lib/sidechain_network.yml`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/network_setup/lib/validate_network.py` & `claudia-0.1.3/src/claudia/network_setup/lib/validate_network.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/network_setup/lib/witness_action.sh` & `claudia-0.1.3/src/claudia/network_setup/lib/witness_action.sh`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/network_setup/lib/xchain_bridge_create.py` & `claudia-0.1.3/src/claudia/network_setup/lib/xchain_bridge_create.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/network_setup/setup.sh` & `claudia-0.1.3/src/claudia/network_setup/setup.sh`

 * *Files 3% similar despite different names*

```diff
@@ -159,44 +159,41 @@
   --rippledVersion)
     get_rippled_version_opt="true"
     ;;
 
   --runUnittests)
     run_unittests_opt="true"
     next_param=$(echo "$2" | grep "^--")
-    if [ -z "${next_param}" ]; then
-      filtered_unittests_to_run="${2:-$filtered_unittests_to_run}"
+    if [ -n "${next_param}" ]; then
+      filtered_unittests_to_run="$2"
       shift
     fi
     ;;
 
   --networkStart)
     start_network_opt="true"
     next_param=$(echo "$2" | grep "^--")
-    if [ -z "${next_param}" ]; then
-      network="${2:-$network}"
-      shift
+    if [ -n "${next_param}" ]; then
+      network="$2"
     fi
     ;;
 
   --networkStop)
     stop_network_opt="true"
     next_param=$(echo "$2" | grep "^--")
-    if [ -z "${next_param}" ]; then
-      network="${2:-$network}"
-      shift
+    if [ -n "${next_param}" ]; then
+      network="$2"
     fi
     ;;
 
   --networkStatus)
     validate_network_opt="true"
     next_param=$(echo "$2" | grep "^--")
-    if [ -z "${next_param}" ]; then
-      network="${2:-$network}"
-      shift
+    if [ -n "${next_param}" ]; then
+      network="$2"
     fi
     ;;
 
   --sidechainStart)
     start_sidechain_opt="true"
     witness_action="--witnessStart"
     network=sidechain
```

### Comparing `claudia-0.1.2/src/claudia/python/features/environment.py` & `claudia-0.1.3/src/claudia/python/features/environment.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/python/features/steps/nft_mint_burn.py` & `claudia-0.1.3/src/claudia/python/features/steps/nft_mint_burn.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/python/features/steps/payments.py` & `claudia-0.1.3/src/claudia/python/features/steps/payments.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/python/features/steps/trustline.py` & `claudia-0.1.3/src/claudia/python/features/steps/trustline.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/python/lib/framework/common.py` & `claudia-0.1.3/src/claudia/python/lib/framework/common.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/python/lib/framework/object_factory.py` & `claudia-0.1.3/src/claudia/python/lib/framework/object_factory.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/python/lib/framework/workflow_helper.py` & `claudia-0.1.3/src/claudia/python/lib/framework/workflow_helper.py`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/python/runSetup` & `claudia-0.1.3/src/claudia/python/runSetup`

 * *Files identical despite different names*

### Comparing `claudia-0.1.2/src/claudia/python/runTest` & `claudia-0.1.3/src/claudia/python/runTest`

 * *Files identical despite different names*

