# Comparing `tmp/flexvalue-2.0.5.tar.gz` & `tmp/flexvalue-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexvalue-2.0.5.tar", last modified: Thu Jun 29 19:44:37 2023, max compression
+gzip compressed data, was "flexvalue-2.0.6.tar", last modified: Thu Aug  3 15:13:16 2023, max compression
```

## Comparing `flexvalue-2.0.5.tar` & `flexvalue-2.0.6.tar`

### file list

```diff
@@ -1,52 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:44:37.967881 flexvalue-2.0.5/
--rw-r--r--   0 root         (0) root         (0)      644 2023-06-29 19:44:37.967881 flexvalue-2.0.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    30648 2023-06-29 00:17:22.000000 flexvalue-2.0.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:44:37.935877 flexvalue-2.0.5/flexvalue/
--rw-rw-r--   0 root         (0) root         (0)     1286 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      984 2023-06-29 19:43:51.000000 flexvalue-2.0.5/flexvalue/__version__.py
--rw-rw-r--   0 root         (0) root         (0)    14642 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/cet_flexvalue_compare.py
--rw-rw-r--   0 root         (0) root         (0)    10248 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/cli.py
--rw-rw-r--   0 root         (0) root         (0)     6030 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/config.py
--rw-rw-r--   0 root         (0) root         (0)    51781 2023-06-29 19:41:04.000000 flexvalue-2.0.5/flexvalue/db.py
--rw-rw-r--   0 root         (0) root         (0)     3440 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/examples.py
--rw-rw-r--   0 root         (0) root         (0)     3152 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/flexvalue.py
--rw-rw-r--   0 root         (0) root         (0)     2198 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/report.py
--rw-rw-r--   0 root         (0) root         (0)     1446 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:44:37.951879 flexvalue-2.0.5/flexvalue/sql/
--rw-rw-r--   0 root         (0) root         (0)      569 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/sql/create_elec_av_cost.sql
--rw-rw-r--   0 root         (0) root         (0)      269 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/sql/create_elec_load_shape.sql
--rw-rw-r--   0 root         (0) root         (0)      311 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/sql/create_gas_av_cost.sql
--rw-rw-r--   0 root         (0) root         (0)      439 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/sql/create_project_info.sql
--rw-rw-r--   0 root         (0) root         (0)      162 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/sql/create_therms_profile.sql
--rw-rw-r--   0 root         (0) root         (0)      125 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/sql/elec_av_costs_index.sql
--rw-rw-r--   0 root         (0) root         (0)      109 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/sql/elec_load_shape_index.sql
--rw-rw-r--   0 root         (0) root         (0)      219 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/sql/gas_av_costs_index.sql
--rw-rw-r--   0 root         (0) root         (0)      520 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/sql/postgres_indexes.sql
--rw-rw-r--   0 root         (0) root         (0)       90 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/sql/project_info_dates_index.sql
--rw-rw-r--   0 root         (0) root         (0)       66 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/sql/project_info_index.sql
--rw-rw-r--   0 root         (0) root         (0)      119 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/sql/therm_profile_index.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:44:37.967881 flexvalue-2.0.5/flexvalue/templates/
--rw-rw-r--   0 root         (0) root         (0)      242 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/templates/bq_create_elec_load_shape.sql
--rw-rw-r--   0 root         (0) root         (0)      186 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/templates/bq_create_therms_profile.sql
--rw-rw-r--   0 root         (0) root         (0)      603 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/templates/bq_populate_elec_load_shape.sql
--rw-rw-r--   0 root         (0) root         (0)      664 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/templates/bq_populate_metered_load_shape.sql
--rw-rw-r--   0 root         (0) root         (0)      571 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/templates/bq_populate_therms_profile.sql
--rw-rw-r--   0 root         (0) root         (0)    12645 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/templates/calculation.sql
--rw-rw-r--   0 root         (0) root         (0)     6677 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/templates/elec_calculation.sql
--rw-rw-r--   0 root         (0) root         (0)     6289 2023-06-29 04:31:43.000000 flexvalue-2.0.5/flexvalue/templates/gas_calculation.sql
--rw-rw-r--   0 root         (0) root         (0)      101 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/templates/get_project_info.sql
--rw-rw-r--   0 root         (0) root         (0)      117 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/templates/get_therms_profiles.sql
--rw-rw-r--   0 root         (0) root         (0)      693 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/templates/load_elec_av_costs.sql
--rw-rw-r--   0 root         (0) root         (0)      291 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/templates/load_elec_load_shape.sql
--rw-rw-r--   0 root         (0) root         (0)      296 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/templates/load_gas_av_costs.sql
--rw-rw-r--   0 root         (0) root         (0)      565 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/templates/load_project_info.sql
--rw-rw-r--   0 root         (0) root         (0)      201 2023-06-29 00:17:22.000000 flexvalue-2.0.5/flexvalue/templates/load_therms_profiles.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 19:44:37.943878 flexvalue-2.0.5/flexvalue.egg-info/
--rw-r--r--   0 root         (0) root         (0)      644 2023-06-29 19:44:37.000000 flexvalue-2.0.5/flexvalue.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1589 2023-06-29 19:44:37.000000 flexvalue-2.0.5/flexvalue.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 19:44:37.000000 flexvalue-2.0.5/flexvalue.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-29 19:44:37.000000 flexvalue-2.0.5/flexvalue.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      249 2023-06-29 19:44:37.000000 flexvalue-2.0.5/flexvalue.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-29 19:44:37.000000 flexvalue-2.0.5/flexvalue.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       63 2023-06-29 19:44:37.971881 flexvalue-2.0.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3536 2023-06-29 00:17:22.000000 flexvalue-2.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:13:16.813013 flexvalue-2.0.6/
+-rw-r--r--   0 root         (0) root         (0)      644 2023-08-03 15:13:16.813013 flexvalue-2.0.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    31706 2023-08-03 12:10:05.000000 flexvalue-2.0.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:13:16.793011 flexvalue-2.0.6/flexvalue/
+-rw-rw-r--   0 root         (0) root         (0)     1286 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      984 2023-08-03 15:10:45.000000 flexvalue-2.0.6/flexvalue/__version__.py
+-rw-rw-r--   0 root         (0) root         (0)    10248 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/cli.py
+-rw-rw-r--   0 root         (0) root         (0)     6167 2023-08-03 12:10:05.000000 flexvalue-2.0.6/flexvalue/config.py
+-rw-rw-r--   0 root         (0) root         (0)    52196 2023-08-03 12:10:05.000000 flexvalue-2.0.6/flexvalue/db.py
+-rw-rw-r--   0 root         (0) root         (0)     3440 2023-06-07 20:28:30.000000 flexvalue-2.0.6/flexvalue/examples.py
+-rw-rw-r--   0 root         (0) root         (0)     3152 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/flexvalue.py
+-rw-rw-r--   0 root         (0) root         (0)     1446 2023-06-07 20:28:30.000000 flexvalue-2.0.6/flexvalue/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:13:16.797011 flexvalue-2.0.6/flexvalue/sql/
+-rw-rw-r--   0 root         (0) root         (0)      596 2023-08-03 12:10:05.000000 flexvalue-2.0.6/flexvalue/sql/create_elec_av_cost.sql
+-rw-rw-r--   0 root         (0) root         (0)      269 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/sql/create_elec_load_shape.sql
+-rw-rw-r--   0 root         (0) root         (0)      338 2023-08-03 12:10:05.000000 flexvalue-2.0.6/flexvalue/sql/create_gas_av_cost.sql
+-rw-rw-r--   0 root         (0) root         (0)      466 2023-08-03 12:10:05.000000 flexvalue-2.0.6/flexvalue/sql/create_project_info.sql
+-rw-rw-r--   0 root         (0) root         (0)      162 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/sql/create_therms_profile.sql
+-rw-rw-r--   0 root         (0) root         (0)      125 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/sql/elec_av_costs_index.sql
+-rw-rw-r--   0 root         (0) root         (0)      109 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/sql/elec_load_shape_index.sql
+-rw-rw-r--   0 root         (0) root         (0)      219 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/sql/gas_av_costs_index.sql
+-rw-rw-r--   0 root         (0) root         (0)      520 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/sql/postgres_indexes.sql
+-rw-rw-r--   0 root         (0) root         (0)       90 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/sql/project_info_dates_index.sql
+-rw-rw-r--   0 root         (0) root         (0)       66 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/sql/project_info_index.sql
+-rw-rw-r--   0 root         (0) root         (0)      119 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/sql/therm_profile_index.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:13:16.813013 flexvalue-2.0.6/flexvalue/templates/
+-rw-rw-r--   0 root         (0) root         (0)      242 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/templates/bq_create_elec_load_shape.sql
+-rw-rw-r--   0 root         (0) root         (0)      186 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/templates/bq_create_therms_profile.sql
+-rw-rw-r--   0 root         (0) root         (0)      603 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/templates/bq_populate_elec_load_shape.sql
+-rw-rw-r--   0 root         (0) root         (0)      664 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/templates/bq_populate_metered_load_shape.sql
+-rw-rw-r--   0 root         (0) root         (0)      571 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/templates/bq_populate_therms_profile.sql
+-rw-rw-r--   0 root         (0) root         (0)    13001 2023-08-03 12:10:05.000000 flexvalue-2.0.6/flexvalue/templates/calculation.sql
+-rw-rw-r--   0 root         (0) root         (0)     6845 2023-08-03 12:10:05.000000 flexvalue-2.0.6/flexvalue/templates/elec_calculation.sql
+-rw-rw-r--   0 root         (0) root         (0)     6455 2023-08-03 12:10:05.000000 flexvalue-2.0.6/flexvalue/templates/gas_calculation.sql
+-rw-rw-r--   0 root         (0) root         (0)      101 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/templates/get_project_info.sql
+-rw-rw-r--   0 root         (0) root         (0)      117 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/templates/get_therms_profiles.sql
+-rw-rw-r--   0 root         (0) root         (0)      775 2023-08-03 12:10:05.000000 flexvalue-2.0.6/flexvalue/templates/load_elec_av_costs.sql
+-rw-rw-r--   0 root         (0) root         (0)      291 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/templates/load_elec_load_shape.sql
+-rw-rw-r--   0 root         (0) root         (0)      374 2023-08-03 12:10:05.000000 flexvalue-2.0.6/flexvalue/templates/load_gas_av_costs.sql
+-rw-rw-r--   0 root         (0) root         (0)      606 2023-08-03 12:10:05.000000 flexvalue-2.0.6/flexvalue/templates/load_project_info.sql
+-rw-rw-r--   0 root         (0) root         (0)      201 2023-06-27 21:10:56.000000 flexvalue-2.0.6/flexvalue/templates/load_therms_profiles.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:13:16.797011 flexvalue-2.0.6/flexvalue.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      644 2023-08-03 15:13:16.000000 flexvalue-2.0.6/flexvalue.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-08-03 15:13:16.000000 flexvalue-2.0.6/flexvalue.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 15:13:16.000000 flexvalue-2.0.6/flexvalue.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-08-03 15:13:16.000000 flexvalue-2.0.6/flexvalue.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-08-03 15:13:16.000000 flexvalue-2.0.6/flexvalue.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-03 15:13:16.000000 flexvalue-2.0.6/flexvalue.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       63 2023-08-03 15:13:16.813013 flexvalue-2.0.6/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3334 2023-07-13 20:34:17.000000 flexvalue-2.0.6/setup.py
```

### Comparing `flexvalue-2.0.5/PKG-INFO` & `flexvalue-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: flexvalue
-Version: 2.0.5
+Version: 2.0.6
 Summary: FLEXvalue: a tool for calculating avoided costs
 Home-page: http://github.com/recurve-methods/flexvalue
 Author: Recurve Analytics, Inc.
 Author-email: support@recurve.com
 License: Apache 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `flexvalue-2.0.5/README.rst` & `flexvalue-2.0.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,21 @@
 
 The gas avoided cost calculator compiles monthly marginal utility avoided costs for gas savings. Costs are provided for four different components and are projected forward through 2050. Avoided costs are distinct for each utility service territory (PG&E, SCE, SDG&E, and SoCalGas). Avoided costs are also somewhat different for distinct end use categories.
 
 The gas avoided cost calculator can be downloaded as a .xlsb file from `here <https://www.cpuc.ca.gov/General.aspx?id=5267>`_.
 
 The gas avoided cost calculator is a macro-driven Excel file, so several data extraction and transformation steps were done to combine all calculator results into a single table.
 
