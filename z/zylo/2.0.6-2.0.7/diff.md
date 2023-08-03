# Comparing `tmp/zylo-2.0.6.tar.gz` & `tmp/zylo-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zylo-2.0.6.tar", last modified: Wed Aug  2 10:58:10 2023, max compression
+gzip compressed data, was "zylo-2.0.7.tar", last modified: Thu Aug  3 15:13:25 2023, max compression
```

## Comparing `zylo-2.0.6.tar` & `zylo-2.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 10:58:10.333855 zylo-2.0.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1857 2023-08-02 10:58:10.333855 zylo-2.0.6/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1268 2023-08-02 10:57:38.000000 zylo-2.0.6/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-08-02 10:58:10.333855 zylo-2.0.6/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2023-08-02 10:56:59.000000 zylo-2.0.6/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 10:58:10.317884 zylo-2.0.6/zylo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-30 03:14:13.000000 zylo-2.0.6/zylo/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 10:58:10.325869 zylo-2.0.6/zylo/components/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 11:07:00.000000 zylo-2.0.6/zylo/components/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2316 2023-07-27 11:14:32.000000 zylo-2.0.6/zylo/components/blueprint.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1268 2023-07-27 11:06:48.000000 zylo-2.0.6/zylo/components/sessions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 10:58:10.329862 zylo-2.0.6/zylo/contrib/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2403 2023-07-28 13:45:18.000000 zylo-2.0.6/zylo/contrib/BaseModal.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-30 11:32:27.000000 zylo-2.0.6/zylo/contrib/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 10:58:10.329862 zylo-2.0.6/zylo/contrib/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 11:24:53.000000 zylo-2.0.6/zylo/contrib/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1156 2023-07-27 11:24:47.000000 zylo-2.0.6/zylo/contrib/utils/limiter.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 10:58:10.329862 zylo-2.0.6/zylo/core/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 11:27:23.000000 zylo-2.0.6/zylo/core/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5497 2023-08-02 10:56:12.000000 zylo-2.0.6/zylo/core/branch.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 10:58:10.329862 zylo-2.0.6/zylo/mail/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 11:25:41.000000 zylo-2.0.6/zylo/mail/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3012 2023-07-28 15:15:20.000000 zylo-2.0.6/zylo/mail/zylo_mailer.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 10:58:10.333855 zylo-2.0.6/zylo/security/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7362 2023-07-27 11:24:02.000000 zylo-2.0.6/zylo/security/JwT.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 11:23:50.000000 zylo-2.0.6/zylo/security/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-07-27 11:26:09.000000 zylo-2.0.6/zylo/security/chiper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-02 10:58:10.325869 zylo-2.0.6/zylo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1857 2023-08-02 10:58:10.000000 zylo-2.0.6/zylo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      531 2023-08-02 10:58:10.000000 zylo-2.0.6/zylo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-08-02 10:58:10.000000 zylo-2.0.6/zylo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-08-02 10:58:10.000000 zylo-2.0.6/zylo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-08-02 10:58:10.000000 zylo-2.0.6/zylo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 15:13:25.272968 zylo-2.0.7/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1857 2023-08-03 15:13:25.272968 zylo-2.0.7/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1268 2023-08-03 13:22:54.000000 zylo-2.0.7/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-08-03 15:13:25.272968 zylo-2.0.7/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2023-08-03 13:23:00.000000 zylo-2.0.7/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 15:13:25.264968 zylo-2.0.7/zylo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-30 03:14:13.000000 zylo-2.0.7/zylo/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 15:13:25.268968 zylo-2.0.7/zylo/components/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 11:07:00.000000 zylo-2.0.7/zylo/components/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2316 2023-07-27 11:14:32.000000 zylo-2.0.7/zylo/components/blueprint.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1268 2023-07-27 11:06:48.000000 zylo-2.0.7/zylo/components/sessions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 15:13:25.268968 zylo-2.0.7/zylo/contrib/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2403 2023-07-28 13:45:18.000000 zylo-2.0.7/zylo/contrib/BaseModal.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-30 11:32:27.000000 zylo-2.0.7/zylo/contrib/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 15:13:25.272968 zylo-2.0.7/zylo/contrib/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 11:24:53.000000 zylo-2.0.7/zylo/contrib/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1156 2023-07-27 11:24:47.000000 zylo-2.0.7/zylo/contrib/utils/limiter.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 15:13:25.272968 zylo-2.0.7/zylo/core/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 11:27:23.000000 zylo-2.0.7/zylo/core/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5916 2023-08-03 13:22:37.000000 zylo-2.0.7/zylo/core/branch.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 15:13:25.272968 zylo-2.0.7/zylo/mail/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 11:25:41.000000 zylo-2.0.7/zylo/mail/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3012 2023-07-28 15:15:20.000000 zylo-2.0.7/zylo/mail/zylo_mailer.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 15:13:25.272968 zylo-2.0.7/zylo/security/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7362 2023-07-27 11:24:02.000000 zylo-2.0.7/zylo/security/JwT.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 11:23:50.000000 zylo-2.0.7/zylo/security/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-07-27 11:26:09.000000 zylo-2.0.7/zylo/security/chiper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 15:13:25.268968 zylo-2.0.7/zylo.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1857 2023-08-03 15:13:25.000000 zylo-2.0.7/zylo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      531 2023-08-03 15:13:25.000000 zylo-2.0.7/zylo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-08-03 15:13:25.000000 zylo-2.0.7/zylo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-08-03 15:13:25.000000 zylo-2.0.7/zylo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-08-03 15:13:25.000000 zylo-2.0.7/zylo.egg-info/top_level.txt
```

### Comparing `zylo-2.0.6/PKG-INFO` & `zylo-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 2.0.6
+Version: 2.0.7
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -52,24 +52,24 @@
 if __name__ == '__main__':
     app.run()
  
 ```
 
 ## changelogs
 
-- Beta version 2.0.6
+- Beta version 2.0.7
 - Latest update of beta
-- Bug fixed with update --> 2.0.6
+- Bug fixed with update --> 2.0.7
 - Updated Usage Guide 1.2.2
 - Newly designed system based on Matrix 1.0.0 Metapolist
 - Major Bug fixies in zylo
 - No longer support for version 1 beta --> # clearout
 - Attractive echosystem in zylo
 - Freshly updated Mailer, Blueprint, Sessions, Chiper, JwT, BaseModals, Zylo
-- Strict route has been removed in version --> 2.0.6
+- Strict route has been removed in version --> 2.0.7
 - Added battries support usign ZyloAdmin 
 
 ## Usage Guide
 
 Our team working hard and the usage guide will be avilable within 24hrs on http://zylo.vvfin.in or https://github.com/E491K8/ZyloProject/
 
 ## Batteries Support
```

