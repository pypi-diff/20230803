# Comparing `tmp/ape-ledger-0.6.1.tar.gz` & `tmp/ape-ledger-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-ledger-0.6.1.tar", last modified: Tue Jun 13 17:16:56 2023, max compression
+gzip compressed data, was "ape-ledger-0.6.2.tar", last modified: Thu Aug  3 14:50:00 2023, max compression
```

## Comparing `ape-ledger-0.6.1.tar` & `ape-ledger-0.6.2.tar`

### file list

```diff
@@ -1,53 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:56.562743 ape-ledger-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:56.554743 ape-ledger-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:56.558743 ape-ledger-0.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:56.558743 ape-ledger-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-13 17:16:56.562743 ape-ledger-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:56.558743 ape-ledger-0.6.1/ape_ledger/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/hdpath.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:56.562743 ape-ledger-0.6.1/ape_ledger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 17:16:56.562743 ape-ledger-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:56.562743 ape-ledger-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/tests/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/tests/test_hdpath.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:50:00.928526 ape-ledger-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:50:00.924526 ape-ledger-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:50:00.924526 ape-ledger-0.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:50:00.924526 ape-ledger-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-08-03 14:50:00.928526 ape-ledger-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:50:00.928526 ape-ledger-0.6.2/ape_ledger/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/ape_ledger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/ape_ledger/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/ape_ledger/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/ape_ledger/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/ape_ledger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/ape_ledger/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/ape_ledger/hdpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/ape_ledger/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 14:50:00.000000 ape-ledger-0.6.2/ape_ledger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:50:00.928526 ape-ledger-0.6.2/ape_ledger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-08-03 14:50:00.000000 ape-ledger-0.6.2/ape_ledger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-03 14:50:00.000000 ape-ledger-0.6.2/ape_ledger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:50:00.000000 ape-ledger-0.6.2/ape_ledger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-03 14:50:00.000000 ape-ledger-0.6.2/ape_ledger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:50:00.000000 ape-ledger-0.6.2/ape_ledger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-03 14:50:00.000000 ape-ledger-0.6.2/ape_ledger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 14:50:00.000000 ape-ledger-0.6.2/ape_ledger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-03 14:50:00.932525 ape-ledger-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:50:00.928526 ape-ledger-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/tests/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/tests/test_hdpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-08-03 14:48:21.000000 ape-ledger-0.6.2/tests/test_integration.py
```

### Comparing `ape-ledger-0.6.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-ledger-0.6.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-ledger-0.6.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-ledger-0.6.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/.github/release-drafter.yml` & `ape-ledger-0.6.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/.github/workflows/codeql.yml` & `ape-ledger-0.6.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/.github/workflows/commitlint.yaml` & `ape-ledger-0.6.2/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/.github/workflows/prtitle.yaml` & `ape-ledger-0.6.2/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/.github/workflows/publish.yaml` & `ape-ledger-0.6.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/.github/workflows/stale-prs.yml` & `ape-ledger-0.6.2/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/.github/workflows/test.yaml` & `ape-ledger-0.6.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/.gitignore` & `ape-ledger-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/.pre-commit-config.yaml` & `ape-ledger-0.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/CONTRIBUTING.md` & `ape-ledger-0.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/LICENSE` & `ape-ledger-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/PKG-INFO` & `ape-ledger-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-ledger
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-ledger: Plugin for Ledger Hardware Wallet
 Home-page: https://github.com/ApeWorX/ape-ledger
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-ledger-0.6.1/README.md` & `ape-ledger-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/ape_ledger/_cli.py` & `ape-ledger-0.6.2/ape_ledger/_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-from typing import List
+from typing import List, Tuple, Union
 
 import click
 from ape import accounts
 from ape.cli import (
     ape_cli_context,
     existing_alias_argument,
+    network_option,
     non_existing_alias_argument,
     skip_confirmation_option,
 )
 from eth_account import Account
 from eth_account.messages import encode_defunct
 
 from ape_ledger.accounts import LedgerAccount
 from ape_ledger.choices import AddressPromptChoice
-from ape_ledger.client import connect_to_ethereum_app
 from ape_ledger.exceptions import LedgerSigningError
