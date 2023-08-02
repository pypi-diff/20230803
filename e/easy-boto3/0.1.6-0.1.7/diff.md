# Comparing `tmp/easy_boto3-0.1.6.tar.gz` & `tmp/easy_boto3-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_boto3-0.1.6.tar", max compression
+gzip compressed data, was "easy_boto3-0.1.7.tar", max compression
```

## Comparing `easy_boto3-0.1.6.tar` & `easy_boto3-0.1.7.tar`

### file list

```diff
@@ -1,33 +1,38 @@
--rw-r--r--   0        0        0    11357 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/LICENSE
--rw-r--r--   0        0        0     8710 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/README.md
--rw-r--r--   0        0        0     1030 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/cloudwatch/__init__.py
--rw-r--r--   0        0        0     1398 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/cloudwatch/create.py
--rw-r--r--   0        0        0     1463 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/cloudwatch/delete.py
--rw-r--r--   0        0        0      878 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/cloudwatch/list.py
--rw-r--r--   0        0        0     1015 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/__init__.py
--rw-r--r--   0        0        0     3439 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/config_parser.py
--rw-r--r--   0        0        0     3554 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/connect.py
--rw-r--r--   0        0        0     1724 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/create.py
--rw-r--r--   0        0        0     2586 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/ec2_connections_management.py
--rw-r--r--   0        0        0     1494 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/ec2_instance_management.py
--rw-r--r--   0        0        0     1741 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/list.py
--rw-r--r--   0        0        0     1487 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/logs.py
--rw-r--r--   0        0        0     3657 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/script.py
--rw-r--r--   0        0        0     2967 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/ssh.py
--rw-r--r--   0        0        0      781 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/start.py
--rw-r--r--   0        0        0      827 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/stop.py
--rw-r--r--   0        0        0        0 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/stop_all.py
--rw-r--r--   0        0        0      998 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/terminate.py
--rw-r--r--   0        0        0    13246 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/main.py
--rw-r--r--   0        0        0        0 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/profile/__init__.py
--rw-r--r--   0        0        0     1141 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/profile/active.py
--rw-r--r--   0        0        0     3948 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/profile/ownership.py
--rw-r--r--   0        0        0     1477 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/profile/validation.py
--rw-r--r--   0        0        0      877 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/setup_session.py
--rw-r--r--   0        0        0        0 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/utilities/__init__.py
--rw-r--r--   0        0        0     1806 2023-07-24 20:46:58.815361 easy_boto3-0.1.6/easy_boto3/utilities/aws_profile_parser.py
--rw-r--r--   0        0        0     2471 2023-07-24 20:46:58.815361 easy_boto3-0.1.6/easy_boto3/utilities/decorators.py
--rw-r--r--   0        0        0     1270 2023-07-24 20:46:58.815361 easy_boto3-0.1.6/easy_boto3/utilities/logger_maker.py
--rw-r--r--   0        0        0     1013 2023-07-24 20:46:58.815361 easy_boto3-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     9861 1970-01-01 00:00:00.000000 easy_boto3-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/LICENSE
+-rw-r--r--   0        0        0     8710 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/README.md
+-rw-r--r--   0        0        0     1812 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/cloudwatch/__init__.py
+-rw-r--r--   0        0        0      789 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/cloudwatch/cloudwatch.py
+-rw-r--r--   0        0        0     1472 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/cloudwatch/create.py
+-rw-r--r--   0        0        0     1463 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/cloudwatch/delete.py
+-rw-r--r--   0        0        0      878 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/cloudwatch/list.py
+-rw-r--r--   0        0        0     6946 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/compound.py
+-rw-r--r--   0        0        0     1015 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/__init__.py
+-rw-r--r--   0        0        0     3690 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/config_parser.py
+-rw-r--r--   0        0        0     3615 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/connect.py
+-rw-r--r--   0        0        0     1707 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/create.py
+-rw-r--r--   0        0        0     2687 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/ec2.py
+-rw-r--r--   0        0        0     2623 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/ec2_connections_management.py
+-rw-r--r--   0        0        0      401 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/ec2_instance_management.py
+-rw-r--r--   0        0        0     1911 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/list.py
+-rw-r--r--   0        0        0     1477 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/logs.py
+-rw-r--r--   0        0        0     2089 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/script.py
+-rw-r--r--   0        0        0     2963 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/ssh.py
+-rw-r--r--   0        0        0      832 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/start.py
+-rw-r--r--   0        0        0      826 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/stop.py
+-rw-r--r--   0        0        0        0 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/stop_all.py
+-rw-r--r--   0        0        0      998 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/ec2/terminate.py
+-rw-r--r--   0        0        0      672 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/main.py
+-rw-r--r--   0        0        0        0 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/profile/__init__.py
+-rw-r--r--   0        0        0     1296 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/profile/active.py
+-rw-r--r--   0        0        0     3949 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/profile/ownership.py
+-rw-r--r--   0        0        0     1309 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/profile/profile.py
+-rw-r--r--   0        0        0     1477 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/profile/validation.py
+-rw-r--r--   0        0        0     2830 2023-08-02 22:18:31.931592 easy_boto3-0.1.7/easy_boto3/router.py
+-rw-r--r--   0        0        0      865 2023-08-02 22:18:31.935593 easy_boto3-0.1.7/easy_boto3/setup_session.py
+-rw-r--r--   0        0        0        0 2023-08-02 22:18:31.935593 easy_boto3-0.1.7/easy_boto3/utilities/__init__.py
+-rw-r--r--   0        0        0     1884 2023-08-02 22:18:31.935593 easy_boto3-0.1.7/easy_boto3/utilities/aws_profile_parser.py
+-rw-r--r--   0        0        0     2471 2023-08-02 22:18:31.935593 easy_boto3-0.1.7/easy_boto3/utilities/decorators.py
+-rw-r--r--   0        0        0     1259 2023-08-02 22:18:31.935593 easy_boto3-0.1.7/easy_boto3/utilities/logger_maker.py
+-rw-r--r--   0        0        0     1045 2023-08-02 22:18:31.935593 easy_boto3-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     9861 1970-01-01 00:00:00.000000 easy_boto3-0.1.7/PKG-INFO
```

### Comparing `easy_boto3-0.1.6/LICENSE` & `easy_boto3-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.6/README.md` & `easy_boto3-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.6/easy_boto3/cloudwatch/create.py` & `easy_boto3-0.1.7/easy_boto3/cloudwatch/create.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,8 +37,11 @@
             Namespace=Namespace,
             Period=Period,
             Statistic=Statistic,
             Threshold=Threshold,
             Dimensions=Dimensions
         )
 