-*Currently the gas avoided costs data uses the same year-month avoided costs (using Utility: PGE, Class: Total Core, End Use: Small Boiler, Emission Control: Uncontrolled) for all analysis. Based on testing against the CET, different numerical factors are applied depending on the program administrator. Future work can incorporate the full suite of gas parameters.*
+*Currently the gas avoided costs data uses the same year-month avoided costs (using Utility: PGE, Class: Total Core, End Use: Small Boiler, Emission Control: Uncontrolled) for all analysis. Based on testing against the CET, different numerical adjustment factors are applied depending on the program administrator.*
+
+The adjustment factors applied are:
+- PGE: 0.933918
+- SCE/SCG: 0.868483
+- SDGE: 0.930421
+
 
 
 Inputs
 ######
 
 Input structures
 ================
@@ -90,14 +96,15 @@
     - **cap_and_trade**:
     - **ghg_adder**:
     - **ghg_rebalancing**:
     - **methane_leakage**:
     - **total**: This is the total avoided cost for this hour. It is the sum of the values in the component columns.
     - **marginal_ghg**:
     - **ghg_adder_rebalancing**:
+    - **value_curve_name**: The name of the value curve representing the avoided costs for a given hour. This may be null if only using a single value curve.
 
 
 Gas Avoided Costs
 -----------------
 
 The columns for the gas avoided cost data are as follows:
 
