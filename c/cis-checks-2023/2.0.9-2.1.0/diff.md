# Comparing `tmp/cis_checks_2023-2.0.9.tar.gz` & `tmp/cis_checks_2023-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cis_checks_2023-2.0.9.tar", last modified: Fri Apr 14 10:50:28 2023, max compression
+gzip compressed data, was "cis_checks_2023-2.1.0.tar", last modified: Thu Aug  3 15:26:29 2023, max compression
```

## Comparing `cis_checks_2023-2.0.9.tar` & `cis_checks_2023-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 10:50:28.737119 cis_checks_2023-2.0.9/
--rw-rw-rw-   0        0        0      836 2023-04-14 10:50:28.736120 cis_checks_2023-2.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 cis_checks_2023-2.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 10:50:28.712140 cis_checks_2023-2.0.9/cis_checks_2023/
--rw-rw-rw-   0        0        0     6880 2023-04-14 10:49:28.000000 cis_checks_2023-2.0.9/cis_checks_2023/__init__.py
--rw-rw-rw-   0        0        0    35333 2023-04-07 14:21:10.000000 cis_checks_2023-2.0.9/cis_checks_2023/_security_control_5.py
--rw-rw-rw-   0        0        0    55484 2023-04-14 06:00:10.000000 cis_checks_2023-2.0.9/cis_checks_2023/iam_control_1.py
--rw-rw-rw-   0        0        0    25256 2023-04-13 06:34:22.000000 cis_checks_2023-2.0.9/cis_checks_2023/logging_control_3.py
--rw-rw-rw-   0        0        0    79813 2023-04-11 05:42:02.000000 cis_checks_2023-2.0.9/cis_checks_2023/monitoring_control_4.py
--rw-rw-rw-   0        0        0    25055 2023-04-11 07:00:11.000000 cis_checks_2023-2.0.9/cis_checks_2023/networking_control_5.py
--rw-rw-rw-   0        0        0    16019 2023-04-13 09:03:31.000000 cis_checks_2023-2.0.9/cis_checks_2023/storage_control_2.py
--rw-rw-rw-   0        0        0    22117 2023-04-14 10:49:45.000000 cis_checks_2023-2.0.9/cis_checks_2023/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:50:28.732120 cis_checks_2023-2.0.9/cis_checks_2023.egg-info/
--rw-rw-rw-   0        0        0      836 2023-04-14 10:50:28.000000 cis_checks_2023-2.0.9/cis_checks_2023.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-04-14 10:50:28.000000 cis_checks_2023-2.0.9/cis_checks_2023.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 10:50:28.000000 cis_checks_2023-2.0.9/cis_checks_2023.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-14 10:50:28.000000 cis_checks_2023-2.0.9/cis_checks_2023.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      557 2023-04-14 10:49:28.000000 cis_checks_2023-2.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 10:50:28.738119 cis_checks_2023-2.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 15:26:29.426399 cis_checks_2023-2.1.0/
+-rw-rw-rw-   0        0        0      836 2023-08-03 15:26:29.425398 cis_checks_2023-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 cis_checks_2023-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 15:26:29.410484 cis_checks_2023-2.1.0/cis_checks_2023/
+-rw-rw-rw-   0        0        0     9485 2023-08-03 15:25:48.000000 cis_checks_2023-2.1.0/cis_checks_2023/__init__.py
+-rw-rw-rw-   0        0        0    35333 2023-04-07 14:21:10.000000 cis_checks_2023-2.1.0/cis_checks_2023/_security_control_5.py
+-rw-rw-rw-   0        0        0    56156 2023-08-03 13:46:02.000000 cis_checks_2023-2.1.0/cis_checks_2023/iam_control_1.py
+-rw-rw-rw-   0        0        0    25608 2023-08-03 14:00:09.000000 cis_checks_2023-2.1.0/cis_checks_2023/logging_control_3.py
+-rw-rw-rw-   0        0        0    80540 2023-08-03 14:03:00.000000 cis_checks_2023-2.1.0/cis_checks_2023/monitoring_control_4.py
+-rw-rw-rw-   0        0        0    26035 2023-08-03 14:02:59.000000 cis_checks_2023-2.1.0/cis_checks_2023/networking_control_5.py
+-rw-rw-rw-   0        0        0    16339 2023-08-03 14:00:09.000000 cis_checks_2023-2.1.0/cis_checks_2023/storage_control_2.py
+-rw-rw-rw-   0        0        0    22150 2023-05-24 10:33:14.000000 cis_checks_2023-2.1.0/cis_checks_2023/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:26:29.423398 cis_checks_2023-2.1.0/cis_checks_2023.egg-info/
+-rw-rw-rw-   0        0        0      836 2023-08-03 15:26:29.000000 cis_checks_2023-2.1.0/cis_checks_2023.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2023-08-03 15:26:29.000000 cis_checks_2023-2.1.0/cis_checks_2023.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 15:26:29.000000 cis_checks_2023-2.1.0/cis_checks_2023.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-03 15:26:29.000000 cis_checks_2023-2.1.0/cis_checks_2023.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-03 15:26:29.000000 cis_checks_2023-2.1.0/cis_checks_2023.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      604 2023-08-03 13:46:02.000000 cis_checks_2023-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 15:26:29.426399 cis_checks_2023-2.1.0/setup.cfg
```

### Comparing `cis_checks_2023-2.0.9/PKG-INFO` & `cis_checks_2023-2.1.0/cis_checks_2023.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cis_checks_2023
-Version: 2.0.9
+Name: cis-checks-2023
+Version: 2.1.0
 Summary: Provides AWS compliance details
 Author-email: Dheeraj Banodha <dheeraj.banodha@impetus.com>, Ravish Sharma <ravish.sharma@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cis_checks_2023-2.0.9/cis_checks_2023/__init__.py` & `cis_checks_2023-2.1.0/cis_checks_2023/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import datetime
 import logging
 
+import boto3
+import pytz
 from boto3 import session
 
 from cis_checks_2023.logging_control_3 import logging_control
 from cis_checks_2023.monitoring_control_4 import monitoring_control
 from cis_checks_2023.networking_control_5 import networking_control
 from cis_checks_2023.storage_control_2 import storage_control
 from cis_checks_2023.utils import utils