### Comparing `zylo-2.0.6/README.md` & `zylo-2.0.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -36,24 +36,24 @@
 if __name__ == '__main__':
     app.run()
  
 ```
 
 ## changelogs
 
-- Beta version 2.0.6
+- Beta version 2.0.7
 - Latest update of beta
-- Bug fixed with update --> 2.0.6
+- Bug fixed with update --> 2.0.7
 - Updated Usage Guide 1.2.2
 - Newly designed system based on Matrix 1.0.0 Metapolist
 - Major Bug fixies in zylo
 - No longer support for version 1 beta --> # clearout
 - Attractive echosystem in zylo
 - Freshly updated Mailer, Blueprint, Sessions, Chiper, JwT, BaseModals, Zylo
-- Strict route has been removed in version --> 2.0.6
+- Strict route has been removed in version --> 2.0.7
 - Added battries support usign ZyloAdmin 
 
 ## Usage Guide
 
 Our team working hard and the usage guide will be avilable within 24hrs on http://zylo.vvfin.in or https://github.com/E491K8/ZyloProject/
 
 ## Batteries Support
```

### Comparing `zylo-2.0.6/setup.py` & `zylo-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='zylo',
-    version='2.0.6',
+    version='2.0.7',
     description='A lightweight web framework made with love',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Pawan kumar',
     author_email='control@vvfin.in',
     url='https://github.com/E491K7/zylo',
     packages=find_packages(),
```

### Comparing `zylo-2.0.6/zylo/components/blueprint.py` & `zylo-2.0.7/zylo/components/blueprint.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.6/zylo/components/sessions.py` & `zylo-2.0.7/zylo/components/sessions.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.6/zylo/contrib/BaseModal.py` & `zylo-2.0.7/zylo/contrib/BaseModal.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.6/zylo/contrib/utils/limiter.py` & `zylo-2.0.7/zylo/contrib/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.6/zylo/core/branch.py` & `zylo-2.0.7/zylo/core/branch.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,14 +70,25 @@
         return decorator
 
     def use(self, middleware):
         self.middlewares.append(middleware)
 
     def config(self):
         return self.config
+    
+    def url_for_static(self, filename):
+        return f'/static/{filename}'
+
+    def serve_static(self, filename):
+        static_path = os.path.join(self.static_folder, filename)
+        if os.path.isfile(static_path):
+            mimetype, _ = mimetypes.guess_type(static_path)
+            if mimetype:
+                return Response(open(static_path, 'rb').read(), mimetype=mimetype)
+        raise NotFound()
 
     def register_blueprint(self, blueprint):
         self.blueprints.append(blueprint)
 
     def handle_request(self, request):
         adapter = self.url_map.bind_to_environ(request.environ)
         try:
```

### Comparing `zylo-2.0.6/zylo/mail/zylo_mailer.py` & `zylo-2.0.7/zylo/mail/zylo_mailer.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.6/zylo/security/JwT.py` & `zylo-2.0.7/zylo/security/JwT.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.6/zylo/security/chiper.py` & `zylo-2.0.7/zylo/security/chiper.py`

 * *Files identical despite different names*

### Comparing `zylo-2.0.6/zylo.egg-info/PKG-INFO` & `zylo-2.0.7/zylo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 2.0.6
+Version: 2.0.7
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -52,24 +52,24 @@
 if __name__ == '__main__':
     app.run()
  
 ```
 
 ## changelogs
 
-- Beta version 2.0.6
+- Beta version 2.0.7
 - Latest update of beta
-- Bug fixed with update --> 2.0.6
+- Bug fixed with update --> 2.0.7
 - Updated Usage Guide 1.2.2
 - Newly designed system based on Matrix 1.0.0 Metapolist
 - Major Bug fixies in zylo
 - No longer support for version 1 beta --> # clearout
 - Attractive echosystem in zylo
 - Freshly updated Mailer, Blueprint, Sessions, Chiper, JwT, BaseModals, Zylo
-- Strict route has been removed in version --> 2.0.6
+- Strict route has been removed in version --> 2.0.7
 - Added battries support usign ZyloAdmin 
 
 ## Usage Guide
 
 Our team working hard and the usage guide will be avilable within 24hrs on http://zylo.vvfin.in or https://github.com/E491K8/ZyloProject/
 
 ## Batteries Support
```

### Comparing `zylo-2.0.6/zylo.egg-info/SOURCES.txt` & `zylo-2.0.7/zylo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

