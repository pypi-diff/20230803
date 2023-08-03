# Comparing `tmp/jet-django-1.7.9.tar.gz` & `tmp/jet-django-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jet-django-1.7.9.tar", last modified: Thu Mar 16 07:39:33 2023, max compression
+gzip compressed data, was "dist/jet-django-1.8.2.tar", last modified: Thu Aug  3 11:16:36 2023, max compression
```

## Comparing `jet-django-1.7.9.tar` & `jet-django-1.8.2.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:33.000000 jet-django-1.7.9/
--rw-r--r--   0 f1nal      (501) staff       (20)     3925 2023-03-16 07:39:33.000000 jet-django-1.7.9/PKG-INFO
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-django-1.7.9/LICENSE
--rw-r--r--   0 f1nal      (501) staff       (20)       66 2021-08-25 15:07:30.000000 jet-django-1.7.9/MANIFEST.in
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django.egg-info/
--rw-r--r--   0 f1nal      (501) staff       (20)     3925 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django.egg-info/PKG-INFO
--rw-r--r--   0 f1nal      (501) staff       (20)        1 2021-08-26 13:49:12.000000 jet-django-1.7.9/jet_django.egg-info/not-zip-safe
--rw-r--r--   0 f1nal      (501) staff       (20)     1219 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django.egg-info/SOURCES.txt
--rw-r--r--   0 f1nal      (501) staff       (20)       39 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django.egg-info/requires.txt
--rw-r--r--   0 f1nal      (501) staff       (20)       11 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django.egg-info/top_level.txt
--rw-r--r--   0 f1nal      (501) staff       (20)        1 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django.egg-info/dependency_links.txt
--rw-r--r--   0 f1nal      (501) staff       (20)      973 2023-03-16 02:56:11.000000 jet-django-1.7.9/setup.py
--rw-r--r--   0 f1nal      (501) staff       (20)       38 2023-03-16 07:39:33.000000 jet-django-1.7.9/setup.cfg
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django/
--rw-r--r--   0 f1nal      (501) staff       (20)    13442 2023-02-14 16:01:58.000000 jet-django-1.7.9/jet_django/configuration.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django/migrations/
--rw-r--r--   0 f1nal      (501) staff       (20)      761 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/0002_auto_20181014_2002.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django/migrations/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     2338 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      789 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/__pycache__/0002_auto_20181014_2002.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1432 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/__pycache__/0003_auto_20191007_2005.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      207 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1218 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/0003_auto_20191007_2005.py
--rw-r--r--   0 f1nal      (501) staff       (20)     5152 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/migrations/0001_initial.py
--rw-r--r--   0 f1nal      (501) staff       (20)       73 2023-03-16 02:56:11.000000 jet-django-1.7.9/jet_django/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     5807 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/__pycache__/route_view.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2359 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/__pycache__/settings.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2941 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/__pycache__/urls.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)    13595 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/__pycache__/configuration.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      244 2023-03-16 07:39:33.000000 jet-django-1.7.9/jet_django/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3329 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/__pycache__/router.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1080 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/__pycache__/apps.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      254 2022-11-13 04:37:35.000000 jet-django-1.7.9/jet_django/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      708 2022-11-13 04:35:29.000000 jet-django-1.7.9/jet_django/apps.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3480 2023-02-14 16:01:58.000000 jet-django-1.7.9/jet_django/settings.py
--rw-r--r--   0 f1nal      (501) staff       (20)     4989 2023-02-14 16:01:58.000000 jet-django-1.7.9/jet_django/route_view.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3446 2023-02-14 16:01:58.000000 jet-django-1.7.9/jet_django/router.py
--rw-r--r--   0 f1nal      (501) staff       (20)     4845 2023-02-14 16:01:58.000000 jet-django-1.7.9/jet_django/urls.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3689 2021-08-25 15:07:30.000000 jet-django-1.7.9/README.rst
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:36.000000 jet-django-1.8.2/
+-rw-r--r--   0 f1nal      (501) staff       (20)     3926 2023-08-03 11:16:36.000000 jet-django-1.8.2/PKG-INFO
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-django-1.8.2/LICENSE
+-rw-r--r--   0 f1nal      (501) staff       (20)       66 2021-08-25 15:07:30.000000 jet-django-1.8.2/MANIFEST.in
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:36.000000 jet-django-1.8.2/jet_django.egg-info/
+-rw-r--r--   0 f1nal      (501) staff       (20)     3926 2023-08-03 11:16:36.000000 jet-django-1.8.2/jet_django.egg-info/PKG-INFO
+-rw-r--r--   0 f1nal      (501) staff       (20)        1 2021-08-26 13:49:12.000000 jet-django-1.8.2/jet_django.egg-info/not-zip-safe
+-rw-r--r--   0 f1nal      (501) staff       (20)     1266 2023-08-03 11:16:36.000000 jet-django-1.8.2/jet_django.egg-info/SOURCES.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)       39 2023-08-03 11:16:36.000000 jet-django-1.8.2/jet_django.egg-info/requires.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)       11 2023-08-03 11:16:36.000000 jet-django-1.8.2/jet_django.egg-info/top_level.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)        1 2023-08-03 11:16:36.000000 jet-django-1.8.2/jet_django.egg-info/dependency_links.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)      973 2023-08-03 09:34:59.000000 jet-django-1.8.2/setup.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       38 2023-08-03 11:16:36.000000 jet-django-1.8.2/setup.cfg
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:36.000000 jet-django-1.8.2/jet_django/
+-rw-r--r--   0 f1nal      (501) staff       (20)    13755 2023-07-27 17:20:08.000000 jet-django-1.8.2/jet_django/configuration.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:36.000000 jet-django-1.8.2/jet_django/migrations/
+-rw-r--r--   0 f1nal      (501) staff       (20)      761 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/migrations/0002_auto_20181014_2002.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/migrations/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:36.000000 jet-django-1.8.2/jet_django/migrations/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     2338 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      789 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/migrations/__pycache__/0002_auto_20181014_2002.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1432 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/migrations/__pycache__/0003_auto_20191007_2005.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      207 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1218 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/migrations/0003_auto_20191007_2005.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     5152 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/migrations/0001_initial.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       73 2023-08-03 09:34:59.000000 jet-django-1.8.2/jet_django/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2023-08-03 11:16:36.000000 jet-django-1.8.2/jet_django/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     5807 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/__pycache__/route_view.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2359 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/__pycache__/settings.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2941 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/__pycache__/urls.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)    13595 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/__pycache__/configuration.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      244 2023-08-03 11:16:36.000000 jet-django-1.8.2/jet_django/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3329 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/__pycache__/router.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1080 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/__pycache__/apps.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      249 2023-04-20 15:52:45.000000 jet-django-1.8.2/jet_django/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      254 2022-11-13 04:37:35.000000 jet-django-1.8.2/jet_django/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      708 2022-11-13 04:35:29.000000 jet-django-1.8.2/jet_django/apps.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3836 2023-07-27 17:20:08.000000 jet-django-1.8.2/jet_django/settings.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     4989 2023-02-14 16:01:58.000000 jet-django-1.8.2/jet_django/route_view.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3446 2023-02-14 16:01:58.000000 jet-django-1.8.2/jet_django/router.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     4845 2023-02-14 16:01:58.000000 jet-django-1.8.2/jet_django/urls.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3690 2023-04-21 03:52:47.000000 jet-django-1.8.2/README.rst
```

### Comparing `jet-django-1.7.9/PKG-INFO` & `jet-django-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jet-django
-Version: 1.7.9
+Version: 1.8.2
 Summary: UNKNOWN
 Home-page: https://github.com/jet-admin/jet-django
 Author: Denis Kildishev
 Author-email: hello@geex-arts.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENSE
