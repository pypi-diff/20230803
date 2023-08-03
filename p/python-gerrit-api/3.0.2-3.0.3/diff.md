# Comparing `tmp/python-gerrit-api-3.0.2.tar.gz` & `tmp/python-gerrit-api-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-gerrit-api-3.0.2.tar", last modified: Mon Jul 31 06:46:19 2023, max compression
+gzip compressed data, was "python-gerrit-api-3.0.3.tar", last modified: Tue Aug  1 03:55:30 2023, max compression
```

## Comparing `python-gerrit-api-3.0.2.tar` & `python-gerrit-api-3.0.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.421979 python-gerrit-api-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-07-31 06:46:19.421979 python-gerrit-api-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.409979 python-gerrit-api-3.0.2/gerrit/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.409979 python-gerrit-api-3.0.2/gerrit/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18261 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/accounts/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/accounts/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/accounts/gpg_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/accounts/ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.413979 python-gerrit-api-3.0.2/gerrit/changes/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27372 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/change.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/reviewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.413979 python-gerrit-api-3.0.2/gerrit/changes/revision/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/revision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/revision/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/revision/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/revision/drafts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/revision/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.413979 python-gerrit-api-3.0.2/gerrit/config/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/config/caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/config/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.417979 python-gerrit-api-3.0.2/gerrit/groups/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/groups/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/groups/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/groups/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/groups/subgroups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.417979 python-gerrit-api-3.0.2/gerrit/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/plugins/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.417979 python-gerrit-api-3.0.2/gerrit/projects/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14138 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.417979 python-gerrit-api-3.0.2/gerrit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/utils/gerritbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/utils/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.417979 python-gerrit-api-3.0.2/gitiles/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gitiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gitiles/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.421979 python-gerrit-api-3.0.2/python_gerrit_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-07-31 06:46:19.000000 python-gerrit-api-3.0.2/python_gerrit_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-31 06:46:19.000000 python-gerrit-api-3.0.2/python_gerrit_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:46:19.000000 python-gerrit-api-3.0.2/python_gerrit_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 06:46:19.000000 python-gerrit-api-3.0.2/python_gerrit_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 06:46:19.000000 python-gerrit-api-3.0.2/python_gerrit_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:46:19.421979 python-gerrit-api-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.421979 python-gerrit-api-3.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/tests/test_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/tests/test_gitiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/tests/test_revision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:55:30.830142 python-gerrit-api-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-08-01 03:55:30.830142 python-gerrit-api-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:55:30.818140 python-gerrit-api-3.0.3/gerrit/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:55:30.822141 python-gerrit-api-3.0.3/gerrit/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18261 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/accounts/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/accounts/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/accounts/gpg_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/accounts/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:55:30.822141 python-gerrit-api-3.0.3/gerrit/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/changes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27372 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/changes/change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/changes/changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/changes/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/changes/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/changes/reviewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:55:30.822141 python-gerrit-api-3.0.3/gerrit/changes/revision/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/changes/revision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/changes/revision/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/changes/revision/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/changes/revision/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/changes/revision/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:55:30.822141 python-gerrit-api-3.0.3/gerrit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/config/caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/config/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:55:30.822141 python-gerrit-api-3.0.3/gerrit/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/groups/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/groups/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/groups/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/groups/subgroups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:55:30.822141 python-gerrit-api-3.0.3/gerrit/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/plugins/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:55:30.826141 python-gerrit-api-3.0.3/gerrit/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/projects/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/projects/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/projects/dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/projects/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14131 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/projects/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/projects/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/projects/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/projects/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:55:30.826141 python-gerrit-api-3.0.3/gerrit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/utils/gerritbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gerrit/utils/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:55:30.826141 python-gerrit-api-3.0.3/gitiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gitiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/gitiles/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:55:30.826141 python-gerrit-api-3.0.3/python_gerrit_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-08-01 03:55:30.000000 python-gerrit-api-3.0.3/python_gerrit_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-01 03:55:30.000000 python-gerrit-api-3.0.3/python_gerrit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 03:55:30.000000 python-gerrit-api-3.0.3/python_gerrit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 03:55:30.000000 python-gerrit-api-3.0.3/python_gerrit_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 03:55:30.000000 python-gerrit-api-3.0.3/python_gerrit_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 03:55:30.830142 python-gerrit-api-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:55:30.826141 python-gerrit-api-3.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/tests/test_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/tests/test_gitiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-08-01 03:55:19.000000 python-gerrit-api-3.0.3/tests/test_revision.py
```

### Comparing `python-gerrit-api-3.0.2/LICENSE` & `python-gerrit-api-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/PKG-INFO` & `python-gerrit-api-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 3.0.2
+Version: 3.0.3
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-gerrit-api-3.0.2/README.rst` & `python-gerrit-api-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/accounts/account.py` & `python-gerrit-api-3.0.3/gerrit/accounts/account.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/accounts/accounts.py` & `python-gerrit-api-3.0.3/gerrit/accounts/accounts.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         try:
             endpoint = self.endpoint + f"/{account}/"
             result = self.gerrit.get(endpoint)
 
             account_ = result.get("_account_id")
             return GerritAccount(account=account_, gerrit=self.gerrit)
         except requests.exceptions.HTTPError as error:
