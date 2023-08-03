# Comparing `tmp/cerc-costs-0.1.0.2.tar.gz` & `tmp/cerc-costs-0.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerc-costs-0.1.0.2.tar", last modified: Tue Jul 25 15:37:49 2023, max compression
+gzip compressed data, was "cerc-costs-0.1.0.3.tar", last modified: Thu Aug  3 13:47:41 2023, max compression
```

## Comparing `cerc-costs-0.1.0.2.tar` & `cerc-costs-0.1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-07-25 15:37:49.422087 cerc-costs-0.1.0.2/
--rw-r--r--   0 jenkins    (109) jenkins    (117)      386 2023-07-25 15:37:49.422087 cerc-costs-0.1.0.2/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (117)      754 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/README.md
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-07-25 15:37:49.418087 cerc-costs-0.1.0.2/cerc_costs.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (117)      386 2023-07-25 15:37:49.000000 cerc-costs-0.1.0.2/cerc_costs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (117)      517 2023-07-25 15:37:49.000000 cerc-costs-0.1.0.2/cerc_costs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)        1 2023-07-25 15:37:49.000000 cerc-costs-0.1.0.2/cerc_costs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)       43 2023-07-25 15:37:49.000000 cerc-costs-0.1.0.2/cerc_costs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)        6 2023-07-25 15:37:49.000000 cerc-costs-0.1.0.2/cerc_costs.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-07-25 15:37:49.418087 cerc-costs-0.1.0.2/costs/
--rw-r--r--   0 jenkins    (109) jenkins    (117)      596 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/costs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      243 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/costs/__main__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    11799 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/costs/capital_costs.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5238 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/costs/configuration.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      572 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/costs/constants.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     6625 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/costs/cost.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1443 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/costs/cost_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1439 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/costs/end_of_life_costs.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2434 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/costs/peak_load.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2327 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/costs/total_maintenance_costs.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4651 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/costs/total_operational_costs.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1792 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/costs/total_operational_incomes.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      344 2023-07-25 15:36:46.000000 cerc-costs-0.1.0.2/costs/version.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      166 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/pyproject.toml
--rw-r--r--   0 jenkins    (109) jenkins    (117)       31 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/requirements.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)       38 2023-07-25 15:37:49.422087 cerc-costs-0.1.0.2/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1018 2023-07-25 13:57:23.000000 cerc-costs-0.1.0.2/setup.py
+drwxr-xr-x   0 guille    (1000) guille    (1000)        0 2023-08-03 13:47:41.223380 cerc-costs-0.1.0.3/
+-rw-r--r--   0 guille    (1000) guille    (1000)      386 2023-08-03 13:47:41.223380 cerc-costs-0.1.0.3/PKG-INFO
+-rw-r--r--   0 guille    (1000) guille    (1000)      754 2023-07-21 17:44:55.000000 cerc-costs-0.1.0.3/README.md
+drwxr-xr-x   0 guille    (1000) guille    (1000)        0 2023-08-03 13:47:41.219380 cerc-costs-0.1.0.3/cerc_costs.egg-info/
+-rw-r--r--   0 guille    (1000) guille    (1000)      386 2023-08-03 13:47:41.000000 cerc-costs-0.1.0.3/cerc_costs.egg-info/PKG-INFO
+-rw-r--r--   0 guille    (1000) guille    (1000)      517 2023-08-03 13:47:41.000000 cerc-costs-0.1.0.3/cerc_costs.egg-info/SOURCES.txt
+-rw-r--r--   0 guille    (1000) guille    (1000)        1 2023-08-03 13:47:41.000000 cerc-costs-0.1.0.3/cerc_costs.egg-info/dependency_links.txt
+-rw-r--r--   0 guille    (1000) guille    (1000)       43 2023-08-03 13:47:41.000000 cerc-costs-0.1.0.3/cerc_costs.egg-info/requires.txt
+-rw-r--r--   0 guille    (1000) guille    (1000)        6 2023-08-03 13:47:41.000000 cerc-costs-0.1.0.3/cerc_costs.egg-info/top_level.txt
+drwxr-xr-x   0 guille    (1000) guille    (1000)        0 2023-08-03 13:47:41.223380 cerc-costs-0.1.0.3/costs/
+-rw-r--r--   0 guille    (1000) guille    (1000)      596 2023-07-21 17:44:55.000000 cerc-costs-0.1.0.3/costs/__init__.py
+-rw-r--r--   0 guille    (1000) guille    (1000)      243 2023-07-21 17:44:55.000000 cerc-costs-0.1.0.3/costs/__main__.py
+-rw-r--r--   0 guille    (1000) guille    (1000)    11726 2023-08-02 14:34:54.000000 cerc-costs-0.1.0.3/costs/capital_costs.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     5238 2023-07-21 17:44:55.000000 cerc-costs-0.1.0.3/costs/configuration.py
+-rw-r--r--   0 guille    (1000) guille    (1000)      572 2023-07-21 17:44:55.000000 cerc-costs-0.1.0.3/costs/constants.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     6360 2023-08-02 14:34:54.000000 cerc-costs-0.1.0.3/costs/cost.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     1384 2023-08-02 14:34:54.000000 cerc-costs-0.1.0.3/costs/cost_base.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     1439 2023-07-21 17:44:55.000000 cerc-costs-0.1.0.3/costs/end_of_life_costs.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     1911 2023-08-02 14:34:54.000000 cerc-costs-0.1.0.3/costs/peak_load.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     2327 2023-07-21 17:44:55.000000 cerc-costs-0.1.0.3/costs/total_maintenance_costs.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     4899 2023-08-02 14:34:54.000000 cerc-costs-0.1.0.3/costs/total_operational_costs.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     1792 2023-07-21 17:44:55.000000 cerc-costs-0.1.0.3/costs/total_operational_incomes.py
+-rw-r--r--   0 guille    (1000) guille    (1000)      344 2023-08-03 13:42:15.000000 cerc-costs-0.1.0.3/costs/version.py
+-rw-r--r--   0 guille    (1000) guille    (1000)      166 2023-07-21 17:44:55.000000 cerc-costs-0.1.0.3/pyproject.toml
+-rw-r--r--   0 guille    (1000) guille    (1000)       31 2023-07-21 17:44:55.000000 cerc-costs-0.1.0.3/requirements.txt
+-rw-r--r--   0 guille    (1000) guille    (1000)       38 2023-08-03 13:47:41.223380 cerc-costs-0.1.0.3/setup.cfg
+-rw-r--r--   0 guille    (1000) guille    (1000)     1018 2023-07-21 17:44:55.000000 cerc-costs-0.1.0.3/setup.py
```

### Comparing `cerc-costs-0.1.0.2/README.md` & `cerc-costs-0.1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cerc-costs-0.1.0.2/cerc_costs.egg-info/SOURCES.txt` & `cerc-costs-0.1.0.3/cerc_costs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cerc-costs-0.1.0.2/costs/__init__.py` & `cerc-costs-0.1.0.3/costs/__init__.py`

 * *Files identical despite different names*

### Comparing `cerc-costs-0.1.0.2/costs/capital_costs.py` & `cerc-costs-0.1.0.3/costs/capital_costs.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,24 +77,23 @@
     capital_cost_roof = 0
     capital_cost_heating_equipment = 0
     capital_cost_cooling_equipment = 0
     capital_cost_distribution_equipment = 0
     capital_cost_other_hvac_ahu = 0
     capital_cost_lighting = 0
 