@@ -20,15 +20,15 @@
     :align: center
     :target: https://s3.us-west-2.amazonaws.com/secure.notion-static.com/079701bd-ea68-4848-a885-d19518cfa746/main.gif?AWSAccessKeyId=AKIAJLJXUMP5IHUZAPFQ&Expires=1539710956&Signature=zSY1L770Uu0gCtG72%2FAGE8rm9G0%3D
 
 Description
 ===========
 
 * Jet Admin: https://www.jetadmin.io
-* **Live Demo**: http://app.jetadmin.io/demo
+* **Live Demo**: https://app.jetadmin.io/demo
 * Support: support@jetadmin.io
 
 **Jet** is a SaaS service that automatically generates back office for your Django Application through REST API of **Jet Bridge** package installed to your project.
 
 – **Visual**. Admin interface can be easily changed without need of development with the help of Visual Editor. 
 
 – **Secure**. Jet does not access your data: its transferred directly from browser to your application.
```

### Comparing `jet-django-1.7.9/jet_django.egg-info/PKG-INFO` & `jet-django-1.8.2/jet_django.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jet-django
-Version: 1.7.9
+Version: 1.8.2
 Summary: UNKNOWN
 Home-page: https://github.com/jet-admin/jet-django
 Author: Denis Kildishev
 Author-email: hello@geex-arts.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENSE
