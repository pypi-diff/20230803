# Comparing `tmp/customerio_cdp_analytics-0.0.1.tar.gz` & `tmp/customerio_cdp_analytics-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customerio_cdp_analytics-0.0.1.tar", last modified: Fri May  5 13:59:38 2023, max compression
+gzip compressed data, was "customerio_cdp_analytics-0.0.2.tar", last modified: Thu Aug  3 09:23:17 2023, max compression
```

## Comparing `customerio_cdp_analytics-0.0.1.tar` & `customerio_cdp_analytics-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxr-xr-x   0 nunofgs    (501) staff       (20)        0 2023-05-05 13:59:38.809862 customerio_cdp_analytics-0.0.1/
--rw-r--r--   0 nunofgs    (501) staff       (20)     1109 2023-05-05 09:31:09.000000 customerio_cdp_analytics-0.0.1/LICENSE
--rw-r--r--   0 nunofgs    (501) staff       (20)       18 2023-05-05 09:31:09.000000 customerio_cdp_analytics-0.0.1/MANIFEST.in
--rw-r--r--   0 nunofgs    (501) staff       (20)     1233 2023-05-05 13:59:38.809914 customerio_cdp_analytics-0.0.1/PKG-INFO
--rw-r--r--   0 nunofgs    (501) staff       (20)      427 2023-05-05 13:55:54.000000 customerio_cdp_analytics-0.0.1/README.md
-drwxr-xr-x   0 nunofgs    (501) staff       (20)        0 2023-05-05 13:59:38.806933 customerio_cdp_analytics-0.0.1/analytics/
-drwxr-xr-x   0 nunofgs    (501) staff       (20)        0 2023-05-05 13:59:38.808198 customerio_cdp_analytics-0.0.1/analytics/test/
--rw-r--r--   0 nunofgs    (501) staff       (20)    13008 2023-05-05 09:31:09.000000 customerio_cdp_analytics-0.0.1/analytics/test/client.py
-drwxr-xr-x   0 nunofgs    (501) staff       (20)        0 2023-05-05 13:59:38.807080 customerio_cdp_analytics-0.0.1/customerio/
-drwxr-xr-x   0 nunofgs    (501) staff       (20)        0 2023-05-05 13:59:38.809120 customerio_cdp_analytics-0.0.1/customerio/analytics/
--rw-r--r--   0 nunofgs    (501) staff       (20)     2036 2023-05-05 09:31:09.000000 customerio_cdp_analytics-0.0.1/customerio/analytics/__init__.py
--rw-r--r--   0 nunofgs    (501) staff       (20)    11183 2023-05-05 09:31:09.000000 customerio_cdp_analytics-0.0.1/customerio/analytics/client.py
--rw-r--r--   0 nunofgs    (501) staff       (20)     4463 2023-05-05 09:31:09.000000 customerio_cdp_analytics-0.0.1/customerio/analytics/consumer.py
--rw-r--r--   0 nunofgs    (501) staff       (20)     2381 2023-05-05 09:31:09.000000 customerio_cdp_analytics-0.0.1/customerio/analytics/request.py
--rw-r--r--   0 nunofgs    (501) staff       (20)     2471 2023-05-05 09:31:09.000000 customerio_cdp_analytics-0.0.1/customerio/analytics/utils.py
--rw-r--r--   0 nunofgs    (501) staff       (20)       18 2023-05-05 09:31:09.000000 customerio_cdp_analytics-0.0.1/customerio/analytics/version.py
-drwxr-xr-x   0 nunofgs    (501) staff       (20)        0 2023-05-05 13:59:38.809753 customerio_cdp_analytics-0.0.1/customerio_cdp_analytics.egg-info/
--rw-r--r--   0 nunofgs    (501) staff       (20)     1233 2023-05-05 13:59:38.000000 customerio_cdp_analytics-0.0.1/customerio_cdp_analytics.egg-info/PKG-INFO
--rw-r--r--   0 nunofgs    (501) staff       (20)      503 2023-05-05 13:59:38.000000 customerio_cdp_analytics-0.0.1/customerio_cdp_analytics.egg-info/SOURCES.txt
--rw-r--r--   0 nunofgs    (501) staff       (20)        1 2023-05-05 13:59:38.000000 customerio_cdp_analytics-0.0.1/customerio_cdp_analytics.egg-info/dependency_links.txt
--rw-r--r--   0 nunofgs    (501) staff       (20)      111 2023-05-05 13:59:38.000000 customerio_cdp_analytics-0.0.1/customerio_cdp_analytics.egg-info/requires.txt
--rw-r--r--   0 nunofgs    (501) staff       (20)       21 2023-05-05 13:59:38.000000 customerio_cdp_analytics-0.0.1/customerio_cdp_analytics.egg-info/top_level.txt
--rw-r--r--   0 nunofgs    (501) staff       (20)       67 2023-05-05 13:59:38.810091 customerio_cdp_analytics-0.0.1/setup.cfg
--rw-r--r--   0 nunofgs    (501) staff       (20)     1999 2023-05-05 13:54:26.000000 customerio_cdp_analytics-0.0.1/setup.py
+drwxr-xr-x   0 nunofgs    (501) staff       (20)        0 2023-08-03 09:23:17.961479 customerio_cdp_analytics-0.0.2/
+-rw-r--r--   0 nunofgs    (501) staff       (20)     1109 2023-08-02 16:54:23.000000 customerio_cdp_analytics-0.0.2/LICENSE
+-rw-r--r--   0 nunofgs    (501) staff       (20)       18 2023-05-05 09:31:09.000000 customerio_cdp_analytics-0.0.2/MANIFEST.in
+-rw-r--r--   0 nunofgs    (501) staff       (20)     1233 2023-08-03 09:23:17.961551 customerio_cdp_analytics-0.0.2/PKG-INFO
+-rw-r--r--   0 nunofgs    (501) staff       (20)      427 2023-08-02 16:54:23.000000 customerio_cdp_analytics-0.0.2/README.md
+drwxr-xr-x   0 nunofgs    (501) staff       (20)        0 2023-08-03 09:23:17.957493 customerio_cdp_analytics-0.0.2/customerio/
+drwxr-xr-x   0 nunofgs    (501) staff       (20)        0 2023-08-03 09:23:17.960254 customerio_cdp_analytics-0.0.2/customerio/analytics/
+-rw-r--r--   0 nunofgs    (501) staff       (20)     2036 2023-08-02 16:54:23.000000 customerio_cdp_analytics-0.0.2/customerio/analytics/__init__.py
+-rw-r--r--   0 nunofgs    (501) staff       (20)    11105 2023-08-03 09:12:00.000000 customerio_cdp_analytics-0.0.2/customerio/analytics/client.py
+-rw-r--r--   0 nunofgs    (501) staff       (20)     4463 2023-08-02 17:10:56.000000 customerio_cdp_analytics-0.0.2/customerio/analytics/consumer.py
+-rw-r--r--   0 nunofgs    (501) staff       (20)     2381 2023-08-02 17:12:52.000000 customerio_cdp_analytics-0.0.2/customerio/analytics/request.py
+-rw-r--r--   0 nunofgs    (501) staff       (20)     2471 2023-08-02 16:54:23.000000 customerio_cdp_analytics-0.0.2/customerio/analytics/utils.py
+-rw-r--r--   0 nunofgs    (501) staff       (20)       18 2023-08-03 09:13:09.000000 customerio_cdp_analytics-0.0.2/customerio/analytics/version.py
+drwxr-xr-x   0 nunofgs    (501) staff       (20)        0 2023-08-03 09:23:17.961316 customerio_cdp_analytics-0.0.2/customerio_cdp_analytics.egg-info/
+-rw-r--r--   0 nunofgs    (501) staff       (20)     1233 2023-08-03 09:23:17.000000 customerio_cdp_analytics-0.0.2/customerio_cdp_analytics.egg-info/PKG-INFO
+-rw-r--r--   0 nunofgs    (501) staff       (20)      478 2023-08-03 09:23:17.000000 customerio_cdp_analytics-0.0.2/customerio_cdp_analytics.egg-info/SOURCES.txt
+-rw-r--r--   0 nunofgs    (501) staff       (20)        1 2023-08-03 09:23:17.000000 customerio_cdp_analytics-0.0.2/customerio_cdp_analytics.egg-info/dependency_links.txt
+-rw-r--r--   0 nunofgs    (501) staff       (20)      111 2023-08-03 09:23:17.000000 customerio_cdp_analytics-0.0.2/customerio_cdp_analytics.egg-info/requires.txt
+-rw-r--r--   0 nunofgs    (501) staff       (20)       11 2023-08-03 09:23:17.000000 customerio_cdp_analytics-0.0.2/customerio_cdp_analytics.egg-info/top_level.txt
+-rw-r--r--   0 nunofgs    (501) staff       (20)       67 2023-08-03 09:23:17.961772 customerio_cdp_analytics-0.0.2/setup.cfg
+-rw-r--r--   0 nunofgs    (501) staff       (20)     1981 2023-08-03 09:12:00.000000 customerio_cdp_analytics-0.0.2/setup.py
```

### Comparing `customerio_cdp_analytics-0.0.1/LICENSE` & `customerio_cdp_analytics-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `customerio_cdp_analytics-0.0.1/PKG-INFO` & `customerio_cdp_analytics-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customerio_cdp_analytics
-Version: 0.0.1
+Version: 0.0.2
 Summary: Customer.io Data Pipelines (CDP) is a customer data platform to improve decision-making with real-time updates and deliver personalized experiences.
 Home-page: https://github.com/customerio/cdp-analytics-python
 Author: Customer.io
 Author-email: cdp@customer.io
 Maintainer: Customer.io
 Maintainer-email: cdp@customer.io
 License: MIT License
```

