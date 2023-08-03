# Comparing `tmp/ims.zip-4.2.1.tar.gz` & `tmp/ims.zip-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ims.zip-4.2.1.tar", last modified: Wed Apr 21 20:51:20 2021, max compression
+gzip compressed data, was "ims.zip-5.0.tar", last modified: Thu Aug  3 20:40:08 2023, max compression
```

## Comparing `ims.zip-4.2.1.tar` & `ims.zip-5.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:20.721987 ims.zip-4.2.1/
--rw-rw----   0 zadmin     (700) wheel       (10)       43 2019-09-12 18:30:06.000000 ims.zip-4.2.1/MANIFEST.in
--rw-rw----   0 zadmin     (700) wheel       (10)      481 2021-04-21 20:51:20.724984 ims.zip-4.2.1/PKG-INFO
--rw-rw----   0 zadmin     (700) wheel       (10)     1304 2021-04-20 19:38:25.000000 ims.zip-4.2.1/README.md
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:15.499761 ims.zip-4.2.1/ims/
--rw-rw----   0 zadmin     (700) wheel       (10)      244 2019-09-12 18:30:06.000000 ims.zip-4.2.1/ims/__init__.py
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:18.294716 ims.zip-4.2.1/ims/zip/
--rw-rw----   0 zadmin     (700) wheel       (10)       77 2021-01-14 17:15:05.000000 ims.zip-4.2.1/ims/zip/__init__.py
--rw-rw----   0 zadmin     (700) wheel       (10)     1529 2020-01-08 15:50:05.000000 ims.zip-4.2.1/ims/zip/adapters.py
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:18.656024 ims.zip-4.2.1/ims/zip/browser/
--rw-rw----   0 zadmin     (700) wheel       (10)        2 2021-01-14 17:15:05.000000 ims.zip-4.2.1/ims/zip/browser/__init__.py
--rw-rw----   0 zadmin     (700) wheel       (10)      780 2019-09-12 18:30:06.000000 ims.zip-4.2.1/ims/zip/browser/configure.zcml
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:18.949015 ims.zip-4.2.1/ims/zip/browser/templates/
--rw-rw----   0 zadmin     (700) wheel       (10)      363 2019-09-12 18:30:06.000000 ims.zip-4.2.1/ims/zip/browser/templates/unzipper.pt
--rw-rw----   0 zadmin     (700) wheel       (10)     2444 2021-04-20 19:38:25.000000 ims.zip-4.2.1/ims/zip/browser/templates/zipper.pt
--rw-rw----   0 zadmin     (700) wheel       (10)     3323 2021-04-20 19:38:25.000000 ims.zip-4.2.1/ims/zip/browser/unzipper.py
--rw-rw----   0 zadmin     (700) wheel       (10)     4105 2021-04-21 20:08:43.000000 ims.zip-4.2.1/ims/zip/browser/zipper.py
--rw-rw----   0 zadmin     (700) wheel       (10)     2164 2020-03-02 18:13:00.000000 ims.zip-4.2.1/ims/zip/configure.zcml
--rw-rw----   0 zadmin     (700) wheel       (10)      943 2020-01-08 15:50:05.000000 ims.zip-4.2.1/ims/zip/interfaces.py
--rw-rw----   0 zadmin     (700) wheel       (10)      198 2019-09-12 18:30:06.000000 ims.zip-4.2.1/ims/zip/permissions.py
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:14.893711 ims.zip-4.2.1/ims/zip/profiles/
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:19.130014 ims.zip-4.2.1/ims/zip/profiles/default/
--rw-rw----   0 zadmin     (700) wheel       (10)     2119 2019-09-12 18:30:06.000000 ims.zip-4.2.1/ims/zip/profiles/default/actions.xml
--rw-rw----   0 zadmin     (700) wheel       (10)      260 2019-09-12 18:30:06.000000 ims.zip-4.2.1/ims/zip/profiles/default/registry.xml
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:19.300007 ims.zip-4.2.1/ims/zip/profiles/uninstall/
--rw-rw----   0 zadmin     (700) wheel       (10)      262 2020-03-02 18:13:00.000000 ims.zip-4.2.1/ims/zip/profiles/uninstall/actions.xml
--rw-rw----   0 zadmin     (700) wheel       (10)       95 2020-03-02 18:13:00.000000 ims.zip-4.2.1/ims/zip/profiles/uninstall/registry.xml
--rw-rw----   0 zadmin     (700) wheel       (10)      695 2020-01-08 15:50:05.000000 ims.zip-4.2.1/ims/zip/testing.py
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:20.068996 ims.zip-4.2.1/ims/zip/tests/
--rw-rw----   0 zadmin     (700) wheel       (10)        2 2021-01-14 17:15:05.000000 ims.zip-4.2.1/ims/zip/tests/__init__.py
--rw-rw----   0 zadmin     (700) wheel       (10)     1304 2021-01-14 17:15:05.000000 ims.zip-4.2.1/ims/zip/tests/base.py
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:20.472997 ims.zip-4.2.1/ims/zip/tests/input/
--rw-rw----   0 zadmin     (700) wheel       (10)     3516 2019-09-12 18:30:06.000000 ims.zip-4.2.1/ims/zip/tests/input/canoneye.jpg
--rw-rw----   0 zadmin     (700) wheel       (10)        7 2019-09-12 18:30:06.000000 ims.zip-4.2.1/ims/zip/tests/input/file.txt
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:20.613985 ims.zip-4.2.1/ims/zip/tests/input/folder1/
--rw-rw----   0 zadmin     (700) wheel       (10)     3516 2019-09-12 18:30:06.000000 ims.zip-4.2.1/ims/zip/tests/input/folder1/canoneye.jpg
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:20.642984 ims.zip-4.2.1/ims/zip/tests/input/folder2/
--rw-rw----   0 zadmin     (700) wheel       (10)        7 2019-09-12 18:30:06.000000 ims.zip-4.2.1/ims/zip/tests/input/folder2/file.txt
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:20.672986 ims.zip-4.2.1/ims/zip/tests/input/folder2/folder3/
--rw-rw----   0 zadmin     (700) wheel       (10)       90 2019-09-12 18:30:06.000000 ims.zip-4.2.1/ims/zip/tests/input/folder2/folder3/page1.html
--rw-rw----   0 zadmin     (700) wheel       (10)       90 2019-09-12 18:30:06.000000 ims.zip-4.2.1/ims/zip/tests/input/page1.html
--rw-rw----   0 zadmin     (700) wheel       (10)     2589 2019-09-12 18:30:06.000000 ims.zip-4.2.1/ims/zip/tests/input/test.zip
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:20.692006 ims.zip-4.2.1/ims/zip/tests/output/
--rw-rw----   0 zadmin     (700) wheel       (10)     2481 2019-09-12 18:30:06.000000 ims.zip-4.2.1/ims/zip/tests/output/test.zip
--rw-rw----   0 zadmin     (700) wheel       (10)      786 2020-03-02 18:13:00.000000 ims.zip-4.2.1/ims/zip/tests/test_uninstall.py
--rw-rw----   0 zadmin     (700) wheel       (10)     4545 2020-01-08 15:50:05.000000 ims.zip-4.2.1/ims/zip/tests/test_zip.py
--rw-rw----   0 zadmin     (700) wheel       (10)     1144 2021-04-20 19:38:25.000000 ims.zip-4.2.1/ims/zip/zipper.py
-drwxrws---   0 zadmin     (700) wheel       (10)        0 2021-04-21 20:51:16.738742 ims.zip-4.2.1/ims.zip.egg-info/
--rw-rw----   0 zadmin     (700) wheel       (10)      481 2021-04-21 20:51:08.000000 ims.zip-4.2.1/ims.zip.egg-info/PKG-INFO
--rw-rw----   0 zadmin     (700) wheel       (10)     1183 2021-04-21 20:51:11.000000 ims.zip-4.2.1/ims.zip.egg-info/SOURCES.txt
--rw-rw----   0 zadmin     (700) wheel       (10)        1 2021-04-21 20:51:09.000000 ims.zip-4.2.1/ims.zip.egg-info/dependency_links.txt
--rw-rw----   0 zadmin     (700) wheel       (10)       90 2021-04-21 20:51:09.000000 ims.zip-4.2.1/ims.zip.egg-info/entry_points.txt
--rw-rw----   0 zadmin     (700) wheel       (10)        4 2021-04-21 20:51:09.000000 ims.zip-4.2.1/ims.zip.egg-info/namespace_packages.txt
--rw-rw----   0 zadmin     (700) wheel       (10)        1 2019-09-12 18:30:44.000000 ims.zip-4.2.1/ims.zip.egg-info/not-zip-safe
--rw-rw----   0 zadmin     (700) wheel       (10)       67 2021-04-21 20:51:09.000000 ims.zip-4.2.1/ims.zip.egg-info/requires.txt
--rw-rw----   0 zadmin     (700) wheel       (10)        4 2021-04-21 20:51:09.000000 ims.zip-4.2.1/ims.zip.egg-info/top_level.txt
--rw-rw----   0 zadmin     (700) wheel       (10)       70 2021-04-21 20:51:20.737984 ims.zip-4.2.1/setup.cfg
--rw-rw----   0 zadmin     (700) wheel       (10)     1002 2021-04-21 20:12:30.000000 ims.zip-4.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.136279 ims.zip-5.0/
+-rw-rw-rw-   0        0        0       44 2023-03-15 21:53:02.000000 ims.zip-5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      331 2023-08-03 20:40:08.136279 ims.zip-5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       65 2023-08-03 20:29:36.000000 ims.zip-5.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.027767 ims.zip-5.0/ims/
+-rw-rw-rw-   0        0        0      250 2023-03-16 19:29:33.000000 ims.zip-5.0/ims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.065179 ims.zip-5.0/ims/zip/
+-rw-rw-rw-   0        0        0       80 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/__init__.py
+-rw-rw-rw-   0        0        0     1529 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/adapters.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.076193 ims.zip-5.0/ims/zip/browser/
+-rw-rw-rw-   0        0        0        3 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/browser/__init__.py
+-rw-rw-rw-   0        0        0      780 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/browser/configure.zcml
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.083243 ims.zip-5.0/ims/zip/browser/templates/
+-rw-rw-rw-   0        0        0      378 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/browser/templates/unzipper.pt
+-rw-rw-rw-   0        0        0     1667 2023-08-03 20:20:45.000000 ims.zip-5.0/ims/zip/browser/templates/zipper.pt
+-rw-rw-rw-   0        0        0     3338 2023-08-03 20:18:43.000000 ims.zip-5.0/ims/zip/browser/unzipper.py
+-rw-rw-rw-   0        0        0     4110 2023-08-03 20:18:43.000000 ims.zip-5.0/ims/zip/browser/zipper.py
+-rw-rw-rw-   0        0        0     2728 2023-08-03 20:30:12.000000 ims.zip-5.0/ims/zip/configure.zcml
+-rw-rw-rw-   0        0        0      942 2023-08-03 20:18:43.000000 ims.zip-5.0/ims/zip/interfaces.py
+-rw-rw-rw-   0        0        0      198 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/permissions.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.011542 ims.zip-5.0/ims/zip/profiles/
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.091249 ims.zip-5.0/ims/zip/profiles/default/
+-rw-rw-rw-   0        0        0     2170 2023-08-03 20:18:43.000000 ims.zip-5.0/ims/zip/profiles/default/actions.xml
+-rw-rw-rw-   0        0        0       74 2023-08-03 20:22:07.000000 ims.zip-5.0/ims/zip/profiles/default/metadata.xml
+-rw-rw-rw-   0        0        0      265 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/profiles/default/registry.xml
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.097263 ims.zip-5.0/ims/zip/profiles/uninstall/
+-rw-rw-rw-   0        0        0      268 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/profiles/uninstall/actions.xml
+-rw-rw-rw-   0        0        0       97 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/profiles/uninstall/registry.xml
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.099256 ims.zip-5.0/ims/zip/profiles/upgrade_1/
+-rw-rw-rw-   0        0        0      579 2023-08-03 20:26:31.000000 ims.zip-5.0/ims/zip/profiles/upgrade_1/actions.xml
+-rw-rw-rw-   0        0        0      721 2023-08-03 20:18:43.000000 ims.zip-5.0/ims/zip/testing.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.111272 ims.zip-5.0/ims/zip/tests/
+-rw-rw-rw-   0        0        0        3 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/tests/__init__.py
+-rw-rw-rw-   0        0        0     1304 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/tests/base.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.122292 ims.zip-5.0/ims/zip/tests/input/
+-rw-rw-rw-   0        0        0     3516 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/tests/input/canoneye.jpg
+-rw-rw-rw-   0        0        0        7 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/tests/input/file.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.125309 ims.zip-5.0/ims/zip/tests/input/folder1/
+-rw-rw-rw-   0        0        0     3516 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/tests/input/folder1/canoneye.jpg
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.128302 ims.zip-5.0/ims/zip/tests/input/folder2/
+-rw-rw-rw-   0        0        0        7 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/tests/input/folder2/file.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.131293 ims.zip-5.0/ims/zip/tests/input/folder2/folder3/
+-rw-rw-rw-   0        0        0       90 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/tests/input/folder2/folder3/page1.html
+-rw-rw-rw-   0        0        0       90 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/tests/input/page1.html
+-rw-rw-rw-   0        0        0     2589 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/tests/input/test.zip
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.133288 ims.zip-5.0/ims/zip/tests/output/
+-rw-rw-rw-   0        0        0     2481 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/tests/output/test.zip
+-rw-rw-rw-   0        0        0      809 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/tests/test_uninstall.py
+-rw-rw-rw-   0        0        0     4667 2023-03-15 21:53:02.000000 ims.zip-5.0/ims/zip/tests/test_zip.py
+-rw-rw-rw-   0        0        0       86 2023-08-03 20:29:36.000000 ims.zip-5.0/ims/zip/upgrades.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:40:08.045100 ims.zip-5.0/ims.zip.egg-info/
+-rw-rw-rw-   0        0        0      331 2023-08-03 20:40:07.000000 ims.zip-5.0/ims.zip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1199 2023-08-03 20:40:07.000000 ims.zip-5.0/ims.zip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 20:40:07.000000 ims.zip-5.0/ims.zip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 20:40:07.000000 ims.zip-5.0/ims.zip.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       67 2023-08-03 20:40:07.000000 ims.zip-5.0/ims.zip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-03 20:40:07.000000 ims.zip-5.0/ims.zip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1014 2023-08-03 20:39:38.000000 ims.zip-5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       77 2023-08-03 20:40:08.139271 ims.zip-5.0/setup.cfg
```

### Comparing `ims.zip-4.2.1/ims/zip/adapters.py` & `ims.zip-5.0/ims/zip/adapters.py`

 * *Files identical despite different names*

### Comparing `ims.zip-4.2.1/ims/zip/browser/configure.zcml` & `ims.zip-5.0/ims/zip/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `ims.zip-4.2.1/ims/zip/browser/unzipper.py` & `ims.zip-5.0/ims/zip/browser/unzipper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import mimetypes
 import os
 import zipfile
 from io import BytesIO
-from zope.lifecycleevent import modified
 
 import plone.api
 from Products.CMFPlone import utils
 from plone.app.textfield import RichText
 from plone.app.textfield.value import RichTextValue
 from plone.autoform.form import AutoExtensibleForm
 from plone.i18n.normalizer.interfaces import IFileNameNormalizer
@@ -50,34 +49,37 @@
             if file_name:
                 stream = zipper.read(name)
                 curr = self.context
                 for folder in [f for f in path.split('/') if f]:
                     try:
                         curr = curr[folder]
                     except KeyError:
-                        curr = plone.api.content.create(type='Folder', container=curr, id=folder, title=folder)
+                        curr.invokeFactory('Folder', folder)
+                        curr = curr[folder]
+                        curr.setTitle(folder)
+                        curr.reindexObject()
 
                 content_type = mimetypes.guess_type(file_name)[0] or ""
                 self.factory(file_name, content_type, stream, curr, force_files)
 
                 plone.api.portal.show_message(_('Zip file imported'), self.request, type="info")
         self.request.response.redirect(self.context.absolute_url())
 
     def factory(self, name, content_type, data, container, force_files):
         ctr = plone.api.portal.get_tool('content_type_registry')
-        portal_type = ctr.findTypeName(name.lower(), content_type, '')
-        if force_files and portal_type not in ('File', 'Image'):
-            portal_type = 'File'
-        elif not portal_type:
-            portal_type = 'File'
+        type_ = ctr.findTypeName(name.lower(), content_type, '')
+        if force_files and type_ not in ('File', 'Image'):
+            type_ = 'File'
+        elif not type_:
+            type_ = 'File'
 
         normalizer = getUtility(IFileNameNormalizer)
         chooser = INameChooser(self.context)
         newid = chooser.chooseName(normalizer.normalize(name), self.context.aq_parent)
 
-        obj = plone.api.content.create(container=container, type=portal_type, id=newid, title=name)
+        obj = plone.api.content.create(container=container, type=type_, id=newid, title=name)
         primary_field = IPrimaryFieldInfo(obj)
         if isinstance(primary_field.field, RichText):
             setattr(obj, primary_field.fieldname, RichTextValue(data))
         else:
             setattr(obj, primary_field.fieldname, primary_field.field._type(data, filename=utils.safe_unicode(name)))
-        modified(obj)
+        obj.reindexObject()
```

