# Comparing `tmp/modelscan-0.1.1.tar.gz` & `tmp/modelscan-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelscan-0.1.1.tar", max compression
+gzip compressed data, was "modelscan-0.2.0.tar", max compression
```

## Comparing `modelscan-0.1.1.tar` & `modelscan-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    10754 2023-08-01 00:26:57.102215 modelscan-0.1.1/LICENSE
--rw-r--r--   0        0        0     4152 2023-08-01 00:26:57.102215 modelscan-0.1.1/README.md
--rw-r--r--   0        0        0      155 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/__init__.py
--rw-r--r--   0        0        0       22 2023-08-01 00:27:27.294091 modelscan-0.1.1/modelscan/_version.py
--rw-r--r--   0        0        0     2304 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/cli.py
--rw-r--r--   0        0        0      530 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/error.py
--rw-r--r--   0        0        0     2742 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/issues.py
--rw-r--r--   0        0        0      198 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/h5/__init__.py
--rw-r--r--   0        0        0     2308 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/h5/scan.py
--rw-r--r--   0        0        0        0 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/pickle/__init__.py
--rw-r--r--   0        0        0     1963 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/pickle/scan.py
--rw-r--r--   0        0        0        0 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/saved_model/__init__.py
--rw-r--r--   0        0        0     5049 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/saved_model/scan.py
--rw-r--r--   0        0        0      620 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/models/scan.py
--rw-r--r--   0        0        0     4483 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/modelscan.py
--rw-r--r--   0        0        0     2052 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/reports.py
--rw-r--r--   0        0        0     1072 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/tools/LICENSE
--rw-r--r--   0        0        0     9387 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/tools/picklescanner.py
--rw-r--r--   0        0        0     3800 2023-08-01 00:26:57.106216 modelscan-0.1.1/modelscan/tools/utils.py
--rw-r--r--   0        0        0     1276 2023-08-01 00:27:27.762089 modelscan-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 modelscan-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10754 2023-08-03 19:29:16.965765 modelscan-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9520 2023-08-03 19:29:16.965765 modelscan-0.2.0/README.md
+-rw-r--r--   0        0        0      155 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-03 19:29:40.874144 modelscan-0.2.0/modelscan/_version.py
+-rw-r--r--   0        0        0     2308 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/cli.py
+-rw-r--r--   0        0        0      530 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/error.py
+-rw-r--r--   0        0        0     3579 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/issues.py
+-rw-r--r--   0        0        0      198 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/models/h5/__init__.py
+-rw-r--r--   0        0        0     2308 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/models/h5/scan.py
+-rw-r--r--   0        0        0        0 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/models/pickle/__init__.py
+-rw-r--r--   0        0        0     1963 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/models/pickle/scan.py
+-rw-r--r--   0        0        0        0 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/models/saved_model/__init__.py
+-rw-r--r--   0        0        0     5049 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/models/saved_model/scan.py
+-rw-r--r--   0        0        0      620 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/models/scan.py
+-rw-r--r--   0        0        0     4483 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/modelscan.py
+-rw-r--r--   0        0        0     2052 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/reports.py
+-rw-r--r--   0        0        0     1072 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/tools/LICENSE
+-rw-r--r--   0        0        0     9387 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/tools/picklescanner.py
+-rw-r--r--   0        0        0     3800 2023-08-03 19:29:16.985765 modelscan-0.2.0/modelscan/tools/utils.py
+-rw-r--r--   0        0        0     1400 2023-08-03 19:29:41.346152 modelscan-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10556 1970-01-01 00:00:00.000000 modelscan-0.2.0/PKG-INFO
```

### Comparing `modelscan-0.1.1/LICENSE` & `modelscan-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.1/modelscan/cli.py` & `modelscan-0.2.0/modelscan/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 @click.option(
     "-p",
     "--path",
     type=click.Path(exists=True),
     default=None,
     help="Path to the file or folder to scan",
 )
-@click.option(
-    "-u", "--url", type=str, default=None, help="URL to the file or folder to scan"
-)
+# @click.option(
+#     "-u", "--url", type=str, default=None, help="URL to the file or folder to scan"
+# )
 @click.option(
     "-hf",
     "--huggingface",
     type=str,
     default=None,
     help="Name of the Hugging Face model to scan",
 )
