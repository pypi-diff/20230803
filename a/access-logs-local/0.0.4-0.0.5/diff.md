# Comparing `tmp/access_logs_local-0.0.4.tar.gz` & `tmp/access_logs_local-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "access_logs_local-0.0.4.tar", last modified: Mon Jul 31 13:43:22 2023, max compression
+gzip compressed data, was "access_logs_local-0.0.5.tar", last modified: Thu Aug  3 15:19:58 2023, max compression
```

## Comparing `access_logs_local-0.0.4.tar` & `access_logs_local-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:43:22.082181 access_logs_local-0.0.4/
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1225 2023-07-31 13:39:05.000000 access_logs_local-0.0.4/LICENSE
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1538 2023-07-31 13:43:22.082181 access_logs_local-0.0.4/PKG-INFO
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1052 2023-07-31 13:40:04.000000 access_logs_local-0.0.4/README.rst
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      632 2023-07-31 13:40:22.000000 access_logs_local-0.0.4/pyproject.toml
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       38 2023-07-31 13:43:22.082181 access_logs_local-0.0.4/setup.cfg
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:43:22.078181 access_logs_local-0.0.4/src/
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:43:22.078181 access_logs_local-0.0.4/src/access_logs_local.egg-info/
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1538 2023-07-31 13:43:22.000000 access_logs_local-0.0.4/src/access_logs_local.egg-info/PKG-INFO
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      492 2023-07-31 13:43:22.000000 access_logs_local-0.0.4/src/access_logs_local.egg-info/SOURCES.txt
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)        1 2023-07-31 13:43:22.000000 access_logs_local-0.0.4/src/access_logs_local.egg-info/dependency_links.txt
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       23 2023-07-31 13:43:22.000000 access_logs_local-0.0.4/src/access_logs_local.egg-info/requires.txt
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       25 2023-07-31 13:43:22.000000 access_logs_local-0.0.4/src/access_logs_local.egg-info/top_level.txt
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:43:22.082181 access_logs_local-0.0.4/src/access_logs_local_driver/
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       79 2023-07-31 13:39:05.000000 access_logs_local-0.0.4/src/access_logs_local_driver/__init__.py
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      967 2023-07-31 13:39:05.000000 access_logs_local-0.0.4/src/access_logs_local_driver/geolookup.py
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     8058 2023-07-31 13:39:05.000000 access_logs_local-0.0.4/src/access_logs_local_driver/logdata.py
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      876 2023-07-31 13:39:05.000000 access_logs_local-0.0.4/src/access_logs_local_driver/process_download_logs.py
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:43:22.082181 access_logs_local-0.0.4/tests/
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)    28563 2023-07-31 13:39:05.000000 access_logs_local-0.0.4/tests/test_logdata.py
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     4272 2023-07-31 13:39:05.000000 access_logs_local-0.0.4/tests/test_process_download_logs.py
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-08-03 15:19:58.516203 access_logs_local-0.0.5/
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1225 2023-08-03 07:37:22.000000 access_logs_local-0.0.5/LICENSE
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1694 2023-08-03 15:19:58.516203 access_logs_local-0.0.5/PKG-INFO
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1208 2023-08-03 10:53:58.000000 access_logs_local-0.0.5/README.rst
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      632 2023-08-03 15:19:00.000000 access_logs_local-0.0.5/pyproject.toml
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       38 2023-08-03 15:19:58.516203 access_logs_local-0.0.5/setup.cfg
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-08-03 15:19:58.500202 access_logs_local-0.0.5/src/
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-08-03 15:19:58.504202 access_logs_local-0.0.5/src/access_logs_local.egg-info/
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1694 2023-08-03 15:19:58.000000 access_logs_local-0.0.5/src/access_logs_local.egg-info/PKG-INFO
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      492 2023-08-03 15:19:58.000000 access_logs_local-0.0.5/src/access_logs_local.egg-info/SOURCES.txt
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)        1 2023-08-03 15:19:58.000000 access_logs_local-0.0.5/src/access_logs_local.egg-info/dependency_links.txt
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       23 2023-08-03 15:19:58.000000 access_logs_local-0.0.5/src/access_logs_local.egg-info/requires.txt
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       25 2023-08-03 15:19:58.000000 access_logs_local-0.0.5/src/access_logs_local.egg-info/top_level.txt
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-08-03 15:19:58.516203 access_logs_local-0.0.5/src/access_logs_local_driver/
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       79 2023-08-03 07:37:22.000000 access_logs_local-0.0.5/src/access_logs_local_driver/__init__.py
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      967 2023-08-03 07:37:22.000000 access_logs_local-0.0.5/src/access_logs_local_driver/geolookup.py
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     8326 2023-08-03 15:15:10.000000 access_logs_local-0.0.5/src/access_logs_local_driver/logdata.py
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      878 2023-08-03 07:37:22.000000 access_logs_local-0.0.5/src/access_logs_local_driver/process_download_logs.py
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-08-03 15:19:58.516203 access_logs_local-0.0.5/tests/
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)    35687 2023-08-03 15:14:57.000000 access_logs_local-0.0.5/tests/test_logdata.py
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     3790 2023-08-03 15:17:57.000000 access_logs_local-0.0.5/tests/test_process_download_logs.py
```

### Comparing `access_logs_local-0.0.4/LICENSE` & `access_logs_local-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `access_logs_local-0.0.4/PKG-INFO` & `access_logs_local-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access_logs_local
-Version: 0.0.4
+Version: 0.0.5
 Summary: Functions required by the access-logs-local-driver
 Author-email: Cristian Garcia <cristian.garcia@ubiquitypress.com>
 Project-URL: Homepage, https://github.com/hirmeos/access_logs_driver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -22,14 +22,21 @@
 We strip out entries where the same (IP address * user agent) pair has accessed
 a URL within the last `SESSION_TIMEOUT` (e.g. half-hour)
 
 Additionally, we convert the URLs to ISBNs and collate request data by date,
 outputting a CSV for ingest via the stats system.
 
 Release Notes:
+[0.0.5] - 2023-07-03
+
+Changed:
+    * Added start_date and end_date for searching in the log files
+    * Added the measure_uri to the result
+
+Release Notes:
 [0.0.4] - 2023-07-31
 
 Changed:
     * Update file structure and name of the driver
 
 Release Notes:
 [0.0.3] - 2023-07-25
```

