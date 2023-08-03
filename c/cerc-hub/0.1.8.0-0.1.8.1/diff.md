# Comparing `tmp/cerc-hub-0.1.8.0.tar.gz` & `tmp/cerc-hub-0.1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerc-hub-0.1.8.0.tar", last modified: Wed Aug  2 19:57:44 2023, max compression
+gzip compressed data, was "cerc-hub-0.1.8.1.tar", last modified: Thu Aug  3 16:10:04 2023, max compression
```

## Comparing `cerc-hub-0.1.8.0.tar` & `cerc-hub-0.1.8.1.tar`

### file list

```diff
@@ -1,376 +1,377 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.076760 cerc-hub-0.1.8.0/
--rw-r--r--   0 jenkins    (109) jenkins    (117)      828 2023-08-02 19:57:44.076760 cerc-hub-0.1.8.0/PKG-INFO
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.012760 cerc-hub-0.1.8.0/cerc_hub.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (117)       32 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/cerc_hub.egg-info/.gitignore
--rw-r--r--   0 jenkins    (109) jenkins    (117)      828 2023-08-02 19:57:43.000000 cerc-hub-0.1.8.0/cerc_hub.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (117)    14377 2023-08-02 19:57:44.000000 cerc-hub-0.1.8.0/cerc_hub.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)        1 2023-08-02 19:57:43.000000 cerc-hub-0.1.8.0/cerc_hub.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)      263 2023-08-02 19:57:43.000000 cerc-hub-0.1.8.0/cerc_hub.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)        4 2023-08-02 19:57:43.000000 cerc-hub-0.1.8.0/cerc_hub.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.012760 cerc-hub-0.1.8.0/hub/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.012760 cerc-hub-0.1.8.0/hub/catalog_factories/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      870 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/catalog.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.012760 cerc-hub-0.1.8.0/hub/catalog_factories/construction/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/construction/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1701 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/construction/construction_helper.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10136 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/construction/eilat_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10217 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/construction/nrcan_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10304 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/construction/nrel_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1507 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/construction_catalog_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.012760 cerc-hub-0.1.8.0/hub/catalog_factories/cost/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/cost/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     8566 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/cost/montreal_custom_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1044 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/costs_catalog_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.012760 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.012760 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/construction/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/construction/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4634 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/construction/archetype.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2057 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/construction/construction.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1370 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/construction/content.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1298 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/construction/layer.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3187 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/construction/material.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1728 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/construction/window.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.012760 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3180 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/archetype.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1801 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/capital_cost.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1320 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/chapter.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      951 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/content.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1938 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/fuel.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2185 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/income.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2612 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/item_description.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2132 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/operational_cost.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.016760 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/energy_systems/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/energy_systems/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1269 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/energy_systems/archetype.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1624 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/energy_systems/content.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2701 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/energy_systems/distribution_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1389 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/energy_systems/emission_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3804 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/energy_systems/generation_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2942 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/energy_systems/system.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.016760 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/greenery/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/greenery/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1164 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/greenery/content.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2912 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/greenery/plant.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1494 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/greenery/plant_percentage.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3584 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/greenery/soil.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5825 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/greenery/vegetation.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.016760 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2071 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/appliances.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      873 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/content.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1879 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/domestic_hot_water.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2053 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/lighting.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2547 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/occupancy.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2225 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/schedule.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3578 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/thermal_control.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4088 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/usage.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.016760 cerc-hub-0.1.8.0/hub/catalog_factories/energy_systems/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/energy_systems/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    11133 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/energy_systems/montreal_custom_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1201 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/energy_systems_catalog_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.016760 cerc-hub-0.1.8.0/hub/catalog_factories/greenery/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/greenery/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.016760 cerc-hub-0.1.8.0/hub/catalog_factories/greenery/ecore_greenery/
--rw-r--r--   0 jenkins    (109) jenkins    (117)    19314 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.ecore
--rw-r--r--   0 jenkins    (109) jenkins    (117)    12388 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    18684 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog_no_quantities.ecore
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4564 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/greenery/greenery_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1107 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/greenery_catalog_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.016760 cerc-hub-0.1.8.0/hub/catalog_factories/usage/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/usage/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10095 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/usage/comnet_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10017 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/usage/eilat_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10380 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/usage/nrcan_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4425 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/usage/usage_helper.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1516 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/catalog_factories/usage_catalog_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.016760 cerc-hub-0.1.8.0/hub/city_model_structure/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.020760 cerc-hub-0.1.8.0/hub/city_model_structure/attributes/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/attributes/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      935 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/attributes/edge.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1194 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/attributes/node.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1929 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/attributes/plane.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      843 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/attributes/point.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    13218 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/attributes/polygon.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     6590 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/attributes/polyhedron.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      763 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/attributes/record.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2922 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/attributes/schedule.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      770 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/attributes/time_series.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    26423 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.020760 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2359 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/appliances.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2052 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/domestic_hot_water.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      650 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/household.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3009 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/internal_gain.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2895 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/internal_zone.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1259 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/layer.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2349 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/lighting.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4070 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/material.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2865 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/occupancy.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3090 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/storey.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    11228 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/surface.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     9018 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/thermal_boundary.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4622 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/thermal_control.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5277 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/thermal_opening.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    24514 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/thermal_zone.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7848 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/usage.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      957 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/buildings_cluster.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1385 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/bus_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    16886 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/city.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     8101 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/city_object.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1638 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/city_objects_cluster.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1613 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_system.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.020760 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3237 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/air_source_hp.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      570 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/control_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      918 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/distribution_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      841 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/emission_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3526 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/energy_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2693 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/generation_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2665 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/generic_distribution_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      775 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/generic_emission_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2577 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/generic_energy_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3996 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/generic_generation_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1508 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/heat_pump.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1115 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/hvac_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      709 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/hvac_terminal_unit.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3093 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/water_to_water_hp.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.024760 cerc-hub-0.1.8.0/hub/city_model_structure/greenery/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/greenery/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2304 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/greenery/plant.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3288 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/greenery/soil.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1630 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/greenery/vegetation.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.024760 cerc-hub-0.1.8.0/hub/city_model_structure/iot/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/iot/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1503 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/iot/sensor.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      867 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/iot/sensor_measure.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      462 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/iot/sensor_type.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      943 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/iot/station.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2502 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/level_of_detail.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1195 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/network.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      974 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/parts_consisting_building.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.024760 cerc-hub-0.1.8.0/hub/city_model_structure/transport/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2403 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/bus.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      880 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/bus_depot.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1045 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/bus_edge.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      970 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/bus_network.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1154 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/bus_node.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1494 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/bus_stop.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2616 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/connection.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1775 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/crossing.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      821 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/join.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3285 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/lane.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1251 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/origin_destination_edge.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1141 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/origin_destination_network.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2159 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/origin_destination_node.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3173 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/phase.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3542 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/traffic_edge.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1877 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/traffic_light.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1080 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/traffic_network.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2186 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/traffic_node.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      965 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/city_model_structure/transport/walkway_node.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.032760 cerc-hub-0.1.8.0/hub/config/
--rw-r--r--   0 jenkins    (109) jenkins    (117)      629 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/config/configuration.ini
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.008760 cerc-hub-0.1.8.0/hub/data/
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.032760 cerc-hub-0.1.8.0/hub/data/construction/
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3280 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/construction/eilat_archetypes.json
--rw-r--r--   0 jenkins    (109) jenkins    (117)    73899 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/construction/eilat_constructions.json
--rw-r--r--   0 jenkins    (109) jenkins    (117)  1894214 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/construction/nrcan_archetypes.json
--rw-r--r--   0 jenkins    (109) jenkins    (117)   274471 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/construction/nrcan_constructions.json
--rw-r--r--   0 jenkins    (109) jenkins    (117)    44638 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/construction/us_archetypes.xml
--rw-r--r--   0 jenkins    (109) jenkins    (117)    32891 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/construction/us_constructions.xml
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.032760 cerc-hub-0.1.8.0/hub/data/costs/
--rw-r--r--   0 jenkins    (109) jenkins    (117)    11017 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/costs/montreal_costs.xml
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.032760 cerc-hub-0.1.8.0/hub/data/customized_imports/
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3228 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/customized_imports/ashrae_archetypes.xml
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.032760 cerc-hub-0.1.8.0/hub/data/energy_systems/
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.036760 cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/
--rw-r--r--   0 jenkins    (109) jenkins    (117)   105875 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/air_source.xlsx
--rw-r--r--   0 jenkins    (109) jenkins    (117)    11051 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/as_parallel.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10802 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/as_series.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)      446 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/constants.yaml
--rw-r--r--   0 jenkins    (109) jenkins    (117)  1040664 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/demand.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10820 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/w2w_parallel.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10411 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/w2w_series.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)    73906 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/water_to_water.xlsx
--rw-r--r--   0 jenkins    (109) jenkins    (117)   257760 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/wt_hourly3.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)    18850 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/energy_systems/montreal_custom_systems.xml
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.036760 cerc-hub-0.1.8.0/hub/data/geolocation/
--rw-r--r--   0 jenkins    (109) jenkins    (117)  2219196 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/geolocation/admin2Codes.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)  6284352 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/geolocation/cities15000.txt
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.040760 cerc-hub-0.1.8.0/hub/data/greenery/
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5044 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/greenery/ecore_greenery_catalog.xml
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.044760 cerc-hub-0.1.8.0/hub/data/usage/
--rw-r--r--   0 jenkins    (109) jenkins    (117)   299386 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/usage/comnet_archetypes.xlsx
--rw-r--r--   0 jenkins    (109) jenkins    (117)   348793 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/usage/comnet_schedules_archetypes.xlsx
--rw-r--r--   0 jenkins    (109) jenkins    (117)    15170 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/usage/eilat_archetypes.xlsx
--rw-r--r--   0 jenkins    (109) jenkins    (117)    78312 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/usage/eilat_schedules_archetypes.xlsx
--rw-r--r--   0 jenkins    (109) jenkins    (117)      398 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/usage/nrcan.xml
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.008760 cerc-hub-0.1.8.0/hub/data/weather/
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.044760 cerc-hub-0.1.8.0/hub/data/weather/epw/
--rw-r--r--   0 jenkins    (109) jenkins    (117)  1588401 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/data/weather/epw/CAN_PQ_Montreal.Intl.AP.716270_CWEC.epw
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.044760 cerc-hub-0.1.8.0/hub/exports/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.044760 cerc-hub-0.1.8.0/hub/exports/building_energy/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/building_energy/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    17060 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/building_energy/energy_ade.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    35617 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/building_energy/idf.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.064760 cerc-hub-0.1.8.0/hub/exports/building_energy/idf_files/
--rw-r--r--   0 jenkins    (109) jenkins    (117)  4241609 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/building_energy/idf_files/Energy+.idd
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7428 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/building_energy/idf_files/Minimal.idf
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.064760 cerc-hub-0.1.8.0/hub/exports/building_energy/insel/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/building_energy/insel/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    13413 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/building_energy/insel/insel_monthly_energy_balance.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2814 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/energy_building_exports_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.064760 cerc-hub-0.1.8.0/hub/exports/energy_systems/
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2379 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/energy_systems/air_source_hp_export.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    12750 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/energy_systems/heat_pump_export.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2228 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/energy_systems/water_to_water_hp_export.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2238 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/energy_systems_factory.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1918 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/exports_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.064760 cerc-hub-0.1.8.0/hub/exports/formats/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/formats/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1737 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/formats/obj.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4828 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/formats/simplified_radiosity_algorithm.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      398 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/formats/stl.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1069 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/exports/formats/triangular.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.064760 cerc-hub-0.1.8.0/hub/helpers/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      766 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/auth.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4765 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/configuration_helper.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     6128 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/constants.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.068760 cerc-hub-0.1.8.0/hub/helpers/data/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     9183 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/alkis_function_to_hub_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      694 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/eilat_function_to_hub_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1039 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/hft_function_to_hub_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      710 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/hub_function_to_eilat_construction_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3266 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/hub_function_to_montreal_custom_costs_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2980 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/hub_function_to_nrcan_construction_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3006 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/hub_function_to_nrel_construction_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3213 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/hub_usage_to_comnet_usage.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      630 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/hub_usage_to_eilat_usage.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3178 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/hub_usage_to_hft_usage.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3228 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/hub_usage_to_nrcan_usage.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      635 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/montreal_custom_fuel_to_hub_fuel.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      813 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/montreal_demand_type_to_hub_energy_demand_type.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    31279 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/montreal_function_to_hub_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2155 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/montreal_system_to_hub_energy_generation_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     6408 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/data/pluto_function_to_hub_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5351 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/dictionaries.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    12422 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/geometry_helper.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      729 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/location.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1632 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/monthly_values.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.068760 cerc-hub-0.1.8.0/hub/helpers/peak_calculation/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/peak_calculation/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     6723 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/peak_calculation/loads_calculation.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4985 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/peak_loads.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      883 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/helpers/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.068760 cerc-hub-0.1.8.0/hub/imports/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.068760 cerc-hub-0.1.8.0/hub/imports/construction/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/construction/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    11083 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/construction/eilat_physics_parameters.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.068760 cerc-hub-0.1.8.0/hub/imports/construction/helpers/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/construction/helpers/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2425 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/construction/helpers/construction_helper.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7447 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/construction/helpers/storeys_generation.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10727 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/construction/nrcan_physics_parameters.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     9906 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/construction/nrel_physics_parameters.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1916 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/construction_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.068760 cerc-hub-0.1.8.0/hub/imports/energy_systems/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/energy_systems/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5582 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/energy_systems/air_source_hp_parameters.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.068760 cerc-hub-0.1.8.0/hub/imports/energy_systems/helpers/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/energy_systems/helpers/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      679 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/energy_systems/helpers/energy_systems_helper.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7609 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/energy_systems/montreal_custom_energy_system_parameters.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     6552 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/energy_systems/water_to_water_hp_parameters.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2217 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/energy_systems_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.072760 cerc-hub-0.1.8.0/hub/imports/geometry/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/geometry/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7933 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/geometry/citygml.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.072760 cerc-hub-0.1.8.0/hub/imports/geometry/citygml_classes/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/geometry/citygml_classes/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      792 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/geometry/citygml_classes/citygml_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2358 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/geometry/citygml_classes/citygml_lod1.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3409 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/geometry/citygml_classes/citygml_lod2.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    14539 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/geometry/geojson.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3944 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/geometry/gpandas.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.072760 cerc-hub-0.1.8.0/hub/imports/geometry/helpers/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/geometry/helpers/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3258 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/geometry/helpers/geometry_helper.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2936 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/geometry/obj.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2676 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/geometry_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.072760 cerc-hub-0.1.8.0/hub/imports/results/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/results/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1432 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/results/insel_heatpump_energy_demand.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5454 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/results/insel_monthly_energry_balance.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3874 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/results/simplified_radiosity_algorithm.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2129 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/results_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.072760 cerc-hub-0.1.8.0/hub/imports/usage/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/usage/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10941 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/usage/comnet_usage_parameters.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10929 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/usage/eilat_usage_parameters.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     9313 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/usage/nrcan_usage_parameters.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1894 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/usage_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.072760 cerc-hub-0.1.8.0/hub/imports/weather/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/weather/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     9545 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/weather/epw_weather_parameters.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.072760 cerc-hub-0.1.8.0/hub/imports/weather/helpers/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/weather/helpers/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5749 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/weather/helpers/weather.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1204 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/imports/weather_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.072760 cerc-hub-0.1.8.0/hub/persistence/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1941 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/configuration.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     9318 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/db_control.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2942 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/db_setup.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.072760 cerc-hub-0.1.8.0/hub/persistence/models/
--rw-r--r--   0 jenkins    (109) jenkins    (117)      203 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/models/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1039 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/models/application.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1235 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/models/city.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2811 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/models/city_object.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1177 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/models/simulation_results.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1129 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/models/user.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.072760 cerc-hub-0.1.8.0/hub/persistence/repositories/
--rw-r--r--   0 jenkins    (109) jenkins    (117)       29 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/repositories/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3574 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/repositories/application.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4441 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/repositories/city.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4733 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/repositories/city_object.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     6022 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/repositories/simulation_results.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5087 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/repositories/user.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      772 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/persistence/repository.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)       51 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/hub/version.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      164 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/pyproject.toml
--rw-r--r--   0 jenkins    (109) jenkins    (117)      251 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/requirements.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)       38 2023-08-02 19:57:44.076760 cerc-hub-0.1.8.0/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5290 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/setup.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-02 19:57:44.076760 cerc-hub-0.1.8.0/tests/
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5014 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_city_merge.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2734 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_construction_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    17918 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_construction_factory.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      938 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_costs_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7637 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_custom_insel_block.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    13088 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_db_factory.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2684 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_energy_systems_air_source_hp.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2497 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_energy_systems_water_to_water_hp.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7368 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_enrichement.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4942 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_exports.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     9903 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_geometry_factory.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1339 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_greenery_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3225 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_greenery_in_idf.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3007 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_heat_pump_results.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7571 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_insel_exports.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4434 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_results_import.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1471 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_systems_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5817 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_systems_factory.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      819 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_usage_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    11500 2023-08-02 19:55:47.000000 cerc-hub-0.1.8.0/tests/test_usage_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.603414 cerc-hub-0.1.8.1/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      828 2023-08-03 16:10:04.603414 cerc-hub-0.1.8.1/PKG-INFO
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.567414 cerc-hub-0.1.8.1/cerc_hub.egg-info/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)       32 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/cerc_hub.egg-info/.gitignore
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      828 2023-08-03 16:10:04.000000 cerc-hub-0.1.8.1/cerc_hub.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    14403 2023-08-03 16:10:04.000000 cerc-hub-0.1.8.1/cerc_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        1 2023-08-03 16:10:04.000000 cerc-hub-0.1.8.1/cerc_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      263 2023-08-03 16:10:04.000000 cerc-hub-0.1.8.1/cerc_hub.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        4 2023-08-03 16:10:04.000000 cerc-hub-0.1.8.1/cerc_hub.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.567414 cerc-hub-0.1.8.1/hub/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.567414 cerc-hub-0.1.8.1/hub/catalog_factories/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      870 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/catalog.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.567414 cerc-hub-0.1.8.1/hub/catalog_factories/construction/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/construction/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1701 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/construction/construction_helper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10136 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/construction/eilat_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10217 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/construction/nrcan_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10304 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/construction/nrel_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1507 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/construction_catalog_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.567414 cerc-hub-0.1.8.1/hub/catalog_factories/cost/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/cost/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     8566 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/cost/montreal_custom_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1044 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/costs_catalog_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.567414 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.571414 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/construction/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/construction/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4634 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/construction/archetype.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2057 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/construction/construction.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1370 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/construction/content.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1298 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/construction/layer.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3187 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/construction/material.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1728 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/construction/window.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.571414 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3180 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/archetype.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1801 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/capital_cost.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1320 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/chapter.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      951 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/content.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1938 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/fuel.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2185 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/income.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2612 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/item_description.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2132 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/operational_cost.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.571414 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/energy_systems/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/energy_systems/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1269 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/energy_systems/archetype.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1624 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/energy_systems/content.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2701 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/energy_systems/distribution_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1389 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/energy_systems/emission_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3804 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/energy_systems/generation_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2942 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/energy_systems/system.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.571414 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/greenery/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/greenery/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1164 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/greenery/content.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2912 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/greenery/plant.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1494 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/greenery/plant_percentage.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3584 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/greenery/soil.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5825 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/greenery/vegetation.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.571414 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2071 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/appliances.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      873 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/content.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1879 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/domestic_hot_water.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2053 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/lighting.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2547 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/occupancy.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2225 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/schedule.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3578 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/thermal_control.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4088 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/usage.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.571414 cerc-hub-0.1.8.1/hub/catalog_factories/energy_systems/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/energy_systems/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    11133 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/energy_systems/montreal_custom_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1201 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/energy_systems_catalog_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.571414 cerc-hub-0.1.8.1/hub/catalog_factories/greenery/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/greenery/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.571414 cerc-hub-0.1.8.1/hub/catalog_factories/greenery/ecore_greenery/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    19314 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.ecore
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    12388 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    18684 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog_no_quantities.ecore
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4564 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/greenery/greenery_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1107 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/greenery_catalog_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.571414 cerc-hub-0.1.8.1/hub/catalog_factories/usage/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/usage/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10095 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/usage/comnet_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10017 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/usage/eilat_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10380 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/usage/nrcan_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4425 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/usage/usage_helper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1516 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/catalog_factories/usage_catalog_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.575414 cerc-hub-0.1.8.1/hub/city_model_structure/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.575414 cerc-hub-0.1.8.1/hub/city_model_structure/attributes/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/attributes/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      935 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/attributes/edge.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1194 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/attributes/node.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1929 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/attributes/plane.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      843 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/attributes/point.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    13218 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/attributes/polygon.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     6590 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/attributes/polyhedron.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      763 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/attributes/record.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2922 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/attributes/schedule.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      770 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/attributes/time_series.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    26423 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.575414 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2359 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/appliances.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2052 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/domestic_hot_water.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      650 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/household.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3009 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/internal_gain.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2895 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/internal_zone.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1259 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/layer.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2349 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/lighting.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4070 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/material.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2865 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/occupancy.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3090 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/storey.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    11228 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/surface.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     9018 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/thermal_boundary.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4622 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/thermal_control.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5277 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/thermal_opening.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    24514 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/thermal_zone.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7848 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/usage.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      957 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/buildings_cluster.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1385 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/bus_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    16886 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/city.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     8101 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/city_object.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1638 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/city_objects_cluster.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1613 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_system.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.575414 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3237 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/air_source_hp.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      570 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/control_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      918 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/distribution_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      841 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/emission_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3526 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/energy_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2693 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/generation_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2665 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/generic_distribution_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      775 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/generic_emission_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2577 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/generic_energy_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3996 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/generic_generation_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1508 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/heat_pump.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1115 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/hvac_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      709 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/hvac_terminal_unit.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3093 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/water_to_water_hp.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.579414 cerc-hub-0.1.8.1/hub/city_model_structure/greenery/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/greenery/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2304 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/greenery/plant.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3288 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/greenery/soil.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1630 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/greenery/vegetation.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.579414 cerc-hub-0.1.8.1/hub/city_model_structure/iot/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/iot/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1503 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/iot/sensor.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      867 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/iot/sensor_measure.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      462 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/iot/sensor_type.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      943 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/iot/station.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2502 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/level_of_detail.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1195 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/network.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      974 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/parts_consisting_building.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.579414 cerc-hub-0.1.8.1/hub/city_model_structure/transport/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2403 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/bus.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      880 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/bus_depot.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1045 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/bus_edge.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      970 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/bus_network.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1154 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/bus_node.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1494 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/bus_stop.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2616 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/connection.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1775 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/crossing.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      821 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/join.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3285 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/lane.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1251 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/origin_destination_edge.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1141 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/origin_destination_network.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2159 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/origin_destination_node.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3173 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/phase.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3542 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/traffic_edge.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1877 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/traffic_light.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1080 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/traffic_network.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2186 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/traffic_node.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      965 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/city_model_structure/transport/walkway_node.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.579414 cerc-hub-0.1.8.1/hub/config/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      629 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/config/configuration.ini
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.567414 cerc-hub-0.1.8.1/hub/data/
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.579414 cerc-hub-0.1.8.1/hub/data/construction/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3280 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/construction/eilat_archetypes.json
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    73899 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/construction/eilat_constructions.json
+-rw-r--r--   0 jenkins    (109) jenkins    (117)  1894214 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/construction/nrcan_archetypes.json
+-rw-r--r--   0 jenkins    (109) jenkins    (117)   274471 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/construction/nrcan_constructions.json
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    44638 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/construction/us_archetypes.xml
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    32891 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/construction/us_constructions.xml
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.583414 cerc-hub-0.1.8.1/hub/data/costs/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    11017 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/costs/montreal_costs.xml
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.583414 cerc-hub-0.1.8.1/hub/data/customized_imports/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3228 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/customized_imports/ashrae_archetypes.xml
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.583414 cerc-hub-0.1.8.1/hub/data/energy_systems/
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.583414 cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)   105875 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/air_source.xlsx
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    11051 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/as_parallel.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10802 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/as_series.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      446 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/constants.yaml
+-rw-r--r--   0 jenkins    (109) jenkins    (117)  1040664 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/demand.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10820 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/w2w_parallel.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10411 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/w2w_series.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    73906 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/water_to_water.xlsx
+-rw-r--r--   0 jenkins    (109) jenkins    (117)   257760 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/wt_hourly3.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    18850 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/energy_systems/montreal_custom_systems.xml
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.583414 cerc-hub-0.1.8.1/hub/data/geolocation/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)  2219196 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/geolocation/admin2Codes.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)  6284352 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/geolocation/cities15000.txt
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.587414 cerc-hub-0.1.8.1/hub/data/greenery/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5044 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/greenery/ecore_greenery_catalog.xml
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.591414 cerc-hub-0.1.8.1/hub/data/usage/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)   299386 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/usage/comnet_archetypes.xlsx
+-rw-r--r--   0 jenkins    (109) jenkins    (117)   348793 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/usage/comnet_schedules_archetypes.xlsx
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    15170 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/usage/eilat_archetypes.xlsx
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    78312 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/usage/eilat_schedules_archetypes.xlsx
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      398 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/usage/nrcan.xml
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.567414 cerc-hub-0.1.8.1/hub/data/weather/
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.591414 cerc-hub-0.1.8.1/hub/data/weather/epw/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)  1588401 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/data/weather/epw/CAN_PQ_Montreal.Intl.AP.716270_CWEC.epw
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.591414 cerc-hub-0.1.8.1/hub/exports/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.591414 cerc-hub-0.1.8.1/hub/exports/building_energy/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/building_energy/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    17060 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/building_energy/energy_ade.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    35617 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/building_energy/idf.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.595414 cerc-hub-0.1.8.1/hub/exports/building_energy/idf_files/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)  4241609 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/building_energy/idf_files/Energy+.idd
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7428 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/building_energy/idf_files/Minimal.idf
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.595414 cerc-hub-0.1.8.1/hub/exports/building_energy/insel/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/building_energy/insel/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    13413 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/building_energy/insel/insel_monthly_energy_balance.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2814 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/energy_building_exports_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.595414 cerc-hub-0.1.8.1/hub/exports/energy_systems/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2379 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/energy_systems/air_source_hp_export.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    12750 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/energy_systems/heat_pump_export.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2228 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/energy_systems/water_to_water_hp_export.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2238 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/energy_systems_factory.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1918 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/exports_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.595414 cerc-hub-0.1.8.1/hub/exports/formats/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/formats/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1737 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/formats/obj.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4828 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/formats/simplified_radiosity_algorithm.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      398 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/formats/stl.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1069 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/exports/formats/triangular.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.595414 cerc-hub-0.1.8.1/hub/helpers/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      766 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/auth.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4765 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/configuration_helper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     6128 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/constants.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.595414 cerc-hub-0.1.8.1/hub/helpers/data/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     9183 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/alkis_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      694 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/eilat_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1039 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/hft_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      710 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/hub_function_to_eilat_construction_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3266 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/hub_function_to_montreal_custom_costs_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2980 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/hub_function_to_nrcan_construction_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3006 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/hub_function_to_nrel_construction_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3213 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/hub_usage_to_comnet_usage.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      630 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/hub_usage_to_eilat_usage.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3178 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/hub_usage_to_hft_usage.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3228 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/hub_usage_to_nrcan_usage.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      635 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/montreal_custom_fuel_to_hub_fuel.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      813 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/montreal_demand_type_to_hub_energy_demand_type.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    31279 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/montreal_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2155 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/montreal_system_to_hub_energy_generation_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     6408 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/data/pluto_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5351 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/dictionaries.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    12422 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/geometry_helper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      729 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/location.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1632 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/monthly_values.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.595414 cerc-hub-0.1.8.1/hub/helpers/peak_calculation/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/peak_calculation/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     6723 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/peak_calculation/loads_calculation.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4985 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/peak_loads.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      883 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/helpers/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.595414 cerc-hub-0.1.8.1/hub/imports/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.599414 cerc-hub-0.1.8.1/hub/imports/construction/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/construction/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    11083 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/construction/eilat_physics_parameters.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.599414 cerc-hub-0.1.8.1/hub/imports/construction/helpers/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/construction/helpers/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2425 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/construction/helpers/construction_helper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7447 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/construction/helpers/storeys_generation.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10727 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/construction/nrcan_physics_parameters.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     9906 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/construction/nrel_physics_parameters.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1916 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/construction_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.599414 cerc-hub-0.1.8.1/hub/imports/energy_systems/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/energy_systems/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5582 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/energy_systems/air_source_hp_parameters.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.599414 cerc-hub-0.1.8.1/hub/imports/energy_systems/helpers/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/energy_systems/helpers/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      679 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/energy_systems/helpers/energy_systems_helper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7609 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/energy_systems/montreal_custom_energy_system_parameters.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     6552 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/energy_systems/water_to_water_hp_parameters.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2217 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/energy_systems_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.599414 cerc-hub-0.1.8.1/hub/imports/geometry/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/geometry/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7933 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/geometry/citygml.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.599414 cerc-hub-0.1.8.1/hub/imports/geometry/citygml_classes/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/geometry/citygml_classes/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      792 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/geometry/citygml_classes/citygml_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2358 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/geometry/citygml_classes/citygml_lod1.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3409 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/geometry/citygml_classes/citygml_lod2.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    14539 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/geometry/geojson.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3944 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/geometry/gpandas.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.599414 cerc-hub-0.1.8.1/hub/imports/geometry/helpers/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/geometry/helpers/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3258 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/geometry/helpers/geometry_helper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2936 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/geometry/obj.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2676 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/geometry_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.599414 cerc-hub-0.1.8.1/hub/imports/results/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/results/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1432 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/results/insel_heatpump_energy_demand.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5454 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/results/insel_monthly_energry_balance.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3874 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/results/simplified_radiosity_algorithm.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2129 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/results_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.599414 cerc-hub-0.1.8.1/hub/imports/usage/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/usage/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10941 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/usage/comnet_usage_parameters.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10929 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/usage/eilat_usage_parameters.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     9313 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/usage/nrcan_usage_parameters.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1894 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/usage_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.599414 cerc-hub-0.1.8.1/hub/imports/weather/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/weather/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     9545 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/weather/epw_weather_parameters.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.599414 cerc-hub-0.1.8.1/hub/imports/weather/helpers/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/weather/helpers/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5749 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/weather/helpers/weather.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1204 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/imports/weather_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.599414 cerc-hub-0.1.8.1/hub/persistence/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1941 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/configuration.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     9486 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/db_control.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2942 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/db_setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.599414 cerc-hub-0.1.8.1/hub/persistence/models/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      203 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/models/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1039 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/models/application.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1235 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/models/city.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2811 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/models/city_object.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1177 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/models/simulation_results.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1129 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/models/user.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.603414 cerc-hub-0.1.8.1/hub/persistence/repositories/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)       29 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/repositories/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3574 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/repositories/application.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4614 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/repositories/city.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4837 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/repositories/city_object.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     6022 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/repositories/simulation_results.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5087 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/repositories/user.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      772 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/persistence/repository.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)       51 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/hub/version.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      164 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/pyproject.toml
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      251 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/requirements.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)       38 2023-08-03 16:10:04.603414 cerc-hub-0.1.8.1/setup.cfg
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5290 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:10:04.603414 cerc-hub-0.1.8.1/tests/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5014 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_city_merge.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2734 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_construction_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    17918 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_construction_factory.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      938 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_costs_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7637 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_custom_insel_block.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    13088 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_db_factory.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4109 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_db_retrieve.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2684 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_energy_systems_air_source_hp.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2497 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_energy_systems_water_to_water_hp.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7368 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_enrichement.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4942 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_exports.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     9903 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_geometry_factory.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1339 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_greenery_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3225 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_greenery_in_idf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3007 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_heat_pump_results.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7571 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_insel_exports.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4434 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_results_import.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1471 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_systems_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5817 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_systems_factory.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      819 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_usage_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    11500 2023-08-03 16:08:23.000000 cerc-hub-0.1.8.1/tests/test_usage_factory.py
```

### Comparing `cerc-hub-0.1.8.0/PKG-INFO` & `cerc-hub-0.1.8.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-hub
-Version: 0.1.8.0
+Version: 0.1.8.1
 Summary: CERC Hub consist in a set of classes (Central data model), importers and exporters to help researchers to create better and sustainable cities
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 
 CERC Hub consist in a set of classes (Central data model), importers and exporters to help researchers to create better and sustainable cities.