@@ -110,14 +117,15 @@
     - **market**: This column and the following, except "total", are the components of the avoided costs for this hour.
     - **t_d**:
     - **environment**:
     - **btm_methane**:
     - **total**: This is the total avoided cost for this hour. It is the sum of the values in the component columns.
     - **upstream_methane**:
     - **marginal_ghg**:
+    - **value_curve_name**: The name of the value curve representing the avoided costs for a given hour. This may be null if only using a single value curve.
 
 
 Electric Load Shapes
 --------------------
 
 The electric load shape data has a variable number of columns; after the fixed columns, there are N columns with each representing a given load shape. The load shape data always has exactly 8760 rows.
 
@@ -167,14 +175,15 @@
     - **discount_rate**: The quarterly discount rate to be applied within the net present value calculation
     - **admin**: The administrative costs assigned to the given measure, project, or portfolio
     - **measure**: The measure costs assigned to the given measure, project, or portfolio
     - **incentive**: The incentive costs assigned to the given measure, project, or portfolio
     - **therms_profile**: Indicates the season in which therms savings are achieved, can be one of ['annual', 'summer', 'winter']
     - **therms_savings**: The first year gas gross savings in Therms
     - **mwh_savings**: The first year electricity gross savings in MWh (used to scale the load shape savings data if using custom load shape)
+    - **value_curve_name**: The name of the value curve that the project should be matched to. This may be null if only using a single value curve.
 
 
 Metered Load Shapes
 -------------------
 
 The `metered_load_shape` CSV requires the following columns:
 
@@ -338,14 +347,15 @@
   reset_therms_profiles = false
   reset_gas_av_costs = false
   elec_components = ["energy", "losses", "ancillary_services", "capacity", "transmission", "distribution"]
   gas_components = ["market", "t_d", "environment", "btm_methane", "upstream_methane"]
   separate_output_tables = True
   electric_output_table = "example_dataset.hourly_electric_output"
   gas_output_table = "example_dataset.hourly_gas_output"
+  use_value_curve_name_for_join = False
 
   [database]
   #credentials = ""
   database_type = "bigquery"
   project = "oeem-avdcosts-platform"
   elec_av_costs_table = "example_dataset.full_ca_avoided_costs_2020acc_copy"
   elec_load_shape_table = "example_dataset.ca_hourly_electric_load_shapes_horizontal_copy"
@@ -369,14 +379,15 @@
   aggregation_columns = ["id", "hour_of_year", "year"]
   reset_elec_load_shape = false
   reset_elec_av_costs = false
   reset_therms_profiles = false
   reset_gas_av_costs = false
   elec_addl_fields = ["hour_of_year", "utility", "region", "month", "quarter", "hour_of_day", "discount"]
   gas_addl_fields = ["total", "month", "quarter"]
+  use_value_curve_name_for_join = False
 
   [database]
   database_type = "postgresql"
   host = "postgresql"
   port = 5432
   user = "postgres"
   password = "mypassword"
@@ -398,26 +409,29 @@
         reset_elec_load_shape=True,
         process_elec_load_shape=True,
         process_metered_load_shape=True,
         project_info_table="example_project_info",
         output_table="example_output_table",
         aggregation_columns=["id"],
         separate_output_tables=False
+        use_value_curve_name_for_join = False
     )
   flex_value_run.run()
 
 
 If the "process_X" flag is set, FLEXvalue will prepare that data for use in its main calculation. The meaning of "prepare" in this case depends on which database type you are using; if you are using BigQuery, it will do the following:
 
 * Create new tables for the therms profiles and electric load shapes. These will then be populated from the relevant tables specified in the config
 * Update the gas avoided costs table by adding and subsequently populating a timestamp column.
 * The electric avoided cost table is not touched - this is a no-op, as the available avoided cost data is already in a format that FLEXvalue can use.
 
 If you are using a relational database, the tables will be created if they don't exist, and then populated based on the data in the input files. The input files are csv files and have the columns described below. Header rows are required for the electrical load shape and therms profiles files. FLEXvalue attempts to determine the presence of header rows and will skip one if found and not needed. Note that FLEXvalue will NOT look up columns by the values in the header row - it's strictly positional.
 
+If the "use_value_curve_name_for_join" flag is set to True, FLEXvalue will include the "value_curve_name" during the "join" step when matching project savings to the avoided cost curve value. This enables users to include multiple value curves in the same avoided costs table if desired. If this flag is set to False, FLEXvalue will ignore the "value_curve_name" columns in both the project inputs and the avoided cost tables.
+
 .. _data-stores-label:
 
 Data stores
 ###########
 
 When using PostgreSQL, you must provide the following information:
```

### Comparing `flexvalue-2.0.5/flexvalue/__init__.py` & `flexvalue-2.0.6/flexvalue/__init__.py`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.5/flexvalue/__version__.py` & `flexvalue-2.0.6/flexvalue/__version__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,12 +16,12 @@
    See the License for the specific language governing permissions and
    limitations under the License.
 
 """
 __title__ = "FLEXvalue"
 __description__ = "FLEXvalue: a tool for calculating avoided costs"
 __url__ = "http://github.com/recurve-methods/flexvalue"
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 __author__ = "Recurve Analytics, Inc."
 __author_email__ = "support@recurve.com"
 __license__ = "Apache 2.0"
 __copyright__ = "Copyright 2021 Recurve Analytics, Inc."
```

### Comparing `flexvalue-2.0.5/flexvalue/cli.py` & `flexvalue-2.0.6/flexvalue/cli.py`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.5/flexvalue/config.py` & `flexvalue-2.0.6/flexvalue/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     reset_therms_profiles: bool = False
     reset_gas_av_costs: bool = False
     elec_components: List[str] = field(default_factory=list)
     gas_components: List[str] = field(default_factory=list)
     elec_addl_fields: List[str] = field(default_factory=list)
     gas_addl_fields: List[str] = field(default_factory=list)
     separate_output_tables: bool = False