### Comparing `access_logs_local-0.0.4/README.rst` & `access_logs_local-0.0.5/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 We strip out entries where the same (IP address * user agent) pair has accessed
 a URL within the last `SESSION_TIMEOUT` (e.g. half-hour)
 
 Additionally, we convert the URLs to ISBNs and collate request data by date,
 outputting a CSV for ingest via the stats system.
 
 Release Notes:
+[0.0.5] - 2023-07-03
+
+Changed:
+    * Added start_date and end_date for searching in the log files
+    * Added the measure_uri to the result
+
+Release Notes:
 [0.0.4] - 2023-07-31
 
 Changed:
     * Update file structure and name of the driver
 
 Release Notes:
 [0.0.3] - 2023-07-25
```

### Comparing `access_logs_local-0.0.4/pyproject.toml` & `access_logs_local-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "access_logs_local"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Cristian Garcia", email="cristian.garcia@ubiquitypress.com" },
 ]
 description = "Functions required by the access-logs-local-driver"
 readme = "README.rst" 
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `access_logs_local-0.0.4/src/access_logs_local.egg-info/PKG-INFO` & `access_logs_local-0.0.5/src/access_logs_local.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access-logs-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: Functions required by the access-logs-local-driver
 Author-email: Cristian Garcia <cristian.garcia@ubiquitypress.com>
 Project-URL: Homepage, https://github.com/hirmeos/access_logs_driver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -22,14 +22,21 @@
 We strip out entries where the same (IP address * user agent) pair has accessed
 a URL within the last `SESSION_TIMEOUT` (e.g. half-hour)
 
 Additionally, we convert the URLs to ISBNs and collate request data by date,
 outputting a CSV for ingest via the stats system.
 
 Release Notes:
+[0.0.5] - 2023-07-03
+
+Changed:
+    * Added start_date and end_date for searching in the log files
+    * Added the measure_uri to the result
+
+Release Notes:
 [0.0.4] - 2023-07-31
 
 Changed:
     * Update file structure and name of the driver
 
 Release Notes:
 [0.0.3] - 2023-07-25
```

### Comparing `access_logs_local-0.0.4/src/access_logs_local_driver/geolookup.py` & `access_logs_local-0.0.5/src/access_logs_local_driver/geolookup.py`

 * *Files identical despite different names*

### Comparing `access_logs_local-0.0.4/src/access_logs_local_driver/logdata.py` & `access_logs_local-0.0.5/src/access_logs_local_driver/logdata.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 import urllib.parse
 
 
 class Request:
     """Represent the data in a single line of the Apache log file."""
 
     def __init__(
-        self,
-        ip_address: str,
-        re_match_dict: dict,
-        url_prefix: str,
-        url: str,
-        response_code: int,
-        content_length: int,
+            self,
+            ip_address: str,
+            re_match_dict: dict,
+            url_prefix: str,
+            url: str,
+            response_code: int,
+            content_length: int,
     ):
         self.ip_address = ip_address
         self.timestamp = time.strptime(
             re_match_dict.get("timestamp")[:20], "%d/%b/%Y:%H:%M:%S"
         )
-        self.user_agent = re_match_dict.get("user_agent")
+        self.user_agent = re_match_dict.get("user_agent", "")
         self.referer = re_match_dict.get("referer")
         self.url = self.parse_url(url, url_prefix)
         self.response_code = response_code
         self.content_length = content_length
 
     def parse_url(self, url: str, url_prefix: str) -> str:
         try:
@@ -44,67 +44,79 @@
 
     def normalise_url(self, url: str) -> str:
         try:
             return url[:-1] if url[-1] == "/" else url
         except IndexError as err:
             raise IndexError(f"Error parsing: {url}, {err}")
 
-    def fmttime(self) -> datetime:
+    def fmttime(self) -> str:
         fmt = "%Y-%m-%d %H:%M:%S"
         return datetime(*self.timestamp[:6]).strftime(fmt)
 
     def __str__(self) -> str:
         return f"Request {self.fmttime()}, {self.ip_address}, {self.url}"
 
