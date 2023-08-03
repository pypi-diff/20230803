# Comparing `tmp/aws_cost_optimization-0.3.1.tar.gz` & `tmp/aws_cost_optimization-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_cost_optimization-0.3.1.tar", last modified: Fri May  5 08:29:10 2023, max compression
+gzip compressed data, was "aws_cost_optimization-0.4.5.tar", last modified: Thu Aug  3 11:42:10 2023, max compression
```

## Comparing `aws_cost_optimization-0.3.1.tar` & `aws_cost_optimization-0.4.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:29:10.729882 aws_cost_optimization-0.3.1/
--rw-rw-rw-   0        0        0        0 2023-03-24 12:23:56.000000 aws_cost_optimization-0.3.1/LICENCE
--rw-rw-rw-   0        0        0      506 2023-05-05 08:29:10.727896 aws_cost_optimization-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      141 2023-03-24 12:23:56.000000 aws_cost_optimization-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 08:29:10.701879 aws_cost_optimization-0.3.1/aws_cost_optimization/
--rw-rw-rw-   0        0        0     4673 2023-05-05 08:28:27.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/__init__.py
--rw-rw-rw-   0        0        0     1440 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/_cloudwatch_costing.py
--rw-rw-rw-   0        0        0    11791 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/_ec2_costing.py
--rw-rw-rw-   0        0        0     2399 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/_elb_costing.py
--rw-rw-rw-   0        0        0     1240 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/_kms_costing.py
--rw-rw-rw-   0        0        0     6814 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/_rds_costing.py
--rw-rw-rw-   0        0        0     5023 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/_ri_recommendations.py
--rw-rw-rw-   0        0        0     5102 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/_savings_plan.py
--rw-rw-rw-   0        0        0     5718 2023-04-04 10:14:19.000000 aws_cost_optimization-0.3.1/aws_cost_optimization/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:29:10.722880 aws_cost_optimization-0.3.1/aws_cost_optimization.egg-info/
--rw-rw-rw-   0        0        0      506 2023-05-05 08:29:10.000000 aws_cost_optimization-0.3.1/aws_cost_optimization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      602 2023-05-05 08:29:10.000000 aws_cost_optimization-0.3.1/aws_cost_optimization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:29:10.000000 aws_cost_optimization-0.3.1/aws_cost_optimization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-05 08:29:10.000000 aws_cost_optimization-0.3.1/aws_cost_optimization.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-05 08:29:10.000000 aws_cost_optimization-0.3.1/aws_cost_optimization.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      536 2023-05-05 08:28:27.000000 aws_cost_optimization-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 08:29:10.730884 aws_cost_optimization-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 11:42:10.007847 aws_cost_optimization-0.4.5/
+-rw-rw-rw-   0        0        0        0 2023-03-24 12:23:56.000000 aws_cost_optimization-0.4.5/LICENCE
+-rw-rw-rw-   0        0        0      437 2023-08-03 11:42:09.996895 aws_cost_optimization-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0       74 2023-08-03 10:42:09.000000 aws_cost_optimization-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 11:42:09.955186 aws_cost_optimization-0.4.5/aws_cost_optimization/
+-rw-rw-rw-   0        0        0     7271 2023-08-03 11:41:43.000000 aws_cost_optimization-0.4.5/aws_cost_optimization/__init__.py
+-rw-rw-rw-   0        0        0     1464 2023-08-03 11:18:01.000000 aws_cost_optimization-0.4.5/aws_cost_optimization/_cloudwatch_costing.py
+-rw-rw-rw-   0        0        0    11927 2023-08-03 11:18:01.000000 aws_cost_optimization-0.4.5/aws_cost_optimization/_ec2_costing.py
+-rw-rw-rw-   0        0        0     2425 2023-08-03 11:41:43.000000 aws_cost_optimization-0.4.5/aws_cost_optimization/_elb_costing.py
+-rw-rw-rw-   0        0        0     1264 2023-08-03 11:18:01.000000 aws_cost_optimization-0.4.5/aws_cost_optimization/_kms_costing.py
+-rw-rw-rw-   0        0        0     6858 2023-08-03 11:41:43.000000 aws_cost_optimization-0.4.5/aws_cost_optimization/_rds_costing.py
+-rw-rw-rw-   0        0        0     5032 2023-08-03 11:18:01.000000 aws_cost_optimization-0.4.5/aws_cost_optimization/_ri_recommendations.py
+-rw-rw-rw-   0        0        0     5113 2023-08-03 11:18:01.000000 aws_cost_optimization-0.4.5/aws_cost_optimization/_savings_plan.py
+-rw-rw-rw-   0        0        0     5928 2023-08-03 11:18:01.000000 aws_cost_optimization-0.4.5/aws_cost_optimization/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:42:09.994406 aws_cost_optimization-0.4.5/aws_cost_optimization.egg-info/
+-rw-rw-rw-   0        0        0      437 2023-08-03 11:42:09.000000 aws_cost_optimization-0.4.5/aws_cost_optimization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      602 2023-08-03 11:42:09.000000 aws_cost_optimization-0.4.5/aws_cost_optimization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 11:42:09.000000 aws_cost_optimization-0.4.5/aws_cost_optimization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-03 11:42:09.000000 aws_cost_optimization-0.4.5/aws_cost_optimization.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-08-03 11:42:09.000000 aws_cost_optimization-0.4.5/aws_cost_optimization.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      549 2023-08-03 11:41:43.000000 aws_cost_optimization-0.4.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 11:42:10.020966 aws_cost_optimization-0.4.5/setup.cfg
```

### Comparing `aws_cost_optimization-0.3.1/aws_cost_optimization/_cloudwatch_costing.py` & `aws_cost_optimization-0.4.5/aws_cost_optimization/_cloudwatch_costing.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 
 class cw:
     def logs_costing(self, data) -> dict:
         """
         :return: cost details for logs costing
         """
         logger.info(" ---Inside _cloudwatch_costing :: cw :: logs_costing--- ")