-    for internal_zone in self._building.internal_zones:
-      for thermal_zone in internal_zone.thermal_zones:
-        for thermal_boundary in thermal_zone.thermal_boundaries:
-          if thermal_boundary.type == 'Ground':
-            surface_ground += thermal_boundary.opaque_area
-          elif thermal_boundary.type == 'Roof':
-            surface_roof += thermal_boundary.opaque_area
-          elif thermal_boundary.type == 'Wall':
-            surface_opaque += thermal_boundary.opaque_area * (1 - thermal_boundary.window_ratio)
-            surface_transparent += thermal_boundary.opaque_area * thermal_boundary.window_ratio
+    for thermal_zone in self._building.thermal_zones:
+      for thermal_boundary in thermal_zone.thermal_boundaries:
+        if thermal_boundary.type == 'Ground':
+          surface_ground += thermal_boundary.opaque_area
+        elif thermal_boundary.type == 'Roof':
+          surface_roof += thermal_boundary.opaque_area
+        elif thermal_boundary.type == 'Wall':
+          surface_opaque += thermal_boundary.opaque_area * (1 - thermal_boundary.window_ratio)
+          surface_transparent += thermal_boundary.opaque_area * thermal_boundary.window_ratio
 
     peak_heating = self._building.heating_peak_load[cte.YEAR][0] / 1000
     peak_cooling = self._building.cooling_peak_load[cte.YEAR][0] / 1000
 
     surface_pv = 0
     for roof in self._building.roofs:
       surface_pv += roof.solid_polygon.area * roof.solar_collectors_area_reduction_factor
