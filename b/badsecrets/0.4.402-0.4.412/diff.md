# Comparing `tmp/badsecrets-0.4.402.tar.gz` & `tmp/badsecrets-0.4.412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badsecrets-0.4.402.tar", max compression
+gzip compressed data, was "badsecrets-0.4.412.tar", max compression
```

## Comparing `badsecrets-0.4.402.tar` & `badsecrets-0.4.412.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0    35149 2023-07-28 19:44:29.402510 badsecrets-0.4.402/LICENSE
--rw-r--r--   0        0        0    32418 2023-07-28 19:44:29.402510 badsecrets-0.4.402/README.md
--rw-r--r--   0        0        0      711 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/__init__.py
--rw-r--r--   0        0        0     7763 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/base.py
--rw-r--r--   0        0        0      233 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/errors.py
--rw-r--r--   0        0        0        0 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/examples/__init__.py
--rwxr-xr-x   0        0        0     4210 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/examples/blacklist3r.py
--rwxr-xr-x   0        0        0     7939 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/examples/cli.py
--rwxr-xr-x   0        0        0     3544 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/examples/symfony_knownkey.py
--rwxr-xr-x   0        0        0    10597 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/examples/telerik_knownkey.py
--rw-r--r--   0        0        0     5076 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/helpers.py
--rw-r--r--   0        0        0        0 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/__init__.py
--rw-r--r--   0        0        0    10468 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/aspnet_viewstate.py
--rw-r--r--   0        0        0     1006 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/django_signedcookies.py
--rw-r--r--   0        0        0     2867 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/express_signedcookies_cs.py
--rw-r--r--   0        0        0     2287 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/express_signedcookies_es.py
--rw-r--r--   0        0        0     1120 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/flask_signedcookies.py
--rw-r--r--   0        0        0     4087 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/generic_jwt.py
--rw-r--r--   0        0        0    14881 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/jsf_viewstate.py
--rw-r--r--   0        0        0     2192 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/laravel_signedcookies.py
--rw-r--r--   0        0        0     1958 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/peoplesoft_pstoken.py
--rw-r--r--   0        0        0     3097 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/rails_secretkeybase.py
--rw-r--r--   0        0        0     2963 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/symfony_signedurl.py
--rw-r--r--   0        0        0     5002 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/telerik_encryptionkey.py
--rw-r--r--   0        0        0     3776 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/telerik_hashkey.py
--rw-r--r--   0        0        0   654096 2023-07-28 19:44:29.410510 badsecrets-0.4.402/badsecrets/resources/aspnet_machinekeys.txt
--rw-r--r--   0        0        0    31178 2023-07-28 19:44:29.410510 badsecrets-0.4.402/badsecrets/resources/django_secret_keys.txt
--rw-r--r--   0        0        0    40993 2023-07-28 19:44:29.410510 badsecrets-0.4.402/badsecrets/resources/express_session_secrets.txt
--rw-r--r--   0        0        0  1777603 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/flask_secret_keys.txt
--rw-r--r--   0        0        0       87 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/jsf_viewstate_passwords.txt
--rw-r--r--   0        0        0     1257 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/jsf_viewstate_passwords_b64.txt
--rw-r--r--   0        0        0     7785 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/jwt_rsakeys_private.txt
--rw-r--r--   0        0        0     2122 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/jwt_rsakeys_public.txt
--rw-r--r--   0        0        0   113170 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/jwt_secrets.txt
--rw-r--r--   0        0        0    45086 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/laravel_app_keys.txt
--rw-r--r--   0        0        0       78 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/peoplesoft_passwords.txt
--rw-r--r--   0        0        0     6184 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/rails_secret_key_base.txt
--rw-r--r--   0        0        0     3009 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/symfony_appsecret.txt
--rw-r--r--   0        0        0    18037 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/telerik_encryption_keys.txt
--rw-r--r--   0        0        0    17990 2023-07-28 19:44:29.434510 badsecrets-0.4.402/badsecrets/resources/telerik_hash_keys.txt
--rw-r--r--   0        0        0    76516 2023-07-28 19:44:29.434510 badsecrets-0.4.402/badsecrets/resources/top_10000_passwords.txt
--rw-r--r--   0        0        0      957 2023-07-28 19:44:54.770801 badsecrets-0.4.402/pyproject.toml
--rw-r--r--   0        0        0    33272 1970-01-01 00:00:00.000000 badsecrets-0.4.402/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-03 04:31:11.911296 badsecrets-0.4.412/LICENSE
+-rw-r--r--   0        0        0    32813 2023-08-03 04:31:11.911296 badsecrets-0.4.412/README.md
+-rw-r--r--   0        0        0      711 2023-08-03 04:31:11.911296 badsecrets-0.4.412/badsecrets/__init__.py
+-rw-r--r--   0        0        0     8056 2023-08-03 04:31:11.911296 badsecrets-0.4.412/badsecrets/base.py
+-rw-r--r--   0        0        0      233 2023-08-03 04:31:11.911296 badsecrets-0.4.412/badsecrets/errors.py
+-rw-r--r--   0        0        0        0 2023-08-03 04:31:11.911296 badsecrets-0.4.412/badsecrets/examples/__init__.py
+-rwxr-xr-x   0        0        0     4210 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/examples/blacklist3r.py
+-rwxr-xr-x   0        0        0     8261 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/examples/cli.py
+-rwxr-xr-x   0        0        0     3544 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/examples/symfony_knownkey.py
+-rwxr-xr-x   0        0        0    10597 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/examples/telerik_knownkey.py
+-rw-r--r--   0        0        0     5076 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/helpers.py
+-rw-r--r--   0        0        0        0 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/__init__.py
+-rw-r--r--   0        0        0    10468 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/aspnet_viewstate.py
+-rw-r--r--   0        0        0      914 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/aspnet_vstate.py
+-rw-r--r--   0        0        0     1006 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/django_signedcookies.py
+-rw-r--r--   0        0        0     2867 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/express_signedcookies_cs.py
+-rw-r--r--   0        0        0     2287 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/express_signedcookies_es.py
+-rw-r--r--   0        0        0     1120 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/flask_signedcookies.py
+-rw-r--r--   0        0        0     4087 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/generic_jwt.py
+-rw-r--r--   0        0        0    14618 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/jsf_viewstate.py
+-rw-r--r--   0        0        0     2192 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/laravel_signedcookies.py
+-rw-r--r--   0        0        0     1958 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/peoplesoft_pstoken.py
+-rw-r--r--   0        0        0     3097 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/rails_secretkeybase.py
+-rw-r--r--   0        0        0     2963 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/symfony_signedurl.py
+-rw-r--r--   0        0        0     5002 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/telerik_encryptionkey.py
+-rw-r--r--   0        0        0     3776 2023-08-03 04:31:11.915296 badsecrets-0.4.412/badsecrets/modules/telerik_hashkey.py
+-rw-r--r--   0        0        0   654096 2023-08-03 04:31:11.919296 badsecrets-0.4.412/badsecrets/resources/aspnet_machinekeys.txt
+-rw-r--r--   0        0        0    31178 2023-08-03 04:31:11.919296 badsecrets-0.4.412/badsecrets/resources/django_secret_keys.txt
+-rw-r--r--   0        0        0    40993 2023-08-03 04:31:11.919296 badsecrets-0.4.412/badsecrets/resources/express_session_secrets.txt
+-rw-r--r--   0        0        0  1777603 2023-08-03 04:31:11.935296 badsecrets-0.4.412/badsecrets/resources/flask_secret_keys.txt
+-rw-r--r--   0        0        0       87 2023-08-03 04:31:11.935296 badsecrets-0.4.412/badsecrets/resources/jsf_viewstate_passwords.txt
+-rw-r--r--   0        0        0     1257 2023-08-03 04:31:11.935296 badsecrets-0.4.412/badsecrets/resources/jsf_viewstate_passwords_b64.txt
+-rw-r--r--   0        0        0     7785 2023-08-03 04:31:11.935296 badsecrets-0.4.412/badsecrets/resources/jwt_rsakeys_private.txt
+-rw-r--r--   0        0        0     2122 2023-08-03 04:31:11.935296 badsecrets-0.4.412/badsecrets/resources/jwt_rsakeys_public.txt
+-rw-r--r--   0        0        0   113170 2023-08-03 04:31:11.939296 badsecrets-0.4.412/badsecrets/resources/jwt_secrets.txt
+-rw-r--r--   0        0        0    45086 2023-08-03 04:31:11.939296 badsecrets-0.4.412/badsecrets/resources/laravel_app_keys.txt
+-rw-r--r--   0        0        0       78 2023-08-03 04:31:11.939296 badsecrets-0.4.412/badsecrets/resources/peoplesoft_passwords.txt
+-rw-r--r--   0        0        0     6184 2023-08-03 04:31:11.939296 badsecrets-0.4.412/badsecrets/resources/rails_secret_key_base.txt
+-rw-r--r--   0        0        0     3009 2023-08-03 04:31:11.939296 badsecrets-0.4.412/badsecrets/resources/symfony_appsecret.txt
+-rw-r--r--   0        0        0    18037 2023-08-03 04:31:11.939296 badsecrets-0.4.412/badsecrets/resources/telerik_encryption_keys.txt
+-rw-r--r--   0        0        0    17990 2023-08-03 04:31:11.939296 badsecrets-0.4.412/badsecrets/resources/telerik_hash_keys.txt
+-rw-r--r--   0        0        0    76516 2023-08-03 04:31:11.939296 badsecrets-0.4.412/badsecrets/resources/top_10000_passwords.txt
+-rw-r--r--   0        0        0      957 2023-08-03 04:31:37.295515 badsecrets-0.4.412/pyproject.toml
+-rw-r--r--   0        0        0    33667 1970-01-01 00:00:00.000000 badsecrets-0.4.412/PKG-INFO
```

### Comparing `badsecrets-0.4.402/LICENSE` & `badsecrets-0.4.412/LICENSE`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/README.md` & `badsecrets-0.4.412/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 | Rails_SecretKeyBase   | Checks Ruby on Rails signed or encrypted session cookies (from multiple major releases) for known secret_key_base |
 | Generic_JWT | Checks JWTs for known HMAC secrets or RSA private keys |
 | Jsf_viewstate | Checks Both Mojarra and Myfaces implimentations of Java Server Faces (JSF) for use of known or weak secret keys | 
 | Symfony_SignedURL | Checks symfony "_fragment" urls for known HMAC key. Operates on Full URL, including hash |
 | Express_SignedCookies_ES | Checks express.js express-session middleware for signed cookies and session cookies for known 'session secret' |
 | Express_SignedCookies_CS | Checks express.js cookie-session middleware for signed cookies and session cookies for known secret |
 | Laravel_SignedCookies | Checks 'laravel_session' cookies for known laravel 'APP_KEY' |
+| ASPNET_Vstate      | Checks for a once popular custom compressed Viewstate [code snippet](https://www.graa.nl/articles/2010.html) vulnerable to RCE|
 
 ## Installation
 
 We have a [pypi](https://pypi.org/project/badsecrets/) package, so you can just do `pip install badsecrets` to make use of the library.
 
 ## Simple Usage
 
@@ -261,14 +262,15 @@
 Rails_SecretKeyBase = modules_loaded["rails_secretkeybase"]
 Generic_JWT = modules_loaded["generic_jwt"]
 Jsf_viewstate = modules_loaded["jsf_viewstate"]
 Symfony_SignedURL = modules_loaded["symfony_signedurl"]
 Express_SignedCookies_ES = modules_loaded["express_signedcookies_es"]
 Express_SignedCookies_CS = modules_loaded["express_signedcookies_cs"]
 Laravel_SignedCookies = modules_loaded["laravel_signedcookies"]
+ASPNET_Vstate = modules_loaded["aspnet_vstate"]
 
 x = ASPNET_Viewstate()
 print(f"###{str(x.__class__.__name__)}###")
 r = x.check_secret("AgF5WuyVO11CsYJ1K5rjyuLXqUGCITSOapG1cYNiriYQ6VTKochMpn8ws4eJRvft81nQIA==","EDD8C9AE")
 if r:
     print(r)
 else:
@@ -370,14 +372,23 @@
 print(f"###{str(x.__class__.__name__)}###")
 r = x.check_secret("eyJpdiI6IlhlNTZ2UjZUQWZKVHdIcG9nZFkwcGc9PSIsInZhbHVlIjoiRlUvY2grU1F1b01lSXdveXJ0T3N1WGJqeVVmZlNRQjNVOWxiSzljL1Z3RDhqYUdDbjZxMU9oSThWRzExT0YvUmthVzVKRE9kL0RvTEw1cFRhQkphOGw4S2loV1ZrMkkwTHd4am9sZkJQd2VCZ3R0VlFSeFo3ay9wTlBMb3lLSG8iLCJtYWMiOiJkMmU3M2ExNDc2NTc5YjAwMGMwMTdkYTQ1NThkMjRkNTY2YTE4OTg2MzY5MzE5NGZmOTM4YWVjOGZmMWU4NTk2IiwidGFnIjoiIn0%3D")
 if r:
     print(r)
 else:
     print("KEY NOT FOUND :(")
 
+
+x = ASPNET_Vstate()
+print(f"###{str(x.__class__.__name__)}###")
+r = x.check_secret("H4sIAAAAAAAEAPvPyJ/Cz8ppZGpgaWpgZmmYAgAAmCJNEQAAAA==")
+if r:
+    print(r)
+else:
+    print("KEY NOT FOUND :(")
+
 ```
 
 #### Carve
 An additional layer of abstraction above check_secret, which accepts a python requests.response object or a string
 
 ```python
 import requests
```