+    if result['ResponseMetadata']['HTTPStatusCode'] == 200:
+        pass
+
     return {'AlarmName': AlarmName}
```

### Comparing `easy_boto3-0.1.6/easy_boto3/cloudwatch/delete.py` & `easy_boto3-0.1.7/easy_boto3/cloudwatch/delete.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from easy_boto3.setup_session import setup
-session_auth = setup()
 from easy_boto3.cloudwatch.list import list_instance_alarms
+session_auth = setup()
 
 
 @session_auth
 def delete_alarm(AlarmName: str,
                  session=None):
 
     # create cloudwatch controller from session
```

### Comparing `easy_boto3-0.1.6/easy_boto3/cloudwatch/list.py` & `easy_boto3-0.1.7/easy_boto3/cloudwatch/list.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.6/easy_boto3/ec2/__init__.py` & `easy_boto3-0.1.7/easy_boto3/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.6/easy_boto3/ec2/config_parser.py` & `easy_boto3-0.1.7/easy_boto3/ec2/config_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import yaml
 from easy_boto3.ec2.script import read_startup_script, inject_aws_creds, add_ssh_forwarding, add_github_host
 from easy_boto3.profile.validation import check_credentials
+from easy_boto3.profile.active import set_active_profile, check_active_profile
 
 
 def parse(base_config):
     # read in base_config
     with open(base_config, 'r') as stream:
         try:
             base_config = yaml.safe_load(stream)