```

### Comparing `cerc-hub-0.1.8.0/cerc_hub.egg-info/PKG-INFO` & `cerc-hub-0.1.8.1/cerc_hub.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-hub
-Version: 0.1.8.0
+Version: 0.1.8.1
 Summary: CERC Hub consist in a set of classes (Central data model), importers and exporters to help researchers to create better and sustainable cities
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 
 CERC Hub consist in a set of classes (Central data model), importers and exporters to help researchers to create better and sustainable cities.
```

### Comparing `cerc-hub-0.1.8.0/cerc_hub.egg-info/SOURCES.txt` & `cerc-hub-0.1.8.1/cerc_hub.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -294,14 +294,15 @@
 hub/persistence/repositories/user.py
 tests/test_city_merge.py
 tests/test_construction_catalog.py
 tests/test_construction_factory.py
 tests/test_costs_catalog.py
 tests/test_custom_insel_block.py
 tests/test_db_factory.py
+tests/test_db_retrieve.py
 tests/test_energy_systems_air_source_hp.py
 tests/test_energy_systems_water_to_water_hp.py
 tests/test_enrichement.py
 tests/test_exports.py
 tests/test_geometry_factory.py
 tests/test_greenery_catalog.py
 tests/test_greenery_in_idf.py
```

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/catalog.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/construction/construction_helper.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/construction/construction_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/construction/eilat_catalog.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/construction/eilat_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/construction/nrcan_catalog.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/construction/nrcan_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/construction/nrel_catalog.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/construction/nrel_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/construction_catalog_factory.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/construction_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/cost/montreal_custom_catalog.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/cost/montreal_custom_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/costs_catalog_factory.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/costs_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/construction/archetype.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/construction/archetype.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/construction/construction.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/construction/construction.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/construction/content.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/construction/content.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/construction/layer.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/construction/layer.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/construction/material.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/construction/material.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/construction/window.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/construction/window.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/archetype.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/archetype.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/capital_cost.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/capital_cost.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/chapter.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/chapter.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/content.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/content.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/fuel.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/fuel.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/income.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/income.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/item_description.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/item_description.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/cost/operational_cost.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/cost/operational_cost.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/energy_systems/archetype.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/energy_systems/archetype.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/energy_systems/content.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/energy_systems/content.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/energy_systems/distribution_system.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/energy_systems/distribution_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/energy_systems/emission_system.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/energy_systems/emission_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/energy_systems/generation_system.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/energy_systems/generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/energy_systems/system.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/energy_systems/system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/greenery/content.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/greenery/content.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/greenery/plant.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/greenery/plant.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/greenery/plant_percentage.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/greenery/plant_percentage.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/greenery/soil.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/greenery/soil.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/greenery/vegetation.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/greenery/vegetation.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/appliances.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/appliances.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/content.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/content.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/domestic_hot_water.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/domestic_hot_water.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/lighting.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/lighting.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/occupancy.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/occupancy.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/schedule.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/schedule.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/thermal_control.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/thermal_control.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/data_models/usages/usage.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/data_models/usages/usage.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/energy_systems/montreal_custom_catalog.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/energy_systems/montreal_custom_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/energy_systems_catalog_factory.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/energy_systems_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.ecore` & `cerc-hub-0.1.8.1/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.ecore`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog_no_quantities.ecore` & `cerc-hub-0.1.8.1/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog_no_quantities.ecore`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/greenery/greenery_catalog.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/greenery/greenery_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/greenery_catalog_factory.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/greenery_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/usage/comnet_catalog.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/usage/comnet_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/usage/eilat_catalog.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/usage/eilat_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/usage/nrcan_catalog.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/usage/nrcan_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/usage/usage_helper.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/usage/usage_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/catalog_factories/usage_catalog_factory.py` & `cerc-hub-0.1.8.1/hub/catalog_factories/usage_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/attributes/edge.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/attributes/edge.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/attributes/node.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/attributes/node.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/attributes/plane.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/attributes/plane.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/attributes/point.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/attributes/point.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/attributes/polygon.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/attributes/polygon.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/attributes/polyhedron.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/attributes/polyhedron.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/attributes/record.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/attributes/record.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/attributes/schedule.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/attributes/schedule.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/attributes/time_series.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/attributes/time_series.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/appliances.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/appliances.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/domestic_hot_water.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/domestic_hot_water.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/household.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/household.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/internal_gain.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/internal_gain.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/internal_zone.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/internal_zone.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/layer.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/layer.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/lighting.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/lighting.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/material.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/material.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/occupancy.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/occupancy.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/storey.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/storey.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/surface.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/surface.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/thermal_boundary.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/thermal_boundary.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/thermal_control.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/thermal_control.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/thermal_opening.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/thermal_opening.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/thermal_zone.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/thermal_zone.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/building_demand/usage.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/building_demand/usage.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/buildings_cluster.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/buildings_cluster.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/bus_system.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/bus_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/city.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/city.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/city_object.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/city_object.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/city_objects_cluster.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/city_objects_cluster.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_system.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/air_source_hp.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/air_source_hp.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/control_system.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/control_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/distribution_system.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/distribution_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/emission_system.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/emission_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/energy_system.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/energy_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/generation_system.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/generic_distribution_system.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/generic_distribution_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/generic_emission_system.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/generic_emission_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/generic_energy_system.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/generic_energy_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/generic_generation_system.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/generic_generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/heat_pump.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/heat_pump.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/hvac_system.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/hvac_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/hvac_terminal_unit.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/hvac_terminal_unit.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/energy_systems/water_to_water_hp.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/energy_systems/water_to_water_hp.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/greenery/plant.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/greenery/plant.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/greenery/soil.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/greenery/soil.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/greenery/vegetation.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/greenery/vegetation.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/iot/sensor.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/iot/sensor.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/iot/sensor_measure.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/iot/sensor_measure.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/iot/station.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/iot/station.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/level_of_detail.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/level_of_detail.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/network.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/network.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/parts_consisting_building.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/parts_consisting_building.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/bus.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/bus.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/bus_depot.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/bus_depot.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/bus_edge.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/bus_edge.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/bus_network.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/bus_network.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/bus_node.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/bus_node.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/bus_stop.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/bus_stop.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/connection.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/connection.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/crossing.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/crossing.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/join.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/join.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/lane.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/lane.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/origin_destination_edge.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/origin_destination_edge.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/origin_destination_network.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/origin_destination_network.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/origin_destination_node.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/origin_destination_node.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/phase.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/phase.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/traffic_edge.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/traffic_edge.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/traffic_light.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/traffic_light.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/traffic_network.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/traffic_network.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/traffic_node.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/traffic_node.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/city_model_structure/transport/walkway_node.py` & `cerc-hub-0.1.8.1/hub/city_model_structure/transport/walkway_node.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/config/configuration.ini` & `cerc-hub-0.1.8.1/hub/config/configuration.ini`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/construction/eilat_archetypes.json` & `cerc-hub-0.1.8.1/hub/data/construction/eilat_archetypes.json`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/construction/eilat_constructions.json` & `cerc-hub-0.1.8.1/hub/data/construction/eilat_constructions.json`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/construction/nrcan_archetypes.json` & `cerc-hub-0.1.8.1/hub/data/construction/nrcan_archetypes.json`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/construction/nrcan_constructions.json` & `cerc-hub-0.1.8.1/hub/data/construction/nrcan_constructions.json`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/construction/us_archetypes.xml` & `cerc-hub-0.1.8.1/hub/data/construction/us_archetypes.xml`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/construction/us_constructions.xml` & `cerc-hub-0.1.8.1/hub/data/construction/us_constructions.xml`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/costs/montreal_costs.xml` & `cerc-hub-0.1.8.1/hub/data/costs/montreal_costs.xml`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/customized_imports/ashrae_archetypes.xml` & `cerc-hub-0.1.8.1/hub/data/customized_imports/ashrae_archetypes.xml`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/air_source.xlsx` & `cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/air_source.xlsx`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/as_parallel.txt` & `cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/as_parallel.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/as_series.txt` & `cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/as_series.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/demand.txt` & `cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/demand.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/w2w_parallel.txt` & `cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/w2w_parallel.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/w2w_series.txt` & `cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/w2w_series.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/water_to_water.xlsx` & `cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/water_to_water.xlsx`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/energy_systems/heat_pumps/wt_hourly3.txt` & `cerc-hub-0.1.8.1/hub/data/energy_systems/heat_pumps/wt_hourly3.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/energy_systems/montreal_custom_systems.xml` & `cerc-hub-0.1.8.1/hub/data/energy_systems/montreal_custom_systems.xml`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/geolocation/admin2Codes.txt` & `cerc-hub-0.1.8.1/hub/data/geolocation/admin2Codes.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/geolocation/cities15000.txt` & `cerc-hub-0.1.8.1/hub/data/geolocation/cities15000.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/greenery/ecore_greenery_catalog.xml` & `cerc-hub-0.1.8.1/hub/data/greenery/ecore_greenery_catalog.xml`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/usage/comnet_archetypes.xlsx` & `cerc-hub-0.1.8.1/hub/data/usage/comnet_archetypes.xlsx`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/usage/comnet_schedules_archetypes.xlsx` & `cerc-hub-0.1.8.1/hub/data/usage/comnet_schedules_archetypes.xlsx`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/usage/eilat_archetypes.xlsx` & `cerc-hub-0.1.8.1/hub/data/usage/eilat_archetypes.xlsx`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/usage/eilat_schedules_archetypes.xlsx` & `cerc-hub-0.1.8.1/hub/data/usage/eilat_schedules_archetypes.xlsx`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/data/weather/epw/CAN_PQ_Montreal.Intl.AP.716270_CWEC.epw` & `cerc-hub-0.1.8.1/hub/data/weather/epw/CAN_PQ_Montreal.Intl.AP.716270_CWEC.epw`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/exports/building_energy/energy_ade.py` & `cerc-hub-0.1.8.1/hub/exports/building_energy/energy_ade.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/exports/building_energy/idf.py` & `cerc-hub-0.1.8.1/hub/exports/building_energy/idf.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/exports/building_energy/idf_files/Energy+.idd` & `cerc-hub-0.1.8.1/hub/exports/building_energy/idf_files/Energy+.idd`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/exports/building_energy/idf_files/Minimal.idf` & `cerc-hub-0.1.8.1/hub/exports/building_energy/idf_files/Minimal.idf`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/exports/building_energy/insel/insel_monthly_energy_balance.py` & `cerc-hub-0.1.8.1/hub/exports/building_energy/insel/insel_monthly_energy_balance.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/exports/energy_building_exports_factory.py` & `cerc-hub-0.1.8.1/hub/exports/energy_building_exports_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/exports/energy_systems/air_source_hp_export.py` & `cerc-hub-0.1.8.1/hub/exports/energy_systems/air_source_hp_export.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/exports/energy_systems/heat_pump_export.py` & `cerc-hub-0.1.8.1/hub/exports/energy_systems/heat_pump_export.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/exports/energy_systems/water_to_water_hp_export.py` & `cerc-hub-0.1.8.1/hub/exports/energy_systems/water_to_water_hp_export.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/exports/energy_systems_factory.py` & `cerc-hub-0.1.8.1/hub/exports/energy_systems_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/exports/exports_factory.py` & `cerc-hub-0.1.8.1/hub/exports/exports_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/exports/formats/obj.py` & `cerc-hub-0.1.8.1/hub/exports/formats/obj.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/exports/formats/simplified_radiosity_algorithm.py` & `cerc-hub-0.1.8.1/hub/exports/formats/simplified_radiosity_algorithm.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/exports/formats/triangular.py` & `cerc-hub-0.1.8.1/hub/exports/formats/triangular.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/auth.py` & `cerc-hub-0.1.8.1/hub/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/configuration_helper.py` & `cerc-hub-0.1.8.1/hub/helpers/configuration_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/constants.py` & `cerc-hub-0.1.8.1/hub/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/alkis_function_to_hub_function.py` & `cerc-hub-0.1.8.1/hub/helpers/data/alkis_function_to_hub_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/eilat_function_to_hub_function.py` & `cerc-hub-0.1.8.1/hub/helpers/data/eilat_function_to_hub_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/hft_function_to_hub_function.py` & `cerc-hub-0.1.8.1/hub/helpers/data/hft_function_to_hub_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/hub_function_to_eilat_construction_function.py` & `cerc-hub-0.1.8.1/hub/helpers/data/hub_function_to_eilat_construction_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/hub_function_to_montreal_custom_costs_function.py` & `cerc-hub-0.1.8.1/hub/helpers/data/hub_function_to_montreal_custom_costs_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/hub_function_to_nrcan_construction_function.py` & `cerc-hub-0.1.8.1/hub/helpers/data/hub_function_to_nrcan_construction_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/hub_function_to_nrel_construction_function.py` & `cerc-hub-0.1.8.1/hub/helpers/data/hub_function_to_nrel_construction_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/hub_usage_to_comnet_usage.py` & `cerc-hub-0.1.8.1/hub/helpers/data/hub_usage_to_comnet_usage.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/hub_usage_to_eilat_usage.py` & `cerc-hub-0.1.8.1/hub/helpers/data/hub_usage_to_eilat_usage.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/hub_usage_to_hft_usage.py` & `cerc-hub-0.1.8.1/hub/helpers/data/hub_usage_to_hft_usage.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/hub_usage_to_nrcan_usage.py` & `cerc-hub-0.1.8.1/hub/helpers/data/hub_usage_to_nrcan_usage.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/montreal_custom_fuel_to_hub_fuel.py` & `cerc-hub-0.1.8.1/hub/helpers/data/montreal_custom_fuel_to_hub_fuel.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/montreal_demand_type_to_hub_energy_demand_type.py` & `cerc-hub-0.1.8.1/hub/helpers/data/montreal_demand_type_to_hub_energy_demand_type.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/montreal_function_to_hub_function.py` & `cerc-hub-0.1.8.1/hub/helpers/data/montreal_function_to_hub_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/montreal_system_to_hub_energy_generation_system.py` & `cerc-hub-0.1.8.1/hub/helpers/data/montreal_system_to_hub_energy_generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/data/pluto_function_to_hub_function.py` & `cerc-hub-0.1.8.1/hub/helpers/data/pluto_function_to_hub_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/dictionaries.py` & `cerc-hub-0.1.8.1/hub/helpers/dictionaries.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/geometry_helper.py` & `cerc-hub-0.1.8.1/hub/helpers/geometry_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/location.py` & `cerc-hub-0.1.8.1/hub/helpers/location.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/monthly_values.py` & `cerc-hub-0.1.8.1/hub/helpers/monthly_values.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/peak_calculation/loads_calculation.py` & `cerc-hub-0.1.8.1/hub/helpers/peak_calculation/loads_calculation.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/peak_loads.py` & `cerc-hub-0.1.8.1/hub/helpers/peak_loads.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/helpers/utils.py` & `cerc-hub-0.1.8.1/hub/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/construction/eilat_physics_parameters.py` & `cerc-hub-0.1.8.1/hub/imports/construction/eilat_physics_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/construction/helpers/construction_helper.py` & `cerc-hub-0.1.8.1/hub/imports/construction/helpers/construction_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/construction/helpers/storeys_generation.py` & `cerc-hub-0.1.8.1/hub/imports/construction/helpers/storeys_generation.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/construction/nrcan_physics_parameters.py` & `cerc-hub-0.1.8.1/hub/imports/construction/nrcan_physics_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/construction/nrel_physics_parameters.py` & `cerc-hub-0.1.8.1/hub/imports/construction/nrel_physics_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/construction_factory.py` & `cerc-hub-0.1.8.1/hub/imports/construction_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/energy_systems/air_source_hp_parameters.py` & `cerc-hub-0.1.8.1/hub/imports/energy_systems/air_source_hp_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/energy_systems/helpers/energy_systems_helper.py` & `cerc-hub-0.1.8.1/hub/imports/energy_systems/helpers/energy_systems_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/energy_systems/montreal_custom_energy_system_parameters.py` & `cerc-hub-0.1.8.1/hub/imports/energy_systems/montreal_custom_energy_system_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/energy_systems/water_to_water_hp_parameters.py` & `cerc-hub-0.1.8.1/hub/imports/energy_systems/water_to_water_hp_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/energy_systems_factory.py` & `cerc-hub-0.1.8.1/hub/imports/energy_systems_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/geometry/citygml.py` & `cerc-hub-0.1.8.1/hub/imports/geometry/citygml.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/geometry/citygml_classes/citygml_base.py` & `cerc-hub-0.1.8.1/hub/imports/geometry/citygml_classes/citygml_base.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/geometry/citygml_classes/citygml_lod1.py` & `cerc-hub-0.1.8.1/hub/imports/geometry/citygml_classes/citygml_lod1.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/geometry/citygml_classes/citygml_lod2.py` & `cerc-hub-0.1.8.1/hub/imports/geometry/citygml_classes/citygml_lod2.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/geometry/geojson.py` & `cerc-hub-0.1.8.1/hub/imports/geometry/geojson.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/geometry/gpandas.py` & `cerc-hub-0.1.8.1/hub/imports/geometry/gpandas.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/geometry/helpers/geometry_helper.py` & `cerc-hub-0.1.8.1/hub/imports/geometry/helpers/geometry_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/geometry/obj.py` & `cerc-hub-0.1.8.1/hub/imports/geometry/obj.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/geometry_factory.py` & `cerc-hub-0.1.8.1/hub/imports/geometry_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/results/insel_heatpump_energy_demand.py` & `cerc-hub-0.1.8.1/hub/imports/results/insel_heatpump_energy_demand.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/results/insel_monthly_energry_balance.py` & `cerc-hub-0.1.8.1/hub/imports/results/insel_monthly_energry_balance.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/results/simplified_radiosity_algorithm.py` & `cerc-hub-0.1.8.1/hub/imports/results/simplified_radiosity_algorithm.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/results_factory.py` & `cerc-hub-0.1.8.1/hub/imports/results_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/usage/comnet_usage_parameters.py` & `cerc-hub-0.1.8.1/hub/imports/usage/comnet_usage_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/usage/eilat_usage_parameters.py` & `cerc-hub-0.1.8.1/hub/imports/usage/eilat_usage_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/usage/nrcan_usage_parameters.py` & `cerc-hub-0.1.8.1/hub/imports/usage/nrcan_usage_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/usage_factory.py` & `cerc-hub-0.1.8.1/hub/imports/usage_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/weather/epw_weather_parameters.py` & `cerc-hub-0.1.8.1/hub/imports/weather/epw_weather_parameters.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/weather/helpers/weather.py` & `cerc-hub-0.1.8.1/hub/imports/weather/helpers/weather.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/imports/weather_factory.py` & `cerc-hub-0.1.8.1/hub/imports/weather_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/persistence/configuration.py` & `cerc-hub-0.1.8.1/hub/persistence/configuration.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/persistence/db_control.py` & `cerc-hub-0.1.8.1/hub/persistence/db_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,40 +110,44 @@
     :param request_values: dictionary containing the scenario and building names to grab the results
     :param result_names: if given, filter the results to the selected names
     """
     if result_names is None:
       result_names = []
     results = {}
     for scenario in request_values['scenarios']:
-      scenario_name = next(iter(scenario))
-      result_sets = self._city.get_by_user_id_application_id_and_scenario(
-        user_id,
-        application_id,
-        scenario_name
-      )
-      if result_sets is None:
-        continue
-      for result_set in result_sets:
-        city_id = result_set[0].id
+      print('scenario', scenario, results)
+      for scenario_name in scenario.keys():
+        print('scenario name', scenario_name)
 
-        results[scenario_name] = []
-        for building_name in scenario[scenario_name]:
-          _building = self._city_object.get_by_name_or_alias_and_city(building_name, city_id)
-          if _building is None:
-            continue
-          city_object_id = _building.id
-          _ = self._simulation_results.get_simulation_results_by_city_id_city_object_id_and_names(
-            city_id,
-            city_object_id,
-            result_names)
+        result_sets = self._city.get_by_user_id_application_id_and_scenario(
+          user_id,
+          application_id,
+          scenario_name
+        )
+        if result_sets is None:
+          continue
+        for result_set in result_sets:
+          city_id = result_set[0].id
 
-          for value in _:
-            values = json.loads(value.values)
-            values["building"] = building_name
-            results[scenario_name].append(values)
+          results[scenario_name] = []
+          for building_name in scenario[scenario_name]:
+            _building = self._city_object.get_by_name_or_alias_and_city(building_name, city_id)
+            if _building is None:
+              continue
+            city_object_id = _building.id
+            _ = self._simulation_results.get_simulation_results_by_city_id_city_object_id_and_names(
+              city_id,
+              city_object_id,
+              result_names)
+
+            for value in _:
+              values = json.loads(value.values)
+              values["building"] = building_name
+              results[scenario_name].append(values)
+      print(scenario, results)
     return results
 
   def persist_city(self, city: City, pickle_path, scenario, application_id: int, user_id: int):
     """
     Creates a city into the database
     :param city: City to be stored
     :param pickle_path: Path to save the pickle file
```