-from ape_ledger.hdpath import HDBasePath
+from ape_ledger.hdpath import HDAccountPath, HDBasePath
+
+
+def _select_account(hd_path: Union[HDBasePath, str]) -> Tuple[str, HDAccountPath]:
+    choices = AddressPromptChoice(hd_path)
+    return choices.get_user_selected_account()
 
 
 @click.group(short_help="Manage Ledger accounts")
 def cli():
     """
     Manage Ledger hardware device accounts.
     """
@@ -32,15 +37,15 @@
 
     ledger_accounts = _get_ledger_accounts()
 
     if len(ledger_accounts) == 0:
         cli_ctx.logger.warning("No accounts found.")
         return
 
-    num_accounts = len(accounts)
+    num_accounts = len(ledger_accounts)
     header = f"Found {num_accounts} account"
     header += "s:" if num_accounts > 1 else ":"
     click.echo(header)
 
     for account in ledger_accounts:
         alias_display = f" (alias: '{account.alias}')" if account.alias else ""
         hd_path_display = f" (hd-path: '{account.hdpath}')" if account.hdpath else ""
@@ -62,17 +67,15 @@
         "Exclude {x} to append the account ID to the end of the base path."
     ),
     callback=lambda ctx, param, arg: HDBasePath(arg),
 )
 def add(cli_ctx, alias, hd_path):
     """Add an account from your Ledger hardware wallet"""
 
-    app = connect_to_ethereum_app(hd_path)
-    choices = AddressPromptChoice(app)
-    address, account_hd_path = choices.get_user_selected_account()
+    address, account_hd_path = _select_account(hd_path)
     container = accounts.containers.get("ledger")
     container.save_account(alias, address, str(account_hd_path))
     cli_ctx.logger.success(f"Account '{address}' successfully added with alias '{alias}'.")
 
 
 @cli.command()
 @ape_cli_context()
@@ -107,17 +110,31 @@
         cli_ctx.logger.success(f"Account '{account.alias}' has been removed.")
 
 
 @cli.command(short_help="Sign a message with your Ledger device")
 @ape_cli_context()
 @click.argument("alias")
 @click.argument("message", default="Hello World!")
-def sign_message(cli_ctx, alias, message):
+@network_option()
+def sign_message(cli_ctx, alias, message, network):
     """Sign a message using a Ledger account"""
 
+    ctx = None
+    if network:
+        ctx = cli_ctx.network_manager.parse_network_choice(network)
+        ctx.__enter__()
+
+    try:
+        _sign_message(cli_ctx, alias, message)
+    finally:
+        if network and ctx and ctx._provider and ctx._provider.is_connected:
+            ctx.__exit__()
+
+
+def _sign_message(cli_ctx, alias, message):
     if alias not in accounts.aliases:
         cli_ctx.abort(f"Account with alias '{alias}' does not exist.")
 
     eip191message = encode_defunct(text=message)
     account = accounts.load(alias)
     signature = account.sign_message(eip191message)
```

### Comparing `ape-ledger-0.6.1/ape_ledger/accounts.py` & `ape-ledger-0.6.2/ape_ledger/accounts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 import json
 from pathlib import Path
-from typing import Iterator, Optional, Union
+from typing import Dict, Iterator, Optional, Union
 
 import click
-import rlp  # type: ignore
 from ape.api import AccountAPI, AccountContainerAPI, TransactionAPI
 from ape.types import AddressType, MessageSignature, TransactionSignature
-from ape_ethereum.transactions import TransactionType
+from ape_ethereum.transactions import DynamicFeeTransaction, StaticFeeTransaction
 from eth_account.messages import SignableMessage
+from eth_utils import is_0x_prefixed, to_bytes
 from hexbytes import HexBytes
 
-from ape_ledger.client import LedgerEthereumAccountClient, connect_to_ethereum_account
+from ape_ledger.client import LedgerDeviceClient, get_device
 from ape_ledger.exceptions import LedgerSigningError
 from ape_ledger.hdpath import HDAccountPath