@@ -11,31 +14,83 @@
 from cis_checks_2023.iam_control_1 import iam_control
 
 logging.basicConfig()
 logging.getLogger().setLevel(logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Dheeraj Banodha'
-__version__ = '2.0.9'
+__version__ = '2.1.0'
 
 
 class aws_client(iam_control, utils, storage_control, logging_control, monitoring_control, networking_control):
     def __init__(self, **kwargs):
         """
         @param str aws_access_key_id: AWS Access Key ID
         @param str aws_secret_access_key: AWS Secret Access Key
         """
 
         if 'aws_access_key_id' in kwargs.keys() and 'aws_secret_access_key' in kwargs.keys():
-            self.session = session.Session(
-                aws_access_key_id=kwargs['aws_access_key_id'],
-                aws_secret_access_key=kwargs['aws_secret_access_key'],
-            )
+            if 'iam_role_to_assume' in kwargs.keys():
+                self.iam_role_to_assume = kwargs['iam_role_to_assume']
+                self.sts_client = boto3.client(
+                    'sts',
+                    aws_access_key_id=kwargs['aws_access_key_id'],
+                    aws_secret_access_key=kwargs['aws_secret_access_key'],
+                )
+                self.creds = self.sts_client.assume_role(
+                    RoleArn=self.iam_role_to_assume,
+                    RoleSessionName='RecommenderSession',
+                    DurationSeconds=3600
+                )
+                self.session = session.Session(
+                    aws_access_key_id=self.creds['Credentials']['AccessKeyId'],
+                    aws_secret_access_key=self.creds['Credentials']['SecretAccessKey'],
+                    aws_session_token=self.creds['Credentials']['SessionToken']
+                )
+            else:
+                self.session = session.Session(
+                    aws_access_key_id=kwargs['aws_access_key_id'],
+                    aws_secret_access_key=kwargs['aws_secret_access_key'],
+                )
         elif 'profile_name' in kwargs.keys():
             self.session = session.Session(profile_name=kwargs['profile_name'])
+        elif 'iam_role_to_assume' in kwargs.keys():
+            self.iam_role_to_assume = kwargs['iam_role_to_assume']
+            self.sts_client = boto3.client('sts')
+            self.creds = self.sts_client.assume_role(
+                RoleArn=kwargs['iam_role_to_assume'],
+                RoleSessionName='RecommenderSession',
+                DurationSeconds=3600
+            )
+            self.session = session.Session(
+                aws_access_key_id=self.creds['Credentials']['AccessKeyId'],
+                aws_secret_access_key=self.creds['Credentials']['SecretAccessKey'],
+                aws_session_token=self.creds['Credentials']['SessionToken']
+            )
+
+    # refresh session
+    def refresh_session(self):
+        try:
+            self.sts_client
+        except AttributeError:
+            logger.info('No need to refresh the session!')
+            return
+        remaining_duration_seconds = (
+                self.creds['Credentials']['Expiration'] - datetime.datetime.now(pytz.utc)).total_seconds()
+        if remaining_duration_seconds < 900:
+            self.creds = self.sts_client.assume_role(
+                RoleArn=self.iam_role_to_assume,
+                RoleSessionName='RecommenderSession',
+                DurationSeconds=3600
+            )
+            self.session = session.Session(
+                aws_access_key_id=self.creds['Credentials']['AccessKeyId'],
+                aws_secret_access_key=self.creds['Credentials']['SecretAccessKey'],
+                aws_session_token=self.creds['Credentials']['SessionToken']
+            )
 
     # consolidate compliance.py details
     def get_compliance(self) -> list:
         """
         :return list: consolidated list  of compliance.py checks
         """
         logger.info(" ---Inside get_compliance()")
```

### Comparing `cis_checks_2023-2.0.9/cis_checks_2023/_security_control_5.py` & `cis_checks_2023-2.1.0/cis_checks_2023/_security_control_5.py`

 * *Files identical despite different names*

### Comparing `cis_checks_2023-2.0.9/cis_checks_2023/iam_control_1.py` & `cis_checks_2023-2.1.0/cis_checks_2023/iam_control_1.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 # --- 1 Identity and Access Management ---
 
 class iam_control:
     # 1.01 Maintain current contact details
     def control_1_01_maintain_contact_details(self):
         logger.info(" ---Inside iam_control_1 :: control_1_01_maintain_contact_details()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Manual"
         offenders = []
@@ -52,14 +53,15 @@
         failReason = "Control not implemented using API, please verify manually"
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.02 Ensure security contact information is registered
     def control_1_02_security_contact_information_registered(self):
         logger.info(" ---Inside iam_control_1 :: control_1_02_security_contact_information_registered()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Manual"
         offenders = []
@@ -69,14 +71,15 @@
         failReason = "Control not implemented using API, please verify manually"
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.03 Ensure security questions are registered in the AWS account (Not Scored/Manual)
     def control_1_03_security_questions_registered(self):
         logger.info(" ---Inside iam_control_1 :: control_1_03_security_questions_registered()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Manual"
         offenders = []
@@ -86,14 +89,15 @@
         failReason = "Control not implemented using API, please verify manually"
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.04 Ensure no root account access key exists (Scored)
     def control_1_04_root_key_exists(self, credreport):
         logger.info(" ---Inside iam_control_1 :: control_1_04_root_key_exists()--- ")
+        self.refresh_session()
         """Summary
     
         Args:
             credreport (TYPE): Description
     
         Returns:
             TYPE: Description
@@ -110,14 +114,15 @@
             offenders.append('root')
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.05 Ensure MFA is enabled for the "root" account (Scored)
     def control_1_05_root_mfa_enabled(self):
         logger.info(" ---Inside iam_control_1 :: control_1_05_root_mfa_enabled()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -133,14 +138,15 @@
             offenders.append('root')
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.06 Ensure hardware MFA is enabled for the "root" account (Scored)
     def control_1_06_root_hardware_mfa_enabled(self):
         logger.info(" ---Inside iam_control_1 :: control_1_06_root_hardware_mfa_enabled()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -170,14 +176,15 @@
             offenders.append('root')
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.07 Avoid the use of the "root" account (Scored)
     def control_1_07_root_use(self, credreport):
         logger.info(" ---Inside iam_control_1 :: control_1_07_root_use()--- ")
+        self.refresh_session()
         """Summary
     
         Args:
             credreport (TYPE): Description
     
         Returns:
             TYPE: Description
@@ -234,14 +241,15 @@
                 logger.error("Something went wrong")
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.08 Ensure IAM password policy requires minimum length of 14 or greater (Scored)
     def control_1_08_password_policy_length(self, passwordpolicy):
         logger.info(" ---Inside iam_control_1 :: control_1_08_password_policy_length()--- ")
+        self.refresh_session()
         """Summary
     
         Args:
             passwordpolicy (TYPE): Description
     
         Returns:
             TYPE: Description
@@ -261,14 +269,15 @@
                 failReason = "Password policy does not require at least 14 characters"
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.09 Ensure IAM password policy prevents password reuse (Scored)
     def control_1_09_password_policy_reuse(self, passwordpolicy):
         logger.info(" ---Inside iam_control_1 :: control_1_09_password_policy_reuse()--- ")
+        self.refresh_session()
         """Summary
     
         Args:
             passwordpolicy (TYPE): Description
     
         Returns:
             TYPE: Description
@@ -294,14 +303,15 @@
                 failReason = "Password policy does not prevent reusing last 24 passwords"
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.10 Ensure multifactor authentication (MFA) is enabled for all IAM users that have a console password (Scored)
     def control_1_10_mfa_on_password_enabled_iam(self, credreport):
         logger.info(" ---Inside iam_control_1 :: control_1_10_mfa_on_password_enabled_iam()--- ")
+        self.refresh_session()
         """Summary
     
         Args:
             credreport (TYPE): Description
     
         Returns:
             TYPE: Description
@@ -323,14 +333,15 @@
                     offenders.append(str(credreport[i]['arn']))
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.11 Do not set up access keys during initial user setup for all IAM users that have a console password
     def control_1_11_no_accesskey_on_initial_setup(self, credreport):
         logger.info(" ---Inside iam_control_1 :: control_1_11_no_accesskey_on_initial_setup()--- ")
+        self.refresh_session()
         """Summary
     
         Args:
             credreport (TYPE): Description
     
         Returns:
             TYPE: Description
@@ -351,14 +362,15 @@
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.12 Ensure credentials unused for 90 days or greater are disabled (Scored)
     def control_1_12_unused_credentials(self, credreport):
         logger.info(" ---Inside iam_control_1 :: control_1_12_unused_credentials()--- ")
+        self.refresh_session()
         """Summary
     
         Args:
             credreport (TYPE): Description
     
         Returns:
             TYPE: Description
@@ -417,14 +429,15 @@
     def control_1_13_one_active_key(self, credsreport):
         """
         :param self:
         :param credsreport:
         :return:
         """
         logger.info(" ---Inside iam_control_1 :: control_1_13_one_active_key()--- ")
+        self.refresh_session()
 
         result = "Compliant"
         failReason = ""
         offenders = []
         control = "1.13"
         description = "Ensure there is only one active access key for single IAM user"
         scored = True
@@ -448,14 +461,15 @@
             'ControlId': control
         }
 
     # 1.14 Ensure access keys are rotated every 90 days or less
 
     def control_1_14_ensure_access_keys_are_rotated_90_days(self):
         logger.info(" ---Inside iam_control_1 :: control_1_14_ensure_access_keys_are_rotated_90_days()---")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -502,14 +516,15 @@
             'Description': description,
             'ControlId': control
         }
 
     # 1.15 Ensure IAM policies are attached only to groups or roles (Scored)
     def control_1_15_no_policies_on_iam_users(self):
         logger.info(" ---Inside iam_control_1 :: control_1_15_no_policies_on_iam_users()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -537,14 +552,15 @@
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.16 Ensure IAM policies that allow full "*:*" administrative privileges are not attached (Scored)
     def control_1_16_no_policies_with_full_administrative_privileges(self):
         logger.info(
             " ---Inside iam_control_1 :: control_1_16_no_policies_with_full_administrative_privileges()--- ")
+        self.refresh_session()
         """Summary
 
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -607,14 +623,15 @@
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.17 Ensure a support role has been created to manage incidents with AWS Support (Scored)
     def control_1_17_AWS_support_role_created(self):
         logger.info(" ---Inside iam_control_1 :: control_1_17_AWS_support_role_created()--- ")
+        self.refresh_session()
         """Summary
     
         Args:
     
         Returns:
             TYPE: Description
         """
@@ -641,14 +658,15 @@
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.18 Ensure IAM instance roles are used for AWS resource access from instances
     def control_1_18_iam_instance_role_for_access_from_instances(self):
         logger.info(" ---Inside iam_control_1 :: control_1_18_iam_instance_role_for_access_from_instances()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Manual"
         failReason = ""
@@ -660,14 +678,15 @@
         failReason = "Control not implemented using API, please verify manually"
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 1.19 Ensure that all the expired SSL/TLS certificates stored in AWS IAM are removed
     def control_1_19_expired_ssl_tls_certificates_removed(self, regions: list) -> dict:
         logger.info(" ---Inside iam_control_1 :: control_1_19_expired_ssl_tls_certificates_removed")
+        self.refresh_session()
 
         """Summary
         
         Returns:
             TYPE: dict
         """
         result = "Compliant"
@@ -715,14 +734,15 @@
             'Description': description,
             'ControlId': control
         }
 
     # 1.2 Ensure that IAM Access analyzer is enabled for all regions
     def control_1_2_iam_access_analyzer_enabled(self, regions: list) -> dict:
         logger.info(" ---Inside iam_control_1 :: control_1_2_iam_access_analyzer_enabled")
+        self.refresh_session()
 
         """Summary
         
         Returns:
             TYPE: dict
         """
         result = "Compliant"
@@ -763,14 +783,15 @@
         }
 
         # 1.21 Ensure IAM users are managed centrally via identity federation or AWS Organizations for multi-account
 
     # environments
     def control_1_21_iam_user_managed_centrally(self):
         logger.info(" ---Inside iam_control_1 :: control_1_21_iam_user_managed_centrally()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Manual"
         offenders = []
```

### Comparing `cis_checks_2023-2.0.9/cis_checks_2023/logging_control_3.py` & `cis_checks_2023-2.1.0/cis_checks_2023/logging_control_3.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # --- 3 Logging ---
 
 
 class logging_control:
     # 3.01 Ensure CloudTrail is enabled in all regions (Scored)
     def control_3_01_ensure_cloud_trail_all_regions(self, cloudtrails):
         logger.info(" ---Inside logging_control_3 :: control_3_01_ensure_cloud_trail_all_regions()--- ")
+        self.refresh_session()
         """Summary
     
         Args:
             cloudtrails (TYPE): Description
     
         Returns:
             TYPE: Description
@@ -52,14 +53,15 @@
             failReason = "No enabled multi region trails found"
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 3.02 Ensure CloudTrail log file validation is enabled (Scored)
     def control_3_02_ensure_cloudtrail_validation(self, cloudtrails):
         logger.info(" ---Inside logging_control_3 :: control_3_02_ensure_cloudtrail_validation()--- ")
+        self.refresh_session()
         """Summary
     
         Args:
             cloudtrails (TYPE): Description
     
         Returns:
             TYPE: Description
@@ -84,14 +86,15 @@
         offenders = list(offenders)
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 3.03 Ensure the S3 bucket CloudTrail logs to is not publicly accessible (Scored)
     def control_3_03_ensure_cloudtrail_bucket_not_public(self, cloudtrails):
         logger.info(" ---Inside logging_control_3 :: control_3_03_ensure_cloudtrail_bucket_not_public()--- ")
+        self.refresh_session()
         """Summary
     
         Args:
             cloudtrails (TYPE): Description
     
         Returns:
             TYPE: Description
@@ -139,14 +142,15 @@
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 3.04 Ensure CloudTrail trails are integrated with CloudWatch Logs (Scored)
     def control_3_04_ensure_cloudtrail_cloudwatch_logs_integration(self, cloudtrails):
         logger.info(" ---Inside logging_control_3 :: control_3_04_ensure_cloudtrail_cloudwatch_logs_integration()--- ")
+        self.refresh_session()
         """Summary
     
         Args:
             cloudtrails (TYPE): Description
     
         Returns:
             TYPE: Description
@@ -176,14 +180,15 @@
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 3.05 Ensure AWS Config is enabled in all regions (Scored)
     def control_3_05_ensure_config_all_regions(self, regions):
         logger.info(" ---Inside logging_control_3 :: control_3_05_ensure_config_all_regions()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -256,14 +261,15 @@
             offenders.append("Global:NotRecording")
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 3.06 Ensure S3 bucket access logging is enabled on the CloudTrail S3 bucket (Scored)
     def control_3_06_ensure_cloudtrail_bucket_logging(self, cloudtrails):
         logger.info(" ---Inside logging_control_3 :: control_3_06_ensure_cloudtrail_bucket_logging()--- ")
+        self.refresh_session()
         """Summary
     
         Args:
             cloudtrails (TYPE): Description
     
         Returns:
             TYPE: Description
@@ -296,14 +302,15 @@
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 3.07 Ensure CloudTrail logs are encrypted at rest using KMS CMKs (Scored)
     def control_3_07_ensure_cloudtrail_encryption_kms(self, cloudtrails):
         logger.info(" ---Inside logging_control_3 :: control_3_07_ensure_cloudtrail_encryption_kms()--- ")
+        self.refresh_session()
         """Summary
     
         Args:
             cloudtrails (TYPE): Description
     
         Returns:
             TYPE: Description
@@ -329,14 +336,15 @@
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 3.08 Ensure rotation for customer created CMKs is enabled (Scored)
     def control_3_08_ensure_kms_cmk_rotation(self, regions):
         logger.info(" ---Inside logging_control_3 :: control_3_08_ensure_kms_cmk_rotation()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -367,14 +375,15 @@
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 3.09 Ensure VPC flow logging is enabled in all VPCs (Scored)
     def control_3_09_ensure_flow_logs_enabled_on_all_vpc(self, regions):
         logger.info(" ---Inside networking_control_3 :: control_3_09_ensure_flow_logs_enabled_on_all_vpc()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -409,14 +418,15 @@
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
    # 3.1 Ensure that Object-level logging for write events is enabled for S3 bucket
 
     def control_3_1_ensure_logging_enabled_for_s3_write(self, regions):
         logger.info(" ---Inside networking_control_3 :: control_3_1_ensure_logging_enabled_for_s3_write()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -470,14 +480,15 @@
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 3.11 Ensure that Object-level logging for read events is enabled for S3 bucket
 
     def control_3_1_1_ensure_logging_enabled_for_s3_read(self, regions):
         logger.info(" ---Inside networking_control_3 :: control_3_1_1_ensure_logging_enabled_for_s3_read()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
```

### Comparing `cis_checks_2023-2.0.9/cis_checks_2023/monitoring_control_4.py` & `cis_checks_2023-2.1.0/cis_checks_2023/monitoring_control_4.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 
 class monitoring_control:
     # 4.01 Ensure a log metric filter and alarm exist for unauthorized API calls (Scored)
     def control_4_0_1_ensure_log_metric_filter_unauthorized_api_calls(self, cloudtrails):
         logger.info(
             " ---Inside monitoring_control_4 :: control_4_0_1_ensure_log_metric_filter_unauthorized_api_calls()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         offenders = []
@@ -97,14 +98,15 @@
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 4.02 Ensure a log metric filter and alarm exist for Management Console sign-in without MFA (Scored)
     def control_4_0_2_ensure_log_metric_filter_console_signin_no_mfa(self, cloudtrails):
         logger.info(
             " ---Inside monitoring_control_4 :: control_4_0_2_ensure_log_metric_filter_console_signin_no_mfa()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         offenders = []
@@ -164,14 +166,15 @@
             logger.error(" No details found for CloudTrail!!! ")
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 4.03 Ensure a log metric filter and alarm exist for usage of "root" account (Scored)
     def control_4_0_3_ensure_log_metric_filter_root_usage(self, cloudtrails):
         logger.info(" ---Inside monitoring_control_4 :: control_4_0_3_ensure_log_metric_filter_root_usage()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         failReason = ""
@@ -229,14 +232,15 @@
             logger.error(" No details found for CloudTrail!!! ")
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 4.04 Ensure a log metric filter and alarm exist for IAM policy changes  (Scored)
     def control_4_0_4_ensure_log_metric_iam_policy_change(self, cloudtrails):
         logger.info(" ---Inside monitoring_control_4 :: control_4_0_4_ensure_log_metric_iam_policy_change()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         ""
@@ -308,14 +312,15 @@
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 4.05 Ensure a log metric filter and alarm exist for CloudTrail configuration changes (Scored)
     def control_4_0_5_ensure_log_metric_cloudtrail_configuration_changes(self, cloudtrails):
         logger.info(
             " ---Inside monitoring_control_4 :: control_4_0_5_ensure_log_metric_cloudtrail_configuration_changes()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         failReason = ""
@@ -375,14 +380,15 @@
             logger.error(" No details found for CloudTrail!!! ")
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 4.06 Ensure a log metric filter and alarm exist for AWS Management Console authentication failures (Scored)
     def control_4_0_6_ensure_log_metric_console_auth_failures(self, cloudtrails):
         logger.info(" ---Inside monitoring_control_4 :: control_4_0_6_ensure_log_metric_console_auth_failures()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         failReason = ""
@@ -441,14 +447,15 @@
                 'Description': description, 'ControlId': control}
 
     # 4.07 Ensure a log metric filter and alarm exist for disabling or scheduled deletion of customer created CMKs (
     # Scored)
     def control_4_0_7_ensure_log_metric_disabling_scheduled_delete_of_kms_cmk(self, cloudtrails):
         logger.info(
             " ---Inside monitoring_control_4 :: control_4_0_7_ensure_log_metric_disabling_scheduled_delete_of_kms_cmk()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         failReason = ""
@@ -506,14 +513,15 @@
             logger.error(" No details found for CloudTrail!!! ")
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 4.08 Ensure a log metric filter and alarm exist for S3 bucket policy changes (Scored)
     def control_4_0_8_ensure_log_metric_s3_bucket_policy_changes(self, cloudtrails):
         logger.info(" ---Inside monitoring_control_4 :: control_4_0_8_ensure_log_metric_s3_bucket_policy_changes()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         failReason = ""
@@ -579,14 +587,15 @@
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 4.09 Ensure a log metric filter and alarm exist for AWS Config configuration changes (Scored)
     def control_4_0_9_ensure_log_metric_config_configuration_changes(self, cloudtrails):
         logger.info(
             " ---Inside monitoring_control_4 :: control_4_0_9_ensure_log_metric_config_configuration_changes()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         failReason = ""
@@ -646,14 +655,15 @@
             logger.error(" No details found for CloudTrail!!! ")
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 4.1 Ensure a log metric filter and alarm exist for security group changes (Scored)
     def control_4_1_ensure_log_metric_security_group_changes(self, cloudtrails):
         logger.info(" ---Inside monitoring_control_4 :: control_4_1_ensure_log_metric_security_group_changes()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         failReason = ""
@@ -714,14 +724,15 @@
             logger.error(" No details found for CloudTrail!!! ")
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 4.11 Ensure a log metric filter and alarm exist for changes to Network Access Control Lists (NACL) (Scored)
     def control_4_11_ensure_log_metric_nacl(self, cloudtrails):
         logger.info(" ---Inside monitoring_control_4 :: control_4_11_ensure_log_metric_nacl()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         failReason = ""
@@ -783,14 +794,15 @@
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 4.12 Ensure a log metric filter and alarm exist for changes to network gateways (Scored)
     def control_4_12_ensure_log_metric_changes_to_network_gateways(self, cloudtrails):
         logger.info(
             " ---Inside monitoring_control_4 :: control_4_12_ensure_log_metric_changes_to_network_gateways()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         failReason = ""
@@ -851,14 +863,15 @@
             logger.error(" No details found for CloudTrail!!! ")
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 4.13 Ensure a log metric filter and alarm exist for route table changes (Scored)
     def control_4_13_ensure_log_metric_changes_to_route_tables(self, cloudtrails):
         logger.info(" ---Inside monitoring_control_4 :: control_4_13_ensure_log_metric_changes_to_route_tables()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         failReason = ""
@@ -920,14 +933,15 @@
             logger.error(" No details found for CloudTrail!!! ")
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 4.14 Ensure a log metric filter and alarm exist for VPC changes (Scored)
     def control_4_14_ensure_log_metric_changes_to_vpc(self, cloudtrails):
         logger.info(" ---Inside monitoring_control_4 :: control_4_14_ensure_log_metric_changes_to_vpc()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         failReason = ""
@@ -992,14 +1006,15 @@
             logger.error(" No details found for CloudTrail!!! ")
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 4.15 Ensure a log metric filter and alarm exist for Organizations changes (Scored)
     def control_4_15_ensure_log_metric_changes_to_org(self, cloudtrails):
         logger.info(" ---Inside monitoring_control_4 :: control_4_15_ensure_log_metric_changes_to_org()--- ")
+        self.refresh_session()
         """Summary
 
         Returns:
             TYPE: Description
         """
         result = "Not Compliant"
         failReason = ""
@@ -1090,14 +1105,15 @@
     # 4.16 Ensure AWS Security Hub is enabled
     def control_4_16_ensure_security_hub_is_enabled(self, regions: list):
         """
         :param self:
         :return:
         """
         logger.info(" ---Inside monitoring_control_4 :: control_4_16_ensure_security_hub_is_enabled()--- ")
+        self.refresh_session()
 
         result = "Not Compliant"
         failReason = "Security hub is enabled"
         offenders = []
         control = "4.16"
         description = "Ensure security hub is enabled"
         scored = True
@@ -1108,112 +1124,112 @@
                 response = client.describe_hub()
                 # Scenario 1: SecurityHub is enabled for an AWS Account
                 if response:
                     pass
             except botocore.exceptions.ClientError as error:
                 # Scenario 2: SecurityHub is not enabled for an AWS account.
                 if error.response['Error']['Code'] == 'InvalidAccessException':
-                    result = False
+                    result = "Not Compliant"
                     offenders.append(region)
                     failReason = "Security hub is not enable in these regions"
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     '''*****************************************************************************'''
 
-    # 3.15 Ensure appropriate subscribers to each SNS topic (Not Scored)
-    def control_3_15_verify_sns_subscribers(self):
-        logger.info(" ---Inside monitoring_control_3 :: control_3_15_verify_sns_subscribers()--- ")
-        """Summary
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Manual"
-        failReason = ""
-        offenders = []
-        control = "3.15"
-        description = "Ensure appropriate subscribers to each SNS topic, please verify manually"
-        scored = False
-        failReason = "Control not implemented using API, please verify manually"
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 3.16 Ensure redshift audit logging is enabled
-    def control_3_16_ensure_redshift_audit_logging_enabled(self, regions: list) -> dict:
-        logger.info(" ---Inside monitoring_control_3 :: control_3_16_ensure_redshift_audit_logging_enabled")
-
-        """Summary
-        
-        Returns:
-            TYPE: dict
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "3.16"
-        description = "Ensure audit logging is enabled in all redshift clusters"
-        scored = True
-        for n in regions:
-            clusters = self.list_redshift_clusters(n)
-            client = self.session.client('redshift', region_name=n)
-
-            for cluster in clusters:
-                response = client.describe_logging_status(
-                    ClusterIdentifier=cluster
-                )
-                if not response['LoggingEnabled']:
-                    result = "Not Compliant"
-                    failReason = "Found Redshift cluster with audit logging disabled"
-                    offenders.append(cluster)
-
-        return {
-            'Result': result,
-            'failReason': failReason,
-            'Offenders': offenders,
-            'ScoredControl': scored,
-            'Description': description,
-            'ControlId': control
-        }
-
-    # 3.17 Ensure ELB access logs are enabled
-    def control_3_17_ensure_elb_access_logs_enabled(self, regions: list) -> dict:
-        logger.info(" ---Inside monitoring_control_3 :: control_3_17_ensure_elb_access_logging_enabled")
-
-        """Summary
-        
-        Returns:
-            TYPE: dict
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "3.17"
-        description = "Ensure access logging is enabled in all load balancers"
-        scored = True
-        for n in regions:
-            elb_lst = self.list_elb(n)
-            client = self.session.client('elb', region_name=n)
-
-            for elb in elb_lst:
-                response = client.describe_load_balancer_attributes(
-                    LoadBalancerName=elb
-                )
-                try:
-                    if not response['LoadBalancerAttributes']['AccessLog']['Enabled']:
-                        result = "Not Compliant"
-                        failReason = "Found load balancer with access logging disabled"
-                        offenders.append(elb)
-                except KeyError:
-                    result = "Not Compliant"
-                    failReason = "Found load balancer with access logging disabled"
-                    offenders.append(elb)
-
-        return {
-            'Result': result,
-            'failReason': failReason,
-            'Offenders': offenders,
-            'ScoredControl': scored,
-            'Description': description,
-            'ControlId': control
-        }
+    # # 3.15 Ensure appropriate subscribers to each SNS topic (Not Scored)
+    # def control_3_15_verify_sns_subscribers(self):
+    #     logger.info(" ---Inside monitoring_control_3 :: control_3_15_verify_sns_subscribers()--- ")
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Manual"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "3.15"
+    #     description = "Ensure appropriate subscribers to each SNS topic, please verify manually"
+    #     scored = False
+    #     failReason = "Control not implemented using API, please verify manually"
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 3.16 Ensure redshift audit logging is enabled
+    # def control_3_16_ensure_redshift_audit_logging_enabled(self, regions: list) -> dict:
+    #     logger.info(" ---Inside monitoring_control_3 :: control_3_16_ensure_redshift_audit_logging_enabled")
+    #
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: dict
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "3.16"
+    #     description = "Ensure audit logging is enabled in all redshift clusters"
+    #     scored = True
+    #     for n in regions:
+    #         clusters = self.list_redshift_clusters(n)
+    #         client = self.session.client('redshift', region_name=n)
+    #
+    #         for cluster in clusters:
+    #             response = client.describe_logging_status(
+    #                 ClusterIdentifier=cluster
+    #             )
+    #             if not response['LoggingEnabled']:
+    #                 result = "Not Compliant"
+    #                 failReason = "Found Redshift cluster with audit logging disabled"
+    #                 offenders.append(cluster)
+    #
+    #     return {
+    #         'Result': result,
+    #         'failReason': failReason,
+    #         'Offenders': offenders,
+    #         'ScoredControl': scored,
+    #         'Description': description,
+    #         'ControlId': control
+    #     }
+    #
+    # # 3.17 Ensure ELB access logs are enabled
+    # def control_3_17_ensure_elb_access_logs_enabled(self, regions: list) -> dict:
+    #     logger.info(" ---Inside monitoring_control_3 :: control_3_17_ensure_elb_access_logging_enabled")
+    #
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: dict
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "3.17"
+    #     description = "Ensure access logging is enabled in all load balancers"
+    #     scored = True
+    #     for n in regions:
+    #         elb_lst = self.list_elb(n)
+    #         client = self.session.client('elb', region_name=n)
+    #
+    #         for elb in elb_lst:
+    #             response = client.describe_load_balancer_attributes(
+    #                 LoadBalancerName=elb
+    #             )
+    #             try:
+    #                 if not response['LoadBalancerAttributes']['AccessLog']['Enabled']:
+    #                     result = "Not Compliant"
+    #                     failReason = "Found load balancer with access logging disabled"
+    #                     offenders.append(elb)
+    #             except KeyError:
+    #                 result = "Not Compliant"
+    #                 failReason = "Found load balancer with access logging disabled"
+    #                 offenders.append(elb)
+    #
+    #     return {
+    #         'Result': result,
+    #         'failReason': failReason,
+    #         'Offenders': offenders,
+    #         'ScoredControl': scored,
+    #         'Description': description,
+    #         'ControlId': control
+    #     }
```

### Comparing `cis_checks_2023-2.0.9/cis_checks_2023/networking_control_5.py` & `cis_checks_2023-2.1.0/cis_checks_2023/networking_control_5.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     def control_5_01_no_nacl_allow_ingress(self, regions):
         """
         :param self:
         :param regions:
         :return:
         """
         logger.info(" ---Inside Networking_control :: control_5_01_no_nacl_allow_ingress()--- ")
+        self.refresh_session()
 
         result = "Compliant"
         failReason = ""
         offenders = []
         control = "5.01"
         description = "Ensure no NACL allow ingress from 0.0.0.0/0 to Admin Ports (22, 3389)"
         scored = True
@@ -77,14 +78,15 @@
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 5.02 Ensure no security groups allow ingress from 0.0.0.0/0 to admin ports (Scored)
     def control_5_02_ensure_admin_ports_open_to_world_over_ipv4(self, regions):
         logger.info(" ---Inside networking_control_5 :: control_5_02_ensure_admin_ports_open_to_world_over_ipv4()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -122,14 +124,15 @@
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 5.03 Ensure no security groups allow ingress from ::/0 to admin ports (Scored)
     def control_5_03_ensure_ports_open_to_world_over_ipv6(self, regions):
         logger.info(" ---Inside networking_control_5 :: control_5_03_ensure_ports_open_to_world_over_ipv6()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -168,14 +171,15 @@
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 5.04 Ensure the default security group of every VPC restricts all traffic (Scored)
     def control_5_04_ensure_default_security_groups_restricts_traffic(self, regions):
         logger.info(
             " ---Inside networking_control_5 :: control_5_04_ensure_default_security_groups_restricts_traffic()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -202,14 +206,15 @@
                     offenders.append(str(n) + " : " + str(m['GroupId']))
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 5.05 Ensure routing tables for VPC peering are "least access" (Not Scored)
     def control_5_05_ensure_route_tables_are_least_access(self, regions):
         logger.info(" ---Inside networking_control_5 :: control_5_05_ensure_route_tables_are_least_access()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -232,283 +237,290 @@
                         pass
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     '''****************************************************************************'''
 
     # 4.2 Ensure no security groups allow ingress from 0.0.0.0/0 to port 3389 (Scored)
-    def control_4_2_ensure_rdp_not_open_to_world(self, regions):
-        logger.info(" ---Inside networking_control_4 :: control_4_2_ensure_rdp_not_open_to_world()--- ")
-        """Summary
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "4.2"
-        description = "Ensure no security groups allow ingress from 0.0.0.0/0 to port 3389"
-        scored = True
-        for n in regions:
-            client = self.session.client('ec2', region_name=n)
-            response = client.describe_security_groups()
-            for m in response['SecurityGroups']:
-                if "0.0.0.0/0" in str(m['IpPermissions']):
-                    for o in m['IpPermissions']:
-                        try:
-                            if int(o['FromPort']) <= 3389 <= int(o['ToPort']) and '0.0.0.0/0' in str(o['IpRanges']):
-                                result = "Not Compliant"
-                                failReason = "Found Security Group with port 3389 open to the world (0.0.0.0/0)"
-                                offenders.append(str(m['GroupId']))
-                        except:
-                            if str(o['IpProtocol']) == "-1" and '0.0.0.0/0' in str(o['IpRanges']):
-                                result = "Not Compliant"
-                                failReason = "Found Security Group with port 3389 open to the world (0.0.0.0/0)"
-                                offenders.append(str(n) + " : " + str(m['GroupId']))
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    def control_4_2_ensure_20_not_open_to_world(self, regions):
-        logger.info(" ---Inside networking_control_4 :: control_4_2_ensure_20_not_open_to_world()--- ")
-        """Summary
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "4.2"
-        description = "Ensure no security groups allow ingress from 0.0.0.0/0 to port 20"
-        scored = True
-        for n in regions:
-            client = self.session.client('ec2', region_name=n)
-            response = client.describe_security_groups()
-            for m in response['SecurityGroups']:
-                if "0.0.0.0/0" in str(m['IpPermissions']):
-                    for o in m['IpPermissions']:
-                        try:
-                            if int(o['FromPort']) <= 20 <= int(o['ToPort']) and '0.0.0.0/0' in str(o['IpRanges']):
-                                result = "Not Compliant"
-                                failReason = "Found Security Group with port 20 open to the world (0.0.0.0/0)"
-                                offenders.append(str(m['GroupId']))
-                        except:
-                            if str(o['IpProtocol']) == "-1" and '0.0.0.0/0' in str(o['IpRanges']):
-                                result = "Not Compliant"
-                                failReason = "Found Security Group with port 20 open to the world (0.0.0.0/0)"
-                                offenders.append(str(n) + " : " + str(m['GroupId']))
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    def control_4_2_ensure_21_not_open_to_world(self, regions):
-        logger.info(" ---Inside networking_control_4 :: control_4_2_ensure_21_not_open_to_world()--- ")
-        """Summary
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "4.2"
-        description = "Ensure no security groups allow ingress from 0.0.0.0/0 to port 21"
-        scored = True
-        for n in regions:
-            client = self.session.client('ec2', region_name=n)
-            response = client.describe_security_groups()
-            for m in response['SecurityGroups']:
-                if "0.0.0.0/0" in str(m['IpPermissions']):
-                    for o in m['IpPermissions']:
-                        try:
-                            if int(o['FromPort']) <= 21 <= int(o['ToPort']) and '0.0.0.0/0' in str(o['IpRanges']):
-                                result = "Not Compliant"
-                                failReason = "Found Security Group with port 21 open to the world (0.0.0.0/0)"
-                                offenders.append(str(m['GroupId']))
-                        except:
-                            if str(o['IpProtocol']) == "-1" and '0.0.0.0/0' in str(o['IpRanges']):
-                                result = "Not Compliant"
-                                failReason = "Found Security Group with port 21 open to the world (0.0.0.0/0)"
-                                offenders.append(str(n) + " : " + str(m['GroupId']))
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    def control_4_2_ensure_3306_not_open_to_world(self, regions):
-        logger.info(" ---Inside networking_control_4 :: control_4_2_ensure_3306_not_open_to_world()--- ")
-        """Summary
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "4.2"
-        description = "Ensure no security groups allow ingress from 0.0.0.0/0 to port 3306"
-        scored = True
-        for n in regions:
-            client = self.session.client('ec2', region_name=n)
-            response = client.describe_security_groups()
-            for m in response['SecurityGroups']:
-                if "0.0.0.0/0" in str(m['IpPermissions']):
-                    for o in m['IpPermissions']:
-                        try:
-                            if int(o['FromPort']) <= 3306 <= int(o['ToPort']) and '0.0.0.0/0' in str(o['IpRanges']):
-                                result = "Not Compliant"
-                                failReason = "Found Security Group with port 3306 open to the world (0.0.0.0/0)"
-                                offenders.append(str(m['GroupId']))
-                        except:
-                            if str(o['IpProtocol']) == "-1" and '0.0.0.0/0' in str(o['IpRanges']):
-                                result = "Not Compliant"
-                                failReason = "Found Security Group with port 3306 open to the world (0.0.0.0/0)"
-                                offenders.append(str(n) + " : " + str(m['GroupId']))
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    def control_4_2_ensure_4333_not_open_to_world(self, regions):
-        logger.info(" ---Inside networking_control_4 :: control_4_2_ensure_4333_not_open_to_world()--- ")
-        """Summary
-    
-        Returns:
-            TYPE: Description
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "4.2"
-        description = "Ensure no security groups allow ingress from 0.0.0.0/0 to port 4333"
-        scored = True
-        for n in regions:
-            client = self.session.client('ec2', region_name=n)
-            response = client.describe_security_groups()
-            for m in response['SecurityGroups']:
-                if "0.0.0.0/0" in str(m['IpPermissions']):
-                    for o in m['IpPermissions']:
-                        try:
-                            if int(o['FromPort']) <= 4333 <= int(o['ToPort']) and '0.0.0.0/0' in str(o['IpRanges']):
-                                result = "Not Compliant"
-                                failReason = "Found Security Group with port 4333 open to the world (0.0.0.0/0)"
-                                offenders.append(str(m['GroupId']))
-                        except:
-                            if str(o['IpProtocol']) == "-1" and '0.0.0.0/0' in str(o['IpRanges']):
-                                result = "Not Compliant"
-                                failReason = "Found Security Group with port 4333 open to the world (0.0.0.0/0)"
-                                offenders.append(str(n) + " : " + str(m['GroupId']))
-        return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
-                'Description': description, 'ControlId': control}
-
-    # 4.6 ensure security group dont have large range of ports open
-    def control_4_6_ensure_sg_dont_have_large_range_of_ports_open(self, regions: list) -> dict:
-        logger.info(" ---Inside networking_control_4 :: control_4_6_ensure_sg_dont_have_large_range_of_ports_open")
-
-        """Summary
-        
-        Returns:
-            TYPE: dict
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = "4.6"
-        description = "Ensure security groups don't have large range of ports open"
-        scored = True
-
-        for region in regions:
-            client = self.session.client('ec2', region_name=region)
-            marker = ''
-            while True:
-                if marker == '' or marker is None:
-                    response = client.describe_security_groups()
-                else:
-                    response = client.describe_security_groups(
-                        NextToken=marker
-                    )
-                for sg in response['SecurityGroups']:
-                    for port_range in sg['IpPermissions']:
-                        try:
-                            count = port_range['ToPort'] - port_range['FromPort']
-                            if count > 1:
-                                result = "Not Compliant"
-                                failReason = "Found Security group with range of port open"
-                                offenders.append(sg['GroupName'])
-                                continue
-                        except KeyError:
-                            continue
-
-                try:
-                    marker = response['NextToken']
-                    if marker == '':
-                        break
-                except:
-                    break
-
-        return {
-            'Result': result,
-            'failReason': failReason,
-            'Offenders': offenders,
-            'ScoredControl': scored,
-            'Description': description,
-            'ControlId': control
-        }
-
-    # 4.7 Ensure use of https for cloudfront distributions
-    def control_4_7_use_https_for_cloudfront_distribution(self) -> dict:
-        logger.info(" ---Inside networking_control_4 :: control_4_7_use_https_for_cloudfront_distribution")
-
-        """Summary
-        
-        Returns:
-            TYPE: dict
-        """
-        result = "Compliant"
-        failReason = ""
-        offenders = []
-        control = '4.7'
-        description = "Use https for cloudfront distributions"
-        scored = True
-
-        client = self.session.client('cloudfront')
-        marker = ''
-        while True:
-            if marker == '' or marker == None:
-                response = client.list_distributions()
-            else:
-                response = client.list_distributions(
-                    Marker=marker
-                )
-            try:
-                for item in response['DistributionList']['Items']:
-                    protocol_policy = item['DefaultCacheBehavior']['ViewerProtocolPolicy']
-                    if protocol_policy == 'allow-all':
-                        result = "Not Compliant"
-                        failReason = "Found cloudfront distribution which accepts http also"
-                        offenders.append(item['Id'])
-                        continue
-
-                    try:
-                        for cache_behaviour in item['CacheBehaviors']['Items']:
-                            protocol_policy = cache_behaviour['ViewerProtocolPolicy']
-                            if protocol_policy == 'allow-all':
-                                result = "Not Compliant"
-                                failReason = "Found cloudfront distribution which accepts http also"
-                                offenders.append(item['Id'])
-                                continue
-
-                    except KeyError:
-                        pass
-            except KeyError:
-                break
-            try:
-                marker = response['NextMarker']
-                if marker == '':
-                    break
-            except KeyError:
-                break
-
-        return {
-            'Result': result,
-            'failReason': failReason,
-            'Offenders': offenders,
-            'ScoredControl': scored,
-            'Description': description,
-            'ControlId': control
-        }
+    # def control_4_2_ensure_rdp_not_open_to_world(self, regions):
+    #     logger.info(" ---Inside networking_control_4 :: control_4_2_ensure_rdp_not_open_to_world()--- ")
+    #     self.refresh_session()
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "4.2"
+    #     description = "Ensure no security groups allow ingress from 0.0.0.0/0 to port 3389"
+    #     scored = True
+    #     for n in regions:
+    #         client = self.session.client('ec2', region_name=n)
+    #         response = client.describe_security_groups()
+    #         for m in response['SecurityGroups']:
+    #             if "0.0.0.0/0" in str(m['IpPermissions']):
+    #                 for o in m['IpPermissions']:
+    #                     try:
+    #                         if int(o['FromPort']) <= 3389 <= int(o['ToPort']) and '0.0.0.0/0' in str(o['IpRanges']):
+    #                             result = "Not Compliant"
+    #                             failReason = "Found Security Group with port 3389 open to the world (0.0.0.0/0)"
+    #                             offenders.append(str(m['GroupId']))
+    #                     except:
+    #                         if str(o['IpProtocol']) == "-1" and '0.0.0.0/0' in str(o['IpRanges']):
+    #                             result = "Not Compliant"
+    #                             failReason = "Found Security Group with port 3389 open to the world (0.0.0.0/0)"
+    #                             offenders.append(str(n) + " : " + str(m['GroupId']))
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # def control_4_2_ensure_20_not_open_to_world(self, regions):
+    #     logger.info(" ---Inside networking_control_4 :: control_4_2_ensure_20_not_open_to_world()--- ")
+    #     self.refresh_session()
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "4.2"
+    #     description = "Ensure no security groups allow ingress from 0.0.0.0/0 to port 20"
+    #     scored = True
+    #     for n in regions:
+    #         client = self.session.client('ec2', region_name=n)
+    #         response = client.describe_security_groups()
+    #         for m in response['SecurityGroups']:
+    #             if "0.0.0.0/0" in str(m['IpPermissions']):
+    #                 for o in m['IpPermissions']:
+    #                     try:
+    #                         if int(o['FromPort']) <= 20 <= int(o['ToPort']) and '0.0.0.0/0' in str(o['IpRanges']):
+    #                             result = "Not Compliant"
+    #                             failReason = "Found Security Group with port 20 open to the world (0.0.0.0/0)"
+    #                             offenders.append(str(m['GroupId']))
+    #                     except:
+    #                         if str(o['IpProtocol']) == "-1" and '0.0.0.0/0' in str(o['IpRanges']):
+    #                             result = "Not Compliant"
+    #                             failReason = "Found Security Group with port 20 open to the world (0.0.0.0/0)"
+    #                             offenders.append(str(n) + " : " + str(m['GroupId']))
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # def control_4_2_ensure_21_not_open_to_world(self, regions):
+    #     logger.info(" ---Inside networking_control_4 :: control_4_2_ensure_21_not_open_to_world()--- ")
+    #     self.refresh_session()
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "4.2"
+    #     description = "Ensure no security groups allow ingress from 0.0.0.0/0 to port 21"
+    #     scored = True
+    #     for n in regions:
+    #         client = self.session.client('ec2', region_name=n)
+    #         response = client.describe_security_groups()
+    #         for m in response['SecurityGroups']:
+    #             if "0.0.0.0/0" in str(m['IpPermissions']):
+    #                 for o in m['IpPermissions']:
+    #                     try:
+    #                         if int(o['FromPort']) <= 21 <= int(o['ToPort']) and '0.0.0.0/0' in str(o['IpRanges']):
+    #                             result = "Not Compliant"
+    #                             failReason = "Found Security Group with port 21 open to the world (0.0.0.0/0)"
+    #                             offenders.append(str(m['GroupId']))
+    #                     except:
+    #                         if str(o['IpProtocol']) == "-1" and '0.0.0.0/0' in str(o['IpRanges']):
+    #                             result = "Not Compliant"
+    #                             failReason = "Found Security Group with port 21 open to the world (0.0.0.0/0)"
+    #                             offenders.append(str(n) + " : " + str(m['GroupId']))
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # def control_4_2_ensure_3306_not_open_to_world(self, regions):
+    #     logger.info(" ---Inside networking_control_4 :: control_4_2_ensure_3306_not_open_to_world()--- ")
+    #     self.refresh_session()
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "4.2"
+    #     description = "Ensure no security groups allow ingress from 0.0.0.0/0 to port 3306"
+    #     scored = True
+    #     for n in regions:
+    #         client = self.session.client('ec2', region_name=n)
+    #         response = client.describe_security_groups()
+    #         for m in response['SecurityGroups']:
+    #             if "0.0.0.0/0" in str(m['IpPermissions']):
+    #                 for o in m['IpPermissions']:
+    #                     try:
+    #                         if int(o['FromPort']) <= 3306 <= int(o['ToPort']) and '0.0.0.0/0' in str(o['IpRanges']):
+    #                             result = "Not Compliant"
+    #                             failReason = "Found Security Group with port 3306 open to the world (0.0.0.0/0)"
+    #                             offenders.append(str(m['GroupId']))
+    #                     except:
+    #                         if str(o['IpProtocol']) == "-1" and '0.0.0.0/0' in str(o['IpRanges']):
+    #                             result = "Not Compliant"
+    #                             failReason = "Found Security Group with port 3306 open to the world (0.0.0.0/0)"
+    #                             offenders.append(str(n) + " : " + str(m['GroupId']))
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # def control_4_2_ensure_4333_not_open_to_world(self, regions):
+    #     logger.info(" ---Inside networking_control_4 :: control_4_2_ensure_4333_not_open_to_world()--- ")
+    #     self.refresh_session()
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: Description
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "4.2"
+    #     description = "Ensure no security groups allow ingress from 0.0.0.0/0 to port 4333"
+    #     scored = True
+    #     for n in regions:
+    #         client = self.session.client('ec2', region_name=n)
+    #         response = client.describe_security_groups()
+    #         for m in response['SecurityGroups']:
+    #             if "0.0.0.0/0" in str(m['IpPermissions']):
+    #                 for o in m['IpPermissions']:
+    #                     try:
+    #                         if int(o['FromPort']) <= 4333 <= int(o['ToPort']) and '0.0.0.0/0' in str(o['IpRanges']):
+    #                             result = "Not Compliant"
+    #                             failReason = "Found Security Group with port 4333 open to the world (0.0.0.0/0)"
+    #                             offenders.append(str(m['GroupId']))
+    #                     except:
+    #                         if str(o['IpProtocol']) == "-1" and '0.0.0.0/0' in str(o['IpRanges']):
+    #                             result = "Not Compliant"
+    #                             failReason = "Found Security Group with port 4333 open to the world (0.0.0.0/0)"
+    #                             offenders.append(str(n) + " : " + str(m['GroupId']))
+    #     return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
+    #             'Description': description, 'ControlId': control}
+    #
+    # # 4.6 ensure security group dont have large range of ports open
+    # def control_4_6_ensure_sg_dont_have_large_range_of_ports_open(self, regions: list) -> dict:
+    #     logger.info(" ---Inside networking_control_4 :: control_4_6_ensure_sg_dont_have_large_range_of_ports_open")
+    #     self.refresh_session()
+    #
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: dict
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = "4.6"
+    #     description = "Ensure security groups don't have large range of ports open"
+    #     scored = True
+    #
+    #     for region in regions:
+    #         client = self.session.client('ec2', region_name=region)
+    #         marker = ''
+    #         while True:
+    #             if marker == '' or marker is None:
+    #                 response = client.describe_security_groups()
+    #             else:
+    #                 response = client.describe_security_groups(
+    #                     NextToken=marker
+    #                 )
+    #             for sg in response['SecurityGroups']:
+    #                 for port_range in sg['IpPermissions']:
+    #                     try:
+    #                         count = port_range['ToPort'] - port_range['FromPort']
+    #                         if count > 1:
+    #                             result = "Not Compliant"
+    #                             failReason = "Found Security group with range of port open"
+    #                             offenders.append(sg['GroupName'])
+    #                             continue
+    #                     except KeyError:
+    #                         continue
+    #
+    #             try:
+    #                 marker = response['NextToken']
+    #                 if marker == '':
+    #                     break
+    #             except:
+    #                 break
+    #
+    #     return {
+    #         'Result': result,
+    #         'failReason': failReason,
+    #         'Offenders': offenders,
+    #         'ScoredControl': scored,
+    #         'Description': description,
+    #         'ControlId': control
+    #     }
+    #
+    # # 4.7 Ensure use of https for cloudfront distributions
+    # def control_4_7_use_https_for_cloudfront_distribution(self) -> dict:
+    #     logger.info(" ---Inside networking_control_4 :: control_4_7_use_https_for_cloudfront_distribution")
+    #     self.refresh_session()
+    #
+    #     """Summary
+    #
+    #     Returns:
+    #         TYPE: dict
+    #     """
+    #     result = "Compliant"
+    #     failReason = ""
+    #     offenders = []
+    #     control = '4.7'
+    #     description = "Use https for cloudfront distributions"
+    #     scored = True
+    #
+    #     client = self.session.client('cloudfront')
+    #     marker = ''
+    #     while True:
+    #         if marker == '' or marker == None:
+    #             response = client.list_distributions()
+    #         else:
+    #             response = client.list_distributions(
+    #                 Marker=marker
+    #             )
+    #         try:
+    #             for item in response['DistributionList']['Items']:
+    #                 protocol_policy = item['DefaultCacheBehavior']['ViewerProtocolPolicy']
+    #                 if protocol_policy == 'allow-all':
+    #                     result = "Not Compliant"
+    #                     failReason = "Found cloudfront distribution which accepts http also"
+    #                     offenders.append(item['Id'])
+    #                     continue
+    #
+    #                 try:
+    #                     for cache_behaviour in item['CacheBehaviors']['Items']:
+    #                         protocol_policy = cache_behaviour['ViewerProtocolPolicy']
+    #                         if protocol_policy == 'allow-all':
+    #                             result = "Not Compliant"
+    #                             failReason = "Found cloudfront distribution which accepts http also"
+    #                             offenders.append(item['Id'])
+    #                             continue
+    #
+    #                 except KeyError:
+    #                     pass
+    #         except KeyError:
+    #             break
+    #         try:
+    #             marker = response['NextMarker']
+    #             if marker == '':
+    #                 break
+    #         except KeyError:
+    #             break
+    #
+    #     return {
+    #         'Result': result,
+    #         'failReason': failReason,
+    #         'Offenders': offenders,
+    #         'ScoredControl': scored,
+    #         'Description': description,
+    #         'ControlId': control
+    #     }
```

### Comparing `cis_checks_2023-2.0.9/cis_checks_2023/storage_control_2.py` & `cis_checks_2023-2.1.0/cis_checks_2023/storage_control_2.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 # --- 2.1 Simple Storage Service (S3) ---
 
 
 class storage_control:
     # 2.1.1 Ensure all S3 buckets employ encryption-at-rest
     def control_2_1_1_s3_default_encryption_at_rest(self, buckets):
         logger.info(" ---Inside storage_control_2 :: control_2_1_1_s3_default_encryption_at_rest()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -69,14 +70,15 @@
             #     continue
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 2.1.2 Ensure S3 Bucket Policy is set to deny HTTP requests
     def control_2_1_2_s3_deny_http_requests(self, buckets):
         logger.info(" ---Inside storage_control_2 :: control_2_1_2_s3_deny_http_requests()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -119,14 +121,15 @@
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 2.1.3 Ensure MFA Delete is enabled on S3 buckets
     def control_2_1_3_s3_mfa_delete_enabled(self, buckets):
         logger.info(" ---Inside storage_control_2 :: control_2_1_3_s3_mfa_delete_enabled()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         failReason = ""
@@ -161,14 +164,15 @@
 
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 2.1.4 Ensure all data in Amazon S3 has been discovered, classified and secured when required
     def control_2_1_4_ensure_all_data_discovered_classified_secured(self):
         logger.info(" ---Inside storage_control_2 :: control_2_1_4_ensure_all_data_discovered_classified_secured()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Manual"
         offenders = []
@@ -179,14 +183,15 @@
         failReason = "Control not implemented using API, please verify manually"
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # 2.1.5 Ensure that S3 Buckets are configured with 'Block public access (bucket settings)'
     def control_2_1_5_s3_blocks_public_access(self, buckets):
         logger.info(" ---Inside storage_control_2 :: control_2_1_5_s3_blocks_public_access()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Compliant"
         offenders = []
@@ -229,14 +234,15 @@
         return {'Result': result, 'failReason': failReason, 'Offenders': offenders, 'ScoredControl': scored,
                 'Description': description, 'ControlId': control}
 
     # --- 2.2 Elastic Compute Cloud (EC2) ---
     # 2.2.1 Ensure that all your Amazon Elastic Block Store (EBS) volumes are encrypted
     def control_2_2_1_ebs_volumes_encrypted(self, regions: list) -> dict:
         logger.info(" ---Inside storage_control_2 :: control_2_2_1_ebs_volumes_encrypted()---")
+        self.refresh_session()
 
         """Summary
         
         Args:
             regions TYPE: list
     
         Returns:
@@ -283,14 +289,15 @@
         }
 
     # --- 2.3 Relational Database Service (RDS) ---
     # 2.3.1 Ensure that encryption is enabled for RDS Instances
 
     def control_2_3_1_rds_encryption_enabled(self, rds_instances: dict) -> dict:
         logger.info(" ---Inside storage_control_2 :: control_2_3_1_rds_encryption_enabled()---")
+        self.refresh_session()
 
         """Summary
         
         Args:
             regions TYPE: list
     
         Returns:
@@ -320,14 +327,15 @@
             'ControlId': control
         }
 
     # 2.3.2 Ensure Auto Minor Version Upgrade feature is Enabled for RDS Instances
 
     def control_2_3_2_rds_auto_minor_version_upgrade_enabled(self, rds_instances: dict) -> dict:
         logger.info(" ---Inside storage_control_2 :: control_2_3_2_rds_auto_minor_version_upgrade_enabled()---")
+        self.refresh_session()
 
         """Summary
         
         Args:
             regions TYPE: list
     
         Returns:
@@ -356,14 +364,15 @@
             'Description': description,
             'ControlId': control
         }
 
     # 2.3.3 Ensure that public access is not given to RDS Instance
     def control_2_3_3_rds_publicly_accessible(self, rds_instances: dict) -> dict:
         logger.info(" ---Inside storage_control_2 :: control_2_3_3_rds_publicly_accessible()")
+        self.refresh_session()
 
         """Summary
         
         Args:
             regions TYPE: list
     
         Returns:
@@ -392,14 +401,15 @@
             'Description': description,
             'ControlId': control
         }
 
     # 2.4.1 Ensure that encryption is enabled for EFS file systems
     def control_2_4_1_encryption_enabled_for_efs(self):
         logger.info(" ---Inside storage_control_2 :: control_2_4_1_encryption_enabled_for_efs()--- ")
+        self.refresh_session()
         """Summary
     
         Returns:
             TYPE: Description
         """
         result = "Manual"
         offenders = []
```

### Comparing `cis_checks_2023-2.0.9/cis_checks_2023/utils.py` & `cis_checks_2023-2.1.0/cis_checks_2023/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 #     IAM_CLIENT = param_IAM_CLIENT
 #     S3_CLIENT = param_S3_CLIENT
 
 
 class utils:
     def get_cred_report(self):
         logger.info(" ---Inside utils :: get_cred_report()--- ")
-        """Summary
+        """
     
         Returns:
             TYPE: Description
         """
         x = 0
         status = ""
         # global self.session.client('iam')
@@ -138,37 +138,37 @@
     
         Returns:
             TYPE: Description
         """
 
         client = self.session.client('ec2', region_name='us-east-1')
         region_response = {}
-        try:
-            region_response = client.describe_regions()
-        except botocore.exceptions.ClientError as error:
-            if error.response['Error']['Code'] == 'AuthFailure':
-                logger.error(f" AccessKey credentails not found here: {error}")
-                return {
-                    'Result': 'Auth Failure',
-                    'failReason': 'Auth Failure',
-                    'Offenders': [],
-                    'ScoredControl': False,
-                    'Description': 'Auth Failure',
-                    'ControlId': 'Auth Failure'
-                }
-        except botocore.exceptions.NoCredentialsError as e:
-            logger.error(f" Unable to locate credentials: {e} ")
-            return {
-                'Result': 'Auth Failure',
-                'failReason': 'Auth Failure',
-                'Offenders': [],
-                'ScoredControl': False,
-                'Description': 'Auth Failure',
-                'ControlId': 'Auth Failure'
-            }
+        # try:
+        region_response = client.describe_regions()
+        # except botocore.exceptions.ClientError as error:
+        #     if error.response['Error']['Code'] == 'AuthFailure':
+        #         logger.error(f" AccessKey credentails not found here: {error}")
+        #         return {
+        #             'Result': 'Auth Failure',
+        #             'failReason': 'Auth Failure',
+        #             'Offenders': [],
+        #             'ScoredControl': False,
+        #             'Description': 'Auth Failure',
+        #             'ControlId': 'Auth Failure'
+        #         }
+        # except botocore.exceptions.NoCredentialsError as e:
+        #     logger.error(f" Unable to locate credentials: {e} ")
+        #     return {
+        #         'Result': 'Auth Failure',
+        #         'failReason': 'Auth Failure',
+        #         'Offenders': [],
+        #         'ScoredControl': False,
+        #         'Description': 'Auth Failure',
+        #         'ControlId': 'Auth Failure'
+        #     }
 
         logger.debug(region_response)
         regions = [region['RegionName'] for region in region_response['Regions']]
         return regions
 
     def get_cloudtrails(self, regions):
         logger.info(" ---Inside utils :: get_cloudtrails()--- ")
```

### Comparing `cis_checks_2023-2.0.9/pyproject.toml` & `cis_checks_2023-2.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "cis_checks_2023"
-version = "2.0.9"
+version = "2.1.0"
 authors = [
   { name="Dheeraj Banodha", email="dheeraj.banodha@impetus.com" },
   { name="Ravish Sharma", email="ravish.sharma@impetus.com"}
 ]
 description = "Provides AWS compliance details"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "boto3",
+    "pytz"
+]
 
 #[project.urls]
 #"Homepage" = ""
 #"Bug Tracker" = ""
```