@@ -16,18 +17,23 @@
     ec2_instance_config = base_config['ec2_instance']
     instance_details = ec2_instance_config['instance_details']
     ssh_instance_details = ec2_instance_config['ssh_details']
     script_details = ec2_instance_config['script_details']
     alarm_details = None
     alarm_instance_details = None
 
+    # check if profile_name is current active_profile
+    if check_active_profile() != profile_name:
+        # set active profile
+        set_active_profile(profile_name)
+
     # re-convert ssh_instance_details IdentityFile to yes/no
-    if ssh_instance_details['Config']['ForwardAgent'] == True:
+    if ssh_instance_details['Config']['ForwardAgent'] is True:
         ssh_instance_details['Config']['ForwardAgent'] = 'yes'
-    elif ssh_instance_details['Config']['ForwardAgent'] == False:
+    elif ssh_instance_details['Config']['ForwardAgent'] is False:
         ssh_instance_details['Config']['ForwardAgent'] = 'no'
 
     # setup alarm_details if present in base_config
     if 'alarm_details' in list(base_config.keys()):
         alarm_details = base_config['alarm_details']
         alarm_instance_details = {}
```

### Comparing `easy_boto3-0.1.6/easy_boto3/ec2/connect.py` & `easy_boto3-0.1.7/easy_boto3/ec2/connect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-from easy_boto3.profile.ownership import lookup_public_ip
-from easy_boto3.setup_session import setup
-session_auth = setup()
 import paramiko
 import time
 import os
 import logging
+from easy_boto3.profile.ownership import lookup_public_ip
+from easy_boto3.setup_session import setup
+session_auth = setup()
 logging.getLogger("paramiko").setLevel(logging.CRITICAL)
 
 
 @session_auth
-def get_public_ip(instance_id, session=None):
+def get_public_ip(instance_id,
+                  session=None):
     # create ec2 controller from session
     ec2_controller = session.client('ec2')
 
     # collect response from aws based on instance_id
     response = ec2_controller.describe_instances(InstanceIds=[instance_id])
 
     # cut out instance data
     instance_data = response['Reservations'][0]['Instances'][0]
 
     # if PublicIpAddress is present as key, return its value
     if 'PublicIpAddress' in instance_data.keys():
-        return instance_data['PublicIpAddress']         
+        return instance_data['PublicIpAddress']
     else:
         # try loading public ip from instance_id_profile_pairs_path via instance_id
         public_ip = lookup_public_ip(instance_id)
         if public_ip is not None:
             return public_ip
     return None
 
 
 @session_auth
 def add_instance_to_known_hosts(instance_ip,
                                 username,
                                 key_name):
     # connect to instance
     username = 'ubuntu'
-    key_path = '/Users/wattjer/.ssh/shiftsmart_transcript_west_2.pem' 
+    key_path = '/Users/wattjer/.ssh/shiftsmart_transcript_west_2.pem'
     ec2_public_ip = instance_ip
 
     # Create an SSH client
     ssh_client = paramiko.SSHClient()
     ssh_client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
 
     # Connect to the EC2 instance
@@ -54,25 +55,25 @@
         try:
             ssh_transport = paramiko.transport.Transport('%s:%s' % (instance_ip, 22))
             inner_options = ssh_transport.get_security_options()
             inner_options.key_types = (key_type,)
 
             ssh_transport.start_client()
             key = ssh_transport.get_remote_server_key()
-            ssh_transport.close()   
+            ssh_transport.close()
 
             name = key.get_name()
             if name not in all_names:
                 all_names.add(name)
                 all_keys.append(key)
-        except:
+        except Exception as e:
+            print(e)
             pass
 
-
-    # Add the remote server's public keys to the local known_hosts file    
+    # Add the remote server's public keys to the local known_hosts file
     home_dir = os.path.expanduser("~")
     known_hosts_path = os.path.join(home_dir, '.ssh', 'known_hosts')
 
     with open(known_hosts_path, 'a') as known_hosts_file:
         for key in all_keys:
             message = f'{instance_ip} {key.get_name()} {key.get_base64()}\n'
             known_hosts_file.write(message)
@@ -99,15 +100,16 @@
 def test_connection(instance_ip):
     max_count = 10
     while True:
         try:
             add_instance_to_known_hosts(instance_ip)
             print('addition to known hosts successful')
             break
