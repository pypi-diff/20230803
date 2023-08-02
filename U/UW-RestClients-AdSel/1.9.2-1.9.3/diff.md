# Comparing `tmp/UW-RestClients-AdSel-1.9.2.tar.gz` & `tmp/UW-RestClients-AdSel-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UW-RestClients-AdSel-1.9.2.tar", last modified: Wed Jul 26 21:30:03 2023, max compression
+gzip compressed data, was "UW-RestClients-AdSel-1.9.3.tar", last modified: Wed Aug  2 23:18:59 2023, max compression
```

## Comparing `UW-RestClients-AdSel-1.9.2.tar` & `UW-RestClients-AdSel-1.9.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.836229 UW-RestClients-AdSel-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-07-26 21:30:03.836229 UW-RestClients-AdSel-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-07-26 21:30:03.000000 UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-07-26 21:30:03.000000 UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 21:30:03.000000 UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-26 21:30:03.000000 UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-26 21:30:03.000000 UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-26 21:30:03.836229 UW-RestClients-AdSel-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-26 21:30:02.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)    20955 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/dao.py
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    10778 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.828229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.828229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.828229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.828229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/academicqtr
--rw-r--r--   0 runner    (1001) docker     (122)     1883 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities?Page=2
--rw-r--r--   0 runner    (1001) docker     (122)      502 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities?assignmentType=major
--rw-r--r--   0 runner    (1001) docker     (122)      938 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage
--rw-r--r--   0 runner    (1001) docker     (122)     1772 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage&systemKey=12345
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/
--rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20194
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20201/
--rw-r--r--   0 runner    (1001) docker     (122)      368 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20201/0
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/major/
--rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/major/1
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/major/2
--rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/majors
--rw-r--r--   0 runner    (1001) docker     (122)     2738 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/majorvalues
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.828229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/0/
--rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/0/123
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/0/all
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/
--rw-r--r--   0 runner    (1001) docker     (122)     2073 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/0
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/assignments/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/assignments/cohort/
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/assignments/cohort/bulk
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/assignments/departmentalDecision
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/assignments/major
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/assignments/purpleAndGold
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/cohorts/
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/cohorts/0
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/cohorts/0?Page=2
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/cohorts/1
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=0
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=1
--rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/filter
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.828229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0/
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_BIOL_1
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_CHEM_1
--rw-r--r--   0 runner    (1001) docker     (122)      328 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_CSE_1
--rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=1&Limit=100
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=2&Limit=100
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/1?Page=1&Limit=100
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/workspaces/
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/workspaces/20194
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11871 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/tests/test_adsel.py
--rw-r--r--   0 runner    (1001) docker     (122)      119 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.822029 UW-RestClients-AdSel-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-08-02 23:18:59.822029 UW-RestClients-AdSel-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.818029 UW-RestClients-AdSel-1.9.3/UW_RestClients_AdSel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-08-02 23:18:59.000000 UW-RestClients-AdSel-1.9.3/UW_RestClients_AdSel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-08-02 23:18:59.000000 UW-RestClients-AdSel-1.9.3/UW_RestClients_AdSel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 23:18:59.000000 UW-RestClients-AdSel-1.9.3/UW_RestClients_AdSel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-08-02 23:18:59.000000 UW-RestClients-AdSel-1.9.3/UW_RestClients_AdSel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-08-02 23:18:59.000000 UW-RestClients-AdSel-1.9.3/UW_RestClients_AdSel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-02 23:18:59.822029 UW-RestClients-AdSel-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.818029 UW-RestClients-AdSel-1.9.3/uw_adsel/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-08-02 23:18:58.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)    20955 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/dao.py
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11103 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.818029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.818029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.818029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.818029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.818029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/academicqtr
+-rw-r--r--   0 runner    (1001) docker     (122)     1883 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/activities
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/activities?Page=2
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/activities?assignmentType=major
+-rw-r--r--   0 runner    (1001) docker     (122)      938 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage
+-rw-r--r--   0 runner    (1001) docker     (122)     1772 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage&systemKey=12345
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.818029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.818029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20194
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.818029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20201/
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20201/0
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.818029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/major/
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/major/1
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/major/2
+-rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/majors
+-rw-r--r--   0 runner    (1001) docker     (122)     2738 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/majorvalues
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.818029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/applications/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.818029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/applications/0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/applications/0/123
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/applications/0/all
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.822029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/
+-rw-r--r--   0 runner    (1001) docker     (122)     2073 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/0
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.822029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/assignments/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.822029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/assignments/cohort/
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/assignments/cohort/bulk
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/assignments/departmentalDecision
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/assignments/major
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/assignments/purpleAndGold
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.822029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/cohorts/
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/cohorts/0
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/cohorts/0?Page=2
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/cohorts/1
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.822029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=0
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=1
+-rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/filter
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.818029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/majors/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.822029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/majors/details/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.822029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/majors/details/0/
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_BIOL_1
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_CHEM_1
+-rw-r--r--   0 runner    (1001) docker     (122)      328 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_CSE_1
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=1&Limit=100
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=2&Limit=100
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/majors/details/1?Page=1&Limit=100
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.822029 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/workspaces/20194
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:59.822029 UW-RestClients-AdSel-1.9.3/uw_adsel/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12326 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/tests/test_adsel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-08-02 23:18:50.000000 UW-RestClients-AdSel-1.9.3/uw_adsel/utilities.py
```

### Comparing `UW-RestClients-AdSel-1.9.2/LICENSE` & `UW-RestClients-AdSel-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/PKG-INFO` & `UW-RestClients-AdSel-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UW-RestClients-AdSel
-Version: 1.9.2
+Version: 1.9.3
 Summary: A library for connecting to the AdSel API at the University of Washington
 Home-page: https://github.com/uw-it-aca/uw-restclients-adsel
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `UW-RestClients-AdSel-1.9.2/README.md` & `UW-RestClients-AdSel-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/PKG-INFO` & `UW-RestClients-AdSel-1.9.3/UW_RestClients_AdSel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UW-RestClients-AdSel
-Version: 1.9.2
+Version: 1.9.3
 Summary: A library for connecting to the AdSel API at the University of Washington
 Home-page: https://github.com/uw-it-aca/uw-restclients-adsel
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/SOURCES.txt` & `UW-RestClients-AdSel-1.9.3/UW_RestClients_AdSel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/setup.py` & `UW-RestClients-AdSel-1.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,9 +35,7 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
     ],
 )
-
-
```

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/__init__.py` & `UW-RestClients-AdSel-1.9.3/uw_adsel/__init__.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/models.py` & `UW-RestClients-AdSel-1.9.3/uw_adsel/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 class Assignment(models.Model):
     assignment_type = models.CharField()
     quarter = models.IntegerField()
     campus = models.IntegerField()
     comments = models.TextField()
     user = models.CharField(max_length=12)
     applicants = []