### Comparing `badsecrets-0.4.402/badsecrets/__init__.py` & `badsecrets-0.4.412/badsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/base.py` & `badsecrets-0.4.412/badsecrets/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import re
 import os
+import gzip
+import base64
 import hashlib
+import binascii
 import requests
 import badsecrets.errors
 from abc import abstractmethod
 
 generic_base64_regex = re.compile(
     r"^(?:[A-Za-z0-9+\/]{4}){8,}(?:[A-Za-z0-9+\/]{4}|[A-Za-z0-9+\/]{3}=|[A-Za-z0-9+\/]{2}={2})$"
 )
@@ -36,14 +39,22 @@
                     f"Custom resource [{self.custom_resource}] does not exist"
                 )
 
     @abstractmethod
     def check_secret(self, secret):
         raise NotImplementedError
 
+    @staticmethod
+    def attempt_decompress(value):
+        try:
+            uncompressed = gzip.decompress(base64.b64decode(value))
+        except (gzip.BadGzipFile, binascii.Error, ValueError):
+            return False
+        return uncompressed
+
     @classmethod
     def get_description(self):
         return self.description
 
     def get_product_from_carve(self, regex_search):
         return regex_search.groups()[0]
```

### Comparing `badsecrets-0.4.402/badsecrets/examples/blacklist3r.py` & `badsecrets-0.4.412/badsecrets/examples/blacklist3r.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/examples/cli.py` & `badsecrets-0.4.412/badsecrets/examples/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,15 +56,22 @@
         print(f"Location: {self.x['location']}")
 
 
 class ReportSecret(BaseReport):
     def report(self):
         self.print_report(print_status("Known Secret Found!\n", color=Fore.GREEN, passthru=True))
         print_status(f"Secret: {self.x['secret']}", color=Fore.GREEN)