-from ape_ledger.objects import DynamicFeeTransaction, StaticFeeTransaction
+
+
+def _to_bytes(val):
+    if val is None:
+        return b""
+    elif isinstance(val, str) and is_0x_prefixed(val):
+        return to_bytes(hexstr=val)
+    elif isinstance(val, str):
+        return to_bytes(text=val)
+    elif isinstance(val, HexBytes):
+        return bytes(val)
+    else:
+        return to_bytes(val)
 
 
 class AccountContainer(AccountContainerAPI):
     @property
     def accounts(self) -> Iterator[AccountAPI]:
         for account_file in self._account_files:
             yield LedgerAccount(container=self, account_file_path=account_file)
@@ -58,71 +70,77 @@
 def _echo_object_to_sign(obj: Union[TransactionAPI, SignableMessage]):
     click.echo(f"{obj}\nPlease follow the prompts on your device.")
 
 
 class LedgerAccount(AccountAPI):
     account_file_path: Path
 
-    # Optional because it's lazily loaded
-    account_client: Optional[LedgerEthereumAccountClient] = None
-
     @property
     def alias(self) -> str:
         return self.account_file_path.stem
 
     @property
+    def _client(self) -> LedgerDeviceClient:
+        return get_device(self.hdpath)
+
+    @property
     def address(self) -> AddressType:
         ecosystem = self.network_manager.get_ecosystem("ethereum")
         return ecosystem.decode_address(self.account_file["address"])
 
     @property
     def hdpath(self) -> HDAccountPath:
         raw_path = self.account_file["hdpath"]
         return HDAccountPath(raw_path)
 
     @property
     def account_file(self) -> dict:
         return json.loads(self.account_file_path.read_text())
 
-    @property
-    def _client(self) -> LedgerEthereumAccountClient:
-        if self.account_client is None:
-            self.account_client = connect_to_ethereum_account(self.address, self.hdpath)
-        return self.account_client
-
     def sign_message(self, msg: SignableMessage) -> Optional[MessageSignature]:
         version = msg.version
         if version == b"E":
             _echo_object_to_sign(msg)
-            signed_msg = self._client.sign_personal_message(msg.body)
+            signed_msg = self._client.sign_message(msg.body)
         elif version == b"\x01":
             _echo_object_to_sign(msg)
-            signed_msg = self._client.sign_typed_data(msg.header, msg.body)
+            header = _to_bytes(msg.header)
+            body = _to_bytes(msg.body)
+            signed_msg = self._client.sign_typed_data(header, body)
         else:
             raise LedgerSigningError(
                 f"Unsupported message-signing specification, (version={version!r})."
             )
 
         v, r, s = signed_msg
-        return MessageSignature(v, r, s)
+        return MessageSignature(v=v, r=HexBytes(r), s=HexBytes(s))
 
     def sign_transaction(self, txn: TransactionAPI, **kwargs) -> Optional[TransactionAPI]:
-        txn_type = TransactionType(txn.type)  # In case it is not enum
-        if txn_type == TransactionType.STATIC:
-            serializable_txn = StaticFeeTransaction(**txn.dict())
-            txn_bytes = rlp.encode(serializable_txn, StaticFeeTransaction)
+        txn.chain_id = 1
+        txn_dict: Dict = {
+            "nonce": txn.nonce,
+            "gas": txn.gas_limit,
+            "amount": txn.value,
+            "data": _to_bytes(txn.data.hex()),
+            "destination": _to_bytes(txn.receiver),
+            "chain_id": txn.chain_id,
+        }
+        if isinstance(txn, StaticFeeTransaction):
+            txn_dict["gas_price"] = txn.gas_price
+
+        elif isinstance(txn, DynamicFeeTransaction):
+            txn_dict["max_fee_per_gas"] = txn.max_fee
+            txn_dict["max_priority_fee_per_gas"] = txn.max_priority_fee
+            if txn.access_list:
+                txn_dict["access_list"] = [[ls.address, ls.storage_keys] for ls in txn.access_list]
+
         else:
-            serializable_txn = DynamicFeeTransaction(**txn.dict())
-            version_byte = bytes(HexBytes(TransactionType.DYNAMIC.value))
-            txn_bytes = version_byte + rlp.encode(serializable_txn, DynamicFeeTransaction)
+            raise TypeError(type(txn))
 
         _echo_object_to_sign(txn)
