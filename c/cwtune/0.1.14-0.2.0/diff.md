# Comparing `tmp/cwtune-0.1.14.tar.gz` & `tmp/cwtune-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwtune-0.1.14.tar", last modified: Tue Aug  1 11:47:42 2023, max compression
+gzip compressed data, was "cwtune-0.2.0.tar", last modified: Thu Aug  3 10:14:49 2023, max compression
```

## Comparing `cwtune-0.1.14.tar` & `cwtune-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,21 @@
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:47:42.245481 cwtune-0.1.14/
--rw-r--r--   0 arran      (501) staff       (20)     1204 2023-07-25 11:17:40.000000 cwtune-0.1.14/.gitignore
--rw-r--r--   0 arran      (501) staff       (20)     1070 2023-07-25 11:24:31.000000 cwtune-0.1.14/LICENSE
--rw-r--r--   0 arran      (501) staff       (20)     1532 2023-08-01 11:47:42.245772 cwtune-0.1.14/PKG-INFO
--rw-r--r--   0 arran      (501) staff       (20)      860 2023-07-11 11:02:07.000000 cwtune-0.1.14/README.rst
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:47:42.155293 cwtune-0.1.14/cwtune/
--rw-r--r--   0 arran      (501) staff       (20)      123 2023-07-11 11:02:07.000000 cwtune-0.1.14/cwtune/__init__.py
--rw-r--r--   0 arran      (501) staff       (20)     9129 2023-08-01 11:46:42.000000 cwtune-0.1.14/cwtune/analyze.py
--rw-r--r--   0 arran      (501) staff       (20)     5599 2023-07-25 10:25:39.000000 cwtune-0.1.14/cwtune/aws.py
--rw-r--r--   0 arran      (501) staff       (20)     1067 2023-08-01 11:42:12.000000 cwtune-0.1.14/cwtune/cli.py
--rw-r--r--   0 arran      (501) staff       (20)     2400 2023-07-24 12:37:41.000000 cwtune-0.1.14/cwtune/timeseries.py
--rw-r--r--   0 arran      (501) staff       (20)     2760 2023-07-25 12:45:29.000000 cwtune-0.1.14/cwtune/utils.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:47:42.165642 cwtune-0.1.14/cwtune.egg-info/
--rw-r--r--   0 arran      (501) staff       (20)     1532 2023-08-01 11:47:41.000000 cwtune-0.1.14/cwtune.egg-info/PKG-INFO
--rw-r--r--   0 arran      (501) staff       (20)      565 2023-08-01 11:47:41.000000 cwtune-0.1.14/cwtune.egg-info/SOURCES.txt
--rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-01 11:47:41.000000 cwtune-0.1.14/cwtune.egg-info/dependency_links.txt
--rw-r--r--   0 arran      (501) staff       (20)       43 2023-08-01 11:47:41.000000 cwtune-0.1.14/cwtune.egg-info/entry_points.txt
--rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-01 11:47:41.000000 cwtune-0.1.14/cwtune.egg-info/not-zip-safe
--rw-r--r--   0 arran      (501) staff       (20)       65 2023-08-01 11:47:41.000000 cwtune-0.1.14/cwtune.egg-info/requires.txt
--rw-r--r--   0 arran      (501) staff       (20)        7 2023-08-01 11:47:41.000000 cwtune-0.1.14/cwtune.egg-info/top_level.txt
--rw-r--r--   0 arran      (501) staff       (20)       66 2023-07-25 12:31:11.000000 cwtune-0.1.14/requirements.txt
--rw-r--r--   0 arran      (501) staff       (20)      424 2023-08-01 11:47:42.248702 cwtune-0.1.14/setup.cfg
--rw-r--r--   0 arran      (501) staff       (20)     1338 2023-08-01 11:46:52.000000 cwtune-0.1.14/setup.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:47:42.171811 cwtune-0.1.14/tests/
--rw-r--r--   0 arran      (501) staff       (20)       36 2023-07-11 11:02:07.000000 cwtune-0.1.14/tests/__init__.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-01 11:47:42.243670 cwtune-0.1.14/tests/__pycache__/
--rw-r--r--   0 arran      (501) staff       (20)      208 2023-07-11 11:10:33.000000 cwtune-0.1.14/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 arran      (501) staff       (20)     4029 2023-07-11 11:10:33.000000 cwtune-0.1.14/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc
--rw-r--r--   0 arran      (501) staff       (20)     7071 2023-07-17 14:03:14.000000 cwtune-0.1.14/tests/__pycache__/test_cwtune.cpython-311.pyc
--rw-r--r--   0 arran      (501) staff       (20)     3754 2023-07-17 14:03:13.000000 cwtune-0.1.14/tests/test_cwtune.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-03 10:14:49.644513 cwtune-0.2.0/
+-rw-r--r--   0 arran      (501) staff       (20)     1070 2023-07-25 11:24:31.000000 cwtune-0.2.0/LICENSE
+-rw-r--r--   0 arran      (501) staff       (20)     3206 2023-08-03 10:14:49.644723 cwtune-0.2.0/PKG-INFO
+-rw-r--r--   0 arran      (501) staff       (20)     2535 2023-08-03 09:01:39.000000 cwtune-0.2.0/README.md
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-03 10:14:49.629230 cwtune-0.2.0/cwtune/
+-rw-r--r--   0 arran      (501) staff       (20)      123 2023-07-11 11:02:07.000000 cwtune-0.2.0/cwtune/__init__.py
+-rw-r--r--   0 arran      (501) staff       (20)     8949 2023-08-03 09:45:53.000000 cwtune-0.2.0/cwtune/analyze.py
+-rw-r--r--   0 arran      (501) staff       (20)     4987 2023-08-03 09:46:34.000000 cwtune-0.2.0/cwtune/aws.py
+-rw-r--r--   0 arran      (501) staff       (20)     2694 2023-08-02 14:44:19.000000 cwtune-0.2.0/cwtune/cli.py
+-rw-r--r--   0 arran      (501) staff       (20)     5116 2023-08-02 13:44:14.000000 cwtune-0.2.0/cwtune/timeseries.py
+-rw-r--r--   0 arran      (501) staff       (20)     2836 2023-08-01 12:29:11.000000 cwtune-0.2.0/cwtune/utils.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-08-03 10:14:49.643873 cwtune-0.2.0/cwtune.egg-info/
+-rw-r--r--   0 arran      (501) staff       (20)     3206 2023-08-03 10:14:49.000000 cwtune-0.2.0/cwtune.egg-info/PKG-INFO
+-rw-r--r--   0 arran      (501) staff       (20)      349 2023-08-03 10:14:49.000000 cwtune-0.2.0/cwtune.egg-info/SOURCES.txt
+-rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-03 10:14:49.000000 cwtune-0.2.0/cwtune.egg-info/dependency_links.txt
+-rw-r--r--   0 arran      (501) staff       (20)       43 2023-08-03 10:14:49.000000 cwtune-0.2.0/cwtune.egg-info/entry_points.txt
+-rw-r--r--   0 arran      (501) staff       (20)        1 2023-08-03 10:14:49.000000 cwtune-0.2.0/cwtune.egg-info/not-zip-safe
+-rw-r--r--   0 arran      (501) staff       (20)      109 2023-08-03 10:14:49.000000 cwtune-0.2.0/cwtune.egg-info/requires.txt
+-rw-r--r--   0 arran      (501) staff       (20)        7 2023-08-03 10:14:49.000000 cwtune-0.2.0/cwtune.egg-info/top_level.txt
+-rw-r--r--   0 arran      (501) staff       (20)      423 2023-08-03 10:14:49.646009 cwtune-0.2.0/setup.cfg
+-rw-r--r--   0 arran      (501) staff       (20)     1336 2023-08-03 10:14:44.000000 cwtune-0.2.0/setup.py
```

### Comparing `cwtune-0.1.14/LICENSE` & `cwtune-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.14/cwtune/analyze.py` & `cwtune-0.2.0/cwtune/analyze.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,234 +1,234 @@
+from enum import Enum
 import click
 from datetime import timedelta
 from terminaltables import AsciiTable
 from thefuzz import fuzz
 import json
 import math
 from .utils import create_cloudwatch_link, format_timestamp, select_range