-        except:
+        except Exception as e:
+            print(e)
             time.sleep(10)
             print('trying again')
-            
+
         max_count -= 1
         if max_count == 0:
             print('max count reached')
-            break
+            break
```

### Comparing `easy_boto3-0.1.6/easy_boto3/ec2/create.py` & `easy_boto3-0.1.7/easy_boto3/ec2/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from easy_boto3.setup_session import setup
+from easy_boto3.ec2.connect import get_public_ip
 session_auth = setup()
-from easy_boto3.ec2.connect import get_public_ip, test_connection
 
 
 @session_auth
 def create_instance(KeyName: str,
                     InstanceName='example_worker',
                     InstanceType='t2.micro',
                     ImageId='ami-03f65b8614a860c29',
```

### Comparing `easy_boto3-0.1.6/easy_boto3/ec2/ec2_connections_management.py` & `easy_boto3-0.1.7/easy_boto3/ec2/ec2_connections_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import os, time
-from easy_boto3 import session_auth
+import os
+import time
 import paramiko
 import logging
 logging.getLogger("paramiko").setLevel(logging.CRITICAL)
 
 
 def add_instance_to_known_hosts(instance_ip):
     # connect to instance
@@ -32,18 +32,19 @@
             key = ssh_transport.get_remote_server_key()
             ssh_transport.close()
 
             name = key.get_name()
             if name not in all_names:
                 all_names.add(name)
                 all_keys.append(key)
-        except:
+        except Exception as e:
+            print(e)
             pass
 
-    # Add the remote server's public keys to the local known_hosts file    
+    # Add the remote server's public keys to the local known_hosts file
     home_dir = os.path.expanduser("~")
     known_hosts_path = os.path.join(home_dir, '.ssh', 'known_hosts')
 
     with open(known_hosts_path, 'a') as known_hosts_file:
         for key in all_keys:
             message = f'{instance_ip} {key.get_name()} {key.get_base64()}\n'
             known_hosts_file.write(message)
@@ -62,23 +63,24 @@
     ssh_client = paramiko.SSHClient()
     ssh_client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
 
     # Connect to the EC2 instance
     ssh_client.connect(instance_ip, username=username, key_filename=key_path)
 
 
-# try test_connect every 10 seconds 
+# try test_connect every 10 seconds
 def test_connection(instance_ip):
     max_count = 10
     while True:
         try:
             add_instance_to_known_hosts(instance_ip)
             print('addition to known hosts successful')
             break
-        except:
+        except Exception as e:
+            print(e)
             time.sleep(10)
             print('trying again')
 
         max_count -= 1
         if max_count == 0:
             print('max count reached')
             break
```

### Comparing `easy_boto3-0.1.6/easy_boto3/ec2/list.py` & `easy_boto3-0.1.7/easy_boto3/ec2/list.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,46 +16,54 @@
     for reservation in instances:
         for instance in reservation['Instances']:
             # get instance data
             instance_id = instance['InstanceId']
             instance_state = instance['State']['Name']
             instance_type = instance['InstanceType']
 
-            # package instance data in small dictionary 
+            # package instance data in small dictionary
             instance_data = {'instance_id': instance_id,
-                            'instance_state': instance_state,
-                            'instance_type': instance_type}
+                             'instance_state': instance_state,
+                             'instance_type': instance_type}
 
             # store instance information
             all_instances.append(instance_data)
-
-    return all_instances
+    if all_instances:
+        return all_instances
+    else:
+        return []
 
 
 @session_auth
 def list_stopped(session=None):
     # get list of all instances
     all_instances = list_all()
 
     # collect stopped instances
     stopped_instances = []
     for instance in all_instances:
         # get instance data
         if instance['instance_state'] == 'stopped':
             stopped_instances.append(instance)
 
-    return stopped_instances
+    if stopped_instances:
+        return stopped_instances
+    else:
+        return []
 
 
 @session_auth
 def list_running(session=None):
     # get list of all instances
     all_instances = list_all()
 
     # collect running instances
     running_instances = []
     for instance in all_instances:
         # get instance data
         if instance['instance_state'] == 'running':
             running_instances.append(instance)
 
