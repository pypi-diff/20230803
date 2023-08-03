# Comparing `tmp/django-silly-stripe-1.0.2.tar.gz` & `tmp/django-silly-stripe-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-silly-stripe-1.0.2.tar", last modified: Mon Jul 31 14:28:20 2023, max compression
+gzip compressed data, was "django-silly-stripe-1.0.3.tar", last modified: Thu Aug  3 16:13:07 2023, max compression
```

## Comparing `django-silly-stripe-1.0.2.tar` & `django-silly-stripe-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:28:20.297106 django-silly-stripe-1.0.2/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-stripe-1.0.2/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1727 2023-07-31 14:28:20.297106 django-silly-stripe-1.0.2/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1104 2023-07-27 19:14:42.000000 django-silly-stripe-1.0.2/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:28:20.289106 django-silly-stripe-1.0.2/django_silly_stripe/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       52 2023-07-31 14:25:00.000000 django-silly-stripe-1.0.2/django_silly_stripe/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1973 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.2/django_silly_stripe/admin.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1406 2023-07-27 19:43:59.000000 django-silly-stripe-1.0.2/django_silly_stripe/conf.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      942 2023-07-27 19:14:42.000000 django-silly-stripe-1.0.2/django_silly_stripe/helpers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:28:20.293106 django-silly-stripe-1.0.2/django_silly_stripe/migrations/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      931 2023-07-16 19:12:41.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0001_initial.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      620 2023-07-17 19:35:25.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0002_alter_customer_user.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      552 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0003_remove_customer_stripe_id_alter_customer_id.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      458 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0004_customer_email.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      414 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0005_customer_name.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1889 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0006_product_price.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      398 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0007_price_metadata.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      868 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0008_subscription.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      814 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0009_subscription_end_time_subscription_start_time_and_more.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      603 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0010_alter_subscription_end_time_and_more.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      435 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0011_subscription_cancel_at_period_end.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-12 12:59:48.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3428 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.2/django_silly_stripe/models.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:28:20.293106 django-silly-stripe-1.0.2/django_silly_stripe/templates/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:26:16.000000 django-silly-stripe-1.0.2/django_silly_stripe/templates/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:28:20.297106 django-silly-stripe-1.0.2/django_silly_stripe/templates/admin/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:26:01.000000 django-silly-stripe-1.0.2/django_silly_stripe/templates/admin/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     6732 2023-07-25 12:20:33.000000 django-silly-stripe-1.0.2/django_silly_stripe/templates/admin/base.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2203 2023-07-27 16:54:42.000000 django-silly-stripe-1.0.2/django_silly_stripe/urls.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     8757 2023-07-27 19:42:29.000000 django-silly-stripe-1.0.2/django_silly_stripe/views.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:28:20.293106 django-silly-stripe-1.0.2/django_silly_stripe.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1727 2023-07-31 14:28:20.000000 django-silly-stripe-1.0.2/django_silly_stripe.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1327 2023-07-31 14:28:20.000000 django-silly-stripe-1.0.2/django_silly_stripe.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-07-31 14:28:20.000000 django-silly-stripe-1.0.2/django_silly_stripe.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       14 2023-07-31 14:28:20.000000 django-silly-stripe-1.0.2/django_silly_stripe.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       20 2023-07-31 14:28:20.000000 django-silly-stripe-1.0.2/django_silly_stripe.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-07-31 14:28:20.297106 django-silly-stripe-1.0.2/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1772 2023-07-31 14:28:03.000000 django-silly-stripe-1.0.2/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-03 16:13:07.174409 django-silly-stripe-1.0.3/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-stripe-1.0.3/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      869 2023-08-03 16:13:07.174409 django-silly-stripe-1.0.3/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      246 2023-08-01 21:29:17.000000 django-silly-stripe-1.0.3/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-03 16:13:07.166410 django-silly-stripe-1.0.3/django_silly_stripe/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       52 2023-08-01 15:29:31.000000 django-silly-stripe-1.0.3/django_silly_stripe/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1973 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.3/django_silly_stripe/admin.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1495 2023-08-03 15:17:42.000000 django-silly-stripe-1.0.3/django_silly_stripe/conf.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1446 2023-08-03 15:22:25.000000 django-silly-stripe-1.0.3/django_silly_stripe/helpers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-03 16:13:07.174409 django-silly-stripe-1.0.3/django_silly_stripe/migrations/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      931 2023-07-16 19:12:41.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0001_initial.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      620 2023-07-17 19:35:25.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0002_alter_customer_user.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      552 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0003_remove_customer_stripe_id_alter_customer_id.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      458 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0004_customer_email.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      414 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0005_customer_name.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1889 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0006_product_price.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      398 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0007_price_metadata.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      868 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0008_subscription.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      814 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0009_subscription_end_time_subscription_start_time_and_more.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      603 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0010_alter_subscription_end_time_and_more.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      435 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0011_subscription_cancel_at_period_end.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-12 12:59:48.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3428 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.3/django_silly_stripe/models.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      718 2023-08-01 16:22:24.000000 django-silly-stripe-1.0.3/django_silly_stripe/serializers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-03 16:13:07.174409 django-silly-stripe-1.0.3/django_silly_stripe/templates/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:29:24.000000 django-silly-stripe-1.0.3/django_silly_stripe/templates/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-03 16:13:07.174409 django-silly-stripe-1.0.3/django_silly_stripe/templates/admin/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:29:24.000000 django-silly-stripe-1.0.3/django_silly_stripe/templates/admin/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6732 2023-07-25 12:20:33.000000 django-silly-stripe-1.0.3/django_silly_stripe/templates/admin/base.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2203 2023-07-27 16:54:42.000000 django-silly-stripe-1.0.3/django_silly_stripe/urls.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4149 2023-08-03 15:44:26.000000 django-silly-stripe-1.0.3/django_silly_stripe/views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5982 2023-08-03 15:27:58.000000 django-silly-stripe-1.0.3/django_silly_stripe/views_api.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5268 2023-08-01 18:07:11.000000 django-silly-stripe-1.0.3/django_silly_stripe/views_classic.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-03 16:13:07.170410 django-silly-stripe-1.0.3/django_silly_stripe.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      869 2023-08-03 16:13:07.000000 django-silly-stripe-1.0.3/django_silly_stripe.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1390 2023-08-03 16:13:07.000000 django-silly-stripe-1.0.3/django_silly_stripe.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-08-03 16:13:07.000000 django-silly-stripe-1.0.3/django_silly_stripe.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       20 2023-08-03 16:13:07.000000 django-silly-stripe-1.0.3/django_silly_stripe.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-08-03 16:13:07.174409 django-silly-stripe-1.0.3/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1744 2023-08-03 16:12:47.000000 django-silly-stripe-1.0.3/setup.py
```

### Comparing `django-silly-stripe-1.0.2/LICENSE.md` & `django-silly-stripe-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.2/django_silly_stripe/admin.py` & `django-silly-stripe-1.0.3/django_silly_stripe/admin.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.2/django_silly_stripe/conf.py` & `django-silly-stripe-1.0.3/django_silly_stripe/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     f"{color['end']}"
 
     )
 
 
 SILLY_STRIPE = {
     # Basic settings
+    'AUTO_SET': 'CLASSIC',  # 'SPA' or 'CLASSIC'
     'DSS_SECRET_KEY': 'sk_xxxxxx',
     'DSS_PUBLIC_KEY': 'pk_xxxxxx',
     'DSS_RESTRICTED_KEY': 'rk_xxxxxx',  # optionnal
     'DSS_WEBHOOK_SECRET': 'wk_xxxxxx',
     'DSS_PREFIX': 'dss/',
     # Django Silly Stripe Endpoints
     'USE_CHECKOUT': True,
@@ -39,11 +40,13 @@
     'SUCCESS_URL': 'https://example.com/checkout_success',
     'CANCEL_URL': 'https://example.com/checkout_cancel',
     # Subscriptions settings
     'SUBSCRIPTION_CANCEL': 'PERIOD',  # 'PERIOD' or 'NOW' (beware with 'NOW': no refund)
     'SUBSCRIBE_ONLY_ONCE': True,
     # Portal settings
     'PORTAL_BACK_URL': 'https://example.com/back_from_portal',
+    # Misc
+    'PRINT_DEV_LOGS': False,
 }
 
 for key in settings.SILLY_STRIPE:
     SILLY_STRIPE[key] = settings.SILLY_STRIPE[key]