-    def as_tuple(self) -> tuple[datetime, int, str]:
+    def __iter__(self):
+        for _item in self.as_tuple():
+            yield _item
+
+    def as_tuple(self) -> tuple[str, str, str, str]:
         return (self.fmttime(), self.ip_address, self.url, self.user_agent)
 
     def sanitise_url(self, regexes: str) -> None:
         for regex in regexes:
             matched = re.search(re.compile(regex), self.url)
             if matched is not None:
                 self.url = matched.group(0)
                 break
 
 
 class LogStream:
     def __init__(
-        self, log_dir: str, filter_groups: list, url_prefix: str, search_date: str
+            self,
+            log_dir: str,
+            filter_groups: list,
+            url_prefix: str,
+            start_date: str,
+            end_date: str,
     ) -> None:
         self.log_dir = log_dir
         self.filter_groups = filter_groups
         self.url_prefix = url_prefix
-        self.search_date = datetime.strptime(search_date, "%Y-%m-%d")
+        self.start_date = datetime.strptime(start_date, "%Y-%m-%d")
+        self.end_date = datetime.strptime(end_date, "%Y-%m-%d")
 
         self.access_logs_re = re.compile(
             r"(?P<ip_address>\d+\.\d+\.\d+\.\d+) "
             r"(?P<users>.+ .+) "
             r"\[(?P<timestamp>.+)\] "
             r'"(?P<request>.+)" '
             r"(?P<status_and_size>\d+ \d+) "
             r'(?P<referer>".+") '
             r'"(?P<user_agent>.+)"'
         )
 
-    def regex_match_line(self, line: str) -> str:
+    def regex_match_line(self, line: str) -> Request | None:
         """
         Use regex to convert the line to a dict identifying all
         parts, if not, just log it and skip the line, then, call the
         Request class. Also if the line doesn't match (strict) the
         timestamp requested, ignore it.
         """
         if re_match_dict := self.access_logs_re.search(line):
             re_match_dict = re_match_dict.groupdict()
         else:
             logging.info(f"Skipping invalid request log entry: {line}")
             return
         timestamp = datetime.strptime(
             re_match_dict.get("timestamp"), "%d/%b/%Y:%H:%M:%S %z"
         ).strftime("%Y-%m-%d")
-        if timestamp != self.search_date.strftime("%Y-%m-%d"):
+        max_date = self.end_date.strftime("%Y-%m-%d")
+        earliest_date = self.start_date.strftime("%Y-%m-%d")
+        if timestamp > max_date or timestamp < earliest_date:
             return
         ip_address = re_match_dict.get("ip_address")
         if not self.validate_ip_address(ip_address) or not re_match_dict:
             logging.info(f"Skipping invalid request log entry: {line}")
             return
         status_n_size = re_match_dict.get("status_and_size")
         response_code, content_length = status_n_size.split(" ", 1)
@@ -162,19 +174,17 @@
                     "Your file has to have a date at the end of it's name"
                 )
             date_dict = match.groupdict()
             timestamp = (
                 f"{date_dict['year']}-{date_dict['month']}"
                 f"-{date_dict['day']}"
             )
-            end_date = self.search_date + timedelta(days=1)
-            previous_date = self.search_date - timedelta(days=1)
             try:
                 timestamp = datetime.strptime(timestamp, "%Y-%m-%d")
-                if timestamp > end_date or timestamp < previous_date:
+                if timestamp > self.end_date or timestamp < self.start_date:
                     raise ValueError
             except ValueError:
                 continue
 
             yield os.path.join(self.log_dir, path)
 
     def lines(self) -> str:
@@ -188,31 +198,31 @@
         """Generate a filtered stream of requests; apply the predicate list
         `self.filters' to these requests; if any predicate fails, ignore
         the request and do not generate it for downstream processing."""
         if self.lines():
             for line in self.lines():
                 if line_request := self.regex_match_line(line):
                     for filter_group in self.filter_groups:
-                        filters, regex = filter_group
+                        measure_uri, filters, regex = filter_group
                         if not self.filter_in_line_request(
                             filters, line_request
                         ):
                             continue
                         line_request.sanitise_url(regex)
-                        yield line_request
+                        yield measure_uri, line_request
         else:
             logging.info("No file was processed")
 
     def filter_in_line_request(self, filters: list, line_request: str) -> bool:
         """If the filter from make_filters doesn't align with the line_request
         ignore the next iteration in the parent loop."""
         for f in filters:
             if not f(line_request):
                 return False
         return True
 
     def __iter__(self):
         return self.relevant_requests()
 
-    def return_output(self) -> list[str]:
+    def return_output(self) -> list[tuple]:
         """Return the results from the filters."""
-        return [str(result) for result in self]
+        return list(self)
```

### Comparing `access_logs_local-0.0.4/src/access_logs_local_driver/process_download_logs.py` & `access_logs_local-0.0.5/src/access_logs_local_driver/process_download_logs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import re
 
 from requests.models import Response
 
 
-def only_successful(request: Response) -> str:
+def only_successful(request: Response) -> bool:
     return request.response_code in [200, 304]
 
 
-def no_star(request: Response) -> str:
+def no_star(request: Response) -> bool:
     return request.url != "*"
 
 
-def no_plus_http(request: str) -> str:
+def no_plus_http(request: str) -> bool:
     return "+http" not in request.user_agent
 
 
-def make_filters(regexes: re, excluded: str, spiders: set()) -> list:
+def make_filters(regexes: re, excluded: list, spiders: set) -> list:
     def not_known_spider(request):
         return request.user_agent not in spiders
 
     def not_excluded_ip(request):
         return request.ip_address not in excluded
 
     def filter_url(request):