-from .aws import list_metrics, get_metric_data, create_cloudwatch_alarm
-from .timeseries import zero_pad, get_breaches, longest_breach
+from .aws import list_metrics, get_metric_data, create_cloudwatch_alarm, cw_client
+from .timeseries import zero_pad, get_breaches, longest_breach, ThresholdAdjustment
 
 # Define constants
 WEIGHTS = {'Namespace': 0.5, 'MetricName': 0.3, 'Dimensions': 0.3}
 MAX_ITERATIONS = 100
-
+NUM_SEARCH_RESULTS = 5
 
 def prompt_metric_search(metrics):
     """Prompts the user for a metric search and returns a selected metric."""
     click.echo('Enter a metric search eg "EC2 CPUUtilization XService"')
     while True:
         search = click.prompt('Search', type=str)
         click.echo('Select a metric from the list below')
 
         metrics = sorted(metrics, key=lambda metric: WEIGHTS['Namespace'] * fuzz.token_set_ratio(search, metric['Namespace']) +
                          WEIGHTS['MetricName'] * fuzz.token_set_ratio(search, metric['MetricName']) +
                          WEIGHTS['Dimensions'] * fuzz.token_set_ratio(search, json.dumps(metric['Dimensions'])), reverse=True)
 
-        for i, metric in enumerate(metrics[:5]):
+        for i, metric in enumerate(metrics[:NUM_SEARCH_RESULTS]):
             click.echo(
                 f"{i + 1}: {metric['Namespace']} {metric['MetricName']} {json.dumps({dimension['Name']: dimension['Value'] for dimension in metric['Dimensions']})}")
 
         click.echo("6: Search again")
 
         selected_metric = click.prompt('Please enter a number to select a metric', type=int)
         click.echo()
 