+    use_value_curve_name_for_join: bool = False
 
     @staticmethod
     def from_file(config_file):
         data = toml.load(config_file)
         db = data.get("database", dict())
         run_info = data.get("run", dict())
         return FLEXValueConfig(
@@ -88,14 +89,15 @@
             process_gas_av_costs=run_info.get("process_gas_av_costs", None),
             process_metered_load_shape=run_info.get("process_metered_load_shape", None),
             elec_components=run_info.get("elec_components", []),
             gas_components=run_info.get("gas_components", []),
             separate_output_tables=run_info.get("separate_output_tables", None),
             elec_addl_fields=run_info.get("elec_addl_fields", []),
             gas_addl_fields=run_info.get("gas_addl_fields", []),
+            use_value_curve_name_for_join=run_info.get("join_on_value_curve_name", None)
         )
 
     def validate(self):
         if not self.database_type:
             return
         if self.database_type == "postgresql":
             if not any(
```

### Comparing `flexvalue-2.0.5/flexvalue/db.py` & `flexvalue-2.0.6/flexvalue/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,22 +58,24 @@
     "units",
     "eul",
     "ntg",
     "discount_rate",
     "admin_cost",
     "measure_cost",
     "incentive_cost",
+    "value_curve_name"
 ]
 ELEC_AV_COSTS_FIELDS = [
     "utility",
     "region",
     "year",
     "hour_of_year",
     "total",
     "marginal_ghg",
+    "value_curve_name"
 ]
 GAS_AV_COSTS_FIELDS = [
     "state",
     "utility",
     "region",
     "year",
     "quarter",
@@ -81,14 +83,15 @@
     "market",
     "t_d",
     "environment",
     "btm_methane",
     "total",
     "upstream_methane",
     "marginal_ghg",
+    "value_curve_name"
 ]
 ELEC_AVOIDED_COSTS_FIELDS = [
     "state",
     "utility",
     "region",
     "datetime",
     "year",
@@ -105,14 +108,15 @@
     "cap_and_trade",
     "ghg_adder",
     "ghg_rebalancing",
     "methane_leakage",
     "total",
     "marginal_ghg",
     "ghg_adder_rebalancing",
+    "value_curve_name"
 ]
 
 logging.basicConfig(
     stream=sys.stderr, format="%(levelname)s:%(message)s", level=logging.INFO
 )
 
 # This is the number of bytes to read when determining whether a csv file has
@@ -323,15 +327,15 @@
                 sql = self._file_to_string(sql_filepath)
                 _ = conn.execute(text(sql))
             for index_filepath in index_filepaths:
                 sql = self._file_to_string(index_filepath)
                 _ = conn.execute(text(sql))
         if truncate:
             self._reset_table(table_name)
-
+        
     def _prepare_table_from_str(
         self,
         table_name: str,
         create_table_sql: str,
         index_filepaths=[],
         truncate: bool = False,
     ):
@@ -476,14 +480,15 @@
             "els_table": "elec_load_shape",
             "gac_table": "gas_av_costs",
             "therms_profile_table": "therms_profile",
             "float_type": self.config.float_type(),
             "database_type": self.config.database_type,
             "elec_components": self._elec_components(),
             "gas_components": self._gas_components(),
+            "use_value_curve_name_for_join": self.config.use_value_curve_name_for_join
         }
         if mode == "electric":
             context["elec_aggregation_columns"] = elec_agg_columns
             context["elec_addl_fields"] = elec_addl_fields
         elif mode == "gas":
             context["gas_aggregation_columns"] = gas_agg_columns
             context["gas_addl_fields"] = gas_addl_fields
@@ -692,15 +697,16 @@
                     datetime,
                     market,
                     t_d,
                     environment,
                     btm_methane,
                     total,
                     upstream_methane,
-                    marginal_ghg)
+                    marginal_ghg,
+                    value_curve_name)
                     FROM STDIN"""
             ) as copy:
                 for row in rows:
                     copy.write_row(row)
 
         self._prepare_table("gas_av_costs", "flexvalue/sql/create_gas_av_cost.sql")
         MAX_ROWS = 10000
@@ -732,14 +738,15 @@
                             float(r["market"]),
                             float(r["t_d"]),
                             float(r["environment"]),
                             float(r["btm_methane"]),
                             float(r["total"]),
                             float(r["upstream_methane"]),
                             float(r["marginal_ghg"]),
+                            r["value_curve_name"],
                         ]
                     )
                     if len(buf) == MAX_ROWS:
                         copy_write(cur, buf)
                         buf = []
                 else:
                     copy_write(cur, buf)
@@ -768,15 +775,16 @@
                     distribution,
                     cap_and_trade,
                     ghg_adder,
                     ghg_rebalancing,
                     methane_leakage,
                     total,
                     marginal_ghg,
-                    ghg_adder_rebalancing)
+                    ghg_adder_rebalancing,
+                    value_curve_name)
                     FROM STDIN"""
             ) as copy:
                 for row in rows:
                     copy.write_row(row)
 
         self._prepare_table(
             "elec_av_costs",
@@ -816,14 +824,15 @@
                             r["cap_and_trade"],
                             r["ghg_adder"],
                             r["ghg_rebalancing"],
                             r["methane_leakage"],
                             float(r["total"]),
                             r["marginal_ghg"],
                             r["ghg_adder_rebalancing"],
+                            r["value_curve_name"],
                         ]
                     )
                     if len(buf) == MAX_ROWS:
                         copy_write(cur, buf)
                         buf = []
                 else:
                     copy_write(cur, buf)
@@ -943,15 +952,15 @@
         self.connection.commit()
 
     def _load_project_info_data(self, insert_text, project_info_dicts):
         """insert_text isn't needed for postgresql"""
 
         def copy_write(cur, rows):
             with cur.copy(
-                "COPY project_info (id, state, utility, region, mwh_savings, therms_savings, load_shape, therms_profile, start_year, start_quarter, start_date, end_date, units, eul, ntg, discount_rate, admin_cost, measure_cost, incentive_cost ) FROM STDIN"
+                "COPY project_info (id, state, utility, region, mwh_savings, therms_savings, load_shape, therms_profile, start_year, start_quarter, start_date, end_date, units, eul, ntg, discount_rate, admin_cost, measure_cost, incentive_cost, value_curve_name) FROM STDIN"
             ) as copy:
                 for row in rows:
                     copy.write_row(row)
 
         rows = [
             (
                 x["id"],
@@ -969,14 +978,15 @@
                 x["units"],
                 x["eul"],
                 x["ntg"],
                 x["discount_rate"],
                 x["admin_cost"],
                 x["measure_cost"],
                 x["incentive_cost"],
+                x["value_curve_name"],
             )
             for x in project_info_dicts
         ]
         cursor = self.connection.cursor()
         copy_write(cursor, rows)
         self.connection.commit()
 