### Comparing `cerc-hub-0.1.8.0/hub/persistence/db_setup.py` & `cerc-hub-0.1.8.1/hub/persistence/db_setup.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/persistence/models/application.py` & `cerc-hub-0.1.8.1/hub/persistence/models/application.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/persistence/models/city.py` & `cerc-hub-0.1.8.1/hub/persistence/models/city.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/persistence/models/city_object.py` & `cerc-hub-0.1.8.1/hub/persistence/models/city_object.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/persistence/models/simulation_results.py` & `cerc-hub-0.1.8.1/hub/persistence/models/simulation_results.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/persistence/models/user.py` & `cerc-hub-0.1.8.1/hub/persistence/models/user.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/persistence/repositories/application.py` & `cerc-hub-0.1.8.1/hub/persistence/repositories/application.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/persistence/repositories/city.py` & `cerc-hub-0.1.8.1/hub/persistence/repositories/city.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Project Coder Peter Yefi peteryefi@gmail.com
 """
 import datetime
 import logging
 
 from sqlalchemy import select
 from sqlalchemy.exc import SQLAlchemyError
+from sqlalchemy.orm import Session
 
 from hub.city_model_structure.city import City as CityHub
 from hub.persistence.repository import Repository
 from hub.persistence.models import City as Model
 from hub.persistence.models import CityObject
 from hub.version import __version__
 
@@ -107,14 +108,16 @@
     :return: [ModelCity]
     """
     try:
       result_set = self.session.execute(select(Model).where(Model.user_id == user_id,
                                                             Model.application_id == application_id,
                                                             Model.scenario == scenario
                                                             )).all()