+        self.refresh_session()
 
         region = data['Metadata']['Region']
 
         resolved_region = self.aws_region_map[region]
 
         filters = [
             {'Type': 'TERM_MATCH', 'Field': 'productFamily', 'Value': 'Storage Snapshot'},
             {'Type': 'TERM_MATCH', 'Field': 'location', 'Value': resolved_region}
         ]
-        price = get_pricing(self.session, region, 'AmazonCloudWatch', Filters=filters, service_name='cwlog')
+        price = get_pricing(self, region, 'AmazonCloudWatch', Filters=filters, service_name='cwlog')
 
         stored_bytes = data['Metadata']['storedBytes']
 
         stored_gb = int(stored_bytes)/(1024**3)
 
         # cost_gb = stored_gb - 5
         cost_gb = stored_gb
```

### Comparing `aws_cost_optimization-0.3.1/aws_cost_optimization/_ec2_costing.py` & `aws_cost_optimization-0.4.5/aws_cost_optimization/_ec2_costing.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     # returns the costing details of delete idle compute instance
     def remove_ec2_costing(self, data: dict) -> dict:
         """
         :param data:
         :return:
         """
         logger.info(" --- Inside aws_client :: remove_ec2_costing()--- ")
+        self.refresh_session()
 
         region = data['Metadata']['Region']
 
         client = self.session.client('ec2', region)
         response = client.describe_instances(
             InstanceIds=[data['Id']]
         )
@@ -64,33 +65,34 @@
         ]
         if data['Metadata']['Platform'] is not None:
             filters.append({
                 'Type': 'TERM_MATCH',
                 'Field': 'operatingSystem',
                 'Value': data['Metadata']['Platform']
             })
-        price = get_pricing(self.session, data['Metadata']['Region'], 'AmazonEC2', filters, service_name='ec2_instance')
+        price = get_pricing(self, data['Metadata']['Region'], 'AmazonEC2', filters, service_name='ec2_instance')
 
         print(price)
 
     def gp2_to_gp3(self, data: dict) -> dict:
         """
         :param data: recommendations data
         :return: cost saving recommendations
         """
         logger.info(" ---Inside aws_client :: gp2_to_gp3()--- ")