@@ -20,15 +20,15 @@
     :align: center
     :target: https://s3.us-west-2.amazonaws.com/secure.notion-static.com/079701bd-ea68-4848-a885-d19518cfa746/main.gif?AWSAccessKeyId=AKIAJLJXUMP5IHUZAPFQ&Expires=1539710956&Signature=zSY1L770Uu0gCtG72%2FAGE8rm9G0%3D
 
 Description
 ===========
 
 * Jet Admin: https://www.jetadmin.io
-* **Live Demo**: http://app.jetadmin.io/demo
+* **Live Demo**: https://app.jetadmin.io/demo
 * Support: support@jetadmin.io
 
 **Jet** is a SaaS service that automatically generates back office for your Django Application through REST API of **Jet Bridge** package installed to your project.
 
 – **Visual**. Admin interface can be easily changed without need of development with the help of Visual Editor. 
 
 – **Secure**. Jet does not access your data: its transferred directly from browser to your application.
```

### Comparing `jet-django-1.7.9/jet_django.egg-info/SOURCES.txt` & `jet-django-1.8.2/jet_django.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 jet_django.egg-info/SOURCES.txt
 jet_django.egg-info/dependency_links.txt
 jet_django.egg-info/not-zip-safe
 jet_django.egg-info/requires.txt
 jet_django.egg-info/top_level.txt
 jet_django/__pycache__/__init__.cpython-310.pyc
 jet_django/__pycache__/__init__.cpython-36.pyc
+jet_django/__pycache__/__init__.cpython-37.pyc
 jet_django/__pycache__/apps.cpython-310.pyc
 jet_django/__pycache__/configuration.cpython-310.pyc
 jet_django/__pycache__/route_view.cpython-310.pyc
 jet_django/__pycache__/router.cpython-310.pyc
 jet_django/__pycache__/settings.cpython-310.pyc
 jet_django/__pycache__/urls.cpython-310.pyc
 jet_django/migrations/0001_initial.py
```

### Comparing `jet-django-1.7.9/setup.py` & `jet-django-1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     return file.read()
 
 
 def get_install_requires():
     install_requires = [
         'Django',
         'requests',
-        'jet-bridge-base==1.7.9',
+        'jet-bridge-base==1.8.2',
     ]
 
     try:
         from collections import OrderedDict
     except ImportError:
         install_requires.append('ordereddict')
```

### Comparing `jet-django-1.7.9/jet_django/configuration.py` & `jet-django-1.8.2/jet_django/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,19 @@
             'DATABASE_PASSWORD': settings.database_settings.get('PASSWORD'),
             'DATABASE_NAME': str(settings.database_settings['NAME'])
                 if settings.database_settings.get('NAME') is not None else None,
             'DATABASE_EXTRA': settings.JET_DATABASE_EXTRA,
             'DATABASE_CONNECTIONS': 1,
             'DATABASE_ONLY': settings.JET_DATABASE_ONLY,
             'DATABASE_EXCEPT': settings.JET_DATABASE_EXCEPT,
+            'DATABASE_MAX_TABLES': settings.JET_DATABASE_MAX_TABLES,
             'DATABASE_SCHEMA': settings.JET_DATABASE_SCHEMA,
