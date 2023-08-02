# Comparing `tmp/pymoises-1.0.2.tar.gz` & `tmp/pymoises-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymoises-1.0.2.tar", last modified: Fri Jul 21 22:43:41 2023, max compression
+gzip compressed data, was "pymoises-1.0.3.tar", last modified: Wed Aug  2 23:43:08 2023, max compression
```

## Comparing `pymoises-1.0.2.tar` & `pymoises-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.717754 pymoises-1.0.2/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      176 2023-07-21 22:43:41.717754 pymoises-1.0.2/PKG-INFO
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       12 2023-06-28 15:16:17.000000 pymoises-1.0.2/README.md
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.689754 pymoises-1.0.2/pymoises/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5064 2023-07-21 22:42:47.000000 pymoises-1.0.2/pymoises/Transactions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       69 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9882 2023-07-21 20:48:22.000000 pymoises-1.0.2/pymoises/customer.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.689754 pymoises-1.0.2/pymoises/dto/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       42 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/__init__.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.689754 pymoises-1.0.2/pymoises/dto/input/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       51 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/input/__init__.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.705754 pymoises-1.0.2/pymoises/dto/input/customer/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       85 2023-07-21 19:59:10.000000 pymoises-1.0.2/pymoises/dto/input/customer/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      516 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1527 2023-07-21 20:19:10.000000 pymoises-1.0.2/pymoises/dto/input/customer/createLead_input_dto.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.705754 pymoises-1.0.2/pymoises/dto/input/transaction/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       43 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/input/transaction/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      509 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/input/transaction/create_transaction_input_dto.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.709754 pymoises-1.0.2/pymoises/dto/output/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       50 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/output/__init__.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.713754 pymoises-1.0.2/pymoises/dto/output/customer/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      106 2023-07-21 20:02:48.000000 pymoises-1.0.2/pymoises/dto/output/customer/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      737 2023-07-21 20:31:25.000000 pymoises-1.0.2/pymoises/dto/output/customer/createLead_output_dto.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1159 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/output/customer/customer_output_dto.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      907 2023-07-17 15:29:47.000000 pymoises-1.0.2/pymoises/dto/output/customer/moveLead_output_dto.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.717754 pymoises-1.0.2/pymoises/dto/output/transaction/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       37 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/output/transaction/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      538 2023-06-28 15:16:17.000000 pymoises-1.0.2/pymoises/dto/output/transaction/transaction_output_dto.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-07-21 22:43:41.689754 pymoises-1.0.2/pymoises.egg-info/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      176 2023-07-21 22:43:41.000000 pymoises-1.0.2/pymoises.egg-info/PKG-INFO
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      897 2023-07-21 22:43:41.000000 pymoises-1.0.2/pymoises.egg-info/SOURCES.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)        1 2023-07-21 22:43:41.000000 pymoises-1.0.2/pymoises.egg-info/dependency_links.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       21 2023-07-21 22:43:41.000000 pymoises-1.0.2/pymoises.egg-info/requires.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)        9 2023-07-21 22:43:41.000000 pymoises-1.0.2/pymoises.egg-info/top_level.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       38 2023-07-21 22:43:41.717754 pymoises-1.0.2/setup.cfg
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      504 2023-07-21 22:43:00.000000 pymoises-1.0.2/setup.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-08-02 23:43:08.322781 pymoises-1.0.3/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      176 2023-08-02 23:43:08.322781 pymoises-1.0.3/PKG-INFO
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       12 2023-06-28 15:16:17.000000 pymoises-1.0.3/README.md
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-08-02 23:43:08.318781 pymoises-1.0.3/pymoises/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5064 2023-07-21 22:42:47.000000 pymoises-1.0.3/pymoises/Transactions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       92 2023-08-02 22:06:28.000000 pymoises-1.0.3/pymoises/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9882 2023-07-21 20:48:22.000000 pymoises-1.0.3/pymoises/customer.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-08-02 23:43:08.318781 pymoises-1.0.3/pymoises/dto/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       42 2023-06-28 15:16:17.000000 pymoises-1.0.3/pymoises/dto/__init__.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-08-02 23:43:08.318781 pymoises-1.0.3/pymoises/dto/input/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       51 2023-06-28 15:16:17.000000 pymoises-1.0.3/pymoises/dto/input/__init__.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-08-02 23:43:08.318781 pymoises-1.0.3/pymoises/dto/input/customer/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       85 2023-07-21 19:59:10.000000 pymoises-1.0.3/pymoises/dto/input/customer/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      516 2023-06-28 15:16:17.000000 pymoises-1.0.3/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1527 2023-07-21 20:19:10.000000 pymoises-1.0.3/pymoises/dto/input/customer/createLead_input_dto.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-08-02 23:43:08.318781 pymoises-1.0.3/pymoises/dto/input/transaction/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       43 2023-06-28 15:16:17.000000 pymoises-1.0.3/pymoises/dto/input/transaction/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      509 2023-06-28 15:16:17.000000 pymoises-1.0.3/pymoises/dto/input/transaction/create_transaction_input_dto.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-08-02 23:43:08.318781 pymoises-1.0.3/pymoises/dto/output/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       50 2023-06-28 15:16:17.000000 pymoises-1.0.3/pymoises/dto/output/__init__.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-08-02 23:43:08.322781 pymoises-1.0.3/pymoises/dto/output/customer/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      106 2023-07-21 20:02:48.000000 pymoises-1.0.3/pymoises/dto/output/customer/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      737 2023-07-21 20:31:25.000000 pymoises-1.0.3/pymoises/dto/output/customer/createLead_output_dto.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1159 2023-06-28 15:16:17.000000 pymoises-1.0.3/pymoises/dto/output/customer/customer_output_dto.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      907 2023-07-17 15:29:47.000000 pymoises-1.0.3/pymoises/dto/output/customer/moveLead_output_dto.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-08-02 23:43:08.322781 pymoises-1.0.3/pymoises/dto/output/psps/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)        0 2023-08-02 21:50:20.000000 pymoises-1.0.3/pymoises/dto/output/psps/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1567 2023-08-02 21:55:56.000000 pymoises-1.0.3/pymoises/dto/output/psps/get_info_psp_output_dto.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-08-02 23:43:08.322781 pymoises-1.0.3/pymoises/dto/output/transaction/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       37 2023-06-28 15:16:17.000000 pymoises-1.0.3/pymoises/dto/output/transaction/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      538 2023-06-28 15:16:17.000000 pymoises-1.0.3/pymoises/dto/output/transaction/transaction_output_dto.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1927 2023-08-02 23:37:17.000000 pymoises-1.0.3/pymoises/psps.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-08-02 23:43:08.318781 pymoises-1.0.3/pymoises.egg-info/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      176 2023-08-02 23:43:08.000000 pymoises-1.0.3/pymoises.egg-info/PKG-INFO
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1003 2023-08-02 23:43:08.000000 pymoises-1.0.3/pymoises.egg-info/SOURCES.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)        1 2023-08-02 23:43:08.000000 pymoises-1.0.3/pymoises.egg-info/dependency_links.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       21 2023-08-02 23:43:08.000000 pymoises-1.0.3/pymoises.egg-info/requires.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)        9 2023-08-02 23:43:08.000000 pymoises-1.0.3/pymoises.egg-info/top_level.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       38 2023-08-02 23:43:08.322781 pymoises-1.0.3/setup.cfg
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      539 2023-08-02 23:42:56.000000 pymoises-1.0.3/setup.py
```

### Comparing `pymoises-1.0.2/pymoises/Transactions.py` & `pymoises-1.0.3/pymoises/Transactions.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.2/pymoises/customer.py` & `pymoises-1.0.3/pymoises/customer.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.2/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py` & `pymoises-1.0.3/pymoises/dto/input/customer/checkEmailPhone_customer_input_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.2/pymoises/dto/input/customer/createLead_input_dto.py` & `pymoises-1.0.3/pymoises/dto/input/customer/createLead_input_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.2/pymoises/dto/output/customer/createLead_output_dto.py` & `pymoises-1.0.3/pymoises/dto/output/customer/createLead_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.2/pymoises/dto/output/customer/customer_output_dto.py` & `pymoises-1.0.3/pymoises/dto/output/customer/customer_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.2/pymoises/dto/output/customer/moveLead_output_dto.py` & `pymoises-1.0.3/pymoises/dto/output/customer/moveLead_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.2/pymoises/dto/output/transaction/transaction_output_dto.py` & `pymoises-1.0.3/pymoises/dto/output/transaction/transaction_output_dto.py`

 * *Files identical despite different names*

### Comparing `pymoises-1.0.2/pymoises.egg-info/SOURCES.txt` & `pymoises-1.0.3/pymoises.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.md
 setup.py
 pymoises/Transactions.py
 pymoises/__init__.py
 pymoises/customer.py
+pymoises/psps.py
 pymoises.egg-info/PKG-INFO
 pymoises.egg-info/SOURCES.txt
 pymoises.egg-info/dependency_links.txt
 pymoises.egg-info/requires.txt
 pymoises.egg-info/top_level.txt
 pymoises/dto/__init__.py
 pymoises/dto/input/__init__.py
@@ -16,9 +17,11 @@
 pymoises/dto/input/transaction/__init__.py
 pymoises/dto/input/transaction/create_transaction_input_dto.py
 pymoises/dto/output/__init__.py
 pymoises/dto/output/customer/__init__.py
 pymoises/dto/output/customer/createLead_output_dto.py
 pymoises/dto/output/customer/customer_output_dto.py
 pymoises/dto/output/customer/moveLead_output_dto.py
+pymoises/dto/output/psps/__init__.py
+pymoises/dto/output/psps/get_info_psp_output_dto.py
 pymoises/dto/output/transaction/__init__.py
 pymoises/dto/output/transaction/transaction_output_dto.py
```

