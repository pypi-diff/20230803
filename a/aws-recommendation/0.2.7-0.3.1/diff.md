# Comparing `tmp/aws_recommendation-0.2.7.tar.gz` & `tmp/aws_recommendation-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_recommendation-0.2.7.tar", last modified: Fri Jul 21 05:14:41 2023, max compression
+gzip compressed data, was "aws_recommendation-0.3.1.tar", last modified: Thu Aug  3 10:41:05 2023, max compression
```

## Comparing `aws_recommendation-0.2.7.tar` & `aws_recommendation-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 05:14:41.075827 aws_recommendation-0.2.7/
--rw-rw-rw-   0        0        0        0 2022-11-22 10:22:06.000000 aws_recommendation-0.2.7/LICENCE
--rw-rw-rw-   0        0        0     1220 2023-07-21 05:14:41.074826 aws_recommendation-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      868 2023-04-04 11:43:43.000000 aws_recommendation-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 05:14:41.056557 aws_recommendation-0.2.7/aws_recommendation/
--rw-rw-rw-   0        0        0     2329 2023-07-21 05:14:13.000000 aws_recommendation-0.2.7/aws_recommendation/__init__.py
--rw-rw-rw-   0        0        0     5487 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/cloudwatch.py
--rw-rw-rw-   0        0        0    11861 2023-07-13 04:02:57.000000 aws_recommendation-0.2.7/aws_recommendation/cost_estimations.py
--rw-rw-rw-   0        0        0     4296 2023-07-12 09:59:38.000000 aws_recommendation-0.2.7/aws_recommendation/dynamodb.py
--rw-rw-rw-   0        0        0    15213 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/ebs.py
--rw-rw-rw-   0        0        0    26661 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/ec2.py
--rw-rw-rw-   0        0        0     8961 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/elb.py
--rw-rw-rw-   0        0        0     4208 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/kms.py
--rw-rw-rw-   0        0        0    11638 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/rds.py
--rw-rw-rw-   0        0        0     5955 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/redshift.py
--rw-rw-rw-   0        0        0    10955 2023-07-21 05:14:13.000000 aws_recommendation-0.2.7/aws_recommendation/s3.py
--rw-rw-rw-   0        0        0     1726 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/truted_advisor.py
--rw-rw-rw-   0        0        0     5821 2023-04-12 12:09:37.000000 aws_recommendation-0.2.7/aws_recommendation/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 05:14:41.071828 aws_recommendation-0.2.7/aws_recommendation.egg-info/
--rw-rw-rw-   0        0        0     1220 2023-07-21 05:14:40.000000 aws_recommendation-0.2.7/aws_recommendation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      626 2023-07-21 05:14:40.000000 aws_recommendation-0.2.7/aws_recommendation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 05:14:40.000000 aws_recommendation-0.2.7/aws_recommendation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-21 05:14:40.000000 aws_recommendation-0.2.7/aws_recommendation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-21 05:14:40.000000 aws_recommendation-0.2.7/aws_recommendation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      525 2023-07-21 05:14:13.000000 aws_recommendation-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 05:14:41.075827 aws_recommendation-0.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 10:41:05.185224 aws_recommendation-0.3.1/
+-rw-rw-rw-   0        0        0        0 2022-11-22 10:22:06.000000 aws_recommendation-0.3.1/LICENCE
+-rw-rw-rw-   0        0        0     1220 2023-08-03 10:41:05.183934 aws_recommendation-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2023-04-04 11:43:43.000000 aws_recommendation-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 10:41:05.157927 aws_recommendation-0.3.1/aws_recommendation/
+-rw-rw-rw-   0        0        0     4938 2023-08-03 10:40:17.000000 aws_recommendation-0.3.1/aws_recommendation/__init__.py
+-rw-rw-rw-   0        0        0     5519 2023-08-03 08:36:03.000000 aws_recommendation-0.3.1/aws_recommendation/cloudwatch.py
+-rw-rw-rw-   0        0        0    11915 2023-08-03 08:36:03.000000 aws_recommendation-0.3.1/aws_recommendation/cost_estimations.py
+-rw-rw-rw-   0        0        0     4328 2023-08-03 08:36:03.000000 aws_recommendation-0.3.1/aws_recommendation/dynamodb.py
+-rw-rw-rw-   0        0        0    15341 2023-08-03 08:36:03.000000 aws_recommendation-0.3.1/aws_recommendation/ebs.py
+-rw-rw-rw-   0        0        0    26853 2023-08-03 08:36:03.000000 aws_recommendation-0.3.1/aws_recommendation/ec2.py
+-rw-rw-rw-   0        0        0     9025 2023-08-03 08:36:03.000000 aws_recommendation-0.3.1/aws_recommendation/elb.py
+-rw-rw-rw-   0        0        0     4240 2023-08-03 08:36:03.000000 aws_recommendation-0.3.1/aws_recommendation/kms.py
+-rw-rw-rw-   0        0        0    11734 2023-08-03 08:36:03.000000 aws_recommendation-0.3.1/aws_recommendation/rds.py
+-rw-rw-rw-   0        0        0     6019 2023-08-03 08:36:03.000000 aws_recommendation-0.3.1/aws_recommendation/redshift.py
+-rw-rw-rw-   0        0        0    11083 2023-08-03 08:36:03.000000 aws_recommendation-0.3.1/aws_recommendation/s3.py
+-rw-rw-rw-   0        0        0     1758 2023-08-03 08:36:03.000000 aws_recommendation-0.3.1/aws_recommendation/truted_advisor.py
+-rw-rw-rw-   0        0        0     6015 2023-08-03 08:36:03.000000 aws_recommendation-0.3.1/aws_recommendation/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 10:41:05.179149 aws_recommendation-0.3.1/aws_recommendation.egg-info/
+-rw-rw-rw-   0        0        0     1220 2023-08-03 10:41:04.000000 aws_recommendation-0.3.1/aws_recommendation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      626 2023-08-03 10:41:04.000000 aws_recommendation-0.3.1/aws_recommendation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 10:41:04.000000 aws_recommendation-0.3.1/aws_recommendation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-03 10:41:04.000000 aws_recommendation-0.3.1/aws_recommendation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-08-03 10:41:04.000000 aws_recommendation-0.3.1/aws_recommendation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      538 2023-08-03 10:40:17.000000 aws_recommendation-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 10:41:05.185723 aws_recommendation-0.3.1/setup.cfg
```

### Comparing `aws_recommendation-0.2.7/PKG-INFO` & `aws_recommendation-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_recommendation
-Version: 0.2.7
+Version: 0.3.1
 Summary: Provides AWS recommendations
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `aws_recommendation-0.2.7/README.md` & `aws_recommendation-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.7/aws_recommendation/cloudwatch.py` & `aws_recommendation-0.3.1/aws_recommendation/cloudwatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
     #Generate the recommendation for log groups with no retention period
     def __log_group_retention_period_check(self, regions: list) -> list:
         """
         :param self:
         :return:
         """
+        self.refresh_session()
         logger.info(" ---Inside log_group_retention_period_check()")
 
         recommendation = []
 
         for region in regions:
             try:
                 client = self.session.client('logs', region_name=region)
```