@@ -1239,14 +1249,15 @@
             "els_table": self._elec_load_shape_for_context(),
             "gac_table": self.config.gas_av_costs_table,
             "therms_profile_table": self._therms_profile_for_context(),
             "float_type": self.config.float_type(),
             "database_type": self.config.database_type,
             "elec_components": self._elec_components(),
             "gas_components": self._gas_components(),
+            "use_value_curve_name_for_join": self.config.use_value_curve_name_for_join
         }
         if mode == "electric":
             context["elec_aggregation_columns"] = elec_agg_columns
             context["elec_addl_fields"] = elec_addl_fields
         elif mode == "gas":
             context["gas_aggregation_columns"] = gas_agg_columns
             context["gas_addl_fields"] = gas_addl_fields
@@ -1322,10 +1333,7 @@
             pass
 
     def _exec_select_sql(self, sql: str):
         # This is just here to support testing
         query_job = self.client.query(sql)
         result = query_job.result()
         return [x for x in result]
-
-    def _select_as_df(self, sql: str):
-        return self.client.query(sql).to_dataframe()
```

### Comparing `flexvalue-2.0.5/flexvalue/examples.py` & `flexvalue-2.0.6/flexvalue/examples.py`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.5/flexvalue/flexvalue.py` & `flexvalue-2.0.6/flexvalue/flexvalue.py`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.5/flexvalue/settings.py` & `flexvalue-2.0.6/flexvalue/settings.py`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.5/flexvalue/sql/create_elec_av_cost.sql` & `flexvalue-2.0.6/flexvalue/sql/create_elec_av_cost.sql`

 * *Files 17% similar despite different names*

```diff
@@ -18,9 +18,10 @@
     distribution FLOAT,
     cap_and_trade FLOAT,
     ghg_adder FLOAT,
     ghg_rebalancing FLOAT,
     methane_leakage FLOAT,
     total FLOAT,
     marginal_ghg FLOAT,
-    ghg_adder_rebalancing FLOAT
+    ghg_adder_rebalancing FLOAT,
+    value_curve_name TEXT
 );
```

### Comparing `flexvalue-2.0.5/flexvalue/sql/postgres_indexes.sql` & `flexvalue-2.0.6/flexvalue/sql/postgres_indexes.sql`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.5/flexvalue/templates/bq_populate_elec_load_shape.sql` & `flexvalue-2.0.6/flexvalue/templates/bq_populate_elec_load_shape.sql`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.5/flexvalue/templates/bq_populate_metered_load_shape.sql` & `flexvalue-2.0.6/flexvalue/templates/bq_populate_metered_load_shape.sql`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.5/flexvalue/templates/bq_populate_therms_profile.sql` & `flexvalue-2.0.6/flexvalue/templates/bq_populate_therms_profile.sql`

 * *Files identical despite different names*

### Comparing `flexvalue-2.0.5/flexvalue/templates/calculation.sql` & `flexvalue-2.0.6/flexvalue/templates/calculation.sql`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,21 @@
         elec_av_costs.energy, elec_av_costs.losses, elec_av_costs.ancillary_services,
         elec_av_costs.capacity, elec_av_costs.transmission, elec_av_costs.distribution,
         elec_av_costs.cap_and_trade, elec_av_costs.ghg_adder, elec_av_costs.ghg_rebalancing,
         elec_av_costs.methane_leakage, elec_av_costs.total, elec_av_costs.marginal_ghg,
         elec_av_costs.ghg_adder_rebalancing,
         1.0 / POW(1.0 + (project_costs.discount_rate / 4.0), ((elec_av_costs.year - project_costs.start_year) * 4) + elec_av_costs.quarter - project_costs.start_quarter) AS discount
     FROM project_costs
-    JOIN {{ eac_table }} elec_av_costs
+    JOIN
+        {{ eac_table }} elec_av_costs
         ON elec_av_costs.utility = project_costs.utility
             AND elec_av_costs.region = project_costs.region
+            {% if use_value_curve_name_for_join -%}
+            AND elec_av_costs.value_curve_name = project_costs.value_curve_name
+            {% endif -%}
             {% if database_type == "postgresql" -%}
             AND elec_av_costs.datetime >= make_timestamp(project_costs.start_year, (project_costs.start_quarter - 1) * 3 + 1, 1, 0, 0, 0)
             AND elec_av_costs.datetime < make_timestamp(project_costs.start_year, (project_costs.start_quarter - 1) * 3 + 1, 1, 0, 0, 0) + make_interval(project_costs.eul)
             {% else -%}
             AND elec_av_costs.datetime >= CAST(DATE(project_costs.start_year, (project_costs.start_quarter - 1) * 3 + 1, 1) AS DATETIME)
             AND elec_av_costs.datetime < CAST(DATE(CAST(project_costs.start_year + project_costs.eul AS INT), (project_costs.start_quarter - 1) * 3 + 1, 1) AS DATETIME)
             {% endif -%}
@@ -53,39 +57,45 @@
     {% endif -%}
     {% endfor -%}
     , SUM(pcwdea.units * pcwdea.ntg * pcwdea.mwh_savings * elec_load_shape.value) / CAST(pcwdea.eul AS {{ float_type }}) as annual_net_mwh_savings
     , MAX(pcwdea.trc_costs) AS trc_costs
     , MAX(pcwdea.pac_costs) AS pac_costs
     , SUM(pcwdea.units * pcwdea.ntg * pcwdea.mwh_savings * elec_load_shape.value) as lifecycle_net_mwh_savings
     , SUM(pcwdea.units * pcwdea.ntg * pcwdea.mwh_savings * elec_load_shape.value * pcwdea.marginal_ghg) as lifecycle_elec_ghg_savings
-    {% for addl_field in elec_addl_fields -%}
-    , pcwdea.{{ addl_field }}
+    {% for field in elec_addl_fields if not field == "datetime" -%}
+    , pcwdea.{{ field }}
     {% endfor -%}
     FROM project_costs_with_discounted_elec_av pcwdea
     JOIN {{ els_table }} elec_load_shape
         ON UPPER(elec_load_shape.load_shape_name) = UPPER(pcwdea.load_shape)
             AND elec_load_shape.utility = pcwdea.utility
             AND elec_load_shape.hour_of_year = pcwdea.hour_of_year
     GROUP BY pcwdea.id, pcwdea.eul, pcwdea.datetime, elec_load_shape.load_shape_name
