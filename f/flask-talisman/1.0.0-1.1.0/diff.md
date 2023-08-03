# Comparing `tmp/flask-talisman-1.0.0.tar.gz` & `tmp/flask-talisman-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-talisman-1.0.0.tar", last modified: Thu Mar 17 14:23:19 2022, max compression
+gzip compressed data, was "flask-talisman-1.1.0.tar", last modified: Thu Aug  3 12:00:25 2023, max compression
```

## Comparing `flask-talisman-1.0.0.tar` & `flask-talisman-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 stargirl   (501) staff       (20)        0 2022-03-17 14:23:19.514867 flask-talisman-1.0.0/
--rw-r--r--   0 stargirl   (501) staff       (20)    11357 2021-06-06 13:21:51.000000 flask-talisman-1.0.0/LICENSE
--rw-r--r--   0 stargirl   (501) staff       (20)    18317 2022-03-17 14:23:19.514948 flask-talisman-1.0.0/PKG-INFO
--rw-r--r--   0 stargirl   (501) staff       (20)    17301 2022-03-17 14:05:46.000000 flask-talisman-1.0.0/README.rst
-drwxr-xr-x   0 stargirl   (501) staff       (20)        0 2022-03-17 14:23:19.514295 flask-talisman-1.0.0/flask_talisman/
--rw-r--r--   0 stargirl   (501) staff       (20)     1027 2022-03-17 14:05:46.000000 flask-talisman-1.0.0/flask_talisman/__init__.py
--rw-r--r--   0 stargirl   (501) staff       (20)    16979 2022-03-17 14:05:46.000000 flask-talisman-1.0.0/flask_talisman/talisman.py
--rw-r--r--   0 stargirl   (501) staff       (20)    13767 2022-03-17 14:05:46.000000 flask-talisman-1.0.0/flask_talisman/talisman_test.py
-drwxr-xr-x   0 stargirl   (501) staff       (20)        0 2022-03-17 14:23:19.514766 flask-talisman-1.0.0/flask_talisman.egg-info/
--rw-r--r--   0 stargirl   (501) staff       (20)    18317 2022-03-17 14:23:19.000000 flask-talisman-1.0.0/flask_talisman.egg-info/PKG-INFO
--rw-r--r--   0 stargirl   (501) staff       (20)      275 2022-03-17 14:23:19.000000 flask-talisman-1.0.0/flask_talisman.egg-info/SOURCES.txt
--rw-r--r--   0 stargirl   (501) staff       (20)        1 2022-03-17 14:23:19.000000 flask-talisman-1.0.0/flask_talisman.egg-info/dependency_links.txt
--rw-r--r--   0 stargirl   (501) staff       (20)       15 2022-03-17 14:23:19.000000 flask-talisman-1.0.0/flask_talisman.egg-info/top_level.txt
--rw-r--r--   0 stargirl   (501) staff       (20)      119 2022-03-17 14:23:19.515248 flask-talisman-1.0.0/setup.cfg
--rw-r--r--   0 stargirl   (501) staff       (20)     1828 2022-03-17 14:06:55.000000 flask-talisman-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:00:25.545419 flask-talisman-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 12:00:17.000000 flask-talisman-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18722 2023-08-03 12:00:25.545419 flask-talisman-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17706 2023-08-03 12:00:17.000000 flask-talisman-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:00:25.545419 flask-talisman-1.1.0/flask_talisman/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-08-03 12:00:17.000000 flask-talisman-1.1.0/flask_talisman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-08-03 12:00:17.000000 flask-talisman-1.1.0/flask_talisman/talisman.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-08-03 12:00:17.000000 flask-talisman-1.1.0/flask_talisman/talisman_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:00:25.545419 flask-talisman-1.1.0/flask_talisman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18722 2023-08-03 12:00:25.000000 flask-talisman-1.1.0/flask_talisman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-03 12:00:25.000000 flask-talisman-1.1.0/flask_talisman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:00:25.000000 flask-talisman-1.1.0/flask_talisman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 12:00:25.000000 flask-talisman-1.1.0/flask_talisman.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-03 12:00:25.545419 flask-talisman-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-08-03 12:00:17.000000 flask-talisman-1.1.0/setup.py
```

### Comparing `flask-talisman-1.0.0/LICENSE` & `flask-talisman-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-talisman-1.0.0/PKG-INFO` & `flask-talisman-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-talisman
-Version: 1.0.0
+Version: 1.1.0
 Summary: HTTP security headers for Flask.
 Home-page: https://github.com/wntrblm/flask-talisman
 Author: Alethea Katherine Flowers
 Author-email: me@thea.codes
 License: Apache Software License
 Keywords: flask security https xss
 Platform: UNKNOWN