+      self.session.close()
+      self.session = Session(self.engine)
       return result_set
     except SQLAlchemyError as err:
       logging.error('Error while fetching city by name %s', err)
       raise SQLAlchemyError from err
 
   def get_by_user_id_and_application_id(self, user_id, application_id) -> [Model]:
     """
@@ -123,12 +126,14 @@
     :param application_id: the application id
     :return: ModelCity
     """
     try:
       result_set = self.session.execute(
         select(Model).where(Model.user_id == user_id, Model.application_id == application_id)
       )
+      self.session.close()
+      self.session = Session(self.engine)
       return [r[0] for r in result_set]
     except SQLAlchemyError as err:
       logging.error('Error while fetching city by name %s', err)
       raise SQLAlchemyError from err
```

### Comparing `cerc-hub-0.1.8.0/hub/persistence/repositories/city_object.py` & `cerc-hub-0.1.8.1/hub/persistence/repositories/city_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Project Coder Guille Gutierrez Guillermo.GutierrezMorote@concordia.ca
 """
 import datetime
 import logging
 
 from sqlalchemy import select, or_
 from sqlalchemy.exc import SQLAlchemyError
+from sqlalchemy.orm import Session
 
 from hub.city_model_structure.building import Building
 from hub.persistence.repository import Repository
 from hub.persistence.models import CityObject as Model
 
 
 class CityObject(Repository):
@@ -104,18 +105,20 @@
     :return: [CityObject] with the provided name or alias belonging to the city with id city_id
     """
     try:
       # search by name first
       city_object = self.session.execute(select(Model).where(Model.name == name, Model.city_id == city_id)).first()
       if city_object is not None:
         return city_object[0]