```

### Comparing `access_logs_local-0.0.4/tests/test_logdata.py` & `access_logs_local-0.0.5/tests/test_logdata.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import gzip
 import os
 import pathlib as pl
 from unittest import TestCase
 
-from access_logs_local.src.access_logs_local_driver import LogStream
-from access_logs_local.src.access_logs_local_driver import (
+from src.access_logs_local_driver import LogStream
+from src.access_logs_local_driver import (
     make_filters
 )
 
 
 class TestLogData(TestCase):
     def setUp(self) -> None:
         self.modes_cjs = [
@@ -92,54 +92,67 @@
         if not pl.Path(path).resolve().is_file():
             return False
         return True
 
     def test_apache_log_stream_creates_is_succesful_one_match_cjs(self) -> None:
         """Test the class LogStream the same way as is executed
         from the plugin"""
-        search_date = '2023-06-02'
+        start_date = '2023-06-01'
+        end_date = '2023-06-03'
         content = str.encode(
             "cjs.testing-url.com:123 12.90.253.37 - - "
             '[02/Jun/2023:04:55:37 +0000] "GET /testing-url/'
             "10.3456768/cjs.abcde.1234/image/1234/download/ "
             'HTTP/1.1" 200 123456 "https://www.google.com/" '
             '"Mozilla/5.0 (Linux; Android 13; testPhone ABCDEF) '
             "TestPhone/123.45 (KHTML, like Gecko) TestBrowser"
             '/21.0 Chrome/120.3.4567.890 Mobile Safari/537.36"'
         )
         self.create_file_log(self.file_log_apache, content)
         filter_groups = []
         for mode in self.modes_cjs:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         result = result.return_output()
-        # Assert the result has got the right content)
+        # Assert the result has got the right content
+        self.assertEqual(
+            result[0][0],
+            'tag:testing.eu,2023:readership:abc-html',
+        )
         self.assertEqual(
-            result,
-            [
+            str(result[0][1]),
+            (
                 "Request 2023-06-02 04:55:37, 12.90.253.37, "
                 "https://abc.test.testing/testing-url/10.3456768"
-                "/cjs.abcde.1234/image/1234/download",
-            ],
+                "/cjs.abcde.1234/image/1234/download"
+            )
         )
 
     def test_apache_log_stream_creates_is_succesful_two_matches_cjs(
         self
     ) -> None:
         """Test the class LogStream the same way as is executed
         from the plugin"""
-        search_date = '2023-06-02'
+        start_date = '2023-06-01'
+        end_date = '2023-06-02'
         content = str.encode(
             "cjs.testing-url.com:123 12.34.253.12 - - "
             '[02/Jun/2023:04:55:37 +0000] "GET /testing-url/'
             "10.3456768/cjs.abcde.1234/image/1234/download/ "
             'HTTP/1.1" 200 123456 "https://www.google.com/" '
             '"Mozilla/5.0 (Linux; Android 13; testPhone ABCDEF) '
             "TestPhone/123.45 (KHTML, like Gecko) TestBrowser"
@@ -152,72 +165,134 @@
             "TestPhone/123.45 (KHTML, like Gecko) TestBrowser"
             '/21.0 Chrome/120.3.4567.890 Mobile Safari/537.36"\n'
         )
         self.create_file_log(self.file_log_apache, content)
         filter_groups = []
         for mode in self.modes_cjs:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         result = result.return_output()
         # Assert the result has got the right content
         self.assertEqual(
-            result,
-            [
-                (
-                    "Request 2023-06-02 04:55:37, 12.34.253.12, "
-                    "https://abc.test.testing/testing-url/10.3456"
-                    "768/cjs.abcde.1234/image/1234/download"
-                ),
-                (
-                    "Request 2023-06-02 04:55:37, 34.34.253.34, "
-                    "https://abc.test.testing/testing-url/10.56789"
-                    "/cjs.fghijk/testing/download"
+            result[0][0],
+            'tag:testing.eu,2023:readership:abc-html',
+        )
+        self.assertEqual(
+            str(result[0][1]),
+            (
+                'Request 2023-06-02 04:55:37, 12.34.253.12, '
+                'https://abc.test.testing/testing-url/10.3456768/cjs'
+                '.abcde.1234/image/1234/download'
+            )
+        )
+        self.assertEqual(
+            result[1][0],
+            'tag:testing.eu,2023:readership:abc-html',
+        )
+        self.assertEqual(
+            str(result[1][1]),
+            (
+                'Request 2023-06-02 04:55:37, 34.34.253.34, '
+                'https://abc.test.testing/testing-url/10.56789/cjs.'
+                'fghijk/testing/download'
+            )
+        )
+
+    def test_apache_log_start_date_and_end_date_no_match(self) -> None:
+        """Test the class LogStream the same way as is executed
+        from the plugin"""
+        start_date = '2023-05-01'
+        end_date = '2023-05-21'
+        content = str.encode(
+            "cjs.testing-url.com:123 12.90.253.37 - - "
+            '[02/Jun/2023:04:55:37 +0000] "GET /testing-url/'
+            "10.3456768/cjs.abcde.1234/image/1234/download/ "
+            'HTTP/1.1" 200 123456 "https://www.google.com/" '
+            '"Mozilla/5.0 (Linux; Android 13; testPhone ABCDEF) '
+            "TestPhone/123.45 (KHTML, like Gecko) TestBrowser"
+            '/21.0 Chrome/120.3.4567.890 Mobile Safari/537.36"'
+        )
+        self.create_file_log(self.file_log_apache, content)
+        filter_groups = []
+        for mode in self.modes_cjs:
+            filters = (
+                mode.get("measure"),
+                make_filters(
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-            ],
+                mode.get("regex")
+            )
+            filter_groups.append(filters)
+        result = LogStream(
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
+        # Assert the result has got the right content
+        self.assertEqual([], result.return_output())
 
     def test_apache_log_stream_no_match_file_structure_is_ok(self) -> None:
         """Test no match with the current filters even if
         the file structure is fine, will return empty list."""
-        search_date = '2023-06-02'
+        start_date = '2023-06-01'
+        end_date = '2023-06-03'
         content = str.encode(
             "abcdef.tyestset.com:123 12.34.253.37 - - "
             '[03/Jun/2023:04:51:45 +0000] "GET /test'
             '/test/12.3456/abc.v12a1.1234/ HTTP/1.1" '
             '200 49221 "-" "test/5.0 (Windows NT 10.0; '
             'Win64; x64; ab:123.4) test/20100101 test/112.0"'
         )
         self.create_file_log(self.file_log_apache, content)
         filter_groups = []
         for mode in self.modes_cjs:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual([], result.return_output())
 
     def test_apache_log_stream_raises_error_no_matches_timestamp(self) -> None:
         """Test the class LogStream fails because there is no match.
         The file test_access.log-NODATE.gz should have a date
         at the end."""
-        search_date = '2023-06-03'
+        start_date = '2023-06-02'
+        end_date = '2023-06-03'
         content = str.encode(
             "abcdef.presstest.com:123 12.12.345.67 - - "
             '[03/Jun/2023:04:51:45 +0000] "GET /articles/'
             'abstract/12.3456/abc.v12a1.1234/ HTTP/1.1" 200 '
             '49221 "-" "Mozilla/5.0 (Windows NT 10.0; Win64; '
             'x64; ab:123.4) Gecko/12345678 Firefox/112.0"'
         )
@@ -225,166 +300,214 @@
         os.rename(
             self.logs_files + self.file_log_apache,
             self.logs_files + "test_access.log-NODATE.gz",
         )
         filter_groups = []
         for mode in self.modes_cjs:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         with self.assertRaises(AttributeError) as err:
             result = LogStream(
-                self.logs_files, filter_groups, self.url_prefix, search_date
+                self.logs_files,
+                filter_groups,
+                self.url_prefix,
+                start_date,
+                end_date
             )
             result = result.return_output()
         self.assertEqual(
             str(err.exception),
             "Your file has to have a date at the end of it's name"
         )
 
     def test_apache_log_stream_raises_error_no_matches_lines(self) -> None:
         """Test the class LogStream fails because there is no match.
         The line method will raise exception because the structure of
         the input file is wrong."""
-        search_date = '2023-06-03'
+        start_date = '2023-06-02'
+        end_date = '2023-06-04'
         content = b'test_worng - wrong structure"'
         self.create_file_log(self.file_log_apache, content)
         filter_groups = []
         for mode in self.modes_cjs:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual([], result.return_output())
 
     def test_apache_log_stream_no_match_request_is_wrong_right_structure(
         self
     ) -> None:
-        search_date = '2023-06-03'
+        start_date = '2023-06-03'
+        end_date = '2023-06-04'
         """Test the class LogStream there is no match.
         The file structure is right but the request is wrong."""
         content = str.encode(
             "abcdef.presstest.com:123 12.34.253.37 - - "
             '[03/Jun/2023:04:51:45 +0000] "ERROR /articles/'
             'abstract/12.3456/abc.v12a1.1234/ HTTP/1.1" 200 '
             '49221 "-" "Mozilla/5.0 (Windows NT 10.0; Win64; '
             'x64; ab:123.4) Gecko/12345678 Firefox/112.0"'
         )
         self.create_file_log(self.file_log_apache, content)
         filter_groups = []
         for mode in self.modes_cjs:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual([], result.return_output())
 
     def test_apache_log_stream_raises_error_there_is_no_timestamp(self) -> None:
         """Test the class LogStream there is no match because of
         missing timestamp."""
-        search_date = '2023-06-03'
+        start_date = '2023-06-03'
+        end_date = '2023-06-04'
         content = str.encode(
             "abcdef.presstest.com:123 12.12.345.67 - - 'NO TIMESTAMP ' GET "
             "/articles/abstract/12.3456/abcdef.v52i2.8160/ "
             'HTTP/1.1" 200 4522 "-" "Scoop.it"'
         )
         self.create_file_log(self.file_log_apache, content)
         filter_groups = []
         for mode in self.modes_cjs:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual([], result.return_output())
 
     def test_apache_log_stream_wrong_request_and_wrong_structure_raises_error(
         self,
     ) -> None:
-        search_date = '2023-06-03'
+        start_date = '2023-06-03'
+        end_date = '2023-06-04'
         """Test the class LogStream fails because there is no match.
         The file structure is wrong and the request is wrong."""
         content = str.encode(
             "abcdef.presstest.com:123 146.249.11.3 - - "
             "[02/Jun/2023:08:18:56 +0000] --->ErrorHEADtest "
             '"-" "Scoop.it"'
         )
         self.create_file_log(self.file_log_apache, content)
         filter_groups = []
         for mode in self.modes_cjs:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual([], result.return_output())
 
     def test_apache_log_stream_no_matches_line_r_n_ua_re(self) -> None:
         """Test the class LogStream fails because there is no match.
         The content of the files doesn't match r_n_ua_re regex."""
-        search_date = '2023-06-01'
+        start_date = '2023-06-01'
+        end_date = '2023-06-02'
         content = str.encode(
             "abcdef.presstest.com:123 12.34.253.37 - - "
             '[01/Jun/2023:06:52:43 +0000] "GET /jms/public'
             '/journals/1/journalFavicon_en_US.ico HTTP/1.1" 404 '
             '5010 "test error!"test error!"'
         )
         self.create_file_log(self.file_log_apache, content)
         filter_groups = []
         for mode in self.modes_cjs:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual([], result.return_output())
 
     def test_apache_log_stream_ignores_reuqest_if_its_missing_parts(
         self
     ) -> None:
         """Test the class LogStream ignores urls that have a missing method,
         url or version."""
-        search_date = '2023-06-01'
+        start_date = '2023-06-01'
+        end_date = '2023-06-02'
         content = str.encode(
             "abc.presstest.com:123 12.34.253.37 - - "
             '[01/Jun/2023:06:52:43 +0000] "GET /jms/public'
             '/journals/1/journalFavicon_en_US.ico" 404 5010 '
             '"https://abc.defg.info/'
             'abc.v52i2.8023/" "Mozilla/5.0 (Linux; Android 10; K) '
             "Appltest_log_stream_ignores_reuqest_if_its_missing_parts"
@@ -393,89 +516,113 @@
             "com:123 12.12.345.67 - - [01/Jun/2023:06:52:50 +0000] "
             '"GET /jms/public/journals/1/journalFavicon_en_US.ico" '
         )
         self.create_file_log(self.file_log_apache, content)
         filter_groups = []
         for mode in self.modes_cjs:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual([], result.return_output())
 
     def test_apache_log_stream_the_ip_address_is_wrong_no_match(
         self,
     ) -> None:
         """Test the class LogStream fails because there is no match.
         The file structure is wrong and the request is wrong."""
-        search_date = '2023-06-01'
+        start_date = '2023-06-01'
+        end_date = '2023-06-02'
         content = str.encode(
             "cjs.testing-url.com:123 99.999.999.999 - - "
             '[02/Jun/2023:04:55:37 +0000] "GET /testing-url/'
             "10.3456768/cjs.abcde.1234/image/1234/download/ "
             'HTTP/1.1" 200 123456 "https://www.google.com/" '
             '"Mozilla/5.0 (Linux; Android 13; testPhone ABCDEF) '
             "TestPhone/123.45 (KHTML, like Gecko) TestBrowser"
             '/21.0 Chrome/120.3.4567.890 Mobile Safari/537.36"'
         )
         self.create_file_log(self.file_log_apache, content)
         filter_groups = []
         for mode in self.modes_cjs:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual([], result.return_output())
 
-    def test_apache_logs_no_matches_search_date_wrong_file(self):
+    def test_apache_logs_no_matches_start_date_wrong_file(self):
         """The search date is in august and the file name is in June."""
-        search_date = '2023-08-01'
+        start_date = '2023-08-01'
+        end_date = '2023-08-02'
         content = str.encode(
             "cjs.testing-url.com:123 12.90.253.37 - - "
             '[02/Jun/2023:04:55:37 +0000] "GET /testing-url/'
             "10.3456768/cjs.abcde.1234/image/1234/download/ "
             'HTTP/1.1" 200 123456 "https://www.google.com/" '
             '"Mozilla/5.0 (Linux; Android 13; testPhone ABCDEF) '
             "TestPhone/123.45 (KHTML, like Gecko) TestBrowser"
             '/21.0 Chrome/120.3.4567.890 Mobile Safari/537.36"'
         )
         self.create_file_log(self.file_log_apache, content)
         filter_groups = []
         for mode in self.modes_nginx:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual(result.return_output(), [])
 
-    def test_nginx_logs_is_successful_four_matches(self):
+    def test_nginx_logs_is_successful_two_matches(self):
         """Test the nginx logs are processed as well
         the four lines will be matched."""
-        search_date = '2023-07-06'
+        start_date = '2023-07-05'
+        end_date = '2023-07-06'
         content = str.encode(
             '25.123.123.1 - - [06/Jul/2023:15:04:34 +0000] "GET '
             '/test.txt HTTP/1.0" 302 555 "-" '
             '"Mozitest (http://Moziddler.io/about)"\n'
             '25.123.123.2 - - [06/Jul/2023:15:49:29 +0000] "GET '
             '/test/books/e/10.5334/bbc HTTP/1.0" 200 547 "-" '
             '"Ozitest/7.7 (X11; Xunil x86_64; rh:123.1) SalaTest/20100101 "'
@@ -488,239 +635,363 @@
             '"Ozitest/7.7 (X11; Xunil x86_64; rh:123.1) SalaTest/20100101 '
             'prüfen/123.1"'
         )
         self.create_file_log(self.file_log_nginx, content)
         filter_groups = []
         for mode in self.modes_nginx:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
+        )
+        result = result.return_output()
+        self.assertEqual(
+            result[0][0],
+            'https://testing.test-eu.org/abc/v1'
+        )
+        self.assertEqual(
+            str(result[0][1]),
+            (
+                'Request 2023-07-06 15:49:29, 25.123.123.2, '
+                'https://abc.test.testing/test/books/e/10.5334/bbc'
+            )
         )
         self.assertEqual(
-            result.return_output(),
-            [
-                "Request 2023-07-06 15:49:29, 25.123.123.2, "
-                "https://abc.test.testing/test/books/e/10.5334/bbc",
-                "Request 2023-07-06 21:23:18, 25.123.123.4, "
-                "https://abc.test.testing/test/10.5334/bay",
-            ],
+            result[1][0],
+            'https://testing.test-eu.org/abc/v1'
+        )
+        self.assertEqual(
+            str(result[1][1]),
+            (
+                'Request 2023-07-06 21:23:18, 25.123.123.4, '
+                'https://abc.test.testing/test/10.5334/bay'
+            )
         )
 
     def test_nginx_logs_no_matches_line_r_n_ua_re(self):
         """Test the nginx logs are processed as well
         the four lines will be matched."""
-        search_date = '2023-07-06'
+        start_date = '2023-07-05'
+        end_date = '2023-07-07'
         content = str.encode(
             '25.123.123.1 - - [06/Jul/2023:15:04:34 +0000] "GET '
             '/test.txt HTTP/1.0" 302 555 "-" '
             '"WrongTESTUSERAGENT"\n'
         )
         self.create_file_log(self.file_log_nginx, content)
         filter_groups = []
         for mode in self.modes_nginx:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual(result.return_output(), [])
 
-    def test_nginx_logs_no_matches_search_date_wrong_file(self):
+    def test_nginx_logs_no_matches_start_date_wrong_file(self):
         """The search date is in august and the file name is in July."""
-        search_date = '2023-08-01'
+        start_date = '2023-07-31'
+        end_date = '2023-08-02'
         content = str.encode(
             '25.123.123.1 - - [06/Jul/2023:15:04:34 +0000] "GET '
             '/test.txt HTTP/1.0" 302 555 "-" '
             '"Mozitest (http://Moziddler.io/about)"\n'
         )
         self.create_file_log(self.file_log_nginx, content)
         filter_groups = []
         for mode in self.modes_nginx:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual(result.return_output(), [])
 
-    def test_nginx_logs_no_matches_search_date_wrong_line(self):
+    def test_nginx_logs_no_matches_start_date_wrong_line(self):
         """The search date is in July and the line is in august."""
-        search_date = '2023-07-06'
+        start_date = '2023-07-06'
+        end_date = '2023-07-07'
         content = str.encode(
             '25.123.123.1 - - [06/Aug/2023:15:04:34 +0000] "GET '
             '/test.txt HTTP/1.0" 302 555 "-" '
             '"Mozitest (http://Moziddler.io/about)"\n'
         )
         self.create_file_log(self.file_log_nginx, content)
         filter_groups = []
         for mode in self.modes_nginx:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual(result.return_output(), [])
 
     def test_nginx_log_stream_no_match_file_structure_is_ok(self) -> None:
         """Test the nginx logs are processed as well
         the four lines will be matched."""
-        search_date = '2023-07-06'
+        start_date = '2023-07-06'
+        end_date = '2023-07-07'
         content = str.encode(
             '25.123.123.1 - - [06/Jul/2023:15:04:34 +0000] "GET '
             'NOMATCH/test.txt HTTP/1.0" 302 555 "-" '
             '"Mozitest (http://Moziddler.io/about)"\n'
             '25.123.123.2 - - [06/Jul/2023:15:49:29 +0000] "GET '
             '/NOMATCH/books/e/10.5334/bbc HTTP/1.0" 200 547 "-" '
             '"Ozitest/7.7 (X11; Xunil x86_64; rh:123.1) SalaTest/20100101 "'
             "prüfen/123.1\n"
         )
         self.create_file_log(self.file_log_nginx, content)
         filter_groups = []
         for mode in self.modes_nginx:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual(result.return_output(), [])
 
     def test_nginx_log_stream_no_match_request_is_wrong_right_structure(
         self
     ) -> None:
         """Test the class LogStream there is no match.
         The file structure is right but the request is wrong."""
-        search_date = '2023-07-06'
+        start_date = '2023-07-06'
+        end_date = '2023-07-07'
         content = str.encode(
             '25.123.123.3 - - [06/Jul/2023:20:15:19 +0000] "ERROR '
             '/test-query HTTP/1.0" 404 502 "-" '
             '"Mozitest (http://Moziddler.io/about)"\n'
             '25.123.123.4 - - [06/Jul/2023:21:23:18 +0000] "WRONG REQUEST '
             '/test/10.5334/bay HTTP/1.0" 200 496 "-" '
             '"Ozitest/7.7 (X11; Xunil x86_64; rh:123.1) SalaTest/20100101 '
             'prüfen/123.1"'
         )
         self.create_file_log(self.file_log_nginx, content)
         filter_groups = []
         for mode in self.modes_nginx:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual([], result.return_output())
 
     def test_nginx_log_stream_raises_error_there_is_no_timestamp(self) -> None:
         """Test the class LogStream there is no match because of
         missing timestamp."""
-        search_date = '2023-07-06'
+        start_date = '2023-07-06'
+        end_date = '2023-07-07'
         content = str.encode(
             '25.123.123.3 - - NO TIMESTAMPP "GET '
             '/test-query HTTP/1.0" 404 502 "-" '
             '"Mozitest (http://Moziddler.io/about)"'
         )
         self.create_file_log(self.file_log_nginx, content)
         filter_groups = []
         for mode in self.modes_nginx:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual([], result.return_output())
 
     def test_nginx_log_stream_no_match_wrong_request_and_structure_raises_error(
         self,
     ) -> None:
-        search_date = '2023-07-06'
+        start_date = '2023-07-06'
+        end_date = '2023-07-07'
         """Test the class LogStream fails because there is no match.
         The file structure is wrong and the request is wrong."""
         content = str.encode(
             '146.249.11.159 - - [06/Jul/2023:21:23:18 +0000] ----> ERRORRR'
             '/wrong/10.5334/bay HTTP/1.0" 200 496 "-" '
             '"Ozitest/7.7 (X11; Xunil x86_64; rh:123.1) SalaTest/20100101 '
             'prüfen/123.1"'
         )
         self.create_file_log(self.file_log_nginx, content)
         filter_groups = []
         for mode in self.modes_cjs:
             filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual([], result.return_output())
 
     def test_nginx_log_stream_the_ip_address_is_wrong_will_raise_error(
         self,
     ) -> None:
-        search_date = '2023-07-06'
+        start_date = '2023-07-05'
+        end_date = '2023-07-07'
         """Test the class LogStream fails because there is no match.
         The file structure is wrong and the request is wrong."""
         content = str.encode(
             '999.999.999.999 - - [06/Jul/2023:15:04:34 +0000] "GET '
             '/test.txt HTTP/1.0" 302 555 "-" '
             '"Mozitest (http://Moziddler.io/about)"'
         )
         self.create_file_log(self.file_log_nginx, content)
         filter_groups = []
         for mode in self.modes_cjs:
             filters = (
+                mode.get("measure"),
+                make_filters(
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
+                ),
+                mode.get("regex")
+            )
+            filter_groups.append(filters)
+
+        result = LogStream(
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
+        )
+        self.assertEqual([], result.return_output())
+
+    def test_nginx_log_stream_the_start_date_and_end_date_no_match(
+        self,
+    ) -> None:
+        start_date = '2023-07-01'
+        end_date = '2023-07-02'
+        """Test the class LogStream fails because there is no match.
+        The file structure is wrong and the request is wrong."""
+        content = str.encode(
+            '25.123.123.1 - - [06/Jul/2023:15:04:34 +0000] "GET '
+            '/test.txt HTTP/1.0" 302 555 "-" '
+            '"Mozitest (http://Moziddler.io/about)"\n'
+            '25.123.123.2 - - [06/Jul/2023:15:49:29 +0000] "GET '
+            '/test/books/e/10.5334/bbc HTTP/1.0" 200 547 "-" '
+            '"Ozitest/7.7 (X11; Xunil x86_64; rh:123.1) SalaTest/20100101 "'
+            "prüfen/123.1\n"
+        )
+        self.create_file_log(self.file_log_nginx, content)
+        filter_groups = []
+        for mode in self.modes_cjs:
+            filters = (
+                mode.get("measure"),
                 make_filters(
-                    mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
+                    mode.get("regex"),
+                    ["8.8.8.8", "9.9.9.9"],
+                    self.spiders
                 ),
-                mode["regex"],
+                mode.get("regex")
             )
             filter_groups.append(filters)
 
         result = LogStream(
-            self.logs_files, filter_groups, self.url_prefix, search_date
+            self.logs_files,
+            filter_groups,
+            self.url_prefix,
+            start_date,
+            end_date
         )
         self.assertEqual([], result.return_output())
```

### Comparing `access_logs_local-0.0.4/tests/test_process_download_logs.py` & `access_logs_local-0.0.5/tests/test_process_download_logs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from unittest import TestCase
 from requests.models import Response
 from src.access_logs_local_driver.process_download_logs import (
     make_filters,
-    method_ok,
     no_plus_http,
     no_star,
     only_successful,
 )
 
 
 class TestProcessDownLogs(TestCase):
@@ -76,25 +75,14 @@
     def test_response_has_no_star(self):
         the_response = Response()
         the_response.url = "nice_url/"
         self.assertTrue(no_star(the_response))
         the_response.url = "*"
         self.assertFalse(no_star(the_response))
 
-    def test_response_method_ok(self):
-        the_response = Response()
-        the_response.method = "GET"
-        self.assertTrue(method_ok(the_response))
-        the_response.method = "POST"
-        self.assertTrue(method_ok(the_response))
-        the_response.method = "PATCH"
-        self.assertFalse(method_ok(the_response))
-        the_response.method = "DELETE"
-        self.assertFalse(method_ok(the_response))
-
     def test_response_no_plus_http(self):
         the_response = Response()
         the_response.user_agent = "http"
         self.assertTrue(no_plus_http(the_response))
         the_response.user_agent = "+http"
         self.assertFalse(no_plus_http(the_response))
 
@@ -107,9 +95,8 @@
                     mode["regex"], ["8.8.8.8", "9.9.9.9"], self.spiders
                 ),
                 mode["regex"],
             )
         self.assertTrue(len(filters) > 0)
         self.assertIn(only_successful, filters[0])
         self.assertIn(no_star, filters[0])
-        self.assertIn(method_ok, filters[0])
         self.assertIn(no_plus_http, filters[0])
```