@@ -45,30 +45,28 @@
    cookie and should be unaffected.
 -  Sets Flask's session cookie to ``Lax``, preventing the cookie to be leaked
    in CSRF-prone request methods.
 -  Sets
    `X-Frame-Options <https://developer.mozilla.org/en-US/docs/Web/HTTP/X-Frame-Options>`_
    to ``SAMEORIGIN`` to avoid
    `clickjacking <https://en.wikipedia.org/wiki/Clickjacking>`_.
--  Sets `X-XSS-Protection
-   <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection>`_
-   to enable a cross site scripting filter for IE and Safari (note Chrome has
-   removed this and Firefox never supported it).
 -  Sets `X-Content-Type-Options
    <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Content-Type-Options>`_
    to prevent content type sniffing.
 -  Sets a strict `Content Security
    Policy <https://developer.mozilla.org/en-US/docs/Web/Security/CSP/Introducing_Content_Security_Policy>`__
    of ``default-src: 'self', 'object-src': 'none'``. This is intended to almost completely
    prevent Cross Site Scripting (XSS) attacks. This is probably the only
    setting that you should reasonably change. See the
    `Content Security Policy`_ section.
 -  Sets a strict `Referrer-Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Referrer-Policy>`_
    of ``strict-origin-when-cross-origin`` that governs which referrer information should be included with
    requests made.
+-  Disables ``browsing-topics`` by default in the `Permissions-Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Feature-Policy>`_
+   like `Drupal <https://www.drupal.org/project/drupal/issues/3209628>`_ to enhance privacy protection.
 
 
 In addition to Talisman, you **should always use a cross-site request
 forgery (CSRF) library**. It's highly recommended to use
 `Flask-SeaSurf <https://flask-seasurf.readthedocs.org/en/latest/>`_,
 which is based on Django's excellent library.
 
@@ -136,15 +134,15 @@
 -  ``referrer_policy``, default ``strict-origin-when-cross-origin``, a string
    that sets the Referrer Policy header to send a full URL when performing a same-origin
    request, only send the origin of the document to an equally secure destination
    (HTTPS->HTTPS), and send no header to a less secure destination (HTTPS->HTTP) (`about Referrer Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Referrer-Policy>`_).
 
 -  ``feature_policy``, default ``{}``, see the `Feature Policy`_ section (`about Feature Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Feature_Policy>`_).
 
--  ``permissions_policy``, default ``{}``, see the `Permissions Policy`_ section (`about Permissions Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Feature_Policy>`_).
+-  ``permissions_policy``, default ``{'browsing-topics': '()'}``, see the `Permissions Policy`_ section (`about Permissions Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Feature_Policy>`_).
 -  ``document_policy``, default ``{}``, see the `Document Policy`_ section (`about Document Policy <https://wicg.github.io/document-policy/>`_).
 
 -  ``session_cookie_secure``, default ``True``, set the session cookie
    to ``secure``, preventing it from being sent over plain ``http`` (`about cookies (https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie)_`).
 -  ``session_cookie_http_only``, default ``True``, set the session
    cookie to ``httponly``, preventing it from being read by JavaScript.
 -  ``session_cookie_samesite``, default ``Lax``, set this to ``Strict`` to prevent the cookie from being sent by the browser to the target site in all cross-site browsing context, even when following a regular link.
