# Comparing `tmp/tcsoa-0.9.0.tar.gz` & `tmp/tcsoa-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcsoa-0.9.0.tar", max compression
+gzip compressed data, was "tcsoa-0.9.1.tar", max compression
```

## Comparing `tcsoa-0.9.0.tar` & `tcsoa-0.9.1.tar`

### file list

```diff
@@ -1,2234 +1,2234 @@
--rw-r--r--   0        0        0     1089 2022-09-26 11:08:11.334023 tcsoa-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0      557 2022-12-06 16:02:03.462003 tcsoa-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-06-09 12:29:08.307759 tcsoa-0.9.0/tcsoa/__init__.py
--rw-r--r--   0        0        0     8300 2022-12-06 16:00:02.842630 tcsoa-0.9.0/tcsoa/backend.py
--rw-r--r--   0        0        0     2059 2022-12-05 08:51:33.454395 tcsoa-0.9.0/tcsoa/base.py
--rw-r--r--   0        0        0     8790 2022-12-06 15:00:47.897479 tcsoa-0.9.0/tcsoa/basics.py
--rw-r--r--   0        0        0     1027 2022-12-05 10:07:21.656126 tcsoa-0.9.0/tcsoa/config.py
--rw-r--r--   0        0        0      546 2022-12-06 15:56:36.649956 tcsoa-0.9.0/tcsoa/exceptions.py
--rw-r--r--   0        0        0        0 2022-07-19 08:50:08.936027 tcsoa-0.9.0/tcsoa/fcc/__init__.py
--rw-r--r--   0        0        0     4718 2022-10-18 14:08:47.281729 tcsoa-0.9.0/tcsoa/fcc/fcc_client_proxy.py
--rw-r--r--   0        0        0     2916 2022-10-18 14:11:34.201245 tcsoa-0.9.0/tcsoa/fcc/fcc_wrapper.py
--rw-r--r--   0        0        0     5824 2022-10-18 14:33:08.079453 tcsoa-0.9.0/tcsoa/fcc/file_management_utility.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.782046 tcsoa-0.9.0/tcsoa/gen/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.868058 tcsoa-0.9.0/tcsoa/gen/ActiveCollaboration/_2020_12/__init__.py
--rw-r--r--   0        0        0     3470 2022-10-20 12:41:57.327454 tcsoa-0.9.0/tcsoa/gen/ActiveCollaboration/_2020_12/ActiveCollaboration.py
--rw-r--r--   0        0        0     8878 2022-10-20 12:41:57.371476 tcsoa-0.9.0/tcsoa/gen/ActiveCollaboration/_2020_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.870055 tcsoa-0.9.0/tcsoa/gen/ActiveCollaboration/__init__.py
--rw-r--r--   0        0        0      480 2022-10-20 12:41:53.739062 tcsoa-0.9.0/tcsoa/gen/ActiveCollaboration/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.955069 tcsoa-0.9.0/tcsoa/gen/ActiveWorkspaceBom/_2015_10/__init__.py
--rw-r--r--   0        0        0     3406 2022-10-20 12:41:58.832622 tcsoa-0.9.0/tcsoa/gen/ActiveWorkspaceBom/_2015_10/OccurrenceManagementCad.py
--rw-r--r--   0        0        0     4444 2022-10-20 12:41:57.403455 tcsoa-0.9.0/tcsoa/gen/ActiveWorkspaceBom/_2015_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.991073 tcsoa-0.9.0/tcsoa/gen/ActiveWorkspaceBom/__init__.py
--rw-r--r--   0        0        0      329 2022-10-20 12:41:53.746070 tcsoa-0.9.0/tcsoa/gen/ActiveWorkspaceBom/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.896060 tcsoa-0.9.0/tcsoa/gen/ActiveWorkspaceVis/_2015_03/__init__.py
--rw-r--r--   0        0        0    10014 2022-10-20 12:42:03.940164 tcsoa-0.9.0/tcsoa/gen/ActiveWorkspaceVis/_2015_03/DataManagement.py
--rw-r--r--   0        0        0     4677 2022-10-20 12:41:57.432462 tcsoa-0.9.0/tcsoa/gen/ActiveWorkspaceVis/_2015_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.587032 tcsoa-0.9.0/tcsoa/gen/ActiveWorkspaceVis/__init__.py
--rw-r--r--   0        0        0      215 2022-10-20 12:41:53.752069 tcsoa-0.9.0/tcsoa/gen/ActiveWorkspaceVis/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.831050 tcsoa-0.9.0/tcsoa/gen/Administration/_2006_03/__init__.py
--rw-r--r--   0        0        0     7246 2022-10-20 12:42:33.996207 tcsoa-0.9.0/tcsoa/gen/Administration/_2006_03/IRM.py
--rw-r--r--   0        0        0     8803 2022-10-20 12:41:57.470471 tcsoa-0.9.0/tcsoa/gen/Administration/_2006_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.702046 tcsoa-0.9.0/tcsoa/gen/Administration/_2007_01/__init__.py
--rw-r--r--   0        0        0     1051 2022-10-20 12:41:57.497471 tcsoa-0.9.0/tcsoa/gen/Administration/_2007_01/services.py
--rw-r--r--   0        0        0     3316 2022-10-20 12:42:34.049187 tcsoa-0.9.0/tcsoa/gen/Administration/_2007_01/UserManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.666046 tcsoa-0.9.0/tcsoa/gen/Administration/_2007_06/__init__.py
--rw-r--r--   0        0        0     2093 2022-10-20 12:42:34.087185 tcsoa-0.9.0/tcsoa/gen/Administration/_2007_06/Authorization.py
--rw-r--r--   0        0        0     3078 2022-10-20 12:42:34.135189 tcsoa-0.9.0/tcsoa/gen/Administration/_2007_06/PreferenceManagement.py
--rw-r--r--   0        0        0     3683 2022-10-20 12:41:57.534471 tcsoa-0.9.0/tcsoa/gen/Administration/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.778055 tcsoa-0.9.0/tcsoa/gen/Administration/_2008_03/__init__.py
--rw-r--r--   0        0        0     2026 2022-10-20 12:42:34.180200 tcsoa-0.9.0/tcsoa/gen/Administration/_2008_03/IRM.py
--rw-r--r--   0        0        0     2096 2022-10-20 12:41:57.563475 tcsoa-0.9.0/tcsoa/gen/Administration/_2008_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.803054 tcsoa-0.9.0/tcsoa/gen/Administration/_2008_06/__init__.py
--rw-r--r--   0        0        0     1705 2022-10-20 12:41:57.594490 tcsoa-0.9.0/tcsoa/gen/Administration/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.851061 tcsoa-0.9.0/tcsoa/gen/Administration/_2008_12/__init__.py
--rw-r--r--   0        0        0     2568 2022-10-20 12:41:57.626488 tcsoa-0.9.0/tcsoa/gen/Administration/_2008_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.931067 tcsoa-0.9.0/tcsoa/gen/Administration/_2010_04/__init__.py
--rw-r--r--   0        0        0      649 2022-10-20 12:42:34.207200 tcsoa-0.9.0/tcsoa/gen/Administration/_2010_04/DisciplineManagement.py
--rw-r--r--   0        0        0     7659 2022-10-20 12:42:34.276209 tcsoa-0.9.0/tcsoa/gen/Administration/_2010_04/IRM.py
--rw-r--r--   0        0        0     7891 2022-10-20 12:41:57.668490 tcsoa-0.9.0/tcsoa/gen/Administration/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.999090 tcsoa-0.9.0/tcsoa/gen/Administration/_2011_05/__init__.py
--rw-r--r--   0        0        0     1001 2022-10-20 12:41:57.697494 tcsoa-0.9.0/tcsoa/gen/Administration/_2011_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.714041 tcsoa-0.9.0/tcsoa/gen/Administration/_2012_09/__init__.py
--rw-r--r--   0        0        0    11218 2022-10-20 12:42:34.372213 tcsoa-0.9.0/tcsoa/gen/Administration/_2012_09/PreferenceManagement.py
--rw-r--r--   0        0        0    17945 2022-10-20 12:41:57.758500 tcsoa-0.9.0/tcsoa/gen/Administration/_2012_09/services.py
--rw-r--r--   0        0        0     3547 2022-10-20 12:42:34.433219 tcsoa-0.9.0/tcsoa/gen/Administration/_2012_09/UserManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.556030 tcsoa-0.9.0/tcsoa/gen/Administration/_2012_10/__init__.py
--rw-r--r--   0        0        0     1464 2022-10-20 12:42:34.467229 tcsoa-0.9.0/tcsoa/gen/Administration/_2012_10/IRM.py
--rw-r--r--   0        0        0     2543 2022-10-20 12:41:57.795514 tcsoa-0.9.0/tcsoa/gen/Administration/_2012_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.659037 tcsoa-0.9.0/tcsoa/gen/Administration/_2014_10/__init__.py
--rw-r--r--   0        0        0     1099 2022-10-20 12:41:57.828507 tcsoa-0.9.0/tcsoa/gen/Administration/_2014_10/services.py
--rw-r--r--   0        0        0     1085 2022-10-20 12:42:34.495229 tcsoa-0.9.0/tcsoa/gen/Administration/_2014_10/UserManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.820055 tcsoa-0.9.0/tcsoa/gen/Administration/_2015_03/__init__.py
--rw-r--r--   0        0        0     1301 2022-10-20 12:41:57.860504 tcsoa-0.9.0/tcsoa/gen/Administration/_2015_03/services.py
--rw-r--r--   0        0        0     1474 2022-10-20 12:42:34.528233 tcsoa-0.9.0/tcsoa/gen/Administration/_2015_03/UserManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.798053 tcsoa-0.9.0/tcsoa/gen/Administration/_2015_07/__init__.py
--rw-r--r--   0        0        0     1750 2022-10-20 12:41:57.892509 tcsoa-0.9.0/tcsoa/gen/Administration/_2015_07/services.py
--rw-r--r--   0        0        0     3109 2022-10-20 12:42:34.566256 tcsoa-0.9.0/tcsoa/gen/Administration/_2015_07/UserManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.893059 tcsoa-0.9.0/tcsoa/gen/Administration/_2016_03/__init__.py
--rw-r--r--   0        0        0     1108 2022-10-20 12:41:57.922518 tcsoa-0.9.0/tcsoa/gen/Administration/_2016_03/services.py
--rw-r--r--   0        0        0     1131 2022-10-20 12:42:34.592243 tcsoa-0.9.0/tcsoa/gen/Administration/_2016_03/UserManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.605029 tcsoa-0.9.0/tcsoa/gen/Administration/_2016_10/__init__.py
--rw-r--r--   0        0        0     1912 2022-10-20 12:41:57.954521 tcsoa-0.9.0/tcsoa/gen/Administration/_2016_10/services.py
--rw-r--r--   0        0        0     1411 2022-10-20 12:42:34.619240 tcsoa-0.9.0/tcsoa/gen/Administration/_2016_10/UserManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.845062 tcsoa-0.9.0/tcsoa/gen/Administration/_2017_05/__init__.py
--rw-r--r--   0        0        0     2466 2022-10-20 12:42:34.652250 tcsoa-0.9.0/tcsoa/gen/Administration/_2017_05/GroupManagement.py
--rw-r--r--   0        0        0     1474 2022-10-20 12:42:34.690242 tcsoa-0.9.0/tcsoa/gen/Administration/_2017_05/RoleManagement.py
--rw-r--r--   0        0        0     4086 2022-10-20 12:41:57.999519 tcsoa-0.9.0/tcsoa/gen/Administration/_2017_05/services.py
--rw-r--r--   0        0        0     3489 2022-10-20 12:42:34.742250 tcsoa-0.9.0/tcsoa/gen/Administration/_2017_05/UserManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.670045 tcsoa-0.9.0/tcsoa/gen/Administration/_2018_11/__init__.py
--rw-r--r--   0        0        0     1793 2022-10-20 12:42:34.776251 tcsoa-0.9.0/tcsoa/gen/Administration/_2018_11/IRM.py
--rw-r--r--   0        0        0      519 2022-10-20 12:42:34.802251 tcsoa-0.9.0/tcsoa/gen/Administration/_2018_11/OrganizationManagement.py
--rw-r--r--   0        0        0     5057 2022-10-20 12:41:58.038528 tcsoa-0.9.0/tcsoa/gen/Administration/_2018_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.873056 tcsoa-0.9.0/tcsoa/gen/Administration/__init__.py
--rw-r--r--   0        0        0     5002 2022-10-20 12:41:53.827071 tcsoa-0.9.0/tcsoa/gen/Administration/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.631037 tcsoa-0.9.0/tcsoa/gen/Ai/_2006_03/__init__.py
--rw-r--r--   0        0        0    10627 2022-10-20 12:42:34.986274 tcsoa-0.9.0/tcsoa/gen/Ai/_2006_03/Ai.py
--rw-r--r--   0        0        0    17303 2022-10-20 12:41:58.115532 tcsoa-0.9.0/tcsoa/gen/Ai/_2006_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.941066 tcsoa-0.9.0/tcsoa/gen/Ai/_2007_12/__init__.py
--rw-r--r--   0        0        0     2291 2022-10-20 12:42:35.030283 tcsoa-0.9.0/tcsoa/gen/Ai/_2007_12/Ai.py
--rw-r--r--   0        0        0     4161 2022-10-20 12:41:58.145541 tcsoa-0.9.0/tcsoa/gen/Ai/_2007_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.603029 tcsoa-0.9.0/tcsoa/gen/Ai/_2008_05/__init__.py
--rw-r--r--   0        0        0      500 2022-10-20 12:42:35.058284 tcsoa-0.9.0/tcsoa/gen/Ai/_2008_05/Ai.py
--rw-r--r--   0        0        0     1434 2022-10-20 12:41:58.171544 tcsoa-0.9.0/tcsoa/gen/Ai/_2008_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.992071 tcsoa-0.9.0/tcsoa/gen/Ai/_2008_06/__init__.py
--rw-r--r--   0        0        0     4199 2022-10-20 12:42:35.117281 tcsoa-0.9.0/tcsoa/gen/Ai/_2008_06/Ai.py
--rw-r--r--   0        0        0     5256 2022-10-20 12:41:58.204551 tcsoa-0.9.0/tcsoa/gen/Ai/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.733049 tcsoa-0.9.0/tcsoa/gen/Ai/_2009_06/__init__.py
--rw-r--r--   0        0        0     1052 2022-10-20 12:42:35.145301 tcsoa-0.9.0/tcsoa/gen/Ai/_2009_06/Ai.py
--rw-r--r--   0        0        0     2983 2022-10-20 12:41:58.234551 tcsoa-0.9.0/tcsoa/gen/Ai/_2009_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.854061 tcsoa-0.9.0/tcsoa/gen/Ai/_2009_10/__init__.py
--rw-r--r--   0        0        0     3740 2022-10-20 12:42:35.197300 tcsoa-0.9.0/tcsoa/gen/Ai/_2009_10/Ai.py
--rw-r--r--   0        0        0      746 2022-10-20 12:41:58.266552 tcsoa-0.9.0/tcsoa/gen/Ai/_2009_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.917065 tcsoa-0.9.0/tcsoa/gen/Ai/_2010_09/__init__.py
--rw-r--r--   0        0        0     1025 2022-10-20 12:42:35.226292 tcsoa-0.9.0/tcsoa/gen/Ai/_2010_09/Ai.py
--rw-r--r--   0        0        0     1501 2022-10-20 12:41:58.294555 tcsoa-0.9.0/tcsoa/gen/Ai/_2010_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.600027 tcsoa-0.9.0/tcsoa/gen/Ai/_2012_09/__init__.py
--rw-r--r--   0        0        0     7312 2022-10-20 12:42:35.292300 tcsoa-0.9.0/tcsoa/gen/Ai/_2012_09/Ai.py
--rw-r--r--   0        0        0     3299 2022-10-20 12:41:58.335560 tcsoa-0.9.0/tcsoa/gen/Ai/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.884063 tcsoa-0.9.0/tcsoa/gen/Ai/_2013_05/__init__.py
--rw-r--r--   0        0        0     1121 2022-10-20 12:42:35.321306 tcsoa-0.9.0/tcsoa/gen/Ai/_2013_05/Ai.py
--rw-r--r--   0        0        0     1078 2022-10-20 12:41:58.366562 tcsoa-0.9.0/tcsoa/gen/Ai/_2013_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.701045 tcsoa-0.9.0/tcsoa/gen/Ai/_2013_12/__init__.py
--rw-r--r--   0        0        0     1298 2022-10-20 12:42:35.349307 tcsoa-0.9.0/tcsoa/gen/Ai/_2013_12/Ai.py
--rw-r--r--   0        0        0     1306 2022-10-20 12:41:58.394562 tcsoa-0.9.0/tcsoa/gen/Ai/_2013_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.740043 tcsoa-0.9.0/tcsoa/gen/Ai/_2014_12/__init__.py
--rw-r--r--   0        0        0     4277 2022-10-20 12:42:35.400317 tcsoa-0.9.0/tcsoa/gen/Ai/_2014_12/Ai.py
--rw-r--r--   0        0        0     2972 2022-10-20 12:41:58.424566 tcsoa-0.9.0/tcsoa/gen/Ai/_2014_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.790046 tcsoa-0.9.0/tcsoa/gen/Ai/_2018_06/__init__.py
--rw-r--r--   0        0        0     3465 2022-10-20 12:42:35.445324 tcsoa-0.9.0/tcsoa/gen/Ai/_2018_06/Ai.py
--rw-r--r--   0        0        0     1073 2022-10-20 12:41:58.454575 tcsoa-0.9.0/tcsoa/gen/Ai/_2018_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.684038 tcsoa-0.9.0/tcsoa/gen/Ai/__init__.py
--rw-r--r--   0        0        0     3283 2022-10-20 12:41:53.900085 tcsoa-0.9.0/tcsoa/gen/Ai/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.856060 tcsoa-0.9.0/tcsoa/gen/Allocations/_2007_01/__init__.py
--rw-r--r--   0        0        0     5381 2022-10-20 12:42:35.505318 tcsoa-0.9.0/tcsoa/gen/Allocations/_2007_01/Allocation.py
--rw-r--r--   0        0        0    19838 2022-10-20 12:41:58.507580 tcsoa-0.9.0/tcsoa/gen/Allocations/_2007_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.924063 tcsoa-0.9.0/tcsoa/gen/Allocations/_2011_06/__init__.py
--rw-r--r--   0        0        0     1967 2022-10-20 12:42:35.536322 tcsoa-0.9.0/tcsoa/gen/Allocations/_2011_06/Allocation.py
--rw-r--r--   0        0        0     1694 2022-10-20 12:41:58.538580 tcsoa-0.9.0/tcsoa/gen/Allocations/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.970063 tcsoa-0.9.0/tcsoa/gen/Allocations/__init__.py
--rw-r--r--   0        0        0      999 2022-10-20 12:41:53.927088 tcsoa-0.9.0/tcsoa/gen/Allocations/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.813096 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2007_06/__init__.py
--rw-r--r--   0        0        0     4577 2022-10-20 12:42:35.590329 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2007_06/LicenseManagement.py
--rw-r--r--   0        0        0    10092 2022-10-20 12:41:58.640590 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.791043 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2009_10/__init__.py
--rw-r--r--   0        0        0     4286 2022-10-20 12:42:35.627329 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2009_10/LicenseManagement.py
--rw-r--r--   0        0        0     6740 2022-10-20 12:41:58.672600 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2009_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.958058 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2012_09/__init__.py
--rw-r--r--   0        0        0     4009 2022-10-20 12:42:35.660338 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2012_09/LicenseManagement.py
--rw-r--r--   0        0        0     2984 2022-10-20 12:41:58.702601 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.630037 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2013_05/__init__.py
--rw-r--r--   0        0        0     4319 2022-10-20 12:42:35.694333 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2013_05/LicenseManagement.py
--rw-r--r--   0        0        0     2974 2022-10-20 12:41:58.732621 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2013_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.765045 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2017_05/__init__.py
--rw-r--r--   0        0        0     3408 2022-10-20 12:42:35.730339 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2017_05/LicenseManagement.py
--rw-r--r--   0        0        0     2141 2022-10-20 12:41:58.761600 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2017_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.961068 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2018_06/__init__.py
--rw-r--r--   0        0        0     4145 2022-10-20 12:42:35.761347 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2018_06/LicenseManagement.py
--rw-r--r--   0        0        0     1716 2022-10-20 12:41:58.789632 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2018_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.749045 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/__init__.py
--rw-r--r--   0        0        0     1412 2022-10-20 12:41:53.954089 tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.804052 tcsoa-0.9.0/tcsoa/gen/AWS2/_2016_12/__init__.py
--rw-r--r--   0        0        0     1114 2022-10-20 12:41:57.223444 tcsoa-0.9.0/tcsoa/gen/AWS2/_2016_12/services.py
--rw-r--r--   0        0        0     8797 2022-10-20 12:42:00.480794 tcsoa-0.9.0/tcsoa/gen/AWS2/_2016_12/UiConfig.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.935069 tcsoa-0.9.0/tcsoa/gen/AWS2/_2017_06/__init__.py
--rw-r--r--   0        0        0     1022 2022-10-20 12:41:57.254438 tcsoa-0.9.0/tcsoa/gen/AWS2/_2017_06/services.py
--rw-r--r--   0        0        0     9755 2022-10-20 12:42:00.548795 tcsoa-0.9.0/tcsoa/gen/AWS2/_2017_06/UiConfig.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.608029 tcsoa-0.9.0/tcsoa/gen/AWS2/_2018_12/__init__.py
--rw-r--r--   0        0        0     4807 2022-10-20 12:42:00.595806 tcsoa-0.9.0/tcsoa/gen/AWS2/_2018_12/RequirementsManagement.py
--rw-r--r--   0        0        0     1644 2022-10-20 12:41:57.286453 tcsoa-0.9.0/tcsoa/gen/AWS2/_2018_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.862059 tcsoa-0.9.0/tcsoa/gen/AWS2/__init__.py
--rw-r--r--   0        0        0      476 2022-10-20 12:41:53.726067 tcsoa-0.9.0/tcsoa/gen/AWS2/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.551030 tcsoa-0.9.0/tcsoa/gen/Bom/_2008_06/__init__.py
--rw-r--r--   0        0        0     3694 2022-10-20 12:42:04.185196 tcsoa-0.9.0/tcsoa/gen/Bom/_2008_06/services.py
--rw-r--r--   0        0        0     7236 2022-10-20 12:42:35.830354 tcsoa-0.9.0/tcsoa/gen/Bom/_2008_06/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.563036 tcsoa-0.9.0/tcsoa/gen/Bom/_2010_09/__init__.py
--rw-r--r--   0        0        0     1396 2022-10-20 12:42:04.222201 tcsoa-0.9.0/tcsoa/gen/Bom/_2010_09/services.py
--rw-r--r--   0        0        0     2282 2022-10-20 12:42:35.873352 tcsoa-0.9.0/tcsoa/gen/Bom/_2010_09/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.581034 tcsoa-0.9.0/tcsoa/gen/Bom/__init__.py
--rw-r--r--   0        0        0      562 2022-10-20 12:41:53.966094 tcsoa-0.9.0/tcsoa/gen/Bom/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.818055 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2007_06/__init__.py
--rw-r--r--   0        0        0     3474 2022-10-20 12:42:35.934362 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2007_06/Constants.py
--rw-r--r--   0        0        0     1944 2022-10-20 12:42:35.972366 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2007_06/RulesBasedFramework.py
--rw-r--r--   0        0        0     3221 2022-10-20 12:42:04.268197 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.870055 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2008_06/__init__.py
--rw-r--r--   0        0        0     1560 2022-10-20 12:42:36.008372 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2008_06/ConditionEngine.py
--rw-r--r--   0        0        0     3161 2022-10-20 12:42:36.051381 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2008_06/DeepCopyRules.py
--rw-r--r--   0        0        0     2333 2022-10-20 12:42:04.305197 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.833056 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2010_04/__init__.py
--rw-r--r--   0        0        0     1927 2022-10-20 12:42:36.091379 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2010_04/BusinessRules.py
--rw-r--r--   0        0        0     3054 2022-10-20 12:42:04.335199 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.705043 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2011_06/__init__.py
--rw-r--r--   0        0        0     1000 2022-10-20 12:42:36.124374 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2011_06/Constants.py
--rw-r--r--   0        0        0     1164 2022-10-20 12:42:04.370204 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.806049 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/__init__.py
--rw-r--r--   0        0        0     1208 2022-10-20 12:41:53.983094 tcsoa-0.9.0/tcsoa/gen/BusinessModeler/services.py
--rw-r--r--   0        0        0   196281 2022-10-20 12:42:12.128041 tcsoa-0.9.0/tcsoa/gen/BusinessObjects.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.916066 tcsoa-0.9.0/tcsoa/gen/Cad/_2007_01/__init__.py
--rw-r--r--   0        0        0    29654 2022-10-20 12:42:36.393400 tcsoa-0.9.0/tcsoa/gen/Cad/_2007_01/DataManagement.py
--rw-r--r--   0        0        0    24920 2022-10-20 12:42:12.207055 tcsoa-0.9.0/tcsoa/gen/Cad/_2007_01/services.py
--rw-r--r--   0        0        0    25378 2022-10-20 12:42:36.640422 tcsoa-0.9.0/tcsoa/gen/Cad/_2007_01/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.955069 tcsoa-0.9.0/tcsoa/gen/Cad/_2007_06/__init__.py
--rw-r--r--   0        0        0     4457 2022-10-20 12:42:12.244053 tcsoa-0.9.0/tcsoa/gen/Cad/_2007_06/services.py
--rw-r--r--   0        0        0     6031 2022-10-20 12:42:36.732443 tcsoa-0.9.0/tcsoa/gen/Cad/_2007_06/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.591030 tcsoa-0.9.0/tcsoa/gen/Cad/_2007_09/__init__.py
--rw-r--r--   0        0        0     1116 2022-10-20 12:42:12.274056 tcsoa-0.9.0/tcsoa/gen/Cad/_2007_09/services.py
--rw-r--r--   0        0        0     2375 2022-10-20 12:42:36.784445 tcsoa-0.9.0/tcsoa/gen/Cad/_2007_09/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.844064 tcsoa-0.9.0/tcsoa/gen/Cad/_2007_12/__init__.py
--rw-r--r--   0        0        0     4744 2022-10-20 12:42:36.829449 tcsoa-0.9.0/tcsoa/gen/Cad/_2007_12/DataManagement.py
--rw-r--r--   0        0        0    12455 2022-10-20 12:42:12.326082 tcsoa-0.9.0/tcsoa/gen/Cad/_2007_12/services.py
--rw-r--r--   0        0        0     8702 2022-10-20 12:42:36.921448 tcsoa-0.9.0/tcsoa/gen/Cad/_2007_12/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.599028 tcsoa-0.9.0/tcsoa/gen/Cad/_2008_03/__init__.py
--rw-r--r--   0        0        0     7489 2022-10-20 12:42:36.981461 tcsoa-0.9.0/tcsoa/gen/Cad/_2008_03/DataManagement.py
--rw-r--r--   0        0        0     5350 2022-10-20 12:42:12.367076 tcsoa-0.9.0/tcsoa/gen/Cad/_2008_03/services.py
--rw-r--r--   0        0        0     2066 2022-10-20 12:42:37.021459 tcsoa-0.9.0/tcsoa/gen/Cad/_2008_03/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.687039 tcsoa-0.9.0/tcsoa/gen/Cad/_2008_06/__init__.py
--rw-r--r--   0        0        0    15078 2022-10-20 12:42:37.137488 tcsoa-0.9.0/tcsoa/gen/Cad/_2008_06/DataManagement.py
--rw-r--r--   0        0        0    23532 2022-10-20 12:42:12.430079 tcsoa-0.9.0/tcsoa/gen/Cad/_2008_06/services.py
--rw-r--r--   0        0        0    41331 2022-10-20 12:42:37.446498 tcsoa-0.9.0/tcsoa/gen/Cad/_2008_06/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.553037 tcsoa-0.9.0/tcsoa/gen/Cad/_2009_04/__init__.py
--rw-r--r--   0        0        0     3427 2022-10-20 12:42:12.463082 tcsoa-0.9.0/tcsoa/gen/Cad/_2009_04/services.py
--rw-r--r--   0        0        0     7612 2022-10-20 12:42:37.504502 tcsoa-0.9.0/tcsoa/gen/Cad/_2009_04/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.943068 tcsoa-0.9.0/tcsoa/gen/Cad/_2010_09/__init__.py
--rw-r--r--   0        0        0     4659 2022-10-20 12:42:37.544513 tcsoa-0.9.0/tcsoa/gen/Cad/_2010_09/DataManagement.py
--rw-r--r--   0        0        0     2238 2022-10-20 12:42:12.493079 tcsoa-0.9.0/tcsoa/gen/Cad/_2010_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.631037 tcsoa-0.9.0/tcsoa/gen/Cad/_2011_06/__init__.py
--rw-r--r--   0        0        0     5037 2022-10-20 12:42:37.582517 tcsoa-0.9.0/tcsoa/gen/Cad/_2011_06/DataManagement.py
--rw-r--r--   0        0        0     1866 2022-10-20 12:42:12.523081 tcsoa-0.9.0/tcsoa/gen/Cad/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.966070 tcsoa-0.9.0/tcsoa/gen/Cad/_2012_09/__init__.py
--rw-r--r--   0        0        0    10891 2022-10-20 12:42:37.645516 tcsoa-0.9.0/tcsoa/gen/Cad/_2012_09/DataManagement.py
--rw-r--r--   0        0        0     4218 2022-10-20 12:42:12.553087 tcsoa-0.9.0/tcsoa/gen/Cad/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.710040 tcsoa-0.9.0/tcsoa/gen/Cad/_2013_05/__init__.py
--rw-r--r--   0        0        0    11796 2022-10-20 12:42:12.587090 tcsoa-0.9.0/tcsoa/gen/Cad/_2013_05/services.py
--rw-r--r--   0        0        0    12241 2022-10-20 12:42:37.715523 tcsoa-0.9.0/tcsoa/gen/Cad/_2013_05/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.701045 tcsoa-0.9.0/tcsoa/gen/Cad/_2014_10/__init__.py
--rw-r--r--   0        0        0     2932 2022-10-20 12:42:37.757525 tcsoa-0.9.0/tcsoa/gen/Cad/_2014_10/DataManagement.py
--rw-r--r--   0        0        0     2235 2022-10-20 12:42:12.615098 tcsoa-0.9.0/tcsoa/gen/Cad/_2014_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.578033 tcsoa-0.9.0/tcsoa/gen/Cad/_2016_03/__init__.py
--rw-r--r--   0        0        0    12961 2022-10-20 12:42:37.814539 tcsoa-0.9.0/tcsoa/gen/Cad/_2016_03/DataManagement.py
--rw-r--r--   0        0        0    16904 2022-10-20 12:42:12.654112 tcsoa-0.9.0/tcsoa/gen/Cad/_2016_03/services.py
--rw-r--r--   0        0        0     4554 2022-10-20 12:42:37.849542 tcsoa-0.9.0/tcsoa/gen/Cad/_2016_03/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.786052 tcsoa-0.9.0/tcsoa/gen/Cad/_2016_09/__init__.py
--rw-r--r--   0        0        0    25023 2022-10-20 12:42:12.690109 tcsoa-0.9.0/tcsoa/gen/Cad/_2016_09/services.py
--rw-r--r--   0        0        0    16193 2022-10-20 12:42:37.925553 tcsoa-0.9.0/tcsoa/gen/Cad/_2016_09/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.848063 tcsoa-0.9.0/tcsoa/gen/Cad/_2018_06/__init__.py
--rw-r--r--   0        0        0     3225 2022-10-20 12:42:12.719108 tcsoa-0.9.0/tcsoa/gen/Cad/_2018_06/services.py
--rw-r--r--   0        0        0      967 2022-10-20 12:42:37.953545 tcsoa-0.9.0/tcsoa/gen/Cad/_2018_06/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.919067 tcsoa-0.9.0/tcsoa/gen/Cad/_2019_06/__init__.py
--rw-r--r--   0        0        0     1774 2022-10-20 12:42:12.748117 tcsoa-0.9.0/tcsoa/gen/Cad/_2019_06/services.py
--rw-r--r--   0        0        0     3280 2022-10-20 12:42:37.983547 tcsoa-0.9.0/tcsoa/gen/Cad/_2019_06/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.659037 tcsoa-0.9.0/tcsoa/gen/Cad/_2020_01/__init__.py
--rw-r--r--   0        0        0    39927 2022-10-20 12:42:38.183566 tcsoa-0.9.0/tcsoa/gen/Cad/_2020_01/AppSessionManagement.py
--rw-r--r--   0        0        0     7315 2022-10-20 12:42:12.779119 tcsoa-0.9.0/tcsoa/gen/Cad/_2020_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.823056 tcsoa-0.9.0/tcsoa/gen/Cad/__init__.py
--rw-r--r--   0        0        0     5836 2022-10-20 12:41:54.101115 tcsoa-0.9.0/tcsoa/gen/Cad/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.964078 tcsoa-0.9.0/tcsoa/gen/Cae/_2009_10/__init__.py
--rw-r--r--   0        0        0      579 2022-10-20 12:42:38.210576 tcsoa-0.9.0/tcsoa/gen/Cae/_2009_10/SimulationProcessManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.739050 tcsoa-0.9.0/tcsoa/gen/Cae/_2011_06/__init__.py
--rw-r--r--   0        0        0     4058 2022-10-20 12:42:12.809114 tcsoa-0.9.0/tcsoa/gen/Cae/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.742044 tcsoa-0.9.0/tcsoa/gen/Cae/_2012_02/__init__.py
--rw-r--r--   0        0        0     8588 2022-10-20 12:42:12.843120 tcsoa-0.9.0/tcsoa/gen/Cae/_2012_02/services.py
--rw-r--r--   0        0        0     2589 2022-10-20 12:42:38.238574 tcsoa-0.9.0/tcsoa/gen/Cae/_2012_02/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.653035 tcsoa-0.9.0/tcsoa/gen/Cae/_2013_12/__init__.py
--rw-r--r--   0        0        0     4072 2022-10-20 12:42:12.873126 tcsoa-0.9.0/tcsoa/gen/Cae/_2013_12/services.py
--rw-r--r--   0        0        0     1155 2022-10-20 12:42:38.271574 tcsoa-0.9.0/tcsoa/gen/Cae/_2013_12/SimulationProcessManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.908058 tcsoa-0.9.0/tcsoa/gen/Cae/_2014_06/__init__.py
--rw-r--r--   0        0        0     3756 2022-10-20 12:42:12.902131 tcsoa-0.9.0/tcsoa/gen/Cae/_2014_06/services.py
--rw-r--r--   0        0        0     2232 2022-10-20 12:42:38.302581 tcsoa-0.9.0/tcsoa/gen/Cae/_2014_06/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.815056 tcsoa-0.9.0/tcsoa/gen/Cae/__init__.py
--rw-r--r--   0        0        0      746 2022-10-20 12:41:54.114103 tcsoa-0.9.0/tcsoa/gen/Cae/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.898059 tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2007_01/__init__.py
--rw-r--r--   0        0        0     3944 2022-10-20 12:42:38.378585 tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2007_01/CalendarManagement.py
--rw-r--r--   0        0        0     4731 2022-10-20 12:42:12.937134 tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2007_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.959069 tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2007_06/__init__.py
--rw-r--r--   0        0        0     5023 2022-10-20 12:42:38.444593 tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2007_06/CalendarManagement.py
--rw-r--r--   0        0        0     1474 2022-10-20 12:42:12.970129 tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.802053 tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2008_06/__init__.py
--rw-r--r--   0        0        0     2759 2022-10-20 12:42:38.486594 tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2008_06/CalendarManagement.py
--rw-r--r--   0        0        0     2318 2022-10-20 12:42:13.001139 tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.855059 tcsoa-0.9.0/tcsoa/gen/CalendarManagement/__init__.py
--rw-r--r--   0        0        0      777 2022-10-20 12:41:54.133108 tcsoa-0.9.0/tcsoa/gen/CalendarManagement/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.913065 tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2008_06/__init__.py
--rw-r--r--   0        0        0    14471 2022-10-20 12:42:38.637615 tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2008_06/ChangeManagement.py
--rw-r--r--   0        0        0    26162 2022-10-20 12:42:13.910230 tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.650034 tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2009_06/__init__.py
--rw-r--r--   0        0        0     2160 2022-10-20 12:42:38.675618 tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2009_06/ChangeManagement.py
--rw-r--r--   0        0        0     3595 2022-10-20 12:42:13.940233 tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2009_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.796046 tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2015_10/__init__.py
--rw-r--r--   0        0        0     2438 2022-10-20 12:42:38.718623 tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2015_10/ChangeManagement.py
--rw-r--r--   0        0        0     3127 2022-10-20 12:42:13.972240 tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2015_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.669045 tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2020_01/__init__.py
--rw-r--r--   0        0        0     5286 2022-10-20 12:42:38.762618 tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2020_01/ChangeManagement.py
--rw-r--r--   0        0        0     1822 2022-10-20 12:42:14.005249 tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2020_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.732052 tcsoa-0.9.0/tcsoa/gen/ChangeManagement/__init__.py
--rw-r--r--   0        0        0     1181 2022-10-20 12:41:54.163116 tcsoa-0.9.0/tcsoa/gen/ChangeManagement/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.762045 tcsoa-0.9.0/tcsoa/gen/Classification/_2007_01/__init__.py
--rw-r--r--   0        0        0    25022 2022-10-20 12:42:38.963669 tcsoa-0.9.0/tcsoa/gen/Classification/_2007_01/Classification.py
--rw-r--r--   0        0        0    24353 2022-10-20 12:42:14.095254 tcsoa-0.9.0/tcsoa/gen/Classification/_2007_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.000074 tcsoa-0.9.0/tcsoa/gen/Classification/_2009_10/__init__.py
--rw-r--r--   0        0        0    10587 2022-10-20 12:42:39.045657 tcsoa-0.9.0/tcsoa/gen/Classification/_2009_10/Classification.py
--rw-r--r--   0        0        0     6943 2022-10-20 12:42:14.132262 tcsoa-0.9.0/tcsoa/gen/Classification/_2009_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.845062 tcsoa-0.9.0/tcsoa/gen/Classification/_2011_06/__init__.py
--rw-r--r--   0        0        0     2679 2022-10-20 12:42:39.083655 tcsoa-0.9.0/tcsoa/gen/Classification/_2011_06/Classification.py
--rw-r--r--   0        0        0     2741 2022-10-20 12:42:14.163266 tcsoa-0.9.0/tcsoa/gen/Classification/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.938068 tcsoa-0.9.0/tcsoa/gen/Classification/_2011_12/__init__.py
--rw-r--r--   0        0        0     5226 2022-10-20 12:42:39.148662 tcsoa-0.9.0/tcsoa/gen/Classification/_2011_12/Classification.py
--rw-r--r--   0        0        0     1621 2022-10-20 12:42:14.194262 tcsoa-0.9.0/tcsoa/gen/Classification/_2011_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.812049 tcsoa-0.9.0/tcsoa/gen/Classification/_2015_03/__init__.py
--rw-r--r--   0        0        0     2572 2022-10-20 12:42:39.193661 tcsoa-0.9.0/tcsoa/gen/Classification/_2015_03/Classification.py
--rw-r--r--   0        0        0     2085 2022-10-20 12:42:14.223264 tcsoa-0.9.0/tcsoa/gen/Classification/_2015_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.628039 tcsoa-0.9.0/tcsoa/gen/Classification/_2015_10/__init__.py
--rw-r--r--   0        0        0     3151 2022-10-20 12:42:39.236663 tcsoa-0.9.0/tcsoa/gen/Classification/_2015_10/Classification.py
--rw-r--r--   0        0        0     1279 2022-10-20 12:42:14.251265 tcsoa-0.9.0/tcsoa/gen/Classification/_2015_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.971062 tcsoa-0.9.0/tcsoa/gen/Classification/_2016_03/__init__.py
--rw-r--r--   0        0        0     6926 2022-10-20 12:42:39.308671 tcsoa-0.9.0/tcsoa/gen/Classification/_2016_03/Classification.py
--rw-r--r--   0        0        0     4631 2022-10-20 12:42:14.286276 tcsoa-0.9.0/tcsoa/gen/Classification/_2016_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.764042 tcsoa-0.9.0/tcsoa/gen/Classification/_2016_09/__init__.py
--rw-r--r--   0        0        0     2883 2022-10-20 12:42:39.353677 tcsoa-0.9.0/tcsoa/gen/Classification/_2016_09/Classification.py
--rw-r--r--   0        0        0     2237 2022-10-20 12:42:14.315281 tcsoa-0.9.0/tcsoa/gen/Classification/_2016_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.797053 tcsoa-0.9.0/tcsoa/gen/Classification/__init__.py
--rw-r--r--   0        0        0     2291 2022-10-20 12:41:54.212125 tcsoa-0.9.0/tcsoa/gen/Classification/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.861060 tcsoa-0.9.0/tcsoa/gen/ClassificationCommon/_2020_01/__init__.py
--rw-r--r--   0        0        0     1440 2022-10-20 12:42:14.035253 tcsoa-0.9.0/tcsoa/gen/ClassificationCommon/_2020_01/Classification.py
--rw-r--r--   0        0        0     3739 2022-10-20 12:42:14.349282 tcsoa-0.9.0/tcsoa/gen/ClassificationCommon/_2020_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.729050 tcsoa-0.9.0/tcsoa/gen/ClassificationCommon/_2020_12/__init__.py
--rw-r--r--   0        0        0     3480 2022-10-20 12:42:14.382283 tcsoa-0.9.0/tcsoa/gen/ClassificationCommon/_2020_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.858074 tcsoa-0.9.0/tcsoa/gen/ClassificationCommon/__init__.py
--rw-r--r--   0        0        0      609 2022-10-20 12:41:54.224120 tcsoa-0.9.0/tcsoa/gen/ClassificationCommon/services.py
--rw-r--r--   0        0        0      889 2022-10-20 12:42:39.395686 tcsoa-0.9.0/tcsoa/gen/Common.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.813096 tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2011_06/__init__.py
--rw-r--r--   0        0        0    17164 2022-10-20 12:42:16.906585 tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2011_06/EffectivityManagement.py
--rw-r--r--   0        0        0    46040 2022-10-20 12:42:14.437281 tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.963092 tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2013_05/__init__.py
--rw-r--r--   0        0        0     3870 2022-10-20 12:42:16.953594 tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2013_05/EffectivityManagement.py
--rw-r--r--   0        0        0    18013 2022-10-20 12:42:14.478290 tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2013_05/services.py
--rw-r--r--   0        0        0    13695 2022-10-20 12:42:17.033596 tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2013_05/VariantManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.713049 tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2017_05/__init__.py
--rw-r--r--   0        0        0     1758 2022-10-20 12:42:17.073603 tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2017_05/EffectivityManagement.py
--rw-r--r--   0        0        0     7726 2022-10-20 12:42:14.511293 tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2017_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.667044 tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/__init__.py
--rw-r--r--   0        0        0     1518 2022-10-20 12:41:54.255116 tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.750043 tcsoa-0.9.0/tcsoa/gen/Configuration/_2010_04/__init__.py
--rw-r--r--   0        0        0     7365 2022-10-20 12:42:14.553298 tcsoa-0.9.0/tcsoa/gen/Configuration/_2010_04/services.py
--rw-r--r--   0        0        0     9804 2022-10-20 12:42:39.498703 tcsoa-0.9.0/tcsoa/gen/Configuration/_2010_04/SmartUiBldr.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.644039 tcsoa-0.9.0/tcsoa/gen/Configuration/__init__.py
--rw-r--r--   0        0        0      592 2022-10-20 12:41:54.271125 tcsoa-0.9.0/tcsoa/gen/Configuration/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.996070 tcsoa-0.9.0/tcsoa/gen/Configurator/_2014_12/__init__.py
--rw-r--r--   0        0        0     2233 2022-10-20 12:42:13.046144 tcsoa-0.9.0/tcsoa/gen/Configurator/_2014_12/ConfiguratorManagement.py
--rw-r--r--   0        0        0     2766 2022-10-20 12:42:14.584353 tcsoa-0.9.0/tcsoa/gen/Configurator/_2014_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.616029 tcsoa-0.9.0/tcsoa/gen/Configurator/__init__.py
--rw-r--r--   0        0        0      225 2022-10-20 12:41:54.277124 tcsoa-0.9.0/tcsoa/gen/Configurator/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.609032 tcsoa-0.9.0/tcsoa/gen/Core/_2006_03/__init__.py
--rw-r--r--   0        0        0    12176 2022-10-20 12:42:39.692708 tcsoa-0.9.0/tcsoa/gen/Core/_2006_03/DataManagement.py
--rw-r--r--   0        0        0     5455 2022-10-20 12:42:39.747713 tcsoa-0.9.0/tcsoa/gen/Core/_2006_03/FileManagement.py
--rw-r--r--   0        0        0     1368 2022-10-20 12:42:39.784714 tcsoa-0.9.0/tcsoa/gen/Core/_2006_03/Reservation.py
--rw-r--r--   0        0        0    33500 2022-10-20 12:42:14.682311 tcsoa-0.9.0/tcsoa/gen/Core/_2006_03/services.py
--rw-r--r--   0        0        0     2759 2022-10-20 12:42:39.843721 tcsoa-0.9.0/tcsoa/gen/Core/_2006_03/Session.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.943068 tcsoa-0.9.0/tcsoa/gen/Core/_2007_01/__init__.py
--rw-r--r--   0        0        0    13487 2022-10-20 12:42:40.011741 tcsoa-0.9.0/tcsoa/gen/Core/_2007_01/DataManagement.py
--rw-r--r--   0        0        0     1445 2022-10-20 12:42:40.050739 tcsoa-0.9.0/tcsoa/gen/Core/_2007_01/FileManagement.py
--rw-r--r--   0        0        0     3478 2022-10-20 12:42:40.123752 tcsoa-0.9.0/tcsoa/gen/Core/_2007_01/ManagedRelations.py
--rw-r--r--   0        0        0    21587 2022-10-20 12:42:14.762321 tcsoa-0.9.0/tcsoa/gen/Core/_2007_01/services.py
--rw-r--r--   0        0        0     4657 2022-10-20 12:42:40.178751 tcsoa-0.9.0/tcsoa/gen/Core/_2007_01/Session.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.005088 tcsoa-0.9.0/tcsoa/gen/Core/_2007_06/__init__.py
--rw-r--r--   0        0        0    11098 2022-10-20 12:42:40.320765 tcsoa-0.9.0/tcsoa/gen/Core/_2007_06/DataManagement.py
--rw-r--r--   0        0        0     1299 2022-10-20 12:42:40.361775 tcsoa-0.9.0/tcsoa/gen/Core/_2007_06/LOV.py
--rw-r--r--   0        0        0     3885 2022-10-20 12:42:40.410775 tcsoa-0.9.0/tcsoa/gen/Core/_2007_06/PropDescriptor.py
--rw-r--r--   0        0        0    10963 2022-10-20 12:42:14.825321 tcsoa-0.9.0/tcsoa/gen/Core/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.629037 tcsoa-0.9.0/tcsoa/gen/Core/_2007_09/__init__.py
--rw-r--r--   0        0        0     4979 2022-10-20 12:42:40.476780 tcsoa-0.9.0/tcsoa/gen/Core/_2007_09/DataManagement.py
--rw-r--r--   0        0        0      842 2022-10-20 12:42:40.503783 tcsoa-0.9.0/tcsoa/gen/Core/_2007_09/ProjectLevelSecurity.py
--rw-r--r--   0        0        0     7743 2022-10-20 12:42:14.868332 tcsoa-0.9.0/tcsoa/gen/Core/_2007_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.915058 tcsoa-0.9.0/tcsoa/gen/Core/_2007_12/__init__.py
--rw-r--r--   0        0        0     5967 2022-10-20 12:42:40.585790 tcsoa-0.9.0/tcsoa/gen/Core/_2007_12/DataManagement.py
--rw-r--r--   0        0        0     8982 2022-10-20 12:42:14.912339 tcsoa-0.9.0/tcsoa/gen/Core/_2007_12/services.py
--rw-r--r--   0        0        0      394 2022-10-20 12:42:40.614792 tcsoa-0.9.0/tcsoa/gen/Core/_2007_12/Session.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.678047 tcsoa-0.9.0/tcsoa/gen/Core/_2008_03/__init__.py
--rw-r--r--   0        0        0     4782 2022-10-20 12:42:14.944341 tcsoa-0.9.0/tcsoa/gen/Core/_2008_03/services.py
--rw-r--r--   0        0        0     4528 2022-10-20 12:42:40.669805 tcsoa-0.9.0/tcsoa/gen/Core/_2008_03/Session.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.792046 tcsoa-0.9.0/tcsoa/gen/Core/_2008_05/__init__.py
--rw-r--r--   0        0        0      955 2022-10-20 12:42:14.973340 tcsoa-0.9.0/tcsoa/gen/Core/_2008_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.871054 tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/__init__.py
--rw-r--r--   0        0        0    42394 2022-10-20 12:42:41.012827 tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/DataManagement.py
--rw-r--r--   0        0        0     2947 2022-10-20 12:42:41.056839 tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/DispatcherManagement.py
--rw-r--r--   0        0        0     1023 2022-10-20 12:42:41.090836 tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/ManagedRelations.py
--rw-r--r--   0        0        0     7354 2022-10-20 12:42:41.139843 tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/PropDescriptor.py
--rw-r--r--   0        0        0    44261 2022-10-20 12:42:15.084360 tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/services.py
--rw-r--r--   0        0        0      858 2022-10-20 12:42:41.176875 tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/Session.py
--rw-r--r--   0        0        0     5315 2022-10-20 12:42:41.250849 tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.688041 tcsoa-0.9.0/tcsoa/gen/Core/_2009_04/__init__.py
--rw-r--r--   0        0        0      554 2022-10-20 12:42:41.280853 tcsoa-0.9.0/tcsoa/gen/Core/_2009_04/ProjectLevelSecurity.py
--rw-r--r--   0        0        0     2654 2022-10-20 12:42:15.126355 tcsoa-0.9.0/tcsoa/gen/Core/_2009_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.698047 tcsoa-0.9.0/tcsoa/gen/Core/_2009_10/__init__.py
--rw-r--r--   0        0        0     5649 2022-10-20 12:42:41.351859 tcsoa-0.9.0/tcsoa/gen/Core/_2009_10/DataManagement.py
--rw-r--r--   0        0        0     3174 2022-10-20 12:42:41.396876 tcsoa-0.9.0/tcsoa/gen/Core/_2009_10/ProjectLevelSecurity.py
--rw-r--r--   0        0        0     8459 2022-10-20 12:42:15.167357 tcsoa-0.9.0/tcsoa/gen/Core/_2009_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.969063 tcsoa-0.9.0/tcsoa/gen/Core/_2010_04/__init__.py
--rw-r--r--   0        0        0    13086 2022-10-20 12:42:41.540879 tcsoa-0.9.0/tcsoa/gen/Core/_2010_04/DataManagement.py
--rw-r--r--   0        0        0     2123 2022-10-20 12:42:41.589887 tcsoa-0.9.0/tcsoa/gen/Core/_2010_04/LanguageInformation.py
--rw-r--r--   0        0        0    14216 2022-10-20 12:42:15.228363 tcsoa-0.9.0/tcsoa/gen/Core/_2010_04/services.py
--rw-r--r--   0        0        0     8315 2022-10-20 12:42:41.649888 tcsoa-0.9.0/tcsoa/gen/Core/_2010_04/Session.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.557031 tcsoa-0.9.0/tcsoa/gen/Core/_2010_09/__init__.py
--rw-r--r--   0        0        0    10139 2022-10-20 12:42:41.759900 tcsoa-0.9.0/tcsoa/gen/Core/_2010_09/DataManagement.py
--rw-r--r--   0        0        0     8728 2022-10-20 12:42:15.268373 tcsoa-0.9.0/tcsoa/gen/Core/_2010_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.621029 tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/__init__.py
--rw-r--r--   0        0        0    14393 2022-10-20 12:42:41.870913 tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/DataManagement.py
--rw-r--r--   0        0        0     1534 2022-10-20 12:42:41.908915 tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/LOV.py
--rw-r--r--   0        0        0    11510 2022-10-20 12:42:41.966927 tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/OperationDescriptor.py
--rw-r--r--   0        0        0     3652 2022-10-20 12:42:42.008926 tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/PropDescriptor.py
--rw-r--r--   0        0        0      891 2022-10-20 12:42:42.035926 tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/Reservation.py
--rw-r--r--   0        0        0    22526 2022-10-20 12:42:15.354385 tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/services.py
--rw-r--r--   0        0        0     3130 2022-10-20 12:42:42.077935 tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/Session.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.646039 tcsoa-0.9.0/tcsoa/gen/Core/_2012_02/__init__.py
--rw-r--r--   0        0        0     5350 2022-10-20 12:42:42.139943 tcsoa-0.9.0/tcsoa/gen/Core/_2012_02/DataManagement.py
--rw-r--r--   0        0        0     1284 2022-10-20 12:42:42.174938 tcsoa-0.9.0/tcsoa/gen/Core/_2012_02/OperationDescriptor.py
--rw-r--r--   0        0        0    11281 2022-10-20 12:42:15.406373 tcsoa-0.9.0/tcsoa/gen/Core/_2012_02/services.py
--rw-r--r--   0        0        0      718 2022-10-20 12:42:42.209947 tcsoa-0.9.0/tcsoa/gen/Core/_2012_02/Session.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.999090 tcsoa-0.9.0/tcsoa/gen/Core/_2012_09/__init__.py
--rw-r--r--   0        0        0      951 2022-10-20 12:42:42.238943 tcsoa-0.9.0/tcsoa/gen/Core/_2012_09/DataManagement.py
--rw-r--r--   0        0        0     4809 2022-10-20 12:42:42.315953 tcsoa-0.9.0/tcsoa/gen/Core/_2012_09/ProjectLevelSecurity.py
--rw-r--r--   0        0        0     4626 2022-10-20 12:42:15.455379 tcsoa-0.9.0/tcsoa/gen/Core/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.912057 tcsoa-0.9.0/tcsoa/gen/Core/_2012_10/__init__.py
--rw-r--r--   0        0        0     8089 2022-10-20 12:42:42.376958 tcsoa-0.9.0/tcsoa/gen/Core/_2012_10/DataManagement.py
--rw-r--r--   0        0        0     6317 2022-10-20 12:42:15.492433 tcsoa-0.9.0/tcsoa/gen/Core/_2012_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.930066 tcsoa-0.9.0/tcsoa/gen/Core/_2013_05/__init__.py
--rw-r--r--   0        0        0    24882 2022-10-20 12:42:42.528979 tcsoa-0.9.0/tcsoa/gen/Core/_2013_05/DataManagement.py
--rw-r--r--   0        0        0    14427 2022-10-20 12:42:42.597983 tcsoa-0.9.0/tcsoa/gen/Core/_2013_05/LOV.py
--rw-r--r--   0        0        0    21845 2022-10-20 12:42:15.548393 tcsoa-0.9.0/tcsoa/gen/Core/_2013_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.011070 tcsoa-0.9.0/tcsoa/gen/Core/_2014_06/__init__.py
--rw-r--r--   0        0        0     7307 2022-10-20 12:42:42.657982 tcsoa-0.9.0/tcsoa/gen/Core/_2014_06/DataManagement.py
--rw-r--r--   0        0        0     1984 2022-10-20 12:42:42.700993 tcsoa-0.9.0/tcsoa/gen/Core/_2014_06/DigitalSignature.py
--rw-r--r--   0        0        0    15021 2022-10-20 12:42:15.601395 tcsoa-0.9.0/tcsoa/gen/Core/_2014_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.916066 tcsoa-0.9.0/tcsoa/gen/Core/_2014_10/__init__.py
--rw-r--r--   0        0        0    10059 2022-10-20 12:42:42.785002 tcsoa-0.9.0/tcsoa/gen/Core/_2014_10/DataManagement.py
--rw-r--r--   0        0        0     1727 2022-10-20 12:42:42.819007 tcsoa-0.9.0/tcsoa/gen/Core/_2014_10/ProjectLevelSecurity.py
--rw-r--r--   0        0        0    13780 2022-10-20 12:42:15.656416 tcsoa-0.9.0/tcsoa/gen/Core/_2014_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.802053 tcsoa-0.9.0/tcsoa/gen/Core/_2015_07/__init__.py
--rw-r--r--   0        0        0    22547 2022-10-20 12:42:42.914013 tcsoa-0.9.0/tcsoa/gen/Core/_2015_07/DataManagement.py
--rw-r--r--   0        0        0    14880 2022-10-20 12:42:15.698398 tcsoa-0.9.0/tcsoa/gen/Core/_2015_07/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.916066 tcsoa-0.9.0/tcsoa/gen/Core/_2015_10/__init__.py
--rw-r--r--   0        0        0     2981 2022-10-20 12:42:42.953017 tcsoa-0.9.0/tcsoa/gen/Core/_2015_10/DataManagement.py
--rw-r--r--   0        0        0     3526 2022-10-20 12:42:42.995016 tcsoa-0.9.0/tcsoa/gen/Core/_2015_10/FileManagement.py
--rw-r--r--   0        0        0    14836 2022-10-20 12:42:15.754414 tcsoa-0.9.0/tcsoa/gen/Core/_2015_10/services.py
--rw-r--r--   0        0        0      206 2022-10-20 12:42:43.017014 tcsoa-0.9.0/tcsoa/gen/Core/_2015_10/Session.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.670045 tcsoa-0.9.0/tcsoa/gen/Core/_2016_05/__init__.py
--rw-r--r--   0        0        0     5393 2022-10-20 12:42:43.067024 tcsoa-0.9.0/tcsoa/gen/Core/_2016_05/DataManagement.py
--rw-r--r--   0        0        0     6543 2022-10-20 12:42:15.786417 tcsoa-0.9.0/tcsoa/gen/Core/_2016_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.989074 tcsoa-0.9.0/tcsoa/gen/Core/_2016_09/__init__.py
--rw-r--r--   0        0        0     1312 2022-10-20 12:42:43.099025 tcsoa-0.9.0/tcsoa/gen/Core/_2016_09/DataManagement.py
--rw-r--r--   0        0        0     3885 2022-10-20 12:42:15.815419 tcsoa-0.9.0/tcsoa/gen/Core/_2016_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.734041 tcsoa-0.9.0/tcsoa/gen/Core/_2016_10/__init__.py
--rw-r--r--   0        0        0     1849 2022-10-20 12:42:15.844414 tcsoa-0.9.0/tcsoa/gen/Core/_2016_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.580034 tcsoa-0.9.0/tcsoa/gen/Core/_2017_05/__init__.py
--rw-r--r--   0        0        0     1199 2022-10-20 12:42:43.124033 tcsoa-0.9.0/tcsoa/gen/Core/_2017_05/FileManagement.py
--rw-r--r--   0        0        0    16168 2022-10-20 12:42:43.236038 tcsoa-0.9.0/tcsoa/gen/Core/_2017_05/ProjectLevelSecurity.py
--rw-r--r--   0        0        0    12864 2022-10-20 12:42:15.896428 tcsoa-0.9.0/tcsoa/gen/Core/_2017_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.697040 tcsoa-0.9.0/tcsoa/gen/Core/_2017_11/__init__.py
--rw-r--r--   0        0        0     7279 2022-10-20 12:42:43.346047 tcsoa-0.9.0/tcsoa/gen/Core/_2017_11/LogicalObject.py
--rw-r--r--   0        0        0     6236 2022-10-20 12:42:15.926443 tcsoa-0.9.0/tcsoa/gen/Core/_2017_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.548030 tcsoa-0.9.0/tcsoa/gen/Core/_2018_06/__init__.py
--rw-r--r--   0        0        0     1164 2022-10-20 12:42:43.374049 tcsoa-0.9.0/tcsoa/gen/Core/_2018_06/DataManagement.py
--rw-r--r--   0        0        0     5620 2022-10-20 12:42:43.480059 tcsoa-0.9.0/tcsoa/gen/Core/_2018_06/LogicalObject.py
--rw-r--r--   0        0        0    11606 2022-10-20 12:42:15.964433 tcsoa-0.9.0/tcsoa/gen/Core/_2018_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.562032 tcsoa-0.9.0/tcsoa/gen/Core/_2018_11/__init__.py
--rw-r--r--   0        0        0     4399 2022-10-20 12:42:43.551067 tcsoa-0.9.0/tcsoa/gen/Core/_2018_11/LogicalObject.py
--rw-r--r--   0        0        0     1894 2022-10-20 12:42:43.599076 tcsoa-0.9.0/tcsoa/gen/Core/_2018_11/ProjectLevelSecurity.py
--rw-r--r--   0        0        0    20392 2022-10-20 12:42:16.005442 tcsoa-0.9.0/tcsoa/gen/Core/_2018_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.894059 tcsoa-0.9.0/tcsoa/gen/Core/_2019_06/__init__.py
--rw-r--r--   0        0        0     1121 2022-10-20 12:42:43.630075 tcsoa-0.9.0/tcsoa/gen/Core/_2019_06/DataManagement.py
--rw-r--r--   0        0        0     2465 2022-10-20 12:42:16.043446 tcsoa-0.9.0/tcsoa/gen/Core/_2019_06/services.py
--rw-r--r--   0        0        0     1200 2022-10-20 12:42:43.657079 tcsoa-0.9.0/tcsoa/gen/Core/_2019_06/Session.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.612029 tcsoa-0.9.0/tcsoa/gen/Core/_2020_01/__init__.py
--rw-r--r--   0        0        0     4349 2022-10-20 12:42:43.708084 tcsoa-0.9.0/tcsoa/gen/Core/_2020_01/DataManagement.py
--rw-r--r--   0        0        0     9799 2022-10-20 12:42:43.807099 tcsoa-0.9.0/tcsoa/gen/Core/_2020_01/ProjectLevelSecurity.py
--rw-r--r--   0        0        0    10879 2022-10-20 12:42:16.094451 tcsoa-0.9.0/tcsoa/gen/Core/_2020_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.574032 tcsoa-0.9.0/tcsoa/gen/Core/_2020_04/__init__.py
--rw-r--r--   0        0        0     1872 2022-10-20 12:42:43.835091 tcsoa-0.9.0/tcsoa/gen/Core/_2020_04/DataManagement.py
--rw-r--r--   0        0        0     1465 2022-10-20 12:42:16.124447 tcsoa-0.9.0/tcsoa/gen/Core/_2020_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.640035 tcsoa-0.9.0/tcsoa/gen/Core/__init__.py
--rw-r--r--   0        0        0    17783 2022-10-20 12:41:54.618157 tcsoa-0.9.0/tcsoa/gen/Core/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.682047 tcsoa-0.9.0/tcsoa/gen/Diagramming/_2011_06/__init__.py
--rw-r--r--   0        0        0    12475 2022-10-20 12:42:17.204620 tcsoa-0.9.0/tcsoa/gen/Diagramming/_2011_06/DiagramManagement.py
--rw-r--r--   0        0        0     7023 2022-10-20 12:42:16.163457 tcsoa-0.9.0/tcsoa/gen/Diagramming/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.809054 tcsoa-0.9.0/tcsoa/gen/Diagramming/_2012_09/__init__.py
--rw-r--r--   0        0        0     1696 2022-10-20 12:42:17.237618 tcsoa-0.9.0/tcsoa/gen/Diagramming/_2012_09/DiagramManagement.py
--rw-r--r--   0        0        0     2303 2022-10-20 12:42:16.193454 tcsoa-0.9.0/tcsoa/gen/Diagramming/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.876055 tcsoa-0.9.0/tcsoa/gen/Diagramming/_2014_06/__init__.py
--rw-r--r--   0        0        0     6113 2022-10-20 12:42:17.303626 tcsoa-0.9.0/tcsoa/gen/Diagramming/_2014_06/DNDManagement.py
--rw-r--r--   0        0        0     9098 2022-10-20 12:42:16.230454 tcsoa-0.9.0/tcsoa/gen/Diagramming/_2014_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.732052 tcsoa-0.9.0/tcsoa/gen/Diagramming/__init__.py
--rw-r--r--   0        0        0      775 2022-10-20 12:41:54.634164 tcsoa-0.9.0/tcsoa/gen/Diagramming/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.866073 tcsoa-0.9.0/tcsoa/gen/DocMgmtAw/_2017_06/__init__.py
--rw-r--r--   0        0        0      770 2022-10-20 12:42:16.264456 tcsoa-0.9.0/tcsoa/gen/DocMgmtAw/_2017_06/DocMgmt.py
--rw-r--r--   0        0        0      894 2022-10-20 12:42:16.355472 tcsoa-0.9.0/tcsoa/gen/DocMgmtAw/_2017_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.951068 tcsoa-0.9.0/tcsoa/gen/DocMgmtAw/__init__.py
--rw-r--r--   0        0        0      202 2022-10-20 12:41:54.640164 tcsoa-0.9.0/tcsoa/gen/DocMgmtAw/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.608029 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2007_01/__init__.py
--rw-r--r--   0        0        0     2238 2022-10-20 12:42:43.880106 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2007_01/DocumentTemplate.py
--rw-r--r--   0        0        0     2515 2022-10-20 12:42:16.388488 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2007_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.932066 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2008_06/__init__.py
--rw-r--r--   0        0        0     4375 2022-10-20 12:42:43.957129 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2008_06/DocumentControl.py
--rw-r--r--   0        0        0     5987 2022-10-20 12:42:16.424479 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.738043 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2010_04/__init__.py
--rw-r--r--   0        0        0     1559 2022-10-20 12:42:43.989119 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2010_04/DigitalSignature.py
--rw-r--r--   0        0        0     4286 2022-10-20 12:42:44.044111 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2010_04/LaunchDefinition.py
--rw-r--r--   0        0        0     3820 2022-10-20 12:42:16.460490 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.922066 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2011_06/__init__.py
--rw-r--r--   0        0        0     9082 2022-10-20 12:42:44.136128 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2011_06/AttributeExchange.py
--rw-r--r--   0        0        0     5352 2022-10-20 12:42:16.492481 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.849072 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2013_12/__init__.py
--rw-r--r--   0        0        0     4632 2022-10-20 12:42:44.192134 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2013_12/PrintOrRender.py
--rw-r--r--   0        0        0     2528 2022-10-20 12:42:16.537135 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2013_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.763049 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2018_06/__init__.py
--rw-r--r--   0        0        0     1266 2022-10-20 12:42:16.570140 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2018_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.710040 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2018_11/__init__.py
--rw-r--r--   0        0        0      712 2022-10-20 12:42:44.220130 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2018_11/PrintOrRender.py
--rw-r--r--   0        0        0     3407 2022-10-20 12:42:16.619543 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2018_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.982071 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/__init__.py
--rw-r--r--   0        0        0     1856 2022-10-20 12:41:54.666168 tcsoa-0.9.0/tcsoa/gen/DocumentManagement/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.712045 tcsoa-0.9.0/tcsoa/gen/EditContext/_2014_12/__init__.py
--rw-r--r--   0        0        0     1416 2022-10-20 12:42:16.653537 tcsoa-0.9.0/tcsoa/gen/EditContext/_2014_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.902061 tcsoa-0.9.0/tcsoa/gen/EditContext/_2015_07/__init__.py
--rw-r--r--   0        0        0     1181 2022-10-20 12:42:17.337622 tcsoa-0.9.0/tcsoa/gen/EditContext/_2015_07/DataManagement.py
--rw-r--r--   0        0        0     1459 2022-10-20 12:42:16.683542 tcsoa-0.9.0/tcsoa/gen/EditContext/_2015_07/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.956087 tcsoa-0.9.0/tcsoa/gen/EditContext/_2016_04/__init__.py
--rw-r--r--   0        0        0      820 2022-10-20 12:42:17.365626 tcsoa-0.9.0/tcsoa/gen/EditContext/_2016_04/DataManagement.py
--rw-r--r--   0        0        0     2877 2022-10-20 12:42:16.714530 tcsoa-0.9.0/tcsoa/gen/EditContext/_2016_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.614029 tcsoa-0.9.0/tcsoa/gen/EditContext/_2016_10/__init__.py
--rw-r--r--   0        0        0     2678 2022-10-20 12:42:17.407661 tcsoa-0.9.0/tcsoa/gen/EditContext/_2016_10/DataManagement.py
--rw-r--r--   0        0        0     3003 2022-10-20 12:42:16.745533 tcsoa-0.9.0/tcsoa/gen/EditContext/_2016_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.828056 tcsoa-0.9.0/tcsoa/gen/EditContext/__init__.py
--rw-r--r--   0        0        0      611 2022-10-20 12:41:54.676168 tcsoa-0.9.0/tcsoa/gen/EditContext/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.965064 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2007_06/__init__.py
--rw-r--r--   0        0        0    19857 2022-10-20 12:42:44.372144 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2007_06/ImportExport.py
--rw-r--r--   0        0        0    20382 2022-10-20 12:42:18.723755 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.921064 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2007_12/__init__.py
--rw-r--r--   0        0        0     1041 2022-10-20 12:42:44.411146 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2007_12/ImportExport.py
--rw-r--r--   0        0        0     2960 2022-10-20 12:42:18.756757 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2007_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.877060 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2008_06/__init__.py
--rw-r--r--   0        0        0     2457 2022-10-20 12:42:44.451158 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2008_06/ImportExport.py
--rw-r--r--   0        0        0     3920 2022-10-20 12:42:18.791758 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.920064 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2010_04/__init__.py
--rw-r--r--   0        0        0     2052 2022-10-20 12:42:44.489155 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2010_04/ImportExport.py
--rw-r--r--   0        0        0     3816 2022-10-20 12:42:18.825766 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.596030 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2011_06/__init__.py
--rw-r--r--   0        0        0     2321 2022-10-20 12:42:44.526158 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2011_06/ImportExport.py
--rw-r--r--   0        0        0     2794 2022-10-20 12:42:18.859768 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.012069 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2020_04/__init__.py
--rw-r--r--   0        0        0     1351 2022-10-20 12:42:44.553160 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2020_04/ImportExport.py
--rw-r--r--   0        0        0     2591 2022-10-20 12:42:18.891768 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2020_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.940067 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/__init__.py
--rw-r--r--   0        0        0     2285 2022-10-20 12:41:54.722165 tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.776046 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2007_06/__init__.py
--rw-r--r--   0        0        0     3117 2022-10-20 12:42:44.597166 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2007_06/FileImportExport.py
--rw-r--r--   0        0        0     5436 2022-10-20 12:42:19.327814 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.960068 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2008_06/__init__.py
--rw-r--r--   0        0        0     7324 2022-10-20 12:42:44.652170 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2008_06/FileImportExport.py
--rw-r--r--   0        0        0     9265 2022-10-20 12:42:19.364822 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.660035 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2011_06/__init__.py
--rw-r--r--   0        0        0    16647 2022-10-20 12:42:44.754186 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2011_06/FileImportExport.py
--rw-r--r--   0        0        0    14690 2022-10-20 12:42:19.402815 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.568034 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2012_09/__init__.py
--rw-r--r--   0        0        0     1801 2022-10-20 12:42:44.781185 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2012_09/FileImportExport.py
--rw-r--r--   0        0        0     1613 2022-10-20 12:42:19.432825 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.750043 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2017_11/__init__.py
--rw-r--r--   0        0        0     1734 2022-10-20 12:42:44.816194 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2017_11/FileImportExport.py
--rw-r--r--   0        0        0     2095 2022-10-20 12:42:19.462828 tcsoa-0.9.0/tcsoa/gen/ImportExport/_2017_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.939068 tcsoa-0.9.0/tcsoa/gen/ImportExport/__init__.py
--rw-r--r--   0        0        0     1138 2022-10-20 12:41:54.746176 tcsoa-0.9.0/tcsoa/gen/ImportExport/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.931067 tcsoa-0.9.0/tcsoa/gen/Internal/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.730042 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2012_10/__init__.py
--rw-r--r--   0        0        0     5723 2022-10-20 12:41:58.892622 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2012_10/BOMIndexManagement.py
--rw-r--r--   0        0        0    27548 2022-10-20 12:41:59.084644 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2012_10/OccurrenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.766045 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_03/__init__.py
--rw-r--r--   0        0        0     2082 2022-10-20 12:41:59.121646 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_03/OccurrenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.658041 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_07/__init__.py
--rw-r--r--   0        0        0    12281 2022-10-20 12:41:59.208657 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_07/OccurrenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.763049 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_10/__init__.py
--rw-r--r--   0        0        0      913 2022-10-20 12:41:59.235649 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_10/OccurrenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.694046 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2016_03/__init__.py
--rw-r--r--   0        0        0    10612 2022-10-20 12:41:59.311673 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2016_03/OccurrenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.789043 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_06/__init__.py
--rw-r--r--   0        0        0     3794 2022-10-20 12:41:59.353666 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_06/OccurrenceConfiguration.py
--rw-r--r--   0        0        0    11699 2022-10-20 12:41:59.426672 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_06/OccurrenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.820055 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_12/__init__.py
--rw-r--r--   0        0        0     4406 2022-10-20 12:41:59.476680 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_12/OccurrenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.827050 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_05/__init__.py
--rw-r--r--   0        0        0      937 2022-10-20 12:41:59.504698 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_05/Compare.py
--rw-r--r--   0        0        0     4617 2022-10-20 12:41:59.559687 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_05/OccurrenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.865059 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_12/__init__.py
--rw-r--r--   0        0        0    11014 2022-10-20 12:41:59.611692 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_12/Compare.py
--rw-r--r--   0        0        0      664 2022-10-20 12:41:59.638698 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_12/Markup.py
--rw-r--r--   0        0        0    13867 2022-10-20 12:41:59.713710 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_12/OccurrenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.980065 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_06/__init__.py
--rw-r--r--   0        0        0     1859 2022-10-20 12:41:59.748710 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_06/Compare.py
--rw-r--r--   0        0        0    22465 2022-10-20 12:41:59.858726 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_06/OccurrenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.771052 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_12/__init__.py
--rw-r--r--   0        0        0     2280 2022-10-20 12:41:59.898734 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_12/DataManagement.py
--rw-r--r--   0        0        0     7862 2022-10-20 12:41:59.975733 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_12/OccurrenceConfiguration.py
--rw-r--r--   0        0        0    20998 2022-10-20 12:42:00.099748 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_12/OccurrenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.892058 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2020_05/__init__.py
--rw-r--r--   0        0        0     2126 2022-10-20 12:42:00.133755 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2020_05/OccurrenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.586038 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2020_12/__init__.py
--rw-r--r--   0        0        0     9877 2022-10-20 12:42:00.217763 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2020_12/OccurrenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.928070 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.791043 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceVis/_2014_11/__init__.py
--rw-r--r--   0        0        0     2642 2022-10-20 12:42:03.985175 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceVis/_2014_11/OccurrenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.780047 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceVis/_2015_03/__init__.py
--rw-r--r--   0        0        0    13386 2022-10-20 12:42:04.103175 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceVis/_2015_03/MassiveModelVisualization.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.794044 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceVis/_2018_05/__init__.py
--rw-r--r--   0        0        0     2695 2022-10-20 12:42:04.148180 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceVis/_2018_05/MassiveModelVisualization.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.683038 tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceVis/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.721045 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2007_06/__init__.py
--rw-r--r--   0        0        0     2612 2022-10-20 12:42:44.861189 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2007_06/Authorization.py
--rw-r--r--   0        0        0     5400 2022-10-20 12:42:44.931196 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2007_06/PreferenceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.577032 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2008_06/__init__.py
--rw-r--r--   0        0        0      985 2022-10-20 12:42:44.965199 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2008_06/IRM.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.637041 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2009_10/__init__.py
--rw-r--r--   0        0        0     1060 2022-10-20 12:42:45.000199 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2009_10/PersonManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.708044 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2011_06/__init__.py
--rw-r--r--   0        0        0     3412 2022-10-20 12:42:45.058205 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2011_06/OrganizationManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.859054 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2012_10/__init__.py
--rw-r--r--   0        0        0     2936 2022-10-20 12:42:45.099213 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2012_10/OrganizationManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.684038 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2013_05/__init__.py
--rw-r--r--   0        0        0     1716 2022-10-20 12:42:45.140214 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2013_05/UserManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.636038 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2014_10/__init__.py
--rw-r--r--   0        0        0     1060 2022-10-20 12:42:45.168226 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2014_10/UserManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.554031 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2016_09/__init__.py
--rw-r--r--   0        0        0      972 2022-10-20 12:42:45.196226 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2016_09/VolumeManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.727040 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2017_11/__init__.py
--rw-r--r--   0        0        0     1297 2022-10-20 12:42:45.229220 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2017_11/IRM.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.581034 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2018_11/__init__.py
--rw-r--r--   0        0        0     2198 2022-10-20 12:42:45.268226 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2018_11/SiteManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.847066 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2019_06/__init__.py
--rw-r--r--   0        0        0     3615 2022-10-20 12:42:45.312236 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2019_06/UserManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.860082 tcsoa-0.9.0/tcsoa/gen/Internal/Administration/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.886054 tcsoa-0.9.0/tcsoa/gen/Internal/Ai/_2008_06/__init__.py
--rw-r--r--   0        0        0     2306 2022-10-20 12:42:45.349233 tcsoa-0.9.0/tcsoa/gen/Internal/Ai/_2008_06/Ai.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.757046 tcsoa-0.9.0/tcsoa/gen/Internal/Ai/_2016_03/__init__.py
--rw-r--r--   0        0        0     3067 2022-10-20 12:42:45.382240 tcsoa-0.9.0/tcsoa/gen/Internal/Ai/_2016_03/Ai.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.949068 tcsoa-0.9.0/tcsoa/gen/Internal/Ai/_2016_04/__init__.py
--rw-r--r--   0        0        0      703 2022-10-20 12:42:45.408244 tcsoa-0.9.0/tcsoa/gen/Internal/Ai/_2016_04/Ai.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.837052 tcsoa-0.9.0/tcsoa/gen/Internal/Ai/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.810050 tcsoa-0.9.0/tcsoa/gen/Internal/AuditManager/_2012_09/__init__.py
--rw-r--r--   0        0        0     1944 2022-10-20 12:42:17.443640 tcsoa-0.9.0/tcsoa/gen/Internal/AuditManager/_2012_09/ProcessHistoryManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.604032 tcsoa-0.9.0/tcsoa/gen/Internal/AuditManager/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.723044 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/__init__.py
--rw-r--r--   0        0        0    10147 2022-10-20 12:42:00.713834 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/DataManagement.py
--rw-r--r--   0        0        0     2650 2022-10-20 12:42:00.769824 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/Finder.py
--rw-r--r--   0        0        0    14461 2022-10-20 12:42:00.951843 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/FullTextSearch.py
--rw-r--r--   0        0        0    12834 2022-10-20 12:42:01.025862 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/LOV.py
--rw-r--r--   0        0        0     2167 2022-10-20 12:42:01.064858 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/OrganizationManagement.py
--rw-r--r--   0        0        0     1877 2022-10-20 12:42:01.107857 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/RequirementsManagement.py
--rw-r--r--   0        0        0     2094 2022-10-20 12:42:01.141861 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/StructureSearch.py
--rw-r--r--   0        0        0      784 2022-10-20 12:42:01.174866 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.993077 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2013_12/__init__.py
--rw-r--r--   0        0        0     2311 2022-10-20 12:42:01.215863 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2013_12/DataManagement.py
--rw-r--r--   0        0        0     2888 2022-10-20 12:42:01.243868 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2013_12/OrganizationManagement.py
--rw-r--r--   0        0        0     6037 2022-10-20 12:42:01.288876 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2013_12/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.828056 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2014_11/__init__.py
--rw-r--r--   0        0        0     2712 2022-10-20 12:42:01.320883 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2014_11/RequirementsManagement.py
--rw-r--r--   0        0        0     7420 2022-10-20 12:42:01.397887 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2014_11/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.741045 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2015_03/__init__.py
--rw-r--r--   0        0        0     4797 2022-10-20 12:42:01.437903 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2015_03/DataManagement.py
--rw-r--r--   0        0        0     2036 2022-10-20 12:42:01.476901 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2015_03/FullTextSearch.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.819055 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2015_10/__init__.py
--rw-r--r--   0        0        0     3481 2022-10-20 12:42:01.522904 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2015_10/DataManagement.py
--rw-r--r--   0        0        0     6979 2022-10-20 12:42:01.582913 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2015_10/FullTextSearch.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.546029 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_03/__init__.py
--rw-r--r--   0        0        0     7872 2022-10-20 12:42:01.642913 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_03/DataManagement.py
--rw-r--r--   0        0        0    16769 2022-10-20 12:42:01.743928 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_03/Finder.py
--rw-r--r--   0        0        0     2161 2022-10-20 12:42:01.774936 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_03/RequirementsManagement.py
--rw-r--r--   0        0        0    12608 2022-10-20 12:42:01.860942 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_03/UiConfig.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.954086 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_04/__init__.py
--rw-r--r--   0        0        0    14676 2022-10-20 12:42:01.956947 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_04/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.725040 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_12/__init__.py
--rw-r--r--   0        0        0      968 2022-10-20 12:42:01.992961 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_12/AdvancedSearch.py
--rw-r--r--   0        0        0     8292 2022-10-20 12:42:02.067964 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_12/DataManagement.py
--rw-r--r--   0        0        0     4244 2022-10-20 12:42:02.104974 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_12/Finder.py
--rw-r--r--   0        0        0     5616 2022-10-20 12:42:02.160968 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_12/RequirementsManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.628039 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_06/__init__.py
--rw-r--r--   0        0        0    19075 2022-10-20 12:42:02.310991 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_06/DataManagement.py
--rw-r--r--   0        0        0      818 2022-10-20 12:42:02.338989 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_06/EffectivityManagment.py
--rw-r--r--   0        0        0    11744 2022-10-20 12:42:02.403994 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_06/Finder.py
--rw-r--r--   0        0        0     1383 2022-10-20 12:42:02.438001 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_06/FullTextSearch.py
--rw-r--r--   0        0        0     5300 2022-10-20 12:42:02.481999 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_06/RequirementsManagement.py
--rw-r--r--   0        0        0      998 2022-10-20 12:42:02.510012 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_06/UiConfig.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.541030 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_12/__init__.py
--rw-r--r--   0        0        0    14030 2022-10-20 12:42:02.593015 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_12/DataManagement.py
--rw-r--r--   0        0        0     4364 2022-10-20 12:42:02.629020 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_12/Finder.py
--rw-r--r--   0        0        0     2523 2022-10-20 12:42:02.671019 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_12/FullTextSearch.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.691046 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_05/__init__.py
--rw-r--r--   0        0        0     9857 2022-10-20 12:42:02.745029 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_05/DataManagement.py
--rw-r--r--   0        0        0     2327 2022-10-20 12:42:02.783034 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_05/FileMgmt.py
--rw-r--r--   0        0        0     8632 2022-10-20 12:42:02.834046 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_05/Finder.py
--rw-r--r--   0        0        0     6088 2022-10-20 12:42:02.869042 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_05/FullTextSearch.py
--rw-r--r--   0        0        0     1176 2022-10-20 12:42:02.908049 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_05/TCXML.py
--rw-r--r--   0        0        0     3702 2022-10-20 12:42:02.945058 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_05/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.981072 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_12/__init__.py
--rw-r--r--   0        0        0     1273 2022-10-20 12:42:02.973061 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_12/Finder.py
--rw-r--r--   0        0        0     1301 2022-10-20 12:42:03.005066 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_12/MultiSite.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.701045 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2019_06/__init__.py
--rw-r--r--   0        0        0     4821 2022-10-20 12:42:03.051078 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2019_06/AdvancedSavedSearch.py
--rw-r--r--   0        0        0    11263 2022-10-20 12:42:03.115076 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2019_06/Finder.py
--rw-r--r--   0        0        0     2364 2022-10-20 12:42:03.158081 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2019_06/RequirementsManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.880064 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2019_12/__init__.py
--rw-r--r--   0        0        0     4349 2022-10-20 12:42:03.214082 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2019_12/DataManagement.py
--rw-r--r--   0        0        0     4772 2022-10-20 12:42:03.271094 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2019_12/Finder.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.800055 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2020_05/__init__.py
--rw-r--r--   0        0        0     1652 2022-10-20 12:42:03.308091 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2020_05/DataManagement.py
--rw-r--r--   0        0        0     1614 2022-10-20 12:42:03.341102 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2020_05/FileMgmt.py
--rw-r--r--   0        0        0     3163 2022-10-20 12:42:03.376104 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2020_05/FullTextSearch.py
--rw-r--r--   0        0        0     4921 2022-10-20 12:42:03.419110 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2020_05/UiConfig.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.927060 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2020_12/__init__.py
--rw-r--r--   0        0        0     4299 2022-10-20 12:42:03.483116 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2020_12/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.687039 tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.984066 tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2007_01/__init__.py
--rw-r--r--   0        0        0     1245 2022-10-20 12:42:45.441252 tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2007_01/DataModelManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.754044 tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2010_04/__init__.py
--rw-r--r--   0        0        0     2808 2022-10-20 12:42:45.489254 tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2010_04/DataModelManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.617030 tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2010_09/__init__.py
--rw-r--r--   0        0        0     1763 2022-10-20 12:42:45.522250 tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2010_09/DataModelManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.690037 tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2011_06/__init__.py
--rw-r--r--   0        0        0      814 2022-10-20 12:42:45.549252 tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2011_06/DataModelManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.550029 tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2013_05/__init__.py
--rw-r--r--   0        0        0     5023 2022-10-20 12:42:45.591255 tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2013_05/DynamicLOVQuery.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.957067 tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.688041 tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2008_03/__init__.py
--rw-r--r--   0        0        0     1903 2022-10-20 12:42:45.630260 tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2008_03/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.993077 tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2008_05/__init__.py
--rw-r--r--   0        0        0     4621 2022-10-20 12:42:45.672261 tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2008_05/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.925062 tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2008_06/__init__.py
--rw-r--r--   0        0        0     5889 2022-10-20 12:42:45.744276 tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2008_06/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.010070 tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2010_04/__init__.py
--rw-r--r--   0        0        0    13165 2022-10-20 12:42:45.831279 tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2010_04/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.718047 tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2013_05/__init__.py
--rw-r--r--   0        0        0     7003 2022-10-20 12:42:45.903283 tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2013_05/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.681046 tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2017_05/__init__.py
--rw-r--r--   0        0        0     7838 2022-10-20 12:42:45.976290 tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2017_05/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.978069 tcsoa-0.9.0/tcsoa/gen/Internal/Cad/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.665047 tcsoa-0.9.0/tcsoa/gen/Internal/Cae/_2011_06/__init__.py
--rw-r--r--   0        0        0     2592 2022-10-20 12:42:46.003294 tcsoa-0.9.0/tcsoa/gen/Internal/Cae/_2011_06/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.592028 tcsoa-0.9.0/tcsoa/gen/Internal/Cae/_2013_05/__init__.py
--rw-r--r--   0        0        0      767 2022-10-20 12:42:46.030300 tcsoa-0.9.0/tcsoa/gen/Internal/Cae/_2013_05/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.542030 tcsoa-0.9.0/tcsoa/gen/Internal/Cae/_2014_06/__init__.py
--rw-r--r--   0        0        0     2233 2022-10-20 12:42:46.066308 tcsoa-0.9.0/tcsoa/gen/Internal/Cae/_2014_06/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.651040 tcsoa-0.9.0/tcsoa/gen/Internal/Cae/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.652035 tcsoa-0.9.0/tcsoa/gen/Internal/ChangeManagement/_2012_10/__init__.py
--rw-r--r--   0        0        0     2948 2022-10-20 12:42:46.110311 tcsoa-0.9.0/tcsoa/gen/Internal/ChangeManagement/_2012_10/ChangeManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.808050 tcsoa-0.9.0/tcsoa/gen/Internal/ChangeManagement/_2015_03/__init__.py
--rw-r--r--   0        0        0     7390 2022-10-20 12:42:46.172312 tcsoa-0.9.0/tcsoa/gen/Internal/ChangeManagement/_2015_03/ChangeManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.719040 tcsoa-0.9.0/tcsoa/gen/Internal/ChangeManagement/_2020_01/__init__.py
--rw-r--r--   0        0        0     1464 2022-10-20 12:42:46.211323 tcsoa-0.9.0/tcsoa/gen/Internal/ChangeManagement/_2020_01/MassUpdate.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.959069 tcsoa-0.9.0/tcsoa/gen/Internal/ChangeManagement/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.945063 tcsoa-0.9.0/tcsoa/gen/Internal/Classification/_2009_10/__init__.py
--rw-r--r--   0        0        0     2570 2022-10-20 12:42:46.253322 tcsoa-0.9.0/tcsoa/gen/Internal/Classification/_2009_10/Classification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.988072 tcsoa-0.9.0/tcsoa/gen/Internal/Classification/_2017_05/__init__.py
--rw-r--r--   0        0        0     5883 2022-10-20 12:42:46.298328 tcsoa-0.9.0/tcsoa/gen/Internal/Classification/_2017_05/Classification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.937067 tcsoa-0.9.0/tcsoa/gen/Internal/Classification/_2018_11/__init__.py
--rw-r--r--   0        0        0     2172 2022-10-20 12:42:46.335326 tcsoa-0.9.0/tcsoa/gen/Internal/Classification/_2018_11/Classification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.900053 tcsoa-0.9.0/tcsoa/gen/Internal/Classification/_2020_04/__init__.py
--rw-r--r--   0        0        0     7976 2022-10-20 12:42:46.400335 tcsoa-0.9.0/tcsoa/gen/Internal/Classification/_2020_04/Classification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.796046 tcsoa-0.9.0/tcsoa/gen/Internal/Classification/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.779053 tcsoa-0.9.0/tcsoa/gen/Internal/ConfigFilterCriteria/_2013_12/__init__.py
--rw-r--r--   0        0        0      805 2022-10-20 12:42:17.477662 tcsoa-0.9.0/tcsoa/gen/Internal/ConfigFilterCriteria/_2013_12/VariantManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.717049 tcsoa-0.9.0/tcsoa/gen/Internal/ConfigFilterCriteria/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.588032 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2014_06/__init__.py
--rw-r--r--   0        0        0    66424 2022-10-20 12:42:13.348173 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2014_06/ConfiguratorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.611029 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2014_12/__init__.py
--rw-r--r--   0        0        0     6953 2022-10-20 12:42:13.425214 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2014_12/ConfiguratorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.850060 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2015_03/__init__.py
--rw-r--r--   0        0        0     4034 2022-10-20 12:42:13.463190 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2015_03/ConfiguratorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.006070 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2015_10/__init__.py
--rw-r--r--   0        0        0    25096 2022-10-20 12:42:13.638206 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2015_10/ConfiguratorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.986071 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2016_09/__init__.py
--rw-r--r--   0        0        0     3581 2022-10-20 12:42:13.692217 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2016_09/ConfiguratorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.610029 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2017_11/__init__.py
--rw-r--r--   0        0        0     4325 2022-10-20 12:42:13.732241 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2017_11/ConfiguratorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.790046 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2018_06/__init__.py
--rw-r--r--   0        0        0     9718 2022-10-20 12:42:13.825222 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2018_06/ConfiguratorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.808050 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2018_11/__init__.py
--rw-r--r--   0        0        0     1118 2022-10-20 12:42:13.859224 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2018_11/ConfiguratorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.567031 tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.900053 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2007_01/__init__.py
--rw-r--r--   0        0        0     3949 2022-10-20 12:42:46.457338 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2007_01/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.656040 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2007_06/__init__.py
--rw-r--r--   0        0        0     4699 2022-10-20 12:42:46.531347 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2007_06/ProjectLevelSecurity.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.692046 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2007_09/__init__.py
--rw-r--r--   0        0        0     1390 2022-10-20 12:42:46.569347 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2007_09/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.861060 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2008_06/__init__.py
--rw-r--r--   0        0        0     4549 2022-10-20 12:42:46.633371 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2008_06/DataManagement.py
--rw-r--r--   0        0        0     7569 2022-10-20 12:42:46.721371 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2008_06/DispatcherManagement.py
--rw-r--r--   0        0        0     9953 2022-10-20 12:42:46.805372 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2008_06/FileManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.876055 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2009_10/__init__.py
--rw-r--r--   0        0        0     1765 2022-10-20 12:42:46.841379 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2009_10/Thumbnail.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.696047 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2010_04/__init__.py
--rw-r--r--   0        0        0     1235 2022-10-20 12:42:46.872391 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2010_04/DataManagement.py
--rw-r--r--   0        0        0     2042 2022-10-20 12:42:46.910380 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2010_04/ProjectLevelSecurity.py
--rw-r--r--   0        0        0     1198 2022-10-20 12:42:46.944382 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2010_04/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.725040 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2010_09/__init__.py
--rw-r--r--   0        0        0     2858 2022-10-20 12:42:46.998386 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2010_09/DataManagement.py
--rw-r--r--   0        0        0     1021 2022-10-20 12:42:47.025405 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2010_09/FileManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.635041 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2011_06/__init__.py
--rw-r--r--   0        0        0     1297 2022-10-20 12:42:47.076394 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2011_06/ICT.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.944079 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2012_02/__init__.py
--rw-r--r--   0        0        0     2490 2022-10-20 12:42:47.113407 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2012_02/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.973071 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2012_09/__init__.py
--rw-r--r--   0        0        0     1836 2022-10-20 12:42:47.140407 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2012_09/Envelope.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.756046 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2012_10/__init__.py
--rw-r--r--   0        0        0     3420 2022-10-20 12:42:47.182412 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2012_10/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.545030 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2013_05/__init__.py
--rw-r--r--   0        0        0     1957 2022-10-20 12:42:47.219410 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2013_05/Licensing.py
--rw-r--r--   0        0        0     4651 2022-10-20 12:42:47.272419 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2013_05/PresentationManagement.py
--rw-r--r--   0        0        0     1071 2022-10-20 12:42:47.303422 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2013_05/ProjectLevelSecurity.py
--rw-r--r--   0        0        0      882 2022-10-20 12:42:47.331428 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2013_05/Thumbnail.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.647036 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2014_10/__init__.py
--rw-r--r--   0        0        0     1951 2022-10-20 12:42:47.367426 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2014_10/FileManagement.py
--rw-r--r--   0        0        0     1273 2022-10-20 12:42:47.395427 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2014_10/Licensing.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.580034 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2016_10/__init__.py
--rw-r--r--   0        0        0     2822 2022-10-20 12:42:47.430428 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2016_10/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.566032 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2017_05/__init__.py
--rw-r--r--   0        0        0     1044 2022-10-20 12:42:47.457440 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2017_05/FileManagement.py
--rw-r--r--   0        0        0     5339 2022-10-20 12:42:47.502439 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2017_05/PresentationManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.789043 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2017_11/__init__.py
--rw-r--r--   0        0        0     4694 2022-10-20 12:42:47.538438 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2017_11/DataManagement.py
--rw-r--r--   0        0        0     5855 2022-10-20 12:42:47.601442 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2017_11/LogicalObject.py
--rw-r--r--   0        0        0     1749 2022-10-20 12:42:47.641449 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2017_11/Type.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.000074 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2018_06/__init__.py
--rw-r--r--   0        0        0     5176 2022-10-20 12:42:47.691451 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2018_06/LogicalObject.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.672047 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2018_11/__init__.py
--rw-r--r--   0        0        0     1209 2022-10-20 12:42:47.724459 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2018_11/FileManagement.py
--rw-r--r--   0        0        0     2261 2022-10-20 12:42:47.763460 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2018_11/LogicalObject.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.584030 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2018_12/__init__.py
--rw-r--r--   0        0        0     1647 2022-10-20 12:42:47.792462 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2018_12/Licensing.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.841051 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2020_01/__init__.py
--rw-r--r--   0        0        0     7334 2022-10-20 12:42:47.835465 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2020_01/ActiveModeler.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.728040 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2020_04/__init__.py
--rw-r--r--   0        0        0     1965 2022-10-20 12:42:47.867471 tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2020_04/LogicalObject.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.657040 tcsoa-0.9.0/tcsoa/gen/Internal/Core/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.847066 tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2011_06/__init__.py
--rw-r--r--   0        0        0     4042 2022-10-20 12:42:17.551644 tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2011_06/DebugLogging.py
--rw-r--r--   0        0        0    11293 2022-10-20 12:42:17.649658 tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2011_06/DebugMonitor.py
--rw-r--r--   0        0        0      638 2022-10-20 12:42:17.676661 tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2011_06/PerformanceMonitor.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.544029 tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2014_06/__init__.py
--rw-r--r--   0        0        0     3244 2022-10-20 12:42:17.721665 tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2014_06/JournalBasedTesting.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.648033 tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2015_07/__init__.py
--rw-r--r--   0        0        0      417 2022-10-20 12:42:17.751678 tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2015_07/DebugLogging.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.801055 tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2015_10/__init__.py
--rw-r--r--   0        0        0      772 2022-10-20 12:42:17.780675 tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2015_10/JournalBasedTesting.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.561031 tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2019_06/__init__.py
--rw-r--r--   0        0        0      703 2022-10-20 12:42:17.809675 tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2019_06/DebugLogging.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.633041 tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.011070 tcsoa-0.9.0/tcsoa/gen/Internal/DocMgmtAw/_2019_06/__init__.py
--rw-r--r--   0        0        0     1133 2022-10-20 12:42:16.296456 tcsoa-0.9.0/tcsoa/gen/Internal/DocMgmtAw/_2019_06/DocMgmt.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.812049 tcsoa-0.9.0/tcsoa/gen/Internal/DocMgmtAw/_2019_12/__init__.py
--rw-r--r--   0        0        0      735 2022-10-20 12:42:16.325466 tcsoa-0.9.0/tcsoa/gen/Internal/DocMgmtAw/_2019_12/DocMgmt.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.951068 tcsoa-0.9.0/tcsoa/gen/Internal/DocMgmtAw/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.797053 tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/_2008_06/__init__.py
--rw-r--r--   0        0        0     2010 2022-10-20 12:42:47.905475 tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/_2008_06/DispatcherManagement.py
--rw-r--r--   0        0        0      554 2022-10-20 12:42:47.951477 tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/_2008_06/DocumentControl.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.925062 tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/_2013_05/__init__.py
--rw-r--r--   0        0        0      712 2022-10-20 12:42:47.983492 tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/_2013_05/DigitalSignature.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.921064 tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/_2013_12/__init__.py
--rw-r--r--   0        0        0      757 2022-10-20 12:42:48.009488 tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/_2013_12/Markup.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.742044 tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/_2020_12/__init__.py
--rw-r--r--   0        0        0     1628 2022-10-20 12:42:48.041486 tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/_2020_12/AttributeExchange.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.620029 tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.630037 tcsoa-0.9.0/tcsoa/gen/Internal/EntCba/_2019_12/__init__.py
--rw-r--r--   0        0        0      821 2022-10-20 12:42:00.244774 tcsoa-0.9.0/tcsoa/gen/Internal/EntCba/_2019_12/Alignments.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.746044 tcsoa-0.9.0/tcsoa/gen/Internal/EntCba/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.953082 tcsoa-0.9.0/tcsoa/gen/Internal/Gdis/_2006_03/__init__.py
--rw-r--r--   0        0        0      859 2022-10-20 12:42:48.074487 tcsoa-0.9.0/tcsoa/gen/Internal/Gdis/_2006_03/Reporting.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.668044 tcsoa-0.9.0/tcsoa/gen/Internal/Gdis/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.696047 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2007_06/__init__.py
--rw-r--r--   0        0        0     2313 2022-10-20 12:42:48.111491 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2007_06/Briefcase.py
--rw-r--r--   0        0        0     6894 2022-10-20 12:42:48.187500 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2007_06/ImportExport.py
--rw-r--r--   0        0        0     3167 2022-10-20 12:42:48.245511 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2007_06/Synchronizer.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.767045 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2008_06/__init__.py
--rw-r--r--   0        0        0     2028 2022-10-20 12:42:48.282517 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2008_06/Synchronizer.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.663035 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2010_02/__init__.py
--rw-r--r--   0        0        0     1256 2022-10-20 12:42:48.320508 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2010_02/LowlevelOwnershipTransfer.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.638044 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2017_05/__init__.py
--rw-r--r--   0        0        0      993 2022-10-20 12:42:48.347511 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2017_05/ImportExport.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.985066 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2018_11/__init__.py
--rw-r--r--   0        0        0     3560 2022-10-20 12:42:48.385516 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2018_11/Briefcase.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.874054 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2020_01/__init__.py
--rw-r--r--   0        0        0     4886 2022-10-20 12:42:48.450523 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2020_01/Briefcase.py
--rw-r--r--   0        0        0     2734 2022-10-20 12:42:48.492528 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2020_01/OwnershipRecovery.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.843052 tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.864060 tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2017_06/__init__.py
--rw-r--r--   0        0        0     2157 2022-10-20 12:42:18.932771 tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2017_06/Author.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.722046 tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2017_12/__init__.py
--rw-r--r--   0        0        0    14621 2022-10-20 12:42:19.044795 tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2017_12/Author.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.641039 tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2018_05/__init__.py
--rw-r--r--   0        0        0    17309 2022-10-20 12:42:19.158820 tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2018_05/Classification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.922066 tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2018_12/__init__.py
--rw-r--r--   0        0        0     6929 2022-10-20 12:42:19.216807 tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2018_12/Classification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.930066 tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2019_06/__init__.py
--rw-r--r--   0        0        0     1098 2022-10-20 12:42:19.244803 tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2019_06/Classification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.913065 tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2019_12/__init__.py
--rw-r--r--   0        0        0     5861 2022-10-20 12:42:19.293805 tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2019_12/Classification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.799058 tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.709040 tcsoa-0.9.0/tcsoa/gen/Internal/ImportExport/_2010_04/__init__.py
--rw-r--r--   0        0        0     5269 2022-10-20 12:42:48.542533 tcsoa-0.9.0/tcsoa/gen/Internal/ImportExport/_2010_04/L10NImportExport.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.998072 tcsoa-0.9.0/tcsoa/gen/Internal/ImportExport/_2017_11/__init__.py
--rw-r--r--   0        0        0     3735 2022-10-20 12:42:48.585543 tcsoa-0.9.0/tcsoa/gen/Internal/ImportExport/_2017_11/FileImportExport.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.807048 tcsoa-0.9.0/tcsoa/gen/Internal/ImportExport/_2018_06/__init__.py
--rw-r--r--   0        0        0     3102 2022-10-20 12:42:48.611535 tcsoa-0.9.0/tcsoa/gen/Internal/ImportExport/_2018_06/L10NImportExport.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.716044 tcsoa-0.9.0/tcsoa/gen/Internal/ImportExport/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.953082 tcsoa-0.9.0/tcsoa/gen/Internal/Integration/_2007_06/__init__.py
--rw-r--r--   0        0        0      441 2022-10-20 12:42:48.638540 tcsoa-0.9.0/tcsoa/gen/Internal/Integration/_2007_06/IntegrationManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.923067 tcsoa-0.9.0/tcsoa/gen/Internal/Integration/_2008_06/__init__.py
--rw-r--r--   0        0        0      610 2022-10-20 12:42:48.665543 tcsoa-0.9.0/tcsoa/gen/Internal/Integration/_2008_06/IntegrationManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.855059 tcsoa-0.9.0/tcsoa/gen/Internal/Integration/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.804052 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2008_12/__init__.py
--rw-r--r--   0        0        0     1092 2022-10-20 12:42:48.698548 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2008_12/Core.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.860082 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2011_12/__init__.py
--rw-r--r--   0        0        0     2462 2022-10-20 12:42:48.743555 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2011_12/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.748043 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2012_09/__init__.py
--rw-r--r--   0        0        0     3116 2022-10-20 12:42:48.789556 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2012_09/StructureSearch.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.852060 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2014_06/__init__.py
--rw-r--r--   0        0        0     3728 2022-10-20 12:42:48.831566 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2014_06/DataManagement.py
--rw-r--r--   0        0        0     2070 2022-10-20 12:42:48.864569 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2014_06/IPAManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.555030 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2014_12/__init__.py
--rw-r--r--   0        0        0     1033 2022-10-20 12:42:48.896567 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2014_12/IPAManagement.py
--rw-r--r--   0        0        0     6303 2022-10-20 12:42:48.952575 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2014_12/Model.py
--rw-r--r--   0        0        0     2439 2022-10-20 12:42:48.987581 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2014_12/ResourceManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.708044 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2015_03/__init__.py
--rw-r--r--   0        0        0     6071 2022-10-20 12:42:49.041578 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2015_03/Attachments.py
--rw-r--r--   0        0        0     3374 2022-10-20 12:42:49.089588 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2015_03/ResourceManagement.py
--rw-r--r--   0        0        0    11116 2022-10-20 12:42:49.172590 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2015_03/StructureManagement.py
--rw-r--r--   0        0        0     3004 2022-10-20 12:42:49.210600 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2015_03/StructureSearch.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.612029 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2015_10/__init__.py
--rw-r--r--   0        0        0    10614 2022-10-20 12:42:49.306603 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2015_10/StructureManagement.py
--rw-r--r--   0        0        0     3062 2022-10-20 12:42:49.352625 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2015_10/StructureSearch.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.892058 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2016_09/__init__.py
--rw-r--r--   0        0        0     5061 2022-10-20 12:42:49.411618 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2016_09/DataManagement.py
--rw-r--r--   0        0        0     3872 2022-10-20 12:42:49.452621 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2016_09/IPAManagement.py
--rw-r--r--   0        0        0     4752 2022-10-20 12:42:49.487619 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2016_09/ResourceManagement.py
--rw-r--r--   0        0        0     9531 2022-10-20 12:42:49.561624 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2016_09/StructureManagement.py
--rw-r--r--   0        0        0     1904 2022-10-20 12:42:49.598639 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2016_09/StructureSearch.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.975074 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2017_05/__init__.py
--rw-r--r--   0        0        0     3398 2022-10-20 12:42:49.652643 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2017_05/DataManagement.py
--rw-r--r--   0        0        0      169 2022-10-20 12:42:49.675660 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2017_05/ImportExport.py
--rw-r--r--   0        0        0     4083 2022-10-20 12:42:49.724651 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2017_05/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.579033 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2017_11/__init__.py
--rw-r--r--   0        0        0     1118 2022-10-20 12:42:49.757645 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2017_11/ResourceManagement.py
--rw-r--r--   0        0        0     4153 2022-10-20 12:42:49.807657 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2017_11/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.842051 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2018_11/__init__.py
--rw-r--r--   0        0        0     1090 2022-10-20 12:42:49.838649 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2018_11/ResourceManagement.py
--rw-r--r--   0        0        0    10480 2022-10-20 12:42:49.926669 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2018_11/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.650034 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2019_06/__init__.py
--rw-r--r--   0        0        0     2429 2022-10-20 12:42:49.964683 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2019_06/ClosureRuleEditor.py
--rw-r--r--   0        0        0     1678 2022-10-20 12:42:50.002668 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2019_06/ResourceManagement.py
--rw-r--r--   0        0        0     4007 2022-10-20 12:42:50.038678 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2019_06/StructureSearch.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.753044 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2020_01/__init__.py
--rw-r--r--   0        0        0     3547 2022-10-20 12:42:50.071681 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2020_01/DataManagement.py
--rw-r--r--   0        0        0     5256 2022-10-20 12:42:50.111691 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2020_01/StructureSearch.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.699049 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2020_04/__init__.py
--rw-r--r--   0        0        0     1288 2022-10-20 12:42:50.140701 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2020_04/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.862059 tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.894059 tcsoa-0.9.0/tcsoa/gen/Internal/Mmv/_2012_09/__init__.py
--rw-r--r--   0        0        0    11263 2022-10-20 12:42:17.928679 tcsoa-0.9.0/tcsoa/gen/Internal/Mmv/_2012_09/SpatialStructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.726040 tcsoa-0.9.0/tcsoa/gen/Internal/Mmv/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.012069 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2007_06/__init__.py
--rw-r--r--   0        0        0     9210 2022-10-20 12:42:50.225691 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2007_06/ObjectDirectory.py
--rw-r--r--   0        0        0    49922 2022-10-20 12:42:50.672736 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2007_06/RemoteOperation.py
--rw-r--r--   0        0        0     6322 2022-10-20 12:42:50.730745 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2007_06/TcEntObjectDirectory.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.583037 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2011_06/__init__.py
--rw-r--r--   0        0        0     1673 2022-10-20 12:42:51.215788 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2011_06/ImportExportAsync.py
--rw-r--r--   0        0        0     5192 2022-10-20 12:42:50.776742 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2011_06/ObjectDirectory.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.941066 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2012_02/__init__.py
--rw-r--r--   0        0        0     5398 2022-10-20 12:42:50.832742 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2012_02/ObjectDirectory.py
--rw-r--r--   0        0        0    42494 2022-10-20 12:42:51.182786 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2012_02/RemoteOperation.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.592028 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2017_11/__init__.py
--rw-r--r--   0        0        0     1504 2022-10-20 12:42:51.253787 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2017_11/ArchiveRestore.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.682047 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2018_06/__init__.py
--rw-r--r--   0        0        0     1262 2022-10-20 12:42:51.287789 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2018_06/Search.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.656040 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2020_12/__init__.py
--rw-r--r--   0        0        0     2749 2022-10-20 12:42:51.319787 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2020_12/ImportExportTCXML.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.624029 tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.638044 tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2014_10/__init__.py
--rw-r--r--   0        0        0      699 2022-10-20 12:42:17.954682 tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2014_10/SubscriptionManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.667044 tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2015_03/__init__.py
--rw-r--r--   0        0        0      915 2022-10-20 12:42:17.981705 tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2015_03/MessageManagement.py
--rw-r--r--   0        0        0    14209 2022-10-20 12:42:18.075704 tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2015_03/SubscriptionManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.871054 tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2015_10/__init__.py
--rw-r--r--   0        0        0      342 2022-10-20 12:42:18.102700 tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2015_10/MessageManagement.py
--rw-r--r--   0        0        0     5046 2022-10-20 12:42:18.168703 tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2015_10/SubscriptionManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.607029 tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2017_11/__init__.py
--rw-r--r--   0        0        0     1436 2022-10-20 12:42:18.200713 tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2017_11/SubscriptionManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.783052 tcsoa-0.9.0/tcsoa/gen/Internal/Notification/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.648033 tcsoa-0.9.0/tcsoa/gen/Internal/OccMgmt/_2020_05/__init__.py
--rw-r--r--   0        0        0     5358 2022-10-20 12:42:03.562120 tcsoa-0.9.0/tcsoa/gen/Internal/OccMgmt/_2020_05/ImportExport.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.901069 tcsoa-0.9.0/tcsoa/gen/Internal/OccMgmt/_2020_12/__init__.py
--rw-r--r--   0        0        0     6880 2022-10-20 12:42:03.613124 tcsoa-0.9.0/tcsoa/gen/Internal/OccMgmt/_2020_12/EffectivityManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.574032 tcsoa-0.9.0/tcsoa/gen/Internal/OccMgmt/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.693045 tcsoa-0.9.0/tcsoa/gen/Internal/ProductConfiguratorAw/_2017_12/__init__.py
--rw-r--r--   0        0        0     9850 2022-10-20 12:42:30.359847 tcsoa-0.9.0/tcsoa/gen/Internal/ProductConfiguratorAw/_2017_12/ConfiguratorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.983065 tcsoa-0.9.0/tcsoa/gen/Internal/ProductConfiguratorAw/_2018_05/__init__.py
--rw-r--r--   0        0        0    23263 2022-10-20 12:42:30.490860 tcsoa-0.9.0/tcsoa/gen/Internal/ProductConfiguratorAw/_2018_05/ConfiguratorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.928070 tcsoa-0.9.0/tcsoa/gen/Internal/ProductConfiguratorAw/_2020_05/__init__.py
--rw-r--r--   0        0        0     6719 2022-10-20 12:42:30.543855 tcsoa-0.9.0/tcsoa/gen/Internal/ProductConfiguratorAw/_2020_05/ConfiguratorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.591030 tcsoa-0.9.0/tcsoa/gen/Internal/ProductConfiguratorAw/_2020_12/__init__.py
--rw-r--r--   0        0        0    29941 2022-10-20 12:42:30.669865 tcsoa-0.9.0/tcsoa/gen/Internal/ProductConfiguratorAw/_2020_12/ConfiguratorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.768045 tcsoa-0.9.0/tcsoa/gen/Internal/ProductConfiguratorAw/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.850060 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2007_01/__init__.py
--rw-r--r--   0        0        0     6870 2022-10-20 12:42:51.393799 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2007_01/ScheduleManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.774045 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2007_06/__init__.py
--rw-r--r--   0        0        0     7733 2022-10-20 12:42:51.475803 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2007_06/ScheduleManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.743042 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2008_06/__init__.py
--rw-r--r--   0        0        0     5765 2022-10-20 12:42:51.546816 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2008_06/ScheduleManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.579033 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2009_10/__init__.py
--rw-r--r--   0        0        0     6185 2022-10-20 12:42:51.634822 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2009_10/ScheduleManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.787047 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2010_04/__init__.py
--rw-r--r--   0        0        0     1337 2022-10-20 12:42:51.668820 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2010_04/ScheduleManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.775046 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2011_06/__init__.py
--rw-r--r--   0        0        0     4749 2022-10-20 12:42:51.722833 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2011_06/ScheduleManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.568034 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2012_02/__init__.py
--rw-r--r--   0        0        0     1220 2022-10-20 12:42:51.754834 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2012_02/ScheduleManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.595030 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2014_10/__init__.py
--rw-r--r--   0        0        0     3956 2022-10-20 12:42:51.793844 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2014_10/ScheduleManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.548030 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.695048 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagementAw/_2019_12/__init__.py
--rw-r--r--   0        0        0     8951 2022-10-20 12:42:32.799072 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagementAw/_2019_12/ScheduleManagementAw.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.666046 tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagementAw/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.683038 tcsoa-0.9.0/tcsoa/gen/Internal/Query/_2008_06/__init__.py
--rw-r--r--   0        0        0     1650 2022-10-20 12:42:51.831853 tcsoa-0.9.0/tcsoa/gen/Internal/Query/_2008_06/Finder.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.695048 tcsoa-0.9.0/tcsoa/gen/Internal/Query/_2012_02/__init__.py
--rw-r--r--   0        0        0     5150 2022-10-20 12:42:51.880852 tcsoa-0.9.0/tcsoa/gen/Internal/Query/_2012_02/SavedQuery.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.878055 tcsoa-0.9.0/tcsoa/gen/Internal/Query/_2013_05/__init__.py
--rw-r--r--   0        0        0     4842 2022-10-20 12:42:51.920853 tcsoa-0.9.0/tcsoa/gen/Internal/Query/_2013_05/SavedQuery.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.816052 tcsoa-0.9.0/tcsoa/gen/Internal/Query/_2014_10/__init__.py
--rw-r--r--   0        0        0     4575 2022-10-20 12:42:51.958850 tcsoa-0.9.0/tcsoa/gen/Internal/Query/_2014_10/SavedQuery.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.830051 tcsoa-0.9.0/tcsoa/gen/Internal/Query/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.875078 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2007_06/__init__.py
--rw-r--r--   0        0        0     2229 2022-10-20 12:42:51.997860 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2007_06/VariantManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.882056 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2007_09/__init__.py
--rw-r--r--   0        0        0     2500 2022-10-20 12:42:52.040863 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2007_09/VariantManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.927060 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2008_03/__init__.py
--rw-r--r--   0        0        0     2244 2022-10-20 12:42:52.080869 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2008_03/VariantManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.745043 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2009_01/__init__.py
--rw-r--r--   0        0        0     8788 2022-10-20 12:42:52.185878 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2009_01/VariantManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.578033 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2009_04/__init__.py
--rw-r--r--   0        0        0     4949 2022-10-20 12:42:52.243876 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2009_04/VariantManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.744043 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2009_05/__init__.py
--rw-r--r--   0        0        0     2339 2022-10-20 12:42:52.284880 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2009_05/VariantManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.858074 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2010_04/__init__.py
--rw-r--r--   0        0        0     9177 2022-10-20 12:42:52.377894 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2010_04/VariantManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.867053 tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.602028 tcsoa-0.9.0/tcsoa/gen/Internal/Reports/_2007_06/__init__.py
--rw-r--r--   0        0        0    10316 2022-10-20 12:42:52.493899 tcsoa-0.9.0/tcsoa/gen/Internal/Reports/_2007_06/BOMRollup.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.809054 tcsoa-0.9.0/tcsoa/gen/Internal/Reports/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.008068 tcsoa-0.9.0/tcsoa/gen/Internal/Requirementsmanagement/_2009_10/__init__.py
--rw-r--r--   0        0        0     3154 2022-10-20 12:42:52.532901 tcsoa-0.9.0/tcsoa/gen/Internal/Requirementsmanagement/_2009_10/RequirementsManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.811050 tcsoa-0.9.0/tcsoa/gen/Internal/Requirementsmanagement/_2012_02/__init__.py
--rw-r--r--   0        0        0     3465 2022-10-20 12:42:52.572908 tcsoa-0.9.0/tcsoa/gen/Internal/Requirementsmanagement/_2012_02/RequirementsManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.543024 tcsoa-0.9.0/tcsoa/gen/Internal/Requirementsmanagement/_2012_10/__init__.py
--rw-r--r--   0        0        0     3809 2022-10-20 12:42:52.621919 tcsoa-0.9.0/tcsoa/gen/Internal/Requirementsmanagement/_2012_10/RequirementsManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.744043 tcsoa-0.9.0/tcsoa/gen/Internal/Requirementsmanagement/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.574032 tcsoa-0.9.0/tcsoa/gen/Internal/RevRuleMgmt/_2019_12/__init__.py
--rw-r--r--   0        0        0     7535 2022-10-20 12:42:03.683132 tcsoa-0.9.0/tcsoa/gen/Internal/RevRuleMgmt/_2019_12/RevisionRuleAdministration.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.995072 tcsoa-0.9.0/tcsoa/gen/Internal/RevRuleMgmt/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.769044 tcsoa-0.9.0/tcsoa/gen/Internal/Search/_2020_12/__init__.py
--rw-r--r--   0        0        0    16853 2022-10-20 12:42:03.773146 tcsoa-0.9.0/tcsoa/gen/Internal/Search/_2020_12/SearchFolder.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.832057 tcsoa-0.9.0/tcsoa/gen/Internal/Search/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.590027 tcsoa-0.9.0/tcsoa/gen/Internal/Security/_2017_12/__init__.py
--rw-r--r--   0        0        0     5755 2022-10-20 12:41:58.603592 tcsoa-0.9.0/tcsoa/gen/Internal/Security/_2017_12/AwLicensing.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.635041 tcsoa-0.9.0/tcsoa/gen/Internal/Security/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.714041 tcsoa-0.9.0/tcsoa/gen/Internal/Structure/_2020_12/__init__.py
--rw-r--r--   0        0        0     7965 2022-10-20 12:42:00.307768 tcsoa-0.9.0/tcsoa/gen/Internal/Structure/_2020_12/WhereUsed.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.576032 tcsoa-0.9.0/tcsoa/gen/Internal/Structure/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.994073 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2007_06/__init__.py
--rw-r--r--   0        0        0     1679 2022-10-20 12:42:52.664919 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2007_06/GlobalAlternate.py
--rw-r--r--   0        0        0     1210 2022-10-20 12:42:52.696929 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2007_06/PublishByLink.py
--rw-r--r--   0        0        0     1430 2022-10-20 12:42:52.733929 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2007_06/Restructure.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.942067 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2007_12/__init__.py
--rw-r--r--   0        0        0     2894 2022-10-20 12:42:52.783924 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2007_12/BrokenLinks.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.645038 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2008_03/__init__.py
--rw-r--r--   0        0        0      738 2022-10-20 12:42:52.812929 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2008_03/Structure.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.007066 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2008_05/__init__.py
--rw-r--r--   0        0        0      504 2022-10-20 12:42:52.842931 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2008_05/Restructure.py
--rw-r--r--   0        0        0      407 2022-10-20 12:42:52.868941 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2008_05/Structure.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.712045 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2008_06/__init__.py
--rw-r--r--   0        0        0     2215 2022-10-20 12:42:52.909940 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2008_06/Structure.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.946062 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2009_10/__init__.py
--rw-r--r--   0        0        0     2732 2022-10-20 12:42:52.946942 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2009_10/EffectivitiesManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.678047 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2010_04/__init__.py
--rw-r--r--   0        0        0     3093 2022-10-20 12:42:52.989946 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2010_04/BOMMarkup.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.715046 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2010_09/__init__.py
--rw-r--r--   0        0        0      841 2022-10-20 12:42:53.015949 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2010_09/Structure.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.643038 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2011_06/__init__.py
--rw-r--r--   0        0        0     7566 2022-10-20 12:42:53.118965 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2011_06/IncrementalChange.py
--rw-r--r--   0        0        0     4705 2022-10-20 12:42:53.170964 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2011_06/Structure.py
--rw-r--r--   0        0        0     7474 2022-10-20 12:42:53.252978 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2011_06/VariantManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.946062 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2012_02/__init__.py
--rw-r--r--   0        0        0     6080 2022-10-20 12:42:53.314015 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2012_02/StructureVerification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.629037 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2012_09/__init__.py
--rw-r--r--   0        0        0     1406 2022-10-20 12:42:53.346987 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2012_09/StructureVerification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.721045 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2013_05/__init__.py
--rw-r--r--   0        0        0    10741 2022-10-20 12:42:53.420986 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2013_05/StructureExpansionLite.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.758045 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2013_12/__init__.py
--rw-r--r--   0        0        0     3123 2022-10-20 12:42:53.459998 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2013_12/StructureExpansionLite.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.952067 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2014_12/__init__.py
--rw-r--r--   0        0        0     3730 2022-10-20 12:42:53.511001 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2014_12/BrokenLinks.py
--rw-r--r--   0        0        0     1306 2022-10-20 12:42:53.539004 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2014_12/Restructure.py
--rw-r--r--   0        0        0    29349 2022-10-20 12:42:53.692016 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2014_12/StructureVerification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.936066 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2015_10/__init__.py
--rw-r--r--   0        0        0      997 2022-10-20 12:42:53.719040 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2015_10/VariantManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.907054 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2016_03/__init__.py
--rw-r--r--   0        0        0     6060 2022-10-20 12:42:53.784020 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2016_03/StructureVerification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.649034 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2016_10/__init__.py
--rw-r--r--   0        0        0     4284 2022-10-20 12:42:53.842031 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2016_10/Effectivity.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.867053 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2017_05/__init__.py
--rw-r--r--   0        0        0    10110 2022-10-20 12:42:53.906029 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2017_05/StructureExpansionLite.py
--rw-r--r--   0        0        0     1542 2022-10-20 12:42:53.938039 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2017_05/StructureLiteConversion.py
--rw-r--r--   0        0        0     3323 2022-10-20 12:42:53.985039 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2017_05/StructureVerification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.549029 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2018_11/__init__.py
--rw-r--r--   0        0        0     1427 2022-10-20 12:42:54.020051 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2018_11/MassUpdate.py
--rw-r--r--   0        0        0     3634 2022-10-20 12:42:54.068072 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2018_11/StructureVerification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.002064 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2020_05/__init__.py
--rw-r--r--   0        0        0     7787 2022-10-20 12:42:54.124066 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2020_05/RevisionRuleAdministration.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.901069 tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.836052 tcsoa-0.9.0/tcsoa/gen/Internal/TCXMLImportExport/_2020_12/__init__.py
--rw-r--r--   0        0        0     4635 2022-10-20 12:42:03.812144 tcsoa-0.9.0/tcsoa/gen/Internal/TCXMLImportExport/_2020_12/Briefcase.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.793051 tcsoa-0.9.0/tcsoa/gen/Internal/TCXMLImportExport/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.783052 tcsoa-0.9.0/tcsoa/gen/Internal/Translation/_2007_06/__init__.py
--rw-r--r--   0        0        0     6924 2022-10-20 12:42:54.197065 tcsoa-0.9.0/tcsoa/gen/Internal/Translation/_2007_06/TranslationManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.830051 tcsoa-0.9.0/tcsoa/gen/Internal/Translation/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.703047 tcsoa-0.9.0/tcsoa/gen/Internal/UiConfig/_2014_11/__init__.py
--rw-r--r--   0        0        0     1405 2022-10-20 12:42:18.236714 tcsoa-0.9.0/tcsoa/gen/Internal/UiConfig/_2014_11/UiConfig.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.835050 tcsoa-0.9.0/tcsoa/gen/Internal/UiConfig/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.872054 tcsoa-0.9.0/tcsoa/gen/Internal/Validation/_2007_06/__init__.py
--rw-r--r--   0        0        0    18115 2022-10-20 12:42:54.321101 tcsoa-0.9.0/tcsoa/gen/Internal/Validation/_2007_06/Validation.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.605029 tcsoa-0.9.0/tcsoa/gen/Internal/Validation/_2008_06/__init__.py
--rw-r--r--   0        0        0     7000 2022-10-20 12:42:54.386082 tcsoa-0.9.0/tcsoa/gen/Internal/Validation/_2008_06/Validation.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.547030 tcsoa-0.9.0/tcsoa/gen/Internal/Validation/_2012_02/__init__.py
--rw-r--r--   0        0        0     9436 2022-10-20 12:42:54.466090 tcsoa-0.9.0/tcsoa/gen/Internal/Validation/_2012_02/Validation.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.609032 tcsoa-0.9.0/tcsoa/gen/Internal/Validation/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.585031 tcsoa-0.9.0/tcsoa/gen/Internal/Vendormanagement/_2008_05/__init__.py
--rw-r--r--   0        0        0     3964 2022-10-20 12:42:54.508090 tcsoa-0.9.0/tcsoa/gen/Internal/Vendormanagement/_2008_05/VendorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.741045 tcsoa-0.9.0/tcsoa/gen/Internal/Vendormanagement/_2008_06/__init__.py
--rw-r--r--   0        0        0      933 2022-10-20 12:42:54.539095 tcsoa-0.9.0/tcsoa/gen/Internal/Vendormanagement/_2008_06/VendorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.919067 tcsoa-0.9.0/tcsoa/gen/Internal/Vendormanagement/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.857059 tcsoa-0.9.0/tcsoa/gen/Internal/VendorManagementAW/_2019_12/__init__.py
--rw-r--r--   0        0        0     5178 2022-10-20 12:43:04.107987 tcsoa-0.9.0/tcsoa/gen/Internal/VendorManagementAW/_2019_12/VendorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.556030 tcsoa-0.9.0/tcsoa/gen/Internal/VendorManagementAW/_2020_05/__init__.py
--rw-r--r--   0        0        0     1561 2022-10-20 12:43:04.141992 tcsoa-0.9.0/tcsoa/gen/Internal/VendorManagementAW/_2020_05/VendorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.843052 tcsoa-0.9.0/tcsoa/gen/Internal/VendorManagementAW/_2020_12/__init__.py
--rw-r--r--   0        0        0     2730 2022-10-20 12:43:04.178991 tcsoa-0.9.0/tcsoa/gen/Internal/VendorManagementAW/_2020_12/VendorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.705043 tcsoa-0.9.0/tcsoa/gen/Internal/VendorManagementAW/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.712045 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2008_06/__init__.py
--rw-r--r--   0        0        0    33963 2022-10-20 12:42:54.749115 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2008_06/DataManagement.py
--rw-r--r--   0        0        0    18894 2022-10-20 12:42:54.899127 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2008_06/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.614029 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2010_04/__init__.py
--rw-r--r--   0        0        0     7925 2022-10-20 12:42:54.983135 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2010_04/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.734041 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2010_09/__init__.py
--rw-r--r--   0        0        0    16115 2022-10-20 12:42:55.127153 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2010_09/DataManagement.py
--rw-r--r--   0        0        0     2540 2022-10-20 12:42:55.165162 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2010_09/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.909059 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2011_12/__init__.py
--rw-r--r--   0        0        0     8571 2022-10-20 12:42:55.235162 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2011_12/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.776046 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2012_10/__init__.py
--rw-r--r--   0        0        0     1826 2022-10-20 12:42:55.267161 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2012_10/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.607029 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2017_05/__init__.py
--rw-r--r--   0        0        0     5634 2022-10-20 12:42:55.327171 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2017_05/DataManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.707045 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2018_11/__init__.py
--rw-r--r--   0        0        0     6419 2022-10-20 12:42:55.385169 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2018_11/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.771052 tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.920064 tcsoa-0.9.0/tcsoa/gen/Internal/Workflow/_2013_05/__init__.py
--rw-r--r--   0        0        0     2172 2022-10-20 12:42:55.418172 tcsoa-0.9.0/tcsoa/gen/Internal/Workflow/_2013_05/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.625030 tcsoa-0.9.0/tcsoa/gen/Internal/Workflow/_2017_11/__init__.py
--rw-r--r--   0        0        0     1689 2022-10-20 12:42:55.446180 tcsoa-0.9.0/tcsoa/gen/Internal/Workflow/_2017_11/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.001066 tcsoa-0.9.0/tcsoa/gen/Internal/Workflow/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.552030 tcsoa-0.9.0/tcsoa/gen/Internal/Workflowaw/_2020_12/__init__.py
--rw-r--r--   0        0        0     9409 2022-10-20 12:42:03.883159 tcsoa-0.9.0/tcsoa/gen/Internal/Workflowaw/_2020_12/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.968069 tcsoa-0.9.0/tcsoa/gen/Internal/Workflowaw/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.637041 tcsoa-0.9.0/tcsoa/gen/Internal/XlsBom/_2020_12/__init__.py
--rw-r--r--   0        0        0    10138 2022-10-20 12:42:00.399779 tcsoa-0.9.0/tcsoa/gen/Internal/XlsBom/_2020_12/Import.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.987071 tcsoa-0.9.0/tcsoa/gen/Internal/XlsBom/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.735048 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2012_10/__init__.py
--rw-r--r--   0        0        0    13932 2022-10-20 12:42:20.406909 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2012_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.571032 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_03/__init__.py
--rw-r--r--   0        0        0     1010 2022-10-20 12:42:20.433918 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.935069 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_07/__init__.py
--rw-r--r--   0        0        0      832 2022-10-20 12:42:20.463916 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_07/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.665047 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_10/__init__.py
--rw-r--r--   0        0        0     2136 2022-10-20 12:42:20.495920 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.926059 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2016_03/__init__.py
--rw-r--r--   0        0        0     3032 2022-10-20 12:42:20.531923 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2016_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.719040 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2017_06/__init__.py
--rw-r--r--   0        0        0     3644 2022-10-20 12:42:20.570922 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2017_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.842051 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2017_12/__init__.py
--rw-r--r--   0        0        0     1303 2022-10-20 12:42:20.598934 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2017_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.582039 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2018_05/__init__.py
--rw-r--r--   0        0        0     4897 2022-10-20 12:42:20.636929 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2018_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.785046 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2018_12/__init__.py
--rw-r--r--   0        0        0     6769 2022-10-20 12:42:20.685934 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2018_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.583037 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2019_06/__init__.py
--rw-r--r--   0        0        0     8286 2022-10-20 12:42:20.759945 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2019_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.982071 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2019_12/__init__.py
--rw-r--r--   0        0        0     9740 2022-10-20 12:42:20.822947 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2019_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.907054 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2020_05/__init__.py
--rw-r--r--   0        0        0     4187 2022-10-20 12:42:20.858952 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2020_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.645038 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2020_12/__init__.py
--rw-r--r--   0        0        0     5323 2022-10-20 12:42:20.898967 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2020_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.586038 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/__init__.py
--rw-r--r--   0        0        0     5532 2022-10-20 12:41:55.049209 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.673044 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceVis/_2014_11/__init__.py
--rw-r--r--   0        0        0     3736 2022-10-20 12:42:20.932958 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceVis/_2014_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.853059 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceVis/_2015_03/__init__.py
--rw-r--r--   0        0        0    14757 2022-10-20 12:42:20.972973 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceVis/_2015_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.598027 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceVis/_2018_05/__init__.py
--rw-r--r--   0        0        0     3936 2022-10-20 12:42:21.003963 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceVis/_2018_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.897060 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceVis/__init__.py
--rw-r--r--   0        0        0      918 2022-10-20 12:41:55.065213 tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceVis/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.570034 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2007_06/__init__.py
--rw-r--r--   0        0        0     9918 2022-10-20 12:42:21.059971 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.838057 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2008_06/__init__.py
--rw-r--r--   0        0        0     1776 2022-10-20 12:42:21.085974 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.770065 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2009_10/__init__.py
--rw-r--r--   0        0        0     2310 2022-10-20 12:42:21.114973 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2009_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.569031 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2011_06/__init__.py
--rw-r--r--   0        0        0     1150 2022-10-20 12:42:21.143976 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.005088 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2012_10/__init__.py
--rw-r--r--   0        0        0     1269 2022-10-20 12:42:21.173981 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2012_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.807048 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2013_05/__init__.py
--rw-r--r--   0        0        0     1060 2022-10-20 12:42:21.202981 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2013_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.598027 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2014_10/__init__.py
--rw-r--r--   0        0        0     1150 2022-10-20 12:42:21.232984 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2014_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.680038 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2015_10/__init__.py
--rw-r--r--   0        0        0     1230 2022-10-20 12:42:21.264989 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2015_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.746044 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2016_09/__init__.py
--rw-r--r--   0        0        0     1161 2022-10-20 12:42:21.295993 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2016_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.885067 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2017_11/__init__.py
--rw-r--r--   0        0        0     1619 2022-10-20 12:42:21.326995 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2017_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.737048 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2018_06/__init__.py
--rw-r--r--   0        0        0     1205 2022-10-20 12:42:21.356998 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2018_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.766045 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2018_11/__init__.py
--rw-r--r--   0        0        0     1505 2022-10-20 12:42:21.385002 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2018_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.967069 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2019_06/__init__.py
--rw-r--r--   0        0        0     1830 2022-10-20 12:42:21.416009 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2019_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.869055 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/__init__.py
--rw-r--r--   0        0        0     2860 2022-10-20 12:41:55.106219 tcsoa-0.9.0/tcsoa/gen/Internal_Administration/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.668044 tcsoa-0.9.0/tcsoa/gen/Internal_Ai/_2008_06/__init__.py
--rw-r--r--   0        0        0     2408 2022-10-20 12:42:21.452010 tcsoa-0.9.0/tcsoa/gen/Internal_Ai/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.825058 tcsoa-0.9.0/tcsoa/gen/Internal_Ai/_2016_03/__init__.py
--rw-r--r--   0        0        0      856 2022-10-20 12:42:21.482016 tcsoa-0.9.0/tcsoa/gen/Internal_Ai/_2016_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.987071 tcsoa-0.9.0/tcsoa/gen/Internal_Ai/_2016_04/__init__.py
--rw-r--r--   0        0        0     1099 2022-10-20 12:42:21.510011 tcsoa-0.9.0/tcsoa/gen/Internal_Ai/_2016_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.552030 tcsoa-0.9.0/tcsoa/gen/Internal_Ai/__init__.py
--rw-r--r--   0        0        0      528 2022-10-20 12:41:55.118212 tcsoa-0.9.0/tcsoa/gen/Internal_Ai/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.549029 tcsoa-0.9.0/tcsoa/gen/Internal_AuditManager/_2012_09/__init__.py
--rw-r--r--   0        0        0     1012 2022-10-20 12:42:21.543017 tcsoa-0.9.0/tcsoa/gen/Internal_AuditManager/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.748043 tcsoa-0.9.0/tcsoa/gen/Internal_AuditManager/__init__.py
--rw-r--r--   0        0        0      262 2022-10-20 12:41:55.124216 tcsoa-0.9.0/tcsoa/gen/Internal_AuditManager/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.561031 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2012_10/__init__.py
--rw-r--r--   0        0        0    24886 2022-10-20 12:42:19.584833 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2012_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.619029 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2013_12/__init__.py
--rw-r--r--   0        0        0     7485 2022-10-20 12:42:19.630838 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2013_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.752043 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2014_11/__init__.py
--rw-r--r--   0        0        0     2928 2022-10-20 12:42:19.667842 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2014_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.550029 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2015_03/__init__.py
--rw-r--r--   0        0        0    10876 2022-10-20 12:42:19.719846 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2015_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.800055 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2015_10/__init__.py
--rw-r--r--   0        0        0     4603 2022-10-20 12:42:19.759850 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2015_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.558030 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2016_03/__init__.py
--rw-r--r--   0        0        0    19107 2022-10-20 12:42:19.819882 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2016_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.009069 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2016_04/__init__.py
--rw-r--r--   0        0        0     5333 2022-10-20 12:42:19.853858 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2016_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.785046 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2016_12/__init__.py
--rw-r--r--   0        0        0    26603 2022-10-20 12:42:19.915865 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2016_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.973071 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2017_06/__init__.py
--rw-r--r--   0        0        0    35016 2022-10-20 12:42:19.993876 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2017_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.636038 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2017_12/__init__.py
--rw-r--r--   0        0        0    15630 2022-10-20 12:42:20.047873 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2017_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.740043 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2018_05/__init__.py
--rw-r--r--   0        0        0    24660 2022-10-20 12:42:20.132882 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2018_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.837052 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2018_12/__init__.py
--rw-r--r--   0        0        0     3745 2022-10-20 12:42:20.169887 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2018_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.988072 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2019_06/__init__.py
--rw-r--r--   0        0        0    11037 2022-10-20 12:42:20.220892 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2019_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.888056 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2019_12/__init__.py
--rw-r--r--   0        0        0    10755 2022-10-20 12:42:20.266899 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2019_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.671045 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2020_05/__init__.py
--rw-r--r--   0        0        0    11815 2022-10-20 12:42:20.324905 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2020_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.546029 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2020_12/__init__.py
--rw-r--r--   0        0        0     3585 2022-10-20 12:42:20.357903 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2020_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.731058 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/__init__.py
--rw-r--r--   0        0        0    12806 2022-10-20 12:41:54.956200 tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.991073 tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2007_01/__init__.py
--rw-r--r--   0        0        0     2159 2022-10-20 12:42:21.574028 tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2007_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.601029 tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2010_04/__init__.py
--rw-r--r--   0        0        0     3092 2022-10-20 12:42:21.608035 tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.565032 tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2010_09/__init__.py
--rw-r--r--   0        0        0     3047 2022-10-20 12:42:21.640027 tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2010_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.730042 tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2011_06/__init__.py
--rw-r--r--   0        0        0     3249 2022-10-20 12:42:21.671029 tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.758045 tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2013_05/__init__.py
--rw-r--r--   0        0        0     1768 2022-10-20 12:42:21.704038 tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2013_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.929066 tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/__init__.py
--rw-r--r--   0        0        0     1149 2022-10-20 12:41:55.144219 tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.587032 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2007_12/__init__.py
--rw-r--r--   0        0        0     1873 2022-10-20 12:42:21.735051 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2007_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.672047 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2008_03/__init__.py
--rw-r--r--   0        0        0     2629 2022-10-20 12:42:21.764046 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2008_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.007066 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2008_05/__init__.py
--rw-r--r--   0        0        0     1797 2022-10-20 12:42:21.793041 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2008_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.629037 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2008_06/__init__.py
--rw-r--r--   0        0        0     1487 2022-10-20 12:42:21.823046 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.815056 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2010_04/__init__.py
--rw-r--r--   0        0        0     3799 2022-10-20 12:42:21.857046 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.642033 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2013_05/__init__.py
--rw-r--r--   0        0        0     1003 2022-10-20 12:42:21.890056 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2013_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.866073 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2017_05/__init__.py
--rw-r--r--   0        0        0     5274 2022-10-20 12:42:21.920058 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2017_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.639047 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/__init__.py
--rw-r--r--   0        0        0     1160 2022-10-20 12:41:55.161222 tcsoa-0.9.0/tcsoa/gen/Internal_Cad/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.933066 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2009_10/__init__.py
--rw-r--r--   0        0        0     1029 2022-10-20 12:42:21.950060 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2009_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.676048 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2011_06/__init__.py
--rw-r--r--   0        0        0     5877 2022-10-20 12:42:21.983063 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.601029 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2012_02/__init__.py
--rw-r--r--   0        0        0     5429 2022-10-20 12:42:22.021068 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2012_02/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.626031 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2012_09/__init__.py
--rw-r--r--   0        0        0     4590 2022-10-20 12:42:22.057063 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.975074 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2013_05/__init__.py
--rw-r--r--   0        0        0     1381 2022-10-20 12:42:22.087066 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2013_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.640035 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2013_12/__init__.py
--rw-r--r--   0        0        0     4785 2022-10-20 12:42:22.123069 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2013_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.711042 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2014_06/__init__.py
--rw-r--r--   0        0        0     4406 2022-10-20 12:42:22.153071 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2014_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.962068 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/__init__.py
--rw-r--r--   0        0        0     1736 2022-10-20 12:41:55.189220 tcsoa-0.9.0/tcsoa/gen/Internal_Cae/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.872054 tcsoa-0.9.0/tcsoa/gen/Internal_ChangeManagement/_2012_10/__init__.py
--rw-r--r--   0        0        0     1192 2022-10-20 12:42:22.193081 tcsoa-0.9.0/tcsoa/gen/Internal_ChangeManagement/_2012_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.706044 tcsoa-0.9.0/tcsoa/gen/Internal_ChangeManagement/_2015_03/__init__.py
--rw-r--r--   0        0        0     4808 2022-10-20 12:42:22.230086 tcsoa-0.9.0/tcsoa/gen/Internal_ChangeManagement/_2015_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.599028 tcsoa-0.9.0/tcsoa/gen/Internal_ChangeManagement/_2020_01/__init__.py
--rw-r--r--   0        0        0     2892 2022-10-20 12:42:22.267080 tcsoa-0.9.0/tcsoa/gen/Internal_ChangeManagement/_2020_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.818055 tcsoa-0.9.0/tcsoa/gen/Internal_ChangeManagement/__init__.py
--rw-r--r--   0        0        0      975 2022-10-20 12:41:55.205226 tcsoa-0.9.0/tcsoa/gen/Internal_ChangeManagement/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.947068 tcsoa-0.9.0/tcsoa/gen/Internal_Classification/_2009_10/__init__.py
--rw-r--r--   0        0        0     3376 2022-10-20 12:42:22.312086 tcsoa-0.9.0/tcsoa/gen/Internal_Classification/_2009_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.877060 tcsoa-0.9.0/tcsoa/gen/Internal_Classification/_2017_05/__init__.py
--rw-r--r--   0        0        0     1449 2022-10-20 12:42:22.344101 tcsoa-0.9.0/tcsoa/gen/Internal_Classification/_2017_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.778055 tcsoa-0.9.0/tcsoa/gen/Internal_Classification/_2018_11/__init__.py
--rw-r--r--   0        0        0     2076 2022-10-20 12:42:22.375096 tcsoa-0.9.0/tcsoa/gen/Internal_Classification/_2018_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.749045 tcsoa-0.9.0/tcsoa/gen/Internal_Classification/_2020_04/__init__.py
--rw-r--r--   0        0        0     2495 2022-10-20 12:42:22.410101 tcsoa-0.9.0/tcsoa/gen/Internal_Classification/_2020_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.760046 tcsoa-0.9.0/tcsoa/gen/Internal_Classification/__init__.py
--rw-r--r--   0        0        0      775 2022-10-20 12:41:55.217229 tcsoa-0.9.0/tcsoa/gen/Internal_Classification/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.890058 tcsoa-0.9.0/tcsoa/gen/Internal_CodeCoverage/_2011_06/__init__.py
--rw-r--r--   0        0        0     1193 2022-10-20 12:42:22.442098 tcsoa-0.9.0/tcsoa/gen/Internal_CodeCoverage/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.843052 tcsoa-0.9.0/tcsoa/gen/Internal_CodeCoverage/__init__.py
--rw-r--r--   0        0        0      234 2022-10-20 12:41:55.223224 tcsoa-0.9.0/tcsoa/gen/Internal_CodeCoverage/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.986071 tcsoa-0.9.0/tcsoa/gen/Internal_ConfigFilterCriteria/_2013_12/__init__.py
--rw-r--r--   0        0        0     5417 2022-10-20 12:42:22.473105 tcsoa-0.9.0/tcsoa/gen/Internal_ConfigFilterCriteria/_2013_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.573032 tcsoa-0.9.0/tcsoa/gen/Internal_ConfigFilterCriteria/__init__.py
--rw-r--r--   0        0        0      252 2022-10-20 12:41:55.230229 tcsoa-0.9.0/tcsoa/gen/Internal_ConfigFilterCriteria/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.777047 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2014_06/__init__.py
--rw-r--r--   0        0        0    34830 2022-10-20 12:42:22.536112 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2014_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.711042 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2014_12/__init__.py
--rw-r--r--   0        0        0     7798 2022-10-20 12:42:22.572113 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2014_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.569031 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2015_03/__init__.py
--rw-r--r--   0        0        0     4071 2022-10-20 12:42:22.604114 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2015_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.910058 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2015_10/__init__.py
--rw-r--r--   0        0        0    21675 2022-10-20 12:42:22.652118 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2015_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.832057 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2016_09/__init__.py
--rw-r--r--   0        0        0     4616 2022-10-20 12:42:22.701122 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2016_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.961068 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2017_11/__init__.py
--rw-r--r--   0        0        0     3763 2022-10-20 12:42:22.734133 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2017_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.594028 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2018_06/__init__.py
--rw-r--r--   0        0        0    12378 2022-10-20 12:42:22.773129 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2018_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.653035 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2018_11/__init__.py
--rw-r--r--   0        0        0     6517 2022-10-20 12:42:22.804140 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2018_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.875078 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/__init__.py
--rw-r--r--   0        0        0     2810 2022-10-20 12:41:55.287226 tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.563036 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2006_03/__init__.py
--rw-r--r--   0        0        0     1046 2022-10-20 12:42:22.832134 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2006_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.825058 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_01/__init__.py
--rw-r--r--   0        0        0     2049 2022-10-20 12:42:22.864140 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.958058 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_05/__init__.py
--rw-r--r--   0        0        0     1336 2022-10-20 12:42:22.894146 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.997071 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_06/__init__.py
--rw-r--r--   0        0        0     3003 2022-10-20 12:42:22.927172 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.975074 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_09/__init__.py
--rw-r--r--   0        0        0      987 2022-10-20 12:42:22.956153 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.594028 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_12/__init__.py
--rw-r--r--   0        0        0      925 2022-10-20 12:42:22.985156 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.679048 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2008_03/__init__.py
--rw-r--r--   0        0        0     1026 2022-10-20 12:42:23.015150 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2008_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.749045 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2008_06/__init__.py
--rw-r--r--   0        0        0    22448 2022-10-20 12:42:23.087161 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.885067 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2009_10/__init__.py
--rw-r--r--   0        0        0     2299 2022-10-20 12:42:23.120164 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2009_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.615033 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2010_04/__init__.py
--rw-r--r--   0        0        0     4697 2022-10-20 12:42:23.167164 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.971062 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2010_09/__init__.py
--rw-r--r--   0        0        0     2721 2022-10-20 12:42:23.208171 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2010_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.774045 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2011_06/__init__.py
--rw-r--r--   0        0        0      732 2022-10-20 12:42:23.238171 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.634037 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2012_02/__init__.py
--rw-r--r--   0        0        0     3403 2022-10-20 12:42:23.268177 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2012_02/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.618030 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2012_09/__init__.py
--rw-r--r--   0        0        0      990 2022-10-20 12:42:23.299178 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.681046 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2012_10/__init__.py
--rw-r--r--   0        0        0     3063 2022-10-20 12:42:23.330192 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2012_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.948069 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2013_05/__init__.py
--rw-r--r--   0        0        0     7860 2022-10-20 12:42:23.383204 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2013_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.613030 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2014_10/__init__.py
--rw-r--r--   0        0        0     5339 2022-10-20 12:42:23.427203 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2014_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.756046 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2014_11/__init__.py
--rw-r--r--   0        0        0     1375 2022-10-20 12:42:23.462200 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2014_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.821055 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2016_10/__init__.py
--rw-r--r--   0        0        0     5578 2022-10-20 12:42:23.493210 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2016_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.741045 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2017_05/__init__.py
--rw-r--r--   0        0        0     5671 2022-10-20 12:42:23.528214 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2017_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.792046 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2017_11/__init__.py
--rw-r--r--   0        0        0     8830 2022-10-20 12:42:23.574215 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2017_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.541030 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2018_06/__init__.py
--rw-r--r--   0        0        0    14951 2022-10-20 12:42:23.607233 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2018_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.782046 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2018_11/__init__.py
--rw-r--r--   0        0        0     3087 2022-10-20 12:42:23.642210 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2018_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.604032 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2018_12/__init__.py
--rw-r--r--   0        0        0     1277 2022-10-20 12:42:23.670218 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2018_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.856060 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2020_01/__init__.py
--rw-r--r--   0        0        0     1839 2022-10-20 12:42:23.702231 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2020_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.009069 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2020_04/__init__.py
--rw-r--r--   0        0        0     1869 2022-10-20 12:42:23.731227 tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2020_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.566032 tcsoa-0.9.0/tcsoa/gen/Internal_Core/__init__.py
--rw-r--r--   0        0        0     7942 2022-10-20 12:41:55.393239 tcsoa-0.9.0/tcsoa/gen/Internal_Core/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.703047 tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2011_06/__init__.py
--rw-r--r--   0        0        0    25857 2022-10-20 12:42:23.831231 tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.854061 tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2014_06/__init__.py
--rw-r--r--   0        0        0     2931 2022-10-20 12:42:23.863232 tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2014_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.627031 tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2015_07/__init__.py
--rw-r--r--   0        0        0     1397 2022-10-20 12:42:23.898235 tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2015_07/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.764042 tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2015_10/__init__.py
--rw-r--r--   0        0        0     2667 2022-10-20 12:42:23.932240 tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2015_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.904062 tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2019_06/__init__.py
--rw-r--r--   0        0        0     1472 2022-10-20 12:42:23.966251 tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2019_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.834055 tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/__init__.py
--rw-r--r--   0        0        0     2774 2022-10-20 12:41:55.455274 tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.691046 tcsoa-0.9.0/tcsoa/gen/Internal_DocMgmtAw/_2019_06/__init__.py
--rw-r--r--   0        0        0     1045 2022-10-20 12:42:24.000241 tcsoa-0.9.0/tcsoa/gen/Internal_DocMgmtAw/_2019_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.967069 tcsoa-0.9.0/tcsoa/gen/Internal_DocMgmtAw/_2019_12/__init__.py
--rw-r--r--   0        0        0     1082 2022-10-20 12:42:24.030248 tcsoa-0.9.0/tcsoa/gen/Internal_DocMgmtAw/_2019_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.572031 tcsoa-0.9.0/tcsoa/gen/Internal_DocMgmtAw/__init__.py
--rw-r--r--   0        0        0      330 2022-10-20 12:41:55.463252 tcsoa-0.9.0/tcsoa/gen/Internal_DocMgmtAw/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.909059 tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/_2008_06/__init__.py
--rw-r--r--   0        0        0     8877 2022-10-20 12:42:24.068250 tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.788046 tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/_2013_05/__init__.py
--rw-r--r--   0        0        0     4997 2022-10-20 12:42:24.101258 tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/_2013_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.753044 tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/_2013_12/__init__.py
--rw-r--r--   0        0        0     1788 2022-10-20 12:42:24.139254 tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/_2013_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.795051 tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/_2020_12/__init__.py
--rw-r--r--   0        0        0     1084 2022-10-20 12:42:24.168262 tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/_2020_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.767045 tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/__init__.py
--rw-r--r--   0        0        0     1132 2022-10-20 12:41:55.481255 tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.960068 tcsoa-0.9.0/tcsoa/gen/Internal_EntCba/_2019_12/__init__.py
--rw-r--r--   0        0        0     1800 2022-10-20 12:42:24.202265 tcsoa-0.9.0/tcsoa/gen/Internal_EntCba/_2019_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.775046 tcsoa-0.9.0/tcsoa/gen/Internal_EntCba/__init__.py
--rw-r--r--   0        0        0      254 2022-10-20 12:41:55.489256 tcsoa-0.9.0/tcsoa/gen/Internal_EntCba/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.573032 tcsoa-0.9.0/tcsoa/gen/Internal_Gdis/_2006_03/__init__.py
--rw-r--r--   0        0        0     1008 2022-10-20 12:42:24.233267 tcsoa-0.9.0/tcsoa/gen/Internal_Gdis/_2006_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.693045 tcsoa-0.9.0/tcsoa/gen/Internal_Gdis/__init__.py
--rw-r--r--   0        0        0      208 2022-10-20 12:41:55.495254 tcsoa-0.9.0/tcsoa/gen/Internal_Gdis/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.669045 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2007_06/__init__.py
--rw-r--r--   0        0        0    20751 2022-10-20 12:42:24.317273 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.677047 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2008_06/__init__.py
--rw-r--r--   0        0        0     3181 2022-10-20 12:42:24.354304 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.606028 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2010_02/__init__.py
--rw-r--r--   0        0        0     5593 2022-10-20 12:42:24.390282 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2010_02/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.852060 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2010_09/__init__.py
--rw-r--r--   0        0        0     1841 2022-10-20 12:42:24.424283 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2010_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.761044 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2017_05/__init__.py
--rw-r--r--   0        0        0     1366 2022-10-20 12:42:24.460310 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2017_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.674047 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2018_11/__init__.py
--rw-r--r--   0        0        0     4097 2022-10-20 12:42:24.498292 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2018_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.825058 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2020_01/__init__.py
--rw-r--r--   0        0        0    12188 2022-10-20 12:42:24.550302 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2020_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.805070 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/__init__.py
--rw-r--r--   0        0        0     3368 2022-10-20 12:41:55.555262 tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.683038 tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2017_06/__init__.py
--rw-r--r--   0        0        0     1936 2022-10-20 12:42:24.583299 tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2017_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.732052 tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2017_12/__init__.py
--rw-r--r--   0        0        0     3439 2022-10-20 12:42:24.614305 tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2017_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.663035 tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2018_05/__init__.py
--rw-r--r--   0        0        0     6963 2022-10-20 12:42:24.650303 tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2018_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.713049 tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2018_12/__init__.py
--rw-r--r--   0        0        0     6431 2022-10-20 12:42:24.685309 tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2018_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.572031 tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2019_06/__init__.py
--rw-r--r--   0        0        0     2043 2022-10-20 12:42:24.722314 tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2019_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.720039 tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2019_12/__init__.py
--rw-r--r--   0        0        0     4182 2022-10-20 12:42:24.753315 tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2019_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.835050 tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/__init__.py
--rw-r--r--   0        0        0     1210 2022-10-20 12:41:55.573279 tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.841051 tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/_2010_04/__init__.py
--rw-r--r--   0        0        0     4263 2022-10-20 12:42:24.785318 tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.686038 tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/_2017_05/__init__.py
--rw-r--r--   0        0        0     1394 2022-10-20 12:42:24.825319 tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/_2017_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.563036 tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/_2017_11/__init__.py
--rw-r--r--   0        0        0     2108 2022-10-20 12:42:24.865328 tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/_2017_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.781046 tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/_2018_06/__init__.py
--rw-r--r--   0        0        0     2277 2022-10-20 12:42:24.903325 tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/_2018_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.911054 tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/__init__.py
--rw-r--r--   0        0        0      916 2022-10-20 12:41:55.588271 tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.989074 tcsoa-0.9.0/tcsoa/gen/Internal_Integration/_2007_06/__init__.py
--rw-r--r--   0        0        0     1319 2022-10-20 12:42:24.951334 tcsoa-0.9.0/tcsoa/gen/Internal_Integration/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.010070 tcsoa-0.9.0/tcsoa/gen/Internal_Integration/_2008_06/__init__.py
--rw-r--r--   0        0        0      755 2022-10-20 12:42:24.987337 tcsoa-0.9.0/tcsoa/gen/Internal_Integration/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.817058 tcsoa-0.9.0/tcsoa/gen/Internal_Integration/__init__.py
--rw-r--r--   0        0        0      344 2022-10-20 12:41:55.596266 tcsoa-0.9.0/tcsoa/gen/Internal_Integration/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.616029 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2008_12/__init__.py
--rw-r--r--   0        0        0     1466 2022-10-20 12:42:25.046341 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2008_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.979064 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2011_12/__init__.py
--rw-r--r--   0        0        0     1023 2022-10-20 12:42:25.089344 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2011_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.965064 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2012_09/__init__.py
--rw-r--r--   0        0        0     1629 2022-10-20 12:42:25.129352 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.801055 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2013_12/__init__.py
--rw-r--r--   0        0        0     2546 2022-10-20 12:42:25.161355 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2013_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.798053 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2014_06/__init__.py
--rw-r--r--   0        0        0     3129 2022-10-20 12:42:25.201363 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2014_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.606028 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2014_12/__init__.py
--rw-r--r--   0        0        0     8836 2022-10-20 12:42:25.273360 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2014_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.754044 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2015_03/__init__.py
--rw-r--r--   0        0        0    19450 2022-10-20 12:42:25.349401 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2015_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.918071 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2015_10/__init__.py
--rw-r--r--   0        0        0     8638 2022-10-20 12:42:25.397374 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2015_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.950068 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2016_03/__init__.py
--rw-r--r--   0        0        0     1257 2022-10-20 12:42:25.434378 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2016_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.623033 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2016_09/__init__.py
--rw-r--r--   0        0        0    25266 2022-10-20 12:42:25.524386 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2016_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.747043 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2017_05/__init__.py
--rw-r--r--   0        0        0     9922 2022-10-20 12:42:25.580400 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2017_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.013069 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2017_11/__init__.py
--rw-r--r--   0        0        0     9646 2022-10-20 12:42:25.621396 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2017_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.577032 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2018_11/__init__.py
--rw-r--r--   0        0        0     6995 2022-10-20 12:42:25.661407 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2018_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.759045 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2019_06/__init__.py
--rw-r--r--   0        0        0     5548 2022-10-20 12:42:25.713403 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2019_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.575032 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2020_01/__init__.py
--rw-r--r--   0        0        0     4246 2022-10-20 12:42:25.749415 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2020_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.575032 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2020_04/__init__.py
--rw-r--r--   0        0        0     1237 2022-10-20 12:42:25.777418 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2020_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.621029 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/__init__.py
--rw-r--r--   0        0        0     8038 2022-10-20 12:41:55.714276 tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.643038 tcsoa-0.9.0/tcsoa/gen/Internal_Mmv/_2012_09/__init__.py
--rw-r--r--   0        0        0    28667 2022-10-20 12:42:25.821416 tcsoa-0.9.0/tcsoa/gen/Internal_Mmv/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.757046 tcsoa-0.9.0/tcsoa/gen/Internal_Mmv/__init__.py
--rw-r--r--   0        0        0      561 2022-10-20 12:41:55.730276 tcsoa-0.9.0/tcsoa/gen/Internal_Mmv/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.903060 tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2007_06/__init__.py
--rw-r--r--   0        0        0    69367 2022-10-20 12:42:25.952427 tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.620029 tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2011_06/__init__.py
--rw-r--r--   0        0        0     2292 2022-10-20 12:42:26.134447 tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.784047 tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2012_02/__init__.py
--rw-r--r--   0        0        0    51330 2022-10-20 12:42:26.103445 tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2012_02/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.726040 tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2017_11/__init__.py
--rw-r--r--   0        0        0     4059 2022-10-20 12:42:26.171454 tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2017_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.772051 tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2018_06/__init__.py
--rw-r--r--   0        0        0     1391 2022-10-20 12:42:26.203449 tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2018_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.745043 tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2020_12/__init__.py
--rw-r--r--   0        0        0     1645 2022-10-20 12:42:26.234459 tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2020_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.642033 tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/__init__.py
--rw-r--r--   0        0        0      852 2022-10-20 12:41:55.878289 tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.576032 tcsoa-0.9.0/tcsoa/gen/Internal_Notification/_2014_10/__init__.py
--rw-r--r--   0        0        0     1309 2022-10-20 12:42:26.274455 tcsoa-0.9.0/tcsoa/gen/Internal_Notification/_2014_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.657040 tcsoa-0.9.0/tcsoa/gen/Internal_Notification/_2015_03/__init__.py
--rw-r--r--   0        0        0    13391 2022-10-20 12:42:26.332475 tcsoa-0.9.0/tcsoa/gen/Internal_Notification/_2015_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.974072 tcsoa-0.9.0/tcsoa/gen/Internal_Notification/_2015_10/__init__.py
--rw-r--r--   0        0        0     9350 2022-10-20 12:42:26.388475 tcsoa-0.9.0/tcsoa/gen/Internal_Notification/_2015_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.579033 tcsoa-0.9.0/tcsoa/gen/Internal_Notification/_2017_11/__init__.py
--rw-r--r--   0        0        0     2054 2022-10-20 12:42:26.418467 tcsoa-0.9.0/tcsoa/gen/Internal_Notification/_2017_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.654034 tcsoa-0.9.0/tcsoa/gen/Internal_Notification/__init__.py
--rw-r--r--   0        0        0     1833 2022-10-20 12:41:55.912295 tcsoa-0.9.0/tcsoa/gen/Internal_Notification/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.652035 tcsoa-0.9.0/tcsoa/gen/Internal_OccMgmt/_2020_05/__init__.py
--rw-r--r--   0        0        0     5378 2022-10-20 12:42:26.455485 tcsoa-0.9.0/tcsoa/gen/Internal_OccMgmt/_2020_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.660035 tcsoa-0.9.0/tcsoa/gen/Internal_OccMgmt/_2020_12/__init__.py
--rw-r--r--   0        0        0     3264 2022-10-20 12:42:26.489477 tcsoa-0.9.0/tcsoa/gen/Internal_OccMgmt/_2020_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.588032 tcsoa-0.9.0/tcsoa/gen/Internal_OccMgmt/__init__.py
--rw-r--r--   0        0        0      604 2022-10-20 12:41:55.924297 tcsoa-0.9.0/tcsoa/gen/Internal_OccMgmt/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.895056 tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/_2017_12/__init__.py
--rw-r--r--   0        0        0     3057 2022-10-20 12:42:26.521480 tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/_2017_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.717049 tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/_2018_05/__init__.py
--rw-r--r--   0        0        0     5894 2022-10-20 12:42:26.560490 tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/_2018_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.899057 tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/_2020_05/__init__.py
--rw-r--r--   0        0        0     1789 2022-10-20 12:42:26.591484 tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/_2020_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.846064 tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/_2020_12/__init__.py
--rw-r--r--   0        0        0     4495 2022-10-20 12:42:26.626492 tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/_2020_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.558030 tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/__init__.py
--rw-r--r--   0        0        0     1299 2022-10-20 12:41:55.947305 tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.934070 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2007_01/__init__.py
--rw-r--r--   0        0        0     1510 2022-10-20 12:42:26.658492 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2007_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.622030 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2007_06/__init__.py
--rw-r--r--   0        0        0     2566 2022-10-20 12:42:26.692497 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.002064 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2008_06/__init__.py
--rw-r--r--   0        0        0     2931 2022-10-20 12:42:26.727507 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.822046 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2009_10/__init__.py
--rw-r--r--   0        0        0     2259 2022-10-20 12:42:26.760499 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2009_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.759045 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2010_04/__init__.py
--rw-r--r--   0        0        0      712 2022-10-20 12:42:26.790508 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.810050 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2011_06/__init__.py
--rw-r--r--   0        0        0     2538 2022-10-20 12:42:26.824516 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.903060 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2012_02/__init__.py
--rw-r--r--   0        0        0     1040 2022-10-20 12:42:26.855521 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2012_02/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.838057 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2014_10/__init__.py
--rw-r--r--   0        0        0     3525 2022-10-20 12:42:26.886513 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2014_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.003067 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/__init__.py
--rw-r--r--   0        0        0     1622 2022-10-20 12:41:55.976306 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.826051 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagementAw/_2019_12/__init__.py
--rw-r--r--   0        0        0     1136 2022-10-20 12:42:26.920517 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagementAw/_2019_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.651040 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagementAw/__init__.py
--rw-r--r--   0        0        0      239 2022-10-20 12:41:55.982311 tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagementAw/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.819055 tcsoa-0.9.0/tcsoa/gen/Internal_Query/_2008_06/__init__.py
--rw-r--r--   0        0        0      867 2022-10-20 12:42:26.953522 tcsoa-0.9.0/tcsoa/gen/Internal_Query/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.641039 tcsoa-0.9.0/tcsoa/gen/Internal_Query/_2012_02/__init__.py
--rw-r--r--   0        0        0     1018 2022-10-20 12:42:26.986523 tcsoa-0.9.0/tcsoa/gen/Internal_Query/_2012_02/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.881065 tcsoa-0.9.0/tcsoa/gen/Internal_Query/_2013_05/__init__.py
--rw-r--r--   0        0        0     1992 2022-10-20 12:42:27.016526 tcsoa-0.9.0/tcsoa/gen/Internal_Query/_2013_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.751045 tcsoa-0.9.0/tcsoa/gen/Internal_Query/_2014_10/__init__.py
--rw-r--r--   0        0        0     2189 2022-10-20 12:42:27.044534 tcsoa-0.9.0/tcsoa/gen/Internal_Query/_2014_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.689045 tcsoa-0.9.0/tcsoa/gen/Internal_Query/__init__.py
--rw-r--r--   0        0        0      732 2022-10-20 12:41:55.993311 tcsoa-0.9.0/tcsoa/gen/Internal_Query/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.794044 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2007_06/__init__.py
--rw-r--r--   0        0        0     1878 2022-10-20 12:42:27.075540 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.558030 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2007_09/__init__.py
--rw-r--r--   0        0        0     1439 2022-10-20 12:42:27.104536 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2007_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.936066 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2008_03/__init__.py
--rw-r--r--   0        0        0     2316 2022-10-20 12:42:27.133540 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2008_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.957067 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2009_01/__init__.py
--rw-r--r--   0        0        0    15626 2022-10-20 12:42:27.182555 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2009_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.765045 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2009_04/__init__.py
--rw-r--r--   0        0        0     5056 2022-10-20 12:42:27.216544 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2009_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.869055 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2009_05/__init__.py
--rw-r--r--   0        0        0     7314 2022-10-20 12:42:27.256549 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2009_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.972071 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2010_04/__init__.py
--rw-r--r--   0        0        0     4821 2022-10-20 12:42:27.290564 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.823056 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/__init__.py
--rw-r--r--   0        0        0     2059 2022-10-20 12:41:56.032313 tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.836052 tcsoa-0.9.0/tcsoa/gen/Internal_Reports/_2007_06/__init__.py
--rw-r--r--   0        0        0     6878 2022-10-20 12:42:27.330554 tcsoa-0.9.0/tcsoa/gen/Internal_Reports/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.571032 tcsoa-0.9.0/tcsoa/gen/Internal_Reports/__init__.py
--rw-r--r--   0        0        0      575 2022-10-20 12:41:56.049323 tcsoa-0.9.0/tcsoa/gen/Internal_Reports/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.980065 tcsoa-0.9.0/tcsoa/gen/Internal_Requirementsmanagement/_2009_10/__init__.py
--rw-r--r--   0        0        0     1710 2022-10-20 12:42:27.363560 tcsoa-0.9.0/tcsoa/gen/Internal_Requirementsmanagement/_2009_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.685041 tcsoa-0.9.0/tcsoa/gen/Internal_Requirementsmanagement/_2012_02/__init__.py
--rw-r--r--   0        0        0     2021 2022-10-20 12:42:27.391567 tcsoa-0.9.0/tcsoa/gen/Internal_Requirementsmanagement/_2012_02/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.676048 tcsoa-0.9.0/tcsoa/gen/Internal_Requirementsmanagement/_2012_10/__init__.py
--rw-r--r--   0        0        0     2966 2022-10-20 12:42:27.422575 tcsoa-0.9.0/tcsoa/gen/Internal_Requirementsmanagement/_2012_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.545030 tcsoa-0.9.0/tcsoa/gen/Internal_Requirementsmanagement/__init__.py
--rw-r--r--   0        0        0      631 2022-10-20 12:41:56.059318 tcsoa-0.9.0/tcsoa/gen/Internal_Requirementsmanagement/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.624029 tcsoa-0.9.0/tcsoa/gen/Internal_RevRuleMgmt/_2019_12/__init__.py
--rw-r--r--   0        0        0     3152 2022-10-20 12:42:27.450582 tcsoa-0.9.0/tcsoa/gen/Internal_RevRuleMgmt/_2019_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.686038 tcsoa-0.9.0/tcsoa/gen/Internal_RevRuleMgmt/__init__.py
--rw-r--r--   0        0        0      313 2022-10-20 12:41:56.067319 tcsoa-0.9.0/tcsoa/gen/Internal_RevRuleMgmt/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.891059 tcsoa-0.9.0/tcsoa/gen/Internal_Search/_2020_12/__init__.py
--rw-r--r--   0        0        0     8337 2022-10-20 12:42:27.486577 tcsoa-0.9.0/tcsoa/gen/Internal_Search/_2020_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.824055 tcsoa-0.9.0/tcsoa/gen/Internal_Search/__init__.py
--rw-r--r--   0        0        0      466 2022-10-20 12:41:56.079328 tcsoa-0.9.0/tcsoa/gen/Internal_Search/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.824055 tcsoa-0.9.0/tcsoa/gen/Internal_Security/_2017_12/__init__.py
--rw-r--r--   0        0        0     1151 2022-10-20 12:42:27.515590 tcsoa-0.9.0/tcsoa/gen/Internal_Security/_2017_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.008068 tcsoa-0.9.0/tcsoa/gen/Internal_Security/__init__.py
--rw-r--r--   0        0        0      216 2022-10-20 12:41:56.085324 tcsoa-0.9.0/tcsoa/gen/Internal_Security/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.739050 tcsoa-0.9.0/tcsoa/gen/Internal_Structure/_2020_12/__init__.py
--rw-r--r--   0        0        0     1124 2022-10-20 12:42:27.543577 tcsoa-0.9.0/tcsoa/gen/Internal_Structure/_2020_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.983065 tcsoa-0.9.0/tcsoa/gen/Internal_Structure/__init__.py
--rw-r--r--   0        0        0      205 2022-10-20 12:41:56.093331 tcsoa-0.9.0/tcsoa/gen/Internal_Structure/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.904062 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2007_06/__init__.py
--rw-r--r--   0        0        0    18151 2022-10-20 12:42:27.604578 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.729050 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2007_12/__init__.py
--rw-r--r--   0        0        0     3859 2022-10-20 12:42:27.636583 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2007_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.811050 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2008_03/__init__.py
--rw-r--r--   0        0        0     1067 2022-10-20 12:42:27.666592 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2008_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.940067 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2008_05/__init__.py
--rw-r--r--   0        0        0     3841 2022-10-20 12:42:27.701594 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2008_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.593027 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2008_06/__init__.py
--rw-r--r--   0        0        0     2042 2022-10-20 12:42:27.734603 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.827050 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2009_10/__init__.py
--rw-r--r--   0        0        0     3168 2022-10-20 12:42:27.768596 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2009_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.649034 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2010_04/__init__.py
--rw-r--r--   0        0        0     5988 2022-10-20 12:42:27.802610 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.632037 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2010_09/__init__.py
--rw-r--r--   0        0        0     1017 2022-10-20 12:42:27.832604 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2010_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.969063 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2011_06/__init__.py
--rw-r--r--   0        0        0    10947 2022-10-20 12:42:27.886636 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.990099 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2012_02/__init__.py
--rw-r--r--   0        0        0     1971 2022-10-20 12:42:27.918619 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2012_02/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.806049 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2012_09/__init__.py
--rw-r--r--   0        0        0     1168 2022-10-20 12:42:27.947613 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.704043 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2013_05/__init__.py
--rw-r--r--   0        0        0     6389 2022-10-20 12:42:27.984616 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2013_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.977064 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2013_12/__init__.py
--rw-r--r--   0        0        0     6530 2022-10-20 12:42:28.021626 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2013_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.873056 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2014_12/__init__.py
--rw-r--r--   0        0        0    12680 2022-10-20 12:42:28.073626 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2014_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.602028 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2015_10/__init__.py
--rw-r--r--   0        0        0     2494 2022-10-20 12:42:28.103646 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2015_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.972071 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2016_03/__init__.py
--rw-r--r--   0        0        0     2739 2022-10-20 12:42:28.137638 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2016_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.814050 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2016_10/__init__.py
--rw-r--r--   0        0        0     6685 2022-10-20 12:42:28.168640 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2016_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.559030 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2017_05/__init__.py
--rw-r--r--   0        0        0     7427 2022-10-20 12:42:28.216638 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2017_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.779053 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2018_11/__init__.py
--rw-r--r--   0        0        0     5557 2022-10-20 12:42:28.256642 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2018_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.655037 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2019_06/__init__.py
--rw-r--r--   0        0        0     1620 2022-10-20 12:42:28.287643 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2019_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.831050 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2020_05/__init__.py
--rw-r--r--   0        0        0     2774 2022-10-20 12:42:28.320656 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2020_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.755045 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/__init__.py
--rw-r--r--   0        0        0     7990 2022-10-20 12:41:56.205330 tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.724039 tcsoa-0.9.0/tcsoa/gen/Internal_TCXMLImportExport/_2020_12/__init__.py
--rw-r--r--   0        0        0     3247 2022-10-20 12:42:28.353656 tcsoa-0.9.0/tcsoa/gen/Internal_TCXMLImportExport/_2020_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.001066 tcsoa-0.9.0/tcsoa/gen/Internal_TCXMLImportExport/__init__.py
--rw-r--r--   0        0        0      443 2022-10-20 12:41:56.215333 tcsoa-0.9.0/tcsoa/gen/Internal_TCXMLImportExport/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.981072 tcsoa-0.9.0/tcsoa/gen/Internal_Translation/_2007_06/__init__.py
--rw-r--r--   0        0        0     4024 2022-10-20 12:42:28.390653 tcsoa-0.9.0/tcsoa/gen/Internal_Translation/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.945063 tcsoa-0.9.0/tcsoa/gen/Internal_Translation/__init__.py
--rw-r--r--   0        0        0      421 2022-10-20 12:41:56.225335 tcsoa-0.9.0/tcsoa/gen/Internal_Translation/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.863060 tcsoa-0.9.0/tcsoa/gen/Internal_UiConfig/_2014_11/__init__.py
--rw-r--r--   0        0        0      924 2022-10-20 12:42:28.421657 tcsoa-0.9.0/tcsoa/gen/Internal_UiConfig/_2014_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.709040 tcsoa-0.9.0/tcsoa/gen/Internal_UiConfig/__init__.py
--rw-r--r--   0        0        0      198 2022-10-20 12:41:56.232336 tcsoa-0.9.0/tcsoa/gen/Internal_UiConfig/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.949068 tcsoa-0.9.0/tcsoa/gen/Internal_Validation/_2007_06/__init__.py
--rw-r--r--   0        0        0     6911 2022-10-20 12:42:28.456658 tcsoa-0.9.0/tcsoa/gen/Internal_Validation/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.595030 tcsoa-0.9.0/tcsoa/gen/Internal_Validation/_2008_06/__init__.py
--rw-r--r--   0        0        0     4109 2022-10-20 12:42:28.489667 tcsoa-0.9.0/tcsoa/gen/Internal_Validation/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.995072 tcsoa-0.9.0/tcsoa/gen/Internal_Validation/_2010_04/__init__.py
--rw-r--r--   0        0        0     6863 2022-10-20 12:42:28.523672 tcsoa-0.9.0/tcsoa/gen/Internal_Validation/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.977064 tcsoa-0.9.0/tcsoa/gen/Internal_Validation/_2012_02/__init__.py
--rw-r--r--   0        0        0     3039 2022-10-20 12:42:28.558670 tcsoa-0.9.0/tcsoa/gen/Internal_Validation/_2012_02/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.840051 tcsoa-0.9.0/tcsoa/gen/Internal_Validation/__init__.py
--rw-r--r--   0        0        0     1151 2022-10-20 12:41:56.257333 tcsoa-0.9.0/tcsoa/gen/Internal_Validation/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.992071 tcsoa-0.9.0/tcsoa/gen/Internal_Vendormanagement/_2008_05/__init__.py
--rw-r--r--   0        0        0     3038 2022-10-20 12:42:28.686687 tcsoa-0.9.0/tcsoa/gen/Internal_Vendormanagement/_2008_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.942067 tcsoa-0.9.0/tcsoa/gen/Internal_Vendormanagement/_2008_06/__init__.py
--rw-r--r--   0        0        0     1103 2022-10-20 12:42:28.714681 tcsoa-0.9.0/tcsoa/gen/Internal_Vendormanagement/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.947068 tcsoa-0.9.0/tcsoa/gen/Internal_Vendormanagement/__init__.py
--rw-r--r--   0        0        0      441 2022-10-20 12:41:56.284342 tcsoa-0.9.0/tcsoa/gen/Internal_Vendormanagement/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.795051 tcsoa-0.9.0/tcsoa/gen/Internal_VendorManagementAW/_2019_12/__init__.py
--rw-r--r--   0        0        0     3174 2022-10-20 12:42:28.593673 tcsoa-0.9.0/tcsoa/gen/Internal_VendorManagementAW/_2019_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.864060 tcsoa-0.9.0/tcsoa/gen/Internal_VendorManagementAW/_2020_05/__init__.py
--rw-r--r--   0        0        0     2506 2022-10-20 12:42:28.627674 tcsoa-0.9.0/tcsoa/gen/Internal_VendorManagementAW/_2020_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.660035 tcsoa-0.9.0/tcsoa/gen/Internal_VendorManagementAW/_2020_12/__init__.py
--rw-r--r--   0        0        0      908 2022-10-20 12:42:28.656686 tcsoa-0.9.0/tcsoa/gen/Internal_VendorManagementAW/_2020_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.880064 tcsoa-0.9.0/tcsoa/gen/Internal_VendorManagementAW/__init__.py
--rw-r--r--   0        0        0      946 2022-10-20 12:41:56.274341 tcsoa-0.9.0/tcsoa/gen/Internal_VendorManagementAW/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.888056 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2008_06/__init__.py
--rw-r--r--   0        0        0    86551 2022-10-20 12:42:28.781696 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.675045 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2010_04/__init__.py
--rw-r--r--   0        0        0     4872 2022-10-20 12:42:28.810699 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.857059 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2010_09/__init__.py
--rw-r--r--   0        0        0    40577 2022-10-20 12:42:28.857717 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2010_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.724039 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2011_12/__init__.py
--rw-r--r--   0        0        0     5475 2022-10-20 12:42:28.884697 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2011_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.950068 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2012_10/__init__.py
--rw-r--r--   0        0        0     4994 2022-10-20 12:42:28.915705 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2012_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.879055 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2017_05/__init__.py
--rw-r--r--   0        0        0     9476 2022-10-20 12:42:28.945715 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2017_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.707045 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2018_11/__init__.py
--rw-r--r--   0        0        0     4916 2022-10-20 12:42:28.974705 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2018_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.865059 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/__init__.py
--rw-r--r--   0        0        0     2433 2022-10-20 12:41:56.335343 tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.658041 tcsoa-0.9.0/tcsoa/gen/Internal_Workflow/_2013_05/__init__.py
--rw-r--r--   0        0        0     1678 2022-10-20 12:42:29.006718 tcsoa-0.9.0/tcsoa/gen/Internal_Workflow/_2013_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.679048 tcsoa-0.9.0/tcsoa/gen/Internal_Workflow/_2017_11/__init__.py
--rw-r--r--   0        0        0     1592 2022-10-20 12:42:29.035726 tcsoa-0.9.0/tcsoa/gen/Internal_Workflow/_2017_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.553037 tcsoa-0.9.0/tcsoa/gen/Internal_Workflow/__init__.py
--rw-r--r--   0        0        0      341 2022-10-20 12:41:56.346350 tcsoa-0.9.0/tcsoa/gen/Internal_Workflow/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.939068 tcsoa-0.9.0/tcsoa/gen/Internal_Workflowaw/_2020_12/__init__.py
--rw-r--r--   0        0        0     2806 2022-10-20 12:42:29.070716 tcsoa-0.9.0/tcsoa/gen/Internal_Workflowaw/_2020_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.664040 tcsoa-0.9.0/tcsoa/gen/Internal_Workflowaw/__init__.py
--rw-r--r--   0        0        0      296 2022-10-20 12:41:56.354349 tcsoa-0.9.0/tcsoa/gen/Internal_Workflowaw/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.004068 tcsoa-0.9.0/tcsoa/gen/Internal_XlsBom/_2020_12/__init__.py
--rw-r--r--   0        0        0     4684 2022-10-20 12:42:29.106718 tcsoa-0.9.0/tcsoa/gen/Internal_XlsBom/_2020_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.715046 tcsoa-0.9.0/tcsoa/gen/Internal_XlsBom/__init__.py
--rw-r--r--   0        0        0      372 2022-10-20 12:41:56.363352 tcsoa-0.9.0/tcsoa/gen/Internal_XlsBom/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.662042 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2008_06/__init__.py
--rw-r--r--   0        0        0      742 2022-10-20 12:42:55.474190 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2008_06/Core.py
--rw-r--r--   0        0        0     4007 2022-10-20 12:42:55.531190 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2008_06/DataManagement.py
--rw-r--r--   0        0        0     4299 2022-10-20 12:42:29.151724 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2008_06/services.py
--rw-r--r--   0        0        0     2672 2022-10-20 12:42:55.581194 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2008_06/TimeManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.787047 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2008_12/__init__.py
--rw-r--r--   0        0        0     2393 2022-10-20 12:42:55.624207 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2008_12/IPAManagement.py
--rw-r--r--   0        0        0     2608 2022-10-20 12:42:29.187726 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2008_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.615033 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_06/__init__.py
--rw-r--r--   0        0        0     6507 2022-10-20 12:42:29.229732 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_06/services.py
--rw-r--r--   0        0        0     3867 2022-10-20 12:42:55.679197 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_06/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.567031 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/__init__.py
--rw-r--r--   0        0        0     5002 2022-10-20 12:42:55.735204 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/DataManagement.py
--rw-r--r--   0        0        0     3663 2022-10-20 12:42:55.795209 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/MFGPropertyCollector.py
--rw-r--r--   0        0        0     4241 2022-10-20 12:42:55.872219 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/Model.py
--rw-r--r--   0        0        0     5501 2022-10-20 12:42:55.941231 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/ModelDefinitions.py
--rw-r--r--   0        0        0    12624 2022-10-20 12:42:29.318745 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/services.py
--rw-r--r--   0        0        0     2532 2022-10-20 12:42:55.978230 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/StructureManagement.py
--rw-r--r--   0        0        0    15212 2022-10-20 12:42:56.121240 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/StructureSearch.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.772051 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2010_09/__init__.py
--rw-r--r--   0        0        0     2732 2022-10-20 12:42:56.169244 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2010_09/Core.py
--rw-r--r--   0        0        0      932 2022-10-20 12:42:56.200246 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2010_09/ImportExport.py
--rw-r--r--   0        0        0     5522 2022-10-20 12:42:29.368745 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2010_09/services.py
--rw-r--r--   0        0        0     2623 2022-10-20 12:42:56.241255 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2010_09/TimeManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.834055 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2011_06/__init__.py
--rw-r--r--   0        0        0     2831 2022-10-20 12:42:56.287284 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2011_06/DataManagement.py
--rw-r--r--   0        0        0     3809 2022-10-20 12:42:29.413767 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2011_06/services.py
--rw-r--r--   0        0        0     1459 2022-10-20 12:42:56.325266 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2011_06/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.822046 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_02/__init__.py
--rw-r--r--   0        0        0    13085 2022-10-20 12:42:56.441276 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_02/Constraints.py
--rw-r--r--   0        0        0     9281 2022-10-20 12:42:56.540284 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_02/DataManagement.py
--rw-r--r--   0        0        0     1323 2022-10-20 12:42:56.577288 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_02/IPAManagement.py
--rw-r--r--   0        0        0     4670 2022-10-20 12:42:56.633293 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_02/Model.py
--rw-r--r--   0        0        0    16739 2022-10-20 12:42:29.489763 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_02/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.996070 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_09/__init__.py
--rw-r--r--   0        0        0     2417 2022-10-20 12:42:56.675291 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_09/DataManagement.py
--rw-r--r--   0        0        0     2665 2022-10-20 12:42:29.528768 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_09/services.py
--rw-r--r--   0        0        0     2777 2022-10-20 12:42:56.726309 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_09/Validation.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.784047 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/__init__.py
--rw-r--r--   0        0        0     4065 2022-10-20 12:42:56.769303 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/Core.py
--rw-r--r--   0        0        0     3173 2022-10-20 12:42:56.817307 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/DataManagement.py
--rw-r--r--   0        0        0     2488 2022-10-20 12:42:56.932314 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/ImportExport.py
--rw-r--r--   0        0        0     7953 2022-10-20 12:42:56.893311 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/IPAManagement.py
--rw-r--r--   0        0        0    16030 2022-10-20 12:42:29.609778 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/services.py
--rw-r--r--   0        0        0     1867 2022-10-20 12:42:56.969327 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/StructureManagement.py
--rw-r--r--   0        0        0      808 2022-10-20 12:42:56.999328 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/StructureSearch.py
--rw-r--r--   0        0        0     6991 2022-10-20 12:42:57.046330 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/TimeWayPlan.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.675045 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_12/__init__.py
--rw-r--r--   0        0        0     2892 2022-10-20 12:42:57.094356 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_12/Model.py
--rw-r--r--   0        0        0     5391 2022-10-20 12:42:57.145341 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_12/ResourceManagement.py
--rw-r--r--   0        0        0     9586 2022-10-20 12:42:29.653772 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.004068 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_06/__init__.py
--rw-r--r--   0        0        0     9722 2022-10-20 12:42:57.211341 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_06/DataManagement.py
--rw-r--r--   0        0        0     1198 2022-10-20 12:42:57.242352 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_06/ResourceManagement.py
--rw-r--r--   0        0        0    10941 2022-10-20 12:42:29.701774 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_06/services.py
--rw-r--r--   0        0        0      930 2022-10-20 12:42:57.274360 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_06/StructureSearch.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.661045 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_12/__init__.py
--rw-r--r--   0        0        0     5016 2022-10-20 12:42:57.338359 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_12/IPAManagement.py
--rw-r--r--   0        0        0     1984 2022-10-20 12:42:57.380362 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_12/Model.py
--rw-r--r--   0        0        0    10871 2022-10-20 12:42:29.756790 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_12/services.py
--rw-r--r--   0        0        0     8254 2022-10-20 12:42:57.443366 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_12/StructureSearch.py
--rw-r--r--   0        0        0     5967 2022-10-20 12:42:57.484372 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_12/Validation.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.788046 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2015_03/__init__.py
--rw-r--r--   0        0        0     3142 2022-10-20 12:42:29.786783 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2015_03/services.py
--rw-r--r--   0        0        0     3452 2022-10-20 12:42:57.517370 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2015_03/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.570034 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2015_10/__init__.py
--rw-r--r--   0        0        0     1979 2022-10-20 12:42:57.554377 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2015_10/ImportExport.py
--rw-r--r--   0        0        0     3131 2022-10-20 12:42:29.820788 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2015_10/services.py
--rw-r--r--   0        0        0     5831 2022-10-20 12:42:57.595382 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2015_10/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.584030 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2016_03/__init__.py
--rw-r--r--   0        0        0     2953 2022-10-20 12:42:57.633381 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2016_03/ImportExport.py
--rw-r--r--   0        0        0     4080 2022-10-20 12:42:29.850797 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2016_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.915058 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2017_05/__init__.py
--rw-r--r--   0        0        0     1114 2022-10-20 12:42:57.659390 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2017_05/ImportExport.py
--rw-r--r--   0        0        0     2630 2022-10-20 12:42:29.884796 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2017_05/services.py
--rw-r--r--   0        0        0     1220 2022-10-20 12:42:57.691395 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2017_05/Validation.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.990099 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2017_11/__init__.py
--rw-r--r--   0        0        0    10399 2022-10-20 12:42:57.757393 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2017_11/DataManagement.py
--rw-r--r--   0        0        0     7317 2022-10-20 12:42:29.920801 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2017_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.564032 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2018_06/__init__.py
--rw-r--r--   0        0        0     3063 2022-10-20 12:42:57.794399 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2018_06/DataManagement.py
--rw-r--r--   0        0        0     2535 2022-10-20 12:42:29.949799 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2018_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.918071 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2018_11/__init__.py
--rw-r--r--   0        0        0     2965 2022-10-20 12:42:29.980803 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2018_11/services.py
--rw-r--r--   0        0        0     7415 2022-10-20 12:42:57.864407 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2018_11/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.898059 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2019_06/__init__.py
--rw-r--r--   0        0        0     1679 2022-10-20 12:42:57.898410 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2019_06/DataManagement.py
--rw-r--r--   0        0        0     2860 2022-10-20 12:42:30.014816 tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2019_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.985066 tcsoa-0.9.0/tcsoa/gen/Manufacturing/__init__.py
--rw-r--r--   0        0        0    11688 2022-10-20 12:41:56.555362 tcsoa-0.9.0/tcsoa/gen/Manufacturing/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.762045 tcsoa-0.9.0/tcsoa/gen/Multisite/_2007_06/__init__.py
--rw-r--r--   0        0        0     1265 2022-10-20 12:42:57.930433 tcsoa-0.9.0/tcsoa/gen/Multisite/_2007_06/ImportExport.py
--rw-r--r--   0        0        0     2257 2022-10-20 12:42:30.043818 tcsoa-0.9.0/tcsoa/gen/Multisite/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.603029 tcsoa-0.9.0/tcsoa/gen/Multisite/_2011_06/__init__.py
--rw-r--r--   0        0        0     4459 2022-10-20 12:42:30.076818 tcsoa-0.9.0/tcsoa/gen/Multisite/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.639047 tcsoa-0.9.0/tcsoa/gen/Multisite/_2014_10/__init__.py
--rw-r--r--   0        0        0    15651 2022-10-20 12:42:58.003422 tcsoa-0.9.0/tcsoa/gen/Multisite/_2014_10/ImportExportTCXML.py
--rw-r--r--   0        0        0     4310 2022-10-20 12:42:30.111822 tcsoa-0.9.0/tcsoa/gen/Multisite/_2014_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.692046 tcsoa-0.9.0/tcsoa/gen/Multisite/_2019_06/__init__.py
--rw-r--r--   0        0        0     2426 2022-10-20 12:42:58.046426 tcsoa-0.9.0/tcsoa/gen/Multisite/_2019_06/ImportExportTCXML.py
--rw-r--r--   0        0        0     1359 2022-10-20 12:42:58.078432 tcsoa-0.9.0/tcsoa/gen/Multisite/_2019_06/Search.py
--rw-r--r--   0        0        0     5558 2022-10-20 12:42:30.152834 tcsoa-0.9.0/tcsoa/gen/Multisite/_2019_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.997071 tcsoa-0.9.0/tcsoa/gen/Multisite/__init__.py
--rw-r--r--   0        0        0      953 2022-10-20 12:41:56.576367 tcsoa-0.9.0/tcsoa/gen/Multisite/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.623033 tcsoa-0.9.0/tcsoa/gen/Notification/_2014_10/__init__.py
--rw-r--r--   0        0        0     7060 2022-10-20 12:42:30.189828 tcsoa-0.9.0/tcsoa/gen/Notification/_2014_10/services.py
--rw-r--r--   0        0        0    10914 2022-10-20 12:42:18.324716 tcsoa-0.9.0/tcsoa/gen/Notification/_2014_10/SubscriptionManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.829051 tcsoa-0.9.0/tcsoa/gen/Notification/__init__.py
--rw-r--r--   0        0        0      377 2022-10-20 12:41:56.588368 tcsoa-0.9.0/tcsoa/gen/Notification/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.817058 tcsoa-0.9.0/tcsoa/gen/OfficeOnline/_2017_11/__init__.py
--rw-r--r--   0        0        0     2123 2022-10-20 12:42:30.255829 tcsoa-0.9.0/tcsoa/gen/OfficeOnline/_2017_11/OfficeOnline.py
--rw-r--r--   0        0        0     1768 2022-10-20 12:42:30.217824 tcsoa-0.9.0/tcsoa/gen/OfficeOnline/_2017_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.677047 tcsoa-0.9.0/tcsoa/gen/OfficeOnline/__init__.py
--rw-r--r--   0        0        0      199 2022-10-20 12:41:56.594381 tcsoa-0.9.0/tcsoa/gen/OfficeOnline/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.979064 tcsoa-0.9.0/tcsoa/gen/Participant/_2018_11/__init__.py
--rw-r--r--   0        0        0     6357 2022-10-20 12:42:18.388756 tcsoa-0.9.0/tcsoa/gen/Participant/_2018_11/Participant.py
--rw-r--r--   0        0        0     3611 2022-10-20 12:42:30.288842 tcsoa-0.9.0/tcsoa/gen/Participant/_2018_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.793051 tcsoa-0.9.0/tcsoa/gen/Participant/__init__.py
--rw-r--r--   0        0        0      304 2022-10-20 12:41:56.604380 tcsoa-0.9.0/tcsoa/gen/Participant/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.833056 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_01/__init__.py
--rw-r--r--   0        0        0     5604 2022-10-20 12:42:58.139433 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_01/ScheduleManagement.py
--rw-r--r--   0        0        0     6274 2022-10-20 12:42:30.710876 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.704043 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_06/__init__.py
--rw-r--r--   0        0        0     5847 2022-10-20 12:42:58.202436 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_06/ScheduleManagement.py
--rw-r--r--   0        0        0     5070 2022-10-20 12:42:30.749879 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.596030 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_12/__init__.py
--rw-r--r--   0        0        0     2706 2022-10-20 12:42:58.249434 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_12/ScheduleManagement.py
--rw-r--r--   0        0        0      853 2022-10-20 12:42:30.780882 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.706044 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2008_06/__init__.py
--rw-r--r--   0        0        0    17407 2022-10-20 12:42:58.363453 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2008_06/ScheduleManagement.py
--rw-r--r--   0        0        0     5856 2022-10-20 12:42:30.818883 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.944079 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2009_10/__init__.py
--rw-r--r--   0        0        0     4732 2022-10-20 12:42:58.413452 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2009_10/ScheduleManagement.py
--rw-r--r--   0        0        0     1637 2022-10-20 12:42:30.850884 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2009_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.863060 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_02/__init__.py
--rw-r--r--   0        0        0     4207 2022-10-20 12:42:58.483459 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_02/ScheduleManagement.py
--rw-r--r--   0        0        0      844 2022-10-20 12:42:30.879887 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_02/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.668044 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_06/__init__.py
--rw-r--r--   0        0        0    16136 2022-10-20 12:42:58.654474 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_06/ScheduleManagement.py
--rw-r--r--   0        0        0    10145 2022-10-20 12:42:30.925896 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.722046 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_12/__init__.py
--rw-r--r--   0        0        0     1128 2022-10-20 12:42:58.687477 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_12/ScheduleManagement.py
--rw-r--r--   0        0        0     1202 2022-10-20 12:42:30.954892 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.878055 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2012_02/__init__.py
--rw-r--r--   0        0        0     7126 2022-10-20 12:42:58.777493 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2012_02/ScheduleManagement.py
--rw-r--r--   0        0        0    15276 2022-10-20 12:42:31.033901 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2012_02/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.565032 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2012_09/__init__.py
--rw-r--r--   0        0        0      819 2022-10-20 12:42:58.805488 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2012_09/ScheduleManagement.py
--rw-r--r--   0        0        0     1599 2022-10-20 12:42:31.065910 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.700049 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2014_06/__init__.py
--rw-r--r--   0        0        0     3034 2022-10-20 12:42:58.849499 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2014_06/ScheduleManagement.py
--rw-r--r--   0        0        0     1107 2022-10-20 12:42:31.099908 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2014_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.747043 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2014_10/__init__.py
--rw-r--r--   0        0        0    10136 2022-10-20 12:42:58.943510 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2014_10/ScheduleManagement.py
--rw-r--r--   0        0        0    10125 2022-10-20 12:42:31.145910 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2014_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.896060 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2015_07/__init__.py
--rw-r--r--   0        0        0      745 2022-10-20 12:42:58.970505 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2015_07/ScheduleManagement.py
--rw-r--r--   0        0        0     2625 2022-10-20 12:42:31.180917 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2015_07/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.593027 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2016_04/__init__.py
--rw-r--r--   0        0        0     1706 2022-10-20 12:42:31.210919 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2016_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.770065 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2017_11/__init__.py
--rw-r--r--   0        0        0      860 2022-10-20 12:42:58.997522 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2017_11/ScheduleManagement.py
--rw-r--r--   0        0        0     2157 2022-10-20 12:42:31.238942 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2017_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.780047 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2018_11/__init__.py
--rw-r--r--   0        0        0     1780 2022-10-20 12:42:31.267922 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2018_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.738043 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/__init__.py
--rw-r--r--   0        0        0     5095 2022-10-20 12:41:56.718383 tcsoa-0.9.0/tcsoa/gen/ProjectManagement/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.617030 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2015_07/__init__.py
--rw-r--r--   0        0        0     2361 2022-10-20 12:42:32.837067 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2015_07/ScheduleManagementAw.py
--rw-r--r--   0        0        0     1021 2022-10-20 12:42:31.294924 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2015_07/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.910058 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2016_12/__init__.py
--rw-r--r--   0        0        0     4660 2022-10-20 12:42:32.880072 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2016_12/ScheduleManagementAw.py
--rw-r--r--   0        0        0     4424 2022-10-20 12:42:31.329933 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2016_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.751045 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2017_06/__init__.py
--rw-r--r--   0        0        0      712 2022-10-20 12:42:32.907079 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2017_06/ScheduleManagementAw.py
--rw-r--r--   0        0        0     2110 2022-10-20 12:42:31.358931 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2017_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.655037 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2018_12/__init__.py
--rw-r--r--   0        0        0     8743 2022-10-20 12:42:32.981083 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2018_12/ScheduleManagementAw.py
--rw-r--r--   0        0        0     6685 2022-10-20 12:42:31.399940 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2018_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.644039 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2019_06/__init__.py
--rw-r--r--   0        0        0     3980 2022-10-20 12:42:33.026088 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2019_06/ScheduleManagementAw.py
--rw-r--r--   0        0        0     1955 2022-10-20 12:42:31.430945 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2019_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.826051 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2020_05/__init__.py
--rw-r--r--   0        0        0     3056 2022-10-20 12:42:33.076090 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2020_05/ScheduleManagementAw.py
--rw-r--r--   0        0        0     3139 2022-10-20 12:42:31.463944 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2020_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.700049 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/__init__.py
--rw-r--r--   0        0        0     1747 2022-10-20 12:41:56.754397 tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.611029 tcsoa-0.9.0/tcsoa/gen/Qualification/_2014_06/__init__.py
--rw-r--r--   0        0        0     3225 2022-10-20 12:42:18.441727 tcsoa-0.9.0/tcsoa/gen/Qualification/_2014_06/QualificationManagement.py
--rw-r--r--   0        0        0     4289 2022-10-20 12:42:31.500942 tcsoa-0.9.0/tcsoa/gen/Qualification/_2014_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.868058 tcsoa-0.9.0/tcsoa/gen/Qualification/__init__.py
--rw-r--r--   0        0        0      530 2022-10-20 12:41:56.769398 tcsoa-0.9.0/tcsoa/gen/Qualification/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.589039 tcsoa-0.9.0/tcsoa/gen/Query/_2006_03/__init__.py
--rw-r--r--   0        0        0     2791 2022-10-20 12:42:59.051511 tcsoa-0.9.0/tcsoa/gen/Query/_2006_03/SavedQuery.py
--rw-r--r--   0        0        0     4058 2022-10-20 12:42:31.532973 tcsoa-0.9.0/tcsoa/gen/Query/_2006_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.597028 tcsoa-0.9.0/tcsoa/gen/Query/_2007_01/__init__.py
--rw-r--r--   0        0        0      924 2022-10-20 12:42:59.084522 tcsoa-0.9.0/tcsoa/gen/Query/_2007_01/SavedQuery.py
--rw-r--r--   0        0        0     3590 2022-10-20 12:42:31.564948 tcsoa-0.9.0/tcsoa/gen/Query/_2007_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.589039 tcsoa-0.9.0/tcsoa/gen/Query/_2007_06/__init__.py
--rw-r--r--   0        0        0     3437 2022-10-20 12:42:59.132526 tcsoa-0.9.0/tcsoa/gen/Query/_2007_06/Finder.py
--rw-r--r--   0        0        0     5401 2022-10-20 12:42:59.180524 tcsoa-0.9.0/tcsoa/gen/Query/_2007_06/SavedQuery.py
--rw-r--r--   0        0        0     4894 2022-10-20 12:42:31.603959 tcsoa-0.9.0/tcsoa/gen/Query/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.837052 tcsoa-0.9.0/tcsoa/gen/Query/_2007_09/__init__.py
--rw-r--r--   0        0        0     3602 2022-10-20 12:42:59.217528 tcsoa-0.9.0/tcsoa/gen/Query/_2007_09/SavedQuery.py
--rw-r--r--   0        0        0     1699 2022-10-20 12:42:31.631971 tcsoa-0.9.0/tcsoa/gen/Query/_2007_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.664040 tcsoa-0.9.0/tcsoa/gen/Query/_2008_06/__init__.py
--rw-r--r--   0        0        0     1961 2022-10-20 12:42:59.245527 tcsoa-0.9.0/tcsoa/gen/Query/_2008_06/SavedQuery.py
--rw-r--r--   0        0        0     1833 2022-10-20 12:42:31.658965 tcsoa-0.9.0/tcsoa/gen/Query/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.618030 tcsoa-0.9.0/tcsoa/gen/Query/_2010_04/__init__.py
--rw-r--r--   0        0        0      966 2022-10-20 12:42:59.279539 tcsoa-0.9.0/tcsoa/gen/Query/_2010_04/SavedQuery.py
--rw-r--r--   0        0        0     1268 2022-10-20 12:42:31.685968 tcsoa-0.9.0/tcsoa/gen/Query/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.954086 tcsoa-0.9.0/tcsoa/gen/Query/_2010_09/__init__.py
--rw-r--r--   0        0        0     1550 2022-10-20 12:42:59.310562 tcsoa-0.9.0/tcsoa/gen/Query/_2010_09/SavedQuery.py
--rw-r--r--   0        0        0      913 2022-10-20 12:42:31.713969 tcsoa-0.9.0/tcsoa/gen/Query/_2010_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.924063 tcsoa-0.9.0/tcsoa/gen/Query/_2012_10/__init__.py
--rw-r--r--   0        0        0     6352 2022-10-20 12:42:59.373543 tcsoa-0.9.0/tcsoa/gen/Query/_2012_10/Finder.py
--rw-r--r--   0        0        0     2727 2022-10-20 12:42:31.740973 tcsoa-0.9.0/tcsoa/gen/Query/_2012_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.699049 tcsoa-0.9.0/tcsoa/gen/Query/_2013_05/__init__.py
--rw-r--r--   0        0        0     1214 2022-10-20 12:42:59.399551 tcsoa-0.9.0/tcsoa/gen/Query/_2013_05/SavedQuery.py
--rw-r--r--   0        0        0      747 2022-10-20 12:42:31.768969 tcsoa-0.9.0/tcsoa/gen/Query/_2013_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.786052 tcsoa-0.9.0/tcsoa/gen/Query/_2014_11/__init__.py
--rw-r--r--   0        0        0     8606 2022-10-20 12:42:59.460556 tcsoa-0.9.0/tcsoa/gen/Query/_2014_11/Finder.py
--rw-r--r--   0        0        0     4418 2022-10-20 12:42:31.800974 tcsoa-0.9.0/tcsoa/gen/Query/_2014_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.938068 tcsoa-0.9.0/tcsoa/gen/Query/_2018_11/__init__.py
--rw-r--r--   0        0        0     1784 2022-10-20 12:42:59.487557 tcsoa-0.9.0/tcsoa/gen/Query/_2018_11/SavedQuery.py
--rw-r--r--   0        0        0     5364 2022-10-20 12:42:31.830976 tcsoa-0.9.0/tcsoa/gen/Query/_2018_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.013069 tcsoa-0.9.0/tcsoa/gen/Query/_2019_06/__init__.py
--rw-r--r--   0        0        0     2235 2022-10-20 12:42:59.524555 tcsoa-0.9.0/tcsoa/gen/Query/_2019_06/SavedQuery.py
--rw-r--r--   0        0        0      812 2022-10-20 12:42:31.859984 tcsoa-0.9.0/tcsoa/gen/Query/_2019_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.632037 tcsoa-0.9.0/tcsoa/gen/Query/_2020_04/__init__.py
--rw-r--r--   0        0        0     2109 2022-10-20 12:42:59.552564 tcsoa-0.9.0/tcsoa/gen/Query/_2020_04/SavedQuery.py
--rw-r--r--   0        0        0     4719 2022-10-20 12:42:31.890982 tcsoa-0.9.0/tcsoa/gen/Query/_2020_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.610029 tcsoa-0.9.0/tcsoa/gen/Query/__init__.py
--rw-r--r--   0        0        0     2346 2022-10-20 12:41:56.809392 tcsoa-0.9.0/tcsoa/gen/Query/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.934070 tcsoa-0.9.0/tcsoa/gen/Rdv/_2008_05/__init__.py
--rw-r--r--   0        0        0     4737 2022-10-20 12:42:59.614571 tcsoa-0.9.0/tcsoa/gen/Rdv/_2008_05/ContextManagement.py
--rw-r--r--   0        0        0     4555 2022-10-20 12:42:31.925988 tcsoa-0.9.0/tcsoa/gen/Rdv/_2008_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.854061 tcsoa-0.9.0/tcsoa/gen/Rdv/_2009_04/__init__.py
--rw-r--r--   0        0        0     1824 2022-10-20 12:42:59.645574 tcsoa-0.9.0/tcsoa/gen/Rdv/_2009_04/ContextManagement.py
--rw-r--r--   0        0        0     2588 2022-10-20 12:42:31.956983 tcsoa-0.9.0/tcsoa/gen/Rdv/_2009_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.906076 tcsoa-0.9.0/tcsoa/gen/Rdv/_2010_09/__init__.py
--rw-r--r--   0        0        0     4097 2022-10-20 12:42:59.695576 tcsoa-0.9.0/tcsoa/gen/Rdv/_2010_09/ContextManagement.py
--rw-r--r--   0        0        0     3719 2022-10-20 12:42:31.987989 tcsoa-0.9.0/tcsoa/gen/Rdv/_2010_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.773053 tcsoa-0.9.0/tcsoa/gen/Rdv/_2012_09/__init__.py
--rw-r--r--   0        0        0     7785 2022-10-20 12:42:59.766589 tcsoa-0.9.0/tcsoa/gen/Rdv/_2012_09/ContextManagement.py
--rw-r--r--   0        0        0     9835 2022-10-20 12:42:32.024994 tcsoa-0.9.0/tcsoa/gen/Rdv/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.839051 tcsoa-0.9.0/tcsoa/gen/Rdv/_2013_05/__init__.py
--rw-r--r--   0        0        0     1284 2022-10-20 12:42:59.793581 tcsoa-0.9.0/tcsoa/gen/Rdv/_2013_05/ContextManagement.py
--rw-r--r--   0        0        0     3889 2022-10-20 12:42:32.054995 tcsoa-0.9.0/tcsoa/gen/Rdv/_2013_05/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.542030 tcsoa-0.9.0/tcsoa/gen/Rdv/__init__.py
--rw-r--r--   0        0        0     1196 2022-10-20 12:41:56.836401 tcsoa-0.9.0/tcsoa/gen/Rdv/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.727040 tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/_2012_10/__init__.py
--rw-r--r--   0        0        0    11494 2022-10-20 12:42:32.659063 tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/_2012_10/NetworkEngine.py
--rw-r--r--   0        0        0     5852 2022-10-20 12:42:32.090000 tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/_2012_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.554031 tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/_2014_11/__init__.py
--rw-r--r--   0        0        0     2991 2022-10-20 12:42:32.702056 tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/_2014_11/NetworkEngine.py
--rw-r--r--   0        0        0     1044 2022-10-20 12:42:32.119001 tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/_2014_11/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.926059 tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/_2019_12/__init__.py
--rw-r--r--   0        0        0      155 2022-10-20 12:42:32.725088 tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/_2019_12/NetworkEngine.py
--rw-r--r--   0        0        0     1189 2022-10-20 12:42:32.146004 tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/_2019_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.968069 tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/__init__.py
--rw-r--r--   0        0        0      639 2022-10-20 12:41:56.852402 tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.853059 tcsoa-0.9.0/tcsoa/gen/Reports/_2007_01/__init__.py
--rw-r--r--   0        0        0     6686 2022-10-20 12:42:59.877594 tcsoa-0.9.0/tcsoa/gen/Reports/_2007_01/CrfReports.py
--rw-r--r--   0        0        0     4089 2022-10-20 12:42:32.181015 tcsoa-0.9.0/tcsoa/gen/Reports/_2007_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.929066 tcsoa-0.9.0/tcsoa/gen/Reports/_2007_06/__init__.py
--rw-r--r--   0        0        0     1118 2022-10-20 12:42:59.914590 tcsoa-0.9.0/tcsoa/gen/Reports/_2007_06/CubeReports.py
--rw-r--r--   0        0        0     1138 2022-10-20 12:42:32.209019 tcsoa-0.9.0/tcsoa/gen/Reports/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.613030 tcsoa-0.9.0/tcsoa/gen/Reports/_2008_06/__init__.py
--rw-r--r--   0        0        0     1111 2022-10-20 12:42:59.944597 tcsoa-0.9.0/tcsoa/gen/Reports/_2008_06/CrfReports.py
--rw-r--r--   0        0        0     1004 2022-10-20 12:42:32.237012 tcsoa-0.9.0/tcsoa/gen/Reports/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.755045 tcsoa-0.9.0/tcsoa/gen/Reports/_2008_12/__init__.py
--rw-r--r--   0        0        0     3410 2022-10-20 12:42:59.987600 tcsoa-0.9.0/tcsoa/gen/Reports/_2008_12/CrfReports.py
--rw-r--r--   0        0        0     1676 2022-10-20 12:42:32.268016 tcsoa-0.9.0/tcsoa/gen/Reports/_2008_12/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.859054 tcsoa-0.9.0/tcsoa/gen/Reports/_2010_04/__init__.py
--rw-r--r--   0        0        0     2292 2022-10-20 12:43:00.018599 tcsoa-0.9.0/tcsoa/gen/Reports/_2010_04/CrfReports.py
--rw-r--r--   0        0        0     1728 2022-10-20 12:42:32.296018 tcsoa-0.9.0/tcsoa/gen/Reports/_2010_04/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.552030 tcsoa-0.9.0/tcsoa/gen/Reports/_2015_03/__init__.py
--rw-r--r--   0        0        0     8951 2022-10-20 12:43:00.082605 tcsoa-0.9.0/tcsoa/gen/Reports/_2015_03/CrfReports.py
--rw-r--r--   0        0        0     4876 2022-10-20 12:42:32.335022 tcsoa-0.9.0/tcsoa/gen/Reports/_2015_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.905061 tcsoa-0.9.0/tcsoa/gen/Reports/_2015_10/__init__.py
--rw-r--r--   0        0        0      605 2022-10-20 12:43:00.111610 tcsoa-0.9.0/tcsoa/gen/Reports/_2015_10/CrfReports.py
--rw-r--r--   0        0        0      794 2022-10-20 12:42:32.363033 tcsoa-0.9.0/tcsoa/gen/Reports/_2015_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.780047 tcsoa-0.9.0/tcsoa/gen/Reports/__init__.py
--rw-r--r--   0        0        0     1372 2022-10-20 12:41:56.877404 tcsoa-0.9.0/tcsoa/gen/Reports/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.647036 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2007_01/__init__.py
--rw-r--r--   0        0        0    18401 2022-10-20 12:43:00.262633 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2007_01/RequirementsManagement.py
--rw-r--r--   0        0        0     9494 2022-10-20 12:42:32.401027 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2007_01/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.560032 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2008_06/__init__.py
--rw-r--r--   0        0        0     1021 2022-10-20 12:43:00.288627 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2008_06/RequirementsManagement.py
--rw-r--r--   0        0        0     1666 2022-10-20 12:42:32.432030 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2008_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.912057 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2009_10/__init__.py
--rw-r--r--   0        0        0     6003 2022-10-20 12:43:00.351633 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2009_10/RequirementsManagement.py
--rw-r--r--   0        0        0     3459 2022-10-20 12:42:32.462035 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2009_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.735048 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2010_09/__init__.py
--rw-r--r--   0        0        0     1487 2022-10-20 12:43:00.381636 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2010_09/RequirementsManagement.py
--rw-r--r--   0        0        0     3614 2022-10-20 12:42:32.490041 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2010_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.661045 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2011_06/__init__.py
--rw-r--r--   0        0        0      746 2022-10-20 12:43:00.409649 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2011_06/RequirementsManagement.py
--rw-r--r--   0        0        0     2363 2022-10-20 12:42:32.520038 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2011_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.948069 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2012_09/__init__.py
--rw-r--r--   0        0        0      748 2022-10-20 12:43:00.433645 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2012_09/RequirementsManagement.py
--rw-r--r--   0        0        0     1083 2022-10-20 12:42:32.548051 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2012_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.966070 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/__init__.py
--rw-r--r--   0        0        0     1198 2022-10-20 12:41:56.899419 tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/services.py
--rw-r--r--   0        0        0     1442 2022-10-20 12:43:00.491652 tcsoa-0.9.0/tcsoa/gen/Server.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.600027 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2007_06/__init__.py
--rw-r--r--   0        0        0     8770 2022-10-20 12:43:00.596664 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2007_06/PublishByLink.py
--rw-r--r--   0        0        0    11093 2022-10-20 12:42:33.122092 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2007_06/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.705043 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_03/__init__.py
--rw-r--r--   0        0        0     1944 2022-10-20 12:43:00.638666 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_03/Composition.py
--rw-r--r--   0        0        0      777 2022-10-20 12:42:33.157111 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.923067 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_05/__init__.py
--rw-r--r--   0        0        0     4347 2022-10-20 12:42:33.197101 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_05/services.py
--rw-r--r--   0        0        0    15160 2022-10-20 12:43:00.765686 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_05/StructureSearch.py
--rw-r--r--   0        0        0     1587 2022-10-20 12:43:00.809686 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_05/StructureVerification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.698047 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_06/__init__.py
--rw-r--r--   0        0        0    11834 2022-10-20 12:42:33.230102 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_06/services.py
--rw-r--r--   0        0        0     6561 2022-10-20 12:43:00.887681 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_06/Structure.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.585031 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_12/__init__.py
--rw-r--r--   0        0        0      857 2022-10-20 12:42:33.260107 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_12/services.py
--rw-r--r--   0        0        0     1623 2022-10-20 12:43:00.926692 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_12/StructureVerification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.760046 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2010_04/__init__.py
--rw-r--r--   0        0        0      926 2022-10-20 12:42:33.287115 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2010_04/services.py
--rw-r--r--   0        0        0     3425 2022-10-20 12:43:00.966693 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2010_04/StructureSearch.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.582039 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2010_09/__init__.py
--rw-r--r--   0        0        0    20591 2022-10-20 12:42:33.339123 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2010_09/services.py
--rw-r--r--   0        0        0     4039 2022-10-20 12:43:01.020704 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2010_09/Structure.py
--rw-r--r--   0        0        0     4465 2022-10-20 12:43:01.060705 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2010_09/StructureSearch.py
--rw-r--r--   0        0        0    10615 2022-10-20 12:43:01.152707 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2010_09/StructureVerification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.846064 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2011_06/__init__.py
--rw-r--r--   0        0        0    18660 2022-10-20 12:42:33.375119 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2011_06/services.py
--rw-r--r--   0        0        0     6370 2022-10-20 12:43:01.236724 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2011_06/Structure.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.625030 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_02/__init__.py
--rw-r--r--   0        0        0      442 2022-10-20 12:43:01.264720 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_02/IncrementalChange.py
--rw-r--r--   0        0        0     9436 2022-10-20 12:42:33.435160 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_02/services.py
--rw-r--r--   0        0        0    30053 2022-10-20 12:43:01.479745 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_02/StructureVerification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.803054 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_09/__init__.py
--rw-r--r--   0        0        0     5174 2022-10-20 12:43:01.544748 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_09/MassUpdate.py
--rw-r--r--   0        0        0    11154 2022-10-20 12:42:33.496128 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_09/services.py
--rw-r--r--   0        0        0     2823 2022-10-20 12:43:01.589756 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_09/Structure.py
--rw-r--r--   0        0        0    12851 2022-10-20 12:43:01.690758 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_09/VariantManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.839051 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_10/__init__.py
--rw-r--r--   0        0        0     4994 2022-10-20 12:42:33.534141 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_10/services.py
--rw-r--r--   0        0        0      557 2022-10-20 12:43:01.718774 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_10/Structure.py
--rw-r--r--   0        0        0     3763 2022-10-20 12:43:01.773772 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_10/StructureVerification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.906076 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2013_05/__init__.py
--rw-r--r--   0        0        0      649 2022-10-20 12:43:01.803774 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2013_05/IncrementalChange.py
--rw-r--r--   0        0        0     9525 2022-10-20 12:42:33.582138 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2013_05/services.py
--rw-r--r--   0        0        0     5741 2022-10-20 12:43:01.866776 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2013_05/StructureVerification.py
--rw-r--r--   0        0        0    11258 2022-10-20 12:43:01.959784 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2013_05/VariantManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.914061 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_06/__init__.py
--rw-r--r--   0        0        0     7057 2022-10-20 12:42:33.616148 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_06/services.py
--rw-r--r--   0        0        0     2836 2022-10-20 12:43:01.997793 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_06/StructureFilterWithExpand.py
--rw-r--r--   0        0        0     2734 2022-10-20 12:43:02.037797 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_06/StructureVerification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.897060 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_10/__init__.py
--rw-r--r--   0        0        0    18834 2022-10-20 12:43:02.205812 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_10/MassUpdate.py
--rw-r--r--   0        0        0    33903 2022-10-20 12:42:33.679150 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_10/services.py
--rw-r--r--   0        0        0    15259 2022-10-20 12:43:02.292822 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_10/Structure.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.743042 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_12/__init__.py
--rw-r--r--   0        0        0     2337 2022-10-20 12:43:02.331832 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_12/Effectivity.py
--rw-r--r--   0        0        0     4563 2022-10-20 12:42:33.716155 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_12/services.py
--rw-r--r--   0        0        0    17099 2022-10-20 12:43:02.454827 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_12/StructureSearch.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.562032 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2015_10/__init__.py
--rw-r--r--   0        0        0     2088 2022-10-20 12:43:02.497834 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2015_10/Effectivity.py
--rw-r--r--   0        0        0     3962 2022-10-20 12:42:33.751168 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2015_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.569031 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2016_05/__init__.py
--rw-r--r--   0        0        0     2814 2022-10-20 12:42:33.782157 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2016_05/services.py
--rw-r--r--   0        0        0     1112 2022-10-20 12:43:02.524835 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2016_05/StructureVerification.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.736044 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2016_09/__init__.py
--rw-r--r--   0        0        0     1275 2022-10-20 12:43:02.556838 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2016_09/PublishByLink.py
--rw-r--r--   0        0        0     1025 2022-10-20 12:42:33.821188 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2016_09/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.844064 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2017_05/__init__.py
--rw-r--r--   0        0        0     3667 2022-10-20 12:42:33.855175 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2017_05/services.py
--rw-r--r--   0        0        0     5256 2022-10-20 12:43:02.603842 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2017_05/StructureSearch.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.937067 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2018_11/__init__.py
--rw-r--r--   0        0        0     2667 2022-10-20 12:42:33.882177 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2018_11/services.py
--rw-r--r--   0        0        0     1669 2022-10-20 12:43:02.631844 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2018_11/Structure.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.759045 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2019_06/__init__.py
--rw-r--r--   0        0        0     4414 2022-10-20 12:42:33.916175 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2019_06/services.py
--rw-r--r--   0        0        0     4718 2022-10-20 12:43:02.684857 tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2019_06/VariantManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.619029 tcsoa-0.9.0/tcsoa/gen/StructureManagement/__init__.py
--rw-r--r--   0        0        0     9234 2022-10-20 12:41:57.063425 tcsoa-0.9.0/tcsoa/gen/StructureManagement/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.597028 tcsoa-0.9.0/tcsoa/gen/Translation/_2007_06/__init__.py
--rw-r--r--   0        0        0     1222 2022-10-20 12:43:03.691970 tcsoa-0.9.0/tcsoa/gen/Translation/_2007_06/services.py
--rw-r--r--   0        0        0     1964 2022-10-20 12:43:02.716864 tcsoa-0.9.0/tcsoa/gen/Translation/_2007_06/TranslationManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.769044 tcsoa-0.9.0/tcsoa/gen/Translation/__init__.py
--rw-r--r--   0        0        0      238 2022-10-20 12:41:57.069426 tcsoa-0.9.0/tcsoa/gen/Translation/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.908058 tcsoa-0.9.0/tcsoa/gen/UiConfig/_2014_11/__init__.py
--rw-r--r--   0        0        0     3024 2022-10-20 12:43:03.724954 tcsoa-0.9.0/tcsoa/gen/UiConfig/_2014_11/services.py
--rw-r--r--   0        0        0    12053 2022-10-20 12:42:18.566742 tcsoa-0.9.0/tcsoa/gen/UiConfig/_2014_11/UiConfig.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.887056 tcsoa-0.9.0/tcsoa/gen/UiConfig/_2015_10/__init__.py
--rw-r--r--   0        0        0     1153 2022-10-20 12:43:03.754958 tcsoa-0.9.0/tcsoa/gen/UiConfig/_2015_10/services.py
--rw-r--r--   0        0        0     3555 2022-10-20 12:42:18.617753 tcsoa-0.9.0/tcsoa/gen/UiConfig/_2015_10/UiConfig.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.937067 tcsoa-0.9.0/tcsoa/gen/UiConfig/__init__.py
--rw-r--r--   0        0        0      339 2022-10-20 12:41:57.078427 tcsoa-0.9.0/tcsoa/gen/UiConfig/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.633041 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2007_06/__init__.py
--rw-r--r--   0        0        0     9039 2022-10-20 12:43:03.796954 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2007_06/services.py
--rw-r--r--   0        0        0     8816 2022-10-20 12:43:02.791866 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2007_06/VendorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.736044 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2008_06/__init__.py
--rw-r--r--   0        0        0     3100 2022-10-20 12:43:03.827963 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2008_06/services.py
--rw-r--r--   0        0        0     4496 2022-10-20 12:43:02.855876 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2008_06/VendorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.899057 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2012_02/__init__.py
--rw-r--r--   0        0        0     1620 2022-10-20 12:43:03.855960 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2012_02/services.py
--rw-r--r--   0        0        0     1562 2022-10-20 12:43:02.882875 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2012_02/VendorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.984066 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2012_09/__init__.py
--rw-r--r--   0        0        0     1405 2022-10-20 12:43:03.883967 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2012_09/services.py
--rw-r--r--   0        0        0      724 2022-10-20 12:43:02.908882 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2012_09/VendorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.544029 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2016_09/__init__.py
--rw-r--r--   0        0        0     1123 2022-10-20 12:43:03.911969 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2016_09/services.py
--rw-r--r--   0        0        0     1327 2022-10-20 12:43:02.935872 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2016_09/VendorManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.564032 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/__init__.py
--rw-r--r--   0        0        0     1187 2022-10-20 12:41:57.101429 tcsoa-0.9.0/tcsoa/gen/Vendormanagement/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.902061 tcsoa-0.9.0/tcsoa/gen/Visualization/_2011_02/__init__.py
--rw-r--r--   0        0        0     4962 2022-10-20 12:43:02.983884 tcsoa-0.9.0/tcsoa/gen/Visualization/_2011_02/DataManagement.py
--rw-r--r--   0        0        0    10675 2022-10-20 12:43:03.949974 tcsoa-0.9.0/tcsoa/gen/Visualization/_2011_02/services.py
--rw-r--r--   0        0        0     4574 2022-10-20 12:43:03.034892 tcsoa-0.9.0/tcsoa/gen/Visualization/_2011_02/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.557031 tcsoa-0.9.0/tcsoa/gen/Visualization/_2013_05/__init__.py
--rw-r--r--   0        0        0     5332 2022-10-20 12:43:03.072886 tcsoa-0.9.0/tcsoa/gen/Visualization/_2013_05/DataManagement.py
--rw-r--r--   0        0        0     8159 2022-10-20 12:43:03.987972 tcsoa-0.9.0/tcsoa/gen/Visualization/_2013_05/services.py
--rw-r--r--   0        0        0      246 2022-10-20 12:43:03.095894 tcsoa-0.9.0/tcsoa/gen/Visualization/_2013_05/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.872054 tcsoa-0.9.0/tcsoa/gen/Visualization/_2013_12/__init__.py
--rw-r--r--   0        0        0     4280 2022-10-20 12:43:04.014975 tcsoa-0.9.0/tcsoa/gen/Visualization/_2013_12/services.py
--rw-r--r--   0        0        0     1614 2022-10-20 12:43:03.122899 tcsoa-0.9.0/tcsoa/gen/Visualization/_2013_12/StructureManagement.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.851061 tcsoa-0.9.0/tcsoa/gen/Visualization/_2016_03/__init__.py
--rw-r--r--   0        0        0     4340 2022-10-20 12:43:03.170906 tcsoa-0.9.0/tcsoa/gen/Visualization/_2016_03/DataManagement.py
--rw-r--r--   0        0        0     3758 2022-10-20 12:43:04.043987 tcsoa-0.9.0/tcsoa/gen/Visualization/_2016_03/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.932066 tcsoa-0.9.0/tcsoa/gen/Visualization/__init__.py
--rw-r--r--   0        0        0     1035 2022-10-20 12:41:57.116431 tcsoa-0.9.0/tcsoa/gen/Visualization/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.671045 tcsoa-0.9.0/tcsoa/gen/Workflow/_2007_06/__init__.py
--rw-r--r--   0        0        0     1104 2022-10-20 12:43:04.234991 tcsoa-0.9.0/tcsoa/gen/Workflow/_2007_06/services.py
--rw-r--r--   0        0        0     1367 2022-10-20 12:43:03.212904 tcsoa-0.9.0/tcsoa/gen/Workflow/_2007_06/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.781046 tcsoa-0.9.0/tcsoa/gen/Workflow/_2008_06/__init__.py
--rw-r--r--   0        0        0    11268 2022-10-20 12:43:04.290019 tcsoa-0.9.0/tcsoa/gen/Workflow/_2008_06/services.py
--rw-r--r--   0        0        0    13763 2022-10-20 12:43:03.355919 tcsoa-0.9.0/tcsoa/gen/Workflow/_2008_06/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.978069 tcsoa-0.9.0/tcsoa/gen/Workflow/_2010_09/__init__.py
--rw-r--r--   0        0        0     1573 2022-10-20 12:43:04.324003 tcsoa-0.9.0/tcsoa/gen/Workflow/_2010_09/services.py
--rw-r--r--   0        0        0     1411 2022-10-20 12:43:03.391921 tcsoa-0.9.0/tcsoa/gen/Workflow/_2010_09/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.886054 tcsoa-0.9.0/tcsoa/gen/Workflow/_2012_10/__init__.py
--rw-r--r--   0        0        0     1480 2022-10-20 12:43:04.353013 tcsoa-0.9.0/tcsoa/gen/Workflow/_2012_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.752043 tcsoa-0.9.0/tcsoa/gen/Workflow/_2013_05/__init__.py
--rw-r--r--   0        0        0     1207 2022-10-20 12:43:04.381013 tcsoa-0.9.0/tcsoa/gen/Workflow/_2013_05/services.py
--rw-r--r--   0        0        0     2043 2022-10-20 12:43:03.431918 tcsoa-0.9.0/tcsoa/gen/Workflow/_2013_05/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.680038 tcsoa-0.9.0/tcsoa/gen/Workflow/_2014_06/__init__.py
--rw-r--r--   0        0        0     9003 2022-10-20 12:43:04.417018 tcsoa-0.9.0/tcsoa/gen/Workflow/_2014_06/services.py
--rw-r--r--   0        0        0     6139 2022-10-20 12:43:03.478922 tcsoa-0.9.0/tcsoa/gen/Workflow/_2014_06/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.962068 tcsoa-0.9.0/tcsoa/gen/Workflow/_2014_10/__init__.py
--rw-r--r--   0        0        0     3249 2022-10-20 12:43:04.447023 tcsoa-0.9.0/tcsoa/gen/Workflow/_2014_10/services.py
--rw-r--r--   0        0        0     4330 2022-10-20 12:43:03.519928 tcsoa-0.9.0/tcsoa/gen/Workflow/_2014_10/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.723044 tcsoa-0.9.0/tcsoa/gen/Workflow/_2015_07/__init__.py
--rw-r--r--   0        0        0     2981 2022-10-20 12:43:04.475030 tcsoa-0.9.0/tcsoa/gen/Workflow/_2015_07/services.py
--rw-r--r--   0        0        0     3719 2022-10-20 12:43:03.552938 tcsoa-0.9.0/tcsoa/gen/Workflow/_2015_07/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.867053 tcsoa-0.9.0/tcsoa/gen/Workflow/_2019_06/__init__.py
--rw-r--r--   0        0        0     5111 2022-10-20 12:43:04.507020 tcsoa-0.9.0/tcsoa/gen/Workflow/_2019_06/services.py
--rw-r--r--   0        0        0    10534 2022-10-20 12:43:03.626938 tcsoa-0.9.0/tcsoa/gen/Workflow/_2019_06/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:05.003067 tcsoa-0.9.0/tcsoa/gen/Workflow/_2020_01/__init__.py
--rw-r--r--   0        0        0     2073 2022-10-20 12:43:04.537030 tcsoa-0.9.0/tcsoa/gen/Workflow/_2020_01/services.py
--rw-r--r--   0        0        0     2264 2022-10-20 12:43:03.662952 tcsoa-0.9.0/tcsoa/gen/Workflow/_2020_01/Workflow.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.685041 tcsoa-0.9.0/tcsoa/gen/Workflow/__init__.py
--rw-r--r--   0        0        0     2399 2022-10-20 12:41:57.180431 tcsoa-0.9.0/tcsoa/gen/Workflow/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.953082 tcsoa-0.9.0/tcsoa/gen/WProxy/_2014_10/__init__.py
--rw-r--r--   0        0        0     1462 2022-10-20 12:42:18.650746 tcsoa-0.9.0/tcsoa/gen/WProxy/_2014_10/ProxyLink.py
--rw-r--r--   0        0        0     1126 2022-10-20 12:43:04.205997 tcsoa-0.9.0/tcsoa/gen/WProxy/_2014_10/services.py
--rw-r--r--   0        0        0        0 2022-10-20 12:43:04.805070 tcsoa-0.9.0/tcsoa/gen/WProxy/__init__.py
--rw-r--r--   0        0        0      191 2022-10-20 12:41:57.123434 tcsoa-0.9.0/tcsoa/gen/WProxy/services.py
--rw-r--r--   0        0        0     1386 2022-11-21 10:08:01.795581 tcsoa-0.9.0/tcsoa/itk_constants.py
--rw-r--r--   0        0        0    36468 1970-01-01 00:00:00.000000 tcsoa-0.9.0/setup.py
--rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 tcsoa-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2022-09-26 11:08:11.334023 tcsoa-0.9.1/LICENSE.txt
+-rw-r--r--   0        0        0      557 2022-12-12 13:23:39.255465 tcsoa-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-06-09 12:29:08.307759 tcsoa-0.9.1/tcsoa/__init__.py
+-rw-r--r--   0        0        0     8300 2022-12-06 16:00:02.842630 tcsoa-0.9.1/tcsoa/backend.py
+-rw-r--r--   0        0        0     2059 2022-12-05 08:51:33.454395 tcsoa-0.9.1/tcsoa/base.py
+-rw-r--r--   0        0        0     8790 2022-12-06 15:00:47.897479 tcsoa-0.9.1/tcsoa/basics.py
+-rw-r--r--   0        0        0     1027 2022-12-05 10:07:21.656126 tcsoa-0.9.1/tcsoa/config.py
+-rw-r--r--   0        0        0      546 2022-12-06 15:56:36.649956 tcsoa-0.9.1/tcsoa/exceptions.py
+-rw-r--r--   0        0        0        0 2022-07-19 08:50:08.936027 tcsoa-0.9.1/tcsoa/fcc/__init__.py
+-rw-r--r--   0        0        0     4718 2022-10-18 14:08:47.281729 tcsoa-0.9.1/tcsoa/fcc/fcc_client_proxy.py
+-rw-r--r--   0        0        0     2916 2022-10-18 14:11:34.201245 tcsoa-0.9.1/tcsoa/fcc/fcc_wrapper.py
+-rw-r--r--   0        0        0     5989 2022-12-12 13:22:24.620737 tcsoa-0.9.1/tcsoa/fcc/file_management_utility.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.782046 tcsoa-0.9.1/tcsoa/gen/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.868058 tcsoa-0.9.1/tcsoa/gen/ActiveCollaboration/_2020_12/__init__.py
+-rw-r--r--   0        0        0     3470 2022-10-20 12:41:57.327454 tcsoa-0.9.1/tcsoa/gen/ActiveCollaboration/_2020_12/ActiveCollaboration.py
+-rw-r--r--   0        0        0     8878 2022-10-20 12:41:57.371476 tcsoa-0.9.1/tcsoa/gen/ActiveCollaboration/_2020_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.870055 tcsoa-0.9.1/tcsoa/gen/ActiveCollaboration/__init__.py
+-rw-r--r--   0        0        0      480 2022-10-20 12:41:53.739062 tcsoa-0.9.1/tcsoa/gen/ActiveCollaboration/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.955069 tcsoa-0.9.1/tcsoa/gen/ActiveWorkspaceBom/_2015_10/__init__.py
+-rw-r--r--   0        0        0     3406 2022-10-20 12:41:58.832622 tcsoa-0.9.1/tcsoa/gen/ActiveWorkspaceBom/_2015_10/OccurrenceManagementCad.py
+-rw-r--r--   0        0        0     4444 2022-10-20 12:41:57.403455 tcsoa-0.9.1/tcsoa/gen/ActiveWorkspaceBom/_2015_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.991073 tcsoa-0.9.1/tcsoa/gen/ActiveWorkspaceBom/__init__.py
+-rw-r--r--   0        0        0      329 2022-10-20 12:41:53.746070 tcsoa-0.9.1/tcsoa/gen/ActiveWorkspaceBom/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.896060 tcsoa-0.9.1/tcsoa/gen/ActiveWorkspaceVis/_2015_03/__init__.py
+-rw-r--r--   0        0        0    10014 2022-10-20 12:42:03.940164 tcsoa-0.9.1/tcsoa/gen/ActiveWorkspaceVis/_2015_03/DataManagement.py
+-rw-r--r--   0        0        0     4677 2022-10-20 12:41:57.432462 tcsoa-0.9.1/tcsoa/gen/ActiveWorkspaceVis/_2015_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.587032 tcsoa-0.9.1/tcsoa/gen/ActiveWorkspaceVis/__init__.py
+-rw-r--r--   0        0        0      215 2022-10-20 12:41:53.752069 tcsoa-0.9.1/tcsoa/gen/ActiveWorkspaceVis/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.831050 tcsoa-0.9.1/tcsoa/gen/Administration/_2006_03/__init__.py
+-rw-r--r--   0        0        0     7246 2022-10-20 12:42:33.996207 tcsoa-0.9.1/tcsoa/gen/Administration/_2006_03/IRM.py
+-rw-r--r--   0        0        0     8803 2022-10-20 12:41:57.470471 tcsoa-0.9.1/tcsoa/gen/Administration/_2006_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.702046 tcsoa-0.9.1/tcsoa/gen/Administration/_2007_01/__init__.py
+-rw-r--r--   0        0        0     1051 2022-10-20 12:41:57.497471 tcsoa-0.9.1/tcsoa/gen/Administration/_2007_01/services.py
+-rw-r--r--   0        0        0     3316 2022-10-20 12:42:34.049187 tcsoa-0.9.1/tcsoa/gen/Administration/_2007_01/UserManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.666046 tcsoa-0.9.1/tcsoa/gen/Administration/_2007_06/__init__.py
+-rw-r--r--   0        0        0     2093 2022-10-20 12:42:34.087185 tcsoa-0.9.1/tcsoa/gen/Administration/_2007_06/Authorization.py
+-rw-r--r--   0        0        0     3078 2022-10-20 12:42:34.135189 tcsoa-0.9.1/tcsoa/gen/Administration/_2007_06/PreferenceManagement.py
+-rw-r--r--   0        0        0     3683 2022-10-20 12:41:57.534471 tcsoa-0.9.1/tcsoa/gen/Administration/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.778055 tcsoa-0.9.1/tcsoa/gen/Administration/_2008_03/__init__.py
+-rw-r--r--   0        0        0     2026 2022-10-20 12:42:34.180200 tcsoa-0.9.1/tcsoa/gen/Administration/_2008_03/IRM.py
+-rw-r--r--   0        0        0     2096 2022-10-20 12:41:57.563475 tcsoa-0.9.1/tcsoa/gen/Administration/_2008_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.803054 tcsoa-0.9.1/tcsoa/gen/Administration/_2008_06/__init__.py
+-rw-r--r--   0        0        0     1705 2022-10-20 12:41:57.594490 tcsoa-0.9.1/tcsoa/gen/Administration/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.851061 tcsoa-0.9.1/tcsoa/gen/Administration/_2008_12/__init__.py
+-rw-r--r--   0        0        0     2568 2022-10-20 12:41:57.626488 tcsoa-0.9.1/tcsoa/gen/Administration/_2008_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.931067 tcsoa-0.9.1/tcsoa/gen/Administration/_2010_04/__init__.py
+-rw-r--r--   0        0        0      649 2022-10-20 12:42:34.207200 tcsoa-0.9.1/tcsoa/gen/Administration/_2010_04/DisciplineManagement.py
+-rw-r--r--   0        0        0     7659 2022-10-20 12:42:34.276209 tcsoa-0.9.1/tcsoa/gen/Administration/_2010_04/IRM.py
+-rw-r--r--   0        0        0     7891 2022-10-20 12:41:57.668490 tcsoa-0.9.1/tcsoa/gen/Administration/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.999090 tcsoa-0.9.1/tcsoa/gen/Administration/_2011_05/__init__.py
+-rw-r--r--   0        0        0     1001 2022-10-20 12:41:57.697494 tcsoa-0.9.1/tcsoa/gen/Administration/_2011_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.714041 tcsoa-0.9.1/tcsoa/gen/Administration/_2012_09/__init__.py
+-rw-r--r--   0        0        0    11218 2022-10-20 12:42:34.372213 tcsoa-0.9.1/tcsoa/gen/Administration/_2012_09/PreferenceManagement.py
+-rw-r--r--   0        0        0    17945 2022-10-20 12:41:57.758500 tcsoa-0.9.1/tcsoa/gen/Administration/_2012_09/services.py
+-rw-r--r--   0        0        0     3547 2022-10-20 12:42:34.433219 tcsoa-0.9.1/tcsoa/gen/Administration/_2012_09/UserManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.556030 tcsoa-0.9.1/tcsoa/gen/Administration/_2012_10/__init__.py
+-rw-r--r--   0        0        0     1464 2022-10-20 12:42:34.467229 tcsoa-0.9.1/tcsoa/gen/Administration/_2012_10/IRM.py
+-rw-r--r--   0        0        0     2543 2022-10-20 12:41:57.795514 tcsoa-0.9.1/tcsoa/gen/Administration/_2012_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.659037 tcsoa-0.9.1/tcsoa/gen/Administration/_2014_10/__init__.py
+-rw-r--r--   0        0        0     1099 2022-10-20 12:41:57.828507 tcsoa-0.9.1/tcsoa/gen/Administration/_2014_10/services.py
+-rw-r--r--   0        0        0     1085 2022-10-20 12:42:34.495229 tcsoa-0.9.1/tcsoa/gen/Administration/_2014_10/UserManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.820055 tcsoa-0.9.1/tcsoa/gen/Administration/_2015_03/__init__.py
+-rw-r--r--   0        0        0     1301 2022-10-20 12:41:57.860504 tcsoa-0.9.1/tcsoa/gen/Administration/_2015_03/services.py
+-rw-r--r--   0        0        0     1474 2022-10-20 12:42:34.528233 tcsoa-0.9.1/tcsoa/gen/Administration/_2015_03/UserManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.798053 tcsoa-0.9.1/tcsoa/gen/Administration/_2015_07/__init__.py
+-rw-r--r--   0        0        0     1750 2022-10-20 12:41:57.892509 tcsoa-0.9.1/tcsoa/gen/Administration/_2015_07/services.py
+-rw-r--r--   0        0        0     3109 2022-10-20 12:42:34.566256 tcsoa-0.9.1/tcsoa/gen/Administration/_2015_07/UserManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.893059 tcsoa-0.9.1/tcsoa/gen/Administration/_2016_03/__init__.py
+-rw-r--r--   0        0        0     1108 2022-10-20 12:41:57.922518 tcsoa-0.9.1/tcsoa/gen/Administration/_2016_03/services.py
+-rw-r--r--   0        0        0     1131 2022-10-20 12:42:34.592243 tcsoa-0.9.1/tcsoa/gen/Administration/_2016_03/UserManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.605029 tcsoa-0.9.1/tcsoa/gen/Administration/_2016_10/__init__.py
+-rw-r--r--   0        0        0     1912 2022-10-20 12:41:57.954521 tcsoa-0.9.1/tcsoa/gen/Administration/_2016_10/services.py
+-rw-r--r--   0        0        0     1411 2022-10-20 12:42:34.619240 tcsoa-0.9.1/tcsoa/gen/Administration/_2016_10/UserManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.845062 tcsoa-0.9.1/tcsoa/gen/Administration/_2017_05/__init__.py
+-rw-r--r--   0        0        0     2466 2022-10-20 12:42:34.652250 tcsoa-0.9.1/tcsoa/gen/Administration/_2017_05/GroupManagement.py
+-rw-r--r--   0        0        0     1474 2022-10-20 12:42:34.690242 tcsoa-0.9.1/tcsoa/gen/Administration/_2017_05/RoleManagement.py
+-rw-r--r--   0        0        0     4086 2022-10-20 12:41:57.999519 tcsoa-0.9.1/tcsoa/gen/Administration/_2017_05/services.py
+-rw-r--r--   0        0        0     3489 2022-10-20 12:42:34.742250 tcsoa-0.9.1/tcsoa/gen/Administration/_2017_05/UserManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.670045 tcsoa-0.9.1/tcsoa/gen/Administration/_2018_11/__init__.py
+-rw-r--r--   0        0        0     1793 2022-10-20 12:42:34.776251 tcsoa-0.9.1/tcsoa/gen/Administration/_2018_11/IRM.py
+-rw-r--r--   0        0        0      519 2022-10-20 12:42:34.802251 tcsoa-0.9.1/tcsoa/gen/Administration/_2018_11/OrganizationManagement.py
+-rw-r--r--   0        0        0     5057 2022-10-20 12:41:58.038528 tcsoa-0.9.1/tcsoa/gen/Administration/_2018_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.873056 tcsoa-0.9.1/tcsoa/gen/Administration/__init__.py
+-rw-r--r--   0        0        0     5002 2022-10-20 12:41:53.827071 tcsoa-0.9.1/tcsoa/gen/Administration/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.631037 tcsoa-0.9.1/tcsoa/gen/Ai/_2006_03/__init__.py
+-rw-r--r--   0        0        0    10627 2022-10-20 12:42:34.986274 tcsoa-0.9.1/tcsoa/gen/Ai/_2006_03/Ai.py
+-rw-r--r--   0        0        0    17303 2022-10-20 12:41:58.115532 tcsoa-0.9.1/tcsoa/gen/Ai/_2006_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.941066 tcsoa-0.9.1/tcsoa/gen/Ai/_2007_12/__init__.py
+-rw-r--r--   0        0        0     2291 2022-10-20 12:42:35.030283 tcsoa-0.9.1/tcsoa/gen/Ai/_2007_12/Ai.py
+-rw-r--r--   0        0        0     4161 2022-10-20 12:41:58.145541 tcsoa-0.9.1/tcsoa/gen/Ai/_2007_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.603029 tcsoa-0.9.1/tcsoa/gen/Ai/_2008_05/__init__.py
+-rw-r--r--   0        0        0      500 2022-10-20 12:42:35.058284 tcsoa-0.9.1/tcsoa/gen/Ai/_2008_05/Ai.py
+-rw-r--r--   0        0        0     1434 2022-10-20 12:41:58.171544 tcsoa-0.9.1/tcsoa/gen/Ai/_2008_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.992071 tcsoa-0.9.1/tcsoa/gen/Ai/_2008_06/__init__.py
+-rw-r--r--   0        0        0     4199 2022-10-20 12:42:35.117281 tcsoa-0.9.1/tcsoa/gen/Ai/_2008_06/Ai.py
+-rw-r--r--   0        0        0     5256 2022-10-20 12:41:58.204551 tcsoa-0.9.1/tcsoa/gen/Ai/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.733049 tcsoa-0.9.1/tcsoa/gen/Ai/_2009_06/__init__.py
+-rw-r--r--   0        0        0     1052 2022-10-20 12:42:35.145301 tcsoa-0.9.1/tcsoa/gen/Ai/_2009_06/Ai.py
+-rw-r--r--   0        0        0     2983 2022-10-20 12:41:58.234551 tcsoa-0.9.1/tcsoa/gen/Ai/_2009_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.854061 tcsoa-0.9.1/tcsoa/gen/Ai/_2009_10/__init__.py
+-rw-r--r--   0        0        0     3740 2022-10-20 12:42:35.197300 tcsoa-0.9.1/tcsoa/gen/Ai/_2009_10/Ai.py
+-rw-r--r--   0        0        0      746 2022-10-20 12:41:58.266552 tcsoa-0.9.1/tcsoa/gen/Ai/_2009_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.917065 tcsoa-0.9.1/tcsoa/gen/Ai/_2010_09/__init__.py
+-rw-r--r--   0        0        0     1025 2022-10-20 12:42:35.226292 tcsoa-0.9.1/tcsoa/gen/Ai/_2010_09/Ai.py
+-rw-r--r--   0        0        0     1501 2022-10-20 12:41:58.294555 tcsoa-0.9.1/tcsoa/gen/Ai/_2010_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.600027 tcsoa-0.9.1/tcsoa/gen/Ai/_2012_09/__init__.py
+-rw-r--r--   0        0        0     7312 2022-10-20 12:42:35.292300 tcsoa-0.9.1/tcsoa/gen/Ai/_2012_09/Ai.py
+-rw-r--r--   0        0        0     3299 2022-10-20 12:41:58.335560 tcsoa-0.9.1/tcsoa/gen/Ai/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.884063 tcsoa-0.9.1/tcsoa/gen/Ai/_2013_05/__init__.py
+-rw-r--r--   0        0        0     1121 2022-10-20 12:42:35.321306 tcsoa-0.9.1/tcsoa/gen/Ai/_2013_05/Ai.py
+-rw-r--r--   0        0        0     1078 2022-10-20 12:41:58.366562 tcsoa-0.9.1/tcsoa/gen/Ai/_2013_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.701045 tcsoa-0.9.1/tcsoa/gen/Ai/_2013_12/__init__.py
+-rw-r--r--   0        0        0     1298 2022-10-20 12:42:35.349307 tcsoa-0.9.1/tcsoa/gen/Ai/_2013_12/Ai.py
+-rw-r--r--   0        0        0     1306 2022-10-20 12:41:58.394562 tcsoa-0.9.1/tcsoa/gen/Ai/_2013_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.740043 tcsoa-0.9.1/tcsoa/gen/Ai/_2014_12/__init__.py
+-rw-r--r--   0        0        0     4277 2022-10-20 12:42:35.400317 tcsoa-0.9.1/tcsoa/gen/Ai/_2014_12/Ai.py
+-rw-r--r--   0        0        0     2972 2022-10-20 12:41:58.424566 tcsoa-0.9.1/tcsoa/gen/Ai/_2014_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.790046 tcsoa-0.9.1/tcsoa/gen/Ai/_2018_06/__init__.py
+-rw-r--r--   0        0        0     3465 2022-10-20 12:42:35.445324 tcsoa-0.9.1/tcsoa/gen/Ai/_2018_06/Ai.py
+-rw-r--r--   0        0        0     1073 2022-10-20 12:41:58.454575 tcsoa-0.9.1/tcsoa/gen/Ai/_2018_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.684038 tcsoa-0.9.1/tcsoa/gen/Ai/__init__.py
+-rw-r--r--   0        0        0     3283 2022-10-20 12:41:53.900085 tcsoa-0.9.1/tcsoa/gen/Ai/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.856060 tcsoa-0.9.1/tcsoa/gen/Allocations/_2007_01/__init__.py
+-rw-r--r--   0        0        0     5381 2022-10-20 12:42:35.505318 tcsoa-0.9.1/tcsoa/gen/Allocations/_2007_01/Allocation.py
+-rw-r--r--   0        0        0    19838 2022-10-20 12:41:58.507580 tcsoa-0.9.1/tcsoa/gen/Allocations/_2007_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.924063 tcsoa-0.9.1/tcsoa/gen/Allocations/_2011_06/__init__.py
+-rw-r--r--   0        0        0     1967 2022-10-20 12:42:35.536322 tcsoa-0.9.1/tcsoa/gen/Allocations/_2011_06/Allocation.py
+-rw-r--r--   0        0        0     1694 2022-10-20 12:41:58.538580 tcsoa-0.9.1/tcsoa/gen/Allocations/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.970063 tcsoa-0.9.1/tcsoa/gen/Allocations/__init__.py
+-rw-r--r--   0        0        0      999 2022-10-20 12:41:53.927088 tcsoa-0.9.1/tcsoa/gen/Allocations/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.813096 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2007_06/__init__.py
+-rw-r--r--   0        0        0     4577 2022-10-20 12:42:35.590329 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2007_06/LicenseManagement.py
+-rw-r--r--   0        0        0    10092 2022-10-20 12:41:58.640590 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.791043 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2009_10/__init__.py
+-rw-r--r--   0        0        0     4286 2022-10-20 12:42:35.627329 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2009_10/LicenseManagement.py
+-rw-r--r--   0        0        0     6740 2022-10-20 12:41:58.672600 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2009_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.958058 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2012_09/__init__.py
+-rw-r--r--   0        0        0     4009 2022-10-20 12:42:35.660338 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2012_09/LicenseManagement.py
+-rw-r--r--   0        0        0     2984 2022-10-20 12:41:58.702601 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.630037 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2013_05/__init__.py
+-rw-r--r--   0        0        0     4319 2022-10-20 12:42:35.694333 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2013_05/LicenseManagement.py
+-rw-r--r--   0        0        0     2974 2022-10-20 12:41:58.732621 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2013_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.765045 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2017_05/__init__.py
+-rw-r--r--   0        0        0     3408 2022-10-20 12:42:35.730339 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2017_05/LicenseManagement.py
+-rw-r--r--   0        0        0     2141 2022-10-20 12:41:58.761600 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2017_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.961068 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2018_06/__init__.py
+-rw-r--r--   0        0        0     4145 2022-10-20 12:42:35.761347 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2018_06/LicenseManagement.py
+-rw-r--r--   0        0        0     1716 2022-10-20 12:41:58.789632 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2018_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.749045 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/__init__.py
+-rw-r--r--   0        0        0     1412 2022-10-20 12:41:53.954089 tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.804052 tcsoa-0.9.1/tcsoa/gen/AWS2/_2016_12/__init__.py
+-rw-r--r--   0        0        0     1114 2022-10-20 12:41:57.223444 tcsoa-0.9.1/tcsoa/gen/AWS2/_2016_12/services.py
+-rw-r--r--   0        0        0     8797 2022-10-20 12:42:00.480794 tcsoa-0.9.1/tcsoa/gen/AWS2/_2016_12/UiConfig.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.935069 tcsoa-0.9.1/tcsoa/gen/AWS2/_2017_06/__init__.py
+-rw-r--r--   0        0        0     1022 2022-10-20 12:41:57.254438 tcsoa-0.9.1/tcsoa/gen/AWS2/_2017_06/services.py
+-rw-r--r--   0        0        0     9755 2022-10-20 12:42:00.548795 tcsoa-0.9.1/tcsoa/gen/AWS2/_2017_06/UiConfig.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.608029 tcsoa-0.9.1/tcsoa/gen/AWS2/_2018_12/__init__.py
+-rw-r--r--   0        0        0     4807 2022-10-20 12:42:00.595806 tcsoa-0.9.1/tcsoa/gen/AWS2/_2018_12/RequirementsManagement.py
+-rw-r--r--   0        0        0     1644 2022-10-20 12:41:57.286453 tcsoa-0.9.1/tcsoa/gen/AWS2/_2018_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.862059 tcsoa-0.9.1/tcsoa/gen/AWS2/__init__.py
+-rw-r--r--   0        0        0      476 2022-10-20 12:41:53.726067 tcsoa-0.9.1/tcsoa/gen/AWS2/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.551030 tcsoa-0.9.1/tcsoa/gen/Bom/_2008_06/__init__.py
+-rw-r--r--   0        0        0     3694 2022-10-20 12:42:04.185196 tcsoa-0.9.1/tcsoa/gen/Bom/_2008_06/services.py
+-rw-r--r--   0        0        0     7236 2022-10-20 12:42:35.830354 tcsoa-0.9.1/tcsoa/gen/Bom/_2008_06/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.563036 tcsoa-0.9.1/tcsoa/gen/Bom/_2010_09/__init__.py
+-rw-r--r--   0        0        0     1396 2022-10-20 12:42:04.222201 tcsoa-0.9.1/tcsoa/gen/Bom/_2010_09/services.py
+-rw-r--r--   0        0        0     2282 2022-10-20 12:42:35.873352 tcsoa-0.9.1/tcsoa/gen/Bom/_2010_09/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.581034 tcsoa-0.9.1/tcsoa/gen/Bom/__init__.py
+-rw-r--r--   0        0        0      562 2022-10-20 12:41:53.966094 tcsoa-0.9.1/tcsoa/gen/Bom/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.818055 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2007_06/__init__.py
+-rw-r--r--   0        0        0     3474 2022-10-20 12:42:35.934362 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2007_06/Constants.py
+-rw-r--r--   0        0        0     1944 2022-10-20 12:42:35.972366 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2007_06/RulesBasedFramework.py
+-rw-r--r--   0        0        0     3221 2022-10-20 12:42:04.268197 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.870055 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2008_06/__init__.py
+-rw-r--r--   0        0        0     1560 2022-10-20 12:42:36.008372 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2008_06/ConditionEngine.py
+-rw-r--r--   0        0        0     3161 2022-10-20 12:42:36.051381 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2008_06/DeepCopyRules.py
+-rw-r--r--   0        0        0     2333 2022-10-20 12:42:04.305197 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.833056 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2010_04/__init__.py
+-rw-r--r--   0        0        0     1927 2022-10-20 12:42:36.091379 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2010_04/BusinessRules.py
+-rw-r--r--   0        0        0     3054 2022-10-20 12:42:04.335199 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.705043 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2011_06/__init__.py
+-rw-r--r--   0        0        0     1000 2022-10-20 12:42:36.124374 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2011_06/Constants.py
+-rw-r--r--   0        0        0     1164 2022-10-20 12:42:04.370204 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.806049 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/__init__.py
+-rw-r--r--   0        0        0     1208 2022-10-20 12:41:53.983094 tcsoa-0.9.1/tcsoa/gen/BusinessModeler/services.py
+-rw-r--r--   0        0        0   196281 2022-10-20 12:42:12.128041 tcsoa-0.9.1/tcsoa/gen/BusinessObjects.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.916066 tcsoa-0.9.1/tcsoa/gen/Cad/_2007_01/__init__.py
+-rw-r--r--   0        0        0    29654 2022-10-20 12:42:36.393400 tcsoa-0.9.1/tcsoa/gen/Cad/_2007_01/DataManagement.py
+-rw-r--r--   0        0        0    24920 2022-10-20 12:42:12.207055 tcsoa-0.9.1/tcsoa/gen/Cad/_2007_01/services.py
+-rw-r--r--   0        0        0    25378 2022-10-20 12:42:36.640422 tcsoa-0.9.1/tcsoa/gen/Cad/_2007_01/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.955069 tcsoa-0.9.1/tcsoa/gen/Cad/_2007_06/__init__.py
+-rw-r--r--   0        0        0     4457 2022-10-20 12:42:12.244053 tcsoa-0.9.1/tcsoa/gen/Cad/_2007_06/services.py
+-rw-r--r--   0        0        0     6031 2022-10-20 12:42:36.732443 tcsoa-0.9.1/tcsoa/gen/Cad/_2007_06/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.591030 tcsoa-0.9.1/tcsoa/gen/Cad/_2007_09/__init__.py
+-rw-r--r--   0        0        0     1116 2022-10-20 12:42:12.274056 tcsoa-0.9.1/tcsoa/gen/Cad/_2007_09/services.py
+-rw-r--r--   0        0        0     2375 2022-10-20 12:42:36.784445 tcsoa-0.9.1/tcsoa/gen/Cad/_2007_09/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.844064 tcsoa-0.9.1/tcsoa/gen/Cad/_2007_12/__init__.py
+-rw-r--r--   0        0        0     4744 2022-10-20 12:42:36.829449 tcsoa-0.9.1/tcsoa/gen/Cad/_2007_12/DataManagement.py
+-rw-r--r--   0        0        0    12455 2022-10-20 12:42:12.326082 tcsoa-0.9.1/tcsoa/gen/Cad/_2007_12/services.py
+-rw-r--r--   0        0        0     8702 2022-10-20 12:42:36.921448 tcsoa-0.9.1/tcsoa/gen/Cad/_2007_12/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.599028 tcsoa-0.9.1/tcsoa/gen/Cad/_2008_03/__init__.py
+-rw-r--r--   0        0        0     7489 2022-10-20 12:42:36.981461 tcsoa-0.9.1/tcsoa/gen/Cad/_2008_03/DataManagement.py
+-rw-r--r--   0        0        0     5350 2022-10-20 12:42:12.367076 tcsoa-0.9.1/tcsoa/gen/Cad/_2008_03/services.py
+-rw-r--r--   0        0        0     2066 2022-10-20 12:42:37.021459 tcsoa-0.9.1/tcsoa/gen/Cad/_2008_03/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.687039 tcsoa-0.9.1/tcsoa/gen/Cad/_2008_06/__init__.py
+-rw-r--r--   0        0        0    15078 2022-10-20 12:42:37.137488 tcsoa-0.9.1/tcsoa/gen/Cad/_2008_06/DataManagement.py
+-rw-r--r--   0        0        0    23532 2022-10-20 12:42:12.430079 tcsoa-0.9.1/tcsoa/gen/Cad/_2008_06/services.py
+-rw-r--r--   0        0        0    41331 2022-10-20 12:42:37.446498 tcsoa-0.9.1/tcsoa/gen/Cad/_2008_06/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.553037 tcsoa-0.9.1/tcsoa/gen/Cad/_2009_04/__init__.py
+-rw-r--r--   0        0        0     3427 2022-10-20 12:42:12.463082 tcsoa-0.9.1/tcsoa/gen/Cad/_2009_04/services.py
+-rw-r--r--   0        0        0     7612 2022-10-20 12:42:37.504502 tcsoa-0.9.1/tcsoa/gen/Cad/_2009_04/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.943068 tcsoa-0.9.1/tcsoa/gen/Cad/_2010_09/__init__.py
+-rw-r--r--   0        0        0     4659 2022-10-20 12:42:37.544513 tcsoa-0.9.1/tcsoa/gen/Cad/_2010_09/DataManagement.py
+-rw-r--r--   0        0        0     2238 2022-10-20 12:42:12.493079 tcsoa-0.9.1/tcsoa/gen/Cad/_2010_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.631037 tcsoa-0.9.1/tcsoa/gen/Cad/_2011_06/__init__.py
+-rw-r--r--   0        0        0     5037 2022-10-20 12:42:37.582517 tcsoa-0.9.1/tcsoa/gen/Cad/_2011_06/DataManagement.py
+-rw-r--r--   0        0        0     1866 2022-10-20 12:42:12.523081 tcsoa-0.9.1/tcsoa/gen/Cad/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.966070 tcsoa-0.9.1/tcsoa/gen/Cad/_2012_09/__init__.py
+-rw-r--r--   0        0        0    10891 2022-10-20 12:42:37.645516 tcsoa-0.9.1/tcsoa/gen/Cad/_2012_09/DataManagement.py
+-rw-r--r--   0        0        0     4218 2022-10-20 12:42:12.553087 tcsoa-0.9.1/tcsoa/gen/Cad/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.710040 tcsoa-0.9.1/tcsoa/gen/Cad/_2013_05/__init__.py
+-rw-r--r--   0        0        0    11796 2022-10-20 12:42:12.587090 tcsoa-0.9.1/tcsoa/gen/Cad/_2013_05/services.py
+-rw-r--r--   0        0        0    12241 2022-10-20 12:42:37.715523 tcsoa-0.9.1/tcsoa/gen/Cad/_2013_05/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.701045 tcsoa-0.9.1/tcsoa/gen/Cad/_2014_10/__init__.py
+-rw-r--r--   0        0        0     2932 2022-10-20 12:42:37.757525 tcsoa-0.9.1/tcsoa/gen/Cad/_2014_10/DataManagement.py
+-rw-r--r--   0        0        0     2235 2022-10-20 12:42:12.615098 tcsoa-0.9.1/tcsoa/gen/Cad/_2014_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.578033 tcsoa-0.9.1/tcsoa/gen/Cad/_2016_03/__init__.py
+-rw-r--r--   0        0        0    12961 2022-10-20 12:42:37.814539 tcsoa-0.9.1/tcsoa/gen/Cad/_2016_03/DataManagement.py
+-rw-r--r--   0        0        0    16904 2022-10-20 12:42:12.654112 tcsoa-0.9.1/tcsoa/gen/Cad/_2016_03/services.py
+-rw-r--r--   0        0        0     4554 2022-10-20 12:42:37.849542 tcsoa-0.9.1/tcsoa/gen/Cad/_2016_03/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.786052 tcsoa-0.9.1/tcsoa/gen/Cad/_2016_09/__init__.py
+-rw-r--r--   0        0        0    25023 2022-10-20 12:42:12.690109 tcsoa-0.9.1/tcsoa/gen/Cad/_2016_09/services.py
+-rw-r--r--   0        0        0    16193 2022-10-20 12:42:37.925553 tcsoa-0.9.1/tcsoa/gen/Cad/_2016_09/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.848063 tcsoa-0.9.1/tcsoa/gen/Cad/_2018_06/__init__.py
+-rw-r--r--   0        0        0     3225 2022-10-20 12:42:12.719108 tcsoa-0.9.1/tcsoa/gen/Cad/_2018_06/services.py
+-rw-r--r--   0        0        0      967 2022-10-20 12:42:37.953545 tcsoa-0.9.1/tcsoa/gen/Cad/_2018_06/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.919067 tcsoa-0.9.1/tcsoa/gen/Cad/_2019_06/__init__.py
+-rw-r--r--   0        0        0     1774 2022-10-20 12:42:12.748117 tcsoa-0.9.1/tcsoa/gen/Cad/_2019_06/services.py
+-rw-r--r--   0        0        0     3280 2022-10-20 12:42:37.983547 tcsoa-0.9.1/tcsoa/gen/Cad/_2019_06/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.659037 tcsoa-0.9.1/tcsoa/gen/Cad/_2020_01/__init__.py
+-rw-r--r--   0        0        0    39927 2022-10-20 12:42:38.183566 tcsoa-0.9.1/tcsoa/gen/Cad/_2020_01/AppSessionManagement.py
+-rw-r--r--   0        0        0     7315 2022-10-20 12:42:12.779119 tcsoa-0.9.1/tcsoa/gen/Cad/_2020_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.823056 tcsoa-0.9.1/tcsoa/gen/Cad/__init__.py
+-rw-r--r--   0        0        0     5836 2022-10-20 12:41:54.101115 tcsoa-0.9.1/tcsoa/gen/Cad/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.964078 tcsoa-0.9.1/tcsoa/gen/Cae/_2009_10/__init__.py
+-rw-r--r--   0        0        0      579 2022-10-20 12:42:38.210576 tcsoa-0.9.1/tcsoa/gen/Cae/_2009_10/SimulationProcessManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.739050 tcsoa-0.9.1/tcsoa/gen/Cae/_2011_06/__init__.py
+-rw-r--r--   0        0        0     4058 2022-10-20 12:42:12.809114 tcsoa-0.9.1/tcsoa/gen/Cae/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.742044 tcsoa-0.9.1/tcsoa/gen/Cae/_2012_02/__init__.py
+-rw-r--r--   0        0        0     8588 2022-10-20 12:42:12.843120 tcsoa-0.9.1/tcsoa/gen/Cae/_2012_02/services.py
+-rw-r--r--   0        0        0     2589 2022-10-20 12:42:38.238574 tcsoa-0.9.1/tcsoa/gen/Cae/_2012_02/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.653035 tcsoa-0.9.1/tcsoa/gen/Cae/_2013_12/__init__.py
+-rw-r--r--   0        0        0     4072 2022-10-20 12:42:12.873126 tcsoa-0.9.1/tcsoa/gen/Cae/_2013_12/services.py
+-rw-r--r--   0        0        0     1155 2022-10-20 12:42:38.271574 tcsoa-0.9.1/tcsoa/gen/Cae/_2013_12/SimulationProcessManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.908058 tcsoa-0.9.1/tcsoa/gen/Cae/_2014_06/__init__.py
+-rw-r--r--   0        0        0     3756 2022-10-20 12:42:12.902131 tcsoa-0.9.1/tcsoa/gen/Cae/_2014_06/services.py
+-rw-r--r--   0        0        0     2232 2022-10-20 12:42:38.302581 tcsoa-0.9.1/tcsoa/gen/Cae/_2014_06/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.815056 tcsoa-0.9.1/tcsoa/gen/Cae/__init__.py
+-rw-r--r--   0        0        0      746 2022-10-20 12:41:54.114103 tcsoa-0.9.1/tcsoa/gen/Cae/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.898059 tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2007_01/__init__.py
+-rw-r--r--   0        0        0     3944 2022-10-20 12:42:38.378585 tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2007_01/CalendarManagement.py
+-rw-r--r--   0        0        0     4731 2022-10-20 12:42:12.937134 tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2007_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.959069 tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2007_06/__init__.py
+-rw-r--r--   0        0        0     5023 2022-10-20 12:42:38.444593 tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2007_06/CalendarManagement.py
+-rw-r--r--   0        0        0     1474 2022-10-20 12:42:12.970129 tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.802053 tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0     2759 2022-10-20 12:42:38.486594 tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2008_06/CalendarManagement.py
+-rw-r--r--   0        0        0     2318 2022-10-20 12:42:13.001139 tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.855059 tcsoa-0.9.1/tcsoa/gen/CalendarManagement/__init__.py
+-rw-r--r--   0        0        0      777 2022-10-20 12:41:54.133108 tcsoa-0.9.1/tcsoa/gen/CalendarManagement/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.913065 tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0    14471 2022-10-20 12:42:38.637615 tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2008_06/ChangeManagement.py
+-rw-r--r--   0        0        0    26162 2022-10-20 12:42:13.910230 tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.650034 tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2009_06/__init__.py
+-rw-r--r--   0        0        0     2160 2022-10-20 12:42:38.675618 tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2009_06/ChangeManagement.py
+-rw-r--r--   0        0        0     3595 2022-10-20 12:42:13.940233 tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2009_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.796046 tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2015_10/__init__.py
+-rw-r--r--   0        0        0     2438 2022-10-20 12:42:38.718623 tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2015_10/ChangeManagement.py
+-rw-r--r--   0        0        0     3127 2022-10-20 12:42:13.972240 tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2015_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.669045 tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2020_01/__init__.py
+-rw-r--r--   0        0        0     5286 2022-10-20 12:42:38.762618 tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2020_01/ChangeManagement.py
+-rw-r--r--   0        0        0     1822 2022-10-20 12:42:14.005249 tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2020_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.732052 tcsoa-0.9.1/tcsoa/gen/ChangeManagement/__init__.py
+-rw-r--r--   0        0        0     1181 2022-10-20 12:41:54.163116 tcsoa-0.9.1/tcsoa/gen/ChangeManagement/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.762045 tcsoa-0.9.1/tcsoa/gen/Classification/_2007_01/__init__.py
+-rw-r--r--   0        0        0    25022 2022-10-20 12:42:38.963669 tcsoa-0.9.1/tcsoa/gen/Classification/_2007_01/Classification.py
+-rw-r--r--   0        0        0    24353 2022-10-20 12:42:14.095254 tcsoa-0.9.1/tcsoa/gen/Classification/_2007_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.000074 tcsoa-0.9.1/tcsoa/gen/Classification/_2009_10/__init__.py
+-rw-r--r--   0        0        0    10587 2022-10-20 12:42:39.045657 tcsoa-0.9.1/tcsoa/gen/Classification/_2009_10/Classification.py
+-rw-r--r--   0        0        0     6943 2022-10-20 12:42:14.132262 tcsoa-0.9.1/tcsoa/gen/Classification/_2009_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.845062 tcsoa-0.9.1/tcsoa/gen/Classification/_2011_06/__init__.py
+-rw-r--r--   0        0        0     2679 2022-10-20 12:42:39.083655 tcsoa-0.9.1/tcsoa/gen/Classification/_2011_06/Classification.py
+-rw-r--r--   0        0        0     2741 2022-10-20 12:42:14.163266 tcsoa-0.9.1/tcsoa/gen/Classification/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.938068 tcsoa-0.9.1/tcsoa/gen/Classification/_2011_12/__init__.py
+-rw-r--r--   0        0        0     5226 2022-10-20 12:42:39.148662 tcsoa-0.9.1/tcsoa/gen/Classification/_2011_12/Classification.py
+-rw-r--r--   0        0        0     1621 2022-10-20 12:42:14.194262 tcsoa-0.9.1/tcsoa/gen/Classification/_2011_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.812049 tcsoa-0.9.1/tcsoa/gen/Classification/_2015_03/__init__.py
+-rw-r--r--   0        0        0     2572 2022-10-20 12:42:39.193661 tcsoa-0.9.1/tcsoa/gen/Classification/_2015_03/Classification.py
+-rw-r--r--   0        0        0     2085 2022-10-20 12:42:14.223264 tcsoa-0.9.1/tcsoa/gen/Classification/_2015_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.628039 tcsoa-0.9.1/tcsoa/gen/Classification/_2015_10/__init__.py
+-rw-r--r--   0        0        0     3151 2022-10-20 12:42:39.236663 tcsoa-0.9.1/tcsoa/gen/Classification/_2015_10/Classification.py
+-rw-r--r--   0        0        0     1279 2022-10-20 12:42:14.251265 tcsoa-0.9.1/tcsoa/gen/Classification/_2015_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.971062 tcsoa-0.9.1/tcsoa/gen/Classification/_2016_03/__init__.py
+-rw-r--r--   0        0        0     6926 2022-10-20 12:42:39.308671 tcsoa-0.9.1/tcsoa/gen/Classification/_2016_03/Classification.py
+-rw-r--r--   0        0        0     4631 2022-10-20 12:42:14.286276 tcsoa-0.9.1/tcsoa/gen/Classification/_2016_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.764042 tcsoa-0.9.1/tcsoa/gen/Classification/_2016_09/__init__.py
+-rw-r--r--   0        0        0     2883 2022-10-20 12:42:39.353677 tcsoa-0.9.1/tcsoa/gen/Classification/_2016_09/Classification.py
+-rw-r--r--   0        0        0     2237 2022-10-20 12:42:14.315281 tcsoa-0.9.1/tcsoa/gen/Classification/_2016_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.797053 tcsoa-0.9.1/tcsoa/gen/Classification/__init__.py
+-rw-r--r--   0        0        0     2291 2022-10-20 12:41:54.212125 tcsoa-0.9.1/tcsoa/gen/Classification/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.861060 tcsoa-0.9.1/tcsoa/gen/ClassificationCommon/_2020_01/__init__.py
+-rw-r--r--   0        0        0     1440 2022-10-20 12:42:14.035253 tcsoa-0.9.1/tcsoa/gen/ClassificationCommon/_2020_01/Classification.py
+-rw-r--r--   0        0        0     3739 2022-10-20 12:42:14.349282 tcsoa-0.9.1/tcsoa/gen/ClassificationCommon/_2020_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.729050 tcsoa-0.9.1/tcsoa/gen/ClassificationCommon/_2020_12/__init__.py
+-rw-r--r--   0        0        0     3480 2022-10-20 12:42:14.382283 tcsoa-0.9.1/tcsoa/gen/ClassificationCommon/_2020_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.858074 tcsoa-0.9.1/tcsoa/gen/ClassificationCommon/__init__.py
+-rw-r--r--   0        0        0      609 2022-10-20 12:41:54.224120 tcsoa-0.9.1/tcsoa/gen/ClassificationCommon/services.py
+-rw-r--r--   0        0        0      889 2022-10-20 12:42:39.395686 tcsoa-0.9.1/tcsoa/gen/Common.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.813096 tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2011_06/__init__.py
+-rw-r--r--   0        0        0    17164 2022-10-20 12:42:16.906585 tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2011_06/EffectivityManagement.py
+-rw-r--r--   0        0        0    46040 2022-10-20 12:42:14.437281 tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.963092 tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2013_05/__init__.py
+-rw-r--r--   0        0        0     3870 2022-10-20 12:42:16.953594 tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2013_05/EffectivityManagement.py
+-rw-r--r--   0        0        0    18013 2022-10-20 12:42:14.478290 tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2013_05/services.py
+-rw-r--r--   0        0        0    13695 2022-10-20 12:42:17.033596 tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2013_05/VariantManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.713049 tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2017_05/__init__.py
+-rw-r--r--   0        0        0     1758 2022-10-20 12:42:17.073603 tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2017_05/EffectivityManagement.py
+-rw-r--r--   0        0        0     7726 2022-10-20 12:42:14.511293 tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2017_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.667044 tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/__init__.py
+-rw-r--r--   0        0        0     1518 2022-10-20 12:41:54.255116 tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.750043 tcsoa-0.9.1/tcsoa/gen/Configuration/_2010_04/__init__.py
+-rw-r--r--   0        0        0     7365 2022-10-20 12:42:14.553298 tcsoa-0.9.1/tcsoa/gen/Configuration/_2010_04/services.py
+-rw-r--r--   0        0        0     9804 2022-10-20 12:42:39.498703 tcsoa-0.9.1/tcsoa/gen/Configuration/_2010_04/SmartUiBldr.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.644039 tcsoa-0.9.1/tcsoa/gen/Configuration/__init__.py
+-rw-r--r--   0        0        0      592 2022-10-20 12:41:54.271125 tcsoa-0.9.1/tcsoa/gen/Configuration/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.996070 tcsoa-0.9.1/tcsoa/gen/Configurator/_2014_12/__init__.py
+-rw-r--r--   0        0        0     2233 2022-10-20 12:42:13.046144 tcsoa-0.9.1/tcsoa/gen/Configurator/_2014_12/ConfiguratorManagement.py
+-rw-r--r--   0        0        0     2766 2022-10-20 12:42:14.584353 tcsoa-0.9.1/tcsoa/gen/Configurator/_2014_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.616029 tcsoa-0.9.1/tcsoa/gen/Configurator/__init__.py
+-rw-r--r--   0        0        0      225 2022-10-20 12:41:54.277124 tcsoa-0.9.1/tcsoa/gen/Configurator/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.609032 tcsoa-0.9.1/tcsoa/gen/Core/_2006_03/__init__.py
+-rw-r--r--   0        0        0    12176 2022-10-20 12:42:39.692708 tcsoa-0.9.1/tcsoa/gen/Core/_2006_03/DataManagement.py
+-rw-r--r--   0        0        0     5455 2022-10-20 12:42:39.747713 tcsoa-0.9.1/tcsoa/gen/Core/_2006_03/FileManagement.py
+-rw-r--r--   0        0        0     1368 2022-10-20 12:42:39.784714 tcsoa-0.9.1/tcsoa/gen/Core/_2006_03/Reservation.py
+-rw-r--r--   0        0        0    33500 2022-10-20 12:42:14.682311 tcsoa-0.9.1/tcsoa/gen/Core/_2006_03/services.py
+-rw-r--r--   0        0        0     2759 2022-10-20 12:42:39.843721 tcsoa-0.9.1/tcsoa/gen/Core/_2006_03/Session.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.943068 tcsoa-0.9.1/tcsoa/gen/Core/_2007_01/__init__.py
+-rw-r--r--   0        0        0    13487 2022-10-20 12:42:40.011741 tcsoa-0.9.1/tcsoa/gen/Core/_2007_01/DataManagement.py
+-rw-r--r--   0        0        0     1445 2022-10-20 12:42:40.050739 tcsoa-0.9.1/tcsoa/gen/Core/_2007_01/FileManagement.py
+-rw-r--r--   0        0        0     3478 2022-10-20 12:42:40.123752 tcsoa-0.9.1/tcsoa/gen/Core/_2007_01/ManagedRelations.py
+-rw-r--r--   0        0        0    21587 2022-10-20 12:42:14.762321 tcsoa-0.9.1/tcsoa/gen/Core/_2007_01/services.py
+-rw-r--r--   0        0        0     4657 2022-10-20 12:42:40.178751 tcsoa-0.9.1/tcsoa/gen/Core/_2007_01/Session.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.005088 tcsoa-0.9.1/tcsoa/gen/Core/_2007_06/__init__.py
+-rw-r--r--   0        0        0    11098 2022-10-20 12:42:40.320765 tcsoa-0.9.1/tcsoa/gen/Core/_2007_06/DataManagement.py
+-rw-r--r--   0        0        0     1299 2022-10-20 12:42:40.361775 tcsoa-0.9.1/tcsoa/gen/Core/_2007_06/LOV.py
+-rw-r--r--   0        0        0     3885 2022-10-20 12:42:40.410775 tcsoa-0.9.1/tcsoa/gen/Core/_2007_06/PropDescriptor.py
+-rw-r--r--   0        0        0    10963 2022-10-20 12:42:14.825321 tcsoa-0.9.1/tcsoa/gen/Core/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.629037 tcsoa-0.9.1/tcsoa/gen/Core/_2007_09/__init__.py
+-rw-r--r--   0        0        0     4979 2022-10-20 12:42:40.476780 tcsoa-0.9.1/tcsoa/gen/Core/_2007_09/DataManagement.py
+-rw-r--r--   0        0        0      842 2022-10-20 12:42:40.503783 tcsoa-0.9.1/tcsoa/gen/Core/_2007_09/ProjectLevelSecurity.py
+-rw-r--r--   0        0        0     7743 2022-10-20 12:42:14.868332 tcsoa-0.9.1/tcsoa/gen/Core/_2007_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.915058 tcsoa-0.9.1/tcsoa/gen/Core/_2007_12/__init__.py
+-rw-r--r--   0        0        0     5967 2022-10-20 12:42:40.585790 tcsoa-0.9.1/tcsoa/gen/Core/_2007_12/DataManagement.py
+-rw-r--r--   0        0        0     8982 2022-10-20 12:42:14.912339 tcsoa-0.9.1/tcsoa/gen/Core/_2007_12/services.py
+-rw-r--r--   0        0        0      394 2022-10-20 12:42:40.614792 tcsoa-0.9.1/tcsoa/gen/Core/_2007_12/Session.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.678047 tcsoa-0.9.1/tcsoa/gen/Core/_2008_03/__init__.py
+-rw-r--r--   0        0        0     4782 2022-10-20 12:42:14.944341 tcsoa-0.9.1/tcsoa/gen/Core/_2008_03/services.py
+-rw-r--r--   0        0        0     4528 2022-10-20 12:42:40.669805 tcsoa-0.9.1/tcsoa/gen/Core/_2008_03/Session.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.792046 tcsoa-0.9.1/tcsoa/gen/Core/_2008_05/__init__.py
+-rw-r--r--   0        0        0      955 2022-10-20 12:42:14.973340 tcsoa-0.9.1/tcsoa/gen/Core/_2008_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.871054 tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/__init__.py
+-rw-r--r--   0        0        0    42394 2022-10-20 12:42:41.012827 tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/DataManagement.py
+-rw-r--r--   0        0        0     2947 2022-10-20 12:42:41.056839 tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/DispatcherManagement.py
+-rw-r--r--   0        0        0     1023 2022-10-20 12:42:41.090836 tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/ManagedRelations.py
+-rw-r--r--   0        0        0     7354 2022-10-20 12:42:41.139843 tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/PropDescriptor.py
+-rw-r--r--   0        0        0    44261 2022-10-20 12:42:15.084360 tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/services.py
+-rw-r--r--   0        0        0      858 2022-10-20 12:42:41.176875 tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/Session.py
+-rw-r--r--   0        0        0     5315 2022-10-20 12:42:41.250849 tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.688041 tcsoa-0.9.1/tcsoa/gen/Core/_2009_04/__init__.py
+-rw-r--r--   0        0        0      554 2022-10-20 12:42:41.280853 tcsoa-0.9.1/tcsoa/gen/Core/_2009_04/ProjectLevelSecurity.py
+-rw-r--r--   0        0        0     2654 2022-10-20 12:42:15.126355 tcsoa-0.9.1/tcsoa/gen/Core/_2009_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.698047 tcsoa-0.9.1/tcsoa/gen/Core/_2009_10/__init__.py
+-rw-r--r--   0        0        0     5649 2022-10-20 12:42:41.351859 tcsoa-0.9.1/tcsoa/gen/Core/_2009_10/DataManagement.py
+-rw-r--r--   0        0        0     3174 2022-10-20 12:42:41.396876 tcsoa-0.9.1/tcsoa/gen/Core/_2009_10/ProjectLevelSecurity.py
+-rw-r--r--   0        0        0     8459 2022-10-20 12:42:15.167357 tcsoa-0.9.1/tcsoa/gen/Core/_2009_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.969063 tcsoa-0.9.1/tcsoa/gen/Core/_2010_04/__init__.py
+-rw-r--r--   0        0        0    13086 2022-10-20 12:42:41.540879 tcsoa-0.9.1/tcsoa/gen/Core/_2010_04/DataManagement.py
+-rw-r--r--   0        0        0     2123 2022-10-20 12:42:41.589887 tcsoa-0.9.1/tcsoa/gen/Core/_2010_04/LanguageInformation.py
+-rw-r--r--   0        0        0    14216 2022-10-20 12:42:15.228363 tcsoa-0.9.1/tcsoa/gen/Core/_2010_04/services.py
+-rw-r--r--   0        0        0     8315 2022-10-20 12:42:41.649888 tcsoa-0.9.1/tcsoa/gen/Core/_2010_04/Session.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.557031 tcsoa-0.9.1/tcsoa/gen/Core/_2010_09/__init__.py
+-rw-r--r--   0        0        0    10139 2022-10-20 12:42:41.759900 tcsoa-0.9.1/tcsoa/gen/Core/_2010_09/DataManagement.py
+-rw-r--r--   0        0        0     8728 2022-10-20 12:42:15.268373 tcsoa-0.9.1/tcsoa/gen/Core/_2010_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.621029 tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/__init__.py
+-rw-r--r--   0        0        0    14393 2022-10-20 12:42:41.870913 tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/DataManagement.py
+-rw-r--r--   0        0        0     1534 2022-10-20 12:42:41.908915 tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/LOV.py
+-rw-r--r--   0        0        0    11510 2022-10-20 12:42:41.966927 tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/OperationDescriptor.py
+-rw-r--r--   0        0        0     3652 2022-10-20 12:42:42.008926 tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/PropDescriptor.py
+-rw-r--r--   0        0        0      891 2022-10-20 12:42:42.035926 tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/Reservation.py
+-rw-r--r--   0        0        0    22526 2022-10-20 12:42:15.354385 tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/services.py
+-rw-r--r--   0        0        0     3130 2022-10-20 12:42:42.077935 tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/Session.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.646039 tcsoa-0.9.1/tcsoa/gen/Core/_2012_02/__init__.py
+-rw-r--r--   0        0        0     5350 2022-10-20 12:42:42.139943 tcsoa-0.9.1/tcsoa/gen/Core/_2012_02/DataManagement.py
+-rw-r--r--   0        0        0     1284 2022-10-20 12:42:42.174938 tcsoa-0.9.1/tcsoa/gen/Core/_2012_02/OperationDescriptor.py
+-rw-r--r--   0        0        0    11281 2022-10-20 12:42:15.406373 tcsoa-0.9.1/tcsoa/gen/Core/_2012_02/services.py
+-rw-r--r--   0        0        0      718 2022-10-20 12:42:42.209947 tcsoa-0.9.1/tcsoa/gen/Core/_2012_02/Session.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.999090 tcsoa-0.9.1/tcsoa/gen/Core/_2012_09/__init__.py
+-rw-r--r--   0        0        0      951 2022-10-20 12:42:42.238943 tcsoa-0.9.1/tcsoa/gen/Core/_2012_09/DataManagement.py
+-rw-r--r--   0        0        0     4809 2022-10-20 12:42:42.315953 tcsoa-0.9.1/tcsoa/gen/Core/_2012_09/ProjectLevelSecurity.py
+-rw-r--r--   0        0        0     4626 2022-10-20 12:42:15.455379 tcsoa-0.9.1/tcsoa/gen/Core/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.912057 tcsoa-0.9.1/tcsoa/gen/Core/_2012_10/__init__.py
+-rw-r--r--   0        0        0     8089 2022-10-20 12:42:42.376958 tcsoa-0.9.1/tcsoa/gen/Core/_2012_10/DataManagement.py
+-rw-r--r--   0        0        0     6317 2022-10-20 12:42:15.492433 tcsoa-0.9.1/tcsoa/gen/Core/_2012_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.930066 tcsoa-0.9.1/tcsoa/gen/Core/_2013_05/__init__.py
+-rw-r--r--   0        0        0    24882 2022-10-20 12:42:42.528979 tcsoa-0.9.1/tcsoa/gen/Core/_2013_05/DataManagement.py
+-rw-r--r--   0        0        0    14427 2022-10-20 12:42:42.597983 tcsoa-0.9.1/tcsoa/gen/Core/_2013_05/LOV.py
+-rw-r--r--   0        0        0    21845 2022-10-20 12:42:15.548393 tcsoa-0.9.1/tcsoa/gen/Core/_2013_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.011070 tcsoa-0.9.1/tcsoa/gen/Core/_2014_06/__init__.py
+-rw-r--r--   0        0        0     7307 2022-10-20 12:42:42.657982 tcsoa-0.9.1/tcsoa/gen/Core/_2014_06/DataManagement.py
+-rw-r--r--   0        0        0     1984 2022-10-20 12:42:42.700993 tcsoa-0.9.1/tcsoa/gen/Core/_2014_06/DigitalSignature.py
+-rw-r--r--   0        0        0    15021 2022-10-20 12:42:15.601395 tcsoa-0.9.1/tcsoa/gen/Core/_2014_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.916066 tcsoa-0.9.1/tcsoa/gen/Core/_2014_10/__init__.py
+-rw-r--r--   0        0        0    10059 2022-10-20 12:42:42.785002 tcsoa-0.9.1/tcsoa/gen/Core/_2014_10/DataManagement.py
+-rw-r--r--   0        0        0     1727 2022-10-20 12:42:42.819007 tcsoa-0.9.1/tcsoa/gen/Core/_2014_10/ProjectLevelSecurity.py
+-rw-r--r--   0        0        0    13780 2022-10-20 12:42:15.656416 tcsoa-0.9.1/tcsoa/gen/Core/_2014_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.802053 tcsoa-0.9.1/tcsoa/gen/Core/_2015_07/__init__.py
+-rw-r--r--   0        0        0    22547 2022-10-20 12:42:42.914013 tcsoa-0.9.1/tcsoa/gen/Core/_2015_07/DataManagement.py
+-rw-r--r--   0        0        0    14880 2022-10-20 12:42:15.698398 tcsoa-0.9.1/tcsoa/gen/Core/_2015_07/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.916066 tcsoa-0.9.1/tcsoa/gen/Core/_2015_10/__init__.py
+-rw-r--r--   0        0        0     2981 2022-10-20 12:42:42.953017 tcsoa-0.9.1/tcsoa/gen/Core/_2015_10/DataManagement.py
+-rw-r--r--   0        0        0     3526 2022-10-20 12:42:42.995016 tcsoa-0.9.1/tcsoa/gen/Core/_2015_10/FileManagement.py
+-rw-r--r--   0        0        0    14836 2022-10-20 12:42:15.754414 tcsoa-0.9.1/tcsoa/gen/Core/_2015_10/services.py
+-rw-r--r--   0        0        0      206 2022-10-20 12:42:43.017014 tcsoa-0.9.1/tcsoa/gen/Core/_2015_10/Session.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.670045 tcsoa-0.9.1/tcsoa/gen/Core/_2016_05/__init__.py
+-rw-r--r--   0        0        0     5393 2022-10-20 12:42:43.067024 tcsoa-0.9.1/tcsoa/gen/Core/_2016_05/DataManagement.py
+-rw-r--r--   0        0        0     6543 2022-10-20 12:42:15.786417 tcsoa-0.9.1/tcsoa/gen/Core/_2016_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.989074 tcsoa-0.9.1/tcsoa/gen/Core/_2016_09/__init__.py
+-rw-r--r--   0        0        0     1312 2022-10-20 12:42:43.099025 tcsoa-0.9.1/tcsoa/gen/Core/_2016_09/DataManagement.py
+-rw-r--r--   0        0        0     3885 2022-10-20 12:42:15.815419 tcsoa-0.9.1/tcsoa/gen/Core/_2016_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.734041 tcsoa-0.9.1/tcsoa/gen/Core/_2016_10/__init__.py
+-rw-r--r--   0        0        0     1849 2022-10-20 12:42:15.844414 tcsoa-0.9.1/tcsoa/gen/Core/_2016_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.580034 tcsoa-0.9.1/tcsoa/gen/Core/_2017_05/__init__.py
+-rw-r--r--   0        0        0     1199 2022-10-20 12:42:43.124033 tcsoa-0.9.1/tcsoa/gen/Core/_2017_05/FileManagement.py
+-rw-r--r--   0        0        0    16168 2022-10-20 12:42:43.236038 tcsoa-0.9.1/tcsoa/gen/Core/_2017_05/ProjectLevelSecurity.py
+-rw-r--r--   0        0        0    12864 2022-10-20 12:42:15.896428 tcsoa-0.9.1/tcsoa/gen/Core/_2017_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.697040 tcsoa-0.9.1/tcsoa/gen/Core/_2017_11/__init__.py
+-rw-r--r--   0        0        0     7279 2022-10-20 12:42:43.346047 tcsoa-0.9.1/tcsoa/gen/Core/_2017_11/LogicalObject.py
+-rw-r--r--   0        0        0     6236 2022-10-20 12:42:15.926443 tcsoa-0.9.1/tcsoa/gen/Core/_2017_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.548030 tcsoa-0.9.1/tcsoa/gen/Core/_2018_06/__init__.py
+-rw-r--r--   0        0        0     1164 2022-10-20 12:42:43.374049 tcsoa-0.9.1/tcsoa/gen/Core/_2018_06/DataManagement.py
+-rw-r--r--   0        0        0     5620 2022-10-20 12:42:43.480059 tcsoa-0.9.1/tcsoa/gen/Core/_2018_06/LogicalObject.py
+-rw-r--r--   0        0        0    11606 2022-10-20 12:42:15.964433 tcsoa-0.9.1/tcsoa/gen/Core/_2018_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.562032 tcsoa-0.9.1/tcsoa/gen/Core/_2018_11/__init__.py
+-rw-r--r--   0        0        0     4399 2022-10-20 12:42:43.551067 tcsoa-0.9.1/tcsoa/gen/Core/_2018_11/LogicalObject.py
+-rw-r--r--   0        0        0     1894 2022-10-20 12:42:43.599076 tcsoa-0.9.1/tcsoa/gen/Core/_2018_11/ProjectLevelSecurity.py
+-rw-r--r--   0        0        0    20392 2022-10-20 12:42:16.005442 tcsoa-0.9.1/tcsoa/gen/Core/_2018_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.894059 tcsoa-0.9.1/tcsoa/gen/Core/_2019_06/__init__.py
+-rw-r--r--   0        0        0     1121 2022-10-20 12:42:43.630075 tcsoa-0.9.1/tcsoa/gen/Core/_2019_06/DataManagement.py
+-rw-r--r--   0        0        0     2465 2022-10-20 12:42:16.043446 tcsoa-0.9.1/tcsoa/gen/Core/_2019_06/services.py
+-rw-r--r--   0        0        0     1200 2022-10-20 12:42:43.657079 tcsoa-0.9.1/tcsoa/gen/Core/_2019_06/Session.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.612029 tcsoa-0.9.1/tcsoa/gen/Core/_2020_01/__init__.py
+-rw-r--r--   0        0        0     4349 2022-10-20 12:42:43.708084 tcsoa-0.9.1/tcsoa/gen/Core/_2020_01/DataManagement.py
+-rw-r--r--   0        0        0     9799 2022-10-20 12:42:43.807099 tcsoa-0.9.1/tcsoa/gen/Core/_2020_01/ProjectLevelSecurity.py
+-rw-r--r--   0        0        0    10879 2022-10-20 12:42:16.094451 tcsoa-0.9.1/tcsoa/gen/Core/_2020_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.574032 tcsoa-0.9.1/tcsoa/gen/Core/_2020_04/__init__.py
+-rw-r--r--   0        0        0     1872 2022-10-20 12:42:43.835091 tcsoa-0.9.1/tcsoa/gen/Core/_2020_04/DataManagement.py
+-rw-r--r--   0        0        0     1465 2022-10-20 12:42:16.124447 tcsoa-0.9.1/tcsoa/gen/Core/_2020_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.640035 tcsoa-0.9.1/tcsoa/gen/Core/__init__.py
+-rw-r--r--   0        0        0    17783 2022-10-20 12:41:54.618157 tcsoa-0.9.1/tcsoa/gen/Core/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.682047 tcsoa-0.9.1/tcsoa/gen/Diagramming/_2011_06/__init__.py
+-rw-r--r--   0        0        0    12475 2022-10-20 12:42:17.204620 tcsoa-0.9.1/tcsoa/gen/Diagramming/_2011_06/DiagramManagement.py
+-rw-r--r--   0        0        0     7023 2022-10-20 12:42:16.163457 tcsoa-0.9.1/tcsoa/gen/Diagramming/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.809054 tcsoa-0.9.1/tcsoa/gen/Diagramming/_2012_09/__init__.py
+-rw-r--r--   0        0        0     1696 2022-10-20 12:42:17.237618 tcsoa-0.9.1/tcsoa/gen/Diagramming/_2012_09/DiagramManagement.py
+-rw-r--r--   0        0        0     2303 2022-10-20 12:42:16.193454 tcsoa-0.9.1/tcsoa/gen/Diagramming/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.876055 tcsoa-0.9.1/tcsoa/gen/Diagramming/_2014_06/__init__.py
+-rw-r--r--   0        0        0     6113 2022-10-20 12:42:17.303626 tcsoa-0.9.1/tcsoa/gen/Diagramming/_2014_06/DNDManagement.py
+-rw-r--r--   0        0        0     9098 2022-10-20 12:42:16.230454 tcsoa-0.9.1/tcsoa/gen/Diagramming/_2014_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.732052 tcsoa-0.9.1/tcsoa/gen/Diagramming/__init__.py
+-rw-r--r--   0        0        0      775 2022-10-20 12:41:54.634164 tcsoa-0.9.1/tcsoa/gen/Diagramming/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.866073 tcsoa-0.9.1/tcsoa/gen/DocMgmtAw/_2017_06/__init__.py
+-rw-r--r--   0        0        0      770 2022-10-20 12:42:16.264456 tcsoa-0.9.1/tcsoa/gen/DocMgmtAw/_2017_06/DocMgmt.py
+-rw-r--r--   0        0        0      894 2022-10-20 12:42:16.355472 tcsoa-0.9.1/tcsoa/gen/DocMgmtAw/_2017_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.951068 tcsoa-0.9.1/tcsoa/gen/DocMgmtAw/__init__.py
+-rw-r--r--   0        0        0      202 2022-10-20 12:41:54.640164 tcsoa-0.9.1/tcsoa/gen/DocMgmtAw/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.608029 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2007_01/__init__.py
+-rw-r--r--   0        0        0     2238 2022-10-20 12:42:43.880106 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2007_01/DocumentTemplate.py
+-rw-r--r--   0        0        0     2515 2022-10-20 12:42:16.388488 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2007_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.932066 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0     4375 2022-10-20 12:42:43.957129 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2008_06/DocumentControl.py
+-rw-r--r--   0        0        0     5987 2022-10-20 12:42:16.424479 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.738043 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2010_04/__init__.py
+-rw-r--r--   0        0        0     1559 2022-10-20 12:42:43.989119 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2010_04/DigitalSignature.py
+-rw-r--r--   0        0        0     4286 2022-10-20 12:42:44.044111 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2010_04/LaunchDefinition.py
+-rw-r--r--   0        0        0     3820 2022-10-20 12:42:16.460490 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.922066 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2011_06/__init__.py
+-rw-r--r--   0        0        0     9082 2022-10-20 12:42:44.136128 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2011_06/AttributeExchange.py
+-rw-r--r--   0        0        0     5352 2022-10-20 12:42:16.492481 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.849072 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2013_12/__init__.py
+-rw-r--r--   0        0        0     4632 2022-10-20 12:42:44.192134 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2013_12/PrintOrRender.py
+-rw-r--r--   0        0        0     2528 2022-10-20 12:42:16.537135 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2013_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.763049 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2018_06/__init__.py
+-rw-r--r--   0        0        0     1266 2022-10-20 12:42:16.570140 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2018_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.710040 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2018_11/__init__.py
+-rw-r--r--   0        0        0      712 2022-10-20 12:42:44.220130 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2018_11/PrintOrRender.py
+-rw-r--r--   0        0        0     3407 2022-10-20 12:42:16.619543 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2018_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.982071 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/__init__.py
+-rw-r--r--   0        0        0     1856 2022-10-20 12:41:54.666168 tcsoa-0.9.1/tcsoa/gen/DocumentManagement/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.712045 tcsoa-0.9.1/tcsoa/gen/EditContext/_2014_12/__init__.py
+-rw-r--r--   0        0        0     1416 2022-10-20 12:42:16.653537 tcsoa-0.9.1/tcsoa/gen/EditContext/_2014_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.902061 tcsoa-0.9.1/tcsoa/gen/EditContext/_2015_07/__init__.py
+-rw-r--r--   0        0        0     1181 2022-10-20 12:42:17.337622 tcsoa-0.9.1/tcsoa/gen/EditContext/_2015_07/DataManagement.py
+-rw-r--r--   0        0        0     1459 2022-10-20 12:42:16.683542 tcsoa-0.9.1/tcsoa/gen/EditContext/_2015_07/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.956087 tcsoa-0.9.1/tcsoa/gen/EditContext/_2016_04/__init__.py
+-rw-r--r--   0        0        0      820 2022-10-20 12:42:17.365626 tcsoa-0.9.1/tcsoa/gen/EditContext/_2016_04/DataManagement.py
+-rw-r--r--   0        0        0     2877 2022-10-20 12:42:16.714530 tcsoa-0.9.1/tcsoa/gen/EditContext/_2016_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.614029 tcsoa-0.9.1/tcsoa/gen/EditContext/_2016_10/__init__.py
+-rw-r--r--   0        0        0     2678 2022-10-20 12:42:17.407661 tcsoa-0.9.1/tcsoa/gen/EditContext/_2016_10/DataManagement.py
+-rw-r--r--   0        0        0     3003 2022-10-20 12:42:16.745533 tcsoa-0.9.1/tcsoa/gen/EditContext/_2016_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.828056 tcsoa-0.9.1/tcsoa/gen/EditContext/__init__.py
+-rw-r--r--   0        0        0      611 2022-10-20 12:41:54.676168 tcsoa-0.9.1/tcsoa/gen/EditContext/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.965064 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2007_06/__init__.py
+-rw-r--r--   0        0        0    19857 2022-10-20 12:42:44.372144 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2007_06/ImportExport.py
+-rw-r--r--   0        0        0    20382 2022-10-20 12:42:18.723755 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.921064 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2007_12/__init__.py
+-rw-r--r--   0        0        0     1041 2022-10-20 12:42:44.411146 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2007_12/ImportExport.py
+-rw-r--r--   0        0        0     2960 2022-10-20 12:42:18.756757 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2007_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.877060 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2008_06/__init__.py
+-rw-r--r--   0        0        0     2457 2022-10-20 12:42:44.451158 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2008_06/ImportExport.py
+-rw-r--r--   0        0        0     3920 2022-10-20 12:42:18.791758 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.920064 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2010_04/__init__.py
+-rw-r--r--   0        0        0     2052 2022-10-20 12:42:44.489155 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2010_04/ImportExport.py
+-rw-r--r--   0        0        0     3816 2022-10-20 12:42:18.825766 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.596030 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2011_06/__init__.py
+-rw-r--r--   0        0        0     2321 2022-10-20 12:42:44.526158 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2011_06/ImportExport.py
+-rw-r--r--   0        0        0     2794 2022-10-20 12:42:18.859768 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.012069 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2020_04/__init__.py
+-rw-r--r--   0        0        0     1351 2022-10-20 12:42:44.553160 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2020_04/ImportExport.py
+-rw-r--r--   0        0        0     2591 2022-10-20 12:42:18.891768 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2020_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.940067 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/__init__.py
+-rw-r--r--   0        0        0     2285 2022-10-20 12:41:54.722165 tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.776046 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2007_06/__init__.py
+-rw-r--r--   0        0        0     3117 2022-10-20 12:42:44.597166 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2007_06/FileImportExport.py
+-rw-r--r--   0        0        0     5436 2022-10-20 12:42:19.327814 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.960068 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2008_06/__init__.py
+-rw-r--r--   0        0        0     7324 2022-10-20 12:42:44.652170 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2008_06/FileImportExport.py
+-rw-r--r--   0        0        0     9265 2022-10-20 12:42:19.364822 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.660035 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2011_06/__init__.py
+-rw-r--r--   0        0        0    16647 2022-10-20 12:42:44.754186 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2011_06/FileImportExport.py
+-rw-r--r--   0        0        0    14690 2022-10-20 12:42:19.402815 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.568034 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2012_09/__init__.py
+-rw-r--r--   0        0        0     1801 2022-10-20 12:42:44.781185 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2012_09/FileImportExport.py
+-rw-r--r--   0        0        0     1613 2022-10-20 12:42:19.432825 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.750043 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2017_11/__init__.py
+-rw-r--r--   0        0        0     1734 2022-10-20 12:42:44.816194 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2017_11/FileImportExport.py
+-rw-r--r--   0        0        0     2095 2022-10-20 12:42:19.462828 tcsoa-0.9.1/tcsoa/gen/ImportExport/_2017_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.939068 tcsoa-0.9.1/tcsoa/gen/ImportExport/__init__.py
+-rw-r--r--   0        0        0     1138 2022-10-20 12:41:54.746176 tcsoa-0.9.1/tcsoa/gen/ImportExport/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.931067 tcsoa-0.9.1/tcsoa/gen/Internal/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.730042 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2012_10/__init__.py
+-rw-r--r--   0        0        0     5723 2022-10-20 12:41:58.892622 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2012_10/BOMIndexManagement.py
+-rw-r--r--   0        0        0    27548 2022-10-20 12:41:59.084644 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2012_10/OccurrenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.766045 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_03/__init__.py
+-rw-r--r--   0        0        0     2082 2022-10-20 12:41:59.121646 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_03/OccurrenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.658041 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_07/__init__.py
+-rw-r--r--   0        0        0    12281 2022-10-20 12:41:59.208657 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_07/OccurrenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.763049 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_10/__init__.py
+-rw-r--r--   0        0        0      913 2022-10-20 12:41:59.235649 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_10/OccurrenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.694046 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2016_03/__init__.py
+-rw-r--r--   0        0        0    10612 2022-10-20 12:41:59.311673 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2016_03/OccurrenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.789043 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_06/__init__.py
+-rw-r--r--   0        0        0     3794 2022-10-20 12:41:59.353666 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_06/OccurrenceConfiguration.py
+-rw-r--r--   0        0        0    11699 2022-10-20 12:41:59.426672 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_06/OccurrenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.820055 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_12/__init__.py
+-rw-r--r--   0        0        0     4406 2022-10-20 12:41:59.476680 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_12/OccurrenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.827050 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_05/__init__.py
+-rw-r--r--   0        0        0      937 2022-10-20 12:41:59.504698 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_05/Compare.py
+-rw-r--r--   0        0        0     4617 2022-10-20 12:41:59.559687 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_05/OccurrenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.865059 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_12/__init__.py
+-rw-r--r--   0        0        0    11014 2022-10-20 12:41:59.611692 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_12/Compare.py
+-rw-r--r--   0        0        0      664 2022-10-20 12:41:59.638698 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_12/Markup.py
+-rw-r--r--   0        0        0    13867 2022-10-20 12:41:59.713710 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_12/OccurrenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.980065 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_06/__init__.py
+-rw-r--r--   0        0        0     1859 2022-10-20 12:41:59.748710 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_06/Compare.py
+-rw-r--r--   0        0        0    22465 2022-10-20 12:41:59.858726 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_06/OccurrenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.771052 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_12/__init__.py
+-rw-r--r--   0        0        0     2280 2022-10-20 12:41:59.898734 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_12/DataManagement.py
+-rw-r--r--   0        0        0     7862 2022-10-20 12:41:59.975733 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_12/OccurrenceConfiguration.py
+-rw-r--r--   0        0        0    20998 2022-10-20 12:42:00.099748 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_12/OccurrenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.892058 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2020_05/__init__.py
+-rw-r--r--   0        0        0     2126 2022-10-20 12:42:00.133755 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2020_05/OccurrenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.586038 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2020_12/__init__.py
+-rw-r--r--   0        0        0     9877 2022-10-20 12:42:00.217763 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2020_12/OccurrenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.928070 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.791043 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceVis/_2014_11/__init__.py
+-rw-r--r--   0        0        0     2642 2022-10-20 12:42:03.985175 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceVis/_2014_11/OccurrenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.780047 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceVis/_2015_03/__init__.py
+-rw-r--r--   0        0        0    13386 2022-10-20 12:42:04.103175 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceVis/_2015_03/MassiveModelVisualization.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.794044 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceVis/_2018_05/__init__.py
+-rw-r--r--   0        0        0     2695 2022-10-20 12:42:04.148180 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceVis/_2018_05/MassiveModelVisualization.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.683038 tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceVis/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.721045 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2007_06/__init__.py
+-rw-r--r--   0        0        0     2612 2022-10-20 12:42:44.861189 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2007_06/Authorization.py
+-rw-r--r--   0        0        0     5400 2022-10-20 12:42:44.931196 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2007_06/PreferenceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.577032 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2008_06/__init__.py
+-rw-r--r--   0        0        0      985 2022-10-20 12:42:44.965199 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2008_06/IRM.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.637041 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2009_10/__init__.py
+-rw-r--r--   0        0        0     1060 2022-10-20 12:42:45.000199 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2009_10/PersonManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.708044 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2011_06/__init__.py
+-rw-r--r--   0        0        0     3412 2022-10-20 12:42:45.058205 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2011_06/OrganizationManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.859054 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2012_10/__init__.py
+-rw-r--r--   0        0        0     2936 2022-10-20 12:42:45.099213 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2012_10/OrganizationManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.684038 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2013_05/__init__.py
+-rw-r--r--   0        0        0     1716 2022-10-20 12:42:45.140214 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2013_05/UserManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.636038 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2014_10/__init__.py
+-rw-r--r--   0        0        0     1060 2022-10-20 12:42:45.168226 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2014_10/UserManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.554031 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2016_09/__init__.py
+-rw-r--r--   0        0        0      972 2022-10-20 12:42:45.196226 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2016_09/VolumeManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.727040 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2017_11/__init__.py
+-rw-r--r--   0        0        0     1297 2022-10-20 12:42:45.229220 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2017_11/IRM.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.581034 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2018_11/__init__.py
+-rw-r--r--   0        0        0     2198 2022-10-20 12:42:45.268226 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2018_11/SiteManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.847066 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2019_06/__init__.py
+-rw-r--r--   0        0        0     3615 2022-10-20 12:42:45.312236 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2019_06/UserManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.860082 tcsoa-0.9.1/tcsoa/gen/Internal/Administration/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.886054 tcsoa-0.9.1/tcsoa/gen/Internal/Ai/_2008_06/__init__.py
+-rw-r--r--   0        0        0     2306 2022-10-20 12:42:45.349233 tcsoa-0.9.1/tcsoa/gen/Internal/Ai/_2008_06/Ai.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.757046 tcsoa-0.9.1/tcsoa/gen/Internal/Ai/_2016_03/__init__.py
+-rw-r--r--   0        0        0     3067 2022-10-20 12:42:45.382240 tcsoa-0.9.1/tcsoa/gen/Internal/Ai/_2016_03/Ai.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.949068 tcsoa-0.9.1/tcsoa/gen/Internal/Ai/_2016_04/__init__.py
+-rw-r--r--   0        0        0      703 2022-10-20 12:42:45.408244 tcsoa-0.9.1/tcsoa/gen/Internal/Ai/_2016_04/Ai.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.837052 tcsoa-0.9.1/tcsoa/gen/Internal/Ai/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.810050 tcsoa-0.9.1/tcsoa/gen/Internal/AuditManager/_2012_09/__init__.py
+-rw-r--r--   0        0        0     1944 2022-10-20 12:42:17.443640 tcsoa-0.9.1/tcsoa/gen/Internal/AuditManager/_2012_09/ProcessHistoryManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.604032 tcsoa-0.9.1/tcsoa/gen/Internal/AuditManager/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.723044 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/__init__.py
+-rw-r--r--   0        0        0    10147 2022-10-20 12:42:00.713834 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/DataManagement.py
+-rw-r--r--   0        0        0     2650 2022-10-20 12:42:00.769824 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/Finder.py
+-rw-r--r--   0        0        0    14461 2022-10-20 12:42:00.951843 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/FullTextSearch.py
+-rw-r--r--   0        0        0    12834 2022-10-20 12:42:01.025862 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/LOV.py
+-rw-r--r--   0        0        0     2167 2022-10-20 12:42:01.064858 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/OrganizationManagement.py
+-rw-r--r--   0        0        0     1877 2022-10-20 12:42:01.107857 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/RequirementsManagement.py
+-rw-r--r--   0        0        0     2094 2022-10-20 12:42:01.141861 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/StructureSearch.py
+-rw-r--r--   0        0        0      784 2022-10-20 12:42:01.174866 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.993077 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2013_12/__init__.py
+-rw-r--r--   0        0        0     2311 2022-10-20 12:42:01.215863 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2013_12/DataManagement.py
+-rw-r--r--   0        0        0     2888 2022-10-20 12:42:01.243868 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2013_12/OrganizationManagement.py
+-rw-r--r--   0        0        0     6037 2022-10-20 12:42:01.288876 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2013_12/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.828056 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2014_11/__init__.py
+-rw-r--r--   0        0        0     2712 2022-10-20 12:42:01.320883 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2014_11/RequirementsManagement.py
+-rw-r--r--   0        0        0     7420 2022-10-20 12:42:01.397887 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2014_11/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.741045 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2015_03/__init__.py
+-rw-r--r--   0        0        0     4797 2022-10-20 12:42:01.437903 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2015_03/DataManagement.py
+-rw-r--r--   0        0        0     2036 2022-10-20 12:42:01.476901 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2015_03/FullTextSearch.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.819055 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2015_10/__init__.py
+-rw-r--r--   0        0        0     3481 2022-10-20 12:42:01.522904 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2015_10/DataManagement.py
+-rw-r--r--   0        0        0     6979 2022-10-20 12:42:01.582913 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2015_10/FullTextSearch.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.546029 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_03/__init__.py
+-rw-r--r--   0        0        0     7872 2022-10-20 12:42:01.642913 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_03/DataManagement.py
+-rw-r--r--   0        0        0    16769 2022-10-20 12:42:01.743928 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_03/Finder.py
+-rw-r--r--   0        0        0     2161 2022-10-20 12:42:01.774936 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_03/RequirementsManagement.py
+-rw-r--r--   0        0        0    12608 2022-10-20 12:42:01.860942 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_03/UiConfig.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.954086 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_04/__init__.py
+-rw-r--r--   0        0        0    14676 2022-10-20 12:42:01.956947 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_04/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.725040 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_12/__init__.py
+-rw-r--r--   0        0        0      968 2022-10-20 12:42:01.992961 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_12/AdvancedSearch.py
+-rw-r--r--   0        0        0     8292 2022-10-20 12:42:02.067964 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_12/DataManagement.py
+-rw-r--r--   0        0        0     4244 2022-10-20 12:42:02.104974 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_12/Finder.py
+-rw-r--r--   0        0        0     5616 2022-10-20 12:42:02.160968 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_12/RequirementsManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.628039 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_06/__init__.py
+-rw-r--r--   0        0        0    19075 2022-10-20 12:42:02.310991 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_06/DataManagement.py
+-rw-r--r--   0        0        0      818 2022-10-20 12:42:02.338989 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_06/EffectivityManagment.py
+-rw-r--r--   0        0        0    11744 2022-10-20 12:42:02.403994 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_06/Finder.py
+-rw-r--r--   0        0        0     1383 2022-10-20 12:42:02.438001 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_06/FullTextSearch.py
+-rw-r--r--   0        0        0     5300 2022-10-20 12:42:02.481999 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_06/RequirementsManagement.py
+-rw-r--r--   0        0        0      998 2022-10-20 12:42:02.510012 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_06/UiConfig.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.541030 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_12/__init__.py
+-rw-r--r--   0        0        0    14030 2022-10-20 12:42:02.593015 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_12/DataManagement.py
+-rw-r--r--   0        0        0     4364 2022-10-20 12:42:02.629020 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_12/Finder.py
+-rw-r--r--   0        0        0     2523 2022-10-20 12:42:02.671019 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_12/FullTextSearch.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.691046 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_05/__init__.py
+-rw-r--r--   0        0        0     9857 2022-10-20 12:42:02.745029 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_05/DataManagement.py
+-rw-r--r--   0        0        0     2327 2022-10-20 12:42:02.783034 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_05/FileMgmt.py
+-rw-r--r--   0        0        0     8632 2022-10-20 12:42:02.834046 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_05/Finder.py
+-rw-r--r--   0        0        0     6088 2022-10-20 12:42:02.869042 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_05/FullTextSearch.py
+-rw-r--r--   0        0        0     1176 2022-10-20 12:42:02.908049 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_05/TCXML.py
+-rw-r--r--   0        0        0     3702 2022-10-20 12:42:02.945058 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_05/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.981072 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_12/__init__.py
+-rw-r--r--   0        0        0     1273 2022-10-20 12:42:02.973061 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_12/Finder.py
+-rw-r--r--   0        0        0     1301 2022-10-20 12:42:03.005066 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_12/MultiSite.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.701045 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2019_06/__init__.py
+-rw-r--r--   0        0        0     4821 2022-10-20 12:42:03.051078 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2019_06/AdvancedSavedSearch.py
+-rw-r--r--   0        0        0    11263 2022-10-20 12:42:03.115076 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2019_06/Finder.py
+-rw-r--r--   0        0        0     2364 2022-10-20 12:42:03.158081 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2019_06/RequirementsManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.880064 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2019_12/__init__.py
+-rw-r--r--   0        0        0     4349 2022-10-20 12:42:03.214082 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2019_12/DataManagement.py
+-rw-r--r--   0        0        0     4772 2022-10-20 12:42:03.271094 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2019_12/Finder.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.800055 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2020_05/__init__.py
+-rw-r--r--   0        0        0     1652 2022-10-20 12:42:03.308091 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2020_05/DataManagement.py
+-rw-r--r--   0        0        0     1614 2022-10-20 12:42:03.341102 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2020_05/FileMgmt.py
+-rw-r--r--   0        0        0     3163 2022-10-20 12:42:03.376104 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2020_05/FullTextSearch.py
+-rw-r--r--   0        0        0     4921 2022-10-20 12:42:03.419110 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2020_05/UiConfig.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.927060 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2020_12/__init__.py
+-rw-r--r--   0        0        0     4299 2022-10-20 12:42:03.483116 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2020_12/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.687039 tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.984066 tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2007_01/__init__.py
+-rw-r--r--   0        0        0     1245 2022-10-20 12:42:45.441252 tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2007_01/DataModelManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.754044 tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2010_04/__init__.py
+-rw-r--r--   0        0        0     2808 2022-10-20 12:42:45.489254 tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2010_04/DataModelManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.617030 tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2010_09/__init__.py
+-rw-r--r--   0        0        0     1763 2022-10-20 12:42:45.522250 tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2010_09/DataModelManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.690037 tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2011_06/__init__.py
+-rw-r--r--   0        0        0      814 2022-10-20 12:42:45.549252 tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2011_06/DataModelManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.550029 tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2013_05/__init__.py
+-rw-r--r--   0        0        0     5023 2022-10-20 12:42:45.591255 tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2013_05/DynamicLOVQuery.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.957067 tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.688041 tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2008_03/__init__.py
+-rw-r--r--   0        0        0     1903 2022-10-20 12:42:45.630260 tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2008_03/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.993077 tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2008_05/__init__.py
+-rw-r--r--   0        0        0     4621 2022-10-20 12:42:45.672261 tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2008_05/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.925062 tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2008_06/__init__.py
+-rw-r--r--   0        0        0     5889 2022-10-20 12:42:45.744276 tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2008_06/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.010070 tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2010_04/__init__.py
+-rw-r--r--   0        0        0    13165 2022-10-20 12:42:45.831279 tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2010_04/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.718047 tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2013_05/__init__.py
+-rw-r--r--   0        0        0     7003 2022-10-20 12:42:45.903283 tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2013_05/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.681046 tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2017_05/__init__.py
+-rw-r--r--   0        0        0     7838 2022-10-20 12:42:45.976290 tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2017_05/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.978069 tcsoa-0.9.1/tcsoa/gen/Internal/Cad/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.665047 tcsoa-0.9.1/tcsoa/gen/Internal/Cae/_2011_06/__init__.py
+-rw-r--r--   0        0        0     2592 2022-10-20 12:42:46.003294 tcsoa-0.9.1/tcsoa/gen/Internal/Cae/_2011_06/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.592028 tcsoa-0.9.1/tcsoa/gen/Internal/Cae/_2013_05/__init__.py
+-rw-r--r--   0        0        0      767 2022-10-20 12:42:46.030300 tcsoa-0.9.1/tcsoa/gen/Internal/Cae/_2013_05/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.542030 tcsoa-0.9.1/tcsoa/gen/Internal/Cae/_2014_06/__init__.py
+-rw-r--r--   0        0        0     2233 2022-10-20 12:42:46.066308 tcsoa-0.9.1/tcsoa/gen/Internal/Cae/_2014_06/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.651040 tcsoa-0.9.1/tcsoa/gen/Internal/Cae/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.652035 tcsoa-0.9.1/tcsoa/gen/Internal/ChangeManagement/_2012_10/__init__.py
+-rw-r--r--   0        0        0     2948 2022-10-20 12:42:46.110311 tcsoa-0.9.1/tcsoa/gen/Internal/ChangeManagement/_2012_10/ChangeManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.808050 tcsoa-0.9.1/tcsoa/gen/Internal/ChangeManagement/_2015_03/__init__.py
+-rw-r--r--   0        0        0     7390 2022-10-20 12:42:46.172312 tcsoa-0.9.1/tcsoa/gen/Internal/ChangeManagement/_2015_03/ChangeManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.719040 tcsoa-0.9.1/tcsoa/gen/Internal/ChangeManagement/_2020_01/__init__.py
+-rw-r--r--   0        0        0     1464 2022-10-20 12:42:46.211323 tcsoa-0.9.1/tcsoa/gen/Internal/ChangeManagement/_2020_01/MassUpdate.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.959069 tcsoa-0.9.1/tcsoa/gen/Internal/ChangeManagement/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.945063 tcsoa-0.9.1/tcsoa/gen/Internal/Classification/_2009_10/__init__.py
+-rw-r--r--   0        0        0     2570 2022-10-20 12:42:46.253322 tcsoa-0.9.1/tcsoa/gen/Internal/Classification/_2009_10/Classification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.988072 tcsoa-0.9.1/tcsoa/gen/Internal/Classification/_2017_05/__init__.py
+-rw-r--r--   0        0        0     5883 2022-10-20 12:42:46.298328 tcsoa-0.9.1/tcsoa/gen/Internal/Classification/_2017_05/Classification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.937067 tcsoa-0.9.1/tcsoa/gen/Internal/Classification/_2018_11/__init__.py
+-rw-r--r--   0        0        0     2172 2022-10-20 12:42:46.335326 tcsoa-0.9.1/tcsoa/gen/Internal/Classification/_2018_11/Classification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.900053 tcsoa-0.9.1/tcsoa/gen/Internal/Classification/_2020_04/__init__.py
+-rw-r--r--   0        0        0     7976 2022-10-20 12:42:46.400335 tcsoa-0.9.1/tcsoa/gen/Internal/Classification/_2020_04/Classification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.796046 tcsoa-0.9.1/tcsoa/gen/Internal/Classification/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.779053 tcsoa-0.9.1/tcsoa/gen/Internal/ConfigFilterCriteria/_2013_12/__init__.py
+-rw-r--r--   0        0        0      805 2022-10-20 12:42:17.477662 tcsoa-0.9.1/tcsoa/gen/Internal/ConfigFilterCriteria/_2013_12/VariantManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.717049 tcsoa-0.9.1/tcsoa/gen/Internal/ConfigFilterCriteria/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.588032 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2014_06/__init__.py
+-rw-r--r--   0        0        0    66424 2022-10-20 12:42:13.348173 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2014_06/ConfiguratorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.611029 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2014_12/__init__.py
+-rw-r--r--   0        0        0     6953 2022-10-20 12:42:13.425214 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2014_12/ConfiguratorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.850060 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2015_03/__init__.py
+-rw-r--r--   0        0        0     4034 2022-10-20 12:42:13.463190 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2015_03/ConfiguratorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.006070 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2015_10/__init__.py
+-rw-r--r--   0        0        0    25096 2022-10-20 12:42:13.638206 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2015_10/ConfiguratorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.986071 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2016_09/__init__.py
+-rw-r--r--   0        0        0     3581 2022-10-20 12:42:13.692217 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2016_09/ConfiguratorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.610029 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2017_11/__init__.py
+-rw-r--r--   0        0        0     4325 2022-10-20 12:42:13.732241 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2017_11/ConfiguratorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.790046 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2018_06/__init__.py
+-rw-r--r--   0        0        0     9718 2022-10-20 12:42:13.825222 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2018_06/ConfiguratorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.808050 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2018_11/__init__.py
+-rw-r--r--   0        0        0     1118 2022-10-20 12:42:13.859224 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2018_11/ConfiguratorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.567031 tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.900053 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2007_01/__init__.py
+-rw-r--r--   0        0        0     3949 2022-10-20 12:42:46.457338 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2007_01/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.656040 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2007_06/__init__.py
+-rw-r--r--   0        0        0     4699 2022-10-20 12:42:46.531347 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2007_06/ProjectLevelSecurity.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.692046 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2007_09/__init__.py
+-rw-r--r--   0        0        0     1390 2022-10-20 12:42:46.569347 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2007_09/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.861060 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2008_06/__init__.py
+-rw-r--r--   0        0        0     4549 2022-10-20 12:42:46.633371 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2008_06/DataManagement.py
+-rw-r--r--   0        0        0     7569 2022-10-20 12:42:46.721371 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2008_06/DispatcherManagement.py
+-rw-r--r--   0        0        0     9953 2022-10-20 12:42:46.805372 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2008_06/FileManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.876055 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2009_10/__init__.py
+-rw-r--r--   0        0        0     1765 2022-10-20 12:42:46.841379 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2009_10/Thumbnail.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.696047 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2010_04/__init__.py
+-rw-r--r--   0        0        0     1235 2022-10-20 12:42:46.872391 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2010_04/DataManagement.py
+-rw-r--r--   0        0        0     2042 2022-10-20 12:42:46.910380 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2010_04/ProjectLevelSecurity.py
+-rw-r--r--   0        0        0     1198 2022-10-20 12:42:46.944382 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2010_04/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.725040 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2010_09/__init__.py
+-rw-r--r--   0        0        0     2858 2022-10-20 12:42:46.998386 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2010_09/DataManagement.py
+-rw-r--r--   0        0        0     1021 2022-10-20 12:42:47.025405 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2010_09/FileManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.635041 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2011_06/__init__.py
+-rw-r--r--   0        0        0     1297 2022-10-20 12:42:47.076394 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2011_06/ICT.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.944079 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2012_02/__init__.py
+-rw-r--r--   0        0        0     2490 2022-10-20 12:42:47.113407 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2012_02/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.973071 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2012_09/__init__.py
+-rw-r--r--   0        0        0     1836 2022-10-20 12:42:47.140407 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2012_09/Envelope.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.756046 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2012_10/__init__.py
+-rw-r--r--   0        0        0     3420 2022-10-20 12:42:47.182412 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2012_10/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.545030 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2013_05/__init__.py
+-rw-r--r--   0        0        0     1957 2022-10-20 12:42:47.219410 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2013_05/Licensing.py
+-rw-r--r--   0        0        0     4651 2022-10-20 12:42:47.272419 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2013_05/PresentationManagement.py
+-rw-r--r--   0        0        0     1071 2022-10-20 12:42:47.303422 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2013_05/ProjectLevelSecurity.py
+-rw-r--r--   0        0        0      882 2022-10-20 12:42:47.331428 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2013_05/Thumbnail.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.647036 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2014_10/__init__.py
+-rw-r--r--   0        0        0     1951 2022-10-20 12:42:47.367426 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2014_10/FileManagement.py
+-rw-r--r--   0        0        0     1273 2022-10-20 12:42:47.395427 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2014_10/Licensing.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.580034 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2016_10/__init__.py
+-rw-r--r--   0        0        0     2822 2022-10-20 12:42:47.430428 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2016_10/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.566032 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2017_05/__init__.py
+-rw-r--r--   0        0        0     1044 2022-10-20 12:42:47.457440 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2017_05/FileManagement.py
+-rw-r--r--   0        0        0     5339 2022-10-20 12:42:47.502439 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2017_05/PresentationManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.789043 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2017_11/__init__.py
+-rw-r--r--   0        0        0     4694 2022-10-20 12:42:47.538438 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2017_11/DataManagement.py
+-rw-r--r--   0        0        0     5855 2022-10-20 12:42:47.601442 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2017_11/LogicalObject.py
+-rw-r--r--   0        0        0     1749 2022-10-20 12:42:47.641449 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2017_11/Type.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.000074 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2018_06/__init__.py
+-rw-r--r--   0        0        0     5176 2022-10-20 12:42:47.691451 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2018_06/LogicalObject.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.672047 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2018_11/__init__.py
+-rw-r--r--   0        0        0     1209 2022-10-20 12:42:47.724459 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2018_11/FileManagement.py
+-rw-r--r--   0        0        0     2261 2022-10-20 12:42:47.763460 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2018_11/LogicalObject.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.584030 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2018_12/__init__.py
+-rw-r--r--   0        0        0     1647 2022-10-20 12:42:47.792462 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2018_12/Licensing.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.841051 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2020_01/__init__.py
+-rw-r--r--   0        0        0     7334 2022-10-20 12:42:47.835465 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2020_01/ActiveModeler.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.728040 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2020_04/__init__.py
+-rw-r--r--   0        0        0     1965 2022-10-20 12:42:47.867471 tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2020_04/LogicalObject.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.657040 tcsoa-0.9.1/tcsoa/gen/Internal/Core/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.847066 tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2011_06/__init__.py
+-rw-r--r--   0        0        0     4042 2022-10-20 12:42:17.551644 tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2011_06/DebugLogging.py
+-rw-r--r--   0        0        0    11293 2022-10-20 12:42:17.649658 tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2011_06/DebugMonitor.py
+-rw-r--r--   0        0        0      638 2022-10-20 12:42:17.676661 tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2011_06/PerformanceMonitor.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.544029 tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2014_06/__init__.py
+-rw-r--r--   0        0        0     3244 2022-10-20 12:42:17.721665 tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2014_06/JournalBasedTesting.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.648033 tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2015_07/__init__.py
+-rw-r--r--   0        0        0      417 2022-10-20 12:42:17.751678 tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2015_07/DebugLogging.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.801055 tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2015_10/__init__.py
+-rw-r--r--   0        0        0      772 2022-10-20 12:42:17.780675 tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2015_10/JournalBasedTesting.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.561031 tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2019_06/__init__.py
+-rw-r--r--   0        0        0      703 2022-10-20 12:42:17.809675 tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2019_06/DebugLogging.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.633041 tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.011070 tcsoa-0.9.1/tcsoa/gen/Internal/DocMgmtAw/_2019_06/__init__.py
+-rw-r--r--   0        0        0     1133 2022-10-20 12:42:16.296456 tcsoa-0.9.1/tcsoa/gen/Internal/DocMgmtAw/_2019_06/DocMgmt.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.812049 tcsoa-0.9.1/tcsoa/gen/Internal/DocMgmtAw/_2019_12/__init__.py
+-rw-r--r--   0        0        0      735 2022-10-20 12:42:16.325466 tcsoa-0.9.1/tcsoa/gen/Internal/DocMgmtAw/_2019_12/DocMgmt.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.951068 tcsoa-0.9.1/tcsoa/gen/Internal/DocMgmtAw/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.797053 tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0     2010 2022-10-20 12:42:47.905475 tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/_2008_06/DispatcherManagement.py
+-rw-r--r--   0        0        0      554 2022-10-20 12:42:47.951477 tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/_2008_06/DocumentControl.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.925062 tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/_2013_05/__init__.py
+-rw-r--r--   0        0        0      712 2022-10-20 12:42:47.983492 tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/_2013_05/DigitalSignature.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.921064 tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/_2013_12/__init__.py
+-rw-r--r--   0        0        0      757 2022-10-20 12:42:48.009488 tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/_2013_12/Markup.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.742044 tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/_2020_12/__init__.py
+-rw-r--r--   0        0        0     1628 2022-10-20 12:42:48.041486 tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/_2020_12/AttributeExchange.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.620029 tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.630037 tcsoa-0.9.1/tcsoa/gen/Internal/EntCba/_2019_12/__init__.py
+-rw-r--r--   0        0        0      821 2022-10-20 12:42:00.244774 tcsoa-0.9.1/tcsoa/gen/Internal/EntCba/_2019_12/Alignments.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.746044 tcsoa-0.9.1/tcsoa/gen/Internal/EntCba/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.953082 tcsoa-0.9.1/tcsoa/gen/Internal/Gdis/_2006_03/__init__.py
+-rw-r--r--   0        0        0      859 2022-10-20 12:42:48.074487 tcsoa-0.9.1/tcsoa/gen/Internal/Gdis/_2006_03/Reporting.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.668044 tcsoa-0.9.1/tcsoa/gen/Internal/Gdis/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.696047 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2007_06/__init__.py
+-rw-r--r--   0        0        0     2313 2022-10-20 12:42:48.111491 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2007_06/Briefcase.py
+-rw-r--r--   0        0        0     6894 2022-10-20 12:42:48.187500 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2007_06/ImportExport.py
+-rw-r--r--   0        0        0     3167 2022-10-20 12:42:48.245511 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2007_06/Synchronizer.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.767045 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2008_06/__init__.py
+-rw-r--r--   0        0        0     2028 2022-10-20 12:42:48.282517 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2008_06/Synchronizer.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.663035 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2010_02/__init__.py
+-rw-r--r--   0        0        0     1256 2022-10-20 12:42:48.320508 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2010_02/LowlevelOwnershipTransfer.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.638044 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2017_05/__init__.py
+-rw-r--r--   0        0        0      993 2022-10-20 12:42:48.347511 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2017_05/ImportExport.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.985066 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2018_11/__init__.py
+-rw-r--r--   0        0        0     3560 2022-10-20 12:42:48.385516 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2018_11/Briefcase.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.874054 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2020_01/__init__.py
+-rw-r--r--   0        0        0     4886 2022-10-20 12:42:48.450523 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2020_01/Briefcase.py
+-rw-r--r--   0        0        0     2734 2022-10-20 12:42:48.492528 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2020_01/OwnershipRecovery.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.843052 tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.864060 tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2017_06/__init__.py
+-rw-r--r--   0        0        0     2157 2022-10-20 12:42:18.932771 tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2017_06/Author.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.722046 tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2017_12/__init__.py
+-rw-r--r--   0        0        0    14621 2022-10-20 12:42:19.044795 tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2017_12/Author.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.641039 tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2018_05/__init__.py
+-rw-r--r--   0        0        0    17309 2022-10-20 12:42:19.158820 tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2018_05/Classification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.922066 tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2018_12/__init__.py
+-rw-r--r--   0        0        0     6929 2022-10-20 12:42:19.216807 tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2018_12/Classification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.930066 tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2019_06/__init__.py
+-rw-r--r--   0        0        0     1098 2022-10-20 12:42:19.244803 tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2019_06/Classification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.913065 tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2019_12/__init__.py
+-rw-r--r--   0        0        0     5861 2022-10-20 12:42:19.293805 tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2019_12/Classification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.799058 tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.709040 tcsoa-0.9.1/tcsoa/gen/Internal/ImportExport/_2010_04/__init__.py
+-rw-r--r--   0        0        0     5269 2022-10-20 12:42:48.542533 tcsoa-0.9.1/tcsoa/gen/Internal/ImportExport/_2010_04/L10NImportExport.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.998072 tcsoa-0.9.1/tcsoa/gen/Internal/ImportExport/_2017_11/__init__.py
+-rw-r--r--   0        0        0     3735 2022-10-20 12:42:48.585543 tcsoa-0.9.1/tcsoa/gen/Internal/ImportExport/_2017_11/FileImportExport.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.807048 tcsoa-0.9.1/tcsoa/gen/Internal/ImportExport/_2018_06/__init__.py
+-rw-r--r--   0        0        0     3102 2022-10-20 12:42:48.611535 tcsoa-0.9.1/tcsoa/gen/Internal/ImportExport/_2018_06/L10NImportExport.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.716044 tcsoa-0.9.1/tcsoa/gen/Internal/ImportExport/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.953082 tcsoa-0.9.1/tcsoa/gen/Internal/Integration/_2007_06/__init__.py
+-rw-r--r--   0        0        0      441 2022-10-20 12:42:48.638540 tcsoa-0.9.1/tcsoa/gen/Internal/Integration/_2007_06/IntegrationManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.923067 tcsoa-0.9.1/tcsoa/gen/Internal/Integration/_2008_06/__init__.py
+-rw-r--r--   0        0        0      610 2022-10-20 12:42:48.665543 tcsoa-0.9.1/tcsoa/gen/Internal/Integration/_2008_06/IntegrationManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.855059 tcsoa-0.9.1/tcsoa/gen/Internal/Integration/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.804052 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2008_12/__init__.py
+-rw-r--r--   0        0        0     1092 2022-10-20 12:42:48.698548 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2008_12/Core.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.860082 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2011_12/__init__.py
+-rw-r--r--   0        0        0     2462 2022-10-20 12:42:48.743555 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2011_12/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.748043 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2012_09/__init__.py
+-rw-r--r--   0        0        0     3116 2022-10-20 12:42:48.789556 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2012_09/StructureSearch.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.852060 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2014_06/__init__.py
+-rw-r--r--   0        0        0     3728 2022-10-20 12:42:48.831566 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2014_06/DataManagement.py
+-rw-r--r--   0        0        0     2070 2022-10-20 12:42:48.864569 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2014_06/IPAManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.555030 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2014_12/__init__.py
+-rw-r--r--   0        0        0     1033 2022-10-20 12:42:48.896567 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2014_12/IPAManagement.py
+-rw-r--r--   0        0        0     6303 2022-10-20 12:42:48.952575 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2014_12/Model.py
+-rw-r--r--   0        0        0     2439 2022-10-20 12:42:48.987581 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2014_12/ResourceManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.708044 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2015_03/__init__.py
+-rw-r--r--   0        0        0     6071 2022-10-20 12:42:49.041578 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2015_03/Attachments.py
+-rw-r--r--   0        0        0     3374 2022-10-20 12:42:49.089588 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2015_03/ResourceManagement.py
+-rw-r--r--   0        0        0    11116 2022-10-20 12:42:49.172590 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2015_03/StructureManagement.py
+-rw-r--r--   0        0        0     3004 2022-10-20 12:42:49.210600 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2015_03/StructureSearch.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.612029 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2015_10/__init__.py
+-rw-r--r--   0        0        0    10614 2022-10-20 12:42:49.306603 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2015_10/StructureManagement.py
+-rw-r--r--   0        0        0     3062 2022-10-20 12:42:49.352625 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2015_10/StructureSearch.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.892058 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2016_09/__init__.py
+-rw-r--r--   0        0        0     5061 2022-10-20 12:42:49.411618 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2016_09/DataManagement.py
+-rw-r--r--   0        0        0     3872 2022-10-20 12:42:49.452621 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2016_09/IPAManagement.py
+-rw-r--r--   0        0        0     4752 2022-10-20 12:42:49.487619 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2016_09/ResourceManagement.py
+-rw-r--r--   0        0        0     9531 2022-10-20 12:42:49.561624 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2016_09/StructureManagement.py
+-rw-r--r--   0        0        0     1904 2022-10-20 12:42:49.598639 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2016_09/StructureSearch.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.975074 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2017_05/__init__.py
+-rw-r--r--   0        0        0     3398 2022-10-20 12:42:49.652643 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2017_05/DataManagement.py
+-rw-r--r--   0        0        0      169 2022-10-20 12:42:49.675660 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2017_05/ImportExport.py
+-rw-r--r--   0        0        0     4083 2022-10-20 12:42:49.724651 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2017_05/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.579033 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2017_11/__init__.py
+-rw-r--r--   0        0        0     1118 2022-10-20 12:42:49.757645 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2017_11/ResourceManagement.py
+-rw-r--r--   0        0        0     4153 2022-10-20 12:42:49.807657 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2017_11/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.842051 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2018_11/__init__.py
+-rw-r--r--   0        0        0     1090 2022-10-20 12:42:49.838649 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2018_11/ResourceManagement.py
+-rw-r--r--   0        0        0    10480 2022-10-20 12:42:49.926669 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2018_11/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.650034 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2019_06/__init__.py
+-rw-r--r--   0        0        0     2429 2022-10-20 12:42:49.964683 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2019_06/ClosureRuleEditor.py
+-rw-r--r--   0        0        0     1678 2022-10-20 12:42:50.002668 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2019_06/ResourceManagement.py
+-rw-r--r--   0        0        0     4007 2022-10-20 12:42:50.038678 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2019_06/StructureSearch.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.753044 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2020_01/__init__.py
+-rw-r--r--   0        0        0     3547 2022-10-20 12:42:50.071681 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2020_01/DataManagement.py
+-rw-r--r--   0        0        0     5256 2022-10-20 12:42:50.111691 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2020_01/StructureSearch.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.699049 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2020_04/__init__.py
+-rw-r--r--   0        0        0     1288 2022-10-20 12:42:50.140701 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2020_04/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.862059 tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.894059 tcsoa-0.9.1/tcsoa/gen/Internal/Mmv/_2012_09/__init__.py
+-rw-r--r--   0        0        0    11263 2022-10-20 12:42:17.928679 tcsoa-0.9.1/tcsoa/gen/Internal/Mmv/_2012_09/SpatialStructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.726040 tcsoa-0.9.1/tcsoa/gen/Internal/Mmv/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.012069 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2007_06/__init__.py
+-rw-r--r--   0        0        0     9210 2022-10-20 12:42:50.225691 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2007_06/ObjectDirectory.py
+-rw-r--r--   0        0        0    49922 2022-10-20 12:42:50.672736 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2007_06/RemoteOperation.py
+-rw-r--r--   0        0        0     6322 2022-10-20 12:42:50.730745 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2007_06/TcEntObjectDirectory.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.583037 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2011_06/__init__.py
+-rw-r--r--   0        0        0     1673 2022-10-20 12:42:51.215788 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2011_06/ImportExportAsync.py
+-rw-r--r--   0        0        0     5192 2022-10-20 12:42:50.776742 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2011_06/ObjectDirectory.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.941066 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2012_02/__init__.py
+-rw-r--r--   0        0        0     5398 2022-10-20 12:42:50.832742 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2012_02/ObjectDirectory.py
+-rw-r--r--   0        0        0    42494 2022-10-20 12:42:51.182786 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2012_02/RemoteOperation.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.592028 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2017_11/__init__.py
+-rw-r--r--   0        0        0     1504 2022-10-20 12:42:51.253787 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2017_11/ArchiveRestore.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.682047 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2018_06/__init__.py
+-rw-r--r--   0        0        0     1262 2022-10-20 12:42:51.287789 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2018_06/Search.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.656040 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2020_12/__init__.py
+-rw-r--r--   0        0        0     2749 2022-10-20 12:42:51.319787 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2020_12/ImportExportTCXML.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.624029 tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.638044 tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2014_10/__init__.py
+-rw-r--r--   0        0        0      699 2022-10-20 12:42:17.954682 tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2014_10/SubscriptionManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.667044 tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2015_03/__init__.py
+-rw-r--r--   0        0        0      915 2022-10-20 12:42:17.981705 tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2015_03/MessageManagement.py
+-rw-r--r--   0        0        0    14209 2022-10-20 12:42:18.075704 tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2015_03/SubscriptionManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.871054 tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2015_10/__init__.py
+-rw-r--r--   0        0        0      342 2022-10-20 12:42:18.102700 tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2015_10/MessageManagement.py
+-rw-r--r--   0        0        0     5046 2022-10-20 12:42:18.168703 tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2015_10/SubscriptionManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.607029 tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2017_11/__init__.py
+-rw-r--r--   0        0        0     1436 2022-10-20 12:42:18.200713 tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2017_11/SubscriptionManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.783052 tcsoa-0.9.1/tcsoa/gen/Internal/Notification/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.648033 tcsoa-0.9.1/tcsoa/gen/Internal/OccMgmt/_2020_05/__init__.py
+-rw-r--r--   0        0        0     5358 2022-10-20 12:42:03.562120 tcsoa-0.9.1/tcsoa/gen/Internal/OccMgmt/_2020_05/ImportExport.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.901069 tcsoa-0.9.1/tcsoa/gen/Internal/OccMgmt/_2020_12/__init__.py
+-rw-r--r--   0        0        0     6880 2022-10-20 12:42:03.613124 tcsoa-0.9.1/tcsoa/gen/Internal/OccMgmt/_2020_12/EffectivityManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.574032 tcsoa-0.9.1/tcsoa/gen/Internal/OccMgmt/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.693045 tcsoa-0.9.1/tcsoa/gen/Internal/ProductConfiguratorAw/_2017_12/__init__.py
+-rw-r--r--   0        0        0     9850 2022-10-20 12:42:30.359847 tcsoa-0.9.1/tcsoa/gen/Internal/ProductConfiguratorAw/_2017_12/ConfiguratorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.983065 tcsoa-0.9.1/tcsoa/gen/Internal/ProductConfiguratorAw/_2018_05/__init__.py
+-rw-r--r--   0        0        0    23263 2022-10-20 12:42:30.490860 tcsoa-0.9.1/tcsoa/gen/Internal/ProductConfiguratorAw/_2018_05/ConfiguratorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.928070 tcsoa-0.9.1/tcsoa/gen/Internal/ProductConfiguratorAw/_2020_05/__init__.py
+-rw-r--r--   0        0        0     6719 2022-10-20 12:42:30.543855 tcsoa-0.9.1/tcsoa/gen/Internal/ProductConfiguratorAw/_2020_05/ConfiguratorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.591030 tcsoa-0.9.1/tcsoa/gen/Internal/ProductConfiguratorAw/_2020_12/__init__.py
+-rw-r--r--   0        0        0    29941 2022-10-20 12:42:30.669865 tcsoa-0.9.1/tcsoa/gen/Internal/ProductConfiguratorAw/_2020_12/ConfiguratorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.768045 tcsoa-0.9.1/tcsoa/gen/Internal/ProductConfiguratorAw/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.850060 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2007_01/__init__.py
+-rw-r--r--   0        0        0     6870 2022-10-20 12:42:51.393799 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2007_01/ScheduleManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.774045 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2007_06/__init__.py
+-rw-r--r--   0        0        0     7733 2022-10-20 12:42:51.475803 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2007_06/ScheduleManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.743042 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0     5765 2022-10-20 12:42:51.546816 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2008_06/ScheduleManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.579033 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2009_10/__init__.py
+-rw-r--r--   0        0        0     6185 2022-10-20 12:42:51.634822 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2009_10/ScheduleManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.787047 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2010_04/__init__.py
+-rw-r--r--   0        0        0     1337 2022-10-20 12:42:51.668820 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2010_04/ScheduleManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.775046 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2011_06/__init__.py
+-rw-r--r--   0        0        0     4749 2022-10-20 12:42:51.722833 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2011_06/ScheduleManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.568034 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2012_02/__init__.py
+-rw-r--r--   0        0        0     1220 2022-10-20 12:42:51.754834 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2012_02/ScheduleManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.595030 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2014_10/__init__.py
+-rw-r--r--   0        0        0     3956 2022-10-20 12:42:51.793844 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2014_10/ScheduleManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.548030 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.695048 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagementAw/_2019_12/__init__.py
+-rw-r--r--   0        0        0     8951 2022-10-20 12:42:32.799072 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagementAw/_2019_12/ScheduleManagementAw.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.666046 tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagementAw/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.683038 tcsoa-0.9.1/tcsoa/gen/Internal/Query/_2008_06/__init__.py
+-rw-r--r--   0        0        0     1650 2022-10-20 12:42:51.831853 tcsoa-0.9.1/tcsoa/gen/Internal/Query/_2008_06/Finder.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.695048 tcsoa-0.9.1/tcsoa/gen/Internal/Query/_2012_02/__init__.py
+-rw-r--r--   0        0        0     5150 2022-10-20 12:42:51.880852 tcsoa-0.9.1/tcsoa/gen/Internal/Query/_2012_02/SavedQuery.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.878055 tcsoa-0.9.1/tcsoa/gen/Internal/Query/_2013_05/__init__.py
+-rw-r--r--   0        0        0     4842 2022-10-20 12:42:51.920853 tcsoa-0.9.1/tcsoa/gen/Internal/Query/_2013_05/SavedQuery.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.816052 tcsoa-0.9.1/tcsoa/gen/Internal/Query/_2014_10/__init__.py
+-rw-r--r--   0        0        0     4575 2022-10-20 12:42:51.958850 tcsoa-0.9.1/tcsoa/gen/Internal/Query/_2014_10/SavedQuery.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.830051 tcsoa-0.9.1/tcsoa/gen/Internal/Query/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.875078 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2007_06/__init__.py
+-rw-r--r--   0        0        0     2229 2022-10-20 12:42:51.997860 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2007_06/VariantManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.882056 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2007_09/__init__.py
+-rw-r--r--   0        0        0     2500 2022-10-20 12:42:52.040863 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2007_09/VariantManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.927060 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2008_03/__init__.py
+-rw-r--r--   0        0        0     2244 2022-10-20 12:42:52.080869 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2008_03/VariantManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.745043 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2009_01/__init__.py
+-rw-r--r--   0        0        0     8788 2022-10-20 12:42:52.185878 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2009_01/VariantManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.578033 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2009_04/__init__.py
+-rw-r--r--   0        0        0     4949 2022-10-20 12:42:52.243876 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2009_04/VariantManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.744043 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2009_05/__init__.py
+-rw-r--r--   0        0        0     2339 2022-10-20 12:42:52.284880 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2009_05/VariantManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.858074 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2010_04/__init__.py
+-rw-r--r--   0        0        0     9177 2022-10-20 12:42:52.377894 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2010_04/VariantManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.867053 tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.602028 tcsoa-0.9.1/tcsoa/gen/Internal/Reports/_2007_06/__init__.py
+-rw-r--r--   0        0        0    10316 2022-10-20 12:42:52.493899 tcsoa-0.9.1/tcsoa/gen/Internal/Reports/_2007_06/BOMRollup.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.809054 tcsoa-0.9.1/tcsoa/gen/Internal/Reports/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.008068 tcsoa-0.9.1/tcsoa/gen/Internal/Requirementsmanagement/_2009_10/__init__.py
+-rw-r--r--   0        0        0     3154 2022-10-20 12:42:52.532901 tcsoa-0.9.1/tcsoa/gen/Internal/Requirementsmanagement/_2009_10/RequirementsManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.811050 tcsoa-0.9.1/tcsoa/gen/Internal/Requirementsmanagement/_2012_02/__init__.py
+-rw-r--r--   0        0        0     3465 2022-10-20 12:42:52.572908 tcsoa-0.9.1/tcsoa/gen/Internal/Requirementsmanagement/_2012_02/RequirementsManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.543024 tcsoa-0.9.1/tcsoa/gen/Internal/Requirementsmanagement/_2012_10/__init__.py
+-rw-r--r--   0        0        0     3809 2022-10-20 12:42:52.621919 tcsoa-0.9.1/tcsoa/gen/Internal/Requirementsmanagement/_2012_10/RequirementsManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.744043 tcsoa-0.9.1/tcsoa/gen/Internal/Requirementsmanagement/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.574032 tcsoa-0.9.1/tcsoa/gen/Internal/RevRuleMgmt/_2019_12/__init__.py
+-rw-r--r--   0        0        0     7535 2022-10-20 12:42:03.683132 tcsoa-0.9.1/tcsoa/gen/Internal/RevRuleMgmt/_2019_12/RevisionRuleAdministration.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.995072 tcsoa-0.9.1/tcsoa/gen/Internal/RevRuleMgmt/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.769044 tcsoa-0.9.1/tcsoa/gen/Internal/Search/_2020_12/__init__.py
+-rw-r--r--   0        0        0    16853 2022-10-20 12:42:03.773146 tcsoa-0.9.1/tcsoa/gen/Internal/Search/_2020_12/SearchFolder.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.832057 tcsoa-0.9.1/tcsoa/gen/Internal/Search/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.590027 tcsoa-0.9.1/tcsoa/gen/Internal/Security/_2017_12/__init__.py
+-rw-r--r--   0        0        0     5755 2022-10-20 12:41:58.603592 tcsoa-0.9.1/tcsoa/gen/Internal/Security/_2017_12/AwLicensing.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.635041 tcsoa-0.9.1/tcsoa/gen/Internal/Security/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.714041 tcsoa-0.9.1/tcsoa/gen/Internal/Structure/_2020_12/__init__.py
+-rw-r--r--   0        0        0     7965 2022-10-20 12:42:00.307768 tcsoa-0.9.1/tcsoa/gen/Internal/Structure/_2020_12/WhereUsed.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.576032 tcsoa-0.9.1/tcsoa/gen/Internal/Structure/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.994073 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2007_06/__init__.py
+-rw-r--r--   0        0        0     1679 2022-10-20 12:42:52.664919 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2007_06/GlobalAlternate.py
+-rw-r--r--   0        0        0     1210 2022-10-20 12:42:52.696929 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2007_06/PublishByLink.py
+-rw-r--r--   0        0        0     1430 2022-10-20 12:42:52.733929 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2007_06/Restructure.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.942067 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2007_12/__init__.py
+-rw-r--r--   0        0        0     2894 2022-10-20 12:42:52.783924 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2007_12/BrokenLinks.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.645038 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2008_03/__init__.py
+-rw-r--r--   0        0        0      738 2022-10-20 12:42:52.812929 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2008_03/Structure.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.007066 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2008_05/__init__.py
+-rw-r--r--   0        0        0      504 2022-10-20 12:42:52.842931 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2008_05/Restructure.py
+-rw-r--r--   0        0        0      407 2022-10-20 12:42:52.868941 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2008_05/Structure.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.712045 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0     2215 2022-10-20 12:42:52.909940 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2008_06/Structure.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.946062 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2009_10/__init__.py
+-rw-r--r--   0        0        0     2732 2022-10-20 12:42:52.946942 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2009_10/EffectivitiesManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.678047 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2010_04/__init__.py
+-rw-r--r--   0        0        0     3093 2022-10-20 12:42:52.989946 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2010_04/BOMMarkup.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.715046 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2010_09/__init__.py
+-rw-r--r--   0        0        0      841 2022-10-20 12:42:53.015949 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2010_09/Structure.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.643038 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2011_06/__init__.py
+-rw-r--r--   0        0        0     7566 2022-10-20 12:42:53.118965 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2011_06/IncrementalChange.py
+-rw-r--r--   0        0        0     4705 2022-10-20 12:42:53.170964 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2011_06/Structure.py
+-rw-r--r--   0        0        0     7474 2022-10-20 12:42:53.252978 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2011_06/VariantManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.946062 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2012_02/__init__.py
+-rw-r--r--   0        0        0     6080 2022-10-20 12:42:53.314015 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2012_02/StructureVerification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.629037 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2012_09/__init__.py
+-rw-r--r--   0        0        0     1406 2022-10-20 12:42:53.346987 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2012_09/StructureVerification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.721045 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2013_05/__init__.py
+-rw-r--r--   0        0        0    10741 2022-10-20 12:42:53.420986 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2013_05/StructureExpansionLite.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.758045 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2013_12/__init__.py
+-rw-r--r--   0        0        0     3123 2022-10-20 12:42:53.459998 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2013_12/StructureExpansionLite.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.952067 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2014_12/__init__.py
+-rw-r--r--   0        0        0     3730 2022-10-20 12:42:53.511001 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2014_12/BrokenLinks.py
+-rw-r--r--   0        0        0     1306 2022-10-20 12:42:53.539004 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2014_12/Restructure.py
+-rw-r--r--   0        0        0    29349 2022-10-20 12:42:53.692016 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2014_12/StructureVerification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.936066 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2015_10/__init__.py
+-rw-r--r--   0        0        0      997 2022-10-20 12:42:53.719040 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2015_10/VariantManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.907054 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2016_03/__init__.py
+-rw-r--r--   0        0        0     6060 2022-10-20 12:42:53.784020 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2016_03/StructureVerification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.649034 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2016_10/__init__.py
+-rw-r--r--   0        0        0     4284 2022-10-20 12:42:53.842031 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2016_10/Effectivity.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.867053 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2017_05/__init__.py
+-rw-r--r--   0        0        0    10110 2022-10-20 12:42:53.906029 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2017_05/StructureExpansionLite.py
+-rw-r--r--   0        0        0     1542 2022-10-20 12:42:53.938039 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2017_05/StructureLiteConversion.py
+-rw-r--r--   0        0        0     3323 2022-10-20 12:42:53.985039 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2017_05/StructureVerification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.549029 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2018_11/__init__.py
+-rw-r--r--   0        0        0     1427 2022-10-20 12:42:54.020051 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2018_11/MassUpdate.py
+-rw-r--r--   0        0        0     3634 2022-10-20 12:42:54.068072 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2018_11/StructureVerification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.002064 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2020_05/__init__.py
+-rw-r--r--   0        0        0     7787 2022-10-20 12:42:54.124066 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2020_05/RevisionRuleAdministration.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.901069 tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.836052 tcsoa-0.9.1/tcsoa/gen/Internal/TCXMLImportExport/_2020_12/__init__.py
+-rw-r--r--   0        0        0     4635 2022-10-20 12:42:03.812144 tcsoa-0.9.1/tcsoa/gen/Internal/TCXMLImportExport/_2020_12/Briefcase.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.793051 tcsoa-0.9.1/tcsoa/gen/Internal/TCXMLImportExport/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.783052 tcsoa-0.9.1/tcsoa/gen/Internal/Translation/_2007_06/__init__.py
+-rw-r--r--   0        0        0     6924 2022-10-20 12:42:54.197065 tcsoa-0.9.1/tcsoa/gen/Internal/Translation/_2007_06/TranslationManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.830051 tcsoa-0.9.1/tcsoa/gen/Internal/Translation/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.703047 tcsoa-0.9.1/tcsoa/gen/Internal/UiConfig/_2014_11/__init__.py
+-rw-r--r--   0        0        0     1405 2022-10-20 12:42:18.236714 tcsoa-0.9.1/tcsoa/gen/Internal/UiConfig/_2014_11/UiConfig.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.835050 tcsoa-0.9.1/tcsoa/gen/Internal/UiConfig/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.872054 tcsoa-0.9.1/tcsoa/gen/Internal/Validation/_2007_06/__init__.py
+-rw-r--r--   0        0        0    18115 2022-10-20 12:42:54.321101 tcsoa-0.9.1/tcsoa/gen/Internal/Validation/_2007_06/Validation.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.605029 tcsoa-0.9.1/tcsoa/gen/Internal/Validation/_2008_06/__init__.py
+-rw-r--r--   0        0        0     7000 2022-10-20 12:42:54.386082 tcsoa-0.9.1/tcsoa/gen/Internal/Validation/_2008_06/Validation.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.547030 tcsoa-0.9.1/tcsoa/gen/Internal/Validation/_2012_02/__init__.py
+-rw-r--r--   0        0        0     9436 2022-10-20 12:42:54.466090 tcsoa-0.9.1/tcsoa/gen/Internal/Validation/_2012_02/Validation.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.609032 tcsoa-0.9.1/tcsoa/gen/Internal/Validation/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.585031 tcsoa-0.9.1/tcsoa/gen/Internal/Vendormanagement/_2008_05/__init__.py
+-rw-r--r--   0        0        0     3964 2022-10-20 12:42:54.508090 tcsoa-0.9.1/tcsoa/gen/Internal/Vendormanagement/_2008_05/VendorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.741045 tcsoa-0.9.1/tcsoa/gen/Internal/Vendormanagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0      933 2022-10-20 12:42:54.539095 tcsoa-0.9.1/tcsoa/gen/Internal/Vendormanagement/_2008_06/VendorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.919067 tcsoa-0.9.1/tcsoa/gen/Internal/Vendormanagement/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.857059 tcsoa-0.9.1/tcsoa/gen/Internal/VendorManagementAW/_2019_12/__init__.py
+-rw-r--r--   0        0        0     5178 2022-10-20 12:43:04.107987 tcsoa-0.9.1/tcsoa/gen/Internal/VendorManagementAW/_2019_12/VendorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.556030 tcsoa-0.9.1/tcsoa/gen/Internal/VendorManagementAW/_2020_05/__init__.py
+-rw-r--r--   0        0        0     1561 2022-10-20 12:43:04.141992 tcsoa-0.9.1/tcsoa/gen/Internal/VendorManagementAW/_2020_05/VendorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.843052 tcsoa-0.9.1/tcsoa/gen/Internal/VendorManagementAW/_2020_12/__init__.py
+-rw-r--r--   0        0        0     2730 2022-10-20 12:43:04.178991 tcsoa-0.9.1/tcsoa/gen/Internal/VendorManagementAW/_2020_12/VendorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.705043 tcsoa-0.9.1/tcsoa/gen/Internal/VendorManagementAW/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.712045 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2008_06/__init__.py
+-rw-r--r--   0        0        0    33963 2022-10-20 12:42:54.749115 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2008_06/DataManagement.py
+-rw-r--r--   0        0        0    18894 2022-10-20 12:42:54.899127 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2008_06/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.614029 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2010_04/__init__.py
+-rw-r--r--   0        0        0     7925 2022-10-20 12:42:54.983135 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2010_04/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.734041 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2010_09/__init__.py
+-rw-r--r--   0        0        0    16115 2022-10-20 12:42:55.127153 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2010_09/DataManagement.py
+-rw-r--r--   0        0        0     2540 2022-10-20 12:42:55.165162 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2010_09/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.909059 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2011_12/__init__.py
+-rw-r--r--   0        0        0     8571 2022-10-20 12:42:55.235162 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2011_12/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.776046 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2012_10/__init__.py
+-rw-r--r--   0        0        0     1826 2022-10-20 12:42:55.267161 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2012_10/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.607029 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2017_05/__init__.py
+-rw-r--r--   0        0        0     5634 2022-10-20 12:42:55.327171 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2017_05/DataManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.707045 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2018_11/__init__.py
+-rw-r--r--   0        0        0     6419 2022-10-20 12:42:55.385169 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2018_11/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.771052 tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.920064 tcsoa-0.9.1/tcsoa/gen/Internal/Workflow/_2013_05/__init__.py
+-rw-r--r--   0        0        0     2172 2022-10-20 12:42:55.418172 tcsoa-0.9.1/tcsoa/gen/Internal/Workflow/_2013_05/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.625030 tcsoa-0.9.1/tcsoa/gen/Internal/Workflow/_2017_11/__init__.py
+-rw-r--r--   0        0        0     1689 2022-10-20 12:42:55.446180 tcsoa-0.9.1/tcsoa/gen/Internal/Workflow/_2017_11/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.001066 tcsoa-0.9.1/tcsoa/gen/Internal/Workflow/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.552030 tcsoa-0.9.1/tcsoa/gen/Internal/Workflowaw/_2020_12/__init__.py
+-rw-r--r--   0        0        0     9409 2022-10-20 12:42:03.883159 tcsoa-0.9.1/tcsoa/gen/Internal/Workflowaw/_2020_12/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.968069 tcsoa-0.9.1/tcsoa/gen/Internal/Workflowaw/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.637041 tcsoa-0.9.1/tcsoa/gen/Internal/XlsBom/_2020_12/__init__.py
+-rw-r--r--   0        0        0    10138 2022-10-20 12:42:00.399779 tcsoa-0.9.1/tcsoa/gen/Internal/XlsBom/_2020_12/Import.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.987071 tcsoa-0.9.1/tcsoa/gen/Internal/XlsBom/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.735048 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2012_10/__init__.py
+-rw-r--r--   0        0        0    13932 2022-10-20 12:42:20.406909 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2012_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.571032 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_03/__init__.py
+-rw-r--r--   0        0        0     1010 2022-10-20 12:42:20.433918 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.935069 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_07/__init__.py
+-rw-r--r--   0        0        0      832 2022-10-20 12:42:20.463916 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_07/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.665047 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_10/__init__.py
+-rw-r--r--   0        0        0     2136 2022-10-20 12:42:20.495920 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.926059 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2016_03/__init__.py
+-rw-r--r--   0        0        0     3032 2022-10-20 12:42:20.531923 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2016_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.719040 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2017_06/__init__.py
+-rw-r--r--   0        0        0     3644 2022-10-20 12:42:20.570922 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2017_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.842051 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2017_12/__init__.py
+-rw-r--r--   0        0        0     1303 2022-10-20 12:42:20.598934 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2017_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.582039 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2018_05/__init__.py
+-rw-r--r--   0        0        0     4897 2022-10-20 12:42:20.636929 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2018_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.785046 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2018_12/__init__.py
+-rw-r--r--   0        0        0     6769 2022-10-20 12:42:20.685934 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2018_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.583037 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2019_06/__init__.py
+-rw-r--r--   0        0        0     8286 2022-10-20 12:42:20.759945 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2019_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.982071 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2019_12/__init__.py
+-rw-r--r--   0        0        0     9740 2022-10-20 12:42:20.822947 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2019_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.907054 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2020_05/__init__.py
+-rw-r--r--   0        0        0     4187 2022-10-20 12:42:20.858952 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2020_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.645038 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2020_12/__init__.py
+-rw-r--r--   0        0        0     5323 2022-10-20 12:42:20.898967 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2020_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.586038 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/__init__.py
+-rw-r--r--   0        0        0     5532 2022-10-20 12:41:55.049209 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.673044 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceVis/_2014_11/__init__.py
+-rw-r--r--   0        0        0     3736 2022-10-20 12:42:20.932958 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceVis/_2014_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.853059 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceVis/_2015_03/__init__.py
+-rw-r--r--   0        0        0    14757 2022-10-20 12:42:20.972973 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceVis/_2015_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.598027 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceVis/_2018_05/__init__.py
+-rw-r--r--   0        0        0     3936 2022-10-20 12:42:21.003963 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceVis/_2018_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.897060 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceVis/__init__.py
+-rw-r--r--   0        0        0      918 2022-10-20 12:41:55.065213 tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceVis/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.570034 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2007_06/__init__.py
+-rw-r--r--   0        0        0     9918 2022-10-20 12:42:21.059971 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.838057 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2008_06/__init__.py
+-rw-r--r--   0        0        0     1776 2022-10-20 12:42:21.085974 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.770065 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2009_10/__init__.py
+-rw-r--r--   0        0        0     2310 2022-10-20 12:42:21.114973 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2009_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.569031 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2011_06/__init__.py
+-rw-r--r--   0        0        0     1150 2022-10-20 12:42:21.143976 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.005088 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2012_10/__init__.py
+-rw-r--r--   0        0        0     1269 2022-10-20 12:42:21.173981 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2012_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.807048 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2013_05/__init__.py
+-rw-r--r--   0        0        0     1060 2022-10-20 12:42:21.202981 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2013_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.598027 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2014_10/__init__.py
+-rw-r--r--   0        0        0     1150 2022-10-20 12:42:21.232984 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2014_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.680038 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2015_10/__init__.py
+-rw-r--r--   0        0        0     1230 2022-10-20 12:42:21.264989 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2015_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.746044 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2016_09/__init__.py
+-rw-r--r--   0        0        0     1161 2022-10-20 12:42:21.295993 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2016_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.885067 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2017_11/__init__.py
+-rw-r--r--   0        0        0     1619 2022-10-20 12:42:21.326995 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2017_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.737048 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2018_06/__init__.py
+-rw-r--r--   0        0        0     1205 2022-10-20 12:42:21.356998 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2018_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.766045 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2018_11/__init__.py
+-rw-r--r--   0        0        0     1505 2022-10-20 12:42:21.385002 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2018_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.967069 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2019_06/__init__.py
+-rw-r--r--   0        0        0     1830 2022-10-20 12:42:21.416009 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2019_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.869055 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/__init__.py
+-rw-r--r--   0        0        0     2860 2022-10-20 12:41:55.106219 tcsoa-0.9.1/tcsoa/gen/Internal_Administration/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.668044 tcsoa-0.9.1/tcsoa/gen/Internal_Ai/_2008_06/__init__.py
+-rw-r--r--   0        0        0     2408 2022-10-20 12:42:21.452010 tcsoa-0.9.1/tcsoa/gen/Internal_Ai/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.825058 tcsoa-0.9.1/tcsoa/gen/Internal_Ai/_2016_03/__init__.py
+-rw-r--r--   0        0        0      856 2022-10-20 12:42:21.482016 tcsoa-0.9.1/tcsoa/gen/Internal_Ai/_2016_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.987071 tcsoa-0.9.1/tcsoa/gen/Internal_Ai/_2016_04/__init__.py
+-rw-r--r--   0        0        0     1099 2022-10-20 12:42:21.510011 tcsoa-0.9.1/tcsoa/gen/Internal_Ai/_2016_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.552030 tcsoa-0.9.1/tcsoa/gen/Internal_Ai/__init__.py
+-rw-r--r--   0        0        0      528 2022-10-20 12:41:55.118212 tcsoa-0.9.1/tcsoa/gen/Internal_Ai/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.549029 tcsoa-0.9.1/tcsoa/gen/Internal_AuditManager/_2012_09/__init__.py
+-rw-r--r--   0        0        0     1012 2022-10-20 12:42:21.543017 tcsoa-0.9.1/tcsoa/gen/Internal_AuditManager/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.748043 tcsoa-0.9.1/tcsoa/gen/Internal_AuditManager/__init__.py
+-rw-r--r--   0        0        0      262 2022-10-20 12:41:55.124216 tcsoa-0.9.1/tcsoa/gen/Internal_AuditManager/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.561031 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2012_10/__init__.py
+-rw-r--r--   0        0        0    24886 2022-10-20 12:42:19.584833 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2012_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.619029 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2013_12/__init__.py
+-rw-r--r--   0        0        0     7485 2022-10-20 12:42:19.630838 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2013_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.752043 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2014_11/__init__.py
+-rw-r--r--   0        0        0     2928 2022-10-20 12:42:19.667842 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2014_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.550029 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2015_03/__init__.py
+-rw-r--r--   0        0        0    10876 2022-10-20 12:42:19.719846 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2015_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.800055 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2015_10/__init__.py
+-rw-r--r--   0        0        0     4603 2022-10-20 12:42:19.759850 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2015_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.558030 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2016_03/__init__.py
+-rw-r--r--   0        0        0    19107 2022-10-20 12:42:19.819882 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2016_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.009069 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2016_04/__init__.py
+-rw-r--r--   0        0        0     5333 2022-10-20 12:42:19.853858 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2016_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.785046 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2016_12/__init__.py
+-rw-r--r--   0        0        0    26603 2022-10-20 12:42:19.915865 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2016_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.973071 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2017_06/__init__.py
+-rw-r--r--   0        0        0    35016 2022-10-20 12:42:19.993876 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2017_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.636038 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2017_12/__init__.py
+-rw-r--r--   0        0        0    15630 2022-10-20 12:42:20.047873 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2017_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.740043 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2018_05/__init__.py
+-rw-r--r--   0        0        0    24660 2022-10-20 12:42:20.132882 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2018_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.837052 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2018_12/__init__.py
+-rw-r--r--   0        0        0     3745 2022-10-20 12:42:20.169887 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2018_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.988072 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2019_06/__init__.py
+-rw-r--r--   0        0        0    11037 2022-10-20 12:42:20.220892 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2019_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.888056 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2019_12/__init__.py
+-rw-r--r--   0        0        0    10755 2022-10-20 12:42:20.266899 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2019_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.671045 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2020_05/__init__.py
+-rw-r--r--   0        0        0    11815 2022-10-20 12:42:20.324905 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2020_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.546029 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2020_12/__init__.py
+-rw-r--r--   0        0        0     3585 2022-10-20 12:42:20.357903 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2020_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.731058 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/__init__.py
+-rw-r--r--   0        0        0    12806 2022-10-20 12:41:54.956200 tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.991073 tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2007_01/__init__.py
+-rw-r--r--   0        0        0     2159 2022-10-20 12:42:21.574028 tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2007_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.601029 tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2010_04/__init__.py
+-rw-r--r--   0        0        0     3092 2022-10-20 12:42:21.608035 tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.565032 tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2010_09/__init__.py
+-rw-r--r--   0        0        0     3047 2022-10-20 12:42:21.640027 tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2010_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.730042 tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2011_06/__init__.py
+-rw-r--r--   0        0        0     3249 2022-10-20 12:42:21.671029 tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.758045 tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2013_05/__init__.py
+-rw-r--r--   0        0        0     1768 2022-10-20 12:42:21.704038 tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2013_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.929066 tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/__init__.py
+-rw-r--r--   0        0        0     1149 2022-10-20 12:41:55.144219 tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.587032 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2007_12/__init__.py
+-rw-r--r--   0        0        0     1873 2022-10-20 12:42:21.735051 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2007_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.672047 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2008_03/__init__.py
+-rw-r--r--   0        0        0     2629 2022-10-20 12:42:21.764046 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2008_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.007066 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2008_05/__init__.py
+-rw-r--r--   0        0        0     1797 2022-10-20 12:42:21.793041 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2008_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.629037 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2008_06/__init__.py
+-rw-r--r--   0        0        0     1487 2022-10-20 12:42:21.823046 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.815056 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2010_04/__init__.py
+-rw-r--r--   0        0        0     3799 2022-10-20 12:42:21.857046 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.642033 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2013_05/__init__.py
+-rw-r--r--   0        0        0     1003 2022-10-20 12:42:21.890056 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2013_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.866073 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2017_05/__init__.py
+-rw-r--r--   0        0        0     5274 2022-10-20 12:42:21.920058 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2017_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.639047 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/__init__.py
+-rw-r--r--   0        0        0     1160 2022-10-20 12:41:55.161222 tcsoa-0.9.1/tcsoa/gen/Internal_Cad/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.933066 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2009_10/__init__.py
+-rw-r--r--   0        0        0     1029 2022-10-20 12:42:21.950060 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2009_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.676048 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2011_06/__init__.py
+-rw-r--r--   0        0        0     5877 2022-10-20 12:42:21.983063 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.601029 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2012_02/__init__.py
+-rw-r--r--   0        0        0     5429 2022-10-20 12:42:22.021068 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2012_02/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.626031 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2012_09/__init__.py
+-rw-r--r--   0        0        0     4590 2022-10-20 12:42:22.057063 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.975074 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2013_05/__init__.py
+-rw-r--r--   0        0        0     1381 2022-10-20 12:42:22.087066 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2013_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.640035 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2013_12/__init__.py
+-rw-r--r--   0        0        0     4785 2022-10-20 12:42:22.123069 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2013_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.711042 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2014_06/__init__.py
+-rw-r--r--   0        0        0     4406 2022-10-20 12:42:22.153071 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2014_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.962068 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/__init__.py
+-rw-r--r--   0        0        0     1736 2022-10-20 12:41:55.189220 tcsoa-0.9.1/tcsoa/gen/Internal_Cae/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.872054 tcsoa-0.9.1/tcsoa/gen/Internal_ChangeManagement/_2012_10/__init__.py
+-rw-r--r--   0        0        0     1192 2022-10-20 12:42:22.193081 tcsoa-0.9.1/tcsoa/gen/Internal_ChangeManagement/_2012_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.706044 tcsoa-0.9.1/tcsoa/gen/Internal_ChangeManagement/_2015_03/__init__.py
+-rw-r--r--   0        0        0     4808 2022-10-20 12:42:22.230086 tcsoa-0.9.1/tcsoa/gen/Internal_ChangeManagement/_2015_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.599028 tcsoa-0.9.1/tcsoa/gen/Internal_ChangeManagement/_2020_01/__init__.py
+-rw-r--r--   0        0        0     2892 2022-10-20 12:42:22.267080 tcsoa-0.9.1/tcsoa/gen/Internal_ChangeManagement/_2020_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.818055 tcsoa-0.9.1/tcsoa/gen/Internal_ChangeManagement/__init__.py
+-rw-r--r--   0        0        0      975 2022-10-20 12:41:55.205226 tcsoa-0.9.1/tcsoa/gen/Internal_ChangeManagement/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.947068 tcsoa-0.9.1/tcsoa/gen/Internal_Classification/_2009_10/__init__.py
+-rw-r--r--   0        0        0     3376 2022-10-20 12:42:22.312086 tcsoa-0.9.1/tcsoa/gen/Internal_Classification/_2009_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.877060 tcsoa-0.9.1/tcsoa/gen/Internal_Classification/_2017_05/__init__.py
+-rw-r--r--   0        0        0     1449 2022-10-20 12:42:22.344101 tcsoa-0.9.1/tcsoa/gen/Internal_Classification/_2017_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.778055 tcsoa-0.9.1/tcsoa/gen/Internal_Classification/_2018_11/__init__.py
+-rw-r--r--   0        0        0     2076 2022-10-20 12:42:22.375096 tcsoa-0.9.1/tcsoa/gen/Internal_Classification/_2018_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.749045 tcsoa-0.9.1/tcsoa/gen/Internal_Classification/_2020_04/__init__.py
+-rw-r--r--   0        0        0     2495 2022-10-20 12:42:22.410101 tcsoa-0.9.1/tcsoa/gen/Internal_Classification/_2020_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.760046 tcsoa-0.9.1/tcsoa/gen/Internal_Classification/__init__.py
+-rw-r--r--   0        0        0      775 2022-10-20 12:41:55.217229 tcsoa-0.9.1/tcsoa/gen/Internal_Classification/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.890058 tcsoa-0.9.1/tcsoa/gen/Internal_CodeCoverage/_2011_06/__init__.py
+-rw-r--r--   0        0        0     1193 2022-10-20 12:42:22.442098 tcsoa-0.9.1/tcsoa/gen/Internal_CodeCoverage/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.843052 tcsoa-0.9.1/tcsoa/gen/Internal_CodeCoverage/__init__.py
+-rw-r--r--   0        0        0      234 2022-10-20 12:41:55.223224 tcsoa-0.9.1/tcsoa/gen/Internal_CodeCoverage/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.986071 tcsoa-0.9.1/tcsoa/gen/Internal_ConfigFilterCriteria/_2013_12/__init__.py
+-rw-r--r--   0        0        0     5417 2022-10-20 12:42:22.473105 tcsoa-0.9.1/tcsoa/gen/Internal_ConfigFilterCriteria/_2013_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.573032 tcsoa-0.9.1/tcsoa/gen/Internal_ConfigFilterCriteria/__init__.py
+-rw-r--r--   0        0        0      252 2022-10-20 12:41:55.230229 tcsoa-0.9.1/tcsoa/gen/Internal_ConfigFilterCriteria/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.777047 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2014_06/__init__.py
+-rw-r--r--   0        0        0    34830 2022-10-20 12:42:22.536112 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2014_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.711042 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2014_12/__init__.py
+-rw-r--r--   0        0        0     7798 2022-10-20 12:42:22.572113 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2014_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.569031 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2015_03/__init__.py
+-rw-r--r--   0        0        0     4071 2022-10-20 12:42:22.604114 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2015_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.910058 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2015_10/__init__.py
+-rw-r--r--   0        0        0    21675 2022-10-20 12:42:22.652118 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2015_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.832057 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2016_09/__init__.py
+-rw-r--r--   0        0        0     4616 2022-10-20 12:42:22.701122 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2016_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.961068 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2017_11/__init__.py
+-rw-r--r--   0        0        0     3763 2022-10-20 12:42:22.734133 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2017_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.594028 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2018_06/__init__.py
+-rw-r--r--   0        0        0    12378 2022-10-20 12:42:22.773129 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2018_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.653035 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2018_11/__init__.py
+-rw-r--r--   0        0        0     6517 2022-10-20 12:42:22.804140 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2018_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.875078 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/__init__.py
+-rw-r--r--   0        0        0     2810 2022-10-20 12:41:55.287226 tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.563036 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2006_03/__init__.py
+-rw-r--r--   0        0        0     1046 2022-10-20 12:42:22.832134 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2006_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.825058 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_01/__init__.py
+-rw-r--r--   0        0        0     2049 2022-10-20 12:42:22.864140 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.958058 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_05/__init__.py
+-rw-r--r--   0        0        0     1336 2022-10-20 12:42:22.894146 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.997071 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_06/__init__.py
+-rw-r--r--   0        0        0     3003 2022-10-20 12:42:22.927172 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.975074 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_09/__init__.py
+-rw-r--r--   0        0        0      987 2022-10-20 12:42:22.956153 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.594028 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_12/__init__.py
+-rw-r--r--   0        0        0      925 2022-10-20 12:42:22.985156 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.679048 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2008_03/__init__.py
+-rw-r--r--   0        0        0     1026 2022-10-20 12:42:23.015150 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2008_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.749045 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2008_06/__init__.py
+-rw-r--r--   0        0        0    22448 2022-10-20 12:42:23.087161 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.885067 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2009_10/__init__.py
+-rw-r--r--   0        0        0     2299 2022-10-20 12:42:23.120164 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2009_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.615033 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2010_04/__init__.py
+-rw-r--r--   0        0        0     4697 2022-10-20 12:42:23.167164 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.971062 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2010_09/__init__.py
+-rw-r--r--   0        0        0     2721 2022-10-20 12:42:23.208171 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2010_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.774045 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2011_06/__init__.py
+-rw-r--r--   0        0        0      732 2022-10-20 12:42:23.238171 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.634037 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2012_02/__init__.py
+-rw-r--r--   0        0        0     3403 2022-10-20 12:42:23.268177 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2012_02/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.618030 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2012_09/__init__.py
+-rw-r--r--   0        0        0      990 2022-10-20 12:42:23.299178 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.681046 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2012_10/__init__.py
+-rw-r--r--   0        0        0     3063 2022-10-20 12:42:23.330192 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2012_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.948069 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2013_05/__init__.py
+-rw-r--r--   0        0        0     7860 2022-10-20 12:42:23.383204 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2013_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.613030 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2014_10/__init__.py
+-rw-r--r--   0        0        0     5339 2022-10-20 12:42:23.427203 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2014_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.756046 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2014_11/__init__.py
+-rw-r--r--   0        0        0     1375 2022-10-20 12:42:23.462200 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2014_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.821055 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2016_10/__init__.py
+-rw-r--r--   0        0        0     5578 2022-10-20 12:42:23.493210 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2016_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.741045 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2017_05/__init__.py
+-rw-r--r--   0        0        0     5671 2022-10-20 12:42:23.528214 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2017_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.792046 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2017_11/__init__.py
+-rw-r--r--   0        0        0     8830 2022-10-20 12:42:23.574215 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2017_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.541030 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2018_06/__init__.py
+-rw-r--r--   0        0        0    14951 2022-10-20 12:42:23.607233 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2018_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.782046 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2018_11/__init__.py
+-rw-r--r--   0        0        0     3087 2022-10-20 12:42:23.642210 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2018_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.604032 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2018_12/__init__.py
+-rw-r--r--   0        0        0     1277 2022-10-20 12:42:23.670218 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2018_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.856060 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2020_01/__init__.py
+-rw-r--r--   0        0        0     1839 2022-10-20 12:42:23.702231 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2020_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.009069 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2020_04/__init__.py
+-rw-r--r--   0        0        0     1869 2022-10-20 12:42:23.731227 tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2020_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.566032 tcsoa-0.9.1/tcsoa/gen/Internal_Core/__init__.py
+-rw-r--r--   0        0        0     7942 2022-10-20 12:41:55.393239 tcsoa-0.9.1/tcsoa/gen/Internal_Core/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.703047 tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2011_06/__init__.py
+-rw-r--r--   0        0        0    25857 2022-10-20 12:42:23.831231 tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.854061 tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2014_06/__init__.py
+-rw-r--r--   0        0        0     2931 2022-10-20 12:42:23.863232 tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2014_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.627031 tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2015_07/__init__.py
+-rw-r--r--   0        0        0     1397 2022-10-20 12:42:23.898235 tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2015_07/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.764042 tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2015_10/__init__.py
+-rw-r--r--   0        0        0     2667 2022-10-20 12:42:23.932240 tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2015_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.904062 tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2019_06/__init__.py
+-rw-r--r--   0        0        0     1472 2022-10-20 12:42:23.966251 tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2019_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.834055 tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/__init__.py
+-rw-r--r--   0        0        0     2774 2022-10-20 12:41:55.455274 tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.691046 tcsoa-0.9.1/tcsoa/gen/Internal_DocMgmtAw/_2019_06/__init__.py
+-rw-r--r--   0        0        0     1045 2022-10-20 12:42:24.000241 tcsoa-0.9.1/tcsoa/gen/Internal_DocMgmtAw/_2019_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.967069 tcsoa-0.9.1/tcsoa/gen/Internal_DocMgmtAw/_2019_12/__init__.py
+-rw-r--r--   0        0        0     1082 2022-10-20 12:42:24.030248 tcsoa-0.9.1/tcsoa/gen/Internal_DocMgmtAw/_2019_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.572031 tcsoa-0.9.1/tcsoa/gen/Internal_DocMgmtAw/__init__.py
+-rw-r--r--   0        0        0      330 2022-10-20 12:41:55.463252 tcsoa-0.9.1/tcsoa/gen/Internal_DocMgmtAw/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.909059 tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0     8877 2022-10-20 12:42:24.068250 tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.788046 tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/_2013_05/__init__.py
+-rw-r--r--   0        0        0     4997 2022-10-20 12:42:24.101258 tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/_2013_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.753044 tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/_2013_12/__init__.py
+-rw-r--r--   0        0        0     1788 2022-10-20 12:42:24.139254 tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/_2013_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.795051 tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/_2020_12/__init__.py
+-rw-r--r--   0        0        0     1084 2022-10-20 12:42:24.168262 tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/_2020_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.767045 tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/__init__.py
+-rw-r--r--   0        0        0     1132 2022-10-20 12:41:55.481255 tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.960068 tcsoa-0.9.1/tcsoa/gen/Internal_EntCba/_2019_12/__init__.py
+-rw-r--r--   0        0        0     1800 2022-10-20 12:42:24.202265 tcsoa-0.9.1/tcsoa/gen/Internal_EntCba/_2019_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.775046 tcsoa-0.9.1/tcsoa/gen/Internal_EntCba/__init__.py
+-rw-r--r--   0        0        0      254 2022-10-20 12:41:55.489256 tcsoa-0.9.1/tcsoa/gen/Internal_EntCba/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.573032 tcsoa-0.9.1/tcsoa/gen/Internal_Gdis/_2006_03/__init__.py
+-rw-r--r--   0        0        0     1008 2022-10-20 12:42:24.233267 tcsoa-0.9.1/tcsoa/gen/Internal_Gdis/_2006_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.693045 tcsoa-0.9.1/tcsoa/gen/Internal_Gdis/__init__.py
+-rw-r--r--   0        0        0      208 2022-10-20 12:41:55.495254 tcsoa-0.9.1/tcsoa/gen/Internal_Gdis/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.669045 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2007_06/__init__.py
+-rw-r--r--   0        0        0    20751 2022-10-20 12:42:24.317273 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.677047 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2008_06/__init__.py
+-rw-r--r--   0        0        0     3181 2022-10-20 12:42:24.354304 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.606028 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2010_02/__init__.py
+-rw-r--r--   0        0        0     5593 2022-10-20 12:42:24.390282 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2010_02/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.852060 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2010_09/__init__.py
+-rw-r--r--   0        0        0     1841 2022-10-20 12:42:24.424283 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2010_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.761044 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2017_05/__init__.py
+-rw-r--r--   0        0        0     1366 2022-10-20 12:42:24.460310 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2017_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.674047 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2018_11/__init__.py
+-rw-r--r--   0        0        0     4097 2022-10-20 12:42:24.498292 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2018_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.825058 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2020_01/__init__.py
+-rw-r--r--   0        0        0    12188 2022-10-20 12:42:24.550302 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2020_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.805070 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/__init__.py
+-rw-r--r--   0        0        0     3368 2022-10-20 12:41:55.555262 tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.683038 tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2017_06/__init__.py
+-rw-r--r--   0        0        0     1936 2022-10-20 12:42:24.583299 tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2017_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.732052 tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2017_12/__init__.py
+-rw-r--r--   0        0        0     3439 2022-10-20 12:42:24.614305 tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2017_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.663035 tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2018_05/__init__.py
+-rw-r--r--   0        0        0     6963 2022-10-20 12:42:24.650303 tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2018_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.713049 tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2018_12/__init__.py
+-rw-r--r--   0        0        0     6431 2022-10-20 12:42:24.685309 tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2018_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.572031 tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2019_06/__init__.py
+-rw-r--r--   0        0        0     2043 2022-10-20 12:42:24.722314 tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2019_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.720039 tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2019_12/__init__.py
+-rw-r--r--   0        0        0     4182 2022-10-20 12:42:24.753315 tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2019_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.835050 tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/__init__.py
+-rw-r--r--   0        0        0     1210 2022-10-20 12:41:55.573279 tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.841051 tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/_2010_04/__init__.py
+-rw-r--r--   0        0        0     4263 2022-10-20 12:42:24.785318 tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.686038 tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/_2017_05/__init__.py
+-rw-r--r--   0        0        0     1394 2022-10-20 12:42:24.825319 tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/_2017_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.563036 tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/_2017_11/__init__.py
+-rw-r--r--   0        0        0     2108 2022-10-20 12:42:24.865328 tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/_2017_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.781046 tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/_2018_06/__init__.py
+-rw-r--r--   0        0        0     2277 2022-10-20 12:42:24.903325 tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/_2018_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.911054 tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/__init__.py
+-rw-r--r--   0        0        0      916 2022-10-20 12:41:55.588271 tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.989074 tcsoa-0.9.1/tcsoa/gen/Internal_Integration/_2007_06/__init__.py
+-rw-r--r--   0        0        0     1319 2022-10-20 12:42:24.951334 tcsoa-0.9.1/tcsoa/gen/Internal_Integration/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.010070 tcsoa-0.9.1/tcsoa/gen/Internal_Integration/_2008_06/__init__.py
+-rw-r--r--   0        0        0      755 2022-10-20 12:42:24.987337 tcsoa-0.9.1/tcsoa/gen/Internal_Integration/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.817058 tcsoa-0.9.1/tcsoa/gen/Internal_Integration/__init__.py
+-rw-r--r--   0        0        0      344 2022-10-20 12:41:55.596266 tcsoa-0.9.1/tcsoa/gen/Internal_Integration/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.616029 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2008_12/__init__.py
+-rw-r--r--   0        0        0     1466 2022-10-20 12:42:25.046341 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2008_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.979064 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2011_12/__init__.py
+-rw-r--r--   0        0        0     1023 2022-10-20 12:42:25.089344 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2011_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.965064 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2012_09/__init__.py
+-rw-r--r--   0        0        0     1629 2022-10-20 12:42:25.129352 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.801055 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2013_12/__init__.py
+-rw-r--r--   0        0        0     2546 2022-10-20 12:42:25.161355 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2013_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.798053 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2014_06/__init__.py
+-rw-r--r--   0        0        0     3129 2022-10-20 12:42:25.201363 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2014_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.606028 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2014_12/__init__.py
+-rw-r--r--   0        0        0     8836 2022-10-20 12:42:25.273360 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2014_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.754044 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2015_03/__init__.py
+-rw-r--r--   0        0        0    19450 2022-10-20 12:42:25.349401 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2015_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.918071 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2015_10/__init__.py
+-rw-r--r--   0        0        0     8638 2022-10-20 12:42:25.397374 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2015_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.950068 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2016_03/__init__.py
+-rw-r--r--   0        0        0     1257 2022-10-20 12:42:25.434378 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2016_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.623033 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2016_09/__init__.py
+-rw-r--r--   0        0        0    25266 2022-10-20 12:42:25.524386 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2016_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.747043 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2017_05/__init__.py
+-rw-r--r--   0        0        0     9922 2022-10-20 12:42:25.580400 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2017_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.013069 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2017_11/__init__.py
+-rw-r--r--   0        0        0     9646 2022-10-20 12:42:25.621396 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2017_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.577032 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2018_11/__init__.py
+-rw-r--r--   0        0        0     6995 2022-10-20 12:42:25.661407 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2018_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.759045 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2019_06/__init__.py
+-rw-r--r--   0        0        0     5548 2022-10-20 12:42:25.713403 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2019_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.575032 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2020_01/__init__.py
+-rw-r--r--   0        0        0     4246 2022-10-20 12:42:25.749415 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2020_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.575032 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2020_04/__init__.py
+-rw-r--r--   0        0        0     1237 2022-10-20 12:42:25.777418 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2020_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.621029 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/__init__.py
+-rw-r--r--   0        0        0     8038 2022-10-20 12:41:55.714276 tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.643038 tcsoa-0.9.1/tcsoa/gen/Internal_Mmv/_2012_09/__init__.py
+-rw-r--r--   0        0        0    28667 2022-10-20 12:42:25.821416 tcsoa-0.9.1/tcsoa/gen/Internal_Mmv/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.757046 tcsoa-0.9.1/tcsoa/gen/Internal_Mmv/__init__.py
+-rw-r--r--   0        0        0      561 2022-10-20 12:41:55.730276 tcsoa-0.9.1/tcsoa/gen/Internal_Mmv/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.903060 tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2007_06/__init__.py
+-rw-r--r--   0        0        0    69367 2022-10-20 12:42:25.952427 tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.620029 tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2011_06/__init__.py
+-rw-r--r--   0        0        0     2292 2022-10-20 12:42:26.134447 tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.784047 tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2012_02/__init__.py
+-rw-r--r--   0        0        0    51330 2022-10-20 12:42:26.103445 tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2012_02/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.726040 tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2017_11/__init__.py
+-rw-r--r--   0        0        0     4059 2022-10-20 12:42:26.171454 tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2017_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.772051 tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2018_06/__init__.py
+-rw-r--r--   0        0        0     1391 2022-10-20 12:42:26.203449 tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2018_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.745043 tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2020_12/__init__.py
+-rw-r--r--   0        0        0     1645 2022-10-20 12:42:26.234459 tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2020_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.642033 tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/__init__.py
+-rw-r--r--   0        0        0      852 2022-10-20 12:41:55.878289 tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.576032 tcsoa-0.9.1/tcsoa/gen/Internal_Notification/_2014_10/__init__.py
+-rw-r--r--   0        0        0     1309 2022-10-20 12:42:26.274455 tcsoa-0.9.1/tcsoa/gen/Internal_Notification/_2014_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.657040 tcsoa-0.9.1/tcsoa/gen/Internal_Notification/_2015_03/__init__.py
+-rw-r--r--   0        0        0    13391 2022-10-20 12:42:26.332475 tcsoa-0.9.1/tcsoa/gen/Internal_Notification/_2015_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.974072 tcsoa-0.9.1/tcsoa/gen/Internal_Notification/_2015_10/__init__.py
+-rw-r--r--   0        0        0     9350 2022-10-20 12:42:26.388475 tcsoa-0.9.1/tcsoa/gen/Internal_Notification/_2015_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.579033 tcsoa-0.9.1/tcsoa/gen/Internal_Notification/_2017_11/__init__.py
+-rw-r--r--   0        0        0     2054 2022-10-20 12:42:26.418467 tcsoa-0.9.1/tcsoa/gen/Internal_Notification/_2017_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.654034 tcsoa-0.9.1/tcsoa/gen/Internal_Notification/__init__.py
+-rw-r--r--   0        0        0     1833 2022-10-20 12:41:55.912295 tcsoa-0.9.1/tcsoa/gen/Internal_Notification/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.652035 tcsoa-0.9.1/tcsoa/gen/Internal_OccMgmt/_2020_05/__init__.py
+-rw-r--r--   0        0        0     5378 2022-10-20 12:42:26.455485 tcsoa-0.9.1/tcsoa/gen/Internal_OccMgmt/_2020_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.660035 tcsoa-0.9.1/tcsoa/gen/Internal_OccMgmt/_2020_12/__init__.py
+-rw-r--r--   0        0        0     3264 2022-10-20 12:42:26.489477 tcsoa-0.9.1/tcsoa/gen/Internal_OccMgmt/_2020_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.588032 tcsoa-0.9.1/tcsoa/gen/Internal_OccMgmt/__init__.py
+-rw-r--r--   0        0        0      604 2022-10-20 12:41:55.924297 tcsoa-0.9.1/tcsoa/gen/Internal_OccMgmt/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.895056 tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/_2017_12/__init__.py
+-rw-r--r--   0        0        0     3057 2022-10-20 12:42:26.521480 tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/_2017_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.717049 tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/_2018_05/__init__.py
+-rw-r--r--   0        0        0     5894 2022-10-20 12:42:26.560490 tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/_2018_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.899057 tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/_2020_05/__init__.py
+-rw-r--r--   0        0        0     1789 2022-10-20 12:42:26.591484 tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/_2020_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.846064 tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/_2020_12/__init__.py
+-rw-r--r--   0        0        0     4495 2022-10-20 12:42:26.626492 tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/_2020_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.558030 tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/__init__.py
+-rw-r--r--   0        0        0     1299 2022-10-20 12:41:55.947305 tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.934070 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2007_01/__init__.py
+-rw-r--r--   0        0        0     1510 2022-10-20 12:42:26.658492 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2007_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.622030 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2007_06/__init__.py
+-rw-r--r--   0        0        0     2566 2022-10-20 12:42:26.692497 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.002064 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0     2931 2022-10-20 12:42:26.727507 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.822046 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2009_10/__init__.py
+-rw-r--r--   0        0        0     2259 2022-10-20 12:42:26.760499 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2009_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.759045 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2010_04/__init__.py
+-rw-r--r--   0        0        0      712 2022-10-20 12:42:26.790508 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.810050 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2011_06/__init__.py
+-rw-r--r--   0        0        0     2538 2022-10-20 12:42:26.824516 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.903060 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2012_02/__init__.py
+-rw-r--r--   0        0        0     1040 2022-10-20 12:42:26.855521 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2012_02/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.838057 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2014_10/__init__.py
+-rw-r--r--   0        0        0     3525 2022-10-20 12:42:26.886513 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2014_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.003067 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/__init__.py
+-rw-r--r--   0        0        0     1622 2022-10-20 12:41:55.976306 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.826051 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagementAw/_2019_12/__init__.py
+-rw-r--r--   0        0        0     1136 2022-10-20 12:42:26.920517 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagementAw/_2019_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.651040 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagementAw/__init__.py
+-rw-r--r--   0        0        0      239 2022-10-20 12:41:55.982311 tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagementAw/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.819055 tcsoa-0.9.1/tcsoa/gen/Internal_Query/_2008_06/__init__.py
+-rw-r--r--   0        0        0      867 2022-10-20 12:42:26.953522 tcsoa-0.9.1/tcsoa/gen/Internal_Query/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.641039 tcsoa-0.9.1/tcsoa/gen/Internal_Query/_2012_02/__init__.py
+-rw-r--r--   0        0        0     1018 2022-10-20 12:42:26.986523 tcsoa-0.9.1/tcsoa/gen/Internal_Query/_2012_02/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.881065 tcsoa-0.9.1/tcsoa/gen/Internal_Query/_2013_05/__init__.py
+-rw-r--r--   0        0        0     1992 2022-10-20 12:42:27.016526 tcsoa-0.9.1/tcsoa/gen/Internal_Query/_2013_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.751045 tcsoa-0.9.1/tcsoa/gen/Internal_Query/_2014_10/__init__.py
+-rw-r--r--   0        0        0     2189 2022-10-20 12:42:27.044534 tcsoa-0.9.1/tcsoa/gen/Internal_Query/_2014_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.689045 tcsoa-0.9.1/tcsoa/gen/Internal_Query/__init__.py
+-rw-r--r--   0        0        0      732 2022-10-20 12:41:55.993311 tcsoa-0.9.1/tcsoa/gen/Internal_Query/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.794044 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2007_06/__init__.py
+-rw-r--r--   0        0        0     1878 2022-10-20 12:42:27.075540 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.558030 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2007_09/__init__.py
+-rw-r--r--   0        0        0     1439 2022-10-20 12:42:27.104536 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2007_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.936066 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2008_03/__init__.py
+-rw-r--r--   0        0        0     2316 2022-10-20 12:42:27.133540 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2008_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.957067 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2009_01/__init__.py
+-rw-r--r--   0        0        0    15626 2022-10-20 12:42:27.182555 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2009_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.765045 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2009_04/__init__.py
+-rw-r--r--   0        0        0     5056 2022-10-20 12:42:27.216544 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2009_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.869055 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2009_05/__init__.py
+-rw-r--r--   0        0        0     7314 2022-10-20 12:42:27.256549 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2009_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.972071 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2010_04/__init__.py
+-rw-r--r--   0        0        0     4821 2022-10-20 12:42:27.290564 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.823056 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/__init__.py
+-rw-r--r--   0        0        0     2059 2022-10-20 12:41:56.032313 tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.836052 tcsoa-0.9.1/tcsoa/gen/Internal_Reports/_2007_06/__init__.py
+-rw-r--r--   0        0        0     6878 2022-10-20 12:42:27.330554 tcsoa-0.9.1/tcsoa/gen/Internal_Reports/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.571032 tcsoa-0.9.1/tcsoa/gen/Internal_Reports/__init__.py
+-rw-r--r--   0        0        0      575 2022-10-20 12:41:56.049323 tcsoa-0.9.1/tcsoa/gen/Internal_Reports/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.980065 tcsoa-0.9.1/tcsoa/gen/Internal_Requirementsmanagement/_2009_10/__init__.py
+-rw-r--r--   0        0        0     1710 2022-10-20 12:42:27.363560 tcsoa-0.9.1/tcsoa/gen/Internal_Requirementsmanagement/_2009_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.685041 tcsoa-0.9.1/tcsoa/gen/Internal_Requirementsmanagement/_2012_02/__init__.py
+-rw-r--r--   0        0        0     2021 2022-10-20 12:42:27.391567 tcsoa-0.9.1/tcsoa/gen/Internal_Requirementsmanagement/_2012_02/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.676048 tcsoa-0.9.1/tcsoa/gen/Internal_Requirementsmanagement/_2012_10/__init__.py
+-rw-r--r--   0        0        0     2966 2022-10-20 12:42:27.422575 tcsoa-0.9.1/tcsoa/gen/Internal_Requirementsmanagement/_2012_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.545030 tcsoa-0.9.1/tcsoa/gen/Internal_Requirementsmanagement/__init__.py
+-rw-r--r--   0        0        0      631 2022-10-20 12:41:56.059318 tcsoa-0.9.1/tcsoa/gen/Internal_Requirementsmanagement/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.624029 tcsoa-0.9.1/tcsoa/gen/Internal_RevRuleMgmt/_2019_12/__init__.py
+-rw-r--r--   0        0        0     3152 2022-10-20 12:42:27.450582 tcsoa-0.9.1/tcsoa/gen/Internal_RevRuleMgmt/_2019_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.686038 tcsoa-0.9.1/tcsoa/gen/Internal_RevRuleMgmt/__init__.py
+-rw-r--r--   0        0        0      313 2022-10-20 12:41:56.067319 tcsoa-0.9.1/tcsoa/gen/Internal_RevRuleMgmt/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.891059 tcsoa-0.9.1/tcsoa/gen/Internal_Search/_2020_12/__init__.py
+-rw-r--r--   0        0        0     8337 2022-10-20 12:42:27.486577 tcsoa-0.9.1/tcsoa/gen/Internal_Search/_2020_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.824055 tcsoa-0.9.1/tcsoa/gen/Internal_Search/__init__.py
+-rw-r--r--   0        0        0      466 2022-10-20 12:41:56.079328 tcsoa-0.9.1/tcsoa/gen/Internal_Search/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.824055 tcsoa-0.9.1/tcsoa/gen/Internal_Security/_2017_12/__init__.py
+-rw-r--r--   0        0        0     1151 2022-10-20 12:42:27.515590 tcsoa-0.9.1/tcsoa/gen/Internal_Security/_2017_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.008068 tcsoa-0.9.1/tcsoa/gen/Internal_Security/__init__.py
+-rw-r--r--   0        0        0      216 2022-10-20 12:41:56.085324 tcsoa-0.9.1/tcsoa/gen/Internal_Security/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.739050 tcsoa-0.9.1/tcsoa/gen/Internal_Structure/_2020_12/__init__.py
+-rw-r--r--   0        0        0     1124 2022-10-20 12:42:27.543577 tcsoa-0.9.1/tcsoa/gen/Internal_Structure/_2020_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.983065 tcsoa-0.9.1/tcsoa/gen/Internal_Structure/__init__.py
+-rw-r--r--   0        0        0      205 2022-10-20 12:41:56.093331 tcsoa-0.9.1/tcsoa/gen/Internal_Structure/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.904062 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2007_06/__init__.py
+-rw-r--r--   0        0        0    18151 2022-10-20 12:42:27.604578 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.729050 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2007_12/__init__.py
+-rw-r--r--   0        0        0     3859 2022-10-20 12:42:27.636583 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2007_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.811050 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2008_03/__init__.py
+-rw-r--r--   0        0        0     1067 2022-10-20 12:42:27.666592 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2008_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.940067 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2008_05/__init__.py
+-rw-r--r--   0        0        0     3841 2022-10-20 12:42:27.701594 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2008_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.593027 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0     2042 2022-10-20 12:42:27.734603 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.827050 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2009_10/__init__.py
+-rw-r--r--   0        0        0     3168 2022-10-20 12:42:27.768596 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2009_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.649034 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2010_04/__init__.py
+-rw-r--r--   0        0        0     5988 2022-10-20 12:42:27.802610 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.632037 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2010_09/__init__.py
+-rw-r--r--   0        0        0     1017 2022-10-20 12:42:27.832604 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2010_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.969063 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2011_06/__init__.py
+-rw-r--r--   0        0        0    10947 2022-10-20 12:42:27.886636 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.990099 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2012_02/__init__.py
+-rw-r--r--   0        0        0     1971 2022-10-20 12:42:27.918619 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2012_02/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.806049 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2012_09/__init__.py
+-rw-r--r--   0        0        0     1168 2022-10-20 12:42:27.947613 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.704043 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2013_05/__init__.py
+-rw-r--r--   0        0        0     6389 2022-10-20 12:42:27.984616 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2013_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.977064 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2013_12/__init__.py
+-rw-r--r--   0        0        0     6530 2022-10-20 12:42:28.021626 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2013_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.873056 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2014_12/__init__.py
+-rw-r--r--   0        0        0    12680 2022-10-20 12:42:28.073626 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2014_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.602028 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2015_10/__init__.py
+-rw-r--r--   0        0        0     2494 2022-10-20 12:42:28.103646 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2015_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.972071 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2016_03/__init__.py
+-rw-r--r--   0        0        0     2739 2022-10-20 12:42:28.137638 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2016_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.814050 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2016_10/__init__.py
+-rw-r--r--   0        0        0     6685 2022-10-20 12:42:28.168640 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2016_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.559030 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2017_05/__init__.py
+-rw-r--r--   0        0        0     7427 2022-10-20 12:42:28.216638 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2017_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.779053 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2018_11/__init__.py
+-rw-r--r--   0        0        0     5557 2022-10-20 12:42:28.256642 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2018_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.655037 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2019_06/__init__.py
+-rw-r--r--   0        0        0     1620 2022-10-20 12:42:28.287643 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2019_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.831050 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2020_05/__init__.py
+-rw-r--r--   0        0        0     2774 2022-10-20 12:42:28.320656 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2020_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.755045 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/__init__.py
+-rw-r--r--   0        0        0     7990 2022-10-20 12:41:56.205330 tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.724039 tcsoa-0.9.1/tcsoa/gen/Internal_TCXMLImportExport/_2020_12/__init__.py
+-rw-r--r--   0        0        0     3247 2022-10-20 12:42:28.353656 tcsoa-0.9.1/tcsoa/gen/Internal_TCXMLImportExport/_2020_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.001066 tcsoa-0.9.1/tcsoa/gen/Internal_TCXMLImportExport/__init__.py
+-rw-r--r--   0        0        0      443 2022-10-20 12:41:56.215333 tcsoa-0.9.1/tcsoa/gen/Internal_TCXMLImportExport/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.981072 tcsoa-0.9.1/tcsoa/gen/Internal_Translation/_2007_06/__init__.py
+-rw-r--r--   0        0        0     4024 2022-10-20 12:42:28.390653 tcsoa-0.9.1/tcsoa/gen/Internal_Translation/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.945063 tcsoa-0.9.1/tcsoa/gen/Internal_Translation/__init__.py
+-rw-r--r--   0        0        0      421 2022-10-20 12:41:56.225335 tcsoa-0.9.1/tcsoa/gen/Internal_Translation/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.863060 tcsoa-0.9.1/tcsoa/gen/Internal_UiConfig/_2014_11/__init__.py
+-rw-r--r--   0        0        0      924 2022-10-20 12:42:28.421657 tcsoa-0.9.1/tcsoa/gen/Internal_UiConfig/_2014_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.709040 tcsoa-0.9.1/tcsoa/gen/Internal_UiConfig/__init__.py
+-rw-r--r--   0        0        0      198 2022-10-20 12:41:56.232336 tcsoa-0.9.1/tcsoa/gen/Internal_UiConfig/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.949068 tcsoa-0.9.1/tcsoa/gen/Internal_Validation/_2007_06/__init__.py
+-rw-r--r--   0        0        0     6911 2022-10-20 12:42:28.456658 tcsoa-0.9.1/tcsoa/gen/Internal_Validation/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.595030 tcsoa-0.9.1/tcsoa/gen/Internal_Validation/_2008_06/__init__.py
+-rw-r--r--   0        0        0     4109 2022-10-20 12:42:28.489667 tcsoa-0.9.1/tcsoa/gen/Internal_Validation/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.995072 tcsoa-0.9.1/tcsoa/gen/Internal_Validation/_2010_04/__init__.py
+-rw-r--r--   0        0        0     6863 2022-10-20 12:42:28.523672 tcsoa-0.9.1/tcsoa/gen/Internal_Validation/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.977064 tcsoa-0.9.1/tcsoa/gen/Internal_Validation/_2012_02/__init__.py
+-rw-r--r--   0        0        0     3039 2022-10-20 12:42:28.558670 tcsoa-0.9.1/tcsoa/gen/Internal_Validation/_2012_02/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.840051 tcsoa-0.9.1/tcsoa/gen/Internal_Validation/__init__.py
+-rw-r--r--   0        0        0     1151 2022-10-20 12:41:56.257333 tcsoa-0.9.1/tcsoa/gen/Internal_Validation/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.992071 tcsoa-0.9.1/tcsoa/gen/Internal_Vendormanagement/_2008_05/__init__.py
+-rw-r--r--   0        0        0     3038 2022-10-20 12:42:28.686687 tcsoa-0.9.1/tcsoa/gen/Internal_Vendormanagement/_2008_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.942067 tcsoa-0.9.1/tcsoa/gen/Internal_Vendormanagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0     1103 2022-10-20 12:42:28.714681 tcsoa-0.9.1/tcsoa/gen/Internal_Vendormanagement/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.947068 tcsoa-0.9.1/tcsoa/gen/Internal_Vendormanagement/__init__.py
+-rw-r--r--   0        0        0      441 2022-10-20 12:41:56.284342 tcsoa-0.9.1/tcsoa/gen/Internal_Vendormanagement/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.795051 tcsoa-0.9.1/tcsoa/gen/Internal_VendorManagementAW/_2019_12/__init__.py
+-rw-r--r--   0        0        0     3174 2022-10-20 12:42:28.593673 tcsoa-0.9.1/tcsoa/gen/Internal_VendorManagementAW/_2019_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.864060 tcsoa-0.9.1/tcsoa/gen/Internal_VendorManagementAW/_2020_05/__init__.py
+-rw-r--r--   0        0        0     2506 2022-10-20 12:42:28.627674 tcsoa-0.9.1/tcsoa/gen/Internal_VendorManagementAW/_2020_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.660035 tcsoa-0.9.1/tcsoa/gen/Internal_VendorManagementAW/_2020_12/__init__.py
+-rw-r--r--   0        0        0      908 2022-10-20 12:42:28.656686 tcsoa-0.9.1/tcsoa/gen/Internal_VendorManagementAW/_2020_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.880064 tcsoa-0.9.1/tcsoa/gen/Internal_VendorManagementAW/__init__.py
+-rw-r--r--   0        0        0      946 2022-10-20 12:41:56.274341 tcsoa-0.9.1/tcsoa/gen/Internal_VendorManagementAW/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.888056 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2008_06/__init__.py
+-rw-r--r--   0        0        0    86551 2022-10-20 12:42:28.781696 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.675045 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2010_04/__init__.py
+-rw-r--r--   0        0        0     4872 2022-10-20 12:42:28.810699 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.857059 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2010_09/__init__.py
+-rw-r--r--   0        0        0    40577 2022-10-20 12:42:28.857717 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2010_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.724039 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2011_12/__init__.py
+-rw-r--r--   0        0        0     5475 2022-10-20 12:42:28.884697 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2011_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.950068 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2012_10/__init__.py
+-rw-r--r--   0        0        0     4994 2022-10-20 12:42:28.915705 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2012_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.879055 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2017_05/__init__.py
+-rw-r--r--   0        0        0     9476 2022-10-20 12:42:28.945715 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2017_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.707045 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2018_11/__init__.py
+-rw-r--r--   0        0        0     4916 2022-10-20 12:42:28.974705 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2018_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.865059 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/__init__.py
+-rw-r--r--   0        0        0     2433 2022-10-20 12:41:56.335343 tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.658041 tcsoa-0.9.1/tcsoa/gen/Internal_Workflow/_2013_05/__init__.py
+-rw-r--r--   0        0        0     1678 2022-10-20 12:42:29.006718 tcsoa-0.9.1/tcsoa/gen/Internal_Workflow/_2013_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.679048 tcsoa-0.9.1/tcsoa/gen/Internal_Workflow/_2017_11/__init__.py
+-rw-r--r--   0        0        0     1592 2022-10-20 12:42:29.035726 tcsoa-0.9.1/tcsoa/gen/Internal_Workflow/_2017_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.553037 tcsoa-0.9.1/tcsoa/gen/Internal_Workflow/__init__.py
+-rw-r--r--   0        0        0      341 2022-10-20 12:41:56.346350 tcsoa-0.9.1/tcsoa/gen/Internal_Workflow/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.939068 tcsoa-0.9.1/tcsoa/gen/Internal_Workflowaw/_2020_12/__init__.py
+-rw-r--r--   0        0        0     2806 2022-10-20 12:42:29.070716 tcsoa-0.9.1/tcsoa/gen/Internal_Workflowaw/_2020_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.664040 tcsoa-0.9.1/tcsoa/gen/Internal_Workflowaw/__init__.py
+-rw-r--r--   0        0        0      296 2022-10-20 12:41:56.354349 tcsoa-0.9.1/tcsoa/gen/Internal_Workflowaw/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.004068 tcsoa-0.9.1/tcsoa/gen/Internal_XlsBom/_2020_12/__init__.py
+-rw-r--r--   0        0        0     4684 2022-10-20 12:42:29.106718 tcsoa-0.9.1/tcsoa/gen/Internal_XlsBom/_2020_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.715046 tcsoa-0.9.1/tcsoa/gen/Internal_XlsBom/__init__.py
+-rw-r--r--   0        0        0      372 2022-10-20 12:41:56.363352 tcsoa-0.9.1/tcsoa/gen/Internal_XlsBom/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.662042 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2008_06/__init__.py
+-rw-r--r--   0        0        0      742 2022-10-20 12:42:55.474190 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2008_06/Core.py
+-rw-r--r--   0        0        0     4007 2022-10-20 12:42:55.531190 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2008_06/DataManagement.py
+-rw-r--r--   0        0        0     4299 2022-10-20 12:42:29.151724 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2008_06/services.py
+-rw-r--r--   0        0        0     2672 2022-10-20 12:42:55.581194 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2008_06/TimeManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.787047 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2008_12/__init__.py
+-rw-r--r--   0        0        0     2393 2022-10-20 12:42:55.624207 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2008_12/IPAManagement.py
+-rw-r--r--   0        0        0     2608 2022-10-20 12:42:29.187726 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2008_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.615033 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_06/__init__.py
+-rw-r--r--   0        0        0     6507 2022-10-20 12:42:29.229732 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_06/services.py
+-rw-r--r--   0        0        0     3867 2022-10-20 12:42:55.679197 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_06/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.567031 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/__init__.py
+-rw-r--r--   0        0        0     5002 2022-10-20 12:42:55.735204 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/DataManagement.py
+-rw-r--r--   0        0        0     3663 2022-10-20 12:42:55.795209 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/MFGPropertyCollector.py
+-rw-r--r--   0        0        0     4241 2022-10-20 12:42:55.872219 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/Model.py
+-rw-r--r--   0        0        0     5501 2022-10-20 12:42:55.941231 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/ModelDefinitions.py
+-rw-r--r--   0        0        0    12624 2022-10-20 12:42:29.318745 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/services.py
+-rw-r--r--   0        0        0     2532 2022-10-20 12:42:55.978230 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/StructureManagement.py
+-rw-r--r--   0        0        0    15212 2022-10-20 12:42:56.121240 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/StructureSearch.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.772051 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2010_09/__init__.py
+-rw-r--r--   0        0        0     2732 2022-10-20 12:42:56.169244 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2010_09/Core.py
+-rw-r--r--   0        0        0      932 2022-10-20 12:42:56.200246 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2010_09/ImportExport.py
+-rw-r--r--   0        0        0     5522 2022-10-20 12:42:29.368745 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2010_09/services.py
+-rw-r--r--   0        0        0     2623 2022-10-20 12:42:56.241255 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2010_09/TimeManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.834055 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2011_06/__init__.py
+-rw-r--r--   0        0        0     2831 2022-10-20 12:42:56.287284 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2011_06/DataManagement.py
+-rw-r--r--   0        0        0     3809 2022-10-20 12:42:29.413767 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2011_06/services.py
+-rw-r--r--   0        0        0     1459 2022-10-20 12:42:56.325266 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2011_06/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.822046 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_02/__init__.py
+-rw-r--r--   0        0        0    13085 2022-10-20 12:42:56.441276 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_02/Constraints.py
+-rw-r--r--   0        0        0     9281 2022-10-20 12:42:56.540284 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_02/DataManagement.py
+-rw-r--r--   0        0        0     1323 2022-10-20 12:42:56.577288 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_02/IPAManagement.py
+-rw-r--r--   0        0        0     4670 2022-10-20 12:42:56.633293 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_02/Model.py
+-rw-r--r--   0        0        0    16739 2022-10-20 12:42:29.489763 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_02/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.996070 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_09/__init__.py
+-rw-r--r--   0        0        0     2417 2022-10-20 12:42:56.675291 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_09/DataManagement.py
+-rw-r--r--   0        0        0     2665 2022-10-20 12:42:29.528768 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_09/services.py
+-rw-r--r--   0        0        0     2777 2022-10-20 12:42:56.726309 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_09/Validation.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.784047 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/__init__.py
+-rw-r--r--   0        0        0     4065 2022-10-20 12:42:56.769303 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/Core.py
+-rw-r--r--   0        0        0     3173 2022-10-20 12:42:56.817307 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/DataManagement.py
+-rw-r--r--   0        0        0     2488 2022-10-20 12:42:56.932314 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/ImportExport.py
+-rw-r--r--   0        0        0     7953 2022-10-20 12:42:56.893311 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/IPAManagement.py
+-rw-r--r--   0        0        0    16030 2022-10-20 12:42:29.609778 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/services.py
+-rw-r--r--   0        0        0     1867 2022-10-20 12:42:56.969327 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/StructureManagement.py
+-rw-r--r--   0        0        0      808 2022-10-20 12:42:56.999328 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/StructureSearch.py
+-rw-r--r--   0        0        0     6991 2022-10-20 12:42:57.046330 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/TimeWayPlan.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.675045 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_12/__init__.py
+-rw-r--r--   0        0        0     2892 2022-10-20 12:42:57.094356 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_12/Model.py
+-rw-r--r--   0        0        0     5391 2022-10-20 12:42:57.145341 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_12/ResourceManagement.py
+-rw-r--r--   0        0        0     9586 2022-10-20 12:42:29.653772 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.004068 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_06/__init__.py
+-rw-r--r--   0        0        0     9722 2022-10-20 12:42:57.211341 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_06/DataManagement.py
+-rw-r--r--   0        0        0     1198 2022-10-20 12:42:57.242352 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_06/ResourceManagement.py
+-rw-r--r--   0        0        0    10941 2022-10-20 12:42:29.701774 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_06/services.py
+-rw-r--r--   0        0        0      930 2022-10-20 12:42:57.274360 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_06/StructureSearch.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.661045 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_12/__init__.py
+-rw-r--r--   0        0        0     5016 2022-10-20 12:42:57.338359 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_12/IPAManagement.py
+-rw-r--r--   0        0        0     1984 2022-10-20 12:42:57.380362 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_12/Model.py
+-rw-r--r--   0        0        0    10871 2022-10-20 12:42:29.756790 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_12/services.py
+-rw-r--r--   0        0        0     8254 2022-10-20 12:42:57.443366 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_12/StructureSearch.py
+-rw-r--r--   0        0        0     5967 2022-10-20 12:42:57.484372 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_12/Validation.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.788046 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2015_03/__init__.py
+-rw-r--r--   0        0        0     3142 2022-10-20 12:42:29.786783 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2015_03/services.py
+-rw-r--r--   0        0        0     3452 2022-10-20 12:42:57.517370 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2015_03/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.570034 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2015_10/__init__.py
+-rw-r--r--   0        0        0     1979 2022-10-20 12:42:57.554377 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2015_10/ImportExport.py
+-rw-r--r--   0        0        0     3131 2022-10-20 12:42:29.820788 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2015_10/services.py
+-rw-r--r--   0        0        0     5831 2022-10-20 12:42:57.595382 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2015_10/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.584030 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2016_03/__init__.py
+-rw-r--r--   0        0        0     2953 2022-10-20 12:42:57.633381 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2016_03/ImportExport.py
+-rw-r--r--   0        0        0     4080 2022-10-20 12:42:29.850797 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2016_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.915058 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2017_05/__init__.py
+-rw-r--r--   0        0        0     1114 2022-10-20 12:42:57.659390 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2017_05/ImportExport.py
+-rw-r--r--   0        0        0     2630 2022-10-20 12:42:29.884796 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2017_05/services.py
+-rw-r--r--   0        0        0     1220 2022-10-20 12:42:57.691395 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2017_05/Validation.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.990099 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2017_11/__init__.py
+-rw-r--r--   0        0        0    10399 2022-10-20 12:42:57.757393 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2017_11/DataManagement.py
+-rw-r--r--   0        0        0     7317 2022-10-20 12:42:29.920801 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2017_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.564032 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2018_06/__init__.py
+-rw-r--r--   0        0        0     3063 2022-10-20 12:42:57.794399 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2018_06/DataManagement.py
+-rw-r--r--   0        0        0     2535 2022-10-20 12:42:29.949799 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2018_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.918071 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2018_11/__init__.py
+-rw-r--r--   0        0        0     2965 2022-10-20 12:42:29.980803 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2018_11/services.py
+-rw-r--r--   0        0        0     7415 2022-10-20 12:42:57.864407 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2018_11/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.898059 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2019_06/__init__.py
+-rw-r--r--   0        0        0     1679 2022-10-20 12:42:57.898410 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2019_06/DataManagement.py
+-rw-r--r--   0        0        0     2860 2022-10-20 12:42:30.014816 tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2019_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.985066 tcsoa-0.9.1/tcsoa/gen/Manufacturing/__init__.py
+-rw-r--r--   0        0        0    11688 2022-10-20 12:41:56.555362 tcsoa-0.9.1/tcsoa/gen/Manufacturing/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.762045 tcsoa-0.9.1/tcsoa/gen/Multisite/_2007_06/__init__.py
+-rw-r--r--   0        0        0     1265 2022-10-20 12:42:57.930433 tcsoa-0.9.1/tcsoa/gen/Multisite/_2007_06/ImportExport.py
+-rw-r--r--   0        0        0     2257 2022-10-20 12:42:30.043818 tcsoa-0.9.1/tcsoa/gen/Multisite/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.603029 tcsoa-0.9.1/tcsoa/gen/Multisite/_2011_06/__init__.py
+-rw-r--r--   0        0        0     4459 2022-10-20 12:42:30.076818 tcsoa-0.9.1/tcsoa/gen/Multisite/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.639047 tcsoa-0.9.1/tcsoa/gen/Multisite/_2014_10/__init__.py
+-rw-r--r--   0        0        0    15651 2022-10-20 12:42:58.003422 tcsoa-0.9.1/tcsoa/gen/Multisite/_2014_10/ImportExportTCXML.py
+-rw-r--r--   0        0        0     4310 2022-10-20 12:42:30.111822 tcsoa-0.9.1/tcsoa/gen/Multisite/_2014_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.692046 tcsoa-0.9.1/tcsoa/gen/Multisite/_2019_06/__init__.py
+-rw-r--r--   0        0        0     2426 2022-10-20 12:42:58.046426 tcsoa-0.9.1/tcsoa/gen/Multisite/_2019_06/ImportExportTCXML.py
+-rw-r--r--   0        0        0     1359 2022-10-20 12:42:58.078432 tcsoa-0.9.1/tcsoa/gen/Multisite/_2019_06/Search.py
+-rw-r--r--   0        0        0     5558 2022-10-20 12:42:30.152834 tcsoa-0.9.1/tcsoa/gen/Multisite/_2019_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.997071 tcsoa-0.9.1/tcsoa/gen/Multisite/__init__.py
+-rw-r--r--   0        0        0      953 2022-10-20 12:41:56.576367 tcsoa-0.9.1/tcsoa/gen/Multisite/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.623033 tcsoa-0.9.1/tcsoa/gen/Notification/_2014_10/__init__.py
+-rw-r--r--   0        0        0     7060 2022-10-20 12:42:30.189828 tcsoa-0.9.1/tcsoa/gen/Notification/_2014_10/services.py
+-rw-r--r--   0        0        0    10914 2022-10-20 12:42:18.324716 tcsoa-0.9.1/tcsoa/gen/Notification/_2014_10/SubscriptionManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.829051 tcsoa-0.9.1/tcsoa/gen/Notification/__init__.py
+-rw-r--r--   0        0        0      377 2022-10-20 12:41:56.588368 tcsoa-0.9.1/tcsoa/gen/Notification/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.817058 tcsoa-0.9.1/tcsoa/gen/OfficeOnline/_2017_11/__init__.py
+-rw-r--r--   0        0        0     2123 2022-10-20 12:42:30.255829 tcsoa-0.9.1/tcsoa/gen/OfficeOnline/_2017_11/OfficeOnline.py
+-rw-r--r--   0        0        0     1768 2022-10-20 12:42:30.217824 tcsoa-0.9.1/tcsoa/gen/OfficeOnline/_2017_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.677047 tcsoa-0.9.1/tcsoa/gen/OfficeOnline/__init__.py
+-rw-r--r--   0        0        0      199 2022-10-20 12:41:56.594381 tcsoa-0.9.1/tcsoa/gen/OfficeOnline/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.979064 tcsoa-0.9.1/tcsoa/gen/Participant/_2018_11/__init__.py
+-rw-r--r--   0        0        0     6357 2022-10-20 12:42:18.388756 tcsoa-0.9.1/tcsoa/gen/Participant/_2018_11/Participant.py
+-rw-r--r--   0        0        0     3611 2022-10-20 12:42:30.288842 tcsoa-0.9.1/tcsoa/gen/Participant/_2018_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.793051 tcsoa-0.9.1/tcsoa/gen/Participant/__init__.py
+-rw-r--r--   0        0        0      304 2022-10-20 12:41:56.604380 tcsoa-0.9.1/tcsoa/gen/Participant/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.833056 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_01/__init__.py
+-rw-r--r--   0        0        0     5604 2022-10-20 12:42:58.139433 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_01/ScheduleManagement.py
+-rw-r--r--   0        0        0     6274 2022-10-20 12:42:30.710876 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.704043 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_06/__init__.py
+-rw-r--r--   0        0        0     5847 2022-10-20 12:42:58.202436 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_06/ScheduleManagement.py
+-rw-r--r--   0        0        0     5070 2022-10-20 12:42:30.749879 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.596030 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_12/__init__.py
+-rw-r--r--   0        0        0     2706 2022-10-20 12:42:58.249434 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_12/ScheduleManagement.py
+-rw-r--r--   0        0        0      853 2022-10-20 12:42:30.780882 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.706044 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0    17407 2022-10-20 12:42:58.363453 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2008_06/ScheduleManagement.py
+-rw-r--r--   0        0        0     5856 2022-10-20 12:42:30.818883 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.944079 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2009_10/__init__.py
+-rw-r--r--   0        0        0     4732 2022-10-20 12:42:58.413452 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2009_10/ScheduleManagement.py
+-rw-r--r--   0        0        0     1637 2022-10-20 12:42:30.850884 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2009_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.863060 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_02/__init__.py
+-rw-r--r--   0        0        0     4207 2022-10-20 12:42:58.483459 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_02/ScheduleManagement.py
+-rw-r--r--   0        0        0      844 2022-10-20 12:42:30.879887 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_02/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.668044 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_06/__init__.py
+-rw-r--r--   0        0        0    16136 2022-10-20 12:42:58.654474 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_06/ScheduleManagement.py
+-rw-r--r--   0        0        0    10145 2022-10-20 12:42:30.925896 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.722046 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_12/__init__.py
+-rw-r--r--   0        0        0     1128 2022-10-20 12:42:58.687477 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_12/ScheduleManagement.py
+-rw-r--r--   0        0        0     1202 2022-10-20 12:42:30.954892 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.878055 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2012_02/__init__.py
+-rw-r--r--   0        0        0     7126 2022-10-20 12:42:58.777493 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2012_02/ScheduleManagement.py
+-rw-r--r--   0        0        0    15276 2022-10-20 12:42:31.033901 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2012_02/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.565032 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2012_09/__init__.py
+-rw-r--r--   0        0        0      819 2022-10-20 12:42:58.805488 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2012_09/ScheduleManagement.py
+-rw-r--r--   0        0        0     1599 2022-10-20 12:42:31.065910 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.700049 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2014_06/__init__.py
+-rw-r--r--   0        0        0     3034 2022-10-20 12:42:58.849499 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2014_06/ScheduleManagement.py
+-rw-r--r--   0        0        0     1107 2022-10-20 12:42:31.099908 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2014_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.747043 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2014_10/__init__.py
+-rw-r--r--   0        0        0    10136 2022-10-20 12:42:58.943510 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2014_10/ScheduleManagement.py
+-rw-r--r--   0        0        0    10125 2022-10-20 12:42:31.145910 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2014_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.896060 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2015_07/__init__.py
+-rw-r--r--   0        0        0      745 2022-10-20 12:42:58.970505 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2015_07/ScheduleManagement.py
+-rw-r--r--   0        0        0     2625 2022-10-20 12:42:31.180917 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2015_07/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.593027 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2016_04/__init__.py
+-rw-r--r--   0        0        0     1706 2022-10-20 12:42:31.210919 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2016_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.770065 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2017_11/__init__.py
+-rw-r--r--   0        0        0      860 2022-10-20 12:42:58.997522 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2017_11/ScheduleManagement.py
+-rw-r--r--   0        0        0     2157 2022-10-20 12:42:31.238942 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2017_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.780047 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2018_11/__init__.py
+-rw-r--r--   0        0        0     1780 2022-10-20 12:42:31.267922 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2018_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.738043 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/__init__.py
+-rw-r--r--   0        0        0     5095 2022-10-20 12:41:56.718383 tcsoa-0.9.1/tcsoa/gen/ProjectManagement/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.617030 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2015_07/__init__.py
+-rw-r--r--   0        0        0     2361 2022-10-20 12:42:32.837067 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2015_07/ScheduleManagementAw.py
+-rw-r--r--   0        0        0     1021 2022-10-20 12:42:31.294924 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2015_07/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.910058 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2016_12/__init__.py
+-rw-r--r--   0        0        0     4660 2022-10-20 12:42:32.880072 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2016_12/ScheduleManagementAw.py
+-rw-r--r--   0        0        0     4424 2022-10-20 12:42:31.329933 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2016_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.751045 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2017_06/__init__.py
+-rw-r--r--   0        0        0      712 2022-10-20 12:42:32.907079 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2017_06/ScheduleManagementAw.py
+-rw-r--r--   0        0        0     2110 2022-10-20 12:42:31.358931 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2017_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.655037 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2018_12/__init__.py
+-rw-r--r--   0        0        0     8743 2022-10-20 12:42:32.981083 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2018_12/ScheduleManagementAw.py
+-rw-r--r--   0        0        0     6685 2022-10-20 12:42:31.399940 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2018_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.644039 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2019_06/__init__.py
+-rw-r--r--   0        0        0     3980 2022-10-20 12:42:33.026088 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2019_06/ScheduleManagementAw.py
+-rw-r--r--   0        0        0     1955 2022-10-20 12:42:31.430945 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2019_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.826051 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2020_05/__init__.py
+-rw-r--r--   0        0        0     3056 2022-10-20 12:42:33.076090 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2020_05/ScheduleManagementAw.py
+-rw-r--r--   0        0        0     3139 2022-10-20 12:42:31.463944 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2020_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.700049 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/__init__.py
+-rw-r--r--   0        0        0     1747 2022-10-20 12:41:56.754397 tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.611029 tcsoa-0.9.1/tcsoa/gen/Qualification/_2014_06/__init__.py
+-rw-r--r--   0        0        0     3225 2022-10-20 12:42:18.441727 tcsoa-0.9.1/tcsoa/gen/Qualification/_2014_06/QualificationManagement.py
+-rw-r--r--   0        0        0     4289 2022-10-20 12:42:31.500942 tcsoa-0.9.1/tcsoa/gen/Qualification/_2014_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.868058 tcsoa-0.9.1/tcsoa/gen/Qualification/__init__.py
+-rw-r--r--   0        0        0      530 2022-10-20 12:41:56.769398 tcsoa-0.9.1/tcsoa/gen/Qualification/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.589039 tcsoa-0.9.1/tcsoa/gen/Query/_2006_03/__init__.py
+-rw-r--r--   0        0        0     2791 2022-10-20 12:42:59.051511 tcsoa-0.9.1/tcsoa/gen/Query/_2006_03/SavedQuery.py
+-rw-r--r--   0        0        0     4058 2022-10-20 12:42:31.532973 tcsoa-0.9.1/tcsoa/gen/Query/_2006_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.597028 tcsoa-0.9.1/tcsoa/gen/Query/_2007_01/__init__.py
+-rw-r--r--   0        0        0      924 2022-10-20 12:42:59.084522 tcsoa-0.9.1/tcsoa/gen/Query/_2007_01/SavedQuery.py
+-rw-r--r--   0        0        0     3590 2022-10-20 12:42:31.564948 tcsoa-0.9.1/tcsoa/gen/Query/_2007_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.589039 tcsoa-0.9.1/tcsoa/gen/Query/_2007_06/__init__.py
+-rw-r--r--   0        0        0     3437 2022-10-20 12:42:59.132526 tcsoa-0.9.1/tcsoa/gen/Query/_2007_06/Finder.py
+-rw-r--r--   0        0        0     5401 2022-10-20 12:42:59.180524 tcsoa-0.9.1/tcsoa/gen/Query/_2007_06/SavedQuery.py
+-rw-r--r--   0        0        0     4894 2022-10-20 12:42:31.603959 tcsoa-0.9.1/tcsoa/gen/Query/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.837052 tcsoa-0.9.1/tcsoa/gen/Query/_2007_09/__init__.py
+-rw-r--r--   0        0        0     3602 2022-10-20 12:42:59.217528 tcsoa-0.9.1/tcsoa/gen/Query/_2007_09/SavedQuery.py
+-rw-r--r--   0        0        0     1699 2022-10-20 12:42:31.631971 tcsoa-0.9.1/tcsoa/gen/Query/_2007_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.664040 tcsoa-0.9.1/tcsoa/gen/Query/_2008_06/__init__.py
+-rw-r--r--   0        0        0     1961 2022-10-20 12:42:59.245527 tcsoa-0.9.1/tcsoa/gen/Query/_2008_06/SavedQuery.py
+-rw-r--r--   0        0        0     1833 2022-10-20 12:42:31.658965 tcsoa-0.9.1/tcsoa/gen/Query/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.618030 tcsoa-0.9.1/tcsoa/gen/Query/_2010_04/__init__.py
+-rw-r--r--   0        0        0      966 2022-10-20 12:42:59.279539 tcsoa-0.9.1/tcsoa/gen/Query/_2010_04/SavedQuery.py
+-rw-r--r--   0        0        0     1268 2022-10-20 12:42:31.685968 tcsoa-0.9.1/tcsoa/gen/Query/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.954086 tcsoa-0.9.1/tcsoa/gen/Query/_2010_09/__init__.py
+-rw-r--r--   0        0        0     1550 2022-10-20 12:42:59.310562 tcsoa-0.9.1/tcsoa/gen/Query/_2010_09/SavedQuery.py
+-rw-r--r--   0        0        0      913 2022-10-20 12:42:31.713969 tcsoa-0.9.1/tcsoa/gen/Query/_2010_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.924063 tcsoa-0.9.1/tcsoa/gen/Query/_2012_10/__init__.py
+-rw-r--r--   0        0        0     6352 2022-10-20 12:42:59.373543 tcsoa-0.9.1/tcsoa/gen/Query/_2012_10/Finder.py
+-rw-r--r--   0        0        0     2727 2022-10-20 12:42:31.740973 tcsoa-0.9.1/tcsoa/gen/Query/_2012_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.699049 tcsoa-0.9.1/tcsoa/gen/Query/_2013_05/__init__.py
+-rw-r--r--   0        0        0     1214 2022-10-20 12:42:59.399551 tcsoa-0.9.1/tcsoa/gen/Query/_2013_05/SavedQuery.py
+-rw-r--r--   0        0        0      747 2022-10-20 12:42:31.768969 tcsoa-0.9.1/tcsoa/gen/Query/_2013_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.786052 tcsoa-0.9.1/tcsoa/gen/Query/_2014_11/__init__.py
+-rw-r--r--   0        0        0     8606 2022-10-20 12:42:59.460556 tcsoa-0.9.1/tcsoa/gen/Query/_2014_11/Finder.py
+-rw-r--r--   0        0        0     4418 2022-10-20 12:42:31.800974 tcsoa-0.9.1/tcsoa/gen/Query/_2014_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.938068 tcsoa-0.9.1/tcsoa/gen/Query/_2018_11/__init__.py
+-rw-r--r--   0        0        0     1784 2022-10-20 12:42:59.487557 tcsoa-0.9.1/tcsoa/gen/Query/_2018_11/SavedQuery.py
+-rw-r--r--   0        0        0     5364 2022-10-20 12:42:31.830976 tcsoa-0.9.1/tcsoa/gen/Query/_2018_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.013069 tcsoa-0.9.1/tcsoa/gen/Query/_2019_06/__init__.py
+-rw-r--r--   0        0        0     2235 2022-10-20 12:42:59.524555 tcsoa-0.9.1/tcsoa/gen/Query/_2019_06/SavedQuery.py
+-rw-r--r--   0        0        0      812 2022-10-20 12:42:31.859984 tcsoa-0.9.1/tcsoa/gen/Query/_2019_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.632037 tcsoa-0.9.1/tcsoa/gen/Query/_2020_04/__init__.py
+-rw-r--r--   0        0        0     2109 2022-10-20 12:42:59.552564 tcsoa-0.9.1/tcsoa/gen/Query/_2020_04/SavedQuery.py
+-rw-r--r--   0        0        0     4719 2022-10-20 12:42:31.890982 tcsoa-0.9.1/tcsoa/gen/Query/_2020_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.610029 tcsoa-0.9.1/tcsoa/gen/Query/__init__.py
+-rw-r--r--   0        0        0     2346 2022-10-20 12:41:56.809392 tcsoa-0.9.1/tcsoa/gen/Query/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.934070 tcsoa-0.9.1/tcsoa/gen/Rdv/_2008_05/__init__.py
+-rw-r--r--   0        0        0     4737 2022-10-20 12:42:59.614571 tcsoa-0.9.1/tcsoa/gen/Rdv/_2008_05/ContextManagement.py
+-rw-r--r--   0        0        0     4555 2022-10-20 12:42:31.925988 tcsoa-0.9.1/tcsoa/gen/Rdv/_2008_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.854061 tcsoa-0.9.1/tcsoa/gen/Rdv/_2009_04/__init__.py
+-rw-r--r--   0        0        0     1824 2022-10-20 12:42:59.645574 tcsoa-0.9.1/tcsoa/gen/Rdv/_2009_04/ContextManagement.py
+-rw-r--r--   0        0        0     2588 2022-10-20 12:42:31.956983 tcsoa-0.9.1/tcsoa/gen/Rdv/_2009_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.906076 tcsoa-0.9.1/tcsoa/gen/Rdv/_2010_09/__init__.py
+-rw-r--r--   0        0        0     4097 2022-10-20 12:42:59.695576 tcsoa-0.9.1/tcsoa/gen/Rdv/_2010_09/ContextManagement.py
+-rw-r--r--   0        0        0     3719 2022-10-20 12:42:31.987989 tcsoa-0.9.1/tcsoa/gen/Rdv/_2010_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.773053 tcsoa-0.9.1/tcsoa/gen/Rdv/_2012_09/__init__.py
+-rw-r--r--   0        0        0     7785 2022-10-20 12:42:59.766589 tcsoa-0.9.1/tcsoa/gen/Rdv/_2012_09/ContextManagement.py
+-rw-r--r--   0        0        0     9835 2022-10-20 12:42:32.024994 tcsoa-0.9.1/tcsoa/gen/Rdv/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.839051 tcsoa-0.9.1/tcsoa/gen/Rdv/_2013_05/__init__.py
+-rw-r--r--   0        0        0     1284 2022-10-20 12:42:59.793581 tcsoa-0.9.1/tcsoa/gen/Rdv/_2013_05/ContextManagement.py
+-rw-r--r--   0        0        0     3889 2022-10-20 12:42:32.054995 tcsoa-0.9.1/tcsoa/gen/Rdv/_2013_05/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.542030 tcsoa-0.9.1/tcsoa/gen/Rdv/__init__.py
+-rw-r--r--   0        0        0     1196 2022-10-20 12:41:56.836401 tcsoa-0.9.1/tcsoa/gen/Rdv/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.727040 tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/_2012_10/__init__.py
+-rw-r--r--   0        0        0    11494 2022-10-20 12:42:32.659063 tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/_2012_10/NetworkEngine.py
+-rw-r--r--   0        0        0     5852 2022-10-20 12:42:32.090000 tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/_2012_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.554031 tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/_2014_11/__init__.py
+-rw-r--r--   0        0        0     2991 2022-10-20 12:42:32.702056 tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/_2014_11/NetworkEngine.py
+-rw-r--r--   0        0        0     1044 2022-10-20 12:42:32.119001 tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/_2014_11/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.926059 tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/_2019_12/__init__.py
+-rw-r--r--   0        0        0      155 2022-10-20 12:42:32.725088 tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/_2019_12/NetworkEngine.py
+-rw-r--r--   0        0        0     1189 2022-10-20 12:42:32.146004 tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/_2019_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.968069 tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/__init__.py
+-rw-r--r--   0        0        0      639 2022-10-20 12:41:56.852402 tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.853059 tcsoa-0.9.1/tcsoa/gen/Reports/_2007_01/__init__.py
+-rw-r--r--   0        0        0     6686 2022-10-20 12:42:59.877594 tcsoa-0.9.1/tcsoa/gen/Reports/_2007_01/CrfReports.py
+-rw-r--r--   0        0        0     4089 2022-10-20 12:42:32.181015 tcsoa-0.9.1/tcsoa/gen/Reports/_2007_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.929066 tcsoa-0.9.1/tcsoa/gen/Reports/_2007_06/__init__.py
+-rw-r--r--   0        0        0     1118 2022-10-20 12:42:59.914590 tcsoa-0.9.1/tcsoa/gen/Reports/_2007_06/CubeReports.py
+-rw-r--r--   0        0        0     1138 2022-10-20 12:42:32.209019 tcsoa-0.9.1/tcsoa/gen/Reports/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.613030 tcsoa-0.9.1/tcsoa/gen/Reports/_2008_06/__init__.py
+-rw-r--r--   0        0        0     1111 2022-10-20 12:42:59.944597 tcsoa-0.9.1/tcsoa/gen/Reports/_2008_06/CrfReports.py
+-rw-r--r--   0        0        0     1004 2022-10-20 12:42:32.237012 tcsoa-0.9.1/tcsoa/gen/Reports/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.755045 tcsoa-0.9.1/tcsoa/gen/Reports/_2008_12/__init__.py
+-rw-r--r--   0        0        0     3410 2022-10-20 12:42:59.987600 tcsoa-0.9.1/tcsoa/gen/Reports/_2008_12/CrfReports.py
+-rw-r--r--   0        0        0     1676 2022-10-20 12:42:32.268016 tcsoa-0.9.1/tcsoa/gen/Reports/_2008_12/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.859054 tcsoa-0.9.1/tcsoa/gen/Reports/_2010_04/__init__.py
+-rw-r--r--   0        0        0     2292 2022-10-20 12:43:00.018599 tcsoa-0.9.1/tcsoa/gen/Reports/_2010_04/CrfReports.py
+-rw-r--r--   0        0        0     1728 2022-10-20 12:42:32.296018 tcsoa-0.9.1/tcsoa/gen/Reports/_2010_04/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.552030 tcsoa-0.9.1/tcsoa/gen/Reports/_2015_03/__init__.py
+-rw-r--r--   0        0        0     8951 2022-10-20 12:43:00.082605 tcsoa-0.9.1/tcsoa/gen/Reports/_2015_03/CrfReports.py
+-rw-r--r--   0        0        0     4876 2022-10-20 12:42:32.335022 tcsoa-0.9.1/tcsoa/gen/Reports/_2015_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.905061 tcsoa-0.9.1/tcsoa/gen/Reports/_2015_10/__init__.py
+-rw-r--r--   0        0        0      605 2022-10-20 12:43:00.111610 tcsoa-0.9.1/tcsoa/gen/Reports/_2015_10/CrfReports.py
+-rw-r--r--   0        0        0      794 2022-10-20 12:42:32.363033 tcsoa-0.9.1/tcsoa/gen/Reports/_2015_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.780047 tcsoa-0.9.1/tcsoa/gen/Reports/__init__.py
+-rw-r--r--   0        0        0     1372 2022-10-20 12:41:56.877404 tcsoa-0.9.1/tcsoa/gen/Reports/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.647036 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2007_01/__init__.py
+-rw-r--r--   0        0        0    18401 2022-10-20 12:43:00.262633 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2007_01/RequirementsManagement.py
+-rw-r--r--   0        0        0     9494 2022-10-20 12:42:32.401027 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2007_01/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.560032 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0     1021 2022-10-20 12:43:00.288627 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2008_06/RequirementsManagement.py
+-rw-r--r--   0        0        0     1666 2022-10-20 12:42:32.432030 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2008_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.912057 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2009_10/__init__.py
+-rw-r--r--   0        0        0     6003 2022-10-20 12:43:00.351633 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2009_10/RequirementsManagement.py
+-rw-r--r--   0        0        0     3459 2022-10-20 12:42:32.462035 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2009_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.735048 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2010_09/__init__.py
+-rw-r--r--   0        0        0     1487 2022-10-20 12:43:00.381636 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2010_09/RequirementsManagement.py
+-rw-r--r--   0        0        0     3614 2022-10-20 12:42:32.490041 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2010_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.661045 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2011_06/__init__.py
+-rw-r--r--   0        0        0      746 2022-10-20 12:43:00.409649 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2011_06/RequirementsManagement.py
+-rw-r--r--   0        0        0     2363 2022-10-20 12:42:32.520038 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2011_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.948069 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2012_09/__init__.py
+-rw-r--r--   0        0        0      748 2022-10-20 12:43:00.433645 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2012_09/RequirementsManagement.py
+-rw-r--r--   0        0        0     1083 2022-10-20 12:42:32.548051 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2012_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.966070 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/__init__.py
+-rw-r--r--   0        0        0     1198 2022-10-20 12:41:56.899419 tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/services.py
+-rw-r--r--   0        0        0     1442 2022-10-20 12:43:00.491652 tcsoa-0.9.1/tcsoa/gen/Server.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.600027 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2007_06/__init__.py
+-rw-r--r--   0        0        0     8770 2022-10-20 12:43:00.596664 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2007_06/PublishByLink.py
+-rw-r--r--   0        0        0    11093 2022-10-20 12:42:33.122092 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2007_06/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.705043 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_03/__init__.py
+-rw-r--r--   0        0        0     1944 2022-10-20 12:43:00.638666 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_03/Composition.py
+-rw-r--r--   0        0        0      777 2022-10-20 12:42:33.157111 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.923067 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_05/__init__.py
+-rw-r--r--   0        0        0     4347 2022-10-20 12:42:33.197101 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_05/services.py
+-rw-r--r--   0        0        0    15160 2022-10-20 12:43:00.765686 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_05/StructureSearch.py
+-rw-r--r--   0        0        0     1587 2022-10-20 12:43:00.809686 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_05/StructureVerification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.698047 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0    11834 2022-10-20 12:42:33.230102 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_06/services.py
+-rw-r--r--   0        0        0     6561 2022-10-20 12:43:00.887681 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_06/Structure.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.585031 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_12/__init__.py
+-rw-r--r--   0        0        0      857 2022-10-20 12:42:33.260107 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_12/services.py
+-rw-r--r--   0        0        0     1623 2022-10-20 12:43:00.926692 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_12/StructureVerification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.760046 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2010_04/__init__.py
+-rw-r--r--   0        0        0      926 2022-10-20 12:42:33.287115 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2010_04/services.py
+-rw-r--r--   0        0        0     3425 2022-10-20 12:43:00.966693 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2010_04/StructureSearch.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.582039 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2010_09/__init__.py
+-rw-r--r--   0        0        0    20591 2022-10-20 12:42:33.339123 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2010_09/services.py
+-rw-r--r--   0        0        0     4039 2022-10-20 12:43:01.020704 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2010_09/Structure.py
+-rw-r--r--   0        0        0     4465 2022-10-20 12:43:01.060705 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2010_09/StructureSearch.py
+-rw-r--r--   0        0        0    10615 2022-10-20 12:43:01.152707 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2010_09/StructureVerification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.846064 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2011_06/__init__.py
+-rw-r--r--   0        0        0    18660 2022-10-20 12:42:33.375119 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2011_06/services.py
+-rw-r--r--   0        0        0     6370 2022-10-20 12:43:01.236724 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2011_06/Structure.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.625030 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_02/__init__.py
+-rw-r--r--   0        0        0      442 2022-10-20 12:43:01.264720 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_02/IncrementalChange.py
+-rw-r--r--   0        0        0     9436 2022-10-20 12:42:33.435160 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_02/services.py
+-rw-r--r--   0        0        0    30053 2022-10-20 12:43:01.479745 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_02/StructureVerification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.803054 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_09/__init__.py
+-rw-r--r--   0        0        0     5174 2022-10-20 12:43:01.544748 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_09/MassUpdate.py
+-rw-r--r--   0        0        0    11154 2022-10-20 12:42:33.496128 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_09/services.py
+-rw-r--r--   0        0        0     2823 2022-10-20 12:43:01.589756 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_09/Structure.py
+-rw-r--r--   0        0        0    12851 2022-10-20 12:43:01.690758 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_09/VariantManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.839051 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_10/__init__.py
+-rw-r--r--   0        0        0     4994 2022-10-20 12:42:33.534141 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_10/services.py
+-rw-r--r--   0        0        0      557 2022-10-20 12:43:01.718774 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_10/Structure.py
+-rw-r--r--   0        0        0     3763 2022-10-20 12:43:01.773772 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_10/StructureVerification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.906076 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2013_05/__init__.py
+-rw-r--r--   0        0        0      649 2022-10-20 12:43:01.803774 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2013_05/IncrementalChange.py
+-rw-r--r--   0        0        0     9525 2022-10-20 12:42:33.582138 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2013_05/services.py
+-rw-r--r--   0        0        0     5741 2022-10-20 12:43:01.866776 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2013_05/StructureVerification.py
+-rw-r--r--   0        0        0    11258 2022-10-20 12:43:01.959784 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2013_05/VariantManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.914061 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_06/__init__.py
+-rw-r--r--   0        0        0     7057 2022-10-20 12:42:33.616148 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_06/services.py
+-rw-r--r--   0        0        0     2836 2022-10-20 12:43:01.997793 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_06/StructureFilterWithExpand.py
+-rw-r--r--   0        0        0     2734 2022-10-20 12:43:02.037797 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_06/StructureVerification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.897060 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_10/__init__.py
+-rw-r--r--   0        0        0    18834 2022-10-20 12:43:02.205812 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_10/MassUpdate.py
+-rw-r--r--   0        0        0    33903 2022-10-20 12:42:33.679150 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_10/services.py
+-rw-r--r--   0        0        0    15259 2022-10-20 12:43:02.292822 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_10/Structure.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.743042 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_12/__init__.py
+-rw-r--r--   0        0        0     2337 2022-10-20 12:43:02.331832 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_12/Effectivity.py
+-rw-r--r--   0        0        0     4563 2022-10-20 12:42:33.716155 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_12/services.py
+-rw-r--r--   0        0        0    17099 2022-10-20 12:43:02.454827 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_12/StructureSearch.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.562032 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2015_10/__init__.py
+-rw-r--r--   0        0        0     2088 2022-10-20 12:43:02.497834 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2015_10/Effectivity.py
+-rw-r--r--   0        0        0     3962 2022-10-20 12:42:33.751168 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2015_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.569031 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2016_05/__init__.py
+-rw-r--r--   0        0        0     2814 2022-10-20 12:42:33.782157 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2016_05/services.py
+-rw-r--r--   0        0        0     1112 2022-10-20 12:43:02.524835 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2016_05/StructureVerification.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.736044 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2016_09/__init__.py
+-rw-r--r--   0        0        0     1275 2022-10-20 12:43:02.556838 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2016_09/PublishByLink.py
+-rw-r--r--   0        0        0     1025 2022-10-20 12:42:33.821188 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2016_09/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.844064 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2017_05/__init__.py
+-rw-r--r--   0        0        0     3667 2022-10-20 12:42:33.855175 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2017_05/services.py
+-rw-r--r--   0        0        0     5256 2022-10-20 12:43:02.603842 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2017_05/StructureSearch.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.937067 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2018_11/__init__.py
+-rw-r--r--   0        0        0     2667 2022-10-20 12:42:33.882177 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2018_11/services.py
+-rw-r--r--   0        0        0     1669 2022-10-20 12:43:02.631844 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2018_11/Structure.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.759045 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2019_06/__init__.py
+-rw-r--r--   0        0        0     4414 2022-10-20 12:42:33.916175 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2019_06/services.py
+-rw-r--r--   0        0        0     4718 2022-10-20 12:43:02.684857 tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2019_06/VariantManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.619029 tcsoa-0.9.1/tcsoa/gen/StructureManagement/__init__.py
+-rw-r--r--   0        0        0     9234 2022-10-20 12:41:57.063425 tcsoa-0.9.1/tcsoa/gen/StructureManagement/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.597028 tcsoa-0.9.1/tcsoa/gen/Translation/_2007_06/__init__.py
+-rw-r--r--   0        0        0     1222 2022-10-20 12:43:03.691970 tcsoa-0.9.1/tcsoa/gen/Translation/_2007_06/services.py
+-rw-r--r--   0        0        0     1964 2022-10-20 12:43:02.716864 tcsoa-0.9.1/tcsoa/gen/Translation/_2007_06/TranslationManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.769044 tcsoa-0.9.1/tcsoa/gen/Translation/__init__.py
+-rw-r--r--   0        0        0      238 2022-10-20 12:41:57.069426 tcsoa-0.9.1/tcsoa/gen/Translation/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.908058 tcsoa-0.9.1/tcsoa/gen/UiConfig/_2014_11/__init__.py
+-rw-r--r--   0        0        0     3024 2022-10-20 12:43:03.724954 tcsoa-0.9.1/tcsoa/gen/UiConfig/_2014_11/services.py
+-rw-r--r--   0        0        0    12053 2022-10-20 12:42:18.566742 tcsoa-0.9.1/tcsoa/gen/UiConfig/_2014_11/UiConfig.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.887056 tcsoa-0.9.1/tcsoa/gen/UiConfig/_2015_10/__init__.py
+-rw-r--r--   0        0        0     1153 2022-10-20 12:43:03.754958 tcsoa-0.9.1/tcsoa/gen/UiConfig/_2015_10/services.py
+-rw-r--r--   0        0        0     3555 2022-10-20 12:42:18.617753 tcsoa-0.9.1/tcsoa/gen/UiConfig/_2015_10/UiConfig.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.937067 tcsoa-0.9.1/tcsoa/gen/UiConfig/__init__.py
+-rw-r--r--   0        0        0      339 2022-10-20 12:41:57.078427 tcsoa-0.9.1/tcsoa/gen/UiConfig/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.633041 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2007_06/__init__.py
+-rw-r--r--   0        0        0     9039 2022-10-20 12:43:03.796954 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2007_06/services.py
+-rw-r--r--   0        0        0     8816 2022-10-20 12:43:02.791866 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2007_06/VendorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.736044 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2008_06/__init__.py
+-rw-r--r--   0        0        0     3100 2022-10-20 12:43:03.827963 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2008_06/services.py
+-rw-r--r--   0        0        0     4496 2022-10-20 12:43:02.855876 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2008_06/VendorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.899057 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2012_02/__init__.py
+-rw-r--r--   0        0        0     1620 2022-10-20 12:43:03.855960 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2012_02/services.py
+-rw-r--r--   0        0        0     1562 2022-10-20 12:43:02.882875 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2012_02/VendorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.984066 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2012_09/__init__.py
+-rw-r--r--   0        0        0     1405 2022-10-20 12:43:03.883967 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2012_09/services.py
+-rw-r--r--   0        0        0      724 2022-10-20 12:43:02.908882 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2012_09/VendorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.544029 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2016_09/__init__.py
+-rw-r--r--   0        0        0     1123 2022-10-20 12:43:03.911969 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2016_09/services.py
+-rw-r--r--   0        0        0     1327 2022-10-20 12:43:02.935872 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2016_09/VendorManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.564032 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/__init__.py
+-rw-r--r--   0        0        0     1187 2022-10-20 12:41:57.101429 tcsoa-0.9.1/tcsoa/gen/Vendormanagement/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.902061 tcsoa-0.9.1/tcsoa/gen/Visualization/_2011_02/__init__.py
+-rw-r--r--   0        0        0     4962 2022-10-20 12:43:02.983884 tcsoa-0.9.1/tcsoa/gen/Visualization/_2011_02/DataManagement.py
+-rw-r--r--   0        0        0    10675 2022-10-20 12:43:03.949974 tcsoa-0.9.1/tcsoa/gen/Visualization/_2011_02/services.py
+-rw-r--r--   0        0        0     4574 2022-10-20 12:43:03.034892 tcsoa-0.9.1/tcsoa/gen/Visualization/_2011_02/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.557031 tcsoa-0.9.1/tcsoa/gen/Visualization/_2013_05/__init__.py
+-rw-r--r--   0        0        0     5332 2022-10-20 12:43:03.072886 tcsoa-0.9.1/tcsoa/gen/Visualization/_2013_05/DataManagement.py
+-rw-r--r--   0        0        0     8159 2022-10-20 12:43:03.987972 tcsoa-0.9.1/tcsoa/gen/Visualization/_2013_05/services.py
+-rw-r--r--   0        0        0      246 2022-10-20 12:43:03.095894 tcsoa-0.9.1/tcsoa/gen/Visualization/_2013_05/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.872054 tcsoa-0.9.1/tcsoa/gen/Visualization/_2013_12/__init__.py
+-rw-r--r--   0        0        0     4280 2022-10-20 12:43:04.014975 tcsoa-0.9.1/tcsoa/gen/Visualization/_2013_12/services.py
+-rw-r--r--   0        0        0     1614 2022-10-20 12:43:03.122899 tcsoa-0.9.1/tcsoa/gen/Visualization/_2013_12/StructureManagement.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.851061 tcsoa-0.9.1/tcsoa/gen/Visualization/_2016_03/__init__.py
+-rw-r--r--   0        0        0     4340 2022-10-20 12:43:03.170906 tcsoa-0.9.1/tcsoa/gen/Visualization/_2016_03/DataManagement.py
+-rw-r--r--   0        0        0     3758 2022-10-20 12:43:04.043987 tcsoa-0.9.1/tcsoa/gen/Visualization/_2016_03/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.932066 tcsoa-0.9.1/tcsoa/gen/Visualization/__init__.py
+-rw-r--r--   0        0        0     1035 2022-10-20 12:41:57.116431 tcsoa-0.9.1/tcsoa/gen/Visualization/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.671045 tcsoa-0.9.1/tcsoa/gen/Workflow/_2007_06/__init__.py
+-rw-r--r--   0        0        0     1104 2022-10-20 12:43:04.234991 tcsoa-0.9.1/tcsoa/gen/Workflow/_2007_06/services.py
+-rw-r--r--   0        0        0     1367 2022-10-20 12:43:03.212904 tcsoa-0.9.1/tcsoa/gen/Workflow/_2007_06/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.781046 tcsoa-0.9.1/tcsoa/gen/Workflow/_2008_06/__init__.py
+-rw-r--r--   0        0        0    11268 2022-10-20 12:43:04.290019 tcsoa-0.9.1/tcsoa/gen/Workflow/_2008_06/services.py
+-rw-r--r--   0        0        0    13763 2022-10-20 12:43:03.355919 tcsoa-0.9.1/tcsoa/gen/Workflow/_2008_06/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.978069 tcsoa-0.9.1/tcsoa/gen/Workflow/_2010_09/__init__.py
+-rw-r--r--   0        0        0     1573 2022-10-20 12:43:04.324003 tcsoa-0.9.1/tcsoa/gen/Workflow/_2010_09/services.py
+-rw-r--r--   0        0        0     1411 2022-10-20 12:43:03.391921 tcsoa-0.9.1/tcsoa/gen/Workflow/_2010_09/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.886054 tcsoa-0.9.1/tcsoa/gen/Workflow/_2012_10/__init__.py
+-rw-r--r--   0        0        0     1480 2022-10-20 12:43:04.353013 tcsoa-0.9.1/tcsoa/gen/Workflow/_2012_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.752043 tcsoa-0.9.1/tcsoa/gen/Workflow/_2013_05/__init__.py
+-rw-r--r--   0        0        0     1207 2022-10-20 12:43:04.381013 tcsoa-0.9.1/tcsoa/gen/Workflow/_2013_05/services.py
+-rw-r--r--   0        0        0     2043 2022-10-20 12:43:03.431918 tcsoa-0.9.1/tcsoa/gen/Workflow/_2013_05/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.680038 tcsoa-0.9.1/tcsoa/gen/Workflow/_2014_06/__init__.py
+-rw-r--r--   0        0        0     9003 2022-10-20 12:43:04.417018 tcsoa-0.9.1/tcsoa/gen/Workflow/_2014_06/services.py
+-rw-r--r--   0        0        0     6139 2022-10-20 12:43:03.478922 tcsoa-0.9.1/tcsoa/gen/Workflow/_2014_06/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.962068 tcsoa-0.9.1/tcsoa/gen/Workflow/_2014_10/__init__.py
+-rw-r--r--   0        0        0     3249 2022-10-20 12:43:04.447023 tcsoa-0.9.1/tcsoa/gen/Workflow/_2014_10/services.py
+-rw-r--r--   0        0        0     4330 2022-10-20 12:43:03.519928 tcsoa-0.9.1/tcsoa/gen/Workflow/_2014_10/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.723044 tcsoa-0.9.1/tcsoa/gen/Workflow/_2015_07/__init__.py
+-rw-r--r--   0        0        0     2981 2022-10-20 12:43:04.475030 tcsoa-0.9.1/tcsoa/gen/Workflow/_2015_07/services.py
+-rw-r--r--   0        0        0     3719 2022-10-20 12:43:03.552938 tcsoa-0.9.1/tcsoa/gen/Workflow/_2015_07/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.867053 tcsoa-0.9.1/tcsoa/gen/Workflow/_2019_06/__init__.py
+-rw-r--r--   0        0        0     5111 2022-10-20 12:43:04.507020 tcsoa-0.9.1/tcsoa/gen/Workflow/_2019_06/services.py
+-rw-r--r--   0        0        0    10534 2022-10-20 12:43:03.626938 tcsoa-0.9.1/tcsoa/gen/Workflow/_2019_06/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:05.003067 tcsoa-0.9.1/tcsoa/gen/Workflow/_2020_01/__init__.py
+-rw-r--r--   0        0        0     2073 2022-10-20 12:43:04.537030 tcsoa-0.9.1/tcsoa/gen/Workflow/_2020_01/services.py
+-rw-r--r--   0        0        0     2264 2022-10-20 12:43:03.662952 tcsoa-0.9.1/tcsoa/gen/Workflow/_2020_01/Workflow.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.685041 tcsoa-0.9.1/tcsoa/gen/Workflow/__init__.py
+-rw-r--r--   0        0        0     2399 2022-10-20 12:41:57.180431 tcsoa-0.9.1/tcsoa/gen/Workflow/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.953082 tcsoa-0.9.1/tcsoa/gen/WProxy/_2014_10/__init__.py
+-rw-r--r--   0        0        0     1462 2022-10-20 12:42:18.650746 tcsoa-0.9.1/tcsoa/gen/WProxy/_2014_10/ProxyLink.py
+-rw-r--r--   0        0        0     1126 2022-10-20 12:43:04.205997 tcsoa-0.9.1/tcsoa/gen/WProxy/_2014_10/services.py
+-rw-r--r--   0        0        0        0 2022-10-20 12:43:04.805070 tcsoa-0.9.1/tcsoa/gen/WProxy/__init__.py
+-rw-r--r--   0        0        0      191 2022-10-20 12:41:57.123434 tcsoa-0.9.1/tcsoa/gen/WProxy/services.py
+-rw-r--r--   0        0        0     1386 2022-11-21 10:08:01.795581 tcsoa-0.9.1/tcsoa/itk_constants.py
+-rw-r--r--   0        0        0    36468 1970-01-01 00:00:00.000000 tcsoa-0.9.1/setup.py
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 tcsoa-0.9.1/PKG-INFO
```

### Comparing `tcsoa-0.9.0/LICENSE.txt` & `tcsoa-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/pyproject.toml` & `tcsoa-0.9.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tcsoa"
-version = "0.9.0"
+version = "0.9.1"
 description = "A framework generated for the purpose of consuming Teamcenter™ services via Python."
 license = "MIT"
 authors = ["Alexander Haas"]
 include = ["tcsoa/**/*.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `tcsoa-0.9.0/tcsoa/backend.py` & `tcsoa-0.9.1/tcsoa/backend.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/base.py` & `tcsoa-0.9.1/tcsoa/base.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/basics.py` & `tcsoa-0.9.1/tcsoa/basics.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/config.py` & `tcsoa-0.9.1/tcsoa/config.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/exceptions.py` & `tcsoa-0.9.1/tcsoa/exceptions.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/fcc/fcc_client_proxy.py` & `tcsoa-0.9.1/tcsoa/fcc/fcc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/fcc/fcc_wrapper.py` & `tcsoa-0.9.1/tcsoa/fcc/fcc_wrapper.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/fcc/file_management_utility.py` & `tcsoa-0.9.1/tcsoa/fcc/file_management_utility.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,40 +73,42 @@
         file_read_tickets = FileManagementService.getFileReadTickets([named_ref])
         partial_errors = file_read_tickets.serviceData.partialErrors
         result = GetFileResponse(named_ref, full_path, partial_errors)
         if not file_read_tickets.tickets:
             logging.debug('No Tickets returned for the named reference')
             return result
 
-        ticket = next(iter(file_read_tickets.tickets.values()))
-        ticket_uids = cls.fcc.register_tickets([ticket])
-        try:
-            cls.fcc.download_file_to_location("IMD", ticket_uids[0], parent_dir, file_name)
-        finally:
-            cls.fcc.unregister_tickets(ticket_uids)
+        ticket = next(iter(file_read_tickets.tickets.values())) if file_read_tickets.tickets else None
+        if ticket:
+            ticket_uids = cls.fcc.register_tickets([ticket])
+            try:
+                cls.fcc.download_file_to_location("IMD", ticket_uids[0], parent_dir, file_name)
+            finally:
+                cls.fcc.unregister_tickets(ticket_uids)
         return result
 
     @classmethod
     def get_files_to_location(cls, get_file_entries: List[GetFilesEntry], destination_dir: str) -> List[ErrorStack]:
         cls.ensure_init()
         if not os.path.isdir(destination_dir):
             raise ValueError('FMSException - ArgumentError: please provide a valid, existing destination directory.')
 
         named_refs = [e.named_ref for e in get_file_entries]
         file_read_tickets = FileManagementService.getFileReadTickets(named_refs)
         partial_errors = file_read_tickets.serviceData.partialErrors
         if partial_errors is None:
             partial_errors = list()
-        tickets = file_read_tickets.tickets.values()
-        ticket_uids = cls.fcc.register_tickets(tickets)
-        try:
-            file_names = [e.file_name for e in get_file_entries]
-            cls.fcc.download_files_to_location("IMD", ticket_uids, destination_dir, file_names)
-        finally:
-            cls.fcc.unregister_tickets(ticket_uids)
+        tickets = file_read_tickets.tickets.values() if file_read_tickets.tickets else list()
+        if tickets:
+            ticket_uids = cls.fcc.register_tickets(tickets)
+            try:
+                file_names = [e.file_name for e in get_file_entries]
+                cls.fcc.download_files_to_location("IMD", ticket_uids, destination_dir, file_names)
+            finally:
+                cls.fcc.unregister_tickets(ticket_uids)
         return partial_errors
 
     @classmethod
     def _process_upload_commits(cls, commit_infos: List[CommitDatasetFileInfo], put_file_records: Dict[str, PutFileRecord]):
         for comm_info in commit_infos:
             tickets = list()
             file_paths = list()
```

### Comparing `tcsoa-0.9.0/tcsoa/gen/ActiveCollaboration/_2020_12/ActiveCollaboration.py` & `tcsoa-0.9.1/tcsoa/gen/ActiveCollaboration/_2020_12/ActiveCollaboration.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ActiveCollaboration/_2020_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/ActiveCollaboration/_2020_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ActiveWorkspaceBom/_2015_10/OccurrenceManagementCad.py` & `tcsoa-0.9.1/tcsoa/gen/ActiveWorkspaceBom/_2015_10/OccurrenceManagementCad.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ActiveWorkspaceBom/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/ActiveWorkspaceBom/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ActiveWorkspaceVis/_2015_03/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ActiveWorkspaceVis/_2015_03/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ActiveWorkspaceVis/_2015_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/ActiveWorkspaceVis/_2015_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2006_03/IRM.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2006_03/IRM.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2006_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2006_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2007_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2007_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2007_01/UserManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2007_01/UserManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2007_06/Authorization.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2007_06/Authorization.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2007_06/PreferenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2007_06/PreferenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2008_03/IRM.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2008_03/IRM.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2008_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2008_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2008_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2008_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2010_04/DisciplineManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2010_04/DisciplineManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2010_04/IRM.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2010_04/IRM.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2011_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2011_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2012_09/PreferenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2012_09/PreferenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2012_09/UserManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2012_09/UserManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2012_10/IRM.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2012_10/IRM.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2012_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2012_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2014_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2014_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2014_10/UserManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2014_10/UserManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2015_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2015_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2015_03/UserManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2015_03/UserManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2015_07/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2015_07/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2015_07/UserManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2015_07/UserManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2016_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2016_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2016_03/UserManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2016_03/UserManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2016_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2016_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2016_10/UserManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2016_10/UserManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2017_05/GroupManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2017_05/GroupManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2017_05/RoleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2017_05/RoleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2017_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2017_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2017_05/UserManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2017_05/UserManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2018_11/IRM.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2018_11/IRM.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2018_11/OrganizationManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2018_11/OrganizationManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Administration/services.py` & `tcsoa-0.9.1/tcsoa/gen/Administration/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2006_03/Ai.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2006_03/Ai.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2006_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2006_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2007_12/Ai.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2007_12/Ai.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2007_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2007_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2008_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2008_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2008_06/Ai.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2008_06/Ai.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2009_06/Ai.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2009_06/Ai.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2009_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2009_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2009_10/Ai.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2009_10/Ai.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2009_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2009_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2010_09/Ai.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2010_09/Ai.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2012_09/Ai.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2012_09/Ai.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2013_05/Ai.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2013_05/Ai.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2013_12/Ai.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2013_12/Ai.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2013_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2013_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2014_12/Ai.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2014_12/Ai.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2014_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2014_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2018_06/Ai.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2018_06/Ai.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/_2018_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/_2018_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Ai/services.py` & `tcsoa-0.9.1/tcsoa/gen/Ai/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Allocations/_2007_01/Allocation.py` & `tcsoa-0.9.1/tcsoa/gen/Allocations/_2007_01/Allocation.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Allocations/_2007_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Allocations/_2007_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Allocations/_2011_06/Allocation.py` & `tcsoa-0.9.1/tcsoa/gen/Allocations/_2011_06/Allocation.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Allocations/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Allocations/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Allocations/services.py` & `tcsoa-0.9.1/tcsoa/gen/Allocations/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2007_06/LicenseManagement.py` & `tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2007_06/LicenseManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2009_10/LicenseManagement.py` & `tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2009_10/LicenseManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2009_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2009_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2012_09/LicenseManagement.py` & `tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2012_09/LicenseManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2013_05/LicenseManagement.py` & `tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2013_05/LicenseManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2017_05/LicenseManagement.py` & `tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2017_05/LicenseManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2017_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2017_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2018_06/LicenseManagement.py` & `tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2018_06/LicenseManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/_2018_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/_2018_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AuthorizedDataAccess/services.py` & `tcsoa-0.9.1/tcsoa/gen/AuthorizedDataAccess/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AWS2/_2016_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/AWS2/_2016_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AWS2/_2016_12/UiConfig.py` & `tcsoa-0.9.1/tcsoa/gen/AWS2/_2016_12/UiConfig.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AWS2/_2017_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/AWS2/_2017_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AWS2/_2017_06/UiConfig.py` & `tcsoa-0.9.1/tcsoa/gen/AWS2/_2017_06/UiConfig.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AWS2/_2018_12/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/AWS2/_2018_12/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/AWS2/_2018_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/AWS2/_2018_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Bom/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Bom/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Bom/_2008_06/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Bom/_2008_06/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Bom/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Bom/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Bom/_2010_09/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Bom/_2010_09/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Bom/services.py` & `tcsoa-0.9.1/tcsoa/gen/Bom/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2007_06/Constants.py` & `tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2007_06/Constants.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2007_06/RulesBasedFramework.py` & `tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2007_06/RulesBasedFramework.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2008_06/ConditionEngine.py` & `tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2008_06/ConditionEngine.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2008_06/DeepCopyRules.py` & `tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2008_06/DeepCopyRules.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2010_04/BusinessRules.py` & `tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2010_04/BusinessRules.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2011_06/Constants.py` & `tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2011_06/Constants.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/BusinessModeler/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/BusinessModeler/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/BusinessModeler/services.py` & `tcsoa-0.9.1/tcsoa/gen/BusinessModeler/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/BusinessObjects.py` & `tcsoa-0.9.1/tcsoa/gen/BusinessObjects.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2007_01/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2007_01/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2007_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2007_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2007_01/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2007_01/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2007_06/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2007_06/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2007_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2007_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2007_09/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2007_09/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2007_12/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2007_12/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2007_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2007_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2007_12/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2007_12/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2008_03/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2008_03/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2008_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2008_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2008_03/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2008_03/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2008_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2008_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2008_06/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2008_06/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2009_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2009_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2009_04/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2009_04/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2010_09/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2010_09/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2011_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2011_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2012_09/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2012_09/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2013_05/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2013_05/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2014_10/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2014_10/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2014_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2014_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2016_03/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2016_03/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2016_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2016_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2016_03/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2016_03/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2016_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2016_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2016_09/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2016_09/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2018_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2018_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2018_06/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2018_06/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2019_06/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2019_06/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2020_01/AppSessionManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2020_01/AppSessionManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/_2020_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/_2020_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cad/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cad/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cae/_2009_10/SimulationProcessManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cae/_2009_10/SimulationProcessManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cae/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cae/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cae/_2012_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cae/_2012_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cae/_2012_02/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cae/_2012_02/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cae/_2013_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cae/_2013_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cae/_2013_12/SimulationProcessManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cae/_2013_12/SimulationProcessManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cae/_2014_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cae/_2014_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cae/_2014_06/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Cae/_2014_06/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Cae/services.py` & `tcsoa-0.9.1/tcsoa/gen/Cae/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2007_01/CalendarManagement.py` & `tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2007_01/CalendarManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2007_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2007_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2007_06/CalendarManagement.py` & `tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2007_06/CalendarManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2008_06/CalendarManagement.py` & `tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2008_06/CalendarManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/CalendarManagement/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/CalendarManagement/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/CalendarManagement/services.py` & `tcsoa-0.9.1/tcsoa/gen/CalendarManagement/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2008_06/ChangeManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2008_06/ChangeManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2009_06/ChangeManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2009_06/ChangeManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2009_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2009_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2015_10/ChangeManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2015_10/ChangeManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2020_01/ChangeManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2020_01/ChangeManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ChangeManagement/_2020_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/ChangeManagement/_2020_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ChangeManagement/services.py` & `tcsoa-0.9.1/tcsoa/gen/ChangeManagement/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2007_01/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2007_01/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2007_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2007_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2009_10/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2009_10/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2009_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2009_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2011_06/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2011_06/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2011_12/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2011_12/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2011_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2011_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2015_03/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2015_03/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2015_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2015_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2015_10/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2015_10/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2016_03/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2016_03/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2016_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2016_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2016_09/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2016_09/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/_2016_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/_2016_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Classification/services.py` & `tcsoa-0.9.1/tcsoa/gen/Classification/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ClassificationCommon/_2020_01/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/ClassificationCommon/_2020_01/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ClassificationCommon/_2020_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/ClassificationCommon/_2020_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ClassificationCommon/_2020_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/ClassificationCommon/_2020_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ClassificationCommon/services.py` & `tcsoa-0.9.1/tcsoa/gen/ClassificationCommon/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Common.py` & `tcsoa-0.9.1/tcsoa/gen/Common.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2011_06/EffectivityManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2011_06/EffectivityManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2013_05/EffectivityManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2013_05/EffectivityManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2013_05/VariantManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2013_05/VariantManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2017_05/EffectivityManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2017_05/EffectivityManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/_2017_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/_2017_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ConfigFilterCriteria/services.py` & `tcsoa-0.9.1/tcsoa/gen/ConfigFilterCriteria/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Configuration/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Configuration/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Configuration/_2010_04/SmartUiBldr.py` & `tcsoa-0.9.1/tcsoa/gen/Configuration/_2010_04/SmartUiBldr.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Configuration/services.py` & `tcsoa-0.9.1/tcsoa/gen/Configuration/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Configurator/_2014_12/ConfiguratorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Configurator/_2014_12/ConfiguratorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Configurator/_2014_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Configurator/_2014_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2006_03/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2006_03/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2006_03/FileManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2006_03/FileManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2006_03/Reservation.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2006_03/Reservation.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2006_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2006_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2006_03/Session.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2006_03/Session.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2007_01/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2007_01/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2007_01/FileManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2007_01/FileManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2007_01/ManagedRelations.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2007_01/ManagedRelations.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2007_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2007_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2007_01/Session.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2007_01/Session.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2007_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2007_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2007_06/LOV.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2007_06/LOV.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2007_06/PropDescriptor.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2007_06/PropDescriptor.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2007_09/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2007_09/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2007_09/ProjectLevelSecurity.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2007_09/ProjectLevelSecurity.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2007_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2007_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2007_12/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2007_12/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2007_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2007_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2008_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2008_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2008_03/Session.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2008_03/Session.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2008_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2008_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/DispatcherManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/DispatcherManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/ManagedRelations.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/ManagedRelations.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/PropDescriptor.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/PropDescriptor.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/Session.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/Session.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2008_06/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2008_06/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2009_04/ProjectLevelSecurity.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2009_04/ProjectLevelSecurity.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2009_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2009_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2009_10/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2009_10/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2009_10/ProjectLevelSecurity.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2009_10/ProjectLevelSecurity.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2009_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2009_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2010_04/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2010_04/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2010_04/LanguageInformation.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2010_04/LanguageInformation.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2010_04/Session.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2010_04/Session.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2010_09/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2010_09/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/LOV.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/LOV.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/OperationDescriptor.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/OperationDescriptor.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/PropDescriptor.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/PropDescriptor.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/Reservation.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/Reservation.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2011_06/Session.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2011_06/Session.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2012_02/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2012_02/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2012_02/OperationDescriptor.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2012_02/OperationDescriptor.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2012_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2012_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2012_02/Session.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2012_02/Session.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2012_09/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2012_09/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2012_09/ProjectLevelSecurity.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2012_09/ProjectLevelSecurity.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2012_10/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2012_10/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2012_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2012_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2013_05/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2013_05/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2013_05/LOV.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2013_05/LOV.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2014_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2014_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2014_06/DigitalSignature.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2014_06/DigitalSignature.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2014_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2014_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2014_10/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2014_10/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2014_10/ProjectLevelSecurity.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2014_10/ProjectLevelSecurity.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2014_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2014_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2015_07/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2015_07/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2015_07/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2015_07/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2015_10/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2015_10/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2015_10/FileManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2015_10/FileManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2016_05/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2016_05/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2016_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2016_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2016_09/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2016_09/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2016_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2016_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2016_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2016_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2017_05/FileManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2017_05/FileManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2017_05/ProjectLevelSecurity.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2017_05/ProjectLevelSecurity.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2017_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2017_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2017_11/LogicalObject.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2017_11/LogicalObject.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2017_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2017_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2018_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2018_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2018_06/LogicalObject.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2018_06/LogicalObject.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2018_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2018_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2018_11/LogicalObject.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2018_11/LogicalObject.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2018_11/ProjectLevelSecurity.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2018_11/ProjectLevelSecurity.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2019_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2019_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2019_06/Session.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2019_06/Session.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2020_01/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2020_01/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2020_01/ProjectLevelSecurity.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2020_01/ProjectLevelSecurity.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2020_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2020_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2020_04/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2020_04/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/_2020_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/_2020_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Core/services.py` & `tcsoa-0.9.1/tcsoa/gen/Core/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Diagramming/_2011_06/DiagramManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Diagramming/_2011_06/DiagramManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Diagramming/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Diagramming/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Diagramming/_2012_09/DiagramManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Diagramming/_2012_09/DiagramManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Diagramming/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Diagramming/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Diagramming/_2014_06/DNDManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Diagramming/_2014_06/DNDManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Diagramming/_2014_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Diagramming/_2014_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Diagramming/services.py` & `tcsoa-0.9.1/tcsoa/gen/Diagramming/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocMgmtAw/_2017_06/DocMgmt.py` & `tcsoa-0.9.1/tcsoa/gen/DocMgmtAw/_2017_06/DocMgmt.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocMgmtAw/_2017_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/DocMgmtAw/_2017_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2007_01/DocumentTemplate.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2007_01/DocumentTemplate.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2007_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2007_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2008_06/DocumentControl.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2008_06/DocumentControl.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2010_04/DigitalSignature.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2010_04/DigitalSignature.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2010_04/LaunchDefinition.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2010_04/LaunchDefinition.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2011_06/AttributeExchange.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2011_06/AttributeExchange.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2013_12/PrintOrRender.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2013_12/PrintOrRender.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2013_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2013_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2018_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2018_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2018_11/PrintOrRender.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2018_11/PrintOrRender.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/DocumentManagement/services.py` & `tcsoa-0.9.1/tcsoa/gen/DocumentManagement/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/EditContext/_2014_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/EditContext/_2014_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/EditContext/_2015_07/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/EditContext/_2015_07/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/EditContext/_2015_07/services.py` & `tcsoa-0.9.1/tcsoa/gen/EditContext/_2015_07/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/EditContext/_2016_04/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/EditContext/_2016_04/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/EditContext/_2016_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/EditContext/_2016_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/EditContext/_2016_10/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/EditContext/_2016_10/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/EditContext/_2016_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/EditContext/_2016_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/EditContext/services.py` & `tcsoa-0.9.1/tcsoa/gen/EditContext/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2007_06/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2007_06/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2007_12/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2007_12/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2007_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2007_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2008_06/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2008_06/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2010_04/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2010_04/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2011_06/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2011_06/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2020_04/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2020_04/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/_2020_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/_2020_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/GlobalMultiSite/services.py` & `tcsoa-0.9.1/tcsoa/gen/GlobalMultiSite/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ImportExport/_2007_06/FileImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/ImportExport/_2007_06/FileImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ImportExport/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/ImportExport/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ImportExport/_2008_06/FileImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/ImportExport/_2008_06/FileImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ImportExport/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/ImportExport/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ImportExport/_2011_06/FileImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/ImportExport/_2011_06/FileImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ImportExport/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/ImportExport/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ImportExport/_2012_09/FileImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/ImportExport/_2012_09/FileImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ImportExport/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/ImportExport/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ImportExport/_2017_11/FileImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/ImportExport/_2017_11/FileImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ImportExport/_2017_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/ImportExport/_2017_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ImportExport/services.py` & `tcsoa-0.9.1/tcsoa/gen/ImportExport/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2012_10/BOMIndexManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2012_10/BOMIndexManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2012_10/OccurrenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2012_10/OccurrenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_03/OccurrenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_03/OccurrenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_07/OccurrenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_07/OccurrenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_10/OccurrenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2015_10/OccurrenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2016_03/OccurrenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2016_03/OccurrenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_06/OccurrenceConfiguration.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_06/OccurrenceConfiguration.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_06/OccurrenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_06/OccurrenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_12/OccurrenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2017_12/OccurrenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_05/Compare.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_05/Compare.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_05/OccurrenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_05/OccurrenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_12/Compare.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_12/Compare.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_12/Markup.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_12/Markup.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_12/OccurrenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2018_12/OccurrenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_06/Compare.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_06/Compare.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_06/OccurrenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_06/OccurrenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_12/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_12/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_12/OccurrenceConfiguration.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_12/OccurrenceConfiguration.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_12/OccurrenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2019_12/OccurrenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2020_05/OccurrenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2020_05/OccurrenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceBom/_2020_12/OccurrenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceBom/_2020_12/OccurrenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceVis/_2014_11/OccurrenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceVis/_2014_11/OccurrenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceVis/_2015_03/MassiveModelVisualization.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceVis/_2015_03/MassiveModelVisualization.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ActiveWorkspaceVis/_2018_05/MassiveModelVisualization.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ActiveWorkspaceVis/_2018_05/MassiveModelVisualization.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2007_06/Authorization.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2007_06/Authorization.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2007_06/PreferenceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2007_06/PreferenceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2008_06/IRM.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2008_06/IRM.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2009_10/PersonManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2009_10/PersonManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2011_06/OrganizationManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2011_06/OrganizationManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2012_10/OrganizationManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2012_10/OrganizationManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2013_05/UserManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2013_05/UserManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2014_10/UserManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2014_10/UserManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2016_09/VolumeManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2016_09/VolumeManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2017_11/IRM.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2017_11/IRM.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2018_11/SiteManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2018_11/SiteManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Administration/_2019_06/UserManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Administration/_2019_06/UserManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Ai/_2008_06/Ai.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Ai/_2008_06/Ai.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Ai/_2016_03/Ai.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Ai/_2016_03/Ai.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Ai/_2016_04/Ai.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Ai/_2016_04/Ai.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AuditManager/_2012_09/ProcessHistoryManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AuditManager/_2012_09/ProcessHistoryManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/Finder.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/Finder.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/FullTextSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/FullTextSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/LOV.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/LOV.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/OrganizationManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/OrganizationManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2012_10/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2012_10/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2013_12/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2013_12/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2013_12/OrganizationManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2013_12/OrganizationManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2013_12/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2013_12/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2014_11/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2014_11/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2014_11/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2014_11/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2015_03/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2015_03/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2015_03/FullTextSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2015_03/FullTextSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2015_10/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2015_10/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2015_10/FullTextSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2015_10/FullTextSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_03/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_03/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_03/Finder.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_03/Finder.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_03/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_03/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_03/UiConfig.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_03/UiConfig.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_04/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_04/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_12/AdvancedSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_12/AdvancedSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_12/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_12/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_12/Finder.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_12/Finder.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2016_12/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2016_12/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_06/EffectivityManagment.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_06/EffectivityManagment.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_06/Finder.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_06/Finder.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_06/FullTextSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_06/FullTextSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_06/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_06/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_06/UiConfig.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_06/UiConfig.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_12/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_12/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_12/Finder.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_12/Finder.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2017_12/FullTextSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2017_12/FullTextSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_05/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_05/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_05/FileMgmt.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_05/FileMgmt.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_05/Finder.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_05/Finder.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_05/FullTextSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_05/FullTextSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_05/TCXML.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_05/TCXML.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_05/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_05/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_12/Finder.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_12/Finder.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2018_12/MultiSite.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2018_12/MultiSite.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2019_06/AdvancedSavedSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2019_06/AdvancedSavedSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2019_06/Finder.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2019_06/Finder.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2019_06/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2019_06/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2019_12/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2019_12/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2019_12/Finder.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2019_12/Finder.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2020_05/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2020_05/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2020_05/FileMgmt.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2020_05/FileMgmt.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2020_05/FullTextSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2020_05/FullTextSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2020_05/UiConfig.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2020_05/UiConfig.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/AWS2/_2020_12/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/AWS2/_2020_12/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2007_01/DataModelManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2007_01/DataModelManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2010_04/DataModelManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2010_04/DataModelManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2010_09/DataModelManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2010_09/DataModelManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2011_06/DataModelManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2011_06/DataModelManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/BusinessModeler/_2013_05/DynamicLOVQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/BusinessModeler/_2013_05/DynamicLOVQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2008_03/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2008_03/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2008_05/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2008_05/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2008_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2008_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2010_04/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2010_04/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2013_05/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2013_05/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Cad/_2017_05/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Cad/_2017_05/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Cae/_2011_06/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Cae/_2011_06/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Cae/_2013_05/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Cae/_2013_05/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Cae/_2014_06/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Cae/_2014_06/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ChangeManagement/_2012_10/ChangeManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ChangeManagement/_2012_10/ChangeManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ChangeManagement/_2015_03/ChangeManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ChangeManagement/_2015_03/ChangeManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ChangeManagement/_2020_01/MassUpdate.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ChangeManagement/_2020_01/MassUpdate.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Classification/_2009_10/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Classification/_2009_10/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Classification/_2017_05/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Classification/_2017_05/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Classification/_2018_11/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Classification/_2018_11/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Classification/_2020_04/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Classification/_2020_04/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ConfigFilterCriteria/_2013_12/VariantManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ConfigFilterCriteria/_2013_12/VariantManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2014_06/ConfiguratorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2014_06/ConfiguratorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2014_12/ConfiguratorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2014_12/ConfiguratorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2015_03/ConfiguratorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2015_03/ConfiguratorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2015_10/ConfiguratorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2015_10/ConfiguratorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2016_09/ConfiguratorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2016_09/ConfiguratorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2017_11/ConfiguratorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2017_11/ConfiguratorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2018_06/ConfiguratorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2018_06/ConfiguratorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Configurator/_2018_11/ConfiguratorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Configurator/_2018_11/ConfiguratorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2007_01/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2007_01/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2007_06/ProjectLevelSecurity.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2007_06/ProjectLevelSecurity.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2007_09/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2007_09/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2008_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2008_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2008_06/DispatcherManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2008_06/DispatcherManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2008_06/FileManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2008_06/FileManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2009_10/Thumbnail.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2009_10/Thumbnail.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2010_04/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2010_04/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2010_04/ProjectLevelSecurity.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2010_04/ProjectLevelSecurity.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2010_04/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2010_04/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2010_09/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2010_09/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2010_09/FileManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2010_09/FileManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2011_06/ICT.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2011_06/ICT.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2012_02/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2012_02/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2012_09/Envelope.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2012_09/Envelope.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2012_10/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2012_10/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2013_05/Licensing.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2013_05/Licensing.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2013_05/PresentationManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2013_05/PresentationManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2013_05/ProjectLevelSecurity.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2013_05/ProjectLevelSecurity.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2013_05/Thumbnail.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2013_05/Thumbnail.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2014_10/FileManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2014_10/FileManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2014_10/Licensing.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2014_10/Licensing.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2016_10/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2016_10/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2017_05/FileManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2017_05/FileManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2017_05/PresentationManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2017_05/PresentationManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2017_11/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2017_11/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2017_11/LogicalObject.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2017_11/LogicalObject.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2017_11/Type.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2017_11/Type.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2018_06/LogicalObject.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2018_06/LogicalObject.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2018_11/FileManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2018_11/FileManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2018_11/LogicalObject.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2018_11/LogicalObject.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2018_12/Licensing.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2018_12/Licensing.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2020_01/ActiveModeler.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2020_01/ActiveModeler.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Core/_2020_04/LogicalObject.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Core/_2020_04/LogicalObject.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2011_06/DebugLogging.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2011_06/DebugLogging.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2011_06/DebugMonitor.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2011_06/DebugMonitor.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2011_06/PerformanceMonitor.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2011_06/PerformanceMonitor.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2014_06/JournalBasedTesting.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2014_06/JournalBasedTesting.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2015_10/JournalBasedTesting.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2015_10/JournalBasedTesting.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/DebugMonitor/_2019_06/DebugLogging.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/DebugMonitor/_2019_06/DebugLogging.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/DocMgmtAw/_2019_06/DocMgmt.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/DocMgmtAw/_2019_06/DocMgmt.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/DocMgmtAw/_2019_12/DocMgmt.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/DocMgmtAw/_2019_12/DocMgmt.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/_2008_06/DispatcherManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/_2008_06/DispatcherManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/_2008_06/DocumentControl.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/_2008_06/DocumentControl.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/_2013_05/DigitalSignature.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/_2013_05/DigitalSignature.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/_2013_12/Markup.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/_2013_12/Markup.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/DocumentManagement/_2020_12/AttributeExchange.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/DocumentManagement/_2020_12/AttributeExchange.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/EntCba/_2019_12/Alignments.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/EntCba/_2019_12/Alignments.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Gdis/_2006_03/Reporting.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Gdis/_2006_03/Reporting.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2007_06/Briefcase.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2007_06/Briefcase.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2007_06/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2007_06/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2007_06/Synchronizer.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2007_06/Synchronizer.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2008_06/Synchronizer.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2008_06/Synchronizer.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2010_02/LowlevelOwnershipTransfer.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2010_02/LowlevelOwnershipTransfer.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2017_05/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2017_05/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2018_11/Briefcase.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2018_11/Briefcase.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2020_01/Briefcase.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2020_01/Briefcase.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/GlobalMultiSite/_2020_01/OwnershipRecovery.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/GlobalMultiSite/_2020_01/OwnershipRecovery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2017_06/Author.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2017_06/Author.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2017_12/Author.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2017_12/Author.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2018_05/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2018_05/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2018_12/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2018_12/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2019_06/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2019_06/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/IcsAw/_2019_12/Classification.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/IcsAw/_2019_12/Classification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ImportExport/_2010_04/L10NImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ImportExport/_2010_04/L10NImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ImportExport/_2017_11/FileImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ImportExport/_2017_11/FileImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ImportExport/_2018_06/L10NImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ImportExport/_2018_06/L10NImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Integration/_2008_06/IntegrationManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Integration/_2008_06/IntegrationManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2008_12/Core.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2008_12/Core.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2011_12/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2011_12/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2012_09/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2012_09/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2014_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2014_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2014_06/IPAManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2014_06/IPAManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2014_12/IPAManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2014_12/IPAManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2014_12/Model.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2014_12/Model.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2014_12/ResourceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2014_12/ResourceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2015_03/Attachments.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2015_03/Attachments.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2015_03/ResourceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2015_03/ResourceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2015_03/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2015_03/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2015_03/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2015_03/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2015_10/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2015_10/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2015_10/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2015_10/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2016_09/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2016_09/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2016_09/IPAManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2016_09/IPAManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2016_09/ResourceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2016_09/ResourceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2016_09/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2016_09/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2016_09/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2016_09/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2017_05/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2017_05/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2017_05/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2017_05/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2017_11/ResourceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2017_11/ResourceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2017_11/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2017_11/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2018_11/ResourceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2018_11/ResourceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2018_11/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2018_11/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2019_06/ClosureRuleEditor.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2019_06/ClosureRuleEditor.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2019_06/ResourceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2019_06/ResourceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2019_06/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2019_06/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2020_01/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2020_01/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2020_01/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2020_01/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Manufacturing/_2020_04/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Manufacturing/_2020_04/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Mmv/_2012_09/SpatialStructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Mmv/_2012_09/SpatialStructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2007_06/ObjectDirectory.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2007_06/ObjectDirectory.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2007_06/RemoteOperation.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2007_06/RemoteOperation.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2007_06/TcEntObjectDirectory.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2007_06/TcEntObjectDirectory.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2011_06/ImportExportAsync.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2011_06/ImportExportAsync.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2011_06/ObjectDirectory.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2011_06/ObjectDirectory.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2012_02/ObjectDirectory.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2012_02/ObjectDirectory.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2012_02/RemoteOperation.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2012_02/RemoteOperation.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2017_11/ArchiveRestore.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2017_11/ArchiveRestore.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2018_06/Search.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2018_06/Search.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/MultiSite/_2020_12/ImportExportTCXML.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/MultiSite/_2020_12/ImportExportTCXML.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2014_10/SubscriptionManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2014_10/SubscriptionManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2015_03/MessageManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2015_03/MessageManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2015_03/SubscriptionManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2015_03/SubscriptionManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2015_10/SubscriptionManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2015_10/SubscriptionManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Notification/_2017_11/SubscriptionManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Notification/_2017_11/SubscriptionManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/OccMgmt/_2020_05/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/OccMgmt/_2020_05/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/OccMgmt/_2020_12/EffectivityManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/OccMgmt/_2020_12/EffectivityManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ProductConfiguratorAw/_2017_12/ConfiguratorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ProductConfiguratorAw/_2017_12/ConfiguratorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ProductConfiguratorAw/_2018_05/ConfiguratorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ProductConfiguratorAw/_2018_05/ConfiguratorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ProductConfiguratorAw/_2020_05/ConfiguratorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ProductConfiguratorAw/_2020_05/ConfiguratorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ProductConfiguratorAw/_2020_12/ConfiguratorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ProductConfiguratorAw/_2020_12/ConfiguratorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2007_01/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2007_01/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2007_06/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2007_06/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2008_06/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2008_06/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2009_10/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2009_10/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2010_04/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2010_04/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2011_06/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2011_06/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2012_02/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2012_02/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagement/_2014_10/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagement/_2014_10/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/ProjectManagementAw/_2019_12/ScheduleManagementAw.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/ProjectManagementAw/_2019_12/ScheduleManagementAw.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Query/_2008_06/Finder.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Query/_2008_06/Finder.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Query/_2012_02/SavedQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Query/_2012_02/SavedQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Query/_2013_05/SavedQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Query/_2013_05/SavedQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Query/_2014_10/SavedQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Query/_2014_10/SavedQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2007_06/VariantManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2007_06/VariantManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2007_09/VariantManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2007_09/VariantManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2008_03/VariantManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2008_03/VariantManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2009_01/VariantManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2009_01/VariantManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2009_04/VariantManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2009_04/VariantManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2009_05/VariantManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2009_05/VariantManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Rdv/_2010_04/VariantManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Rdv/_2010_04/VariantManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Reports/_2007_06/BOMRollup.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Reports/_2007_06/BOMRollup.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Requirementsmanagement/_2009_10/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Requirementsmanagement/_2009_10/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Requirementsmanagement/_2012_02/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Requirementsmanagement/_2012_02/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Requirementsmanagement/_2012_10/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Requirementsmanagement/_2012_10/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/RevRuleMgmt/_2019_12/RevisionRuleAdministration.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/RevRuleMgmt/_2019_12/RevisionRuleAdministration.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Search/_2020_12/SearchFolder.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Search/_2020_12/SearchFolder.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Security/_2017_12/AwLicensing.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Security/_2017_12/AwLicensing.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Structure/_2020_12/WhereUsed.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Structure/_2020_12/WhereUsed.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2007_06/GlobalAlternate.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2007_06/GlobalAlternate.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2007_06/PublishByLink.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2007_06/PublishByLink.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2007_06/Restructure.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2007_06/Restructure.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2007_12/BrokenLinks.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2007_12/BrokenLinks.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2008_03/Structure.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2008_03/Structure.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2008_06/Structure.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2008_06/Structure.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2009_10/EffectivitiesManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2009_10/EffectivitiesManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2010_04/BOMMarkup.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2010_04/BOMMarkup.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2010_09/Structure.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2010_09/Structure.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2011_06/IncrementalChange.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2011_06/IncrementalChange.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2011_06/Structure.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2011_06/Structure.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2011_06/VariantManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2011_06/VariantManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2012_02/StructureVerification.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2012_02/StructureVerification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2012_09/StructureVerification.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2012_09/StructureVerification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2013_05/StructureExpansionLite.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2013_05/StructureExpansionLite.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2013_12/StructureExpansionLite.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2013_12/StructureExpansionLite.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2014_12/BrokenLinks.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2014_12/BrokenLinks.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2014_12/Restructure.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2014_12/Restructure.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2014_12/StructureVerification.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2014_12/StructureVerification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2015_10/VariantManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2015_10/VariantManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2016_03/StructureVerification.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2016_03/StructureVerification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2016_10/Effectivity.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2016_10/Effectivity.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2017_05/StructureExpansionLite.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2017_05/StructureExpansionLite.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2017_05/StructureLiteConversion.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2017_05/StructureLiteConversion.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2017_05/StructureVerification.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2017_05/StructureVerification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2018_11/MassUpdate.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2018_11/MassUpdate.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2018_11/StructureVerification.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2018_11/StructureVerification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/StructureManagement/_2020_05/RevisionRuleAdministration.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/StructureManagement/_2020_05/RevisionRuleAdministration.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/TCXMLImportExport/_2020_12/Briefcase.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/TCXMLImportExport/_2020_12/Briefcase.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Translation/_2007_06/TranslationManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Translation/_2007_06/TranslationManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/UiConfig/_2014_11/UiConfig.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/UiConfig/_2014_11/UiConfig.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Validation/_2007_06/Validation.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Validation/_2007_06/Validation.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Validation/_2008_06/Validation.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Validation/_2008_06/Validation.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Validation/_2012_02/Validation.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Validation/_2012_02/Validation.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Vendormanagement/_2008_05/VendorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Vendormanagement/_2008_05/VendorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Vendormanagement/_2008_06/VendorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Vendormanagement/_2008_06/VendorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/VendorManagementAW/_2019_12/VendorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/VendorManagementAW/_2019_12/VendorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/VendorManagementAW/_2020_05/VendorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/VendorManagementAW/_2020_05/VendorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/VendorManagementAW/_2020_12/VendorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/VendorManagementAW/_2020_12/VendorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2008_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2008_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2008_06/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2008_06/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2010_04/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2010_04/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2010_09/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2010_09/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2010_09/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2010_09/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2011_12/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2011_12/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2012_10/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2012_10/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2017_05/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2017_05/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Visualization/_2018_11/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Visualization/_2018_11/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Workflow/_2013_05/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Workflow/_2013_05/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Workflow/_2017_11/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Workflow/_2017_11/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/Workflowaw/_2020_12/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/Workflowaw/_2020_12/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal/XlsBom/_2020_12/Import.py` & `tcsoa-0.9.1/tcsoa/gen/Internal/XlsBom/_2020_12/Import.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2012_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2012_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_07/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_07/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2016_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2016_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2017_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2017_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2017_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2017_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2018_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2018_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2018_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2018_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2019_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2019_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2020_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2020_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/_2020_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/_2020_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceBom/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceBom/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceVis/_2014_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceVis/_2014_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceVis/_2015_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceVis/_2015_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceVis/_2018_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceVis/_2018_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ActiveWorkspaceVis/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ActiveWorkspaceVis/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2009_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2009_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2012_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2012_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2014_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2014_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2016_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2016_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2017_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2017_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2018_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2018_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Administration/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Administration/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Administration/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Administration/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Ai/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Ai/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Ai/_2016_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Ai/_2016_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Ai/_2016_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Ai/_2016_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Ai/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Ai/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AuditManager/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AuditManager/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2012_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2012_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2013_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2013_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2014_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2014_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2015_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2015_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2016_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2016_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2016_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2016_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2016_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2016_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2017_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2017_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2017_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2017_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2018_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2018_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2018_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2018_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2019_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2019_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2020_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2020_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/_2020_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/_2020_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_AWS2/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_AWS2/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2007_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2007_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_BusinessModeler/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_BusinessModeler/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2007_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2007_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2008_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2008_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2008_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2008_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cad/_2017_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cad/_2017_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cad/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cad/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2009_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2009_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2012_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2012_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2013_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2013_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cae/_2014_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cae/_2014_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Cae/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Cae/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ChangeManagement/_2012_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ChangeManagement/_2012_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ChangeManagement/_2015_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ChangeManagement/_2015_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ChangeManagement/_2020_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ChangeManagement/_2020_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ChangeManagement/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ChangeManagement/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Classification/_2009_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Classification/_2009_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Classification/_2017_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Classification/_2017_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Classification/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Classification/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Classification/_2020_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Classification/_2020_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Classification/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Classification/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_CodeCoverage/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_CodeCoverage/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ConfigFilterCriteria/_2013_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ConfigFilterCriteria/_2013_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2014_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2014_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2014_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2014_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2015_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2015_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2016_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2016_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2017_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2017_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2018_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2018_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Configurator/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Configurator/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2006_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2006_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2007_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2007_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2008_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2008_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2009_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2009_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2012_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2012_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2012_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2012_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2014_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2014_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2014_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2014_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2016_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2016_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2017_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2017_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2017_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2017_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2018_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2018_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2018_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2018_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2020_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2020_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/_2020_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/_2020_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Core/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Core/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2014_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2014_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2015_07/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2015_07/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_DebugMonitor/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_DebugMonitor/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_DocMgmtAw/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_DocMgmtAw/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_DocMgmtAw/_2019_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_DocMgmtAw/_2019_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/_2013_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/_2013_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/_2020_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/_2020_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_DocumentManagement/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_DocumentManagement/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_EntCba/_2019_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_EntCba/_2019_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Gdis/_2006_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Gdis/_2006_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2010_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2010_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2017_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2017_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/_2020_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/_2020_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_GlobalMultiSite/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_GlobalMultiSite/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2017_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2017_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2017_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2017_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2018_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2018_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2018_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2018_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/_2019_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/_2019_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_IcsAw/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_IcsAw/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/_2017_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/_2017_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/_2017_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/_2017_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/_2018_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/_2018_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ImportExport/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ImportExport/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Integration/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Integration/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Integration/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Integration/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2008_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2008_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2011_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2011_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2013_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2013_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2014_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2014_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2014_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2014_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2015_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2015_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2016_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2016_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2016_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2016_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2017_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2017_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2017_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2017_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2020_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2020_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/_2020_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/_2020_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Manufacturing/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Manufacturing/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Mmv/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Mmv/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Mmv/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Mmv/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2012_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2012_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2017_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2017_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2018_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2018_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/_2020_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/_2020_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_MultiSite/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_MultiSite/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Notification/_2014_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Notification/_2014_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Notification/_2015_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Notification/_2015_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Notification/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Notification/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Notification/_2017_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Notification/_2017_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Notification/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Notification/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_OccMgmt/_2020_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_OccMgmt/_2020_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_OccMgmt/_2020_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_OccMgmt/_2020_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_OccMgmt/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_OccMgmt/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/_2017_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/_2017_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/_2018_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/_2018_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/_2020_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/_2020_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/_2020_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/_2020_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProductConfiguratorAw/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProductConfiguratorAw/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2007_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2007_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2009_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2009_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2012_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2012_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/_2014_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/_2014_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagement/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagement/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_ProjectManagementAw/_2019_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_ProjectManagementAw/_2019_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Query/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Query/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Query/_2012_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Query/_2012_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Query/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Query/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Query/_2014_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Query/_2014_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Query/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Query/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2007_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2007_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2008_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2008_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2009_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2009_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2009_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2009_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2009_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2009_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Rdv/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Rdv/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Reports/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Reports/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Reports/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Reports/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Requirementsmanagement/_2009_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Requirementsmanagement/_2009_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Requirementsmanagement/_2012_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Requirementsmanagement/_2012_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Requirementsmanagement/_2012_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Requirementsmanagement/_2012_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Requirementsmanagement/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Requirementsmanagement/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_RevRuleMgmt/_2019_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_RevRuleMgmt/_2019_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Search/_2020_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Search/_2020_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Security/_2017_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Security/_2017_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Structure/_2020_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Structure/_2020_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2007_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2007_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2008_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2008_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2008_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2008_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2009_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2009_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2012_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2012_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2013_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2013_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2014_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2014_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2016_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2016_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2016_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2016_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2017_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2017_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/_2020_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/_2020_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_StructureManagement/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_StructureManagement/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_TCXMLImportExport/_2020_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_TCXMLImportExport/_2020_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Translation/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Translation/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_UiConfig/_2014_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_UiConfig/_2014_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Validation/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Validation/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Validation/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Validation/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Validation/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Validation/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Validation/_2012_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Validation/_2012_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Validation/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Validation/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Vendormanagement/_2008_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Vendormanagement/_2008_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Vendormanagement/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Vendormanagement/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_VendorManagementAW/_2019_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_VendorManagementAW/_2019_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_VendorManagementAW/_2020_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_VendorManagementAW/_2020_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_VendorManagementAW/_2020_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_VendorManagementAW/_2020_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_VendorManagementAW/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_VendorManagementAW/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2011_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2011_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2012_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2012_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2017_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2017_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Visualization/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Visualization/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Workflow/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Workflow/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Workflow/_2017_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Workflow/_2017_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_Workflowaw/_2020_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_Workflowaw/_2020_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Internal_XlsBom/_2020_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Internal_XlsBom/_2020_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2008_06/Core.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2008_06/Core.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2008_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2008_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2008_06/TimeManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2008_06/TimeManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2008_12/IPAManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2008_12/IPAManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2008_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2008_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_06/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_06/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/MFGPropertyCollector.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/MFGPropertyCollector.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/Model.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/Model.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/ModelDefinitions.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/ModelDefinitions.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2009_10/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2009_10/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2010_09/Core.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2010_09/Core.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2010_09/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2010_09/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2010_09/TimeManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2010_09/TimeManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2011_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2011_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2011_06/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2011_06/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_02/Constraints.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_02/Constraints.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_02/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_02/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_02/IPAManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_02/IPAManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_02/Model.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_02/Model.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_09/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_09/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2012_09/Validation.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2012_09/Validation.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/Core.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/Core.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/IPAManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/IPAManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_05/TimeWayPlan.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_05/TimeWayPlan.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_12/Model.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_12/Model.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_12/ResourceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_12/ResourceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2013_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2013_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_06/ResourceManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_06/ResourceManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_06/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_06/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_12/IPAManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_12/IPAManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_12/Model.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_12/Model.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_12/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_12/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2014_12/Validation.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2014_12/Validation.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2015_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2015_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2015_03/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2015_03/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2015_10/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2015_10/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2015_10/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2015_10/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2016_03/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2016_03/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2016_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2016_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2017_05/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2017_05/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2017_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2017_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2017_05/Validation.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2017_05/Validation.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2017_11/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2017_11/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2017_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2017_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2018_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2018_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2018_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2018_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2018_11/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2018_11/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2019_06/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2019_06/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Manufacturing/services.py` & `tcsoa-0.9.1/tcsoa/gen/Manufacturing/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Multisite/_2007_06/ImportExport.py` & `tcsoa-0.9.1/tcsoa/gen/Multisite/_2007_06/ImportExport.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Multisite/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Multisite/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Multisite/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Multisite/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Multisite/_2014_10/ImportExportTCXML.py` & `tcsoa-0.9.1/tcsoa/gen/Multisite/_2014_10/ImportExportTCXML.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Multisite/_2014_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Multisite/_2014_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Multisite/_2019_06/ImportExportTCXML.py` & `tcsoa-0.9.1/tcsoa/gen/Multisite/_2019_06/ImportExportTCXML.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Multisite/_2019_06/Search.py` & `tcsoa-0.9.1/tcsoa/gen/Multisite/_2019_06/Search.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Multisite/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Multisite/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Multisite/services.py` & `tcsoa-0.9.1/tcsoa/gen/Multisite/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Notification/_2014_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Notification/_2014_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Notification/_2014_10/SubscriptionManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Notification/_2014_10/SubscriptionManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/OfficeOnline/_2017_11/OfficeOnline.py` & `tcsoa-0.9.1/tcsoa/gen/OfficeOnline/_2017_11/OfficeOnline.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/OfficeOnline/_2017_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/OfficeOnline/_2017_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Participant/_2018_11/Participant.py` & `tcsoa-0.9.1/tcsoa/gen/Participant/_2018_11/Participant.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Participant/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Participant/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_01/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_01/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_06/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_06/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_12/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_12/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2007_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2007_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2008_06/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2008_06/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2009_10/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2009_10/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2009_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2009_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_02/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_02/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_06/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_06/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_12/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_12/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2011_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2011_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2012_02/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2012_02/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2012_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2012_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2012_09/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2012_09/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2014_06/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2014_06/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2014_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2014_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2014_10/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2014_10/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2014_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2014_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2015_07/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2015_07/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2015_07/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2015_07/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2016_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2016_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2017_11/ScheduleManagement.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2017_11/ScheduleManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2017_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2017_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagement/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagement/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2015_07/ScheduleManagementAw.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2015_07/ScheduleManagementAw.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2015_07/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2015_07/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2016_12/ScheduleManagementAw.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2016_12/ScheduleManagementAw.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2016_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2016_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2017_06/ScheduleManagementAw.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2017_06/ScheduleManagementAw.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2017_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2017_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2018_12/ScheduleManagementAw.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2018_12/ScheduleManagementAw.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2018_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2018_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2019_06/ScheduleManagementAw.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2019_06/ScheduleManagementAw.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2020_05/ScheduleManagementAw.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2020_05/ScheduleManagementAw.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/_2020_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/_2020_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/ProjectManagementAw/services.py` & `tcsoa-0.9.1/tcsoa/gen/ProjectManagementAw/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Qualification/_2014_06/QualificationManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Qualification/_2014_06/QualificationManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Qualification/_2014_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Qualification/_2014_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Qualification/services.py` & `tcsoa-0.9.1/tcsoa/gen/Qualification/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2006_03/SavedQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2006_03/SavedQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2006_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2006_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2007_01/SavedQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2007_01/SavedQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2007_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2007_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2007_06/Finder.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2007_06/Finder.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2007_06/SavedQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2007_06/SavedQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2007_09/SavedQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2007_09/SavedQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2007_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2007_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2008_06/SavedQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2008_06/SavedQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2010_04/SavedQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2010_04/SavedQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2010_09/SavedQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2010_09/SavedQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2012_10/Finder.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2012_10/Finder.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2012_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2012_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2013_05/SavedQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2013_05/SavedQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2014_11/Finder.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2014_11/Finder.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2014_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2014_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2018_11/SavedQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2018_11/SavedQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2019_06/SavedQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2019_06/SavedQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2020_04/SavedQuery.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2020_04/SavedQuery.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/_2020_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Query/_2020_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Query/services.py` & `tcsoa-0.9.1/tcsoa/gen/Query/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Rdv/_2008_05/ContextManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Rdv/_2008_05/ContextManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Rdv/_2008_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Rdv/_2008_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Rdv/_2009_04/ContextManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Rdv/_2009_04/ContextManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Rdv/_2009_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Rdv/_2009_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Rdv/_2010_09/ContextManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Rdv/_2010_09/ContextManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Rdv/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Rdv/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Rdv/_2012_09/ContextManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Rdv/_2012_09/ContextManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Rdv/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Rdv/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Rdv/_2013_05/ContextManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Rdv/_2013_05/ContextManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Rdv/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Rdv/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Rdv/services.py` & `tcsoa-0.9.1/tcsoa/gen/Rdv/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/_2012_10/NetworkEngine.py` & `tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/_2012_10/NetworkEngine.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/_2012_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/_2012_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/_2014_11/NetworkEngine.py` & `tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/_2014_11/NetworkEngine.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/_2014_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/_2014_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/_2019_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/_2019_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/RelationshipViewer/services.py` & `tcsoa-0.9.1/tcsoa/gen/RelationshipViewer/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/_2007_01/CrfReports.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/_2007_01/CrfReports.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/_2007_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/_2007_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/_2007_06/CubeReports.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/_2007_06/CubeReports.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/_2008_06/CrfReports.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/_2008_06/CrfReports.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/_2008_12/CrfReports.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/_2008_12/CrfReports.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/_2008_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/_2008_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/_2010_04/CrfReports.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/_2010_04/CrfReports.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/_2015_03/CrfReports.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/_2015_03/CrfReports.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/_2015_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/_2015_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/_2015_10/CrfReports.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/_2015_10/CrfReports.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Reports/services.py` & `tcsoa-0.9.1/tcsoa/gen/Reports/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2007_01/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2007_01/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2007_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2007_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2008_06/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2008_06/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2009_10/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2009_10/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2009_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2009_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2010_09/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2010_09/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2011_06/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2011_06/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2012_09/RequirementsManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2012_09/RequirementsManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Requirementsmanagement/services.py` & `tcsoa-0.9.1/tcsoa/gen/Requirementsmanagement/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Server.py` & `tcsoa-0.9.1/tcsoa/gen/Server.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2007_06/PublishByLink.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2007_06/PublishByLink.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_03/Composition.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_03/Composition.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_05/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_05/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_05/StructureVerification.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_05/StructureVerification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_06/Structure.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_06/Structure.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2008_12/StructureVerification.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2008_12/StructureVerification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2010_04/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2010_04/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2010_04/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2010_04/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2010_09/Structure.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2010_09/Structure.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2010_09/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2010_09/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2010_09/StructureVerification.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2010_09/StructureVerification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2011_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2011_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2011_06/Structure.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2011_06/Structure.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_02/StructureVerification.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_02/StructureVerification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_09/MassUpdate.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_09/MassUpdate.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_09/Structure.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_09/Structure.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_09/VariantManagement.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_09/VariantManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_10/Structure.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_10/Structure.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2012_10/StructureVerification.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2012_10/StructureVerification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2013_05/IncrementalChange.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2013_05/IncrementalChange.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2013_05/StructureVerification.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2013_05/StructureVerification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2013_05/VariantManagement.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2013_05/VariantManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_06/StructureFilterWithExpand.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_06/StructureFilterWithExpand.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_06/StructureVerification.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_06/StructureVerification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_10/MassUpdate.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_10/MassUpdate.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_10/Structure.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_10/Structure.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_12/Effectivity.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_12/Effectivity.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2014_12/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2014_12/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2015_10/Effectivity.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2015_10/Effectivity.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2016_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2016_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2016_05/StructureVerification.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2016_05/StructureVerification.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2016_09/PublishByLink.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2016_09/PublishByLink.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2016_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2016_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2017_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2017_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2017_05/StructureSearch.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2017_05/StructureSearch.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2018_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2018_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2018_11/Structure.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2018_11/Structure.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/_2019_06/VariantManagement.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/_2019_06/VariantManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/StructureManagement/services.py` & `tcsoa-0.9.1/tcsoa/gen/StructureManagement/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Translation/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Translation/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Translation/_2007_06/TranslationManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Translation/_2007_06/TranslationManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/UiConfig/_2014_11/services.py` & `tcsoa-0.9.1/tcsoa/gen/UiConfig/_2014_11/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/UiConfig/_2014_11/UiConfig.py` & `tcsoa-0.9.1/tcsoa/gen/UiConfig/_2014_11/UiConfig.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/UiConfig/_2015_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/UiConfig/_2015_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/UiConfig/_2015_10/UiConfig.py` & `tcsoa-0.9.1/tcsoa/gen/UiConfig/_2015_10/UiConfig.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2007_06/VendorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2007_06/VendorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2008_06/VendorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2008_06/VendorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2012_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2012_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2012_02/VendorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2012_02/VendorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2012_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2012_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2012_09/VendorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2012_09/VendorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2016_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2016_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Vendormanagement/_2016_09/VendorManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Vendormanagement/_2016_09/VendorManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Vendormanagement/services.py` & `tcsoa-0.9.1/tcsoa/gen/Vendormanagement/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Visualization/_2011_02/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Visualization/_2011_02/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Visualization/_2011_02/services.py` & `tcsoa-0.9.1/tcsoa/gen/Visualization/_2011_02/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Visualization/_2011_02/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Visualization/_2011_02/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Visualization/_2013_05/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Visualization/_2013_05/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Visualization/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Visualization/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Visualization/_2013_12/services.py` & `tcsoa-0.9.1/tcsoa/gen/Visualization/_2013_12/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Visualization/_2013_12/StructureManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Visualization/_2013_12/StructureManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Visualization/_2016_03/DataManagement.py` & `tcsoa-0.9.1/tcsoa/gen/Visualization/_2016_03/DataManagement.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Visualization/_2016_03/services.py` & `tcsoa-0.9.1/tcsoa/gen/Visualization/_2016_03/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Visualization/services.py` & `tcsoa-0.9.1/tcsoa/gen/Visualization/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2007_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2007_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2007_06/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2007_06/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2008_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2008_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2008_06/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2008_06/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2010_09/services.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2010_09/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2010_09/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2010_09/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2012_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2012_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2013_05/services.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2013_05/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2013_05/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2013_05/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2014_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2014_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2014_06/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2014_06/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2014_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2014_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2014_10/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2014_10/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2015_07/services.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2015_07/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2015_07/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2015_07/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2019_06/services.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2019_06/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2019_06/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2019_06/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2020_01/services.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2020_01/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/_2020_01/Workflow.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/_2020_01/Workflow.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/Workflow/services.py` & `tcsoa-0.9.1/tcsoa/gen/Workflow/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/WProxy/_2014_10/ProxyLink.py` & `tcsoa-0.9.1/tcsoa/gen/WProxy/_2014_10/ProxyLink.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/gen/WProxy/_2014_10/services.py` & `tcsoa-0.9.1/tcsoa/gen/WProxy/_2014_10/services.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/tcsoa/itk_constants.py` & `tcsoa-0.9.1/tcsoa/itk_constants.py`

 * *Files identical despite different names*

### Comparing `tcsoa-0.9.0/setup.py` & `tcsoa-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -913,15 +913,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Deprecated>=1.2.13,<2.0.0', 'requests>=2.27.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'tcsoa',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'A framework generated for the purpose of consuming Teamcenter™ services via Python.',
     'long_description': 'None',
     'author': 'Alexander Haas',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tcsoa-0.9.0/PKG-INFO` & `tcsoa-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcsoa
-Version: 0.9.0
+Version: 0.9.1
 Summary: A framework generated for the purpose of consuming Teamcenter™ services via Python.
 License: MIT
 Author: Alexander Haas
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

