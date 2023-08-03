# Comparing `tmp/actions_security_analyzer-1.3.5.tar.gz` & `tmp/actions_security_analyzer-1.4.5.tar.gz`

## Comparing `actions_security_analyzer-1.3.5.tar` & `actions_security_analyzer-1.4.5.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/__about__.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/action.yml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/colors.py
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/main.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/requirements.txt
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/.github/workflows/asa-scan.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-that-creates-or-approves-pr.yml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-using-configure-aws-creds-non-oidc-auth.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-using-github-cache.yml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-using-self-hosted-runner-in-matrix.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-using-self-hosted-runner-referenced-by-group.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-using-self-hosted-runners.yml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-dangerous-gh-context-variables.yml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-dangerous-gh-variables-2.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-dangerous-gh-variables.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-inline-script.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-pull-request-target.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-unsecure-command-env-var.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-write-all-permissions.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-write-permissions-all-jobs.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/actions/action-with-write-permissions-one-job.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/analyzer/__init__.py
--rw-r--r--   0        0        0    13432 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/analyzer/analyzer.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/analyzer/analyzer_test.py
--rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/images/asa-stdout.png
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/LICENSE
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/README.md
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 actions_security_analyzer-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/__about__.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/action.yml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/colors.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/main.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/.github/workflows/asa-scan.yml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-create-or-approves-pr-using-curl.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-creates-or-approves-pr-using-gh-cli.yml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-creates-or-approves-pr-using-gh-script.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-using-configure-aws-creds-non-oidc-auth.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-using-github-cache.yml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-using-self-hosted-runner-in-matrix.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-using-self-hosted-runner-referenced-by-group.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-using-self-hosted-runners.yml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-with-dangerous-gh-context-variables.yml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-with-dangerous-gh-variables-2.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-with-dangerous-gh-variables.yml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-with-inline-script.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-with-pull-request-target.yml
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-with-remote-script.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-with-unsecure-command-env-var.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-with-write-all-permissions.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-with-write-permissions-all-jobs.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/actions/action-with-write-permissions-one-job.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/analyzer/__init__.py
+-rw-r--r--   0        0        0    15239 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/analyzer/analyzer.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/analyzer/analyzer_test.py
+-rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/images/asa-stdout.png
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/LICENSE
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/README.md
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 actions_security_analyzer-1.4.5/PKG-INFO
```

### Comparing `actions_security_analyzer-1.3.5/action.yml` & `actions_security_analyzer-1.4.5/action.yml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.3.5/colors.py` & `actions_security_analyzer-1.4.5/colors.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.3.5/main.py` & `actions_security_analyzer-1.4.5/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         elif list_checks:
             for i, check in enumerate(analyzer.get_checks(), 1):
                 print(f"{i}. {check[1:]}")
         else:
             errored = True
             print(f"[{Colors.LIGHT_GRAY}INFO{Colors.END}] must provide `--file` or `--dir`")
 
