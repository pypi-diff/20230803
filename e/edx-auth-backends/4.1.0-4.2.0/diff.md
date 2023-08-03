# Comparing `tmp/edx-auth-backends-4.1.0.tar.gz` & `tmp/edx-auth-backends-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-auth-backends-4.1.0.tar", last modified: Fri Jan 28 15:14:25 2022, max compression
+gzip compressed data, was "edx-auth-backends-4.2.0.tar", last modified: Thu Aug  3 13:34:59 2023, max compression
```

## Comparing `edx-auth-backends-4.1.0.tar` & `edx-auth-backends-4.2.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 15:14:25.947736 edx-auth-backends-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     1820 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35136 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11017 2022-01-28 15:14:25.947736 edx-auth-backends-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7575 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 15:14:25.947736 edx-auth-backends-4.1.0/auth_backends/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/auth_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5108 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/auth_backends/backends.py
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/auth_backends/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     3216 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/auth_backends/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 15:14:25.947736 edx-auth-backends-4.1.0/auth_backends/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/auth_backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2245 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/auth_backends/tests/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     6516 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/auth_backends/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (121)     2269 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/auth_backends/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/auth_backends/tests/test_strategies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/auth_backends/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/auth_backends/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2786 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/auth_backends/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 15:14:25.947736 edx-auth-backends-4.1.0/edx_auth_backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11017 2022-01-28 15:14:25.000000 edx-auth-backends-4.1.0/edx_auth_backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-01-28 15:14:25.000000 edx-auth-backends-4.1.0/edx_auth_backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-28 15:14:25.000000 edx-auth-backends-4.1.0/edx_auth_backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-01-28 15:14:25.000000 edx-auth-backends-4.1.0/edx_auth_backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-28 15:14:25.000000 edx-auth-backends-4.1.0/edx_auth_backends.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 15:14:25.947736 edx-auth-backends-4.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-01-28 15:14:25.951736 edx-auth-backends-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4874 2022-01-28 15:14:22.000000 edx-auth-backends-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:34:59.550680 edx-auth-backends-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-08-03 13:34:35.000000 edx-auth-backends-4.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     1909 2023-08-03 13:34:35.000000 edx-auth-backends-4.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2555 2023-08-03 13:34:35.000000 edx-auth-backends-4.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-08-03 13:34:35.000000 edx-auth-backends-4.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-08-03 13:34:35.000000 edx-auth-backends-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10855 2023-08-03 13:34:59.550680 edx-auth-backends-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7425 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:34:59.546679 edx-auth-backends-4.2.0/auth_backends/
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5108 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3216 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:34:59.550680 edx-auth-backends-4.2.0/auth_backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2245 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/tests/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6457 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2269 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/tests/test_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/auth_backends/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:34:59.550680 edx-auth-backends-4.2.0/edx_auth_backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10855 2023-08-03 13:34:59.000000 edx-auth-backends-4.2.0/edx_auth_backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-08-03 13:34:59.000000 edx-auth-backends-4.2.0/edx_auth_backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 13:34:59.000000 edx-auth-backends-4.2.0/edx_auth_backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-08-03 13:34:59.000000 edx-auth-backends-4.2.0/edx_auth_backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-08-03 13:34:59.000000 edx-auth-backends-4.2.0/edx_auth_backends.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 13:34:59.550680 edx-auth-backends-4.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-08-03 13:34:59.550680 edx-auth-backends-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-08-03 13:34:36.000000 edx-auth-backends-4.2.0/setup.py
```

### Comparing `edx-auth-backends-4.1.0/CHANGELOG.rst` & `edx-auth-backends-4.2.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
 *
 
+[4.2.0] - 2023-08-03
+--------------------
+
+Added
+~~~~~~~
+* Added support for Django 4.2
+
 [4.1.0] - 2022-01-28
 --------------------
 
 Removed
 ~~~~~~~
 
 * Removed Django22, 30, 31
```

### Comparing `edx-auth-backends-4.1.0/HISTORY.rst` & `edx-auth-backends-4.2.0/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 Updated LoginRedirectBaseView to include querystring
 
 [unlisted]
 ----------
 
 Intervening releases not documented here; see Releases:
 
-https://github.com/edx/auth-backends/releases?after=1.1.2
+https://github.com/openedx/auth-backends/releases?after=1.1.2
 
 
 0.1.3 (2015-03-31)
 ------------------
 
 - Update required version of Python Social Auth to 0.2.3.