+        self.refresh_session()
 
         region = data['Metadata']['Region']
         resolved_region = self.aws_region_map[region]
 
         Filters = [
             {'Type': 'TERM_MATCH', 'Field': 'volumeType', 'Value': 'General Purpose'},
             {'Type': 'TERM_MATCH', 'Field': 'location', 'Value': resolved_region}
         ]
-        price = get_pricing(self.session, region, 'AmazonEC2', Filters=Filters, service_name='volume')
+        price = get_pricing(self, region, 'AmazonEC2', Filters=Filters, service_name='volume')
 
         client = self.session.client('ec2', region_name=region)
         response = client.describe_volumes(
             VolumeIds=[
                 data['Id']
             ]
         )
@@ -112,26 +114,27 @@
         return recommendation
 
     def unallocated_eip(self, data) -> dict:
         """
         :return: this list the potential savings
         """
         logger.info(" ---Inside aws_client :: unallocated_eip()--- ")
+        self.refresh_session()
 
         region = data['Metadata']['Region']
 
         resolved_region = self.aws_region_map[region]
 
         filters = [
             {'Type': 'TERM_MATCH', 'Field': 'productFamily', 'Value': 'IP Address'},
             # {'Type': 'TERM_MATCH', 'Field': 'location', 'Value': resolved_region},
             # {'Type': 'TERM_MATCH', 'Field': 'usagetype', 'Value': 'APS3-ElasticIP:IdleAddress'}
             {'Type': 'TERM_MATCH', 'Field': 'usagetype', 'Value': 'ElasticIP:IdleAddress'}
         ]
