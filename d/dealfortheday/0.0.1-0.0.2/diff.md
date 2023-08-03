# Comparing `tmp/dealfortheday-0.0.1.tar.gz` & `tmp/dealfortheday-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dealfortheday-0.0.1.tar", last modified: Thu Aug  3 19:53:54 2023, max compression
+gzip compressed data, was "dealfortheday-0.0.2.tar", last modified: Thu Aug  3 20:18:35 2023, max compression
```

## Comparing `dealfortheday-0.0.1.tar` & `dealfortheday-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 19:53:54.732165 dealfortheday-0.0.1/
--rw-rw-rw-   0        0        0       76 2023-08-03 17:27:13.000000 dealfortheday-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1075 2023-08-03 17:28:09.000000 dealfortheday-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-08-03 17:23:10.000000 dealfortheday-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      709 2023-08-03 19:53:54.731185 dealfortheday-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       97 2023-08-03 17:29:08.000000 dealfortheday-0.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 19:53:54.684174 dealfortheday-0.0.1/dealfortheday/
--rw-rw-rw-   0        0        0        0 2023-08-03 19:46:34.000000 dealfortheday-0.0.1/dealfortheday/__init__.py
--rw-rw-rw-   0        0        0      733 2023-08-03 19:51:24.000000 dealfortheday-0.0.1/dealfortheday/mydealfortheday.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:53:54.728184 dealfortheday-0.0.1/dealfortheday.egg-info/
--rw-rw-rw-   0        0        0      709 2023-08-03 19:53:54.000000 dealfortheday-0.0.1/dealfortheday.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-08-03 19:53:54.000000 dealfortheday-0.0.1/dealfortheday.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 19:53:54.000000 dealfortheday-0.0.1/dealfortheday.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-08-03 19:53:54.000000 dealfortheday-0.0.1/dealfortheday.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 19:53:54.732165 dealfortheday-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      726 2023-08-03 19:52:53.000000 dealfortheday-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:18:35.098287 dealfortheday-0.0.2/
+-rw-rw-rw-   0        0        0      129 2023-08-03 20:17:41.000000 dealfortheday-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1075 2023-08-03 17:28:09.000000 dealfortheday-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-08-03 17:23:10.000000 dealfortheday-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      762 2023-08-03 20:18:35.097286 dealfortheday-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       97 2023-08-03 17:29:08.000000 dealfortheday-0.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 20:18:35.070283 dealfortheday-0.0.2/dealfortheday/
+-rw-rw-rw-   0        0        0        0 2023-08-03 19:46:34.000000 dealfortheday-0.0.2/dealfortheday/__init__.py
+-rw-rw-rw-   0        0        0     1239 2023-08-03 20:16:33.000000 dealfortheday-0.0.2/dealfortheday/mydealfortheday.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:18:35.095288 dealfortheday-0.0.2/dealfortheday.egg-info/
+-rw-rw-rw-   0        0        0      762 2023-08-03 20:18:34.000000 dealfortheday-0.0.2/dealfortheday.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-08-03 20:18:34.000000 dealfortheday-0.0.2/dealfortheday.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 20:18:34.000000 dealfortheday-0.0.2/dealfortheday.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-03 20:18:34.000000 dealfortheday-0.0.2/dealfortheday.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 20:18:35.099288 dealfortheday-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      726 2023-08-03 20:17:25.000000 dealfortheday-0.0.2/setup.py
```

### Comparing `dealfortheday-0.0.1/LICENCE.txt` & `dealfortheday-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dealfortheday-0.0.1/PKG-INFO` & `dealfortheday-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dealfortheday
-Version: 0.0.1
+Version: 0.0.2
 Summary: deal of the day generator
 Home-page: 
 Author: Prakash Shankar Mishra
 Author-email: x21172684@student.ncirl.ie
 License: MIT
 Keywords: dealforthedaygenerator
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,7 +18,11 @@
 
 Change log
 ===========
 
 0.0.1 (25/07/23)
 ----------------
 First Release
+
+0.0.2 (25/07/23)
+----------------
+First Release
```

### Comparing `dealfortheday-0.0.1/dealfortheday/mydealfortheday.py` & `dealfortheday-0.0.2/dealfortheday/mydealfortheday.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,33 @@
+# dealfortheday/mydealfortheday.py
+
 import random
+import datetime
 
-def getDealForTheDay(allProducts):
+def getDealForTheDay(allProducts, request):
     """
     Randomly selects a "Deal of the Day" from the available products.
 
     Parameters:
         allProducts (list): A list of strings representing the names of all available products.
+        request: The Django request object.
 
     Returns:
         str: The name of the selected product as the "Deal of the Day."
     """
     if not isinstance(allProducts, list) or not all(isinstance(product, str) for product in allProducts):
         raise ValueError("allProducts must be a list of strings representing the names of available products.")
 
     if not allProducts:
         raise ValueError("allProducts list must not be empty.")
 
-    dealOfTheDay = random.choice(allProducts)
-    return dealOfTheDay
+    deal_of_the_day_key = 'deal_of_the_day'
+    current_date = datetime.date.today()
+
+    if deal_of_the_day_key not in request.session or request.session.get('deal_date') != current_date:
+        deal_of_the_day = random.choice(allProducts)
+        request.session[deal_of_the_day_key] = deal_of_the_day
+        request.session['deal_date'] = current_date
+    else:
+        deal_of_the_day = request.session[deal_of_the_day_key]
+
+    return deal_of_the_day
```

### Comparing `dealfortheday-0.0.1/dealfortheday.egg-info/PKG-INFO` & `dealfortheday-0.0.2/dealfortheday.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dealfortheday
-Version: 0.0.1
+Version: 0.0.2
 Summary: deal of the day generator
 Home-page: 
 Author: Prakash Shankar Mishra
 Author-email: x21172684@student.ncirl.ie
 License: MIT
 Keywords: dealforthedaygenerator
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,7 +18,11 @@
 
 Change log
 ===========
 
 0.0.1 (25/07/23)
 ----------------
 First Release
+
+0.0.2 (25/07/23)
+----------------
+First Release
```

### Comparing `dealfortheday-0.0.1/setup.py` & `dealfortheday-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='dealfortheday',
-  version='0.0.1',
+  version='0.0.2',
   description='deal of the day generator',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Prakash Shankar Mishra',
   author_email='x21172684@student.ncirl.ie',
   license='MIT', 
   classifiers=classifiers,
```