-    except (FileNotFoundError, KeyError, YAMLError) as exception:
+    except Exception as exception:
         errored = True
         print(f"[{Colors.RED}ERROR{Colors.END}] {exception}")
     finally:
         if not no_summary:
             if not errored and not list_checks:
                 if failed_actions:
                     print(
```

### Comparing `actions_security_analyzer-1.3.5/.github/workflows/asa-scan.yml` & `actions_security_analyzer-1.4.5/.github/workflows/asa-scan.yml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.3.5/actions/action-using-configure-aws-creds-non-oidc-auth.yml` & `actions_security_analyzer-1.4.5/actions/action-using-configure-aws-creds-non-oidc-auth.yml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.3.5/analyzer/analyzer.py` & `actions_security_analyzer-1.4.5/analyzer/analyzer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """analyzer.py contains all the INFOic related to analyzing GitHub Actions"""
+from sys import flags
 from colors import Colors
-from re import search
-from pathlib import Path
+from re import search, DOTALL
 
 
 class Analyzer:
     """Analyzer contains all the checks that will run
     against a specified GitHub Action parsed into a Python
     dictionary.
     """
@@ -108,17 +108,23 @@
     def _check_for_allow_unsecure_commands(self) -> bool:
         passed = True
         for job in self.jobs.keys():
             steps = self.jobs[job]["steps"]
             for step in steps:
                 if "env" in step and "ACTIONS_ALLOW_UNSECURE_COMMANDS" in step["env"]:
                     if self.verbose:
-                        print(
-                            f"{Colors.LIGHT_GRAY}INFO{Colors.END} step('{step['name']}') contains dangerous ACTIONS_ALLOW_UNSECURE_COMMANDS environment variable"
-                        )
+                        if "name" in step:
+                            print(
+                                f"{Colors.LIGHT_GRAY}INFO{Colors.END} step('{step['name']}') contains dangerous ACTIONS_ALLOW_UNSECURE_COMMANDS environment variable"
+                            )
+                        else:
+                            print(
+                                f"{Colors.LIGHT_GRAY}INFO{Colors.END} step contains dangerous ACTIONS_ALLOW_UNSECURE_COMMANDS environment variable"
+                            )
+
                     passed = False
                     return passed
         return passed
 
     def _check_for_pull_request_target(self) -> bool:
         passed = True
         event_triggers = self.action["on"]
@@ -128,25 +134,25 @@
         elif type(event_triggers) == str:
             if event_triggers == "pull_request_target":
                 passed = False
         return passed
 
     def _check_for_remote_script(self) -> bool:
         passed = True
-        POTENTIAL_REMOTE_SCRIPT = r"((?<=[^a-zA-Z0-9])(?:https?\:\/\/|[a-zA-Z0-9]{1,}\.{1}|\b)(?:\w{1,}\.{1}){1,5}(?:com|org|edu|gov|uk|net|ca|de|jp|fr|au|us|ru|ch|it|nl|se|no|es|mil|iq|io|ac|ly|sm){1}(?:\/[a-zA-Z0-9]{1,})*)"
+        POTENTIAL_REMOTE_SCRIPT_REGEX = r"((?<=[^a-zA-Z0-9])(?:https?\:\/\/|[a-zA-Z0-9]{1,}\.{1}|\b)(?:\w{1,}\.{1}){1,5}(?:com|org|edu|gov|uk|net|ca|de|jp|fr|au|us|ru|ch|it|nl|se|no|es|mil|iq|io|ac|ly|sm){1}(?:\/[a-zA-Z0-9.]{1,})*)"
         for job in self.jobs.keys():
             steps = self.jobs[job]["steps"]
             for step in steps:
                 if "run" in step:
                     script = step["run"]
-                    variable = search(POTENTIAL_REMOTE_SCRIPT, script)
+                    variable = search(POTENTIAL_REMOTE_SCRIPT_REGEX, script)
                     if variable:
                         if self.verbose:
                             print(
-                                f"{Colors.LIGHT_GRAY}INFO{Colors.END} remote script ('{variable.group()}') being called"
+                                f"{Colors.LIGHT_GRAY}INFO{Colors.END} remote script('{variable.group()}') found in inline script"
                             )
                         passed = False
         return passed
 
     def _check_for_cache_action_usage(self) -> bool:
         passed = True
         CACHE_ACTION_REGEX = r"actions\/cache@(v\d+(\.\d+)?(\.\d+)?|[a-f0-9]{40})"
@@ -256,38 +262,67 @@
             steps = self.jobs[job]["steps"]
             for step in steps:
                 if "uses" in step:
                     action = search(CONFIGURE_AWS_CREDS_ACTION_REGEX, step["uses"])
                     if action:
                         if any(input in non_oidc_inputs for input in step["with"]):
                             if self.verbose:
-                                print(
-                                    f"{Colors.LIGHT_GRAY}INFO{Colors.END} found step('{step['name']}') not using OIDC with `configure-aws-credentials`"
-                                )
+                                if "name" in step:
+                                    print(
+                                        f"{Colors.LIGHT_GRAY}INFO{Colors.END} found step('{step['name']}') not using OIDC with `configure-aws-credentials`"
+                                    )
+                                else:
+                                    print(
+                                        f"{Colors.LIGHT_GRAY}INFO{Colors.END} found step not using OIDC with `configure-aws-credentials`"
+                                    )
                         if passed:
                             passed = False
         return passed
 
     def _check_for_pull_request_create_or_approve(self) -> bool:
         passed = True
-        GH_CLI_PR_APPROVAL_REGEX = f"gh pr (review.*--approve|create.*)"
-        # TODO: add checks for alternatives ways to create/approve pull request
-        # e.g. via curl or github script ('actions/github-script')
+
+        def __print_msg(job: str, step: dict):
+            if self.verbose:
+                if "name" in step:
+                    print(
+                        f"{Colors.LIGHT_GRAY}INFO{Colors.END} job('{job}') has a step('{step['name']}') that creates or approves a pull request"
+                    )
+                else:
+                    print(
+                        f"{Colors.LIGHT_GRAY}INFO{Colors.END} job('{job}') has a step that creates or approves a pull request"
+                    )
+
+        GH_CLI_PR_CREATE_APPROVE_REGEX = r"gh pr (review.*--approve|create.*)"
+        GITHUB_SCRIPT_ACTION_REGEX = r"actions\/github\-script@(v\d+(\.\d+)?(\.\d+)?|[a-f0-9]{40})"
+        GITHUB_SCRIPT_CREATE_APPROVE_PR_REGEX = r".*github\.rest\.pulls\.(create\(.*|reviews\(.*APPROVE.*)"
+        CURL_CREATE_APPROVE_PR_REGEX = (
+            r".*curl.*https:\/\/api\.github\.com\/repos\/[0-9a-zA-Z-._]+\/[0-9a-zA-Z-._]+\/pulls\/[0-9]{1,}\/reviews.*"
+        )
         for job in self.jobs:
             steps = self.jobs[job]["steps"]
             for step in steps:
                 if "run" in step:
                     script = step["run"]
-                    match = search(GH_CLI_PR_APPROVAL_REGEX, script)
+                    match = search(GH_CLI_PR_CREATE_APPROVE_REGEX, script, flags=DOTALL) or search(
+                        CURL_CREATE_APPROVE_PR_REGEX, script, flags=DOTALL
+                    )
                     if match:
-                        if self.verbose:
-                            print(
-                                f"{Colors.LIGHT_GRAY}INFO{Colors.END} job('{job}') has a step('{step['name']}') that creates or approves a pull request"
-                            )
+                        __print_msg(job, step)
+
                         passed = False
+                if "uses" in step:
+                    action = search(GITHUB_SCRIPT_ACTION_REGEX, step["uses"])
+                    if action:
+                        if "script" in step["with"]:
+                            script = step["with"]["script"]
+                            match = search(GITHUB_SCRIPT_CREATE_APPROVE_PR_REGEX, script, flags=DOTALL)
+                            if match:
+                                __print_msg(job, step)
+                                passed = False
         return passed
 
     def get_checks(self) -> list:
         return [*self.checks.keys()]
 
     def run_checks(self, action: dict) -> bool:
         self.action = action
```

### Comparing `actions_security_analyzer-1.3.5/analyzer/analyzer_test.py` & `actions_security_analyzer-1.4.5/analyzer/analyzer_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from analyzer.analyzer import Analyzer
 
 
 @pytest.fixture(name="analyzer")
 def analyzer_fixture():
     """Returns instance of Analyzer class as fixture for pytests"""
-    return Analyzer()
+    return Analyzer(ignore_checks=[])
 
 
 def test_all_checks(analyzer):
     dir_ = Path("./actions")
     for file_ in dir_.iterdir():
         with open(file_, "r", encoding="utf-8") as action:
             action_dict = yaml.safe_load(action)
```

### Comparing `actions_security_analyzer-1.3.5/images/asa-stdout.png` & `actions_security_analyzer-1.4.5/images/asa-stdout.png`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.3.5/.gitignore` & `actions_security_analyzer-1.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.3.5/LICENSE` & `actions_security_analyzer-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.3.5/README.md` & `actions_security_analyzer-1.4.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -86,10 +86,13 @@
 
     - This checks looks for the usage of AWS's `aws-actions/configure-aws-credentials` action and attempts to identify non-OIDC authentication parameters. Non-OIDC authentication types are less secure than OIDC because they require the creation of long-term credentials which can be compromised, however, OIDC tokens are short-lived and are usually scoped to only the permissions that are essential to a workflow and thus help reduce the attack surface.
 
 10. Name: `check_for_pull_request_create_or_approve`, Level: `WARN`
 
     - This check looks for Action that have logic related to creating or improving pull requests. Creating or approving pull requests via automation poses a security risk if sufficient controls aren't in place to protect against malicious code being merged into a repository.
 
+11. Name: `check_for_remote_script`, Level: `WARN`
+
+    - This check looks for a URL in an inline script of a GitHub Action which usually signals the inclusion of a remote script which can be dangerous.
 ### References
 
 - [Security hardening for GitHub Actions](https://docs.github.com/en/actions/security-guides/security-hardening-for-github-actions)
```

### Comparing `actions_security_analyzer-1.3.5/pyproject.toml` & `actions_security_analyzer-1.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.3.5/PKG-INFO` & `actions_security_analyzer-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actions-security-analyzer
-Version: 1.3.5
+Version: 1.4.5
 Summary: Analyze the security posture of one or more GitHub Actions
 Project-URL: Documentation, https://github.com/bin3xish477/asa#readme
 Project-URL: Issues, https://github.com/bin3xish477/asa/issues
 Project-URL: Source, https://github.com/bin3xish477/asa
 Author-email: Alexis Rodriguez <arodriguez99@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -113,10 +113,13 @@
 
     - This checks looks for the usage of AWS's `aws-actions/configure-aws-credentials` action and attempts to identify non-OIDC authentication parameters. Non-OIDC authentication types are less secure than OIDC because they require the creation of long-term credentials which can be compromised, however, OIDC tokens are short-lived and are usually scoped to only the permissions that are essential to a workflow and thus help reduce the attack surface.
 
 10. Name: `check_for_pull_request_create_or_approve`, Level: `WARN`
 
     - This check looks for Action that have logic related to creating or improving pull requests. Creating or approving pull requests via automation poses a security risk if sufficient controls aren't in place to protect against malicious code being merged into a repository.
 
+11. Name: `check_for_remote_script`, Level: `WARN`
+
+    - This check looks for a URL in an inline script of a GitHub Action which usually signals the inclusion of a remote script which can be dangerous.
 ### References
 
 - [Security hardening for GitHub Actions](https://docs.github.com/en/actions/security-guides/security-hardening-for-github-actions)
```