+      # name not found, so search by alias instead
       city_objects = self.session.execute(
         select(Model).where(Model.aliases.contains(name), Model.city_id == city_id)
       ).all()
-      # name not found, so search by alias instead
+      self.session.close()
+      self.session = Session(self.engine)
       for city_object in city_objects:
         aliases = city_object[0].aliases.replace('{', '').replace('}', '').split(',')
         for alias in aliases:
           if alias == name:
             # force the name as the alias
             city_object[0].name = name
             return city_object[0]
```

### Comparing `cerc-hub-0.1.8.0/hub/persistence/repositories/simulation_results.py` & `cerc-hub-0.1.8.1/hub/persistence/repositories/simulation_results.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/persistence/repositories/user.py` & `cerc-hub-0.1.8.1/hub/persistence/repositories/user.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/hub/persistence/repository.py` & `cerc-hub-0.1.8.1/hub/persistence/repository.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/setup.py` & `cerc-hub-0.1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_city_merge.py` & `cerc-hub-0.1.8.1/tests/test_city_merge.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_construction_catalog.py` & `cerc-hub-0.1.8.1/tests/test_construction_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_construction_factory.py` & `cerc-hub-0.1.8.1/tests/test_construction_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_costs_catalog.py` & `cerc-hub-0.1.8.1/tests/test_costs_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_custom_insel_block.py` & `cerc-hub-0.1.8.1/tests/test_custom_insel_block.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_db_factory.py` & `cerc-hub-0.1.8.1/tests/test_db_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_energy_systems_air_source_hp.py` & `cerc-hub-0.1.8.1/tests/test_energy_systems_air_source_hp.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_energy_systems_water_to_water_hp.py` & `cerc-hub-0.1.8.1/tests/test_energy_systems_water_to_water_hp.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_enrichement.py` & `cerc-hub-0.1.8.1/tests/test_enrichement.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_exports.py` & `cerc-hub-0.1.8.1/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_geometry_factory.py` & `cerc-hub-0.1.8.1/tests/test_geometry_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_greenery_catalog.py` & `cerc-hub-0.1.8.1/tests/test_greenery_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_greenery_in_idf.py` & `cerc-hub-0.1.8.1/tests/test_greenery_in_idf.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_heat_pump_results.py` & `cerc-hub-0.1.8.1/tests/test_heat_pump_results.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_insel_exports.py` & `cerc-hub-0.1.8.1/tests/test_insel_exports.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_results_import.py` & `cerc-hub-0.1.8.1/tests/test_results_import.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_systems_catalog.py` & `cerc-hub-0.1.8.1/tests/test_systems_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_systems_factory.py` & `cerc-hub-0.1.8.1/tests/test_systems_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_usage_catalog.py` & `cerc-hub-0.1.8.1/tests/test_usage_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.0/tests/test_usage_factory.py` & `cerc-hub-0.1.8.1/tests/test_usage_factory.py`

 * *Files identical despite different names*