-        print(f"Severity: {self.x['description']['severity']}")
+        severity = self.x["description"]["severity"]
+        if severity in ["CRITICAL", "HIGH"]:
+            severity_color = Fore.RED
+        elif severity in ["LOW", "MEDIUM"]:
+            severity_color = Fore.YELLOW
+        elif severity == "INFO":
+            severity_color = Fore.BLUE
+        print_status(f"Severity: {self.x['description']['severity']}", color=severity_color)
         print(f"Details: {self.x['details']}")
 
 
 class ReportIdentify(BaseReport):
     def report(self):
         self.print_report(
             print_status("Cryptographic Product Identified (no vulnerability)\n", color=Fore.YELLOW, passthru=True)
```

### Comparing `badsecrets-0.4.402/badsecrets/examples/symfony_knownkey.py` & `badsecrets-0.4.412/badsecrets/examples/symfony_knownkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/examples/telerik_knownkey.py` & `badsecrets-0.4.412/badsecrets/examples/telerik_knownkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/helpers.py` & `badsecrets-0.4.412/badsecrets/helpers.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/modules/aspnet_viewstate.py` & `badsecrets-0.4.412/badsecrets/modules/aspnet_viewstate.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/modules/django_signedcookies.py` & `badsecrets-0.4.412/badsecrets/modules/django_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/modules/express_signedcookies_cs.py` & `badsecrets-0.4.412/badsecrets/modules/express_signedcookies_cs.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/modules/express_signedcookies_es.py` & `badsecrets-0.4.412/badsecrets/modules/express_signedcookies_es.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/modules/flask_signedcookies.py` & `badsecrets-0.4.412/badsecrets/modules/flask_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/modules/generic_jwt.py` & `badsecrets-0.4.412/badsecrets/modules/generic_jwt.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/modules/jsf_viewstate.py` & `badsecrets-0.4.412/badsecrets/modules/jsf_viewstate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re
-import gzip
 import hmac
 import base64
 import hashlib
 import binascii
 import urllib.parse
 from Crypto.Cipher import DES3, AES, DES
 from Crypto.Util.Padding import unpad
@@ -21,22 +20,14 @@
         "product": "Java Server Faces Viewstate",
         "secret": "com.sun.faces.ClientStateSavingPassword",
         "severity": "CRITICAL",
     }
 
     hashcat_hashalg_table = {"MD5": "50", "SHA1": "150", "SHA256": "1450", "SHA384": "10800", "SHA512": "1750"}
 