-            if error.response.status_code in (404, 400):
+            if error.response.status_code == 404:
                 message = f"Account {account} does not exist"
                 logger.error(message)
                 raise AccountNotFoundError(message)
             raise GerritAPIException from error
 
     def create(self, username, input_):
         """
```

### Comparing `python-gerrit-api-3.0.2/gerrit/accounts/emails.py` & `python-gerrit-api-3.0.3/gerrit/accounts/emails.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         """
         try:
             result = self.gerrit.get(self.endpoint + f"/{email}")
 
             email_ = result.get("email")
             return GerritAccountEmail(email=email_, account=self.account, gerrit=self.gerrit)
         except requests.exceptions.HTTPError as error:
-            if error.response.status_code in (404, 400):
+            if error.response.status_code == 404:
                 message = f"Account Email {email} does not exist"
                 logger.error(message)
                 raise AccountEmailNotFoundError(message)
             raise GerritAPIException from error
 
     def set_preferred(self, email):
         """
```

### Comparing `python-gerrit-api-3.0.2/gerrit/accounts/gpg_keys.py` & `python-gerrit-api-3.0.3/gerrit/accounts/gpg_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         """
         try:
             result = self.gerrit.get(self.endpoint + f"/{id_}")
 
             id = result.get("id")
             return GerritAccountGPGKey(id=id, account=self.account, gerrit=self.gerrit)
         except requests.exceptions.HTTPError as error:
-            if error.response.status_code in (404, 400):
+            if error.response.status_code == 404:
                 message = f"GPG key {id_} does not exist"
                 logger.error(message)
                 raise GPGKeyNotFoundError(message)
             raise GerritAPIException from error
 
     def modify(self, input_):
         """
```

### Comparing `python-gerrit-api-3.0.2/gerrit/accounts/ssh_keys.py` & `python-gerrit-api-3.0.3/gerrit/accounts/ssh_keys.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         """
         try:
             result = self.gerrit.get(self.endpoint + f"/{str(seq)}")
 
             seq = result.get("seq")
             return GerritAccountSSHKey(seq=seq, account=self.account, gerrit=self.gerrit)
         except requests.exceptions.HTTPError as error:
-            if error.response.status_code in (404, 400):
+            if error.response.status_code == 404:
                 message = f"SSH key {seq} does not exist"
                 logger.error(message)
                 raise SSHKeyNotFoundError(message)
             raise GerritAPIException from error
 
     def add(self, ssh_key):
         """
```

### Comparing `python-gerrit-api-3.0.2/gerrit/base.py` & `python-gerrit-api-3.0.3/gerrit/base.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/changes/change.py` & `python-gerrit-api-3.0.3/gerrit/changes/change.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/changes/changes.py` & `python-gerrit-api-3.0.3/gerrit/changes/changes.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         try:
             endpoint = self.endpoint + f"/{id_}/"
             result = self.gerrit.get(endpoint)
 
             id = result.get("id")
             return GerritChange(id=id, gerrit=self.gerrit)
         except requests.exceptions.HTTPError as error:
-            if error.response.status_code in (404, 400):
+            if error.response.status_code == 404:
                 message = f"Change {id_} does not exist"
                 if id_.startswith("I"):
                     res = self.search(query=f"change: {id_}")
                     if len(res) > 0:
                         change_ids = [item.get("id") for item in res]
                         message = f"Change {id_} query multiple changes: {', '.join(change_ids)}, which one do you want?"
```

### Comparing `python-gerrit-api-3.0.2/gerrit/changes/edit.py` & `python-gerrit-api-3.0.3/gerrit/changes/edit.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/changes/messages.py` & `python-gerrit-api-3.0.3/gerrit/changes/messages.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/changes/reviewers.py` & `python-gerrit-api-3.0.3/gerrit/changes/reviewers.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         """
         try:
             result = self.gerrit.get(self.endpoint + f"/{account}")
 
             account = result[0].get("_account_id")
             return GerritChangeReviewer(account=account, change=self.change, gerrit=self.gerrit)
         except requests.exceptions.HTTPError as error:
-            if error.response.status_code in (404, 400):
+            if error.response.status_code == 404:
                 message = f"Reviewer {account} does not exist"
                 logger.error(message)
                 raise ReviewerNotFoundError(message)
             raise GerritAPIException from error
 
     def add(self, input_):
         """
```

### Comparing `python-gerrit-api-3.0.2/gerrit/changes/revision/base.py` & `python-gerrit-api-3.0.3/gerrit/changes/revision/base.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/changes/revision/comments.py` & `python-gerrit-api-3.0.3/gerrit/changes/revision/comments.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/changes/revision/drafts.py` & `python-gerrit-api-3.0.3/gerrit/changes/revision/drafts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/changes/revision/files.py` & `python-gerrit-api-3.0.3/gerrit/changes/revision/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         """
         try:
             result = self.gerrit.get(self.endpoint + "/content")
             if decode:
                 return b64decode(result).decode("utf-8")
             return result
         except requests.exceptions.HTTPError as error:
-            if error.response.status_code in (404, 400):
+            if error.response.status_code == 404:
                 message = f"Revision File {self.path} content does not exist"
                 logger.error(message)
                 raise FileContentNotFoundError(message)
             raise GerritAPIException from error
 
     def download_content(self):
         """
```

### Comparing `python-gerrit-api-3.0.2/gerrit/config/caches.py` & `python-gerrit-api-3.0.3/gerrit/config/caches.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/config/config.py` & `python-gerrit-api-3.0.3/gerrit/config/config.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/config/tasks.py` & `python-gerrit-api-3.0.3/gerrit/config/tasks.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/groups/group.py` & `python-gerrit-api-3.0.3/gerrit/groups/group.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/groups/groups.py` & `python-gerrit-api-3.0.3/gerrit/groups/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         try:
             endpoint = self.endpoint + f"/{id_}/"
             res = self.gerrit.get(endpoint)
 
             group_id = res.get("id")
             return GerritGroup(group_id=group_id, gerrit=self.gerrit)
         except requests.exceptions.HTTPError as error:
-            if error.response.status_code in (404, 400):
+            if error.response.status_code == 404:
                 message = f"Group {id_} does not exist"
                 logger.error(message)
                 raise GroupNotFoundError(message)
             raise GerritAPIException from error
 
     def create(self, name, input_):
         """
```

### Comparing `python-gerrit-api-3.0.2/gerrit/groups/members.py` & `python-gerrit-api-3.0.3/gerrit/groups/members.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         :return:
         """
         try:
             result = self.gerrit.get(self.endpoint + f"/{account}")
             account_id = result.get("_account_id")
             return self.gerrit.accounts.get(account_id)
         except requests.exceptions.HTTPError as error:
-            if error.response.status_code in (404, 400):
+            if error.response.status_code == 404:
                 message = f"Group member {account} does not exist"
                 logger.error(message)
                 raise GroupMemberNotFoundError(message)
             raise GerritAPIException from error
 
     def add(self, account):
         """