-    {% for field in elec_addl_fields %}, pcwdea.{{ field }}{% endfor -%}
+    {% for field in elec_addl_fields if not field == "datetime" -%}
+    , pcwdea.{{ field }}
+    {% endfor -%}
     {%- for column in elec_aggregation_columns -%}, pcwdea.{{ column }}{% endfor -%}
 )
 , project_costs_with_discounted_gas_av AS (
     SELECT
         project_costs.*
         , gas_av_costs.year
         , gas_av_costs.month
         , gas_av_costs.quarter
         , gas_av_costs.total, gas_av_costs.market, gas_av_costs.t_d
         , gas_av_costs.environment, gas_av_costs.btm_methane, gas_av_costs.upstream_methane, gas_av_costs.marginal_ghg
         , 1.0 / POW(1.0 + (project_costs.discount_rate / 4.0), ((gas_av_costs.year - project_costs.start_year) * 4) + gas_av_costs.quarter - project_costs.start_quarter) AS discount
         , gas_av_costs.datetime
     FROM project_costs
-    JOIN {{ gac_table }} gas_av_costs
+    JOIN 
+      {{ gac_table }} gas_av_costs
         ON gas_av_costs.utility = project_costs.utility
+            {% if use_value_curve_name_for_join -%}
+            AND gas_av_costs.value_curve_name = project_costs.value_curve_name
+            {% endif -%}
             {% if database_type == "postgresql" -%}
             AND gas_av_costs.datetime >= make_timestamp(project_costs.start_year, (project_costs.start_quarter - 1) * 3 + 1, 1, 0, 0, 0)
             AND gas_av_costs.datetime < make_timestamp(project_costs.start_year, (project_costs.start_quarter - 1) * 3 + 1, 1, 0, 0, 0) + make_interval(project_costs.eul)
             {% else -%}
             AND gas_av_costs.datetime >= CAST(DATE(project_costs.start_year, (project_costs.start_quarter - 1) * 3 + 1, 1) AS DATETIME)
             AND gas_av_costs.datetime < CAST(DATE(CAST(project_costs.start_year + project_costs.eul AS INT), (project_costs.start_quarter - 1) * 3 + 1, 1) AS DATETIME)
             {% endif -%}
@@ -96,25 +106,25 @@
     , MAX(pcwdga.trc_costs) as trc_costs
     , MAX(pcwdga.pac_costs) as pac_costs
     {% for column in gas_aggregation_columns -%}
     , pcwdga.{{ column }}
     {% endfor -%}
     , SUM(pcwdga.units * pcwdga.ntg * pcwdga.therms_savings * therms_profile.value * pcwdga.discount * pcwdga.total) as gas_benefits
     , SUM((pcwdga.units * pcwdga.therms_savings * pcwdga.ntg * therms_profile.value) / CAST(pcwdga.eul AS {{ float_type }}) ) as annual_net_therms_savings
-    , SUM(pcwdga.units * pcwdga.therms_savings * pcwdga.ntg * therms_profile.value) as lifecyle_net_therms_savings
+    , SUM(pcwdga.units * pcwdga.therms_savings * pcwdga.ntg * therms_profile.value) as lifecycle_net_therms_savings
     , SUM(pcwdga.units * pcwdga.therms_savings * pcwdga.ntg * therms_profile.value * pcwdga.marginal_ghg) as lifecycle_gas_ghg_savings
     {% for component in gas_components -%}
     {% if component == 'marginal_ghg' %}
     , SUM(pcwdga.units * pcwdga.ntg * pcwdga.therms_savings * therms_profile.value * pcwdga.{{component}}) as {{component}}
     {% else %}
     , SUM(pcwdga.units * pcwdga.ntg * pcwdga.therms_savings * therms_profile.value * pcwdga.discount * pcwdga.{{component}}) as {{component}}
     {% endif %}
     {% endfor -%}
-    {% for addl_field in gas_addl_fields -%}
-    , pcwdga.{{ addl_field }}
+    {% for field in gas_addl_fields -%}
+    , pcwdga.{{ field }}
     {% endfor -%}
     , pcwdga.datetime
     FROM project_costs_with_discounted_gas_av pcwdga
     JOIN {{ therms_profile_table }} therms_profile
         ON UPPER(pcwdga.therms_profile) = UPPER(therms_profile.profile_name)
             AND therms_profile.utility = pcwdga.utility
             AND therms_profile.month = pcwdga.month
@@ -182,29 +192,29 @@
 , COALESCE(SUM(gas_calculations.gas_benefits), 0) as gas_benefits
 , SUM(COALESCE(elec_calculations.electric_benefits, 0)) + SUM(COALESCE(gas_calculations.gas_benefits, 0)) as total_benefits
 , MAX(COALESCE(elec_calculations.trc_costs, gas_calculations.trc_costs)) as trc_costs
 , MAX(COALESCE(elec_calculations.pac_costs, gas_calculations.pac_costs)) as pac_costs
 , COALESCE(SUM(elec_calculations.annual_net_mwh_savings), 0) as annual_net_mwh_savings
 , COALESCE(SUM(elec_calculations.lifecycle_net_mwh_savings), 0) as lifecycle_net_mwh_savings
 , COALESCE(SUM(gas_calculations.annual_net_therms_savings), 0) as annual_net_therms_savings
-, COALESCE(SUM(gas_calculations.lifecyle_net_therms_savings), 0) as lifecyle_net_therms_savings
+, COALESCE(SUM(gas_calculations.lifecycle_net_therms_savings), 0) as lifecycle_net_therms_savings
 , COALESCE(SUM(elec_calculations.lifecycle_elec_ghg_savings), 0) as lifecycle_elec_ghg_savings
 , COALESCE(SUM(gas_calculations.lifecycle_gas_ghg_savings), 0) as lifecycle_gas_ghg_savings
 , SUM(COALESCE(elec_calculations.lifecycle_elec_ghg_savings, 0)) + SUM(COALESCE(gas_calculations.lifecycle_gas_ghg_savings, 0)) as lifecycle_total_ghg_savings
 {% for column in elec_aggregation_columns -%}
 , elec_calculations.{{ column }} as elec_{{ column }}
 {% endfor -%}
 {% for column in gas_aggregation_columns -%}
 , gas_calculations.{{ column }} as gas_{{ column }}
 {% endfor -%}
-{% for addl_field in elec_addl_fields -%}
-, elec_calculations.{{ addl_field }}
+{% for field in elec_addl_fields -%}
+, elec_calculations.{{ field }}
 {% endfor -%}
-{% for addl_field in gas_addl_fields -%}
-, gas_calculations.{{ addl_field }}
+{% for field in gas_addl_fields -%}
+, gas_calculations.{{ field }}
 {% endfor -%}
 {% for comp in elec_components -%}
 , COALESCE(SUM(elec_calculations.{{comp}}), 0) as {{ comp }}
 {% endfor -%}
 {% for comp in gas_components -%}
 , COALESCE(SUM(gas_calculations.{{comp}}), 0) as {{ comp }}
 {% endfor -%}
```

### Comparing `flexvalue-2.0.5/flexvalue/templates/elec_calculation.sql` & `flexvalue-2.0.6/flexvalue/templates/elec_calculation.sql`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,21 @@
         elec_av_costs.capacity, elec_av_costs.transmission, elec_av_costs.distribution,
         elec_av_costs.cap_and_trade, elec_av_costs.ghg_adder, elec_av_costs.ghg_rebalancing,
         elec_av_costs.methane_leakage, elec_av_costs.total, elec_av_costs.marginal_ghg,
         elec_av_costs.ghg_adder_rebalancing,
         1.0 / POW(1.0 + (project_costs.discount_rate / 4.0), ((elec_av_costs.year - project_costs.start_year) * 4) + elec_av_costs.quarter - project_costs.start_quarter) AS discount
         , ((elec_av_costs.year - project_costs.start_year) * 4) + elec_av_costs.quarter - project_costs.start_quarter + 1 as eul_quarter
     FROM project_costs
-    JOIN {{ eac_table }} elec_av_costs
+    JOIN 
+        {{ eac_table }} elec_av_costs
         ON elec_av_costs.utility = project_costs.utility
             AND elec_av_costs.region = project_costs.region
+            {% if use_value_curve_name_for_join -%}
+            AND elec_av_costs.value_curve_name = project_costs.value_curve_name
+            {% endif -%}
             {% if database_type == "postgresql" -%}
             AND elec_av_costs.datetime >= make_timestamp(project_costs.start_year, (project_costs.start_quarter - 1) * 3 + 1, 1, 0, 0, 0)
             AND elec_av_costs.datetime < make_timestamp(project_costs.start_year, (project_costs.start_quarter - 1) * 3 + 1, 1, 0, 0, 0) + make_interval(project_costs.eul)
             {% else %}
             AND elec_av_costs.datetime >= CAST(DATE(project_costs.start_year, (project_costs.start_quarter - 1) * 3 + 1, 1) AS DATETIME)
             AND elec_av_costs.datetime < CAST(DATE(CAST(project_costs.start_year + project_costs.eul AS INT), (project_costs.start_quarter - 1) * 3 + 1, 1) AS DATETIME)
             {% endif -%}
@@ -55,15 +59,15 @@
     {% endfor -%}
     , SUM(pcwdea.units * pcwdea.ntg * pcwdea.mwh_savings * elec_load_shape.value) / CAST(pcwdea.eul AS {{ float_type }}) as annual_net_mwh_savings
     , SUM(pcwdea.units * pcwdea.ntg * pcwdea.mwh_savings * elec_load_shape.value) as lifecycle_net_mwh_savings
     , MAX(pcwdea.trc_costs) AS trc_costs
     , MAX(pcwdea.pac_costs) AS pac_costs
     , SUM(pcwdea.units * pcwdea.ntg * pcwdea.mwh_savings * elec_load_shape.value * pcwdea.marginal_ghg) as lifecycle_elec_ghg_savings
     {% for field in elec_addl_fields if not field == "datetime" -%}
-    , pcwdea.{{field}}
+    , pcwdea.{{ field }}
     {% endfor -%}
     FROM project_costs_with_discounted_elec_av pcwdea
     JOIN {{ els_table}} elec_load_shape
         ON UPPER(elec_load_shape.load_shape_name) = UPPER(pcwdea.load_shape)
             AND elec_load_shape.utility = pcwdea.utility
             AND elec_load_shape.hour_of_year = pcwdea.hour_of_year
     GROUP BY pcwdea.id, pcwdea.eul, pcwdea.datetime, elec_load_shape.load_shape_name
```

### Comparing `flexvalue-2.0.5/flexvalue/templates/gas_calculation.sql` & `flexvalue-2.0.6/flexvalue/templates/gas_calculation.sql`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,20 @@
         , gas_av_costs.quarter
         , gas_av_costs.total, gas_av_costs.market, gas_av_costs.t_d
         , gas_av_costs.environment, gas_av_costs.btm_methane, gas_av_costs.upstream_methane, gas_av_costs.marginal_ghg
         , 1.0 / POW(1.0 + (project_costs.discount_rate / 4.0), ((gas_av_costs.year - project_costs.start_year) * 4) + gas_av_costs.quarter - project_costs.start_quarter) AS discount
         , ((gas_av_costs.year - project_costs.start_year) * 4) + gas_av_costs.quarter - project_costs.start_quarter + 1 as eul_quarter
         , gas_av_costs.datetime
     FROM project_costs
-    JOIN {{ gac_table }} gas_av_costs
+    JOIN 
+      {{ gac_table }} gas_av_costs
         ON gas_av_costs.utility = project_costs.utility
+            {% if use_value_curve_name_for_join -%}
+            AND gas_av_costs.value_curve_name = project_costs.value_curve_name
+            {% endif -%}
             {% if database_type == "postgresql" %}
             AND gas_av_costs.datetime >= make_timestamp(project_costs.start_year, (project_costs.start_quarter - 1) * 3 + 1, 1, 0, 0, 0)
             AND gas_av_costs.datetime < make_timestamp(project_costs.start_year, (project_costs.start_quarter - 1) * 3 + 1, 1, 0, 0, 0) + make_interval(project_costs.eul)
             {% else %}
             AND gas_av_costs.datetime >= CAST(DATE(project_costs.start_year, (project_costs.start_quarter - 1) * 3 + 1, 1) AS DATETIME)
             AND gas_av_costs.datetime < CAST(DATE(CAST(project_costs.start_year + project_costs.eul AS INT), (project_costs.start_quarter - 1) * 3 + 1, 1) AS DATETIME)
             {% endif %}
@@ -35,15 +39,15 @@
     SELECT pcwdga.id
     , pcwdga.total
     {% for column in gas_aggregation_columns -%}
     , pcwdga.{{ column }}
     {% endfor -%}
     , SUM(pcwdga.units * pcwdga.ntg * pcwdga.therms_savings * therms_profile.value * pcwdga.discount * pcwdga.total) as gas_benefits
     , SUM((pcwdga.units * pcwdga.therms_savings * pcwdga.ntg * therms_profile.value) / CAST(pcwdga.eul AS {{ float_type }}) ) as annual_net_therms_savings
-    , SUM(pcwdga.units * pcwdga.therms_savings * pcwdga.ntg * therms_profile.value) as lifecyle_net_therms_savings
+    , SUM(pcwdga.units * pcwdga.therms_savings * pcwdga.ntg * therms_profile.value) as lifecycle_net_therms_savings
     , SUM(pcwdga.units * pcwdga.therms_savings * pcwdga.ntg * therms_profile.value * pcwdga.marginal_ghg) as lifecycle_gas_ghg_savings
     , therms_profile.value as therms_profile_value
     , MAX(pcwdga.trc_costs) AS trc_costs
     , MAX(pcwdga.pac_costs) AS pac_costs
     {% for component in gas_components -%}
     {% if component == 'marginal_ghg' %}
     , SUM(pcwdga.units * pcwdga.ntg * pcwdga.therms_savings * therms_profile.value * pcwdga.{{component}}) as {{component}}
@@ -86,15 +90,15 @@
 , IF (MAX(gas_calculations.trc_costs) = 0, IF(SUM(gas_calculations.gas_benefits) > 0, cast("inf" as {{ float_type }}), cast("-inf" as {{ float_type }})), SUM(gas_calculations.gas_benefits) / MAX(gas_calculations.trc_costs)) as trc_ratio
 , IF (MAX(gas_calculations.pac_costs) = 0, IF(SUM(gas_calculations.gas_benefits) > 0, cast("inf" as {{ float_type }}), cast("-inf" as {{ float_type }})), SUM(gas_calculations.gas_benefits) / MAX(gas_calculations.pac_costs)) as pac_ratio
 {% endif -%}
 , SUM(gas_calculations.gas_benefits) as gas_benefits
 , MAX(gas_calculations.trc_costs) as trc_costs
 , MAX(gas_calculations.pac_costs) as pac_costs
 , SUM(gas_calculations.annual_net_therms_savings) as annual_net_therms_savings
-, SUM(gas_calculations.lifecyle_net_therms_savings) as lifecyle_net_therms_savings
+, SUM(gas_calculations.lifecycle_net_therms_savings) as lifecycle_net_therms_savings
 , MAX(gas_calculations.therms_profile_value) as therms_profile_value
 , SUM(gas_calculations.lifecycle_gas_ghg_savings) as lifecycle_gas_ghg_savings
 {% for field in gas_addl_fields -%}
 , gas_calculations.{{ field }}
 {% endfor -%}
 {% for column in gas_aggregation_columns -%}
 , gas_calculations.{{ column }}
```

### Comparing `flexvalue-2.0.5/flexvalue/templates/load_elec_av_costs.sql` & `flexvalue-2.0.6/flexvalue/templates/load_elec_av_costs.sql`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+-- sqlite only - will need to be updated
 INSERT INTO elec_av_costs (
 	state,
     utility,
     region,
     date_time,
     year,
     quarter,
@@ -17,10 +18,11 @@
     distribution,
     cap_and_trade,
     ghg_adder,
     ghg_rebalancing,
     methane_leakage,
     total,
     marginal_ghg,
-    ghg_adder_rebalancing
-) VALUES ( :state, :utility, :region, :datetime, :year, :quarter, :month, :date_str, :hour_of_day, :hour_of_year, :energy, :losses, :ancillary_services, :capacity, :transmission, :distribution, :cap_and_trade, :ghg_adder, :ghg_rebalancing, :methane_leakage, :total, :marginal_ghg, :ghg_adder_rebalancing
+    ghg_adder_rebalancing,
+    value_curve_name
+) VALUES ( :state, :utility, :region, :datetime, :year, :quarter, :month, :date_str, :hour_of_day, :hour_of_year, :energy, :losses, :ancillary_services, :capacity, :transmission, :distribution, :cap_and_trade, :ghg_adder, :ghg_rebalancing, :methane_leakage, :total, :marginal_ghg, :ghg_adder_rebalancing, :value_curve_name
 )
```

### Comparing `flexvalue-2.0.5/flexvalue/templates/load_project_info.sql` & `flexvalue-2.0.6/flexvalue/templates/load_project_info.sql`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     end_date,
     units,
     eul,
     ntg,
     discount_rate,
     admin_cost,
     measure_cost,
-    incentive_cost
+    incentive_cost,
+    value_curve_name
 )
 VALUES (
     :id, :state, :utility, :region, :mwh_savings, :therms_savings,
     :load_shape, :therms_profile, :start_year, :start_quarter,
     :start_date, :end_date, :units, :eul, :ntg, :discount_rate, :admin_cost,
-    :measure_cost, :incentive_cost
+    :measure_cost, :incentive_cost, :value_curve_name
 )