@@ -40,15 +40,15 @@
     default="INFO",
     help="level of log messages to display (default: INFO)",
 )
 @click.pass_context
 def cli(
     ctx: click.Context,
     log: str,
-    url: Optional[str],
+    # url: Optional[str],
     huggingface: Optional[str],
     path: Optional[str],
 ) -> int:
     logger.setLevel(logging.INFO)
     logger.addHandler(logging.StreamHandler(stream=sys.stdout))
 
     if log is not None:
@@ -61,21 +61,21 @@
                 pathlibPath = Path().cwd()
             else:
                 pathlibPath = Path(path).absolute()
             if not pathlibPath.exists():
                 raise FileNotFoundError(f"Path {path} does not exist")
             else:
                 modelscan.scan_path(pathlibPath)
-        elif url is not None:
-            modelscan.scan_url(url)
+        # elif url is not None:
+        #     modelscan.scan_url(url)
         elif huggingface is not None:
             modelscan.scan_huggingface_model(huggingface)
         else:
             raise click.UsageError(
-                "Command line must include either a path, a URL, or a Hugging Face model"
+                "Command line must include either a path or a Hugging Face model"
             )
         ConsoleReport.generate(modelscan.issues, modelscan.errors)
         return 0
 
     except click.UsageError as e:
         click.echo(e)
         click.echo(ctx.get_help())
```

### Comparing `modelscan-0.1.1/modelscan/error.py` & `modelscan-0.2.0/modelscan/error.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.1/modelscan/issues.py` & `modelscan-0.2.0/modelscan/reports.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,69 @@
 import abc
 import logging
-from enum import Enum
-from pathlib import Path
-from typing import List, Union, Dict, Optional
+from typing import List, Optional
 
-from collections import defaultdict
-
-logger = logging.getLogger("modelscan")
-
-
-class IssueSeverity(Enum):
-    LOW = 1
-    MEDIUM = 2
-    HIGH = 3
-    CRITICAL = 4
-
-
-class IssueCode(Enum):
-    UNSAFE_OPERATOR = 1
+from rich import print
 
+from modelscan.error import Error
+from modelscan.issues import Issues, IssueSeverity
 
-class IssueDetails(metaclass=abc.ABCMeta):
-    @abc.abstractmethod
-    def output_lines(self) -> List[str]:
-        raise NotImplemented
+logger = logging.getLogger("modelscan")
 
 
-class Issue:
+class Report(metaclass=abc.ABCMeta):
     """
-    Defines properties of a issue
+    Abstract base class for different reporting modules.
     """
 
-    def __init__(
-        self,
-        code: IssueCode,
-        severity: IssueSeverity,
-        details: IssueDetails,
-    ) -> None:
-        """
-        Create a issue with given information
+    def __init__(self) -> None:
+        pass
 
-        :param code: Code of the issue from the issue code enum.
-        :param severity: The severity level of the issue from Severity enum.
-        :param details: An implementation of the IssueDetails object.
+    @staticmethod
+    def generate(
+        issues: Issues,
+        errors: List[Error],
+    ) -> Optional[str]:
         """
-        self.code = code
-        self.severity = severity
-        self.details = details
-
-    def print(self) -> None:
-        issue_description = self.code.name
-        if self.code == IssueCode.UNSAFE_OPERATOR:
-            issue_description = "Unsafe operator"
-        else:
-            logger.error(f"No issue description for issue code ${self.code}")
+        Generate report for the given codebase.
+        Derived classes must provide implementation of this method.
 
-        print(f"\n{issue_description} found:")
-        print(f"  - Severity: {self.severity.name}")
-        for output_line in self.details.output_lines():
-            print(f"  - {output_line}")
+        :param issues: Instance of Issues object
 