-        if selected_metric == 6:
+        if selected_metric == NUM_SEARCH_RESULTS + 1:
             continue
 
-        if selected_metric < 1 or selected_metric > 5:
+        if selected_metric < 1 or selected_metric > NUM_SEARCH_RESULTS:
             click.echo('Invalid selection.')
             continue
 
         return metrics[selected_metric - 1]
 
 
-def retrieve_and_pad_data(metric, period, statistic, aws_profile, region):
+def retrieve_and_pad_data(metric, period, statistic, client):
     """Retrieves and pads metric data."""
     start, end = select_range()
 
     click.echo(f"Retrieving data from {format_timestamp(start)} to {format_timestamp(end)}.")
 
-    data = get_metric_data(start, end, metric['MetricName'], metric['Namespace'],
-                           metric['Dimensions'], period, statistic, aws_profile, region)
+    data = get_metric_data(start, end, metric['MetricName'], metric['Namespace'], metric['Dimensions'], period, statistic, client)
     click.echo(f"Retrieved {len(data)} data points.")
 
     if len(data) == 0:
         click.echo("No data found.")
         return []
 
     data = zero_pad(data, period, start, end)
     click.echo(f"Padded data to {len(data)} data points.")
     return data, start, end
 
 
-def calculate_threshold_and_breaches(data, alarm_type, min_duration, max_alerts):
+def calculate_threshold_and_breaches(data, alarm_type, window_size, max_alerts):
     """Calculates threshold and breaches for the given data."""
     # Initial values
-    threshold = 0
+    threshold = 1 if alarm_type.is_lt() else 0
     breaches = get_breaches(data, threshold, alarm_type,
-                            min_duration, int(min_duration/2))
+                            window_size, math.ceil(window_size / 2))
 
     values = [value for timestamp, value in data]
     sum_values = sum(values)
     std_dev = sum([abs(value - sum_values / len(values))
                   for value in values]) / len(values)
 
     # Threshold search when breaches are too many or too long
     if len(breaches) > max_alerts or longest_breach(breaches) > timedelta(days=2):
         click.echo('Starting binary search for threshold.')
 
         # mean +/- 5 standard deviations depending on the alarm type
-        if alarm_type == 'gt':
+        if alarm_type.is_gt():
             threshold = math.ceil(sum_values / len(values) + 5 * std_dev)
-        elif alarm_type == 'lt':
-            threshold = math.ceil(sum_values / len(values) - 5 * std_dev)
+        elif alarm_type.is_lt():
+            threshold = max(math.ceil(sum_values / len(values) - 5 * std_dev), 1)
 
         min_threshold = min(values)
         max_threshold = max(values) * 2
 
         for i in range(MAX_ITERATIONS):
             click.echo(
                 f"Iteration {i + 1}. Evaluating threshold of {threshold}.")
             threshold = math.ceil((min_threshold + max_threshold) / 2)
             breaches = get_breaches(
-                data, threshold, alarm_type, min_duration, int(min_duration/2))
+                data, threshold, alarm_type, window_size, math.ceil(window_size / 2))
 
             if len(breaches) > max_alerts:
                 min_threshold = threshold
             else:
                 if longest_breach(breaches) < timedelta(days=2):
                     break
                 else:
                     min_threshold = threshold
                     max_threshold = max_threshold * 2
 
     return threshold, breaches
 
 