@@ -152,15 +150,15 @@
 
 -  ``force_file_save``, default ``False``, whether to set the
    `X-Download-Options <https://docs.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/compatibility/jj542450(v=vs.85)?redirectedfrom=MSDN>`_
    header to ``noopen`` to prevent IE >= 8 to from opening file downloads
    directly and only save them instead.
 
 -  ``x_content_type_options``, default ``True``, Protects against MIME sniffing vulnerabilities (`about Content Type Options <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Content-Type-Options>`_).
--  ``x_xss_protection``, default ``True``, Protects against cross-site scripting (XSS) attacks (`about XSS Protection <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection>`_).
+-  ``x_xss_protection``, default ``False``, Protects against cross-site scripting (XSS) attacks (`about XSS Protection <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection>`_). This option is disabled by default because no modern browser (`supports this header <https://caniuse.com/mdn-http_headers_x-xss-protection>`_) anymore.
 
 For a full list of (security) headers, check out: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers.
 
 Per-view options
 ~~~~~~~~~~~~~~~~
 
 Sometimes you want to change the policy for a specific view. The
@@ -397,35 +395,39 @@
 
 When the same feature or permission is set in both Feature Policy and Permission Policy,
 the Permission Policy setting will take precedence in browsers that support both.
 
 It should be noted that the syntax differs between Feature Policy and Permission Policy
 as can be seen from the ``geolocation`` examples provided.
 
+The default Permissions Policy is ``browsing-topics=()``, which opts sites out of
+`Federated Learning of Cohorts <https://wicg.github.io/floc/>`_ an interest-based advertising initiative
+called Topics API.
+
 Permission Policy can be set either using a dictionary, or using a string.
 
 Geolocation and Microphone Example
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Disable access to Geolocation interface and Microphone using dictionary syntax
 
 .. code:: python
 