-    return running_instances
+    if running_instances:
+        return running_instances
+    else:
+        return []
```

### Comparing `easy_boto3-0.1.6/easy_boto3/ec2/logs.py` & `easy_boto3-0.1.7/easy_boto3/ec2/logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import paramiko
 import logging
 from easy_boto3.setup_session import setup
 session_auth = setup()
 logging.getLogger("paramiko").setLevel(logging.CRITICAL)
```

### Comparing `easy_boto3-0.1.6/easy_boto3/ec2/ssh.py` & `easy_boto3-0.1.7/easy_boto3/ec2/ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     config.save()
 
 
 @session_auth
 def lookup_host_data_by_hostname(instance_ip,
                                  session=None):
 
-    # get ssh config 
+    # get ssh config
     config = create_config_object()
 
     # loop over hosts, find host with matching host_name = instance_ip
     for host in config.hosts():
         # lookup host_data config
         host_data = config.host(host)
 
@@ -82,15 +82,15 @@
 @session_auth
 def change_host_name_by_host(host,
                              public_ip,
                              session=None):
     # get ssh config
     config = create_config_object()
 
-    # reset hostname   
+    # reset hostname
     config.set(host, Hostname=public_ip)
 
     # save config
     config.save()
 
 
 @session_auth
```

### Comparing `easy_boto3-0.1.6/easy_boto3/ec2/start.py` & `easy_boto3-0.1.7/easy_boto3/ec2/start.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     # Check if instance exists
     response = ec2_controller.describe_instances(InstanceIds=[instance_id])
 
     # start instance if it exists
     if len(response["Reservations"]) > 0:
         # Start instance
         instances = ec2_controller.start_instances(InstanceIds=[instance_id])
+        if instances is not None:
+            pass
 
         # wait for the instance to be running
         waiter = ec2_controller.get_waiter('instance_running')
         waiter.wait(InstanceIds=[instance_id])
     else:
         message = f"Instance {instance_id} does not exist"
         print(message)
```

### Comparing `easy_boto3-0.1.6/easy_boto3/ec2/stop.py` & `easy_boto3-0.1.7/easy_boto3/ec2/stop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from easy_boto3.setup_session import setup
 session_auth = setup()
 
 
 @session_auth