```

### Comparing `edx-auth-backends-4.1.0/LICENSE.txt` & `edx-auth-backends-4.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.1.0/PKG-INFO` & `edx-auth-backends-4.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edx-auth-backends
-Version: 4.1.0
+Version: 4.2.0
 Summary: Custom edX authentication backends and pipeline steps
-Home-page: https://github.com/edx/auth-backends
+Home-page: https://github.com/openedx/auth-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Keywords: authentication edx
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -20,16 +19,16 @@
 Classifier: Framework :: Django :: 4.0
 Classifier: Topic :: Internet
 License-File: LICENSE.txt
 License-File: AUTHORS
 
 auth-backends  |CI|_ |Codecov|_
 ===================================
-.. |CI| image:: https://github.com/edx/auth-backends/workflows/Python%20CI/badge.svg?branch=master
-.. _CI: https://github.com/edx/auth-backends/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/auth-backends/workflows/Python%20CI/badge.svg?branch=master
+.. _CI: https://github.com/openedx/auth-backends/actions?query=workflow%3A%22Python+CI%22
 
 .. |Codecov| image:: http://codecov.io/github/edx/auth-backends/coverage.svg?branch=master
 .. _Codecov: http://codecov.io/github/edx/auth-backends?branch=master
 
 This package contains custom authentication backends, views, and pipeline steps used by edX services for single sign-on.
 
 This package is compatible with Python 3.8, Django 2.2 and Django 3.0
@@ -138,15 +137,15 @@
 
 Call ``make test``.
 
 Publishing a Release
 --------------------
 
 After a PR merges, create a new tag from ``master`` branch with a new version of the package and create a
-`Github release <https://github.com/edx/auth-backends/releases>`_
+`Github release <https://github.com/openedx/auth-backends/releases>`_
 using the new tag that will automatically publish the package to PyPi when a release is created.
 
 
 License
 -------
 
 The code in this repository is licensed under the AGPL unless otherwise noted.
@@ -154,18 +153,15 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome!
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though it was written with `edx-platform <https://github.com/edx/edx-platform>`_ in mind,
-the guidelines should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Mailing List and IRC Channel
@@ -270,15 +266,15 @@
 Updated LoginRedirectBaseView to include querystring
 
 [unlisted]
 ----------
 
 Intervening releases not documented here; see Releases:
 
-https://github.com/edx/auth-backends/releases?after=1.1.2
+https://github.com/openedx/auth-backends/releases?after=1.1.2
 
 
 0.1.3 (2015-03-31)
 ------------------
 
 - Update required version of Python Social Auth to 0.2.3.
 
@@ -291,9 +287,7 @@
 ------------------
 
 - Initial release.
 
 
 Renzo Lucioni <renzo@edx.org>
 Troy Sankey <tsankey@edx.org>
-
-
```

### Comparing `edx-auth-backends-4.1.0/README.rst` & `edx-auth-backends-4.2.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 auth-backends  |CI|_ |Codecov|_
 ===================================
-.. |CI| image:: https://github.com/edx/auth-backends/workflows/Python%20CI/badge.svg?branch=master
-.. _CI: https://github.com/edx/auth-backends/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/auth-backends/workflows/Python%20CI/badge.svg?branch=master
+.. _CI: https://github.com/openedx/auth-backends/actions?query=workflow%3A%22Python+CI%22
 
 .. |Codecov| image:: http://codecov.io/github/edx/auth-backends/coverage.svg?branch=master
 .. _Codecov: http://codecov.io/github/edx/auth-backends?branch=master
 
 This package contains custom authentication backends, views, and pipeline steps used by edX services for single sign-on.
 
 This package is compatible with Python 3.8, Django 2.2 and Django 3.0
@@ -114,15 +114,15 @@
 
 Call ``make test``.
 
 Publishing a Release
 --------------------
 
 After a PR merges, create a new tag from ``master`` branch with a new version of the package and create a
-`Github release <https://github.com/edx/auth-backends/releases>`_
+`Github release <https://github.com/openedx/auth-backends/releases>`_
 using the new tag that will automatically publish the package to PyPi when a release is created.
 
 
 License
 -------
 
 The code in this repository is licensed under the AGPL unless otherwise noted.