-    permission_policy = {
+    permissions_policy = {
         'geolocation': '()',
         'microphone': '()'
     }
-    talisman = Talisman(app, permission_policy=permission_policy)
+    talisman = Talisman(app, permissions_policy=permissions_policy)
 
 Disable access to Geolocation interface and Microphone using string syntax
 
 .. code:: python
 
-    permission_policy = 'geolocation=(), microphone=()'
-    talisman = Talisman(app, permission_policy=permission_policy)
+    permissions_policy = 'geolocation=(), microphone=()'
+    talisman = Talisman(app, permissions_policy=permissions_policy)
 
 Document Policy
 ---------------
 
 Feature Policy has been split into Permissions Policy and Document Policy but
 at this writing `browser support of Document Policy is very limited <https://caniuse.com/document-policy>`_,
 and it is recommended to still set the ``Feature-Policy`` HTTP Header.
```

### Comparing `flask-talisman-1.0.0/README.rst` & `flask-talisman-1.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,28 @@
    cookie and should be unaffected.
 -  Sets Flask's session cookie to ``Lax``, preventing the cookie to be leaked
    in CSRF-prone request methods.
 -  Sets
    `X-Frame-Options <https://developer.mozilla.org/en-US/docs/Web/HTTP/X-Frame-Options>`_
    to ``SAMEORIGIN`` to avoid
    `clickjacking <https://en.wikipedia.org/wiki/Clickjacking>`_.
--  Sets `X-XSS-Protection
-   <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection>`_
-   to enable a cross site scripting filter for IE and Safari (note Chrome has
-   removed this and Firefox never supported it).
 -  Sets `X-Content-Type-Options
    <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Content-Type-Options>`_
    to prevent content type sniffing.
 -  Sets a strict `Content Security
    Policy <https://developer.mozilla.org/en-US/docs/Web/Security/CSP/Introducing_Content_Security_Policy>`__
    of ``default-src: 'self', 'object-src': 'none'``. This is intended to almost completely
    prevent Cross Site Scripting (XSS) attacks. This is probably the only
    setting that you should reasonably change. See the
    `Content Security Policy`_ section.
 -  Sets a strict `Referrer-Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Referrer-Policy>`_
    of ``strict-origin-when-cross-origin`` that governs which referrer information should be included with
    requests made.
+-  Disables ``browsing-topics`` by default in the `Permissions-Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Feature-Policy>`_
+   like `Drupal <https://www.drupal.org/project/drupal/issues/3209628>`_ to enhance privacy protection.
 
 
 In addition to Talisman, you **should always use a cross-site request
 forgery (CSRF) library**. It's highly recommended to use
 `Flask-SeaSurf <https://flask-seasurf.readthedocs.org/en/latest/>`_,
 which is based on Django's excellent library.
 
@@ -110,15 +108,15 @@
 -  ``referrer_policy``, default ``strict-origin-when-cross-origin``, a string
    that sets the Referrer Policy header to send a full URL when performing a same-origin
    request, only send the origin of the document to an equally secure destination
    (HTTPS->HTTPS), and send no header to a less secure destination (HTTPS->HTTP) (`about Referrer Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Referrer-Policy>`_).
 
 -  ``feature_policy``, default ``{}``, see the `Feature Policy`_ section (`about Feature Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Feature_Policy>`_).
 
--  ``permissions_policy``, default ``{}``, see the `Permissions Policy`_ section (`about Permissions Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Feature_Policy>`_).
+-  ``permissions_policy``, default ``{'browsing-topics': '()'}``, see the `Permissions Policy`_ section (`about Permissions Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Feature_Policy>`_).
 -  ``document_policy``, default ``{}``, see the `Document Policy`_ section (`about Document Policy <https://wicg.github.io/document-policy/>`_).
 
 -  ``session_cookie_secure``, default ``True``, set the session cookie
    to ``secure``, preventing it from being sent over plain ``http`` (`about cookies (https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie)_`).
 -  ``session_cookie_http_only``, default ``True``, set the session
    cookie to ``httponly``, preventing it from being read by JavaScript.
 -  ``session_cookie_samesite``, default ``Lax``, set this to ``Strict`` to prevent the cookie from being sent by the browser to the target site in all cross-site browsing context, even when following a regular link.
@@ -126,15 +124,15 @@
 
 -  ``force_file_save``, default ``False``, whether to set the
    `X-Download-Options <https://docs.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/compatibility/jj542450(v=vs.85)?redirectedfrom=MSDN>`_
    header to ``noopen`` to prevent IE >= 8 to from opening file downloads
    directly and only save them instead.
 
 -  ``x_content_type_options``, default ``True``, Protects against MIME sniffing vulnerabilities (`about Content Type Options <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Content-Type-Options>`_).
--  ``x_xss_protection``, default ``True``, Protects against cross-site scripting (XSS) attacks (`about XSS Protection <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection>`_).
+-  ``x_xss_protection``, default ``False``, Protects against cross-site scripting (XSS) attacks (`about XSS Protection <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection>`_). This option is disabled by default because no modern browser (`supports this header <https://caniuse.com/mdn-http_headers_x-xss-protection>`_) anymore.
 
 For a full list of (security) headers, check out: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers.
 
 Per-view options
 ~~~~~~~~~~~~~~~~
 
 Sometimes you want to change the policy for a specific view. The
@@ -371,35 +369,39 @@
 
 When the same feature or permission is set in both Feature Policy and Permission Policy,
 the Permission Policy setting will take precedence in browsers that support both.
 
 It should be noted that the syntax differs between Feature Policy and Permission Policy
 as can be seen from the ``geolocation`` examples provided.
 
+The default Permissions Policy is ``browsing-topics=()``, which opts sites out of
+`Federated Learning of Cohorts <https://wicg.github.io/floc/>`_ an interest-based advertising initiative
+called Topics API.
+
 Permission Policy can be set either using a dictionary, or using a string.
 
 Geolocation and Microphone Example
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Disable access to Geolocation interface and Microphone using dictionary syntax
 
 .. code:: python
 
-    permission_policy = {
+    permissions_policy = {
         'geolocation': '()',
         'microphone': '()'
     }
-    talisman = Talisman(app, permission_policy=permission_policy)
+    talisman = Talisman(app, permissions_policy=permissions_policy)
 
 Disable access to Geolocation interface and Microphone using string syntax
 
 .. code:: python
 
-    permission_policy = 'geolocation=(), microphone=()'
-    talisman = Talisman(app, permission_policy=permission_policy)
+    permissions_policy = 'geolocation=(), microphone=()'
+    talisman = Talisman(app, permissions_policy=permissions_policy)
 
 Document Policy
 ---------------
 
 Feature Policy has been split into Permissions Policy and Document Policy but
 at this writing `browser support of Document Policy is very limited <https://caniuse.com/document-policy>`_,
 and it is recommended to still set the ``Feature-Policy`` HTTP Header.
```

### Comparing `flask-talisman-1.0.0/flask_talisman/__init__.py` & `flask-talisman-1.1.0/flask_talisman/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-talisman-1.0.0/flask_talisman/talisman.py` & `flask-talisman-1.1.0/flask_talisman/talisman.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     'style-src': '\'self\' ajax.googleapis.com fonts.googleapis.com '
                  '*.gstatic.com',
     'object-src': '\'none\'',
     'default-src': '\'self\' *.gstatic.com',
 }
 
 DEFAULT_PERMISSIONS_POLICY = {
+    # Disable Topics API
+    'browsing-topics': '()'
 }
 
 DEFAULT_DOCUMENT_POLICY = {
 }
 
 DEFAULT_FEATURE_POLICY = {
 }
@@ -86,15 +88,15 @@
             content_security_policy_report_only=False,
             content_security_policy_nonce_in=None,
             referrer_policy=DEFAULT_REFERRER_POLICY,
             session_cookie_secure=True,
             session_cookie_http_only=True,
             session_cookie_samesite=DEFAULT_SESSION_COOKIE_SAMESITE,
             x_content_type_options=True,
-            x_xss_protection=True):
+            x_xss_protection=False):
         """
         Initialization.
 
         Args:
             app: A Flask application.
             feature_policy: A string or dictionary describing the
                 feature policy for the response.
```

### Comparing `flask-talisman-1.0.0/flask_talisman/talisman_test.py` & `flask-talisman-1.1.0/flask_talisman/talisman_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         # HTTPS request.
         response = self.client.get('/', environ_overrides=HTTPS_ENVIRON)
 
         headers = {
             'X-Frame-Options': 'SAMEORIGIN',
             'Strict-Transport-Security':
             'max-age=31556926; includeSubDomains',
-            'X-XSS-Protection': '1; mode=block',
             'X-Content-Type-Options': 'nosniff',
             'Referrer-Policy': 'strict-origin-when-cross-origin'
         }
 
         for key, value in headers.items():
             self.assertEqual(response.headers.get(key), value)
 
@@ -81,14 +80,22 @@
         self.assertEqual(response.status_code, 301)
 
         # Disable forced ssl, should allow the request.
         self.talisman.force_https = False
         response = self.client.get('/')
         self.assertEqual(response.status_code, 200)
 
+    def testForceXSSProtectionOptions(self):
+        self.talisman.x_xss_protection = True
+
+        # HTTP request from Proxy
+        response = self.client.get('/')
+        self.assertIn('X-XSS-Protection', response.headers)
+        self.assertEqual(response.headers['X-XSS-Protection'], '1; mode=block')
+
     def testHstsOptions(self):
         self.talisman.force_ssl = False
 
         # No HSTS headers for non-ssl requests
         response = self.client.get('/')
         self.assertNotIn('Strict-Transport-Security', response.headers)
 
@@ -292,20 +299,22 @@
         response = app.test_client().get('/', environ_overrides=HTTPS_ENVIRON)
         self.assertIn('vibrate \'none\'', response.headers['Feature-Policy'])
 
     def testPermissionsPolicy(self):
         self.talisman.permissions_policy['geolocation'] = '()'
         response = self.client.get('/', environ_overrides=HTTPS_ENVIRON)
         permissions_policy = response.headers['Permissions-Policy']
+        self.assertIn('browsing-topics=()', permissions_policy)
         self.assertIn('geolocation=()', permissions_policy)
 
         self.talisman.permissions_policy['geolocation'] = '()'
         self.talisman.permissions_policy['fullscreen'] = '(self, "https://example.com")'
         response = self.client.get('/', environ_overrides=HTTPS_ENVIRON)
         permissions_policy = response.headers['Permissions-Policy']
+        self.assertIn('browsing-topics=()', permissions_policy)
         self.assertIn('geolocation=(), fullscreen=(self, "https://example.com")', permissions_policy)
 
         # no policy
         self.talisman.permissions_policy = {}
         response = self.client.get('/', environ_overrides=HTTPS_ENVIRON)
         permissions_policy = response.headers.get('Permissions-Policy')
         self.assertEqual(None, permissions_policy)
```

### Comparing `flask-talisman-1.0.0/flask_talisman.egg-info/PKG-INFO` & `flask-talisman-1.1.0/flask_talisman.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-talisman
-Version: 1.0.0
+Version: 1.1.0
 Summary: HTTP security headers for Flask.
 Home-page: https://github.com/wntrblm/flask-talisman
 Author: Alethea Katherine Flowers
 Author-email: me@thea.codes
 License: Apache Software License
 Keywords: flask security https xss
 Platform: UNKNOWN
@@ -45,30 +45,28 @@
    cookie and should be unaffected.
 -  Sets Flask's session cookie to ``Lax``, preventing the cookie to be leaked
    in CSRF-prone request methods.
 -  Sets
    `X-Frame-Options <https://developer.mozilla.org/en-US/docs/Web/HTTP/X-Frame-Options>`_
    to ``SAMEORIGIN`` to avoid
    `clickjacking <https://en.wikipedia.org/wiki/Clickjacking>`_.
--  Sets `X-XSS-Protection
-   <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection>`_
-   to enable a cross site scripting filter for IE and Safari (note Chrome has
-   removed this and Firefox never supported it).
 -  Sets `X-Content-Type-Options
    <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Content-Type-Options>`_
    to prevent content type sniffing.
 -  Sets a strict `Content Security
    Policy <https://developer.mozilla.org/en-US/docs/Web/Security/CSP/Introducing_Content_Security_Policy>`__
    of ``default-src: 'self', 'object-src': 'none'``. This is intended to almost completely
    prevent Cross Site Scripting (XSS) attacks. This is probably the only
    setting that you should reasonably change. See the
    `Content Security Policy`_ section.
 -  Sets a strict `Referrer-Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Referrer-Policy>`_
    of ``strict-origin-when-cross-origin`` that governs which referrer information should be included with
    requests made.
+-  Disables ``browsing-topics`` by default in the `Permissions-Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Feature-Policy>`_
+   like `Drupal <https://www.drupal.org/project/drupal/issues/3209628>`_ to enhance privacy protection.
 
 
 In addition to Talisman, you **should always use a cross-site request
 forgery (CSRF) library**. It's highly recommended to use
 `Flask-SeaSurf <https://flask-seasurf.readthedocs.org/en/latest/>`_,
 which is based on Django's excellent library.
 
@@ -136,15 +134,15 @@
 -  ``referrer_policy``, default ``strict-origin-when-cross-origin``, a string
    that sets the Referrer Policy header to send a full URL when performing a same-origin
    request, only send the origin of the document to an equally secure destination
    (HTTPS->HTTPS), and send no header to a less secure destination (HTTPS->HTTP) (`about Referrer Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Referrer-Policy>`_).
 
 -  ``feature_policy``, default ``{}``, see the `Feature Policy`_ section (`about Feature Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Feature_Policy>`_).
 
--  ``permissions_policy``, default ``{}``, see the `Permissions Policy`_ section (`about Permissions Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Feature_Policy>`_).
+-  ``permissions_policy``, default ``{'browsing-topics': '()'}``, see the `Permissions Policy`_ section (`about Permissions Policy <https://developer.mozilla.org/en-US/docs/Web/HTTP/Feature_Policy>`_).
 -  ``document_policy``, default ``{}``, see the `Document Policy`_ section (`about Document Policy <https://wicg.github.io/document-policy/>`_).
 
 -  ``session_cookie_secure``, default ``True``, set the session cookie
    to ``secure``, preventing it from being sent over plain ``http`` (`about cookies (https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie)_`).
 -  ``session_cookie_http_only``, default ``True``, set the session
    cookie to ``httponly``, preventing it from being read by JavaScript.
 -  ``session_cookie_samesite``, default ``Lax``, set this to ``Strict`` to prevent the cookie from being sent by the browser to the target site in all cross-site browsing context, even when following a regular link.
@@ -152,15 +150,15 @@
 
 -  ``force_file_save``, default ``False``, whether to set the
    `X-Download-Options <https://docs.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/compatibility/jj542450(v=vs.85)?redirectedfrom=MSDN>`_
    header to ``noopen`` to prevent IE >= 8 to from opening file downloads
    directly and only save them instead.
 
 -  ``x_content_type_options``, default ``True``, Protects against MIME sniffing vulnerabilities (`about Content Type Options <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Content-Type-Options>`_).
--  ``x_xss_protection``, default ``True``, Protects against cross-site scripting (XSS) attacks (`about XSS Protection <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection>`_).
+-  ``x_xss_protection``, default ``False``, Protects against cross-site scripting (XSS) attacks (`about XSS Protection <https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection>`_). This option is disabled by default because no modern browser (`supports this header <https://caniuse.com/mdn-http_headers_x-xss-protection>`_) anymore.
 
 For a full list of (security) headers, check out: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers.
 
 Per-view options
 ~~~~~~~~~~~~~~~~
 
 Sometimes you want to change the policy for a specific view. The
@@ -397,35 +395,39 @@
 
 When the same feature or permission is set in both Feature Policy and Permission Policy,
 the Permission Policy setting will take precedence in browsers that support both.
 
 It should be noted that the syntax differs between Feature Policy and Permission Policy
 as can be seen from the ``geolocation`` examples provided.
 
+The default Permissions Policy is ``browsing-topics=()``, which opts sites out of
+`Federated Learning of Cohorts <https://wicg.github.io/floc/>`_ an interest-based advertising initiative
+called Topics API.
+
 Permission Policy can be set either using a dictionary, or using a string.
 
 Geolocation and Microphone Example
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Disable access to Geolocation interface and Microphone using dictionary syntax
 
 .. code:: python
 
-    permission_policy = {
+    permissions_policy = {
         'geolocation': '()',
         'microphone': '()'
     }
-    talisman = Talisman(app, permission_policy=permission_policy)
+    talisman = Talisman(app, permissions_policy=permissions_policy)
 
 Disable access to Geolocation interface and Microphone using string syntax
 
 .. code:: python
 
-    permission_policy = 'geolocation=(), microphone=()'
-    talisman = Talisman(app, permission_policy=permission_policy)
+    permissions_policy = 'geolocation=(), microphone=()'
+    talisman = Talisman(app, permissions_policy=permissions_policy)
 
 Document Policy
 ---------------
 
 Feature Policy has been split into Permissions Policy and Document Policy but
 at this writing `browser support of Document Policy is very limited <https://caniuse.com/document-policy>`_,
 and it is recommended to still set the ``Feature-Policy`` HTTP Header.
```

### Comparing `flask-talisman-1.0.0/setup.py` & `flask-talisman-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 long_description = open('README.rst', 'r', encoding='utf-8').read()
 
 
 setup(
     name='flask-talisman',
 
-    version='1.0.0',
+    version='1.1.0',
 
     description='HTTP security headers for Flask.',
     long_description=long_description,
 
     url='https://github.com/wntrblm/flask-talisman',
 
     author='Alethea Katherine Flowers',
```