```

### Comparing `django-silly-stripe-1.0.2/django_silly_stripe/migrations/0001_initial.py` & `django-silly-stripe-1.0.3/django_silly_stripe/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.2/django_silly_stripe/migrations/0002_alter_customer_user.py` & `django-silly-stripe-1.0.3/django_silly_stripe/migrations/0002_alter_customer_user.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.2/django_silly_stripe/migrations/0003_remove_customer_stripe_id_alter_customer_id.py` & `django-silly-stripe-1.0.3/django_silly_stripe/migrations/0003_remove_customer_stripe_id_alter_customer_id.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.2/django_silly_stripe/migrations/0006_product_price.py` & `django-silly-stripe-1.0.3/django_silly_stripe/migrations/0006_product_price.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.2/django_silly_stripe/migrations/0008_subscription.py` & `django-silly-stripe-1.0.3/django_silly_stripe/migrations/0008_subscription.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.2/django_silly_stripe/migrations/0009_subscription_end_time_subscription_start_time_and_more.py` & `django-silly-stripe-1.0.3/django_silly_stripe/migrations/0009_subscription_end_time_subscription_start_time_and_more.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.2/django_silly_stripe/migrations/0010_alter_subscription_end_time_and_more.py` & `django-silly-stripe-1.0.3/django_silly_stripe/migrations/0010_alter_subscription_end_time_and_more.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.2/django_silly_stripe/models.py` & `django-silly-stripe-1.0.3/django_silly_stripe/models.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.2/django_silly_stripe/templates/admin/base.html` & `django-silly-stripe-1.0.3/django_silly_stripe/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.2/django_silly_stripe/urls.py` & `django-silly-stripe-1.0.3/django_silly_stripe/urls.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.2/django_silly_stripe.egg-info/SOURCES.txt` & `django-silly-stripe-1.0.3/django_silly_stripe.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 README.md
 setup.py
 django_silly_stripe/__init__.py
 django_silly_stripe/admin.py
 django_silly_stripe/conf.py
 django_silly_stripe/helpers.py
 django_silly_stripe/models.py
