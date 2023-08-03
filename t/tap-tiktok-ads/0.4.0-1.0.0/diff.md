# Comparing `tmp/tap-tiktok-ads-0.4.0.tar.gz` & `tmp/tap-tiktok-ads-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-tiktok-ads-0.4.0.tar", last modified: Thu Jun 22 08:31:04 2023, max compression
+gzip compressed data, was "tap-tiktok-ads-1.0.0.tar", last modified: Thu Aug  3 18:30:39 2023, max compression
```

## Comparing `tap-tiktok-ads-0.4.0.tar` & `tap-tiktok-ads-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 08:31:04.401244 tap-tiktok-ads-0.4.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      263 2023-06-22 08:31:04.401244 tap-tiktok-ads-0.4.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7970 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-06-22 08:31:04.401244 tap-tiktok-ads-0.4.0/setup.cfg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      790 2023-06-22 08:24:58.000000 tap-tiktok-ads-0.4.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 08:31:04.397244 tap-tiktok-ads-0.4.0/tap_tiktok_ads/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1798 2023-05-24 06:51:41.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7638 2023-06-21 21:32:34.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      674 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/discover.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 08:31:04.401244 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5078 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights_by_age_and_gender.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3082 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights_by_country.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3078 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights_by_platform.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10070 2023-06-21 21:32:34.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/adgroups.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3802 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ads.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2095 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/advertisers.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1531 2023-06-21 21:32:34.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/campaigns.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1009 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17030 2023-06-22 08:24:58.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1630 2023-05-26 18:02:58.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 08:31:04.397244 tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      263 2023-06-22 08:31:04.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      965 2023-06-22 08:31:04.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-22 08:31:04.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-06-22 08:31:04.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-06-22 08:31:04.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-06-22 08:31:04.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 08:31:04.401244 tap-tiktok-ads-0.4.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4633 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.4.0/tests/test_all_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2269 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.4.0/tests/test_automatic_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8049 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.4.0/tests/test_bookmarks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6083 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.4.0/tests/test_discovery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9068 2023-06-20 05:59:29.000000 tap-tiktok-ads-0.4.0/tests/test_interrupted_sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3174 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.4.0/tests/test_pagination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6996 2023-06-22 08:24:58.000000 tap-tiktok-ads-0.4.0/tests/test_start_date.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 18:30:39.119762 tap-tiktok-ads-1.0.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2023-07-21 06:11:23.000000 tap-tiktok-ads-1.0.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2023-07-21 06:11:23.000000 tap-tiktok-ads-1.0.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      263 2023-08-03 18:30:39.119762 tap-tiktok-ads-1.0.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8073 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-08-03 18:30:39.119762 tap-tiktok-ads-1.0.0/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      790 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 18:30:39.115762 tap-tiktok-ads-1.0.0/tap_tiktok_ads/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1805 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7605 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      674 2023-07-21 06:11:23.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 18:30:39.119762 tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6577 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/ad_insights.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4561 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/ad_insights_by_age_and_gender.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4490 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/ad_insights_by_country.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4486 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/ad_insights_by_platform.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11425 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/adgroups.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6581 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/ads.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2225 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/advertisers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/campaign_insights_by_province.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2553 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/campaigns.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1009 2023-07-21 06:11:23.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20261 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1630 2023-07-21 06:11:23.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 18:30:39.115762 tap-tiktok-ads-1.0.0/tap_tiktok_ads.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      263 2023-08-03 18:30:39.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1023 2023-08-03 18:30:39.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-08-03 18:30:39.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-08-03 18:30:39.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-08-03 18:30:39.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-08-03 18:30:39.000000 tap-tiktok-ads-1.0.0/tap_tiktok_ads.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-03 18:30:39.119762 tap-tiktok-ads-1.0.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5926 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tests/test_all_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2300 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tests/test_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8080 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tests/test_bookmarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6083 2023-07-21 06:11:23.000000 tap-tiktok-ads-1.0.0/tests/test_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9099 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tests/test_interrupted_sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3314 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tests/test_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6939 2023-08-03 18:24:52.000000 tap-tiktok-ads-1.0.0/tests/test_start_date.py
```

### Comparing `tap-tiktok-ads-0.4.0/LICENSE` & `tap-tiktok-ads-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.4.0/README.md` & `tap-tiktok-ads-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 This is a [Singer](https://singer.io) tap that produces JSON-formatted
 data from the TikTok Marketing API following the [Singer
 spec](https://github.com/singer-io/getting-started/blob/master/SPEC.md).
 
 This tap: 
 
 - Pulls raw data from the [TikTok Marketing API](https://ads.tiktok.com/marketing_api/docs). 
-- Extracts the following resources from TikTok Marketing API for a single repository: 
-	- [Accounts](https://ads.tiktok.com/marketing_api/docs?id=1708503235186689) - Endpoint: https://business-api.tiktok.com/open_api/v1.2/advertiser/info/ 
-	- [Campaigns](https://ads.tiktok.com/marketing_api/docs?id=1708582970809346) - Endpoint: https://ads.tiktok.com/open_api/v1.2/campaign/get/ 
-	- [Adgroups](https://ads.tiktok.com/marketing_api/docs?id=1708503489590273) - Endpoint: https://ads.tiktok.com/open_api/v1.2/adgroup/get/ 
-	- [Ads](https://ads.tiktok.com/marketing_api/docs?id=1708572923161602) - Endpoint: https://business-api.tiktok.com/open_api/v1.2/ad/get/ 
-	- [Reporting](https://ads.tiktok.com/marketing_api/docs?id=1701890949889025) - Endpoint: https://ads.tiktok.com/open_api/v1.2/reports/integrated/get/ 
-		- [Ad Insights](https://ads.tiktok.com/marketing_api/docs?id=1707957200780290)
-		- [Ad Insights by Age and Gender](https://ads.tiktok.com/marketing_api/docs?id=1707957217727489)
-		- [Ad Insights by Country](https://ads.tiktok.com/marketing_api/docs?id=1707957217727489)
-		- [Ad Insights by Platform](https://ads.tiktok.com/marketing_api/docs?id=1707957217727489)
+- Extracts the following resources from TikTok Marketing API for a single repository:
+	- [Accounts](https://ads.tiktok.com/marketing_api/docs?id=1739593083610113) - Endpoint: https://business-api.tiktok.com/open_api/v1.3/advertiser/info/ 
+	- [Campaigns](https://ads.tiktok.com/marketing_api/docs?id=1739315828649986) - Endpoint: https://ads.tiktok.com/open_api/v1.3/campaign/get/ 
+	- [Adgroups](https://ads.tiktok.com/marketing_api/docs?id=1739314558673922) - Endpoint: https://ads.tiktok.com/open_api/v1.3/adgroup/get/ 
+	- [Ads](https://ads.tiktok.com/marketing_api/docs?id=1735735588640770) - Endpoint: https://business-api.tiktok.com/open_api/v1.3/ad/get/ 
+	- [Reporting](https://ads.tiktok.com/marketing_api/docs?id=1751087777884161) - Endpoint: https://ads.tiktok.com/open_api/v1.3/report/integrated/get/ 
+		- [Ad Insights](https://ads.tiktok.com/marketing_api/docs?id=1738864915188737)
+		- [Ad Insights by Age and Gender](https://ads.tiktok.com/marketing_api/docs?id=1738864928947201)
+		- [Ad Insights by Country](https://ads.tiktok.com/marketing_api/docs?id=1738864928947201)
+		- [Ad Insights by Platform](https://ads.tiktok.com/marketing_api/docs?id=1738864928947201)
+        - [Campaign Insights by Province](https://ads.tiktok.com/marketing_api/docs?id=1738864928947201)
 - Outputs the schema for each resource
 - Incrementally pulls data based on the input state
 
 ## Authentication
 
 The tap uses an access token provided by the TikTok Marketing API to make the calls to the API. The access token does not expire, but it'll become invalid if the advertiser cancels the authorization. An invalid access token cannot be renewed or refreshed. THis access token can be obtained by following the step-by-step instructions on the [TikTok Marketing API Docs - Authorization](https://ads.tiktok.com/marketing_api/docs?id=1701890912382977) and [TikTok Marketing API Docs - Authentication](https://ads.tiktok.com/marketing_api/docs?id=1701890914536450).
```

### Comparing `tap-tiktok-ads-0.4.0/setup.py` & `tap-tiktok-ads-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="tap-tiktok-ads",
-    version="0.4.0",
+    version="1.0.0",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["tap_tiktok_ads"],
     install_requires=[
         "singer-python==5.13.0",
```

### Comparing `tap-tiktok-ads-0.4.0/tap_tiktok_ads/__init__.py` & `tap-tiktok-ads-1.0.0/tap_tiktok_ads/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import singer
 from singer import utils
 
 from tap_tiktok_ads.client import TikTokClient
 from tap_tiktok_ads.discover import discover
 from tap_tiktok_ads.sync import sync
 
-REQUIRED_CONFIG_KEYS = ['start_date', 'user_agent', 'access_token', 'accounts']
+REQUIRED_CONFIG_KEYS = ['start_date', 'access_token', 'accounts']
 LOGGER = singer.get_logger()
 
 
 @utils.handle_top_exception(LOGGER)
 def main():
     # Parse command line arguments
     args = utils.parse_args(REQUIRED_CONFIG_KEYS)
@@ -18,24 +18,24 @@
     # get comma-separated string of accounts
     accounts = args.config['accounts'].replace(" ", "")
     # raise error if no accounts is passed
     if not accounts:
         raise Exception("Please provide atleast 1 Account ID.")
     try:
         # create list of accounts
-        accounts_list = [int(i) for i in accounts.split(",")]
+        # typecasting account to determine string is an integer
+        accounts_list = [str(int(account)) for account in accounts.split(",")]
     except ValueError:
         raise Exception("Provided list of account IDs contains invalid IDs. Kindly check your Account IDs.") from None
     # update string to list in the config
     args.config['accounts'] = accounts_list
 
     with TikTokClient(access_token=args.config['access_token'],
                       advertiser_id=args.config['accounts'],
                       sandbox=args.config.get('sandbox', "false"),
-                      user_agent=args.config['user_agent'],
                       request_timeout=args.config.get('request_timeout')) as tik_tok_client:
 
         # If discover flag was passed, run discovery mode and dump output to stdout
         if args.discover:
             catalog = discover()
             catalog.dump()
         # Otherwise run in sync mode
```

### Comparing `tap-tiktok-ads-0.4.0/tap_tiktok_ads/client.py` & `tap-tiktok-ads-1.0.0/tap_tiktok_ads/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 from urllib.parse import urlencode
 import backoff
-
+import json
 import requests
 import backoff
 import singer
 
 from singer import metrics
 
 # max tries for backoff
 MAX_TRIES = 5
 # default timeout for requests
 REQUEST_TIMEOUT = 300
 
 LOGGER = singer.get_logger()
-
-ENDPOINT_BASE = "https://{api}.tiktok.com/open_api/v1.2"
-TOKEN_URL = 'https://{api}.tiktok.com/open_api/v1.2/user/info'
+ENDPOINT_VERSION = "v1.3"
 
 # pylint: disable=missing-class-docstring
 class TikTokAdsClientError(Exception):
     def __init__(self, message=None, response=None):
         super().__init__(message)
         self.message = message
         self.response = response
 
 def should_retry(e):
     """ Return true if exception is required to retry otherwise return false """
     response = e.response
     error_code = response.json().get("code")
     # Backoff in case of below error codes. Refer doc: https://ads.tiktok.com/marketing_api/docs?rid=xmtaqatxqj8&id=1737172488964097
     # for more information.
-    if error_code in (40200, 40201, 40202, 40700, 50000, 50002):
+    if error_code in (40100, 40200, 40201, 40202, 40700, 50000, 50002):
         return True
     if (type(e) == Exception and type(e.args[0][1]) == ConnectionResetError) or type(e) == ConnectionResetError:
         # Tap raises Exception: ConnectionResetError(104, 'Connection reset by peer').
         return True
 
 class TikTokClient:
     def __init__(self,
@@ -87,15 +85,15 @@
             raise Exception('Error: Missing access_token.')
         headers = {}
         if self.__user_agent:
             headers['User-Agent'] = self.__user_agent
         headers['Access-Token'] = self.__access_token
         headers['Accept'] = 'application/json'
         response = self.__session.get(
-            url='https://{}.tiktok.com/open_api/v1.2/user/info'.format(self.__base_url_prefix),
+            url='https://{}.tiktok.com/open_api/{}/user/info'.format(self.__base_url_prefix, ENDPOINT_VERSION),
             headers=headers,
             timeout=self.__request_timeout)
 
         if response.status_code != 200:
             raise Exception('Error status_code = %s', response.status_code)
         resp = response.json()
         error_code = resp.get('code')
@@ -106,15 +104,15 @@
         # if the check_access_token() succeeds, then check the account access with the account ids provided in config.
         if resp['message'] == 'OK':
             self.__verified = True
             headers = {
                 "Access-Token": self.__access_token
             }
             params = {
-                "advertiser_ids": self.__advertiser_id
+                "advertiser_ids": json.dumps(self.__advertiser_id)
             }
             if self.__base_url_prefix == 'sandbox-ads':
                 return True
             # Call the advertisers API with the account ids to check whether the accounts are valid or not.
             adv_response = self.get(path='advertiser/info/', headers=headers,
                                         params=params)
             return bool(adv_response.get('message') == 'OK')
@@ -131,15 +129,15 @@
                           max_tries=MAX_TRIES,
                           factor=2)
     def request(self, method, url=None, path=None, **kwargs):
         if not self.__verified:
             self.__verified = self.check_access_token()
 
         if not url and self.__base_url is None:
-            self.__base_url = 'https://{}.tiktok.com/open_api/v1.2'.format(self.__base_url_prefix)
+            self.__base_url = 'https://{}.tiktok.com/open_api/{}'.format(self.__base_url_prefix, ENDPOINT_VERSION)
 
         if not url and path:
             url = f'{self.__base_url}/{path}'
         else:
             url = f'{url}/{path}'
 
         if 'endpoint' in kwargs:
```

### Comparing `tap-tiktok-ads-0.4.0/tap_tiktok_ads/discover.py` & `tap-tiktok-ads-1.0.0/tap_tiktok_ads/discover.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights.json` & `tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/ad_insights_by_country.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.903903903903904%*

 * *Differences: {"'properties'": "{'advertiser_id': {'type': {insert: [(1, 'string')], delete: [1]}}, 'ad_id': "*

 * *                 "{'type': {insert: [(1, 'string')], delete: [1]}}, 'adgroup_id': {'type': "*

 * *                 "{insert: [(1, 'string')], delete: [1]}}, 'campaign_id': {'type': {insert: [(1, "*

 * *                 "'string')], delete: [1]}}, 'country_code': OrderedDict([('type', ['null', "*

 * *                 "'string'])]), 'user_action': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'gross_impression […]*

```diff
@@ -1,14 +1,14 @@
 {
     "additionalProperties": false,
     "properties": {
         "ad_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "ad_name": {
             "type": [
                 "null",
                 "string"
             ]
@@ -18,90 +18,102 @@
                 "null",
                 "string"
             ]
         },
         "adgroup_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "adgroup_name": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "advertiser_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "average_video_play": {
+        "bid": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "average_video_play_per_user": {
+        "bid_strategy": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "campaign_id": {
+        "billing_event": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "campaign_name": {
+        "budget": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "clicks": {
+        "call_to_action": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "clicks_on_music_disc": {
+        "campaign_budget": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "comments": {
+        "campaign_dedicate_type": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "conversion": {
+        "campaign_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "campaign_name": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "clicks": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "conversion_rate": {
+        "conversion": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
-        "cost_per_1000_reached": {
+        "conversion_rate": {
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "cost_per_100_reached": {
+        "conversion_rate_v2": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "cost_per_conversion": {
             "type": [
@@ -111,18 +123,18 @@
         },
         "cost_per_result": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "cost_per_secondary_goal_result": {
+        "country_code": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
         "cpc": {
             "type": [
                 "null",
                 "number"
             ]
@@ -141,81 +153,69 @@
         },
         "dpa_target_audience_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "follows": {
+        "gross_impressions": {
             "type": [
                 "null",
-                "integer"
-            ]
-        },
-        "frequency": {
-            "type": [
-                "null",
-                "number"
+                "string"
             ]
         },
         "impressions": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "likes": {
+        "is_smart_creative": {
             "type": [
                 "null",
-                "integer"
+                "boolean"
             ]
         },
         "mobile_app_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "placement": {
+        "objective_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "profile_visits": {
+        "opt_status": {
             "type": [
                 "null",
-                "integer"
-            ]
-        },
-        "profile_visits_rate": {
-            "type": [
-                "null",
-                "number"
+                "string"
             ]
         },
         "promotion_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "reach": {
+        "real_time_conversion": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "real_time_conversion": {
+        "real_time_conversion_rate": {
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
-        "real_time_conversion_rate": {
+        "real_time_conversion_rate_v2": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "real_time_cost_per_conversion": {
             "type": [
@@ -249,36 +249,36 @@
         },
         "result_rate": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "secondary_goal_result": {
+        "rf_campaign_type": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "secondary_goal_result_rate": {
+        "smart_target": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "shares": {
+        "spend": {
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
-        "spend": {
+        "split_test": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
         "stat_time_day": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
@@ -292,54 +292,18 @@
         },
         "tt_app_name": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "video_play_actions": {
+        "user_action": {
             "type": [
                 "null",
-                "integer"
-            ]
-        },
-        "video_views_p100": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "video_views_p25": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "video_views_p50": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "video_views_p75": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "video_watched_2s": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "video_watched_6s": {
-            "type": [
-                "null",
-                "integer"
+                "string"
             ]
         }
     },
     "type": [
         "null",
         "object"
     ]
```

### Comparing `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights_by_age_and_gender.json` & `tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/campaign_insights_by_province.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9154040404040403%*

 * *Differences: {"'properties'": "{'advertiser_id': {'type': {insert: [(1, 'string')], delete: [1]}}, "*

 * *                 "'campaign_id': {'type': {insert: [(1, 'string')], delete: [1]}}, 'province_id': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'gross_impressions': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'conversion_rate_v2': "*

 * *                 "OrderedDict([('type', ['null', 'number'])]), 'real_time_conversion_rate_v2': "*

 * *                 "OrderedDict([('type', ['null', 'numb […]*

```diff
@@ -1,56 +1,32 @@
 {
     "additionalProperties": false,
     "properties": {
-        "ad_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "ad_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "ad_text": {
+        "advertiser_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "adgroup_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "adgroup_name": {
+        "campaign_budget": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "advertiser_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "age": {
+        "campaign_dedicate_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "campaign_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "campaign_name": {
             "type": [
                 "null",
                 "string"
             ]
@@ -69,14 +45,20 @@
         },
         "conversion_rate": {
             "type": [
                 "null",
                 "number"
             ]
         },
+        "conversion_rate_v2": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "cost_per_conversion": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "cost_per_result": {
@@ -99,39 +81,33 @@
         },
         "ctr": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "dpa_target_audience_type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "gender": {
+        "gross_impressions": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "impressions": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "mobile_app_id": {
+        "objective_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "promotion_type": {
+        "province_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "real_time_conversion": {
             "type": [
@@ -141,14 +117,20 @@
         },
         "real_time_conversion_rate": {
             "type": [
                 "null",
                 "number"
             ]
         },
+        "real_time_conversion_rate_v2": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "real_time_cost_per_conversion": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "real_time_cost_per_result": {
@@ -177,40 +159,34 @@
         },
         "result_rate": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "spend": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "stat_time_day": {
-            "format": "date-time",
+        "rf_campaign_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "tt_app_id": {
+        "spend": {
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "tt_app_name": {
+        "split_test": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "user_action": {
+        "stat_time_day": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": [
```

### Comparing `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights_by_country.json` & `tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/ad_insights_by_platform.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9389978213507625%*

 * *Differences: {"'properties'": "{'advertiser_id': {'type': {insert: [(1, 'string')], delete: [1]}}, 'ad_id': "*

 * *                 "{'type': {insert: [(1, 'string')], delete: [1]}}, 'adgroup_id': {'type': "*

 * *                 "{insert: [(1, 'string')], delete: [1]}}, 'campaign_id': {'type': {insert: [(1, "*

 * *                 "'string')], delete: [1]}}, 'platform': OrderedDict([('type', ['null', "*

 * *                 "'string'])]), 'gross_impressions': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'is_smart_creat […]*

```diff
@@ -1,14 +1,14 @@
 {
     "additionalProperties": false,
     "properties": {
         "ad_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "ad_name": {
             "type": [
                 "null",
                 "string"
             ]
@@ -18,33 +18,75 @@
                 "null",
                 "string"
             ]
         },
         "adgroup_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "adgroup_name": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "advertiser_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
+            ]
+        },
+        "bid": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "bid_strategy": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "billing_event": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "budget": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "call_to_action": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "campaign_budget": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "campaign_dedicate_type": {
+            "type": [
+                "null",
+                "string"
             ]
         },
         "campaign_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "campaign_name": {
             "type": [
                 "null",
                 "string"
             ]
@@ -63,30 +105,30 @@
         },
         "conversion_rate": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "cost_per_conversion": {
+        "conversion_rate_v2": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "cost_per_result": {
+        "cost_per_conversion": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "country_code": {
+        "cost_per_result": {
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
         "cpc": {
             "type": [
                 "null",
                 "number"
             ]
@@ -105,26 +147,56 @@
         },
         "dpa_target_audience_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "gross_impressions": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "impressions": {
             "type": [
                 "null",
                 "integer"
             ]
         },
+        "is_smart_creative": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
         "mobile_app_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "objective_type": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "opt_status": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "platform": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "promotion_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "real_time_conversion": {
@@ -135,14 +207,20 @@
         },
         "real_time_conversion_rate": {
             "type": [
                 "null",
                 "number"
             ]
         },
+        "real_time_conversion_rate_v2": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "real_time_cost_per_conversion": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "real_time_cost_per_result": {
@@ -171,20 +249,38 @@
         },
         "result_rate": {
             "type": [
                 "null",
                 "number"
             ]
         },
+        "rf_campaign_type": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "smart_target": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "spend": {
             "type": [
                 "null",
                 "number"
             ]
         },
+        "split_test": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "stat_time_day": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
```

### Comparing `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights_by_platform.json` & `tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/campaigns.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.841130604288499%*

 * *Differences: {"'properties'": "{'advertiser_id': {'type': {insert: [(1, 'string')], delete: [1]}}, "*

 * *                 "'campaign_id': {'type': {insert: [(1, 'string')], delete: [1]}}, "*

 * *                 "'campaign_type': OrderedDict([('type', ['null', 'string'])]), 'budget': "*

 * *                 "OrderedDict([('type', ['null', 'number'])]), 'budget_mode': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'secondary_status': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'operation_status': […]*

```diff
@@ -1,213 +1,172 @@
 {
     "additionalProperties": false,
     "properties": {
-        "ad_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "ad_name": {
+        "advertiser_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ad_text": {
+        "app_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "adgroup_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "adgroup_name": {
+        "app_promotion_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "advertiser_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "campaign_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "campaign_name": {
+        "bid_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "clicks": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "conversion": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "conversion_rate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "cost_per_conversion": {
+        "budget": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "cost_per_result": {
+        "budget_mode": {
             "type": [
                 "null",
-                "number"
-            ]
-        },
-        "cpc": {
-            "type": [
-                "null",
-                "number"
+                "string"
             ]
         },
-        "cpm": {
+        "budget_optimize_on": {
             "type": [
                 "null",
-                "number"
+                "boolean"
             ]
         },
-        "ctr": {
+        "campaign_app_profile_page_state": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "dpa_target_audience_type": {
+        "campaign_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "impressions": {
+        "campaign_name": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "mobile_app_id": {
+        "campaign_product_source": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "platform": {
+        "campaign_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "promotion_type": {
+        "create_time": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "real_time_conversion": {
+        "current_status": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "real_time_conversion_rate": {
+        "deep_bid_type": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "real_time_cost_per_conversion": {
+        "is_new_structure": {
             "type": [
                 "null",
-                "number"
+                "boolean"
             ]
         },
-        "real_time_cost_per_result": {
+        "is_smart_performance_campaign": {
             "type": [
                 "null",
-                "number"
+                "boolean"
             ]
         },
-        "real_time_result": {
+        "modify_time": {
+            "format": "date-time",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "real_time_result_rate": {
+        "objective": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "result": {
+        "objective_type": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "result_rate": {
+        "operation_status": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "spend": {
+        "optimization_goal": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "stat_time_day": {
-            "format": "date-time",
+        "rf_campaign_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "tt_app_id": {
+        "roas_bid": {
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "tt_app_name": {
+        "secondary_status": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "user_action": {
+        "special_industries": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         }
     },
     "type": [
         "null",
         "object"
     ]
```

### Comparing `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/adgroups.json` & `tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/adgroups.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9087475633528266%*

 * *Differences: {"'properties'": "{'advertiser_id': {'type': {insert: [(1, 'string')], delete: [1]}}, "*

 * *                 "'adgroup_id': {'type': {insert: [(1, 'string')], delete: [1]}}, 'campaign_id': "*

 * *                 "{'type': {insert: [(1, 'string')], delete: [1]}}, 'app_id': {'type': {insert: "*

 * *                 "[(1, 'string')], delete: [1]}}, 'pixel_id': {'type': {insert: [(1, 'string')], "*

 * *                 "delete: [1]}}, 'skip_learning_phase': {'type': {insert: [(1, 'boolean')], "*

 * *                 "delete: [1]}}, ' […]*

```diff
@@ -1,39 +1,39 @@
 {
     "additionalProperties": false,
     "properties": {
-        "action_v2": {
+        "actions": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
-                    "action_categories": {
+                    "action_category_ids": {
                         "items": {
                             "type": [
                                 "null",
-                                "integer"
+                                "string"
                             ]
                         },
                         "type": [
                             "null",
                             "array"
                         ]
                     },
                     "action_period": {
                         "type": [
                             "null",
-                            "integer"
+                            "number"
                         ]
                     },
                     "action_scene": {
                         "type": [
                             "null",
                             "string"
                         ]
                     },
-                    "user_actions": {
+                    "video_user_actions": {
                         "items": {
                             "type": [
                                 "null",
                                 "string"
                             ]
                         },
                         "type": [
@@ -48,60 +48,60 @@
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
+        "adgroup_app_profile_page_state": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "adgroup_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "adgroup_name": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "advertiser_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "age": {
+        "age_groups": {
             "items": {
                 "type": [
                     "null",
                     "string"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "android_osv": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "app_download_url": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "app_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "audience": {
             "items": {
                 "type": [
                     "null",
                     "integer"
@@ -114,15 +114,15 @@
         },
         "audience_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "bid": {
+        "bid_price": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "bid_type": {
             "type": [
@@ -132,21 +132,21 @@
         },
         "billing_event": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "brand_safety": {
+        "brand_safety_partner": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "brand_safety_partner": {
+        "brand_safety_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "budget": {
             "type": [
@@ -156,30 +156,18 @@
         },
         "budget_mode": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "buy_impression": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "buy_reach": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "campaign_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "carriers_v2": {
             "items": {
                 "type": [
                     "null",
                     "integer"
@@ -195,30 +183,18 @@
                 "null",
                 "integer"
             ]
         },
         "catalog_id": {
             "type": [
                 "null",
-                "integer"
-            ]
-        },
-        "connection_type": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
+                "string"
             ]
         },
-        "conversion_bid": {
+        "conversion_bid_price": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "conversion_window": {
             "type": [
@@ -241,39 +217,39 @@
         },
         "creative_material_mode": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "daily_retention_ratio": {
+        "current_status": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
         "dayparting": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "deep_bid_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "deep_cpabid": {
+        "deep_cpa_bid": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "deep_external_action": {
+        "delivery_mode": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "device_models": {
             "items": {
@@ -283,60 +259,63 @@
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "device_price": {
+        "device_price_ranges": {
             "items": {
                 "type": [
                     "null",
-                    "integer"
+                    "number"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "dpa_retargeting_type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "enable_inventory_filter": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
         "excluded_audience": {
             "items": {
                 "type": [
                     "null",
                     "integer"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "external_action": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "external_type": {
+        "excluded_custom_actions": {
+            "items": {
+                "additionalProperties": false,
+                "properties": {
+                    "code": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "days": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
         "frequency": {
             "type": [
                 "null",
                 "integer"
             ]
@@ -349,14 +328,41 @@
         },
         "gender": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "included_custom_actions": {
+            "items": {
+                "additionalProperties": false,
+                "properties": {
+                    "code": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "days": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
         "interest_category_v2": {
             "items": {
                 "type": [
                     "null",
                     "integer"
                 ]
             },
@@ -373,27 +379,27 @@
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "ios_osv": {
+        "inventory_filter_enabled": {
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "ios_quota_type": {
+        "ios14_targeting": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ios_target_device": {
+        "ios_quota_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "is_comment_disable": {
             "type": [
@@ -409,20 +415,14 @@
         },
         "is_new_structure": {
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "is_share_disable": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
         "languages": {
             "items": {
                 "type": [
                     "null",
                     "string"
                 ]
             },
@@ -439,40 +439,76 @@
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
+        "min_android_version": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "min_ios_version": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "modify_time": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "operation_system": {
+        "network_types": {
             "items": {
                 "type": [
                     "null",
                     "string"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "opt_status": {
+        "next_day_retention": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "operating_systems": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "operation_status": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "optimize_goal": {
+        "optimization_event": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "optimization_goal": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "pacing": {
             "type": [
@@ -521,63 +557,81 @@
                 "null",
                 "array"
             ]
         },
         "pixel_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
+            ]
+        },
+        "placement_type": {
+            "type": [
+                "null",
+                "string"
             ]
         },
-        "placement": {
+        "placements": {
             "items": {
                 "type": [
                     "null",
                     "string"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "placement_type": {
+        "product_set_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "product_set_id": {
+        "promotion_type": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "promotion_website_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "rf_buy_type": {
+        "purchased_impression": {
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "rf_predict_cpr": {
+        "purchased_reach": {
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
-        "rf_predict_frequency": {
+        "rf_estimated_cpr": {
             "type": [
                 "null",
-                "integer"
+                "number"
+            ]
+        },
+        "rf_estimated_frequency": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "rf_purchased_type": {
+            "type": [
+                "null",
+                "string"
             ]
         },
         "roas_bid": {
             "type": [
                 "null",
                 "number"
             ]
@@ -598,35 +652,53 @@
         },
         "schedule_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "skip_learning_phase": {
+        "secondary_optimization_event": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "statistic_type": {
+        "secondary_status": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "share_disabled": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "shopping_ads_retargeting_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "status": {
+        "skip_learning_phase": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "statistic_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "targeting_expansion": {
             "properties": {
-                "enable_expansion": {
+                "expansion_enabled": {
                     "type": [
                         "null",
                         "boolean"
                     ]
                 },
                 "expansion_types": {
                     "items": {
```

### Comparing `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ads.json` & `tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/ad_insights_by_age_and_gender.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8523035230352303%*

 * *Differences: {"'properties'": "{'advertiser_id': {'type': {insert: [(1, 'string')], delete: [1]}}, "*

 * *                 "'campaign_id': {'type': {insert: [(1, 'string')], delete: [1]}}, 'adgroup_id': "*

 * *                 "{'type': {insert: [(1, 'string')], delete: [1]}}, 'ad_id': {'type': {insert: "*

 * *                 "[(1, 'string')], delete: [1]}}, 'stat_time_day': OrderedDict([('type', ['null', "*

 * *                 "'string']), ('format', 'date-time')]), 'age': OrderedDict([('type', ['null', "*

 * *                 "'string'])]), […]*

```diff
@@ -1,20 +1,14 @@
 {
     "additionalProperties": false,
     "properties": {
-        "ad_format": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "ad_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "ad_name": {
             "type": [
                 "null",
                 "string"
             ]
@@ -24,236 +18,295 @@
                 "null",
                 "string"
             ]
         },
         "adgroup_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "adgroup_name": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "advertiser_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "app_name": {
+        "age": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "call_to_action": {
+        "bid": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "campaign_id": {
+        "bid_strategy": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "campaign_name": {
+        "billing_event": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "card_id": {
+        "budget": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "click_tracking_url": {
+        "call_to_action": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "create_time": {
-            "format": "date-time",
+        "campaign_budget": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "display_name": {
+        "campaign_dedicate_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "dpa_fallback_type": {
+        "campaign_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "dpa_open_url_type": {
+        "campaign_name": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "dpa_video_tpl_id": {
+        "clicks": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "fallback_type": {
+        "conversion": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "image_ids": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
+        "conversion_rate": {
             "type": [
                 "null",
-                "array"
+                "number"
             ]
         },
-        "image_mode": {
+        "conversion_rate_v2": {
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "impression_tracking_url": {
+        "cost_per_conversion": {
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "is_aco": {
+        "cost_per_result": {
             "type": [
                 "null",
-                "boolean"
+                "number"
             ]
         },
-        "is_creative_authorized": {
+        "cpc": {
             "type": [
                 "null",
-                "boolean"
+                "number"
             ]
         },
-        "is_new_structure": {
+        "cpm": {
             "type": [
                 "null",
-                "boolean"
+                "number"
             ]
         },
-        "item_duet_status": {
+        "ctr": {
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "item_stitch_status": {
+        "dpa_target_audience_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "landing_page_url": {
+        "gender": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "landing_page_urls": {
+        "gross_impressions": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "modify_time": {
-            "format": "date-time",
+        "impressions": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "open_url": {
+        "is_smart_creative": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "mobile_app_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "open_url_type": {
+        "objective_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "opt_status": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "page_id": {
+        "promotion_type": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "real_time_conversion": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "real_time_conversion_rate": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "real_time_conversion_rate_v2": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "real_time_cost_per_conversion": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "real_time_cost_per_result": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "real_time_result": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "playable_url": {
+        "real_time_result_rate": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "result": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "result_rate": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "rf_campaign_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "profile_image": {
+        "smart_target": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "promotional_music_disabled": {
+        "spend": {
             "type": [
                 "null",
-                "boolean"
+                "number"
             ]
         },
-        "status": {
+        "split_test": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "tiktok_item_id": {
+        "stat_time_day": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "vast_moat": {
+        "tt_app_id": {
             "type": [
                 "null",
-                "boolean"
+                "string"
+            ]
+        },
+        "tt_app_name": {
+            "type": [
+                "null",
+                "string"
             ]
         },
-        "video_id": {
+        "user_action": {
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": [
```

### Comparing `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/advertisers.json` & `tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas/advertisers.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9482758620689656%*

 * *Differences: {"'properties'": "{'advertiser_id': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'cellphone_number': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'rejection_reason': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'telephone_number': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'advertiser_account_type': OrderedDict([('type', ['null', 'string'])]), delete: "*

 * *                 "['id', 'phonenumber', 'reason', 'telephone']}"}*

```diff
@@ -3,20 +3,38 @@
     "properties": {
         "address": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "advertiser_account_type": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "advertiser_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "balance": {
             "type": [
                 "null",
                 "number"
             ]
         },
+        "cellphone_number": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "company": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "contacter": {
@@ -51,20 +69,14 @@
         },
         "email": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "industry": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "language": {
@@ -87,20 +99,14 @@
         },
         "name": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "phonenumber": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "promotion_area": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "promotion_center_city": {
@@ -111,15 +117,15 @@
         },
         "promotion_center_province": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "reason": {
+        "rejection_reason": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "role": {
             "type": [
@@ -129,15 +135,15 @@
         },
         "status": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "telephone": {
+        "telephone_number": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "timezone": {
             "type": [
```

### Comparing `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas.py` & `tap-tiktok-ads-1.0.0/tap_tiktok_ads/schemas.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.4.0/tap_tiktok_ads/streams.py` & `tap-tiktok-ads-1.0.0/tap_tiktok_ads/streams.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from datetime import timedelta, datetime, timezone
-
+import json
 import singer
 from dateutil.parser import parse
 from singer.utils import now
 from singer import utils, Transformer, UNIX_MILLISECONDS_INTEGER_DATETIME_PARSING, metadata
 
 from tap_tiktok_ads.client import TikTokClient
 
 LOGGER = singer.get_logger()
 
-AUCTION_FIELDS = """[
+AUCTION_FIELDS = [
     "ad_name",
     "ad_text",
     "adgroup_id",
     "adgroup_name",
     "campaign_id",
     "campaign_name",
-    "placement",
+    "placement_type",
     "spend",
     "cpc",
     "cpm",
     "impressions",
     "clicks",
     "ctr",
     "reach",
@@ -57,22 +57,33 @@
     "shares",
     "follows",
     "clicks_on_music_disc",
     "tt_app_id",
     "tt_app_name",
     "mobile_app_id",
     "promotion_type",
-    "dpa_target_audience_type"
-]"""
-AUDIENCE_FIELDS = """[
-    "ad_name",
-    "ad_text",
-    "adgroup_id",
-    "adgroup_name",
-    "campaign_id",
+    "dpa_target_audience_type",
+    "gross_impressions",
+    "is_smart_creative",
+    "conversion_rate_v2",
+    "real_time_conversion_rate_v2",
+    "app_promotion_type",
+    "split_test",
+    "campaign_budget",
+    "campaign_dedicate_type",
+    "opt_status",
+    "budget",
+    "smart_target",
+    "bid_strategy",
+    "bid",
+    "call_to_action",
+    "image_mode",
+    "billing_event"
+]
+AUDIENCE_FIELDS = [
     "campaign_name",
     "spend",
     "cpc",
     "cpm",
     "impressions",
     "clicks",
     "ctr",
@@ -84,33 +95,58 @@
     "real_time_conversion_rate",
     "result",
     "cost_per_result",
     "result_rate",
     "real_time_result",
     "real_time_cost_per_result",
     "real_time_result_rate",
+    "gross_impressions",
+    "conversion_rate_v2",
+    "real_time_conversion_rate_v2",
+    "rf_campaign_type",
+    "objective_type",
+    "split_test",
+    "campaign_budget",
+    "campaign_dedicate_type"
+]
+AD_AUDIENCE_FIELDS = [
+    "ad_name",
+    "ad_text",
+    "adgroup_id",
+    "adgroup_name",
+    "campaign_id",
+    "billing_event",
+    "dpa_target_audience_type",
+    "is_smart_creative",
+    "mobile_app_id",
+    "promotion_type",
     "tt_app_id",
     "tt_app_name",
-    "mobile_app_id",
+    "opt_status",
+    "budget",
+    "smart_target",
+    "bid_strategy",
+    "bid",
+    "call_to_action",
     "promotion_type",
-    "dpa_target_audience_type"
-]"""
+]
 ENDPOINT_ADVERTISERS = [
     'advertisers'
 ]
 ENDPOINT_AD_MANAGEMENT = [
     'campaigns',
     'adgroups',
     'ads'
 ]
 ENDPOINT_INSIGHTS = [
     'ad_insights',
     'ad_insights_by_age_and_gender',
     'ad_insights_by_country',
-    'ad_insights_by_platform'
+    'ad_insights_by_platform',
+    'campaign_insights_by_province'
 ]
 
 def get_date_batches(start_date, end_date):
     """
         Returns batches with start_date and end_date for the date_windowing from the provided start_date and end_date
     """
     date_batches = []
@@ -159,14 +195,17 @@
 
 def transform_ad_management_records(records, bookmark_value):
     """
         Transforms records for ad_management streams before writing to output
     """
     transformed_records = []
     for record in records:
+        # Setting the custom 'current_status' as 'ACTIVE', Tiktok does not differentiate between ACTIVE/DELETE records in response.
+        if "current_status" not in record:
+            record["current_status"] = "ACTIVE"
         if 'modify_time' not in record:
             record['modify_time'] = record['create_time']
         # In case of an adgroup request, transform 'is_comment_disabled' type from integer to boolean
         if 'is_comment_disable' in record:
             record['is_comment_disable'] = bool(record['is_comment_disable'] == 0)
         # The `modify_time` format is different that the bookmark_value format(which is currently in TZ format),
         # hence resulted into falsy comparision. Thus, converted both to same formats.
@@ -270,15 +309,16 @@
         bookmark_data = self.get_bookmark(stream.tap_stream_id)
         bookmark_value = get_bookmark_value(stream.tap_stream_id, bookmark_data, advertiser_id, self.config['start_date'])
         transformed_records = pre_transform(stream.tap_stream_id, records, bookmark_value)
         sorted_records = sorted(transformed_records, key=lambda x: x[bookmark_column])
         for record in sorted_records:
             with Transformer(integer_datetime_fmt=UNIX_MILLISECONDS_INTEGER_DATETIME_PARSING) as transformer:
                 # for 'insights' stream, 'advertiser_id' is not getting populated and it is one for the Primary Keys
-                record['advertiser_id'] = advertiser_id
+                if not isinstance(record.get("advertiser_id"), str):
+                    record['advertiser_id'] = advertiser_id
                 transformed_record = transformer.transform(record, stream.schema.to_dict(),
                                                            metadata.to_map(stream.metadata))
                 # write one or more rows to the stream:
                 singer.write_record(stream.tap_stream_id, transformed_record)
                 if bookmark_column:
                     # update bookmark to latest value
                     if stream.tap_stream_id in ENDPOINT_ADVERTISERS:
@@ -306,47 +346,68 @@
             self.params['page'] = page
             response = self.client.get(path=self.path, headers=headers,
                                          params=self.params)
             if response['message'] == 'OK':
                 total_records = response['data']['page_info']['total_number']
                 records = records + response['data']['list']
             page = page + 1
+
+        # Exclusively query to retrieve the deleted records for streams - Ads, AdGroups and Campaigns
+        if stream.tap_stream_id in ENDPOINT_AD_MANAGEMENT and str(self.config.get('include_deleted') or "false").lower() == "true":
+            LOGGER.info(f"Fetching the deleted records for stream - {stream.tap_stream_id}")
+            deleted_records = []
+            total_records = 0
+            page = 1
+            # Add the 'filtering' query param
+            self.params['filtering'] = json.dumps({"primary_status": "STATUS_DELETE"})
+            while (len(deleted_records) < total_records) or (page == 1):
+                self.params['page'] = page
+                response = self.client.get(path=self.path, headers=headers,
+                                            params=self.params)
+                if response['message'] == 'OK':
+                    total_records = response['data']['page_info']['total_number']
+                    deleted_records = deleted_records + response['data']['list']
+                page = page + 1
+            # Setting the custom 'current_status' as 'DELETE', Tiktok does not differentiate between ACTIVE/DELETE records in response.
+            for item in deleted_records:
+                item["current_status"] = "DELETE"
+            records = records + deleted_records
         self.process_batch(stream, records, advertiser_id)
 
     def do_sync(self, stream):
         """ Sync data from tap source """
 
         if 'accounts' in self.config and self.req_advertiser_id:
             advertiser_ids = self.config['accounts']
             for advertiser_id in advertiser_ids:
                 self.params['advertiser_id'] = advertiser_id
                 self.sync_pages(stream)
 
 
 class Advertisers(Stream):
     tap_stream_id = "advertisers"
-    key_properties = ['id', 'create_time']
+    key_properties = ['advertiser_id', 'create_time']
     replication_keys  = ['create_time']
     path = "advertiser/info/"
 
     def sync_advertisers(self, stream):
         """Returns records of advertisers for the processing"""
         headers = {
             "Access-Token": self.config['access_token']
         }
         response = self.client.get(path=self.path, headers=headers,
                                      params=self.params)
         if response['message'] == 'OK':
-            records = response['data']
+            records = response['data']['list']
             self.process_batch(stream, records, None)
 
     def do_sync(self, stream):
         """ Sync data from tap source for advertisers"""
         if 'accounts' in self.config and self.req_advertiser_id:
-            self.params['advertiser_ids'] = self.config['accounts']
+            self.params['advertiser_ids'] = json.dumps(self.config['accounts'])
             self.sync_advertisers(stream)
 
 class Campaigns(Stream):
     tap_stream_id = "campaigns"
     key_properties = ['advertiser_id', 'campaign_id', 'modify_time']
     replication_keys  = ['modify_time']
     path = "campaign/get/"
@@ -381,85 +442,104 @@
                     self.sync_pages(stream)
 
 
 class AdInsights(Insights):
     tap_stream_id = "ad_insights"
     key_properties = ['advertiser_id', 'ad_id', 'adgroup_id', 'campaign_id', 'stat_time_day']
     replication_keys  = ['stat_time_day']
-    path = "reports/integrated/get/"
+    path = "report/integrated/get/"
     params = {
         "service_type": "AUCTION",
         "report_type": "BASIC",
         "data_level": "AUCTION_AD",
         "dimensions": """[
             "ad_id",
             "stat_time_day"
         ]""",
-        "metrics": AUCTION_FIELDS,
-        "lifetime": "false"
+        "metrics": json.dumps(AUCTION_FIELDS),
+        "query_lifetime": "false"
     }
 
 class AdInsightsByAgeAndGender(Insights):
     tap_stream_id = "ad_insights_by_age_and_gender"
     key_properties = ['advertiser_id', 'ad_id', 'adgroup_id', 'campaign_id', 'stat_time_day', 'age', 'gender']
     replication_keys  = ['stat_time_day']
-    path = "reports/integrated/get/"
+    path = "report/integrated/get/"
     params = {
         "service_type": "AUCTION",
         "report_type": "AUDIENCE",
         "data_level": "AUCTION_AD",
         "dimensions": """[
             "ad_id",
             "age",
             "gender",
             "stat_time_day"
         ]""",
-        "metrics": AUDIENCE_FIELDS,
-        "lifetime": "false"
+        "metrics": json.dumps(AUDIENCE_FIELDS + AD_AUDIENCE_FIELDS),
+        "query_lifetime": "false"
     }
 
 class AdInsightsByCountry(Insights):
     tap_stream_id = "ad_insights_by_country"
     key_properties = ['advertiser_id', 'ad_id', 'adgroup_id', 'campaign_id', 'stat_time_day', 'country_code']
     replication_keys  = ['stat_time_day']
-    path = "reports/integrated/get/"
+    path = "report/integrated/get/"
     params = {
         "service_type": "AUCTION",
         "report_type": "AUDIENCE",
         "data_level": "AUCTION_AD",
         "dimensions": """[
             "ad_id",
             "country_code",
             "stat_time_day"
         ]""",
-        "metrics": AUDIENCE_FIELDS,
-        "lifetime": "false"
+        "metrics": json.dumps(AUDIENCE_FIELDS + AD_AUDIENCE_FIELDS),
+        "query_lifetime": "false"
     }
 
 class AdInsightsByPlatform(Insights):
     tap_stream_id = "ad_insights_by_platform"
     key_properties = ['advertiser_id', 'ad_id', 'adgroup_id', 'campaign_id', 'stat_time_day', 'platform']
     replication_keys  = ['stat_time_day']
-    path = "reports/integrated/get/"
+    path = "report/integrated/get/"
     params = {
         "service_type": "AUCTION",
         "report_type": "AUDIENCE",
         "data_level": "AUCTION_AD",
         "dimensions": """[
             "ad_id",
             "platform",
             "stat_time_day"
         ]""",
-        "metrics": AUDIENCE_FIELDS,
+        "metrics": json.dumps(AUDIENCE_FIELDS + AD_AUDIENCE_FIELDS),
+        "query_lifetime": "false"
+    }
+
+class CampaignInsightsByProvince(Insights):
+    tap_stream_id = "campaign_insights_by_province"
+    key_properties = ['advertiser_id', 'campaign_id', 'stat_time_day', 'province_id']
+    replication_keys  = ['stat_time_day']
+    path = "report/integrated/get/"
+    params = {
+        "service_type": "AUCTION",
+        "report_type": "AUDIENCE",
+        "data_level": "AUCTION_CAMPAIGN",
+        "dimensions": """[
+            "campaign_id",
+            "province_id",
+            "stat_time_day"
+        ]""",
+        "metrics": json.dumps(AUDIENCE_FIELDS),
         "lifetime": "false"
     }
 
 STREAMS = {
     'advertisers': Advertisers,
     'campaigns': Campaigns,
     'adgroups': AdGroups,
     'ads': Ads,
     'ad_insights': AdInsights,
     'ad_insights_by_age_and_gender': AdInsightsByAgeAndGender,
     'ad_insights_by_country': AdInsightsByCountry,
-    'ad_insights_by_platform': AdInsightsByPlatform
+    'ad_insights_by_platform': AdInsightsByPlatform,
+    'campaign_insights_by_province': CampaignInsightsByProvince
 }
```

### Comparing `tap-tiktok-ads-0.4.0/tap_tiktok_ads/sync.py` & `tap-tiktok-ads-1.0.0/tap_tiktok_ads/sync.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/SOURCES.txt` & `tap-tiktok-ads-1.0.0/tap_tiktok_ads.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 tap_tiktok_ads/schemas/ad_insights.json
 tap_tiktok_ads/schemas/ad_insights_by_age_and_gender.json
 tap_tiktok_ads/schemas/ad_insights_by_country.json
 tap_tiktok_ads/schemas/ad_insights_by_platform.json
 tap_tiktok_ads/schemas/adgroups.json
 tap_tiktok_ads/schemas/ads.json
 tap_tiktok_ads/schemas/advertisers.json
+tap_tiktok_ads/schemas/campaign_insights_by_province.json
 tap_tiktok_ads/schemas/campaigns.json
 tests/test_all_fields.py
 tests/test_automatic_fields.py
 tests/test_bookmarks.py
 tests/test_discovery.py
 tests/test_interrupted_sync.py
 tests/test_pagination.py
```

### Comparing `tap-tiktok-ads-0.4.0/tests/test_all_fields.py` & `tap-tiktok-ads-1.0.0/tests/test_all_fields.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,50 @@
 from base import TiktokBase
 
 class TiktokAllFieldsTest(TiktokBase):
 
     # fields which is data is not generated
     fields_to_remove = {
         'campaigns': [
-            'status'
+            'status',
+            'app_promotion_type',
+            'special_industries',
+            'secondary_status',
+            'app_id',
+            'campaign_app_profile_page_state',
+            'rf_campaign_type',
+            'campaign_product_source'
             ],
         'ads': [
             'dpa_fallback_type',
             'image_mode',
             'item_stitch_status',
             'dpa_open_url_type',
             'dpa_video_tpl_id',
             'item_duet_status',
             'tiktok_item_id',
             'status',
-            'promotional_music_disabled'],
+            'promotional_music_disabled',
+            'sku_ids',
+            'shopping_ads_fallback_type',
+            'utm_params',
+            'product_set_id',
+            'showcase_products',
+            'shopping_ads_video_package_id',
+            'shopping_deeplink_type',
+            'product_specific_type',
+            'dynamic_destination',
+            'catalog_id',
+            'dynamic_format',
+            'tracking_offline_event_set_ids',
+            'secondary_status',
+            'item_group_ids',
+            'vertical_video_strategy',
+            'tracking_app_id',
+            'carousel_image_index'],
         'adgroups': [
             'cpv_video_duration',
             'targeting_expansion',
             'product_set_id',
             'package',
             'ios_osv',
             'audience_type',
@@ -34,15 +58,27 @@
             'status',
             'pangle_audience_package_include',
             'promotion_website_type',
             'ios_quota_type',
             'android_osv',
             'roas_bid',
             'device_models',
-            'carriers_v2'
+            'carriers_v2',
+            'video_download',
+            'interest_category_v2',
+            'is_comment_disable',
+            'shopping_ads_retargeting_type',
+            'excluded_audience',
+            'min_ios_version',
+            'ios14_targeting',
+            'secondary_status',
+            'interest_keywords',
+            'audience',
+            'location',
+            'min_android_version'
             ],
         'ad_insights_by_age_and_gender': ['user_action'],
         'ad_insights_by_platform': ['user_action'],
         'ad_insights_by_country': ['user_action'],
         'ad_insights': ['cost_per_100_reached']
     }
 
@@ -60,15 +96,15 @@
         # instantiate connection
         conn_id = connections.ensure_connection(self)
 
         # run check mode
         found_catalogs = self.run_and_verify_check_mode(conn_id)
 
         # table and field selection
-        self.select_found_catalogs(conn_id, found_catalogs)
+        self.select_found_catalogs(conn_id, found_catalogs, only_streams=expected_streams)
 
         # grab metadata after performing table-and-field selection to set expectations
         stream_to_all_catalog_fields = dict() # used for asserting all fields are replicated
         for catalog in found_catalogs:
             stream_id, stream_name = catalog['stream_id'], catalog['stream_name']
             catalog_entry = menagerie.get_annotated_schema(conn_id, stream_id)
             fields_from_field_level_md = [md_entry['breadcrumb'][1] for md_entry in catalog_entry['metadata']
@@ -107,10 +143,11 @@
                 # verify all fields for a stream were replicated
                 self.assertGreater(len(expected_all_keys), len(expected_automatic_keys))
                 self.assertTrue(expected_automatic_keys.issubset(expected_all_keys), msg=f'{expected_automatic_keys-expected_all_keys} is not in "expected_all_keys"')
 
                 # remove some fields as data cannot be generated / retrieved
                 fields = self.fields_to_remove.get(stream) or []
                 for field in fields:
-                    expected_all_keys.remove(field)
+                    if field in expected_all_keys:
+                        expected_all_keys.remove(field)
 
                 self.assertSetEqual(expected_all_keys, actual_all_keys)
```

### Comparing `tap-tiktok-ads-0.4.0/tests/test_automatic_fields.py` & `tap-tiktok-ads-1.0.0/tests/test_automatic_fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         conn_id = connections.ensure_connection(self)
         expected_streams = self.expected_streams() -  self.unsupported_streams
 
         # run check mode
         found_catalogs = self.run_and_verify_check_mode(conn_id)
 
         # de-select all the fields
-        self.select_found_catalogs(conn_id, found_catalogs, deselect_all_fields=True)
+        self.select_found_catalogs(conn_id, found_catalogs, deselect_all_fields=True, only_streams=expected_streams)
 
         # run sync
         record_count_by_stream = self.run_and_verify_sync(conn_id)
         synced_records = runner.get_records_from_target_output()
 
         for stream in expected_streams:
             with self.subTest(stream=stream):
```

### Comparing `tap-tiktok-ads-0.4.0/tests/test_bookmarks.py` & `tap-tiktok-ads-1.0.0/tests/test_bookmarks.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         conn_id = connections.ensure_connection(self)
         runner.run_check_mode(self, conn_id)
 
         expected_streams = self.expected_streams()  - self.unsupported_streams
 
         found_catalogs = self.run_and_verify_check_mode(conn_id)
-        self.select_found_catalogs(conn_id, found_catalogs)
+        self.select_found_catalogs(conn_id, found_catalogs, only_streams=expected_streams)
 
         # Run a sync job using orchestrator
         first_sync_record_count = self.run_and_verify_sync(conn_id)
         first_sync_records = runner.get_records_from_target_output()
         first_sync_bookmarks = menagerie.get_state(conn_id)
 
         ##########################################################################
```

### Comparing `tap-tiktok-ads-0.4.0/tests/test_discovery.py` & `tap-tiktok-ads-1.0.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.4.0/tests/test_interrupted_sync.py` & `tap-tiktok-ads-1.0.0/tests/test_interrupted_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         # Run check mode
         found_catalogs = self.run_and_verify_check_mode(conn_id)
 
         # Select only the expected streams tables
         catalog_entries = [ce for ce in found_catalogs if ce["tap_stream_id"] in expected_streams]
 
         # Catalog selection
-        self.select_found_catalogs(conn_id, catalog_entries)
+        self.select_found_catalogs(conn_id, catalog_entries, only_streams=expected_streams)
 
         # Run a sync job
         self.run_and_verify_sync(conn_id)
         first_full_sync = runner.get_records_from_target_output()
 
         first_full_sync_state = menagerie.get_state(conn_id)
```

### Comparing `tap-tiktok-ads-0.4.0/tests/test_pagination.py` & `tap-tiktok-ads-1.0.0/tests/test_pagination.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,16 @@
         """
         Testing that the pagination works when there are records greater than the page size
         - Verify for each stream you can get multiple pages of data
         - Verify by pks that the data replicated matches the data we expect.
         """
 
         # 'advertisers' records depends on the number of accounts passed for syncing
-        expected_streams = self.expected_streams() - self.unsupported_streams
+        # 'campaign_insights_by_province' has some API side issue. Returns 0 records for page size - 25
+        expected_streams = self.expected_streams() - self.unsupported_streams - {"campaign_insights_by_province"}
         conn_id = connections.ensure_connection(self)
 
         # Select all streams and all fields within streams
         found_catalogs = self.run_and_verify_check_mode(conn_id)
 
         self.select_found_catalogs(conn_id, found_catalogs, only_streams=expected_streams)
```

### Comparing `tap-tiktok-ads-0.4.0/tests/test_start_date.py` & `tap-tiktok-ads-1.0.0/tests/test_start_date.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
         self.START_DATE = self.first_start_date
 
         ##########################################################################
         ### First Sync
         ##########################################################################
 
-        expected_streams = self.expected_streams() - { "advertisers", "ad_insights", "ad_insights_by_age_and_gender", "ad_insights_by_country", "ad_insights_by_platform"}
+        expected_streams = self.expected_streams() - self.unsupported_streams - {"campaign_insights_by_province"}
 
         conn_id_1 = connections.ensure_connection(self, original_properties=False)
         runner.run_check_mode(self, conn_id_1)
 
         found_catalogs_1 = self.run_and_verify_check_mode(conn_id_1)
         self.select_found_catalogs(conn_id_1, found_catalogs_1, only_streams=expected_streams)
```

