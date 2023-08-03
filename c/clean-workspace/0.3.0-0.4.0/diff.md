# Comparing `tmp/clean_workspace-0.3.0.tar.gz` & `tmp/clean_workspace-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_workspace-0.3.0.tar", max compression
+gzip compressed data, was "clean_workspace-0.4.0.tar", max compression
```

## Comparing `clean_workspace-0.3.0.tar` & `clean_workspace-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2023-07-31 16:31:03.677692 clean_workspace-0.3.0/LICENSE
--rw-r--r--   0        0        0     2387 2023-07-31 16:31:03.761129 clean_workspace-0.3.0/README.md
--rw-r--r--   0        0        0     7864 2023-07-31 16:31:03.925908 clean_workspace-0.3.0/clean_workspace/__init__.py
--rw-r--r--   0        0        0      762 2023-07-31 16:35:11.892773 clean_workspace-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 clean_workspace-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-03 13:12:49.214667 clean_workspace-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2696 2023-08-03 13:12:49.215162 clean_workspace-0.4.0/README.md
+-rw-r--r--   0        0        0     9216 2023-08-03 13:12:49.216200 clean_workspace-0.4.0/clean_workspace/__init__.py
+-rw-r--r--   0        0        0      903 2023-08-03 13:14:37.853568 clean_workspace-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3617 1970-01-01 00:00:00.000000 clean_workspace-0.4.0/PKG-INFO
```

### Comparing `clean_workspace-0.3.0/LICENSE` & `clean_workspace-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_workspace-0.3.0/README.md` & `clean_workspace-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,24 @@
 Options:
   --blacklist-domains PATH
   --blacklist-urls PATH
   --tab-description TEXT    Description for tab
   --help                    Show this message and exit.
 ```
 
+### Regex Entries
+
+You can use regex matches in both the url and domain blacklist files. For example, if you want to blacklist all Zoom domains, you can use the following:
+
+```shell
+echo "/.*zoom\.us/" >> ~/.config/clean-workspace/blacklist-domains.txt
+```
+
+A regex entry starts & ends with `/`, like `sed`.
+
 ### Collecting Tab Description Via AppleScript
 
 Here's a quick script you can use to collect a description of what you were working on via applescript:
 
 ```shell
 dialogResult=$(
 osascript <<EOT
```

### Comparing `clean_workspace-0.3.0/pyproject.toml` & `clean_workspace-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "clean-workspace"
-version = "0.3.0"
-description = "Collect all browser URLs, output to terminal, and archive to todoist"
-authors = ["Michael Bianco <mike@mikebian.co>"]
+version = "0.4.0"
+description = "Collect all browser URLs, output to terminal, and archive to todoist. Useful for cleaning up your workspace at the end of the day, without loosing important urls."
+authors = ["Mike Bianco <mike@mikebian.co>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/iloveitaly/clean-workspace"
+keywords = ["todoist", "browser", "productivity"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pyobjc-framework-ScriptingBridge = "^9.0.1"
 todoist-api-python = "^2.0.1"
 python-dotenv = "^1.0.0"
 chrome-bookmarks = "^2020.10.25"
```

### Comparing `clean_workspace-0.3.0/PKG-INFO` & `clean_workspace-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: clean-workspace
-Version: 0.3.0
-Summary: Collect all browser URLs, output to terminal, and archive to todoist
+Version: 0.4.0
+Summary: Collect all browser URLs, output to terminal, and archive to todoist. Useful for cleaning up your workspace at the end of the day, without loosing important urls.
 Home-page: https://github.com/iloveitaly/clean-workspace
 License: MIT
-Author: Michael Bianco
+Keywords: todoist,browser,productivity
+Author: Mike Bianco
 Author-email: mike@mikebian.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chrome-bookmarks (>=2020.10.25,<2021.0.0)
@@ -55,14 +56,24 @@
 Options:
   --blacklist-domains PATH
   --blacklist-urls PATH
   --tab-description TEXT    Description for tab
   --help                    Show this message and exit.
 ```
 
+### Regex Entries
+
+You can use regex matches in both the url and domain blacklist files. For example, if you want to blacklist all Zoom domains, you can use the following:
+
+```shell
+echo "/.*zoom\.us/" >> ~/.config/clean-workspace/blacklist-domains.txt
+```
+
+A regex entry starts & ends with `/`, like `sed`.
+
 ### Collecting Tab Description Via AppleScript
 
 Here's a quick script you can use to collect a description of what you were working on via applescript:
 
 ```shell
 dialogResult=$(
 osascript <<EOT
```