-def stop_instance(instance_id: str, 
+def stop_instance(instance_id: str,
                   session=None) -> str:
     # create ec2 controller from session
     ec2_controller = session.client('ec2')
 
     # check if instance is running
     response = ec2_controller.describe_instances(InstanceIds=[instance_id])
     if response['Reservations'][0]['Instances'][0]['State']['Name'] == 'running':
```

### Comparing `easy_boto3-0.1.6/easy_boto3/ec2/terminate.py` & `easy_boto3-0.1.7/easy_boto3/ec2/terminate.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from easy_boto3.cloudwatch.delete import delete_instance_alarm
 from easy_boto3.setup_session import setup
 session_auth = setup()
-from easy_boto3.cloudwatch.delete import delete_instance_alarm
 
 
 @session_auth
 def terminate_instance(instance_id: str,
                        session=None) -> str:
     # create ec2 controller from session
     ec2_controller = session.client('ec2')
```

### Comparing `easy_boto3-0.1.6/easy_boto3/profile/ownership.py` & `easy_boto3-0.1.7/easy_boto3/profile/ownership.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 
     # save if new_data is not None
     if new_data is not None:
         save_json_file(new_data)
 
     return None
 
+
 def list() -> list:
     # read in profile data
     data = read_json_file()
 
     # print all profile list
     if len(data) == 0:
         print('No profile / instsance ids')
```

### Comparing `easy_boto3-0.1.6/easy_boto3/profile/validation.py` & `easy_boto3-0.1.7/easy_boto3/profile/validation.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.6/easy_boto3/setup_session.py` & `easy_boto3-0.1.7/easy_boto3/setup_session.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from easy_boto3.utilities.decorators import SessionAuthenticator
 from easy_boto3.utilities.aws_profile_parser import get_aws_login_data
 from easy_boto3 import active_profile_path
-import yaml
 import json
 
 
 # create session authenticator based on aws credentials
 def setup() -> SessionAuthenticator:
     # read in json file at active_profile_path
     with open(active_profile_path, 'r') as f:
```

### Comparing `easy_boto3-0.1.6/easy_boto3/utilities/aws_profile_parser.py` & `easy_boto3-0.1.7/easy_boto3/utilities/aws_profile_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 from easy_boto3 import aws_config_directory
 
 
 def get_aws_config_data(aws_config_path: str,
                         selected_profile_name: str) -> dict:
     # read in aws config
     aws_config = configparser.ConfigParser()
-    aws_config.read(aws_config_path);
+
+    # read in config file but quiet output
+    f = aws_config.read(aws_config_path)  # noqa: F841
 
     # select data associated with selected profile
     aws_profile_region = aws_config[selected_profile_name]['region']
     aws_profile_output = aws_config[selected_profile_name]['output']
 
     return {'aws_profile_region': aws_profile_region,
             'aws_profile_output': aws_profile_output}
 
 
 def get_aws_creds_data(aws_creds_path: str,
                        selected_profile_name: str) -> dict:
     # read in credentials config
     aws_creds = configparser.ConfigParser()
-    aws_creds.read(aws_creds_path);
+    f = aws_creds.read(aws_creds_path)  # noqa: F841
 
     # select data associated with selected profile
     aws_access_key_id = aws_creds[selected_profile_name]['aws_access_key_id']
     aws_secret_access_key = aws_creds[selected_profile_name]['aws_secret_access_key']
 
     return {'aws_access_key_id': aws_access_key_id,
             'aws_secret_access_key': aws_secret_access_key}
```

### Comparing `easy_boto3-0.1.6/easy_boto3/utilities/decorators.py` & `easy_boto3-0.1.7/easy_boto3/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.6/easy_boto3/utilities/logger_maker.py` & `easy_boto3-0.1.7/easy_boto3/utilities/logger_maker.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         pass
 
     def __call__(self, func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             func_name = func.__name__
             try:
-                result = func(*args, **kwargs)           
+                result = func(*args, **kwargs)
             except Exception as e:
                 # with open(self.file_path, 'a') as file:
                 #     file.write(f"FAILURE: {func_name} failed: {e}\n")
                 #     traceback.print_exc(file=file)
                 print(f"FAILURE: {func_name} failed: {e}")
             else:
                 # with open(self.file_path, 'a') as file:
```

### Comparing `easy_boto3-0.1.6/pyproject.toml` & `easy_boto3-0.1.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [tool.poetry]
 name = "easy_boto3"
-version = "0.1.6"
+version = "0.1.7"
 description = "`easy_boto3` simplifies `boto3` usage by adding a command line interface (CLI) and abridged Python API that allows you to easily create, manage, and tear-down AWS resources using `boto3` and `awscli` in a simple, easy to use, and easy to refactor `.yaml` configuration file."
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jermwatt/easy_boto3"
 packages = [{include = "easy_boto3"}]
-include = ["easy_boto3/.easy_boto3_internal.yaml"]
 
 
 [tool.poetry.scripts]
 easy_boto3 = "easy_boto3.main:main"
 
 
 [tool.poetry.dependencies]
@@ -23,14 +22,18 @@
 pyyaml = "^6.0"
 fire = "^0.5.0"
 tomli = "^2.0.1"
 botocore = "^1.31.1"
 yaspin = "^2.3.0"
 sshconf = "^0.2.5"
 
+[tool.poetry.dev-dependencies]
+pytest = "^6.2.5"
+flake8 = "^4.0.1"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.23.1"
+mypy = "^1.4.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `easy_boto3-0.1.6/PKG-INFO` & `easy_boto3-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-boto3
-Version: 0.1.6
+Version: 0.1.7
 Summary: `easy_boto3` simplifies `boto3` usage by adding a command line interface (CLI) and abridged Python API that allows you to easily create, manage, and tear-down AWS resources using `boto3` and `awscli` in a simple, easy to use, and easy to refactor `.yaml` configuration file.
 Home-page: https://github.com/jermwatt/easy_boto3
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