+            'DATABASE_SSL_CA': settings.JET_DATABASE_SSL_CA,
+            'DATABASE_SSL_CERT': settings.JET_DATABASE_SSL_CERT,
+            'DATABASE_SSL_KEY': settings.JET_DATABASE_SSL_KEY,
             'DATABASE_SSH_HOST': settings.JET_DATABASE_SSH_HOST,
             'DATABASE_SSH_PORT': settings.JET_DATABASE_SSH_PORT,
             'DATABASE_SSH_USER': settings.JET_DATABASE_SSH_USER,
             'DATABASE_SSH_PRIVATE_KEY': settings.JET_DATABASE_SSH_PRIVATE_KEY,
             'COOKIE_SAMESITE': settings.JET_COOKIE_SAMESITE,
             'COOKIE_SECURE': settings.JET_COOKIE_SECURE,
             'COOKIE_DOMAIN': settings.JET_COOKIE_DOMAIN,
@@ -85,15 +89,16 @@
             'STORE_PATH': settings.JET_STORE_PATH,
             'SSO_APPLICATIONS': self.clean_sso_applications(settings.JET_SSO_APPLICATIONS),
             'ALLOW_ORIGIN': settings.JET_ALLOW_ORIGIN,
             'TRACK_DATABASES': settings.JET_TRACK_DATABASES,
             'TRACK_DATABASES_ENDPOINT': settings.JET_TRACK_DATABASES_ENDPOINT,
             'TRACK_DATABASES_AUTH': settings.JET_TRACK_DATABASES_AUTH,
             'TRACK_MODELS_ENDPOINT': settings.JET_TRACK_MODELS_ENDPOINT,
-            'TRACK_MODELS_AUTH': settings.JET_TRACK_MODELS_AUTH
+            'TRACK_MODELS_AUTH': settings.JET_TRACK_MODELS_AUTH,
+            'DISABLE_AUTH': settings.JET_DISABLE_AUTH
         }
 
     def get_django_instance(self, model, instance):
         model_cls = self.model_classes.get(model)
         pk = model_cls._meta.pk.column
         if getattr(instance, pk):
             return model_cls, model_cls.objects.get(pk=getattr(instance, pk))
```

### Comparing `jet-django-1.7.9/jet_django/migrations/0002_auto_20181014_2002.py` & `jet-django-1.8.2/jet_django/migrations/0002_auto_20181014_2002.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/migrations/__pycache__/0001_initial.cpython-310.pyc` & `jet-django-1.8.2/jet_django/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/migrations/__pycache__/0002_auto_20181014_2002.cpython-310.pyc` & `jet-django-1.8.2/jet_django/migrations/__pycache__/0002_auto_20181014_2002.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/migrations/__pycache__/0003_auto_20191007_2005.cpython-310.pyc` & `jet-django-1.8.2/jet_django/migrations/__pycache__/0003_auto_20191007_2005.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/migrations/0003_auto_20191007_2005.py` & `jet-django-1.8.2/jet_django/migrations/0003_auto_20191007_2005.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/migrations/0001_initial.py` & `jet-django-1.8.2/jet_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/__pycache__/route_view.cpython-310.pyc` & `jet-django-1.8.2/jet_django/__pycache__/route_view.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/__pycache__/settings.cpython-310.pyc` & `jet-django-1.8.2/jet_django/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/__pycache__/urls.cpython-310.pyc` & `jet-django-1.8.2/jet_django/__pycache__/urls.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/__pycache__/configuration.cpython-310.pyc` & `jet-django-1.8.2/jet_django/__pycache__/configuration.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/__pycache__/router.cpython-310.pyc` & `jet-django-1.8.2/jet_django/__pycache__/router.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/__pycache__/apps.cpython-310.pyc` & `jet-django-1.8.2/jet_django/__pycache__/apps.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/apps.py` & `jet-django-1.8.2/jet_django/apps.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/settings.py` & `jet-django-1.8.2/jet_django/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,16 +21,21 @@
 
 JET_MEDIA_FILE_STORAGE = getattr(settings, 'JET_MEDIA_FILE_STORAGE', settings.DEFAULT_FILE_STORAGE)
 
 JET_DJANGO_DATABASE = getattr(settings, 'JET_DJANGO_DATABASE', 'default')
 JET_DATABASE_EXTRA = getattr(settings, 'JET_DATABASE_EXTRA', None)
 JET_DATABASE_ONLY = getattr(settings, 'JET_DATABASE_ONLY', None)
 JET_DATABASE_EXCEPT = getattr(settings, 'JET_DATABASE_EXCEPT', None)