+    workspace_id = models.IntegerField()
 
 
 class CohortAssignment(Assignment):
     cohort_number = models.IntegerField()
     override_previous = models.BooleanField()
     override_protected = models.BooleanField()
 
@@ -119,15 +120,16 @@
                 'cohortNbr': int(self.cohort_number),
                 'overridePreviousCohort': self.override_previous,
                 'overridePreviousProtectedCohort': self.override_protected,
                 'assignmentDetail': {'assignmentType': self.assignment_type,
                                      'academicQtrKeyId': self.quarter,
                                      'campus': int(self.campus),
                                      'comments': self.comments,
-                                     'decisionImportUser': self.user}
+                                     'decisionImportUser': self.user,
+                                     'workspaceId': self.workspace_id}
                 }
 
 
 class MajorAssignment(Assignment):
     major_code = models.CharField()
 
     def json_data(self):
@@ -136,28 +138,30 @@
             applicant_json.append(application.json_data())
         return {'applicants': applicant_json,
                 'majorProgramCode': self.major_code,
                 'assignmentDetail': {'assignmentType': self.assignment_type,
                                      'academicQtrKeyId': self.quarter,
                                      'campus': int(self.campus),
                                      'comments': self.comments,
-                                     'decisionImportUser': self.user}
+                                     'decisionImportUser': self.user,
+                                     'workspaceId': self.workspace_id}
                 }
 
 
 class PurpleGoldAssignment(Assignment):
     def json_data(self):
         applicant_json = []
         for application in self.applicants:
             applicant_json.append(application.json_data())
         return {'applicants': applicant_json,
                 'assignmentDetail': {'assignmentType': self.assignment_type,
                                      'academicQtrKeyId': self.quarter,
                                      'comments': self.comments,
-                                     'decisionImportUser': self.user}
+                                     'decisionImportUser': self.user,
+                                     'workspaceId': self.workspace_id}
                 }
 
 
 class DecisionAssignment(Assignment):
     decision = models.CharField()
     decision_number = models.IntegerField()
 
@@ -169,15 +173,16 @@
                 'assignmentDetail': {'assignmentType': self.assignment_type,
                                      'assignmentCategory':
                                          "DepartmentalDecision",
                                      'academicQtrKeyId': self.quarter,
                                      'campus': int(self.campus),
                                      'comments': self.comments,
                                      'decisionImportUser': self.user,
-                                     'decisionNumber': self.decision_number}
+                                     'decisionNumber': self.decision_number,
+                                     'workspaceId': self.workspace_id}
                 }
 
 
 class AdminMajor(models.Model):
     major_id = models.IntegerField()
     major_abbr = models.CharField(max_length=32)
     begin_academic_qtr_key_id = models.IntegerField()