+django_silly_stripe/serializers.py
 django_silly_stripe/urls.py
 django_silly_stripe/views.py
+django_silly_stripe/views_api.py
+django_silly_stripe/views_classic.py
 django_silly_stripe.egg-info/PKG-INFO
 django_silly_stripe.egg-info/SOURCES.txt
 django_silly_stripe.egg-info/dependency_links.txt
-django_silly_stripe.egg-info/requires.txt
 django_silly_stripe.egg-info/top_level.txt
 django_silly_stripe/migrations/0001_initial.py
 django_silly_stripe/migrations/0002_alter_customer_user.py
 django_silly_stripe/migrations/0003_remove_customer_stripe_id_alter_customer_id.py
 django_silly_stripe/migrations/0004_customer_email.py
 django_silly_stripe/migrations/0005_customer_name.py
 django_silly_stripe/migrations/0006_product_price.py
```

### Comparing `django-silly-stripe-1.0.2/setup.py` & `django-silly-stripe-1.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     name="django-silly-stripe",
     version=f"{__version__}",
     description=(
         "Wrapper package for python stripe with Django and/or DRF"
         ),
     long_description=README,
     long_description_content_type="text/markdown",
-    url="https://github.com/byoso/django_silly_stripe",
+    url="https://github.com/byoso/django-silly-stripe",
     author="Vincent Fabre",
     author_email="peigne.plume@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Development Status :: 4 - Beta",
@@ -49,17 +49,15 @@
         "django_silly_stripe.migrations",
         "django_silly_stripe.templates",
         "django_silly_stripe.templates.admin",
         ],
     # include_package_data=True,
     package_data={'': ['*.txt', '*.html', '*.po', '*.mo', '*.pot']},
     python_requires='>=3.7',
-    install_requires=[
-        "stripe>=5.4.0",
-    ],
+    # install_requires=[],
     keywords='django stripe',
     # entry_points={
     #     "console_scripts": [
     #         "django_silly_auth=main.cmd:cmd",
     #     ]
     # },
     setup_requires=['wheel'],
```