-        price = get_pricing(self.session, region, 'AmazonEC2', filters, service_name='eip')
+        price = get_pricing(self, region, 'AmazonEC2', filters, service_name='eip')
         current_cost = float(price['ElasticIP:IdleAddress']) * 730
         effective_cost = 0
         recommendation = {
             'Current Cost': current_cost,
             'Effective Cost': effective_cost,
             'Savings': current_cost - effective_cost,
             'Savings %': ((current_cost - effective_cost) / current_cost) * 100,
@@ -143,29 +146,30 @@
     #   Provides cost details for recommendation unused_ebs
     def unused_ebs_costing(self, data: dict) -> dict:
         """
         :param data:
         :return:
         """
         logger.info(" ---Inside _ec2_costing.ec2 :: unused_ebs_costing()--- ")
+        self.refresh_session()
 
         region = data['Metadata']['Region']
 
         if data['Metadata']['Instance Type'].startswith('gp'):
             volume_type = 'General Purpose'
         else:
             volume_type = "Provisioned IOPS"
 
         resolved_region = self.aws_region_map[region]
         filters = [
             {'Type': 'TERM_MATCH', 'Field': 'volumeType', 'Value': volume_type},
             {'Type': 'TERM_MATCH', 'Field': 'location', 'Value': resolved_region}
         ]
 
-        price = get_pricing(self.session, data['Metadata']['Region'], 'AmazonEC2', filters, service_name='volume')
+        price = get_pricing(self, data['Metadata']['Region'], 'AmazonEC2', filters, service_name='volume')
 
         client = self.session.client('ec2', region_name=region)
         response = client.describe_volumes(
             VolumeIds=[
                 data['Id']
             ]
         )
@@ -223,14 +227,15 @@
     #  Provides the cost details for delete older snapshot recommendations
     def older_snapshot_costing(self, data: dict) -> dict:
         """
         :param data: recommendations details
         :return: cost and savings information
         """
         logger.info(" ---Inside _ec2_costing.ec2 :: older_snapshot_costing()--- ")
+        self.refresh_session()
 
         region = data['Metadata']['Region']
         resolved_region = self.aws_region_map[region]
 
         client = self.session.client('ec2', region_name=region)
         response = client.describe_snapshots(
             SnapshotIds=[data['Id']]
@@ -245,15 +250,15 @@
             usage_type = 'EBS:SnapshotUsage'
 
         filters = [
             {'Type': 'TERM_MATCH', 'Field': 'productFamily', 'Value': 'Storage Snapshot'},
             {'Type': 'TERM_MATCH', 'Field': 'usagetype', 'Value': usage_type},
             # {'Type': 'TERM_MATCH', 'Field': 'location', 'Value': resolved_region}
         ]
-        price = get_pricing(self.session, region, 'AmazonEC2', Filters=filters, service_name='snapshot')
+        price = get_pricing(self, region, 'AmazonEC2', Filters=filters, service_name='snapshot')
         print(price)
         size = response['Snapshots'][0]['VolumeSize']
         current_cost = float(price['EBS:SnapshotUsage']) * float(size)
         effective_cost = 0
 
         recommendation = {
             'Current Cost': current_cost,
@@ -268,29 +273,30 @@
     # returns the costing details for upgrading the volume type to GP
     def upgrade_ebs_costing(self, data: dict) -> dict:
         """
         :param data: recommendation details
         :return: cost details for ebs
         """
         logger.info(" ---Inside _ec2_costing :: ec2 :: upgrading_ebs_costing()--- ")
+        self.refresh_session()
 
         region = data['Metadata']['Region']
         resolved_region = self.aws_region_map[region]
 
         filters = lambda v_type: [
             {'Type': 'TERM_MATCH', 'Field': 'volumeType', 'Value': v_type},
             {'Type': 'TERM_MATCH', 'Field': 'location', 'Value': resolved_region}
         ]
 
-        price_provisioned = get_pricing(self.session, region, 'AmazonEC2', filters('Provisioned IOPS'), service_name='volume')
+        price_provisioned = get_pricing(self, region, 'AmazonEC2', filters('Provisioned IOPS'), service_name='volume')
 
         # print(price_provisioned)
         current_cost = float(price_provisioned[data['Metadata']['Instance Type']]) * data['Metadata']['size']
 
-        price_gp3 = get_pricing(self.session, region, 'AmazonEC2', filters('General Purpose'), service_name='volume')
+        price_gp3 = get_pricing(self, region, 'AmazonEC2', filters('General Purpose'), service_name='volume')
 
         # print(price_gp3)
         effective_cost = float(price_gp3['gp3']) * data['Metadata']['size']
         savings = current_cost - effective_cost
         try:
             savings_p = ((current_cost - effective_cost) / current_cost) * 100
         except ZeroDivisionError:
```

### Comparing `aws_cost_optimization-0.3.1/aws_cost_optimization/_elb_costing.py` & `aws_cost_optimization-0.4.5/aws_cost_optimization/_elb_costing.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 class elb:
     def elb_costing(self, data: dict) -> dict:
         """
         :param data:
         :return:
         """
         logger.info(" ---Inside _elb_costing :: elb :: elb_costing()--- ")
+        self.refresh_session()
 
         region = data['Metadata']['Region']
 
         resolved_region = self.aws_region_map[region]
 
         # client = self.session.client('elbv2', region_name=region)
         # response = client.describe_load_balancers(
@@ -50,18 +51,18 @@
             return {
                 'Current Cost': 0,
                 'Effective Cost': 0,
                 'Savings': 0,
                 'Savings %': 0
             }
 
-        price = get_pricing(self.session, region, 'AWSELB', filter_elb_type, service_name='elb')
+        price = get_pricing(self, region, 'AWSELB', filter_elb_type, service_name='elb')
         current_cost = (float(price['Used Application Load Balancer capacity units-hr']) +
                         float(price['LoadBalancer hourly usage by Application Load Balancer'])) * 24 * 30
-        print(price)
+        # print(price)
         effective_cost = 0
         try:
             savings_p = ((current_cost - effective_cost) / current_cost) * 100
         except ZeroDivisionError:
             savings_p = 0
 
         return {
```

### Comparing `aws_cost_optimization-0.3.1/aws_cost_optimization/_kms_costing.py` & `aws_cost_optimization-0.4.5/aws_cost_optimization/_kms_costing.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 class kms:
     def cmk_cost(self, data: dict) -> dict:
         """
         :param data: recommendations data
         :return: cost details for kms cmk
         """
         logger.info(" ---Inside _kms_costing.kms :: cmk_cost")
+        self.refresh_session()
 
         region = data['Metadata']['Region']
         resolved_region = self.aws_region_map[region]
 
         Filters = [
             {'Type': 'TERM_MATCH', 'Field': 'productFamily', 'Value': 'Encryption Key'},
             {'Type': 'TERM_MATCH', 'Field': 'location', 'Value': resolved_region}
         ]
-        price = get_pricing(self.session, region, 'awskms', Filters=Filters, service_name='cmk')
+        price = get_pricing(self, region, 'awskms', Filters=Filters, service_name='cmk')
 
         current_cost = float(price['AWS Key Management Service'])
         effective_cost = 0
 
         return {
             'Current Cost': current_cost,
             'Effective Cost': effective_cost,
```

### Comparing `aws_cost_optimization-0.3.1/aws_cost_optimization/_rds_costing.py` & `aws_cost_optimization-0.4.5/aws_cost_optimization/_rds_costing.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 
 class rds:
     def rds_upgrades(self) -> list:
         """
         :return: list of cost saving recommendations
         """
         logger.info(" ---Inside aws_client :: rds_upgrades()--- ")
+        self.refresh_session()
 
         recommendations = []
 
-        rds_instances = list_rds_instances(self.session, self.regions)
+        rds_instances = list_rds_instances(self, self.regions)
 
         for region, rds_list in rds_instances.items():
             resolved_region = self.aws_region_map[region]
             for instance in rds_list:
                 instance_type = instance['DBInstanceClass']
                 instance_family = instance_type.split('.')[1]
 
@@ -29,25 +30,25 @@
                      'Value': 'Single-AZ' if instance['MultiAZ'] else 'Multi-AZ'},
                     {'Type': 'TERM_MATCH', 'Field': 'productFamily', 'Value': 'Database Instance'},
                     {'Type': 'TERM_MATCH', 'Field': 'location', 'Value': resolved_region}
                 ]
 
                 def evaluate(frm: str, to: str):
                     price_from = get_pricing(
-                        self.session, region, 'AmazonRDS',
+                        self, region, 'AmazonRDS',
                         Filters,
                         service_name='instanceType'
                     )
-                    print(price_from)
+                    # print(price_from)
                     Filters[0]['Value'] = instance_type.replace(frm, to)
                     price_to = get_pricing(
-                        self.session, region, 'AmazonRDS', Filters,
+                        self, region, 'AmazonRDS', Filters,
                         service_name='rds'
                     )
-                    print(price_to)
+                    # print(price_to)
                     current_cost = float(price_from[instance_type]) * 730
                     effective_cost = float(price_to[instance_type.replace(frm, to)]) * 730
 
                     recommendation = {
                         'Region': region,
                         'Instance Id': instance['DBInstanceIdentifier'],
                         'Instance Type': instance_type,
@@ -71,14 +72,15 @@
 
     def delete_rds_costing(self, data: dict) -> dict:
         """
         :param data:
         :return:
         """
         logger.info(" ---Inside aws_client :: rds_costing()--- ")
+        self.refresh_session()
 
         region = data['Metadata']['Region']
 
         resolved_region = self.aws_region_map[region]
         filters = [
             {
                 'Type': 'TERM_MATCH',
@@ -102,15 +104,15 @@
             },
             {
                 'Type': 'TERM_MATCH',
                 'Field': 'deploymentOption',
                 'Value': 'Multi-AZ' if data['Metadata']['MultiAZ'] else 'Single-AZ'
             }
         ]
-        price = get_pricing(self.session, data['Metadata']['Region'], 'AmazonRDS', filters, service_name='rds')
+        price = get_pricing(self, data['Metadata']['Region'], 'AmazonRDS', filters, service_name='rds')
         # print(price)
 
         current_cost = float(price[data['Metadata']['DBInstanceClass']]) * 730
         effective_cost = 0
         recommendation = {
             'Current Cost': current_cost,
             'Effective Cost': effective_cost,
@@ -123,14 +125,15 @@
     # returns the costing details of  rds general purpose ssd
     def rds_gp_ssd(self, data: dict) -> dict:
         """
         :param data:
         :return:
         """
         logger.info(" ---Inside aws_client :: rds_gp_ssd()--- ")
+        self.refresh_session()
 
         region = data['Metadata']['Region']
 
         resolved_region = self.aws_region_map[region]
 
         filters = lambda family, vtype: [
             {
@@ -151,20 +154,20 @@
             {
                 'Type': 'TERM_MATCH',
                 'Field': 'databaseEdition',
                 'Value': 'Standard'
             }
         ]
 
-        price_instance = get_pricing(self.session, region, 'AmazonRDS', filters('Database Storage', 'Provisioned IOPS (SSD)'), service_name='rds_storage')
-        price_iops = get_pricing(self.session, region, 'AmazonRDS', filters('Provisioned IOPS', 'Provisioned IOPS (SSD)'), service_name='rds_storage')
+        price_instance = get_pricing(self, region, 'AmazonRDS', filters('Database Storage', 'Provisioned IOPS (SSD)'), service_name='rds_storage')
+        price_iops = get_pricing(self, region, 'AmazonRDS', filters('Provisioned IOPS', 'Provisioned IOPS (SSD)'), service_name='rds_storage')
         current_cost = float(price_instance['io1']) + float(price_iops['io1'])
         # print(current_cost)
 
-        gp2_price = get_pricing(self.session, region, 'AmazonRDS', filters('Database Storage', 'General Purpose (SSD)'), service_name='rds_storage')
+        gp2_price = get_pricing(self, region, 'AmazonRDS', filters('Database Storage', 'General Purpose (SSD)'), service_name='rds_storage')
 
         # print(gp2_price)
         effective_cost = float(gp2_price['gp2'])
 
         recommendation = {
             'Current Cost': current_cost,
             'Effective Cost': effective_cost,
```

### Comparing `aws_cost_optimization-0.3.1/aws_cost_optimization/_ri_recommendations.py` & `aws_cost_optimization-0.4.5/aws_cost_optimization/_ri_recommendations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 Returns the recommendation for purchasing the Reserved instance
 """
 import logging
 
-import pandas as pd
-
 logger = logging.getLogger()
 
 
 class ri:
     def ri_recommendations(self) -> list:
         """
         :return: list of recommendations for purchasing the savings plan
         """
         logger.info(" ---Inside _ri_recommendations:: ri :: ri_recommendations()--- ")
+        self.refresh_session()
 
         client = self.session.client('ce')
 
         res_recommendations = []
 
         service_map = {
             'Amazon Elastic Compute Cloud - Compute': 'EC2InstanceDetails',
```

### Comparing `aws_cost_optimization-0.3.1/aws_cost_optimization/_savings_plan.py` & `aws_cost_optimization-0.4.5/aws_cost_optimization/_savings_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Provides the recommendations for purchasing the savings plan
 """
 import logging
-import pandas as pd
 
 logger = logging.getLogger()
 
 
 class sp:
     def sp_recommendations(self) -> list:
         """
         :return: list of savings plan recommendations
         """
         logger.info(" ---Inside _savings_plan :: sp :: sp_recommendations()--- ")
+        self.refresh_session()
 
         # response recommendations list
         res_recommendations = []
 
         # creation of aws client for cost explorer
         client = self.session.client('ce')
```

### Comparing `aws_cost_optimization-0.3.1/aws_cost_optimization/utils.py` & `aws_cost_optimization-0.4.5/aws_cost_optimization/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 import json
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def get_regions(session):
+def get_regions(self):
     """
     :session: aws session object
     :return: list of regions
     """
     logger.info(" ---Inside utils :: get_regions()--- ")
-    client = session.client('ec2', region_name='us-east-1')
+    self.refresh_session()
+    client = self.session.client('ec2', region_name='us-east-1')
     region_response = client.describe_regions()
 
     regions = [region['RegionName'] for region in region_response['Regions']]
     return regions
 
 
-def list_volumes(session, regions: list) -> dict:
+def list_volumes(self, regions: list) -> dict:
     """
     :param regions:
     :param session:
     :return:
     """
     logger.info(" ---Inside utils :: list_gp2_volumes()--- ")
+    self.refresh_session()
 
     volume_list = {}
 
     for region in regions:
-        client = session.client('ec2', region_name=region)
+        client = self.session.client('ec2', region_name=region)
         marker = ''
         while True:
             if marker == '':
                 response = client.describe_volumes()
             else:
                 response = client.describe_volumes(
                     NextToken=marker
@@ -47,28 +49,30 @@
             except KeyError:
                 break
 
     return volume_list
 
 
 # returns the pricing of resource
-def get_pricing(session, region: str, service_code: str, Filters: list, service_name: str) -> dict:
+def get_pricing(self, region: str, service_code: str, Filters: list, service_name: str) -> dict:
     """
+    :param self:
     :param service_name:
     :param Filters:
     :param service_code:
     :param region: aws region
     :param session: aws session
     :return: pricing
     """
     logger.info(" ---Inside utils :: get_pricing()--- ")
+    self.refresh_session()
 
     aws_pricing_region = region
 
-    client = session.client('pricing', 'us-east-1')
+    client = self.session.client('pricing', 'us-east-1')
 
     response = client.get_products(
         ServiceCode=service_code,
         Filters=Filters
     )
     print(response)
     prices = {}
@@ -97,25 +101,27 @@
                 elif service_name == 'elb':
                     prices[price['product']['attributes']['groupDescription']] = temp
 
     return prices
 
 
 # returns the list of rds instances
-def list_rds_instances(session, regions: list) -> dict:
+def list_rds_instances(self, regions: list) -> dict:
     """
+    :param self:
     :param regions:
     :param session:
     :return:
     """
     logger.info(" ---Inside utils :: list_rds_instances()--- ")
+    self.refresh_session()
     rds_instance_lst = {}
 
     for region in regions:
-        client = session.client('rds', region_name=region)
+        client = self.session.client('rds', region_name=region)
 
         marker = ''
         while True:
             response = client.describe_db_instances(
                 MaxRecords=100,
                 Marker=marker
             )
@@ -127,26 +133,27 @@
                     break
             except KeyError:
                 break
     return rds_instance_lst
 
 
 # returns the list of ec2 instances
-def list_ec2_instances(session, regions: list) -> dict:
+def list_ec2_instances(self, regions: list) -> dict:
     """
-    :param session:
+    :param self:
     :param regions:
     :return:
     """
     logger.info(" ---Inside utils :: list_ec2_instances()--- ")
+    self.refresh_session()
 
     instances = {}
     print('Instances')
     for region in regions:
-        client = session.client('ec2', region_name=region)
+        client = self.session.client('ec2', region_name=region)
         marker = ''
         while True:
             if marker == '':
                 response = client.describe_instances()
             else:
                 response = client.describe_instances(
                     NextToken=marker
@@ -161,23 +168,24 @@
             except KeyError:
                 break
 
     return instances
 
 
 # returns the list eip
-def list_eip(session, regions: list) -> dict:
+def list_eip(self, regions: list) -> dict:
     """
-    :param session:
+    :param self:
     :param regions:
     :return:
     """
     logger.info(" ---Inside utils :: list_eip()--- ")
+    self.refresh_session()
 
     eip_list = {}
 
     for region in regions:
-        client = session.client('ec2', region_name=region)
+        client = self.session.client('ec2', region_name=region)
         response = client.describe_addresses()
         eip_list.setdefault(region, []).extend(response['Addresses'])
 
     return eip_list
```

### Comparing `aws_cost_optimization-0.3.1/aws_cost_optimization.egg-info/SOURCES.txt` & `aws_cost_optimization-0.4.5/aws_cost_optimization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws_cost_optimization-0.3.1/pyproject.toml` & `aws_cost_optimization-0.4.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aws_cost_optimization"
-version = "0.3.1"
+version = "0.4.5"
 authors = [
   { name="dheeraj.banodha", email="dheeraj.banodha@impetus.com" },
 ]
 description = "Provides AWS cost recommendations"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "boto3"
+    "boto3",
+    "pytz"
 ]
 
 #[project.urls]
 #"Homepage" = ""
 #"Bug Tracker" = ""
```