```

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/activities`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage&systemKey=12345` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage&systemKey=12345`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20194` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20194`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/major/1` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/major/1`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/major/2` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/major/2`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/majors` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/majors`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/majorvalues` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/admin/majorvalues`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/0/123` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/applications/0/123`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/0/all` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/applications/0/all`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/0` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/0`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/cohorts/0` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/cohorts/0`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/cohorts/0?Page=2` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/cohorts/0?Page=2`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/cohorts/1` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/cohorts/1`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=0` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=0`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=1` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=1`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/filter` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/filter`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=1&Limit=100` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=1&Limit=100`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=2&Limit=100` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=2&Limit=100`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/1?Page=1&Limit=100` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/majors/details/1?Page=1&Limit=100`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/workspaces/20194` & `UW-RestClients-AdSel-1.9.3/uw_adsel/resources/adsel/file/api/v1/workspaces/20194`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.2/uw_adsel/tests/test_adsel.py` & `UW-RestClients-AdSel-1.9.3/uw_adsel/tests/test_adsel.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,37 +115,41 @@
         cohort_assign.cohort_number = 1
         cohort_assign.override_protected = True
         cohort_assign.override_previous = False
         cohort_assign.quarter = 0
         cohort_assign.campus = 1
         cohort_assign.comments = "My comment"
         cohort_assign.user = "javerage"
+        cohort_assign.workspace_id = 1
 
         cohort_json = cohort_assign.json_data()
         self.assertEqual(cohort_json['overridePreviousCohort'], False)
         self.assertEqual(cohort_json['overridePreviousProtectedCohort'], True)
+        self.assertEqual(cohort_json['assignmentDetail']['workspaceId'], 1)
 
         try:
             submission = self.adsel.assign_cohorts_bulk(cohort_assign)
         except Exception:
             self.fail('assign_cohorts raised an exception')
 
         major_assign = MajorAssignment()
         major_assign.applicants = [a1, a2]
         major_assign.assignment_type = "upload"
         major_assign.major_code = "CSE"
         major_assign.quarter = 0
         major_assign.campus = 1
         major_assign.comments = "My comment"
         major_assign.user = "javerage"
+        major_assign.workspace_id = 1
 
         major_json = major_assign.json_data()
         self.assertEqual(len(major_json['applicants']), 2)
         self.assertEqual(major_json['applicants'][0]['admissionSelectionId'],
                          123)
+        self.assertEqual(major_json['assignmentDetail']['workspaceId'], 1)
 
         try:
             submission = self.adsel.assign_majors(major_assign)
         except Exception:
             self.fail('assign_majors raised an exception')
 
     def test_get_all_app(self):
@@ -167,17 +171,19 @@
         purple_gold_assign = PurpleGoldAssignment()
         purple_gold_assign.applicants = [a1, a2]
         purple_gold_assign.assignment_type = "upload"
         purple_gold_assign.quarter = 0
         purple_gold_assign.campus = 1
         purple_gold_assign.comments = "My comment"
         purple_gold_assign.user = "javerage"
+        purple_gold_assign.workspace_id = 1
 
         json_data = purple_gold_assign.json_data()
         self.assertEqual(json_data['applicants'][0]['awardAmount'], 1000)
+        self.assertEqual(json_data['assignmentDetail']['workspaceId'], 1)
 
         try:
             submission = self.adsel.assign_purple_gold(purple_gold_assign)
         except Exception:
             self.fail('assign_purple_gold raised an exception')
 
     def test_get_major_details(self):
@@ -213,21 +219,23 @@
         dd_assign.applicants = [a1, a2]
         dd_assign.assignment_type = "upload"
         dd_assign.quarter = 0
         dd_assign.campus = 1
         dd_assign.comments = "My comment"
         dd_assign.user = "javerage"
         dd_assign.decision_number = 1
+        dd_assign.workspace_id = 1
 
         json_data = dd_assign.json_data()
         self.assertEqual(json_data['applicants'][0]['departmentalDecisionId'],
                          1)
         self.assertEqual(json_data['assignmentDetail']['assignmentCategory'],
                          "DepartmentalDecision")
         self.assertEqual(json_data['assignmentDetail']['decisionNumber'], 1)
+        self.assertEqual(json_data['assignmentDetail']['workspaceId'], 1)
 
         try:
             submission = self.adsel.assign_decisions(dd_assign)
         except Exception:
             self.fail('assign_decisions raised an exception')
 
     def test_admin_majors(self):
```

