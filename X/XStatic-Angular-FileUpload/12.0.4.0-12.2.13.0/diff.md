# Comparing `tmp/XStatic-Angular-FileUpload-12.0.4.0.tar.gz` & `tmp/XStatic-Angular-FileUpload-12.2.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/XStatic-Angular-FileUpload-12.0.4.0.tar", last modified: Tue May 17 13:33:14 2016, max compression
+gzip compressed data, was "XStatic-Angular-FileUpload-12.2.13.0.tar", last modified: Thu Aug  3 12:50:01 2023, max compression
```

## Comparing `XStatic-Angular-FileUpload-12.0.4.0.tar` & `XStatic-Angular-FileUpload-12.2.13.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 robcresswell   (501) staff       (20)        0 2016-05-17 13:33:14.000000 XStatic-Angular-FileUpload-12.0.4.0/
--rw-r--r--   0 robcresswell   (501) staff       (20)      157 2016-05-13 10:56:33.000000 XStatic-Angular-FileUpload-12.0.4.0/MANIFEST.in
--rw-r--r--   0 robcresswell   (501) staff       (20)      964 2016-05-17 13:33:14.000000 XStatic-Angular-FileUpload-12.0.4.0/PKG-INFO
--rw-r--r--   0 robcresswell   (501) staff       (20)      493 2016-05-13 10:56:33.000000 XStatic-Angular-FileUpload-12.0.4.0/README.txt
--rw-r--r--   0 robcresswell   (501) staff       (20)       59 2016-05-17 13:33:14.000000 XStatic-Angular-FileUpload-12.0.4.0/setup.cfg
--rw-r--r--   0 robcresswell   (501) staff       (20)      844 2016-05-13 10:56:33.000000 XStatic-Angular-FileUpload-12.0.4.0/setup.py
-drwxr-xr-x   0 robcresswell   (501) staff       (20)        0 2016-05-17 13:33:14.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/
--rw-r--r--   0 robcresswell   (501) staff       (20)       56 2016-05-13 10:56:33.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/__init__.py
-drwxr-xr-x   0 robcresswell   (501) staff       (20)        0 2016-05-17 13:33:14.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/
--rw-r--r--   0 robcresswell   (501) staff       (20)       56 2016-05-13 10:56:33.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/__init__.py
-drwxr-xr-x   0 robcresswell   (501) staff       (20)        0 2016-05-17 13:33:14.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/
--rw-r--r--   0 robcresswell   (501) staff       (20)     1858 2016-05-17 13:31:17.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/__init__.py
-drwxr-xr-x   0 robcresswell   (501) staff       (20)        0 2016-05-17 13:33:14.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/
--rw-r--r--   0 robcresswell   (501) staff       (20)    71214 2016-05-17 13:31:17.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/FileAPI.flash.swf
--rw-r--r--   0 robcresswell   (501) staff       (20)   104332 2016-05-17 13:31:17.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/FileAPI.js
--rw-r--r--   0 robcresswell   (501) staff       (20)    44031 2016-05-17 13:31:17.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/FileAPI.min.js
--rw-r--r--   0 robcresswell   (501) staff       (20)    92827 2016-05-17 13:31:17.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-all.js
--rw-r--r--   0 robcresswell   (501) staff       (20)    43738 2016-05-17 13:31:17.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-all.min.js
--rw-r--r--   0 robcresswell   (501) staff       (20)    14393 2016-05-17 13:31:17.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-shim.js
--rw-r--r--   0 robcresswell   (501) staff       (20)     7261 2016-05-17 13:31:17.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-shim.min.js
--rw-r--r--   0 robcresswell   (501) staff       (20)    78433 2016-05-17 13:31:17.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/ng-file-upload.js
--rw-r--r--   0 robcresswell   (501) staff       (20)    36489 2016-05-17 13:31:17.000000 XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/ng-file-upload.min.js
-drwxr-xr-x   0 robcresswell   (501) staff       (20)        0 2016-05-17 13:33:14.000000 XStatic-Angular-FileUpload-12.0.4.0/XStatic_Angular_FileUpload.egg-info/
--rw-r--r--   0 robcresswell   (501) staff       (20)        1 2016-05-17 13:33:14.000000 XStatic-Angular-FileUpload-12.0.4.0/XStatic_Angular_FileUpload.egg-info/dependency_links.txt
--rw-r--r--   0 robcresswell   (501) staff       (20)       20 2016-05-17 13:33:14.000000 XStatic-Angular-FileUpload-12.0.4.0/XStatic_Angular_FileUpload.egg-info/namespace_packages.txt
--rw-r--r--   0 robcresswell   (501) staff       (20)        1 2016-05-17 13:33:14.000000 XStatic-Angular-FileUpload-12.0.4.0/XStatic_Angular_FileUpload.egg-info/not-zip-safe
--rw-r--r--   0 robcresswell   (501) staff       (20)      964 2016-05-17 13:33:14.000000 XStatic-Angular-FileUpload-12.0.4.0/XStatic_Angular_FileUpload.egg-info/PKG-INFO
--rw-r--r--   0 robcresswell   (501) staff       (20)      932 2016-05-17 13:33:14.000000 XStatic-Angular-FileUpload-12.0.4.0/XStatic_Angular_FileUpload.egg-info/SOURCES.txt
--rw-r--r--   0 robcresswell   (501) staff       (20)        8 2016-05-17 13:33:14.000000 XStatic-Angular-FileUpload-12.0.4.0/XStatic_Angular_FileUpload.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:01.687422 XStatic-Angular-FileUpload-12.2.13.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      974 2023-08-03 12:50:01.687422 XStatic-Angular-FileUpload-12.2.13.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/README.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:01.683422 XStatic-Angular-FileUpload-12.2.13.0/XStatic_Angular_FileUpload.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      974 2023-08-03 12:50:01.000000 XStatic-Angular-FileUpload-12.2.13.0/XStatic_Angular_FileUpload.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2023-08-03 12:50:01.000000 XStatic-Angular-FileUpload-12.2.13.0/XStatic_Angular_FileUpload.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-08-03 12:50:01.000000 XStatic-Angular-FileUpload-12.2.13.0/XStatic_Angular_FileUpload.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2023-08-03 12:50:01.000000 XStatic-Angular-FileUpload-12.2.13.0/XStatic_Angular_FileUpload.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-08-03 12:50:01.000000 XStatic-Angular-FileUpload-12.2.13.0/XStatic_Angular_FileUpload.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2023-08-03 12:50:01.000000 XStatic-Angular-FileUpload-12.2.13.0/XStatic_Angular_FileUpload.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2023-08-03 12:50:01.687422 XStatic-Angular-FileUpload-12.2.13.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      750 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:01.683422 XStatic-Angular-FileUpload-12.2.13.0/xstatic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/xstatic/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:01.683422 XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:01.683422 XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1859 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-08-03 12:50:01.687422 XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    71214 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/FileAPI.flash.swf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   104332 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/FileAPI.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44032 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/FileAPI.min.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    96078 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-all.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44742 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-all.min.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14394 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-shim.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7262 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-shim.min.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    81683 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/ng-file-upload.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37495 2023-08-03 12:49:37.000000 XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/ng-file-upload.min.js
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `XStatic-Angular-FileUpload-12.0.4.0/PKG-INFO` & `XStatic-Angular-FileUpload-12.2.13.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 1.0
+Metadata-Version: 1.2
 Name: XStatic-Angular-FileUpload
-Version: 12.0.4.0
-Summary: Angular-FileUpload 12.0.4 (XStatic packaging standard)
+Version: 12.2.13.0
+Summary: Angular-FileUpload 12.2.13 (XStatic packaging standard)
 Home-page: https://github.com/danialfarid/angular-file-upload
-Author: Rob Cresswell
-Author-email: robert.cresswell@outlook.com
+Maintainer: Radomir Dopieralski
+Maintainer-email: openstack@sheep.art.pl
 License: (same as Angular-FileUpload)
 Description: XStatic-Angular-Filepload
         -------------------------
         
         Angular-FileUpload JavaScript library packaged for setuptools (easy_install) / pip.
         
         This package is intended to be used by **any** project that needs these files.
```

### Comparing `XStatic-Angular-FileUpload-12.0.4.0/setup.py` & `XStatic-Angular-FileUpload-12.2.13.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,25 @@
+from setuptools import setup, find_packages
 from xstatic.pkg import angular_fileupload as xs
 
 # The README.txt file should be written in reST so that PyPI can use
 # it to generate your project's PyPI page.
 long_description = open('README.txt').read()
 
-from setuptools import setup, find_packages
-
 setup(
     name=xs.PACKAGE_NAME,
     version=xs.PACKAGE_VERSION,
     description=xs.DESCRIPTION,
     long_description=long_description,
     classifiers=xs.CLASSIFIERS,
     keywords=xs.KEYWORDS,
     maintainer=xs.MAINTAINER,
     maintainer_email=xs.MAINTAINER_EMAIL,
     license=xs.LICENSE,
     url=xs.HOMEPAGE,
     platforms=xs.PLATFORMS,
     packages=find_packages(),
-    namespace_packages=['xstatic', 'xstatic.pkg', ],
+    namespace_packages=['xstatic', 'xstatic.pkg'],
     include_package_data=True,
     zip_safe=False,
-    install_requires=[],  # nothing! :)
-                          # if you like, you MAY use the 'XStatic' package.
+    install_requires=[],
 )
```

### Comparing `XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/__init__.py` & `XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 DISPLAY_NAME = 'Angular-FileUpload' # official name, upper/lowercase allowed, no spaces
 PACKAGE_NAME = 'XStatic-%s' % DISPLAY_NAME # name used for PyPi
 
 NAME = __name__.split('.')[-1] # package name (e.g. 'foo' or 'foo_bar')
                                # please use a all-lowercase valid python
                                # package name
 
-VERSION = '12.0.4' # version of the packaged files, please use the upstream
+VERSION = '12.2.13' # version of the packaged files, please use the upstream
                   # version number
 BUILD = '0' # our package build number, so we can release new builds
              # with fixes for xstatic stuff.
 PACKAGE_VERSION = VERSION + '.' + BUILD # version used for PyPi
 
 DESCRIPTION = "%s %s (XStatic packaging standard)" % (DISPLAY_NAME, VERSION)
 
 PLATFORMS = 'any'
 CLASSIFIERS = []
 KEYWORDS = '%s xstatic' % NAME
 
 # XStatic-* package maintainer:
-MAINTAINER = 'Rob Cresswell'
-MAINTAINER_EMAIL = 'robert.cresswell@outlook.com'
+MAINTAINER = 'Radomir Dopieralski'
+MAINTAINER_EMAIL = 'openstack@sheep.art.pl'
 
 # this refers to the project homepage of the stuff we packaged:
 HOMEPAGE = 'https://github.com/danialfarid/angular-file-upload'
 
 # this refers to all files:
 LICENSE = '(same as %s)' % DISPLAY_NAME
```

### Comparing `XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/FileAPI.flash.swf` & `XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/FileAPI.flash.swf`

 * *Files identical despite different names*

### Comparing `XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/FileAPI.js` & `XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/FileAPI.js`

 * *Files identical despite different names*

### Comparing `XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/FileAPI.min.js` & `XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/FileAPI.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! 12.0.4 */
+/*! 12.2.13 */
 /*! FileAPI 2.0.7 - BSD | git://github.com/mailru/FileAPI.git
  * FileAPI — a set of  javascript tools for working with files. Multiupload, drag'n'drop and chunked file upload. Images: crop, resize and auto orientation by EXIF.
  */
 ! function(a) {
     "use strict";
     var b = a.HTMLCanvasElement && a.HTMLCanvasElement.prototype,
         c = a.Blob && function() {
```

### Comparing `XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-all.js` & `XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-all.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 /**!
- * AngularJS file upload directives and services. Supoorts: file upload/drop/paste, resume, cancel/abort,
+ * AngularJS file upload directives and services. Supports: file upload/drop/paste, resume, cancel/abort,
  * progress, resize, thumbnail, preview, validation and CORS
  * FileAPI Flash shim for old browsers not supporting FormData
  * @author  Danial  <danial.farid@gmail.com>
- * @version 12.0.4
+ * @version 12.2.13
  */
 
 (function() {
     /** @namespace FileAPI.noContentTimeout */
 
     function patchXHR(fnName, newFn) {
         window.XMLHttpRequest.prototype[fnName] = newFn(window.XMLHttpRequest.prototype[fnName]);
@@ -434,15 +434,15 @@
     };
 }
 
 /**!
  * AngularJS file upload directives and services. Supoorts: file upload/drop/paste, resume, cancel/abort,
  * progress, resize, thumbnail, preview, validation and CORS
  * @author  Danial  <danial.farid@gmail.com>
- * @version 12.0.4
+ * @version 12.2.13
  */
 
 if (window.XMLHttpRequest && !(window.FileAPI && FileAPI.shouldLoad)) {
     window.XMLHttpRequest.prototype.setRequestHeader = (function(orig) {
         return function(header, value) {
             if (header === '__setXHR_') {
                 var val = value(this);
@@ -455,15 +455,15 @@
             }
         };
     })(window.XMLHttpRequest.prototype.setRequestHeader);
 }
 
 var ngFileUpload = angular.module('ngFileUpload', []);
 
-ngFileUpload.version = '12.0.4';
+ngFileUpload.version = '12.2.13';
 
 ngFileUpload.service('UploadBase', ['$http', '$q', '$timeout', function($http, $q, $timeout) {
         var upload = this;
         upload.promisesCount = 0;
 
         this.isResumeSupported = function() {
             return window.Blob && window.Blob.prototype.slice;
@@ -524,17 +524,18 @@
                     };
                 };
             }
 
             function uploadWithAngular() {
                 $http(config).then(function(r) {
                     if (resumeSupported && config._chunkSize && !config._finished && config._file) {
+                        var fileSize = config._file && config._file.size || 0;
                         notifyProgress({
-                            loaded: config._end,
-                            total: config._file && config._file.size,
+                            loaded: Math.min(config._end, fileSize),
+                            total: fileSize,
                             config: config,
                             type: 'progress'
                         });
                         upload.upload(config, true);
                     } else {
                         if (config._finished) delete config._finished;
                         deferred.resolve(r);
@@ -565,14 +566,17 @@
                     uploadWithAngular();
                 }, function(e) {
                     throw e;
                 });
             } else if (config.resumeSize) {
                 config.resumeSize().then(function(size) {
                     config._start = size;
+                    if (config._chunkSize) {
+                        config._end = config._start + config._chunkSize;
+                    }
                     uploadWithAngular();
                 }, function(e) {
                     throw e;
                 });
             } else {
                 if (config._chunkSize) {
                     config._start = 0;
@@ -618,17 +622,19 @@
                         fn.apply(promise, arguments);
                     };
                 })(config.xhrFn);
                 return promise;
             };
 
             upload.promisesCount++;
-            promise['finally'](function() {
-                upload.promisesCount--;
-            });
+            if (promise['finally'] && promise['finally'] instanceof Function) {
+                promise['finally'](function() {
+                    upload.promisesCount--;
+                });
+            }
             return promise;
         }
 
         this.isUploadInProgress = function() {
             return upload.promisesCount > 0;
         };
 
@@ -813,17 +819,19 @@
                 responseType: 'arraybuffer'
             }).then(function(resp) {
                 var arrayBufferView = new Uint8Array(resp.data);
                 var type = resp.headers('content-type') || 'image/WebP';
                 var blob = new window.Blob([arrayBufferView], {
                     type: type
                 });
+                var matches = url.match(/.*\/(.+?)(\?.*)?$/);
+                if (matches.length > 1) {
+                    blob.name = matches[1];
+                }
                 defer.resolve(blob);
-                //var split = type.split('[/;]');
-                //blob.name = url.substring(0, 150).replace(/\W+/g, '') + '.' + (split.length > 1 ? split[1] : 'jpg');
             }, function(e) {
                 defer.reject(e);
             });
             return defer.promise;
         };
 
         this.setDefaults = function(defaults) {
@@ -863,15 +871,15 @@
             }
         } else {
             return attrVal;
         }
     };
 
     upload.shouldUpdateOn = function(type, attr, scope) {
-        var modelOptions = upload.attrGetter('ngModelOptions', attr, scope);
+        var modelOptions = upload.attrGetter('ngfModelOptions', attr, scope);
         if (modelOptions && modelOptions.updateOn) {
             return modelOptions.updateOn.split(' ').indexOf(type) > -1;
         }
         return true;
     };
 
     upload.emptyPromise = function() {
@@ -915,54 +923,59 @@
                     files.splice(i, 1, fixedFile);
                 }));
             }
         });
         return $q.all(promises);
     }
 