-def output_rating_and_adjustment(metric, data, alarm_type, threshold, min_duration, breaches, start, region, statistic, period):
+def output_rating_and_adjustment(metric, data, alarm_type, threshold, window_size, breaches, start, region, statistic, period):
     """Handles output rating and adjustment based on user feedback."""
-    while True:
-        if threshold > 1:
-            threshold = math.ceil(threshold)
 
-        click.echo(f"X {alarm_type} {threshold} for {int(min_duration/2)} in {min_duration} datapoints would have resulted in {len(breaches)} breaches since {format_timestamp(start)}.")
+    # Create an instance of ThresholdAdjustment
+    adjustment = ThresholdAdjustment(threshold, breaches, data, alarm_type, window_size)
 
+    # Define option map
+    option_map = {
+        1: {
+            "description": "Too many alerts",
+            "action": adjustment.decrease_sensitivity,
+        },
+        2: {
+            "description": "Too few alerts",
+            "action": adjustment.increase_sensitivity,
+        },
+        3: {
+            "description": "Too many flapping alerts",
+            "action": adjustment.increase_window_size,
+        },
+        4: {
+            "description": "Alets are too slow to trigger",
+            "action": adjustment.decrease_window_size,
+        },
+        5: {
+            "description": "Just right",
+            "action": None,  # No action for this option
+        },
+    }
+
+    while True:
+        if adjustment.threshold > 1:
+            adjustment.threshold = math.ceil(adjustment.threshold)
+
+        click.echo(f"X {'>' if alarm_type.is_gt() else '<'} {adjustment.threshold} for {int(adjustment.window_size/2)} in {adjustment.window_size} datapoints would have triggered {len(adjustment.breaches)} alerts.")
         table_data = [['Start', 'End', 'Duration', 'Link']]
 
-        for breach in breaches:
+        for breach in adjustment.breaches:
             duration = breach['end'] - breach['start']
             link = create_cloudwatch_link(
                 metric['Namespace'], metric['MetricName'], breach['start'],
-                breach['end'], metric['Dimensions'], threshold, region, statistic, period
+                breach['end'], metric['Dimensions'], adjustment.threshold, region, statistic, period
             )
             table_data.append([format_timestamp(breach['start']),
                               format_timestamp(breach['end']), duration, link])
 
         if len(table_data) > 1:
-            table = AsciiTable(table_data)
+            table = AsciiTable(table_data) 
             click.echo(table.table)
             click.echo()
 
         click.echo("Rate the output")
-        click.echo("1: Too many alerts")
-        click.echo("2: Too few alerts")
-
-        if len(breaches) > 0:
-            click.echo("3: Incident(s) too short")
-            click.echo("4: Incident(s) alerted too late")
-
-        click.echo("5: Just right")
+        for option, details in option_map.items():
+            click.echo(f"{option}: {details['description']}")
 
-        rating = click.prompt(
-            'Please enter a number to rate the output', type=int)
+        rating = click.prompt('Please enter a number to rate the output', type=int)
         click.echo()
 
-        if rating == 1:
-            click.echo("Increasing threshold by 10%")
-            threshold = math.ceil(threshold * 1.1)
-            breaches = get_breaches(
-                data, threshold, alarm_type, min_duration, int(min_duration/2))
-        elif rating == 2:
-            click.echo("Decreasing threshold")
-            if threshold < 10:
-                threshold = threshold - 1
+        selected_option = option_map.get(rating)
+        if selected_option:
+            action = selected_option.get('action')
+            if action:
+                action()
             else:
-                threshold = math.ceil(threshold * 0.9)
-            breaches = get_breaches(
-                data, threshold, alarm_type, min_duration, int(min_duration/2))
-        elif rating == 3:
-            click.echo("Increasing minimum duration by 1 minute")
-            min_duration += 1
-            breaches = get_breaches(
-                data, threshold, alarm_type, min_duration, int(min_duration/2))
-        elif rating == 4:
-            if min_duration == 1:
-                click.echo("Minimum duration cannot be decreased further")
-                continue
-            click.echo("Decreasing minimum duration by 1 minute")
-            min_duration -= 1
-            breaches = get_breaches(
-                data, threshold, alarm_type, min_duration, int(min_duration/2))
-        elif rating == 5:
-            break
+                break
 