@@ -130,18 +130,15 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome!
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though it was written with `edx-platform <https://github.com/edx/edx-platform>`_ in mind,
-the guidelines should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Mailing List and IRC Channel
```

### Comparing `edx-auth-backends-4.1.0/auth_backends/backends.py` & `edx-auth-backends-4.2.0/auth_backends/backends.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.1.0/auth_backends/pipeline.py` & `edx-auth-backends-4.2.0/auth_backends/pipeline.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.1.0/auth_backends/strategies.py` & `edx-auth-backends-4.2.0/auth_backends/strategies.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.1.0/auth_backends/tests/mixins.py` & `edx-auth-backends-4.2.0/auth_backends/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.1.0/auth_backends/tests/test_backends.py` & `edx-auth-backends-4.2.0/auth_backends/tests/test_backends.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """ Tests for the backends. """
 import datetime
 import json
 from calendar import timegm
 
+import jwt
 import six
 from Cryptodome.PublicKey import RSA
 from django.core.cache import cache
-from jwkest.jwk import RSAKey
-from jwkest.jws import JWS
 from social_core.tests.backends.oauth import OAuth2Test
 
 
 class EdXOAuth2Tests(OAuth2Test):
     """ Tests for the EdXOAuth2 backend. """
 
     backend_path = 'auth_backends.backends.EdXOAuth2'
@@ -21,15 +20,15 @@
     url_root = 'https://example.com'
     public_url_root = 'https://public.example.com'
     logout_redirect_url = 'https://example.com/logout_redirect'
 
     def setUp(self):
         cache.clear()
         super().setUp()
-        self.key = RSAKey(kid='testkey', key=RSA.generate(2048))
+        self.key = RSA.generate(2048).export_key('PEM')
 
     def set_social_auth_setting(self, setting_name, value):
         """
         Set a social auth django setting during the middle of a test.
         """
         # The inherited backend defines self.name, i.e. "EDX_OAUTH2".
         backend_name = self.name
@@ -41,35 +40,35 @@
     def access_token_body(self, request, _url, headers):
         """ Generates a response from the provider's access token endpoint. """
         # The backend should always request JWT access tokens, not Bearer.
         body = six.moves.urllib.parse.parse_qs(request.body.decode('utf8'))
         self.assertEqual(body['token_type'], ['jwt'])
 
         expires_in = 3600
-        access_token = self.create_jws_access_token(expires_in)
+        access_token = self.create_jwt_access_token(expires_in)
         body = json.dumps({
             'scope': 'read write profile email user_id',
             'token_type': 'JWT',
             'expires_in': expires_in,
             'access_token': access_token
         })
         return 200, headers, body
 
-    def create_jws_access_token(self, expires_in=3600, issuer=None, key=None, alg='RS512'):
+    def create_jwt_access_token(self, expires_in=3600, issuer=None, key=None, alg='RS512'):
         """
-        Creates a signed (JWS) access token.
+        Creates a signed (JWT) access token.
 
         Arguments:
             expires_in (int): Number of seconds after which the token expires.
             issuer (str): Issuer of the token.
-            key (jwkest.jwk.Key): Key used to sign the token.
+            key (bytes PEM-format): Key used to sign the token.
             alg (str): Signing algorithm.
 
         Returns:
-            str: JWS
+            str: JWT
         """
         key = key or self.key
         now = datetime.datetime.utcnow()
         expiration_datetime = now + datetime.timedelta(seconds=expires_in)
         issue_datetime = now
         payload = {
             'iss': issuer or self.url_root,
@@ -82,15 +81,15 @@
             'scopes': ['read', 'write', 'profile', 'email', 'user_id'],
             'email': 'jsmith@example.com',
             'exp': timegm(expiration_datetime.utctimetuple()),
             'name': 'Joe Smith',
             'family_name': 'Smith',
             'user_id': '1',
         }
-        access_token = JWS(payload, jwk=key, alg=alg).sign_compact()
+        access_token = jwt.encode(payload, key, algorithm=alg)
         return access_token
 
     def extra_settings(self):
         """
         Create extra Django settings for use with tests.
         """
         settings = super().extra_settings()
@@ -146,15 +145,15 @@
         self.assertEqual(self.backend.end_session_url(), self.url_root + logout_location)
 
         # Now, add the public url root to the settings.
         self.set_social_auth_setting('PUBLIC_URL_ROOT', self.public_url_root)
         self.assertEqual(self.backend.end_session_url(), self.public_url_root + logout_location)
 
     def test_user_data(self):