```

### Comparing `python-gerrit-api-3.0.2/gerrit/groups/subgroups.py` & `python-gerrit-api-3.0.3/gerrit/groups/subgroups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/plugins/plugins.py` & `python-gerrit-api-3.0.3/gerrit/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/projects/branches.py` & `python-gerrit-api-3.0.3/gerrit/projects/branches.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         :return:
         """
         source = input_.get("source")
         try:
             project = self.gerrit.projects.get(unquote_plus(self.project))
             project.branches.get(name=source)
         except requests.exceptions.HTTPError as error:
-            if error.response.status_code in (404, 400):
+            if error.response.status_code == 404:
                 message = f"Source Branch {source} does not exist"
                 logger.error(message)
                 raise BranchNotFoundError(message)
 
         return self.gerrit.get(self.endpoint + "/mergeable", params=input_)
 
     def get_reflog(self):
@@ -119,15 +119,15 @@
         try:
             result = self.gerrit.get(self.endpoint + f"/{quote_plus(name)}")
 
             ref = result.get("ref")
             name = ref.replace(self.branch_prefix, "")
             return GerritProjectBranch(name=name, project=self.project, gerrit=self.gerrit)
         except requests.exceptions.HTTPError as error:
-            if error.response.status_code in (404, 400):
+            if error.response.status_code == 404:
                 message = f"Branch {name} does not exist"
                 logger.error(message)
                 raise BranchNotFoundError(message)
             raise GerritAPIException from error
 
     def create(self, name, input_):
         """
```

### Comparing `python-gerrit-api-3.0.2/gerrit/projects/commit.py` & `python-gerrit-api-3.0.3/gerrit/projects/commit.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/projects/dashboards.py` & `python-gerrit-api-3.0.3/gerrit/projects/dashboards.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/projects/labels.py` & `python-gerrit-api-3.0.3/gerrit/projects/labels.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/projects/project.py` & `python-gerrit-api-3.0.3/gerrit/projects/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,15 +387,15 @@
         """
         try:
             result = self.gerrit.get(self.endpoint + f"/commits/{commit}")
 
             commit = result.get("commit")
             return GerritProjectCommit(commit=commit, project=self.id, gerrit=self.gerrit)
         except requests.exceptions.HTTPError as error:
-            if error.response.status_code in (404, 400):
+            if error.response.status_code == 404:
                 message = f"Commit {commit} does not exist"
                 logger.error(message)
                 raise CommitNotFoundError(message)
             raise GerritAPIException from error
 
     @property
     def dashboards(self):
```

### Comparing `python-gerrit-api-3.0.2/gerrit/projects/projects.py` & `python-gerrit-api-3.0.3/gerrit/projects/projects.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         pattern_types = {"prefix": "p", "match": "m", "regex": "r"}
         tuples = (("n", limit), ("S", skip), ("type", project_type), ("b", branch), ("state", state))
         params = params_creator(tuples, pattern_types, pattern_dispatcher)
         if is_all:
             params.clear()
             params["all"] = int(is_all)
         params["d"] = int(description)
-        print(params)
 
         return self.gerrit.get(self.endpoint + "/", params=params)
 
     def search(self, query: str, limit: int = 25, skip: int = 0) -> List:
         """
         Queries projects visible to the caller. The query string must be provided by the
         query parameter.
@@ -104,15 +103,15 @@
         :return:
         """
         try:
             res = self.gerrit.get(self.endpoint + f"/{quote_plus(name)}")
             project_id = res.get("id")
             return GerritProject(project_id=project_id, gerrit=self.gerrit)
         except requests.exceptions.HTTPError as error:
-            if error.response.status_code in (404, 400):
+            if error.response.status_code == 404:
                 message = f"Project {name} does not exist"
                 logger.error(message)
                 raise ProjectNotFoundError(message)
             raise GerritAPIException from error
 
     def create(self, project_name: str, input_: Dict[str, Any]):
         """