### Comparing `ims.zip-4.2.1/ims/zip/browser/zipper.py` & `ims.zip-5.0/ims/zip/browser/zipper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,257 +1,257 @@
-00000000: 696d 706f 7274 207a 6970 6669 6c65 0d0a  import zipfile..
-00000010: 6672 6f6d 2065 6d61 696c 2e6d 696d 652e  from email.mime.
-00000020: 7465 7874 2069 6d70 6f72 7420 4d49 4d45  text import MIME
-00000030: 5465 7874 0d0a 0d0a 696d 706f 7274 2070  Text....import p
-00000040: 6c6f 6e65 2e61 7069 0d0a 6672 6f6d 2050  lone.api..from P
-00000050: 726f 6475 6374 732e 4669 7665 2e62 726f  roducts.Five.bro
-00000060: 7773 6572 2069 6d70 6f72 7420 4272 6f77  wser import Brow
-00000070: 7365 7256 6965 770d 0a66 726f 6d20 706c  serView..from pl
-00000080: 6f6e 652e 6e61 6d65 6466 696c 652e 6669  one.namedfile.fi
-00000090: 6c65 2069 6d70 6f72 7420 4e61 6d65 6442  le import NamedB
-000000a0: 6c6f 6246 696c 650d 0a0d 0a66 726f 6d20  lobFile....from 
-000000b0: 2e2e 2069 6d70 6f72 7420 5f0d 0a66 726f  .. import _..fro
-000000c0: 6d20 2e2e 696e 7465 7266 6163 6573 2069  m ..interfaces i
-000000d0: 6d70 6f72 7420 495a 6970 7061 626c 650d  mport IZippable.
-000000e0: 0a66 726f 6d20 2e2e 7a69 7070 6572 2069  .from ..zipper i
-000000f0: 6d70 6f72 7420 7a69 7066 696c 6573 0d0a  mport zipfiles..
-00000100: 0d0a 0d0a 6465 6620 636f 6e76 6572 745f  ....def convert_
-00000110: 746f 5f62 7974 6573 2873 697a 6529 3a0d  to_bytes(size):.
-00000120: 0a20 2020 206e 756d 2c20 756e 6974 203d  .    num, unit =
-00000130: 2073 697a 652e 7370 6c69 7428 290d 0a20   size.split().. 
-00000140: 2020 2069 6620 756e 6974 2e6c 6f77 6572     if unit.lower
-00000150: 2829 203d 3d20 276b 6227 3a0d 0a20 2020  () == 'kb':..   
-00000160: 2020 2020 2072 6574 7572 6e20 666c 6f61       return floa
-00000170: 7428 6e75 6d29 202a 2031 3032 340d 0a20  t(num) * 1024.. 
-00000180: 2020 2065 6c69 6620 756e 6974 2e6c 6f77     elif unit.low
-00000190: 6572 2829 203d 3d20 276d 6227 3a0d 0a20  er() == 'mb':.. 
-000001a0: 2020 2020 2020 2072 6574 7572 6e20 666c         return fl
-000001b0: 6f61 7428 6e75 6d29 202a 2031 3032 3420  oat(num) * 1024 
-000001c0: 2a20 3130 3234 0d0a 2020 2020 656c 6966  * 1024..    elif
-000001d0: 2075 6e69 742e 6c6f 7765 7228 2920 3d3d   unit.lower() ==
-000001e0: 2027 6762 273a 0d0a 2020 2020 2020 2020   'gb':..        
-000001f0: 7265 7475 726e 2066 6c6f 6174 286e 756d  return float(num
-00000200: 2920 2a20 3130 3234 202a 2031 3032 3420  ) * 1024 * 1024 
-00000210: 2a20 3130 3234 0d0a 2020 2020 656c 7365  * 1024..    else
-00000220: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-00000230: 6e20 666c 6f61 7428 6e75 6d29 0d0a 0d0a  n float(num)....
-00000240: 0d0a 6465 6620 5f67 6574 5f73 697a 6528  ..def _get_size(
-00000250: 7669 6577 293a 0d0a 2020 2020 6361 7420  view):..    cat 
-00000260: 3d20 706c 6f6e 652e 6170 692e 706f 7274  = plone.api.port
-00000270: 616c 2e67 6574 5f74 6f6f 6c28 2770 6f72  al.get_tool('por
-00000280: 7461 6c5f 6361 7461 6c6f 6727 290d 0a0d  tal_catalog')...
-00000290: 0a20 2020 2062 6173 655f 7061 7468 203d  .    base_path =
-000002a0: 2027 2f27 2e6a 6f69 6e28 7669 6577 2e63   '/'.join(view.c
-000002b0: 6f6e 7465 7874 2e67 6574 5068 7973 6963  ontext.getPhysic
-000002c0: 616c 5061 7468 2829 2920 2b20 272f 2720  alPath()) + '/' 
-000002d0: 2023 2074 6865 2070 6174 6820 696e 2074   # the path in t
-000002e0: 6865 205a 4361 7461 6c6f 670d 0a20 2020  he ZCatalog..   
-000002f0: 2070 7479 7065 7320 3d20 6361 742e 756e   ptypes = cat.un
-00000300: 6971 7565 5661 6c75 6573 466f 7228 2770  iqueValuesFor('p
-00000310: 6f72 7461 6c5f 7479 7065 2729 0d0a 0d0a  ortal_type')....
-00000320: 2020 2020 636f 6e74 656e 7420 3d20 6361      content = ca
-00000330: 7428 7061 7468 3d62 6173 655f 7061 7468  t(path=base_path
-00000340: 2c20 6f62 6a65 6374 5f70 726f 7669 6465  , object_provide
-00000350: 733d 495a 6970 7061 626c 652e 5f5f 6964  s=IZippable.__id
-00000360: 656e 7469 6669 6572 5f5f 2c20 706f 7274  entifier__, port
-00000370: 616c 5f74 7970 653d 7074 7970 6573 290d  al_type=ptypes).
-00000380: 0a20 2020 2072 6574 7572 6e20 7375 6d28  .    return sum(
-00000390: 5b62 2e67 6574 4f62 6a53 697a 6520 616e  [b.getObjSize an
-000003a0: 6420 636f 6e76 6572 745f 746f 5f62 7974  d convert_to_byt
-000003b0: 6573 2862 2e67 6574 4f62 6a53 697a 6529  es(b.getObjSize)
-000003c0: 206f 7220 3020 666f 7220 6220 696e 2063   or 0 for b in c
-000003d0: 6f6e 7465 6e74 5d29 0d0a 0d0a 0d0a 6465  ontent])......de
-000003e0: 6620 5f69 735f 736d 616c 6c5f 7a69 7028  f _is_small_zip(
-000003f0: 7669 6577 293a 0d0a 2020 2020 7265 7475  view):..    retu
-00000400: 726e 205f 6765 745f 7369 7a65 2876 6965  rn _get_size(vie
-00000410: 7729 203c 3d20 3420 2a20 3130 3234 2e30  w) <= 4 * 1024.0
-00000420: 202a 2031 3032 342e 3020 2a20 3130 3234   * 1024.0 * 1024
-00000430: 2e30 2020 2320 3420 4742 0d0a 0d0a 0d0a  .0  # 4 GB......
-00000440: 636c 6173 7320 5a69 7050 726f 6d70 7428  class ZipPrompt(
-00000450: 4272 6f77 7365 7256 6965 7729 3a0d 0a20  BrowserView):.. 
-00000460: 2020 2022 2222 2063 6f6e 6669 726d 207a     """ confirm z
-00000470: 6970 2022 2222 0d0a 0d0a 2020 2020 6465  ip """....    de
-00000480: 6620 7465 6368 6e69 6361 6c5f 7375 7070  f technical_supp
-00000490: 6f72 745f 6164 6472 6573 7328 7365 6c66  ort_address(self
-000004a0: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-000004b0: 726e 2070 6c6f 6e65 2e61 7069 2e70 6f72  rn plone.api.por
-000004c0: 7461 6c2e 6765 745f 7265 6769 7374 7279  tal.get_registry
-000004d0: 5f72 6563 6f72 6428 2769 6d73 2e7a 6970  _record('ims.zip
-000004e0: 2e69 6e74 6572 6661 6365 732e 495a 6970  .interfaces.IZip
-000004f0: 5365 7474 696e 6773 2e74 6563 686e 6963  Settings.technic
-00000500: 616c 5f73 7570 706f 7274 5f61 6464 7265  al_support_addre
-00000510: 7373 2729 0d0a 0d0a 2020 2020 6465 6620  ss')....    def 
-00000520: 6765 745f 7369 7a65 2873 656c 6629 3a0d  get_size(self):.
-00000530: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000540: 5f67 6574 5f73 697a 6528 7365 6c66 290d  _get_size(self).
-00000550: 0a0d 0a20 2020 2064 6566 2073 6d61 6c6c  ...    def small
-00000560: 5f7a 6970 2873 656c 6629 3a0d 0a20 2020  _zip(self):..   
-00000570: 2020 2020 2072 6574 7572 6e20 5f69 735f       return _is_
-00000580: 736d 616c 6c5f 7a69 7028 7365 6c66 290d  small_zip(self).
-00000590: 0a0d 0a20 2020 2064 6566 2073 697a 655f  ...    def size_
-000005a0: 6573 7469 6d61 7465 2873 656c 6629 3a0d  estimate(self):.
-000005b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000005c0: 2725 2e32 6620 4d42 2720 2520 285f 6765  '%.2f MB' % (_ge
-000005d0: 745f 7369 7a65 2873 656c 6629 202f 2031  t_size(self) / 1
-000005e0: 3032 342e 3020 2f20 3130 3234 290d 0a0d  024.0 / 1024)...
-000005f0: 0a0d 0a63 6c61 7373 205a 6970 7065 7228  ...class Zipper(
-00000600: 4272 6f77 7365 7256 6965 7729 3a0d 0a20  BrowserView):.. 
-00000610: 2020 2022 2222 205a 6970 7320 636f 6e74     """ Zips cont
-00000620: 656e 7420 746f 2061 2074 656d 7020 6669  ent to a temp fi
-00000630: 6c65 2022 2222 0d0a 0d0a 2020 2020 6465  le """....    de
-00000640: 6620 7465 6368 6e69 6361 6c5f 7375 7070  f technical_supp
-00000650: 6f72 745f 6164 6472 6573 7328 7365 6c66  ort_address(self
-00000660: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-00000670: 726e 2070 6c6f 6e65 2e61 7069 2e70 6f72  rn plone.api.por
-00000680: 7461 6c2e 6765 745f 7265 6769 7374 7279  tal.get_registry
-00000690: 5f72 6563 6f72 6428 2769 6d73 2e7a 6970  _record('ims.zip
-000006a0: 2e69 6e74 6572 6661 6365 732e 495a 6970  .interfaces.IZip
-000006b0: 5365 7474 696e 6773 2e74 6563 686e 6963  Settings.technic
-000006c0: 616c 5f73 7570 706f 7274 5f61 6464 7265  al_support_addre
-000006d0: 7373 2729 206f 7220 5c0d 0a20 2020 2020  ss') or \..     
-000006e0: 2020 2020 2020 2070 6c6f 6e65 2e61 7069         plone.api
-000006f0: 2e70 6f72 7461 6c2e 6765 745f 7265 6769  .portal.get_regi
-00000700: 7374 7279 5f72 6563 6f72 6428 2770 6c6f  stry_record('plo
-00000710: 6e65 2e65 6d61 696c 5f66 726f 6d5f 6164  ne.email_from_ad
-00000720: 6472 6573 7327 290d 0a0d 0a20 2020 2064  dress')....    d
-00000730: 6566 205f 5f63 616c 6c5f 5f28 7365 6c66  ef __call__(self
-00000740: 293a 0d0a 2020 2020 2020 2020 7472 793a  ):..        try:
-00000750: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00000760: 7475 726e 2073 656c 662e 646f 5f7a 6970  turn self.do_zip
-00000770: 2829 0d0a 2020 2020 2020 2020 6578 6365  ()..        exce
-00000780: 7074 207a 6970 6669 6c65 2e4c 6172 6765  pt zipfile.Large
-00000790: 5a69 7046 696c 653a 0d0a 2020 2020 2020  ZipFile:..      
-000007a0: 2020 2020 2020 6d65 7373 6167 6520 3d20        message = 
-000007b0: 5f28 2254 6869 7320 666f 6c64 6572 2069  _("This folder i
-000007c0: 7320 746f 6f20 6c61 7267 6520 746f 2062  s too large to b
-000007d0: 6520 7a69 7070 6564 2e20 5472 7920 7a69  e zipped. Try zi
-000007e0: 7070 696e 6720 7375 6266 6f6c 6465 7273  pping subfolders
-000007f0: 2069 6e64 6976 6964 7561 6c6c 792e 2229   individually.")
-00000800: 0d0a 2020 2020 2020 2020 2020 2020 706c  ..            pl
-00000810: 6f6e 652e 6170 692e 706f 7274 616c 2e73  one.api.portal.s
-00000820: 686f 775f 6d65 7373 6167 6528 6d65 7373  how_message(mess
-00000830: 6167 652c 2073 656c 662e 7265 7175 6573  age, self.reques
-00000840: 742c 2074 7970 653d 2265 7272 6f72 2229  t, type="error")
-00000850: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00000860: 7475 726e 2073 656c 662e 7265 7175 6573  turn self.reques
-00000870: 742e 7265 7370 6f6e 7365 2e72 6564 6972  t.response.redir
-00000880: 6563 7428 7365 6c66 2e63 6f6e 7465 7874  ect(self.context
-00000890: 2e61 6273 6f6c 7574 655f 7572 6c28 2929  .absolute_url())
-000008a0: 0d0a 0d0a 2020 2020 6465 6620 646f 5f7a  ....    def do_z
-000008b0: 6970 2873 656c 6629 3a0d 0a20 2020 2020  ip(self):..     
-000008c0: 2020 2022 2222 205a 6970 2061 6c6c 206f     """ Zip all o
-000008d0: 6620 7468 6520 636f 6e74 656e 7420 696e  f the content in
-000008e0: 2074 6869 7320 6c6f 6361 7469 6f6e 2028   this location (
-000008f0: 636f 6e74 6578 7429 2222 220d 0a20 2020  context)"""..   
-00000900: 2020 2020 2069 6620 6e6f 7420 5f69 735f       if not _is_
-00000910: 736d 616c 6c5f 7a69 7028 7365 6c66 293a  small_zip(self):
-00000920: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00000930: 666f 7263 6520 7468 6973 2c20 7768 6574  force this, whet
-00000940: 6865 7220 6974 2077 6173 2070 6173 7365  her it was passe
-00000950: 6420 696e 2074 6865 2072 6571 7565 7374  d in the request
-00000960: 206f 7220 6e6f 740d 0a20 2020 2020 2020   or not..       
-00000970: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-00000980: 745b 277a 6970 3634 275d 203d 2031 0d0a  t['zip64'] = 1..
-00000990: 0d0a 2020 2020 2020 2020 6261 7365 5f70  ..        base_p
-000009a0: 6174 6820 3d20 272f 272e 6a6f 696e 2873  ath = '/'.join(s
-000009b0: 656c 662e 636f 6e74 6578 742e 6765 7450  elf.context.getP
-000009c0: 6879 7369 6361 6c50 6174 6828 2929 202b  hysicalPath()) +
-000009d0: 2027 2f27 2020 2320 7468 6520 7061 7468   '/'  # the path
-000009e0: 2069 6e20 7468 6520 5a43 6174 616c 6f67   in the ZCatalog
-000009f0: 0d0a 2020 2020 2020 2020 6361 7420 3d20  ..        cat = 
-00000a00: 706c 6f6e 652e 6170 692e 706f 7274 616c  plone.api.portal
-00000a10: 2e67 6574 5f74 6f6f 6c28 2770 6f72 7461  .get_tool('porta
-00000a20: 6c5f 6361 7461 6c6f 6727 290d 0a20 2020  l_catalog')..   
-00000a30: 2020 2020 2070 7479 7065 7320 3d20 6361       ptypes = ca
-00000a40: 742e 756e 6971 7565 5661 6c75 6573 466f  t.uniqueValuesFo
-00000a50: 7228 2770 6f72 7461 6c5f 7479 7065 2729  r('portal_type')
-00000a60: 0d0a 2020 2020 2020 2020 636f 6e74 656e  ..        conten
-00000a70: 7420 3d20 6361 7428 7061 7468 3d62 6173  t = cat(path=bas
-00000a80: 655f 7061 7468 2c20 6f62 6a65 6374 5f70  e_path, object_p
-00000a90: 726f 7669 6465 733d 495a 6970 7061 626c  rovides=IZippabl
-00000aa0: 652e 5f5f 6964 656e 7469 6669 6572 5f5f  e.__identifier__
-00000ab0: 2c20 706f 7274 616c 5f74 7970 653d 7074  , portal_type=pt
-00000ac0: 7970 6573 290d 0a20 2020 2020 2020 2069  ypes)..        i
-00000ad0: 6620 6e6f 7420 7365 6c66 2e72 6571 7565  f not self.reque
-00000ae0: 7374 2e67 6574 2827 7a69 7036 3427 293a  st.get('zip64'):
-00000af0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00000b00: 6c66 2e72 6571 7565 7374 2e72 6573 706f  lf.request.respo
-00000b10: 6e73 652e 7365 7448 6561 6465 7228 2743  nse.setHeader('C
-00000b20: 6f6e 7465 6e74 2d54 7970 6527 2c20 2761  ontent-Type', 'a
-00000b30: 7070 6c69 6361 7469 6f6e 2f7a 6970 2729  pplication/zip')
-00000b40: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00000b50: 6c66 2e72 6571 7565 7374 2e72 6573 706f  lf.request.respo
-00000b60: 6e73 652e 7365 7448 6561 6465 7228 2743  nse.setHeader('C
-00000b70: 6f6e 7465 6e74 2d64 6973 706f 7369 7469  ontent-dispositi
-00000b80: 6f6e 272c 2027 6174 7461 6368 6d65 6e74  on', 'attachment
-00000b90: 3b66 696c 656e 616d 653d 2573 2e7a 6970  ;filename=%s.zip
-00000ba0: 2720 2520 7365 6c66 2e63 6f6e 7465 7874  ' % self.context
-00000bb0: 2e67 6574 4964 2829 290d 0a20 2020 2020  .getId())..     
-00000bc0: 2020 2020 2020 2072 6574 7572 6e20 7a69         return zi
-00000bd0: 7066 696c 6573 2863 6f6e 7465 6e74 2c20  pfiles(content, 
-00000be0: 6261 7365 5f70 6174 6829 0d0a 2020 2020  base_path)..    
-00000bf0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00000c00: 2020 2020 2020 2066 7374 7265 616d 203d         fstream =
-00000c10: 207a 6970 6669 6c65 7328 636f 6e74 656e   zipfiles(conten
-00000c20: 742c 2062 6173 655f 7061 7468 2c20 7a69  t, base_path, zi
-00000c30: 7036 343d 5472 7565 290d 0a20 2020 2020  p64=True)..     
-00000c40: 2020 2020 2020 206f 626a 5f69 6420 3d20         obj_id = 
-00000c50: 6627 7b73 656c 662e 636f 6e74 6578 742e  f'{self.context.
-00000c60: 6765 7449 6428 297d 2e7a 6970 270d 0a20  getId()}.zip'.. 
-00000c70: 2020 2020 2020 2020 2020 2063 6f6e 7461             conta
-00000c80: 696e 6572 203d 2070 6c6f 6e65 2e61 7069  iner = plone.api
-00000c90: 2e70 6f72 7461 6c2e 6765 7428 290d 0a20  .portal.get().. 
-00000ca0: 2020 2020 2020 2020 2020 2069 6620 6f62             if ob
-00000cb0: 6a5f 6964 206e 6f74 2069 6e20 636f 6e74  j_id not in cont
-00000cc0: 6169 6e65 723a 0d0a 2020 2020 2020 2020  ainer:..        
-00000cd0: 2020 2020 2020 2020 6f62 6a20 3d20 706c          obj = pl
-00000ce0: 6f6e 652e 6170 692e 636f 6e74 656e 742e  one.api.content.
-00000cf0: 6372 6561 7465 2874 7970 653d 2746 696c  create(type='Fil
-00000d00: 6527 2c20 6964 3d6f 626a 5f69 642c 2063  e', id=obj_id, c
-00000d10: 6f6e 7461 696e 6572 3d63 6f6e 7461 696e  ontainer=contain
-00000d20: 6572 2c0d 0a20 2020 2020 2020 2020 2020  er,..           
-00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d50: 2020 2020 6669 6c65 3d4e 616d 6564 426c      file=NamedBl
-00000d60: 6f62 4669 6c65 2866 7374 7265 616d 2c20  obFile(fstream, 
-00000d70: 6669 6c65 6e61 6d65 3d6f 626a 5f69 6429  filename=obj_id)
-00000d80: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00000d90: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00000da0: 2020 2020 2020 6f62 6a20 3d20 636f 6e74        obj = cont
-00000db0: 6169 6e65 725b 6f62 6a5f 6964 5d2e 6669  ainer[obj_id].fi
-00000dc0: 6c65 203d 204e 616d 6564 426c 6f62 4669  le = NamedBlobFi
-00000dd0: 6c65 2866 7374 7265 616d 2c20 6669 6c65  le(fstream, file
-00000de0: 6e61 6d65 3d6f 626a 5f69 6429 0d0a 0d0a  name=obj_id)....
-00000df0: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
-00000e00: 3d20 6622 3c70 3e59 6f75 7220 7a69 7020  = f"<p>Your zip 
-00000e10: 6669 6c65 2069 7320 7265 6164 7920 666f  file is ready fo
-00000e20: 7220 646f 776e 6c6f 6164 2061 7420 3c61  r download at <a
-00000e30: 2068 7265 663d 5c22 7b6f 626a 2e61 6273   href=\"{obj.abs
-00000e40: 6f6c 7574 655f 7572 6c28 297d 2f76 6965  olute_url()}/vie
-00000e50: 775c 223e 7b6f 626a 2e74 6974 6c65 7d3c  w\">{obj.title}<
-00000e60: 2f61 3e22 0d0a 2020 2020 2020 2020 2020  /a>"..          
-00000e70: 2020 6d61 696c 203d 2070 6c6f 6e65 2e61    mail = plone.a
-00000e80: 7069 2e70 6f72 7461 6c2e 6765 745f 746f  pi.portal.get_to
-00000e90: 6f6c 2827 4d61 696c 486f 7374 2729 0d0a  ol('MailHost')..
-00000ea0: 2020 2020 2020 2020 2020 2020 7369 7465              site
-00000eb0: 5f66 726f 6d20 3d20 706c 6f6e 652e 6170  _from = plone.ap
-00000ec0: 692e 706f 7274 616c 2e67 6574 5f72 6567  i.portal.get_reg
-00000ed0: 6973 7472 795f 7265 636f 7264 2827 706c  istry_record('pl
-00000ee0: 6f6e 652e 656d 6169 6c5f 6672 6f6d 5f61  one.email_from_a
-00000ef0: 6464 7265 7373 2729 0d0a 2020 2020 2020  ddress')..      
-00000f00: 2020 2020 2020 706f 7274 616c 5f74 6974        portal_tit
-00000f10: 6c65 203d 2070 6c6f 6e65 2e61 7069 2e70  le = plone.api.p
-00000f20: 6f72 7461 6c2e 6765 745f 7265 6769 7374  ortal.get_regist
-00000f30: 7279 5f72 6563 6f72 6428 2770 6c6f 6e65  ry_record('plone
-00000f40: 2e73 6974 655f 7469 746c 6527 290d 0a20  .site_title').. 
-00000f50: 2020 2020 2020 2020 2020 206d 6169 6c2e             mail.
-00000f60: 7365 6e64 284d 494d 4554 6578 7428 6d73  send(MIMEText(ms
-00000f70: 672c 2027 6874 6d6c 2729 2c20 6d74 6f3d  g, 'html'), mto=
-00000f80: 706c 6f6e 652e 6170 692e 7573 6572 2e67  plone.api.user.g
-00000f90: 6574 5f63 7572 7265 6e74 2829 2e67 6574  et_current().get
-00000fa0: 5072 6f70 6572 7479 2827 656d 6169 6c27  Property('email'
-00000fb0: 292c 206d 6672 6f6d 3d73 6974 655f 6672  ), mfrom=site_fr
-00000fc0: 6f6d 2c0d 0a20 2020 2020 2020 2020 2020  om,..           
-00000fd0: 2020 2020 2020 2020 2020 2073 7562 6a65             subje
-00000fe0: 6374 3d66 275a 6970 2066 696c 6520 7265  ct=f'Zip file re
-00000ff0: 6164 7920 6174 207b 706f 7274 616c 5f74  ady at {portal_t
-00001000: 6974 6c65 7d27 290d 0a                   itle}')..
+00000000: 696d 706f 7274 206f 730d 0a69 6d70 6f72  import os..impor
+00000010: 7420 7a69 7066 696c 650d 0a66 726f 6d20  t zipfile..from 
+00000020: 696f 2069 6d70 6f72 7420 4279 7465 7349  io import BytesI
+00000030: 4f0d 0a0d 0a69 6d70 6f72 7420 706c 6f6e  O....import plon
+00000040: 652e 6170 690d 0a66 726f 6d20 5072 6f64  e.api..from Prod
+00000050: 7563 7473 2e46 6976 652e 6272 6f77 7365  ucts.Five.browse
+00000060: 7220 696d 706f 7274 2042 726f 7773 6572  r import Browser
+00000070: 5669 6577 0d0a 6672 6f6d 207a 6f70 652e  View..from zope.
+00000080: 636f 6d70 6f6e 656e 7420 696d 706f 7274  component import
+00000090: 2071 7565 7279 4164 6170 7465 720d 0a0d   queryAdapter...
+000000a0: 0a66 726f 6d20 2e2e 2069 6d70 6f72 7420  .from .. import 
+000000b0: 5f0d 0a66 726f 6d20 2e2e 696e 7465 7266  _..from ..interf
+000000c0: 6163 6573 2069 6d70 6f72 7420 495a 6970  aces import IZip
+000000d0: 7061 626c 650d 0a0d 0a0d 0a64 6566 2063  pable......def c
+000000e0: 6f6e 7665 7274 5f74 6f5f 6279 7465 7328  onvert_to_bytes(
+000000f0: 7369 7a65 293a 0d0a 2020 2020 6e75 6d2c  size):..    num,
+00000100: 2075 6e69 7420 3d20 7369 7a65 2e73 706c   unit = size.spl
+00000110: 6974 2829 0d0a 2020 2020 6966 2075 6e69  it()..    if uni
+00000120: 742e 6c6f 7765 7228 2920 3d3d 2027 6b62  t.lower() == 'kb
+00000130: 273a 0d0a 2020 2020 2020 2020 7265 7475  ':..        retu
+00000140: 726e 2066 6c6f 6174 286e 756d 2920 2a20  rn float(num) * 
+00000150: 3130 3234 0d0a 2020 2020 656c 6966 2075  1024..    elif u
+00000160: 6e69 742e 6c6f 7765 7228 2920 3d3d 2027  nit.lower() == '
+00000170: 6d62 273a 0d0a 2020 2020 2020 2020 7265  mb':..        re
+00000180: 7475 726e 2066 6c6f 6174 286e 756d 2920  turn float(num) 
+00000190: 2a20 3130 3234 202a 2031 3032 340d 0a20  * 1024 * 1024.. 
+000001a0: 2020 2065 6c69 6620 756e 6974 2e6c 6f77     elif unit.low
+000001b0: 6572 2829 203d 3d20 2767 6227 3a0d 0a20  er() == 'gb':.. 
+000001c0: 2020 2020 2020 2072 6574 7572 6e20 666c         return fl
+000001d0: 6f61 7428 6e75 6d29 202a 2031 3032 3420  oat(num) * 1024 
+000001e0: 2a20 3130 3234 202a 2031 3032 340d 0a20  * 1024 * 1024.. 
+000001f0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00000200: 2020 7265 7475 726e 2066 6c6f 6174 286e    return float(n
+00000210: 756d 290d 0a0d 0a0d 0a64 6566 205f 6765  um)......def _ge
+00000220: 745f 7369 7a65 2876 6965 7729 3a0d 0a20  t_size(view):.. 
+00000230: 2020 2063 6174 203d 2070 6c6f 6e65 2e61     cat = plone.a
+00000240: 7069 2e70 6f72 7461 6c2e 6765 745f 746f  pi.portal.get_to
+00000250: 6f6c 2827 706f 7274 616c 5f63 6174 616c  ol('portal_catal
+00000260: 6f67 2729 0d0a 0d0a 2020 2020 6261 7365  og')....    base
+00000270: 5f70 6174 6820 3d20 272f 272e 6a6f 696e  _path = '/'.join
+00000280: 2876 6965 772e 636f 6e74 6578 742e 6765  (view.context.ge
+00000290: 7450 6879 7369 6361 6c50 6174 6828 2929  tPhysicalPath())
+000002a0: 202b 2027 2f27 2020 2320 7468 6520 7061   + '/'  # the pa
+000002b0: 7468 2069 6e20 7468 6520 5a43 6174 616c  th in the ZCatal
+000002c0: 6f67 0d0a 2020 2020 7074 7970 6573 203d  og..    ptypes =
+000002d0: 2063 6174 2e75 6e69 7175 6556 616c 7565   cat.uniqueValue
+000002e0: 7346 6f72 2827 706f 7274 616c 5f74 7970  sFor('portal_typ
+000002f0: 6527 290d 0a0d 0a20 2020 2063 6f6e 7465  e')....    conte
+00000300: 6e74 203d 2063 6174 2870 6174 683d 6261  nt = cat(path=ba
+00000310: 7365 5f70 6174 682c 206f 626a 6563 745f  se_path, object_
+00000320: 7072 6f76 6964 6573 3d49 5a69 7070 6162  provides=IZippab
+00000330: 6c65 2e5f 5f69 6465 6e74 6966 6965 725f  le.__identifier_
+00000340: 5f2c 2070 6f72 7461 6c5f 7479 7065 3d70  _, portal_type=p
+00000350: 7479 7065 7329 0d0a 2020 2020 7265 7475  types)..    retu
+00000360: 726e 2073 756d 285b 622e 6765 744f 626a  rn sum([b.getObj
+00000370: 5369 7a65 2061 6e64 2063 6f6e 7665 7274  Size and convert
+00000380: 5f74 6f5f 6279 7465 7328 622e 6765 744f  _to_bytes(b.getO
+00000390: 626a 5369 7a65 2920 6f72 2030 2066 6f72  bjSize) or 0 for
+000003a0: 2062 2069 6e20 636f 6e74 656e 745d 290d   b in content]).
+000003b0: 0a0d 0a0d 0a64 6566 205f 6973 5f7a 6970  .....def _is_zip
+000003c0: 7061 626c 6528 7669 6577 293a 0d0a 2020  pable(view):..  
+000003d0: 2020 7265 7475 726e 205f 6765 745f 7369    return _get_si
+000003e0: 7a65 2876 6965 7729 203c 3d20 3220 2a20  ze(view) <= 2 * 
+000003f0: 3130 3234 2e30 202a 2031 3032 342e 3020  1024.0 * 1024.0 
+00000400: 2a20 3130 3234 2e30 2020 2320 3220 4742  * 1024.0  # 2 GB
+00000410: 0d0a 0d0a 0d0a 636c 6173 7320 5a69 7050  ......class ZipP
+00000420: 726f 6d70 7428 4272 6f77 7365 7256 6965  rompt(BrowserVie
+00000430: 7729 3a0d 0a20 2020 2022 2222 2063 6f6e  w):..    """ con
+00000440: 6669 726d 207a 6970 2022 2222 0d0a 0d0a  firm zip """....
+00000450: 2020 2020 6465 6620 7465 6368 6e69 6361      def technica
+00000460: 6c5f 7375 7070 6f72 745f 6164 6472 6573  l_support_addres
+00000470: 7328 7365 6c66 293a 0d0a 2020 2020 2020  s(self):..      
+00000480: 2020 7265 7475 726e 2070 6c6f 6e65 2e61    return plone.a
+00000490: 7069 2e70 6f72 7461 6c2e 6765 745f 7265  pi.portal.get_re
+000004a0: 6769 7374 7279 5f72 6563 6f72 6428 2769  gistry_record('i
+000004b0: 6d73 2e7a 6970 2e69 6e74 6572 6661 6365  ms.zip.interface
+000004c0: 732e 495a 6970 5365 7474 696e 6773 2e74  s.IZipSettings.t
+000004d0: 6563 686e 6963 616c 5f73 7570 706f 7274  echnical_support
+000004e0: 5f61 6464 7265 7373 2729 0d0a 0d0a 2020  _address')....  
+000004f0: 2020 6465 6620 6765 745f 7369 7a65 2873    def get_size(s
+00000500: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
+00000510: 6574 7572 6e20 5f67 6574 5f73 697a 6528  eturn _get_size(
+00000520: 7365 6c66 290d 0a0d 0a20 2020 2064 6566  self)....    def
+00000530: 2069 735f 7a69 7070 6162 6c65 2873 656c   is_zippable(sel
+00000540: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
+00000550: 7572 6e20 5f69 735f 7a69 7070 6162 6c65  urn _is_zippable
+00000560: 2873 656c 6629 0d0a 0d0a 2020 2020 6465  (self)....    de
+00000570: 6620 7369 7a65 5f65 7374 696d 6174 6528  f size_estimate(
+00000580: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000590: 7265 7475 726e 2027 252e 3266 204d 4227  return '%.2f MB'
+000005a0: 2025 2028 5f67 6574 5f73 697a 6528 7365   % (_get_size(se
+000005b0: 6c66 2920 2f20 3130 3234 2e30 202f 2031  lf) / 1024.0 / 1
+000005c0: 3032 3429 0d0a 0d0a 0d0a 636c 6173 7320  024)......class 
+000005d0: 5a69 7070 6572 2842 726f 7773 6572 5669  Zipper(BrowserVi
+000005e0: 6577 293a 0d0a 2020 2020 2222 2220 5a69  ew):..    """ Zi
+000005f0: 7073 2063 6f6e 7465 6e74 2074 6f20 6120  ps content to a 
+00000600: 7465 6d70 2066 696c 6520 2222 220d 0a0d  temp file """...
+00000610: 0a20 2020 2064 6566 2074 6563 686e 6963  .    def technic
+00000620: 616c 5f73 7570 706f 7274 5f61 6464 7265  al_support_addre
+00000630: 7373 2873 656c 6629 3a0d 0a20 2020 2020  ss(self):..     
+00000640: 2020 2072 6574 7572 6e20 706c 6f6e 652e     return plone.
+00000650: 6170 692e 706f 7274 616c 2e67 6574 5f72  api.portal.get_r
+00000660: 6567 6973 7472 795f 7265 636f 7264 2827  egistry_record('
+00000670: 696d 732e 7a69 702e 696e 7465 7266 6163  ims.zip.interfac
+00000680: 6573 2e49 5a69 7053 6574 7469 6e67 732e  es.IZipSettings.
+00000690: 7465 6368 6e69 6361 6c5f 7375 7070 6f72  technical_suppor
+000006a0: 745f 6164 6472 6573 7327 290d 0a0d 0a20  t_address').... 
+000006b0: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
+000006c0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+000006d0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+000006e0: 2020 7365 6c66 2e72 6571 7565 7374 2e72    self.request.r
+000006f0: 6573 706f 6e73 652e 7365 7448 6561 6465  esponse.setHeade
+00000700: 7228 2743 6f6e 7465 6e74 2d54 7970 6527  r('Content-Type'
+00000710: 2c20 2761 7070 6c69 6361 7469 6f6e 2f7a  , 'application/z
+00000720: 6970 2729 0d0a 2020 2020 2020 2020 2020  ip')..          
+00000730: 2020 7365 6c66 2e72 6571 7565 7374 2e72    self.request.r
+00000740: 6573 706f 6e73 652e 7365 7448 6561 6465  esponse.setHeade
+00000750: 7228 2743 6f6e 7465 6e74 2d64 6973 706f  r('Content-dispo
+00000760: 7369 7469 6f6e 272c 2027 6174 7461 6368  sition', 'attach
+00000770: 6d65 6e74 3b66 696c 656e 616d 653d 2573  ment;filename=%s
+00000780: 2e7a 6970 2720 2520 7365 6c66 2e63 6f6e  .zip' % self.con
+00000790: 7465 7874 2e67 6574 4964 2829 290d 0a20  text.getId()).. 
+000007a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000007b0: 6e20 7365 6c66 2e64 6f5f 7a69 7028 290d  n self.do_zip().
+000007c0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000007d0: 7a69 7066 696c 652e 4c61 7267 655a 6970  zipfile.LargeZip
+000007e0: 4669 6c65 3a0d 0a20 2020 2020 2020 2020  File:..         
+000007f0: 2020 206d 6573 7361 6765 203d 205f 2822     message = _("
+00000800: 5468 6973 2066 6f6c 6465 7220 6973 2074  This folder is t
+00000810: 6f6f 206c 6172 6765 2074 6f20 6265 207a  oo large to be z
+00000820: 6970 7065 642e 2054 7279 207a 6970 7069  ipped. Try zippi
+00000830: 6e67 2073 7562 666f 6c64 6572 7320 696e  ng subfolders in
+00000840: 6469 7669 6475 616c 6c79 2e22 290d 0a20  dividually.").. 
+00000850: 2020 2020 2020 2020 2020 2070 6c6f 6e65             plone
+00000860: 2e61 7069 2e70 6f72 7461 6c2e 7368 6f77  .api.portal.show
+00000870: 5f6d 6573 7361 6765 286d 6573 7361 6765  _message(message
+00000880: 2c20 7365 6c66 2e72 6571 7565 7374 2c20  , self.request, 
+00000890: 7479 7065 3d22 6572 726f 7222 290d 0a20  type="error").. 
+000008a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000008b0: 6e20 7365 6c66 2e72 6571 7565 7374 2e72  n self.request.r
+000008c0: 6573 706f 6e73 652e 7265 6469 7265 6374  esponse.redirect
+000008d0: 2873 656c 662e 636f 6e74 6578 742e 6162  (self.context.ab
+000008e0: 736f 6c75 7465 5f75 726c 2829 290d 0a0d  solute_url())...
+000008f0: 0a20 2020 2064 6566 2064 6f5f 7a69 7028  .    def do_zip(
+00000900: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000910: 2222 2220 5a69 7020 616c 6c20 6f66 2074  """ Zip all of t
+00000920: 6865 2063 6f6e 7465 6e74 2069 6e20 7468  he content in th
+00000930: 6973 206c 6f63 6174 696f 6e20 2863 6f6e  is location (con
+00000940: 7465 7874 2922 2222 0d0a 2020 2020 2020  text)"""..      
+00000950: 2020 6966 206e 6f74 205f 6973 5f7a 6970    if not _is_zip
+00000960: 7061 626c 6528 7365 6c66 293a 0d0a 2020  pable(self):..  
+00000970: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+00000980: 6520 3d20 5f28 2254 6869 7320 666f 6c64  e = _("This fold
+00000990: 6572 2069 7320 746f 6f20 6c61 7267 6520  er is too large 
+000009a0: 746f 2062 6520 7a69 7070 6564 2e20 5472  to be zipped. Tr
+000009b0: 7920 7a69 7070 696e 6720 7375 6266 6f6c  y zipping subfol
+000009c0: 6465 7273 2069 6e64 6976 6964 7561 6c6c  ders individuall
+000009d0: 792e 2229 0d0a 2020 2020 2020 2020 2020  y.")..          
+000009e0: 2020 706c 6f6e 652e 6170 692e 706f 7274    plone.api.port
+000009f0: 616c 2e73 686f 775f 6d65 7373 6167 6528  al.show_message(
+00000a00: 6d65 7373 6167 652c 2073 656c 662e 7265  message, self.re
+00000a10: 7175 6573 742c 2074 7970 653d 2265 7272  quest, type="err
+00000a20: 6f72 2229 0d0a 2020 2020 2020 2020 2020  or")..          
+00000a30: 2020 7265 7475 726e 2073 656c 662e 7265    return self.re
+00000a40: 7175 6573 742e 7265 7370 6f6e 7365 2e72  quest.response.r
+00000a50: 6564 6972 6563 7428 7365 6c66 2e63 6f6e  edirect(self.con
+00000a60: 7465 7874 2e61 6273 6f6c 7574 655f 7572  text.absolute_ur
+00000a70: 6c28 2929 0d0a 0d0a 2020 2020 2020 2020  l())....        
+00000a80: 7374 7265 616d 203d 2042 7974 6573 494f  stream = BytesIO
+00000a90: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
+00000aa0: 2e7a 6970 6669 6c65 7328 7374 7265 616d  .zipfiles(stream
+00000ab0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00000ac0: 6e20 7374 7265 616d 2e67 6574 7661 6c75  n stream.getvalu
+00000ad0: 6528 290d 0a0d 0a20 2020 2064 6566 207a  e()....    def z
+00000ae0: 6970 6669 6c65 7328 7365 6c66 2c20 6673  ipfiles(self, fs
+00000af0: 7472 6561 6d29 3a0d 0a20 2020 2020 2020  tream):..       
+00000b00: 2022 2222 5265 7475 726e 2074 6865 2070   """Return the p
+00000b10: 6174 6820 616e 6420 6669 6c65 2073 7472  ath and file str
+00000b20: 6561 6d20 6f66 2061 6c6c 2063 6f6e 7465  eam of all conte
+00000b30: 6e74 2077 6520 6669 6e64 2068 6572 6522  nt we find here"
+00000b40: 2222 0d0a 2020 2020 2020 2020 6261 7365  ""..        base
+00000b50: 5f70 6174 6820 3d20 272f 272e 6a6f 696e  _path = '/'.join
+00000b60: 2873 656c 662e 636f 6e74 6578 742e 6765  (self.context.ge
+00000b70: 7450 6879 7369 6361 6c50 6174 6828 2929  tPhysicalPath())
+00000b80: 202b 2027 2f27 2020 2320 7468 6520 7061   + '/'  # the pa
+00000b90: 7468 2069 6e20 7468 6520 5a43 6174 616c  th in the ZCatal
+00000ba0: 6f67 0d0a 2020 2020 2020 2020 6361 7420  og..        cat 
+00000bb0: 3d20 706c 6f6e 652e 6170 692e 706f 7274  = plone.api.port
+00000bc0: 616c 2e67 6574 5f74 6f6f 6c28 2770 6f72  al.get_tool('por
+00000bd0: 7461 6c5f 6361 7461 6c6f 6727 290d 0a0d  tal_catalog')...
+00000be0: 0a20 2020 2020 2020 207a 6970 7065 7220  .        zipper 
+00000bf0: 3d20 7a69 7066 696c 652e 5a69 7046 696c  = zipfile.ZipFil
+00000c00: 6528 6673 7472 6561 6d2c 2027 7727 2c20  e(fstream, 'w', 
+00000c10: 7a69 7066 696c 652e 5a49 505f 4445 464c  zipfile.ZIP_DEFL
+00000c20: 4154 4544 290d 0a20 2020 2020 2020 2070  ATED)..        p
+00000c30: 7479 7065 7320 3d20 6361 742e 756e 6971  types = cat.uniq
+00000c40: 7565 5661 6c75 6573 466f 7228 2770 6f72  ueValuesFor('por
+00000c50: 7461 6c5f 7479 7065 2729 0d0a 0d0a 2020  tal_type')....  
+00000c60: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
+00000c70: 6361 7428 7061 7468 3d62 6173 655f 7061  cat(path=base_pa
+00000c80: 7468 2c20 6f62 6a65 6374 5f70 726f 7669  th, object_provi
+00000c90: 6465 733d 495a 6970 7061 626c 652e 5f5f  des=IZippable.__
+00000ca0: 6964 656e 7469 6669 6572 5f5f 2c20 706f  identifier__, po
+00000cb0: 7274 616c 5f74 7970 653d 7074 7970 6573  rtal_type=ptypes
+00000cc0: 290d 0a20 2020 2020 2020 2066 6f72 2063  )..        for c
+00000cd0: 2069 6e20 636f 6e74 656e 743a 0d0a 2020   in content:..  
+00000ce0: 2020 2020 2020 2020 2020 7265 6c5f 7061            rel_pa
+00000cf0: 7468 203d 2063 2e67 6574 5061 7468 2829  th = c.getPath()
+00000d00: 2e73 706c 6974 2862 6173 655f 7061 7468  .split(base_path
+00000d10: 295b 313a 5d20 6f72 205b 632e 6765 7449  )[1:] or [c.getI
+00000d20: 645d 2020 2320 7468 6520 6c61 7474 6572  d]  # the latter
+00000d30: 2069 6620 7468 6520 726f 6f74 206f 626a   if the root obj
+00000d40: 6563 7420 6861 7320 616e 2061 6461 7074  ect has an adapt
+00000d50: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
+00000d60: 6966 2072 656c 5f70 6174 683a 0d0a 2020  if rel_path:..  
+00000d70: 2020 2020 2020 2020 2020 2020 2020 6f62                ob
+00000d80: 6a20 3d20 632e 6765 744f 626a 6563 7428  j = c.getObject(
+00000d90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00000da0: 2020 207a 6970 5f70 6174 6820 3d20 6f73     zip_path = os
+00000db0: 2e70 6174 682e 6a6f 696e 282a 7265 6c5f  .path.join(*rel_
+00000dc0: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
+00000dd0: 2020 2020 2020 2061 6461 7074 6572 203d         adapter =
+00000de0: 2071 7565 7279 4164 6170 7465 7228 6f62   queryAdapter(ob
+00000df0: 6a2c 2049 5a69 7070 6162 6c65 290d 0a20  j, IZippable).. 
+00000e00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00000e10: 7472 6561 6d20 3d20 6164 6170 7465 722e  tream = adapter.
+00000e20: 7a69 7070 6162 6c65 2829 0d0a 2020 2020  zippable()..    
+00000e30: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00000e40: 7472 6561 6d3a 0d0a 2020 2020 2020 2020  tream:..        
+00000e50: 2020 2020 2020 2020 2020 2020 6578 7420              ext 
+00000e60: 3d20 6164 6170 7465 722e 6578 7465 6e73  = adapter.extens
+00000e70: 696f 6e28 290d 0a20 2020 2020 2020 2020  ion()..         
+00000e80: 2020 2020 2020 2020 2020 2063 6f6d 706f             compo
+00000e90: 6e65 6e74 5f6e 616d 6520 3d20 7a69 705f  nent_name = zip_
+00000ea0: 7061 7468 202b 2065 7874 0d0a 2020 2020  path + ext..    
+00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ec0: 7a69 7070 6572 2e77 7269 7465 7374 7228  zipper.writestr(
+00000ed0: 636f 6d70 6f6e 656e 745f 6e61 6d65 2c20  component_name, 
+00000ee0: 7374 7265 616d 290d 0a20 2020 2020 2020  stream)..       
+00000ef0: 2020 2020 2020 2020 2020 2020 2063 7265               cre
+00000f00: 6174 6564 203d 206f 626a 2e63 7265 6174  ated = obj.creat
+00000f10: 6564 2829 0d0a 2020 2020 2020 2020 2020  ed()..          
+00000f20: 2020 2020 2020 2020 2020 7a69 7070 6572            zipper
+00000f30: 2e4e 616d 6554 6f49 6e66 6f5b 636f 6d70  .NameToInfo[comp
+00000f40: 6f6e 656e 745f 6e61 6d65 5d2e 6461 7465  onent_name].date
+00000f50: 5f74 696d 6520 3d20 280d 0a20 2020 2020  _time = (..     
+00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f70: 2020 2063 7265 6174 6564 2e79 6561 7228     created.year(
+00000f80: 292c 2063 7265 6174 6564 2e6d 6f6e 7468  ), created.month
+00000f90: 2829 2c20 6372 6561 7465 642e 6461 7928  (), created.day(
+00000fa0: 292c 2063 7265 6174 6564 2e68 6f75 7228  ), created.hour(
+00000fb0: 292c 2063 7265 6174 6564 2e6d 696e 7574  ), created.minut
+00000fc0: 6528 292c 0d0a 2020 2020 2020 2020 2020  e(),..          
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00000fe0: 7428 6372 6561 7465 642e 7365 636f 6e64  t(created.second
+00000ff0: 2829 2929 0d0a 2020 2020 2020 2020 7a69  ()))..        zi
+00001000: 7070 6572 2e63 6c6f 7365 2829 0d0a       pper.close()..
```

### Comparing `ims.zip-4.2.1/ims/zip/configure.zcml` & `ims.zip-5.0/ims/zip/configure.zcml`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,82 @@
-<configure
-        xmlns="http://namespaces.zope.org/zope"
-        xmlns:five="http://namespaces.zope.org/five"
-        xmlns:i18n="http://namespaces.zope.org/i18n"
-        xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
-        i18n_domain="ims.zip">
-
-    <permission
-            id="ims.CanZip"
-            title="ims.zip: can zip"/>
-
-    <permission
-            id="ims.CanUnzip"
-            title="ims.zip: can unzip"/>
-
-    <include package=".browser"/>
-
-    <adapter
-            for="plone.app.contenttypes.interfaces.IFile"
-            provides=".interfaces.IZippable"
-            factory=".adapters.FileZip"/>
-
-    <adapter
-            for="plone.app.contenttypes.interfaces.IImage"
-            provides=".interfaces.IZippable"
-            factory=".adapters.ImageZip"/>
-
-    <adapter
-            for="plone.app.contenttypes.interfaces.IDocument"
-            provides=".interfaces.IZippable"
-            factory=".adapters.DocumentZip"/>
-
-    <class class="plone.app.contenttypes.content.File">
-        <implements interface=".interfaces.IZippable"/>
-    </class>
-
-    <class class="plone.app.contenttypes.content.Image">
-        <implements interface=".interfaces.IZippable"/>
-    </class>
-
-    <class class="plone.app.contenttypes.content.Document">
-        <implements interface=".interfaces.IZippable"/>
-    </class>
-
-    <class class="plone.app.contenttypes.content.Folder">
-        <implements interface=".interfaces.IZipFolder"/>
-    </class>
-
-    <class class="Products.CMFPlone.Portal.PloneSite">
-        <implements interface=".interfaces.IZipFolder"/>
-    </class>
-
-    <genericsetup:registerProfile
-            name="default"
-            title="ims.zip"
-            directory="profiles/default"
-            description="Provides actions for zipping and unzipping "
-            provides="Products.GenericSetup.interfaces.EXTENSION"/>
-
-    <genericsetup:registerProfile
-            name="uninstall"
-            title="ims.zip [uninstall]"
-            directory="profiles/uninstall"
-            description="Provides actions for zipping and unzipping "
-            provides="Products.GenericSetup.interfaces.EXTENSION"/>
-
+<configure
+        xmlns="http://namespaces.zope.org/zope"
+        xmlns:five="http://namespaces.zope.org/five"
+        xmlns:i18n="http://namespaces.zope.org/i18n"
+        xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
+        i18n_domain="ims.zip">
+
+    <permission
+            id="ims.CanZip"
+            title="ims.zip: can zip"/>
+
+    <permission
+            id="ims.CanUnzip"
+            title="ims.zip: can unzip"/>
+
+    <include package=".browser"/>
+
+    <adapter
+            for="plone.app.contenttypes.interfaces.IFile"
+            provides=".interfaces.IZippable"
+            factory=".adapters.FileZip"/>
+
+    <adapter
+            for="plone.app.contenttypes.interfaces.IImage"
+            provides=".interfaces.IZippable"
+            factory=".adapters.ImageZip"/>
+
+    <adapter
+            for="plone.app.contenttypes.interfaces.IDocument"
+            provides=".interfaces.IZippable"
+            factory=".adapters.DocumentZip"/>
+
+    <class class="plone.app.contenttypes.content.File">
+        <implements interface=".interfaces.IZippable"/>
+    </class>
+
+    <class class="plone.app.contenttypes.content.Image">
+        <implements interface=".interfaces.IZippable"/>
+    </class>
+
+    <class class="plone.app.contenttypes.content.Document">
+        <implements interface=".interfaces.IZippable"/>
+    </class>
+
+    <class class="plone.app.contenttypes.content.Folder">
+        <implements interface=".interfaces.IZipFolder"/>
+    </class>
+
+    <class class="Products.CMFPlone.Portal.PloneSite">
+        <implements interface=".interfaces.IZipFolder"/>
+    </class>
+
+    <genericsetup:registerProfile
+            name="default"
+            title="ims.zip"
+            directory="profiles/default"
+            description="Provides actions for zipping and unzipping "
+            provides="Products.GenericSetup.interfaces.EXTENSION"/>
+
+    <genericsetup:registerProfile
+            name="uninstall"
+            title="ims.zip [uninstall]"
+            directory="profiles/uninstall"
+            description="Provides actions for zipping and unzipping "
+            provides="Products.GenericSetup.interfaces.EXTENSION"/>
+
+    <genericsetup:registerProfile
+            name="upgrade to plone 6"
+            title="ims.zip"
+            directory="profiles/upgrade_1"
+            description="Adds icons"
+            provides="Products.GenericSetup.interfaces.EXTENSION"/>
+
+    <genericsetup:upgradeStep
+            title="Upgrade to 5"
+            description="Adds icons"
+            source="*"
+            destination="1"
+            handler=".upgrades.upgrade_1"
+            profile="ims.zip:default"/>
+
 </configure>
```

### Comparing `ims.zip-4.2.1/ims/zip/interfaces.py` & `ims.zip-5.0/ims/zip/interfaces.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class IZipFolder(Interface):
     """ Locations where you can zip content """
 
 
 class IUnzipForm(model.Schema):
     file = NamedFile(
         title=_("Zip File"),
-        required=False,
+        required=True,
     )
     force_files = schema.Bool(
         title=_("Force upload as Files"),
         description=_("If unchecked, some files will become Pages, such as .html and .txt"),
         required=False,
     )
```

### Comparing `ims.zip-4.2.1/ims/zip/profiles/default/actions.xml` & `ims.zip-5.0/ims/zip/profiles/default/actions.xml`

 * *Files 11% similar despite different names*

#### Comparing `ims.zip-4.2.1/ims/zip/profiles/default/actions.xml` & `ims.zip-5.0/ims/zip/profiles/default/actions.xml`

```diff
@@ -1,26 +1,26 @@
 <?xml version="1.0" encoding="utf-8"?>
 <object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="portal_actions" meta_type="Plone Actions Tool">
   <object name="object_buttons" meta_type="CMF Action Category">
     <object name="zip" meta_type="CMF Action" i18n:domain="ims.zip">
       <property name="title" i18n:translate="">Create zip archive</property>
       <property name="description" i18n:translate="">Zip all files</property>
+      <property name="icon_expr">string:file-earmark-zip-fill</property>
       <property name="url_expr">string:${plone_context_state/canonical_object_url}/@@zipfiles</property>
-      <property name="icon_expr"/>
       <property name="available_expr">python:plone_context_state.is_folderish() or plone_context_state.is_default_page()</property>
       <property name="permissions">
         <element value="ims.zip: can zip"/>
       </property>
       <property name="visible">True</property>
     </object>
     <object name="unzip" meta_type="CMF Action" i18n:domain="ims.zip">
       <property name="title" i18n:translate="">Unpack zip archive</property>
       <property name="description" i18n:translate="">Unzip files into a folder</property>
+      <property name="icon_expr">string:file-earmark-zip</property>
       <property name="url_expr">string:${plone_context_state/canonical_object_url}/@@unzip</property>
-      <property name="icon_expr"/>
       <property name="available_expr">python:plone_context_state.is_folderish() or plone_context_state.is_default_page()</property>
       <property name="permissions">
         <element value="ims.zip: can unzip"/>
       </property>
       <property name="visible">True</property>
     </object>
   </object>
```

### Comparing `ims.zip-4.2.1/ims/zip/testing.py` & `ims.zip-5.0/ims/zip/testing.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import ims.zip
-from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
-from plone.app.testing import PloneSandboxLayer, IntegrationTesting, FunctionalTesting, applyProfile
-
-
-class ZipSiteLayer(PloneSandboxLayer):
-    defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
-
-    def setUpZope(self, app, configuration_context):
-        self.loadZCML(package=ims.zip)
-
-    def setUpPloneSite(self, portal):
-        applyProfile(portal, 'ims.zip:default')
-
-
-ZIP_SITE_FIXTURE = ZipSiteLayer()
-
-INTEGRATION = IntegrationTesting(
-    bases=(ZIP_SITE_FIXTURE,),
-    name="ims.zip:Integration"
-)
-
-FUNCTIONAL = FunctionalTesting(
-    bases=(ZIP_SITE_FIXTURE,),
-    name="ims.zip:Functional"
-)
+import ims.zip
+from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
+from plone.app.testing import PloneSandboxLayer, IntegrationTesting, FunctionalTesting, applyProfile
+
+
+class ZipSiteLayer(PloneSandboxLayer):
+    defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
+
+    def setUpZope(self, app, configuration_context):
+        self.loadZCML(package=ims.zip)
+
+    def setUpPloneSite(self, portal):
+        applyProfile(portal, 'ims.zip:default')
+
+
+ZIP_SITE_FIXTURE = ZipSiteLayer()
+
+INTEGRATION = IntegrationTesting(
+    bases=(ZIP_SITE_FIXTURE,),
+    name="ims.zip:Integration"
+)
+
+FUNCTIONAL = FunctionalTesting(
+    bases=(ZIP_SITE_FIXTURE,),
+    name="ims.zip:Functional"
+)
```

### Comparing `ims.zip-4.2.1/ims/zip/tests/base.py` & `ims.zip-5.0/ims/zip/tests/base.py`

 * *Files identical despite different names*

### Comparing `ims.zip-4.2.1/ims/zip/tests/input/canoneye.jpg` & `ims.zip-5.0/ims/zip/tests/input/canoneye.jpg`

 * *Files identical despite different names*

### Comparing `ims.zip-4.2.1/ims/zip/tests/input/folder1/canoneye.jpg` & `ims.zip-5.0/ims/zip/tests/input/folder1/canoneye.jpg`

 * *Files identical despite different names*

### Comparing `ims.zip-4.2.1/ims/zip/tests/input/test.zip` & `ims.zip-5.0/ims/zip/tests/input/test.zip`

 * *Files identical despite different names*

### Comparing `ims.zip-4.2.1/ims/zip/tests/output/test.zip` & `ims.zip-5.0/ims/zip/tests/output/test.zip`

 * *Files identical despite different names*

### Comparing `ims.zip-4.2.1/ims/zip/tests/test_uninstall.py` & `ims.zip-5.0/ims/zip/tests/test_uninstall.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from Products.CMFPlone.utils import get_installer
-from plone import api
-from plone.app.testing import TEST_USER_ID
-from plone.app.testing import setRoles
-
-from . import base
-from .. import testing
-
-
-class TestUninstall(base.IntegrationTestCase):
-    layer = testing.INTEGRATION
-
-    def setUp(self):
-        self.portal = self.layer['portal']
-        roles_before = api.user.get_roles(TEST_USER_ID)
-        setRoles(self.portal, TEST_USER_ID, ['Manager'])
-        self.installer = get_installer(self.portal)
-        self.installer.uninstall_product('ims.zip')
-        setRoles(self.portal, TEST_USER_ID, roles_before)
-
-    def test_product_uninstalled(self):
-        """Test if ims.zip is cleanly uninstalled."""
-        self.assertFalse(self.installer.is_product_installed('ims.zip'))
+from Products.CMFPlone.utils import get_installer
+from plone import api
+from plone.app.testing import TEST_USER_ID
+from plone.app.testing import setRoles
+
+from . import base
+from .. import testing
+
+
+class TestUninstall(base.IntegrationTestCase):
+    layer = testing.INTEGRATION
+
+    def setUp(self):
+        self.portal = self.layer['portal']
+        roles_before = api.user.get_roles(TEST_USER_ID)
+        setRoles(self.portal, TEST_USER_ID, ['Manager'])
+        self.installer = get_installer(self.portal)
+        self.installer.uninstall_product('ims.zip')
+        setRoles(self.portal, TEST_USER_ID, roles_before)
+
+    def test_product_uninstalled(self):
+        """Test if ims.zip is cleanly uninstalled."""
+        self.assertFalse(self.installer.is_product_installed('ims.zip'))
```

### Comparing `ims.zip-4.2.1/ims/zip/tests/test_zip.py` & `ims.zip-5.0/ims/zip/tests/test_zip.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-import os
-import zipfile
-from io import BytesIO
-
-import plone.api as api
-from App.Common import package_home
-from ims.zip.interfaces import IZippable, IZipFolder
-from plone.app.textfield import RichTextValue
-from plone.namedfile.file import NamedBlobFile, NamedBlobImage
-
-from . import base
-
-PACKAGE_HOME = package_home(globals())
-
-PAGE_TEXT = b'<html><meta http-equiv="Content-Type" content="text/html; charset=utf-8" /><body><h1>My page</h1>' \
-            b'<p class="description">A test page</p><p>hi!</p></body></html>'
-
-
-def load_file(name):
-    """Load image from testing directory"""
-    path = os.path.join(PACKAGE_HOME, 'input', name)
-    with open(path, 'rb') as _file:
-        data = _file.read()
-    return NamedBlobFile(data)
-
-
-def load_image(name):
-    """Load image from testing directory"""
-    path = os.path.join(PACKAGE_HOME, 'input', name)
-    with open(path, 'rb') as _file:
-        data = _file.read()
-    return NamedBlobImage(data)
-
-
-class TestBasic(base.IntegrationTestCase):
-    def create_file(self, parent):
-        ob = api.content.create(container=parent, id='file1', type='File', file=load_file('file.txt'))
-        ob.file.filename = 'file.txt'
-        self.file1 = ob
-        return ob
-
-    def create_image(self, parent):
-        ob = api.content.create(container=parent, id='image1', type='Image', image=load_image('canoneye.jpg'))
-        ob.image.filename = 'canoneye.jpg'
-        self.image1 = ob
-        return ob
-
-    def create_document(self, parent):
-        ob = api.content.create(container=parent, id='page1', type='Document', text=RichTextValue('<p>hi!</p>'),
-                                description='A test page', title='My page')
-        self.page1 = ob
-        return ob
-
-    def test_interfaces(self):
-        self.create_image(self.folder1)
-        self.create_file(self.folder1)
-        self.create_document(self.folder1)
-        self.assertTrue(IZipFolder.providedBy(self.folder1))
-        self.assertTrue(IZippable.providedBy(self.image1))
-        self.assertTrue(IZippable.providedBy(self.file1))
-        self.assertTrue(IZippable.providedBy(self.page1))
-
-    def test_file_indexed(self):
-        parent = self.folder2
-        base_path = '/'.join(parent.getPhysicalPath())
-        self.assertEqual(len(self.cat(path=base_path, object_provides=IZippable.__identifier__)), 0)
-        self.create_file(parent)
-        self.assertEqual(len(self.cat(path=base_path, object_provides=IZippable.__identifier__)), 1)
-
-    def test_image_indexed(self):
-        parent = self.folder1
-        base_path = '/'.join(parent.getPhysicalPath())
-        self.assertEqual(len(self.cat(path=base_path, object_provides=IZippable.__identifier__)), 0)
-        self.create_image(parent)
-        self.assertEqual(len(self.cat(path=base_path, object_provides=IZippable.__identifier__)), 1)
-
-    def testDocumentIndexed(self):
-        parent = self.folder3
-        base_path = '/'.join(parent.getPhysicalPath())
-        self.assertEqual(len(self.cat(path=base_path, object_provides=IZippable.__identifier__)), 0)
-        self.create_document(parent)
-        self.assertEqual(len(self.cat(path=base_path, object_provides=IZippable.__identifier__)), 1)
-
-    def test_zip(self):
-        self.create_image(self.folder1)
-        self.create_document(self.folder3)
-        self.create_file(self.folder2)
-
-        view = self.portal.restrictedTraverse('zipconfirm')
-        data = view()
-        zipper = zipfile.ZipFile(BytesIO(data), 'r', zipfile.ZIP_DEFLATED)
-
-        namelist = zipper.namelist()
-        self.assertIn('f1/image1.jpg', namelist)
-        self.assertIn('f2/f3/page1.html', namelist)
-        self.assertIn('f2/file1.txt', namelist)
-
-        stream = zipper.read('f1/image1.jpg')
-        self.assertEqual(stream, load_image('canoneye.jpg').data)
-
-        stream = zipper.read('f2/f3/page1.html')
-        self.assertEqual(stream, PAGE_TEXT)
-
-        stream = zipper.read('f2/file1.txt')
-        self.assertEqual(stream, load_file('file.txt').data)
-
-    def test_unzip(self):
-        view = self.portal.restrictedTraverse('unzip')
-
-        with open(os.path.join(PACKAGE_HOME, 'input', 'test.zip'), 'rb') as zipf:
-            data = zipf.read()
-        zipf = NamedBlobFile(data=data)
-        view.unzip(zipf)
-
-        page1 = self.cat(path='/plone/folder2/folder3/page1.html')[0].getObject()
-        self.assertEqual(page1.text.raw, PAGE_TEXT)
-        self.assertEqual(page1.title, 'page1.html')
-
-
-def test_suite():
-    import unittest
-    return unittest.defaultTestLoader.loadTestsFromName(__name__)
+import os
+import zipfile
+from io import BytesIO
+
+import plone.api as api
+from App.Common import package_home
+from ims.zip.interfaces import IZippable, IZipFolder
+from plone.app.textfield import RichTextValue
+from plone.namedfile.file import NamedBlobFile, NamedBlobImage
+
+from . import base
+
+PACKAGE_HOME = package_home(globals())
+
+PAGE_TEXT = b'<html><meta http-equiv="Content-Type" content="text/html; charset=utf-8" /><body><h1>My page</h1>' \
+            b'<p class="description">A test page</p><p>hi!</p></body></html>'
+
+
+def load_file(name):
+    """Load image from testing directory"""
+    path = os.path.join(PACKAGE_HOME, 'input', name)
+    with open(path, 'rb') as _file:
+        data = _file.read()
+    return NamedBlobFile(data)
+
+
+def load_image(name):
+    """Load image from testing directory"""
+    path = os.path.join(PACKAGE_HOME, 'input', name)
+    with open(path, 'rb') as _file:
+        data = _file.read()
+    return NamedBlobImage(data)
+
+
+class TestBasic(base.IntegrationTestCase):
+    def create_file(self, parent):
+        ob = api.content.create(container=parent, id='file1', type='File', file=load_file('file.txt'))
+        ob.file.filename = 'file.txt'
+        self.file1 = ob
+        return ob
+
+    def create_image(self, parent):
+        ob = api.content.create(container=parent, id='image1', type='Image', image=load_image('canoneye.jpg'))
+        ob.image.filename = 'canoneye.jpg'
+        self.image1 = ob
+        return ob
+
+    def create_document(self, parent):
+        ob = api.content.create(container=parent, id='page1', type='Document', text=RichTextValue('<p>hi!</p>'),
+                                description='A test page', title='My page')
+        self.page1 = ob
+        return ob
+
+    def test_interfaces(self):
+        self.create_image(self.folder1)
+        self.create_file(self.folder1)
+        self.create_document(self.folder1)
+        self.assertTrue(IZipFolder.providedBy(self.folder1))
+        self.assertTrue(IZippable.providedBy(self.image1))
+        self.assertTrue(IZippable.providedBy(self.file1))
+        self.assertTrue(IZippable.providedBy(self.page1))
+
+    def test_file_indexed(self):
+        parent = self.folder2
+        base_path = '/'.join(parent.getPhysicalPath())
+        self.assertEqual(len(self.cat(path=base_path, object_provides=IZippable.__identifier__)), 0)
+        self.create_file(parent)
+        self.assertEqual(len(self.cat(path=base_path, object_provides=IZippable.__identifier__)), 1)
+
+    def test_image_indexed(self):
+        parent = self.folder1
+        base_path = '/'.join(parent.getPhysicalPath())
+        self.assertEqual(len(self.cat(path=base_path, object_provides=IZippable.__identifier__)), 0)
+        self.create_image(parent)
+        self.assertEqual(len(self.cat(path=base_path, object_provides=IZippable.__identifier__)), 1)
+
+    def testDocumentIndexed(self):
+        parent = self.folder3
+        base_path = '/'.join(parent.getPhysicalPath())
+        self.assertEqual(len(self.cat(path=base_path, object_provides=IZippable.__identifier__)), 0)
+        self.create_document(parent)
+        self.assertEqual(len(self.cat(path=base_path, object_provides=IZippable.__identifier__)), 1)
+
+    def test_zip(self):
+        self.create_image(self.folder1)
+        self.create_document(self.folder3)
+        self.create_file(self.folder2)
+
+        view = self.portal.restrictedTraverse('zipconfirm')
+        data = view()
+        zipper = zipfile.ZipFile(BytesIO(data), 'r', zipfile.ZIP_DEFLATED)
+
+        namelist = zipper.namelist()
+        self.assertIn('f1/image1.jpg', namelist)
+        self.assertIn('f2/f3/page1.html', namelist)
+        self.assertIn('f2/file1.txt', namelist)
+
+        stream = zipper.read('f1/image1.jpg')
+        self.assertEqual(stream, load_image('canoneye.jpg').data)
+
+        stream = zipper.read('f2/f3/page1.html')
+        self.assertEqual(stream, PAGE_TEXT)
+
+        stream = zipper.read('f2/file1.txt')
+        self.assertEqual(stream, load_file('file.txt').data)
+
+    def test_unzip(self):
+        view = self.portal.restrictedTraverse('unzip')
+
+        with open(os.path.join(PACKAGE_HOME, 'input', 'test.zip'), 'rb') as zipf:
+            data = zipf.read()
+        zipf = NamedBlobFile(data=data)
+        view.unzip(zipf)
+
+        page1 = self.cat(path='/plone/folder2/folder3/page1.html')[0].getObject()
+        self.assertEqual(page1.text.raw, PAGE_TEXT)
+        self.assertEqual(page1.title, 'page1.html')
+
+
+def test_suite():
+    import unittest
+    return unittest.defaultTestLoader.loadTestsFromName(__name__)
```

### Comparing `ims.zip-4.2.1/ims.zip.egg-info/SOURCES.txt` & `ims.zip-5.0/ims.zip.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 MANIFEST.in
-README.md
+README.txt
+pyproject.toml
 setup.cfg
-setup.py
 ims/__init__.py
 ims.zip.egg-info/PKG-INFO
 ims.zip.egg-info/SOURCES.txt
 ims.zip.egg-info/dependency_links.txt
 ims.zip.egg-info/entry_points.txt
-ims.zip.egg-info/namespace_packages.txt
-ims.zip.egg-info/not-zip-safe
 ims.zip.egg-info/requires.txt
 ims.zip.egg-info/top_level.txt
 ims/zip/__init__.py
 ims/zip/adapters.py
 ims/zip/configure.zcml
 ims/zip/interfaces.py
 ims/zip/permissions.py
 ims/zip/testing.py
-ims/zip/zipper.py
+ims/zip/upgrades.py
 ims/zip/browser/__init__.py
 ims/zip/browser/configure.zcml
 ims/zip/browser/unzipper.py
 ims/zip/browser/zipper.py
 ims/zip/browser/templates/unzipper.pt
 ims/zip/browser/templates/zipper.pt
 ims/zip/profiles/default/actions.xml
+ims/zip/profiles/default/metadata.xml
 ims/zip/profiles/default/registry.xml
 ims/zip/profiles/uninstall/actions.xml
 ims/zip/profiles/uninstall/registry.xml
+ims/zip/profiles/upgrade_1/actions.xml
 ims/zip/tests/__init__.py
 ims/zip/tests/base.py
 ims/zip/tests/test_uninstall.py
 ims/zip/tests/test_zip.py
 ims/zip/tests/input/canoneye.jpg
 ims/zip/tests/input/file.txt
 ims/zip/tests/input/page1.html
```