-        user_data = self.backend.user_data(self.create_jws_access_token())
+        user_data = self.backend.user_data(self.create_jwt_access_token())
         self.assertDictEqual(user_data, {
             'name': 'Joe Smith',
             'preferred_username': 'jsmith',
             'email': 'jsmith@example.com',
             'given_name': 'Joe',
             'user_id': '1',
             'family_name': 'Smith',
```

### Comparing `edx-auth-backends-4.1.0/auth_backends/tests/test_pipeline.py` & `edx-auth-backends-4.2.0/auth_backends/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.1.0/auth_backends/tests/test_strategies.py` & `edx-auth-backends-4.2.0/auth_backends/tests/test_strategies.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.1.0/auth_backends/tests/test_views.py` & `edx-auth-backends-4.2.0/auth_backends/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.1.0/auth_backends/views.py` & `edx-auth-backends-4.2.0/auth_backends/views.py`

 * *Files identical despite different names*

### Comparing `edx-auth-backends-4.1.0/edx_auth_backends.egg-info/PKG-INFO` & `edx-auth-backends-4.2.0/edx_auth_backends.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edx-auth-backends
-Version: 4.1.0
+Version: 4.2.0
 Summary: Custom edX authentication backends and pipeline steps
-Home-page: https://github.com/edx/auth-backends
+Home-page: https://github.com/openedx/auth-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Keywords: authentication edx
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -20,16 +19,16 @@
 Classifier: Framework :: Django :: 4.0
 Classifier: Topic :: Internet
 License-File: LICENSE.txt
 License-File: AUTHORS
 
 auth-backends  |CI|_ |Codecov|_
 ===================================
-.. |CI| image:: https://github.com/edx/auth-backends/workflows/Python%20CI/badge.svg?branch=master
-.. _CI: https://github.com/edx/auth-backends/actions?query=workflow%3A%22Python+CI%22
+.. |CI| image:: https://github.com/openedx/auth-backends/workflows/Python%20CI/badge.svg?branch=master
+.. _CI: https://github.com/openedx/auth-backends/actions?query=workflow%3A%22Python+CI%22
 
 .. |Codecov| image:: http://codecov.io/github/edx/auth-backends/coverage.svg?branch=master
 .. _Codecov: http://codecov.io/github/edx/auth-backends?branch=master
 
 This package contains custom authentication backends, views, and pipeline steps used by edX services for single sign-on.
 
 This package is compatible with Python 3.8, Django 2.2 and Django 3.0
@@ -138,15 +137,15 @@
 
 Call ``make test``.
 
 Publishing a Release
 --------------------
 
 After a PR merges, create a new tag from ``master`` branch with a new version of the package and create a
-`Github release <https://github.com/edx/auth-backends/releases>`_
+`Github release <https://github.com/openedx/auth-backends/releases>`_
 using the new tag that will automatically publish the package to PyPi when a release is created.
 
 
 License
 -------
 
 The code in this repository is licensed under the AGPL unless otherwise noted.
@@ -154,18 +153,15 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome!
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though it was written with `edx-platform <https://github.com/edx/edx-platform>`_ in mind,
-the guidelines should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Mailing List and IRC Channel
@@ -270,15 +266,15 @@
 Updated LoginRedirectBaseView to include querystring
 
 [unlisted]
 ----------
 
 Intervening releases not documented here; see Releases:
 
-https://github.com/edx/auth-backends/releases?after=1.1.2
+https://github.com/openedx/auth-backends/releases?after=1.1.2
 
 
 0.1.3 (2015-03-31)
 ------------------
 
 - Update required version of Python Social Auth to 0.2.3.
 
@@ -291,9 +287,7 @@
 ------------------
 
 - Initial release.
 
 
 Renzo Lucioni <renzo@edx.org>
 Troy Sankey <tsankey@edx.org>
-
-
```

### Comparing `edx-auth-backends-4.1.0/edx_auth_backends.egg-info/SOURCES.txt` & `edx-auth-backends-4.2.0/edx_auth_backends.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 AUTHORS
 CHANGELOG.rst
-CONTRIBUTING.rst
 HISTORY.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 auth_backends/__init__.py
```

### Comparing `edx-auth-backends-4.1.0/setup.py` & `edx-auth-backends-4.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,14 @@
         'Programming Language :: Python :: 3.8',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Topic :: Internet',
     ],
     keywords='authentication edx',
-    url='https://github.com/edx/auth-backends',
+    url='https://github.com/openedx/auth-backends',
     author='edX',
     author_email='oscm@edx.org',
     license='AGPL',
     packages=find_packages(),
     install_requires=load_requirements('requirements/base.in'),
 )
```

