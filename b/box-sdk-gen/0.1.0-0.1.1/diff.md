# Comparing `tmp/box-sdk-gen-0.1.0.tar.gz` & `tmp/box-sdk-gen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "box-sdk-gen-0.1.0.tar", last modified: Wed Aug  2 14:53:07 2023, max compression
+gzip compressed data, was "box-sdk-gen-0.1.1.tar", last modified: Thu Aug  3 14:44:16 2023, max compression
```

## Comparing `box-sdk-gen-0.1.0.tar` & `box-sdk-gen-0.1.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 mcong      (502) staff       (20)        0 2023-08-02 14:53:07.866122 box-sdk-gen-0.1.0/
--rw-r--r--   0 mcong      (502) staff       (20)     9574 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/LICENSE
--rw-r--r--   0 mcong      (502) staff       (20)     6030 2023-08-02 14:53:07.905623 box-sdk-gen-0.1.0/PKG-INFO
--rw-r--r--   0 mcong      (502) staff       (20)     4498 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/README.md
-drwxr-xr-x   0 mcong      (502) staff       (20)        0 2023-08-02 14:53:07.874020 box-sdk-gen-0.1.0/box_sdk_gen/
--rw-r--r--   0 mcong      (502) staff       (20)        0 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/__init__.py
--rw-r--r--   0 mcong      (502) staff       (20)      354 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/auth.py
--rw-r--r--   0 mcong      (502) staff       (20)     2929 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/auth_schemas.py
--rw-r--r--   0 mcong      (502) staff       (20)     3662 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/base_object.py
--rw-r--r--   0 mcong      (502) staff       (20)      936 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/box_response.py
--rw-r--r--   0 mcong      (502) staff       (20)     4977 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/ccg_auth.py
--rw-r--r--   0 mcong      (502) staff       (20)    13031 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/client.py
--rw-r--r--   0 mcong      (502) staff       (20)      486 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/developer_token_auth.py
--rw-r--r--   0 mcong      (502) staff       (20)     7707 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/fetch.py
--rw-r--r--   0 mcong      (502) staff       (20)    10076 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/jwt_auth.py
-drwxr-xr-x   0 mcong      (502) staff       (20)        0 2023-08-02 14:53:07.905252 box-sdk-gen-0.1.0/box_sdk_gen/managers/
--rw-r--r--   0 mcong      (502) staff       (20)        0 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/__init__.py
--rw-r--r--   0 mcong      (502) staff       (20)     3919 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/authorization.py
--rw-r--r--   0 mcong      (502) staff       (20)     2862 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/avatars.py
--rw-r--r--   0 mcong      (502) staff       (20)     9741 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/chunked_uploads.py
--rw-r--r--   0 mcong      (502) staff       (20)     4876 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/classifications.py
--rw-r--r--   0 mcong      (502) staff       (20)     4613 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/collaboration_allowlist_entries.py
--rw-r--r--   0 mcong      (502) staff       (20)     4731 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/collaboration_allowlist_exempt_targets.py
--rw-r--r--   0 mcong      (502) staff       (20)     4176 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/collections.py
--rw-r--r--   0 mcong      (502) staff       (20)     8911 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/comments.py
--rw-r--r--   0 mcong      (502) staff       (20)     3607 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/device_pinners.py
--rw-r--r--   0 mcong      (502) staff       (20)     3195 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/downloads.py
--rw-r--r--   0 mcong      (502) staff       (20)     3081 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/email_aliases.py
--rw-r--r--   0 mcong      (502) staff       (20)     7939 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/events.py
--rw-r--r--   0 mcong      (502) staff       (20)     4838 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/file_classifications.py
--rw-r--r--   0 mcong      (502) staff       (20)     5695 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/file_metadata.py
--rw-r--r--   0 mcong      (502) staff       (20)    11200 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/file_requests.py
--rw-r--r--   0 mcong      (502) staff       (20)     3797 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/file_version_legal_holds.py
--rw-r--r--   0 mcong      (502) staff       (20)     4163 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/file_version_retentions.py
--rw-r--r--   0 mcong      (502) staff       (20)    10431 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/file_versions.py
--rw-r--r--   0 mcong      (502) staff       (20)     3927 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/file_watermarks.py
--rw-r--r--   0 mcong      (502) staff       (20)    20759 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/files.py
--rw-r--r--   0 mcong      (502) staff       (20)     5205 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/folder_classifications.py
--rw-r--r--   0 mcong      (502) staff       (20)     4658 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/folder_locks.py
--rw-r--r--   0 mcong      (502) staff       (20)     6540 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/folder_metadata.py
--rw-r--r--   0 mcong      (502) staff       (20)     4300 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/folder_watermarks.py
--rw-r--r--   0 mcong      (502) staff       (20)    30103 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/folders.py
--rw-r--r--   0 mcong      (502) staff       (20)    13439 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/groups.py
--rw-r--r--   0 mcong      (502) staff       (20)     7382 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/integration_mappings.py
--rw-r--r--   0 mcong      (502) staff       (20)     4542 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/invites.py
--rw-r--r--   0 mcong      (502) staff       (20)     7825 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/legal_hold_policies.py
--rw-r--r--   0 mcong      (502) staff       (20)    12243 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/legal_hold_policy_assignments.py
--rw-r--r--   0 mcong      (502) staff       (20)     7783 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/list_collaborations.py
--rw-r--r--   0 mcong      (502) staff       (20)    11465 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/memberships.py
--rw-r--r--   0 mcong      (502) staff       (20)     8128 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/metadata_cascade_policies.py
--rw-r--r--   0 mcong      (502) staff       (20)     8881 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/metadata_templates.py
--rw-r--r--   0 mcong      (502) staff       (20)     2417 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/recent_items.py
--rw-r--r--   0 mcong      (502) staff       (20)    14453 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/retention_policies.py
--rw-r--r--   0 mcong      (502) staff       (20)    10382 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/retention_policy_assignments.py
--rw-r--r--   0 mcong      (502) staff       (20)    22628 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/search.py
--rw-r--r--   0 mcong      (502) staff       (20)     2610 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/session_termination.py
--rw-r--r--   0 mcong      (502) staff       (20)    16235 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/shared_links_files.py
--rw-r--r--   0 mcong      (502) staff       (20)    16356 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/shared_links_folders.py
--rw-r--r--   0 mcong      (502) staff       (20)    14822 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/shared_links_web_links.py
--rw-r--r--   0 mcong      (502) staff       (20)     3644 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/shield_information_barrier_reports.py
--rw-r--r--   0 mcong      (502) staff       (20)     6473 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/shield_information_barrier_segment_members.py
--rw-r--r--   0 mcong      (502) staff       (20)     7864 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/shield_information_barrier_segment_restrictions.py
--rw-r--r--   0 mcong      (502) staff       (20)     5924 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/shield_information_barrier_segments.py
--rw-r--r--   0 mcong      (502) staff       (20)     6136 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/shield_information_barriers.py
--rw-r--r--   0 mcong      (502) staff       (20)     9174 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/sign_requests.py
--rw-r--r--   0 mcong      (502) staff       (20)     2328 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/sign_templates.py
--rw-r--r--   0 mcong      (502) staff       (20)     8343 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/skills.py
--rw-r--r--   0 mcong      (502) staff       (20)     2940 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/storage_policies.py
--rw-r--r--   0 mcong      (502) staff       (20)     7877 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/storage_policy_assignments.py
--rw-r--r--   0 mcong      (502) staff       (20)     6243 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/task_assignments.py
--rw-r--r--   0 mcong      (502) staff       (20)     7435 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/tasks.py
--rw-r--r--   0 mcong      (502) staff       (20)     4931 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/terms_of_service_user_statuses.py
--rw-r--r--   0 mcong      (502) staff       (20)     4858 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/terms_of_services.py
--rw-r--r--   0 mcong      (502) staff       (20)     4544 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/transfer.py
--rw-r--r--   0 mcong      (502) staff       (20)     5963 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/trashed_files.py
--rw-r--r--   0 mcong      (502) staff       (20)     6747 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/trashed_folders.py
--rw-r--r--   0 mcong      (502) staff       (20)     4528 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/trashed_items.py
--rw-r--r--   0 mcong      (502) staff       (20)     4683 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/trashed_web_links.py
--rw-r--r--   0 mcong      (502) staff       (20)    11775 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/uploads.py
--rw-r--r--   0 mcong      (502) staff       (20)    11807 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/user_collaborations.py
--rw-r--r--   0 mcong      (502) staff       (20)    22955 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/users.py
--rw-r--r--   0 mcong      (502) staff       (20)     7957 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/web_links.py
--rw-r--r--   0 mcong      (502) staff       (20)     7256 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/webhooks.py
--rw-r--r--   0 mcong      (502) staff       (20)     5553 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/workflows.py
--rw-r--r--   0 mcong      (502) staff       (20)     5582 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/managers/zip_downloads.py
--rw-r--r--   0 mcong      (502) staff       (20)      137 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/network.py
--rw-r--r--   0 mcong      (502) staff       (20)     5726 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/oauth.py
--rw-r--r--   0 mcong      (502) staff       (20)   455388 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/schemas.py
--rw-r--r--   0 mcong      (502) staff       (20)     2307 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/box_sdk_gen/utils.py
-drwxr-xr-x   0 mcong      (502) staff       (20)        0 2023-08-02 14:53:07.876256 box-sdk-gen-0.1.0/box_sdk_gen.egg-info/
--rw-r--r--   0 mcong      (502) staff       (20)     6030 2023-08-02 14:53:07.000000 box-sdk-gen-0.1.0/box_sdk_gen.egg-info/PKG-INFO
--rw-r--r--   0 mcong      (502) staff       (20)     3415 2023-08-02 14:53:07.000000 box-sdk-gen-0.1.0/box_sdk_gen.egg-info/SOURCES.txt
--rw-r--r--   0 mcong      (502) staff       (20)        1 2023-08-02 14:53:07.000000 box-sdk-gen-0.1.0/box_sdk_gen.egg-info/dependency_links.txt
--rw-r--r--   0 mcong      (502) staff       (20)      154 2023-08-02 14:53:07.000000 box-sdk-gen-0.1.0/box_sdk_gen.egg-info/requires.txt
--rw-r--r--   0 mcong      (502) staff       (20)       12 2023-08-02 14:53:07.000000 box-sdk-gen-0.1.0/box_sdk_gen.egg-info/top_level.txt
--rw-r--r--   0 mcong      (502) staff       (20)       38 2023-08-02 14:53:07.906024 box-sdk-gen-0.1.0/setup.cfg
--rw-r--r--   0 mcong      (502) staff       (20)     2028 2023-08-02 14:52:26.000000 box-sdk-gen-0.1.0/setup.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-08-03 14:44:16.967000 box-sdk-gen-0.1.1/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9574 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/LICENSE
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6030 2023-08-03 14:44:16.967000 box-sdk-gen-0.1.1/PKG-INFO
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4498 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/README.md
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-08-03 14:44:16.935000 box-sdk-gen-0.1.1/box_sdk_gen/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      354 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2929 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/auth_schemas.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3662 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/base_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      936 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/box_response.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4977 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/ccg_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    13031 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/client.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      486 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/developer_token_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7707 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/fetch.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10076 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/jwt_auth.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-08-03 14:44:16.966000 box-sdk-gen-0.1.1/box_sdk_gen/managers/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3919 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/authorization.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2862 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/avatars.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9741 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/chunked_uploads.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4876 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/classifications.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4613 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/collaboration_allowlist_entries.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4731 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/collaboration_allowlist_exempt_targets.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4176 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/collections.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8911 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/comments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3607 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/device_pinners.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3195 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/downloads.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3081 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/email_aliases.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7939 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/events.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4838 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/file_classifications.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5749 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/file_metadata.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11200 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/file_requests.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3797 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/file_version_legal_holds.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4163 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/file_version_retentions.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10431 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/file_versions.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3927 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/file_watermarks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    20759 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/files.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5205 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_classifications.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4658 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_locks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6540 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_metadata.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4300 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_watermarks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    30103 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/folders.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    13439 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/groups.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7382 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/integration_mappings.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4542 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/invites.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7825 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/legal_hold_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12243 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/legal_hold_policy_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7783 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/list_collaborations.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11465 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/memberships.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8128 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/metadata_cascade_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8881 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/metadata_templates.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2417 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/recent_items.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    14453 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/retention_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10382 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/retention_policy_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    22628 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/search.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2610 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/session_termination.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    16235 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shared_links_files.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    16356 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shared_links_folders.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    14822 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shared_links_web_links.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3644 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barrier_reports.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6473 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barrier_segment_members.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7864 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barrier_segment_restrictions.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5924 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barrier_segments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6136 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barriers.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9174 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/sign_requests.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2328 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/sign_templates.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8343 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/skills.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2940 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/storage_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7877 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/storage_policy_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6243 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/task_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7435 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/tasks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4931 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/terms_of_service_user_statuses.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4858 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/terms_of_services.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4544 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/transfer.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5963 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/trashed_files.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6747 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/trashed_folders.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4528 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/trashed_items.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4683 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/trashed_web_links.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11775 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/uploads.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11807 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/user_collaborations.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    22955 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/users.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7957 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/web_links.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7256 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/webhooks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5553 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/workflows.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5582 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/managers/zip_downloads.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      137 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/network.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5726 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/oauth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)   455388 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/schemas.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2307 2023-08-03 14:44:03.000000 box-sdk-gen-0.1.1/box_sdk_gen/utils.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2023-08-03 14:44:16.937000 box-sdk-gen-0.1.1/box_sdk_gen.egg-info/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6030 2023-08-03 14:44:16.000000 box-sdk-gen-0.1.1/box_sdk_gen.egg-info/PKG-INFO
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3415 2023-08-03 14:44:16.000000 box-sdk-gen-0.1.1/box_sdk_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        1 2023-08-03 14:44:16.000000 box-sdk-gen-0.1.1/box_sdk_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      154 2023-08-03 14:44:16.000000 box-sdk-gen-0.1.1/box_sdk_gen.egg-info/requires.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       12 2023-08-03 14:44:16.000000 box-sdk-gen-0.1.1/box_sdk_gen.egg-info/top_level.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       38 2023-08-03 14:44:16.967000 box-sdk-gen-0.1.1/setup.cfg
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2011 2023-08-03 14:44:04.000000 box-sdk-gen-0.1.1/setup.py
```

### Comparing `box-sdk-gen-0.1.0/LICENSE` & `box-sdk-gen-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/PKG-INFO` & `box-sdk-gen-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: box-sdk-gen
-Version: 0.1.0
+Version: 0.1.1
 Summary: [Box Platform](https://box.dev) provides functionality to provide access to content stored within [Box](https://box.com). It provides endpoints for basic manipulation of files and folders, management of users within an enterprise, as well as more complex topics such as legal holds and retention policies.
 Home-page: https://github.com/box/box-python-sdk-gen.git
 Author: Box
 Author-email: oss@box.com
 License: Apache-2.0, http://www.apache.org/licenses/LICENSE-2.0
 Keywords: box,sdk,api,rest,boxsdk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `box-sdk-gen-0.1.0/README.md` & `box-sdk-gen-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/auth_schemas.py` & `box-sdk-gen-0.1.1/box_sdk_gen/auth_schemas.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/base_object.py` & `box-sdk-gen-0.1.1/box_sdk_gen/base_object.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/box_response.py` & `box-sdk-gen-0.1.1/box_sdk_gen/box_response.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/ccg_auth.py` & `box-sdk-gen-0.1.1/box_sdk_gen/ccg_auth.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/client.py` & `box-sdk-gen-0.1.1/box_sdk_gen/client.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/fetch.py` & `box-sdk-gen-0.1.1/box_sdk_gen/fetch.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/jwt_auth.py` & `box-sdk-gen-0.1.1/box_sdk_gen/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/authorization.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/authorization.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/avatars.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/avatars.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/chunked_uploads.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/chunked_uploads.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/classifications.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/classifications.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/collaboration_allowlist_entries.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/collaboration_allowlist_entries.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/collaboration_allowlist_exempt_targets.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/collaboration_allowlist_exempt_targets.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/collections.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/collections.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/comments.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/comments.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/device_pinners.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/device_pinners.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/downloads.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/downloads.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/email_aliases.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/email_aliases.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/events.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/events.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/file_classifications.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/file_classifications.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/file_metadata.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/file_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from box_sdk_gen.base_object import BaseObject
 
 from box_sdk_gen.schemas import Metadatas
 
 from box_sdk_gen.schemas import ClientError
 
+from box_sdk_gen.schemas import MetadataFull
+
 from box_sdk_gen.schemas import Metadata
 
 from box_sdk_gen.auth import Authentication
 
 from box_sdk_gen.network import NetworkSession
 
 from box_sdk_gen.utils import prepare_params
@@ -54,15 +56,15 @@
             for the URL `https://*.app.box.com/files/123`
             the `file_id` is `123`.
             Example: "12345"
         :type file_id: str
         """
         response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata']), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
         return Metadatas.from_dict(json.loads(response.text))
-    def get_file_metadata_by_id(self, file_id: str, scope: GetFileMetadataByIdScopeArg, template_key: str) -> Metadata:
+    def get_file_metadata_by_id(self, file_id: str, scope: GetFileMetadataByIdScopeArg, template_key: str) -> MetadataFull:
         """
         Retrieves the instance of a metadata template that has been applied to a
         
         file.
 
         :param file_id: The unique identifier that represents a file.
             The ID for any file can be determined
@@ -76,15 +78,15 @@
             Example: "global"
         :type scope: GetFileMetadataByIdScopeArg
         :param template_key: The name of the metadata template
             Example: "properties"
         :type template_key: str
         """
         response: FetchResponse = fetch(''.join(['https://api.box.com/2.0/files/', file_id, '/metadata/', scope, '/', template_key]), FetchOptions(method='GET', response_format='json', auth=self.auth, network_session=self.network_session))
-        return Metadata.from_dict(json.loads(response.text))
+        return MetadataFull.from_dict(json.loads(response.text))
     def create_file_metadata_by_id(self, file_id: str, scope: CreateFileMetadataByIdScopeArg, template_key: str) -> Metadata:
         """
         Applies an instance of a metadata template to a file.
         
         In most cases only values that are present in the metadata template
```

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/file_requests.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/file_requests.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/file_version_legal_holds.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/file_version_legal_holds.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/file_version_retentions.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/file_version_retentions.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/file_versions.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/file_versions.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/file_watermarks.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/file_watermarks.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/files.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/files.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/folder_classifications.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_classifications.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/folder_locks.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_locks.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/folder_metadata.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_metadata.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/folder_watermarks.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/folder_watermarks.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/folders.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/folders.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/groups.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/groups.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/integration_mappings.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/integration_mappings.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/invites.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/invites.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/legal_hold_policies.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/legal_hold_policies.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/legal_hold_policy_assignments.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/legal_hold_policy_assignments.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/list_collaborations.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/list_collaborations.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/memberships.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/memberships.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/metadata_cascade_policies.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/metadata_cascade_policies.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/metadata_templates.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/metadata_templates.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/recent_items.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/recent_items.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/retention_policies.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/retention_policies.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/retention_policy_assignments.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/retention_policy_assignments.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/search.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/search.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/session_termination.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/session_termination.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/shared_links_files.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/shared_links_files.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/shared_links_folders.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/shared_links_folders.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/shared_links_web_links.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/shared_links_web_links.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/shield_information_barrier_reports.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barrier_reports.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/shield_information_barrier_segment_members.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barrier_segment_members.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/shield_information_barrier_segment_restrictions.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barrier_segment_restrictions.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/shield_information_barrier_segments.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barrier_segments.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/shield_information_barriers.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/shield_information_barriers.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/sign_requests.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/sign_requests.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/sign_templates.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/sign_templates.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/skills.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/skills.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/storage_policies.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/storage_policies.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/storage_policy_assignments.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/storage_policy_assignments.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/task_assignments.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/task_assignments.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/tasks.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/tasks.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/terms_of_service_user_statuses.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/terms_of_service_user_statuses.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/terms_of_services.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/terms_of_services.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/transfer.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/transfer.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/trashed_files.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/trashed_files.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/trashed_folders.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/trashed_folders.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/trashed_items.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/trashed_items.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/trashed_web_links.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/trashed_web_links.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/uploads.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/uploads.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/user_collaborations.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/user_collaborations.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/users.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/users.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/web_links.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/web_links.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/webhooks.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/webhooks.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/workflows.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/workflows.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/managers/zip_downloads.py` & `box-sdk-gen-0.1.1/box_sdk_gen/managers/zip_downloads.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/oauth.py` & `box-sdk-gen-0.1.1/box_sdk_gen/oauth.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/schemas.py` & `box-sdk-gen-0.1.1/box_sdk_gen/schemas.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen/utils.py` & `box-sdk-gen-0.1.1/box_sdk_gen/utils.py`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen.egg-info/PKG-INFO` & `box-sdk-gen-0.1.1/box_sdk_gen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: box-sdk-gen
-Version: 0.1.0
+Version: 0.1.1
 Summary: [Box Platform](https://box.dev) provides functionality to provide access to content stored within [Box](https://box.com). It provides endpoints for basic manipulation of files and folders, management of users within an enterprise, as well as more complex topics such as legal holds and retention policies.
 Home-page: https://github.com/box/box-python-sdk-gen.git
 Author: Box
 Author-email: oss@box.com
 License: Apache-2.0, http://www.apache.org/licenses/LICENSE-2.0
 Keywords: box,sdk,api,rest,boxsdk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `box-sdk-gen-0.1.0/box_sdk_gen.egg-info/SOURCES.txt` & `box-sdk-gen-0.1.1/box_sdk_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `box-sdk-gen-0.1.0/setup.py` & `box-sdk-gen-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 
 def main():
     install_requires = ['requests', 'requests_toolbelt', 'urllib3<2']
     tests_require = ['pytest', 'pytest-timeout', 'pytest-cov']
     dev_requires = ['tox']
     jwt_requires = ['pyjwt>=1.7.0', 'cryptography>=3']
     extras_require = {'test': tests_require + jwt_requires, 'dev': dev_requires, 'jwt': jwt_requires}
-    setup(name='box-sdk-gen', version='0.1.0', description='[Box Platform](https://box.dev) provides functionality to provide access to content stored within [Box](https://box.com). It provides endpoints for basic manipulation of files and folders, management of users within an enterprise, as well as more complex topics such as legal holds and retention policies.', url='https://github.com/box/box-python-sdk-gen.git', licence='Apache-2.0, http://www.apache.org/licenses/LICENSE-2.0', author='Box', long_description_content_type='text/markdown', long_description=open(join(dirname(__file__), 'README.md'), encoding='utf-8').read(), author_email='oss@box.com', project_urls={}, classifiers=['Development Status :: 4 - Beta', 'Intended Audience :: Developers', 'License :: OSI Approved :: Apache Software License', 'Programming Language :: Python', 'Programming Language :: Python :: 3.6', 'Programming Language :: Python :: 3.7', 'Programming Language :: Python :: 3.8', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: Implementation :: CPython', 'Programming Language :: Python :: Implementation :: PyPy', 'Operating System :: OS Independent', 'Operating System :: POSIX', 'Operating System :: Microsoft :: Windows', 'Operating System :: MacOS :: MacOS X', 'Topic :: Software Development :: Libraries :: Python Modules'], keywords='box, sdk, api, rest, boxsdk', install_requires=install_requires, tests_require=tests_require, extras_require=extras_require, packages=find_packages(exclude=['docs', '*test*']))
+    setup(name='box-sdk-gen', version='0.1.1', description='[Box Platform](https://box.dev) provides functionality to provide access to content stored within [Box](https://box.com). It provides endpoints for basic manipulation of files and folders, management of users within an enterprise, as well as more complex topics such as legal holds and retention policies.', url='https://github.com/box/box-python-sdk-gen.git', licence='Apache-2.0, http://www.apache.org/licenses/LICENSE-2.0', author='Box', long_description_content_type='text/markdown', long_description=open(join(dirname(__file__), 'README.md'), encoding='utf-8').read(), author_email='oss@box.com', classifiers=['Development Status :: 4 - Beta', 'Intended Audience :: Developers', 'License :: OSI Approved :: Apache Software License', 'Programming Language :: Python', 'Programming Language :: Python :: 3.6', 'Programming Language :: Python :: 3.7', 'Programming Language :: Python :: 3.8', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: Implementation :: CPython', 'Programming Language :: Python :: Implementation :: PyPy', 'Operating System :: OS Independent', 'Operating System :: POSIX', 'Operating System :: Microsoft :: Windows', 'Operating System :: MacOS :: MacOS X', 'Topic :: Software Development :: Libraries :: Python Modules'], keywords='box, sdk, api, rest, boxsdk', install_requires=install_requires, tests_require=tests_require, extras_require=extras_require, packages=find_packages(exclude=['docs', '*test*']))
 
 if __name__ == '__main__':
     main()
```