+JET_DATABASE_MAX_TABLES = getattr(settings, 'JET_DATABASE_MAX_TABLES', None)
 JET_DATABASE_SCHEMA = getattr(settings, 'JET_DATABASE_SCHEMA', None)
 
+JET_DATABASE_SSL_CA = getattr(settings, 'JET_DATABASE_SSL_CA', None)
+JET_DATABASE_SSL_CERT = getattr(settings, 'JET_DATABASE_SSL_CERT', None)
+JET_DATABASE_SSL_KEY = getattr(settings, 'JET_DATABASE_SSL_KEY', None)
+
 JET_DATABASE_SSH_HOST = getattr(settings, 'JET_DATABASE_SSH_HOST', None)
 JET_DATABASE_SSH_PORT = getattr(settings, 'JET_DATABASE_SSH_PORT', None)
 JET_DATABASE_SSH_USER = getattr(settings, 'JET_DATABASE_SSH_USER', None)
 JET_DATABASE_SSH_PRIVATE_KEY = getattr(settings, 'JET_DATABASE_SSH_PRIVATE_KEY', None)
 
 JET_COOKIE_SAMESITE = getattr(settings, 'JET_COOKIE_SAMESITE', 'None')
 JET_COOKIE_SECURE = getattr(settings, 'JET_COOKIE_SECURE', True)
@@ -45,14 +50,16 @@
 JET_TRACK_DATABASES = getattr(settings, 'JET_TRACK_DATABASES', '')
 JET_TRACK_DATABASES_ENDPOINT = getattr(settings, 'JET_TRACK_DATABASES_ENDPOINT', '')
 JET_TRACK_DATABASES_AUTH = getattr(settings, 'JET_TRACK_DATABASES_AUTH', '')
 
 JET_TRACK_MODELS_ENDPOINT = getattr(settings, 'JET_TRACK_MODELS_ENDPOINT', '')
 JET_TRACK_MODELS_AUTH = getattr(settings, 'JET_TRACK_MODELS_AUTH', '')
 
+JET_DISABLE_AUTH = getattr(settings, 'JET_DISABLE_AUTH', False)
+
 try:
     JET_SSO_APPLICATIONS = json.loads(JET_SSO_APPLICATIONS)
 except Exception as e:
     logger.error('SSO_APPLICATIONS parsing failed', exc_info=e)
     JET_SSO_APPLICATIONS = {}
 
 database_settings = settings.DATABASES.get(JET_DJANGO_DATABASE, {})
```

### Comparing `jet-django-1.7.9/jet_django/route_view.py` & `jet-django-1.8.2/jet_django/route_view.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/router.py` & `jet-django-1.8.2/jet_django/router.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/jet_django/urls.py` & `jet-django-1.8.2/jet_django/urls.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.7.9/README.rst` & `jet-django-1.8.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     :align: center
     :target: https://s3.us-west-2.amazonaws.com/secure.notion-static.com/079701bd-ea68-4848-a885-d19518cfa746/main.gif?AWSAccessKeyId=AKIAJLJXUMP5IHUZAPFQ&Expires=1539710956&Signature=zSY1L770Uu0gCtG72%2FAGE8rm9G0%3D
 
 Description
 ===========
 
 * Jet Admin: https://www.jetadmin.io
-* **Live Demo**: http://app.jetadmin.io/demo
+* **Live Demo**: https://app.jetadmin.io/demo
 * Support: support@jetadmin.io
 
 **Jet** is a SaaS service that automatically generates back office for your Django Application through REST API of **Jet Bridge** package installed to your project.
 
 – **Visual**. Admin interface can be easily changed without need of development with the help of Visual Editor. 
 
 – **Secure**. Jet does not access your data: its transferred directly from browser to your application.
```