```

### Comparing `flexvalue-2.0.5/flexvalue.egg-info/PKG-INFO` & `flexvalue-2.0.6/flexvalue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: flexvalue
-Version: 2.0.5
+Version: 2.0.6
 Summary: FLEXvalue: a tool for calculating avoided costs
 Home-page: http://github.com/recurve-methods/flexvalue
 Author: Recurve Analytics, Inc.
 Author-email: support@recurve.com
 License: Apache 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `flexvalue-2.0.5/flexvalue.egg-info/SOURCES.txt` & `flexvalue-2.0.6/flexvalue.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 README.rst
 setup.cfg
 setup.py
 flexvalue/__init__.py
 flexvalue/__version__.py
-flexvalue/cet_flexvalue_compare.py
 flexvalue/cli.py
 flexvalue/config.py
 flexvalue/db.py
 flexvalue/examples.py
 flexvalue/flexvalue.py
-flexvalue/report.py
 flexvalue/settings.py
 flexvalue.egg-info/PKG-INFO
 flexvalue.egg-info/SOURCES.txt
 flexvalue.egg-info/dependency_links.txt
 flexvalue.egg-info/entry_points.txt
 flexvalue.egg-info/requires.txt
 flexvalue.egg-info/top_level.txt
```

### Comparing `flexvalue-2.0.5/setup.py` & `flexvalue-2.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,29 +29,20 @@
 
 from setuptools import find_packages, setup, Command
 
 NAME = "flexvalue"
 
 # TODO: fix psycopg-binary; use correct dependency for distributing
 INSTALL_REQUIRES = [
-    "click==8.0.3",
-    "toml==0.10.2",
-    "pandas==1.3.4",
-    "statsmodels==0.13.1",
-    "scipy==1.7.2",
-    "seaborn==0.11.2",
+    "click>=8.0.0",
+    "toml>=0.10.2",
     "sqlalchemy==2.0",
-    "nbformat==5.1.3",
-    "nbconvert==6.3.0",
     "jinja2==3.0.3",
-    "matplotlib<3.6",
-    "numpy<1.23.0",
     "psycopg[binary]==3.1.8",
-    "google-cloud-bigquery==3.6.0",
-    "db-dtypes>=1.0.5"
+    "google-cloud-bigquery>=2.34.3",
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Load the package's __version__.py module as a dictionary.
 about = {}
 with open(os.path.join(here, NAME, "__version__.py")) as f:
```