-    return threshold, min_duration
+    return adjustment.threshold, adjustment.window_size
 
 
-def ask_to_create_alarm(metric, threshold, alarm_type, aws_profile, region, statistic, period, min_duration):
+def ask_to_create_alarm(metric, threshold, alarm_type, client, statistic, period, window_size):
     """Asks the user if they want to create a CloudWatch alarm and creates it if they do."""
     if click.confirm('Create/Update an alarm for this metric?', default=True):
         create_cloudwatch_alarm(
             metric['MetricName'], metric['Namespace'], metric['Dimensions'], threshold, alarm_type,
-            aws_profile=aws_profile, region=region, statistic=statistic, period=period, min_duration=min_duration
+            client, statistic=statistic, period=period, window_size=window_size
         )
 
 
-def run(alarm_type, aws_profile=None, period=5, statistic='Sum', region='us-east-1', min_duration=5, max_alerts=5):
+def run(alarm_type, aws_profile=None, period=5, statistic='Sum', region='us-east-1', window_size=5, max_alerts=5, client=None):
     """Select threshold for CloudWatch metrics."""
+
+    if not client:
+        client = cw_client(aws_profile, region)
+
     try:
-        metrics = list_metrics(aws_profile, region)
+        metrics = list_metrics(client)
     except Exception as e:
         click.echo(f"Failed to list metrics: {e}")
         return 1  # Non-zero status code to indicate an error
 
     try:
         metric = prompt_metric_search(metrics)
     except Exception as e:
         click.echo(f"Failed to prompt for metric search: {e}")
         return 1
 
     try:
-        data, start, end = retrieve_and_pad_data(
-            metric, period, statistic, aws_profile, region)
+        data, start, end = retrieve_and_pad_data(metric, period, statistic, client)
     except Exception as e:
         click.echo(f"Failed to retrieve and pad data: {e}")
         return 1
 
     if len(data) == 0:
         return 0
 
     try:
-        threshold, breaches = calculate_threshold_and_breaches(
-            data, alarm_type, min_duration, max_alerts)
+        threshold, breaches = calculate_threshold_and_breaches(data, alarm_type, window_size, max_alerts)
     except Exception as e:
         click.echo(f"Failed to calculate threshold and breaches: {e}")
         return 1
 
     try:
-        threshold, min_duration = output_rating_and_adjustment(
-            metric, data, alarm_type, threshold, min_duration, breaches, start, region, statistic, period
+        threshold, window_size = output_rating_and_adjustment(
+            metric, data, alarm_type, threshold, window_size, breaches, start, region, statistic, period
         )
     except Exception as e:
         click.echo(f"Failed to adjust output based on rating: {e}")
         return 1
 
     try:
-        ask_to_create_alarm(metric, threshold, alarm_type,
-                            aws_profile, region, statistic, period, min_duration)
+        ask_to_create_alarm(metric, threshold, alarm_type, client, statistic, period, window_size)
     except Exception as e:
         click.echo(f"Failed to create alarm: {e}")
         return 1
 
     return 0
```

### Comparing `cwtune-0.1.14/cwtune/utils.py` & `cwtune-0.2.0/cwtune/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         response.raise_for_status()
         return response.text
     except requests.exceptions.RequestException as e:
         print(f"Error while shortening the URL: {e}")
         return url
 
 
+# This should probaly extacted to a standalone lib as it is generaly useful
 def create_cloudwatch_link(namespace: str, metric_name: str, start: datetime, end: datetime, dimensions: list, threshold: float, region: str, statistic: str, period: int, shorten=True) -> str:
     """Create a link to the CloudWatch graph for the given metric."""
     base_url = f"https://{region}.console.aws.amazon.com/cloudwatch/home?region={region}#metricsV2?"
 
     encoded_namespace = namespace.replace('/', '*2f')
 
     encoded_dimensions_list = [
```

### Comparing `cwtune-0.1.14/setup.py` & `cwtune-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-with open('README.rst') as readme_file:
+with open('README.md') as readme_file:
     readme = readme_file.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 test_requirements = ['pytest>=3', ]
 
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords='cwtune',
     name='cwtune',
     packages=find_packages(include=['cwtune', 'cwtune.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/availabl-co/cwtune',
-    version='0.1.14',
+    version='0.2.0',
     zip_safe=False,
 )
```