### Comparing `aws_recommendation-0.2.7/aws_recommendation/cost_estimations.py` & `aws_recommendation-0.3.1/aws_recommendation/cost_estimations.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     :param os:
     :param region: AWS region
     :param self:
     :param from_instance: source instance
     :param to_instance: destination instance
     :return:
     """
+    self.refresh_session()
     logger.info(" ---Inside cost_estimations :: get_savings()")
 
     client = self.session.client('pricing', region_name='us-east-1')
     price1 = get_price(client=client, region=get_region_name(region), instance=from_instance, os=os)
 
     price2 = get_price(client=client, region=get_region_name(region), instance=to_instance, os=os)
 
@@ -120,15 +121,15 @@
     """
     :param ec2_instances:
     :param regions:
     :param self:
     :return list: details of estimated savings
     """
     logger.info(" ---Inside cost_estimations :: estimated_savings()")
-
+    self.refresh_session()
     possible_upgrade = [
             ('t1.micro', 't2.micro'),
 
             ('m1.large', 't2.large'),
             ('m1.xlarge', 't2.xlarge'),
             ('m1.medium', 't2.medium'),
             ('m1.small', 't2.small'),
```

### Comparing `aws_recommendation-0.2.7/aws_recommendation/dynamodb.py` & `aws_recommendation-0.3.1/aws_recommendation/dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     # generated the recommendations for unused dynamodb tables
     def unused_dynamodb_tables(self, regions) -> list:
         """
         :param regions:
         :param self:
         :return:
         """
+        self.refresh_session()
         logger.info(" ---Inside dynamodb :: unused_dynamodb_tables()")
 
         recommendation = []
 
         for region in regions:
             try:
                 client = self.session.client('dynamodb', region_name=region)
```

### Comparing `aws_recommendation-0.2.7/aws_recommendation/ebs.py` & `aws_recommendation-0.3.1/aws_recommendation/ebs.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     # Generated the recommendation for unused EBS volumes
     def idle_ebs_volumes(self, ebs_volumes) -> list:
         """
         :param ebs_volumes:
         :param self:
         :return:
         """
+        self.refresh_session()
         logger.info(" ---Inside ebs :: idle_ebs_volumes")
 
         recommendation = []
 
         try:
             for region, volumes in ebs_volumes.items():
                 for volume in volumes:
@@ -145,14 +146,15 @@
     # Generated the recommendation for general purpose ssd
     def ebs_general_purpose_ssd(self, ebs_volumes) -> list:
         """
         :param ebs_volumes:
         :param self:
         :return:
         """
+        self.refresh_session()
         logger.info(" ---Inside ebs :: ebs_general_purpose_ssd()")
 
         recommendation = []
 
         try:
             for region, volumes in ebs_volumes.items():
                 for volume in volumes:
@@ -214,14 +216,15 @@
     # Generate the recommendation for upgrade volume from GP2 to gp3 to save cost
     def gp2_to_gp3(self, ebs_volumes) -> list:
         """
         :param ebs_volumes:
         :param self:
         :return:
         """
+        self.refresh_session()
         logger.info(" ---Inside ebs :: gp2_to_gp3()")
 
         recommendation = []
 
         try:
             for region, volumes in ebs_volumes.items():
                 for volume in volumes:
@@ -285,14 +288,15 @@
     # Generate recommendation for unused ebs volume
     def unused_ebs_volume(self, ebs_volumes) -> list:
         """
         :param ebs_volumes:
         :param self:
         :return:
         """
+        self.refresh_session()
         logger.info(" ---Inside ebs :: unused_ebs_volume()")
 
         recommendation = []
 
         try:
             for region, volumes in ebs_volumes.items():
                 for volume in volumes:
```

### Comparing `aws_recommendation-0.2.7/aws_recommendation/ec2.py` & `aws_recommendation-0.3.1/aws_recommendation/ec2.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
         return response
 
 
     # Generates recommendation to delete idle instances
     def delete_or_downsize_instance_recommendation(self, ec2_instances) -> list:
         logger.info(" ---Inside delete_or_downsize_instance_recommendation()")
+        self.refresh_session()
 
         recommendation = []
 
 
         try:
             for region, instances in ec2_instances.items():
                 for instance in instances:
@@ -146,14 +147,15 @@
 
         return recommendation
 
 
     # generates the recommendation to delete unattached volumes
     def purge_unattached_vol_recommendation(self, regions) -> list:
         logger.info(" ---Inside purge_unattached_vol_recommendation()")
+        self.refresh_session()
 
         recommendation = []
 
         # iterating through all the available regions
         for region in regions:
             try:
                 vol_data = {}
@@ -230,14 +232,15 @@
 
         return recommendation
 
 
     # Generates the recommendation to purge the snapshots which are older than 8 weeks
     def purge_8_weeks_older_snapshots(self, regions) -> list:
         logger.info(" ---Inside purge_8_weeks_older_snapshots()")
+        self.refresh_session()
 
         recommendation = []
 
         datetime_8_weeks_ago = dt.datetime.now() - dt.timedelta(weeks=8)
         timezone = pytz.timezone("UTC")
         datetime_8_weeks_ago = timezone.localize(datetime_8_weeks_ago)
 
@@ -324,14 +327,15 @@
     def reserved_instance_lease_expiration(self, regions) -> list:
         """
         :param regions:
         :param self:
         :return list: list of recommendations for reserved instances for lease expiration
         """
         logger.info(' ---Inside ec2 :: reserved_instance_lease_expiration()')
+        self.refresh_session()
 
         recommendation = []
 
         datetime_now = dt.datetime.utcnow()
         timezone = pytz.timezone("UTC")
         datetime_30_days_ago = timezone.localize(datetime_now - dt.timedelta(days=30))
 
@@ -402,14 +406,15 @@
     def unassociated_elastic_ip_addresses(self, regions) -> list:
         """
         :param regions:
         :param self:
         :return list: list of recommendations for unassociated elastic ip addresses
         """
         logger.info(" ---Inside ec2 :: unassociated_elastic_ip_addresses()")
+        self.refresh_session()
 
         recommendation = []
 
         for region in regions:
             try:
                 client = self.session.client('ec2', region_name=region)
                 response = client.describe_addresses()
@@ -472,14 +477,15 @@
     def unused_ami(self, regions) -> list:
         """
         :param regions:
         :param self:
         :return:
         """
         logger.info(' ---Inside ec2 :: unused_ami()')
+        self.refresh_session()
 
         recommendation = []
 
         for region in regions:
             try:
                 client = self.session.client('ec2', region_name=region)
```

### Comparing `aws_recommendation-0.2.7/aws_recommendation/elb.py` & `aws_recommendation-0.3.1/aws_recommendation/elb.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     def idle_elastic_load_balancer(self, regions):
         """
         :param regions:
         :param self:
         :return:
         """
         logger.info(" ---Inside elb :: idle_elastic_load_balancer()")
+        self.refresh_session()
 
         recommendation = []
 
         for region in regions:
             try:
                 client = self.session.client('elbv2', region_name=region)
                 marker = ''
@@ -130,14 +131,15 @@
     def unused_elb(self, regions) -> list:
         """
         :param regions:
         :param self:
         :return:
         """
         logger.info(" ---Inside elb :: unused_elb()")
+        self.refresh_session()
 
         recommendation = []
 
         for region in regions:
             try:
                 client = self.session.client('elb', region_name=region)
                 marker = ''
```

### Comparing `aws_recommendation-0.2.7/aws_recommendation/kms.py` & `aws_recommendation-0.3.1/aws_recommendation/kms.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     def unused_cmk(self, regions: list) -> list:
         """
         :param regions:
         :param self:
         :return:
         """
         logger.info(" ---Inside kms :: unused_cmk()")
+        self.refresh_session()
 
         recommendation = []
 
         for region in regions:
             try:
                 client = self.session.client('kms', region_name=region)
```

### Comparing `aws_recommendation-0.2.7/aws_recommendation/rds.py` & `aws_recommendation-0.3.1/aws_recommendation/rds.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         response.extend(self.rds_general_purpose_ssd(rds_instances))
 
         return response
 
     # Generates the recommendation to downsize underutilized rds instance
     def downsize_underutilized_rds_recommendation(self, rds_instances) -> list:
         logger.info(" ---Inside downsize_underutilized_rds_recommendation()")
+        self.refresh_session()
 
         recommendation = []
 
         try:
             for region, instances in rds_instances.items():
                 for instance in instances:
                     cpu_stats = self.get_metrics_stats(
@@ -104,14 +105,15 @@
     def rds_idle_db_instances(self, rds_instances) -> list:
         """
 
         :param self:
         :return list: recommendation list for rds idle db instances
         """
         logger.info(' ---Inside rds :: rds_idle_db_instances()')
+        self.refresh_session()
 
         recommendation = []
 
         try:
             for region, instances in rds_instances.items():
                 for instance in instances:
                     datapoints = self.get_metrics_stats(
@@ -182,14 +184,15 @@
     def rds_general_purpose_ssd(self, rds_instances) -> list:
         """
         :param rds_instances:
         :param self:
         :return:
         """
         logger.info(' ---Inside rds :: rds_general_purpose_ssd()')
+        self.refresh_session()
 
         recommendation = []
 
         try:
             for region, instances in rds_instances.items():
                 for instance in instances:
                     storage = instance['StorageType']
```

### Comparing `aws_recommendation-0.2.7/aws_recommendation/redshift.py` & `aws_recommendation-0.3.1/aws_recommendation/redshift.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 class redshift:
     def get_redshift_recommendations(self, regions=None):
         """
         :param regions:
         :return:
         """
         logger.info(" ---Inside redshift :: get_redshift_recommendations()--- ")
+        self.refresh_session()
 
         if regions is None:
             regions = self.get_regions()
 
         return self.under_utilized_redshift_cluster(regions)
 
     # Generated recommendation for under utilized redshift cluster
     def under_utilized_redshift_cluster(self, regions) -> list:
         """
         :param regions:
         :param self:
         :return:
         """
         logger.info(" ---Inside redshift :: under_utilized_redshift_cluster()")
+        self.refresh_session()
 
         recommendation = []
 
         for region in regions:
             try:
                 client = self.session.client('redshift', region_name=region)
                 clusters = self.list_redshift_clusters(client)
```

### Comparing `aws_recommendation-0.2.7/aws_recommendation/s3.py` & `aws_recommendation-0.3.1/aws_recommendation/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     # returns the list of s3 buckets
     def __list_s3_buckets(self):
         """
         :return:
         """
         logger.info(" ---Inside utils :: list_s3_buckets()--- ")
+        self.refresh_session()
         client = self.session.client('s3')
 
         try:
             response = client.list_buckets()
             return response['Buckets']
         except ClientError as e:
             return e.response['Error']['Code']
@@ -34,14 +35,15 @@
     def __enable_s3_bucket_keys(self, bucket_list: list) -> list:
         """
         :param bucket_list:
         :param self:
         :return:
         """
         logger.info(" ---Inside s3 :: enable_s3_bucket_keys()")
+        self.refresh_session()
 
         recommendation = []
 
         client = self.session.client('s3')
 
         for bucket in bucket_list:
             try:
@@ -96,14 +98,15 @@
     def __s3_bucket_versioning_enabled(self, bucket_list: list):
         """
         :param bucket_list:
         :param self:
         :return dict: details of s3 bucket versioning enabled compliance.py
         """
         logger.info(" ---Inside s3 :: s3_bucket_versioning_enabled()")
+        self.refresh_session()
 
         recommendation = []
 
         client = self.session.client('s3')
 
         for bucket in bucket_list:
             bucket_name = bucket['Name']
@@ -197,14 +200,15 @@
     def __s3_bucket_lifecycle_configuration(self, bucket_list: list)-> list:
         """
         :param bucket_list:
         :param self:
         :return dict: details of s3 bucket versioning enabled compliance.py
         """
         logger.info(" ---Inside s3 :: s3_bucket_lifecycle_configuration()")
+        self.refresh_session()
 
         recommendation = []
 
         client = self.session.client('s3')
 
         for bucket in bucket_list:
             bucket_name = bucket['Name']
```

### Comparing `aws_recommendation-0.2.7/aws_recommendation/truted_advisor.py` & `aws_recommendation-0.3.1/aws_recommendation/truted_advisor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     # Generates recommendation from trusted advisor
     def get_trusted_advisor_recommendations(self) -> list:
         """
         :param self:
         :return: list of
         """
         logger.info(" ---Inside get_trusted_advisor_recommendations")
+        self.refresh_session()
 
         recommendation = []
         client = self.session.client('support')
         try:
             response = client.describe_trusted_advisor_checks(
                 language='en'
             )
```

### Comparing `aws_recommendation-0.2.7/aws_recommendation/utils.py` & `aws_recommendation-0.3.1/aws_recommendation/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 class utils:
     # returns the list of instances
     def list_instances(self, regions) -> dict:
         logger.info(" ---Inside utils :: list_instances()--- ")
+        self.refresh_session()
 
         instance_lst = {}
 
         for region in regions:
             client = self.session.client('ec2', region_name=region)
 
             marker = ''
@@ -44,14 +45,15 @@
     # returns the list of rds instances
     def list_rds_instances(self, regions) -> dict:
         """
         :param regions:
         :return:
         """
         logger.info(" ---Inside utils :: list_rds_instances()--- ")
+        self.refresh_session()
         rds_instance_lst = {}
 
         for region in regions:
             client = self.session.client('rds', region_name=region)
             marker = ''
             while True:
                 response = client.describe_db_instances(
@@ -69,14 +71,15 @@
         return rds_instance_lst
 
 
     # returns the metrics data
     def get_metrics_stats(self, region, namespace: str, dimensions: list,
                           metric_name='CPUUtilization', start_time=dt.datetime.utcnow() - relativedelta(days=7),
                           end_time=dt.datetime.utcnow(), period=86400, stats=None, unit='Percent'):
+        self.refresh_session()
         if stats is None:
             stats = ["Average"]
 
         client = self.session.client('cloudwatch', region_name=region)
 
         if unit is None:
             response_cpu = client.get_metric_statistics(
@@ -105,14 +108,15 @@
     # returns the list of redshift clusters
     def list_redshift_clusters(self, client) -> list:
         """
         :param client:
         :return:
         """
         logger.info(" ---Inside utils() :: list_redshift_clusters()")
+        self.refresh_session()
 
         cluster_list = []
 
         marker = ''
         while True:
             if marker == '' or marker is None:
                 response = client.describe_clusters()
@@ -135,27 +139,30 @@
     # returns the list of aws regions
     def get_regions(self):
         """
         :session: aws session object
         :return: list of regions
         """
         logger.info(" ---Inside utils :: get_regions()--- ")
+        self.refresh_session()
+
         client = self.session.client('ec2', region_name='us-east-1')
         region_response = client.describe_regions()
 
         regions = [region['RegionName'] for region in region_response['Regions']]
         return regions
 
 #     returns the list of ebs volumes
     def list_ebs_volumes(self, regions: list) -> dict:
         """
         :param regions:
         :return:
         """
         logger.info("---Inside utils :: list_ebs_volumes()--- ")
+        self.refresh_session()
 
         ebs_volumes = {}
 
         for region in regions:
             client = self.session.client('ec2', region_name=region)
             marker = ''
             while True:
```

### Comparing `aws_recommendation-0.2.7/aws_recommendation.egg-info/PKG-INFO` & `aws_recommendation-0.3.1/aws_recommendation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-recommendation
-Version: 0.2.7
+Version: 0.3.1
 Summary: Provides AWS recommendations
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `aws_recommendation-0.2.7/aws_recommendation.egg-info/SOURCES.txt` & `aws_recommendation-0.3.1/aws_recommendation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.7/pyproject.toml` & `aws_recommendation-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aws_recommendation"
-version = "0.2.7"
+version = "0.3.1"
 authors = [
   { name="dheeraj.banodha", email="dheerajmbanodha@gmail.com" },
 ]
 description = "Provides AWS recommendations"
 readme = "README.md"
 requires-python = ">=3.7"
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