+        :param errors: Any errors that occurred during the scan.
+        """
+        raise NotImplemented
 
-class Issues:
-    all_issues: List[Issue]
 
-    def __init__(self, issues: Optional[List[Issue]] = None) -> None:
-        if issues is None:
-            self.all_issues = []
+class ConsoleReport(Report):
+    @staticmethod
+    def generate(
+        issues: Issues,
+        errors: List[Error],
+    ) -> None:
+        issues_by_severity = issues.group_by_severity()
+        print("\n[blue]--- Summary ---")
+        total_issue_count = len(issues.all_issues)
+        if total_issue_count > 0:
+            print(f"\nTotal Issues: {total_issue_count}")
+            print(f"\nTotal Issues By Severity:\n")
+            for severity in IssueSeverity:
+                if severity.name in issues_by_severity:
+                    print(
+                        f"    - {severity.name}: {len(issues_by_severity[severity.name])}"
+                    )
+                else:
+                    print(f"    - {severity.name}: [green]0")
+
+            print("\n[blue]--- Issues by Severity ---")
+            for issue_keys in issues_by_severity.keys():
+                print(f"\n[blue]--- {issue_keys} ---")
+                for issue in issues_by_severity[issue_keys]:
+                    issue.print()
         else:
-            self.all_issues = issues
-
-    def add_issue(self, issue: Issue) -> None:
-        """
-        Add a single issue
-        """
-        self.all_issues.append(issue)
+            print("\n[green] No issues found! 🎉")
 
-    def add_issues(self, issues: List[Issue]) -> None:
-        """
-        Add a list of issues
-        """
-        self.all_issues.extend(issues)
-
-    def group_by_severity(self) -> Dict[str, List[Issue]]:
-        """
-        Group issues by severity.
-        """
-        issues: Dict[str, List[Issue]] = defaultdict(list)
-        for issue in self.all_issues:
-            issues[issue.severity.name].append(issue)
-        return issues
-
-
-class OperatorIssueDetails(IssueDetails):
-    def __init__(self, module: str, operator: str, source: Union[Path, str]) -> None:
-        self.module = module
-        self.operator = operator
-        self.source = source
-
-    def output_lines(self) -> List[str]:
-        return [
-            f"Description: Use of unsafe operator '{self.operator}' from module '{self.module}'",
-            f"Source: {str(self.source)}",
-        ]
+        if len(errors) > 0:
+            print("\n[red]--- Errors --- ")
+            for index, error in enumerate(errors):
+                print(f"\nError {index+1}:")
+                print(str(error))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `modelscan-0.1.1/modelscan/models/h5/scan.py` & `modelscan-0.2.0/modelscan/models/h5/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.1/modelscan/models/pickle/scan.py` & `modelscan-0.2.0/modelscan/models/pickle/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.1/modelscan/models/saved_model/scan.py` & `modelscan-0.2.0/modelscan/models/saved_model/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.1/modelscan/models/scan.py` & `modelscan-0.2.0/modelscan/models/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.1/modelscan/modelscan.py` & `modelscan-0.2.0/modelscan/modelscan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.1/modelscan/tools/LICENSE` & `modelscan-0.2.0/modelscan/tools/LICENSE`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.1/modelscan/tools/picklescanner.py` & `modelscan-0.2.0/modelscan/tools/picklescanner.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.1/modelscan/tools/utils.py` & `modelscan-0.2.0/modelscan/tools/utils.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.1.1/pyproject.toml` & `modelscan-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "modelscan"
-version = "0.1.1"
+version = "0.2.0"
 description = "The modelscan package is a cli tool for detecting unsafe operations in model files across various model serialization formats."
 authors = ["ProtectAI <community@protectai.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{ include = "modelscan" }]
 exclude = ["tests/*", "Makefile"]
 
 [tool.poetry.scripts]
 modelscan = "modelscan.cli:cli"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.12"
 click = "^8.1.3"
 numpy = "1.24.0"
 rich = "^13.4.2"
 h5py = { version = "^3.9.0", optional = true }
 tensorflow = { version = "^2.13.0", optional = true }
 tensorflow-macos = { version = "^2.13.0", platform = "darwin", optional = true }
 
@@ -24,14 +24,18 @@
 tensorflow = ["tensorflow", "tensorflow-macos"]
 h5py = ["h5py"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 bandit = { version = "1.7.5", extras = ["toml"] }
 mypy = "^1.4.1"
+aiohttp = "^3.8.5"
+dill = "^0.3.7"
+pandas = "^2.0.3"
+requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 dunamai = "^1.18.0"
 pre-commit = "^3.3.3"
 black = "^23.7.0"
 
 [tool.poetry.group.prod.dependencies]
@@ -41,8 +45,11 @@
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry-dynamic-versioning]
 enable = true
 
 [tool.bandit]
-exclude_dirs = ["tests"]
+exclude_dirs = ["tests", "notebooks"]
+
+[tool.mypy]
+exclude = ["notebooks"]
```