```

### Comparing `python-gerrit-api-3.0.2/gerrit/projects/tags.py` & `python-gerrit-api-3.0.3/gerrit/projects/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         try:
             result = self.gerrit.get(self.endpoint + f"/{quote_plus(name)}")
 
             ref = result.get("ref")
             name = ref.replace(self.tag_prefix, "")
             return GerritProjectTag(name=name, project=self.project, gerrit=self.gerrit)
         except requests.exceptions.HTTPError as error:
-            if error.response.status_code in (404, 400):
+            if error.response.status_code == 404:
                 message = f"Tag {name} does not exist"
                 logger.error(message)
                 raise TagNotFoundError(message)
             raise GerritAPIException from error
 
     def create(self, name, input_):
         """
```

### Comparing `python-gerrit-api-3.0.2/gerrit/projects/webhooks.py` & `python-gerrit-api-3.0.3/gerrit/projects/webhooks.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/utils/common.py` & `python-gerrit-api-3.0.3/gerrit/utils/common.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gerrit/utils/exceptions.py` & `python-gerrit-api-3.0.3/gerrit/utils/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,26 @@
 
 class GerritAPIException(Exception):
     """
     Base class for all errors
     """
 
 
+class ClientError(GerritAPIException):
+    """
+    Client Error
+    """
+
+
+class ServerError(GerritAPIException):
+    """
+    Server Error
+    """
+
+
 class UnauthorizedError(GerritAPIException):
     """
     401 Unauthorized
     """
 
 
 class AuthError(GerritAPIException):
```

### Comparing `python-gerrit-api-3.0.2/gerrit/utils/gerritbase.py` & `python-gerrit-api-3.0.3/gerrit/utils/gerritbase.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/gitiles/base.py` & `python-gerrit-api-3.0.3/gitiles/base.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/python_gerrit_api.egg-info/PKG-INFO` & `python-gerrit-api-3.0.3/python_gerrit_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 3.0.2
+Version: 3.0.3
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-gerrit-api-3.0.2/python_gerrit_api.egg-info/SOURCES.txt` & `python-gerrit-api-3.0.3/python_gerrit_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/setup.py` & `python-gerrit-api-3.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,25 @@
 # Get the long description from the relevant file
 with open(path.join(here, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
+
 def get_version() -> str:
     version = ""
     with open("gerrit/__init__.py", "r", encoding="utf-8") as f:
         for line in f:
             if line.startswith("__version__"):
                 version = ast.literal_eval(line.split("=")[-1])
                 break
     return version
 
+
 setup(
     name="python-gerrit-api",
     # https://packaging.python.org/en/latest/single_source_version.html
     version=get_version(),
     description="Python wrapper for the Gerrit REST API.",
     long_description=long_description,
     url="https://github.com/shijl0925/python-gerrit-api",
```

### Comparing `python-gerrit-api-3.0.2/tests/test_accounts.py` & `python-gerrit-api-3.0.3/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/tests/test_changes.py` & `python-gerrit-api-3.0.3/tests/test_changes.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/tests/test_gitiles.py` & `python-gerrit-api-3.0.3/tests/test_gitiles.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/tests/test_groups.py` & `python-gerrit-api-3.0.3/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.2/tests/test_projects.py` & `python-gerrit-api-3.0.3/tests/test_projects.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         "project_name": "LineageOS/Superuser",
         "branch": "master",
         "tag": "cm-10.2.1",
         "file": "README.md",
     },
 ]
 
+
 @pytest.mark.parametrize('is_all, limit, skip, pattern_dispatcher, project_type, description, branch, state',
                          [(False, 25, 0, None, None, False, None, "ACTIVE"),
                           (False, 25, 25, None, None, False, None, "ACTIVE"),
                           (True, 25, 0, None, None, False, None, None),
                           (False, 25, 0, {"prefix": "Lineage"}, None, False, None, None),
                           (False, 25, 0, None, "all", False, None, None),
                           (False, 25, 0, None, None, True, None, None),
```

### Comparing `python-gerrit-api-3.0.2/tests/test_revision.py` & `python-gerrit-api-3.0.3/tests/test_revision.py`

 * *Files identical despite different names*