-    @staticmethod
-    def attempt_decompress(value):
-        try:
-            uncompressed = gzip.decompress(base64.b64decode(value))
-        except (gzip.BadGzipFile, binascii.Error, ValueError):
-            return False
-        return uncompressed
-
     def carve_regex(self):
         return re.compile(r"<input.+?name=\"javax\.faces\.ViewState\".+?value=\"([^\"]*)\"")
 
     # Mojarra 1.2.x - 2.0.3
     def DES3_decrypt(self, ct, password):
         x = Java_sha1prng(password)
         derivedKey = x.get_sha1prng_key(24)
```

### Comparing `badsecrets-0.4.402/badsecrets/modules/laravel_signedcookies.py` & `badsecrets-0.4.412/badsecrets/modules/laravel_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/modules/peoplesoft_pstoken.py` & `badsecrets-0.4.412/badsecrets/modules/peoplesoft_pstoken.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/modules/rails_secretkeybase.py` & `badsecrets-0.4.412/badsecrets/modules/rails_secretkeybase.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/modules/symfony_signedurl.py` & `badsecrets-0.4.412/badsecrets/modules/symfony_signedurl.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/modules/telerik_encryptionkey.py` & `badsecrets-0.4.412/badsecrets/modules/telerik_encryptionkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/modules/telerik_hashkey.py` & `badsecrets-0.4.412/badsecrets/modules/telerik_hashkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/resources/aspnet_machinekeys.txt` & `badsecrets-0.4.412/badsecrets/resources/aspnet_machinekeys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/resources/django_secret_keys.txt` & `badsecrets-0.4.412/badsecrets/resources/django_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/resources/express_session_secrets.txt` & `badsecrets-0.4.412/badsecrets/resources/express_session_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/resources/flask_secret_keys.txt` & `badsecrets-0.4.412/badsecrets/resources/flask_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/resources/jsf_viewstate_passwords_b64.txt` & `badsecrets-0.4.412/badsecrets/resources/jsf_viewstate_passwords_b64.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/resources/jwt_rsakeys_private.txt` & `badsecrets-0.4.412/badsecrets/resources/jwt_rsakeys_private.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/resources/jwt_rsakeys_public.txt` & `badsecrets-0.4.412/badsecrets/resources/jwt_rsakeys_public.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/resources/jwt_secrets.txt` & `badsecrets-0.4.412/badsecrets/resources/jwt_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/resources/laravel_app_keys.txt` & `badsecrets-0.4.412/badsecrets/resources/laravel_app_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/resources/rails_secret_key_base.txt` & `badsecrets-0.4.412/badsecrets/resources/rails_secret_key_base.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/resources/symfony_appsecret.txt` & `badsecrets-0.4.412/badsecrets/resources/symfony_appsecret.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/resources/telerik_encryption_keys.txt` & `badsecrets-0.4.412/badsecrets/resources/telerik_encryption_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/resources/telerik_hash_keys.txt` & `badsecrets-0.4.412/badsecrets/resources/telerik_hash_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/badsecrets/resources/top_10000_passwords.txt` & `badsecrets-0.4.412/badsecrets/resources/top_10000_passwords.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.402/pyproject.toml` & `badsecrets-0.4.412/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "badsecrets"
-version = "v0.4.402"
+version = "v0.4.412"
 description = "About"
 authors = ["A library for detecting known or weak secrets on across many platforms"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dev-dependencies]
 requests-mock = "^1.10.0"