-        v, r, s = self._client.sign_transaction(txn_bytes)
-
-        chain_id = txn.chain_id
-        # NOTE: EIP-1559 transactions don't pack 'chain_id' with 'v'.
-        if txn_type != TransactionType.DYNAMIC and (chain_id * 2 + 35) + 1 > 255:
-            ecc_parity = v - ((chain_id * 2 + 35) % 256)
-            v = (chain_id * 2 + 35) + ecc_parity
-
-        txn.signature = TransactionSignature(v, r, s)
+        v, r, s = self._client.sign_transaction(txn_dict)
+        txn.signature = TransactionSignature(
+            v=v,
+            r=HexBytes(r),
+            s=HexBytes(s),
+        )
         return txn
```

### Comparing `ape-ledger-0.6.1/ape_ledger/choices.py` & `ape-ledger-0.6.2/ape_ledger/choices.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-from typing import Any, Optional, Tuple
+from typing import Any, Optional, Tuple, Union
 
 import click
 from ape.cli import PromptChoice
 from click import Context, Parameter
 
-from ape_ledger.client import LedgerEthereumAppClient
+from ape_ledger.client import get_device
 from ape_ledger.hdpath import HDAccountPath, HDBasePath
 
 
 class AddressPromptChoice(PromptChoice):
     """
     A class for handling prompting the user for an address selection.
     """
 
     DEFAULT_PAGE_SIZE = 5
 
     def __init__(
         self,
-        app: LedgerEthereumAppClient,
+        hd_path: Union[HDBasePath, str],
         index_offset: int = 0,
         page_size: int = DEFAULT_PAGE_SIZE,
     ):
-        self._app = app
+        if isinstance(hd_path, str):
+            hd_path = HDBasePath(base_path=hd_path)
+
+        self._hd_root_path = hd_path
         self._index_offset = index_offset
         self._page_size = page_size
         self._choice_index = None
 
         # Must call ``_load_choices()`` to set address choices
         super().__init__([])
 
     @property