-    function resize(files, attr, scope) {
+    function resizeFile(files, attr, scope, ngModel) {
         var resizeVal = upload.attrGetter('ngfResize', attr, scope);
         if (!resizeVal || !upload.isResizeSupported() || !files.length) return upload.emptyPromise();
         if (resizeVal instanceof Function) {
             var defer = $q.defer();
-            resizeVal(files).then(function(p) {
-                resizeWithParams(p, files, attr, scope).then(function(r) {
+            return resizeVal(files).then(function(p) {
+                resizeWithParams(p, files, attr, scope, ngModel).then(function(r) {
                     defer.resolve(r);
                 }, function(e) {
                     defer.reject(e);
                 });
             }, function(e) {
                 defer.reject(e);
             });
         } else {
-            return resizeWithParams(resizeVal, files, attr, scope);
+            return resizeWithParams(resizeVal, files, attr, scope, ngModel);
         }
     }
 
-    function resizeWithParams(param, files, attr, scope) {
+    function resizeWithParams(params, files, attr, scope, ngModel) {
         var promises = [upload.emptyPromise()];
 
         function handleFile(f, i) {
             if (f.type.indexOf('image') === 0) {
-                if (param.pattern && !upload.validatePattern(f, param.pattern)) return;
-                var promise = upload.resize(f, param.width, param.height, param.quality,
-                    param.type, param.ratio, param.centerCrop,
-                    function(width, height) {
-                        return upload.attrGetter('ngfResizeIf', attr, scope, {
-                            $width: width,
-                            $height: height,
-                            $file: f
-                        });
-                    }, param.restoreExif !== false);
+                if (params.pattern && !upload.validatePattern(f, params.pattern)) return;
+                params.resizeIf = function(width, height) {
+                    return upload.attrGetter('ngfResizeIf', attr, scope, {
+                        $width: width,
+                        $height: height,
+                        $file: f
+                    });
+                };
+                var promise = upload.resize(f, params);
                 promises.push(promise);
                 promise.then(function(resizedFile) {
                     files.splice(i, 1, resizedFile);
                 }, function(e) {
                     f.$error = 'resize';
+                    (f.$errorMessages = (f.$errorMessages || {})).resize = true;
                     f.$errorParam = (e ? (e.message ? e.message : e) + ': ' : '') + (f && f.name);
+                    ngModel.$ngfValidations.push({
+                        name: 'resize',
+                        valid: false
+                    });
+                    upload.applyModelValidation(ngModel, files);
                 });
             }
         }
 
         for (var i = 0; i < files.length; i++) {
             handleFile(files[i], i);
         }
@@ -1043,46 +1056,47 @@
             }
         }
 
         function toArray(v) {
             return angular.isArray(v) ? v : [v];
         }
 
-        function separateInvalids() {
-            valids = [];
-            invalids = [];
-            angular.forEach(allNewFiles, function(file) {
-                if (file.$error) {
-                    invalids.push(file);
-                } else {
-                    valids.push(file);
-                }
-            });
-        }
-
         function resizeAndUpdate() {
             function updateModel() {
                 $timeout(function() {
                     update(keep ? prevValidFiles.concat(valids) : valids,
                         keep ? prevInvalidFiles.concat(invalids) : invalids,
                         files, dupFiles, isSingleModel);
                 }, options && options.debounce ? options.debounce.change || options.debounce : 0);
             }
 
-            resize(validateAfterResize ? allNewFiles : valids, attr, scope).then(function() {
+            var resizingFiles = validateAfterResize ? allNewFiles : valids;
+            resizeFile(resizingFiles, attr, scope, ngModel).then(function() {
                 if (validateAfterResize) {
-                    upload.validate(allNewFiles, prevValidFiles.length, ngModel, attr, scope).then(function() {
-                        separateInvalids();
-                        updateModel();
-                    });
+                    upload.validate(allNewFiles, keep ? prevValidFiles.length : 0, ngModel, attr, scope)
+                        .then(function(validationResult) {
+                            valids = validationResult.validsFiles;
+                            invalids = validationResult.invalidsFiles;
+                            updateModel();
+                        });
                 } else {
                     updateModel();
                 }
-            }, function(e) {
-                throw 'Could not resize files ' + e;
+            }, function() {
+                for (var i = 0; i < resizingFiles.length; i++) {
+                    var f = resizingFiles[i];
+                    if (f.$error === 'resize') {
+                        var index = valids.indexOf(f);
+                        if (index > -1) {
+                            valids.splice(index, 1);
+                            invalids.push(f);
+                        }
+                        updateModel();
+                    }
+                }
             });
         }
 
         prevValidFiles = attr.$$ngfPrevValidFiles || [];
         prevInvalidFiles = attr.$$ngfPrevInvalidFiles || [];
         if (ngModel && ngModel.$modelValue) {
             prevValidFiles = toArray(ngModel.$modelValue);
@@ -1104,33 +1118,35 @@
             $newFiles: allNewFiles,
             $duplicateFiles: dupFiles,
             $event: evt
         });
 
         var validateAfterResize = upload.attrGetter('ngfValidateAfterResize', attr, scope);
 
-        var options = upload.attrGetter('ngModelOptions', attr, scope);
-        upload.validate(allNewFiles, prevValidFiles.length, ngModel, attr, scope).then(function() {
-            if (noDelay) {
-                update(allNewFiles, [], files, dupFiles, isSingleModel);
-            } else {
-                if ((!options || !options.allowInvalid) && !validateAfterResize) {
-                    separateInvalids();
+        var options = upload.attrGetter('ngfModelOptions', attr, scope);
+        upload.validate(allNewFiles, keep ? prevValidFiles.length : 0, ngModel, attr, scope)
+            .then(function(validationResult) {
+                if (noDelay) {
+                    update(allNewFiles, [], files, dupFiles, isSingleModel);
                 } else {
-                    valids = allNewFiles;
-                }
-                if (upload.attrGetter('ngfFixOrientation', attr, scope) && upload.isExifSupported()) {
-                    applyExifRotations(valids, attr, scope).then(function() {
+                    if ((!options || !options.allowInvalid) && !validateAfterResize) {
+                        valids = validationResult.validFiles;
+                        invalids = validationResult.invalidFiles;
+                    } else {
+                        valids = allNewFiles;
+                    }
+                    if (upload.attrGetter('ngfFixOrientation', attr, scope) && upload.isExifSupported()) {
+                        applyExifRotations(valids, attr, scope).then(function() {
+                            resizeAndUpdate();
+                        });
+                    } else {
                         resizeAndUpdate();
-                    });
-                } else {
-                    resizeAndUpdate();
+                    }
                 }
-            }
-        });
+            });
     };
 
     return upload;
 }]);
 
 ngFileUpload.directive('ngfSelect', ['$parse', '$timeout', '$compile', 'Upload', function($parse, $timeout, $compile, Upload) {
     var generatedElems = [];
@@ -1147,15 +1163,15 @@
         return ua.indexOf('Chrome') === -1 && /.*Windows.*Safari.*/.test(ua);
     }
 
     function linkFileSelect(scope, elem, attr, ngModel, $parse, $timeout, $compile, upload) {
         /** @namespace attr.ngfSelect */
         /** @namespace attr.ngfChange */
         /** @namespace attr.ngModel */
-        /** @namespace attr.ngModelOptions */
+        /** @namespace attr.ngfModelOptions */
         /** @namespace attr.ngfMultiple */
         /** @namespace attr.ngfCapture */
         /** @namespace attr.ngfValidate */
         /** @namespace attr.ngfKeep */
         var attrGetter = function(name, scope) {
             return upload.attrGetter(name, attr, scope);
         };
@@ -1168,86 +1184,95 @@
             return attrGetter('ngfChange') || attrGetter('ngfSelect');
         }
 
         function changeFn(evt) {
             if (upload.shouldUpdateOn('change', attr, scope)) {
                 var fileList = evt.__files_ || (evt.target && evt.target.files),
                     files = [];
+                /* Handle duplicate call in  IE11 */
+                if (!fileList) return;
                 for (var i = 0; i < fileList.length; i++) {
                     files.push(fileList[i]);
                 }
                 upload.updateModel(ngModel, attr, scope, fileChangeAttr(),
                     files.length ? files : null, evt);
             }
         }
 
         upload.registerModelChangeValidator(ngModel, attr, scope);
 
         var unwatches = [];
-        unwatches.push(scope.$watch(attrGetter('ngfMultiple'), function() {
-            fileElem.attr('multiple', attrGetter('ngfMultiple', scope));
-        }));
-        unwatches.push(scope.$watch(attrGetter('ngfCapture'), function() {
-            fileElem.attr('capture', attrGetter('ngfCapture', scope));
-        }));
-        unwatches.push(scope.$watch(attrGetter('ngfAccept'), function() {
-            fileElem.attr('accept', attrGetter('ngfAccept', scope));
-        }));
-        attr.$observe('accept', function() {
+        if (attrGetter('ngfMultiple')) {
+            unwatches.push(scope.$watch(attrGetter('ngfMultiple'), function() {
+                fileElem.attr('multiple', attrGetter('ngfMultiple', scope));
+            }));
+        }
+        if (attrGetter('ngfCapture')) {
+            unwatches.push(scope.$watch(attrGetter('ngfCapture'), function() {
+                fileElem.attr('capture', attrGetter('ngfCapture', scope));
+            }));
+        }
+        if (attrGetter('ngfAccept')) {
+            unwatches.push(scope.$watch(attrGetter('ngfAccept'), function() {
+                fileElem.attr('accept', attrGetter('ngfAccept', scope));
+            }));
+        }
+        unwatches.push(attr.$observe('accept', function() {
             fileElem.attr('accept', attrGetter('accept'));
-        });
-        unwatches.push(function() {
-            if (attr.$$observers) delete attr.$$observers.accept;
-        });
+        }));
 
-        function bindAttrToFileInput(fileElem) {
-            if (elem !== fileElem) {
-                for (var i = 0; i < elem[0].attributes.length; i++) {
-                    var attribute = elem[0].attributes[i];
-                    if (attribute.name !== 'type' && attribute.name !== 'class' && attribute.name !== 'style') {
-                        if (attribute.value == null || attribute.value === '') {
-                            if (attribute.name === 'required') attribute.value = 'required';
-                            if (attribute.name === 'multiple') attribute.value = 'multiple';
-                        }
-                        fileElem.attr(attribute.name, attribute.name === 'id' ? 'ngf-' + attribute.value : attribute.value);
+        function bindAttrToFileInput(fileElem, label) {
+            function updateId(val) {
+                fileElem.attr('id', 'ngf-' + val);
+                label.attr('id', 'ngf-label-' + val);
+            }
+
+            for (var i = 0; i < elem[0].attributes.length; i++) {
+                var attribute = elem[0].attributes[i];
+                if (attribute.name !== 'type' && attribute.name !== 'class' && attribute.name !== 'style') {
+                    if (attribute.name === 'id') {
+                        updateId(attribute.value);
+                        unwatches.push(attr.$observe('id', updateId));
+                    } else {
+                        fileElem.attr(attribute.name, (!attribute.value && (attribute.name === 'required' ||
+                            attribute.name === 'multiple')) ? attribute.name : attribute.value);
                     }
                 }
             }
         }
 
         function createFileInput() {
             if (isInputTypeFile()) {
                 return elem;
             }
 
             var fileElem = angular.element('<input type="file">');
 
-            bindAttrToFileInput(fileElem);
-
             var label = angular.element('<label>upload</label>');
             label.css('visibility', 'hidden').css('position', 'absolute').css('overflow', 'hidden')
                 .css('width', '0px').css('height', '0px').css('border', 'none')
                 .css('margin', '0px').css('padding', '0px').attr('tabindex', '-1');
+            bindAttrToFileInput(fileElem, label);
+
             generatedElems.push({
                 el: elem,
                 ref: label
             });
 
             document.body.appendChild(label.append(fileElem)[0]);
 
             return fileElem;
         }
 
-        var initialTouchStartY = 0;
-
         function clickHandler(evt) {
             if (elem.attr('disabled')) return false;
             if (attrGetter('ngfSelectDisabled', scope)) return;
 
-            var r = handleTouch(evt);
+            var r = detectSwipe(evt);
+            // prevent the click if it is a swipe
             if (r != null) return r;
 
             resetModel(evt);
 
             // fix for md when the element is removed from the DOM and added back #460
             try {
                 if (!isInputTypeFile() && !document.body.contains(fileElem[0])) {
@@ -1268,27 +1293,38 @@
             } else {
                 fileElem[0].click();
             }
 
             return false;
         }
 
-        function handleTouch(evt) {
-            var touches = evt.changedTouches || (evt.originalEvent && evt.originalEvent.changedTouches);
-            if (evt.type === 'touchstart') {
-                initialTouchStartY = touches ? touches[0].clientY : 0;
-                return true; // don't block event default
-            } else {
-                evt.stopPropagation();
-                evt.preventDefault();
 
-                // prevent scroll from triggering event
-                if (evt.type === 'touchend') {
-                    var currentLocation = touches ? touches[0].clientY : 0;
-                    if (Math.abs(currentLocation - initialTouchStartY) > 20) return false;
+        var initialTouchStartY = 0;
+        var initialTouchStartX = 0;
+
+        function detectSwipe(evt) {
+            var touches = evt.changedTouches || (evt.originalEvent && evt.originalEvent.changedTouches);
+            if (touches) {
+                if (evt.type === 'touchstart') {
+                    initialTouchStartX = touches[0].clientX;
+                    initialTouchStartY = touches[0].clientY;
+                    return true; // don't block event default
+                } else {
+                    // prevent scroll from triggering event
+                    if (evt.type === 'touchend') {
+                        var currentX = touches[0].clientX;
+                        var currentY = touches[0].clientY;
+                        if ((Math.abs(currentX - initialTouchStartX) > 20) ||
+                            (Math.abs(currentY - initialTouchStartY) > 20)) {
+                            evt.stopPropagation();
+                            evt.preventDefault();
+                            return false;
+                        }
+                    }
+                    return true;
                 }
             }
         }
 
         var fileElem = elem;
 
         function resetModel(evt) {
@@ -1516,39 +1552,48 @@
 
         $timeout(function() {
             var unwatch = scope.$watch(attr[directiveName], function(file) {
                 var size = resizeParams;
                 if (directiveName === 'ngfThumbnail') {
                     if (!size) {
                         size = {
-                            width: elem[0].clientWidth,
-                            height: elem[0].clientHeight
+                            width: elem[0].naturalWidth || elem[0].clientWidth,
+                            height: elem[0].naturalHeight || elem[0].clientHeight
                         };
                     }
                     if (size.width === 0 && window.getComputedStyle) {
                         var style = getComputedStyle(elem[0]);
-                        size = {
-                            width: parseInt(style.width.slice(0, -2)),
-                            height: parseInt(style.height.slice(0, -2))
-                        };
+                        if (style.width && style.width.indexOf('px') > -1 && style.height && style.height.indexOf('px') > -1) {
+                            size = {
+                                width: parseInt(style.width.slice(0, -2)),
+                                height: parseInt(style.height.slice(0, -2))
+                            };
+                        }
                     }
                 }
 
                 if (angular.isString(file)) {
                     elem.removeClass('ng-hide');
                     if (isBackground) {
                         return elem.css('background-image', 'url(\'' + file + '\')');
                     } else {
                         return elem.attr('src', file);
                     }
                 }
                 if (file && file.type && file.type.search(getTagType(elem[0])) === 0 &&
                     (!isBackground || file.type.indexOf('image') === 0)) {
                     if (size && Upload.isResizeSupported()) {
-                        Upload.resize(file, size.width, size.height, size.quality).then(
+                        size.resizeIf = function(width, height) {
+                            return Upload.attrGetter('ngfResizeIf', attr, scope, {
+                                $width: width,
+                                $height: height,
+                                $file: file
+                            });
+                        };
+                        Upload.resize(file, size).then(
                             function(f) {
                                 constructDataUrl(f);
                             },
                             function(e) {
                                 throw e;
                             }
                         );
@@ -1603,16 +1648,16 @@
                 linkFileDirective(Upload, $timeout, scope, elem, attr, 'ngfThumbnail', size,
                     Upload.attrGetter('ngfAsBackground', attr, scope));
             }
         };
     }]);
 
     ngFileUpload.config(['$compileProvider', function($compileProvider) {
-        if ($compileProvider.imgSrcSanitizationWhitelist) $compileProvider.imgSrcSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|local|file|data|blob):/);
-        if ($compileProvider.aHrefSanitizationWhitelist) $compileProvider.aHrefSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|local|file|data|blob):/);
+        if ($compileProvider.imgSrcSanitizationWhitelist) $compileProvider.imgSrcSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|webcal|local|file|data|blob):/);
+        if ($compileProvider.aHrefSanitizationWhitelist) $compileProvider.aHrefSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|webcal|local|file|data|blob):/);
     }]);
 
     ngFileUpload.filter('ngfDataUrl', ['UploadDataUrl', '$sce', function(UploadDataUrl, $sce) {
         return function(file, disallowObjectUrl, trustedUrl) {
             if (angular.isString(file)) {
                 return $sce.trustAsResourceUrl(file);
             }
@@ -1702,21 +1747,23 @@
         return r;
     };
 
     upload.registerModelChangeValidator = function(ngModel, attr, scope) {
         if (ngModel) {
             ngModel.$formatters.push(function(files) {
                 if (ngModel.$dirty) {
+                    var filesArray = files;
                     if (files && !angular.isArray(files)) {
-                        files = [files];
+                        filesArray = [files];
                     }
-                    upload.validate(files, 0, ngModel, attr, scope).then(function() {
-                        upload.applyModelValidation(ngModel, files);
+                    upload.validate(filesArray, 0, ngModel, attr, scope).then(function() {
+                        upload.applyModelValidation(ngModel, filesArray);
                     });
                 }
+                return files;
             });
         }
     };
 
     function markModelAsDirty(ngModel, files) {
         if (files != null && !ngModel.$dirty) {
             if (ngModel.$setDirty) {
@@ -1762,51 +1809,64 @@
             v.valid = true;
         });
 
         var attrGetter = function(name, params) {
             return upload.attrGetter(name, attr, scope, params);
         };
 
+        var ignoredErrors = (upload.attrGetter('ngfIgnoreInvalid', attr, scope) || '').split(' ');
+        var runAllValidation = upload.attrGetter('ngfRunAllValidations', attr, scope);
+
         if (files == null || files.length === 0) {
-            return upload.emptyPromise(ngModel);
+            return upload.emptyPromise({
+                'validFiles': files,
+                'invalidFiles': []
+            });
         }
 
         files = files.length === undefined ? [files] : files.slice(0);
+        var invalidFiles = [];
 
         function validateSync(name, validationName, fn) {
             if (files) {
                 var i = files.length,
                     valid = null;
                 while (i--) {
                     var file = files[i];
                     if (file) {
                         var val = upload.getValidationAttr(attr, scope, name, validationName, file);
                         if (val != null) {
                             if (!fn(file, val, i)) {
-                                file.$error = name;
-                                (file.$errorMessages = (file.$errorMessages || {}))[name] = true;
-                                file.$errorParam = val;
-                                files.splice(i, 1);
-                                valid = false;
+                                if (ignoredErrors.indexOf(name) === -1) {
+                                    file.$error = name;
+                                    (file.$errorMessages = (file.$errorMessages || {}))[name] = true;
+                                    file.$errorParam = val;
+                                    if (invalidFiles.indexOf(file) === -1) {
+                                        invalidFiles.push(file);
+                                    }
+                                    if (!runAllValidation) {
+                                        files.splice(i, 1);
+                                    }
+                                    valid = false;
+                                } else {
+                                    files.splice(i, 1);
+                                }
                             }
                         }
                     }
                 }
                 if (valid !== null) {
                     ngModel.$ngfValidations.push({
                         name: name,
                         valid: valid
                     });
                 }
             }
         }
 
-        validateSync('maxFiles', null, function(file, val, i) {
-            return prevLength + i < val;
-        });
         validateSync('pattern', null, upload.validatePattern);
         validateSync('minSize', 'size.min', function(file, val) {
             return file.size + 0.1 >= upload.translateScalars(val);
         });
         validateSync('maxSize', 'size.max', function(file, val) {
             return file.size - 0.1 <= upload.translateScalars(val);
         });
@@ -1821,177 +1881,218 @@
         });
 
         validateSync('validateFn', null, function(file, r) {
             return r === true || r === null || r === '';
         });
 
         if (!files.length) {
-            return upload.emptyPromise(ngModel, ngModel.$ngfValidations);
+            return upload.emptyPromise({
+                'validFiles': [],
+                'invalidFiles': invalidFiles
+            });
         }
 
         function validateAsync(name, validationName, type, asyncFn, fn) {
             function resolveResult(defer, file, val) {
-                if (val != null) {
-                    asyncFn(file, val).then(function(d) {
-                        if (!fn(d, val)) {
+                function resolveInternal(fn) {
+                    if (fn()) {
+                        if (ignoredErrors.indexOf(name) === -1) {
                             file.$error = name;
                             (file.$errorMessages = (file.$errorMessages || {}))[name] = true;
                             file.$errorParam = val;
-                            defer.reject();
+                            if (invalidFiles.indexOf(file) === -1) {
+                                invalidFiles.push(file);
+                            }
+                            if (!runAllValidation) {
+                                var i = files.indexOf(file);
+                                if (i > -1) files.splice(i, 1);
+                            }
+                            defer.resolve(false);
                         } else {
-                            defer.resolve();
+                            var j = files.indexOf(file);
+                            if (j > -1) files.splice(j, 1);
+                            defer.resolve(true);
                         }
+                    } else {
+                        defer.resolve(true);
+                    }
+                }
+
+                if (val != null) {
+                    asyncFn(file, val).then(function(d) {
+                        resolveInternal(function() {
+                            return !fn(d, val);
+                        });
                     }, function() {
-                        if (attrGetter('ngfValidateForce', {
+                        resolveInternal(function() {
+                            return attrGetter('ngfValidateForce', {
                                 $file: file
-                            })) {
-                            file.$error = name;
-                            (file.$errorMessages = (file.$errorMessages || {}))[name] = true;
-                            file.$errorParam = val;
-                            defer.reject();
-                        } else {
-                            defer.resolve();
-                        }
+                            });
+                        });
                     });
                 } else {
-                    defer.resolve();
+                    defer.resolve(true);
                 }
             }
 
-            var promises = [upload.emptyPromise()];
+            var promises = [upload.emptyPromise(true)];
             if (files) {
                 files = files.length === undefined ? [files] : files;
                 angular.forEach(files, function(file) {
                     var defer = $q.defer();
                     promises.push(defer.promise);
                     if (type && (file.type == null || file.type.search(type) !== 0)) {
-                        defer.resolve();
+                        defer.resolve(true);
                         return;
                     }
                     if (name === 'dimensions' && upload.attrGetter('ngfDimensions', attr) != null) {
                         upload.imageDimensions(file).then(function(d) {
                             resolveResult(defer, file,
                                 attrGetter('ngfDimensions', {
                                     $file: file,
                                     $width: d.width,
                                     $height: d.height
                                 }));
                         }, function() {
-                            defer.reject();
+                            defer.resolve(false);
                         });
                     } else if (name === 'duration' && upload.attrGetter('ngfDuration', attr) != null) {
                         upload.mediaDuration(file).then(function(d) {
                             resolveResult(defer, file,
                                 attrGetter('ngfDuration', {
                                     $file: file,
                                     $duration: d
                                 }));
                         }, function() {
-                            defer.reject();
+                            defer.resolve(false);
                         });
                     } else {
                         resolveResult(defer, file,
                             upload.getValidationAttr(attr, scope, name, validationName, file));
                     }
                 });
-                return $q.all(promises).then(function() {
-                    ngModel.$ngfValidations.push({
-                        name: name,
-                        valid: true
-                    });
-                }, function() {
-                    ngModel.$ngfValidations.push({
-                        name: name,
-                        valid: false
-                    });
-                });
             }
+            var deffer = $q.defer();
+            $q.all(promises).then(function(values) {
+                var isValid = true;
+                for (var i = 0; i < values.length; i++) {
+                    if (!values[i]) {
+                        isValid = false;
+                        break;
+                    }
+                }
+                ngModel.$ngfValidations.push({
+                    name: name,
+                    valid: isValid
+                });
+                deffer.resolve(isValid);
+            });
+            return deffer.promise;
         }
 
         var deffer = $q.defer();
         var promises = [];
 
-        promises.push(upload.happyPromise(validateAsync('maxHeight', 'height.max', /image/,
+        promises.push(validateAsync('maxHeight', 'height.max', /image/,
             this.imageDimensions,
             function(d, val) {
                 return d.height <= val;
-            })));
-        promises.push(upload.happyPromise(validateAsync('minHeight', 'height.min', /image/,
+            }));
+        promises.push(validateAsync('minHeight', 'height.min', /image/,
             this.imageDimensions,
             function(d, val) {
                 return d.height >= val;
-            })));
-        promises.push(upload.happyPromise(validateAsync('maxWidth', 'width.max', /image/,
+            }));
+        promises.push(validateAsync('maxWidth', 'width.max', /image/,
             this.imageDimensions,
             function(d, val) {
                 return d.width <= val;
-            })));
-        promises.push(upload.happyPromise(validateAsync('minWidth', 'width.min', /image/,
+            }));
+        promises.push(validateAsync('minWidth', 'width.min', /image/,
             this.imageDimensions,
             function(d, val) {
                 return d.width >= val;
-            })));
-        promises.push(upload.happyPromise(validateAsync('dimensions', null, /image/,
+            }));
+        promises.push(validateAsync('dimensions', null, /image/,
             function(file, val) {
                 return upload.emptyPromise(val);
             },
             function(r) {
                 return r;
-            })));
-        promises.push(upload.happyPromise(validateAsync('ratio', null, /image/,
+            }));
+        promises.push(validateAsync('ratio', null, /image/,
             this.imageDimensions,
             function(d, val) {
                 var split = val.toString().split(','),
                     valid = false;
                 for (var i = 0; i < split.length; i++) {
-                    if (Math.abs((d.width / d.height) - upload.ratioToFloat(split[i])) < 0.0001) {
+                    if (Math.abs((d.width / d.height) - upload.ratioToFloat(split[i])) < 0.01) {
                         valid = true;
                     }
                 }
                 return valid;
-            })));
-        promises.push(upload.happyPromise(validateAsync('maxRatio', 'ratio.max', /image/,
+            }));
+        promises.push(validateAsync('maxRatio', 'ratio.max', /image/,
             this.imageDimensions,
             function(d, val) {
                 return (d.width / d.height) - upload.ratioToFloat(val) < 0.0001;
-            })));
-        promises.push(upload.happyPromise(validateAsync('minRatio', 'ratio.min', /image/,
+            }));
+        promises.push(validateAsync('minRatio', 'ratio.min', /image/,
             this.imageDimensions,
             function(d, val) {
                 return (d.width / d.height) - upload.ratioToFloat(val) > -0.0001;
-            })));
-        promises.push(upload.happyPromise(validateAsync('maxDuration', 'duration.max', /audio|video/,
+            }));
+        promises.push(validateAsync('maxDuration', 'duration.max', /audio|video/,
             this.mediaDuration,
             function(d, val) {
                 return d <= upload.translateScalars(val);
-            })));
-        promises.push(upload.happyPromise(validateAsync('minDuration', 'duration.min', /audio|video/,
+            }));
+        promises.push(validateAsync('minDuration', 'duration.min', /audio|video/,
             this.mediaDuration,
             function(d, val) {
                 return d >= upload.translateScalars(val);
-            })));
-        promises.push(upload.happyPromise(validateAsync('duration', null, /audio|video/,
+            }));
+        promises.push(validateAsync('duration', null, /audio|video/,
             function(file, val) {
                 return upload.emptyPromise(val);
             },
             function(r) {
                 return r;
-            })));
+            }));
 
-        promises.push(upload.happyPromise(validateAsync('validateAsyncFn', null, null,
+        promises.push(validateAsync('validateAsyncFn', null, null,
             function(file, val) {
                 return val;
             },
             function(r) {
                 return r === true || r === null || r === '';
-            })));
+            }));
+
+        $q.all(promises).then(function() {
 
-        return $q.all(promises).then(function() {
-            deffer.resolve(ngModel, ngModel.$ngfValidations);
+            if (runAllValidation) {
+                for (var i = 0; i < files.length; i++) {
+                    var file = files[i];
+                    if (file.$error) {
+                        files.splice(i--, 1);
+                    }
+                }
+            }
+
+            runAllValidation = false;
+            validateSync('maxFiles', null, function(file, val, i) {
+                return prevLength + i < val;
+            });
+
+            deffer.resolve({
+                'validFiles': files,
+                'invalidFiles': invalidFiles
+            });
         });
+        return deffer.promise;
     };
 
     upload.imageDimensions = function(file) {
         if (file.$ngfWidth && file.$ngfHeight) {
             var d = $q.defer();
             $timeout(function() {
                 d.resolve({
@@ -2011,16 +2112,16 @@
             }
             upload.dataUrl(file).then(function(dataUrl) {
                 var img = angular.element('<img>').attr('src', dataUrl)
                     .css('visibility', 'hidden').css('position', 'fixed')
                     .css('max-width', 'none !important').css('max-height', 'none !important');
 
                 function success() {
-                    var width = img[0].clientWidth;
-                    var height = img[0].clientHeight;
+                    var width = img[0].naturalWidth || img[0].clientWidth;
+                    var height = img[0].naturalHeight || img[0].clientHeight;
                     img.remove();
                     file.$ngfWidth = width;
                     file.$ngfHeight = height;
                     deferred.resolve({
                         width: width,
                         height: height
                     });
@@ -2029,31 +2130,32 @@
                 function error() {
                     img.remove();
                     deferred.reject('load error');
                 }
 
                 img.on('load', success);
                 img.on('error', error);
-                var count = 0;
 
-                function checkLoadError() {
+                var secondsCounter = 0;
+
+                function checkLoadErrorInCaseOfNoCallback() {
                     $timeout(function() {
                         if (img[0].parentNode) {
                             if (img[0].clientWidth) {
                                 success();
-                            } else if (count > 10) {
+                            } else if (secondsCounter++ > 10) {
                                 error();
                             } else {
-                                checkLoadError();
+                                checkLoadErrorInCaseOfNoCallback();
                             }
                         }
                     }, 1000);
                 }
 
-                checkLoadError();
+                checkLoadErrorInCaseOfNoCallback();
 
                 angular.element(document.getElementsByTagName('body')[0]).append(img);
             }, function() {
                 deferred.reject('load error');
             });
         });
 
@@ -2157,51 +2259,57 @@
     };
 
     // Extracted from https://github.com/romelgomez/angular-firebase-image-upload/blob/master/app/scripts/fileUpload.js#L89
     var resize = function(imagen, width, height, quality, type, ratio, centerCrop, resizeIf) {
         var deferred = $q.defer();
         var canvasElement = document.createElement('canvas');
         var imageElement = document.createElement('img');
+        imageElement.setAttribute('style', 'visibility:hidden;position:fixed;z-index:-100000');
+        document.body.appendChild(imageElement);
 
         imageElement.onload = function() {
-            if (resizeIf != null && resizeIf(imageElement.width, imageElement.height) === false) {
+            var imgWidth = imageElement.width,
+                imgHeight = imageElement.height;
+            imageElement.parentNode.removeChild(imageElement);
+            if (resizeIf != null && resizeIf(imgWidth, imgHeight) === false) {
                 deferred.reject('resizeIf');
                 return;
             }
             try {
                 if (ratio) {
                     var ratioFloat = upload.ratioToFloat(ratio);
-                    var imgRatio = imageElement.width / imageElement.height;
+                    var imgRatio = imgWidth / imgHeight;
                     if (imgRatio < ratioFloat) {
-                        width = imageElement.width;
+                        width = imgWidth;
                         height = width / ratioFloat;
                     } else {
-                        height = imageElement.height;
+                        height = imgHeight;
                         width = height * ratioFloat;
                     }
                 }
                 if (!width) {
-                    width = imageElement.width;
+                    width = imgWidth;
                 }
                 if (!height) {
-                    height = imageElement.height;
+                    height = imgHeight;
                 }
-                var dimensions = calculateAspectRatioFit(imageElement.width, imageElement.height, width, height, centerCrop);
+                var dimensions = calculateAspectRatioFit(imgWidth, imgHeight, width, height, centerCrop);
                 canvasElement.width = Math.min(dimensions.width, width);
                 canvasElement.height = Math.min(dimensions.height, height);
                 var context = canvasElement.getContext('2d');
                 context.drawImage(imageElement,
                     Math.min(0, -dimensions.marginX / 2), Math.min(0, -dimensions.marginY / 2),
                     dimensions.width, dimensions.height);
                 deferred.resolve(canvasElement.toDataURL(type || 'image/WebP', quality || 0.934));
             } catch (e) {
                 deferred.reject(e);
             }
         };
         imageElement.onerror = function() {
+            imageElement.parentNode.removeChild(imageElement);
             deferred.reject();
         };
         imageElement.src = imagen;
         return deferred.promise;
     };
 
     upload.dataUrltoBlob = function(dataurl, name, origSize) {
@@ -2235,22 +2343,23 @@
             set: function(v) {
                 this.$ngfName = v;
             },
             configurable: true
         });
     }
 
-    upload.resize = function(file, width, height, quality, type, ratio, centerCrop, resizeIf, restoreExif) {
+    upload.resize = function(file, options) {
         if (file.type.indexOf('image') !== 0) return upload.emptyPromise(file);
 
         var deferred = $q.defer();
         upload.dataUrl(file, true).then(function(url) {
-            resize(url, width, height, quality, type || file.type, ratio, centerCrop, resizeIf)
+            resize(url, options.width, options.height, options.quality, options.type || file.type,
+                    options.ratio, options.centerCrop, options.resizeIf)
                 .then(function(dataUrl) {
-                    if (file.type === 'image/jpeg' && restoreExif) {
+                    if (file.type === 'image/jpeg' && options.restoreExif !== false) {
                         try {
                             dataUrl = upload.restoreExif(url, dataUrl);
                         } catch (e) {
                             setTimeout(function() {
                                 throw e;
                             }, 1);
                         }
@@ -2273,21 +2382,21 @@
         return deferred.promise;
     };
 
     return upload;
 }]);
 
 (function() {
-    ngFileUpload.directive('ngfDrop', ['$parse', '$timeout', '$location', 'Upload', '$http', '$q',
-        function($parse, $timeout, $location, Upload, $http, $q) {
+    ngFileUpload.directive('ngfDrop', ['$parse', '$timeout', '$window', 'Upload', '$http', '$q',
+        function($parse, $timeout, $window, Upload, $http, $q) {
             return {
                 restrict: 'AEC',
                 require: '?ngModel',
                 link: function(scope, elem, attr, ngModel) {
-                    linkDrop(scope, elem, attr, ngModel, $parse, $timeout, $location, Upload, $http, $q);
+                    linkDrop(scope, elem, attr, ngModel, $parse, $timeout, $window, Upload, $http, $q);
                 }
             };
         }
     ]);
 
     ngFileUpload.directive('ngfNoFileDrop', function() {
         return function(scope, elem) {
@@ -2305,15 +2414,15 @@
                         model.assign(scope, true);
                     }
                 });
             }
         };
     }]);
 
-    function linkDrop(scope, elem, attr, ngModel, $parse, $timeout, $location, upload, $http, $q) {
+    function linkDrop(scope, elem, attr, ngModel, $parse, $timeout, $window, upload, $http, $q) {
         var available = dropAvailable();
 
         var attrGetter = function(name, scope, params) {
             return upload.attrGetter(name, attr, scope, params);
         };
 
         if (attrGetter('dropAvailable')) {
@@ -2388,72 +2497,62 @@
         }, false);
         elem[0].addEventListener('drop', function(evt) {
             if (isDisabled() || !upload.shouldUpdateOn('drop', attr, scope)) return;
             evt.preventDefault();
             if (stopPropagation(scope)) evt.stopPropagation();
             if (actualDragOverClass) elem.removeClass(actualDragOverClass);
             actualDragOverClass = null;
-            var items = evt.dataTransfer.items;
-            var html;
-            try {
-                html = evt.dataTransfer && evt.dataTransfer.getData && evt.dataTransfer.getData('text/html');
-            } catch (e) {
-                /* Fix IE11 that throw error calling getData */ }
-
-            extractFiles(items, evt.dataTransfer.files, attrGetter('ngfAllowDir', scope) !== false,
-                attrGetter('multiple') || attrGetter('ngfMultiple', scope)).then(function(files) {
-                if (files.length) {
-                    updateModel(files, evt);
-                } else {
-                    extractFilesFromHtml('dropUrl', html).then(function(files) {
-                        updateModel(files, evt);
-                    });
-                }
-            });
+            extractFilesAndUpdateModel(evt.dataTransfer, evt, 'dropUrl');
         }, false);
         elem[0].addEventListener('paste', function(evt) {
             if (navigator.userAgent.toLowerCase().indexOf('firefox') > -1 &&
                 attrGetter('ngfEnableFirefoxPaste', scope)) {
                 evt.preventDefault();
             }
             if (isDisabled() || !upload.shouldUpdateOn('paste', attr, scope)) return;
-            var files = [];
-            var clipboard = evt.clipboardData || evt.originalEvent.clipboardData;
-            if (clipboard && clipboard.items) {
-                for (var k = 0; k < clipboard.items.length; k++) {
-                    if (clipboard.items[k].type.indexOf('image') !== -1) {
-                        files.push(clipboard.items[k].getAsFile());
-                    }
-                }
-            }
-            if (files.length) {
-                updateModel(files, evt);
-            } else {
-                extractFilesFromHtml('pasteUrl', clipboard).then(function(files) {
-                    updateModel(files, evt);
-                });
-            }
+            extractFilesAndUpdateModel(evt.clipboardData || evt.originalEvent.clipboardData, evt, 'pasteUrl');
         }, false);
 
         if (navigator.userAgent.toLowerCase().indexOf('firefox') > -1 &&
             attrGetter('ngfEnableFirefoxPaste', scope)) {
             elem.attr('contenteditable', true);
             elem.on('keypress', function(e) {
                 if (!e.metaKey && !e.ctrlKey) {
                     e.preventDefault();
                 }
             });
         }
 
+        function extractFilesAndUpdateModel(source, evt, updateOnType) {
+            if (!source) return;
+            // html needs to be calculated on the same process otherwise the data will be wiped
+            // after promise resolve or setTimeout.
+            var html;
+            try {
+                html = source && source.getData && source.getData('text/html');
+            } catch (e) {
+                /* Fix IE11 that throw error calling getData */ }
+            extractFiles(source.items, source.files, attrGetter('ngfAllowDir', scope) !== false,
+                attrGetter('multiple') || attrGetter('ngfMultiple', scope)).then(function(files) {
+                if (files.length) {
+                    updateModel(files, evt);
+                } else {
+                    extractFilesFromHtml(updateOnType, html).then(function(files) {
+                        updateModel(files, evt);
+                    });
+                }
+            });
+        }
+
         function updateModel(files, evt) {
             upload.updateModel(ngModel, attr, scope, attrGetter('ngfChange') || attrGetter('ngfDrop'), files, evt);
         }
 
         function extractFilesFromHtml(updateOn, html) {
-            if (!upload.shouldUpdateOn(updateOn, attr, scope) || !html) return upload.rejectPromise([]);
+            if (!upload.shouldUpdateOn(updateOn, attr, scope) || typeof html !== 'string') return upload.rejectPromise([]);
             var urls = [];
             html.replace(/<(img src|img [^>]* src) *=\"([^\"]*)\"/gi, function(m, n, src) {
                 urls.push(src);
             });
             var promises = [],
                 files = [];
             if (urls.length) {
@@ -2502,30 +2601,36 @@
                     }
                 }
             }
             callback(dClass);
         }
 
         function extractFiles(items, fileList, allowDir, multiple) {
-            var maxFiles = upload.getValidationAttr(attr, scope, 'maxFiles') || Number.MAX_VALUE;
-            var maxTotalSize = upload.getValidationAttr(attr, scope, 'maxTotalSize') || Number.MAX_VALUE;
+            var maxFiles = upload.getValidationAttr(attr, scope, 'maxFiles');
+            if (maxFiles == null) {
+                maxFiles = Number.MAX_VALUE;
+            }
+            var maxTotalSize = upload.getValidationAttr(attr, scope, 'maxTotalSize');
+            if (maxTotalSize == null) {
+                maxTotalSize = Number.MAX_VALUE;
+            }
             var includeDir = attrGetter('ngfIncludeDir', scope);
             var files = [],
                 totalSize = 0;
 
             function traverseFileTree(entry, path) {
                 var defer = $q.defer();
                 if (entry != null) {
                     if (entry.isDirectory) {
                         var promises = [upload.emptyPromise()];
                         if (includeDir) {
                             var file = {
                                 type: 'directory'
                             };
-                            file.name = file.path = (path || '') + entry.name + entry.name;
+                            file.name = file.path = (path || '') + entry.name;
                             files.push(file);
                         }
                         var dirReader = entry.createReader();
                         var entries = [];
                         var readEntries = function() {
                             dirReader.readEntries(function(results) {
                                 try {
@@ -2571,15 +2676,15 @@
                     }
                 }
                 return defer.promise;
             }
 
             var promises = [upload.emptyPromise()];
 
-            if (items && items.length > 0 && $location.protocol() !== 'file') {
+            if (items && items.length > 0 && $window.location.protocol !== 'file:') {
                 for (var i = 0; i < items.length; i++) {
                     if (items[i].webkitGetAsEntry && items[i].webkitGetAsEntry() && items[i].webkitGetAsEntry().isDirectory) {
                         var entry = items[i].webkitGetAsEntry();
                         if (entry.isDirectory && !allowDir) {
                             continue;
                         }
                         if (entry != null) {
```

### Comparing `XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-all.min.js` & `XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-all.min.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! 12.0.4 */ ! function() {
+/*! 12.2.13 */ ! function() {
     function a(a, b) {
         window.XMLHttpRequest.prototype[a] = b(window.XMLHttpRequest.prototype[a])
     }
 
     function b(a, b, c) {
         try {
             Object.defineProperty(a, b, {
@@ -238,15 +238,15 @@
         if ("__setXHR_" === b) {
             var d = c(this);
             d instanceof Function && d(this)
         } else a.apply(this, arguments)
     }
 }(window.XMLHttpRequest.prototype.setRequestHeader));
 var ngFileUpload = angular.module("ngFileUpload", []);
-ngFileUpload.version = "12.0.4", ngFileUpload.service("UploadBase", ["$http", "$q", "$timeout", function(a, b, c) {
+ngFileUpload.version = "12.2.13", ngFileUpload.service("UploadBase", ["$http", "$q", "$timeout", function(a, b, c) {
         function d(d) {
             function e(a) {
                 j.notify && j.notify(a), k.progressFunc && c(function() {
                     k.progressFunc(a)
                 })
             }
 
@@ -259,20 +259,23 @@
                     lengthComputable: !0,
                     target: a.target
                 } : a
             }
 
             function i() {
                 a(d).then(function(a) {
-                    g && d._chunkSize && !d._finished && d._file ? (e({
-                        loaded: d._end,
-                        total: d._file && d._file.size,
-                        config: d,
-                        type: "progress"
-                    }), f.upload(d, !0)) : (d._finished && delete d._finished, j.resolve(a))
+                    if (g && d._chunkSize && !d._finished && d._file) {
+                        var b = d._file && d._file.size || 0;
+                        e({
+                            loaded: Math.min(d._end, b),
+                            total: b,
+                            config: d,
+                            type: "progress"
+                        }), f.upload(d, !0)
+                    } else d._finished && delete d._finished, j.resolve(a)
                 }, function(a) {
                     j.reject(a)
                 }, function(a) {
                     j.notify(a)
                 })
             }
             d.method = d.method || "POST", d.headers = d.headers || {};
@@ -287,15 +290,15 @@
                     }, !1))
                 }
             }), g ? d._chunkSize && d._end && !d._finished ? (d._start = d._end, d._end += d._chunkSize, i()) : d.resumeSizeUrl ? a.get(d.resumeSizeUrl).then(function(a) {
                 d._start = d.resumeSizeResponseReader ? d.resumeSizeResponseReader(a.data) : parseInt((null == a.data.size ? a.data : a.data.size).toString()), d._chunkSize && (d._end = d._start + d._chunkSize), i()
             }, function(a) {
                 throw a
             }) : d.resumeSize ? d.resumeSize().then(function(a) {
-                d._start = a, i()
+                d._start = a, d._chunkSize && (d._end = d._start + d._chunkSize), i()
             }, function(a) {
                 throw a
             }) : (d._chunkSize && (d._start = 0, d._end = d._start + d._chunkSize), i()) : i(), k.success = function(a) {
                 return k.then(function(b) {
                     a(b.data, b.status, b.headers, d)
                 }), k
             }, k.error = function(a) {
@@ -312,15 +315,15 @@
                 }), k
             }, k.xhr = function(a) {
                 return d.xhrFn = function(b) {
                     return function() {
                         b && b.apply(k, arguments), a.apply(k, arguments)
                     }
                 }(d.xhrFn), k
-            }, f.promisesCount++, k["finally"](function() {
+            }, f.promisesCount++, k["finally"] && k["finally"] instanceof Function && k["finally"](function() {
                 f.promisesCount--
             }), k
         }
 
         function e(a) {
             var b = {};
             for (var c in a) a.hasOwnProperty(c) && (b[c] = a[c]);
@@ -409,19 +412,20 @@
             var d = b.defer();
             return a({
                 url: c,
                 method: "get",
                 responseType: "arraybuffer"
             }).then(function(a) {
                 var b = new Uint8Array(a.data),
-                    c = a.headers("content-type") || "image/WebP",
-                    e = new window.Blob([b], {
-                        type: c
-                    });
-                d.resolve(e)
+                    e = a.headers("content-type") || "image/WebP",
+                    f = new window.Blob([b], {
+                        type: e
+                    }),
+                    g = c.match(/.*\/(.+?)(\?.*)?$/);
+                g.length > 1 && (f.name = g[1]), d.resolve(f)
             }, function(a) {
                 d.reject(a)
             }), d.promise
         }, this.setDefaults = function(a) {
             this.defaults = a || {}
         }, this.defaults = {}, this.version = ngFileUpload.version
     }]), ngFileUpload.service("Upload", ["$parse", "$timeout", "$compile", "$q", "UploadExif", function(a, b, c, d, e) {
@@ -432,50 +436,56 @@
                     $file: d
                 }) && e.push(i.happyPromise(i.applyExifRotation(d), d).then(function(b) {
                     a.splice(f, 1, b)
                 }))
             }), d.all(e)
         }
 
-        function g(a, b, c) {
-            var e = i.attrGetter("ngfResize", b, c);
-            if (!e || !i.isResizeSupported() || !a.length) return i.emptyPromise();
-            if (!(e instanceof Function)) return h(e, a, b, c);
-            var f = d.defer();
-            e(a).then(function(d) {
-                h(d, a, b, c).then(function(a) {
-                    f.resolve(a)
+        function g(a, b, c, e) {
+            var f = i.attrGetter("ngfResize", b, c);
+            if (!f || !i.isResizeSupported() || !a.length) return i.emptyPromise();
+            if (f instanceof Function) {
+                var g = d.defer();
+                return f(a).then(function(d) {
+                    h(d, a, b, c, e).then(function(a) {
+                        g.resolve(a)
+                    }, function(a) {
+                        g.reject(a)
+                    })
                 }, function(a) {
-                    f.reject(a)
+                    g.reject(a)
                 })
-            }, function(a) {
-                f.reject(a)
-            })
+            }
+            return h(f, a, b, c, e)
         }
 
-        function h(a, b, c, e) {
-            function f(d, f) {
+        function h(a, b, c, e, f) {
+            function g(d, g) {
                 if (0 === d.type.indexOf("image")) {
                     if (a.pattern && !i.validatePattern(d, a.pattern)) return;
-                    var h = i.resize(d, a.width, a.height, a.quality, a.type, a.ratio, a.centerCrop, function(a, b) {
+                    a.resizeIf = function(a, b) {
                         return i.attrGetter("ngfResizeIf", c, e, {
                             $width: a,
                             $height: b,
                             $file: d
                         })
-                    }, a.restoreExif !== !1);
-                    g.push(h), h.then(function(a) {
-                        b.splice(f, 1, a)
+                    };
+                    var j = i.resize(d, a);
+                    h.push(j), j.then(function(a) {
+                        b.splice(g, 1, a)
                     }, function(a) {
-                        d.$error = "resize", d.$errorParam = (a ? (a.message ? a.message : a) + ": " : "") + (d && d.name)
+                        d.$error = "resize", (d.$errorMessages = d.$errorMessages || {}).resize = !0, d.$errorParam = (a ? (a.message ? a.message : a) + ": " : "") + (d && d.name), f.$ngfValidations.push({
+                            name: "resize",
+                            valid: !1
+                        }), i.applyModelValidation(f, b)
                     })
                 }
             }
-            for (var g = [i.emptyPromise()], h = 0; h < b.length; h++) f(b[h], h);
-            return d.all(g)
+            for (var h = [i.emptyPromise()], j = 0; j < b.length; j++) g(b[j], j);
+            return d.all(h)
         }
         var i = e;
         return i.getAttrWithDefaults = function(a, b) {
             if (null != a[b]) return a[b];
             var c = i.defaults[b];
             return null == c ? c : angular.isString(c) ? c : JSON.stringify(c)
         }, i.attrGetter = function(b, c, d, e) {
@@ -484,15 +494,15 @@
             try {
                 return e ? a(f)(d, e) : a(f)(d)
             } catch (g) {
                 if (b.search(/min|max|pattern/i)) return f;
                 throw g
             }
         }, i.shouldUpdateOn = function(a, b, c) {
-            var d = i.attrGetter("ngModelOptions", b, c);
+            var d = i.attrGetter("ngfModelOptions", b, c);
             return d && d.updateOn ? d.updateOn.split(" ").indexOf(a) > -1 : !0
         }, i.emptyPromise = function() {
             var a = d.defer(),
                 c = arguments;
             return b(function() {
                 a.resolve.apply(a, c)
             }), a.promise
@@ -534,71 +544,72 @@
             function n() {
                 function a(a, b) {
                     return a.name === b.name && (a.$ngfOrigSize || a.size) === (b.$ngfOrigSize || b.size) && a.type === b.type
                 }
 
                 function b(b) {
                     var c;
+                    for (c = 0; c < r.length; c++)
+                        if (a(b, r[c])) return !0;
                     for (c = 0; c < s.length; c++)
                         if (a(b, s[c])) return !0;
-                    for (c = 0; c < t.length; c++)
-                        if (a(b, t[c])) return !0;
                     return !1
                 }
                 if (j) {
-                    r = [], u = [];
-                    for (var c = 0; c < j.length; c++) b(j[c]) ? u.push(j[c]) : r.push(j[c])
+                    q = [], t = [];
+                    for (var c = 0; c < j.length; c++) b(j[c]) ? t.push(j[c]) : q.push(j[c])
                 }
             }
 
             function o(a) {
                 return angular.isArray(a) ? a : [a]
             }
 
             function p() {
-                w = [], v = [], angular.forEach(r, function(a) {
-                    a.$error ? v.push(a) : w.push(a)
-                })
-            }
-
-            function q() {
                 function a() {
                     b(function() {
-                        m(x ? s.concat(w) : w, x ? t.concat(v) : v, j, u, y)
-                    }, A && A.debounce ? A.debounce.change || A.debounce : 0)
+                        m(w ? r.concat(v) : v, w ? s.concat(u) : u, j, t, x)
+                    }, z && z.debounce ? z.debounce.change || z.debounce : 0)
                 }
-                g(z ? r : w, d, e).then(function() {
-                    z ? i.validate(r, s.length, c, d, e).then(function() {
-                        p(), a()
+                var f = y ? q : v;
+                g(f, d, e, c).then(function() {
+                    y ? i.validate(q, w ? r.length : 0, c, d, e).then(function(b) {
+                        v = b.validsFiles, u = b.invalidsFiles, a()
                     }) : a()
-                }, function(a) {
-                    throw "Could not resize files " + a
+                }, function() {
+                    for (var b = 0; b < f.length; b++) {
+                        var c = f[b];
+                        if ("resize" === c.$error) {
+                            var d = v.indexOf(c);
+                            d > -1 && (v.splice(d, 1), u.push(c)), a()
+                        }
+                    }
                 })
             }
-            var r, s, t, u = [],
-                v = [],
-                w = [];
-            s = d.$$ngfPrevValidFiles || [], t = d.$$ngfPrevInvalidFiles || [], c && c.$modelValue && (s = o(c.$modelValue));
-            var x = i.attrGetter("ngfKeep", d, e);
-            r = (j || []).slice(0), ("distinct" === x || i.attrGetter("ngfKeepDistinct", d, e) === !0) && n(d, e);
-            var y = !x && !i.attrGetter("ngfMultiple", d, e) && !i.attrGetter("multiple", d);
-            if (!x || r.length) {
+            var q, r, s, t = [],
+                u = [],
+                v = [];
+            r = d.$$ngfPrevValidFiles || [], s = d.$$ngfPrevInvalidFiles || [], c && c.$modelValue && (r = o(c.$modelValue));
+            var w = i.attrGetter("ngfKeep", d, e);
+            q = (j || []).slice(0), ("distinct" === w || i.attrGetter("ngfKeepDistinct", d, e) === !0) && n(d, e);
+            var x = !w && !i.attrGetter("ngfMultiple", d, e) && !i.attrGetter("multiple", d);
+            if (!w || q.length) {
                 i.attrGetter("ngfBeforeModelChange", d, e, {
                     $files: j,
                     $file: j && j.length ? j[0] : null,
-                    $newFiles: r,
-                    $duplicateFiles: u,
+                    $newFiles: q,
+                    $duplicateFiles: t,
                     $event: k
                 });
-                var z = i.attrGetter("ngfValidateAfterResize", d, e),
-                    A = i.attrGetter("ngModelOptions", d, e);
-                i.validate(r, s.length, c, d, e).then(function() {
-                    l ? m(r, [], j, u, y) : (A && A.allowInvalid || z ? w = r : p(), i.attrGetter("ngfFixOrientation", d, e) && i.isExifSupported() ? f(w, d, e).then(function() {
-                        q()
-                    }) : q())
+                var y = i.attrGetter("ngfValidateAfterResize", d, e),
+                    z = i.attrGetter("ngfModelOptions", d, e);
+                i.validate(q, w ? r.length : 0, c, d, e).then(function(a) {
+                    l ? m(q, [], j, t, x) : (z && z.allowInvalid || y ? v = q : (v = a.validFiles, u = a.invalidFiles), i.attrGetter("ngfFixOrientation", d, e) && i.isExifSupported() ? f(v, d, e).then(function() {
+                        p()
+                    }) : p())
                 })
             }
         }, i
     }]), ngFileUpload.directive("ngfSelect", ["$parse", "$timeout", "$compile", "Upload", function(a, b, c, d) {
         function e(a) {
             var b = a.match(/Android[^\d]*(\d+)\.(\d+)/);
             if (b && b.length > 2) {
@@ -615,108 +626,115 @@
 
             function l() {
                 return t("ngfChange") || t("ngfSelect")
             }
 
             function m(b) {
                 if (j.shouldUpdateOn("change", c, a)) {
-                    for (var e = b.__files_ || b.target && b.target.files, f = [], g = 0; g < e.length; g++) f.push(e[g]);
+                    var e = b.__files_ || b.target && b.target.files,
+                        f = [];
+                    if (!e) return;
+                    for (var g = 0; g < e.length; g++) f.push(e[g]);
                     j.updateModel(d, c, a, l(), f.length ? f : null, b)
                 }
             }
 
-            function n(a) {
-                if (b !== a)
-                    for (var c = 0; c < b[0].attributes.length; c++) {
-                        var d = b[0].attributes[c];
-                        "type" !== d.name && "class" !== d.name && "style" !== d.name && ((null == d.value || "" === d.value) && ("required" === d.name && (d.value = "required"), "multiple" === d.name && (d.value = "multiple")), a.attr(d.name, "id" === d.name ? "ngf-" + d.value : d.value))
-                    }
+            function n(a, d) {
+                function e(b) {
+                    a.attr("id", "ngf-" + b), d.attr("id", "ngf-label-" + b)
+                }
+                for (var f = 0; f < b[0].attributes.length; f++) {
+                    var g = b[0].attributes[f];
+                    "type" !== g.name && "class" !== g.name && "style" !== g.name && ("id" === g.name ? (e(g.value), u.push(c.$observe("id", e))) : a.attr(g.name, g.value || "required" !== g.name && "multiple" !== g.name ? g.value : g.name))
+                }
             }
 
             function o() {
                 if (k()) return b;
-                var a = angular.element('<input type="file">');
-                n(a);
-                var c = angular.element("<label>upload</label>");
-                return c.css("visibility", "hidden").css("position", "absolute").css("overflow", "hidden").css("width", "0px").css("height", "0px").css("border", "none").css("margin", "0px").css("padding", "0px").attr("tabindex", "-1"), g.push({
+                var a = angular.element('<input type="file">'),
+                    c = angular.element("<label>upload</label>");
+                return c.css("visibility", "hidden").css("position", "absolute").css("overflow", "hidden").css("width", "0px").css("height", "0px").css("border", "none").css("margin", "0px").css("padding", "0px").attr("tabindex", "-1"), n(a, c), g.push({
                     el: b,
                     ref: c
                 }), document.body.appendChild(c.append(a)[0]), a
             }
 
             function p(c) {
                 if (b.attr("disabled")) return !1;
                 if (!t("ngfSelectDisabled", a)) {
                     var d = q(c);
                     if (null != d) return d;
                     r(c);
                     try {
-                        k() || document.body.contains(w[0]) || (g.push({
+                        k() || document.body.contains(x[0]) || (g.push({
                             el: b,
-                            ref: w.parent()
-                        }), document.body.appendChild(w.parent()[0]), w.bind("change", m))
+                            ref: x.parent()
+                        }), document.body.appendChild(x.parent()[0]), x.bind("change", m))
                     } catch (f) {}
                     return e(navigator.userAgent) ? setTimeout(function() {
-                        w[0].click()
-                    }, 0) : w[0].click(), !1
+                        x[0].click()
+                    }, 0) : x[0].click(), !1
                 }
             }
 
             function q(a) {
                 var b = a.changedTouches || a.originalEvent && a.originalEvent.changedTouches;
-                if ("touchstart" === a.type) return v = b ? b[0].clientY : 0, !0;
-                if (a.stopPropagation(), a.preventDefault(), "touchend" === a.type) {
-                    var c = b ? b[0].clientY : 0;
-                    if (Math.abs(c - v) > 20) return !1
+                if (b) {
+                    if ("touchstart" === a.type) return w = b[0].clientX, v = b[0].clientY, !0;
+                    if ("touchend" === a.type) {
+                        var c = b[0].clientX,
+                            d = b[0].clientY;
+                        if (Math.abs(c - w) > 20 || Math.abs(d - v) > 20) return a.stopPropagation(), a.preventDefault(), !1
+                    }
+                    return !0
                 }
             }
 
             function r(b) {
-                j.shouldUpdateOn("click", c, a) && w.val() && (w.val(null), j.updateModel(d, c, a, l(), null, b, !0))
+                j.shouldUpdateOn("click", c, a) && x.val() && (x.val(null), j.updateModel(d, c, a, l(), null, b, !0))
             }
 
             function s(a) {
-                if (w && !w.attr("__ngf_ie10_Fix_")) {
-                    if (!w[0].parentNode) return void(w = null);
-                    a.preventDefault(), a.stopPropagation(), w.unbind("click");
-                    var b = w.clone();
-                    return w.replaceWith(b), w = b, w.attr("__ngf_ie10_Fix_", "true"), w.bind("change", m), w.bind("click", s), w[0].click(), !1
+                if (x && !x.attr("__ngf_ie10_Fix_")) {
+                    if (!x[0].parentNode) return void(x = null);
+                    a.preventDefault(), a.stopPropagation(), x.unbind("click");
+                    var b = x.clone();
+                    return x.replaceWith(b), x = b, x.attr("__ngf_ie10_Fix_", "true"), x.bind("change", m), x.bind("click", s), x[0].click(), !1
                 }
-                w.removeAttr("__ngf_ie10_Fix_")
+                x.removeAttr("__ngf_ie10_Fix_")
             }
             var t = function(a, b) {
                 return j.attrGetter(a, c, b)
             };
             j.registerModelChangeValidator(d, c, a);
             var u = [];
-            u.push(a.$watch(t("ngfMultiple"), function() {
-                w.attr("multiple", t("ngfMultiple", a))
-            })), u.push(a.$watch(t("ngfCapture"), function() {
-                w.attr("capture", t("ngfCapture", a))
-            })), u.push(a.$watch(t("ngfAccept"), function() {
-                w.attr("accept", t("ngfAccept", a))
-            })), c.$observe("accept", function() {
-                w.attr("accept", t("accept"))
-            }), u.push(function() {
-                c.$$observers && delete c.$$observers.accept
-            });
+            t("ngfMultiple") && u.push(a.$watch(t("ngfMultiple"), function() {
+                x.attr("multiple", t("ngfMultiple", a))
+            })), t("ngfCapture") && u.push(a.$watch(t("ngfCapture"), function() {
+                x.attr("capture", t("ngfCapture", a))
+            })), t("ngfAccept") && u.push(a.$watch(t("ngfAccept"), function() {
+                x.attr("accept", t("ngfAccept", a))
+            })), u.push(c.$observe("accept", function() {
+                x.attr("accept", t("accept"))
+            }));
             var v = 0,
-                w = b;
-            k() || (w = o()), w.bind("change", m), k() ? b.bind("click", r) : b.bind("click touchstart touchend", p), -1 !== navigator.appVersion.indexOf("MSIE 10") && w.bind("click", s), d && d.$formatters.push(function(a) {
-                return (null == a || 0 === a.length) && w.val() && w.val(null), a
+                w = 0,
+                x = b;
+            k() || (x = o()), x.bind("change", m), k() ? b.bind("click", r) : b.bind("click touchstart touchend", p), -1 !== navigator.appVersion.indexOf("MSIE 10") && x.bind("click", s), d && d.$formatters.push(function(a) {
+                return (null == a || 0 === a.length) && x.val() && x.val(null), a
             }), a.$on("$destroy", function() {
-                k() || w.parent().remove(), angular.forEach(u, function(a) {
+                k() || x.parent().remove(), angular.forEach(u, function(a) {
                     a()
                 })
             }), h(function() {
                 for (var a = 0; a < g.length; a++) {
                     var b = g[a];
                     document.body.contains(b.el[0]) || (g.splice(a, 1), b.ref.remove())
                 }
-            }), window.FileAPI && window.FileAPI.ngfFixIE && window.FileAPI.ngfFixIE(b, w, m)
+            }), window.FileAPI && window.FileAPI.ngfFixIE && window.FileAPI.ngfFixIE(b, x, m)
         }
         var g = [];
         return {
             restrict: "AEC",
             require: "?ngModel",
             link: function(e, g, h, i) {
                 f(e, g, h, i, a, b, c, d)
@@ -736,30 +754,36 @@
                         var b = (g ? a.$ngfDataUrl : a.$ngfBlobUrl) || a.$ngfDataUrl;
                         i ? e.css("background-image", "url('" + (b || "") + "')") : e.attr("src", b), b ? e.removeClass("ng-hide") : e.addClass("ng-hide")
                     })
                 })
             }
             c(function() {
                 var c = d.$watch(f[g], function(c) {
-                    var d = h;
-                    if ("ngfThumbnail" === g && (d || (d = {
-                            width: e[0].clientWidth,
-                            height: e[0].clientHeight
-                        }), 0 === d.width && window.getComputedStyle)) {
-                        var f = getComputedStyle(e[0]);
-                        d = {
-                            width: parseInt(f.width.slice(0, -2)),
-                            height: parseInt(f.height.slice(0, -2))
-                        }
+                    var k = h;
+                    if ("ngfThumbnail" === g && (k || (k = {
+                            width: e[0].naturalWidth || e[0].clientWidth,
+                            height: e[0].naturalHeight || e[0].clientHeight
+                        }), 0 === k.width && window.getComputedStyle)) {
+                        var l = getComputedStyle(e[0]);
+                        l.width && l.width.indexOf("px") > -1 && l.height && l.height.indexOf("px") > -1 && (k = {
+                            width: parseInt(l.width.slice(0, -2)),
+                            height: parseInt(l.height.slice(0, -2))
+                        })
                     }
-                    return angular.isString(c) ? (e.removeClass("ng-hide"), i ? e.css("background-image", "url('" + c + "')") : e.attr("src", c)) : void(!c || !c.type || 0 !== c.type.search(a(e[0])) || i && 0 !== c.type.indexOf("image") ? e.addClass("ng-hide") : d && b.isResizeSupported() ? b.resize(c, d.width, d.height, d.quality).then(function(a) {
+                    return angular.isString(c) ? (e.removeClass("ng-hide"), i ? e.css("background-image", "url('" + c + "')") : e.attr("src", c)) : void(!c || !c.type || 0 !== c.type.search(a(e[0])) || i && 0 !== c.type.indexOf("image") ? e.addClass("ng-hide") : k && b.isResizeSupported() ? (k.resizeIf = function(a, e) {
+                        return b.attrGetter("ngfResizeIf", f, d, {
+                            $width: a,
+                            $height: e,
+                            $file: c
+                        })
+                    }, b.resize(c, k).then(function(a) {
                         j(a)
                     }, function(a) {
                         throw a
-                    }) : j(c))
+                    })) : j(c))
                 });
                 d.$on("$destroy", function() {
                     c()
                 })
             })
         }
         ngFileUpload.service("UploadDataUrl", ["UploadBase", "$timeout", "$q", function(a, b, c) {
@@ -851,15 +875,15 @@
                 restrict: "AE",
                 link: function(d, e, f) {
                     var g = a.attrGetter("ngfSize", f, d);
                     b(a, c, d, e, f, "ngfThumbnail", g, a.attrGetter("ngfAsBackground", f, d))
                 }
             }
         }]), ngFileUpload.config(["$compileProvider", function(a) {
-            a.imgSrcSanitizationWhitelist && a.imgSrcSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|local|file|data|blob):/), a.aHrefSanitizationWhitelist && a.aHrefSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|local|file|data|blob):/)
+            a.imgSrcSanitizationWhitelist && a.imgSrcSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|webcal|local|file|data|blob):/), a.aHrefSanitizationWhitelist && a.aHrefSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|webcal|local|file|data|blob):/)
         }]), ngFileUpload.filter("ngfDataUrl", ["UploadDataUrl", "$sce", function(a, b) {
             return function(c, d, e) {
                 if (angular.isString(c)) return b.trustAsResourceUrl(c);
                 var f = c && ((d ? c.$ngfDataUrl : c.$ngfBlobUrl) || c.$ngfDataUrl);
                 return c && !f ? (!c.$ngfDataUrlFilterInProgress && angular.isObject(c) && (c.$ngfDataUrlFilterInProgress = !0, a.dataUrl(c, d)), "") : (c && delete c.$ngfDataUrlFilterInProgress, (c && f ? e ? b.trustAsResourceUrl(f) : f : c) || "")
             }
         }])
@@ -901,17 +925,21 @@
             return e
         }, f.ratioToFloat = function(a) {
             var b = a.toString(),
                 c = b.search(/[x:]/i);
             return b = c > -1 ? parseFloat(b.substring(0, c)) / parseFloat(b.substring(c + 1)) : parseFloat(b)
         }, f.registerModelChangeValidator = function(a, b, c) {
             a && a.$formatters.push(function(d) {
-                a.$dirty && (d && !angular.isArray(d) && (d = [d]), f.validate(d, 0, a, b, c).then(function() {
-                    f.applyModelValidation(a, d)
-                }))
+                if (a.$dirty) {
+                    var e = d;
+                    d && !angular.isArray(d) && (e = [d]), f.validate(e, 0, a, b, c).then(function() {
+                        f.applyModelValidation(a, e)
+                    })
+                }
+                return d
             })
         }, f.applyModelValidation = function(a, b) {
             e(a, b), angular.forEach(a.$ngfValidations, function(b) {
                 a.$setValidity(b.name, b.valid)
             })
         }, f.getValidationAttr = function(a, b, c, d, e) {
             var g = "ngf" + c[0].toUpperCase() + c.substr(1),
@@ -925,124 +953,161 @@
                 h = h[i[0]], i.length > 1 && (h = h && h[i[1]])
             }
             return h
         }, f.validate = function(a, c, d, e, g) {
             function h(b, c, h) {
                 if (a) {
                     for (var i = a.length, j = null; i--;) {
-                        var k = a[i];
-                        if (k) {
-                            var l = f.getValidationAttr(e, g, b, c, k);
-                            null != l && (h(k, l, i) || (k.$error = b, (k.$errorMessages = k.$errorMessages || {})[b] = !0, k.$errorParam = l, a.splice(i, 1), j = !1))
+                        var n = a[i];
+                        if (n) {
+                            var o = f.getValidationAttr(e, g, b, c, n);
+                            null != o && (h(n, o, i) || (-1 === k.indexOf(b) ? (n.$error = b, (n.$errorMessages = n.$errorMessages || {})[b] = !0, n.$errorParam = o, -1 === m.indexOf(n) && m.push(n), l || a.splice(i, 1), j = !1) : a.splice(i, 1)))
                         }
                     }
                     null !== j && d.$ngfValidations.push({
                         name: b,
                         valid: j
                     })
                 }
             }
 
-            function i(c, h, i, k, l) {
-                function m(a, b, d) {
-                    null != d ? k(b, d).then(function(e) {
-                        l(e, d) ? a.resolve() : (b.$error = c, (b.$errorMessages = b.$errorMessages || {})[c] = !0, b.$errorParam = d, a.reject())
+            function i(c, h, i, n, o) {
+                function p(b, d, e) {
+                    function f(f) {
+                        if (f())
+                            if (-1 === k.indexOf(c)) {
+                                if (d.$error = c, (d.$errorMessages = d.$errorMessages || {})[c] = !0, d.$errorParam = e, -1 === m.indexOf(d) && m.push(d), !l) {
+                                    var g = a.indexOf(d);
+                                    g > -1 && a.splice(g, 1)
+                                }
+                                b.resolve(!1)
+                            } else {
+                                var h = a.indexOf(d);
+                                h > -1 && a.splice(h, 1), b.resolve(!0)
+                            }
+                        else b.resolve(!0)
+                    }
+                    null != e ? n(d, e).then(function(a) {
+                        f(function() {
+                            return !o(a, e)
+                        })
                     }, function() {
-                        j("ngfValidateForce", {
-                            $file: b
-                        }) ? (b.$error = c, (b.$errorMessages = b.$errorMessages || {})[c] = !0, b.$errorParam = d, a.reject()) : a.resolve()
-                    }) : a.resolve()
+                        f(function() {
+                            return j("ngfValidateForce", {
+                                $file: d
+                            })
+                        })
+                    }) : b.resolve(!0)
                 }
-                var n = [f.emptyPromise()];
-                return a ? (a = void 0 === a.length ? [a] : a, angular.forEach(a, function(a) {
+                var q = [f.emptyPromise(!0)];
+                a && (a = void 0 === a.length ? [a] : a, angular.forEach(a, function(a) {
                     var d = b.defer();
-                    return n.push(d.promise), !i || null != a.type && 0 === a.type.search(i) ? void("dimensions" === c && null != f.attrGetter("ngfDimensions", e) ? f.imageDimensions(a).then(function(b) {
-                        m(d, a, j("ngfDimensions", {
+                    return q.push(d.promise), !i || null != a.type && 0 === a.type.search(i) ? void("dimensions" === c && null != f.attrGetter("ngfDimensions", e) ? f.imageDimensions(a).then(function(b) {
+                        p(d, a, j("ngfDimensions", {
                             $file: a,
                             $width: b.width,
                             $height: b.height
                         }))
                     }, function() {
-                        d.reject()
+                        d.resolve(!1)
                     }) : "duration" === c && null != f.attrGetter("ngfDuration", e) ? f.mediaDuration(a).then(function(b) {
-                        m(d, a, j("ngfDuration", {
+                        p(d, a, j("ngfDuration", {
                             $file: a,
                             $duration: b
                         }))
                     }, function() {
-                        d.reject()
-                    }) : m(d, a, f.getValidationAttr(e, g, c, h, a))) : void d.resolve()
-                }), b.all(n).then(function() {
-                    d.$ngfValidations.push({
-                        name: c,
-                        valid: !0
-                    })
-                }, function() {
-                    d.$ngfValidations.push({
+                        d.resolve(!1)
+                    }) : p(d, a, f.getValidationAttr(e, g, c, h, a))) : void d.resolve(!0)
+                }));
+                var r = b.defer();
+                return b.all(q).then(function(a) {
+                    for (var b = !0, e = 0; e < a.length; e++)
+                        if (!a[e]) {
+                            b = !1;
+                            break
+                        } d.$ngfValidations.push({
                         name: c,
-                        valid: !1
-                    })
-                })) : void 0
+                        valid: b
+                    }), r.resolve(b)
+                }), r.promise
             }
             d = d || {}, d.$ngfValidations = d.$ngfValidations || [], angular.forEach(d.$ngfValidations, function(a) {
                 a.valid = !0
             });
             var j = function(a, b) {
-                return f.attrGetter(a, e, g, b)
-            };
-            if (null == a || 0 === a.length) return f.emptyPromise(d);
-            a = void 0 === a.length ? [a] : a.slice(0), h("maxFiles", null, function(a, b, d) {
-                return b > c + d
-            }), h("pattern", null, f.validatePattern), h("minSize", "size.min", function(a, b) {
+                    return f.attrGetter(a, e, g, b)
+                },
+                k = (f.attrGetter("ngfIgnoreInvalid", e, g) || "").split(" "),
+                l = f.attrGetter("ngfRunAllValidations", e, g);
+            if (null == a || 0 === a.length) return f.emptyPromise({
+                validFiles: a,
+                invalidFiles: []
+            });
+            a = void 0 === a.length ? [a] : a.slice(0);
+            var m = [];
+            h("pattern", null, f.validatePattern), h("minSize", "size.min", function(a, b) {
                 return a.size + .1 >= f.translateScalars(b)
             }), h("maxSize", "size.max", function(a, b) {
                 return a.size - .1 <= f.translateScalars(b)
             });
-            var k = 0;
+            var n = 0;
             if (h("maxTotalSize", null, function(b, c) {
-                    return k += b.size, k > f.translateScalars(c) ? (a.splice(0, a.length), !1) : !0
+                    return n += b.size, n > f.translateScalars(c) ? (a.splice(0, a.length), !1) : !0
                 }), h("validateFn", null, function(a, b) {
                     return b === !0 || null === b || "" === b
-                }), !a.length) return f.emptyPromise(d, d.$ngfValidations);
-            var l = b.defer(),
-                m = [];
-            return m.push(f.happyPromise(i("maxHeight", "height.max", /image/, this.imageDimensions, function(a, b) {
+                }), !a.length) return f.emptyPromise({
+                validFiles: [],
+                invalidFiles: m
+            });
+            var o = b.defer(),
+                p = [];
+            return p.push(i("maxHeight", "height.max", /image/, this.imageDimensions, function(a, b) {
                 return a.height <= b
-            }))), m.push(f.happyPromise(i("minHeight", "height.min", /image/, this.imageDimensions, function(a, b) {
+            })), p.push(i("minHeight", "height.min", /image/, this.imageDimensions, function(a, b) {
                 return a.height >= b
-            }))), m.push(f.happyPromise(i("maxWidth", "width.max", /image/, this.imageDimensions, function(a, b) {
+            })), p.push(i("maxWidth", "width.max", /image/, this.imageDimensions, function(a, b) {
                 return a.width <= b
-            }))), m.push(f.happyPromise(i("minWidth", "width.min", /image/, this.imageDimensions, function(a, b) {
+            })), p.push(i("minWidth", "width.min", /image/, this.imageDimensions, function(a, b) {
                 return a.width >= b
-            }))), m.push(f.happyPromise(i("dimensions", null, /image/, function(a, b) {
+            })), p.push(i("dimensions", null, /image/, function(a, b) {
                 return f.emptyPromise(b)
             }, function(a) {
                 return a
-            }))), m.push(f.happyPromise(i("ratio", null, /image/, this.imageDimensions, function(a, b) {
-                for (var c = b.toString().split(","), d = !1, e = 0; e < c.length; e++) Math.abs(a.width / a.height - f.ratioToFloat(c[e])) < 1e-4 && (d = !0);
+            })), p.push(i("ratio", null, /image/, this.imageDimensions, function(a, b) {
+                for (var c = b.toString().split(","), d = !1, e = 0; e < c.length; e++) Math.abs(a.width / a.height - f.ratioToFloat(c[e])) < .01 && (d = !0);
                 return d
-            }))), m.push(f.happyPromise(i("maxRatio", "ratio.max", /image/, this.imageDimensions, function(a, b) {
+            })), p.push(i("maxRatio", "ratio.max", /image/, this.imageDimensions, function(a, b) {
                 return a.width / a.height - f.ratioToFloat(b) < 1e-4
-            }))), m.push(f.happyPromise(i("minRatio", "ratio.min", /image/, this.imageDimensions, function(a, b) {
+            })), p.push(i("minRatio", "ratio.min", /image/, this.imageDimensions, function(a, b) {
                 return a.width / a.height - f.ratioToFloat(b) > -1e-4
-            }))), m.push(f.happyPromise(i("maxDuration", "duration.max", /audio|video/, this.mediaDuration, function(a, b) {
+            })), p.push(i("maxDuration", "duration.max", /audio|video/, this.mediaDuration, function(a, b) {
                 return a <= f.translateScalars(b)
-            }))), m.push(f.happyPromise(i("minDuration", "duration.min", /audio|video/, this.mediaDuration, function(a, b) {
+            })), p.push(i("minDuration", "duration.min", /audio|video/, this.mediaDuration, function(a, b) {
                 return a >= f.translateScalars(b)
-            }))), m.push(f.happyPromise(i("duration", null, /audio|video/, function(a, b) {
+            })), p.push(i("duration", null, /audio|video/, function(a, b) {
                 return f.emptyPromise(b)
             }, function(a) {
                 return a
-            }))), m.push(f.happyPromise(i("validateAsyncFn", null, null, function(a, b) {
+            })), p.push(i("validateAsyncFn", null, null, function(a, b) {
                 return b
             }, function(a) {
                 return a === !0 || null === a || "" === a
-            }))), b.all(m).then(function() {
-                l.resolve(d, d.$ngfValidations)
-            })
+            })), b.all(p).then(function() {
+                if (l)
+                    for (var b = 0; b < a.length; b++) {
+                        var d = a[b];
+                        d.$error && a.splice(b--, 1)
+                    }
+                l = !1, h("maxFiles", null, function(a, b, d) {
+                    return b > c + d
+                }), o.resolve({
+                    validFiles: a,
+                    invalidFiles: m
+                })
+            }), o.promise
         }, f.imageDimensions = function(a) {
             if (a.$ngfWidth && a.$ngfHeight) {
                 var d = b.defer();
                 return c(function() {
                     d.resolve({
                         width: a.$ngfWidth,
                         height: a.$ngfHeight
@@ -1050,29 +1115,29 @@
                 }), d.promise
             }
             if (a.$ngfDimensionPromise) return a.$ngfDimensionPromise;
             var e = b.defer();
             return c(function() {
                 return 0 !== a.type.indexOf("image") ? void e.reject("not image") : void f.dataUrl(a).then(function(b) {
                     function d() {
-                        var b = h[0].clientWidth,
-                            c = h[0].clientHeight;
+                        var b = h[0].naturalWidth || h[0].clientWidth,
+                            c = h[0].naturalHeight || h[0].clientHeight;
                         h.remove(), a.$ngfWidth = b, a.$ngfHeight = c, e.resolve({
                             width: b,
                             height: c
                         })
                     }
 
                     function f() {
                         h.remove(), e.reject("load error")
                     }
 
                     function g() {
                         c(function() {
-                            h[0].parentNode && (h[0].clientWidth ? d() : i > 10 ? f() : g())
+                            h[0].parentNode && (h[0].clientWidth ? d() : i++ > 10 ? f() : g())
                         }, 1e3)
                     }
                     var h = angular.element("<img>").attr("src", b).css("visibility", "hidden").css("position", "fixed").css("max-width", "none !important").css("max-height", "none !important");
                     h.on("load", d), h.on("error", f);
                     var i = 0;
                     g(), angular.element(document.getElementsByTagName("body")[0]).append(h)
                 }, function() {
@@ -1090,16 +1155,15 @@
             }
             if (a.$ngfDurationPromise) return a.$ngfDurationPromise;
             var e = b.defer();
             return c(function() {
                 return 0 !== a.type.indexOf("audio") && 0 !== a.type.indexOf("video") ? void e.reject("not media") : void f.dataUrl(a).then(function(b) {
                     function d() {
                         var b = h[0].duration;
-                        a.$ngfDuration = b, h.remove(), e.resolve(b);
-
+                        a.$ngfDuration = b, h.remove(), e.resolve(b)
                     }
 
                     function f() {
                         h.remove(), e.reject("load error")
                     }
 
                     function g() {
@@ -1129,32 +1193,34 @@
                     marginY: b * f - d
                 }
             },
             e = function(a, e, f, g, h, i, j, k) {
                 var l = b.defer(),
                     m = document.createElement("canvas"),
                     n = document.createElement("img");
-                return n.onload = function() {
-                    if (null != k && k(n.width, n.height) === !1) return void l.reject("resizeIf");
+                return n.setAttribute("style", "visibility:hidden;position:fixed;z-index:-100000"), document.body.appendChild(n), n.onload = function() {
+                    var a = n.width,
+                        b = n.height;
+                    if (n.parentNode.removeChild(n), null != k && k(a, b) === !1) return void l.reject("resizeIf");
                     try {
                         if (i) {
-                            var a = c.ratioToFloat(i),
-                                b = n.width / n.height;
-                            a > b ? (e = n.width, f = e / a) : (f = n.height, e = f * a)
+                            var o = c.ratioToFloat(i),
+                                p = a / b;
+                            o > p ? (e = a, f = e / o) : (f = b, e = f * o)
                         }
-                        e || (e = n.width), f || (f = n.height);
-                        var o = d(n.width, n.height, e, f, j);
-                        m.width = Math.min(o.width, e), m.height = Math.min(o.height, f);
-                        var p = m.getContext("2d");
-                        p.drawImage(n, Math.min(0, -o.marginX / 2), Math.min(0, -o.marginY / 2), o.width, o.height), l.resolve(m.toDataURL(h || "image/WebP", g || .934))
-                    } catch (q) {
-                        l.reject(q)
+                        e || (e = a), f || (f = b);
+                        var q = d(a, b, e, f, j);
+                        m.width = Math.min(q.width, e), m.height = Math.min(q.height, f);
+                        var r = m.getContext("2d");
+                        r.drawImage(n, Math.min(0, -q.marginX / 2), Math.min(0, -q.marginY / 2), q.width, q.height), l.resolve(m.toDataURL(h || "image/WebP", g || .934))
+                    } catch (s) {
+                        l.reject(s)
                     }
                 }, n.onerror = function() {
-                    l.reject()
+                    n.parentNode.removeChild(n), l.reject()
                 }, n.src = a, l.promise
             };
         return c.dataUrltoBlob = function(a, b, c) {
             for (var d = a.split(","), e = d[0].match(/:(.*?);/)[1], f = atob(d[1]), g = f.length, h = new Uint8Array(g); g--;) h[g] = f.charCodeAt(g);
             var i = new window.Blob([h], {
                 type: e
             });
@@ -1166,52 +1232,66 @@
             get: function() {
                 return this.$ngfName
             },
             set: function(a) {
                 this.$ngfName = a
             },
             configurable: !0
-        }), c.resize = function(a, d, f, g, h, i, j, k, l) {
+        }), c.resize = function(a, d) {
             if (0 !== a.type.indexOf("image")) return c.emptyPromise(a);
-            var m = b.defer();
+            var f = b.defer();
             return c.dataUrl(a, !0).then(function(b) {
-                e(b, d, f, g, h || a.type, i, j, k).then(function(d) {
-                    if ("image/jpeg" === a.type && l) try {
-                        d = c.restoreExif(b, d)
-                    } catch (e) {
+                e(b, d.width, d.height, d.quality, d.type || a.type, d.ratio, d.centerCrop, d.resizeIf).then(function(e) {
+                    if ("image/jpeg" === a.type && d.restoreExif !== !1) try {
+                        e = c.restoreExif(b, e)
+                    } catch (g) {
                         setTimeout(function() {
-                            throw e
+                            throw g
                         }, 1)
                     }
                     try {
-                        var f = c.dataUrltoBlob(d, a.name, a.size);
-                        m.resolve(f)
-                    } catch (e) {
-                        m.reject(e)
+                        var h = c.dataUrltoBlob(e, a.name, a.size);
+                        f.resolve(h)
+                    } catch (g) {
+                        f.reject(g)
                     }
                 }, function(b) {
-                    "resizeIf" === b && m.resolve(a), m.reject(b)
+                    "resizeIf" === b && f.resolve(a), f.reject(b)
                 })
             }, function(a) {
-                m.reject(a)
-            }), m.promise
+                f.reject(a)
+            }), f.promise
         }, c
     }]),
     function() {
         function a(a, c, d, e, f, g, h, i, j, k) {
             function l() {
-                return c.attr("disabled") || r("ngfDropDisabled", a)
+                return c.attr("disabled") || s("ngfDropDisabled", a)
             }
 
-            function m(b, c) {
-                i.updateModel(e, d, a, r("ngfChange") || r("ngfDrop"), b, c)
+            function m(b, c, d) {
+                if (b) {
+                    var e;
+                    try {
+                        e = b && b.getData && b.getData("text/html")
+                    } catch (f) {}
+                    q(b.items, b.files, s("ngfAllowDir", a) !== !1, s("multiple") || s("ngfMultiple", a)).then(function(a) {
+                        a.length ? n(a, c) : o(d, e).then(function(a) {
+                            n(a, c)
+                        })
+                    })
+                }
             }
 
             function n(b, c) {
-                if (!i.shouldUpdateOn(b, d, a) || !c) return i.rejectPromise([]);
+                i.updateModel(e, d, a, s("ngfChange") || s("ngfDrop"), b, c)
+            }
+
+            function o(b, c) {
+                if (!i.shouldUpdateOn(b, d, a) || "string" != typeof c) return i.rejectPromise([]);
                 var e = [];
                 c.replace(/<(img src|img [^>]* src) *=\"([^\"]*)\"/gi, function(a, b, c) {
                     e.push(c)
                 });
                 var f = [],
                     g = [];
                 if (e.length) {
@@ -1226,47 +1306,47 @@
                     }, function(a) {
                         h.reject(a)
                     }), h.promise
                 }
                 return i.emptyPromise()
             }
 
-            function o(a, b, c, d) {
-                var e = r("ngfDragOverClass", a, {
+            function p(a, b, c, d) {
+                var e = s("ngfDragOverClass", a, {
                         $event: c
                     }),
                     f = "dragover";
                 if (angular.isString(e)) f = e;
-                else if (e && (e.delay && (v = e.delay), e.accept || e.reject)) {
+                else if (e && (e.delay && (w = e.delay), e.accept || e.reject)) {
                     var g = c.dataTransfer.items;
                     if (null != g && g.length)
-                        for (var h = e.pattern || r("ngfPattern", a, {
+                        for (var h = e.pattern || s("ngfPattern", a, {
                                 $event: c
                             }), j = g.length; j--;) {
                             if (!i.validatePattern(g[j], h)) {
                                 f = e.reject;
                                 break
                             }
                             f = e.accept
                         } else f = e.accept
                 }
                 d(f)
             }
 
-            function p(b, c, e, f) {
+            function q(b, c, e, f) {
                 function g(a, b) {
                     var c = k.defer();
                     if (null != a)
                         if (a.isDirectory) {
                             var d = [i.emptyPromise()];
                             if (m) {
                                 var e = {
                                     type: "directory"
                                 };
-                                e.name = e.path = (b || "") + a.name + a.name, n.push(e)
+                                e.name = e.path = (b || "") + a.name, n.push(e)
                             }
                             var f = a.createReader(),
                                 h = [],
                                 p = function() {
                                     f.readEntries(function(e) {
                                         try {
                                             e.length ? (h = h.concat(Array.prototype.slice.call(e || [], 0)), p()) : (angular.forEach(h.slice(0), function(c) {
@@ -1291,26 +1371,28 @@
                                 c.reject(d)
                             }
                         }, function(a) {
                             c.reject(a)
                         });
                     return c.promise
                 }
-                var j = i.getValidationAttr(d, a, "maxFiles") || Number.MAX_VALUE,
-                    l = i.getValidationAttr(d, a, "maxTotalSize") || Number.MAX_VALUE,
-                    m = r("ngfIncludeDir", a),
+                var j = i.getValidationAttr(d, a, "maxFiles");
+                null == j && (j = Number.MAX_VALUE);
+                var l = i.getValidationAttr(d, a, "maxTotalSize");
+                null == l && (l = Number.MAX_VALUE);
+                var m = s("ngfIncludeDir", a),
                     n = [],
                     o = 0,
                     p = [i.emptyPromise()];
-                if (b && b.length > 0 && "file" !== h.protocol())
+                if (b && b.length > 0 && "file:" !== h.location.protocol)
                     for (var q = 0; q < b.length; q++) {
                         if (b[q].webkitGetAsEntry && b[q].webkitGetAsEntry() && b[q].webkitGetAsEntry().isDirectory) {
-                            var s = b[q].webkitGetAsEntry();
-                            if (s.isDirectory && !e) continue;
-                            null != s && p.push(g(s))
+                            var r = b[q].webkitGetAsEntry();
+                            if (r.isDirectory && !e) continue;
+                            null != r && p.push(g(r))
                         } else {
                             var t = b[q].getAsFile();
                             null != t && (n.push(t), o += t.size)
                         }
                         if (n.length > j || o > l || !f && n.length > 0) break
                     } else if (null != c)
                         for (var u = 0; u < c.length; u++) {
@@ -1324,81 +1406,62 @@
                         for (var a = 0; n[a] && "directory" === n[a].type;) a++;
                         w.resolve([n[a]])
                     }
                 }, function(a) {
                     w.reject(a)
                 }), w.promise
             }
-            var q = b(),
-                r = function(a, b, c) {
+            var r = b(),
+                s = function(a, b, c) {
                     return i.attrGetter(a, d, b, c)
                 };
-            if (r("dropAvailable") && g(function() {
-                    a[r("dropAvailable")] ? a[r("dropAvailable")].value = q : a[r("dropAvailable")] = q
-                }), !q) return void(r("ngfHideOnDropNotAvailable", a) === !0 && c.css("display", "none"));
-            null == r("ngfSelect") && i.registerModelChangeValidator(e, d, a);
-            var s, t = null,
-                u = f(r("ngfStopPropagation")),
-                v = 1;
+            if (s("dropAvailable") && g(function() {
+                    a[s("dropAvailable")] ? a[s("dropAvailable")].value = r : a[s("dropAvailable")] = r
+                }), !r) return void(s("ngfHideOnDropNotAvailable", a) === !0 && c.css("display", "none"));
+            null == s("ngfSelect") && i.registerModelChangeValidator(e, d, a);
+            var t, u = null,
+                v = f(s("ngfStopPropagation")),
+                w = 1;
             c[0].addEventListener("dragover", function(b) {
                 if (!l() && i.shouldUpdateOn("drop", d, a)) {
-                    if (b.preventDefault(), u(a) && b.stopPropagation(), navigator.userAgent.indexOf("Chrome") > -1) {
+                    if (b.preventDefault(), v(a) && b.stopPropagation(), navigator.userAgent.indexOf("Chrome") > -1) {
                         var e = b.dataTransfer.effectAllowed;
                         b.dataTransfer.dropEffect = "move" === e || "linkMove" === e ? "move" : "copy"
                     }
-                    g.cancel(t), s || (s = "C", o(a, d, b, function(d) {
-                        s = d, c.addClass(s), r("ngfDrag", a, {
+                    g.cancel(u), t || (t = "C", p(a, d, b, function(d) {
+                        t = d, c.addClass(t), s("ngfDrag", a, {
                             $isDragging: !0,
-                            $class: s,
+                            $class: t,
                             $event: b
                         })
                     }))
                 }
             }, !1), c[0].addEventListener("dragenter", function(b) {
-                !l() && i.shouldUpdateOn("drop", d, a) && (b.preventDefault(), u(a) && b.stopPropagation())
+                !l() && i.shouldUpdateOn("drop", d, a) && (b.preventDefault(), v(a) && b.stopPropagation())
             }, !1), c[0].addEventListener("dragleave", function(b) {
-                !l() && i.shouldUpdateOn("drop", d, a) && (b.preventDefault(), u(a) && b.stopPropagation(), t = g(function() {
-                    s && c.removeClass(s), s = null, r("ngfDrag", a, {
+                !l() && i.shouldUpdateOn("drop", d, a) && (b.preventDefault(), v(a) && b.stopPropagation(), u = g(function() {
+                    t && c.removeClass(t), t = null, s("ngfDrag", a, {
                         $isDragging: !1,
                         $event: b
                     })
-                }, v || 100))
+                }, w || 100))
             }, !1), c[0].addEventListener("drop", function(b) {
-                if (!l() && i.shouldUpdateOn("drop", d, a)) {
-                    b.preventDefault(), u(a) && b.stopPropagation(), s && c.removeClass(s), s = null;
-                    var e, f = b.dataTransfer.items;
-                    try {
-                        e = b.dataTransfer && b.dataTransfer.getData && b.dataTransfer.getData("text/html")
-                    } catch (g) {}
-                    p(f, b.dataTransfer.files, r("ngfAllowDir", a) !== !1, r("multiple") || r("ngfMultiple", a)).then(function(a) {
-                        a.length ? m(a, b) : n("dropUrl", e).then(function(a) {
-                            m(a, b)
-                        })
-                    })
-                }
+                !l() && i.shouldUpdateOn("drop", d, a) && (b.preventDefault(), v(a) && b.stopPropagation(), t && c.removeClass(t), t = null, m(b.dataTransfer, b, "dropUrl"))
             }, !1), c[0].addEventListener("paste", function(b) {
-                if (navigator.userAgent.toLowerCase().indexOf("firefox") > -1 && r("ngfEnableFirefoxPaste", a) && b.preventDefault(), !l() && i.shouldUpdateOn("paste", d, a)) {
-                    var c = [],
-                        e = b.clipboardData || b.originalEvent.clipboardData;
-                    if (e && e.items)
-                        for (var f = 0; f < e.items.length; f++) - 1 !== e.items[f].type.indexOf("image") && c.push(e.items[f].getAsFile());
-                    c.length ? m(c, b) : n("pasteUrl", e).then(function(a) {
-                        m(a, b)
-                    })
-                }
-            }, !1), navigator.userAgent.toLowerCase().indexOf("firefox") > -1 && r("ngfEnableFirefoxPaste", a) && (c.attr("contenteditable", !0), c.on("keypress", function(a) {
+                navigator.userAgent.toLowerCase().indexOf("firefox") > -1 && s("ngfEnableFirefoxPaste", a) && b.preventDefault(), !l() && i.shouldUpdateOn("paste", d, a) && m(b.clipboardData || b.originalEvent.clipboardData, b, "pasteUrl")
+            }, !1), navigator.userAgent.toLowerCase().indexOf("firefox") > -1 && s("ngfEnableFirefoxPaste", a) && (c.attr("contenteditable", !0), c.on("keypress", function(a) {
                 a.metaKey || a.ctrlKey || a.preventDefault()
             }))
         }
 
         function b() {
             var a = document.createElement("div");
             return "draggable" in a && "ondrop" in a && !/Edge\/12./i.test(navigator.userAgent)
         }
-        ngFileUpload.directive("ngfDrop", ["$parse", "$timeout", "$location", "Upload", "$http", "$q", function(b, c, d, e, f, g) {
+        ngFileUpload.directive("ngfDrop", ["$parse", "$timeout", "$window", "Upload", "$http", "$q", function(b, c, d, e, f, g) {
             return {
                 restrict: "AEC",
                 require: "?ngModel",
                 link: function(h, i, j, k) {
                     a(h, i, j, k, b, c, d, e, f, g)
                 }
             }
```

### Comparing `XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-shim.js` & `XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-shim.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 /**!
- * AngularJS file upload directives and services. Supoorts: file upload/drop/paste, resume, cancel/abort,
+ * AngularJS file upload directives and services. Supports: file upload/drop/paste, resume, cancel/abort,
  * progress, resize, thumbnail, preview, validation and CORS
  * FileAPI Flash shim for old browsers not supporting FormData
  * @author  Danial  <danial.farid@gmail.com>
- * @version 12.0.4
+ * @version 12.2.13
  */
 
 (function() {
     /** @namespace FileAPI.noContentTimeout */
 
     function patchXHR(fnName, newFn) {
         window.XMLHttpRequest.prototype[fnName] = newFn(window.XMLHttpRequest.prototype[fnName]);
```

### Comparing `XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-shim.min.js` & `XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/ng-file-upload-shim.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! 12.0.4 */ ! function() {
+/*! 12.2.13 */ ! function() {
     function a(a, b) {
         window.XMLHttpRequest.prototype[a] = b(window.XMLHttpRequest.prototype[a])
     }
 
     function b(a, b, c) {
         try {
             Object.defineProperty(a, b, {
```

### Comparing `XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/ng-file-upload.js` & `XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/ng-file-upload.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 /**!
  * AngularJS file upload directives and services. Supoorts: file upload/drop/paste, resume, cancel/abort,
  * progress, resize, thumbnail, preview, validation and CORS
  * @author  Danial  <danial.farid@gmail.com>
- * @version 12.0.4
+ * @version 12.2.13
  */
 
 if (window.XMLHttpRequest && !(window.FileAPI && FileAPI.shouldLoad)) {
     window.XMLHttpRequest.prototype.setRequestHeader = (function(orig) {
         return function(header, value) {
             if (header === '__setXHR_') {
                 var val = value(this);
@@ -19,15 +19,15 @@
             }
         };
     })(window.XMLHttpRequest.prototype.setRequestHeader);
 }
 
 var ngFileUpload = angular.module('ngFileUpload', []);
 
-ngFileUpload.version = '12.0.4';
+ngFileUpload.version = '12.2.13';
 
 ngFileUpload.service('UploadBase', ['$http', '$q', '$timeout', function($http, $q, $timeout) {
         var upload = this;
         upload.promisesCount = 0;
 
         this.isResumeSupported = function() {
             return window.Blob && window.Blob.prototype.slice;
@@ -88,17 +88,18 @@
                     };
                 };
             }
 
             function uploadWithAngular() {
                 $http(config).then(function(r) {
                     if (resumeSupported && config._chunkSize && !config._finished && config._file) {
+                        var fileSize = config._file && config._file.size || 0;
                         notifyProgress({
-                            loaded: config._end,
-                            total: config._file && config._file.size,
+                            loaded: Math.min(config._end, fileSize),
+                            total: fileSize,
                             config: config,
                             type: 'progress'
                         });
                         upload.upload(config, true);
                     } else {
                         if (config._finished) delete config._finished;
                         deferred.resolve(r);
@@ -129,14 +130,17 @@
                     uploadWithAngular();
                 }, function(e) {
                     throw e;
                 });
             } else if (config.resumeSize) {
                 config.resumeSize().then(function(size) {
                     config._start = size;
+                    if (config._chunkSize) {
+                        config._end = config._start + config._chunkSize;
+                    }
                     uploadWithAngular();
                 }, function(e) {
                     throw e;
                 });
             } else {
                 if (config._chunkSize) {
                     config._start = 0;
@@ -182,17 +186,19 @@
                         fn.apply(promise, arguments);
                     };
                 })(config.xhrFn);
                 return promise;
             };
 
             upload.promisesCount++;
-            promise['finally'](function() {
-                upload.promisesCount--;
-            });
+            if (promise['finally'] && promise['finally'] instanceof Function) {
+                promise['finally'](function() {
+                    upload.promisesCount--;
+                });
+            }
             return promise;
         }
 
         this.isUploadInProgress = function() {
             return upload.promisesCount > 0;
         };
 
@@ -377,17 +383,19 @@
                 responseType: 'arraybuffer'
             }).then(function(resp) {
                 var arrayBufferView = new Uint8Array(resp.data);
                 var type = resp.headers('content-type') || 'image/WebP';
                 var blob = new window.Blob([arrayBufferView], {
                     type: type
                 });
+                var matches = url.match(/.*\/(.+?)(\?.*)?$/);
+                if (matches.length > 1) {
+                    blob.name = matches[1];
+                }
                 defer.resolve(blob);
-                //var split = type.split('[/;]');
-                //blob.name = url.substring(0, 150).replace(/\W+/g, '') + '.' + (split.length > 1 ? split[1] : 'jpg');
             }, function(e) {
                 defer.reject(e);
             });
             return defer.promise;
         };
 
         this.setDefaults = function(defaults) {
@@ -427,15 +435,15 @@
             }
         } else {
             return attrVal;
         }
     };
 
     upload.shouldUpdateOn = function(type, attr, scope) {
-        var modelOptions = upload.attrGetter('ngModelOptions', attr, scope);
+        var modelOptions = upload.attrGetter('ngfModelOptions', attr, scope);
         if (modelOptions && modelOptions.updateOn) {
             return modelOptions.updateOn.split(' ').indexOf(type) > -1;
         }
         return true;
     };
 
     upload.emptyPromise = function() {
@@ -479,54 +487,59 @@
                     files.splice(i, 1, fixedFile);
                 }));
             }
         });
         return $q.all(promises);
     }
 
-    function resize(files, attr, scope) {
+    function resizeFile(files, attr, scope, ngModel) {
         var resizeVal = upload.attrGetter('ngfResize', attr, scope);
         if (!resizeVal || !upload.isResizeSupported() || !files.length) return upload.emptyPromise();
         if (resizeVal instanceof Function) {
             var defer = $q.defer();
-            resizeVal(files).then(function(p) {
-                resizeWithParams(p, files, attr, scope).then(function(r) {
+            return resizeVal(files).then(function(p) {
+                resizeWithParams(p, files, attr, scope, ngModel).then(function(r) {
                     defer.resolve(r);
                 }, function(e) {
                     defer.reject(e);
                 });
             }, function(e) {
                 defer.reject(e);
             });
         } else {
-            return resizeWithParams(resizeVal, files, attr, scope);
+            return resizeWithParams(resizeVal, files, attr, scope, ngModel);
         }
     }
 
-    function resizeWithParams(param, files, attr, scope) {
+    function resizeWithParams(params, files, attr, scope, ngModel) {
         var promises = [upload.emptyPromise()];
 
         function handleFile(f, i) {
             if (f.type.indexOf('image') === 0) {
-                if (param.pattern && !upload.validatePattern(f, param.pattern)) return;
-                var promise = upload.resize(f, param.width, param.height, param.quality,
-                    param.type, param.ratio, param.centerCrop,
-                    function(width, height) {
-                        return upload.attrGetter('ngfResizeIf', attr, scope, {
-                            $width: width,
-                            $height: height,
-                            $file: f
-                        });
-                    }, param.restoreExif !== false);
+                if (params.pattern && !upload.validatePattern(f, params.pattern)) return;
+                params.resizeIf = function(width, height) {
+                    return upload.attrGetter('ngfResizeIf', attr, scope, {
+                        $width: width,
+                        $height: height,
+                        $file: f
+                    });
+                };
+                var promise = upload.resize(f, params);
                 promises.push(promise);
                 promise.then(function(resizedFile) {
                     files.splice(i, 1, resizedFile);
                 }, function(e) {
                     f.$error = 'resize';
+                    (f.$errorMessages = (f.$errorMessages || {})).resize = true;
                     f.$errorParam = (e ? (e.message ? e.message : e) + ': ' : '') + (f && f.name);
+                    ngModel.$ngfValidations.push({
+                        name: 'resize',
+                        valid: false
+                    });
+                    upload.applyModelValidation(ngModel, files);
                 });
             }
         }
 
         for (var i = 0; i < files.length; i++) {
             handleFile(files[i], i);
         }
@@ -607,46 +620,47 @@
             }
         }
 
         function toArray(v) {
             return angular.isArray(v) ? v : [v];
         }
 
-        function separateInvalids() {
-            valids = [];
-            invalids = [];
-            angular.forEach(allNewFiles, function(file) {
-                if (file.$error) {
-                    invalids.push(file);
-                } else {
-                    valids.push(file);
-                }
-            });
-        }
-
         function resizeAndUpdate() {
             function updateModel() {
                 $timeout(function() {
                     update(keep ? prevValidFiles.concat(valids) : valids,
                         keep ? prevInvalidFiles.concat(invalids) : invalids,
                         files, dupFiles, isSingleModel);
                 }, options && options.debounce ? options.debounce.change || options.debounce : 0);
             }
 
-            resize(validateAfterResize ? allNewFiles : valids, attr, scope).then(function() {
+            var resizingFiles = validateAfterResize ? allNewFiles : valids;
+            resizeFile(resizingFiles, attr, scope, ngModel).then(function() {
                 if (validateAfterResize) {
-                    upload.validate(allNewFiles, prevValidFiles.length, ngModel, attr, scope).then(function() {
-                        separateInvalids();
-                        updateModel();
-                    });
+                    upload.validate(allNewFiles, keep ? prevValidFiles.length : 0, ngModel, attr, scope)
+                        .then(function(validationResult) {
+                            valids = validationResult.validsFiles;
+                            invalids = validationResult.invalidsFiles;
+                            updateModel();
+                        });
                 } else {
                     updateModel();
                 }
-            }, function(e) {
-                throw 'Could not resize files ' + e;
+            }, function() {
+                for (var i = 0; i < resizingFiles.length; i++) {
+                    var f = resizingFiles[i];
+                    if (f.$error === 'resize') {
+                        var index = valids.indexOf(f);
+                        if (index > -1) {
+                            valids.splice(index, 1);
+                            invalids.push(f);
+                        }
+                        updateModel();
+                    }
+                }
             });
         }
 
         prevValidFiles = attr.$$ngfPrevValidFiles || [];
         prevInvalidFiles = attr.$$ngfPrevInvalidFiles || [];
         if (ngModel && ngModel.$modelValue) {
             prevValidFiles = toArray(ngModel.$modelValue);
@@ -668,33 +682,35 @@
             $newFiles: allNewFiles,
             $duplicateFiles: dupFiles,
             $event: evt
         });
 
         var validateAfterResize = upload.attrGetter('ngfValidateAfterResize', attr, scope);
 
-        var options = upload.attrGetter('ngModelOptions', attr, scope);
-        upload.validate(allNewFiles, prevValidFiles.length, ngModel, attr, scope).then(function() {
-            if (noDelay) {
-                update(allNewFiles, [], files, dupFiles, isSingleModel);
-            } else {
-                if ((!options || !options.allowInvalid) && !validateAfterResize) {
-                    separateInvalids();
+        var options = upload.attrGetter('ngfModelOptions', attr, scope);
+        upload.validate(allNewFiles, keep ? prevValidFiles.length : 0, ngModel, attr, scope)
+            .then(function(validationResult) {
+                if (noDelay) {
+                    update(allNewFiles, [], files, dupFiles, isSingleModel);
                 } else {
-                    valids = allNewFiles;
-                }
-                if (upload.attrGetter('ngfFixOrientation', attr, scope) && upload.isExifSupported()) {
-                    applyExifRotations(valids, attr, scope).then(function() {
+                    if ((!options || !options.allowInvalid) && !validateAfterResize) {
+                        valids = validationResult.validFiles;
+                        invalids = validationResult.invalidFiles;
+                    } else {
+                        valids = allNewFiles;
+                    }
+                    if (upload.attrGetter('ngfFixOrientation', attr, scope) && upload.isExifSupported()) {
+                        applyExifRotations(valids, attr, scope).then(function() {
+                            resizeAndUpdate();
+                        });
+                    } else {
                         resizeAndUpdate();
-                    });
-                } else {
-                    resizeAndUpdate();
+                    }
                 }
-            }
-        });
+            });
     };
 
     return upload;
 }]);
 
 ngFileUpload.directive('ngfSelect', ['$parse', '$timeout', '$compile', 'Upload', function($parse, $timeout, $compile, Upload) {
     var generatedElems = [];
@@ -711,15 +727,15 @@
         return ua.indexOf('Chrome') === -1 && /.*Windows.*Safari.*/.test(ua);
     }
 
     function linkFileSelect(scope, elem, attr, ngModel, $parse, $timeout, $compile, upload) {
         /** @namespace attr.ngfSelect */
         /** @namespace attr.ngfChange */
         /** @namespace attr.ngModel */
-        /** @namespace attr.ngModelOptions */
+        /** @namespace attr.ngfModelOptions */
         /** @namespace attr.ngfMultiple */
         /** @namespace attr.ngfCapture */
         /** @namespace attr.ngfValidate */
         /** @namespace attr.ngfKeep */
         var attrGetter = function(name, scope) {
             return upload.attrGetter(name, attr, scope);
         };
@@ -732,86 +748,95 @@
             return attrGetter('ngfChange') || attrGetter('ngfSelect');
         }
 
         function changeFn(evt) {
             if (upload.shouldUpdateOn('change', attr, scope)) {
                 var fileList = evt.__files_ || (evt.target && evt.target.files),
                     files = [];
+                /* Handle duplicate call in  IE11 */
+                if (!fileList) return;
                 for (var i = 0; i < fileList.length; i++) {
                     files.push(fileList[i]);
                 }
                 upload.updateModel(ngModel, attr, scope, fileChangeAttr(),
                     files.length ? files : null, evt);
             }
         }
 
         upload.registerModelChangeValidator(ngModel, attr, scope);
 
         var unwatches = [];
-        unwatches.push(scope.$watch(attrGetter('ngfMultiple'), function() {
-            fileElem.attr('multiple', attrGetter('ngfMultiple', scope));
-        }));
-        unwatches.push(scope.$watch(attrGetter('ngfCapture'), function() {
-            fileElem.attr('capture', attrGetter('ngfCapture', scope));
-        }));
-        unwatches.push(scope.$watch(attrGetter('ngfAccept'), function() {
-            fileElem.attr('accept', attrGetter('ngfAccept', scope));
-        }));
-        attr.$observe('accept', function() {
+        if (attrGetter('ngfMultiple')) {
+            unwatches.push(scope.$watch(attrGetter('ngfMultiple'), function() {
+                fileElem.attr('multiple', attrGetter('ngfMultiple', scope));
+            }));
+        }
+        if (attrGetter('ngfCapture')) {
+            unwatches.push(scope.$watch(attrGetter('ngfCapture'), function() {
+                fileElem.attr('capture', attrGetter('ngfCapture', scope));
+            }));
+        }
+        if (attrGetter('ngfAccept')) {
+            unwatches.push(scope.$watch(attrGetter('ngfAccept'), function() {
+                fileElem.attr('accept', attrGetter('ngfAccept', scope));
+            }));
+        }
+        unwatches.push(attr.$observe('accept', function() {
             fileElem.attr('accept', attrGetter('accept'));
-        });
-        unwatches.push(function() {
-            if (attr.$$observers) delete attr.$$observers.accept;
-        });
+        }));
 
-        function bindAttrToFileInput(fileElem) {
-            if (elem !== fileElem) {
-                for (var i = 0; i < elem[0].attributes.length; i++) {
-                    var attribute = elem[0].attributes[i];
-                    if (attribute.name !== 'type' && attribute.name !== 'class' && attribute.name !== 'style') {
-                        if (attribute.value == null || attribute.value === '') {
-                            if (attribute.name === 'required') attribute.value = 'required';
-                            if (attribute.name === 'multiple') attribute.value = 'multiple';
-                        }
-                        fileElem.attr(attribute.name, attribute.name === 'id' ? 'ngf-' + attribute.value : attribute.value);
+        function bindAttrToFileInput(fileElem, label) {
+            function updateId(val) {
+                fileElem.attr('id', 'ngf-' + val);
+                label.attr('id', 'ngf-label-' + val);
+            }
+
+            for (var i = 0; i < elem[0].attributes.length; i++) {
+                var attribute = elem[0].attributes[i];
+                if (attribute.name !== 'type' && attribute.name !== 'class' && attribute.name !== 'style') {
+                    if (attribute.name === 'id') {
+                        updateId(attribute.value);
+                        unwatches.push(attr.$observe('id', updateId));
+                    } else {
+                        fileElem.attr(attribute.name, (!attribute.value && (attribute.name === 'required' ||
+                            attribute.name === 'multiple')) ? attribute.name : attribute.value);
                     }
                 }
             }
         }
 
         function createFileInput() {
             if (isInputTypeFile()) {
                 return elem;
             }
 
             var fileElem = angular.element('<input type="file">');
 
-            bindAttrToFileInput(fileElem);
-
             var label = angular.element('<label>upload</label>');
             label.css('visibility', 'hidden').css('position', 'absolute').css('overflow', 'hidden')
                 .css('width', '0px').css('height', '0px').css('border', 'none')
                 .css('margin', '0px').css('padding', '0px').attr('tabindex', '-1');
+            bindAttrToFileInput(fileElem, label);
+
             generatedElems.push({
                 el: elem,
                 ref: label
             });
 
             document.body.appendChild(label.append(fileElem)[0]);
 
             return fileElem;
         }
 
-        var initialTouchStartY = 0;
-
         function clickHandler(evt) {
             if (elem.attr('disabled')) return false;
             if (attrGetter('ngfSelectDisabled', scope)) return;
 
-            var r = handleTouch(evt);
+            var r = detectSwipe(evt);
+            // prevent the click if it is a swipe
             if (r != null) return r;
 
             resetModel(evt);
 
             // fix for md when the element is removed from the DOM and added back #460
             try {
                 if (!isInputTypeFile() && !document.body.contains(fileElem[0])) {
@@ -832,27 +857,38 @@
             } else {
                 fileElem[0].click();
             }
 
             return false;
         }
 
-        function handleTouch(evt) {
-            var touches = evt.changedTouches || (evt.originalEvent && evt.originalEvent.changedTouches);
-            if (evt.type === 'touchstart') {
-                initialTouchStartY = touches ? touches[0].clientY : 0;
-                return true; // don't block event default
-            } else {
-                evt.stopPropagation();
-                evt.preventDefault();
 
-                // prevent scroll from triggering event
-                if (evt.type === 'touchend') {
-                    var currentLocation = touches ? touches[0].clientY : 0;
-                    if (Math.abs(currentLocation - initialTouchStartY) > 20) return false;
+        var initialTouchStartY = 0;
+        var initialTouchStartX = 0;
+
+        function detectSwipe(evt) {
+            var touches = evt.changedTouches || (evt.originalEvent && evt.originalEvent.changedTouches);
+            if (touches) {
+                if (evt.type === 'touchstart') {
+                    initialTouchStartX = touches[0].clientX;
+                    initialTouchStartY = touches[0].clientY;
+                    return true; // don't block event default
+                } else {
+                    // prevent scroll from triggering event
+                    if (evt.type === 'touchend') {
+                        var currentX = touches[0].clientX;
+                        var currentY = touches[0].clientY;
+                        if ((Math.abs(currentX - initialTouchStartX) > 20) ||
+                            (Math.abs(currentY - initialTouchStartY) > 20)) {
+                            evt.stopPropagation();
+                            evt.preventDefault();
+                            return false;
+                        }
+                    }
+                    return true;
                 }
             }
         }
 
         var fileElem = elem;
 
         function resetModel(evt) {
@@ -1080,39 +1116,48 @@
 
         $timeout(function() {
             var unwatch = scope.$watch(attr[directiveName], function(file) {
                 var size = resizeParams;
                 if (directiveName === 'ngfThumbnail') {
                     if (!size) {
                         size = {
-                            width: elem[0].clientWidth,
-                            height: elem[0].clientHeight
+                            width: elem[0].naturalWidth || elem[0].clientWidth,
+                            height: elem[0].naturalHeight || elem[0].clientHeight
                         };
                     }
                     if (size.width === 0 && window.getComputedStyle) {
                         var style = getComputedStyle(elem[0]);
-                        size = {
-                            width: parseInt(style.width.slice(0, -2)),
-                            height: parseInt(style.height.slice(0, -2))
-                        };
+                        if (style.width && style.width.indexOf('px') > -1 && style.height && style.height.indexOf('px') > -1) {
+                            size = {
+                                width: parseInt(style.width.slice(0, -2)),
+                                height: parseInt(style.height.slice(0, -2))
+                            };
+                        }
                     }
                 }
 
                 if (angular.isString(file)) {
                     elem.removeClass('ng-hide');
                     if (isBackground) {
                         return elem.css('background-image', 'url(\'' + file + '\')');
                     } else {
                         return elem.attr('src', file);
                     }
                 }
                 if (file && file.type && file.type.search(getTagType(elem[0])) === 0 &&
                     (!isBackground || file.type.indexOf('image') === 0)) {
                     if (size && Upload.isResizeSupported()) {
-                        Upload.resize(file, size.width, size.height, size.quality).then(
+                        size.resizeIf = function(width, height) {
+                            return Upload.attrGetter('ngfResizeIf', attr, scope, {
+                                $width: width,
+                                $height: height,
+                                $file: file
+                            });
+                        };
+                        Upload.resize(file, size).then(
                             function(f) {
                                 constructDataUrl(f);
                             },
                             function(e) {
                                 throw e;
                             }
                         );
@@ -1167,16 +1212,16 @@
                 linkFileDirective(Upload, $timeout, scope, elem, attr, 'ngfThumbnail', size,
                     Upload.attrGetter('ngfAsBackground', attr, scope));
             }
         };
     }]);
 
     ngFileUpload.config(['$compileProvider', function($compileProvider) {
-        if ($compileProvider.imgSrcSanitizationWhitelist) $compileProvider.imgSrcSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|local|file|data|blob):/);
-        if ($compileProvider.aHrefSanitizationWhitelist) $compileProvider.aHrefSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|local|file|data|blob):/);
+        if ($compileProvider.imgSrcSanitizationWhitelist) $compileProvider.imgSrcSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|webcal|local|file|data|blob):/);
+        if ($compileProvider.aHrefSanitizationWhitelist) $compileProvider.aHrefSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|webcal|local|file|data|blob):/);
     }]);
 
     ngFileUpload.filter('ngfDataUrl', ['UploadDataUrl', '$sce', function(UploadDataUrl, $sce) {
         return function(file, disallowObjectUrl, trustedUrl) {
             if (angular.isString(file)) {
                 return $sce.trustAsResourceUrl(file);
             }
@@ -1266,21 +1311,23 @@
         return r;
     };
 
     upload.registerModelChangeValidator = function(ngModel, attr, scope) {
         if (ngModel) {
             ngModel.$formatters.push(function(files) {
                 if (ngModel.$dirty) {
+                    var filesArray = files;
                     if (files && !angular.isArray(files)) {
-                        files = [files];
+                        filesArray = [files];
                     }
-                    upload.validate(files, 0, ngModel, attr, scope).then(function() {
-                        upload.applyModelValidation(ngModel, files);
+                    upload.validate(filesArray, 0, ngModel, attr, scope).then(function() {
+                        upload.applyModelValidation(ngModel, filesArray);
                     });
                 }
+                return files;
             });
         }
     };
 
     function markModelAsDirty(ngModel, files) {
         if (files != null && !ngModel.$dirty) {
             if (ngModel.$setDirty) {
@@ -1326,51 +1373,64 @@
             v.valid = true;
         });
 
         var attrGetter = function(name, params) {
             return upload.attrGetter(name, attr, scope, params);
         };
 
+        var ignoredErrors = (upload.attrGetter('ngfIgnoreInvalid', attr, scope) || '').split(' ');
+        var runAllValidation = upload.attrGetter('ngfRunAllValidations', attr, scope);
+
         if (files == null || files.length === 0) {
-            return upload.emptyPromise(ngModel);
+            return upload.emptyPromise({
+                'validFiles': files,
+                'invalidFiles': []
+            });
         }
 
         files = files.length === undefined ? [files] : files.slice(0);
+        var invalidFiles = [];
 
         function validateSync(name, validationName, fn) {
             if (files) {
                 var i = files.length,
                     valid = null;
                 while (i--) {
                     var file = files[i];
                     if (file) {
                         var val = upload.getValidationAttr(attr, scope, name, validationName, file);
                         if (val != null) {
                             if (!fn(file, val, i)) {
-                                file.$error = name;
-                                (file.$errorMessages = (file.$errorMessages || {}))[name] = true;
-                                file.$errorParam = val;
-                                files.splice(i, 1);
-                                valid = false;
+                                if (ignoredErrors.indexOf(name) === -1) {
+                                    file.$error = name;
+                                    (file.$errorMessages = (file.$errorMessages || {}))[name] = true;
+                                    file.$errorParam = val;
+                                    if (invalidFiles.indexOf(file) === -1) {
+                                        invalidFiles.push(file);
+                                    }
+                                    if (!runAllValidation) {
+                                        files.splice(i, 1);
+                                    }
+                                    valid = false;
+                                } else {
+                                    files.splice(i, 1);
+                                }
                             }
                         }
                     }
                 }
                 if (valid !== null) {
                     ngModel.$ngfValidations.push({
                         name: name,
                         valid: valid
                     });
                 }
             }
         }
 
-        validateSync('maxFiles', null, function(file, val, i) {
-            return prevLength + i < val;
-        });
         validateSync('pattern', null, upload.validatePattern);
         validateSync('minSize', 'size.min', function(file, val) {
             return file.size + 0.1 >= upload.translateScalars(val);
         });
         validateSync('maxSize', 'size.max', function(file, val) {
             return file.size - 0.1 <= upload.translateScalars(val);
         });
@@ -1385,177 +1445,218 @@
         });
 
         validateSync('validateFn', null, function(file, r) {
             return r === true || r === null || r === '';
         });
 
         if (!files.length) {
-            return upload.emptyPromise(ngModel, ngModel.$ngfValidations);
+            return upload.emptyPromise({
+                'validFiles': [],
+                'invalidFiles': invalidFiles
+            });
         }
 
         function validateAsync(name, validationName, type, asyncFn, fn) {
             function resolveResult(defer, file, val) {
-                if (val != null) {
-                    asyncFn(file, val).then(function(d) {
-                        if (!fn(d, val)) {
+                function resolveInternal(fn) {
+                    if (fn()) {
+                        if (ignoredErrors.indexOf(name) === -1) {
                             file.$error = name;
                             (file.$errorMessages = (file.$errorMessages || {}))[name] = true;
                             file.$errorParam = val;
-                            defer.reject();
+                            if (invalidFiles.indexOf(file) === -1) {
+                                invalidFiles.push(file);
+                            }
+                            if (!runAllValidation) {
+                                var i = files.indexOf(file);
+                                if (i > -1) files.splice(i, 1);
+                            }
+                            defer.resolve(false);
                         } else {
-                            defer.resolve();
+                            var j = files.indexOf(file);
+                            if (j > -1) files.splice(j, 1);
+                            defer.resolve(true);
                         }
+                    } else {
+                        defer.resolve(true);
+                    }
+                }
+
+                if (val != null) {
+                    asyncFn(file, val).then(function(d) {
+                        resolveInternal(function() {
+                            return !fn(d, val);
+                        });
                     }, function() {
-                        if (attrGetter('ngfValidateForce', {
+                        resolveInternal(function() {
+                            return attrGetter('ngfValidateForce', {
                                 $file: file
-                            })) {
-                            file.$error = name;
-                            (file.$errorMessages = (file.$errorMessages || {}))[name] = true;
-                            file.$errorParam = val;
-                            defer.reject();
-                        } else {
-                            defer.resolve();
-                        }
+                            });
+                        });
                     });
                 } else {
-                    defer.resolve();
+                    defer.resolve(true);
                 }
             }
 
-            var promises = [upload.emptyPromise()];
+            var promises = [upload.emptyPromise(true)];
             if (files) {
                 files = files.length === undefined ? [files] : files;
                 angular.forEach(files, function(file) {
                     var defer = $q.defer();
                     promises.push(defer.promise);
                     if (type && (file.type == null || file.type.search(type) !== 0)) {
-                        defer.resolve();
+                        defer.resolve(true);
                         return;
                     }
                     if (name === 'dimensions' && upload.attrGetter('ngfDimensions', attr) != null) {
                         upload.imageDimensions(file).then(function(d) {
                             resolveResult(defer, file,
                                 attrGetter('ngfDimensions', {
                                     $file: file,
                                     $width: d.width,
                                     $height: d.height
                                 }));
                         }, function() {
-                            defer.reject();
+                            defer.resolve(false);
                         });
                     } else if (name === 'duration' && upload.attrGetter('ngfDuration', attr) != null) {
                         upload.mediaDuration(file).then(function(d) {
                             resolveResult(defer, file,
                                 attrGetter('ngfDuration', {
                                     $file: file,
                                     $duration: d
                                 }));
                         }, function() {
-                            defer.reject();
+                            defer.resolve(false);
                         });
                     } else {
                         resolveResult(defer, file,
                             upload.getValidationAttr(attr, scope, name, validationName, file));
                     }
                 });
-                return $q.all(promises).then(function() {
-                    ngModel.$ngfValidations.push({
-                        name: name,
-                        valid: true
-                    });
-                }, function() {
-                    ngModel.$ngfValidations.push({
-                        name: name,
-                        valid: false
-                    });
-                });
             }
+            var deffer = $q.defer();
+            $q.all(promises).then(function(values) {
+                var isValid = true;
+                for (var i = 0; i < values.length; i++) {
+                    if (!values[i]) {
+                        isValid = false;
+                        break;
+                    }
+                }
+                ngModel.$ngfValidations.push({
+                    name: name,
+                    valid: isValid
+                });
+                deffer.resolve(isValid);
+            });
+            return deffer.promise;
         }
 
         var deffer = $q.defer();
         var promises = [];
 
-        promises.push(upload.happyPromise(validateAsync('maxHeight', 'height.max', /image/,
+        promises.push(validateAsync('maxHeight', 'height.max', /image/,
             this.imageDimensions,
             function(d, val) {
                 return d.height <= val;
-            })));
-        promises.push(upload.happyPromise(validateAsync('minHeight', 'height.min', /image/,
+            }));
+        promises.push(validateAsync('minHeight', 'height.min', /image/,
             this.imageDimensions,
             function(d, val) {
                 return d.height >= val;
-            })));
-        promises.push(upload.happyPromise(validateAsync('maxWidth', 'width.max', /image/,
+            }));
+        promises.push(validateAsync('maxWidth', 'width.max', /image/,
             this.imageDimensions,
             function(d, val) {
                 return d.width <= val;
-            })));
-        promises.push(upload.happyPromise(validateAsync('minWidth', 'width.min', /image/,
+            }));
+        promises.push(validateAsync('minWidth', 'width.min', /image/,
             this.imageDimensions,
             function(d, val) {
                 return d.width >= val;
-            })));
-        promises.push(upload.happyPromise(validateAsync('dimensions', null, /image/,
+            }));
+        promises.push(validateAsync('dimensions', null, /image/,
             function(file, val) {
                 return upload.emptyPromise(val);
             },
             function(r) {
                 return r;
-            })));
-        promises.push(upload.happyPromise(validateAsync('ratio', null, /image/,
+            }));
+        promises.push(validateAsync('ratio', null, /image/,
             this.imageDimensions,
             function(d, val) {
                 var split = val.toString().split(','),
                     valid = false;
                 for (var i = 0; i < split.length; i++) {
-                    if (Math.abs((d.width / d.height) - upload.ratioToFloat(split[i])) < 0.0001) {
+                    if (Math.abs((d.width / d.height) - upload.ratioToFloat(split[i])) < 0.01) {
                         valid = true;
                     }
                 }
                 return valid;
-            })));
-        promises.push(upload.happyPromise(validateAsync('maxRatio', 'ratio.max', /image/,
+            }));
+        promises.push(validateAsync('maxRatio', 'ratio.max', /image/,
             this.imageDimensions,
             function(d, val) {
                 return (d.width / d.height) - upload.ratioToFloat(val) < 0.0001;
-            })));
-        promises.push(upload.happyPromise(validateAsync('minRatio', 'ratio.min', /image/,
+            }));
+        promises.push(validateAsync('minRatio', 'ratio.min', /image/,
             this.imageDimensions,
             function(d, val) {
                 return (d.width / d.height) - upload.ratioToFloat(val) > -0.0001;
-            })));
-        promises.push(upload.happyPromise(validateAsync('maxDuration', 'duration.max', /audio|video/,
+            }));
+        promises.push(validateAsync('maxDuration', 'duration.max', /audio|video/,
             this.mediaDuration,
             function(d, val) {
                 return d <= upload.translateScalars(val);
-            })));
-        promises.push(upload.happyPromise(validateAsync('minDuration', 'duration.min', /audio|video/,
+            }));
+        promises.push(validateAsync('minDuration', 'duration.min', /audio|video/,
             this.mediaDuration,
             function(d, val) {
                 return d >= upload.translateScalars(val);
-            })));
-        promises.push(upload.happyPromise(validateAsync('duration', null, /audio|video/,
+            }));
+        promises.push(validateAsync('duration', null, /audio|video/,
             function(file, val) {
                 return upload.emptyPromise(val);
             },
             function(r) {
                 return r;
-            })));
+            }));
 
-        promises.push(upload.happyPromise(validateAsync('validateAsyncFn', null, null,
+        promises.push(validateAsync('validateAsyncFn', null, null,
             function(file, val) {
                 return val;
             },
             function(r) {
                 return r === true || r === null || r === '';
-            })));
+            }));
+
+        $q.all(promises).then(function() {
+
+            if (runAllValidation) {
+                for (var i = 0; i < files.length; i++) {
+                    var file = files[i];
+                    if (file.$error) {
+                        files.splice(i--, 1);
+                    }
+                }
+            }
 
-        return $q.all(promises).then(function() {
-            deffer.resolve(ngModel, ngModel.$ngfValidations);
+            runAllValidation = false;
+            validateSync('maxFiles', null, function(file, val, i) {
+                return prevLength + i < val;
+            });
+
+            deffer.resolve({
+                'validFiles': files,
+                'invalidFiles': invalidFiles
+            });
         });
+        return deffer.promise;
     };
 
     upload.imageDimensions = function(file) {
         if (file.$ngfWidth && file.$ngfHeight) {
             var d = $q.defer();
             $timeout(function() {
                 d.resolve({
@@ -1575,16 +1676,16 @@
             }
             upload.dataUrl(file).then(function(dataUrl) {
                 var img = angular.element('<img>').attr('src', dataUrl)
                     .css('visibility', 'hidden').css('position', 'fixed')
                     .css('max-width', 'none !important').css('max-height', 'none !important');
 
                 function success() {
-                    var width = img[0].clientWidth;
-                    var height = img[0].clientHeight;
+                    var width = img[0].naturalWidth || img[0].clientWidth;
+                    var height = img[0].naturalHeight || img[0].clientHeight;
                     img.remove();
                     file.$ngfWidth = width;
                     file.$ngfHeight = height;
                     deferred.resolve({
                         width: width,
                         height: height
                     });
@@ -1593,31 +1694,32 @@
                 function error() {
                     img.remove();
                     deferred.reject('load error');
                 }
 
                 img.on('load', success);
                 img.on('error', error);
-                var count = 0;
 
-                function checkLoadError() {
+                var secondsCounter = 0;
+
+                function checkLoadErrorInCaseOfNoCallback() {
                     $timeout(function() {
                         if (img[0].parentNode) {
                             if (img[0].clientWidth) {
                                 success();
-                            } else if (count > 10) {
+                            } else if (secondsCounter++ > 10) {
                                 error();
                             } else {
-                                checkLoadError();
+                                checkLoadErrorInCaseOfNoCallback();
                             }
                         }
                     }, 1000);
                 }
 
-                checkLoadError();
+                checkLoadErrorInCaseOfNoCallback();
 
                 angular.element(document.getElementsByTagName('body')[0]).append(img);
             }, function() {
                 deferred.reject('load error');
             });
         });
 
@@ -1721,51 +1823,57 @@
     };
 
     // Extracted from https://github.com/romelgomez/angular-firebase-image-upload/blob/master/app/scripts/fileUpload.js#L89
     var resize = function(imagen, width, height, quality, type, ratio, centerCrop, resizeIf) {
         var deferred = $q.defer();
         var canvasElement = document.createElement('canvas');
         var imageElement = document.createElement('img');
+        imageElement.setAttribute('style', 'visibility:hidden;position:fixed;z-index:-100000');
+        document.body.appendChild(imageElement);
 
         imageElement.onload = function() {
-            if (resizeIf != null && resizeIf(imageElement.width, imageElement.height) === false) {
+            var imgWidth = imageElement.width,
+                imgHeight = imageElement.height;
+            imageElement.parentNode.removeChild(imageElement);
+            if (resizeIf != null && resizeIf(imgWidth, imgHeight) === false) {
                 deferred.reject('resizeIf');
                 return;
             }
             try {
                 if (ratio) {
                     var ratioFloat = upload.ratioToFloat(ratio);
-                    var imgRatio = imageElement.width / imageElement.height;
+                    var imgRatio = imgWidth / imgHeight;
                     if (imgRatio < ratioFloat) {
-                        width = imageElement.width;
+                        width = imgWidth;
                         height = width / ratioFloat;
                     } else {
-                        height = imageElement.height;
+                        height = imgHeight;
                         width = height * ratioFloat;
                     }
                 }
                 if (!width) {
-                    width = imageElement.width;
+                    width = imgWidth;
                 }
                 if (!height) {
-                    height = imageElement.height;
+                    height = imgHeight;
                 }
-                var dimensions = calculateAspectRatioFit(imageElement.width, imageElement.height, width, height, centerCrop);
+                var dimensions = calculateAspectRatioFit(imgWidth, imgHeight, width, height, centerCrop);
                 canvasElement.width = Math.min(dimensions.width, width);
                 canvasElement.height = Math.min(dimensions.height, height);
                 var context = canvasElement.getContext('2d');
                 context.drawImage(imageElement,
                     Math.min(0, -dimensions.marginX / 2), Math.min(0, -dimensions.marginY / 2),
                     dimensions.width, dimensions.height);
                 deferred.resolve(canvasElement.toDataURL(type || 'image/WebP', quality || 0.934));
             } catch (e) {
                 deferred.reject(e);
             }
         };
         imageElement.onerror = function() {
+            imageElement.parentNode.removeChild(imageElement);
             deferred.reject();
         };
         imageElement.src = imagen;
         return deferred.promise;
     };
 
     upload.dataUrltoBlob = function(dataurl, name, origSize) {
@@ -1799,22 +1907,23 @@
             set: function(v) {
                 this.$ngfName = v;
             },
             configurable: true
         });
     }
 
-    upload.resize = function(file, width, height, quality, type, ratio, centerCrop, resizeIf, restoreExif) {
+    upload.resize = function(file, options) {
         if (file.type.indexOf('image') !== 0) return upload.emptyPromise(file);
 
         var deferred = $q.defer();
         upload.dataUrl(file, true).then(function(url) {
-            resize(url, width, height, quality, type || file.type, ratio, centerCrop, resizeIf)
+            resize(url, options.width, options.height, options.quality, options.type || file.type,
+                    options.ratio, options.centerCrop, options.resizeIf)
                 .then(function(dataUrl) {
-                    if (file.type === 'image/jpeg' && restoreExif) {
+                    if (file.type === 'image/jpeg' && options.restoreExif !== false) {
                         try {
                             dataUrl = upload.restoreExif(url, dataUrl);
                         } catch (e) {
                             setTimeout(function() {
                                 throw e;
                             }, 1);
                         }
@@ -1837,21 +1946,21 @@
         return deferred.promise;
     };
 
     return upload;
 }]);
 
 (function() {
-    ngFileUpload.directive('ngfDrop', ['$parse', '$timeout', '$location', 'Upload', '$http', '$q',
-        function($parse, $timeout, $location, Upload, $http, $q) {
+    ngFileUpload.directive('ngfDrop', ['$parse', '$timeout', '$window', 'Upload', '$http', '$q',
+        function($parse, $timeout, $window, Upload, $http, $q) {
             return {
                 restrict: 'AEC',
                 require: '?ngModel',
                 link: function(scope, elem, attr, ngModel) {
-                    linkDrop(scope, elem, attr, ngModel, $parse, $timeout, $location, Upload, $http, $q);
+                    linkDrop(scope, elem, attr, ngModel, $parse, $timeout, $window, Upload, $http, $q);
                 }
             };
         }
     ]);
 
     ngFileUpload.directive('ngfNoFileDrop', function() {
         return function(scope, elem) {
@@ -1869,15 +1978,15 @@
                         model.assign(scope, true);
                     }
                 });
             }
         };
     }]);
 
-    function linkDrop(scope, elem, attr, ngModel, $parse, $timeout, $location, upload, $http, $q) {
+    function linkDrop(scope, elem, attr, ngModel, $parse, $timeout, $window, upload, $http, $q) {
         var available = dropAvailable();
 
         var attrGetter = function(name, scope, params) {
             return upload.attrGetter(name, attr, scope, params);
         };
 
         if (attrGetter('dropAvailable')) {
@@ -1952,72 +2061,62 @@
         }, false);
         elem[0].addEventListener('drop', function(evt) {
             if (isDisabled() || !upload.shouldUpdateOn('drop', attr, scope)) return;
             evt.preventDefault();
             if (stopPropagation(scope)) evt.stopPropagation();
             if (actualDragOverClass) elem.removeClass(actualDragOverClass);
             actualDragOverClass = null;
-            var items = evt.dataTransfer.items;
-            var html;
-            try {
-                html = evt.dataTransfer && evt.dataTransfer.getData && evt.dataTransfer.getData('text/html');
-            } catch (e) {
-                /* Fix IE11 that throw error calling getData */ }
-
-            extractFiles(items, evt.dataTransfer.files, attrGetter('ngfAllowDir', scope) !== false,
-                attrGetter('multiple') || attrGetter('ngfMultiple', scope)).then(function(files) {
-                if (files.length) {
-                    updateModel(files, evt);
-                } else {
-                    extractFilesFromHtml('dropUrl', html).then(function(files) {
-                        updateModel(files, evt);
-                    });
-                }
-            });
+            extractFilesAndUpdateModel(evt.dataTransfer, evt, 'dropUrl');
         }, false);
         elem[0].addEventListener('paste', function(evt) {
             if (navigator.userAgent.toLowerCase().indexOf('firefox') > -1 &&
                 attrGetter('ngfEnableFirefoxPaste', scope)) {
                 evt.preventDefault();
             }
             if (isDisabled() || !upload.shouldUpdateOn('paste', attr, scope)) return;
-            var files = [];
-            var clipboard = evt.clipboardData || evt.originalEvent.clipboardData;
-            if (clipboard && clipboard.items) {
-                for (var k = 0; k < clipboard.items.length; k++) {
-                    if (clipboard.items[k].type.indexOf('image') !== -1) {
-                        files.push(clipboard.items[k].getAsFile());
-                    }
-                }
-            }
-            if (files.length) {
-                updateModel(files, evt);
-            } else {
-                extractFilesFromHtml('pasteUrl', clipboard).then(function(files) {
-                    updateModel(files, evt);
-                });
-            }
+            extractFilesAndUpdateModel(evt.clipboardData || evt.originalEvent.clipboardData, evt, 'pasteUrl');
         }, false);
 
         if (navigator.userAgent.toLowerCase().indexOf('firefox') > -1 &&
             attrGetter('ngfEnableFirefoxPaste', scope)) {
             elem.attr('contenteditable', true);
             elem.on('keypress', function(e) {
                 if (!e.metaKey && !e.ctrlKey) {
                     e.preventDefault();
                 }
             });
         }
 
+        function extractFilesAndUpdateModel(source, evt, updateOnType) {
+            if (!source) return;
+            // html needs to be calculated on the same process otherwise the data will be wiped
+            // after promise resolve or setTimeout.
+            var html;
+            try {
+                html = source && source.getData && source.getData('text/html');
+            } catch (e) {
+                /* Fix IE11 that throw error calling getData */ }
+            extractFiles(source.items, source.files, attrGetter('ngfAllowDir', scope) !== false,
+                attrGetter('multiple') || attrGetter('ngfMultiple', scope)).then(function(files) {
+                if (files.length) {
+                    updateModel(files, evt);
+                } else {
+                    extractFilesFromHtml(updateOnType, html).then(function(files) {
+                        updateModel(files, evt);
+                    });
+                }
+            });
+        }
+
         function updateModel(files, evt) {
             upload.updateModel(ngModel, attr, scope, attrGetter('ngfChange') || attrGetter('ngfDrop'), files, evt);
         }
 
         function extractFilesFromHtml(updateOn, html) {
-            if (!upload.shouldUpdateOn(updateOn, attr, scope) || !html) return upload.rejectPromise([]);
+            if (!upload.shouldUpdateOn(updateOn, attr, scope) || typeof html !== 'string') return upload.rejectPromise([]);
             var urls = [];
             html.replace(/<(img src|img [^>]* src) *=\"([^\"]*)\"/gi, function(m, n, src) {
                 urls.push(src);
             });
             var promises = [],
                 files = [];
             if (urls.length) {
@@ -2066,30 +2165,36 @@
                     }
                 }
             }
             callback(dClass);
         }
 
         function extractFiles(items, fileList, allowDir, multiple) {
-            var maxFiles = upload.getValidationAttr(attr, scope, 'maxFiles') || Number.MAX_VALUE;
-            var maxTotalSize = upload.getValidationAttr(attr, scope, 'maxTotalSize') || Number.MAX_VALUE;
+            var maxFiles = upload.getValidationAttr(attr, scope, 'maxFiles');
+            if (maxFiles == null) {
+                maxFiles = Number.MAX_VALUE;
+            }
+            var maxTotalSize = upload.getValidationAttr(attr, scope, 'maxTotalSize');
+            if (maxTotalSize == null) {
+                maxTotalSize = Number.MAX_VALUE;
+            }
             var includeDir = attrGetter('ngfIncludeDir', scope);
             var files = [],
                 totalSize = 0;
 
             function traverseFileTree(entry, path) {
                 var defer = $q.defer();
                 if (entry != null) {
                     if (entry.isDirectory) {
                         var promises = [upload.emptyPromise()];
                         if (includeDir) {
                             var file = {
                                 type: 'directory'
                             };
-                            file.name = file.path = (path || '') + entry.name + entry.name;
+                            file.name = file.path = (path || '') + entry.name;
                             files.push(file);
                         }
                         var dirReader = entry.createReader();
                         var entries = [];
                         var readEntries = function() {
                             dirReader.readEntries(function(results) {
                                 try {
@@ -2135,15 +2240,15 @@
                     }
                 }
                 return defer.promise;
             }
 
             var promises = [upload.emptyPromise()];
 
-            if (items && items.length > 0 && $location.protocol() !== 'file') {
+            if (items && items.length > 0 && $window.location.protocol !== 'file:') {
                 for (var i = 0; i < items.length; i++) {
                     if (items[i].webkitGetAsEntry && items[i].webkitGetAsEntry() && items[i].webkitGetAsEntry().isDirectory) {
                         var entry = items[i].webkitGetAsEntry();
                         if (entry.isDirectory && !allowDir) {
                             continue;
                         }
                         if (entry != null) {
```

### Comparing `XStatic-Angular-FileUpload-12.0.4.0/xstatic/pkg/angular_fileupload/data/ng-file-upload.min.js` & `XStatic-Angular-FileUpload-12.2.13.0/xstatic/pkg/angular_fileupload/data/ng-file-upload.min.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
-/*! 12.0.4 */ !window.XMLHttpRequest || window.FileAPI && FileAPI.shouldLoad || (window.XMLHttpRequest.prototype.setRequestHeader = function(a) {
+/*! 12.2.13 */ !window.XMLHttpRequest || window.FileAPI && FileAPI.shouldLoad || (window.XMLHttpRequest.prototype.setRequestHeader = function(a) {
     return function(b, c) {
         if ("__setXHR_" === b) {
             var d = c(this);
             d instanceof Function && d(this)
         } else a.apply(this, arguments)
     }
 }(window.XMLHttpRequest.prototype.setRequestHeader));
 var ngFileUpload = angular.module("ngFileUpload", []);
-ngFileUpload.version = "12.0.4", ngFileUpload.service("UploadBase", ["$http", "$q", "$timeout", function(a, b, c) {
+ngFileUpload.version = "12.2.13", ngFileUpload.service("UploadBase", ["$http", "$q", "$timeout", function(a, b, c) {
         function d(d) {
             function e(a) {
                 j.notify && j.notify(a), k.progressFunc && c(function() {
                     k.progressFunc(a)
                 })
             }
 
@@ -24,20 +24,23 @@
                     lengthComputable: !0,
                     target: a.target
                 } : a
             }
 
             function i() {
                 a(d).then(function(a) {
-                    g && d._chunkSize && !d._finished && d._file ? (e({
-                        loaded: d._end,
-                        total: d._file && d._file.size,
-                        config: d,
-                        type: "progress"
-                    }), f.upload(d, !0)) : (d._finished && delete d._finished, j.resolve(a))
+                    if (g && d._chunkSize && !d._finished && d._file) {
+                        var b = d._file && d._file.size || 0;
+                        e({
+                            loaded: Math.min(d._end, b),
+                            total: b,
+                            config: d,
+                            type: "progress"
+                        }), f.upload(d, !0)
+                    } else d._finished && delete d._finished, j.resolve(a)
                 }, function(a) {
                     j.reject(a)
                 }, function(a) {
                     j.notify(a)
                 })
             }
             d.method = d.method || "POST", d.headers = d.headers || {};
@@ -52,15 +55,15 @@
                     }, !1))
                 }
             }), g ? d._chunkSize && d._end && !d._finished ? (d._start = d._end, d._end += d._chunkSize, i()) : d.resumeSizeUrl ? a.get(d.resumeSizeUrl).then(function(a) {
                 d._start = d.resumeSizeResponseReader ? d.resumeSizeResponseReader(a.data) : parseInt((null == a.data.size ? a.data : a.data.size).toString()), d._chunkSize && (d._end = d._start + d._chunkSize), i()
             }, function(a) {
                 throw a
             }) : d.resumeSize ? d.resumeSize().then(function(a) {
-                d._start = a, i()
+                d._start = a, d._chunkSize && (d._end = d._start + d._chunkSize), i()
             }, function(a) {
                 throw a
             }) : (d._chunkSize && (d._start = 0, d._end = d._start + d._chunkSize), i()) : i(), k.success = function(a) {
                 return k.then(function(b) {
                     a(b.data, b.status, b.headers, d)
                 }), k
             }, k.error = function(a) {
@@ -77,15 +80,15 @@
                 }), k
             }, k.xhr = function(a) {
                 return d.xhrFn = function(b) {
                     return function() {
                         b && b.apply(k, arguments), a.apply(k, arguments)
                     }
                 }(d.xhrFn), k
-            }, f.promisesCount++, k["finally"](function() {
+            }, f.promisesCount++, k["finally"] && k["finally"] instanceof Function && k["finally"](function() {
                 f.promisesCount--
             }), k
         }
 
         function e(a) {
             var b = {};
             for (var c in a) a.hasOwnProperty(c) && (b[c] = a[c]);
@@ -174,19 +177,20 @@
             var d = b.defer();
             return a({
                 url: c,
                 method: "get",
                 responseType: "arraybuffer"
             }).then(function(a) {
                 var b = new Uint8Array(a.data),
-                    c = a.headers("content-type") || "image/WebP",
-                    e = new window.Blob([b], {
-                        type: c
-                    });
-                d.resolve(e)
+                    e = a.headers("content-type") || "image/WebP",
+                    f = new window.Blob([b], {
+                        type: e
+                    }),
+                    g = c.match(/.*\/(.+?)(\?.*)?$/);
+                g.length > 1 && (f.name = g[1]), d.resolve(f)
             }, function(a) {
                 d.reject(a)
             }), d.promise
         }, this.setDefaults = function(a) {
             this.defaults = a || {}
         }, this.defaults = {}, this.version = ngFileUpload.version
     }]), ngFileUpload.service("Upload", ["$parse", "$timeout", "$compile", "$q", "UploadExif", function(a, b, c, d, e) {
@@ -197,50 +201,56 @@
                     $file: d
                 }) && e.push(i.happyPromise(i.applyExifRotation(d), d).then(function(b) {
                     a.splice(f, 1, b)
                 }))
             }), d.all(e)
         }
 
-        function g(a, b, c) {
-            var e = i.attrGetter("ngfResize", b, c);
-            if (!e || !i.isResizeSupported() || !a.length) return i.emptyPromise();
-            if (!(e instanceof Function)) return h(e, a, b, c);
-            var f = d.defer();
-            e(a).then(function(d) {
-                h(d, a, b, c).then(function(a) {
-                    f.resolve(a)
+        function g(a, b, c, e) {
+            var f = i.attrGetter("ngfResize", b, c);
+            if (!f || !i.isResizeSupported() || !a.length) return i.emptyPromise();
+            if (f instanceof Function) {
+                var g = d.defer();
+                return f(a).then(function(d) {
+                    h(d, a, b, c, e).then(function(a) {
+                        g.resolve(a)
+                    }, function(a) {
+                        g.reject(a)
+                    })
                 }, function(a) {
-                    f.reject(a)
+                    g.reject(a)
                 })
-            }, function(a) {
-                f.reject(a)
-            })
+            }
+            return h(f, a, b, c, e)
         }
 
-        function h(a, b, c, e) {
-            function f(d, f) {
+        function h(a, b, c, e, f) {
+            function g(d, g) {
                 if (0 === d.type.indexOf("image")) {
                     if (a.pattern && !i.validatePattern(d, a.pattern)) return;
-                    var h = i.resize(d, a.width, a.height, a.quality, a.type, a.ratio, a.centerCrop, function(a, b) {
+                    a.resizeIf = function(a, b) {
                         return i.attrGetter("ngfResizeIf", c, e, {
                             $width: a,
                             $height: b,
                             $file: d
                         })
-                    }, a.restoreExif !== !1);
-                    g.push(h), h.then(function(a) {
-                        b.splice(f, 1, a)
+                    };
+                    var j = i.resize(d, a);
+                    h.push(j), j.then(function(a) {
+                        b.splice(g, 1, a)
                     }, function(a) {
-                        d.$error = "resize", d.$errorParam = (a ? (a.message ? a.message : a) + ": " : "") + (d && d.name)
+                        d.$error = "resize", (d.$errorMessages = d.$errorMessages || {}).resize = !0, d.$errorParam = (a ? (a.message ? a.message : a) + ": " : "") + (d && d.name), f.$ngfValidations.push({
+                            name: "resize",
+                            valid: !1
+                        }), i.applyModelValidation(f, b)
                     })
                 }
             }
-            for (var g = [i.emptyPromise()], h = 0; h < b.length; h++) f(b[h], h);
-            return d.all(g)
+            for (var h = [i.emptyPromise()], j = 0; j < b.length; j++) g(b[j], j);
+            return d.all(h)
         }
         var i = e;
         return i.getAttrWithDefaults = function(a, b) {
             if (null != a[b]) return a[b];
             var c = i.defaults[b];
             return null == c ? c : angular.isString(c) ? c : JSON.stringify(c)
         }, i.attrGetter = function(b, c, d, e) {
@@ -249,15 +259,15 @@
             try {
                 return e ? a(f)(d, e) : a(f)(d)
             } catch (g) {
                 if (b.search(/min|max|pattern/i)) return f;
                 throw g
             }
         }, i.shouldUpdateOn = function(a, b, c) {
-            var d = i.attrGetter("ngModelOptions", b, c);
+            var d = i.attrGetter("ngfModelOptions", b, c);
             return d && d.updateOn ? d.updateOn.split(" ").indexOf(a) > -1 : !0
         }, i.emptyPromise = function() {
             var a = d.defer(),
                 c = arguments;
             return b(function() {
                 a.resolve.apply(a, c)
             }), a.promise
@@ -299,71 +309,72 @@
             function n() {
                 function a(a, b) {
                     return a.name === b.name && (a.$ngfOrigSize || a.size) === (b.$ngfOrigSize || b.size) && a.type === b.type
                 }
 
                 function b(b) {
                     var c;
+                    for (c = 0; c < r.length; c++)
+                        if (a(b, r[c])) return !0;
                     for (c = 0; c < s.length; c++)
                         if (a(b, s[c])) return !0;
-                    for (c = 0; c < t.length; c++)
-                        if (a(b, t[c])) return !0;
                     return !1
                 }
                 if (j) {
-                    r = [], u = [];
-                    for (var c = 0; c < j.length; c++) b(j[c]) ? u.push(j[c]) : r.push(j[c])
+                    q = [], t = [];
+                    for (var c = 0; c < j.length; c++) b(j[c]) ? t.push(j[c]) : q.push(j[c])
                 }
             }
 
             function o(a) {
                 return angular.isArray(a) ? a : [a]
             }
 
             function p() {
-                w = [], v = [], angular.forEach(r, function(a) {
-                    a.$error ? v.push(a) : w.push(a)
-                })
-            }
-
-            function q() {
                 function a() {
                     b(function() {
-                        m(x ? s.concat(w) : w, x ? t.concat(v) : v, j, u, y)
-                    }, A && A.debounce ? A.debounce.change || A.debounce : 0)
+                        m(w ? r.concat(v) : v, w ? s.concat(u) : u, j, t, x)
+                    }, z && z.debounce ? z.debounce.change || z.debounce : 0)
                 }
-                g(z ? r : w, d, e).then(function() {
-                    z ? i.validate(r, s.length, c, d, e).then(function() {
-                        p(), a()
+                var f = y ? q : v;
+                g(f, d, e, c).then(function() {
+                    y ? i.validate(q, w ? r.length : 0, c, d, e).then(function(b) {
+                        v = b.validsFiles, u = b.invalidsFiles, a()
                     }) : a()
-                }, function(a) {
-                    throw "Could not resize files " + a
+                }, function() {
+                    for (var b = 0; b < f.length; b++) {
+                        var c = f[b];
+                        if ("resize" === c.$error) {
+                            var d = v.indexOf(c);
+                            d > -1 && (v.splice(d, 1), u.push(c)), a()
+                        }
+                    }
                 })
             }
-            var r, s, t, u = [],
-                v = [],
-                w = [];
-            s = d.$$ngfPrevValidFiles || [], t = d.$$ngfPrevInvalidFiles || [], c && c.$modelValue && (s = o(c.$modelValue));
-            var x = i.attrGetter("ngfKeep", d, e);
-            r = (j || []).slice(0), ("distinct" === x || i.attrGetter("ngfKeepDistinct", d, e) === !0) && n(d, e);
-            var y = !x && !i.attrGetter("ngfMultiple", d, e) && !i.attrGetter("multiple", d);
-            if (!x || r.length) {
+            var q, r, s, t = [],
+                u = [],
+                v = [];
+            r = d.$$ngfPrevValidFiles || [], s = d.$$ngfPrevInvalidFiles || [], c && c.$modelValue && (r = o(c.$modelValue));
+            var w = i.attrGetter("ngfKeep", d, e);
+            q = (j || []).slice(0), ("distinct" === w || i.attrGetter("ngfKeepDistinct", d, e) === !0) && n(d, e);
+            var x = !w && !i.attrGetter("ngfMultiple", d, e) && !i.attrGetter("multiple", d);
+            if (!w || q.length) {
                 i.attrGetter("ngfBeforeModelChange", d, e, {
                     $files: j,
                     $file: j && j.length ? j[0] : null,
-                    $newFiles: r,
-                    $duplicateFiles: u,
+                    $newFiles: q,
+                    $duplicateFiles: t,
                     $event: k
                 });
-                var z = i.attrGetter("ngfValidateAfterResize", d, e),
-                    A = i.attrGetter("ngModelOptions", d, e);
-                i.validate(r, s.length, c, d, e).then(function() {
-                    l ? m(r, [], j, u, y) : (A && A.allowInvalid || z ? w = r : p(), i.attrGetter("ngfFixOrientation", d, e) && i.isExifSupported() ? f(w, d, e).then(function() {
-                        q()
-                    }) : q())
+                var y = i.attrGetter("ngfValidateAfterResize", d, e),
+                    z = i.attrGetter("ngfModelOptions", d, e);
+                i.validate(q, w ? r.length : 0, c, d, e).then(function(a) {
+                    l ? m(q, [], j, t, x) : (z && z.allowInvalid || y ? v = q : (v = a.validFiles, u = a.invalidFiles), i.attrGetter("ngfFixOrientation", d, e) && i.isExifSupported() ? f(v, d, e).then(function() {
+                        p()
+                    }) : p())
                 })
             }
         }, i
     }]), ngFileUpload.directive("ngfSelect", ["$parse", "$timeout", "$compile", "Upload", function(a, b, c, d) {
         function e(a) {
             var b = a.match(/Android[^\d]*(\d+)\.(\d+)/);
             if (b && b.length > 2) {
@@ -380,108 +391,115 @@
 
             function l() {
                 return t("ngfChange") || t("ngfSelect")
             }
 
             function m(b) {
                 if (j.shouldUpdateOn("change", c, a)) {
-                    for (var e = b.__files_ || b.target && b.target.files, f = [], g = 0; g < e.length; g++) f.push(e[g]);
+                    var e = b.__files_ || b.target && b.target.files,
+                        f = [];
+                    if (!e) return;
+                    for (var g = 0; g < e.length; g++) f.push(e[g]);
                     j.updateModel(d, c, a, l(), f.length ? f : null, b)
                 }
             }
 
-            function n(a) {
-                if (b !== a)
-                    for (var c = 0; c < b[0].attributes.length; c++) {
-                        var d = b[0].attributes[c];
-                        "type" !== d.name && "class" !== d.name && "style" !== d.name && ((null == d.value || "" === d.value) && ("required" === d.name && (d.value = "required"), "multiple" === d.name && (d.value = "multiple")), a.attr(d.name, "id" === d.name ? "ngf-" + d.value : d.value))
-                    }
+            function n(a, d) {
+                function e(b) {
+                    a.attr("id", "ngf-" + b), d.attr("id", "ngf-label-" + b)
+                }
+                for (var f = 0; f < b[0].attributes.length; f++) {
+                    var g = b[0].attributes[f];
+                    "type" !== g.name && "class" !== g.name && "style" !== g.name && ("id" === g.name ? (e(g.value), u.push(c.$observe("id", e))) : a.attr(g.name, g.value || "required" !== g.name && "multiple" !== g.name ? g.value : g.name))
+                }
             }
 
             function o() {
                 if (k()) return b;
-                var a = angular.element('<input type="file">');
-                n(a);
-                var c = angular.element("<label>upload</label>");
-                return c.css("visibility", "hidden").css("position", "absolute").css("overflow", "hidden").css("width", "0px").css("height", "0px").css("border", "none").css("margin", "0px").css("padding", "0px").attr("tabindex", "-1"), g.push({
+                var a = angular.element('<input type="file">'),
+                    c = angular.element("<label>upload</label>");
+                return c.css("visibility", "hidden").css("position", "absolute").css("overflow", "hidden").css("width", "0px").css("height", "0px").css("border", "none").css("margin", "0px").css("padding", "0px").attr("tabindex", "-1"), n(a, c), g.push({
                     el: b,
                     ref: c
                 }), document.body.appendChild(c.append(a)[0]), a
             }
 
             function p(c) {
                 if (b.attr("disabled")) return !1;
                 if (!t("ngfSelectDisabled", a)) {
                     var d = q(c);
                     if (null != d) return d;
                     r(c);
                     try {
-                        k() || document.body.contains(w[0]) || (g.push({
+                        k() || document.body.contains(x[0]) || (g.push({
                             el: b,
-                            ref: w.parent()
-                        }), document.body.appendChild(w.parent()[0]), w.bind("change", m))
+                            ref: x.parent()
+                        }), document.body.appendChild(x.parent()[0]), x.bind("change", m))
                     } catch (f) {}
                     return e(navigator.userAgent) ? setTimeout(function() {
-                        w[0].click()
-                    }, 0) : w[0].click(), !1
+                        x[0].click()
+                    }, 0) : x[0].click(), !1
                 }
             }
 
             function q(a) {
                 var b = a.changedTouches || a.originalEvent && a.originalEvent.changedTouches;
-                if ("touchstart" === a.type) return v = b ? b[0].clientY : 0, !0;
-                if (a.stopPropagation(), a.preventDefault(), "touchend" === a.type) {
-                    var c = b ? b[0].clientY : 0;
-                    if (Math.abs(c - v) > 20) return !1
+                if (b) {
+                    if ("touchstart" === a.type) return w = b[0].clientX, v = b[0].clientY, !0;
+                    if ("touchend" === a.type) {
+                        var c = b[0].clientX,
+                            d = b[0].clientY;
+                        if (Math.abs(c - w) > 20 || Math.abs(d - v) > 20) return a.stopPropagation(), a.preventDefault(), !1
+                    }
+                    return !0
                 }
             }
 
             function r(b) {
-                j.shouldUpdateOn("click", c, a) && w.val() && (w.val(null), j.updateModel(d, c, a, l(), null, b, !0))
+                j.shouldUpdateOn("click", c, a) && x.val() && (x.val(null), j.updateModel(d, c, a, l(), null, b, !0))
             }
 
             function s(a) {
-                if (w && !w.attr("__ngf_ie10_Fix_")) {
-                    if (!w[0].parentNode) return void(w = null);
-                    a.preventDefault(), a.stopPropagation(), w.unbind("click");
-                    var b = w.clone();
-                    return w.replaceWith(b), w = b, w.attr("__ngf_ie10_Fix_", "true"), w.bind("change", m), w.bind("click", s), w[0].click(), !1
+                if (x && !x.attr("__ngf_ie10_Fix_")) {
+                    if (!x[0].parentNode) return void(x = null);
+                    a.preventDefault(), a.stopPropagation(), x.unbind("click");
+                    var b = x.clone();
+                    return x.replaceWith(b), x = b, x.attr("__ngf_ie10_Fix_", "true"), x.bind("change", m), x.bind("click", s), x[0].click(), !1
                 }
-                w.removeAttr("__ngf_ie10_Fix_")
+                x.removeAttr("__ngf_ie10_Fix_")
             }
             var t = function(a, b) {
                 return j.attrGetter(a, c, b)
             };
             j.registerModelChangeValidator(d, c, a);
             var u = [];
-            u.push(a.$watch(t("ngfMultiple"), function() {
-                w.attr("multiple", t("ngfMultiple", a))
-            })), u.push(a.$watch(t("ngfCapture"), function() {
-                w.attr("capture", t("ngfCapture", a))
-            })), u.push(a.$watch(t("ngfAccept"), function() {
-                w.attr("accept", t("ngfAccept", a))
-            })), c.$observe("accept", function() {
-                w.attr("accept", t("accept"))
-            }), u.push(function() {
-                c.$$observers && delete c.$$observers.accept
-            });
+            t("ngfMultiple") && u.push(a.$watch(t("ngfMultiple"), function() {
+                x.attr("multiple", t("ngfMultiple", a))
+            })), t("ngfCapture") && u.push(a.$watch(t("ngfCapture"), function() {
+                x.attr("capture", t("ngfCapture", a))
+            })), t("ngfAccept") && u.push(a.$watch(t("ngfAccept"), function() {
+                x.attr("accept", t("ngfAccept", a))
+            })), u.push(c.$observe("accept", function() {
+                x.attr("accept", t("accept"))
+            }));
             var v = 0,
-                w = b;
-            k() || (w = o()), w.bind("change", m), k() ? b.bind("click", r) : b.bind("click touchstart touchend", p), -1 !== navigator.appVersion.indexOf("MSIE 10") && w.bind("click", s), d && d.$formatters.push(function(a) {
-                return (null == a || 0 === a.length) && w.val() && w.val(null), a
+                w = 0,
+                x = b;
+            k() || (x = o()), x.bind("change", m), k() ? b.bind("click", r) : b.bind("click touchstart touchend", p), -1 !== navigator.appVersion.indexOf("MSIE 10") && x.bind("click", s), d && d.$formatters.push(function(a) {
+                return (null == a || 0 === a.length) && x.val() && x.val(null), a
             }), a.$on("$destroy", function() {
-                k() || w.parent().remove(), angular.forEach(u, function(a) {
+                k() || x.parent().remove(), angular.forEach(u, function(a) {
                     a()
                 })
             }), h(function() {
                 for (var a = 0; a < g.length; a++) {
                     var b = g[a];
                     document.body.contains(b.el[0]) || (g.splice(a, 1), b.ref.remove())
                 }
-            }), window.FileAPI && window.FileAPI.ngfFixIE && window.FileAPI.ngfFixIE(b, w, m)
+            }), window.FileAPI && window.FileAPI.ngfFixIE && window.FileAPI.ngfFixIE(b, x, m)
         }
         var g = [];
         return {
             restrict: "AEC",
             require: "?ngModel",
             link: function(e, g, h, i) {
                 f(e, g, h, i, a, b, c, d)
@@ -501,30 +519,36 @@
                         var b = (g ? a.$ngfDataUrl : a.$ngfBlobUrl) || a.$ngfDataUrl;
                         i ? e.css("background-image", "url('" + (b || "") + "')") : e.attr("src", b), b ? e.removeClass("ng-hide") : e.addClass("ng-hide")
                     })
                 })
             }
             c(function() {
                 var c = d.$watch(f[g], function(c) {
-                    var d = h;
-                    if ("ngfThumbnail" === g && (d || (d = {
-                            width: e[0].clientWidth,
-                            height: e[0].clientHeight
-                        }), 0 === d.width && window.getComputedStyle)) {
-                        var f = getComputedStyle(e[0]);
-                        d = {
-                            width: parseInt(f.width.slice(0, -2)),
-                            height: parseInt(f.height.slice(0, -2))
-                        }
+                    var k = h;
+                    if ("ngfThumbnail" === g && (k || (k = {
+                            width: e[0].naturalWidth || e[0].clientWidth,
+                            height: e[0].naturalHeight || e[0].clientHeight
+                        }), 0 === k.width && window.getComputedStyle)) {
+                        var l = getComputedStyle(e[0]);
+                        l.width && l.width.indexOf("px") > -1 && l.height && l.height.indexOf("px") > -1 && (k = {
+                            width: parseInt(l.width.slice(0, -2)),
+                            height: parseInt(l.height.slice(0, -2))
+                        })
                     }
-                    return angular.isString(c) ? (e.removeClass("ng-hide"), i ? e.css("background-image", "url('" + c + "')") : e.attr("src", c)) : void(!c || !c.type || 0 !== c.type.search(a(e[0])) || i && 0 !== c.type.indexOf("image") ? e.addClass("ng-hide") : d && b.isResizeSupported() ? b.resize(c, d.width, d.height, d.quality).then(function(a) {
+                    return angular.isString(c) ? (e.removeClass("ng-hide"), i ? e.css("background-image", "url('" + c + "')") : e.attr("src", c)) : void(!c || !c.type || 0 !== c.type.search(a(e[0])) || i && 0 !== c.type.indexOf("image") ? e.addClass("ng-hide") : k && b.isResizeSupported() ? (k.resizeIf = function(a, e) {
+                        return b.attrGetter("ngfResizeIf", f, d, {
+                            $width: a,
+                            $height: e,
+                            $file: c
+                        })
+                    }, b.resize(c, k).then(function(a) {
                         j(a)
                     }, function(a) {
                         throw a
-                    }) : j(c))
+                    })) : j(c))
                 });
                 d.$on("$destroy", function() {
                     c()
                 })
             })
         }
         ngFileUpload.service("UploadDataUrl", ["UploadBase", "$timeout", "$q", function(a, b, c) {
@@ -616,15 +640,15 @@
                 restrict: "AE",
                 link: function(d, e, f) {
                     var g = a.attrGetter("ngfSize", f, d);
                     b(a, c, d, e, f, "ngfThumbnail", g, a.attrGetter("ngfAsBackground", f, d))
                 }
             }
         }]), ngFileUpload.config(["$compileProvider", function(a) {
-            a.imgSrcSanitizationWhitelist && a.imgSrcSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|local|file|data|blob):/), a.aHrefSanitizationWhitelist && a.aHrefSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|local|file|data|blob):/)
+            a.imgSrcSanitizationWhitelist && a.imgSrcSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|webcal|local|file|data|blob):/), a.aHrefSanitizationWhitelist && a.aHrefSanitizationWhitelist(/^\s*(https?|ftp|mailto|tel|webcal|local|file|data|blob):/)
         }]), ngFileUpload.filter("ngfDataUrl", ["UploadDataUrl", "$sce", function(a, b) {
             return function(c, d, e) {
                 if (angular.isString(c)) return b.trustAsResourceUrl(c);
                 var f = c && ((d ? c.$ngfDataUrl : c.$ngfBlobUrl) || c.$ngfDataUrl);
                 return c && !f ? (!c.$ngfDataUrlFilterInProgress && angular.isObject(c) && (c.$ngfDataUrlFilterInProgress = !0, a.dataUrl(c, d)), "") : (c && delete c.$ngfDataUrlFilterInProgress, (c && f ? e ? b.trustAsResourceUrl(f) : f : c) || "")
             }
         }])
@@ -666,17 +690,21 @@
             return e
         }, f.ratioToFloat = function(a) {
             var b = a.toString(),
                 c = b.search(/[x:]/i);
             return b = c > -1 ? parseFloat(b.substring(0, c)) / parseFloat(b.substring(c + 1)) : parseFloat(b)
         }, f.registerModelChangeValidator = function(a, b, c) {
             a && a.$formatters.push(function(d) {
-                a.$dirty && (d && !angular.isArray(d) && (d = [d]), f.validate(d, 0, a, b, c).then(function() {
-                    f.applyModelValidation(a, d)
-                }))
+                if (a.$dirty) {
+                    var e = d;
+                    d && !angular.isArray(d) && (e = [d]), f.validate(e, 0, a, b, c).then(function() {
+                        f.applyModelValidation(a, e)
+                    })
+                }
+                return d
             })
         }, f.applyModelValidation = function(a, b) {
             e(a, b), angular.forEach(a.$ngfValidations, function(b) {
                 a.$setValidity(b.name, b.valid)
             })
         }, f.getValidationAttr = function(a, b, c, d, e) {
             var g = "ngf" + c[0].toUpperCase() + c.substr(1),
@@ -690,124 +718,161 @@
                 h = h[i[0]], i.length > 1 && (h = h && h[i[1]])
             }
             return h
         }, f.validate = function(a, c, d, e, g) {
             function h(b, c, h) {
                 if (a) {
                     for (var i = a.length, j = null; i--;) {
-                        var k = a[i];
-                        if (k) {
-                            var l = f.getValidationAttr(e, g, b, c, k);
-                            null != l && (h(k, l, i) || (k.$error = b, (k.$errorMessages = k.$errorMessages || {})[b] = !0, k.$errorParam = l, a.splice(i, 1), j = !1))
+                        var n = a[i];
+                        if (n) {
+                            var o = f.getValidationAttr(e, g, b, c, n);
+                            null != o && (h(n, o, i) || (-1 === k.indexOf(b) ? (n.$error = b, (n.$errorMessages = n.$errorMessages || {})[b] = !0, n.$errorParam = o, -1 === m.indexOf(n) && m.push(n), l || a.splice(i, 1), j = !1) : a.splice(i, 1)))
                         }
                     }
                     null !== j && d.$ngfValidations.push({
                         name: b,
                         valid: j
                     })
                 }
             }
 
-            function i(c, h, i, k, l) {
-                function m(a, b, d) {
-                    null != d ? k(b, d).then(function(e) {
-                        l(e, d) ? a.resolve() : (b.$error = c, (b.$errorMessages = b.$errorMessages || {})[c] = !0, b.$errorParam = d, a.reject())
+            function i(c, h, i, n, o) {
+                function p(b, d, e) {
+                    function f(f) {
+                        if (f())
+                            if (-1 === k.indexOf(c)) {
+                                if (d.$error = c, (d.$errorMessages = d.$errorMessages || {})[c] = !0, d.$errorParam = e, -1 === m.indexOf(d) && m.push(d), !l) {
+                                    var g = a.indexOf(d);
+                                    g > -1 && a.splice(g, 1)
+                                }
+                                b.resolve(!1)
+                            } else {
+                                var h = a.indexOf(d);
+                                h > -1 && a.splice(h, 1), b.resolve(!0)
+                            }
+                        else b.resolve(!0)
+                    }
+                    null != e ? n(d, e).then(function(a) {
+                        f(function() {
+                            return !o(a, e)
+                        })
                     }, function() {
-                        j("ngfValidateForce", {
-                            $file: b
-                        }) ? (b.$error = c, (b.$errorMessages = b.$errorMessages || {})[c] = !0, b.$errorParam = d, a.reject()) : a.resolve()
-                    }) : a.resolve()
+                        f(function() {
+                            return j("ngfValidateForce", {
+                                $file: d
+                            })
+                        })
+                    }) : b.resolve(!0)
                 }
-                var n = [f.emptyPromise()];
-                return a ? (a = void 0 === a.length ? [a] : a, angular.forEach(a, function(a) {
+                var q = [f.emptyPromise(!0)];
+                a && (a = void 0 === a.length ? [a] : a, angular.forEach(a, function(a) {
                     var d = b.defer();
-                    return n.push(d.promise), !i || null != a.type && 0 === a.type.search(i) ? void("dimensions" === c && null != f.attrGetter("ngfDimensions", e) ? f.imageDimensions(a).then(function(b) {
-                        m(d, a, j("ngfDimensions", {
+                    return q.push(d.promise), !i || null != a.type && 0 === a.type.search(i) ? void("dimensions" === c && null != f.attrGetter("ngfDimensions", e) ? f.imageDimensions(a).then(function(b) {
+                        p(d, a, j("ngfDimensions", {
                             $file: a,
                             $width: b.width,
                             $height: b.height
                         }))
                     }, function() {
-                        d.reject()
+                        d.resolve(!1)
                     }) : "duration" === c && null != f.attrGetter("ngfDuration", e) ? f.mediaDuration(a).then(function(b) {
-                        m(d, a, j("ngfDuration", {
+                        p(d, a, j("ngfDuration", {
                             $file: a,
                             $duration: b
                         }))
                     }, function() {
-                        d.reject()
-                    }) : m(d, a, f.getValidationAttr(e, g, c, h, a))) : void d.resolve()
-                }), b.all(n).then(function() {
-                    d.$ngfValidations.push({
-                        name: c,
-                        valid: !0
-                    })
-                }, function() {
-                    d.$ngfValidations.push({
+                        d.resolve(!1)
+                    }) : p(d, a, f.getValidationAttr(e, g, c, h, a))) : void d.resolve(!0)
+                }));
+                var r = b.defer();
+                return b.all(q).then(function(a) {
+                    for (var b = !0, e = 0; e < a.length; e++)
+                        if (!a[e]) {
+                            b = !1;
+                            break
+                        } d.$ngfValidations.push({
                         name: c,
-                        valid: !1
-                    })
-                })) : void 0
+                        valid: b
+                    }), r.resolve(b)
+                }), r.promise
             }
             d = d || {}, d.$ngfValidations = d.$ngfValidations || [], angular.forEach(d.$ngfValidations, function(a) {
                 a.valid = !0
             });
             var j = function(a, b) {
-                return f.attrGetter(a, e, g, b)
-            };
-            if (null == a || 0 === a.length) return f.emptyPromise(d);
-            a = void 0 === a.length ? [a] : a.slice(0), h("maxFiles", null, function(a, b, d) {
-                return b > c + d
-            }), h("pattern", null, f.validatePattern), h("minSize", "size.min", function(a, b) {
+                    return f.attrGetter(a, e, g, b)
+                },
+                k = (f.attrGetter("ngfIgnoreInvalid", e, g) || "").split(" "),
+                l = f.attrGetter("ngfRunAllValidations", e, g);
+            if (null == a || 0 === a.length) return f.emptyPromise({
+                validFiles: a,
+                invalidFiles: []
+            });
+            a = void 0 === a.length ? [a] : a.slice(0);
+            var m = [];
+            h("pattern", null, f.validatePattern), h("minSize", "size.min", function(a, b) {
                 return a.size + .1 >= f.translateScalars(b)
             }), h("maxSize", "size.max", function(a, b) {
                 return a.size - .1 <= f.translateScalars(b)
             });
-            var k = 0;
+            var n = 0;
             if (h("maxTotalSize", null, function(b, c) {
-                    return k += b.size, k > f.translateScalars(c) ? (a.splice(0, a.length), !1) : !0
+                    return n += b.size, n > f.translateScalars(c) ? (a.splice(0, a.length), !1) : !0
                 }), h("validateFn", null, function(a, b) {
                     return b === !0 || null === b || "" === b
-                }), !a.length) return f.emptyPromise(d, d.$ngfValidations);
-            var l = b.defer(),
-                m = [];
-            return m.push(f.happyPromise(i("maxHeight", "height.max", /image/, this.imageDimensions, function(a, b) {
+                }), !a.length) return f.emptyPromise({
+                validFiles: [],
+                invalidFiles: m
+            });
+            var o = b.defer(),
+                p = [];
+            return p.push(i("maxHeight", "height.max", /image/, this.imageDimensions, function(a, b) {
                 return a.height <= b
-            }))), m.push(f.happyPromise(i("minHeight", "height.min", /image/, this.imageDimensions, function(a, b) {
+            })), p.push(i("minHeight", "height.min", /image/, this.imageDimensions, function(a, b) {
                 return a.height >= b
-            }))), m.push(f.happyPromise(i("maxWidth", "width.max", /image/, this.imageDimensions, function(a, b) {
+            })), p.push(i("maxWidth", "width.max", /image/, this.imageDimensions, function(a, b) {
                 return a.width <= b
-            }))), m.push(f.happyPromise(i("minWidth", "width.min", /image/, this.imageDimensions, function(a, b) {
+            })), p.push(i("minWidth", "width.min", /image/, this.imageDimensions, function(a, b) {
                 return a.width >= b
-            }))), m.push(f.happyPromise(i("dimensions", null, /image/, function(a, b) {
+            })), p.push(i("dimensions", null, /image/, function(a, b) {
                 return f.emptyPromise(b)
             }, function(a) {
                 return a
-            }))), m.push(f.happyPromise(i("ratio", null, /image/, this.imageDimensions, function(a, b) {
-                for (var c = b.toString().split(","), d = !1, e = 0; e < c.length; e++) Math.abs(a.width / a.height - f.ratioToFloat(c[e])) < 1e-4 && (d = !0);
+            })), p.push(i("ratio", null, /image/, this.imageDimensions, function(a, b) {
+                for (var c = b.toString().split(","), d = !1, e = 0; e < c.length; e++) Math.abs(a.width / a.height - f.ratioToFloat(c[e])) < .01 && (d = !0);
                 return d
-            }))), m.push(f.happyPromise(i("maxRatio", "ratio.max", /image/, this.imageDimensions, function(a, b) {
+            })), p.push(i("maxRatio", "ratio.max", /image/, this.imageDimensions, function(a, b) {
                 return a.width / a.height - f.ratioToFloat(b) < 1e-4
-            }))), m.push(f.happyPromise(i("minRatio", "ratio.min", /image/, this.imageDimensions, function(a, b) {
+            })), p.push(i("minRatio", "ratio.min", /image/, this.imageDimensions, function(a, b) {
                 return a.width / a.height - f.ratioToFloat(b) > -1e-4
-            }))), m.push(f.happyPromise(i("maxDuration", "duration.max", /audio|video/, this.mediaDuration, function(a, b) {
+            })), p.push(i("maxDuration", "duration.max", /audio|video/, this.mediaDuration, function(a, b) {
                 return a <= f.translateScalars(b)
-            }))), m.push(f.happyPromise(i("minDuration", "duration.min", /audio|video/, this.mediaDuration, function(a, b) {
+            })), p.push(i("minDuration", "duration.min", /audio|video/, this.mediaDuration, function(a, b) {
                 return a >= f.translateScalars(b)
-            }))), m.push(f.happyPromise(i("duration", null, /audio|video/, function(a, b) {
+            })), p.push(i("duration", null, /audio|video/, function(a, b) {
                 return f.emptyPromise(b)
             }, function(a) {
                 return a
-            }))), m.push(f.happyPromise(i("validateAsyncFn", null, null, function(a, b) {
+            })), p.push(i("validateAsyncFn", null, null, function(a, b) {
                 return b
             }, function(a) {
                 return a === !0 || null === a || "" === a
-            }))), b.all(m).then(function() {
-                l.resolve(d, d.$ngfValidations)
-            })
+            })), b.all(p).then(function() {
+                if (l)
+                    for (var b = 0; b < a.length; b++) {
+                        var d = a[b];
+                        d.$error && a.splice(b--, 1)
+                    }
+                l = !1, h("maxFiles", null, function(a, b, d) {
+                    return b > c + d
+                }), o.resolve({
+                    validFiles: a,
+                    invalidFiles: m
+                })
+            }), o.promise
         }, f.imageDimensions = function(a) {
             if (a.$ngfWidth && a.$ngfHeight) {
                 var d = b.defer();
                 return c(function() {
                     d.resolve({
                         width: a.$ngfWidth,
                         height: a.$ngfHeight
@@ -815,29 +880,29 @@
                 }), d.promise
             }
             if (a.$ngfDimensionPromise) return a.$ngfDimensionPromise;
             var e = b.defer();
             return c(function() {
                 return 0 !== a.type.indexOf("image") ? void e.reject("not image") : void f.dataUrl(a).then(function(b) {
                     function d() {
-                        var b = h[0].clientWidth,
-                            c = h[0].clientHeight;
+                        var b = h[0].naturalWidth || h[0].clientWidth,
+                            c = h[0].naturalHeight || h[0].clientHeight;
                         h.remove(), a.$ngfWidth = b, a.$ngfHeight = c, e.resolve({
                             width: b,
                             height: c
                         })
                     }
 
                     function f() {
                         h.remove(), e.reject("load error")
                     }
 
                     function g() {
                         c(function() {
-                            h[0].parentNode && (h[0].clientWidth ? d() : i > 10 ? f() : g())
+                            h[0].parentNode && (h[0].clientWidth ? d() : i++ > 10 ? f() : g())
                         }, 1e3)
                     }
                     var h = angular.element("<img>").attr("src", b).css("visibility", "hidden").css("position", "fixed").css("max-width", "none !important").css("max-height", "none !important");
                     h.on("load", d), h.on("error", f);
                     var i = 0;
                     g(), angular.element(document.getElementsByTagName("body")[0]).append(h)
                 }, function() {
@@ -893,32 +958,34 @@
                     marginY: b * f - d
                 }
             },
             e = function(a, e, f, g, h, i, j, k) {
                 var l = b.defer(),
                     m = document.createElement("canvas"),
                     n = document.createElement("img");
-                return n.onload = function() {
-                    if (null != k && k(n.width, n.height) === !1) return void l.reject("resizeIf");
+                return n.setAttribute("style", "visibility:hidden;position:fixed;z-index:-100000"), document.body.appendChild(n), n.onload = function() {
+                    var a = n.width,
+                        b = n.height;
+                    if (n.parentNode.removeChild(n), null != k && k(a, b) === !1) return void l.reject("resizeIf");
                     try {
                         if (i) {
-                            var a = c.ratioToFloat(i),
-                                b = n.width / n.height;
-                            a > b ? (e = n.width, f = e / a) : (f = n.height, e = f * a)
+                            var o = c.ratioToFloat(i),
+                                p = a / b;
+                            o > p ? (e = a, f = e / o) : (f = b, e = f * o)
                         }
-                        e || (e = n.width), f || (f = n.height);
-                        var o = d(n.width, n.height, e, f, j);
-                        m.width = Math.min(o.width, e), m.height = Math.min(o.height, f);
-                        var p = m.getContext("2d");
-                        p.drawImage(n, Math.min(0, -o.marginX / 2), Math.min(0, -o.marginY / 2), o.width, o.height), l.resolve(m.toDataURL(h || "image/WebP", g || .934))
-                    } catch (q) {
-                        l.reject(q)
+                        e || (e = a), f || (f = b);
+                        var q = d(a, b, e, f, j);
+                        m.width = Math.min(q.width, e), m.height = Math.min(q.height, f);
+                        var r = m.getContext("2d");
+                        r.drawImage(n, Math.min(0, -q.marginX / 2), Math.min(0, -q.marginY / 2), q.width, q.height), l.resolve(m.toDataURL(h || "image/WebP", g || .934))
+                    } catch (s) {
+                        l.reject(s)
                     }
                 }, n.onerror = function() {
-                    l.reject()
+                    n.parentNode.removeChild(n), l.reject()
                 }, n.src = a, l.promise
             };
         return c.dataUrltoBlob = function(a, b, c) {
             for (var d = a.split(","), e = d[0].match(/:(.*?);/)[1], f = atob(d[1]), g = f.length, h = new Uint8Array(g); g--;) h[g] = f.charCodeAt(g);
             var i = new window.Blob([h], {
                 type: e
             });
@@ -930,52 +997,66 @@
             get: function() {
                 return this.$ngfName
             },
             set: function(a) {
                 this.$ngfName = a
             },
             configurable: !0
-        }), c.resize = function(a, d, f, g, h, i, j, k, l) {
+        }), c.resize = function(a, d) {
             if (0 !== a.type.indexOf("image")) return c.emptyPromise(a);
-            var m = b.defer();
+            var f = b.defer();
             return c.dataUrl(a, !0).then(function(b) {
-                e(b, d, f, g, h || a.type, i, j, k).then(function(d) {
-                    if ("image/jpeg" === a.type && l) try {
-                        d = c.restoreExif(b, d)
-                    } catch (e) {
+                e(b, d.width, d.height, d.quality, d.type || a.type, d.ratio, d.centerCrop, d.resizeIf).then(function(e) {
+                    if ("image/jpeg" === a.type && d.restoreExif !== !1) try {
+                        e = c.restoreExif(b, e)
+                    } catch (g) {
                         setTimeout(function() {
-                            throw e
+                            throw g
                         }, 1)
                     }
                     try {
-                        var f = c.dataUrltoBlob(d, a.name, a.size);
-                        m.resolve(f)
-                    } catch (e) {
-                        m.reject(e)
+                        var h = c.dataUrltoBlob(e, a.name, a.size);
+                        f.resolve(h)
+                    } catch (g) {
+                        f.reject(g)
                     }
                 }, function(b) {
-                    "resizeIf" === b && m.resolve(a), m.reject(b)
+                    "resizeIf" === b && f.resolve(a), f.reject(b)
                 })
             }, function(a) {
-                m.reject(a)
-            }), m.promise
+                f.reject(a)
+            }), f.promise
         }, c
     }]),
     function() {
         function a(a, c, d, e, f, g, h, i, j, k) {
             function l() {
-                return c.attr("disabled") || r("ngfDropDisabled", a)
+                return c.attr("disabled") || s("ngfDropDisabled", a)
             }
 
-            function m(b, c) {
-                i.updateModel(e, d, a, r("ngfChange") || r("ngfDrop"), b, c)
+            function m(b, c, d) {
+                if (b) {
+                    var e;
+                    try {
+                        e = b && b.getData && b.getData("text/html")
+                    } catch (f) {}
+                    q(b.items, b.files, s("ngfAllowDir", a) !== !1, s("multiple") || s("ngfMultiple", a)).then(function(a) {
+                        a.length ? n(a, c) : o(d, e).then(function(a) {
+                            n(a, c)
+                        })
+                    })
+                }
             }
 
             function n(b, c) {
-                if (!i.shouldUpdateOn(b, d, a) || !c) return i.rejectPromise([]);
+                i.updateModel(e, d, a, s("ngfChange") || s("ngfDrop"), b, c)
+            }
+
+            function o(b, c) {
+                if (!i.shouldUpdateOn(b, d, a) || "string" != typeof c) return i.rejectPromise([]);
                 var e = [];
                 c.replace(/<(img src|img [^>]* src) *=\"([^\"]*)\"/gi, function(a, b, c) {
                     e.push(c)
                 });
                 var f = [],
                     g = [];
                 if (e.length) {
@@ -990,47 +1071,47 @@
                     }, function(a) {
                         h.reject(a)
                     }), h.promise
                 }
                 return i.emptyPromise()
             }
 
-            function o(a, b, c, d) {
-                var e = r("ngfDragOverClass", a, {
+            function p(a, b, c, d) {
+                var e = s("ngfDragOverClass", a, {
                         $event: c
                     }),
                     f = "dragover";
                 if (angular.isString(e)) f = e;
-                else if (e && (e.delay && (v = e.delay), e.accept || e.reject)) {
+                else if (e && (e.delay && (w = e.delay), e.accept || e.reject)) {
                     var g = c.dataTransfer.items;
                     if (null != g && g.length)
-                        for (var h = e.pattern || r("ngfPattern", a, {
+                        for (var h = e.pattern || s("ngfPattern", a, {
                                 $event: c
                             }), j = g.length; j--;) {
                             if (!i.validatePattern(g[j], h)) {
                                 f = e.reject;
                                 break
                             }
                             f = e.accept
                         } else f = e.accept
                 }
                 d(f)
             }
 
-            function p(b, c, e, f) {
+            function q(b, c, e, f) {
                 function g(a, b) {
                     var c = k.defer();
                     if (null != a)
                         if (a.isDirectory) {
                             var d = [i.emptyPromise()];
                             if (m) {
                                 var e = {
                                     type: "directory"
                                 };
-                                e.name = e.path = (b || "") + a.name + a.name, n.push(e)
+                                e.name = e.path = (b || "") + a.name, n.push(e)
                             }
                             var f = a.createReader(),
                                 h = [],
                                 p = function() {
                                     f.readEntries(function(e) {
                                         try {
                                             e.length ? (h = h.concat(Array.prototype.slice.call(e || [], 0)), p()) : (angular.forEach(h.slice(0), function(c) {
@@ -1055,26 +1136,28 @@
                                 c.reject(d)
                             }
                         }, function(a) {
                             c.reject(a)
                         });
                     return c.promise
                 }
-                var j = i.getValidationAttr(d, a, "maxFiles") || Number.MAX_VALUE,
-                    l = i.getValidationAttr(d, a, "maxTotalSize") || Number.MAX_VALUE,
-                    m = r("ngfIncludeDir", a),
+                var j = i.getValidationAttr(d, a, "maxFiles");
+                null == j && (j = Number.MAX_VALUE);
+                var l = i.getValidationAttr(d, a, "maxTotalSize");
+                null == l && (l = Number.MAX_VALUE);
+                var m = s("ngfIncludeDir", a),
                     n = [],
                     o = 0,
                     p = [i.emptyPromise()];
-                if (b && b.length > 0 && "file" !== h.protocol())
+                if (b && b.length > 0 && "file:" !== h.location.protocol)
                     for (var q = 0; q < b.length; q++) {
                         if (b[q].webkitGetAsEntry && b[q].webkitGetAsEntry() && b[q].webkitGetAsEntry().isDirectory) {
-                            var s = b[q].webkitGetAsEntry();
-                            if (s.isDirectory && !e) continue;
-                            null != s && p.push(g(s))
+                            var r = b[q].webkitGetAsEntry();
+                            if (r.isDirectory && !e) continue;
+                            null != r && p.push(g(r))
                         } else {
                             var t = b[q].getAsFile();
                             null != t && (n.push(t), o += t.size)
                         }
                         if (n.length > j || o > l || !f && n.length > 0) break
                     } else if (null != c)
                         for (var u = 0; u < c.length; u++) {
@@ -1088,81 +1171,63 @@
                         for (var a = 0; n[a] && "directory" === n[a].type;) a++;
                         w.resolve([n[a]])
                     }
                 }, function(a) {
                     w.reject(a)
                 }), w.promise
             }
-            var q = b(),
-                r = function(a, b, c) {
+            var r = b(),
+                s = function(a, b, c) {
                     return i.attrGetter(a, d, b, c)
                 };
-            if (r("dropAvailable") && g(function() {
-                    a[r("dropAvailable")] ? a[r("dropAvailable")].value = q : a[r("dropAvailable")] = q
-                }), !q) return void(r("ngfHideOnDropNotAvailable", a) === !0 && c.css("display", "none"));
-            null == r("ngfSelect") && i.registerModelChangeValidator(e, d, a);
-            var s, t = null,
-                u = f(r("ngfStopPropagation")),
-                v = 1;
+            if (s("dropAvailable") && g(function() {
+                    a[s("dropAvailable")] ? a[s("dropAvailable")].value = r : a[s("dropAvailable")] = r
+                }), !r) return void(s("ngfHideOnDropNotAvailable", a) === !0 && c.css("display", "none"));
+            null == s("ngfSelect") && i.registerModelChangeValidator(e, d, a);
+            var t, u = null,
+                v = f(s("ngfStopPropagation")),
+                w = 1;
             c[0].addEventListener("dragover", function(b) {
                 if (!l() && i.shouldUpdateOn("drop", d, a)) {
-                    if (b.preventDefault(), u(a) && b.stopPropagation(), navigator.userAgent.indexOf("Chrome") > -1) {
+                    if (b.preventDefault(), v(a) && b.stopPropagation(), navigator.userAgent.indexOf("Chrome") > -1) {
                         var e = b.dataTransfer.effectAllowed;
                         b.dataTransfer.dropEffect = "move" === e || "linkMove" === e ? "move" : "copy"
                     }
-                    g.cancel(t), s || (s = "C", o(a, d, b, function(d) {
-                        s = d, c.addClass(s), r("ngfDrag", a, {
+                    g.cancel(u), t || (t = "C", p(a, d, b, function(d) {
+                        t = d, c.addClass(t), s("ngfDrag", a, {
                             $isDragging: !0,
-                            $class: s,
+                            $class: t,
                             $event: b
                         })
                     }))
                 }
             }, !1), c[0].addEventListener("dragenter", function(b) {
-                !l() && i.shouldUpdateOn("drop", d, a) && (b.preventDefault(), u(a) && b.stopPropagation())
+                !l() && i.shouldUpdateOn("drop", d, a) && (b.preventDefault(), v(a) && b.stopPropagation())
             }, !1), c[0].addEventListener("dragleave", function(b) {
-                !l() && i.shouldUpdateOn("drop", d, a) && (b.preventDefault(), u(a) && b.stopPropagation(), t = g(function() {
-                    s && c.removeClass(s), s = null, r("ngfDrag", a, {
-                        $isDragging: !1,
-                        $event: b
-                    })
-                }, v || 100))
-            }, !1), c[0].addEventListener("drop", function(b) {
-                if (!l() && i.shouldUpdateOn("drop", d, a)) {
-                    b.preventDefault(), u(a) && b.stopPropagation(), s && c.removeClass(s), s = null;
-                    var e, f = b.dataTransfer.items;
-                    try {
-                        e = b.dataTransfer && b.dataTransfer.getData && b.dataTransfer.getData("text/html")
-                    } catch (g) {}
-                    p(f, b.dataTransfer.files, r("ngfAllowDir", a) !== !1, r("multiple") || r("ngfMultiple", a)).then(function(a) {
-                        a.length ? m(a, b) : n("dropUrl", e).then(function(a) {
-                            m(a, b)
+                !l() && i.shouldUpdateOn("drop", d, a) && (b.preventDefault(),
+                    v(a) && b.stopPropagation(), u = g(function() {
+                        t && c.removeClass(t), t = null, s("ngfDrag", a, {
+                            $isDragging: !1,
+                            $event: b
                         })
-                    })
-                }
+                    }, w || 100))
+            }, !1), c[0].addEventListener("drop", function(b) {
+                !l() && i.shouldUpdateOn("drop", d, a) && (b.preventDefault(), v(a) && b.stopPropagation(), t && c.removeClass(t), t = null, m(b.dataTransfer, b, "dropUrl"))
             }, !1), c[0].addEventListener("paste", function(b) {
-                if (navigator.userAgent.toLowerCase().indexOf("firefox") > -1 && r("ngfEnableFirefoxPaste", a) && b.preventDefault(), !l() && i.shouldUpdateOn("paste", d, a)) {
-                    var c = [],
-                        e = b.clipboardData || b.originalEvent.clipboardData;
-                    if (e && e.items)
-                        for (var f = 0; f < e.items.length; f++) - 1 !== e.items[f].type.indexOf("image") && c.push(e.items[f].getAsFile());
-                    c.length ? m(c, b) : n("pasteUrl", e).then(function(a) {
-                        m(a, b)
-                    })
-                }
-            }, !1), navigator.userAgent.toLowerCase().indexOf("firefox") > -1 && r("ngfEnableFirefoxPaste", a) && (c.attr("contenteditable", !0), c.on("keypress", function(a) {
+                navigator.userAgent.toLowerCase().indexOf("firefox") > -1 && s("ngfEnableFirefoxPaste", a) && b.preventDefault(), !l() && i.shouldUpdateOn("paste", d, a) && m(b.clipboardData || b.originalEvent.clipboardData, b, "pasteUrl")
+            }, !1), navigator.userAgent.toLowerCase().indexOf("firefox") > -1 && s("ngfEnableFirefoxPaste", a) && (c.attr("contenteditable", !0), c.on("keypress", function(a) {
                 a.metaKey || a.ctrlKey || a.preventDefault()
             }))
         }
 
         function b() {
             var a = document.createElement("div");
             return "draggable" in a && "ondrop" in a && !/Edge\/12./i.test(navigator.userAgent)
         }
-        ngFileUpload.directive("ngfDrop", ["$parse", "$timeout", "$location", "Upload", "$http", "$q", function(b, c, d, e, f, g) {
+        ngFileUpload.directive("ngfDrop", ["$parse", "$timeout", "$window", "Upload", "$http", "$q", function(b, c, d, e, f, g) {
             return {
                 restrict: "AEC",
                 require: "?ngModel",
                 link: function(h, i, j, k) {
                     a(h, i, j, k, b, c, d, e, f, g)
                 }
             }
```

### Comparing `XStatic-Angular-FileUpload-12.0.4.0/XStatic_Angular_FileUpload.egg-info/PKG-INFO` & `XStatic-Angular-FileUpload-12.2.13.0/XStatic_Angular_FileUpload.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 1.0
+Metadata-Version: 1.2
 Name: XStatic-Angular-FileUpload
-Version: 12.0.4.0
-Summary: Angular-FileUpload 12.0.4 (XStatic packaging standard)
+Version: 12.2.13.0
+Summary: Angular-FileUpload 12.2.13 (XStatic packaging standard)
 Home-page: https://github.com/danialfarid/angular-file-upload
-Author: Rob Cresswell
-Author-email: robert.cresswell@outlook.com
+Maintainer: Radomir Dopieralski
+Maintainer-email: openstack@sheep.art.pl
 License: (same as Angular-FileUpload)
 Description: XStatic-Angular-Filepload
         -------------------------
         
         Angular-FileUpload JavaScript library packaged for setuptools (easy_install) / pip.
         
         This package is intended to be used by **any** project that needs these files.
```

### Comparing `XStatic-Angular-FileUpload-12.0.4.0/XStatic_Angular_FileUpload.egg-info/SOURCES.txt` & `XStatic-Angular-FileUpload-12.2.13.0/XStatic_Angular_FileUpload.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 MANIFEST.in
 README.txt
+setup.cfg
 setup.py
 XStatic_Angular_FileUpload.egg-info/PKG-INFO
 XStatic_Angular_FileUpload.egg-info/SOURCES.txt
 XStatic_Angular_FileUpload.egg-info/dependency_links.txt
 XStatic_Angular_FileUpload.egg-info/namespace_packages.txt
 XStatic_Angular_FileUpload.egg-info/not-zip-safe
 XStatic_Angular_FileUpload.egg-info/top_level.txt
```

