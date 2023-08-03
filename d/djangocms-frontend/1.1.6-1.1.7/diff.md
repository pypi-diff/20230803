# Comparing `tmp/djangocms-frontend-1.1.6.tar.gz` & `tmp/djangocms-frontend-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-frontend-1.1.6.tar", last modified: Thu Jul 27 11:52:13 2023, max compression
+gzip compressed data, was "djangocms-frontend-1.1.7.tar", last modified: Thu Aug  3 20:08:58 2023, max compression
```

## Comparing `djangocms-frontend-1.1.6.tar` & `djangocms-frontend-1.1.7.tar`

### file list

```diff
@@ -1,700 +1,700 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.444592 djangocms-frontend-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-07-27 11:52:13.444592 djangocms-frontend-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/cms_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/background.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/responsive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/responsive.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/common/title.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.348593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.348593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion.html
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.352593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.352593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.352593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/badge.html
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/templates/djangocms_frontend/badge.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.356593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.356593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card.html
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.380592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.356593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.356593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/carousel.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.356593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.356593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.360592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.360592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/collapse.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-container.html
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.360592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.360592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.384592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/figure.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/code.html
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/figure.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/grid_row.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.388593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/ckeditor.icons.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.404592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   277297 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    59388 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   123564 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   516494 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   123376 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   123452 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    54568 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   150535 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    56976 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    32020 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   643290 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   127824 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   103304 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   105448 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot
--rw-r--r--   0 runner    (1001) docker     (123)   304476 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg
--rw-r--r--   0 runner    (1001) docker     (123)   105284 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105360 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot
--rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf
--rw-r--r--   0 runner    (1001) docker     (123)    54789 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   729984 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)  2883039 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   729800 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   386256 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   282928 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    99774 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   184969 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)    99564 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    56468 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    44720 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    45816 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot
--rw-r--r--   0 runner    (1001) docker     (123)   132305 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45648 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    45724 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.408592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/
--rw-r--r--   0 runner    (1001) docker     (123)    48146 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)    30533 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json
--rw-r--r--   0 runner    (1001) docker     (123)    35481 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    18498 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json
--rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json
--rw-r--r--   0 runner    (1001) docker     (123)    23027 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    35227 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.408592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.408592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.408592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.412593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)    30045 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    28165 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   137737 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)   115209 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    20997 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    18213 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css
--rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    77647 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    65062 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    32569 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    26765 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.412593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.412593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/icon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.412593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/add_css.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.412593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templatetags/icon_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.412593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.412593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/image.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/jumbotron.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/jumbotron.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.364593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.416592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/list-group.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/media.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/media.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.420592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navlink.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/tabs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.424592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/toc.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.372593 djangocms-frontend-1.1.6/djangocms_frontend/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    35898 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    28086 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    44731 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    34046 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.368593 djangocms-frontend-1.1.6/djangocms_frontend/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    28086 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    44731 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.372593 djangocms-frontend-1.1.6/djangocms_frontend/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    29617 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.372593 djangocms-frontend-1.1.6/djangocms_frontend/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    37743 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.372593 djangocms-frontend-1.1.6/djangocms_frontend/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    24671 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    43925 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17985 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/bootstrap4_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.428592 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.432592 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/frequency_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/stale_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/sync_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/icon_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/management/styled_link_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.432592 djangocms-frontend-1.1.6/djangocms_frontend/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.372593 djangocms-frontend-1.1.6/djangocms_frontend/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.372593 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.432592 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/
--rw-r--r--   0 runner    (1001) docker     (123)    78932 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/base.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/button_group.css
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/div_select.css
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/select2.css
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/select2.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/auto_input.js
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js
--rw-r--r--   0 runner    (1001) docker     (123)    95562 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/django_select2.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/templates/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/bootstrap5/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/bootstrap5/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/bootstrap5/menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/base-collapse.html
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/html_container.html
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/djangocms_frontend/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/djangocms_frontend/templatetags/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.376592 djangocms-frontend-1.1.6/djangocms_frontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-07-27 11:52:13.000000 djangocms-frontend-1.1.6/djangocms_frontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33417 2023-07-27 11:52:13.000000 djangocms-frontend-1.1.6/djangocms_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:52:13.000000 djangocms-frontend-1.1.6/djangocms_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:52:13.000000 djangocms-frontend-1.1.6/djangocms_frontend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-27 11:52:13.000000 djangocms-frontend-1.1.6/djangocms_frontend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 11:52:13.000000 djangocms-frontend-1.1.6/djangocms_frontend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-27 11:52:13.444592 djangocms-frontend-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/tests/accordion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/accordion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/accordion/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/accordion/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.436592 djangocms-frontend-1.1.6/tests/alert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/alert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/alert/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/alert/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/badge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/badge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/badge/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/badge/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/card/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/card/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/carousel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/carousel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/carousel/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/carousel/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/collapse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/collapse/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/collapse/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/content/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/content/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/grid/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/grid/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/icon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/icon/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/icon/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/image/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/image/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/jumbotron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/jumbotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/jumbotron/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/jumbotron/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/link/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/link/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/link/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/link/test_urlconf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/listgroup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/listgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/listgroup/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/listgroup/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/media/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/media/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/media/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.440592 djangocms-frontend-1.1.6/tests/navigation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/navigation/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/navigation/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.444592 djangocms-frontend-1.1.6/tests/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/tabs/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/tabs/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:13.444592 djangocms-frontend-1.1.6/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/utilities/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-27 11:52:02.000000 djangocms-frontend-1.1.6/tests/utilities/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.280435 djangocms-frontend-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-08-03 20:08:58.280435 djangocms-frontend-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.188429 djangocms-frontend-1.1.7/djangocms_frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/cms_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.192429 djangocms-frontend-1.1.7/djangocms_frontend/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/common/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/common/background.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.192429 djangocms-frontend-1.1.7/djangocms_frontend/common/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/common/bootstrap5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/common/bootstrap5/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/common/bootstrap5/responsive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/common/bootstrap5/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/common/responsive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/common/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/common/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/common/title.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.192429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.192429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.192429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.192429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.168428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.168428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.192429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.192429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.196430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.196430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.168428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.168428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.196430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.196430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.196430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.196430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.196430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.196430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.168428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.196430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.196430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/templates/djangocms_frontend/badge.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.196430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.196430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.200430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.168428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.168428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.200430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card.html
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.200430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.200430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.200430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.200430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.168428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.168428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.200430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/carousel.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.168428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.168428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.200430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.200430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.200430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.200430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.172428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.172428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.204430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/collapse.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.204430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.204430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.204430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.204430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.172428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.172428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.204430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/figure.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.204430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/figure.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.204430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.208430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.208430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.172428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.172428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.208430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.208430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/grid_row.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.208430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.208430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.208430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.172428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.172428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.172428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.208430 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/ckeditor.icons.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.172428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.172428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.228432 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   277297 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    59388 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   123564 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   516494 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   123376 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   123452 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    54568 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   150535 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    56976 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32020 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   643290 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   127824 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   103304 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   105448 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   304476 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   105284 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105360 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    54789 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   729984 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)  2883039 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   729800 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   386256 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   282928 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    99774 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   184969 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    99564 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    56468 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    44720 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    45816 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   132305 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45648 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    45724 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.236432 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/
+-rw-r--r--   0 runner    (1001) docker     (123)    48146 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30533 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35481 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18498 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23027 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35227 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.236432 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.236432 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.236432 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.240432 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)    30045 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28165 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   137737 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   115209 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20997 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18213 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    77647 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    65062 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32569 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    26765 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.172428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.172428 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.240432 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.240432 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/icon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.240432 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/add_css.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.244433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/templatetags/icon_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.244433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.244433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.244433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.244433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/image.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.244433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.244433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.244433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.244433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.244433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/jumbotron.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.244433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/jumbotron.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.248433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.248433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.248433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.248433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.248433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.248433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.176429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.248433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.248433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.248433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.248433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.180429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.180429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.248433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/list-group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.252433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.252433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.252433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.180429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.180429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.252433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/media.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.252433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/media.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.252433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.252433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.252433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.180429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.180429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.252433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navlink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.180429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.180429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.256433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.256433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.256433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.256433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.256433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.180429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.180429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.256433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/tabs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.180429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.180429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.256433 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.260434 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.260434 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.260434 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.180429 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.260434 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.260434 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.260434 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/toc.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.260434 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.260434 djangocms-frontend-1.1.7/djangocms_frontend/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.184429 djangocms-frontend-1.1.7/djangocms_frontend/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.184429 djangocms-frontend-1.1.7/djangocms_frontend/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.260434 djangocms-frontend-1.1.7/djangocms_frontend/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    35898 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.184429 djangocms-frontend-1.1.7/djangocms_frontend/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.260434 djangocms-frontend-1.1.7/djangocms_frontend/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    28086 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    44731 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.184429 djangocms-frontend-1.1.7/djangocms_frontend/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.260434 djangocms-frontend-1.1.7/djangocms_frontend/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    34046 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.184429 djangocms-frontend-1.1.7/djangocms_frontend/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.264434 djangocms-frontend-1.1.7/djangocms_frontend/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    28066 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    45024 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.184429 djangocms-frontend-1.1.7/djangocms_frontend/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.264434 djangocms-frontend-1.1.7/djangocms_frontend/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    29617 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.184429 djangocms-frontend-1.1.7/djangocms_frontend/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.264434 djangocms-frontend-1.1.7/djangocms_frontend/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    37743 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.184429 djangocms-frontend-1.1.7/djangocms_frontend/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.264434 djangocms-frontend-1.1.7/djangocms_frontend/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    24671 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    43925 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.264434 djangocms-frontend-1.1.7/djangocms_frontend/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17985 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/management/bootstrap4_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.264434 djangocms-frontend-1.1.7/djangocms_frontend/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/management/commands/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.264434 djangocms-frontend-1.1.7/djangocms_frontend/management/commands/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/management/commands/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/management/commands/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/management/commands/subcommands/frequency_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/management/commands/subcommands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/management/commands/subcommands/stale_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/management/commands/subcommands/sync_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/management/icon_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/management/styled_link_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.264434 djangocms-frontend-1.1.7/djangocms_frontend/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.184429 djangocms-frontend-1.1.7/djangocms_frontend/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.184429 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.268434 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    78932 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/css/base.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/css/button_group.css
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/css/div_select.css
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/css/select2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/css/select2.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.268434 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/js/auto_input.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95562 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/js/django_select2.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.268434 djangocms-frontend-1.1.7/djangocms_frontend/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.268434 djangocms-frontend-1.1.7/djangocms_frontend/templates/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templates/bootstrap5/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templates/bootstrap5/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templates/bootstrap5/menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.268434 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.268434 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/base-collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.268434 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.272434 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/html_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.272434 djangocms-frontend-1.1.7/djangocms_frontend/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/djangocms_frontend/templatetags/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.188429 djangocms-frontend-1.1.7/djangocms_frontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-08-03 20:08:58.000000 djangocms-frontend-1.1.7/djangocms_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33417 2023-08-03 20:08:58.000000 djangocms-frontend-1.1.7/djangocms_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:08:58.000000 djangocms-frontend-1.1.7/djangocms_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:08:57.000000 djangocms-frontend-1.1.7/djangocms_frontend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-03 20:08:58.000000 djangocms-frontend-1.1.7/djangocms_frontend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 20:08:58.000000 djangocms-frontend-1.1.7/djangocms_frontend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-03 20:08:58.284435 djangocms-frontend-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.272434 djangocms-frontend-1.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.272434 djangocms-frontend-1.1.7/tests/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/accordion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/accordion/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/accordion/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.272434 djangocms-frontend-1.1.7/tests/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/alert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/alert/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/alert/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.272434 djangocms-frontend-1.1.7/tests/badge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/badge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/badge/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/badge/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.272434 djangocms-frontend-1.1.7/tests/card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/card/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/card/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.276435 djangocms-frontend-1.1.7/tests/carousel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/carousel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/carousel/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/carousel/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.276435 djangocms-frontend-1.1.7/tests/collapse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/collapse/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/collapse/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.276435 djangocms-frontend-1.1.7/tests/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/content/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/content/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.276435 djangocms-frontend-1.1.7/tests/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/grid/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/grid/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.276435 djangocms-frontend-1.1.7/tests/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/icon/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/icon/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.276435 djangocms-frontend-1.1.7/tests/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/image/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/image/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.276435 djangocms-frontend-1.1.7/tests/jumbotron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/jumbotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/jumbotron/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/jumbotron/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.280435 djangocms-frontend-1.1.7/tests/link/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/link/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/link/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/link/test_urlconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.280435 djangocms-frontend-1.1.7/tests/listgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/listgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/listgroup/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/listgroup/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.280435 djangocms-frontend-1.1.7/tests/media/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/media/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/media/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.280435 djangocms-frontend-1.1.7/tests/navigation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/navigation/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/navigation/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.280435 djangocms-frontend-1.1.7/tests/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/tabs/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/tabs/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:58.280435 djangocms-frontend-1.1.7/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/utilities/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-03 20:08:45.000000 djangocms-frontend-1.1.7/tests/utilities/test_plugins.py
```

### Comparing `djangocms-frontend-1.1.6/LICENSE` & `djangocms-frontend-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/PKG-INFO` & `djangocms-frontend-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-frontend
-Version: 1.1.6
+Version: 1.1.7
 Summary: Adds abstract User Interface items as plugins to django CMS.
 Home-page: https://github.com/django-cms/djangocms-frontend
 Author: fsbraun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-frontend-1.1.6/README.rst` & `djangocms-frontend-1.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/__init__.py` & `djangocms-frontend-1.1.7/djangocms_frontend/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
  9. git push
 10. Assure that all tests pass on https://github.com/django-cms/djangocms-frontend/actions
 11. Create a new release on https://github.com/django-cms/djangocms-frontend/releases/new
 12. Publish the release when ready
 13. Github actions will publish the new package to pypi
 """
 
-__version__ = "1.1.6"
+__version__ = "1.1.7"
```

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/common/attributes.py` & `djangocms-frontend-1.1.7/djangocms_frontend/common/attributes.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/background.py` & `djangocms-frontend-1.1.7/djangocms_frontend/common/bootstrap5/background.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/responsive.py` & `djangocms-frontend-1.1.7/djangocms_frontend/common/bootstrap5/responsive.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/common/bootstrap5/sizing.py` & `djangocms-frontend-1.1.7/djangocms_frontend/common/bootstrap5/sizing.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/common/spacing.py` & `djangocms-frontend-1.1.7/djangocms_frontend/common/spacing.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/common/title.py` & `djangocms-frontend-1.1.7/djangocms_frontend/common/title.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/models.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/badge/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/badge/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/constants.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/frameworks/foundation6.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/frameworks/foundation6.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/models.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/constants.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/models.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/models.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/models.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/constants.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/frameworks/foundation6.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/frameworks/foundation6.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/models.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/conf.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/conf.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/fields.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/icon/templatetags/icon_tags.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/icon/templatetags/icon_tags.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/models.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% load thumbnail frontend %}{% spaceless %}
     {% if picture_link %}
         <a href="{{ picture_link }}"
-            {% if instance.link_target %} target="{{ instance.link_target }}"{% endif %}
+            {% if instance.target %} target="{{ instance.target }}"{% endif %}
             {% get_attributes instance.link_attributes %}>
     {% endif %}
     <img src="{{ instance.img_src }}" {% if not instance.attributes.alt and instance.rel_image.default_alt_text %}alt="{{ instance.rel_image.default_alt_text }}"{% endif %} {% if instance.width %} width="{{ instance.width|safe }}"{% endif %} {% if instance.height %} height="{{ instance.height|safe }}"{% endif %}
         {% if img_srcset_data %}
             srcset="{% for size, thumb in img_srcset_data %}{{ thumb.url }} {{ size|safe }}w,{% endfor %}{{ instance.img_src }} {{ picture_size.size.0|safe }}w"
             sizes="{% for size, thumb in img_srcset_data %}(max-width: {{ size|safe }}px) {{ size|safe }}px, {% endfor %} {{ picture_size.size.0|safe }}px"
         {% endif %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% load thumbnail frontend %}{% spaceless %} {% if picture_link %}
-% if instance.link_target %} target="{{ instance.link_target }}"{% endif %} {%
+% if instance.target %} target="{{ instance.target }}"{% endif %} {%
 get_attributes instance.link_attributes %}> {% endif %}
 % if not instance.attributes.alt and instance.rel_image.default_alt_text
 %}alt="{{ instance.rel_image.default_alt_text }}"{% endif %} {% if
 instance.width %} width="{{ instance.width|safe }}"{% endif %} {% if
 instance.height %} height="{{ instance.height|safe }}"{% endif %} {% if
 img_srcset_data %} srcset="{% for size, thumb in img_srcset_data %}{{ thumb.url
 }} {{ size|safe }}w,{% endfor %}{{ instance.img_src }} {
```

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/constants.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/helpers.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/models.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/link/views.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/link/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/listgroup/models.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/listgroup/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/media/models.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/media/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/models.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/constants.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/models.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/cms_plugins.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/forms.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/models.py` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html` & `djangocms-frontend-1.1.7/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/fields.py` & `djangocms-frontend-1.1.7/djangocms_frontend/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.7/djangocms_frontend/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/helpers.py` & `djangocms-frontend-1.1.7/djangocms_frontend/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/locale/ar/LC_MESSAGES/django.mo` & `djangocms-frontend-1.1.7/djangocms_frontend/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/locale/ar/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.7/djangocms_frontend/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/locale/de/LC_MESSAGES/django.mo` & `djangocms-frontend-1.1.7/djangocms_frontend/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/locale/de/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.7/djangocms_frontend/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/locale/en/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.7/djangocms_frontend/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/locale/es/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.7/djangocms_frontend/locale/sq/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,198 +1,195 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 # 
 # Translators:
 # Mark Walker <theshow@gmail.com>, 2023
-# Fabian Braun <fsbraun@gmx.de>, 2023
+# Besnik Bleta <besnik@programeshqip.org>, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-03-11 17:20+0100\n"
 "PO-Revision-Date: 2023-01-20 15:48+0000\n"
-"Last-Translator: Fabian Braun <fsbraun@gmx.de>, 2023\n"
-"Language-Team: German (https://app.transifex.com/divio/teams/58664/de/)\n"
+"Last-Translator: Besnik Bleta <besnik@programeshqip.org>, 2023\n"
+"Language-Team: Albanian (https://app.transifex.com/divio/teams/58664/sq/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: de\n"
+"Language: sq\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: common/attributes.py:9
 msgid ""
 "Advanced settings lets you add html attributes to render this element. Use "
 "them wisely and rarely."
 msgstr ""
-"Die erweiterten Einstellungen erlaubt Ihnen, HTML-Attribute des Elements "
-"direkt anzugeben."
+"Rregullimet e mëtejshme ju lejojnë të shtoni atribute HTML për shfaqjen e "
+"këtij elementi. Përdoreni me mend dhe rrallë."
 
 #: common/attributes.py:26 contrib/accordion/cms_plugins.py:91
 msgid "Advanced settings"
-msgstr "Erweiterte Einstellungen"
+msgstr "Rregullime të mëtejshme"
 
 #: common/bootstrap5/background.py:20
 msgid "Background"
-msgstr "Hintergrund"
+msgstr "Sfond"
 
 #: common/bootstrap5/background.py:48
 msgid "Background context"
-msgstr "Hintergrund-Kontext"
+msgstr "Kontekst sfondi"
 
 #: common/bootstrap5/background.py:52 contrib/card/forms.py:32
 #: contrib/card/models.py:7
 msgid "Transparent"
-msgstr "Transparent"
+msgstr "I tejdukshëm"
 
 #: common/bootstrap5/background.py:57
 msgid "Background opacity"
-msgstr "Deckkraft des Hintergrundes"
+msgstr "Patejdukshmëri sfondi"
 
 #: common/bootstrap5/background.py:62
 msgid "Opacity of card background color (only if no outline selected)"
 msgstr ""
-"Gibt die Deckkraft der Hintergrundfarbe an (nur wirksam, wenn Kontur nicht "
-"angewählt ist)."
+"Patejdukshmëri e ngjyrës së sfondit të kartës (nëse s’është përzgjedhur "
+"përvijim)"
 
 #: common/bootstrap5/background.py:66
 #: contrib/alert/frameworks/bootstrap5.py:42
 msgid "Shadow"
-msgstr "Schatten"
+msgstr "Hije"
 
 #: common/bootstrap5/background.py:71
 msgid "Use shadows to optically lift cards from the background."
-msgstr "Schatten heben Karten optisch vom Hintergrund ab."
+msgstr "Përdorni hije për t’i dalluar nga ana pamore kartat nga sfondi."
 
 #: common/bootstrap5/responsive.py:35
 msgid "Visibility"
-msgstr "Sichtbarkeit"
+msgstr "Dukshmëri"
 
 #: common/bootstrap5/responsive.py:58
 msgid "Show element on device"
-msgstr "Zeige Element auf diesen Bildschirmgrößen"
+msgstr "Shfaq elementin në pajisje"
 
 #: common/bootstrap5/responsive.py:60
 msgid "Select only devices on which this element should be shown."
-msgstr ""
-"Nur die Bildschirmgrößen auswählen, auf denen dieses Element angezeigt "
-"werden soll."
+msgstr "Përzgjidhni vetëm pajisjet te të cilat ky element duhet shfaqur."
 
 #: common/bootstrap5/sizing.py:8 common/spacing.py:11
 #: contrib/utilities/forms.py:51 frameworks/bootstrap5.py:90
 #: frameworks/bootstrap5.py:103
 msgid "Auto"
 msgstr "Auto"
 
 #: common/bootstrap5/sizing.py:44
 msgid "Horizontal size"
-msgstr "Horizontale Größe"
+msgstr "Madhësi horizontale"
 
 #: common/bootstrap5/sizing.py:50
 msgid ""
 "Sets the horizontal size relative to the surrounding container or the "
 "viewport."
 msgstr ""
-"Legt die horizontale Größe im Verhältnis zum umgebenden Container oder dem "
-"Fenster fest."
+"Cakton madhësinë horizontale, relative ndaj kontejnerit ose pjesës së "
+"ekranit që e rrethon."
 
 #: common/bootstrap5/sizing.py:54
 msgid "Vertical size"
-msgstr "Vertikale Größe"
+msgstr "Madhësi vertikale"
 
 #: common/bootstrap5/sizing.py:60
 msgid ""
 "Sets the vertical size relative to the surrounding container or the "
 "viewport."
 msgstr ""
-"Legt die vertikale Größe im Verhältnis zum umgebenden Container oder dem "
-"Fenster fest."
+"Cakton madhësinë vertikale, relative ndaj kontejnerit ose pjesës së ekranit "
+"që e rrethon."
 
 #: common/spacing.py:84
 msgid "Please choose a side to which the spacing should be applied."
-msgstr "Bitte Seite auswählen, auf die der Abstand angewendet werden soll."
+msgstr "Ju lutemi, zgjidhni një anë mbi të cilën duhet aplikuar hapësira."
 
 #: common/spacing.py:113
 msgid "Margin"
-msgstr "Abstand außen"
+msgstr "Mënjanë"
 
 #: common/spacing.py:139 common/spacing.py:147
 msgid "Padding"
-msgstr "Abstand zum Rand innen"
+msgstr "Mbushje"
 
 #: common/spacing.py:175 contrib/utilities/cms_plugins.py:22
 #: contrib/utilities/models.py:14
 msgid "Spacing"
-msgstr "Abstand"
+msgstr "Hapësirë"
 
 #: common/spacing.py:189
 msgid "Horizontal margin"
-msgstr "Horizontaler Abstand außen"
+msgstr "Mënjanë horizontale"
 
 #: common/spacing.py:195
 msgid "Vertical margin"
-msgstr "Vertikaler Abstand außen"
+msgstr "Mënjanë vertikale"
 
 #: common/spacing.py:201
 msgid "Apply margin on device"
-msgstr "Anzuwenden auf diesen Geräten"
+msgstr "Apliko mënjanë te pajisja"
 
 #: common/spacing.py:204
 msgid ""
 "Select only devices on which the margin should be applied. On other devices "
 "larger than the first selected device the margin will be set to zero."
 msgstr ""
-"Nur Bildschirmgrößen auswählen, auf denen der Abstand angewendet werden "
-"soll. Auf größeren Bildschirmen als dem ersten ausgewählten, wird der "
-"Außenabstand auf Null gesetzt."
+"Përgjidhni një anë mbi të cilën duhet aplikuar hapësira. Select only devices"
+" on which the margin should be applied. On other devices larger than the "
+"first selected device the margin will be set to zero."
 
 #: common/spacing.py:221
 msgid "Horizontal padding"
-msgstr "Horizontaler Abstand zum Rand"
+msgstr "Mbushje horizontale"
 
 #: common/spacing.py:227
 msgid "Vertical padding"
-msgstr "Vertikaler Abstand zum Rand"
+msgstr "Mbushje vertikale"
 
 #: common/spacing.py:233
 msgid "Apply padding on device"
-msgstr "Anzuwenden auf diesen Geräten"
+msgstr "Apliko mbushje te pajisja"
 
 #: common/spacing.py:236
 msgid ""
 "Select only devices on which the padding should be applied. On other devices"
 " larger than the first selected device the padding will be set to zero."
 msgstr ""
-"Nur Bildschirmgrößen auswählen, auf denen der Abstand angewendet werden "
-"soll. Auf größeren Bildschirmen als dem ersten ausgewählten, wird der "
-"Abstand zum Rand auf Null gesetzt."
+"Përzgjidhni vetëm pajisjet mbi të cilat duhet aplikuar mbushja. Në pajisje "
+"të tjera, më të mëdha se pajisja e parë e përzgjedhur, mbushja do të "
+"caktohet si zero."
 
 #: common/title.py:40
 msgid "Please add a title if you want to publish it."
-msgstr "Bitte Titel-Attribut hinzufügen, wenn es öffentlich sein soll."
+msgstr "Ju lutemi, shtoni një titull, nëse doni të botohet."
 
 #: common/title.py:64
 msgid "Title"
-msgstr "Titel-Attribut"
+msgstr "Titull"
 
 #: common/title.py:67
 msgid ""
 "Optional title of the plugin for easier identification. Its "
 "<code>title</code> attribute will only be set if the checkbox is selected."
 msgstr ""
-"Optionaler Titel des Plugin für eine einfachere Identifikation. Sei "
-"<code>title</code>-Attribut wird nur gesetzt, wenn das Auswahlkästchen "
-"angewählt ist"
+"Titull i shtojcës, në daçi, për identifikim më të kollajtë. Atributi "
+"<code>title</code> për të do të ujdiset vetëm nëse përzgjidhet kutiza."
 
 #: contrib/accordion/cms_plugins.py:21 contrib/accordion/models.py:14
 msgid "Accordion"
-msgstr "Akkordion"
+msgstr "Fizarmonikë"
 
 #: contrib/accordion/cms_plugins.py:22 contrib/accordion/cms_plugins.py:72
 #: contrib/alert/cms_plugins.py:25 contrib/badge/cms_plugins.py:21
 #: contrib/card/cms_plugins.py:25 contrib/card/cms_plugins.py:86
 #: contrib/card/cms_plugins.py:146 contrib/carousel/cms_plugins.py:26
 #: contrib/carousel/cms_plugins.py:71 contrib/collapse/cms_plugins.py:21
 #: contrib/collapse/cms_plugins.py:50 contrib/collapse/cms_plugins.py:76
@@ -206,1472 +203,1470 @@
 #: contrib/navigation/cms_plugins.py:30 contrib/navigation/cms_plugins.py:75
 #: contrib/navigation/cms_plugins.py:106 contrib/navigation/cms_plugins.py:134
 #: contrib/navigation/cms_plugins.py:165 contrib/tabs/cms_plugins.py:25
 #: contrib/tabs/cms_plugins.py:59 contrib/utilities/cms_plugins.py:23
 #: contrib/utilities/cms_plugins.py:50 contrib/utilities/cms_plugins.py:62
 #: contrib/utilities/cms_plugins.py:123
 msgid "Frontend"
-msgstr "Frontend"
+msgstr "Pjesa e dukshme"
 
 #: contrib/accordion/cms_plugins.py:57
 msgid "Item {}"
-msgstr "Element {}"
+msgstr "Objekt {}"
 
 #: contrib/accordion/cms_plugins.py:71 contrib/accordion/models.py:33
 msgid "Accordion item"
-msgstr "Akkordion-Element"
+msgstr "Objekt fizarmonike"
 
 #: contrib/accordion/forms.py:34
 msgid "Create accordion items"
-msgstr "Akkordion-Element erstellen"
+msgstr "Krijoni objekte fizarmonikë"
 
 #: contrib/accordion/forms.py:35
 msgid "Number of accordion items to create when saving."
-msgstr ""
-"Anzahl der Akkordion-Elemente, die beim Speichern erstellt werden soll."
+msgstr "Numër objektesh fizarmonikë për t’u krijuar, kur ruhet."
 
 #: contrib/accordion/forms.py:42
 msgid "Header type"
-msgstr "Überschritften-Typ"
+msgstr "Lloj kryesh"
 
 #: contrib/accordion/forms.py:48
 msgid "Integrate into parent"
-msgstr "In Eltern-Element einfügen"
+msgstr "Integroje te mëma"
 
 #: contrib/accordion/forms.py:52
 msgid ""
 "Removes the default background-color, some borders, and some rounded corners"
 " to render accordions edge-to-edge with their parent container "
 msgstr ""
-"Entfernt die Hintergrundfarbe, Rahmen und ausgewählte abgerundete Ecken, um "
-"Akkordions direkt in ihren Eltern-Elementen anzuzeigen."
+"Bën heqjen e ngjyrës parazgjedhje për sfondin, disa anë dhe disa cepa të "
+"rrumbullakosur, për t’i shfaqur fizarmonikat nga skaji në skaj, me "
+"kontejnerin e tyre mëmë "
 
 #: contrib/accordion/forms.py:78 contrib/card/constants.py:16
 msgid "Header"
-msgstr "Überschrift"
+msgstr "Krye"
 
 #: contrib/accordion/forms.py:82
 msgid "Item open"
-msgstr "Offenes element"
+msgstr ""
 
 #: contrib/accordion/forms.py:85
 msgid "Initially shows this accordion item on page load."
-msgstr "Zeigt nach dem Laden dieses Akkordion-Element."
+msgstr "E shfaq fillimisht këtë objekt fizarmonikë gjatë ngarkimit të faqes."
 
 #: contrib/accordion/models.py:20
 msgid "({} entries)"
-msgstr "({} Einträge)"
+msgstr "({} zëra)"
 
 #: contrib/accordion/models.py:29
 msgid "AccordionItem"
-msgstr "Akkordion-Element"
+msgstr ""
 
 #: contrib/alert/cms_plugins.py:24 contrib/alert/models.py:14
 msgid "Alert"
-msgstr "Warnung"
+msgstr "Sinjalizim"
 
 #: contrib/alert/forms.py:41 contrib/badge/forms.py:37
 #: contrib/link/forms.py:340 contrib/listgroup/forms.py:71
 msgid "Context"
-msgstr "Kontext"
+msgstr "Kontekst"
 
 #: contrib/alert/forms.py:47
 msgid "Dismissible"
-msgstr "Schließbar"
+msgstr "Që mund të hidhet tej"
 
 #: contrib/alert/forms.py:50
 msgid "Allows the alert to be closed."
-msgstr "Erlaubt, die Warnung zu schliessen."
+msgstr "Lejon mbylljen e sinjalizimit."
 
 #: contrib/alert/frameworks/bootstrap5.py:47
 msgid "Use shadows to optically lift alerts from the background."
-msgstr "Schatten heben Warnungen optisch vom Hintergrund ab."
+msgstr "Përdorni hije për t’i dalluar nga ana pamore sinjalizimet nga sfondi."
 
 #: contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html:4
 msgid "Close"
-msgstr "Schliessen"
+msgstr "Mbylle"
 
 #: contrib/badge/cms_plugins.py:20 contrib/badge/models.py:14
 msgid "Badge"
-msgstr "Badge"
+msgstr "Stemë"
 
 #: contrib/badge/forms.py:33
 msgid "Badge text"
-msgstr "Badge-Text"
+msgstr "Tekst i stemës"
 
 #: contrib/badge/forms.py:43
 msgid "Pills style"
-msgstr "Pillen-Stil"
+msgstr "Stil sumbullash"
 
 #: contrib/badge/forms.py:46
 msgid "Activates the pills style."
-msgstr "Aktiviert den Pillen-Stil."
+msgstr "Aktivizon stilin e sumbullave."
 
 #: contrib/card/cms_plugins.py:24 contrib/card/models.py:20
 msgid "Card layout"
-msgstr "Karten-Layout"
+msgstr "Skemë karte"
 
 #: contrib/card/cms_plugins.py:47 contrib/grid/cms_plugins.py:93
 #: contrib/grid/cms_plugins.py:173
 msgid "Responsive settings"
-msgstr "Responsive-Hilfsmittel"
+msgstr "Rregullime reaguese"
 
 #: contrib/card/cms_plugins.py:85 contrib/card/models.py:35
 msgid "Card"
-msgstr "Karte"
+msgstr "Kartë"
 
 #: contrib/card/cms_plugins.py:145 contrib/card/models.py:57
 msgid "Card inner"
-msgstr "Karten-Inhalt"
+msgstr ""
 
 #: contrib/card/constants.py:4
 msgid "Card group"
-msgstr "Karten-Gruppe"
+msgstr "Grup karte"
 
 #: contrib/card/constants.py:5
 msgid "Grid cards"
-msgstr "Karten-Gitter"
+msgstr ""
 
 #: contrib/card/constants.py:9 contrib/utilities/forms.py:108
 #: frameworks/bootstrap5.py:59 settings.py:47
 msgid "Left"
-msgstr "Links"
+msgstr "Majtas"
 
 #: contrib/card/constants.py:10 contrib/utilities/forms.py:109 settings.py:48
 msgid "Center"
-msgstr "Mitte"
+msgstr "Në qendër"
 
 #: contrib/card/constants.py:11 contrib/utilities/forms.py:110
 #: frameworks/bootstrap5.py:60 settings.py:49
 msgid "Right"
-msgstr "Rechts"
+msgstr "Djathtas"
 
 #: contrib/card/constants.py:15
 msgid "Body"
-msgstr "Body"
+msgstr "Lëndë"
 
 #: contrib/card/constants.py:17
 msgid "Footer"
-msgstr "Footer"
+msgstr "Fundfaqe"
 
 #: contrib/card/constants.py:18
 msgid "Image overlay"
-msgstr "Bild-Überlagerung"
+msgstr ""
 
 #: contrib/card/forms.py:35 contrib/card/models.py:9
 msgid "White"
-msgstr "Weiss"
+msgstr "E bardhë"
 
 #: contrib/card/forms.py:61
 msgid "Create cards"
-msgstr "Karten erstellen"
+msgstr "Krijoni karta"
 
 #: contrib/card/forms.py:62
 msgid "Number of cards to create when saving."
-msgstr "Anzahl der Karten, die beim Speichern erstellt werden soll."
+msgstr "Numër kartash për t’u krijuar, kur ruhet."
 
 #: contrib/card/forms.py:68
 msgid "Card type"
-msgstr "Card-Typ"
+msgstr "Lloj karte"
 
 #: contrib/card/forms.py:122
 msgid "Card outline context"
-msgstr "Kontext Kartenrand"
+msgstr ""
 
 #: contrib/card/forms.py:126
 msgid "Uses the border to indicate context."
-msgstr "Färbt den Rand gemäß dem Kontext"
+msgstr "Përdor anën për të treguar kontekstin."
 
 #: contrib/card/forms.py:132 contrib/content/forms.py:99
 #: contrib/content/forms.py:137 contrib/grid/cms_plugins.py:99
 #: contrib/image/forms.py:147 contrib/tabs/forms.py:57
 #: contrib/utilities/forms.py:139
 msgid "Alignment"
-msgstr "Ausrichtung"
+msgstr "Drejtim"
 
 #: contrib/card/forms.py:140
 msgid "Text context"
-msgstr "Text-Kontext"
+msgstr "Kontekst teksti"
 
 #: contrib/card/forms.py:148
 msgid "Full height"
-msgstr "Volle Höhe"
+msgstr "Lartësi e plotë"
 
 #: contrib/card/forms.py:152
 msgid ""
 "If checked cards in one row will automatically extend to the full row "
 "height."
-msgstr "Wenn angewählt, erhalten alle Cards in einer Reihe die volle Höhe."
+msgstr ""
+"Në iu vëntë shenjë, kartat e një rreshti do të zgjerohen vetvetiu sa "
+"lartësia e plotë e rreshtit."
 
 #: contrib/card/forms.py:186
 msgid "Inner type"
-msgstr "Inhalts-Typ"
+msgstr "Lloj i Brendshëm"
 
 #: contrib/card/forms.py:189
 msgid "Define the structure of the plugin."
-msgstr "Definiert die Struktur des Plugins."
+msgstr "Përcaktoni strukturën e shtojcës."
 
 #: contrib/card/forms.py:193 contrib/grid/forms.py:173
 msgid "Content alignment"
-msgstr "Inhalts-Ausrichtung"
+msgstr "Drejtim lënde"
 
 #: contrib/card/templates/djangocms_frontend/admin/card_layout.html:14
 #: contrib/grid/templates/djangocms_frontend/admin/grid_row.html:13
 msgid "Colums per row"
-msgstr "Splaten pro Zeile"
+msgstr "Shtylla për rresht"
 
 #: contrib/carousel/cms_plugins.py:25 contrib/carousel/models.py:20
 msgid "Carousel"
-msgstr "Karussell"
+msgstr "Rrotullame"
 
 #: contrib/carousel/cms_plugins.py:70 contrib/carousel/models.py:42
 msgid "Carousel slide"
-msgstr "Karussell-Eintrag"
+msgstr "Rrëshqitës rrotullame"
 
 #: contrib/carousel/cms_plugins.py:88 contrib/link/cms_plugins.py:45
 #: contrib/link/cms_plugins.py:83
 msgid "Link settings"
-msgstr "Link-Einstellungen"
+msgstr "Rregullime lidhjesh"
 
 #: contrib/carousel/constants.py:5
 msgid "On hover"
-msgstr "Mit Maus"
+msgstr ""
 
 #: contrib/carousel/constants.py:6
 msgid "Never"
-msgstr "Nie"
+msgstr ""
 
 #: contrib/carousel/constants.py:12 contrib/image/forms.py:39
 #: contrib/tabs/constants.py:27 settings.py:56 settings.py:64 settings.py:72
 msgid "Default"
-msgstr "Standard"
+msgstr "Parazgjedhje"
 
 #: contrib/carousel/constants.py:36
 msgid "Slide"
-msgstr "Gleiten"
+msgstr ""
 
 #: contrib/carousel/constants.py:37 contrib/tabs/constants.py:21
 msgid "Fade"
-msgstr "Überblenden"
+msgstr "Zbehje"
 
 #: contrib/carousel/forms.py:58 contrib/image/forms.py:103
 #: contrib/jumbotron/forms.py:44 contrib/link/forms.py:320
 #: contrib/navigation/forms.py:42 contrib/tabs/forms.py:45
 msgid "Template"
-msgstr "Vorlage"
+msgstr "Gjedhe"
 
 #: contrib/carousel/forms.py:61 contrib/tabs/forms.py:48
 msgid "This is the template that will be used for the component."
-msgstr "Dies ist das Template das für die Komponente genutzt wird."
+msgstr "Kjo është gjedhja që do të përdoret për përbërësin."
 
 #: contrib/carousel/forms.py:64 contrib/carousel/models.py:24
 msgid "Interval"
-msgstr "Intervall"
+msgstr "Interval"
 
 #: contrib/carousel/forms.py:67
 msgid ""
 "The amount of time to delay between automatically cycling an item. If false,"
 " carousel will not automatically cycle."
 msgstr ""
-"Die Zeitspanne zwischen dem automatischen Wechseln der Einträge. Wenn false,"
-" dann wird nicht automatisch gewechselt."
+"Sasia e kohës në sekonda për vonim zërash te kalimi automatikisht në ta. Në "
+"u vëntë 0, rrotullamja s’do të kalojë automatikisht nëpër ta."
 
 #: contrib/carousel/forms.py:72 contrib/carousel/models.py:25
 msgid "Controls"
-msgstr "Steuerelemente"
+msgstr "Kontrolle"
 
 #: contrib/carousel/forms.py:75
 msgid "Adding in the previous and next controls."
-msgstr "Fügt die Weiter und Zurück Steuerelemente hinzu."
+msgstr "Po shtohen kontrollet “i mëparshmi” dhe “pasuesi”."
 
 #: contrib/carousel/forms.py:78 contrib/carousel/models.py:26
 msgid "Indicators"
-msgstr "Indikatoren"
+msgstr "Tregues"
 
 #: contrib/carousel/forms.py:81
 msgid "Adding in the indicators to the carousel."
-msgstr "Fügt dem Karussell Positions-Indikatoren hinzu."
+msgstr "Po shtohen treguesit te rrotullamja."
 
 #: contrib/carousel/forms.py:84 contrib/carousel/models.py:27
 msgid "Keyboard"
-msgstr "Tastatur"
+msgstr "Tastierë"
 
 #: contrib/carousel/forms.py:87
 msgid "Whether the carousel should react to keyboard events."
-msgstr "Soll das Karussell mit der Tastatur bedienbar sein."
+msgstr "Nëse duhet të reagojë apo jo rrotullamja ndaj aktesh tastiere."
 
 #: contrib/carousel/forms.py:90 contrib/carousel/models.py:28
 msgid "Pause"
-msgstr "Pause"
+msgstr "Ndalesë"
 
 #: contrib/carousel/forms.py:94
 msgid ""
 "If set to \"hover\", pauses the cycling of the carousel on \"mouseenter\" "
 "and resumes the cycling of the carousel on \"mouseleave\". If set to "
 "\"false\", hovering over the carousel won't pause it."
 msgstr ""
-"Pausiert das Karussells, sobald sich die Maus über dem Karussell befindet. "
-"Startet wieder, nachdem die Maus das Karussell verlassen hat."
+"Në u vëntë si “hover”, e ndal rrotullimin e rrotullames pas një akti "
+"“mouseenter” dhe e rifillon rrotullimin e rrotullames pas një akti "
+"“mouseleave”. Në u vëntë si “false”, kalimi i kursorit mbi rrotullamen s’do "
+"ta ndalë atë."
 
 #: contrib/carousel/forms.py:102
 msgid "Auto start"
-msgstr "Autostart"
+msgstr ""
 
 #: contrib/carousel/forms.py:106
 msgid ""
 "Autoplays the carousel after the user manually cycles the first item. If "
 "\"carousel\", autoplays the carousel on load."
-msgstr "Startet das Karussell direkt nach dem Laden."
+msgstr ""
+"Vetëluhet rrotullamja, pasi përdoruesi vë në punë dorazi kuadrin e parë. Në "
+"u vëntë “carousel”, vetëluhet automatikisht rrotullamja, kur ngarkohet "
+"faqja."
 
 #: contrib/carousel/forms.py:111 contrib/carousel/models.py:30
 msgid "Wrap"
-msgstr "Endlos"
+msgstr ""
 
 #: contrib/carousel/forms.py:115
 msgid "Whether the carousel should cycle continuously or have hard stops."
-msgstr "Startet nach einem Durchlauf wieder von vorne."
+msgstr ""
+"Nëse rrotullamja duhet të rrotullohet vazhdimisht, apo të ketë ndalesa."
 
 #: contrib/carousel/forms.py:119
 msgid "Aspect ratio"
-msgstr "Seitenverhältnis"
+msgstr "Përpjesëtim"
 
 #: contrib/carousel/forms.py:124
 msgid ""
 "Determines width and height of the image according to the selected ratio."
 msgstr ""
-"Bestimmt die Höhe und Breite der Bilder anhand des ausgewählten "
-"Seitenverhältnises."
+"Përcakton gjerësinë dhe lartësinë e fizarmonikës së figurave sa përpjesëtimi"
+" i përzgjedhur."
 
 #: contrib/carousel/forms.py:129
 msgid "Transition"
-msgstr "Übergang"
+msgstr ""
 
 #: contrib/carousel/forms.py:133
 msgid "Determines if slides change by sliding or fading."
-msgstr "Legt fest, ob Karussell-Bild herein gleitet oder übergeblendet wird."
+msgstr ""
 
 #: contrib/carousel/forms.py:177
 msgid "Slide image"
-msgstr "Karussell-Bild"
+msgstr ""
 
 #: contrib/carousel/forms.py:181
 msgid "Content"
-msgstr "Inhalt"
+msgstr "Lëndë"
 
 #: contrib/carousel/forms.py:184
 msgid "Content may also be added using child plugins."
-msgstr "Inhalt kann auch über weitere Plugins hinzugefügt werden."
+msgstr "Lëndë mund të shtohet edhe duke përdorur shtojca pjellë."
 
 #: contrib/carousel/models.py:29
 msgid "Ride"
-msgstr "Autostart"
+msgstr ""
 
 #: contrib/carousel/models.py:51 contrib/image/models.py:154
 msgid "<file is missing>"
-msgstr "<Datei fehlt>"
+msgstr "<kartela mungon>"
 
 #: contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html:32
 msgid "Previous"
-msgstr "Zurück"
+msgstr "E mëparshmja"
 
 #: contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html:36
 msgid "Next"
-msgstr "Weiter"
+msgstr "Pasuesja"
 
 #: contrib/collapse/cms_plugins.py:20 contrib/collapse/models.py:21
 msgid "Collapse"
-msgstr "Collapse"
+msgstr "Tkurre"
 
 #: contrib/collapse/cms_plugins.py:49 contrib/collapse/models.py:35
 msgid "Collapse trigger"
-msgstr "Collapse-Auslöser"
+msgstr ""
 
 #: contrib/collapse/cms_plugins.py:75 contrib/collapse/models.py:49
 msgid "Collapse container"
-msgstr "Collapse-Container"
+msgstr "Tkurre kontejnerin"
 
 #: contrib/collapse/forms.py:37
 msgid "Siblings"
-msgstr "Geschwister"
+msgstr ""
 
 #: contrib/collapse/forms.py:40
 msgid "Element to be used to create accordions."
-msgstr "Element, welches genutzt wird, um Akkordions zu erstellen."
+msgstr "Element i përdorur për të krijuar fizarmonika."
 
 #: contrib/collapse/forms.py:63 contrib/collapse/forms.py:88
 msgid "Unique identifier"
-msgstr "Einzigartige Kennung (ID)"
+msgstr "Identifikues unik"
 
 #: contrib/collapse/forms.py:65 contrib/collapse/forms.py:90
 msgid "Identifier to connect trigger with container."
-msgstr "Kennung, welche den Auslöser mit dem Collapse-Kontainer verbindet."
+msgstr "Identifikues për të lidhur shkaktues me kontejner."
 
 #: contrib/collapse/templates/djangocms_frontend/admin/collapse.html:7
 #: contrib/media/templates/djangocms_frontend/admin/media.html:7
 #: contrib/utilities/templates/djangocms_frontend/admin/no_form.html:5
 msgid "There is no configuration required here."
-msgstr "Keine Konfiguration nötig"
+msgstr "S’lypset formësim këtu."
 
 #: contrib/content/cms_plugins.py:30 contrib/content/forms.py:51
 msgid "Code"
-msgstr "Code"
+msgstr "Kod"
 
 #: contrib/content/cms_plugins.py:63 contrib/content/models.py:28
 msgid "Blockquote"
-msgstr "Blockquote"
+msgstr "Citat"
 
 #: contrib/content/cms_plugins.py:98 contrib/content/models.py:42
 msgid "Figure"
-msgstr "Abbildung"
+msgstr "Figurë"
 
 #: contrib/content/constants.py:4
 msgid "Inline code"
-msgstr "Inline-Code"
+msgstr "Kod brendazi"
 
 #: contrib/content/constants.py:5 contrib/content/models.py:14
 msgid "Code block"
-msgstr "Code-Block"
+msgstr "Bllok kodi"
 
 #: contrib/content/constants.py:6
 msgid "Variables"
-msgstr "Variablen"
+msgstr "Ndryshore"
 
 #: contrib/content/constants.py:7
 msgid "User input"
-msgstr "Benutzer-Eingabe"
+msgstr "Dhënie nga përdoruesi"
 
 #: contrib/content/constants.py:8
 msgid "Sample output"
-msgstr "Muster-Ausgabe"
+msgstr "Shembull dhënieje"
 
 #: contrib/content/forms.py:57
 msgid "Code type"
-msgstr "Code-Typ"
+msgstr "Lloj kodi"
 
 #: contrib/content/forms.py:90
 msgid "Quote"
-msgstr "Quote"
+msgstr "Citim"
 
 #: contrib/content/forms.py:95
 msgid "Source"
-msgstr "Quelle"
+msgstr "Burim"
 
 #: contrib/content/forms.py:132
 msgid "Caption"
-msgstr "Bildlegende"
+msgstr "Titull"
 
 #: contrib/grid/cms_plugins.py:36 contrib/grid/constants.py:19
 #: contrib/grid/models.py:28 contrib/navigation/forms.py:48
 msgid "Container"
-msgstr "Container"
+msgstr "Kontejner"
 
 #: contrib/grid/cms_plugins.py:72 contrib/grid/models.py:55
 msgid "Row"
-msgstr "Zeile"
+msgstr "Rresht"
 
 #: contrib/grid/cms_plugins.py:149 contrib/grid/models.py:79
 #: contrib/tabs/constants.py:15
 msgid "Column"
-msgstr "Spalte"
+msgstr "Shtyllë"
 
 #: contrib/grid/cms_plugins.py:184
 msgid "Title settings"
-msgstr "Titel-Einstellungen"
+msgstr "Rregullime titulli"
 
 #: contrib/grid/constants.py:20
 msgid "Fluid container"
-msgstr "Container mit voller Breite"
+msgstr ""
 
 #: contrib/grid/constants.py:21
 msgid "Full container"
-msgstr "Container mit voller Breite ohne Rand"
+msgstr "Kontejner i plotë"
 
 #: contrib/grid/constants.py:28
 msgid "Align items start"
-msgstr "Element-Ausrichtung Anfang"
+msgstr ""
 
 #: contrib/grid/constants.py:29
 msgid "Align items center"
-msgstr "Element-Ausrichtung Mittig"
+msgstr ""
 
 #: contrib/grid/constants.py:30
 msgid "Align items end"
-msgstr "Element-Ausrichtung Ende"
+msgstr ""
 
 #: contrib/grid/constants.py:34
 msgid "Justify content start"
-msgstr "Ausrichtung Inhalt Anfang"
+msgstr ""
 
 #: contrib/grid/constants.py:35
 msgid "Justify content center"
-msgstr "Ausrichtung Inhalt Mittig"
+msgstr ""
 
 #: contrib/grid/constants.py:36
 msgid "Justify content end"
-msgstr "Ausrichtung Inhalt Ende"
+msgstr ""
 
 #: contrib/grid/constants.py:37
 msgid "Justify content around"
-msgstr "Ausrichtung Inhalt herum"
+msgstr ""
 
 #: contrib/grid/constants.py:38
 msgid "Justify content between"
-msgstr "Ausrichtung Inhalt zwischen"
+msgstr ""
 
 #: contrib/grid/constants.py:42
 msgid "Align self start"
-msgstr "Selbst-Ausrichtung Anfang"
+msgstr ""
 
 #: contrib/grid/constants.py:43
 msgid "Align self center"
-msgstr "Selbst-Ausrichtung Mittig"
+msgstr ""
 
 #: contrib/grid/constants.py:44
 msgid "Align self end"
-msgstr "Selbst-Ausrichtung Ende"
+msgstr ""
 
 #: contrib/grid/forms.py:61
 msgid "Container type"
-msgstr "Container-Typ"
+msgstr "Lloj kontejneri"
 
 #: contrib/grid/forms.py:65
 msgid ""
 "Defines if the grid should use fixed width, fluid width or the container "
 "should fill the full width without margins or padding."
 msgstr ""
-"Legt fest, ob das Raster feste Breiten, variable Breiten nutzt oder der "
-"Container die volle Breite ohne Rand einnehmen soll."
+"Përcakton nëse rrjeta duhet të përdorë gjerësi të fiksuar, të ndryshueshme "
+"apo kontejneri duhet të mbushë gjerësinë e plotë, pa mënjana apo mbushje."
 
 #: contrib/grid/forms.py:97
 msgid "Create columns"
-msgstr "Spalten erstellen"
+msgstr "Krijoni shtylla"
 
 #: contrib/grid/forms.py:98
 msgid "Number of columns to create when saving."
-msgstr "Anzahl der Spalten, die beim Speichern erstellt werden soll."
+msgstr "Numër shtyllash për t’u krijuar, kur ruhet."
 
 #: contrib/grid/forms.py:104
 msgid "Vertical alignment"
-msgstr "Vertikale Ausrichtung"
+msgstr "Drejtim vertikalisht"
 
 #: contrib/grid/forms.py:111
 msgid "Horizontal alignment"
-msgstr "Horizontale Ausrichtung"
+msgstr "Drejtim horizontalisht"
 
 #: contrib/grid/forms.py:118
 msgid "Gutters"
-msgstr "Abstand"
+msgstr ""
 
 #: contrib/grid/forms.py:122
 msgid "To remove all spaces between rows set gutters to 0."
-msgstr "Um den Abstand zwischen den Spalten zu entfernen hier 0 eintragen."
+msgstr ""
 
 #: contrib/grid/forms.py:167
 msgid "Column alignment"
-msgstr "Spalten-Ausrichtung"
+msgstr "Drejtim shtylle"
 
 #: contrib/grid/forms.py:195
 #, python-format
 msgid ""
 "Column size needs to be empty, \"auto\", or a number between 1 and %(cols)d"
 msgstr ""
-"Spaltengröße muss entweder leer, \"auto\" oder eine Zahl zwischen 1 und "
-"%(cols)d sein."
+"Madhësia e shtyllës lypset të jetë e zbrazët, “auto”, ose një numër mes 1 "
+"dhe %(cols)d"
 
 #: contrib/grid/models.py:29
 msgid "GridContainer"
-msgstr "Container"
+msgstr ""
 
 #: contrib/grid/models.py:56
 msgid "GridRow"
-msgstr "Zeile"
+msgstr ""
 
 #: contrib/grid/models.py:64
 #, python-format
 msgid "(1 column)"
 msgid_plural "(%(count)i columns)"
-msgstr[0] "(1 Spalte)"
-msgstr[1] "(%(count)i Spalten)"
+msgstr[0] "(1 shtyllë)"
+msgstr[1] "(%(count)i shtylla)"
 
 #: contrib/grid/models.py:80
 msgid "GridColumn"
-msgstr "Spalte"
+msgstr ""
 
 #: contrib/grid/templates/djangocms_frontend/admin/grid_column.html:15
 msgid "Column size"
-msgstr "Spaltengröße"
+msgstr "Madhësi shtylle"
 
 #: contrib/grid/templates/djangocms_frontend/admin/grid_column.html:16
 msgid "Order"
-msgstr "Anordnung"
+msgstr "Renditje"
 
 #: contrib/grid/templates/djangocms_frontend/admin/grid_column.html:17
 msgid "Offset"
-msgstr "Versatz"
+msgstr "Shmangie"
 
 #: contrib/grid/templates/djangocms_frontend/admin/grid_column.html:18
 msgid "Margin left"
-msgstr "Rand links"
+msgstr "Mënjanë majtas"
 
 #: contrib/grid/templates/djangocms_frontend/admin/grid_column.html:19
 msgid "Margin right"
-msgstr "Rand rechts"
+msgstr "Mënjanë djathtas"
 
 #: contrib/grid/templates/djangocms_frontend/admin/grid_column.html:21
 msgid "Reset"
-msgstr "Zurücksetzen"
+msgstr "Riktheje te parazgjedhje"
 
 #: contrib/icon/apps.py:7 contrib/icon/cms_plugins.py:29
 #: contrib/icon/models.py:14
 msgid "Icon"
-msgstr "Icon"
+msgstr ""
 
 #: contrib/icon/conf.py:52
 msgid "Regular"
-msgstr "Schriftgröße"
+msgstr ""
 
 #: contrib/icon/conf.py:53
 msgid "x 2"
-msgstr "x 2"
+msgstr ""
 
 #: contrib/icon/conf.py:54
 msgid "x 3"
-msgstr "x 3"
+msgstr ""
 
 #: contrib/icon/conf.py:55
 msgid "x 4"
-msgstr "x 4"
+msgstr ""
 
 #: contrib/icon/conf.py:56
 msgid "x 5"
-msgstr "x 5"
+msgstr ""
 
 #: contrib/icon/conf.py:57
 msgid "x 8"
-msgstr "x 8"
+msgstr ""
 
 #: contrib/icon/conf.py:58
 msgid "x 12"
-msgstr "x 12"
+msgstr ""
 
 #: contrib/icon/forms.py:43
 msgid "Icon size"
-msgstr "Icon-Größe"
+msgstr ""
 
 #: contrib/icon/forms.py:49
 msgid "Foreground context"
-msgstr "Kontext für Vordergrund"
+msgstr ""
 
 #: contrib/icon/forms.py:56
 msgid "Circular icon"
-msgstr "Kreisförmiges Icon"
+msgstr ""
 
 #: contrib/icon/models.py:17
 msgid "undefined"
-msgstr "undefiniert"
+msgstr ""
 
 #: contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html:5
 msgid "Click to add icon"
-msgstr "Klicken zum Hinzufügen"
+msgstr ""
 
 #: contrib/image/cms_plugins.py:30
 msgid "Picture / Image"
-msgstr "Bild"
+msgstr "Foto / Figurë"
 
 #: contrib/image/cms_plugins.py:56
 msgid "Format"
-msgstr "Format"
+msgstr "Formatoje"
 
 #: contrib/image/cms_plugins.py:67
 msgid "Cropping"
-msgstr "Beschneiden"
+msgstr "Qethje"
 
 #: contrib/image/forms.py:25
 msgid "Align left"
-msgstr "Links ausrichten"
+msgstr "Vëre majtas"
 
 #: contrib/image/forms.py:26
 msgid "Align right"
-msgstr "Rechts ausrichten"
+msgstr "Vëre djathtas"
 
 #: contrib/image/forms.py:27
 msgid "Align center"
-msgstr "Zentriert ausrichten"
+msgstr "Vëre në qendër"
 
 #: contrib/image/forms.py:50 contrib/link/constants.py:22
 msgid "Open in new window"
-msgstr "In neuem Fenster öffnen"
+msgstr "Hape në dritare të re"
 
 #: contrib/image/forms.py:51 contrib/link/constants.py:23
 msgid "Open in same window"
-msgstr "Im selben Fenster öffnen"
+msgstr "Hape në të njëjtën dritare"
 
 #: contrib/image/forms.py:52 contrib/link/constants.py:24
 msgid "Delegate to parent"
-msgstr "An Elternelement delegieren"
+msgstr ""
 
 #: contrib/image/forms.py:53 contrib/link/constants.py:25
 msgid "Delegate to top"
-msgstr "An oberstes Element delegieren"
+msgstr ""
 
 #: contrib/image/forms.py:57
 msgid "Let settings.DJANGOCMS_PICTURE_RESPONSIVE_IMAGES decide"
-msgstr ""
-"Gemäß Einstellungen in "
-"<code>settings.DJANGOCMS_PICTURE_RESPONSIVE_IMAGES</code>"
+msgstr "Lëria settings.DJANGOCMS_PICTURE_RESPONSIVE_IMAGES të vendosë"
 
 #: contrib/image/forms.py:58
 msgid "Yes"
-msgstr "Ja"
+msgstr "Po"
 
 #: contrib/image/forms.py:59
 msgid "No"
-msgstr "Nein"
+msgstr "Jo"
 
 #: contrib/image/forms.py:111 contrib/image/models.py:71
 msgid "Image"
-msgstr "Bild"
+msgstr "Figurë"
 
 #: contrib/image/forms.py:115
 msgid "External image"
-msgstr "Externes Bild"
+msgstr "Figurë e jashtme"
 
 #: contrib/image/forms.py:118
 msgid ""
 "If provided, overrides the embedded image. Certain options such as cropping "
 "are not applicable to external images."
 msgstr ""
-"Wenn ein Verweis auf ein externes Bild angegeben wird, ersetzt es ein "
-"internes. Bestimmte Optionen (wie Auschnitte) können nicht auf externe "
-"Bilder angewendet werden."
+"Nëse jepet, anashkalon figurën e trupëzuar. Disa mundësi, bie fjala, qethja,"
+" s’janë të zbatueshme mbi figura të jashtme."
 
 #: contrib/image/forms.py:123
 msgid "Load lazily"
-msgstr "Nachgelagert laden"
+msgstr "Ngarkim dembel"
 
 #: contrib/image/forms.py:126
 msgid ""
 "Use for images below the fold. This will load images only if user scrolls "
 "them into view. "
 msgstr ""
-"Für Bilder unterhalb des sichtbaren Beriechs. Bild wird erst geladen, wenn "
-"der Nutzer scrollt und sie sichtbar werden."
+"Përdoreni për figura nën palosjen. Kjo do të ngarkojë figurat vetëm nëse "
+"përdoruesi rrëshqet në faqe dhe ato vijnë në pamje. "
 
 #: contrib/image/forms.py:131
 msgid "Width"
-msgstr "Breite"
+msgstr "Gjerësi"
 
 #: contrib/image/forms.py:135
 msgid "The image width as number in pixels. Example: \"720\" and not \"720px\"."
-msgstr "Bild-Breite in Pixeln (ohne Enheit). Beispiel: \"720\" and not \"720px\"."
+msgstr ""
+"Gjerësia e figurës si numër pikselash. Shembull: “720” dhe jo “720px”."
 
 #: contrib/image/forms.py:139
 msgid "Height"
-msgstr "Höhe"
+msgstr "Lartësi"
 
 #: contrib/image/forms.py:143
 msgid "The image height as number in pixels. Example: \"720\" and not \"720px\"."
-msgstr "Bild-Höhe in Pixeln (ohne Enheit). Beispiel: \"720\" and not \"720px\"."
+msgstr ""
+"Lartësia e figurës si numër pikselash. Shembull: “720” dhe jo “720px”."
 
 #: contrib/image/forms.py:150
 msgid "Aligns the image according to the selected option."
-msgstr "Richtet das Bild entsprechend der ausgewählten Option aus."
+msgstr "E drejton figurën sipas mundësisë së përzgjedhur."
 
 #: contrib/image/forms.py:153 contrib/utilities/forms.py:167
 msgid "Link attributes"
-msgstr "Link-Attribute"
+msgstr "Atribute lidhjeje"
 
 #: contrib/image/forms.py:154
 msgid "Attributes apply to the <b>link</b>."
-msgstr "Attribute werden auf den <b>Link</b> angewendet."
+msgstr "Atribute që aplikohen mbi <b>lidhjen</b>."
 
 #: contrib/image/forms.py:160
 msgid "Automatic scaling"
-msgstr "Automatische Skalierung"
+msgstr "Përshkallëzim automatik"
 
 #: contrib/image/forms.py:163
 msgid "Uses the placeholder dimensions to automatically calculate the size."
-msgstr "Skaliert das Bild autmatisch auf die Größe des Platzhalters."
+msgstr ""
+"Përdor përmasat e vendmbajtëses për të llogaritur automatikisht madhësinë."
 
 #: contrib/image/forms.py:169
 msgid "Use original image"
-msgstr "Original-Bild nutzen"
+msgstr "Përdor figurën origjinale"
 
 #: contrib/image/forms.py:171
 msgid "Outputs the raw image without cropping."
-msgstr "Erzeugt das Originalbild ohne Zuschneiden"
+msgstr "Jep figurën e papërpunuar pa qethje."
 
 #: contrib/image/forms.py:176
 msgid "Crop image"
-msgstr "Bild beschneiden"
+msgstr "Qetheni figurën"
 
 #: contrib/image/forms.py:179
 msgid ""
 "Crops the image according to the thumbnail settings provided in the "
 "template."
-msgstr ""
-"Schneidet das Bild gemäß der Vorschau-Einstellungen in der Vorlage zu."
+msgstr "E qeth figurën sipas rregullimeve miniaturash të dhëna te gjedhja."
 
 #: contrib/image/forms.py:183
 msgid "Upscale image"
-msgstr "Bildgröße anpassen"
+msgstr ""
 
 #: contrib/image/forms.py:186
 msgid ""
 "Upscales the image to the size of the thumbnail settings in the template."
-msgstr "Passt die Bildgröße auf die Vorschau-Einstellungen in der Vorlage"
+msgstr ""
 
 #: contrib/image/forms.py:190
 msgid "Use responsive image"
-msgstr "Bild responsive darstellen"
+msgstr "Përdor figurë reaguese"
 
 #: contrib/image/forms.py:194
 msgid ""
 "Uses responsive image technique to choose better image to display based upon"
 " screen viewport. This configuration only applies to uploaded images "
 "(external pictures will not be affected). "
 msgstr ""
-"Nutzt Responsive-Technologie, um die optimale Bildgröße auf Basis der "
-"Bildschirmgröße des Nutzers auszuwählen. Dies erfolgt nur bei hochgeladenen "
-"Bildern."
+"Përdor teknikën e figurave reaguese për të zgjedhur figurë më të mirë për "
+"shfaqje, bazuar në ekranin e parjes. Ky formësim zbatohet vetëm mbi figurat "
+"e ngarkuara (fotot e jashtme nuk do të preken prej kësaj). "
 
 #: contrib/image/forms.py:203
 msgid "Thumbnail options"
-msgstr "Optionen für Vorschaubilder"
+msgstr "Mundësi miniaturash"
 
 #: contrib/image/forms.py:206
 msgid ""
 "Overrides width, height, and crop; scales up to the provided preset "
 "dimensions."
 msgstr ""
-"Überschreibt Breite, Höhe und Zuschneide-Einstellungen. Passt die Bildgröße "
-"auf die Voreingestellung an."
+"Anashkalon gjerësi, lartësi dhe qethje, e bën sa përmasat e paracaktuara të "
+"dhëna."
 
 #: contrib/image/forms.py:210
 msgid "Responsive"
-msgstr "Responsive"
+msgstr "Reaguese"
 
 #: contrib/image/forms.py:213
 msgid "Adds the .img-fluid class to make the image responsive."
-msgstr "Fügt die Klasse .img-fluid hinzu um das Bild responsiv zu machen."
+msgstr "Shton klasën .img-fluid për ta bërë figurën reaguese."
 
 #: contrib/image/forms.py:216
 msgid "Rounded"
-msgstr "Abgerundet"
+msgstr "Rrumbullake"
 
 #: contrib/image/forms.py:219
 msgid "Adds the .rounded class for round corners."
-msgstr "Fügt die Klasse .rounded für abgerundete Ecken hinzu."
+msgstr "Shton klasën .rounded për cepa të rrumbullakët."
 
 #: contrib/image/forms.py:222
 msgid "Thumbnail"
-msgstr "Vorschaubild"
+msgstr "Miniaturë"
 
 #: contrib/image/forms.py:225
 msgid "Adds the .img-thumbnail class."
-msgstr "Fügt die Klasse .img-thumbnail hinzu."
+msgstr "Shton .img-thumbnail class."
 
 #: contrib/image/forms.py:246
 msgid ""
 "You have given more than one external, internal, or file link target. Only "
 "one option is allowed."
 msgstr ""
-"Nur ein Ziel kann angegbenen werden: Extern, intern oder eine Datei. Es ist "
-"mehr als ein Ziel ausgewählt."
+"Keni dhënë më shumë se një objektiv të jashtëm, të brendshëm, ose lidhje për"
+" te kartelë. Lejohet vetëm një mundësi."
 
 #: contrib/image/forms.py:255
 msgid ""
 "You need to add either an image, or a URL linking to an external image."
-msgstr "Entweder ein Bild oder eine URL für ein externed Bild angeben."
+msgstr ""
+"Lypset të shtoni ose një figurë, ose një URL që shpie te një figurë e "
+"jashtme."
 
 #: contrib/image/forms.py:281
 #, python-brace-format
 msgid ""
 "Invalid cropping settings. You cannot combine \"{field_a}\" with "
 "\"{field_b}\"."
 msgstr ""
-"Ungültige Zuschnitts-Einstellungen: \"{field_a}\" und \"{field_b}\" können "
-"nicht kombiniert werden."
+"Rregullime të pavlefshme qethjeje. S’mund të ndërthurni “{field_a}” me "
+"“{field_b}”."
 
 #: contrib/jumbotron/cms_plugins.py:31 contrib/jumbotron/models.py:14
 msgid "Jumbotron"
-msgstr "Jumbotron"
+msgstr ""
 
 #: contrib/jumbotron/forms.py:49 contrib/jumbotron/models.py:19
 msgid "Fluid"
-msgstr "Fließend"
+msgstr ""
 
 #: contrib/jumbotron/forms.py:53
 msgid "Makes the jumbotron fill the full width of the container or window."
 msgstr ""
-"Erweitert Jas Jumbotron auf die volle Breite des Containers oder Fensters."
+"E bën jumbotron-in të mbushë krejt gjerësinë e kontejnerit ose dritares."
 
 #: contrib/link/apps.py:11 contrib/link/constants.py:5
 #: contrib/link/models.py:11 contrib/link/models.py:114
 msgid "Link"
-msgstr "Link"
+msgstr "Lidhje"
 
 #: contrib/link/cms_plugins.py:97
 msgid "Link / Button"
-msgstr "Link / Button"
+msgstr "Lidhje / Buton"
 
 #: contrib/link/constants.py:6
 msgid "Button"
-msgstr "Button"
+msgstr "Buton"
 
 #: contrib/link/constants.py:10 frameworks/bootstrap5.py:7
 #: frameworks/bootstrap5.py:133
 msgid "Small"
-msgstr "Klein"
+msgstr "I vogël"
 
 #: contrib/link/constants.py:11 frameworks/bootstrap5.py:8
 #: frameworks/bootstrap5.py:134
 msgid "Medium"
-msgstr "Mittel"
+msgstr "Mesatar"
 
 #: contrib/link/constants.py:12 frameworks/bootstrap5.py:9
 #: frameworks/bootstrap5.py:135
 msgid "Large"
-msgstr "Groß"
+msgstr "I madh"
 
 #: contrib/link/forms.py:59
 msgid "Select a destination"
-msgstr "Ein Ziel auswählen"
+msgstr "Përzgjidhni vendmbërritje"
 
 #: contrib/link/forms.py:135
 msgid "Site"
-msgstr "Website"
+msgstr "Sajt"
 
 #: contrib/link/forms.py:138
 msgid "Select site"
-msgstr "Ein Ziel auswählen"
+msgstr "Përzgjidhni sajt"
 
 #: contrib/link/forms.py:143
 msgid "Url"
-msgstr "URL"
+msgstr "Url"
 
 #: contrib/link/forms.py:146
 msgid "Select URL object from list"
-msgstr "URL-Objekt aus der Liste wählen"
+msgstr "Përzgjidhni objekt URL nga lista"
 
 #: contrib/link/forms.py:174
 msgid "External link"
-msgstr "Externer Link"
+msgstr "Lidhje e jashtme"
 
 #: contrib/link/forms.py:177
 msgid "Provide a link to an external source."
-msgstr "Vollständiger Link zu einer externen Quelle"
+msgstr "Jepni një lidhje për te një burim i jashtëm."
 
 #: contrib/link/forms.py:180
 msgid "Internal link"
-msgstr "Interner Link"
+msgstr "Lidhje e brendshme"
 
 #: contrib/link/forms.py:182
 msgid "If provided, overrides the external link."
-msgstr "Wenn angegeben, wird ein externer Link überschrieben."
+msgstr "Në u dhëntë, anashkalon lidhjen e jashtme."
 
 #: contrib/link/forms.py:188
 msgid "File link"
-msgstr "Datei-Link"
+msgstr "Lidhje kartele"
 
 #: contrib/link/forms.py:190
 msgid "If provided links a file from the filer app."
-msgstr "Verlink eine Datei der Filer-App."
+msgstr "Në u dhëntë, lidh një kartelë prej një aplikacioni kartelash."
 
 #: contrib/link/forms.py:194
 msgid "Anchor"
-msgstr "Anker"
+msgstr "Spirancë"
 
 #: contrib/link/forms.py:197
 msgid ""
 "Appends the value only after the internal or external link. Do <em>not</em> "
 "include a preceding \"&#35;\" symbol."
 msgstr ""
-"Hängt bei internen oder externen Links einen Anker an. <em>Ohne</em> "
-"führendes \"&#35;\"-Symbol."
+"Shton vlerën vetëm pas lidhjes së brendshme, ose të jashtme. <em>Mos</em> "
+"përfshini një simbol paraprirës “&#35”."
 
 #: contrib/link/forms.py:202
 msgid "Email address"
-msgstr "Email-Adresse"
+msgstr "Adresë email"
 
 #: contrib/link/forms.py:206
 msgid "Phone"
-msgstr "Telefonnummer"
+msgstr "Telefon"
 
 #: contrib/link/forms.py:211
 msgid "Target"
-msgstr "Ziel"
+msgstr "Objektiv"
 
 #: contrib/link/forms.py:262
 #, python-brace-format
 msgid "Only one of {0} or {1} may be given."
-msgstr "Nur einer aus {0} oder {1} können ausgewählt werden."
+msgstr "Mund të jepet vetëm një nga {0} ose {1}."
 
 #: contrib/link/forms.py:274
 msgid "Please provide a link."
-msgstr "Bitte geben Sie ein Ziel an."
+msgstr "Ju lutemi, jepni një lidhje."
 
 #: contrib/link/forms.py:280
 #, python-format
 msgid ""
 "%(anchor_field_verbose_name)s is not allowed together with %(field_name)s"
-msgstr ""
-"%(anchor_field_verbose_name)s kann nicht zusammen mit %(field_name)s gewählt"
-" werden."
+msgstr "%(anchor_field_verbose_name)s nuk lejohet tok me %(field_name)s"
 
 #: contrib/link/forms.py:316
 msgid "Display name"
-msgstr "Anzeige-Text"
+msgstr "Emër në ekran"
 
 #: contrib/link/forms.py:325
 msgid "Stretch link"
-msgstr "Link ausdehnen"
+msgstr "Shformoje lidhjen"
 
 #: contrib/link/forms.py:329
 msgid ""
 "Stretches the active link area to the containing block (with position: "
 "relative)."
 msgstr ""
-"Dehnt die aktive Fläche des Link auf den umgebenden Block aus (sofern dieser"
-" mit position: relative markiert ist)."
+"E tendos fushën e lidhjes aktive sa blloku që e përmban (me pozicionin: "
+"relative)."
 
 #: contrib/link/forms.py:333 contrib/tabs/forms.py:51
 msgid "Type"
-msgstr "Typ"
+msgstr "Lloj"
 
 #: contrib/link/forms.py:337
 msgid "Adds either a text link or a button which links to the target."
-msgstr ""
-"Fügt entweder einen regulären Link oder einen Button hinzu, der das Ziel "
-"verlinkt."
+msgstr "Shton ose një lidhje tekst, ose një buton që shpie te objektivi."
 
 #: contrib/link/forms.py:347
 msgid "Button size"
-msgstr "Button-Größe"
+msgstr "Madhësi butoni"
 
 #: contrib/link/forms.py:356
 msgid "Outline"
-msgstr "Kontur"
+msgstr "Përvijim"
 
 #: contrib/link/forms.py:359
 msgid "Removes the coloring from a button and keeps the outline."
-msgstr "Beschränkt die Färbung auf den Umriß der Schaltfläche."
+msgstr "Heq ngjyrimin prej një butoni dhe mban vetëm përvijimin."
 
 #: contrib/link/forms.py:362
 msgid "Block"
-msgstr "Block"
+msgstr ""
 
 #: contrib/link/forms.py:365
 msgid "Extends the button to the width of its container."
-msgstr "Erweitert die Breite des Buttons auf den Container."
+msgstr "E zgjeron butonin sa gjerësia e kontejnerit përkatës."
 
 #: contrib/link/forms.py:368
 msgid "Icon left"
-msgstr "Icon links"
+msgstr "Ikonë majtas"
 
 #: contrib/link/forms.py:373
 msgid "Icon right"
-msgstr "Icon rechts"
+msgstr "Ikonë djathas"
 
 #: contrib/link/models.py:119
 msgid "<link is missing>"
-msgstr "<Link fehlt>"
+msgstr "<lidhja mungon>"
 
 #: contrib/link/templates/djangocms_frontend/admin/link.html:12
 msgid "Preview"
-msgstr "Vorschau"
+msgstr "Paraparje"
 
 #: contrib/listgroup/cms_plugins.py:28 contrib/listgroup/models.py:14
 msgid "List group"
-msgstr "Listen-Gruppe"
+msgstr ""
 
 #: contrib/listgroup/cms_plugins.py:55
 msgid "List item"
-msgstr "Listen-Eintrag"
+msgstr ""
 
 #: contrib/listgroup/constants.py:4
 msgid "Active"
-msgstr "Aktiv"
+msgstr "Aktive"
 
 #: contrib/listgroup/constants.py:5
 msgid "Disabled"
-msgstr "Deaktiviert"
+msgstr "E çaktivizuar"
 
 #: contrib/listgroup/forms.py:36
 msgid "List group flush"
-msgstr "Eingebettete Listen-Gruppe"
+msgstr ""
 
 #: contrib/listgroup/forms.py:39
 msgid "Create lists of content in a card with a flush list group."
 msgstr ""
-"Erstellt eine Listengruppe, die in einer Karte eingebettet werden kann."
 
 #: contrib/listgroup/forms.py:64
 msgid "One line content"
-msgstr "Inhalt (eine Zeile)"
+msgstr "Lëndë një rresht"
 
 #: contrib/listgroup/forms.py:67
 msgid "List item text. Is only show if this list item has no child plugins."
 msgstr ""
-"Text des Listen-Eintrags. Wird nur angezeigt, wenn der Listen-Eintrag keine "
-"Töchter-Plugins hat."
 
 #: contrib/listgroup/forms.py:78
 msgid "State"
-msgstr "Zustand"
+msgstr "Gjendje"
 
 #: contrib/listgroup/models.py:31
 msgid "List group item"
-msgstr "Listen-Eintrag"
+msgstr ""
 
 #: contrib/media/cms_plugins.py:23 contrib/media/models.py:14
 msgid "Media"
-msgstr "Medien"
+msgstr "Media"
 
 #: contrib/media/cms_plugins.py:40 contrib/media/models.py:28
 msgid "Media body"
-msgstr "Medienkörper"
+msgstr "Lëndë media"
 
 #: contrib/navigation/cms_plugins.py:29 contrib/navigation/models.py:15
 msgid "Navigation"
-msgstr "Navigation"
+msgstr "Lëvizje"
 
 #: contrib/navigation/cms_plugins.py:74 contrib/navigation/models.py:36
 msgid "Page tree"
-msgstr "Seitenbaum"
+msgstr "Pemë faqeje"
 
 #: contrib/navigation/cms_plugins.py:105 contrib/navigation/forms.py:104
 #: contrib/navigation/models.py:42
 msgid "Brand"
-msgstr "Marke"
+msgstr "Markë"
 
 #: contrib/navigation/cms_plugins.py:133 contrib/navigation/models.py:24
 msgid "Navigation container"
-msgstr "Navigationscontainer"
+msgstr "Kontejner Menuje Lëvizjesh"
 
 #: contrib/navigation/cms_plugins.py:164
 msgid "Navigation link"
-msgstr "Navigationsverweis"
+msgstr "Lidhje lëvizjeje"
 
 #: contrib/navigation/forms.py:45
 msgid "Defines the whole template set for this navigation."
-msgstr "Legt die Vorlagen für die Navigation fest."
+msgstr "Përcakton krejt grupin e gjedheve për këtë menu lëvizjesh."
 
 #: contrib/navigation/forms.py:53
 msgid "Design"
-msgstr "Design"
+msgstr ""
 
 #: contrib/navigation/forms.py:60
 msgid "Expand on device (and larger)"
-msgstr "Aufgeklappt für Gerät (oder größer)"
+msgstr "Zgjeroje në pajisje (dhe më të mëdha)"
 
 #: contrib/navigation/forms.py:81
 msgid "Start level"
-msgstr "Start-Ebene"
+msgstr "Nivel fillimi"
 
 #: contrib/navigation/forms.py:84
 msgid "Start level of this page tree (0: root, 1: level below root, etc.)"
-msgstr "Start-Ebene dieser Seite (0: Wurzel, 1: erste Ebene, ...)"
+msgstr ""
+"Nivel fillimi për këtë pemë faqesh (0: rrënjë, 1: niveli nën rrënjë, etj.)"
 
 #: contrib/navigation/forms.py:106
 msgid "Enter brand name or add child plugins for brand icon or image"
-msgstr "Marke eingeben oder Plugins für Markenlogo einfügen"
+msgstr ""
+"Jepni emër marke, ose shtoni shtojca pjellë për ikonë ose figurë marke"
 
 #: contrib/navigation/models.py:30
 msgid "Navigation Link"
-msgstr "Navigationsverweis"
+msgstr "Lidhje Lëvizjeje"
 
 #: contrib/tabs/cms_plugins.py:24 contrib/tabs/constants.py:5
 msgid "Tabs"
-msgstr "Reiter"
+msgstr "Skeda"
 
 #: contrib/tabs/cms_plugins.py:58 contrib/tabs/models.py:27
 msgid "Tab item"
-msgstr "Reiter-Eintrag"
+msgstr "Element skede"
 
 #: contrib/tabs/constants.py:6
 msgid "Pills"
-msgstr "Pillen-Form"
+msgstr "Sumbulla"
 
 #: contrib/tabs/constants.py:10
 msgid "Fill"
-msgstr "Füllung"
+msgstr "Mbushje"
 
 #: contrib/tabs/constants.py:11
 msgid "Justified"
-msgstr "Bündig"
+msgstr "Përligjur"
 
 #: contrib/tabs/constants.py:12
 msgid "Justify start"
-msgstr "Ausrichtung Anfang"
+msgstr ""
 
 #: contrib/tabs/constants.py:13
 msgid "Justify center"
-msgstr "Ausrichtung Mittig"
+msgstr ""
 
 #: contrib/tabs/constants.py:14
 msgid "Justify end"
-msgstr "Ausrichtung Ende"
+msgstr ""
 
 #: contrib/tabs/forms.py:64
 msgid "Index"
-msgstr "Index"
+msgstr "Tregues"
 
 #: contrib/tabs/forms.py:67
 msgid "Index of element to open on page load starting at 1."
 msgstr ""
-"Index des Elementes, das beim Öffnen der Seite gezeigt werden soll, startet "
-"bei 1."
+"Tregues elementësh për t’u hapur në ngarkim faqeje, duke filluar me 1."
 
 #: contrib/tabs/forms.py:70
 msgid "Animation effect"
-msgstr "Animationseffekt"
+msgstr "Efekt animacioni"
 
 #: contrib/tabs/forms.py:96
 msgid "Tab title"
-msgstr "Reiter-Titel"
+msgstr "Titull skede"
 
 #: contrib/tabs/forms.py:99
 msgid "Bordered"
-msgstr "Mit Rand"
+msgstr "Me anë"
 
 #: contrib/tabs/forms.py:101
 msgid "Add borders to the tab item"
-msgstr "Füge einen Rand zum Tab-Element hinzu"
+msgstr "Shto anë te objekti skedë"
 
 #: contrib/tabs/models.py:9
 msgid "Tab"
-msgstr "Reiter"
+msgstr "Skedë"
 
 #: contrib/utilities/cms_plugins.py:49
 msgid "Editor note"
-msgstr "Autoren-Anmerkung"
+msgstr "Shënim i redaktorit"
 
 #: contrib/utilities/cms_plugins.py:61 contrib/utilities/forms.py:120
 #: contrib/utilities/models.py:44
 msgid "Heading"
-msgstr "Überschrift"
+msgstr "Krye"
 
 #: contrib/utilities/cms_plugins.py:122 contrib/utilities/models.py:59
 msgid "Table of contents"
-msgstr "Inhaltsverzeichnis"
+msgstr "Tryezë e lëndës"
 
 #: contrib/utilities/forms.py:37
 msgid "Property"
-msgstr "Eigenschaft"
+msgstr "Veti"
 
 #: contrib/utilities/forms.py:43
 msgid "Sides"
-msgstr "Seiten"
+msgstr "Anë"
 
 #: contrib/utilities/forms.py:50
 msgid "Size"
-msgstr "Größe"
+msgstr "Madhësi"
 
 #: contrib/utilities/forms.py:56
 msgid "Device"
-msgstr "Gerät"
+msgstr "Pajisje"
 
 #: contrib/utilities/forms.py:74
 msgid ""
 "Padding does not have an auto spacing. Either switch to margin or a defined "
 "size."
 msgstr ""
-"\"Padding\" (innerer Abständ) hat keine automatische Größe. Entweder "
-"\"margin\" (äußerer Abstand) oder eine feste Größe wählen."
+"Mbushja s’ka aplikim vetvetiu hapësire. Ose kaloni te mënjanë, ose te një "
+"madhësi e përcaktuar."
 
 #: contrib/utilities/forms.py:78
 msgid ""
 "Padding does not have an auto spacing. Either switch to a defined size or "
 "change the spacing property."
 msgstr ""
-"\"Padding\" (innerer Abständ) hat keine automatische Größe. Entweder eine "
-"feste Größe oder \"marin\" (äußerer Abstand) wählen."
+"Mbushja s’ka aplikim vetvetiu hapësire. Ose kaloni te një madhësi e "
+"përcaktuar, ose ndryshoni vetinë për hapësira."
 
 #: contrib/utilities/forms.py:101 settings.py:38
 msgid "Heading 1"
-msgstr "Überschrift 1"
+msgstr "Krye 1"
 
 #: contrib/utilities/forms.py:102 settings.py:39
 msgid "Heading 2"
-msgstr "Überschrift 2"
+msgstr "Krye 2"
 
 #: contrib/utilities/forms.py:103 settings.py:40
 msgid "Heading 3"
-msgstr "Überschrift 3"
+msgstr "Krye 3"
 
 #: contrib/utilities/forms.py:104 settings.py:41
 msgid "Heading 4"
-msgstr "Überschrift 4"
+msgstr "Krye 4"
 
 #: contrib/utilities/forms.py:105 settings.py:42
 msgid "Heading 5"
-msgstr "Überschrift 5"
+msgstr "Krye 5"
 
 #: contrib/utilities/forms.py:114
 msgid "Heading level"
-msgstr "Überschrifts-Stufe"
+msgstr "Shkallë kryesh"
 
 #: contrib/utilities/forms.py:125
 msgid "ID"
 msgstr "ID"
 
 #: contrib/utilities/forms.py:128
 msgid ""
 "Fill in unique ID for table of contents. If empty heading will not appear in"
 " table of contents."
 msgstr ""
-"Eine eindeutige ID nimmt die Überschrift in das Inhaltsverzeichnis auf."
+"Plotësoni ID unike për tryezë lënde. Në u lëntë e zbrazët, kryet s’do të "
+"duken te tryezë e lëndës."
 
 #: contrib/utilities/forms.py:132
 msgid "Heading context"
-msgstr "Überschriften-Kontext"
+msgstr "Kontekst kryesh"
 
 #: contrib/utilities/forms.py:160
 msgid "List attributes"
-msgstr "Listen-Attribute"
+msgstr "Atribute liste"
 
 #: contrib/utilities/forms.py:162
 msgid ""
 "Attributes apply to the <b>list</b> for each level in the table of contents."
-msgstr ""
-"Attribute werden auf die auf die Liste für jede Einrückungstiefe im "
-"Inhaltesverzeichnis angewendet."
+msgstr "Atribute aplikohen te <b>lista</b> për çdo nivel te tryeza e lëndës."
 
 #: contrib/utilities/forms.py:169
 msgid ""
 "Attributes apply to the <b>link</b> for each entry in the table of contents."
-msgstr ""
-"Attribute werden auf die auf die Links für jeden Eintrag im "
-"Inhaltesverzeichnis angewendet."
+msgstr "Atribute aplikohen te <b>lidhja</b> për çdo nivel te tryeza e lëndës."
 
 #: contrib/utilities/forms.py:173
 msgid "Item attributes"
-msgstr "Listen-Element-Attribute"
+msgstr "Atribute objekti"
 
 #: contrib/utilities/forms.py:175
 msgid ""
 "Attributes apply to the <b>list items</b> for each entry in the table of "
 "contents."
 msgstr ""
-"Attribute werden auf die auf die Listen-Elemente für jeden Eintrag im "
-"Inhaltesverzeichnis angewendet."
+"Atribute aplikohen te <b>zëra liste</b> për çdo zë te tryeza e lëndës."
 
 #: fields.py:94
 msgid "Please select at least one device size"
-msgstr "Bitte mindestens eine Bildschirmgröße auswählen."
+msgstr "Ju lutemi, përzgjidhni të paktën një madhësi pajisjeje"
 
 #: fields.py:102 fields.py:110
 msgid "Attributes"
-msgstr "Attribute"
+msgstr "Atribute"
 
 #: fields.py:131
 msgid "Choices"
-msgstr "Optionen"
+msgstr "Zgjedhje"
 
 #: fields.py:142
 msgid ""
 "Please enter at least one choice. Use the <code>+</code> symbol to add a "
 "choice."
 msgstr ""
-"Mindestens eine Option angeben. <code>+</code>-Symbol nutzen, um eine Option"
-" hinzuzufügen."
+"Ju lutemi, jepni të paktën një zgjedhje. Që të shtoni një zgjedhje, përdorni"
+" simbolin <code>+</code>."
 
 #: fields.py:161 fields.py:175
 msgid "Tag type"
-msgstr "HTML-Tag"
+msgstr "Lloj etikete"
 
 #: fields.py:169
 msgid "Select the HTML tag to be used."
-msgstr "HTML-Tag auswählen, der genutzt werden soll."
+msgstr "Përzgjidhni etiketë HTML për t’u përdorur."
 
 #: frameworks/bootstrap5.py:6 frameworks/bootstrap5.py:132
 msgid "Extra small"
-msgstr "Sehr klein"
+msgstr ""
 
 #: frameworks/bootstrap5.py:10 frameworks/bootstrap5.py:136
 msgid "Extra large"
-msgstr "Sehr groß"
+msgstr ""
 
 #: frameworks/bootstrap5.py:11
 msgid "Extra-extra large"
-msgstr "XXL"
+msgstr ""
 
 #: frameworks/bootstrap5.py:19
 msgid "Primary"
-msgstr "Primär"
+msgstr "Parësore"
 
 #: frameworks/bootstrap5.py:20
 msgid "Secondary"
-msgstr "Sekundär"
+msgstr "Sekondare"
 
 #: frameworks/bootstrap5.py:21
 msgid "Success"
-msgstr "Erfolg"
+msgstr "Sukses"
 
 #: frameworks/bootstrap5.py:22
 msgid "Danger"
-msgstr "Gefahr"
+msgstr "Rrezik"
 
 #: frameworks/bootstrap5.py:23
 msgid "Warning"
-msgstr "Warnung"
+msgstr "Kujdes"
 
 #: frameworks/bootstrap5.py:24
 msgid "Info"
-msgstr "Info"
+msgstr "Hollësi"
 
 #: frameworks/bootstrap5.py:25 frameworks/bootstrap5.py:178
 msgid "Light"
-msgstr "Hell"
+msgstr "E çelët"
 
 #: frameworks/bootstrap5.py:26 frameworks/bootstrap5.py:179
 msgid "Dark"
-msgstr "Dunkel"
+msgstr "E errët"
 
 #: frameworks/bootstrap5.py:58 frameworks/bootstrap5.py:64
 msgid "Both"
-msgstr "Beide Seiten"
+msgstr "Që të dyja"
 
 #: frameworks/bootstrap5.py:65
 msgid "Top"
-msgstr "Oben"
+msgstr "Në krye"
 
 #: frameworks/bootstrap5.py:66
 msgid "Bottom"
-msgstr "Unten"
+msgstr "Në fund"
 
 #: frameworks/bootstrap5.py:91
 msgid "Screen"
-msgstr "Bildschirm"
+msgstr "Ekran"
 
 #: frameworks/bootstrap5.py:104
 msgid "Screen (minimum)"
-msgstr "Bildschirm (Minimum)"
+msgstr "Ekran (minimum)"
 
 #: frameworks/bootstrap5.py:124
 msgctxt "shadow"
 msgid "None"
-msgstr "Keiner"
+msgstr "Asnjë"
 
 #: frameworks/bootstrap5.py:137
 msgid "XX large"
-msgstr "XXL"
+msgstr ""
 
 #: helpers.py:112
 #, python-brace-format
 msgid "Read more in the <a href=\"{link}\" target=\"_blank\">documentation</a>."
-msgstr "Mehr in der <a href=\"{link}\" target=\"_blank\">Dokumentation</a>."
+msgstr "Lexoni më tepër, te <a href=\"{link}\" target=\"_blank\">dokumentimi</a>."
 
 #: models.py:24
 msgid "UI item"
-msgstr "Frontend-Element"
+msgstr "Element UI"
 
 #: settings.py:14
 msgid "There are no further settings for this plugin. Please press save."
 msgstr ""
-"Für dieses Plugin gibt es keine weiteren Einstellungen. Bitte klicken Sie "
-"\"Speichern\"."
+"S’ka rregullime të tjera për këtë shtojcë. Ju lutemi, shtypni “Ruaje”."
 
 #: settings.py:73
 msgid "Offcanvas"
-msgstr "Off-Canvas"
+msgstr ""
```

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/locale/fr/LC_MESSAGES/django.mo` & `djangocms-frontend-1.1.7/djangocms_frontend/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/locale/fr/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.7/djangocms_frontend/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/locale/nl/LC_MESSAGES/django.mo` & `djangocms-frontend-1.1.7/djangocms_frontend/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/locale/nl/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.7/djangocms_frontend/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo` & `djangocms-frontend-1.1.7/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/locale/sq/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.7/djangocms_frontend/locale/es/LC_MESSAGES/django.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,195 +1,190 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 # 
 # Translators:
-# Mark Walker <theshow@gmail.com>, 2023
-# Besnik Bleta <besnik@programeshqip.org>, 2023
+# Biel Frontera, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-03-11 17:20+0100\n"
 "PO-Revision-Date: 2023-01-20 15:48+0000\n"
-"Last-Translator: Besnik Bleta <besnik@programeshqip.org>, 2023\n"
-"Language-Team: Albanian (https://app.transifex.com/divio/teams/58664/sq/)\n"
+"Last-Translator: Biel Frontera, 2023\n"
+"Language-Team: Spanish (https://app.transifex.com/divio/teams/58664/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: sq\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: es\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: common/attributes.py:9
 msgid ""
 "Advanced settings lets you add html attributes to render this element. Use "
 "them wisely and rarely."
 msgstr ""
-"Rregullimet e mëtejshme ju lejojnë të shtoni atribute HTML për shfaqjen e "
-"këtij elementi. Përdoreni me mend dhe rrallë."
+"En las opciones avanzadas se pueden añadir atributos html de este elemento. "
+"Se debería utilizar con precaución y de forma ocasional."
 
 #: common/attributes.py:26 contrib/accordion/cms_plugins.py:91
 msgid "Advanced settings"
-msgstr "Rregullime të mëtejshme"
+msgstr "Opciones avanzadas"
 
 #: common/bootstrap5/background.py:20
 msgid "Background"
-msgstr "Sfond"
+msgstr "Fondo"
 
 #: common/bootstrap5/background.py:48
 msgid "Background context"
-msgstr "Kontekst sfondi"
+msgstr "Contexto del fondo"
 
 #: common/bootstrap5/background.py:52 contrib/card/forms.py:32
 #: contrib/card/models.py:7
 msgid "Transparent"
-msgstr "I tejdukshëm"
+msgstr "Transparente"
 
 #: common/bootstrap5/background.py:57
 msgid "Background opacity"
-msgstr "Patejdukshmëri sfondi"
+msgstr "Opacidad del fondo"
 
 #: common/bootstrap5/background.py:62
 msgid "Opacity of card background color (only if no outline selected)"
 msgstr ""
-"Patejdukshmëri e ngjyrës së sfondit të kartës (nëse s’është përzgjedhur "
-"përvijim)"
+"Opacidad del color de fondo de la tarjeta (solo si no se ha seleccionado "
+"contorno)"
 
 #: common/bootstrap5/background.py:66
 #: contrib/alert/frameworks/bootstrap5.py:42
 msgid "Shadow"
-msgstr "Hije"
+msgstr "Sombra"
 
 #: common/bootstrap5/background.py:71
 msgid "Use shadows to optically lift cards from the background."
-msgstr "Përdorni hije për t’i dalluar nga ana pamore kartat nga sfondi."
+msgstr ""
+"Utiliza la sombra para el efecto de elevación de la tarjeta respecto del "
+"fondo."
 
 #: common/bootstrap5/responsive.py:35
 msgid "Visibility"
-msgstr "Dukshmëri"
+msgstr "Visibilidad"
 
 #: common/bootstrap5/responsive.py:58
 msgid "Show element on device"
-msgstr "Shfaq elementin në pajisje"
+msgstr "Muestra el elemento en dispositivo"
 
 #: common/bootstrap5/responsive.py:60
 msgid "Select only devices on which this element should be shown."
-msgstr "Përzgjidhni vetëm pajisjet te të cilat ky element duhet shfaqur."
+msgstr "Selecciona los dispositivos en los que este elemento se debe mostrar."
 
 #: common/bootstrap5/sizing.py:8 common/spacing.py:11
 #: contrib/utilities/forms.py:51 frameworks/bootstrap5.py:90
 #: frameworks/bootstrap5.py:103
 msgid "Auto"
-msgstr "Auto"
+msgstr "Automático"
 
 #: common/bootstrap5/sizing.py:44
 msgid "Horizontal size"
-msgstr "Madhësi horizontale"
+msgstr "Ancho"
 
 #: common/bootstrap5/sizing.py:50
 msgid ""
 "Sets the horizontal size relative to the surrounding container or the "
 "viewport."
-msgstr ""
-"Cakton madhësinë horizontale, relative ndaj kontejnerit ose pjesës së "
-"ekranit që e rrethon."
+msgstr "Configura el ancho relativo a su contenedor o el viewport."
 
 #: common/bootstrap5/sizing.py:54
 msgid "Vertical size"
-msgstr "Madhësi vertikale"
+msgstr "Alto"
 
 #: common/bootstrap5/sizing.py:60
 msgid ""
 "Sets the vertical size relative to the surrounding container or the "
 "viewport."
-msgstr ""
-"Cakton madhësinë vertikale, relative ndaj kontejnerit ose pjesës së ekranit "
-"që e rrethon."
+msgstr "Configura el alto relativo a su contenedor o el viewport."
 
 #: common/spacing.py:84
 msgid "Please choose a side to which the spacing should be applied."
-msgstr "Ju lutemi, zgjidhni një anë mbi të cilën duhet aplikuar hapësira."
+msgstr "Selecciona una opción para indicar donde se aplicará el espaciado."
 
 #: common/spacing.py:113
 msgid "Margin"
-msgstr "Mënjanë"
+msgstr "Margen"
 
 #: common/spacing.py:139 common/spacing.py:147
 msgid "Padding"
-msgstr "Mbushje"
+msgstr "Padding"
 
 #: common/spacing.py:175 contrib/utilities/cms_plugins.py:22
 #: contrib/utilities/models.py:14
 msgid "Spacing"
-msgstr "Hapësirë"
+msgstr "Espaciado"
 
 #: common/spacing.py:189
 msgid "Horizontal margin"
-msgstr "Mënjanë horizontale"
+msgstr "Margen horizontal"
 
 #: common/spacing.py:195
 msgid "Vertical margin"
-msgstr "Mënjanë vertikale"
+msgstr "Margen vertical"
 
 #: common/spacing.py:201
 msgid "Apply margin on device"
-msgstr "Apliko mënjanë te pajisja"
+msgstr "Aplica el margen en dispositivo"
 
 #: common/spacing.py:204
 msgid ""
 "Select only devices on which the margin should be applied. On other devices "
 "larger than the first selected device the margin will be set to zero."
 msgstr ""
-"Përgjidhni një anë mbi të cilën duhet aplikuar hapësira. Select only devices"
-" on which the margin should be applied. On other devices larger than the "
-"first selected device the margin will be set to zero."
+"Selecciona aquellos dispositivos en los que el margen se aplicará. En los "
+"dispositivos superiores a los seleccionados, el margen será cero."
 
 #: common/spacing.py:221
 msgid "Horizontal padding"
-msgstr "Mbushje horizontale"
+msgstr "Padding horizontal"
 
 #: common/spacing.py:227
 msgid "Vertical padding"
-msgstr "Mbushje vertikale"
+msgstr "Padding vertical"
 
 #: common/spacing.py:233
 msgid "Apply padding on device"
-msgstr "Apliko mbushje te pajisja"
+msgstr "Aplica el padding en dispositivo"
 
 #: common/spacing.py:236
 msgid ""
 "Select only devices on which the padding should be applied. On other devices"
 " larger than the first selected device the padding will be set to zero."
 msgstr ""
-"Përzgjidhni vetëm pajisjet mbi të cilat duhet aplikuar mbushja. Në pajisje "
-"të tjera, më të mëdha se pajisja e parë e përzgjedhur, mbushja do të "
-"caktohet si zero."
+"Selecciona aquellos dispositivos en los que el padding se aplicará. En los "
+"dispositivos superiores a los seleccionados, el padding será cero."
 
 #: common/title.py:40
 msgid "Please add a title if you want to publish it."
-msgstr "Ju lutemi, shtoni një titull, nëse doni të botohet."
+msgstr "Añade un título para publicar."
 
 #: common/title.py:64
 msgid "Title"
-msgstr "Titull"
+msgstr "Título"
 
 #: common/title.py:67
 msgid ""
 "Optional title of the plugin for easier identification. Its "
 "<code>title</code> attribute will only be set if the checkbox is selected."
 msgstr ""
-"Titull i shtojcës, në daçi, për identifikim më të kollajtë. Atributi "
-"<code>title</code> për të do të ujdiset vetëm nëse përzgjidhet kutiza."
+"Título opcional de la extensión para su mejor identificación. El atributo "
+"<code>title</code> solo se asignará si se selecciona la casilla."
 
 #: contrib/accordion/cms_plugins.py:21 contrib/accordion/models.py:14
 msgid "Accordion"
-msgstr "Fizarmonikë"
+msgstr "Acordeón"
 
 #: contrib/accordion/cms_plugins.py:22 contrib/accordion/cms_plugins.py:72
 #: contrib/alert/cms_plugins.py:25 contrib/badge/cms_plugins.py:21
 #: contrib/card/cms_plugins.py:25 contrib/card/cms_plugins.py:86
 #: contrib/card/cms_plugins.py:146 contrib/carousel/cms_plugins.py:26
 #: contrib/carousel/cms_plugins.py:71 contrib/collapse/cms_plugins.py:21
 #: contrib/collapse/cms_plugins.py:50 contrib/collapse/cms_plugins.py:76
@@ -203,1470 +198,1487 @@
 #: contrib/navigation/cms_plugins.py:30 contrib/navigation/cms_plugins.py:75
 #: contrib/navigation/cms_plugins.py:106 contrib/navigation/cms_plugins.py:134
 #: contrib/navigation/cms_plugins.py:165 contrib/tabs/cms_plugins.py:25
 #: contrib/tabs/cms_plugins.py:59 contrib/utilities/cms_plugins.py:23
 #: contrib/utilities/cms_plugins.py:50 contrib/utilities/cms_plugins.py:62
 #: contrib/utilities/cms_plugins.py:123
 msgid "Frontend"
-msgstr "Pjesa e dukshme"
+msgstr "Frontend"
 
 #: contrib/accordion/cms_plugins.py:57
 msgid "Item {}"
-msgstr "Objekt {}"
+msgstr "Elemento {}"
 
 #: contrib/accordion/cms_plugins.py:71 contrib/accordion/models.py:33
 msgid "Accordion item"
-msgstr "Objekt fizarmonike"
+msgstr "Elemento de acordeón"
 
 #: contrib/accordion/forms.py:34
 msgid "Create accordion items"
-msgstr "Krijoni objekte fizarmonikë"
+msgstr "Crea elementos de acordeón"
 
 #: contrib/accordion/forms.py:35
 msgid "Number of accordion items to create when saving."
-msgstr "Numër objektesh fizarmonikë për t’u krijuar, kur ruhet."
+msgstr "Número de elementos de acordeón a crear al guardar."
 
 #: contrib/accordion/forms.py:42
 msgid "Header type"
-msgstr "Lloj kryesh"
+msgstr "Tipo de encabezado"
 
 #: contrib/accordion/forms.py:48
 msgid "Integrate into parent"
-msgstr "Integroje te mëma"
+msgstr "Integra en su contenedor"
 
 #: contrib/accordion/forms.py:52
 msgid ""
 "Removes the default background-color, some borders, and some rounded corners"
 " to render accordions edge-to-edge with their parent container "
 msgstr ""
-"Bën heqjen e ngjyrës parazgjedhje për sfondin, disa anë dhe disa cepa të "
-"rrumbullakosur, për t’i shfaqur fizarmonikat nga skaji në skaj, me "
-"kontejnerin e tyre mëmë "
+"Elimina el color de fondo por defecto, algunos bordes y algunas esquinas "
+"redondeadas para renderizar los acordeones de borde a borde de su contenedor"
 
 #: contrib/accordion/forms.py:78 contrib/card/constants.py:16
 msgid "Header"
-msgstr "Krye"
+msgstr "Encabezado"
 
 #: contrib/accordion/forms.py:82
 msgid "Item open"
-msgstr ""
+msgstr "Elemento abierto"
 
 #: contrib/accordion/forms.py:85
 msgid "Initially shows this accordion item on page load."
-msgstr "E shfaq fillimisht këtë objekt fizarmonikë gjatë ngarkimit të faqes."
+msgstr "Muestra este elemento abierto al cargar la página."
 
 #: contrib/accordion/models.py:20
 msgid "({} entries)"
-msgstr "({} zëra)"
+msgstr "({} elementos)"
 
 #: contrib/accordion/models.py:29
 msgid "AccordionItem"
-msgstr ""
+msgstr "Elemento-Acordeón"
 
 #: contrib/alert/cms_plugins.py:24 contrib/alert/models.py:14
 msgid "Alert"
-msgstr "Sinjalizim"
+msgstr "Alerta"
 
 #: contrib/alert/forms.py:41 contrib/badge/forms.py:37
 #: contrib/link/forms.py:340 contrib/listgroup/forms.py:71
 msgid "Context"
-msgstr "Kontekst"
+msgstr "Contexto"
 
 #: contrib/alert/forms.py:47
 msgid "Dismissible"
-msgstr "Që mund të hidhet tej"
+msgstr "Descartable"
 
 #: contrib/alert/forms.py:50
 msgid "Allows the alert to be closed."
-msgstr "Lejon mbylljen e sinjalizimit."
+msgstr "Permite que la alerta se pueda cerrar."
 
 #: contrib/alert/frameworks/bootstrap5.py:47
 msgid "Use shadows to optically lift alerts from the background."
-msgstr "Përdorni hije për t’i dalluar nga ana pamore sinjalizimet nga sfondi."
+msgstr ""
+"Utiliza la sombra para el efecto de elevación de la alerta respecto del "
+"fondo."
 
 #: contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html:4
 msgid "Close"
-msgstr "Mbylle"
+msgstr "Cerrar"
 
 #: contrib/badge/cms_plugins.py:20 contrib/badge/models.py:14
 msgid "Badge"
-msgstr "Stemë"
+msgstr "Insignia"
 
 #: contrib/badge/forms.py:33
 msgid "Badge text"
-msgstr "Tekst i stemës"
+msgstr "Texto de la insignia"
 
 #: contrib/badge/forms.py:43
 msgid "Pills style"
-msgstr "Stil sumbullash"
+msgstr "Estilo de píldora"
 
 #: contrib/badge/forms.py:46
 msgid "Activates the pills style."
-msgstr "Aktivizon stilin e sumbullave."
+msgstr "Activa el estilo de píldora."
 
 #: contrib/card/cms_plugins.py:24 contrib/card/models.py:20
 msgid "Card layout"
-msgstr "Skemë karte"
+msgstr "Layout de la tarjeta"
 
 #: contrib/card/cms_plugins.py:47 contrib/grid/cms_plugins.py:93
 #: contrib/grid/cms_plugins.py:173
 msgid "Responsive settings"
-msgstr "Rregullime reaguese"
+msgstr "Opciones responsive"
 
 #: contrib/card/cms_plugins.py:85 contrib/card/models.py:35
 msgid "Card"
-msgstr "Kartë"
+msgstr "Tarjeta"
 
 #: contrib/card/cms_plugins.py:145 contrib/card/models.py:57
 msgid "Card inner"
-msgstr ""
+msgstr "Interior de la tarjeta"
 
 #: contrib/card/constants.py:4
 msgid "Card group"
-msgstr "Grup karte"
+msgstr "Grupo de tarjetas"
 
 #: contrib/card/constants.py:5
 msgid "Grid cards"
-msgstr ""
+msgstr "Cuadrícula de tarjetas"
 
 #: contrib/card/constants.py:9 contrib/utilities/forms.py:108
 #: frameworks/bootstrap5.py:59 settings.py:47
 msgid "Left"
-msgstr "Majtas"
+msgstr "Izquierda"
 
 #: contrib/card/constants.py:10 contrib/utilities/forms.py:109 settings.py:48
 msgid "Center"
-msgstr "Në qendër"
+msgstr "Centro"
 
 #: contrib/card/constants.py:11 contrib/utilities/forms.py:110
 #: frameworks/bootstrap5.py:60 settings.py:49
 msgid "Right"
-msgstr "Djathtas"
+msgstr "Derecha"
 
 #: contrib/card/constants.py:15
 msgid "Body"
-msgstr "Lëndë"
+msgstr "Cuerpo"
 
 #: contrib/card/constants.py:17
 msgid "Footer"
-msgstr "Fundfaqe"
+msgstr "Pie"
 
 #: contrib/card/constants.py:18
 msgid "Image overlay"
-msgstr ""
+msgstr "Superposición de imagen"
 
 #: contrib/card/forms.py:35 contrib/card/models.py:9
 msgid "White"
-msgstr "E bardhë"
+msgstr "Blanco"
 
 #: contrib/card/forms.py:61
 msgid "Create cards"
-msgstr "Krijoni karta"
+msgstr "Crea tarjetas"
 
 #: contrib/card/forms.py:62
 msgid "Number of cards to create when saving."
-msgstr "Numër kartash për t’u krijuar, kur ruhet."
+msgstr "Número de tarjetas a crear al guardar."
 
 #: contrib/card/forms.py:68
 msgid "Card type"
-msgstr "Lloj karte"
+msgstr "Tipo de tarjeta"
 
 #: contrib/card/forms.py:122
 msgid "Card outline context"
-msgstr ""
+msgstr "Contexto del contorno de la tarjeta"
 
 #: contrib/card/forms.py:126
 msgid "Uses the border to indicate context."
-msgstr "Përdor anën për të treguar kontekstin."
+msgstr "Usa el borde para indicar el contexto."
 
 #: contrib/card/forms.py:132 contrib/content/forms.py:99
 #: contrib/content/forms.py:137 contrib/grid/cms_plugins.py:99
 #: contrib/image/forms.py:147 contrib/tabs/forms.py:57
 #: contrib/utilities/forms.py:139
 msgid "Alignment"
-msgstr "Drejtim"
+msgstr "Alineación"
 
 #: contrib/card/forms.py:140
 msgid "Text context"
-msgstr "Kontekst teksti"
+msgstr "Contexto del texto"
 
 #: contrib/card/forms.py:148
 msgid "Full height"
-msgstr "Lartësi e plotë"
+msgstr "Altura completa"
 
 #: contrib/card/forms.py:152
 msgid ""
 "If checked cards in one row will automatically extend to the full row "
 "height."
 msgstr ""
-"Në iu vëntë shenjë, kartat e një rreshti do të zgjerohen vetvetiu sa "
-"lartësia e plotë e rreshtit."
+"Las tarjetas que se muestren en la misma fila se extenderán hasta la altura "
+"de la fila."
 
 #: contrib/card/forms.py:186
 msgid "Inner type"
-msgstr "Lloj i Brendshëm"
+msgstr "Tipo de interior"
 
 #: contrib/card/forms.py:189
 msgid "Define the structure of the plugin."
-msgstr "Përcaktoni strukturën e shtojcës."
+msgstr "Define la estructura de la extensión."
 
 #: contrib/card/forms.py:193 contrib/grid/forms.py:173
 msgid "Content alignment"
-msgstr "Drejtim lënde"
+msgstr "Alineación del contenido"
 
 #: contrib/card/templates/djangocms_frontend/admin/card_layout.html:14
 #: contrib/grid/templates/djangocms_frontend/admin/grid_row.html:13
 msgid "Colums per row"
-msgstr "Shtylla për rresht"
+msgstr "Columnas por fila"
 
 #: contrib/carousel/cms_plugins.py:25 contrib/carousel/models.py:20
 msgid "Carousel"
-msgstr "Rrotullame"
+msgstr "Carrusel"
 
 #: contrib/carousel/cms_plugins.py:70 contrib/carousel/models.py:42
 msgid "Carousel slide"
-msgstr "Rrëshqitës rrotullame"
+msgstr "Diapositiva de carrusel"
 
 #: contrib/carousel/cms_plugins.py:88 contrib/link/cms_plugins.py:45
 #: contrib/link/cms_plugins.py:83
 msgid "Link settings"
-msgstr "Rregullime lidhjesh"
+msgstr "Opciones del enlace"
 
 #: contrib/carousel/constants.py:5
 msgid "On hover"
-msgstr ""
+msgstr "Al pasar por encima"
 
 #: contrib/carousel/constants.py:6
 msgid "Never"
-msgstr ""
+msgstr "Nunca"
 
 #: contrib/carousel/constants.py:12 contrib/image/forms.py:39
 #: contrib/tabs/constants.py:27 settings.py:56 settings.py:64 settings.py:72
 msgid "Default"
-msgstr "Parazgjedhje"
+msgstr "Valor por defecto"
 
 #: contrib/carousel/constants.py:36
 msgid "Slide"
-msgstr ""
+msgstr "Diapositiva"
 
 #: contrib/carousel/constants.py:37 contrib/tabs/constants.py:21
 msgid "Fade"
-msgstr "Zbehje"
+msgstr "Desvanece (fade)"
 
 #: contrib/carousel/forms.py:58 contrib/image/forms.py:103
 #: contrib/jumbotron/forms.py:44 contrib/link/forms.py:320
 #: contrib/navigation/forms.py:42 contrib/tabs/forms.py:45
 msgid "Template"
-msgstr "Gjedhe"
+msgstr "Plantilla"
 
 #: contrib/carousel/forms.py:61 contrib/tabs/forms.py:48
 msgid "This is the template that will be used for the component."
-msgstr "Kjo është gjedhja që do të përdoret për përbërësin."
+msgstr "Plantilla que se utilizará para el componente."
 
 #: contrib/carousel/forms.py:64 contrib/carousel/models.py:24
 msgid "Interval"
-msgstr "Interval"
+msgstr "Intervalo"
 
 #: contrib/carousel/forms.py:67
 msgid ""
 "The amount of time to delay between automatically cycling an item. If false,"
 " carousel will not automatically cycle."
 msgstr ""
-"Sasia e kohës në sekonda për vonim zërash te kalimi automatikisht në ta. Në "
-"u vëntë 0, rrotullamja s’do të kalojë automatikisht nëpër ta."
+"Tiempo de espera entre las transiciones automáticas de elementos. Si no se "
+"selecciona, el carrusel no realizará transiciones automáticas."
 
 #: contrib/carousel/forms.py:72 contrib/carousel/models.py:25
 msgid "Controls"
-msgstr "Kontrolle"
+msgstr "Controles"
 
 #: contrib/carousel/forms.py:75
 msgid "Adding in the previous and next controls."
-msgstr "Po shtohen kontrollet “i mëparshmi” dhe “pasuesi”."
+msgstr ""
+"Añade los controles para pasar a la diapositiva anterior y la siguiente."
 
 #: contrib/carousel/forms.py:78 contrib/carousel/models.py:26
 msgid "Indicators"
-msgstr "Tregues"
+msgstr "Indicadores"
 
 #: contrib/carousel/forms.py:81
 msgid "Adding in the indicators to the carousel."
-msgstr "Po shtohen treguesit te rrotullamja."
+msgstr "Añade los indicadores de diapositiva en el carrusel."
 
 #: contrib/carousel/forms.py:84 contrib/carousel/models.py:27
 msgid "Keyboard"
-msgstr "Tastierë"
+msgstr "Teclado"
 
 #: contrib/carousel/forms.py:87
 msgid "Whether the carousel should react to keyboard events."
-msgstr "Nëse duhet të reagojë apo jo rrotullamja ndaj aktesh tastiere."
+msgstr "Permite que el carrusel reaccione a eventos del teclado."
 
 #: contrib/carousel/forms.py:90 contrib/carousel/models.py:28
 msgid "Pause"
-msgstr "Ndalesë"
+msgstr "Pausa"
 
 #: contrib/carousel/forms.py:94
 msgid ""
 "If set to \"hover\", pauses the cycling of the carousel on \"mouseenter\" "
 "and resumes the cycling of the carousel on \"mouseleave\". If set to "
 "\"false\", hovering over the carousel won't pause it."
 msgstr ""
-"Në u vëntë si “hover”, e ndal rrotullimin e rrotullames pas një akti "
-"“mouseenter” dhe e rifillon rrotullimin e rrotullames pas një akti "
-"“mouseleave”. Në u vëntë si “false”, kalimi i kursorit mbi rrotullamen s’do "
-"ta ndalë atë."
+"Si se selecciona \"Al pasar por encima\", las transiciones se pausan con el "
+"evento \"mouseenter\" y se reanudan con el evento \"mouseleave\". Si se "
+"selecciona \"Nunca\", las transiciones no se pausan cuando el cursor está "
+"encima del carrusel."
 
 #: contrib/carousel/forms.py:102
 msgid "Auto start"
-msgstr ""
+msgstr "Reproduce automáticamente"
 
 #: contrib/carousel/forms.py:106
 msgid ""
 "Autoplays the carousel after the user manually cycles the first item. If "
 "\"carousel\", autoplays the carousel on load."
-msgstr ""
-"Vetëluhet rrotullamja, pasi përdoruesi vë në punë dorazi kuadrin e parë. Në "
-"u vëntë “carousel”, vetëluhet automatikisht rrotullamja, kur ngarkohet "
-"faqja."
+msgstr "Reproduce automáticamente el carrusel al cargar la página."
 
 #: contrib/carousel/forms.py:111 contrib/carousel/models.py:30
 msgid "Wrap"
 msgstr ""
 
 #: contrib/carousel/forms.py:115
 msgid "Whether the carousel should cycle continuously or have hard stops."
-msgstr ""
-"Nëse rrotullamja duhet të rrotullohet vazhdimisht, apo të ketë ndalesa."
+msgstr "Si el carrusel debe circular continuamente o tener paradas bruscas."
 
 #: contrib/carousel/forms.py:119
 msgid "Aspect ratio"
-msgstr "Përpjesëtim"
+msgstr "Relación de aspecto"
 
 #: contrib/carousel/forms.py:124
 msgid ""
 "Determines width and height of the image according to the selected ratio."
 msgstr ""
-"Përcakton gjerësinë dhe lartësinë e fizarmonikës së figurave sa përpjesëtimi"
-" i përzgjedhur."
+"Calcula el ancho y el alto de la imagen en función de la relación de aspecto"
+" seleccionada."
 
 #: contrib/carousel/forms.py:129
 msgid "Transition"
-msgstr ""
+msgstr "Transición"
 
 #: contrib/carousel/forms.py:133
 msgid "Determines if slides change by sliding or fading."
 msgstr ""
+"Determina si la transición entre las dispositivas es por desplazamiento o "
+"por desvanecimiento."
 
 #: contrib/carousel/forms.py:177
 msgid "Slide image"
-msgstr ""
+msgstr "Imagen de la diapositiva"
 
 #: contrib/carousel/forms.py:181
 msgid "Content"
-msgstr "Lëndë"
+msgstr "Contenido"
 
 #: contrib/carousel/forms.py:184
 msgid "Content may also be added using child plugins."
-msgstr "Lëndë mund të shtohet edhe duke përdorur shtojca pjellë."
+msgstr "El contenido también se puede añadir utilizando extensiones hijas."
 
 #: contrib/carousel/models.py:29
 msgid "Ride"
-msgstr ""
+msgstr "Animación"
 
 #: contrib/carousel/models.py:51 contrib/image/models.py:154
 msgid "<file is missing>"
-msgstr "<kartela mungon>"
+msgstr "<sin imagen>"
 
 #: contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html:32
 msgid "Previous"
-msgstr "E mëparshmja"
+msgstr "Anterior"
 
 #: contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html:36
 msgid "Next"
-msgstr "Pasuesja"
+msgstr "Siguiente"
 
 #: contrib/collapse/cms_plugins.py:20 contrib/collapse/models.py:21
 msgid "Collapse"
-msgstr "Tkurre"
+msgstr "Colapsa"
 
 #: contrib/collapse/cms_plugins.py:49 contrib/collapse/models.py:35
 msgid "Collapse trigger"
-msgstr ""
+msgstr "Trigger de colapso"
 
 #: contrib/collapse/cms_plugins.py:75 contrib/collapse/models.py:49
 msgid "Collapse container"
-msgstr "Tkurre kontejnerin"
+msgstr "Contenedor para colapsar"
 
 #: contrib/collapse/forms.py:37
 msgid "Siblings"
-msgstr ""
+msgstr "Hermanos"
 
 #: contrib/collapse/forms.py:40
 msgid "Element to be used to create accordions."
-msgstr "Element i përdorur për të krijuar fizarmonika."
+msgstr ""
 
 #: contrib/collapse/forms.py:63 contrib/collapse/forms.py:88
 msgid "Unique identifier"
-msgstr "Identifikues unik"
+msgstr "Identificador único"
 
 #: contrib/collapse/forms.py:65 contrib/collapse/forms.py:90
 msgid "Identifier to connect trigger with container."
-msgstr "Identifikues për të lidhur shkaktues me kontejner."
+msgstr "Identificador para conectar el trigger con el contenedor."
 
 #: contrib/collapse/templates/djangocms_frontend/admin/collapse.html:7
 #: contrib/media/templates/djangocms_frontend/admin/media.html:7
 #: contrib/utilities/templates/djangocms_frontend/admin/no_form.html:5
 msgid "There is no configuration required here."
-msgstr "S’lypset formësim këtu."
+msgstr "No hay ninguna configuración necesaria en esta extensión."
 
 #: contrib/content/cms_plugins.py:30 contrib/content/forms.py:51
 msgid "Code"
-msgstr "Kod"
+msgstr "Código"
 
 #: contrib/content/cms_plugins.py:63 contrib/content/models.py:28
 msgid "Blockquote"
-msgstr "Citat"
+msgstr "Bloque de cita"
 
 #: contrib/content/cms_plugins.py:98 contrib/content/models.py:42
 msgid "Figure"
-msgstr "Figurë"
+msgstr "Figura"
 
 #: contrib/content/constants.py:4
 msgid "Inline code"
-msgstr "Kod brendazi"
+msgstr "Código en línia"
 
 #: contrib/content/constants.py:5 contrib/content/models.py:14
 msgid "Code block"
-msgstr "Bllok kodi"
+msgstr "Bloque de código"
 
 #: contrib/content/constants.py:6
 msgid "Variables"
-msgstr "Ndryshore"
+msgstr "Variables"
 
 #: contrib/content/constants.py:7
 msgid "User input"
-msgstr "Dhënie nga përdoruesi"
+msgstr "Input de usuario"
 
 #: contrib/content/constants.py:8
 msgid "Sample output"
-msgstr "Shembull dhënieje"
+msgstr "Ejemplo de output"
 
 #: contrib/content/forms.py:57
 msgid "Code type"
-msgstr "Lloj kodi"
+msgstr "Tipo de código"
 
 #: contrib/content/forms.py:90
 msgid "Quote"
-msgstr "Citim"
+msgstr "Cita"
 
 #: contrib/content/forms.py:95
 msgid "Source"
-msgstr "Burim"
+msgstr "Fuente"
 
 #: contrib/content/forms.py:132
 msgid "Caption"
-msgstr "Titull"
+msgstr "Descripción de la imagen"
 
 #: contrib/grid/cms_plugins.py:36 contrib/grid/constants.py:19
 #: contrib/grid/models.py:28 contrib/navigation/forms.py:48
 msgid "Container"
-msgstr "Kontejner"
+msgstr "Contenedor"
 
 #: contrib/grid/cms_plugins.py:72 contrib/grid/models.py:55
 msgid "Row"
-msgstr "Rresht"
+msgstr "Fila"
 
 #: contrib/grid/cms_plugins.py:149 contrib/grid/models.py:79
 #: contrib/tabs/constants.py:15
 msgid "Column"
-msgstr "Shtyllë"
+msgstr "Columna"
 
 #: contrib/grid/cms_plugins.py:184
 msgid "Title settings"
-msgstr "Rregullime titulli"
+msgstr "Opciones del título"
 
 #: contrib/grid/constants.py:20
 msgid "Fluid container"
-msgstr ""
+msgstr "Contenedor fluido"
 
 #: contrib/grid/constants.py:21
 msgid "Full container"
-msgstr "Kontejner i plotë"
+msgstr "Contenedor ancho completo"
 
 #: contrib/grid/constants.py:28
 msgid "Align items start"
-msgstr ""
+msgstr "Alinea los elementos al principio"
 
 #: contrib/grid/constants.py:29
 msgid "Align items center"
-msgstr ""
+msgstr "Alinea los elementos en el centro"
 
 #: contrib/grid/constants.py:30
 msgid "Align items end"
-msgstr ""
+msgstr "Alinea los elementos al final"
 
 #: contrib/grid/constants.py:34
 msgid "Justify content start"
-msgstr ""
+msgstr "Justifica el contenido al principio"
 
 #: contrib/grid/constants.py:35
 msgid "Justify content center"
-msgstr ""
+msgstr "Justifica el contenido en el centro"
 
 #: contrib/grid/constants.py:36
 msgid "Justify content end"
-msgstr ""
+msgstr "Justifica el contenido al final"
 
 #: contrib/grid/constants.py:37
 msgid "Justify content around"
-msgstr ""
+msgstr "Justifica el contenido alrededor"
 
 #: contrib/grid/constants.py:38
 msgid "Justify content between"
-msgstr ""
+msgstr "Justifica el contenido entre los elementos"
 
 #: contrib/grid/constants.py:42
 msgid "Align self start"
-msgstr ""
+msgstr "Auto-alinea al principio"
 
 #: contrib/grid/constants.py:43
 msgid "Align self center"
-msgstr ""
+msgstr "Auto-alinea en el centro"
 
 #: contrib/grid/constants.py:44
 msgid "Align self end"
-msgstr ""
+msgstr "Auto-alinea al final"
 
 #: contrib/grid/forms.py:61
 msgid "Container type"
-msgstr "Lloj kontejneri"
+msgstr "Tipo de contenedor"
 
 #: contrib/grid/forms.py:65
 msgid ""
 "Defines if the grid should use fixed width, fluid width or the container "
 "should fill the full width without margins or padding."
 msgstr ""
-"Përcakton nëse rrjeta duhet të përdorë gjerësi të fiksuar, të ndryshueshme "
-"apo kontejneri duhet të mbushë gjerësinë e plotë, pa mënjana apo mbushje."
+"Define si el contenedor usará un ancho fijo, fluido o con el ancho máximo "
+"sin márgenes ni padding."
 
 #: contrib/grid/forms.py:97
 msgid "Create columns"
-msgstr "Krijoni shtylla"
+msgstr "Crear columnas"
 
 #: contrib/grid/forms.py:98
 msgid "Number of columns to create when saving."
-msgstr "Numër shtyllash për t’u krijuar, kur ruhet."
+msgstr "Número de columnas a crear al guardar."
 
 #: contrib/grid/forms.py:104
 msgid "Vertical alignment"
-msgstr "Drejtim vertikalisht"
+msgstr "Alineación vertical"
 
 #: contrib/grid/forms.py:111
 msgid "Horizontal alignment"
-msgstr "Drejtim horizontalisht"
+msgstr "Alineación horizontal"
 
 #: contrib/grid/forms.py:118
 msgid "Gutters"
 msgstr ""
 
 #: contrib/grid/forms.py:122
 msgid "To remove all spaces between rows set gutters to 0."
 msgstr ""
+"Para eliminar todos los espacios entre las filas, pon el valor de gutters a "
+"0."
 
 #: contrib/grid/forms.py:167
 msgid "Column alignment"
-msgstr "Drejtim shtylle"
+msgstr "Alineación de la columna"
 
 #: contrib/grid/forms.py:195
 #, python-format
 msgid ""
 "Column size needs to be empty, \"auto\", or a number between 1 and %(cols)d"
 msgstr ""
-"Madhësia e shtyllës lypset të jetë e zbrazët, “auto”, ose një numër mes 1 "
-"dhe %(cols)d"
+"El tamaño de la columna debe estar vacío o ser \"auto\" o un número entre 1 "
+"y%(cols)d"
 
 #: contrib/grid/models.py:29
 msgid "GridContainer"
 msgstr ""
 
 #: contrib/grid/models.py:56
 msgid "GridRow"
 msgstr ""
 
 #: contrib/grid/models.py:64
 #, python-format
 msgid "(1 column)"
 msgid_plural "(%(count)i columns)"
-msgstr[0] "(1 shtyllë)"
-msgstr[1] "(%(count)i shtylla)"
+msgstr[0] "(1 columna)"
+msgstr[1] "(%(count)i columnas)"
+msgstr[2] "(%(count)i columnas)"
 
 #: contrib/grid/models.py:80
 msgid "GridColumn"
 msgstr ""
 
 #: contrib/grid/templates/djangocms_frontend/admin/grid_column.html:15
 msgid "Column size"
-msgstr "Madhësi shtylle"
+msgstr "Tamaño de la columna"
 
 #: contrib/grid/templates/djangocms_frontend/admin/grid_column.html:16
 msgid "Order"
-msgstr "Renditje"
+msgstr "Orden"
 
 #: contrib/grid/templates/djangocms_frontend/admin/grid_column.html:17
 msgid "Offset"
-msgstr "Shmangie"
+msgstr ""
 
 #: contrib/grid/templates/djangocms_frontend/admin/grid_column.html:18
 msgid "Margin left"
-msgstr "Mënjanë majtas"
+msgstr "Margen izquierdo"
 
 #: contrib/grid/templates/djangocms_frontend/admin/grid_column.html:19
 msgid "Margin right"
-msgstr "Mënjanë djathtas"
+msgstr "Margen derecho"
 
 #: contrib/grid/templates/djangocms_frontend/admin/grid_column.html:21
 msgid "Reset"
-msgstr "Riktheje te parazgjedhje"
+msgstr ""
 
 #: contrib/icon/apps.py:7 contrib/icon/cms_plugins.py:29
 #: contrib/icon/models.py:14
 msgid "Icon"
-msgstr ""
+msgstr "Icono"
 
 #: contrib/icon/conf.py:52
 msgid "Regular"
-msgstr ""
+msgstr "Normal"
 
 #: contrib/icon/conf.py:53
 msgid "x 2"
-msgstr ""
+msgstr "x 2"
 
 #: contrib/icon/conf.py:54
 msgid "x 3"
-msgstr ""
+msgstr "x 3"
 
 #: contrib/icon/conf.py:55
 msgid "x 4"
-msgstr ""
+msgstr "x 4"
 
 #: contrib/icon/conf.py:56
 msgid "x 5"
-msgstr ""
+msgstr "x 5"
 
 #: contrib/icon/conf.py:57
 msgid "x 8"
-msgstr ""
+msgstr "x 8"
 
 #: contrib/icon/conf.py:58
 msgid "x 12"
-msgstr ""
+msgstr "x 12"
 
 #: contrib/icon/forms.py:43
 msgid "Icon size"
-msgstr ""
+msgstr "Tamaño del icono"
 
 #: contrib/icon/forms.py:49
 msgid "Foreground context"
-msgstr ""
+msgstr "Contexto del primer plano"
 
 #: contrib/icon/forms.py:56
 msgid "Circular icon"
-msgstr ""
+msgstr "Icono circular"
 
 #: contrib/icon/models.py:17
 msgid "undefined"
-msgstr ""
+msgstr "Sin definir"
 
 #: contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html:5
 msgid "Click to add icon"
-msgstr ""
+msgstr "Clica para añadir un icono"
 
 #: contrib/image/cms_plugins.py:30
 msgid "Picture / Image"
-msgstr "Foto / Figurë"
+msgstr "Imagen"
 
 #: contrib/image/cms_plugins.py:56
 msgid "Format"
-msgstr "Formatoje"
+msgstr "Formato"
 
 #: contrib/image/cms_plugins.py:67
 msgid "Cropping"
-msgstr "Qethje"
+msgstr "Recorte"
 
 #: contrib/image/forms.py:25
 msgid "Align left"
-msgstr "Vëre majtas"
+msgstr "Alinear a la izquierda"
 
 #: contrib/image/forms.py:26
 msgid "Align right"
-msgstr "Vëre djathtas"
+msgstr "Alinear a la derecha"
 
 #: contrib/image/forms.py:27
 msgid "Align center"
-msgstr "Vëre në qendër"
+msgstr "Centrar"
 
 #: contrib/image/forms.py:50 contrib/link/constants.py:22
 msgid "Open in new window"
-msgstr "Hape në dritare të re"
+msgstr "Abrir en nueva ventana"
 
 #: contrib/image/forms.py:51 contrib/link/constants.py:23
 msgid "Open in same window"
-msgstr "Hape në të njëjtën dritare"
+msgstr "Abrir en la misma ventana"
 
 #: contrib/image/forms.py:52 contrib/link/constants.py:24
 msgid "Delegate to parent"
-msgstr ""
+msgstr "Abrir en el frame anterior"
 
 #: contrib/image/forms.py:53 contrib/link/constants.py:25
 msgid "Delegate to top"
-msgstr ""
+msgstr "Abrir en el frame superior"
 
 #: contrib/image/forms.py:57
 msgid "Let settings.DJANGOCMS_PICTURE_RESPONSIVE_IMAGES decide"
-msgstr "Lëria settings.DJANGOCMS_PICTURE_RESPONSIVE_IMAGES të vendosë"
+msgstr "Configura según settings.DJANGOCMS_PICTURE_RESPONSIVE_IMAGES"
 
 #: contrib/image/forms.py:58
 msgid "Yes"
-msgstr "Po"
+msgstr "Sí"
 
 #: contrib/image/forms.py:59
 msgid "No"
-msgstr "Jo"
+msgstr "No"
 
 #: contrib/image/forms.py:111 contrib/image/models.py:71
 msgid "Image"
-msgstr "Figurë"
+msgstr "Imagen"
 
 #: contrib/image/forms.py:115
 msgid "External image"
-msgstr "Figurë e jashtme"
+msgstr "Imagen externa"
 
 #: contrib/image/forms.py:118
 msgid ""
 "If provided, overrides the embedded image. Certain options such as cropping "
 "are not applicable to external images."
 msgstr ""
-"Nëse jepet, anashkalon figurën e trupëzuar. Disa mundësi, bie fjala, qethja,"
-" s’janë të zbatueshme mbi figura të jashtme."
+"Si se introduce, sobrescribe la imagen añadida. Algunas opciones como el "
+"recorte no se pueden aplicar a las imágenes externas."
 
 #: contrib/image/forms.py:123
 msgid "Load lazily"
-msgstr "Ngarkim dembel"
+msgstr "Carga lazy"
 
 #: contrib/image/forms.py:126
 msgid ""
 "Use for images below the fold. This will load images only if user scrolls "
 "them into view. "
 msgstr ""
-"Përdoreni për figura nën palosjen. Kjo do të ngarkojë figurat vetëm nëse "
-"përdoruesi rrëshqet në faqe dhe ato vijnë në pamje. "
+"Útil en imágenes fuera de la vista inicial. La imagen se cargará cuando el "
+"usuario mueva la página hasta la ubicación de la imagen. "
 
 #: contrib/image/forms.py:131
 msgid "Width"
-msgstr "Gjerësi"
+msgstr "Ancho"
 
 #: contrib/image/forms.py:135
 msgid "The image width as number in pixels. Example: \"720\" and not \"720px\"."
-msgstr ""
-"Gjerësia e figurës si numër pikselash. Shembull: “720” dhe jo “720px”."
+msgstr "El ancho de la imagen como número en píxeles. Ejemplo: \"720\" y no \"720px\""
 
 #: contrib/image/forms.py:139
 msgid "Height"
-msgstr "Lartësi"
+msgstr "Altura"
 
 #: contrib/image/forms.py:143
 msgid "The image height as number in pixels. Example: \"720\" and not \"720px\"."
 msgstr ""
-"Lartësia e figurës si numër pikselash. Shembull: “720” dhe jo “720px”."
+"La altura de la imagen como número en píxeles. Ejemplo: \"720\" y no "
+"\"720px\""
 
 #: contrib/image/forms.py:150
 msgid "Aligns the image according to the selected option."
-msgstr "E drejton figurën sipas mundësisë së përzgjedhur."
+msgstr "Alinea la imagen según la opción seleccionada."
 
 #: contrib/image/forms.py:153 contrib/utilities/forms.py:167
 msgid "Link attributes"
-msgstr "Atribute lidhjeje"
+msgstr "Atributos del enlace"
 
 #: contrib/image/forms.py:154
 msgid "Attributes apply to the <b>link</b>."
-msgstr "Atribute që aplikohen mbi <b>lidhjen</b>."
+msgstr "Atributos que se aplicarán al <b>enlace</b>."
 
 #: contrib/image/forms.py:160
 msgid "Automatic scaling"
-msgstr "Përshkallëzim automatik"
+msgstr "Escalado automático"
 
 #: contrib/image/forms.py:163
 msgid "Uses the placeholder dimensions to automatically calculate the size."
 msgstr ""
-"Përdor përmasat e vendmbajtëses për të llogaritur automatikisht madhësinë."
+"Usa las dimensiones del contenedor para calcular automáticamente el tamaño."
 
 #: contrib/image/forms.py:169
 msgid "Use original image"
-msgstr "Përdor figurën origjinale"
+msgstr "Utiliza la imagen original"
 
 #: contrib/image/forms.py:171
 msgid "Outputs the raw image without cropping."
-msgstr "Jep figurën e papërpunuar pa qethje."
+msgstr "Muestra la imagen sin ningún recorte."
 
 #: contrib/image/forms.py:176
 msgid "Crop image"
-msgstr "Qetheni figurën"
+msgstr "Recorte de la imagen"
 
 #: contrib/image/forms.py:179
 msgid ""
 "Crops the image according to the thumbnail settings provided in the "
 "template."
-msgstr "E qeth figurën sipas rregullimeve miniaturash të dhëna te gjedhja."
+msgstr ""
+"Recorta la imagen según las opciones de miniatura proporcionadas en la "
+"plantilla."
 
 #: contrib/image/forms.py:183
 msgid "Upscale image"
-msgstr ""
+msgstr "Aumento de tamaño de la imagen"
 
 #: contrib/image/forms.py:186
 msgid ""
 "Upscales the image to the size of the thumbnail settings in the template."
 msgstr ""
+"Escala la imagen hasta el tamaño de las opciones de las miniaturas en la "
+"plantilla."
 
 #: contrib/image/forms.py:190
 msgid "Use responsive image"
-msgstr "Përdor figurë reaguese"
+msgstr "Utiliza imagen responsive"
 
 #: contrib/image/forms.py:194
 msgid ""
 "Uses responsive image technique to choose better image to display based upon"
 " screen viewport. This configuration only applies to uploaded images "
 "(external pictures will not be affected). "
 msgstr ""
-"Përdor teknikën e figurave reaguese për të zgjedhur figurë më të mirë për "
-"shfaqje, bazuar në ekranin e parjes. Ky formësim zbatohet vetëm mbi figurat "
-"e ngarkuara (fotot e jashtme nuk do të preken prej kësaj). "
+"Utiliza la técnica de imagen adaptable para seleccionar las dimensiones de "
+"la imagen en función del tamaño de la pantalla. Esta configuración solo se "
+"aplica a imágenes subidas (las imágenes externas no se verán afectadas). "
 
 #: contrib/image/forms.py:203
 msgid "Thumbnail options"
-msgstr "Mundësi miniaturash"
+msgstr "Opciones de miniatura"
 
 #: contrib/image/forms.py:206
 msgid ""
 "Overrides width, height, and crop; scales up to the provided preset "
 "dimensions."
 msgstr ""
-"Anashkalon gjerësi, lartësi dhe qethje, e bën sa përmasat e paracaktuara të "
-"dhëna."
+"Sobrescribe las opciones de ancho, alto y recorte; escala hasta las "
+"dimensiones predefinidas."
 
 #: contrib/image/forms.py:210
 msgid "Responsive"
-msgstr "Reaguese"
+msgstr "Responsive"
 
 #: contrib/image/forms.py:213
 msgid "Adds the .img-fluid class to make the image responsive."
-msgstr "Shton klasën .img-fluid për ta bërë figurën reaguese."
+msgstr "Añade la clase .img-fluid para hacer la imagen responsive."
 
 #: contrib/image/forms.py:216
 msgid "Rounded"
-msgstr "Rrumbullake"
+msgstr "Redondeado"
 
 #: contrib/image/forms.py:219
 msgid "Adds the .rounded class for round corners."
-msgstr "Shton klasën .rounded për cepa të rrumbullakët."
+msgstr "Añade la clase .rounder para redondear las esquinas."
 
 #: contrib/image/forms.py:222
 msgid "Thumbnail"
-msgstr "Miniaturë"
+msgstr "Miniatura"
 
 #: contrib/image/forms.py:225
 msgid "Adds the .img-thumbnail class."
-msgstr "Shton .img-thumbnail class."
+msgstr "Añade la clase .img-thumbnail."
 
 #: contrib/image/forms.py:246
 msgid ""
 "You have given more than one external, internal, or file link target. Only "
 "one option is allowed."
 msgstr ""
-"Keni dhënë më shumë se një objektiv të jashtëm, të brendshëm, ose lidhje për"
-" te kartelë. Lejohet vetëm një mundësi."
+"Solo se permite rellenar una opción entre externo, interno o enlace a "
+"fichero."
 
 #: contrib/image/forms.py:255
 msgid ""
 "You need to add either an image, or a URL linking to an external image."
-msgstr ""
-"Lypset të shtoni ose një figurë, ose një URL që shpie te një figurë e "
-"jashtme."
+msgstr "Debes introducir o una imagen o un enlace a una imagen externa."
 
 #: contrib/image/forms.py:281
 #, python-brace-format
 msgid ""
 "Invalid cropping settings. You cannot combine \"{field_a}\" with "
 "\"{field_b}\"."
 msgstr ""
-"Rregullime të pavlefshme qethjeje. S’mund të ndërthurni “{field_a}” me "
-"“{field_b}”."
+"Opciones de recorte inválidas. No puedes combinar \"{field_a}\" con "
+"\"{field_b}\"."
 
 #: contrib/jumbotron/cms_plugins.py:31 contrib/jumbotron/models.py:14
 msgid "Jumbotron"
 msgstr ""
 
 #: contrib/jumbotron/forms.py:49 contrib/jumbotron/models.py:19
 msgid "Fluid"
-msgstr ""
+msgstr "Fluido"
 
 #: contrib/jumbotron/forms.py:53
 msgid "Makes the jumbotron fill the full width of the container or window."
 msgstr ""
-"E bën jumbotron-in të mbushë krejt gjerësinë e kontejnerit ose dritares."
+"Configura el jumbotron para que ocupe todo el ancho del contenedor o de la "
+"ventana."
 
 #: contrib/link/apps.py:11 contrib/link/constants.py:5
 #: contrib/link/models.py:11 contrib/link/models.py:114
 msgid "Link"
-msgstr "Lidhje"
+msgstr "Enlace"
 
 #: contrib/link/cms_plugins.py:97
 msgid "Link / Button"
-msgstr "Lidhje / Buton"
+msgstr "Enlace / Botón"
 
 #: contrib/link/constants.py:6
 msgid "Button"
-msgstr "Buton"
+msgstr "Botón"
 
 #: contrib/link/constants.py:10 frameworks/bootstrap5.py:7
 #: frameworks/bootstrap5.py:133
 msgid "Small"
-msgstr "I vogël"
+msgstr "Pequeño"
 
 #: contrib/link/constants.py:11 frameworks/bootstrap5.py:8
 #: frameworks/bootstrap5.py:134
 msgid "Medium"
-msgstr "Mesatar"
+msgstr "Medio"
 
 #: contrib/link/constants.py:12 frameworks/bootstrap5.py:9
 #: frameworks/bootstrap5.py:135
 msgid "Large"
-msgstr "I madh"
+msgstr "Grande"
 
 #: contrib/link/forms.py:59
 msgid "Select a destination"
-msgstr "Përzgjidhni vendmbërritje"
+msgstr "Selecciona un destino"
 
 #: contrib/link/forms.py:135
 msgid "Site"
-msgstr "Sajt"
+msgstr "Sitio web"
 
 #: contrib/link/forms.py:138
 msgid "Select site"
-msgstr "Përzgjidhni sajt"
+msgstr "Selecciona el sitio web"
 
 #: contrib/link/forms.py:143
 msgid "Url"
-msgstr "Url"
+msgstr "URL"
 
 #: contrib/link/forms.py:146
 msgid "Select URL object from list"
-msgstr "Përzgjidhni objekt URL nga lista"
+msgstr "Selecciona una URL de la lista"
 
 #: contrib/link/forms.py:174
 msgid "External link"
-msgstr "Lidhje e jashtme"
+msgstr "Enlace externo"
 
 #: contrib/link/forms.py:177
 msgid "Provide a link to an external source."
-msgstr "Jepni një lidhje për te një burim i jashtëm."
+msgstr "Configura el enlace hacia una web externa."
 
 #: contrib/link/forms.py:180
 msgid "Internal link"
-msgstr "Lidhje e brendshme"
+msgstr "Enlace interno"
 
 #: contrib/link/forms.py:182
 msgid "If provided, overrides the external link."
-msgstr "Në u dhëntë, anashkalon lidhjen e jashtme."
+msgstr "Si se selecciona, sobrescribe el enlace externo."
 
 #: contrib/link/forms.py:188
 msgid "File link"
-msgstr "Lidhje kartele"
+msgstr "Enlace a fichero"
 
 #: contrib/link/forms.py:190
 msgid "If provided links a file from the filer app."
-msgstr "Në u dhëntë, lidh një kartelë prej një aplikacioni kartelash."
+msgstr "Si se selecciona, enlaza a un fichero de la aplicación Filer."
 
 #: contrib/link/forms.py:194
 msgid "Anchor"
-msgstr "Spirancë"
+msgstr "Ancla"
 
 #: contrib/link/forms.py:197
 msgid ""
 "Appends the value only after the internal or external link. Do <em>not</em> "
 "include a preceding \"&#35;\" symbol."
 msgstr ""
-"Shton vlerën vetëm pas lidhjes së brendshme, ose të jashtme. <em>Mos</em> "
-"përfshini një simbol paraprirës “&#35”."
+"Añade el valor solo después del enlace interno o externo. <em>No</em> debes "
+"incluir el símbolo \"&#35;\" como prefijo."
 
 #: contrib/link/forms.py:202
 msgid "Email address"
-msgstr "Adresë email"
+msgstr "Correo electrónico"
 
 #: contrib/link/forms.py:206
 msgid "Phone"
-msgstr "Telefon"
+msgstr "Teléfono"
 
 #: contrib/link/forms.py:211
 msgid "Target"
-msgstr "Objektiv"
+msgstr "Objetivo"
 
 #: contrib/link/forms.py:262
 #, python-brace-format
 msgid "Only one of {0} or {1} may be given."
-msgstr "Mund të jepet vetëm një nga {0} ose {1}."
+msgstr "Sólo se puede utilizar o bien {0} o bien {1}."
 
 #: contrib/link/forms.py:274
 msgid "Please provide a link."
-msgstr "Ju lutemi, jepni një lidhje."
+msgstr "Introduce un enlace."
 
 #: contrib/link/forms.py:280
 #, python-format
 msgid ""
 "%(anchor_field_verbose_name)s is not allowed together with %(field_name)s"
-msgstr "%(anchor_field_verbose_name)s nuk lejohet tok me %(field_name)s"
+msgstr ""
+"%(anchor_field_verbose_name)s no se permite conjuntamente con "
+"%(field_name)s."
 
 #: contrib/link/forms.py:316
 msgid "Display name"
-msgstr "Emër në ekran"
+msgstr "Nombre a mostrar"
 
 #: contrib/link/forms.py:325
 msgid "Stretch link"
-msgstr "Shformoje lidhjen"
+msgstr "Enlace estirado"
 
 #: contrib/link/forms.py:329
 msgid ""
 "Stretches the active link area to the containing block (with position: "
 "relative)."
 msgstr ""
-"E tendos fushën e lidhjes aktive sa blloku që e përmban (me pozicionin: "
-"relative)."
+"Estira el enlace para hacer que se pueda hacer clic en su bloque contenedor "
+"(con position: relative)."
 
 #: contrib/link/forms.py:333 contrib/tabs/forms.py:51
 msgid "Type"
-msgstr "Lloj"
+msgstr "Tipo"
 
 #: contrib/link/forms.py:337
 msgid "Adds either a text link or a button which links to the target."
-msgstr "Shton ose një lidhje tekst, ose një buton që shpie te objektivi."
+msgstr "Configura el enlace como enlace de texto o como botón."
 
 #: contrib/link/forms.py:347
 msgid "Button size"
-msgstr "Madhësi butoni"
+msgstr "Tamaño del botón"
 
 #: contrib/link/forms.py:356
 msgid "Outline"
-msgstr "Përvijim"
+msgstr "Contorno"
 
 #: contrib/link/forms.py:359
 msgid "Removes the coloring from a button and keeps the outline."
-msgstr "Heq ngjyrimin prej një butoni dhe mban vetëm përvijimin."
+msgstr "Elimina el color de fondo del botón y mantiene el contorno."
 
 #: contrib/link/forms.py:362
 msgid "Block"
-msgstr ""
+msgstr "Bloque"
 
 #: contrib/link/forms.py:365
 msgid "Extends the button to the width of its container."
-msgstr "E zgjeron butonin sa gjerësia e kontejnerit përkatës."
+msgstr "Extiende el botón al ancho de su contenedor."
 
 #: contrib/link/forms.py:368
 msgid "Icon left"
-msgstr "Ikonë majtas"
+msgstr "Icono izquierda"
 
 #: contrib/link/forms.py:373
 msgid "Icon right"
-msgstr "Ikonë djathas"
+msgstr "Icono derecha"
 
 #: contrib/link/models.py:119
 msgid "<link is missing>"
-msgstr "<lidhja mungon>"
+msgstr "<sin enlace>"
 
 #: contrib/link/templates/djangocms_frontend/admin/link.html:12
 msgid "Preview"
-msgstr "Paraparje"
+msgstr "Previsualización"
 
 #: contrib/listgroup/cms_plugins.py:28 contrib/listgroup/models.py:14
 msgid "List group"
-msgstr ""
+msgstr "Grupo de listas"
 
 #: contrib/listgroup/cms_plugins.py:55
 msgid "List item"
-msgstr ""
+msgstr "Elemento de lista"
 
 #: contrib/listgroup/constants.py:4
 msgid "Active"
-msgstr "Aktive"
+msgstr "Activa"
 
 #: contrib/listgroup/constants.py:5
 msgid "Disabled"
-msgstr "E çaktivizuar"
+msgstr "Deshabilitada"
 
 #: contrib/listgroup/forms.py:36
 msgid "List group flush"
-msgstr ""
+msgstr "Grupo de lista sin bordes"
 
 #: contrib/listgroup/forms.py:39
 msgid "Create lists of content in a card with a flush list group."
 msgstr ""
+"Crea listas de contenido en una tarjeta eliminando algunos bordes de los "
+"elementos."
 
 #: contrib/listgroup/forms.py:64
 msgid "One line content"
-msgstr "Lëndë një rresht"
+msgstr "Contenido en una línea"
 
 #: contrib/listgroup/forms.py:67
 msgid "List item text. Is only show if this list item has no child plugins."
 msgstr ""
+"Texto del elemento. Sólo se mostrará si el elemento no tiene ninguna "
+"extensión hija."
 
 #: contrib/listgroup/forms.py:78
 msgid "State"
-msgstr "Gjendje"
+msgstr "Estado"
 
 #: contrib/listgroup/models.py:31
 msgid "List group item"
-msgstr ""
+msgstr "Elemento de grupo de lista"
 
 #: contrib/media/cms_plugins.py:23 contrib/media/models.py:14
 msgid "Media"
-msgstr "Media"
+msgstr "Multimedia"
 
 #: contrib/media/cms_plugins.py:40 contrib/media/models.py:28
 msgid "Media body"
-msgstr "Lëndë media"
+msgstr "Cuerpo de multimedia"
 
 #: contrib/navigation/cms_plugins.py:29 contrib/navigation/models.py:15
 msgid "Navigation"
-msgstr "Lëvizje"
+msgstr "Navegación"
 
 #: contrib/navigation/cms_plugins.py:74 contrib/navigation/models.py:36
 msgid "Page tree"
-msgstr "Pemë faqeje"
+msgstr "Árbol de páginas"
 
 #: contrib/navigation/cms_plugins.py:105 contrib/navigation/forms.py:104
 #: contrib/navigation/models.py:42
 msgid "Brand"
-msgstr "Markë"
+msgstr "Marca"
 
 #: contrib/navigation/cms_plugins.py:133 contrib/navigation/models.py:24
 msgid "Navigation container"
-msgstr "Kontejner Menuje Lëvizjesh"
+msgstr "Contenedor de navegación"
 
 #: contrib/navigation/cms_plugins.py:164
 msgid "Navigation link"
-msgstr "Lidhje lëvizjeje"
+msgstr "Enlace de navegación"
 
 #: contrib/navigation/forms.py:45
 msgid "Defines the whole template set for this navigation."
-msgstr "Përcakton krejt grupin e gjedheve për këtë menu lëvizjesh."
+msgstr "Define la plantilla para esta navegación."
 
 #: contrib/navigation/forms.py:53
 msgid "Design"
-msgstr ""
+msgstr "Diseño"
 
 #: contrib/navigation/forms.py:60
 msgid "Expand on device (and larger)"
-msgstr "Zgjeroje në pajisje (dhe më të mëdha)"
+msgstr "Expande en dispositivo (y superiores)"
 
 #: contrib/navigation/forms.py:81
 msgid "Start level"
-msgstr "Nivel fillimi"
+msgstr "Nivel inicial"
 
 #: contrib/navigation/forms.py:84
 msgid "Start level of this page tree (0: root, 1: level below root, etc.)"
 msgstr ""
-"Nivel fillimi për këtë pemë faqesh (0: rrënjë, 1: niveli nën rrënjë, etj.)"
+"Nivel inicial de este árbol de páginas (0: raíz, 1: nivel bajo la raíz, "
+"etc.)"
 
 #: contrib/navigation/forms.py:106
 msgid "Enter brand name or add child plugins for brand icon or image"
 msgstr ""
-"Jepni emër marke, ose shtoni shtojca pjellë për ikonë ose figurë marke"
+"Introduce el nombre de la marca o añade extensiones hijas para mostrar el "
+"icono o imagen de la marca"
 
 #: contrib/navigation/models.py:30
 msgid "Navigation Link"
-msgstr "Lidhje Lëvizjeje"
+msgstr "Enlace de navegación"
 
 #: contrib/tabs/cms_plugins.py:24 contrib/tabs/constants.py:5
 msgid "Tabs"
-msgstr "Skeda"
+msgstr "Pestañas"
 
 #: contrib/tabs/cms_plugins.py:58 contrib/tabs/models.py:27
 msgid "Tab item"
-msgstr "Element skede"
+msgstr "Pestaña"
 
 #: contrib/tabs/constants.py:6
 msgid "Pills"
-msgstr "Sumbulla"
+msgstr "Pastillas"
 
 #: contrib/tabs/constants.py:10
 msgid "Fill"
-msgstr "Mbushje"
+msgstr "Rellena"
 
 #: contrib/tabs/constants.py:11
 msgid "Justified"
-msgstr "Përligjur"
+msgstr "Justificado"
 
 #: contrib/tabs/constants.py:12
 msgid "Justify start"
-msgstr ""
+msgstr "Justificado al principio"
 
 #: contrib/tabs/constants.py:13
 msgid "Justify center"
-msgstr ""
+msgstr "Centrado"
 
 #: contrib/tabs/constants.py:14
 msgid "Justify end"
-msgstr ""
+msgstr "Justificado al final"
 
 #: contrib/tabs/forms.py:64
 msgid "Index"
-msgstr "Tregues"
+msgstr "Índice"
 
 #: contrib/tabs/forms.py:67
 msgid "Index of element to open on page load starting at 1."
-msgstr ""
-"Tregues elementësh për t’u hapur në ngarkim faqeje, duke filluar me 1."
+msgstr "Índice del elemento a abrir al cargar la página comenzando por 1."
 
 #: contrib/tabs/forms.py:70
 msgid "Animation effect"
-msgstr "Efekt animacioni"
+msgstr "Efecto de la animación"
 
 #: contrib/tabs/forms.py:96
 msgid "Tab title"
-msgstr "Titull skede"
+msgstr "Título de la pestaña"
 
 #: contrib/tabs/forms.py:99
 msgid "Bordered"
-msgstr "Me anë"
+msgstr "Con borde"
 
 #: contrib/tabs/forms.py:101
 msgid "Add borders to the tab item"
-msgstr "Shto anë te objekti skedë"
+msgstr "Añade bordes a la pestaña"
 
 #: contrib/tabs/models.py:9
 msgid "Tab"
-msgstr "Skedë"
+msgstr "Pestaña"
 
 #: contrib/utilities/cms_plugins.py:49
 msgid "Editor note"
-msgstr "Shënim i redaktorit"
+msgstr "Nota del editor"
 
 #: contrib/utilities/cms_plugins.py:61 contrib/utilities/forms.py:120
 #: contrib/utilities/models.py:44
 msgid "Heading"
-msgstr "Krye"
+msgstr "Encabezado"
 
 #: contrib/utilities/cms_plugins.py:122 contrib/utilities/models.py:59
 msgid "Table of contents"
-msgstr "Tryezë e lëndës"
+msgstr "Tabla de contenidos"
 
 #: contrib/utilities/forms.py:37
 msgid "Property"
-msgstr "Veti"
+msgstr "Propiedad"
 
 #: contrib/utilities/forms.py:43
 msgid "Sides"
-msgstr "Anë"
+msgstr "Lados"
 
 #: contrib/utilities/forms.py:50
 msgid "Size"
-msgstr "Madhësi"
+msgstr "Tamaño"
 
 #: contrib/utilities/forms.py:56
 msgid "Device"
-msgstr "Pajisje"
+msgstr "Dispositivo"
 
 #: contrib/utilities/forms.py:74
 msgid ""
 "Padding does not have an auto spacing. Either switch to margin or a defined "
 "size."
 msgstr ""
-"Mbushja s’ka aplikim vetvetiu hapësire. Ose kaloni te mënjanë, ose te një "
-"madhësi e përcaktuar."
+"Padding no tiene un auto-espaciado. Cambia a margen o bien define un tamaño "
+"de padding."
 
 #: contrib/utilities/forms.py:78
 msgid ""
 "Padding does not have an auto spacing. Either switch to a defined size or "
 "change the spacing property."
 msgstr ""
-"Mbushja s’ka aplikim vetvetiu hapësire. Ose kaloni te një madhësi e "
-"përcaktuar, ose ndryshoni vetinë për hapësira."
+"Padding no tiene un auto-espaciado. Define un tamaño de padding o bien "
+"cambia la propiedad de espaciado."
 
 #: contrib/utilities/forms.py:101 settings.py:38
 msgid "Heading 1"
-msgstr "Krye 1"
+msgstr "Encabezado 1"
 
 #: contrib/utilities/forms.py:102 settings.py:39
 msgid "Heading 2"
-msgstr "Krye 2"
+msgstr "Encabezado 2"
 
 #: contrib/utilities/forms.py:103 settings.py:40
 msgid "Heading 3"
-msgstr "Krye 3"
+msgstr "Encabezado 3"
 
 #: contrib/utilities/forms.py:104 settings.py:41
 msgid "Heading 4"
-msgstr "Krye 4"
+msgstr "Encabezado 4"
 
 #: contrib/utilities/forms.py:105 settings.py:42
 msgid "Heading 5"
-msgstr "Krye 5"
+msgstr "Encabezado 5"
 
 #: contrib/utilities/forms.py:114
 msgid "Heading level"
-msgstr "Shkallë kryesh"
+msgstr "Nivel de encabezado"
 
 #: contrib/utilities/forms.py:125
 msgid "ID"
-msgstr "ID"
+msgstr "Identificador"
 
 #: contrib/utilities/forms.py:128
 msgid ""
 "Fill in unique ID for table of contents. If empty heading will not appear in"
 " table of contents."
 msgstr ""
-"Plotësoni ID unike për tryezë lënde. Në u lëntë e zbrazët, kryet s’do të "
-"duken te tryezë e lëndës."
+"Asigna un identificador único para la tabla de contenidos. En caso de no "
+"rellenar, este encabezado no aparecerá en la tabla de contenidos."
 
 #: contrib/utilities/forms.py:132
 msgid "Heading context"
-msgstr "Kontekst kryesh"
+msgstr "Contexto del encabezado"
 
 #: contrib/utilities/forms.py:160
 msgid "List attributes"
-msgstr "Atribute liste"
+msgstr "Lista de atributos"
 
 #: contrib/utilities/forms.py:162
 msgid ""
 "Attributes apply to the <b>list</b> for each level in the table of contents."
-msgstr "Atribute aplikohen te <b>lista</b> për çdo nivel te tryeza e lëndës."
+msgstr ""
+"Los atributos se aplican al <b>listado</b> por cada nivel en la tabla de "
+"contenidos."
 
 #: contrib/utilities/forms.py:169
 msgid ""
 "Attributes apply to the <b>link</b> for each entry in the table of contents."
-msgstr "Atribute aplikohen te <b>lidhja</b> për çdo nivel te tryeza e lëndës."
+msgstr ""
+"Los atributos se aplican al <b>enlace</b> por cada entrada de la tabla de "
+"contenidos."
 
 #: contrib/utilities/forms.py:173
 msgid "Item attributes"
-msgstr "Atribute objekti"
+msgstr "Atributos del elemento"
 
 #: contrib/utilities/forms.py:175
 msgid ""
 "Attributes apply to the <b>list items</b> for each entry in the table of "
 "contents."
 msgstr ""
-"Atribute aplikohen te <b>zëra liste</b> për çdo zë te tryeza e lëndës."
+"Los atributos se aplican a los <b>elementos de listado</b> por cada entrada "
+"de la tabla de contenidos."
 
 #: fields.py:94
 msgid "Please select at least one device size"
-msgstr "Ju lutemi, përzgjidhni të paktën një madhësi pajisjeje"
+msgstr "Selecciona como mínimo un tamaño de dispositivo"
 
 #: fields.py:102 fields.py:110
 msgid "Attributes"
-msgstr "Atribute"
+msgstr "Atributos"
 
 #: fields.py:131
 msgid "Choices"
-msgstr "Zgjedhje"
+msgstr "Opciones"
 
 #: fields.py:142
 msgid ""
 "Please enter at least one choice. Use the <code>+</code> symbol to add a "
 "choice."
 msgstr ""
-"Ju lutemi, jepni të paktën një zgjedhje. Që të shtoni një zgjedhje, përdorni"
-" simbolin <code>+</code>."
+"Selecciona como mínimo una opción. Utiliza el símbolo <code>+</code> para "
+"añadir una opción."
 
 #: fields.py:161 fields.py:175
 msgid "Tag type"
-msgstr "Lloj etikete"
+msgstr "Etiqueta HTML"
 
 #: fields.py:169
 msgid "Select the HTML tag to be used."
-msgstr "Përzgjidhni etiketë HTML për t’u përdorur."
+msgstr "Selecciona la etiqueta HTML que se utilizará."
 
 #: frameworks/bootstrap5.py:6 frameworks/bootstrap5.py:132
 msgid "Extra small"
-msgstr ""
+msgstr "Extra pequeña"
 
 #: frameworks/bootstrap5.py:10 frameworks/bootstrap5.py:136
 msgid "Extra large"
-msgstr ""
+msgstr "Extra grande"
 
 #: frameworks/bootstrap5.py:11
 msgid "Extra-extra large"
-msgstr ""
+msgstr "Extra-extra grande"
 
 #: frameworks/bootstrap5.py:19
 msgid "Primary"
-msgstr "Parësore"
+msgstr "Primario"
 
 #: frameworks/bootstrap5.py:20
 msgid "Secondary"
-msgstr "Sekondare"
+msgstr "Secundario"
 
 #: frameworks/bootstrap5.py:21
 msgid "Success"
-msgstr "Sukses"
+msgstr "Éxito"
 
 #: frameworks/bootstrap5.py:22
 msgid "Danger"
-msgstr "Rrezik"
+msgstr "Peligro"
 
 #: frameworks/bootstrap5.py:23
 msgid "Warning"
-msgstr "Kujdes"
+msgstr "Aviso"
 
 #: frameworks/bootstrap5.py:24
 msgid "Info"
-msgstr "Hollësi"
+msgstr "Información"
 
 #: frameworks/bootstrap5.py:25 frameworks/bootstrap5.py:178
 msgid "Light"
-msgstr "E çelët"
+msgstr "Claro"
 
 #: frameworks/bootstrap5.py:26 frameworks/bootstrap5.py:179
 msgid "Dark"
-msgstr "E errët"
+msgstr "Oscuro"
 
 #: frameworks/bootstrap5.py:58 frameworks/bootstrap5.py:64
 msgid "Both"
-msgstr "Që të dyja"
+msgstr "Ambos"
 
 #: frameworks/bootstrap5.py:65
 msgid "Top"
-msgstr "Në krye"
+msgstr "Arriba"
 
 #: frameworks/bootstrap5.py:66
 msgid "Bottom"
-msgstr "Në fund"
+msgstr "Abajo"
 
 #: frameworks/bootstrap5.py:91
 msgid "Screen"
-msgstr "Ekran"
+msgstr "Pantalla"
 
 #: frameworks/bootstrap5.py:104
 msgid "Screen (minimum)"
-msgstr "Ekran (minimum)"
+msgstr "Pantalla (mínimo)"
 
 #: frameworks/bootstrap5.py:124
 msgctxt "shadow"
 msgid "None"
-msgstr "Asnjë"
+msgstr "Ninguno"
 
 #: frameworks/bootstrap5.py:137
 msgid "XX large"
-msgstr ""
+msgstr "XX grande"
 
 #: helpers.py:112
 #, python-brace-format
 msgid "Read more in the <a href=\"{link}\" target=\"_blank\">documentation</a>."
-msgstr "Lexoni më tepër, te <a href=\"{link}\" target=\"_blank\">dokumentimi</a>."
+msgstr "Leer más en la <a href=\"{link}\" target=\"_blank\">documentación</a>."
 
 #: models.py:24
 msgid "UI item"
-msgstr "Element UI"
+msgstr "Elemento UI"
 
 #: settings.py:14
 msgid "There are no further settings for this plugin. Please press save."
-msgstr ""
-"S’ka rregullime të tjera për këtë shtojcë. Ju lutemi, shtypni “Ruaje”."
+msgstr "No hay más opciones para esta extensión. Haz clic en guardar."
 
 #: settings.py:73
 msgid "Offcanvas"
 msgstr ""
```

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/management/bootstrap4_migration.py` & `djangocms-frontend-1.1.7/djangocms_frontend/management/bootstrap4_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/management/commands/frontend.py` & `djangocms-frontend-1.1.7/djangocms_frontend/management/commands/frontend.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/base.py` & `djangocms-frontend-1.1.7/djangocms_frontend/management/commands/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/frequency_analysis.py` & `djangocms-frontend-1.1.7/djangocms_frontend/management/commands/subcommands/frequency_analysis.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/migrate.py` & `djangocms-frontend-1.1.7/djangocms_frontend/management/commands/subcommands/migrate.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/stale_references.py` & `djangocms-frontend-1.1.7/djangocms_frontend/management/commands/subcommands/stale_references.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/management/commands/subcommands/sync_permissions.py` & `djangocms-frontend-1.1.7/djangocms_frontend/management/commands/subcommands/sync_permissions.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/management/icon_migration.py` & `djangocms-frontend-1.1.7/djangocms_frontend/management/icon_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/management/styled_link_migration.py` & `djangocms-frontend-1.1.7/djangocms_frontend/management/styled_link_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/migrations/0001_initial.py` & `djangocms-frontend-1.1.7/djangocms_frontend/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/models.py` & `djangocms-frontend-1.1.7/djangocms_frontend/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/settings.py` & `djangocms-frontend-1.1.7/djangocms_frontend/settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/base.css` & `djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/css/base.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/base.css.map` & `djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/css/base.css.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/button_group.css` & `djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/css/button_group.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map` & `djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/css/select2.css` & `djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/css/select2.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/auto_input.js` & `djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/js/auto_input.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js` & `djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js` & `djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js` & `djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/static/djangocms_frontend/js/django_select2.js` & `djangocms-frontend-1.1.7/djangocms_frontend/static/djangocms_frontend/js/django_select2.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/templates/bootstrap5/base.html` & `djangocms-frontend-1.1.7/djangocms_frontend/templates/bootstrap5/base.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/templates/bootstrap5/menu.html` & `djangocms-frontend-1.1.7/djangocms_frontend/templates/bootstrap5/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html` & `djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html` & `djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html` & `djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html` & `djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html` & `djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html` & `djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/templates/djangocms_frontend.html` & `djangocms-frontend-1.1.7/djangocms_frontend/templates/djangocms_frontend.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend/templatetags/frontend.py` & `djangocms-frontend-1.1.7/djangocms_frontend/templatetags/frontend.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend.egg-info/PKG-INFO` & `djangocms-frontend-1.1.7/djangocms_frontend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-frontend
-Version: 1.1.6
+Version: 1.1.7
 Summary: Adds abstract User Interface items as plugins to django CMS.
 Home-page: https://github.com/django-cms/djangocms-frontend
 Author: fsbraun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-frontend-1.1.6/djangocms_frontend.egg-info/SOURCES.txt` & `djangocms-frontend-1.1.7/djangocms_frontend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/pyproject.toml` & `djangocms-frontend-1.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/setup.py` & `djangocms-frontend-1.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/accordion/test_models.py` & `djangocms-frontend-1.1.7/tests/accordion/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/accordion/test_plugins.py` & `djangocms-frontend-1.1.7/tests/accordion/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/alert/test_plugins.py` & `djangocms-frontend-1.1.7/tests/alert/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/badge/test_plugins.py` & `djangocms-frontend-1.1.7/tests/badge/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/card/test_models.py` & `djangocms-frontend-1.1.7/tests/card/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/card/test_plugins.py` & `djangocms-frontend-1.1.7/tests/card/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/carousel/test_models.py` & `djangocms-frontend-1.1.7/tests/carousel/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/carousel/test_plugins.py` & `djangocms-frontend-1.1.7/tests/carousel/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/collapse/test_models.py` & `djangocms-frontend-1.1.7/tests/collapse/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/collapse/test_plugins.py` & `djangocms-frontend-1.1.7/tests/collapse/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/content/test_models.py` & `djangocms-frontend-1.1.7/tests/content/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/content/test_plugins.py` & `djangocms-frontend-1.1.7/tests/content/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/fixtures.py` & `djangocms-frontend-1.1.7/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/grid/test_models.py` & `djangocms-frontend-1.1.7/tests/grid/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/grid/test_plugins.py` & `djangocms-frontend-1.1.7/tests/grid/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/helpers.py` & `djangocms-frontend-1.1.7/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/icon/test_models.py` & `djangocms-frontend-1.1.7/tests/icon/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/icon/test_plugins.py` & `djangocms-frontend-1.1.7/tests/icon/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/image/test_plugins.py` & `djangocms-frontend-1.1.7/tests/image/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/jumbotron/test_plugins.py` & `djangocms-frontend-1.1.7/tests/jumbotron/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/link/test_plugins.py` & `djangocms-frontend-1.1.7/tests/link/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/link/test_urlconf.py` & `djangocms-frontend-1.1.7/tests/link/test_urlconf.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/listgroup/test_models.py` & `djangocms-frontend-1.1.7/tests/listgroup/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/listgroup/test_plugins.py` & `djangocms-frontend-1.1.7/tests/listgroup/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/media/test_models.py` & `djangocms-frontend-1.1.7/tests/media/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/media/test_plugins.py` & `djangocms-frontend-1.1.7/tests/media/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/navigation/test_models.py` & `djangocms-frontend-1.1.7/tests/navigation/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/navigation/test_plugins.py` & `djangocms-frontend-1.1.7/tests/navigation/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/tabs/test_models.py` & `djangocms-frontend-1.1.7/tests/tabs/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/tabs/test_plugins.py` & `djangocms-frontend-1.1.7/tests/tabs/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/test_constants.py` & `djangocms-frontend-1.1.7/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/test_fields.py` & `djangocms-frontend-1.1.7/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/test_helpers.py` & `djangocms-frontend-1.1.7/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/test_migrations.py` & `djangocms-frontend-1.1.7/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/test_settings.py` & `djangocms-frontend-1.1.7/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/utilities/test_models.py` & `djangocms-frontend-1.1.7/tests/utilities/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.6/tests/utilities/test_plugins.py` & `djangocms-frontend-1.1.7/tests/utilities/test_plugins.py`

 * *Files identical despite different names*