```

### Comparing `cerc-costs-0.1.0.2/costs/configuration.py` & `cerc-costs-0.1.0.3/costs/configuration.py`

 * *Files identical despite different names*

### Comparing `cerc-costs-0.1.0.2/costs/constants.py` & `cerc-costs-0.1.0.3/costs/constants.py`

 * *Files identical despite different names*

### Comparing `cerc-costs-0.1.0.2/costs/cost.py` & `cerc-costs-0.1.0.3/costs/cost.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,21 +58,14 @@
   @property
   def building(self) -> Building:
     """
     Get current building.
     """
     return self._building
 
-  @building.setter
-  def building(self, value: Building):
-    """
-    Set current building.
-    """
-    self._building = value
-
   def _npv_from_list(self, list_cashflow):
     return npf.npv(self._configuration.discount_rate, list_cashflow)
 
   @property
   def life_cycle(self) -> pd.DataFrame:
     """
     Get complete life cycle costs
@@ -99,16 +92,14 @@
         global_capital_costs['D301010_photovoltaic_system']
     )
 
     df_end_of_life_costs = global_end_of_life_costs['End_of_life_costs']
     df_operational_costs = (
         global_operational_costs['Fixed_costs_electricity_peak'] +
         global_operational_costs['Fixed_costs_electricity_monthly'] +
-        global_operational_costs['Fixed_costs_electricity_peak'] +
-        global_operational_costs['Fixed_costs_electricity_monthly'] +
         global_operational_costs['Variable_costs_electricity'] +
         global_operational_costs['Fixed_costs_gas'] +
         global_operational_costs['Variable_costs_gas']
     )
     df_maintenance_costs = (
         global_maintenance_costs['Heating_maintenance'] +
         global_maintenance_costs['Cooling_maintenance'] +
```

### Comparing `cerc-costs-0.1.0.2/costs/cost_base.py` & `cerc-costs-0.1.0.3/costs/cost_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,16 @@
   """
   Abstract base class for the costs
   """
   def __init__(self, building: Building, configuration: Configuration):
     self._building = building
     self._configuration = configuration
     self._total_floor_area = 0
-    for internal_zone in building.internal_zones:
-      for thermal_zone in internal_zone.thermal_zones:
-        self._total_floor_area += thermal_zone.total_floor_area
+    for thermal_zone in building.thermal_zones:
+      self._total_floor_area += thermal_zone.total_floor_area
     self._archetype = None
     self._capital_costs_chapter = None
     for archetype in self._configuration.costs_catalog.entries().archetypes:
       if configuration.dictionary[str(building.function)] == str(archetype.function):
         self._archetype = archetype
         self._capital_costs_chapter = self._archetype.capital_cost
         break
```

### Comparing `cerc-costs-0.1.0.2/costs/end_of_life_costs.py` & `cerc-costs-0.1.0.3/costs/end_of_life_costs.py`

 * *Files identical despite different names*

### Comparing `cerc-costs-0.1.0.2/costs/peak_load.py` & `cerc-costs-0.1.0.3/costs/peak_load.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,36 +30,24 @@
     for system in self._building.energy_systems:
       for demand_type in system.demand_types:
         if demand_type == cte.HEATING:
           heating = 1
         if demand_type == cte.COOLING:
           cooling = 1
     if cte.MONTH in self._building.heating_peak_load.keys() and cte.MONTH in self._building.cooling_peak_load.keys():
-      peak_lighting = 0
-      peak_appliances = 0
-      for thermal_zone in self._building.internal_zones[0].thermal_zones:
-        lighting = thermal_zone.lighting
-        for schedule in lighting.schedules:
-          peak = max(schedule.values) * lighting.density * thermal_zone.total_floor_area
-          if peak > peak_lighting:
-            peak_lighting = peak
-        appliances = thermal_zone.appliances
-        for schedule in appliances.schedules:
-          peak = max(schedule.values) * appliances.density * thermal_zone.total_floor_area
-          if peak > peak_appliances:
-            peak_appliances = peak
+      peak_lighting = self._building.lighting_peak_load[cte.YEAR][0]
+      peak_appliances = self._building.appliances_peak_load[cte.YEAR][0]
       monthly_electricity_peak = [0.9 * peak_lighting + 0.7 * peak_appliances] * 12
       conditioning_peak = []
       for i, value in enumerate(self._building.heating_peak_load[cte.MONTH]):
         if cooling * self._building.cooling_peak_load[cte.MONTH][i] > heating * value:
           conditioning_peak.append(cooling * self._building.cooling_peak_load[cte.MONTH][i])
         else:
           conditioning_peak.append(heating * value)
         monthly_electricity_peak[i] += 0.8 * conditioning_peak[i]
       electricity_peak_load_results = pd.DataFrame(
         monthly_electricity_peak,
-        columns=[f'{self._building.name} electricity peak load W']
+        columns=[f'electricity peak load W']
       )
     else:
-      electricity_peak_load_results = pd.DataFrame(array, columns=[f'{self._building.name} electricity peak load W'])
-
+      electricity_peak_load_results = pd.DataFrame(array, columns=[f'electricity peak load W'])
     return electricity_peak_load_results
```

### Comparing `cerc-costs-0.1.0.2/costs/total_maintenance_costs.py` & `cerc-costs-0.1.0.3/costs/total_maintenance_costs.py`

 * *Files identical despite different names*

### Comparing `cerc-costs-0.1.0.2/costs/total_operational_costs.py` & `cerc-costs-0.1.0.3/costs/total_operational_costs.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,16 +81,20 @@
       price_increase_gas = math.pow(1 + self._configuration.gas_price_index, year)
       self._yearly_operational_costs.at[year, 'Fixed_costs_electricity_peak'] = (
           peak_electricity_cost_year_0 * price_increase_peak_electricity
       )
       self._yearly_operational_costs.at[year, 'Fixed_costs_electricity_monthly'] = (
           monthly_electricity_cost_year_0 * price_increase_peak_electricity
       )
+      if not isinstance(variable_electricity_cost_year_0, pd.DataFrame):
+        variable_costs_electricity = variable_electricity_cost_year_0 * price_increase_electricity
+      else:
+        variable_costs_electricity = float(variable_electricity_cost_year_0.iloc[0] * price_increase_electricity)
       self._yearly_operational_costs.at[year, 'Variable_costs_electricity'] = (
-        float(variable_electricity_cost_year_0.iloc[0] * price_increase_electricity)
+        variable_costs_electricity
       )
       self._yearly_operational_costs.at[year, 'Fixed_costs_gas'] = fixed_gas_cost_year_0 * price_increase_gas
       self._yearly_operational_costs.at[year, 'Variable_costs_gas'] = (
           variable_gas_cost_year_0 * price_increase_peak_electricity
       )
       self._yearly_operational_costs.at[year, 'Variable_costs_gas'] = (
           variable_gas_cost_year_0 * price_increase_peak_electricity
```

### Comparing `cerc-costs-0.1.0.2/costs/total_operational_incomes.py` & `cerc-costs-0.1.0.3/costs/total_operational_incomes.py`

 * *Files identical despite different names*

### Comparing `cerc-costs-0.1.0.2/setup.py` & `cerc-costs-0.1.0.3/setup.py`

 * *Files identical despite different names*