### Comparing `customerio_cdp_analytics-0.0.1/customerio/analytics/__init__.py` & `customerio_cdp_analytics-0.0.2/customerio/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `customerio_cdp_analytics-0.0.1/customerio/analytics/client.py` & `customerio_cdp_analytics-0.0.2/customerio/analytics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,14 @@
 
     def group(self, user_id=None, group_id=None, traits=None, context=None,
               timestamp=None, anonymous_id=None, integrations=None,
               message_id=None):
         traits = traits or {}
         context = context or {}
         integrations = integrations or {}
-        require('user_id or anonymous_id', user_id or anonymous_id, ID_TYPES)
         require('group_id', group_id, ID_TYPES)
         require('traits', traits, dict)
 
         msg = {
             'integrations': integrations,
             'anonymousId': anonymous_id,
             'timestamp': timestamp,
```

### Comparing `customerio_cdp_analytics-0.0.1/customerio/analytics/consumer.py` & `customerio_cdp_analytics-0.0.2/customerio/analytics/consumer.py`

 * *Files identical despite different names*

### Comparing `customerio_cdp_analytics-0.0.1/customerio/analytics/request.py` & `customerio_cdp_analytics-0.0.2/customerio/analytics/request.py`

 * *Files identical despite different names*

### Comparing `customerio_cdp_analytics-0.0.1/customerio/analytics/utils.py` & `customerio_cdp_analytics-0.0.2/customerio/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `customerio_cdp_analytics-0.0.1/customerio_cdp_analytics.egg-info/PKG-INFO` & `customerio_cdp_analytics-0.0.2/customerio_cdp_analytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customerio-cdp-analytics
-Version: 0.0.1
+Version: 0.0.2
 Summary: Customer.io Data Pipelines (CDP) is a customer data platform to improve decision-making with real-time updates and deliver personalized experiences.
 Home-page: https://github.com/customerio/cdp-analytics-python
 Author: Customer.io
 Author-email: cdp@customer.io
 Maintainer: Customer.io
 Maintainer-email: cdp@customer.io
 License: MIT License
```

### Comparing `customerio_cdp_analytics-0.0.1/setup.py` & `customerio_cdp_analytics-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     version=VERSION,
     url='https://github.com/customerio/cdp-analytics-python',
     author='Customer.io',
     author_email='cdp@customer.io',
     maintainer='Customer.io',
     maintainer_email='cdp@customer.io',
     test_suite='analytics.test.all',
-    packages=['customerio.analytics', 'analytics.test'],
+    packages=['customerio.analytics'],
     python_requires='>=3.6.0',
     license='MIT License',
     install_requires=install_requires,
     extras_require={
         'test': tests_require
     },
     description='Customer.io Data Pipelines (CDP) is a customer data platform to improve decision-making with real-time updates and deliver personalized experiences.',
```

