# Comparing `tmp/sectxt-0.8.3.tar.gz` & `tmp/sectxt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sectxt-0.8.3.tar", last modified: Mon Apr 17 09:00:15 2023, max compression
+gzip compressed data, was "sectxt-0.9.0.tar", last modified: Thu Aug  3 08:37:49 2023, max compression
```

## Comparing `sectxt-0.8.3.tar` & `sectxt-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 09:00:15.918703 sectxt-0.8.3/
--rw-rw-rw-   0        0        0    13827 2023-04-17 08:37:08.000000 sectxt-0.8.3/LICENCE
--rw-rw-rw-   0        0        0    10776 2023-04-17 09:00:15.920744 sectxt-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     9725 2023-04-17 08:37:08.000000 sectxt-0.8.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 09:00:15.885722 sectxt-0.8.3/sectxt/
--rw-rw-rw-   0        0        0    17133 2023-04-17 08:37:08.000000 sectxt-0.8.3/sectxt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:00:15.915734 sectxt-0.8.3/sectxt.egg-info/
--rw-rw-rw-   0        0        0    10776 2023-04-17 09:00:15.000000 sectxt-0.8.3/sectxt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-17 09:00:15.000000 sectxt-0.8.3/sectxt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 09:00:15.000000 sectxt-0.8.3/sectxt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-17 09:00:15.000000 sectxt-0.8.3/sectxt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 09:00:15.000000 sectxt-0.8.3/sectxt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 09:00:15.000000 sectxt-0.8.3/sectxt.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1021 2023-04-17 09:00:15.928702 sectxt-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0       60 2023-04-17 08:37:08.000000 sectxt-0.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:00:15.916700 sectxt-0.8.3/test/
--rw-rw-rw-   0        0        0     8679 2023-04-17 08:37:08.000000 sectxt-0.8.3/test/test_sectxt.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:37:49.318207 sectxt-0.9.0/
+-rw-rw-rw-   0        0        0    13827 2023-08-03 08:06:16.000000 sectxt-0.9.0/LICENCE
+-rw-rw-rw-   0        0        0    11858 2023-08-03 08:37:49.318207 sectxt-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10800 2023-08-03 08:06:16.000000 sectxt-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 08:37:49.298205 sectxt-0.9.0/sectxt/
+-rw-rw-rw-   0        0        0    18567 2023-08-03 08:06:16.000000 sectxt-0.9.0/sectxt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:37:49.314206 sectxt-0.9.0/sectxt.egg-info/
+-rw-rw-rw-   0        0        0    11858 2023-08-03 08:37:48.000000 sectxt-0.9.0/sectxt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-08-03 08:37:48.000000 sectxt-0.9.0/sectxt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 08:37:48.000000 sectxt-0.9.0/sectxt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-03 08:37:48.000000 sectxt-0.9.0/sectxt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-03 08:37:48.000000 sectxt-0.9.0/sectxt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-08-03 08:35:17.000000 sectxt-0.9.0/sectxt.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1028 2023-08-03 08:37:49.319207 sectxt-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0       60 2023-08-03 08:06:16.000000 sectxt-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:37:49.316209 sectxt-0.9.0/test/
+-rw-rw-rw-   0        0        0    11280 2023-08-03 08:06:16.000000 sectxt-0.9.0/test/test_sectxt.py
```

### Comparing `sectxt-0.8.3/LICENCE` & `sectxt-0.9.0/LICENCE`

 * *Files identical despite different names*

### Comparing `sectxt-0.8.3/PKG-INFO` & `sectxt-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sectxt
-Version: 0.8.3
+Version: 0.9.0
 Summary: security.txt parser and validator
 Author: DigitalTrustCenter
 Author-email: algemeen@digitaltrustcenter.nl
 License: EUPL-1.2
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-# SecTXT: Security.txt parser and validator
+# SecTXT: security.txt parser and validator
 
 This package contains a security.txt ([RFC 9116](https://www.rfc-editor.org/info/rfc9116)) parser and validator.
 
 When security risks in web services are discovered by independent security researchers who understand the severity of the risk, they often lack the channels to disclose them properly. As a result, security issues may be left unreported. security.txt defines a standard to help organizations define the process for security researchers to disclose security vulnerabilities securely.
 
 ## Installation
 
@@ -50,15 +50,15 @@
 ## Validation
 
 ```python
 
 >>> from sectxt import SecurityTXT
 >>> s = SecurityTXT("www.example.com")
 >>> s.errors
-[{'code': 'no_uri', 'message': 'The field value must be an URI', 'line': 2}, {'code': 'no_expire', 'message': 'The Expires field is missing', 'line': None}]
+[{'code': 'no_uri', 'message': 'Field policy value must be an URI', 'line': 2}, {'code': 'no_expire', 'message': 'The Expires field is missing', 'line': None}]
 >>> s.recommendations
 [{'code': 'long_expiry', 'message': 'Expiry date is more than one year in the future', 'line': 3}]
 ```
 
 The "errors", "recommendations" and "notifications" attribute return a list of entries. An entry is
 a dict with three keys:
 
@@ -84,25 +84,27 @@
 | "multi_expire"        | "'Expires' field must not appear more than once."                                                                                                                      |
 | "invalid_expiry"      | "Date and time in 'Expires' field must be formatted according to ISO 8601."                                                                                            | 
 | "expired"             | "Date and time in 'Expires' field must not be in the past."                                                                                                            |
 | "no_contact"          | "'Contact' field must appear at least once."                                                                                                                           |
 | "no_canonical_match"  | "Web URI where security.txt is located must match with a 'Canonical' field. In case of redirecting either the first or last web URI of the redirect chain must match." |
 | "multi_lang"          | "'Preferred-Languages' field must not appear more than once."                                                                                                          |
 | "invalid_lang"        | "Value in 'Preferred-Languages' field must match one or more language tags as defined in RFC5646, separated by commas."                                                |
-| "no_uri"              | "Field value must be a URI (e.g. beginning with 'mailto:')."                                                                                                           |
+| "no_uri"              | "Field '{field}' value must be a URI."                                                                                                                                 |
 | "no_https"            | "Web URI must begin with 'https://'."                                                                                                                                  |
 | "prec_ws"             | "There must be no whitespace before the field separator (colon)."                                                                                                      |
 | "no_space"            | "Field separator (colon) must be followed by a space."                                                                                                                 | 
 | "empty_key"           | "Field name must not be empty."                                                                                                                                        |
 | "empty_value"         | "Field value must not be empty."                                                                                                                                       |
 | "invalid_line"        | "Line must contain a field name and value, unless the line is blank or contains a comment."                                                                            |
-| "no_line_separators"  | "Every line must end with either a carriage return and line feed characters or just a line feed character"                                                             |
+| "no_line_separators"  | "Every line, including the last one, must end with either a carriage return and line feed characters or just a line feed character"                                    |
 | "signed_format_issue" | "Signed security.txt must start with the header '-----BEGIN PGP SIGNED MESSAGE-----'. "                                                                                |
 | "data_after_sig"      | "Signed security.txt must not contain data after the signature."                                                                                                       |
 | "no_csaf_file"        | "All CSAF fields must point to a provider-metadata.json file."                                                                                                         |
+| "pgp_data_error"      | "Signed message did not contain a correct ASCII-armored PGP block."                                                                                                    |
+| "pgp_error"           | "Decoding or parsing of the pgp message failed."                                                                                                                       |
 
 
 ### Possible recommendations
 
 | code                       | message                                                                                        |
 |----------------------------|------------------------------------------------------------------------------------------------|
 | "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."                 |
@@ -111,17 +113,22 @@
 | "no_canonical"             | "'Canonical' field should be present in a signed file."                                        |
 | "multiple_csaf_fields"     | "It is allowed to have more than one CSAF field, however this should be removed if possible."  |
 
 ### Possible notifications
 
 | code                          | message                                                                                                                                                                     |
 |-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| "unknown_field"<sup>[2]</sup> | "Security.txt contains an unknown field. Field {unknown_field} is either a custom field which may not be widely supported, or there is a typo in a standardised field name. |
+| "unknown_field"<sup>[2]</sup> | "security.txt contains an unknown field. Field {unknown_field} is either a custom field which may not be widely supported, or there is a typo in a standardised field name. |
 
 
+### Security.txt scraping information
+
+The scraper attempts to find the security.txt of the given domain in the correct location `/.well-known/security.txt`. It also looks in the old location and with unsecure `http` scheme which would result in validation errors. To prevent possible errors getting the file from the domain a user-agent is added to the header of the request. The user agent that is added is `Mozilla/5.0 (Windows NT 6.1; WOW64; rv:12.0) Gecko/20100101 Firefox/12.0`, which would mock a browser in firefox with a Windows 7 OS.
+If a security.txt file is found that file is than parsed. Any errors, recommendations or notifications that are found would be returned.
+
 ---
 
 [1] The security.txt parser will check for the addition of the digital signature, but it will not verify the validity of the signature.
 
 [2] Regarding code "unknown_field": According to RFC 9116 section 2.4, any fields that are not explicitly supported must be ignored. This parser does add a notification for unknown fields by default. This behaviour can be turned off using the parameter recommend_unknown_fields:
 ```python
```

### Comparing `sectxt-0.8.3/README.md` & `sectxt-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SecTXT: Security.txt parser and validator
+# SecTXT: security.txt parser and validator
 
 This package contains a security.txt ([RFC 9116](https://www.rfc-editor.org/info/rfc9116)) parser and validator.
 
 When security risks in web services are discovered by independent security researchers who understand the severity of the risk, they often lack the channels to disclose them properly. As a result, security issues may be left unreported. security.txt defines a standard to help organizations define the process for security researchers to disclose security vulnerabilities securely.
 
 ## Installation
 
@@ -26,15 +26,15 @@
 ## Validation
 
 ```python
 
 >>> from sectxt import SecurityTXT
 >>> s = SecurityTXT("www.example.com")
 >>> s.errors
-[{'code': 'no_uri', 'message': 'The field value must be an URI', 'line': 2}, {'code': 'no_expire', 'message': 'The Expires field is missing', 'line': None}]
+[{'code': 'no_uri', 'message': 'Field policy value must be an URI', 'line': 2}, {'code': 'no_expire', 'message': 'The Expires field is missing', 'line': None}]
 >>> s.recommendations
 [{'code': 'long_expiry', 'message': 'Expiry date is more than one year in the future', 'line': 3}]
 ```
 
 The "errors", "recommendations" and "notifications" attribute return a list of entries. An entry is
 a dict with three keys:
 
@@ -60,25 +60,27 @@
 | "multi_expire"        | "'Expires' field must not appear more than once."                                                                                                                      |
 | "invalid_expiry"      | "Date and time in 'Expires' field must be formatted according to ISO 8601."                                                                                            | 
 | "expired"             | "Date and time in 'Expires' field must not be in the past."                                                                                                            |
 | "no_contact"          | "'Contact' field must appear at least once."                                                                                                                           |
 | "no_canonical_match"  | "Web URI where security.txt is located must match with a 'Canonical' field. In case of redirecting either the first or last web URI of the redirect chain must match." |
 | "multi_lang"          | "'Preferred-Languages' field must not appear more than once."                                                                                                          |
 | "invalid_lang"        | "Value in 'Preferred-Languages' field must match one or more language tags as defined in RFC5646, separated by commas."                                                |
-| "no_uri"              | "Field value must be a URI (e.g. beginning with 'mailto:')."                                                                                                           |
+| "no_uri"              | "Field '{field}' value must be a URI."                                                                                                                                 |
 | "no_https"            | "Web URI must begin with 'https://'."                                                                                                                                  |
 | "prec_ws"             | "There must be no whitespace before the field separator (colon)."                                                                                                      |
 | "no_space"            | "Field separator (colon) must be followed by a space."                                                                                                                 | 
 | "empty_key"           | "Field name must not be empty."                                                                                                                                        |
 | "empty_value"         | "Field value must not be empty."                                                                                                                                       |
 | "invalid_line"        | "Line must contain a field name and value, unless the line is blank or contains a comment."                                                                            |
-| "no_line_separators"  | "Every line must end with either a carriage return and line feed characters or just a line feed character"                                                             |
+| "no_line_separators"  | "Every line, including the last one, must end with either a carriage return and line feed characters or just a line feed character"                                    |
 | "signed_format_issue" | "Signed security.txt must start with the header '-----BEGIN PGP SIGNED MESSAGE-----'. "                                                                                |
 | "data_after_sig"      | "Signed security.txt must not contain data after the signature."                                                                                                       |
 | "no_csaf_file"        | "All CSAF fields must point to a provider-metadata.json file."                                                                                                         |
+| "pgp_data_error"      | "Signed message did not contain a correct ASCII-armored PGP block."                                                                                                    |
+| "pgp_error"           | "Decoding or parsing of the pgp message failed."                                                                                                                       |
 
 
 ### Possible recommendations
 
 | code                       | message                                                                                        |
 |----------------------------|------------------------------------------------------------------------------------------------|
 | "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."                 |
@@ -87,17 +89,22 @@
 | "no_canonical"             | "'Canonical' field should be present in a signed file."                                        |
 | "multiple_csaf_fields"     | "It is allowed to have more than one CSAF field, however this should be removed if possible."  |
 
 ### Possible notifications
 
 | code                          | message                                                                                                                                                                     |
 |-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| "unknown_field"<sup>[2]</sup> | "Security.txt contains an unknown field. Field {unknown_field} is either a custom field which may not be widely supported, or there is a typo in a standardised field name. |
+| "unknown_field"<sup>[2]</sup> | "security.txt contains an unknown field. Field {unknown_field} is either a custom field which may not be widely supported, or there is a typo in a standardised field name. |
 
 
+### Security.txt scraping information
+
+The scraper attempts to find the security.txt of the given domain in the correct location `/.well-known/security.txt`. It also looks in the old location and with unsecure `http` scheme which would result in validation errors. To prevent possible errors getting the file from the domain a user-agent is added to the header of the request. The user agent that is added is `Mozilla/5.0 (Windows NT 6.1; WOW64; rv:12.0) Gecko/20100101 Firefox/12.0`, which would mock a browser in firefox with a Windows 7 OS.
+If a security.txt file is found that file is than parsed. Any errors, recommendations or notifications that are found would be returned.
+
 ---
 
 [1] The security.txt parser will check for the addition of the digital signature, but it will not verify the validity of the signature.
 
 [2] Regarding code "unknown_field": According to RFC 9116 section 2.4, any fields that are not explicitly supported must be ignored. This parser does add a notification for unknown fields by default. This behaviour can be turned off using the parameter recommend_unknown_fields:
 ```python
```

### Comparing `sectxt-0.8.3/sectxt/__init__.py` & `sectxt-0.9.0/sectxt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 #
 # SPDX-License-Identifier: EUPL-1.2
 #
+import codecs
+
 import langcodes
 import re
 import sys
 from cgi import parse_header
 from collections import defaultdict
 from datetime import datetime, timezone
 from typing import Optional, Union, List, DefaultDict
 from urllib.parse import urlsplit, urlunsplit
+import pgpy
+from pgpy.errors import PGPError
 
 if sys.version_info < (3, 8):
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
 import dateutil.parser
 import requests
 
-__version__ = "0.8.3"
+__version__ = "0.9.0"
 
 s = requests.Session()
 
 
 class ErrorDict(TypedDict):
     code: str
     message: str
@@ -92,15 +96,18 @@
         self._line_no = None
         self.validate_contents()
 
     def _add_error(
         self,
         code: str,
         message: str,
+        explicit_line_no=None
     ) -> None:
+        if explicit_line_no:
+            self._line_no = explicit_line_no
         err_dict: ErrorDict = {"code": code, "message": message, "line": self._line_no}
         self._errors.append(err_dict)
 
     def _add_recommendation(
         self,
         code: str,
         message: str,
@@ -140,14 +147,29 @@
             if self._line_no != 1:
                 self._add_error(
                     "signed_format_issue",
                     "Signed security.txt must start with the header "
                     "'-----BEGIN PGP SIGNED MESSAGE-----'.",
                 )
             self._signed = True
+
+            # Check pgp formatting if signed
+            try:
+                pgpy.PGPMessage.from_blob(self._content)
+            except ValueError:
+                self._add_error(
+                    "pgp_data_error",
+                    "Signed message did not contain a correct ASCII-armored PGP block."
+                )
+            except PGPError as e:
+                self._add_error(
+                    "pgp_error",
+                    "Decoding or parsing of the pgp message failed."
+                )
+
             return {"type": "pgp_envelope", "field_name": None, "value": line}
 
         if line == "-----BEGIN PGP SIGNATURE-----" and self._signed:
             self._reading_sig = True
             return {"type": "pgp_envelope", "field_name": None, "value": line}
 
         if line.startswith("#"):
@@ -195,15 +217,15 @@
             return {"type": "error", "value": line, "field_name": None}
 
         if key in self.uri_fields:
             url_parts = urlsplit(value)
             if url_parts.scheme == "":
                 self._add_error(
                     "no_uri",
-                    "Field value must be a URI (e.g. beginning with 'mailto:').",
+                    f"Field '{key}' value must be a URI.",
                 )
             elif url_parts.scheme == "http":
                 self._add_error("no_https", "Web URI must begin with 'https://'.")
         elif key == "expires":
             self._parse_expires(value)
         elif key == PREFERRED_LANGUAGES:
             self._langs = [v.strip() for v in value.split(",")]
@@ -217,15 +239,15 @@
                         "or more language tags as defined in RFC5646, "
                         "separated by commas.",
                     )
 
         if self.recommend_unknown_fields and key not in self.known_fields:
             self._add_notification(
                 "unknown_field",
-                "Security.txt contains an unknown field. "
+                "security.txt contains an unknown field. "
                 'Field "%s" is either a custom field which may not be widely '
                 "supported, or there is a typo in a standardised field name." % key,
             )
 
         self._values[key].append(value)
         return {"type": "field", "field_name": key, "value": value}
 
@@ -280,17 +302,18 @@
                     "Web URI where security.txt is located must match with a "
                     "'Canonical' field. In case of redirecting either the "
                     "first or last web URI of the redirect chain must match.",
                 )
         if self.lines[-1]["type"] != "empty":
             self._add_error(
                 "no_line_separators",
-                "Every line must end with either a carriage "
-                "return and line feed characters or just a line "
-                "feed character",
+                "Every line, including the last one, must end with "
+                "either a carriage return and line feed characters "
+                "or just a line feed character",
+                len(self.lines)
             )
 
         if "csaf" in self._values:
             if not all(
                 v.endswith("provider-metadata.json") for v in self._values["csaf"]
             ):
                 self._add_error(
@@ -389,34 +412,49 @@
         self._netloc = netloc
         self._path: Optional[str] = None
         self._url: Optional[str] = None
         super().__init__("", recommend_unknown_fields=recommend_unknown_fields)
 
     def _get_str(self, content: bytes) -> str:
         try:
-            return content.decode()
+            if content.startswith(codecs.BOM_UTF8):
+                content = content.replace(codecs.BOM_UTF8, b'')
+            return content.decode('utf-8')
         except UnicodeError:
             self._add_error("utf8", "Content must be utf-8 encoded.")
-        return content.decode(errors="replace")
+        return content.decode('utf-8', errors="replace")
 
     def _process(self) -> None:
         security_txt_found = False
         for scheme in ["https", "http"]:
             for path in [".well-known/security.txt", "security.txt"]:
                 url = urlunsplit((scheme, self._netloc, path, None, None))
                 try:
-                    resp = requests.get(url, timeout=5)
+                    resp = requests.get(
+                        url,
+                        headers={
+                            'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; WOW64; rv:12.0) '
+                                          'Gecko/20100101 Firefox/12.0'},
+                        timeout=5
+                    )
                 except requests.exceptions.SSLError:
                     if not any(d["code"] == "invalid_cert" for d in self._errors):
                         self._add_error(
                             "invalid_cert",
                             "security.txt must be served with a valid TLS certificate.",
                         )
                     try:
-                        resp = requests.get(url, timeout=5, verify=False)
+                        resp = requests.get(
+                            url,
+                            headers={
+                                'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; WOW64; rv:12.0) '
+                                              'Gecko/20100101 Firefox/12.0'},
+                            timeout=5,
+                            verify=False
+                        )
                     except:
                         continue
                 except:
                     continue
                 if resp.status_code == 200:
                     self._path = path
                     self._url = url
```

### Comparing `sectxt-0.8.3/sectxt.egg-info/PKG-INFO` & `sectxt-0.9.0/sectxt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sectxt
-Version: 0.8.3
+Version: 0.9.0
 Summary: security.txt parser and validator
 Author: DigitalTrustCenter
 Author-email: algemeen@digitaltrustcenter.nl
 License: EUPL-1.2
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-# SecTXT: Security.txt parser and validator
+# SecTXT: security.txt parser and validator
 
 This package contains a security.txt ([RFC 9116](https://www.rfc-editor.org/info/rfc9116)) parser and validator.
 
 When security risks in web services are discovered by independent security researchers who understand the severity of the risk, they often lack the channels to disclose them properly. As a result, security issues may be left unreported. security.txt defines a standard to help organizations define the process for security researchers to disclose security vulnerabilities securely.
 
 ## Installation
 
@@ -50,15 +50,15 @@
 ## Validation
 
 ```python
 
 >>> from sectxt import SecurityTXT
 >>> s = SecurityTXT("www.example.com")
 >>> s.errors
-[{'code': 'no_uri', 'message': 'The field value must be an URI', 'line': 2}, {'code': 'no_expire', 'message': 'The Expires field is missing', 'line': None}]
+[{'code': 'no_uri', 'message': 'Field policy value must be an URI', 'line': 2}, {'code': 'no_expire', 'message': 'The Expires field is missing', 'line': None}]
 >>> s.recommendations
 [{'code': 'long_expiry', 'message': 'Expiry date is more than one year in the future', 'line': 3}]
 ```
 
 The "errors", "recommendations" and "notifications" attribute return a list of entries. An entry is
 a dict with three keys:
 
@@ -84,25 +84,27 @@
 | "multi_expire"        | "'Expires' field must not appear more than once."                                                                                                                      |
 | "invalid_expiry"      | "Date and time in 'Expires' field must be formatted according to ISO 8601."                                                                                            | 
 | "expired"             | "Date and time in 'Expires' field must not be in the past."                                                                                                            |
 | "no_contact"          | "'Contact' field must appear at least once."                                                                                                                           |
 | "no_canonical_match"  | "Web URI where security.txt is located must match with a 'Canonical' field. In case of redirecting either the first or last web URI of the redirect chain must match." |
 | "multi_lang"          | "'Preferred-Languages' field must not appear more than once."                                                                                                          |
 | "invalid_lang"        | "Value in 'Preferred-Languages' field must match one or more language tags as defined in RFC5646, separated by commas."                                                |
-| "no_uri"              | "Field value must be a URI (e.g. beginning with 'mailto:')."                                                                                                           |
+| "no_uri"              | "Field '{field}' value must be a URI."                                                                                                                                 |
 | "no_https"            | "Web URI must begin with 'https://'."                                                                                                                                  |
 | "prec_ws"             | "There must be no whitespace before the field separator (colon)."                                                                                                      |
 | "no_space"            | "Field separator (colon) must be followed by a space."                                                                                                                 | 
 | "empty_key"           | "Field name must not be empty."                                                                                                                                        |
 | "empty_value"         | "Field value must not be empty."                                                                                                                                       |
 | "invalid_line"        | "Line must contain a field name and value, unless the line is blank or contains a comment."                                                                            |
-| "no_line_separators"  | "Every line must end with either a carriage return and line feed characters or just a line feed character"                                                             |
+| "no_line_separators"  | "Every line, including the last one, must end with either a carriage return and line feed characters or just a line feed character"                                    |
 | "signed_format_issue" | "Signed security.txt must start with the header '-----BEGIN PGP SIGNED MESSAGE-----'. "                                                                                |
 | "data_after_sig"      | "Signed security.txt must not contain data after the signature."                                                                                                       |
 | "no_csaf_file"        | "All CSAF fields must point to a provider-metadata.json file."                                                                                                         |
+| "pgp_data_error"      | "Signed message did not contain a correct ASCII-armored PGP block."                                                                                                    |
+| "pgp_error"           | "Decoding or parsing of the pgp message failed."                                                                                                                       |
 
 
 ### Possible recommendations
 
 | code                       | message                                                                                        |
 |----------------------------|------------------------------------------------------------------------------------------------|
 | "long_expiry"              | "Date and time in 'Expires' field should be less than a year into the future."                 |
@@ -111,17 +113,22 @@
 | "no_canonical"             | "'Canonical' field should be present in a signed file."                                        |
 | "multiple_csaf_fields"     | "It is allowed to have more than one CSAF field, however this should be removed if possible."  |
 
 ### Possible notifications
 
 | code                          | message                                                                                                                                                                     |
 |-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| "unknown_field"<sup>[2]</sup> | "Security.txt contains an unknown field. Field {unknown_field} is either a custom field which may not be widely supported, or there is a typo in a standardised field name. |
+| "unknown_field"<sup>[2]</sup> | "security.txt contains an unknown field. Field {unknown_field} is either a custom field which may not be widely supported, or there is a typo in a standardised field name. |
 
 
+### Security.txt scraping information
+
+The scraper attempts to find the security.txt of the given domain in the correct location `/.well-known/security.txt`. It also looks in the old location and with unsecure `http` scheme which would result in validation errors. To prevent possible errors getting the file from the domain a user-agent is added to the header of the request. The user agent that is added is `Mozilla/5.0 (Windows NT 6.1; WOW64; rv:12.0) Gecko/20100101 Firefox/12.0`, which would mock a browser in firefox with a Windows 7 OS.
+If a security.txt file is found that file is than parsed. Any errors, recommendations or notifications that are found would be returned.
+
 ---
 
 [1] The security.txt parser will check for the addition of the digital signature, but it will not verify the validity of the signature.
 
 [2] Regarding code "unknown_field": According to RFC 9116 section 2.4, any fields that are not explicitly supported must be ignored. This parser does add a notification for unknown fields by default. This behaviour can be turned off using the parameter recommend_unknown_fields:
 ```python
```

### Comparing `sectxt-0.8.3/setup.cfg` & `sectxt-0.9.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -55,10 +55,11 @@
 00000360: 7569 7265 7320 3d20 3e3d 332e 370d 0a7a  uires = >=3.7..z
 00000370: 6970 5f73 6166 6520 3d20 5472 7565 0d0a  ip_safe = True..
 00000380: 7061 636b 6167 6573 203d 2073 6563 7478  packages = sectx
 00000390: 740d 0a69 6e73 7461 6c6c 5f72 6571 7569  t..install_requi
 000003a0: 7265 7320 3d20 0d0a 0972 6571 7565 7374  res = ...request
 000003b0: 730d 0a09 7079 7468 6f6e 2d64 6174 6575  s...python-dateu
 000003c0: 7469 6c0d 0a09 6c61 6e67 636f 6465 730d  til...langcodes.
-000003d0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-000003e0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-000003f0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+000003d0: 0a09 5047 5079 0d0a 0d0a 5b65 6767 5f69  ..PGPy....[egg_i
+000003e0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+000003f0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+00000400: 0d0a 0d0a                                ....
```

### Comparing `sectxt-0.8.3/test/test_sectxt.py` & `sectxt-0.9.0/test/test_sectxt.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,15 +29,19 @@
 # CSAF link
 CSAF: https://example.com/.well-known/csaf/provider-metadata.json
 
 Expires: {(date.today() + timedelta(days=10)).isoformat()}T18:37:07z
 -----BEGIN PGP SIGNATURE-----
 Version: GnuPG v2.2
 
-[signature]
+wpwEAQEIABAFAmTHcawJEDs4gPMoG10dAACN5wP/UozhFqHcUWRNhg4KwfY4
+HHXU8bf222naeYJHgaHadLTJJ8YQIQ9N5fYF7K4BM0jPZc48aaUPaBdhNxw+
+KDtQJWPzVREIbbGLRQ5WNYrLR6/7v1LHTI8RvgY22QZD9EAkFQwgdG8paIP4
+2APWewNf8e01t1oh4n5bDBtr4IaQoj0=
+=DHXw
 -----END PGP SIGNATURE-----
 """
 
 
 class SecTxtTestCase(TestCase):
     def test_future_expires(self):
         content = f"Expires: {date.today().year + 3}-01-01T12:00:00Z\n"
@@ -123,14 +127,45 @@
         p = Parser(content)
         self.assertEqual(p._errors[0]["code"], "no_uri")
 
     def test_signed(self):
         p = Parser(_signed_example)
         self.assertTrue(p.is_valid())
 
+    def test_signed_invalid_pgp(self):
+        # Remove required pgp signature header for pgp data error
+        content = _signed_example.replace(
+            "-----BEGIN PGP SIGNATURE-----", ""
+        )
+        p1 = Parser(content)
+        self.assertFalse(p1.is_valid())
+        self.assertEqual(
+            len([1 for r in p1._errors if r["code"] == "pgp_data_error"]), 1
+        )
+        # Add dash escaping within the pgp signature for pgp data error
+        content = _signed_example.replace(
+            "-----BEGIN PGP SIGNATURE-----", "-----BEGIN PGP SIGNATURE-----\n- \n"
+        )
+        p2 = Parser(content)
+        self.assertFalse(p2.is_valid())
+        self.assertEqual(
+            len([1 for r in p2._errors if r["code"] == "pgp_data_error"]), 1
+        )
+        # create an error in the pgp message by invalidating the base64 encoding of the signature
+        content = _signed_example.replace(
+            "wpwEAQEIABAFAmTHcawJEDs4gPMoG10dAACN5wP/UozhFqHcUWRNhg4KwfY4", "wpwEAQEIABAFAmTH"
+        ).replace(
+            "HHXU8bf222naeYJHgaHadLTJJ8YQIQ9N5fYF7K4BM0jPZc48aaUPaBdhNxw+", "HHXU8bf222naeYJHga"
+        )
+        p3 = Parser(content)
+        self.assertFalse(p3.is_valid())
+        self.assertEqual(
+            len([1 for r in p3._errors if r["code"] == "pgp_error"]), 1
+        )
+
     def test_signed_no_canonical(self):
         content = _signed_example.replace(
             "Canonical: https://example.com/.well-known/security.txt", ""
         )
         p = Parser(content)
         self.assertEqual(p._recommendations[0]["code"], "no_canonical")
 
@@ -170,21 +205,35 @@
         self.assertEqual(
             len([1 for r in p._notifications if r["code"] == "unknown_field"]), 0
         )
 
     def test_no_line_separators(self):
         expire_date = (date.today() + timedelta(days=10)).isoformat()
         single_line_security_txt = (
-            f"Contact: mailto:security@example.com  Expires: "
+            "Contact: mailto:security@example.com  Expires: "
             f"{expire_date}T18:37:07z  # All on a single line"
         )
-        p = Parser(single_line_security_txt)
-        self.assertFalse(p.is_valid())
+        p_line_separator = Parser(single_line_security_txt)
+        self.assertFalse(p_line_separator.is_valid())
+        self.assertEqual(
+            len([1 for r in p_line_separator._errors if r["code"] == "no_line_separators"]), 1
+        )
+        line_length_4_no_carriage_feed = (
+            "line 1\n"
+            "line 2\n"
+            "line 3\n"
+            "Contact: mailto:security@example.com  Expires"
+        )
+        p_length_4 = Parser(line_length_4_no_carriage_feed)
+        self.assertFalse(p_length_4.is_valid())
         self.assertEqual(
-            len([1 for r in p._errors if r["code"] == "no_line_separators"]), 1
+            len([1 for r in p_length_4._errors if r["code"] == "no_line_separators"]), 1
+        )
+        self.assertEqual(
+            [r["line"] for r in p_length_4._errors if r["code"] == "no_line_separators"], [4]
         )
 
     def test_csaf_https_uri(self):
         content = _signed_example.replace(
             "CSAF: https://example.com/.well-known/csaf/provider-metadata.json",
             "CSAF: http://example.com/.well-known/csaf/provider-metadata.json",
         )
@@ -235,7 +284,20 @@
         m.get(
             "https://example.com/security.txt", exc=requests.exceptions.ConnectTimeout
         )
         m.get("http://example.com/.well-known/security.txt", text=_signed_example)
         s = SecurityTXT("example.com")
         if not any(d["code"] == "invalid_uri_scheme" for d in s.errors):
             pytest.fail("invalid_uri_scheme error code should be given")
+
+
+def test_byte_order_mark(requests_mock: Mocker):
+    with Mocker() as m:
+        byte_content_with_bom = b'\xef\xbb\xbf\xef\xbb\xbfContact: mailto:me@example.com\n' \
+                                b'Expires: 2023-08-11T18:37:07z\n'
+        m.get(
+            "https://example.com/.well-known/security.txt",
+            headers={"content-type": "text/plain"},
+            content=byte_content_with_bom,
+        )
+        s = SecurityTXT("example.com")
+        assert(s.is_valid())
```