```

### Comparing `badsecrets-0.4.402/PKG-INFO` & `badsecrets-0.4.412/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badsecrets
-Version: 0.4.402
+Version: 0.4.412
 Summary: About
 License: GPL-3.0
 Author: A library for detecting known or weak secrets on across many platforms
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -52,14 +52,15 @@
 | Rails_SecretKeyBase   | Checks Ruby on Rails signed or encrypted session cookies (from multiple major releases) for known secret_key_base |
 | Generic_JWT | Checks JWTs for known HMAC secrets or RSA private keys |
 | Jsf_viewstate | Checks Both Mojarra and Myfaces implimentations of Java Server Faces (JSF) for use of known or weak secret keys | 
 | Symfony_SignedURL | Checks symfony "_fragment" urls for known HMAC key. Operates on Full URL, including hash |
 | Express_SignedCookies_ES | Checks express.js express-session middleware for signed cookies and session cookies for known 'session secret' |
 | Express_SignedCookies_CS | Checks express.js cookie-session middleware for signed cookies and session cookies for known secret |
 | Laravel_SignedCookies | Checks 'laravel_session' cookies for known laravel 'APP_KEY' |
+| ASPNET_Vstate      | Checks for a once popular custom compressed Viewstate [code snippet](https://www.graa.nl/articles/2010.html) vulnerable to RCE|
 
 ## Installation
 
 We have a [pypi](https://pypi.org/project/badsecrets/) package, so you can just do `pip install badsecrets` to make use of the library.
 
 ## Simple Usage
 
@@ -283,14 +284,15 @@
 Rails_SecretKeyBase = modules_loaded["rails_secretkeybase"]
 Generic_JWT = modules_loaded["generic_jwt"]
 Jsf_viewstate = modules_loaded["jsf_viewstate"]
 Symfony_SignedURL = modules_loaded["symfony_signedurl"]
 Express_SignedCookies_ES = modules_loaded["express_signedcookies_es"]
 Express_SignedCookies_CS = modules_loaded["express_signedcookies_cs"]
 Laravel_SignedCookies = modules_loaded["laravel_signedcookies"]
+ASPNET_Vstate = modules_loaded["aspnet_vstate"]
 
 x = ASPNET_Viewstate()
 print(f"###{str(x.__class__.__name__)}###")
 r = x.check_secret("AgF5WuyVO11CsYJ1K5rjyuLXqUGCITSOapG1cYNiriYQ6VTKochMpn8ws4eJRvft81nQIA==","EDD8C9AE")
 if r:
     print(r)
 else:
@@ -392,14 +394,23 @@
 print(f"###{str(x.__class__.__name__)}###")
 r = x.check_secret("eyJpdiI6IlhlNTZ2UjZUQWZKVHdIcG9nZFkwcGc9PSIsInZhbHVlIjoiRlUvY2grU1F1b01lSXdveXJ0T3N1WGJqeVVmZlNRQjNVOWxiSzljL1Z3RDhqYUdDbjZxMU9oSThWRzExT0YvUmthVzVKRE9kL0RvTEw1cFRhQkphOGw4S2loV1ZrMkkwTHd4am9sZkJQd2VCZ3R0VlFSeFo3ay9wTlBMb3lLSG8iLCJtYWMiOiJkMmU3M2ExNDc2NTc5YjAwMGMwMTdkYTQ1NThkMjRkNTY2YTE4OTg2MzY5MzE5NGZmOTM4YWVjOGZmMWU4NTk2IiwidGFnIjoiIn0%3D")
 if r:
     print(r)
 else:
     print("KEY NOT FOUND :(")
 
+
+x = ASPNET_Vstate()
+print(f"###{str(x.__class__.__name__)}###")
+r = x.check_secret("H4sIAAAAAAAEAPvPyJ/Cz8ppZGpgaWpgZmmYAgAAmCJNEQAAAA==")
+if r:
+    print(r)
+else:
+    print("KEY NOT FOUND :(")
+
 ```
 
 #### Carve
 An additional layer of abstraction above check_secret, which accepts a python requests.response object or a string
 
 ```python
 import requests
```