-    def _hd_root_path(self) -> HDBasePath:
-        """The base HD path of the Ethereum wallet."""
-        return self._app.hd_root_path
-
-    @property
     def _is_incremented(self) -> bool:
         """Returns ``True`` if the user has paged past the first page."""
         return (self._index_offset + self._page_size) > self._page_size
 
     @property
     def _prompt_message(self) -> str:
         return (
@@ -95,11 +93,13 @@
 
     def _load_choices(self):
         end_range = self._index_offset + self._page_size
         index_range = range(self._index_offset, end_range)
         self.choices = [self._get_address(i) for i in index_range]
 
     def _get_address(self, account_id: int) -> str:
-        return str(self._app.load_account(account_id))
+        path = self._hd_root_path.get_account_path(account_id)
+        device = get_device(path)
+        return device.get_address()
 
 
-__all__ = ["AddressPromptChoice", "PromptChoice"]
+__all__ = ["AddressPromptChoice"]
```

### Comparing `ape-ledger-0.6.1/ape_ledger.egg-info/PKG-INFO` & `ape-ledger-0.6.2/ape_ledger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-ledger
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-ledger: Plugin for Ledger Hardware Wallet
 Home-page: https://github.com/ApeWorX/ape-ledger
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-ledger-0.6.1/ape_ledger.egg-info/SOURCES.txt` & `ape-ledger-0.6.2/ape_ledger.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -22,24 +22,22 @@
 ape_ledger/__init__.py
 ape_ledger/_cli.py
 ape_ledger/accounts.py
 ape_ledger/choices.py
 ape_ledger/client.py
 ape_ledger/exceptions.py
 ape_ledger/hdpath.py
-ape_ledger/objects.py
 ape_ledger/py.typed
 ape_ledger/version.py
 ape_ledger.egg-info/PKG-INFO
 ape_ledger.egg-info/SOURCES.txt
 ape_ledger.egg-info/dependency_links.txt
 ape_ledger.egg-info/entry_points.txt
 ape_ledger.egg-info/not-zip-safe
 ape_ledger.egg-info/requires.txt
 ape_ledger.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_accounts.py
 tests/test_choices.py
-tests/test_client.py
 tests/test_hdpath.py
 tests/test_integration.py
```

### Comparing `ape-ledger-0.6.1/ape_ledger.egg-info/requires.txt` & `ape-ledger-0.6.2/ape_ledger.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 click
 eth-ape<0.7,>=0.6.0
-hidapi<0.14,>=0.13.1
+ledgereth<0.9,>=0.8.1
 importlib-metadata
-rlp>=3.0.0
 eth-account
 eth-typing
 eth-utils
 hexbytes
 
 [dev]
 pytest>=6.0
```

### Comparing `ape-ledger-0.6.1/pyproject.toml` & `ape-ledger-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/setup.py` & `ape-ledger-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,16 @@
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-ledger",
     include_package_data=True,
     install_requires=[
         "click",  # Use same version as eth-ape
         "eth-ape>=0.6.0,<0.7",
-        "hidapi>=0.13.1,<0.14",
+        "ledgereth>=0.8.1,<0.9",
         "importlib-metadata",
-        "rlp>=3.0.0",
         # EF Dependencies
         "eth-account",  # Use same version as eth-ape
         "eth-typing",  # Influenced by eth-ape
         "eth-utils",  # Use same version as eth-ape
         "hexbytes",  # Use same version as eth-ape
     ],
     entry_points={
```

### Comparing `ape-ledger-0.6.1/tests/conftest.py` & `ape-ledger-0.6.2/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,123 @@
 import json
 
 import pytest
+from ape import accounts, networks
 from ape.api.accounts import AccountContainerAPI
 from click.testing import CliRunner
-from eth_typing import ChecksumAddress, HexAddress, HexStr
+from eth_account.messages import encode_defunct
+from ethpm_types import HexBytes
+
+from ape_ledger.client import LedgerDeviceClient
 
-from ape_ledger.client import (
-    LedgerEthereumAccountClient,
-    LedgerEthereumAppClient,
-    LedgerUsbDeviceClient,
-)
-from ape_ledger.hdpath import HDAccountPath, HDBasePath
-
-TEST_ADDRESSES = [
-    HexAddress(HexStr("0x0A78AAAAA2122100000b9046f0A085AB2E111113")),
-    HexAddress(HexStr("0x1A78AAAAA2122100000b9046f0A085AB2E111113")),
-    HexAddress(HexStr("0x2A78AAAAA2122100000b9046f0A085AB2E111113")),
-    HexAddress(HexStr("0x3A78AAAAA2122100000b9046f0A085AB2E111113")),
-    HexAddress(HexStr("0x4A78AAAAA2122100000b9046f0A085AB2E111113")),
-    HexAddress(HexStr("0x5A78AAAAA2122100000b9046f0A085AB2E111113")),
-    HexAddress(HexStr("0x6A78AAAAA2122100000b9046f0A085AB2E111113")),
-    HexAddress(HexStr("0x7A78AAAAA2122100000b9046f0A085AB2E111113")),
-    HexAddress(HexStr("0x8A78AAAAA2122100000b9046f0A085AB2E111113")),
-    HexAddress(HexStr("0x9A78AAAAA2122100000b9046f0A085AB2E111113")),
-]
-TEST_ADDRESS = TEST_ADDRESSES[0]
 TEST_ALIAS = "TestAlias"
-TEST_HD_PATH = "m/44'/60'/0'/0/0"
+TEST_HD_PATH = "m/44'/60'/{x}'/0/0"
 
 
 @pytest.fixture
-def mock_apdu(mocker):
-    return mocker.MagicMock()
+def hd_path():
+    return TEST_HD_PATH
 
 
 @pytest.fixture
-def mock_device(mocker):
-    return mocker.MagicMock(spec=LedgerUsbDeviceClient)
+def alias():
+    return TEST_ALIAS
 
 
-def create_test_account(mock_device, address=TEST_ADDRESS):
-    address = ChecksumAddress(address)
-    path = HDAccountPath(TEST_HD_PATH)
-    return LedgerEthereumAccountClient(mock_device, address, path)
+@pytest.fixture
+def test_accounts():
+    return accounts.test_accounts
 
 
 @pytest.fixture
-def ledger_account(mock_device):
-    return create_test_account(mock_device)
+def account_addresses(test_accounts):
+    return [a.address for a in test_accounts]
 
 
 @pytest.fixture
-def mock_ethereum_app(mocker, mock_device):
-    mock = mocker.MagicMock(spec=LedgerEthereumAppClient)
-    mock.hd_root_path = HDBasePath()
+def account_0(test_accounts):
+    return test_accounts[0]
 
-    def _get_address(account_id: int):
-        if len(TEST_ADDRESSES) > account_id >= 0:
-            address = TEST_ADDRESSES[account_id]
-            return create_test_account(mock_device, address=address)
 
-    mock.load_account.side_effect = _get_address
-    return mock
+@pytest.fixture
+def account_1(test_accounts):
+    return test_accounts[0]
+
+
+@pytest.fixture
+def address(account_addresses):
+    return account_addresses[0]
+
+
+@pytest.fixture(autouse=True)
+def connection():
+    with networks.ethereum.local.use_provider("test") as provider:
+        yield provider
+
+
+@pytest.fixture
+def msg_signature(account_0):
+    msg = encode_defunct(text="__TEST_MESSAGE__")
+    sig = account_0.sign_message(msg)
+    return (
+        sig.v,
+        int(HexBytes(sig.r).hex(), 16),
+        int(HexBytes(sig.s).hex(), 16),
+    )
+
+
+@pytest.fixture
+def receipt(account_0, account_1):
+    return account_0.transfer(account_1, "1 gwei")
+
+
+@pytest.fixture
+def tx_signature(receipt):
+    return (
+        receipt.signature.v,
+        int(HexBytes(receipt.signature.r).hex(), 16),
+        int(HexBytes(receipt.signature.s).hex(), 16),
+    )
+
+
+@pytest.fixture(autouse=True)
+def mock_device(mocker, hd_path, account_addresses, msg_signature, tx_signature):
+    device = mocker.MagicMock(spec=LedgerDeviceClient)
+    device._account = hd_path
+    device.get_address.side_effect = (
+        lambda *args, **kwargs: account_addresses[args[0]] if args else account_addresses[0]
+    )
+    device.sign_message.side_effect = lambda *args, **kwargs: msg_signature
+    device.sign_typed_data.side_effect = lambda *args, **kwargs: msg_signature
+    device.sign_transaction.side_effect = lambda *args, **kwargs: tx_signature
+    return device
 
 
 @pytest.fixture
 def mock_container(mocker):
     return mocker.MagicMock(spec=AccountContainerAPI)
 
 
 @pytest.fixture
 def runner():
     return CliRunner()
 
 
-def assert_account(account_path, expected_address=TEST_ADDRESS, expected_hdpath="m/44'/60'/0'/0/0"):
-    with open(account_path) as account_file:
-        account_data = json.load(account_file)
-        assert account_data["address"] == expected_address
-        assert account_data["hdpath"] == expected_hdpath
+@pytest.fixture
+def assert_account(address):
+    def fn(account_path, expected_address=None, expected_hdpath="m/44'/60'/0'/0/0"):
+        expected_address = expected_address or address
+        with open(account_path) as account_file:
+            account_data = json.load(account_file)
+            assert account_data["address"] == expected_address
+            assert account_data["hdpath"] == expected_hdpath
+
+    return fn
+
+
+@pytest.fixture
+def device_factory(mocker, mock_device):
+    def fn(module):
+        patch = mocker.patch(f"ape_ledger.{module}.get_device")
+        patch.return_value = mock_device
+
+    return fn
```

### Comparing `ape-ledger-0.6.1/tests/test_choices.py` & `ape-ledger-0.6.2/tests/test_choices.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+import pytest
+
 from ape_ledger.choices import AddressPromptChoice
 
-from .conftest import TEST_ADDRESS
+
+@pytest.fixture(autouse=True)
+def patch_device(device_factory):
+    return device_factory("choices")
 
 
 class TestAddressPromptChoice:
-    def test_get_user_selected_account(self, mocker, mock_ethereum_app):
+    def test_get_user_selected_account(self, mocker, hd_path, address):
         mock_prompt = mocker.patch("ape_ledger.choices.click.prompt")
-        choices = AddressPromptChoice(mock_ethereum_app)
+        choices = AddressPromptChoice(hd_path)
         choices._choice_index = 3
         choices._index_offset = 2
 
         # `None` means the user hasn't selected yeet
         # And is entering other keys, possible the paging keys.
-        mock_prompt_return_values = iter((None, None, None, None, TEST_ADDRESS, None))
+        mock_prompt_return_values = iter((None, None, None, None, address, None))
 
         def _side_effect(*args, **kwargs):
             return next(mock_prompt_return_values)
 
         mock_prompt.side_effect = _side_effect
         address, hdpath = choices.get_user_selected_account()
-        assert address == TEST_ADDRESS
+        assert address == address
         assert str(hdpath) == f"m/44'/60'/{choices._choice_index + choices._index_offset}'/0/0"
```

### Comparing `ape-ledger-0.6.1/tests/test_hdpath.py` & `ape-ledger-0.6.2/tests/test_hdpath.py`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.1/tests/test_integration.py` & `ape-ledger-0.6.2/tests/test_integration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,126 @@
 import pytest
 from ape import accounts
 from ape._cli import cli
 
 from ape_ledger.hdpath import HDBasePath
 
-from .conftest import TEST_ADDRESS, TEST_HD_PATH, assert_account
-
 
 def _get_container():
     return accounts.containers["ledger"]
 
 
-TEST_ALIAS = "__integration_test_alias__"
-TEST_ACCOUNT_PATH = _get_container().data_folder.joinpath(f"{TEST_ALIAS}.json")
+@pytest.fixture
+def alias():
+    val = "__integration_test_alias__"
+    container = _get_container()
+    if val in [a.alias for a in container.accounts]:
+        container.delete_account(val)
+
+    return val
 
 
 @pytest.fixture
-def mock_device_connection(mocker, mock_ethereum_app):
-    patch = mocker.patch("ape_ledger._cli.connect_to_ethereum_app")
-    patch.return_value = mock_ethereum_app
-    return patch
+def test_account_path(alias):
+    return _get_container().data_folder.joinpath(f"{alias}.json")
 
 
 @pytest.fixture
-def existing_account(runner):
+def existing_account(runner, alias, address, hd_path):
     try:
         container = _get_container()
-        container.save_account(TEST_ALIAS, TEST_ADDRESS, TEST_HD_PATH)
+        container.save_account(alias, address, hd_path)
         yield
     finally:
         _clean_up(runner)
 
 
 @pytest.fixture(autouse=True)
 def clean_after(runner):
     try:
         yield
     finally:
         _clean_up(runner)
 
 
+@pytest.fixture
+def choices(mocker):
+    def fn(addr, account_id):
+        patch = mocker.patch("ape_ledger._cli._select_account")
+
+        def se(hd_path):
+            return addr, HDBasePath(hd_path).get_account_path(account_id)
+
+        patch.side_effect = se
+
+    return fn
+
+
 def _clean_up(runner):
-    runner.invoke(cli, ["ledger", "delete", TEST_ALIAS], input="y")
+    runner.invoke(cli, ["ledger", "delete", alias], input="y")
 
 
-def _get_account_path(alias=TEST_ALIAS):
+def _get_account_path(alias=alias):
     container = _get_container()
     return container.data_folder.joinpath(f"{alias}.json")
 
 
 @pytest.mark.parametrize("cmd", (["ledger", "list"], ["accounts", "list", "--all"]))
-def test_list(runner, existing_account, cmd):
+def test_list(runner, existing_account, cmd, address, alias):
     result = runner.invoke(cli, cmd)
     assert result.exit_code == 0, result.output
-    assert TEST_ALIAS in result.output
-    assert TEST_ADDRESS.lower() in result.output.lower()
+    assert alias in result.output
+    assert address.lower() in result.output.lower()
 
 
-def test_add(runner, mock_device_connection):
-    selected_account_id = 0
-    result = runner.invoke(cli, ["ledger", "add", TEST_ALIAS], input=str(selected_account_id))
+def test_add(runner, assert_account, address, alias, choices, hd_path):
+    container = _get_container()
+    choices(address, 2)
+    result = runner.invoke(cli, ["ledger", "add", alias])
     assert result.exit_code == 0, result.output
-    assert (
-        f"SUCCESS: Account '{TEST_ADDRESS}' successfully added with alias '{TEST_ALIAS}'."
-        in result.output
-    )
+    assert f"SUCCESS: Account '{address}' successfully added with alias '{alias}'." in result.output
 
-    container = _get_container()
-    expected_path = container.data_folder.joinpath(f"{TEST_ALIAS}.json")
-    expected_hd_path = f"m/44'/60'/{selected_account_id}'/0/0"
+    expected_path = container.data_folder.joinpath(f"{alias}.json")
+    expected_hd_path = "m/44'/60'/2'/0/0"
     assert_account(expected_path, expected_hdpath=expected_hd_path)
 
 
-def test_add_when_hd_path_specified(runner, mock_ethereum_app, mock_device_connection):
+def test_add_when_hd_path_specified(runner, alias, address, hd_path, assert_account, choices):
     test_hd_path = "m/44'/60'/0'"
-    mock_ethereum_app.hd_root_path = HDBasePath(test_hd_path)
-
-    selected_account_id = 0
+    container = _get_container()
+    choices(address, 2)
     result = runner.invoke(
         cli,
-        ["ledger", "add", TEST_ALIAS, "--hd-path", test_hd_path],
-        input=str(selected_account_id),
+        ["ledger", "add", alias, "--hd-path", test_hd_path],
     )
     assert result.exit_code == 0, result.output
-    assert (
-        f"SUCCESS: Account '{TEST_ADDRESS}' successfully added with alias '{TEST_ALIAS}'."
-        in result.output
-    )
+    assert f"SUCCESS: Account '{address}' successfully added with alias '{alias}'." in result.output
 
-    expected_path = TEST_ACCOUNT_PATH
-    expected_hd_path = f"m/44'/60'/0'/{selected_account_id}"
+    expected_path = container.data_folder.joinpath(f"{alias}.json")
+    expected_hd_path = "m/44'/60'/0'/2"
     assert_account(expected_path, expected_hdpath=expected_hd_path)
 
 
-def test_add_alias_already_exists(
-    runner, mock_ethereum_app, mock_device_connection, existing_account
-):
-    result = runner.invoke(cli, ["ledger", "add", TEST_ALIAS], input="0")
+def test_add_alias_already_exists(runner, existing_account, choices, address, alias):
+    choices(address, 2)
+
+    # Ensure exists
+    runner.invoke(cli, ["ledger", "add", alias])
+
+    result = runner.invoke(cli, ["ledger", "add", alias])
     assert result.exit_code == 1, result.output
     assert (
-        f"ERROR: (AliasAlreadyInUseError) Account with alias '{TEST_ALIAS}' already in use."
+        f"ERROR: (AliasAlreadyInUseError) Account with alias '{alias}' already in use."
         in result.output
     )
 
 
-def test_delete(runner, existing_account):
-    result = runner.invoke(cli, ["ledger", "delete", TEST_ALIAS])
+def test_delete(runner, existing_account, alias):
+    result = runner.invoke(cli, ["ledger", "delete", alias])
     assert result.exit_code == 0, result.output
-    assert f"SUCCESS: Account '{TEST_ALIAS}' has been removed" in result.output
+    assert f"SUCCESS: Account '{alias}' has been removed" in result.output
 
 
-def test_delete_account_not_exists(runner):
-    result = runner.invoke(cli, ["ledger", "delete", TEST_ALIAS])
+def test_delete_account_not_exists(runner, alias):
+    result = runner.invoke(cli, ["ledger", "delete", alias])
     assert result.exit_code == 2
-    assert f"'{TEST_ALIAS}' is not one of" in result.output
+    assert f"'{alias}' is not one of" in result.output
```

