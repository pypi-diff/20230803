# Comparing `tmp/bddl-3.0.0b1.tar.gz` & `tmp/bddl-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bddl-3.0.0b1.tar", last modified: Thu Dec 15 09:37:28 2022, max compression
+gzip compressed data, was "bddl-3.1.0.tar", last modified: Thu Aug  3 21:07:53 2023, max compression
```

## Comparing `bddl-3.0.0b1.tar` & `bddl-3.1.0.tar`

### file list

```diff
@@ -1,165 +1,2127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.871277 bddl-3.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2022-12-15 09:37:16.000000 bddl-3.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-15 09:37:16.000000 bddl-3.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2022-12-15 09:37:28.871277 bddl-3.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2022-12-15 09:37:16.000000 bddl-3.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.859277 bddl-3.0.0b1/bddl/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/assembling_gift_baskets/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/assembling_gift_baskets/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/boxing_books_up_for_storage/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/boxing_books_up_for_storage/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/bringing_in_wood/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/bringing_in_wood/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/brushing_lint_off_clothing/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/brushing_lint_off_clothing/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_barbecue_grill/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_barbecue_grill/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_bathrooms/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_bathrooms/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_bathtub/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_bathtub/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_bedroom/
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_bedroom/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_carpets/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_carpets/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_floors/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_floors/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_freezer/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_freezer/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_garage/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_garage/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_high_chair/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_high_chair/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_kitchen_cupboard/
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_kitchen_cupboard/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_microwave_oven/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_microwave_oven/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_out_drawers/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_out_drawers/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_oven/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_oven/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_shoes/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_shoes/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_sneakers/
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_sneakers/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_stove/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_stove/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_table_after_clearing/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_table_after_clearing/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_the_hot_tub/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_the_hot_tub/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_the_pool/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_the_pool/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_toilet/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_toilet/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_up_after_a_meal/
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_up_after_a_meal/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_up_refrigerator/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_up_refrigerator/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/cleaning_windows/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/cleaning_windows/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/clearing_the_table_after_dinner/
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/clearing_the_table_after_dinner/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/collecting_aluminum_cans/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/collecting_aluminum_cans/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/defrosting_freezer/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/defrosting_freezer/problem0.bddl
--rw-r--r--   0 runner    (1001) docker     (123)      511 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/domain_igibson.bddl
--rw-r--r--   0 runner    (1001) docker     (123)      514 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/domain_omnigibson.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/installing_a_fax_machine/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/installing_a_fax_machine/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/installing_a_modem/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/installing_a_modem/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/installing_a_printer/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/installing_a_printer/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/installing_a_scanner/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/installing_a_scanner/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/installing_alarms/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/installing_alarms/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/laying_tile_floors/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/laying_tile_floors/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/laying_wood_floors/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/laying_wood_floors/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/loading_the_dishwasher/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/loading_the_dishwasher/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/mopping_floors/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/mopping_floors/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/moving_boxes_to_storage/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/moving_boxes_to_storage/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/organizing_boxes_in_garage/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/organizing_boxes_in_garage/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/organizing_file_cabinet/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/organizing_file_cabinet/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/organizing_school_stuff/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/organizing_school_stuff/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/packing_bags_or_suitcase/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/packing_bags_or_suitcase/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/picking_up_take-out_food/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/picking_up_take-out_food/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/picking_up_trash/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/picking_up_trash/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/polishing_furniture/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/polishing_furniture/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/polishing_shoes/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/polishing_shoes/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/polishing_silver/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/polishing_silver/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/putting_away_Christmas_decorations/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/putting_away_Christmas_decorations/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/putting_away_Halloween_decorations/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/putting_away_Halloween_decorations/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/putting_away_toys/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/putting_away_toys/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/putting_dishes_away_after_cleaning/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/putting_dishes_away_after_cleaning/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/putting_leftovers_away/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/putting_leftovers_away/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/putting_up_Christmas_decorations_inside/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/putting_up_Christmas_decorations_inside/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/re-shelving_library_books/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/re-shelving_library_books/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/rearranging_furniture/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/rearranging_furniture/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/serving_hors_d_oeuvres/
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/serving_hors_d_oeuvres/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/setting_mousetraps/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/setting_mousetraps/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/sorting_mail/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/sorting_mail/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.867277 bddl-3.0.0b1/bddl/activity_definitions/storing_food/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/storing_food/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.871277 bddl-3.0.0b1/bddl/activity_definitions/thawing_frozen_food/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/thawing_frozen_food/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.871277 bddl-3.0.0b1/bddl/activity_definitions/unpacking_suitcase/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/unpacking_suitcase/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.871277 bddl-3.0.0b1/bddl/activity_definitions/vacuuming_floors/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/vacuuming_floors/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.871277 bddl-3.0.0b1/bddl/activity_definitions/washing_floor/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/washing_floor/problem0.bddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.871277 bddl-3.0.0b1/bddl/activity_definitions/washing_pots_and_pans/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_definitions/washing_pots_and_pans/problem0.bddl
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_manifest.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15836 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/activity_to_preselected_scenes.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/backend_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19183 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/condition_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/config.py
--rw-r--r--   0 runner    (1001) docker     (123)  1409864 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/hierarchy_all.json
--rw-r--r--   0 runner    (1001) docker     (123)  1335562 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/hierarchy_articles.json
--rw-r--r--   0 runner    (1001) docker     (123)  3211497 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/hierarchy_b1k.json
--rw-r--r--   0 runner    (1001) docker     (123)   516175 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/hierarchy_owned.json
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/logic_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8690 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/object_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17484 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2022-12-15 09:37:16.000000 bddl-3.0.0b1/bddl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 09:37:28.863277 bddl-3.0.0b1/bddl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2022-12-15 09:37:28.000000 bddl-3.0.0b1/bddl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2022-12-15 09:37:28.000000 bddl-3.0.0b1/bddl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 09:37:28.000000 bddl-3.0.0b1/bddl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 09:37:28.000000 bddl-3.0.0b1/bddl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-15 09:37:28.000000 bddl-3.0.0b1/bddl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-15 09:37:28.000000 bddl-3.0.0b1/bddl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-15 09:37:28.871277 bddl-3.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      559 2022-12-15 09:37:16.000000 bddl-3.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.886028 bddl-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-03 21:07:39.000000 bddl-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 21:07:39.000000 bddl-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-08-03 21:07:53.886028 bddl-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-08-03 21:07:39.000000 bddl-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.570027 bddl-3.1.0/bddl/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.570027 bddl-3.1.0/bddl/activity_definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.574027 bddl-3.1.0/bddl/activity_definitions/adding_chemicals_to_hot_tub/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/adding_chemicals_to_hot_tub/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.574027 bddl-3.1.0/bddl/activity_definitions/adding_chemicals_to_lawn/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/adding_chemicals_to_lawn/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.574027 bddl-3.1.0/bddl/activity_definitions/adding_chemicals_to_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/adding_chemicals_to_pool/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.574027 bddl-3.1.0/bddl/activity_definitions/adding_fabric_softener/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/adding_fabric_softener/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.574027 bddl-3.1.0/bddl/activity_definitions/applying_pesticides/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/applying_pesticides/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.574027 bddl-3.1.0/bddl/activity_definitions/assembling_furniture/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/assembling_furniture/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.574027 bddl-3.1.0/bddl/activity_definitions/assembling_gift_baskets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/assembling_gift_baskets/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.574027 bddl-3.1.0/bddl/activity_definitions/attach_a_camera_to_a_tripod/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/attach_a_camera_to_a_tripod/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.574027 bddl-3.1.0/bddl/activity_definitions/bag_groceries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/bag_groceries/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.574027 bddl-3.1.0/bddl/activity_definitions/baking_cookies_for_the_PTA_bake_sale/
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/baking_cookies_for_the_PTA_bake_sale/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.574027 bddl-3.1.0/bddl/activity_definitions/baking_sugar_cookies/
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/baking_sugar_cookies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.574027 bddl-3.1.0/bddl/activity_definitions/boil_water/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/boil_water/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.574027 bddl-3.1.0/bddl/activity_definitions/boil_water_in_the_microwave/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/boil_water_in_the_microwave/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.578027 bddl-3.1.0/bddl/activity_definitions/bottling_wine/
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/bottling_wine/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.578027 bddl-3.1.0/bddl/activity_definitions/boxing_books_up_for_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/boxing_books_up_for_storage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.578027 bddl-3.1.0/bddl/activity_definitions/boxing_food_after_dinner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/boxing_food_after_dinner/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.578027 bddl-3.1.0/bddl/activity_definitions/brewing_coffee/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/brewing_coffee/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.578027 bddl-3.1.0/bddl/activity_definitions/bringing_glass_to_recycling/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/bringing_glass_to_recycling/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.578027 bddl-3.1.0/bddl/activity_definitions/bringing_in_kindling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/bringing_in_kindling/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.578027 bddl-3.1.0/bddl/activity_definitions/bringing_in_mail/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/bringing_in_mail/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.578027 bddl-3.1.0/bddl/activity_definitions/bringing_in_wood/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/bringing_in_wood/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.578027 bddl-3.1.0/bddl/activity_definitions/bringing_laundry/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/bringing_laundry/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.578027 bddl-3.1.0/bddl/activity_definitions/bringing_newspaper_in/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/bringing_newspaper_in/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.578027 bddl-3.1.0/bddl/activity_definitions/bringing_paper_to_recycling/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/bringing_paper_to_recycling/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.578027 bddl-3.1.0/bddl/activity_definitions/bringing_water/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/bringing_water/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.578027 bddl-3.1.0/bddl/activity_definitions/brushing_lint_off_clothing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/brushing_lint_off_clothing/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.578027 bddl-3.1.0/bddl/activity_definitions/buy_a_air_conditioner/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_a_air_conditioner/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.582027 bddl-3.1.0/bddl/activity_definitions/buy_a_belt/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_a_belt/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.582027 bddl-3.1.0/bddl/activity_definitions/buy_a_good_avocado/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_a_good_avocado/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.582027 bddl-3.1.0/bddl/activity_definitions/buy_a_keg/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_a_keg/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.582027 bddl-3.1.0/bddl/activity_definitions/buy_alcohol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_alcohol/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.582027 bddl-3.1.0/bddl/activity_definitions/buy_and_clean_mussels/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_and_clean_mussels/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.582027 bddl-3.1.0/bddl/activity_definitions/buy_basic_garden_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_basic_garden_tools/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.582027 bddl-3.1.0/bddl/activity_definitions/buy_boxes_for_packing/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_boxes_for_packing/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.582027 bddl-3.1.0/bddl/activity_definitions/buy_candle_making_supplies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_candle_making_supplies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.582027 bddl-3.1.0/bddl/activity_definitions/buy_dog_food/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_dog_food/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.582027 bddl-3.1.0/bddl/activity_definitions/buy_eggs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_eggs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.582027 bddl-3.1.0/bddl/activity_definitions/buy_fish/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_fish/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.582027 bddl-3.1.0/bddl/activity_definitions/buy_food_for_a_party/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_food_for_a_party/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.582027 bddl-3.1.0/bddl/activity_definitions/buy_food_for_camping/
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_food_for_camping/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.582027 bddl-3.1.0/bddl/activity_definitions/buy_good_chocolate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_good_chocolate/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.586027 bddl-3.1.0/bddl/activity_definitions/buy_home_use_medical_supplies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_home_use_medical_supplies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.586027 bddl-3.1.0/bddl/activity_definitions/buy_meat_from_a_butcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_meat_from_a_butcher/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.586027 bddl-3.1.0/bddl/activity_definitions/buy_mulch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_mulch/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.586027 bddl-3.1.0/bddl/activity_definitions/buy_natural_beef/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_natural_beef/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.586027 bddl-3.1.0/bddl/activity_definitions/buy_natural_supplements/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_natural_supplements/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.586027 bddl-3.1.0/bddl/activity_definitions/buy_pet_food_for_less/
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_pet_food_for_less/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.586027 bddl-3.1.0/bddl/activity_definitions/buy_rechargeable_batteries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_rechargeable_batteries/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.586027 bddl-3.1.0/bddl/activity_definitions/buy_salad_greens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_salad_greens/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.586027 bddl-3.1.0/bddl/activity_definitions/buy_school_supplies/
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_school_supplies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.586027 bddl-3.1.0/bddl/activity_definitions/buy_school_supplies_for_high_school/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_school_supplies_for_high_school/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.586027 bddl-3.1.0/bddl/activity_definitions/buy_used_gardening_equipment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buy_used_gardening_equipment/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.586027 bddl-3.1.0/bddl/activity_definitions/buying_cleaning_supplies/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buying_cleaning_supplies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.590027 bddl-3.1.0/bddl/activity_definitions/buying_everyday_consumer_goods/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buying_everyday_consumer_goods/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.590027 bddl-3.1.0/bddl/activity_definitions/buying_fast_food/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buying_fast_food/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.590027 bddl-3.1.0/bddl/activity_definitions/buying_gardening_supplies/
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buying_gardening_supplies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.590027 bddl-3.1.0/bddl/activity_definitions/buying_groceries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buying_groceries/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.590027 bddl-3.1.0/bddl/activity_definitions/buying_groceries_for_a_feast/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buying_groceries_for_a_feast/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.590027 bddl-3.1.0/bddl/activity_definitions/buying_office_supplies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buying_office_supplies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.590027 bddl-3.1.0/bddl/activity_definitions/buying_postage_stamps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/buying_postage_stamps/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.590027 bddl-3.1.0/bddl/activity_definitions/can_beans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/can_beans/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.590027 bddl-3.1.0/bddl/activity_definitions/can_fruit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/can_fruit/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.590027 bddl-3.1.0/bddl/activity_definitions/can_meat/
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/can_meat/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.590027 bddl-3.1.0/bddl/activity_definitions/can_syrup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/can_syrup/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.590027 bddl-3.1.0/bddl/activity_definitions/can_vegetables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/can_vegetables/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.594027 bddl-3.1.0/bddl/activity_definitions/canning_food/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/canning_food/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.594027 bddl-3.1.0/bddl/activity_definitions/carrying_in_groceries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/carrying_in_groceries/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.594027 bddl-3.1.0/bddl/activity_definitions/carrying_out_garden_furniture/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/carrying_out_garden_furniture/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.594027 bddl-3.1.0/bddl/activity_definitions/carrying_water/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/carrying_water/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.594027 bddl-3.1.0/bddl/activity_definitions/changing_bulbs/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/changing_bulbs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.594027 bddl-3.1.0/bddl/activity_definitions/changing_dogs_water/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/changing_dogs_water/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.594027 bddl-3.1.0/bddl/activity_definitions/changing_light_bulbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/changing_light_bulbs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.594027 bddl-3.1.0/bddl/activity_definitions/changing_sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/changing_sheets/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.594027 bddl-3.1.0/bddl/activity_definitions/chlorinating_the_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/chlorinating_the_pool/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.594027 bddl-3.1.0/bddl/activity_definitions/chop_an_onion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/chop_an_onion/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.594027 bddl-3.1.0/bddl/activity_definitions/chopping_wood/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/chopping_wood/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.594027 bddl-3.1.0/bddl/activity_definitions/clean_a_LED_screen/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_LED_screen/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.594027 bddl-3.1.0/bddl/activity_definitions/clean_a_air_conditioner/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_air_conditioner/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.594027 bddl-3.1.0/bddl/activity_definitions/clean_a_backpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_backpack/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.598027 bddl-3.1.0/bddl/activity_definitions/clean_a_baking_stone/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_baking_stone/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.598027 bddl-3.1.0/bddl/activity_definitions/clean_a_baseball_glove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_baseball_glove/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.598027 bddl-3.1.0/bddl/activity_definitions/clean_a_beer_keg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_beer_keg/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.598027 bddl-3.1.0/bddl/activity_definitions/clean_a_bicycle_chain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_bicycle_chain/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.598027 bddl-3.1.0/bddl/activity_definitions/clean_a_birdcage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_birdcage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.598027 bddl-3.1.0/bddl/activity_definitions/clean_a_blender/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_blender/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.598027 bddl-3.1.0/bddl/activity_definitions/clean_a_book/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_book/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.598027 bddl-3.1.0/bddl/activity_definitions/clean_a_bowling_ball/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_bowling_ball/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.598027 bddl-3.1.0/bddl/activity_definitions/clean_a_box_fan/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_box_fan/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.598027 bddl-3.1.0/bddl/activity_definitions/clean_a_broiler_pan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_broiler_pan/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.598027 bddl-3.1.0/bddl/activity_definitions/clean_a_camera_lens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_camera_lens/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.598027 bddl-3.1.0/bddl/activity_definitions/clean_a_candle_jar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_candle_jar/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.598027 bddl-3.1.0/bddl/activity_definitions/clean_a_chicken_coop/
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_chicken_coop/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.598027 bddl-3.1.0/bddl/activity_definitions/clean_a_coffee_maker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_coffee_maker/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.602027 bddl-3.1.0/bddl/activity_definitions/clean_a_company_office/
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_company_office/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.602027 bddl-3.1.0/bddl/activity_definitions/clean_a_computer_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_computer_monitor/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.602027 bddl-3.1.0/bddl/activity_definitions/clean_a_couch/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_couch/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.602027 bddl-3.1.0/bddl/activity_definitions/clean_a_crab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_crab/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.602027 bddl-3.1.0/bddl/activity_definitions/clean_a_dirty_baseball/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_dirty_baseball/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.602027 bddl-3.1.0/bddl/activity_definitions/clean_a_dirty_tent/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_dirty_tent/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.602027 bddl-3.1.0/bddl/activity_definitions/clean_a_drain/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_drain/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.602027 bddl-3.1.0/bddl/activity_definitions/clean_a_faucet/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_faucet/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.602027 bddl-3.1.0/bddl/activity_definitions/clean_a_felt_pool_table_top/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_felt_pool_table_top/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.602027 bddl-3.1.0/bddl/activity_definitions/clean_a_fence/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_fence/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.602027 bddl-3.1.0/bddl/activity_definitions/clean_a_fish/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_fish/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.602027 bddl-3.1.0/bddl/activity_definitions/clean_a_flat_iron/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_flat_iron/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.602027 bddl-3.1.0/bddl/activity_definitions/clean_a_flat_panel_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_flat_panel_monitor/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.602027 bddl-3.1.0/bddl/activity_definitions/clean_a_garden_sprayer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_garden_sprayer/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.606027 bddl-3.1.0/bddl/activity_definitions/clean_a_glass_pipe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_glass_pipe/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.606027 bddl-3.1.0/bddl/activity_definitions/clean_a_glass_windshield/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_glass_windshield/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.606027 bddl-3.1.0/bddl/activity_definitions/clean_a_golf_club/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_golf_club/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.606027 bddl-3.1.0/bddl/activity_definitions/clean_a_gravestone/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_gravestone/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.606027 bddl-3.1.0/bddl/activity_definitions/clean_a_grill_pan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_grill_pan/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.606027 bddl-3.1.0/bddl/activity_definitions/clean_a_guitar/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_guitar/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.606027 bddl-3.1.0/bddl/activity_definitions/clean_a_hamper/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_hamper/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.606027 bddl-3.1.0/bddl/activity_definitions/clean_a_hat/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_hat/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.606027 bddl-3.1.0/bddl/activity_definitions/clean_a_hot_water_dispenser/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_hot_water_dispenser/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.606027 bddl-3.1.0/bddl/activity_definitions/clean_a_keyboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_keyboard/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.606027 bddl-3.1.0/bddl/activity_definitions/clean_a_kitchen_sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_kitchen_sink/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.606027 bddl-3.1.0/bddl/activity_definitions/clean_a_kitchen_table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_kitchen_table/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.610027 bddl-3.1.0/bddl/activity_definitions/clean_a_knife/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_knife/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.610027 bddl-3.1.0/bddl/activity_definitions/clean_a_knife_block/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_knife_block/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.610027 bddl-3.1.0/bddl/activity_definitions/clean_a_leather_belt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_leather_belt/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.610027 bddl-3.1.0/bddl/activity_definitions/clean_a_light_bulb/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_light_bulb/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.610027 bddl-3.1.0/bddl/activity_definitions/clean_a_lobster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_lobster/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.610027 bddl-3.1.0/bddl/activity_definitions/clean_a_longboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_longboard/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.610027 bddl-3.1.0/bddl/activity_definitions/clean_a_loofah_or_natural_sponge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_loofah_or_natural_sponge/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.610027 bddl-3.1.0/bddl/activity_definitions/clean_a_mattress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_mattress/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.610027 bddl-3.1.0/bddl/activity_definitions/clean_a_mousepad/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_mousepad/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.610027 bddl-3.1.0/bddl/activity_definitions/clean_a_patio/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_patio/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.610027 bddl-3.1.0/bddl/activity_definitions/clean_a_piano/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_piano/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.610027 bddl-3.1.0/bddl/activity_definitions/clean_a_pickup_truck/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_pickup_truck/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.610027 bddl-3.1.0/bddl/activity_definitions/clean_a_pizza_stone/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_pizza_stone/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.610027 bddl-3.1.0/bddl/activity_definitions/clean_a_popcorn_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_popcorn_machine/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.614027 bddl-3.1.0/bddl/activity_definitions/clean_a_pumpkin/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_pumpkin/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.614027 bddl-3.1.0/bddl/activity_definitions/clean_a_purse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_purse/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.614027 bddl-3.1.0/bddl/activity_definitions/clean_a_quilt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_quilt/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.614027 bddl-3.1.0/bddl/activity_definitions/clean_a_raincoat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_raincoat/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.614027 bddl-3.1.0/bddl/activity_definitions/clean_a_razor_blade/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_razor_blade/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.614027 bddl-3.1.0/bddl/activity_definitions/clean_a_rice_cooker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_rice_cooker/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.614027 bddl-3.1.0/bddl/activity_definitions/clean_a_rug/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_rug/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.614027 bddl-3.1.0/bddl/activity_definitions/clean_a_sauna/
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_sauna/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.614027 bddl-3.1.0/bddl/activity_definitions/clean_a_sauna_suit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_sauna_suit/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.614027 bddl-3.1.0/bddl/activity_definitions/clean_a_saxophone/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_saxophone/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.614027 bddl-3.1.0/bddl/activity_definitions/clean_a_shower/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_shower/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.614027 bddl-3.1.0/bddl/activity_definitions/clean_a_sieve/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_sieve/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_small_pet_cage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_small_pet_cage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_sofa/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_sofa/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_softball_bat/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_softball_bat/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_sponge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_sponge/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_stainless_steel_dishwasher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_stainless_steel_dishwasher/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_suitcase/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_suitcase/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_teddy_bear/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_teddy_bear/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_tie/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_tie/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_toaster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_toaster/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_toaster_oven/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_toaster_oven/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_trombone/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_trombone/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_trumpet/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_trumpet/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_turkey/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_turkey/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_vacuum/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_vacuum/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.618027 bddl-3.1.0/bddl/activity_definitions/clean_a_violin/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_violin/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.622027 bddl-3.1.0/bddl/activity_definitions/clean_a_watch/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_watch/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.622027 bddl-3.1.0/bddl/activity_definitions/clean_a_whiteboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_whiteboard/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.622027 bddl-3.1.0/bddl/activity_definitions/clean_a_wood_pipe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_a_wood_pipe/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.622027 bddl-3.1.0/bddl/activity_definitions/clean_an_air_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_an_air_filter/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.622027 bddl-3.1.0/bddl/activity_definitions/clean_an_electric_kettle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_an_electric_kettle/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.622027 bddl-3.1.0/bddl/activity_definitions/clean_an_electric_razor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_an_electric_razor/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.622027 bddl-3.1.0/bddl/activity_definitions/clean_an_eraser/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_an_eraser/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.622027 bddl-3.1.0/bddl/activity_definitions/clean_an_espresso_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_an_espresso_machine/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.622027 bddl-3.1.0/bddl/activity_definitions/clean_an_iron/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_an_iron/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.622027 bddl-3.1.0/bddl/activity_definitions/clean_an_office_chair/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_an_office_chair/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.622027 bddl-3.1.0/bddl/activity_definitions/clean_and_disinfect_ice_trays/
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_and_disinfect_ice_trays/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.622027 bddl-3.1.0/bddl/activity_definitions/clean_apples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_apples/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.626027 bddl-3.1.0/bddl/activity_definitions/clean_baby_toys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_baby_toys/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.626027 bddl-3.1.0/bddl/activity_definitions/clean_baking_sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_baking_sheets/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.626027 bddl-3.1.0/bddl/activity_definitions/clean_batting_gloves/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_batting_gloves/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.626027 bddl-3.1.0/bddl/activity_definitions/clean_black_rims/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_black_rims/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.626027 bddl-3.1.0/bddl/activity_definitions/clean_bok_choy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_bok_choy/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.626027 bddl-3.1.0/bddl/activity_definitions/clean_boxing_gloves/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_boxing_gloves/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.626027 bddl-3.1.0/bddl/activity_definitions/clean_brass/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_brass/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.626027 bddl-3.1.0/bddl/activity_definitions/clean_brass_casings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_brass_casings/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.626027 bddl-3.1.0/bddl/activity_definitions/clean_brooms/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_brooms/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.626027 bddl-3.1.0/bddl/activity_definitions/clean_cabbage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_cabbage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.626027 bddl-3.1.0/bddl/activity_definitions/clean_carpets/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_carpets/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.626027 bddl-3.1.0/bddl/activity_definitions/clean_cement/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_cement/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_clams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_clams/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_clear_plastic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_clear_plastic/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_conch_shells/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_conch_shells/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_copper_mugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_copper_mugs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_copper_wire/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_copper_wire/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_cork_mats/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_cork_mats/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_couch_pillows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_couch_pillows/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_cup_holders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_cup_holders/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_cups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_cups/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_decking/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_decking/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_deer_antlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_deer_antlers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_dentures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_dentures/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_dentures_with_vinegar/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_dentures_with_vinegar/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_dog_collars/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_dog_collars/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.630027 bddl-3.1.0/bddl/activity_definitions/clean_eggs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_eggs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.634027 bddl-3.1.0/bddl/activity_definitions/clean_fishing_lures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_fishing_lures/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.634027 bddl-3.1.0/bddl/activity_definitions/clean_flip_flops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_flip_flops/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.634027 bddl-3.1.0/bddl/activity_definitions/clean_fur/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_fur/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.634027 bddl-3.1.0/bddl/activity_definitions/clean_garden_gloves/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_garden_gloves/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.634027 bddl-3.1.0/bddl/activity_definitions/clean_gas_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_gas_logs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.634027 bddl-3.1.0/bddl/activity_definitions/clean_geodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_geodes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.634027 bddl-3.1.0/bddl/activity_definitions/clean_gold/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_gold/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.634027 bddl-3.1.0/bddl/activity_definitions/clean_gourds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_gourds/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.634027 bddl-3.1.0/bddl/activity_definitions/clean_grease/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_grease/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.634027 bddl-3.1.0/bddl/activity_definitions/clean_green_beans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_green_beans/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.634027 bddl-3.1.0/bddl/activity_definitions/clean_greens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_greens/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.634027 bddl-3.1.0/bddl/activity_definitions/clean_household_cleaning_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_household_cleaning_tools/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.634027 bddl-3.1.0/bddl/activity_definitions/clean_invisalign/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_invisalign/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.638027 bddl-3.1.0/bddl/activity_definitions/clean_jade/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_jade/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.638027 bddl-3.1.0/bddl/activity_definitions/clean_jewels/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_jewels/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.638027 bddl-3.1.0/bddl/activity_definitions/clean_kitchen_appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_kitchen_appliances/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.638027 bddl-3.1.0/bddl/activity_definitions/clean_leather_boots/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_leather_boots/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.638027 bddl-3.1.0/bddl/activity_definitions/clean_leather_sandals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_leather_sandals/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.638027 bddl-3.1.0/bddl/activity_definitions/clean_marker_off_a_doll/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_marker_off_a_doll/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.638027 bddl-3.1.0/bddl/activity_definitions/clean_mirrors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_mirrors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.642027 bddl-3.1.0/bddl/activity_definitions/clean_mushrooms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_mushrooms/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.642027 bddl-3.1.0/bddl/activity_definitions/clean_mussels/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_mussels/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.642027 bddl-3.1.0/bddl/activity_definitions/clean_nickel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_nickel/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.642027 bddl-3.1.0/bddl/activity_definitions/clean_out_a_guinea_pigs_hutch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_out_a_guinea_pigs_hutch/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.642027 bddl-3.1.0/bddl/activity_definitions/clean_outdoor_tiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_outdoor_tiles/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.642027 bddl-3.1.0/bddl/activity_definitions/clean_oysters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_oysters/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.642027 bddl-3.1.0/bddl/activity_definitions/clean_paper_lampshades/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_paper_lampshades/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.642027 bddl-3.1.0/bddl/activity_definitions/clean_pearls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_pearls/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.642027 bddl-3.1.0/bddl/activity_definitions/clean_pennies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_pennies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.642027 bddl-3.1.0/bddl/activity_definitions/clean_piano_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_piano_keys/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.642027 bddl-3.1.0/bddl/activity_definitions/clean_pine_cones/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_pine_cones/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.642027 bddl-3.1.0/bddl/activity_definitions/clean_place_mats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_place_mats/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.642027 bddl-3.1.0/bddl/activity_definitions/clean_plastic_containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_plastic_containers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.642027 bddl-3.1.0/bddl/activity_definitions/clean_potatoes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_potatoes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.646027 bddl-3.1.0/bddl/activity_definitions/clean_pottery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_pottery/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.646027 bddl-3.1.0/bddl/activity_definitions/clean_prawns/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_prawns/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.646027 bddl-3.1.0/bddl/activity_definitions/clean_quarters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_quarters/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.646027 bddl-3.1.0/bddl/activity_definitions/clean_quartz/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_quartz/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.646027 bddl-3.1.0/bddl/activity_definitions/clean_raw_denim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_raw_denim/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.646027 bddl-3.1.0/bddl/activity_definitions/clean_reusable_shopping_bags/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_reusable_shopping_bags/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.646027 bddl-3.1.0/bddl/activity_definitions/clean_rubber/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_rubber/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.646027 bddl-3.1.0/bddl/activity_definitions/clean_rubber_bathmats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_rubber_bathmats/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.646027 bddl-3.1.0/bddl/activity_definitions/clean_scallops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_scallops/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.646027 bddl-3.1.0/bddl/activity_definitions/clean_seashells/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_seashells/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.646027 bddl-3.1.0/bddl/activity_definitions/clean_sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_sheets/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.646027 bddl-3.1.0/bddl/activity_definitions/clean_shrimp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_shrimp/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.646027 bddl-3.1.0/bddl/activity_definitions/clean_silver_coins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_silver_coins/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.650027 bddl-3.1.0/bddl/activity_definitions/clean_skateboard_bearings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_skateboard_bearings/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.650027 bddl-3.1.0/bddl/activity_definitions/clean_snap_peas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_snap_peas/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.650027 bddl-3.1.0/bddl/activity_definitions/clean_snow_peas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_snow_peas/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.650027 bddl-3.1.0/bddl/activity_definitions/clean_soot_from_glass_lanterns/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_soot_from_glass_lanterns/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.650027 bddl-3.1.0/bddl/activity_definitions/clean_stainless_steel_sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_stainless_steel_sinks/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.650027 bddl-3.1.0/bddl/activity_definitions/clean_strawberries/
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_strawberries/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.650027 bddl-3.1.0/bddl/activity_definitions/clean_stucco/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_stucco/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.650027 bddl-3.1.0/bddl/activity_definitions/clean_suede_gloves/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_suede_gloves/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.650027 bddl-3.1.0/bddl/activity_definitions/clean_sunglasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_sunglasses/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.650027 bddl-3.1.0/bddl/activity_definitions/clean_synthetic_hiking_gear/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_synthetic_hiking_gear/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.650027 bddl-3.1.0/bddl/activity_definitions/clean_tennis_balls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_tennis_balls/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.650027 bddl-3.1.0/bddl/activity_definitions/clean_the_bottom_of_an_iron/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_the_bottom_of_an_iron/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.650027 bddl-3.1.0/bddl/activity_definitions/clean_the_exterior_of_your_garage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_the_exterior_of_your_garage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.650027 bddl-3.1.0/bddl/activity_definitions/clean_the_interior_of_your_car/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_the_interior_of_your_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.654027 bddl-3.1.0/bddl/activity_definitions/clean_the_outside_of_a_house/
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_the_outside_of_a_house/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.654027 bddl-3.1.0/bddl/activity_definitions/clean_tweed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_tweed/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.654027 bddl-3.1.0/bddl/activity_definitions/clean_up_after_a_dinner_party/
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_up_after_a_dinner_party/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.654027 bddl-3.1.0/bddl/activity_definitions/clean_up_broken_glass/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_up_broken_glass/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.654027 bddl-3.1.0/bddl/activity_definitions/clean_up_gasoline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_up_gasoline/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.654027 bddl-3.1.0/bddl/activity_definitions/clean_up_spilled_egg/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_up_spilled_egg/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.654027 bddl-3.1.0/bddl/activity_definitions/clean_up_water_damage/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_up_water_damage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.654027 bddl-3.1.0/bddl/activity_definitions/clean_up_your_desk/
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_up_your_desk/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.654027 bddl-3.1.0/bddl/activity_definitions/clean_vans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_vans/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.654027 bddl-3.1.0/bddl/activity_definitions/clean_vases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_vases/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.654027 bddl-3.1.0/bddl/activity_definitions/clean_vintage_stereo_equipment/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_vintage_stereo_equipment/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.654027 bddl-3.1.0/bddl/activity_definitions/clean_vinyl_shutters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_vinyl_shutters/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.654027 bddl-3.1.0/bddl/activity_definitions/clean_walls/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_walls/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.658027 bddl-3.1.0/bddl/activity_definitions/clean_whiskey_stones/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_whiskey_stones/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.658027 bddl-3.1.0/bddl/activity_definitions/clean_white_wall_tires/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_white_wall_tires/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.658027 bddl-3.1.0/bddl/activity_definitions/clean_wine_glasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_wine_glasses/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.658027 bddl-3.1.0/bddl/activity_definitions/clean_wood_doors/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_wood_doors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.658027 bddl-3.1.0/bddl/activity_definitions/clean_wood_pallets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_wood_pallets/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.658027 bddl-3.1.0/bddl/activity_definitions/clean_wood_siding/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_wood_siding/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.658027 bddl-3.1.0/bddl/activity_definitions/clean_wooden_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_wooden_blocks/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.658027 bddl-3.1.0/bddl/activity_definitions/clean_your_baseboard_radiators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_your_baseboard_radiators/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.658027 bddl-3.1.0/bddl/activity_definitions/clean_your_cleaning_supplies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_your_cleaning_supplies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.658027 bddl-3.1.0/bddl/activity_definitions/clean_your_electronics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_your_electronics/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.658027 bddl-3.1.0/bddl/activity_definitions/clean_your_goal_keeper_gloves/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_your_goal_keeper_gloves/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.658027 bddl-3.1.0/bddl/activity_definitions/clean_your_house_after_a_wild_party/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_your_house_after_a_wild_party/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/clean_your_kitty_litter_box/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_your_kitty_litter_box/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/clean_your_laundry_room/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_your_laundry_room/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/clean_your_pencil_case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_your_pencil_case/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/clean_your_rusty_garden_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clean_your_rusty_garden_tools/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/cleaning_around_pool_in_garden/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_around_pool_in_garden/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/cleaning_barbecue_grill/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_barbecue_grill/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/cleaning_bathrooms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_bathrooms/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/cleaning_bathtub/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_bathtub/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/cleaning_bedroom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_bedroom/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/cleaning_boat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_boat/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/cleaning_camper_or_RV/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_camper_or_RV/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/cleaning_carpets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_carpets/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/cleaning_computer/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_computer/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/cleaning_cups_in_living_room/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_cups_in_living_room/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/cleaning_debris_out_of_car/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_debris_out_of_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.662027 bddl-3.1.0/bddl/activity_definitions/cleaning_driveway/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_driveway/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.666027 bddl-3.1.0/bddl/activity_definitions/cleaning_fan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_fan/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.666027 bddl-3.1.0/bddl/activity_definitions/cleaning_fishing_gear/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_fishing_gear/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.666027 bddl-3.1.0/bddl/activity_definitions/cleaning_floors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_floors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.666027 bddl-3.1.0/bddl/activity_definitions/cleaning_freezer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_freezer/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.666027 bddl-3.1.0/bddl/activity_definitions/cleaning_garage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_garage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.666027 bddl-3.1.0/bddl/activity_definitions/cleaning_garden_path/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_garden_path/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.666027 bddl-3.1.0/bddl/activity_definitions/cleaning_garden_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_garden_tools/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.666027 bddl-3.1.0/bddl/activity_definitions/cleaning_glasses_off_bar/
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_glasses_off_bar/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.666027 bddl-3.1.0/bddl/activity_definitions/cleaning_high_chair/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_high_chair/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.666027 bddl-3.1.0/bddl/activity_definitions/cleaning_kitchen_cupboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_kitchen_cupboard/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.666027 bddl-3.1.0/bddl/activity_definitions/cleaning_kitchen_knives/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_kitchen_knives/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.666027 bddl-3.1.0/bddl/activity_definitions/cleaning_lawnmowers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_lawnmowers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.670027 bddl-3.1.0/bddl/activity_definitions/cleaning_microwave_oven/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_microwave_oven/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.670027 bddl-3.1.0/bddl/activity_definitions/cleaning_mushrooms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_mushrooms/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.670027 bddl-3.1.0/bddl/activity_definitions/cleaning_out_drawers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_out_drawers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.670027 bddl-3.1.0/bddl/activity_definitions/cleaning_oven/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_oven/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.670027 bddl-3.1.0/bddl/activity_definitions/cleaning_parks/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_parks/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.670027 bddl-3.1.0/bddl/activity_definitions/cleaning_patio_furniture/
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_patio_furniture/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.670027 bddl-3.1.0/bddl/activity_definitions/cleaning_pavement/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_pavement/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.670027 bddl-3.1.0/bddl/activity_definitions/cleaning_pet_bed/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_pet_bed/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.670027 bddl-3.1.0/bddl/activity_definitions/cleaning_rainboots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_rainboots/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.670027 bddl-3.1.0/bddl/activity_definitions/cleaning_restaurant_table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_restaurant_table/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.670027 bddl-3.1.0/bddl/activity_definitions/cleaning_shed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_shed/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.670027 bddl-3.1.0/bddl/activity_definitions/cleaning_shoes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_shoes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.670027 bddl-3.1.0/bddl/activity_definitions/cleaning_skis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_skis/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.670027 bddl-3.1.0/bddl/activity_definitions/cleaning_sneakers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_sneakers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.674027 bddl-3.1.0/bddl/activity_definitions/cleaning_stove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_stove/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.674027 bddl-3.1.0/bddl/activity_definitions/cleaning_stuff_out_of_car/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_stuff_out_of_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.674027 bddl-3.1.0/bddl/activity_definitions/cleaning_table_after_clearing/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_table_after_clearing/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.674027 bddl-3.1.0/bddl/activity_definitions/cleaning_the_hot_tub/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_the_hot_tub/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.674027 bddl-3.1.0/bddl/activity_definitions/cleaning_the_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_the_pool/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.674027 bddl-3.1.0/bddl/activity_definitions/cleaning_the_yard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_the_yard/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.674027 bddl-3.1.0/bddl/activity_definitions/cleaning_toilet/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_toilet/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.674027 bddl-3.1.0/bddl/activity_definitions/cleaning_tools_and_equipment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_tools_and_equipment/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.674027 bddl-3.1.0/bddl/activity_definitions/cleaning_up_after_a_meal/
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_up_after_a_meal/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.674027 bddl-3.1.0/bddl/activity_definitions/cleaning_up_after_an_event/
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_up_after_an_event/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.674027 bddl-3.1.0/bddl/activity_definitions/cleaning_up_branches_and_twigs/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_up_branches_and_twigs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.674027 bddl-3.1.0/bddl/activity_definitions/cleaning_up_plates_and_food/
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_up_plates_and_food/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.674027 bddl-3.1.0/bddl/activity_definitions/cleaning_up_refrigerator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_up_refrigerator/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.678027 bddl-3.1.0/bddl/activity_definitions/cleaning_vehicles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_vehicles/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.678027 bddl-3.1.0/bddl/activity_definitions/cleaning_windows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cleaning_windows/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.678027 bddl-3.1.0/bddl/activity_definitions/clearing_food_from_table_into_fridge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clearing_food_from_table_into_fridge/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.678027 bddl-3.1.0/bddl/activity_definitions/clearing_table_after_breakfast/
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clearing_table_after_breakfast/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.678027 bddl-3.1.0/bddl/activity_definitions/clearing_table_after_coffee/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clearing_table_after_coffee/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/clearing_table_after_dinner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clearing_table_after_dinner/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/clearing_table_after_snacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clearing_table_after_snacks/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/clearing_table_after_supper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clearing_table_after_supper/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/clearing_the_table_after_dinner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/clearing_the_table_after_dinner/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/cold_brew_coffee/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cold_brew_coffee/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/collecting_aluminum_cans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/collecting_aluminum_cans/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/collecting_berries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/collecting_berries/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/collecting_childrens_toys/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/collecting_childrens_toys/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/collecting_dishes_from_around_house/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/collecting_dishes_from_around_house/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/collecting_dishes_from_restaurant_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/collecting_dishes_from_restaurant_tables/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/collecting_mail_from_the_letterbox/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/collecting_mail_from_the_letterbox/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/collecting_wood/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/collecting_wood/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/composting_waste/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/composting_waste/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/cook_a_brisket/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_a_brisket/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/cook_a_crab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_a_crab/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.682027 bddl-3.1.0/bddl/activity_definitions/cook_a_duck/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_a_duck/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.686027 bddl-3.1.0/bddl/activity_definitions/cook_a_frozen_pie/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_a_frozen_pie/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.686027 bddl-3.1.0/bddl/activity_definitions/cook_a_ham/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_a_ham/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.686027 bddl-3.1.0/bddl/activity_definitions/cook_a_pumpkin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_a_pumpkin/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.686027 bddl-3.1.0/bddl/activity_definitions/cook_a_turkey/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_a_turkey/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.686027 bddl-3.1.0/bddl/activity_definitions/cook_arepas/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_arepas/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.686027 bddl-3.1.0/bddl/activity_definitions/cook_asparagus/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_asparagus/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.686027 bddl-3.1.0/bddl/activity_definitions/cook_bacon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_bacon/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.686027 bddl-3.1.0/bddl/activity_definitions/cook_beef/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_beef/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.686027 bddl-3.1.0/bddl/activity_definitions/cook_beef_and_onions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_beef_and_onions/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.686027 bddl-3.1.0/bddl/activity_definitions/cook_bok_choy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_bok_choy/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.686027 bddl-3.1.0/bddl/activity_definitions/cook_broccolini/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_broccolini/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.686027 bddl-3.1.0/bddl/activity_definitions/cook_brussels_sprouts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_brussels_sprouts/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.686027 bddl-3.1.0/bddl/activity_definitions/cook_cabbage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_cabbage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.686027 bddl-3.1.0/bddl/activity_definitions/cook_carrots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_carrots/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.690028 bddl-3.1.0/bddl/activity_definitions/cook_chicken/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_chicken/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.690028 bddl-3.1.0/bddl/activity_definitions/cook_chicken_and_rice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_chicken_and_rice/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.690028 bddl-3.1.0/bddl/activity_definitions/cook_chickpeas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_chickpeas/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.690028 bddl-3.1.0/bddl/activity_definitions/cook_chorizo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_chorizo/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.690028 bddl-3.1.0/bddl/activity_definitions/cook_clams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_clams/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.690028 bddl-3.1.0/bddl/activity_definitions/cook_corn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_corn/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.690028 bddl-3.1.0/bddl/activity_definitions/cook_eggplant/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_eggplant/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.690028 bddl-3.1.0/bddl/activity_definitions/cook_eggs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_eggs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.690028 bddl-3.1.0/bddl/activity_definitions/cook_fish/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_fish/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.690028 bddl-3.1.0/bddl/activity_definitions/cook_green_beans/
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_green_beans/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.690028 bddl-3.1.0/bddl/activity_definitions/cook_ground_beef/
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_ground_beef/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.690028 bddl-3.1.0/bddl/activity_definitions/cook_ham_hocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_ham_hocks/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.694028 bddl-3.1.0/bddl/activity_definitions/cook_hot_dogs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_hot_dogs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.694028 bddl-3.1.0/bddl/activity_definitions/cook_kabobs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_kabobs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.694028 bddl-3.1.0/bddl/activity_definitions/cook_kale/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_kale/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.694028 bddl-3.1.0/bddl/activity_definitions/cook_kielbasa/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_kielbasa/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.694028 bddl-3.1.0/bddl/activity_definitions/cook_lamb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_lamb/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.694028 bddl-3.1.0/bddl/activity_definitions/cook_lasagne/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_lasagne/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.694028 bddl-3.1.0/bddl/activity_definitions/cook_mussels/
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_mussels/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.694028 bddl-3.1.0/bddl/activity_definitions/cook_mustard_greens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_mustard_greens/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.694028 bddl-3.1.0/bddl/activity_definitions/cook_noodles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_noodles/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.694028 bddl-3.1.0/bddl/activity_definitions/cook_onions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_onions/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.694028 bddl-3.1.0/bddl/activity_definitions/cook_oysters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_oysters/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.694028 bddl-3.1.0/bddl/activity_definitions/cook_pasta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_pasta/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.694028 bddl-3.1.0/bddl/activity_definitions/cook_peas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_peas/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.698027 bddl-3.1.0/bddl/activity_definitions/cook_peppers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_peppers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.698027 bddl-3.1.0/bddl/activity_definitions/cook_pork_ribs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_pork_ribs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.698027 bddl-3.1.0/bddl/activity_definitions/cook_potatoes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_potatoes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.698027 bddl-3.1.0/bddl/activity_definitions/cook_pumpkin_seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_pumpkin_seeds/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.698027 bddl-3.1.0/bddl/activity_definitions/cook_quail/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_quail/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.698027 bddl-3.1.0/bddl/activity_definitions/cook_ramen_noodles/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_ramen_noodles/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.698027 bddl-3.1.0/bddl/activity_definitions/cook_red_peppers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_red_peppers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.698027 bddl-3.1.0/bddl/activity_definitions/cook_rice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_rice/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.698027 bddl-3.1.0/bddl/activity_definitions/cook_sausages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_sausages/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.698027 bddl-3.1.0/bddl/activity_definitions/cook_seafood_paella/
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_seafood_paella/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.698027 bddl-3.1.0/bddl/activity_definitions/cook_shrimp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_shrimp/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.698027 bddl-3.1.0/bddl/activity_definitions/cook_snap_peas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_snap_peas/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.698027 bddl-3.1.0/bddl/activity_definitions/cook_soup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_soup/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.698027 bddl-3.1.0/bddl/activity_definitions/cook_spinach/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_spinach/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/cook_squash/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_squash/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/cook_sweet_potatoes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_sweet_potatoes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/cook_tofu/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_tofu/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/cook_turkey_drumsticks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_turkey_drumsticks/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/cook_vegetables/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_vegetables/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/cook_zucchini/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cook_zucchini/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/cooking_a_feast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cooking_a_feast/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/cooking_breakfast/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cooking_breakfast/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/cooking_dinner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cooking_dinner/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/cooking_food_for_adult/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cooking_food_for_adult/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/cooking_lunch/
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cooking_lunch/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/cool_cakes/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cool_cakes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/cover_a_flower_pot_in_fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/cover_a_flower_pot_in_fabric/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/covering_boat/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/covering_boat/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.702027 bddl-3.1.0/bddl/activity_definitions/de_clutter_your_garage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/de_clutter_your_garage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.706028 bddl-3.1.0/bddl/activity_definitions/de_ice_a_car/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/de_ice_a_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.706028 bddl-3.1.0/bddl/activity_definitions/decorating_for_religious_ceremony/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/decorating_for_religious_ceremony/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.706028 bddl-3.1.0/bddl/activity_definitions/decorating_outside_for_holidays/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/decorating_outside_for_holidays/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.706028 bddl-3.1.0/bddl/activity_definitions/decorating_outside_for_parties/
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/decorating_outside_for_parties/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.706028 bddl-3.1.0/bddl/activity_definitions/defrost_meat/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/defrost_meat/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.706028 bddl-3.1.0/bddl/activity_definitions/defrosting_freezer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/defrosting_freezer/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.706028 bddl-3.1.0/bddl/activity_definitions/delivering_groceries_to_doorstep/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/delivering_groceries_to_doorstep/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.706028 bddl-3.1.0/bddl/activity_definitions/disinfect_laundry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/disinfect_laundry/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.706028 bddl-3.1.0/bddl/activity_definitions/disinfect_nail_clippers/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/disinfect_nail_clippers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.706028 bddl-3.1.0/bddl/activity_definitions/dispose_of_a_pizza_box/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/dispose_of_a_pizza_box/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.706028 bddl-3.1.0/bddl/activity_definitions/dispose_of_batteries/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/dispose_of_batteries/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.706028 bddl-3.1.0/bddl/activity_definitions/dispose_of_fireworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/dispose_of_fireworks/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.706028 bddl-3.1.0/bddl/activity_definitions/dispose_of_glass/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/dispose_of_glass/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/dispose_of_medication/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/dispose_of_medication/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/dispose_of_paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/dispose_of_paper/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/disposing_of_lawn_clippings/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/disposing_of_lawn_clippings/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/disposing_of_trash_for_adult/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/disposing_of_trash_for_adult/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/distributing_event_T_shirts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/distributing_event_T_shirts/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/distributing_groceries_at_food_bank/
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/distributing_groceries_at_food_bank/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/doing_housework_for_adult/
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/doing_housework_for_adult/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/doing_laundry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/doing_laundry/problem0.bddl
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/domain_igibson.bddl
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/domain_omnigibson.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/donating_clothing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/donating_clothing/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/donating_toys/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/donating_toys/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/drape_window_scarves/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/drape_window_scarves/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/drying_dishes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/drying_dishes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/drying_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/drying_table/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/dust_houseplants/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/dust_houseplants/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/dusting_rugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/dusting_rugs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.710028 bddl-3.1.0/bddl/activity_definitions/emptying_ashtray/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/emptying_ashtray/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/emptying_trash_cans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/emptying_trash_cans/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/fertilize_a_lawn/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fertilize_a_lawn/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/fertilize_plants/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fertilize_plants/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/fertilizing_garden/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fertilizing_garden/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/fill_a_bucket_in_a_small_sink/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fill_a_bucket_in_a_small_sink/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/fill_a_canteen/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fill_a_canteen/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/fill_a_hot_water_bottle/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fill_a_hot_water_bottle/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/fill_a_punching_bag/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fill_a_punching_bag/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/filling_pepper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/filling_pepper/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/filling_salt/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/filling_salt/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/filling_sugar/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/filling_sugar/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/filling_the_bird_feeder/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/filling_the_bird_feeder/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/fixing_broken_chair/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fixing_broken_chair/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/fixing_broken_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fixing_broken_table/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.714028 bddl-3.1.0/bddl/activity_definitions/fixing_mailbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fixing_mailbox/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.718028 bddl-3.1.0/bddl/activity_definitions/fold_a_cloth_napkin/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fold_a_cloth_napkin/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.718028 bddl-3.1.0/bddl/activity_definitions/fold_a_plastic_bag/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fold_a_plastic_bag/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.718028 bddl-3.1.0/bddl/activity_definitions/fold_a_tortilla/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fold_a_tortilla/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.718028 bddl-3.1.0/bddl/activity_definitions/fold_bandanas/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fold_bandanas/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.718028 bddl-3.1.0/bddl/activity_definitions/fold_towels/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fold_towels/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.718028 bddl-3.1.0/bddl/activity_definitions/folding_clean_laundry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/folding_clean_laundry/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.718028 bddl-3.1.0/bddl/activity_definitions/folding_clothes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/folding_clothes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.718028 bddl-3.1.0/bddl/activity_definitions/folding_piece_of_cloth/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/folding_piece_of_cloth/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.718028 bddl-3.1.0/bddl/activity_definitions/folding_sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/folding_sheets/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.718028 bddl-3.1.0/bddl/activity_definitions/freeze_fruit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/freeze_fruit/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.718028 bddl-3.1.0/bddl/activity_definitions/freeze_lasagna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/freeze_lasagna/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.718028 bddl-3.1.0/bddl/activity_definitions/freeze_meat/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/freeze_meat/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.722028 bddl-3.1.0/bddl/activity_definitions/freeze_pies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/freeze_pies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.722028 bddl-3.1.0/bddl/activity_definitions/freeze_quiche/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/freeze_quiche/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.722028 bddl-3.1.0/bddl/activity_definitions/freeze_vegetables/
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/freeze_vegetables/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.722028 bddl-3.1.0/bddl/activity_definitions/fry_pot_stickers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/fry_pot_stickers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.722028 bddl-3.1.0/bddl/activity_definitions/gathering_nuts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/gathering_nuts/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.722028 bddl-3.1.0/bddl/activity_definitions/getting_a_drink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/getting_a_drink/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.722028 bddl-3.1.0/bddl/activity_definitions/getting_organized_for_work/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/getting_organized_for_work/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.722028 bddl-3.1.0/bddl/activity_definitions/getting_package_from_post_office/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/getting_package_from_post_office/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.722028 bddl-3.1.0/bddl/activity_definitions/glaze_a_ham/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/glaze_a_ham/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.722028 bddl-3.1.0/bddl/activity_definitions/grease_and_flour_a_pan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/grease_and_flour_a_pan/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.722028 bddl-3.1.0/bddl/activity_definitions/grill_burgers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/grill_burgers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.722028 bddl-3.1.0/bddl/activity_definitions/grill_vegetables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/grill_vegetables/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.722028 bddl-3.1.0/bddl/activity_definitions/halve_an_egg/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/halve_an_egg/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.726028 bddl-3.1.0/bddl/activity_definitions/hand_washing_clothing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hand_washing_clothing/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.726028 bddl-3.1.0/bddl/activity_definitions/hang_a_bike_on_the_wall/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hang_a_bike_on_the_wall/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.726028 bddl-3.1.0/bddl/activity_definitions/hang_a_dartboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hang_a_dartboard/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.726028 bddl-3.1.0/bddl/activity_definitions/hang_a_hammock_indoors/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hang_a_hammock_indoors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.726028 bddl-3.1.0/bddl/activity_definitions/hang_a_rug_on_a_wall/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hang_a_rug_on_a_wall/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.726028 bddl-3.1.0/bddl/activity_definitions/hang_icicle_lights/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hang_icicle_lights/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.726028 bddl-3.1.0/bddl/activity_definitions/hang_paper_lanterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hang_paper_lanterns/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.726028 bddl-3.1.0/bddl/activity_definitions/hanging_address_numbers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hanging_address_numbers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.726028 bddl-3.1.0/bddl/activity_definitions/hanging_blinds/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hanging_blinds/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.726028 bddl-3.1.0/bddl/activity_definitions/hanging_clothes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hanging_clothes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.726028 bddl-3.1.0/bddl/activity_definitions/hanging_clothes_on_clothesline/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hanging_clothes_on_clothesline/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.726028 bddl-3.1.0/bddl/activity_definitions/hanging_flags/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hanging_flags/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.726028 bddl-3.1.0/bddl/activity_definitions/hanging_outdoor_lights/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hanging_outdoor_lights/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/hanging_pictures/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hanging_pictures/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/hanging_shades/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hanging_shades/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/hanging_up_bedsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hanging_up_bedsheets/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/hanging_up_curtains/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hanging_up_curtains/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/hanging_up_wind_chimes/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hanging_up_wind_chimes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/hard_boil_an_egg/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hard_boil_an_egg/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/heating_food_up/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/heating_food_up/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/hiding_Easter_eggs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hiding_Easter_eggs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/hoe_weeds/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/hoe_weeds/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/ice_cookies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/ice_cookies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/installing_a_fax_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/installing_a_fax_machine/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/installing_a_fence/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/installing_a_fence/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/installing_a_modem/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/installing_a_modem/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/installing_a_printer/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/installing_a_printer/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/installing_a_scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/installing_a_scanner/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.730028 bddl-3.1.0/bddl/activity_definitions/installing_a_trailer_hitch/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/installing_a_trailer_hitch/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.734028 bddl-3.1.0/bddl/activity_definitions/installing_alarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/installing_alarms/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.734028 bddl-3.1.0/bddl/activity_definitions/installing_carpet/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/installing_carpet/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.734028 bddl-3.1.0/bddl/activity_definitions/installing_smoke_detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/installing_smoke_detectors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.734028 bddl-3.1.0/bddl/activity_definitions/iron_a_tie/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/iron_a_tie/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.734028 bddl-3.1.0/bddl/activity_definitions/iron_curtains/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/iron_curtains/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.734028 bddl-3.1.0/bddl/activity_definitions/ironing_bedsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/ironing_bedsheets/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.734028 bddl-3.1.0/bddl/activity_definitions/ironing_clothes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/ironing_clothes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.734028 bddl-3.1.0/bddl/activity_definitions/ironing_curtains/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/ironing_curtains/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.734028 bddl-3.1.0/bddl/activity_definitions/lay_sod/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/lay_sod/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.734028 bddl-3.1.0/bddl/activity_definitions/laying_clothes_out/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/laying_clothes_out/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.734028 bddl-3.1.0/bddl/activity_definitions/laying_out_a_feast/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/laying_out_a_feast/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.734028 bddl-3.1.0/bddl/activity_definitions/laying_out_snacks_at_work/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/laying_out_snacks_at_work/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.734028 bddl-3.1.0/bddl/activity_definitions/laying_paving_stones/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/laying_paving_stones/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.734028 bddl-3.1.0/bddl/activity_definitions/laying_restaurant_table_for_dinner/
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/laying_restaurant_table_for_dinner/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.738028 bddl-3.1.0/bddl/activity_definitions/laying_tile_floors/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/laying_tile_floors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.738028 bddl-3.1.0/bddl/activity_definitions/laying_wood_floors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/laying_wood_floors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.738028 bddl-3.1.0/bddl/activity_definitions/lighting_fireplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/lighting_fireplace/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.738028 bddl-3.1.0/bddl/activity_definitions/line_kitchen_shelves/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/line_kitchen_shelves/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.738028 bddl-3.1.0/bddl/activity_definitions/loading_shopping_into_car/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/loading_shopping_into_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.738028 bddl-3.1.0/bddl/activity_definitions/loading_the_car/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/loading_the_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.738028 bddl-3.1.0/bddl/activity_definitions/loading_the_dishwasher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/loading_the_dishwasher/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.738028 bddl-3.1.0/bddl/activity_definitions/lube_a_bicycle_chain/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/lube_a_bicycle_chain/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.742028 bddl-3.1.0/bddl/activity_definitions/mailing_letters/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/mailing_letters/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.742028 bddl-3.1.0/bddl/activity_definitions/make_a_bake_sale_stand_stall/
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_bake_sale_stand_stall/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.742028 bddl-3.1.0/bddl/activity_definitions/make_a_basic_brine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_basic_brine/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.742028 bddl-3.1.0/bddl/activity_definitions/make_a_blended_iced_cappuccino/
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_blended_iced_cappuccino/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.742028 bddl-3.1.0/bddl/activity_definitions/make_a_candy_centerpiece/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_candy_centerpiece/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.742028 bddl-3.1.0/bddl/activity_definitions/make_a_cappuccino/
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_cappuccino/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.742028 bddl-3.1.0/bddl/activity_definitions/make_a_car_emergency_kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_car_emergency_kit/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.742028 bddl-3.1.0/bddl/activity_definitions/make_a_cheese_pastry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_cheese_pastry/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.742028 bddl-3.1.0/bddl/activity_definitions/make_a_chia_breakfast_bowl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_chia_breakfast_bowl/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.742028 bddl-3.1.0/bddl/activity_definitions/make_a_christmas_gift_box/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_christmas_gift_box/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.742028 bddl-3.1.0/bddl/activity_definitions/make_a_clothes_line/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_clothes_line/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.742028 bddl-3.1.0/bddl/activity_definitions/make_a_frappe/
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_frappe/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.742028 bddl-3.1.0/bddl/activity_definitions/make_a_lunch_box/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_lunch_box/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_a_military_care_package/
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_military_care_package/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_a_milkshake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_milkshake/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_a_mojito/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_mojito/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_a_red_meat_sauce/
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_red_meat_sauce/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_a_salad/
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_salad/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_a_sandwich/
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_sandwich/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_a_small_vegetable_garden/
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_small_vegetable_garden/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_a_steak/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_steak/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_a_strawberry_slushie/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_strawberry_slushie/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_a_sugar_and_coffee_scrub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_sugar_and_coffee_scrub/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_a_tropical_breakfast/
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_tropical_breakfast/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_a_vinegar_cleaning_solution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_vinegar_cleaning_solution/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_a_wiener_schnitzle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_a_wiener_schnitzle/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_an_egg_tomato_and_toast_breakfast/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_an_egg_tomato_and_toast_breakfast/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.746028 bddl-3.1.0/bddl/activity_definitions/make_an_iced_espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_an_iced_espresso/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.750028 bddl-3.1.0/bddl/activity_definitions/make_applesauce/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_applesauce/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.750028 bddl-3.1.0/bddl/activity_definitions/make_bagels/
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_bagels/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.750028 bddl-3.1.0/bddl/activity_definitions/make_baked_pears/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_baked_pears/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.750028 bddl-3.1.0/bddl/activity_definitions/make_batter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_batter/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.750028 bddl-3.1.0/bddl/activity_definitions/make_beef_and_broccoli/
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_beef_and_broccoli/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.750028 bddl-3.1.0/bddl/activity_definitions/make_bento/
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_bento/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.750028 bddl-3.1.0/bddl/activity_definitions/make_biscuits/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_biscuits/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.750028 bddl-3.1.0/bddl/activity_definitions/make_blueberry_mousse/
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_blueberry_mousse/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.750028 bddl-3.1.0/bddl/activity_definitions/make_brownies/
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_brownies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.750028 bddl-3.1.0/bddl/activity_definitions/make_burrito_bowls/
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_burrito_bowls/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.750028 bddl-3.1.0/bddl/activity_definitions/make_cabinet_doors/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_cabinet_doors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.750028 bddl-3.1.0/bddl/activity_definitions/make_cake_filling/
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_cake_filling/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.750028 bddl-3.1.0/bddl/activity_definitions/make_cake_mix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_cake_mix/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.750028 bddl-3.1.0/bddl/activity_definitions/make_chicken_and_waffles/
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_chicken_and_waffles/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_chicken_curry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_chicken_curry/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_chicken_fajitas/
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_chicken_fajitas/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_chocolate_biscuits/
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_chocolate_biscuits/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_chocolate_milk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_chocolate_milk/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_chocolate_spread/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_chocolate_spread/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_chocolate_syrup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_chocolate_syrup/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_cinnamon_sugar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_cinnamon_sugar/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_cinnamon_toast/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_cinnamon_toast/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_citrus_punch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_citrus_punch/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_coffee/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_coffee/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_cookie_dough/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_cookie_dough/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_cookies/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_cookies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_cream_from_milk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_cream_from_milk/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_cream_soda/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_cream_soda/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_curry_rice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_curry_rice/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_dessert_watermelons/
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_dessert_watermelons/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_dinner_rolls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_dinner_rolls/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.754028 bddl-3.1.0/bddl/activity_definitions/make_dinosaur_goody_bags/
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_dinosaur_goody_bags/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_edible_chocolate_chip_cookie_dough/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_edible_chocolate_chip_cookie_dough/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_eggnog/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_eggnog/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_fish_and_chips/
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_fish_and_chips/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_fried_rice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_fried_rice/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_fruit_punch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_fruit_punch/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_garlic_mushrooms/
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_garlic_mushrooms/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_gift_bags_for_baby_showers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_gift_bags_for_baby_showers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_granola/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_granola/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_green_tea_latte/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_green_tea_latte/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_homemade_bird_food/
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_homemade_bird_food/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_hot_cocoa/
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_hot_cocoa/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_ice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_ice/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_iced_chocolate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_iced_chocolate/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_iced_tea/
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_iced_tea/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_instant_coffee/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_instant_coffee/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_jamaican_jerk_seasoning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_jamaican_jerk_seasoning/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.758028 bddl-3.1.0/bddl/activity_definitions/make_king_prawns_with_garlic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_king_prawns_with_garlic/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_lemon_or_lime_water/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_lemon_or_lime_water/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_lemon_pepper_seasoning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_lemon_pepper_seasoning/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_lemon_pepper_wings/
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_lemon_pepper_wings/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_lemon_stain_remover/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_lemon_stain_remover/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_lemonade/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_lemonade/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_limeade/
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_limeade/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_macaroni_and_cheese/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_macaroni_and_cheese/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_meatloaf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_meatloaf/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_microwave_popcorn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_microwave_popcorn/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_muffins/
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_muffins/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_mustard_herb_and_spice_seasoning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_mustard_herb_and_spice_seasoning/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_nachos/
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_nachos/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_oatmeal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_oatmeal/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_onion_ring_batter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_onion_ring_batter/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_party_favors_from_candy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_party_favors_from_candy/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_pasta_sauce/
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_pasta_sauce/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_pastry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_pastry/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_pizza/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_pizza/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_pizza_dough/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_pizza_dough/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_pizza_sauce/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_pizza_sauce/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.762028 bddl-3.1.0/bddl/activity_definitions/make_popsicles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_popsicles/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_pumpkin_pie_spice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_pumpkin_pie_spice/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_red_beans_and_rice/
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_red_beans_and_rice/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_rose_centerpieces/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_rose_centerpieces/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_seafood_stew/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_seafood_stew/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_soup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_soup/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_spa_water/
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_spa_water/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_stew/
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_stew/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_stewed_fruit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_stewed_fruit/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_strawberries_and_cream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_strawberries_and_cream/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_tacos/
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_tacos/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_the_ultimate_spa_basket/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_the_ultimate_spa_basket/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_the_workplace_exciting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_the_workplace_exciting/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_toast/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_toast/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_tomato_rice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_tomato_rice/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_waffles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_waffles/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.766028 bddl-3.1.0/bddl/activity_definitions/make_watermelon_punch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_watermelon_punch/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/make_white_wine_sauce/
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_white_wine_sauce/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/make_yams/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/make_yams/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/making_a_drink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/making_a_drink/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/making_a_meal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/making_a_meal/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/making_a_snack/
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/making_a_snack/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/making_coffee/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/making_coffee/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/making_the_bed/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/making_the_bed/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/melt_white_chocolate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/melt_white_chocolate/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/mixing_drinks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/mixing_drinks/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/mopping_floors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/mopping_floors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/mopping_the_kitchen_floor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/mopping_the_kitchen_floor/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/moving_boxes_to_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/moving_boxes_to_storage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/moving_stuff_to_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/moving_stuff_to_storage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/mowing_the_lawn/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/mowing_the_lawn/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/mulching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/mulching/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/opening_doors/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/opening_doors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/opening_windows/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/opening_windows/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.770028 bddl-3.1.0/bddl/activity_definitions/organise_a_linen_closet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/organise_a_linen_closet/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/organizing_art_supplies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/organizing_art_supplies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/organizing_boxes_in_garage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/organizing_boxes_in_garage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/organizing_file_cabinet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/organizing_file_cabinet/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/organizing_items_for_yard_sale/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/organizing_items_for_yard_sale/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/organizing_office_documents/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/organizing_office_documents/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/organizing_school_stuff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/organizing_school_stuff/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/organizing_skating_stuff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/organizing_skating_stuff/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/organizing_volunteer_materials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/organizing_volunteer_materials/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/outfit_a_basic_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/outfit_a_basic_toolbox/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/pack_a_beach_bag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/pack_a_beach_bag/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/pack_a_pencil_case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/pack_a_pencil_case/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/pack_for_the_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/pack_for_the_pool/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/pack_your_gym_bag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/pack_your_gym_bag/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/packing_art_supplies_into_car/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_art_supplies_into_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/packing_bags_or_suitcase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_bags_or_suitcase/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.774028 bddl-3.1.0/bddl/activity_definitions/packing_books_into_car/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_books_into_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/packing_car_for_trip/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_car_for_trip/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/packing_cleaning_suppies_into_car/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_cleaning_suppies_into_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/packing_documents_into_car/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_documents_into_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/packing_fishing_gear_into_car/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_fishing_gear_into_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/packing_grocery_bags_into_car/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_grocery_bags_into_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/packing_hiking_equipment_into_car/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_hiking_equipment_into_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/packing_hobby_equipment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_hobby_equipment/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/packing_meal_for_delivery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_meal_for_delivery/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/packing_moving_van/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_moving_van/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/packing_picnic_food_into_car/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_picnic_food_into_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/packing_picnic_into_car/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_picnic_into_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/packing_recreational_vehicle_for_trip/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_recreational_vehicle_for_trip/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/packing_sports_equipment_into_car/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/packing_sports_equipment_into_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/painting_house_exterior/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/painting_house_exterior/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/painting_porch/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/painting_porch/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.778028 bddl-3.1.0/bddl/activity_definitions/passing_out_drinks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/passing_out_drinks/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/paying_for_purchases/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/paying_for_purchases/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/picking_fruit_and_vegetables/
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/picking_fruit_and_vegetables/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/picking_up_baggage/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/picking_up_baggage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/picking_up_books_at_library/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/picking_up_books_at_library/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/picking_up_clothes/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/picking_up_clothes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/picking_up_litter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/picking_up_litter/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/picking_up_prescriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/picking_up_prescriptions/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/picking_up_take_out_food/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/picking_up_take_out_food/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/picking_up_toys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/picking_up_toys/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/picking_up_trash/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/picking_up_trash/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/picking_vegetables_in_garden/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/picking_vegetables_in_garden/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/place_houseplants_around_your_home/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/place_houseplants_around_your_home/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/planting_flowers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/planting_flowers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/planting_plants/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/planting_plants/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/planting_trees/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/planting_trees/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/planting_vegetables/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/planting_vegetables/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.782028 bddl-3.1.0/bddl/activity_definitions/polish_a_car/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/polish_a_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/polish_copper/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/polish_copper/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/polish_cymbals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/polish_cymbals/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/polish_gold/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/polish_gold/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/polish_pewter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/polish_pewter/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/polish_rocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/polish_rocks/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/polish_wood_floors/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/polish_wood_floors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/polishing_furniture/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/polishing_furniture/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/polishing_shoes/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/polishing_shoes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/polishing_silver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/polishing_silver/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/pour_a_glass_of_wine/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/pour_a_glass_of_wine/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/pour_beer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/pour_beer/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/pouring_water_in_a_glass/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/pouring_water_in_a_glass/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/prepare_a_boat_for_fishing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_a_boat_for_fishing/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/prepare_a_breakfast_bar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_a_breakfast_bar/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/prepare_a_filling_breakfast/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_a_filling_breakfast/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/prepare_a_hanging_basket/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_a_hanging_basket/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/prepare_a_raised_bed_garden/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_a_raised_bed_garden/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.786028 bddl-3.1.0/bddl/activity_definitions/prepare_a_slow_dinner_party/
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_a_slow_dinner_party/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/prepare_an_emergency_school_kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_an_emergency_school_kit/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/prepare_and_cook_prawns/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_and_cook_prawns/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/prepare_and_cook_swiss_chard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_and_cook_swiss_chard/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/prepare_baking_pans/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_baking_pans/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/prepare_make_ahead_breakfast_bowls/
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_make_ahead_breakfast_bowls/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/prepare_quinoa/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_quinoa/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/prepare_sea_salt_soak/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_sea_salt_soak/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/prepare_wine_and_cheese/
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_wine_and_cheese/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/prepare_your_garden_for_a_cat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_your_garden_for_a_cat/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/prepare_your_garden_for_winter/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/prepare_your_garden_for_winter/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/preparing_clothes_for_the_next_day/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/preparing_clothes_for_the_next_day/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/preparing_existing_coffee/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/preparing_existing_coffee/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/preparing_food_for_a_fundraiser/
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/preparing_food_for_a_fundraiser/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/preparing_food_for_adult/
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/preparing_food_for_adult/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/preparing_food_for_company/
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/preparing_food_for_company/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/preparing_food_or_drink_for_sale/
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/preparing_food_or_drink_for_sale/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/preparing_lunch_box/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/preparing_lunch_box/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.790028 bddl-3.1.0/bddl/activity_definitions/preserving_fruit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/preserving_fruit/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/preserving_meat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/preserving_meat/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/preserving_vegetables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/preserving_vegetables/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/put_together_a_goodie_bag/
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/put_together_a_goodie_bag/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/put_together_a_scrapping_tool_kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/put_together_a_scrapping_tool_kit/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/put_togethera_basic_pruning_kit/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/put_togethera_basic_pruning_kit/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/putting_away_Christmas_decorations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_away_Christmas_decorations/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/putting_away_Halloween_decorations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_away_Halloween_decorations/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/putting_away_bicycles/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_away_bicycles/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/putting_away_cleaning_supplies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_away_cleaning_supplies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/putting_away_games/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_away_games/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/putting_away_purchased_clothes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_away_purchased_clothes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/putting_away_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_away_tools/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/putting_away_toys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_away_toys/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/putting_away_yard_equipment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_away_yard_equipment/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.794028 bddl-3.1.0/bddl/activity_definitions/putting_backpack_in_car_for_school/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_backpack_in_car_for_school/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_bike_in_garage/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_bike_in_garage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_birdseed_in_cage/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_birdseed_in_cage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_clean_laundry_away/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_clean_laundry_away/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_clothes_in_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_clothes_in_storage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_clothes_into_closet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_clothes_into_closet/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_dirty_dishes_in_sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_dirty_dishes_in_sink/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_dishes_away_after_cleaning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_dishes_away_after_cleaning/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_food_in_fridge/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_food_in_fridge/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_in_a_hot_tub/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_in_a_hot_tub/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_in_a_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_in_a_pool/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_laundry_in_drawer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_laundry_in_drawer/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_leftovers_away/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_leftovers_away/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_meal_in_fridge_at_work/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_meal_in_fridge_at_work/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_meal_on_plate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_meal_on_plate/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_on_license_plates/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_on_license_plates/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.798028 bddl-3.1.0/bddl/activity_definitions/putting_on_registration_stickers/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_on_registration_stickers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_on_tags_car/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_on_tags_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_out_cat_food/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_out_cat_food/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_out_clean_towels/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_out_clean_towels/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_out_condiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_out_condiments/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_out_dog_food/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_out_dog_food/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_pesticides_on_lawn/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_pesticides_on_lawn/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_protective_cover_on_vehicle/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_protective_cover_on_vehicle/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_roast_in_oven/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_roast_in_oven/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_shoes_on_rack/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_shoes_on_rack/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_shopping_away/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_shopping_away/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_tablecloth_on_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_tablecloth_on_table/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_towels_in_bathroom/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_towels_in_bathroom/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_up_Christmas_decorations_inside/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_up_Christmas_decorations_inside/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_up_Christmas_decorations_outside/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_up_Christmas_decorations_outside/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_up_Christmas_lights_inside/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_up_Christmas_lights_inside/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.802028 bddl-3.1.0/bddl/activity_definitions/putting_up_Christmas_lights_outside/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_up_Christmas_lights_outside/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/putting_up_outdoor_holiday_decorations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_up_outdoor_holiday_decorations/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/putting_up_posters/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_up_posters/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/putting_up_shelves/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_up_shelves/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/putting_up_wallpaper/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_up_wallpaper/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/putting_wood_in_fireplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/putting_wood_in_fireplace/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/raking_leaves/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/raking_leaves/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/re_shelving_library_books/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/re_shelving_library_books/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/rearrange_your_room/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/rearrange_your_room/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/rearranging_furniture/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/rearranging_furniture/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/rearranging_kitchen_furniture/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/rearranging_kitchen_furniture/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/recycling_glass_bottles/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/recycling_glass_bottles/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/recycling_newspapers/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/recycling_newspapers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/recycling_office_papers/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/recycling_office_papers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/reheat_frozen_or_chilled_food/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/reheat_frozen_or_chilled_food/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/remove_a_broken_light_bulb/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/remove_a_broken_light_bulb/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/remove_a_wall_mirror/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/remove_a_wall_mirror/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/remove_hard_water_spots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/remove_hard_water_spots/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.806028 bddl-3.1.0/bddl/activity_definitions/remove_scorch_marks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/remove_scorch_marks/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/remove_sod/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/remove_sod/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/remove_spots_from_linen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/remove_spots_from_linen/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/removing_ice_from_walkways/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/removing_ice_from_walkways/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/removing_lint_from_dryer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/removing_lint_from_dryer/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/repairs_to_furniture/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/repairs_to_furniture/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/returning_consumer_goods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/returning_consumer_goods/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/returning_videotapes_to_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/returning_videotapes_to_store/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/rinsing_dishes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/rinsing_dishes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/roast_meat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/roast_meat/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/roast_nuts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/roast_nuts/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/roast_vegetables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/roast_vegetables/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/sanding_wood_furniture/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sanding_wood_furniture/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/saute_vegetables/
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/saute_vegetables/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/scraping_snow_off_vehicle/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/scraping_snow_off_vehicle/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/scrubbing_bathroom_floor/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/scrubbing_bathroom_floor/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/selling_products_at_flea_market/
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/selling_products_at_flea_market/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/sending_packages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sending_packages/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/serving_food_at_a_homeless_shelter/
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/serving_food_at_a_homeless_shelter/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.810028 bddl-3.1.0/bddl/activity_definitions/serving_food_on_the_table/
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/serving_food_on_the_table/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/serving_hors_d_oeuvres/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/serving_hors_d_oeuvres/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/set_a_dinner_table/
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/set_a_dinner_table/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/set_a_fancy_table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/set_a_fancy_table/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/set_a_table_for_a_tea_party/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/set_a_table_for_a_tea_party/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/set_up_a_bird_cage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/set_up_a_bird_cage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/set_up_a_buffet/
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/set_up_a_buffet/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/set_up_a_coffee_station_in_your_kitchen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/set_up_a_coffee_station_in_your_kitchen/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/set_up_a_guinea_pig_cage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/set_up_a_guinea_pig_cage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/set_up_a_home_office_in_your_garage/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/set_up_a_home_office_in_your_garage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/set_up_a_hot_dog_bar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/set_up_a_hot_dog_bar/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/set_up_a_mouse_cage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/set_up_a_mouse_cage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/set_up_a_preschool_classroom/
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/set_up_a_preschool_classroom/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/set_up_a_webcam/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/set_up_a_webcam/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/setting_mousetraps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setting_mousetraps/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/setting_table_for_coffee/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setting_table_for_coffee/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/setting_the_fire/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setting_the_fire/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.814028 bddl-3.1.0/bddl/activity_definitions/setting_the_table/
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setting_the_table/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/setting_up_bedroom_for_guest/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setting_up_bedroom_for_guest/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/setting_up_for_an_event/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setting_up_for_an_event/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/setting_up_garden_furniture/
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setting_up_garden_furniture/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/setting_up_living_room_for_guest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setting_up_living_room_for_guest/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/setting_up_room_for_a_movie/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setting_up_room_for_a_movie/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/setting_up_room_for_games/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setting_up_room_for_games/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/setting_up_silent_auction/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setting_up_silent_auction/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/setting_up_toy_train_track/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setting_up_toy_train_track/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/setup_a_baby_crib/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setup_a_baby_crib/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/setup_a_bar_for_a_cocktail_party/
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setup_a_bar_for_a_cocktail_party/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/setup_a_fish_tank/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setup_a_fish_tank/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/setup_a_garden_party/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setup_a_garden_party/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/setup_a_trampoline/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/setup_a_trampoline/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/shampooing_carpet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/shampooing_carpet/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/shopping_at_warehouse_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/shopping_at_warehouse_stores/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/shoveling_coal/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/shoveling_coal/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/shoveling_snow/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/shoveling_snow/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/slicing_vegetables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/slicing_vegetables/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/sorting_art_supplies/
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sorting_art_supplies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.818028 bddl-3.1.0/bddl/activity_definitions/sorting_books_on_shelf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sorting_books_on_shelf/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/sorting_bottles_cans_and_paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sorting_bottles_cans_and_paper/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/sorting_clothes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sorting_clothes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/sorting_clothing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sorting_clothing/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/sorting_household_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sorting_household_items/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/sorting_items_for_garage_sale/
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sorting_items_for_garage_sale/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/sorting_laundry/
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sorting_laundry/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/sorting_mail/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sorting_mail/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/sorting_newspapers_for_recycling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sorting_newspapers_for_recycling/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/sorting_potatoes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sorting_potatoes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/sorting_vegetables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sorting_vegetables/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/sorting_volunteer_materials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sorting_volunteer_materials/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/spray_stucco/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/spray_stucco/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/spraying_for_bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/spraying_for_bugs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/spraying_fruit_trees/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/spraying_fruit_trees/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/spring_clean_your_skateboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/spring_clean_your_skateboard/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/stacking_wood/
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/stacking_wood/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/staining_wood_furniture/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/staining_wood_furniture/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/stash_snacks_in_your_room/
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/stash_snacks_in_your_room/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.822028 bddl-3.1.0/bddl/activity_definitions/stock_a_bar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/stock_a_bar/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/stock_a_bar_cart/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/stock_a_bar_cart/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/stock_grocery_shelves/
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/stock_grocery_shelves/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_a_fur_coat/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_a_fur_coat/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_a_kayak/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_a_kayak/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_a_quilt/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_a_quilt/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_an_uncooked_turkey/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_an_uncooked_turkey/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_baby_clothes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_baby_clothes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_baking_soda/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_baking_soda/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_batteries/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_batteries/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_beer/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_beer/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_bobby_pins/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_bobby_pins/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_brownies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_brownies/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_christmas_lights/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_christmas_lights/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_coffee_beans_or_ground_coffee/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_coffee_beans_or_ground_coffee/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_daffodil_bulbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_daffodil_bulbs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_feta_cheese/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_feta_cheese/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_firewood/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_firewood/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_firewood_outdoors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_firewood_outdoors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_honey/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_honey/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.826028 bddl-3.1.0/bddl/activity_definitions/store_loose_leaf_tea/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_loose_leaf_tea/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/store_nuts/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_nuts/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/store_produce/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_produce/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/store_rugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_rugs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/store_silver_coins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_silver_coins/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/store_tulip_bulbs/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_tulip_bulbs/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/store_vintage_linens/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_vintage_linens/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/store_vodka/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_vodka/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/store_whole_grains/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_whole_grains/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/store_winter_coats/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/store_winter_coats/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/storing_food/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/storing_food/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/stripping_furniture/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/stripping_furniture/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/sweeping_floors/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sweeping_floors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/sweeping_garage/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sweeping_garage/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/sweeping_outside_entrance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sweeping_outside_entrance/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/sweeping_patio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sweeping_patio/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/sweeping_porch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sweeping_porch/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/sweeping_steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/sweeping_steps/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/taking_clothes_off_of_the_drying_rack/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/taking_clothes_off_of_the_drying_rack/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.830028 bddl-3.1.0/bddl/activity_definitions/taking_clothes_off_the_line/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/taking_clothes_off_the_line/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/taking_clothes_out_of_the_dryer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/taking_clothes_out_of_the_dryer/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/taking_clothes_out_of_washer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/taking_clothes_out_of_washer/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/taking_down_curtains/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/taking_down_curtains/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/taking_fish_out_of_freezer/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/taking_fish_out_of_freezer/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/taking_trash_outside/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/taking_trash_outside/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/thaw_frozen_fish/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/thaw_frozen_fish/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/thawing_frozen_food/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/thawing_frozen_food/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/throwing_out_used_napkins/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/throwing_out_used_napkins/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/tidy_your_garden/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/tidy_your_garden/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/tidying_bathroom/
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/tidying_bathroom/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/tidying_bedroom/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/tidying_bedroom/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/tidying_living_room/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/tidying_living_room/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/tidying_up_wardrobe/
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/tidying_up_wardrobe/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/toast_buns/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/toast_buns/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/toast_coconut/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/toast_coconut/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/toast_sunflower_seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/toast_sunflower_seeds/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/treating_clothes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/treating_clothes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/treating_spot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/treating_spot/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/treating_stains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/treating_stains/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/turn_off_a_normal_school_calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/turn_off_a_normal_school_calculator/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/turning_off_the_hot_tub/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/turning_off_the_hot_tub/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.834028 bddl-3.1.0/bddl/activity_definitions/turning_on_radio/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/turning_on_radio/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/turning_on_the_hot_tub/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/turning_on_the_hot_tub/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/turning_out_all_lights_before_sleep/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/turning_out_all_lights_before_sleep/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/turning_sprinkler_off/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/turning_sprinkler_off/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/turning_sprinkler_on/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/turning_sprinkler_on/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/unhook_a_fish/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/unhook_a_fish/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/unloading_groceries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/unloading_groceries/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/unloading_shopping_from_car/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/unloading_shopping_from_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/unloading_shopping_items/
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/unloading_shopping_items/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/unloading_the_car/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/unloading_the_car/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/unpacking_car_for_trip/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/unpacking_car_for_trip/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/unpacking_childs_bag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/unpacking_childs_bag/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/unpacking_hobby_equipment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/unpacking_hobby_equipment/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/unpacking_moving_van/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/unpacking_moving_van/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/unpacking_recreational_vehicle_for_trip/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/unpacking_recreational_vehicle_for_trip/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/unpacking_suitcase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/unpacking_suitcase/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/vacuuming_floors/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/vacuuming_floors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/vacuuming_vehicles/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/vacuuming_vehicles/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.838028 bddl-3.1.0/bddl/activity_definitions/warm_tortillas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/warm_tortillas/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.842028 bddl-3.1.0/bddl/activity_definitions/wash_a_backpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_a_backpack/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.842028 bddl-3.1.0/bddl/activity_definitions/wash_a_baseball_cap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_a_baseball_cap/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.842028 bddl-3.1.0/bddl/activity_definitions/wash_a_bra/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_a_bra/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.842028 bddl-3.1.0/bddl/activity_definitions/wash_a_leotard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_a_leotard/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.842028 bddl-3.1.0/bddl/activity_definitions/wash_a_motorcycle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_a_motorcycle/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.842028 bddl-3.1.0/bddl/activity_definitions/wash_a_wool_coat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_a_wool_coat/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.842028 bddl-3.1.0/bddl/activity_definitions/wash_an_infant_car_seat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_an_infant_car_seat/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.842028 bddl-3.1.0/bddl/activity_definitions/wash_baby_bottles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_baby_bottles/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.842028 bddl-3.1.0/bddl/activity_definitions/wash_delicates_in_the_laundry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_delicates_in_the_laundry/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.842028 bddl-3.1.0/bddl/activity_definitions/wash_dog_toys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_dog_toys/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.842028 bddl-3.1.0/bddl/activity_definitions/wash_duvets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_duvets/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.842028 bddl-3.1.0/bddl/activity_definitions/wash_fruit_and_vegetables/
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_fruit_and_vegetables/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.842028 bddl-3.1.0/bddl/activity_definitions/wash_goalkeeper_gloves/
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_goalkeeper_gloves/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.842028 bddl-3.1.0/bddl/activity_definitions/wash_grapes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_grapes/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/wash_jeans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_jeans/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/wash_lettuce/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_lettuce/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/wash_towels/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_towels/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/wash_your_bike/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_your_bike/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/wash_your_rings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wash_your_rings/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/washing_bowls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/washing_bowls/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/washing_curtains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/washing_curtains/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/washing_fabrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/washing_fabrics/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/washing_floor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/washing_floor/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/washing_outside_walls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/washing_outside_walls/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/washing_outside_windows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/washing_outside_windows/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/washing_plates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/washing_plates/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/washing_pots_and_pans/
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/washing_pots_and_pans/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/washing_utensils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/washing_utensils/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/washing_vegetables/
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/washing_vegetables/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.846028 bddl-3.1.0/bddl/activity_definitions/washing_walls/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/washing_walls/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.850028 bddl-3.1.0/bddl/activity_definitions/washing_windows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/washing_windows/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.850028 bddl-3.1.0/bddl/activity_definitions/water_your_lawn_efficiently/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/water_your_lawn_efficiently/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.850028 bddl-3.1.0/bddl/activity_definitions/watering_indoor_flowers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/watering_indoor_flowers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.850028 bddl-3.1.0/bddl/activity_definitions/watering_outdoor_flowers/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/watering_outdoor_flowers/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.850028 bddl-3.1.0/bddl/activity_definitions/watering_outdoor_plants/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/watering_outdoor_plants/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.850028 bddl-3.1.0/bddl/activity_definitions/waxing_floors/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/waxing_floors/problem0.bddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.850028 bddl-3.1.0/bddl/activity_definitions/wrap_silverware/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_definitions/wrap_silverware/problem0.bddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_manifest.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/activity_to_preselected_scenes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/backend_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21793 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/condition_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.850028 bddl-3.1.0/bddl/data_generation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.850028 bddl-3.1.0/bddl/data_generation/WIP/
+-rw-r--r--   0 runner    (1001) docker     (123)    15058 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/data_generation/WIP/hierarchy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/data_generation/WIP/prune_object_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/data_generation/get_hierarchy_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/data_generation/get_syn_prop_annots_canonical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/data_generation/parse_tm_cleaning_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/data_generation/process_prop_param_annots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/data_generation/prop_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/data_generation/propagate_by_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/data_generation/pull_sheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/data_generation/run_everything.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.878028 bddl-3.1.0/bddl/generated_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/allowed_room_types.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   151239 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/category_mapping.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1174991 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/output_hierarchy.json
+-rw-r--r--   0 runner    (1001) docker     (123)  9947101 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/output_hierarchy_properties.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.882028 bddl-3.1.0/bddl/generated_data/prop_param_annots/
+-rw-r--r--   0 runner    (1001) docker     (123)   467045 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/prop_param_annots/coldSource.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   490194 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/prop_param_annots/cooking.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   468771 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/prop_param_annots/heatSource.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/prop_param_annots/particleApplier.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/prop_param_annots/particleSource.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   391506 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/prop_param_annots/tm_cleaning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1078634 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/propagated_annots_canonical.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1518384 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/propagated_annots_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1251007 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/properties_to_synsets.json
+-rw-r--r--   0 runner    (1001) docker     (123)   824340 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/remover_synset_mapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)    52579 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/substance_hyperparams.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/substance_synset_mapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)   906720 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/syn_prop_annots_canonical.json
+-rw-r--r--   0 runner    (1001) docker     (123)   190771 2023-08-03 21:07:39.000000 bddl-3.1.0/bddl/generated_data/synsets.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  2400085 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/synsets_to_descriptors.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.886028 bddl-3.1.0/bddl/generated_data/transition_map/
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/transition_map/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/transition_map/gen_transitionmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.886028 bddl-3.1.0/bddl/generated_data/transition_map/tm_jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/transition_map/tm_jsons/electric_mixer.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/transition_map/tm_jsons/heat_cook.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/transition_map/tm_jsons/mixing_stick.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/transition_map/tm_jsons/single_toggleable_machine.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.886028 bddl-3.1.0/bddl/generated_data/transition_map/tm_raw_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/transition_map/tm_raw_data/electric_mixer.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20550 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/transition_map/tm_raw_data/heat_cook.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/transition_map/tm_raw_data/mixing_stick.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/transition_map/tm_raw_data/single_toggleable_machine.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/transition_map/tm_submap_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.886028 bddl-3.1.0/bddl/generated_data/unresolved/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/unresolved/param_but_no_prop.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/unresolved/prop_but_no_param_or_malformed_param.json
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/generated_data/unresolved/synset_nonexistent.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/logic_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/object_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19899 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-08-03 21:07:40.000000 bddl-3.1.0/bddl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.570027 bddl-3.1.0/bddl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-08-03 21:07:53.000000 bddl-3.1.0/bddl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    64416 2023-08-03 21:07:53.000000 bddl-3.1.0/bddl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 21:07:53.000000 bddl-3.1.0/bddl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 21:07:52.000000 bddl-3.1.0/bddl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 21:07:53.000000 bddl-3.1.0/bddl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 21:07:53.000000 bddl-3.1.0/bddl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 21:07:53.886028 bddl-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-03 21:07:40.000000 bddl-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 21:07:53.886028 bddl-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-08-03 21:07:40.000000 bddl-3.1.0/tests/test_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16226 2023-08-03 21:07:40.000000 bddl-3.1.0/tests/test_utils.py
```

### Comparing `bddl-3.0.0b1/LICENSE` & `bddl-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bddl-3.0.0b1/PKG-INFO` & `bddl-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: bddl
-Version: 3.0.0b1
+Version: 3.1.0
 Home-page: https://github.com/StanfordVL/bddl
 Author: Stanford University
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Behavior Domain Definition Language 
 
-**Note: You are reading the docs for the 3.0.0b1 release, which is a backwards-incompatible version of BDDL containing a subset of BEHAVIOR-1K activities released as part of the BEHAVIOR-1K beta release. Please go to the tags menu to see BEHAVIOR-100 code and files.**
+**Note: You are reading the docs for the 3.1.0 release, which is a backwards-incompatible version of BDDL containing a subset of BEHAVIOR-1K activities released as part of the BEHAVIOR-1K beta release. Please go to the tags menu to see BEHAVIOR-100 code and files.**
 
 The Behavior Domain Definition Language (BDDL) is a domain-specific language designed for the Benchmark for Everyday Household Activities in Virtual, Interactive, and ecOlogical enviRonments (BEHAVIOR). 
 
 BDDL is a predicate logic-based language inspired by, but distinct from, the Planning Domain Definition Language [1]. It defines each BEHAVIOR activity definition as a BDDL `problem`, consisting of of a categorized object list (`:objects`), an initial condition that has only ground literals (`:init`), and a goal condition that is a logical expression (`:goal`). 
 
 ## Installation
```

### Comparing `bddl-3.0.0b1/README.md` & `bddl-3.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Behavior Domain Definition Language 
 
-**Note: You are reading the docs for the 3.0.0b1 release, which is a backwards-incompatible version of BDDL containing a subset of BEHAVIOR-1K activities released as part of the BEHAVIOR-1K beta release. Please go to the tags menu to see BEHAVIOR-100 code and files.**
+**Note: You are reading the docs for the 3.1.0 release, which is a backwards-incompatible version of BDDL containing a subset of BEHAVIOR-1K activities released as part of the BEHAVIOR-1K beta release. Please go to the tags menu to see BEHAVIOR-100 code and files.**
 
 The Behavior Domain Definition Language (BDDL) is a domain-specific language designed for the Benchmark for Everyday Household Activities in Virtual, Interactive, and ecOlogical enviRonments (BEHAVIOR). 
 
 BDDL is a predicate logic-based language inspired by, but distinct from, the Planning Domain Definition Language [1]. It defines each BEHAVIOR activity definition as a BDDL `problem`, consisting of of a categorized object list (`:objects`), an initial condition that has only ground literals (`:init`), and a goal condition that is a logical expression (`:goal`). 
 
 ## Installation
```

### Comparing `bddl-3.0.0b1/bddl/__init__.py` & `bddl-3.1.0/bddl/__init__.py`

 * *Files identical despite different names*

### Comparing `bddl-3.0.0b1/bddl/activity.py` & `bddl-3.1.0/bddl/activity.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-import bddl
+import os
+import re
 from bddl.condition_evaluation import (
     compile_state,
     create_scope,
     evaluate_state,
     get_ground_state_options,
 )
+from bddl.config import ACTIVITY_CONFIGS_PATH
 from bddl.object_taxonomy import ObjectTaxonomy
 from bddl.parsing import (
     gen_natural_language_condition,
     gen_natural_language_conditions,
     parse_domain,
     parse_problem,
 )
 
+INSTANCE_EXPR = re.compile(r"problem(\d+).bddl")
+
 
 class Conditions(object):
     def __init__(self, behavior_activity, activity_definition, simulator_name, predefined_problem=None):
         """Object to store behavior activity content and compile conditions for checking and
             simulator use
 
         Args:
@@ -46,15 +50,15 @@
     Returns:
         dict<str: None>: unpopulated scope with string keys to be mapped to
                             simulator object values
     """
     return create_scope(conds.parsed_objects)
 
 
-def get_initial_conditions(conds, backend, scope):
+def get_initial_conditions(conds, backend, scope, generate_ground_options=True):
     """Create compiled initial conditions that can be checked and sampled
 
     Args:
         conds (Conditions): conditions for the particular activity and definition
 
     Returns:
         list<bddl.condition_evaluation.HEAD>: compiled conditions if initial
@@ -63,34 +67,39 @@
     """
     if bool(conds.parsed_initial_conditions[0]):
         initial_conditions = compile_state(
             [cond for cond in conds.parsed_initial_conditions if cond[0] not in ["inroom"]],
             backend,
             scope=scope,
             object_map=conds.parsed_objects,
+            generate_ground_options=generate_ground_options
         )
         return initial_conditions
 
 
-def get_goal_conditions(conds, backend, scope):
+def get_goal_conditions(conds, backend, scope, generate_ground_options=True):
     """Create compiled goal conditions with a populated object scope for checking
 
     Args:
         conds (Conditions): conditions for the particular activity and definition
         populated_object_scope (dict<str: simulator object>): scope mapping object
                                                                 terms in BDDL to
                                                                 simulator objects
 
     Returns:
         list<bddl.condition_evaluation.HEAD>: compiled conditions if goal condition
                                                 definition is not empty else None
     """
     if bool(conds.parsed_goal_conditions[0]):
         goal_conditions = compile_state(
-            conds.parsed_goal_conditions, backend, scope=scope, object_map=conds.parsed_objects
+            conds.parsed_goal_conditions, 
+            backend, 
+            scope=scope, 
+            object_map=conds.parsed_objects,
+            generate_ground_options=generate_ground_options
         )
         return goal_conditions
 
 
 def get_ground_goal_state_options(conds, backend, scope, goal_conditions):
     """Create compiled ground solutions to goal state with a populated object scope
         for checking progress on specific solutions
@@ -146,7 +155,31 @@
     Args:
         conditions (list): conditions being translated
 
     Returns:
         list<str>: natural language translations, one per condition in conditions
     """
     return gen_natural_language_conditions(conds.parsed_goal_conditions)
+
+
+def get_all_activities():
+    """Return a list of all activities included in this version of BDDL.
+        
+    Returns:
+        list<str>: list containing the name of each included activity
+    """
+    return [x for x in os.listdir(ACTIVITY_CONFIGS_PATH) if os.path.isdir(os.path.join(ACTIVITY_CONFIGS_PATH, x))]
+
+
+def get_instance_count(act):
+    """Return the number of instances of a given activity that are included in this version of BDDL.
+    
+    Args:
+        act (str): name of the activity to check
+        
+    Returns:
+        int: number of instances of the given activity
+    """
+    problem_files = [INSTANCE_EXPR.fullmatch(x) for x in os.listdir(os.path.join(ACTIVITY_CONFIGS_PATH, act))]
+    ids = set(int(x.group(1)) for x in problem_files if x is not None)
+    assert ids == set(range(len(ids))), f"Non-contiguous instance IDs found for problem {act}"
+    return len(ids)
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/assembling_gift_baskets/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/collecting_childrens_toys/problem0.bddl`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,62 @@
-(define (problem assembling_gift_baskets_0)
-    (:domain igibson)
+(define (problem collecting_childrens_toys-0)
+    (:domain omnigibson)
 
     (:objects
-     	basket.n.01_1 basket.n.01_2 basket.n.01_3 basket.n.01_4 - basket.n.01
-    	floor.n.01_1 - floor.n.01
-    	candle.n.01_1 candle.n.01_2 candle.n.01_3 candle.n.01_4 - candle.n.01
-    	cookie.n.01_1 cookie.n.01_2 cookie.n.01_3 cookie.n.01_4 - cookie.n.01
-    	cheese.n.01_1 cheese.n.01_2 cheese.n.01_3 cheese.n.01_4 - cheese.n.01
-    	bow.n.08_1 bow.n.08_2 bow.n.08_3 bow.n.08_4 - bow.n.08
-        table.n.02_1 table.n.02_2 - table.n.02
+        die.n.01_1 die.n.01_2 - die.n.01
+        floor.n.01_1 - floor.n.01
+        teddy.n.01_1 teddy.n.01_2 - teddy.n.01
+        train_set.n.01_1 - train_set.n.01
+        board_game.n.01_1 board_game.n.01_2 - board_game.n.01
+        coffee_table.n.01_1 - coffee_table.n.01
+        shelf.n.01_1 - shelf.n.01
         agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (ontop basket.n.01_1 floor.n.01_1) 
-        (ontop basket.n.01_2 floor.n.01_1) 
-        (ontop basket.n.01_3 floor.n.01_1) 
-        (ontop basket.n.01_4 floor.n.01_1) 
-        (ontop candle.n.01_1 table.n.02_1) 
-        (ontop candle.n.01_2 table.n.02_1) 
-        (ontop candle.n.01_3 table.n.02_1) 
-        (ontop candle.n.01_4 table.n.02_1) 
-        (ontop cookie.n.01_1 table.n.02_1) 
-        (ontop cookie.n.01_2 table.n.02_1) 
-        (ontop cookie.n.01_3 table.n.02_1) 
-        (ontop cookie.n.01_4 table.n.02_1) 
-        (ontop cheese.n.01_1 table.n.02_2) 
-        (ontop cheese.n.01_2 table.n.02_2) 
-        (ontop cheese.n.01_3 table.n.02_2) 
-        (ontop cheese.n.01_4 table.n.02_2) 
-        (ontop bow.n.08_1 table.n.02_2) 
-        (ontop bow.n.08_2 table.n.02_2) 
-        (ontop bow.n.08_3 table.n.02_2) 
-        (ontop bow.n.08_4 table.n.02_2) 
+        (ontop die.n.01_1 floor.n.01_1) 
+        (ontop die.n.01_2 floor.n.01_1) 
+        (ontop teddy.n.01_1 floor.n.01_1) 
+        (ontop train_set.n.01_1 coffee_table.n.01_1) 
+        (ontop teddy.n.01_2 floor.n.01_1) 
+        (ontop board_game.n.01_1 coffee_table.n.01_1) 
+        (ontop board_game.n.01_2 floor.n.01_1) 
+        (inroom shelf.n.01_1 childs_room) 
         (inroom floor.n.01_1 living_room) 
-        (inroom table.n.02_1 living_room) 
-        (inroom table.n.02_2 living_room) 
+        (inroom coffee_table.n.01_1 living_room) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
-            (forpairs 
-                (?basket.n.01 - basket.n.01) 
-                (?candle.n.01 - candle.n.01) 
-                (inside ?candle.n.01 ?basket.n.01)
-            ) 
-            (forpairs 
-                (?basket.n.01 - basket.n.01) 
-                (?cheese.n.01 - cheese.n.01) 
-                (inside ?cheese.n.01 ?basket.n.01)
-            ) 
-            (forpairs 
-                (?basket.n.01 - basket.n.01) 
-                (?cookie.n.01 - cookie.n.01) 
-                (inside ?cookie.n.01 ?basket.n.01)
-            ) 
-            (forpairs 
-                (?basket.n.01 - basket.n.01) 
-                (?bow.n.08 - bow.n.08) 
-                (inside ?bow.n.08 ?basket.n.01)
+            (or 
+                (inside ?train_set.n.01_1 ?shelf.n.01_1)
+                (ontop ?train_set.n.01_1 ?shelf.n.01_1)
+            )
+            (forall
+                (?die.n.01 - die.n.01)
+                (or 
+                    (inside ?die.n.01 ?shelf.n.01_1)
+                    (ontop ?die.n.01 ?shelf.n.01_1)
+                )
+            )            
+            (forall
+                (?teddy.n.01 - teddy.n.01)
+                (or 
+                    (inside ?teddy.n.01 ?shelf.n.01_1)
+                    (ontop ?teddy.n.01 ?shelf.n.01_1)
+                )            
+            )
+            (forall
+                (?board_game.n.01 - board_game.n.01)
+                (or 
+                    (inside ?board_game.n.01 ?shelf.n.01_1)
+                    (ontop ?board_game.n.01 ?shelf.n.01_1)
+                )
+            )
+            (or
+                (inside ?train_set.n.01_1 ?shelf.n.01_1)
+                (ontop ?train_set.n.01_1 ?shelf.n.01_1)
             )
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/boxing_books_up_for_storage/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/boxing_books_up_for_storage/problem0.bddl`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem boxing_books_up_for_storage_0)
-    (:domain igibson)
+(define (problem boxing_books_up_for_storage-0)
+    (:domain omnigibson)
 
     (:objects
      	book.n.02_1 book.n.02_2 book.n.02_3 book.n.02_4 book.n.02_5 book.n.02_6 book.n.02_7 - book.n.02
     	floor.n.01_1 - floor.n.01
     	shelf.n.01_1 - shelf.n.01
     	carton.n.02_1 - carton.n.02
     	agent.n.01_1 - agent.n.01
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/bringing_in_wood/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/bringing_in_wood/problem0.bddl`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem bringing_in_wood_0)
-    (:domain igibson)
+(define (problem bringing_in_wood-0)
+    (:domain omnigibson)
 
     (:objects
         plywood.n.01_1 plywood.n.01_2 plywood.n.01_3 - plywood.n.01
         floor.n.01_1 floor.n.01_2 - floor.n.01
         agent.n.01_1 - agent.n.01
     )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/brushing_lint_off_clothing/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/brushing_lint_off_clothing/problem0.bddl`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem brushing_lint_off_clothing_0)
-    (:domain igibson)
+(define (problem brushing_lint_off_clothing-0)
+    (:domain omnigibson)
 
     (:objects
         dust.n.01_1 - dust.n.01
      	sweater.n.01_1 sweater.n.01_2 sweater.n.01_3 sweater.n.01_4 - sweater.n.01
     	floor.n.01_1 - floor.n.01
     	bed.n.01_1 - bed.n.01
     	scrub_brush.n.01_1 - scrub_brush.n.01
@@ -29,15 +29,15 @@
     )
     
     (:goal 
         (and 
             (forall 
                 (?sweater.n.01 - sweater.n.01) 
                 (not 
-                    (covered ?sweater.n.01 dust.n.01_1)
+                    (covered ?sweater.n.01 ?dust.n.01_1)
                 )
             ) 
             (forall 
                 (?sweater.n.01 - sweater.n.01) 
                 (ontop ?sweater.n.01 ?bed.n.01_1)
             )
         )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_barbecue_grill/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_barbecue_grill/problem0.bddl`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-(define (problem cleaning_barbecue_grill_0)
-    (:domain igibson)
+(define (problem cleaning_barbecue_grill-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
         dust.n.01_1 - dust.n.01
      	grill.n.02_1 - grill.n.02
     	floor.n.01_1 - floor.n.01
     	rag.n.01_1 - rag.n.01
     	bucket.n.01_1 - bucket.n.01
         table.n.02_1 - table.n.02
         sink.n.01_1 - sink.n.01
         agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (ontop grill.n.02_1 floor.n.01_1) 
+        (inroom grill.n.02_1 garage)
         (covered grill.n.02_1 stain.n.01_1) 
         (covered grill.n.02_1 dust.n.01_1) 
         (ontop bucket.n.01_1 table.n.02_1) 
         (ontop rag.n.01_1 table.n.02_1) 
         (inroom floor.n.01_1 garage) 
         (inroom table.n.02_1 storage_room) 
         (inroom sink.n.01_1 storage_room)
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (not 
-                (covered ?grill.n.02_1 stain.n.01_1)
+                (covered ?grill.n.02_1 ?stain.n.01_1)
             ) 
             (not 
-                (covered ?grill.n.02_1 dust.n.01_1)
+                (covered ?grill.n.02_1 ?dust.n.01_1)
             )
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_bathrooms/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/grease_and_flour_a_pan/problem0.bddl`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,42 @@
-(define (problem cleaning_bathrooms_0)
-    (:domain igibson)
+(define (problem grease_and_flour_a_pan-0)
+    (:domain omnigibson)
 
     (:objects
-        stain.n.01_1 - stain.n.01
+        cookie_sheet.n.01_1 - cookie_sheet.n.01
         sink.n.01_1 - sink.n.01
-        bathtub.n.01_1 - bathtub.n.01
-        toilet.n.02_1 - toilet.n.02
+        spatula.n.01_1 - spatula.n.01
+        tissue.n.02_1 - tissue.n.02
+        margarine.n.01_1 - margarine.n.01
+        margarine__box.n.01_1 - margarine__box.n.01
+        flour__sack.n.01_1 - flour__sack.n.01
+        flour.n.01_1 - flour.n.01
+        cabinet.n.01_1 - cabinet.n.01
+        countertop.n.01_1 - countertop.n.01
+        electric_refrigerator.n.01_1 - electric_refrigerator.n.01
         floor.n.01_1 - floor.n.01
-        bucket.n.01_1 - bucket.n.01
-        soap.n.01_1 - soap.n.01
-        brush.n.02_1 - brush.n.02
-        rag.n.01_1 - rag.n.01
         agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (covered sink.n.01_1 stain.n.01_1) 
-        (covered bathtub.n.01_1 stain.n.01_1) 
-        (covered toilet.n.02_1 stain.n.01_1) 
-        (covered floor.n.01_1 stain.n.01_1) 
-        (inside soap.n.01_1 sink.n.01_1) 
-        (inside brush.n.02_1 bathtub.n.01_1) 
-        (ontop bucket.n.01_1 floor.n.01_1) 
-        (ontop rag.n.01_1 floor.n.01_1) 
-        (ontop agent.n.01_1 floor.n.01_1) 
-        (inroom floor.n.01_1 bathroom) 
-        (inroom toilet.n.02_1 bathroom) 
-        (inroom sink.n.01_1 bathroom) 
-        (inroom bathtub.n.01_1 bathroom)
+        (inside cookie_sheet.n.01_1 cabinet.n.01_1) 
+        (inside spatula.n.01_1 cabinet.n.01_1) 
+        (ontop tissue.n.02_1 countertop.n.01_1)
+        (filled margarine__box.n.01_1 margarine.n.01_1) 
+        (filled flour__sack.n.01_1 flour.n.01_1) 
+        (inside margarine__box.n.01_1 electric_refrigerator.n.01_1) 
+        (inside flour__sack.n.01_1 cabinet.n.01_1) 
+        (inroom floor.n.01_1 kitchen) 
+        (inroom sink.n.01_1 kitchen) 
+        (inroom cabinet.n.01_1 kitchen) 
+        (inroom countertop.n.01_1 kitchen)
+        (inroom electric_refrigerator.n.01_1 kitchen)
+        (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
-            (not 
-                (covered ?toilet.n.02_1 stain.n.01_1)
-            ) 
-            (not 
-                (covered ?bathtub.n.01_1 stain.n.01_1)
-            ) 
-            (not 
-                (covered ?sink.n.01_1 stain.n.01_1)
-            ) 
-            (not 
-                (covered ?floor.n.01_1 stain.n.01_1)
-            ) 
-            (inside ?rag.n.01_1 ?bucket.n.01_1)
+            (covered ?cookie_sheet.n.01_1 ?margarine.n.01_1) 
+            (covered ?cookie_sheet.n.01_1 ?flour.n.01_1)
         )
     )
-)
+)
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_bathtub/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_bathtub/problem0.bddl`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-(define (problem cleaning_bathtub_0)
-    (:domain igibson)
+(define (problem cleaning_bathtub-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
+        water.n.06_1 - water.n.06
         sink.n.01_1 - sink.n.01
      	bathtub.n.01_1 - bathtub.n.01
-    	soap.n.01_1 - soap.n.01
+    	bar_soap.n.01_1 - bar_soap.n.01
     	floor.n.01_1 - floor.n.01
     	bucket.n.01_1 - bucket.n.01
     	scrub_brush.n.01_1 - scrub_brush.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
         (covered bathtub.n.01_1 stain.n.01_1) 
-        (ontop soap.n.01_1 floor.n.01_1) 
+        (ontop bar_soap.n.01_1 floor.n.01_1) 
         (ontop bucket.n.01_1 floor.n.01_1) 
         (inside scrub_brush.n.01_1 bathtub.n.01_1) 
+        (insource sink.n.01_1 water.n.06_1)
         (inroom floor.n.01_1 bathroom) 
         (inroom bathtub.n.01_1 bathroom) 
         (inroom sink.n.01_1 bathroom) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (not 
-                (covered ?bathtub.n.01_1 stain.n.01_1)
+                (covered ?bathtub.n.01_1 ?stain.n.01_1)
             )
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_bedroom/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_bedroom/problem0.bddl`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-(define (problem cleaning_bedroom_0)
-    (:domain igibson)
+(define (problem cleaning_bedroom-0)
+    (:domain omnigibson)
 
     (:objects
         dust.n.01_1 - dust.n.01
         floor.n.01_1 - floor.n.01
-        apparel.n.01_1 apparel.n.01_2 - apparel.n.01
+        jean.n.01_1 jean.n.01_2 - jean.n.01
         bed.n.01_1 - bed.n.01
         jewelry.n.01_1 - jewelry.n.01
-        perfume.n.02_1 - perfume.n.02
+        bottle__of__perfume.n.01_1 - bottle__of__perfume.n.01
         painting.n.01_1 - painting.n.01
         vacuum.n.04_1 - vacuum.n.04
         hand_towel.n.01_1 - hand_towel.n.01
         sheet.n.03_1 - sheet.n.03
         cabinet.n.01_1 cabinet.n.01_2 - cabinet.n.01
         agent.n.01_1 - agent.n.01
     )
     
     (:init 
         (covered cabinet.n.01_1 dust.n.01_1) 
         (covered cabinet.n.01_2 dust.n.01_1) 
-        (ontop apparel.n.01_1 bed.n.01_1) 
-        (ontop apparel.n.01_2 bed.n.01_1) 
+        (ontop jean.n.01_1 bed.n.01_1)
+        (ontop jean.n.01_2 bed.n.01_1)
         (ontop jewelry.n.01_1 floor.n.01_1) 
-        (ontop perfume.n.02_1 floor.n.01_1) 
+        (ontop bottle__of__perfume.n.01_1 floor.n.01_1)
         (ontop painting.n.01_1 bed.n.01_1) 
         (not 
             (covered vacuum.n.04_1 dust.n.01_1)
         ) 
         (ontop vacuum.n.04_1 floor.n.01_1) 
         (ontop hand_towel.n.01_1 floor.n.01_1)
         (ontop sheet.n.03_1 floor.n.01_1) 
@@ -36,23 +36,23 @@
         (inroom cabinet.n.01_2 bedroom) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (forall 
-                (?apparel.n.01 - apparel.n.01) 
+                (?jean.n.01 - jean.n.01)
                 (exists 
                     (?cabinet.n.01 - cabinet.n.01) 
-                    (inside ?apparel.n.01 ?cabinet.n.01)
+                    (inside ?jean.n.01 ?cabinet.n.01)
                 )
             ) 
             (and 
                 (inside ?jewelry.n.01_1 ?cabinet.n.01_1) 
-                (inside ?perfume.n.02_1 ?cabinet.n.01_1)
+                (inside ?bottle__of__perfume.n.01_1 ?cabinet.n.01_1)
             ) 
             (ontop ?sheet.n.03_1 ?bed.n.01_1) 
             (forall 
                 (?cabinet.n.01 - cabinet.n.01) 
                 (not 
                     (covered ?cabinet.n.01 dust.n.01_1)
                 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_carpets/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/filling_sugar/problem0.bddl`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,30 @@
-(define (problem cleaning_carpets_0)
-    (:domain igibson)
+(define (problem filling_sugar-0)
+    (:domain omnigibson)
 
     (:objects
-        stain.n.01_1 - stain.n.01
-     	floor.n.01_1 floor.n.01_2 - floor.n.01
-        hand_towel.n.01_1 - hand_towel.n.01
-    	shampoo.n.01_1 - shampoo.n.01
-    	cabinet.n.01_1 - cabinet.n.01
-    	washer.n.03_1 - washer.n.03
-    	dryer.n.01_1 - dryer.n.01
-    	door.n.01_1 - door.n.01
-        sink.n.01_1 - sink.n.01
-    	agent.n.01_1 - agent.n.01
+        bowl.n.01_1 - bowl.n.01
+        granulated_sugar.n.01_1 - granulated_sugar.n.01
+        sugar__sack.n.01_1 - sugar__sack.n.01
+        cabinet.n.01_1 - cabinet.n.01
+        teaspoon.n.02_1 - teaspoon.n.02
+        floor.n.01_1 - floor.n.01
+        agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (covered floor.n.01_1 stain.n.01_1) 
-        (ontop hand_towel.n.01_1 floor.n.01_2)
-        (inside shampoo.n.01_1 cabinet.n.01_1) 
-        (inroom floor.n.01_1 corridor) 
-        (inroom floor.n.01_2 utility_room) 
-        (inroom washer.n.03_1 utility_room) 
-        (inroom dryer.n.01_1 utility_room) 
-        (inroom door.n.01_1 corridor) 
-        (inroom cabinet.n.01_1 utility_room) 
-        (inroom sink.n.01_1 utility_room)
+        (inside bowl.n.01_1 cabinet.n.01_1) 
+        (filled sugar__sack.n.01_1 granulated_sugar.n.01_1) 
+        (inside sugar__sack.n.01_1 cabinet.n.01_1) 
+        (inside teaspoon.n.02_1 cabinet.n.01_1)
+        (inroom floor.n.01_1 kitchen) 
+        (inroom cabinet.n.01_1 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
-            (not 
-                (covered ?floor.n.01_1 stain.n.01_1)
-            )
+            (filled ?bowl.n.01_1 ?granulated_sugar.n.01_1)
+            (inside ?teaspoon.n.02_1 ?bowl.n.01_1)
         )
     )
-)
+)
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_floors/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/treating_spot/problem0.bddl`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-(define (problem cleaning_floors_0)
-    (:domain igibson)
+(define (problem treating_spot-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
-        dust.n.01_1 - dust.n.01
-     	floor.n.01_1 - floor.n.01
-    	broom.n.01_1 - broom.n.01
-    	dustpan.n.02_1 - dustpan.n.02
-    	cleansing_agent.n.01_1 - cleansing_agent.n.01
-    	scrub_brush.n.01_1 - scrub_brush.n.01
-    	door.n.01_1 - door.n.01
-    	sink.n.01_1 - sink.n.01
-    	agent.n.01_1 - agent.n.01
+        dress.n.01_1 - dress.n.01
+        sponge.n.01_1 - sponge.n.01
+        detergent.n.02_1 - detergent.n.02
+        detergent__bottle.n.01_1 - detergent__bottle.n.01
+        sink.n.01_1 - sink.n.01
+        water.n.06_1 - water.n.06
+        floor.n.01_1 - floor.n.01
+        agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (covered floor.n.01_1 dust.n.01_1) 
-        (covered floor.n.01_1 stain.n.01_1) 
-        (ontop broom.n.01_1 floor.n.01_1) 
-        (ontop dustpan.n.02_1 floor.n.01_1) 
-        (ontop cleansing_agent.n.01_1 floor.n.01_1) 
-        (ontop scrub_brush.n.01_1 floor.n.01_1) 
-        (inroom floor.n.01_1 bathroom) 
-        (inroom door.n.01_1 bathroom) 
+        (covered dress.n.01_1 stain.n.01_1) 
+        (ontop sponge.n.01_1 floor.n.01_1) 
+        (ontop dress.n.01_1 floor.n.01_1) 
+        (filled detergent__bottle.n.01_1 detergent.n.02_1)
+        (ontop detergent__bottle.n.01_1 floor.n.01_1)
+        (insource sink.n.01_1 water.n.06_1) 
         (inroom sink.n.01_1 bathroom) 
+        (inroom floor.n.01_1 bathroom) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (not 
-                (covered ?floor.n.01_1 stain.n.01_1)
+                (covered ?dress.n.01_1 ?stain.n.01_1)
             ) 
-            (not 
-                (covered ?floor.n.01_1 dust.n.01_1)
-            )
+            (covered ?dress.n.01_1 ?detergent.n.02_1)
         )
     )
-)
-
+)
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_freezer/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/prepare_a_filling_breakfast/problem0.bddl`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,57 @@
-(define (problem cleaning_freezer_0)
-    (:domain igibson)
+(define (problem prepare_a_filling_breakfast-0)
+    (:domain omnigibson)
 
     (:objects
-        stain.n.01_1 - stain.n.01
-     	electric_refrigerator.n.01_1 - electric_refrigerator.n.01
-    	food.n.01_1 food.n.01_2 food.n.01_3 - food.n.01
-    	cleansing_agent.n.01_1 - cleansing_agent.n.01
-    	table.n.02_1 - table.n.02
-    	towel.n.01_1 - towel.n.01
-    	floor.n.01_1 - floor.n.01
-    	sink.n.01_1 - sink.n.01
-    	countertop.n.01_1 - countertop.n.01
-    	stove.n.01_1 - stove.n.01
-    	door.n.01_1 - door.n.01
-    	chair.n.01_1 - chair.n.01
-    	agent.n.01_1 - agent.n.01
+        table_knife.n.01_1 - table_knife.n.01
+        countertop.n.01_1 - countertop.n.01
+        stove.n.01_1 - stove.n.01
+        egg.n.02_1 egg.n.02_2 - egg.n.02
+        frying_pan.n.01_1 - frying_pan.n.01
+        bratwurst.n.01_1 - bratwurst.n.01
+        carving_knife.n.01_1 - carving_knife.n.01
+        orange.n.01_1 - orange.n.01
+        half__orange.n.01_1 half__orange.n.01_2 - half__orange.n.01
+        plate.n.04_1 - plate.n.04
+        floor.n.01_1 - floor.n.01
+        electric_refrigerator.n.01_1 - electric_refrigerator.n.01
+        agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (covered electric_refrigerator.n.01_1 stain.n.01_1) 
-        (inside food.n.01_1 electric_refrigerator.n.01_1) 
-        (inside food.n.01_2 electric_refrigerator.n.01_1) 
-        (inside food.n.01_3 electric_refrigerator.n.01_1) 
-        (ontop cleansing_agent.n.01_1 table.n.02_1) 
-        (ontop towel.n.01_1 table.n.02_1) 
-        (inroom floor.n.01_1 kitchen) 
-        (inroom sink.n.01_1 kitchen) 
-        (inroom countertop.n.01_1 kitchen) 
+        (ontop table_knife.n.01_1 countertop.n.01_1) 
+        (inside egg.n.02_1 electric_refrigerator.n.01_1) 
+        (inside egg.n.02_2 electric_refrigerator.n.01_1) 
+        (inside bratwurst.n.01_1 electric_refrigerator.n.01_1) 
+        (ontop frying_pan.n.01_1 countertop.n.01_1) 
+        (inside orange.n.01_1 electric_refrigerator.n.01_1) 
+        (ontop plate.n.04_1 countertop.n.01_1)
+        (ontop carving_knife.n.01_1 countertop.n.01_1)
         (inroom stove.n.01_1 kitchen) 
+        (inroom countertop.n.01_1 kitchen) 
         (inroom electric_refrigerator.n.01_1 kitchen) 
-        (inroom door.n.01_1 kitchen) 
-        (inroom table.n.02_1 kitchen) 
-        (inroom chair.n.01_1 kitchen) 
+        (inroom floor.n.01_1 kitchen) 
+        (future half__orange.n.01_1)
+        (future half__orange.n.01_2)
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
-            (not 
-                (covered ?electric_refrigerator.n.01_1 stain.n.01_1)
-            ) 
+            (real ?half__orange.n.01_1)
+            (real ?half__orange.n.01_2)
+            (cooked ?bratwurst.n.01_1) 
             (forall 
-                (?food.n.01 - food.n.01) 
-                (not 
-                    (inside ?food.n.01 ?electric_refrigerator.n.01_1)
+                (?egg.n.02 - egg.n.02)
+                (and 
+                    (cooked ?egg.n.02)
+                    (ontop ?egg.n.02 ?plate.n.04_1)
                 )
             )
+            (ontop ?bratwurst.n.01_1 ?plate.n.04_1)
+            (forall 
+                (?half__orange.n.01 - half__orange.n.01)
+                (ontop ?half__orange.n.01 ?plate.n.04_1)
+            )
         )
     )
-)
+)
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_garage/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_garage/problem0.bddl`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,61 @@
-(define (problem cleaning_garage_0)
-    (:domain igibson)
+(define (problem cleaning_garage-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
         dust.n.01_1 - dust.n.01
-     	box.n.01_1 - box.n.01
     	floor.n.01_1 floor.n.01_2 - floor.n.01
     	newspaper.n.03_1 newspaper.n.03_2 - newspaper.n.03
     	bottle.n.01_1 bottle.n.01_2 - bottle.n.01
     	cabinet.n.01_1 - cabinet.n.01
     	broom.n.01_1 - broom.n.01
     	rag.n.01_1 - rag.n.01
     	table.n.02_1 - table.n.02
-    	bin.n.01_1 - bin.n.01
+    	recycling_bin.n.01_1 - recycling_bin.n.01
     	sink.n.01_1 - sink.n.01
     	shelf.n.01_1 - shelf.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (ontop box.n.01_1 floor.n.01_1) 
-        (ontop newspaper.n.03_1 floor.n.01_1) 
+        (ontop newspaper.n.03_1 floor.n.01_1)
         (ontop newspaper.n.03_2 floor.n.01_1) 
         (ontop bottle.n.01_1 floor.n.01_1) 
         (ontop bottle.n.01_2 floor.n.01_1) 
         (covered floor.n.01_1 dust.n.01_1) 
         (covered floor.n.01_1 stain.n.01_1) 
         (covered cabinet.n.01_1 dust.n.01_1) 
         (ontop broom.n.01_1 floor.n.01_1) 
         (ontop rag.n.01_1 table.n.02_1) 
-        (ontop bin.n.01_1 floor.n.01_1) 
+        (ontop recycling_bin.n.01_1 floor.n.01_1) 
         (inroom floor.n.01_1 garage) 
         (inroom cabinet.n.01_1 garage) 
         (inroom sink.n.01_1 storage_room) 
         (inroom shelf.n.01_1 storage_room) 
         (inroom table.n.02_1 storage_room) 
         (inroom floor.n.01_2 storage_room) 
         (ontop agent.n.01_1 floor.n.01_2)
     )
     
     (:goal 
         (and 
             (not 
-                (covered ?floor.n.01_1 dust.n.01_1)
+                (covered ?floor.n.01_1 ?dust.n.01_1)
             ) 
             (not 
-                (covered ?cabinet.n.01_1 dust.n.01_1)
+                (covered ?cabinet.n.01_1 ?dust.n.01_1)
             ) 
             (not 
-                (covered ?cabinet.n.01_1 stain.n.01_1)
+                (covered ?cabinet.n.01_1 ?stain.n.01_1)
             ) 
             (forall 
                 (?newspaper.n.03 - newspaper.n.03) 
                 (or 
-                    (inside ?newspaper.n.03 ?bin.n.01_1) 
+                    (inside ?newspaper.n.03 ?recycling_bin.n.01_1) 
                     (not 
                         (ontop ?newspaper.n.03 ?floor.n.01_1)
                     )
                 )
             ) 
             (forall 
                 (?bottle.n.01 - bottle.n.01)
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_high_chair/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_high_chair/problem0.bddl`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-(define (problem cleaning_high_chair_0)
-    (:domain igibson)
+(define (problem cleaning_high_chair-0)
+    (:domain omnigibson)
 
     (:objects
         dust.n.01_1 - dust.n.01
         highchair.n.01_1 - highchair.n.01
-        piece_of_cloth.n.01_1 - piece_of_cloth.n.01
+        hand_towel.n.01_1 - hand_towel.n.01
         cabinet.n.01_1 - cabinet.n.01
         floor.n.01_1 floor.n.01_2 - floor.n.01
         agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (covered highchair.n.01_1 dust.n.01_1) 
-        (inside piece_of_cloth.n.01_1 cabinet.n.01_1) 
-        (ontop highchair.n.01_1 floor.n.01_2) 
+        (covered highchair.n.01_1 dust.n.01_1)
+        (inside hand_towel.n.01_1 cabinet.n.01_1) 
+        (ontop highchair.n.01_1 floor.n.01_2)
         (inroom cabinet.n.01_1 kitchen) 
         (inroom floor.n.01_2 dining_room) 
         (inroom floor.n.01_1 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (not 
-                (covered ?highchair.n.01_1 dust.n.01_1)
+                (covered ?highchair.n.01_1 ?dust.n.01_1)
             )
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_kitchen_cupboard/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_kitchen_cupboard/problem0.bddl`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-(define (problem cleaning_kitchen_cupboard_0)
-    (:domain igibson)
+(define (problem cleaning_kitchen_cupboard-0)
+    (:domain omnigibson)
 
     (:objects
         dust.n.01_1 - dust.n.01
      	cabinet.n.01_1 cabinet.n.01_2 - cabinet.n.01
         countertop.n.01_1 - countertop.n.01
-    	piece_of_cloth.n.01_1 - piece_of_cloth.n.01
-    	cleansing_agent.n.01_1 - cleansing_agent.n.01
+    	hand_towel.n.01_1 - hand_towel.n.01
+    	detergent.n.02_1 - detergent.n.02
+    	detergent__bottle.n.01_1 - detergent__bottle.n.01
     	bowl.n.01_1 bowl.n.01_2 - bowl.n.01
     	cup.n.01_1 cup.n.01_2 - cup.n.01
     	floor.n.01_1 - floor.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
         (covered cabinet.n.01_1 dust.n.01_1) 
         (covered cabinet.n.01_2 dust.n.01_1) 
-        (ontop piece_of_cloth.n.01_1 countertop.n.01_1) 
-        (ontop cleansing_agent.n.01_1 countertop.n.01_1) 
+        (ontop hand_towel.n.01_1 countertop.n.01_1)
+        (filled detergent__bottle.n.01_1 detergent.n.02_1)
+        (ontop detergent__bottle.n.01_1 countertop.n.01_1)
         (inside bowl.n.01_2 cabinet.n.01_2) 
         (inside cup.n.01_1 cabinet.n.01_2) 
         (inside cup.n.01_2 cabinet.n.01_1) 
         (ontop bowl.n.01_1 countertop.n.01_1) 
         (inroom cabinet.n.01_1 kitchen) 
         (inroom cabinet.n.01_2 kitchen) 
         (inroom floor.n.01_1 kitchen) 
@@ -30,15 +32,15 @@
     )
     
     (:goal 
         (and 
             (forall 
                 (?cabinet.n.01 - cabinet.n.01) 
                 (not 
-                    (covered ?cabinet.n.01 dust.n.01_1)
+                    (covered ?cabinet.n.01 ?dust.n.01_1)
                 )
             ) 
             (exists 
                 (?cabinet.n.01 - cabinet.n.01) 
                 (forall 
                     (?bowl.n.01 - bowl.n.01) 
                     (and
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_microwave_oven/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_microwave_oven/problem0.bddl`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem cleaning_microwave_oven_0)
-    (:domain igibson)
+(define (problem cleaning_microwave_oven-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
         dust.n.01_1 - dust.n.01
      	microwave.n.02_1 - microwave.n.02
     	rag.n.01_1 - rag.n.01
     	countertop.n.01_1 - countertop.n.01
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_out_drawers/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_out_drawers/problem0.bddl`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-(define (problem cleaning_out_drawers_0)
-    (:domain igibson)
+(define (problem cleaning_out_drawers-0)
+    (:domain omnigibson)
 
     (:objects
      	bowl.n.01_1 bowl.n.01_2 - bowl.n.01
     	cabinet.n.01_1 cabinet.n.01_2 - cabinet.n.01
-    	spoon.n.01_1 spoon.n.01_2 - spoon.n.01
-    	piece_of_cloth.n.01_1 - piece_of_cloth.n.01
+    	tablespoon.n.02_1 tablespoon.n.02_2 - tablespoon.n.02
+    	dinner_napkin.n.01_1 - dinner_napkin.n.01
     	sink.n.01_1 - sink.n.01
     	floor.n.01_1 - floor.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
         (inside bowl.n.01_1 cabinet.n.01_1) 
         (inside bowl.n.01_2 cabinet.n.01_1) 
-        (inside spoon.n.01_1 cabinet.n.01_2) 
-        (inside spoon.n.01_2 cabinet.n.01_2) 
-        (inside piece_of_cloth.n.01_1 cabinet.n.01_1) 
+        (inside tablespoon.n.02_1 cabinet.n.01_2) 
+        (inside tablespoon.n.02_2 cabinet.n.01_2) 
+        (inside dinner_napkin.n.01_1 cabinet.n.01_1) 
         (inroom cabinet.n.01_1 kitchen) 
         (inroom cabinet.n.01_2 kitchen) 
         (inroom sink.n.01_1 kitchen) 
         (inroom floor.n.01_1 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
-            (nextto ?piece_of_cloth.n.01_1 ?sink.n.01_1) 
+            (nextto ?dinner_napkin.n.01_1 ?sink.n.01_1) 
             (nextto ?bowl.n.01_1 ?sink.n.01_1) 
             (nextto ?bowl.n.01_2 ?sink.n.01_1) 
-            (nextto ?spoon.n.01_1 ?sink.n.01_1) 
-            (nextto ?spoon.n.01_2 ?sink.n.01_1)
+            (nextto ?tablespoon.n.02_1 ?sink.n.01_1) 
+            (nextto ?tablespoon.n.02_2 ?sink.n.01_1)
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_oven/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/boil_water/problem0.bddl`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,33 @@
-(define (problem cleaning_oven_0)
-    (:domain igibson)
+(define (problem boil_water-0)
+    (:domain omnigibson)
 
     (:objects
-        stain.n.01_1 - stain.n.01
-     	receptacle.n.01_1 - receptacle.n.01
-    	floor.n.01_1 - floor.n.01
-    	soap.n.01_1 - soap.n.01
-    	cabinet.n.01_1 - cabinet.n.01
-    	rag.n.01_1 rag.n.01_2 - rag.n.01
-    	newspaper.n.03_1 - newspaper.n.03
-    	sink.n.01_1 - sink.n.01
-    	scrub_brush.n.01_1 - scrub_brush.n.01
-    	oven.n.01_1 - oven.n.01
-    	agent.n.01_1 - agent.n.01
+        stove.n.01_1 - stove.n.01
+        kettle.n.01_1 - kettle.n.01
+        sink.n.01_1 - sink.n.01
+        cabinet.n.01_1 - cabinet.n.01
+        water.n.06_1 - water.n.06
+        cooked__water.n.01_1 - cooked__water.n.01
+        floor.n.01_1 - floor.n.01
+        agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (ontop receptacle.n.01_1 floor.n.01_1) 
-        (inside soap.n.01_1 cabinet.n.01_1) 
-        (inside rag.n.01_1 cabinet.n.01_1) 
-        (inside rag.n.01_2 cabinet.n.01_1) 
-        (ontop newspaper.n.03_1 floor.n.01_1) 
-        (inside scrub_brush.n.01_1 cabinet.n.01_1) 
-        (covered oven.n.01_1 stain.n.01_1) 
-        (inroom oven.n.01_1 kitchen) 
-        (inroom cabinet.n.01_1 kitchen) 
+        (inside kettle.n.01_1 cabinet.n.01_1) 
+        (filled kettle.n.01_1 water.n.06_1) 
+        (insource sink.n.01_1 water.n.06_1) 
+        (inroom floor.n.01_1 kitchen)
         (inroom sink.n.01_1 kitchen) 
-        (inroom floor.n.01_1 kitchen) 
+        (inroom cabinet.n.01_1 kitchen) 
+        (inroom stove.n.01_1 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
+        (future cooked__water.n.01_1)
     )
     
     (:goal 
         (and 
-            (not 
-                (covered ?oven.n.01_1 stain.n.01_1)
-            )
+            (real ?cooked__water.n.01_1)
+            (filled ?kettle.n.01_1 ?cooked__water.n.01_1) 
         )
     )
-)
+)
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_shoes/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/wash_a_leotard/problem0.bddl`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,63 @@
-(define (problem cleaning_shoes_0)
-    (:domain igibson)
+(define (problem wash_a_leotard-0)
+    (:domain omnigibson)
 
     (:objects
-        stain.n.01_1 - stain.n.01
-        dust.n.01_1 - dust.n.01
-     	soap.n.01_1 - soap.n.01
-    	bed.n.01_1 - bed.n.01
-    	floor.n.01_1 - floor.n.01
-    	rag.n.01_1 - rag.n.01
-    	towel.n.01_1 - towel.n.01
-    	shoe.n.01_1 shoe.n.01_2 shoe.n.01_3 shoe.n.01_4 - shoe.n.01
+        leotard.n.01_1 - leotard.n.01
         sink.n.01_1 - sink.n.01
-    	agent.n.01_1 - agent.n.01
+        stain.n.01_1 - stain.n.01
+        tights.n.01_1 - tights.n.01
+        hanger.n.02_1 hanger.n.02_2 - hanger.n.02
+        hamper.n.02_1 - hamper.n.02
+        detergent.n.02_1 - detergent.n.02
+        detergent__bottle.n.01_1 - detergent__bottle.n.01
+        wardrobe.n.01_1 - wardrobe.n.01
+        scrub_brush.n.01_1 - scrub_brush.n.01
+        water.n.06_1 - water.n.06
+        floor.n.01_1 floor.n.01_2 - floor.n.01
+        agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (ontop soap.n.01_1 bed.n.01_1) 
-        (ontop rag.n.01_1 bed.n.01_1) 
-        (ontop towel.n.01_1 floor.n.01_1) 
-        (ontop shoe.n.01_1 bed.n.01_1) 
-        (ontop shoe.n.01_2 bed.n.01_1) 
-        (ontop shoe.n.01_3 bed.n.01_1) 
-        (ontop shoe.n.01_4 bed.n.01_1) 
-        (covered shoe.n.01_1 stain.n.01_1) 
-        (covered shoe.n.01_2 stain.n.01_1) 
-        (covered shoe.n.01_3 dust.n.01_1) 
-        (covered shoe.n.01_4 dust.n.01_1) 
+        (ontop hamper.n.02_1 floor.n.01_1)
+        (inside leotard.n.01_1 hamper.n.02_1) 
+        (covered leotard.n.01_1 stain.n.01_1) 
+        (inside tights.n.01_1 hamper.n.02_1) 
+        (covered tights.n.01_1 stain.n.01_1) 
+        (attached hanger.n.02_1 wardrobe.n.01_1) 
+        (attached hanger.n.02_2 wardrobe.n.01_1) 
+        (filled detergent__bottle.n.01_1 detergent.n.02_1) 
+        (ontop detergent__bottle.n.01_1 floor.n.01_2) 
+        (insource sink.n.01_1 water.n.06_1) 
+        (ontop wardrobe.n.01_1 floor.n.01_1)
+        (ontop scrub_brush.n.01_1 floor.n.01_2)
         (inroom floor.n.01_1 bedroom) 
-        (inroom bed.n.01_1 bedroom) 
-        (inroom sink.n.01_1 bathroom)
+        (inroom floor.n.01_2 bathroom) 
+        (inroom sink.n.01_1 bathroom) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
-            (forall 
-                (?shoe.n.01 - shoe.n.01) 
-                (not 
-                    (covered ?shoe.n.01 stain.n.01_1)
-                )
+            (not 
+                (covered ?leotard.n.01_1 ?stain.n.01_1)
             ) 
-            (forall 
-                (?shoe.n.01 - shoe.n.01) 
-                (not 
-                    (covered ?shoe.n.01 dust.n.01_1)
-                )
+            (not 
+                (covered ?tights.n.01_1 ?stain.n.01_1)
             ) 
-            (ontop ?towel.n.01_1 ?floor.n.01_1)
+            (exists 
+                (?hanger.n.02 - hanger.n.02)
+                (and
+                    (draped ?leotard.n.01_1 ?hanger.n.02)
+                    (attached ?hanger.n.02 ?wardrobe.n.01_1)
+                )
+            )
+            (exists 
+                (?hanger.n.02 - hanger.n.02)
+                (and
+                    (draped ?tights.n.01_1 ?hanger.n.02)
+                    (attached ?hanger.n.02 ?wardrobe.n.01_1)
+                )
+            )
         )
     )
-)
-
+)
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_sneakers/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_sneakers/problem0.bddl`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-(define (problem cleaning_sneakers_0)
-    (:domain igibson)
+(define (problem cleaning_sneakers-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
         dust.n.01_1 - dust.n.01
      	gym_shoe.n.01_1 gym_shoe.n.01_2 gym_shoe.n.01_3 gym_shoe.n.01_4 - gym_shoe.n.01
             countertop.n.01_1 - countertop.n.01
-            soap.n.01_1 - soap.n.01
+            bar_soap.n.01_1 - bar_soap.n.01
             cabinet.n.01_1 - cabinet.n.01
             towel.n.01_1 - towel.n.01
-            brush.n.02_1 - brush.n.02
+            scrub_brush.n.01_1 - scrub_brush.n.01
             sink.n.01_1 - sink.n.01
             floor.n.01_1 floor.n.01_2 - floor.n.01
             table.n.02_1 - table.n.02
             agent.n.01_1 - agent.n.01
     )
     
     (:init 
@@ -21,37 +21,37 @@
         (covered gym_shoe.n.01_1 stain.n.01_1) 
         (ontop gym_shoe.n.01_2 floor.n.01_2) 
         (covered gym_shoe.n.01_2 stain.n.01_1) 
         (ontop gym_shoe.n.01_3 floor.n.01_2) 
         (covered gym_shoe.n.01_3 dust.n.01_1) 
         (ontop gym_shoe.n.01_4 floor.n.01_2) 
         (covered gym_shoe.n.01_4 dust.n.01_1) 
-        (inside soap.n.01_1 cabinet.n.01_1) 
+        (inside bar_soap.n.01_1 cabinet.n.01_1) 
         (ontop towel.n.01_1 countertop.n.01_1) 
         (not 
             (covered towel.n.01_1 stain.n.01_1)
         ) 
-        (ontop brush.n.02_1 countertop.n.01_1) 
+        (ontop scrub_brush.n.01_1 countertop.n.01_1)
         (not 
-            (covered brush.n.02_1 stain.n.01_1)
+            (covered scrub_brush.n.01_1 stain.n.01_1)
         ) 
         (inroom sink.n.01_1 kitchen) 
         (inroom countertop.n.01_1 kitchen) 
         (inroom cabinet.n.01_1 kitchen) 
         (inroom floor.n.01_1 living_room) 
         (inroom table.n.02_1 living_room) 
         (inroom floor.n.01_2 kitchen) 
         (ontop agent.n.01_1 floor.n.01_2)
     )
     
     (:goal 
         (and 
             (ontop ?towel.n.01_1 ?countertop.n.01_1) 
-            (nextto ?brush.n.02_1 ?towel.n.01_1) 
-            (inside ?soap.n.01_1 ?sink.n.01_1) 
+            (inside ?bar_soap.n.01_1 ?sink.n.01_1) 
+            (nextto ?scrub_brush.n.01_1 ?towel.n.01_1)
             (forall 
                 (?gym_shoe.n.01 - gym_shoe.n.01) 
                 (not 
                     (covered ?gym_shoe.n.01 dust.n.01_1)
                 )
             ) 
             (forall
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_stove/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_stove/problem0.bddl`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-(define (problem cleaning_stove_0)
-    (:domain igibson)
+(define (problem cleaning_stove-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
         dust.n.01_1 - dust.n.01
      	stove.n.01_1 - stove.n.01
-    	soap.n.01_1 - soap.n.01
+    	bar_soap.n.01_1 - bar_soap.n.01
     	cabinet.n.01_1 - cabinet.n.01
     	rag.n.01_1 - rag.n.01
     	sink.n.01_1 - sink.n.01
     	dishtowel.n.01_1 - dishtowel.n.01
         floor.n.01_1 - floor.n.01
         agent.n.01_1 - agent.n.01
     )
     
     (:init 
         (covered stove.n.01_1 dust.n.01_1) 
         (covered stove.n.01_1 stain.n.01_1) 
-        (inside soap.n.01_1 cabinet.n.01_1) 
+        (inside bar_soap.n.01_1 cabinet.n.01_1) 
         (inside rag.n.01_1 cabinet.n.01_1) 
         (inside dishtowel.n.01_1 cabinet.n.01_1) 
         (inroom sink.n.01_1 kitchen) 
         (inroom stove.n.01_1 kitchen) 
         (inroom cabinet.n.01_1 kitchen) 
         (inroom floor.n.01_1 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (not 
-                (covered ?stove.n.01_1 dust.n.01_1)
+                (covered ?stove.n.01_1 ?dust.n.01_1)
             ) 
             (not 
-                (covered ?stove.n.01_1 stain.n.01_1)
+                (covered ?stove.n.01_1 ?stain.n.01_1)
             ) 
             (nextto ?rag.n.01_1 ?sink.n.01_1) 
             (nextto ?dishtowel.n.01_1 ?sink.n.01_1)
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_table_after_clearing/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_table_after_clearing/problem0.bddl`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-(define (problem cleaning_table_after_clearing_0)
-    (:domain igibson)
+(define (problem cleaning_table_after_clearing-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
      	table.n.02_1 - table.n.02
-    	soap.n.01_1 - soap.n.01
+    	bar_soap.n.01_1 - bar_soap.n.01
     	sink.n.01_1 - sink.n.01
     	floor.n.01_1 - floor.n.01
             dishtowel.n.01_1 - dishtowel.n.01
             cabinet.n.01_1 - cabinet.n.01
             agent.n.01_1 - agent.n.01
     )
     
     (:init 
         (covered table.n.02_1 stain.n.01_1) 
-        (inside soap.n.01_1 cabinet.n.01_1) 
+        (inside bar_soap.n.01_1 cabinet.n.01_1) 
         (inside dishtowel.n.01_1 cabinet.n.01_1) 
         (inroom table.n.02_1 dining_room) 
         (inroom floor.n.01_1 dining_room) 
         (inroom cabinet.n.01_1 kitchen) 
         (inroom sink.n.01_1 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_the_hot_tub/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_the_hot_tub/problem0.bddl`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-(define (problem cleaning_the_hot_tub_0)
-    (:domain igibson)
+(define (problem cleaning_the_hot_tub-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
      	pool.n.01_1 - pool.n.01
     	floor.n.01_1 - floor.n.01
     	scrub_brush.n.01_1 - scrub_brush.n.01
         sink.n.01_1 - sink.n.01
     	agent.n.01_1 - agent.n.01
     )
-    
-    (:init 
-        (ontop pool.n.01_1 floor.n.01_1) 
-        (covered pool.n.01_1 stain.n.01_1) 
-        (ontop scrub_brush.n.01_1 floor.n.01_1) 
-        (inroom floor.n.01_1 garage) 
+
+    (:init
+        (inroom pool.n.01_1 garden)
+        (covered pool.n.01_1 stain.n.01_1)
+        (ontop scrub_brush.n.01_1 floor.n.01_1)
+        (inroom floor.n.01_1 garage)
         (inroom sink.n.01_1 bathroom)
         (ontop agent.n.01_1 floor.n.01_1)
     )
-    
-    (:goal 
-        (and 
-            (ontop ?pool.n.01_1 ?floor.n.01_1) 
-            (not 
-                (covered ?pool.n.01_1 stain.n.01_1)
+
+    (:goal
+        (and
+            (not
+                (covered ?pool.n.01_1 ?stain.n.01_1)
             )
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_the_pool/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_the_pool/problem0.bddl`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-(define (problem cleaning_the_pool_0)
-    (:domain igibson)
+(define (problem cleaning_the_pool-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
      	pool.n.01_1 - pool.n.01
     	floor.n.01_1 - floor.n.01
     	scrub_brush.n.01_1 - scrub_brush.n.01
     	shelf.n.01_1 - shelf.n.01
     	detergent.n.02_1 - detergent.n.02
+    	detergent__bottle.n.01_1 - detergent__bottle.n.01
         sink.n.01_1 - sink.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (ontop pool.n.01_1 floor.n.01_1) 
+        (inroom pool.n.01_1 garden)
         (covered pool.n.01_1 stain.n.01_1) 
-        (ontop scrub_brush.n.01_1 floor.n.01_1) 
-        (ontop detergent.n.02_1 floor.n.01_1) 
+        (ontop scrub_brush.n.01_1 floor.n.01_1)
+        (filled detergent__bottle.n.01_1 detergent.n.02_1)
+        (ontop detergent__bottle.n.01_1 floor.n.01_1)
         (inroom shelf.n.01_1 garage) 
         (inroom floor.n.01_1 garage) 
         (inroom sink.n.01_1 storage_room)
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (ontop ?pool.n.01_1 ?floor.n.01_1) 
             (not 
-                (covered ?pool.n.01_1 stain.n.01_1)
+                (covered ?pool.n.01_1 ?stain.n.01_1)
             ) 
             (ontop ?scrub_brush.n.01_1 ?shelf.n.01_1) 
-            (ontop ?detergent.n.02_1 ?floor.n.01_1)
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_toilet/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_floors/problem0.bddl`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,43 @@
-(define (problem cleaning_toilet_0)
-    (:domain igibson)
+(define (problem cleaning_floors-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
-     	toilet.n.02_1 - toilet.n.02
+        dust.n.01_1 - dust.n.01
+     	floor.n.01_1 - floor.n.01
+    	broom.n.01_1 - broom.n.01
+    	dustpan.n.02_1 - dustpan.n.02
+        detergent.n.02_1 - detergent.n.02
+        detergent__bottle.n.01_1 - detergent__bottle.n.01
     	scrub_brush.n.01_1 - scrub_brush.n.01
-    	floor.n.01_1 - floor.n.01
-    	detergent.n.02_1 - detergent.n.02
-        sink.n.01_1 - sink.n.01
+    	door.n.01_1 - door.n.01
+    	sink.n.01_1 - sink.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (covered toilet.n.02_1 stain.n.01_1) 
+        (covered floor.n.01_1 dust.n.01_1) 
+        (covered floor.n.01_1 stain.n.01_1) 
+        (ontop broom.n.01_1 floor.n.01_1) 
+        (ontop dustpan.n.02_1 floor.n.01_1) 
+        (filled detergent__bottle.n.01_1 detergent.n.02_1)
+        (ontop detergent__bottle.n.01_1 floor.n.01_1)
         (ontop scrub_brush.n.01_1 floor.n.01_1) 
-        (ontop detergent.n.02_1 floor.n.01_1) 
-        (inroom toilet.n.02_1 bathroom) 
         (inroom floor.n.01_1 bathroom) 
-        (inroom sink.n.01_1 bathroom)
+        (inroom door.n.01_1 bathroom) 
+        (inroom sink.n.01_1 bathroom) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (not 
-                (covered ?toilet.n.02_1 stain.n.01_1)
+                (covered ?floor.n.01_1 ?stain.n.01_1)
             ) 
-            (ontop ?scrub_brush.n.01_1 ?floor.n.01_1) 
-            (ontop ?detergent.n.02_1 ?floor.n.01_1)
+            (not 
+                (covered ?floor.n.01_1 ?dust.n.01_1)
+            )
         )
     )
 )
+
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_up_after_a_meal/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_up_after_a_meal/problem0.bddl`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-(define (problem cleaning_up_after_a_meal_0)
-    (:domain igibson)
+(define (problem cleaning_up_after_a_meal-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
      	bowl.n.01_1 bowl.n.01_2 - bowl.n.01
     	table.n.02_1 - table.n.02
     	sack.n.01_1 - sack.n.01
     	chair.n.01_1 chair.n.01_2 - chair.n.01
     	plate.n.04_1 plate.n.04_2 plate.n.04_3 plate.n.04_4 - plate.n.04
     	cup.n.01_1 cup.n.01_2 - cup.n.01
     	hamburger.n.01_1 hamburger.n.01_2 - hamburger.n.01
     	floor.n.01_1 floor.n.01_2 - floor.n.01
     	detergent.n.02_1 - detergent.n.02
+    	detergent__bottle.n.01_1 - detergent__bottle.n.01
     	dishwasher.n.01_1 - dishwasher.n.01
         sink.n.01_1 - sink.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
         (ontop bowl.n.01_1 table.n.02_1) 
@@ -31,63 +32,61 @@
         (covered plate.n.04_2 stain.n.01_1) 
         (covered plate.n.04_3 stain.n.01_1) 
         (covered plate.n.04_4 stain.n.01_1) 
         (ontop cup.n.01_1 table.n.02_1) 
         (ontop cup.n.01_2 table.n.02_1) 
         (covered cup.n.01_1 stain.n.01_1) 
         (covered cup.n.01_2 stain.n.01_1) 
-        (ontop hamburger.n.01_1 chair.n.01_2) 
-        (ontop hamburger.n.01_2 floor.n.01_1) 
-        (ontop detergent.n.02_1 floor.n.01_1) 
-        (covered chair.n.01_1 stain.n.01_1) 
-        (covered chair.n.01_2 stain.n.01_1) 
+        (ontop hamburger.n.01_1 chair.n.01_2)
+        (ontop hamburger.n.01_2 floor.n.01_1)
+        (filled detergent__bottle.n.01_1 detergent.n.02_1)
+        (ontop detergent__bottle.n.01_1 floor.n.01_1)
+        (covered chair.n.01_1 stain.n.01_1)
+        (covered chair.n.01_2 stain.n.01_1)
         (covered table.n.02_1 stain.n.01_1) 
         (inroom dishwasher.n.01_1 kitchen) 
         (inroom floor.n.01_1 dining_room) 
         (inroom floor.n.01_2 kitchen) 
         (inroom table.n.02_1 dining_room) 
-        (inroom chair.n.01_1 dining_room) 
-        (inroom chair.n.01_2 dining_room) 
+        (inroom chair.n.01_1 dining_room)
+        (inroom chair.n.01_2 dining_room)
         (inroom sink.n.01_1 kitchen)
         (ontop agent.n.01_1 floor.n.01_2)
     )
     
     (:goal 
         (and 
             (forall 
                 (?bowl.n.01 - bowl.n.01) 
                 (not 
-                    (covered ?bowl.n.01 stain.n.01_1)
+                    (covered ?bowl.n.01 ?stain.n.01_1)
                 )
             ) 
             (forall 
                 (?plate.n.04 - plate.n.04) 
                 (not 
-                    (covered ?plate.n.04 stain.n.01_1)
+                    (covered ?plate.n.04 ?stain.n.01_1)
                 )
             ) 
             (forall 
                 (?cup.n.01 - cup.n.01) 
                 (not 
-                    (covered ?cup.n.01 stain.n.01_1)
+                    (covered ?cup.n.01 ?stain.n.01_1)
                 )
             ) 
             (forall 
                 (?hamburger.n.01 - hamburger.n.01) 
                 (inside ?hamburger.n.01 ?sack.n.01_1)
             ) 
             (ontop ?sack.n.01_1 ?floor.n.01_1) 
             (not 
-                (covered ?floor.n.01_1 stain.n.01_1)
+                (covered ?table.n.02_1 ?stain.n.01_1)
             ) 
-            (not 
-                (covered ?chair.n.01_2 stain.n.01_1)
-            ) 
-            (not 
-                (covered ?floor.n.01_1 stain.n.01_1)
-            ) 
-            (not 
-                (covered ?table.n.02_1 stain.n.01_1)
-            )
+            (forall
+                (?chair.n.01 - chair.n.01)
+                (not
+                    (covered ?chair.n.01 ?stain.n.01_1)
+                 )
+            )        
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_up_refrigerator/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_up_refrigerator/problem0.bddl`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-(define (problem cleaning_up_refrigerator_0)
-    (:domain igibson)
+(define (problem cleaning_up_refrigerator-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
         dust.n.01_1 - dust.n.01
      	rag.n.01_1 rag.n.01_2 - rag.n.01
     	cabinet.n.01_1 - cabinet.n.01
-    	soap.n.01_1 - soap.n.01
+    	bar_soap.n.01_1 - bar_soap.n.01
     	countertop.n.01_1 - countertop.n.01
     	tray.n.01_1 tray.n.01_2 - tray.n.01
     	electric_refrigerator.n.01_1 - electric_refrigerator.n.01
     	bowl.n.01_1 - bowl.n.01
     	sink.n.01_1 - sink.n.01
         agent.n.01_1 - agent.n.01
         floor.n.01_1 - floor.n.01
     )
     
     (:init 
         (inside rag.n.01_1 cabinet.n.01_1) 
         (inside rag.n.01_2 cabinet.n.01_1) 
-        (ontop soap.n.01_1 countertop.n.01_1) 
+        (ontop bar_soap.n.01_1 countertop.n.01_1) 
         (inside tray.n.01_1 electric_refrigerator.n.01_1) 
         (inside tray.n.01_2 electric_refrigerator.n.01_1) 
         (inside bowl.n.01_1 electric_refrigerator.n.01_1) 
         (covered tray.n.01_1 stain.n.01_1) 
         (covered tray.n.01_2 stain.n.01_1) 
         (covered bowl.n.01_1 dust.n.01_1) 
         (covered electric_refrigerator.n.01_1 stain.n.01_1) 
@@ -37,28 +37,28 @@
     
     (:goal 
         (and 
             (forall 
                 (?rag.n.01 - rag.n.01) 
                 (nextto ?rag.n.01 ?sink.n.01_1)
             ) 
-            (inside ?soap.n.01_1 ?sink.n.01_1) 
+            (inside ?bar_soap.n.01_1 ?sink.n.01_1) 
             (forall 
                 (?tray.n.01 - tray.n.01) 
                 (inside ?tray.n.01 ?electric_refrigerator.n.01_1)
             ) 
             (not 
-                (covered ?tray.n.01_1 stain.n.01_1)
+                (covered ?tray.n.01_1 ?stain.n.01_1)
             ) 
             (not 
-                (covered ?tray.n.01_2 stain.n.01_1)
+                (covered ?tray.n.01_2 ?stain.n.01_1)
             ) 
             (nextto ?bowl.n.01_1 ?sink.n.01_1) 
             (not 
-                (covered ?bowl.n.01_1 dust.n.01_1)
+                (covered ?bowl.n.01_1 ?dust.n.01_1)
             ) 
             (not 
                 (covered ?electric_refrigerator.n.01_1 stain.n.01_1)
             )
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/cleaning_windows/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/cleaning_oven/problem0.bddl`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,40 @@
-(define (problem cleaning_windows_0)
-    (:domain igibson)
+(define (problem cleaning_oven-0)
+    (:domain omnigibson)
 
     (:objects
-        dust.n.01_1 - dust.n.01
-     	towel.n.01_1 towel.n.01_2 - towel.n.01
+        stain.n.01_1 - stain.n.01
+     	dustpan.n.02_1 - dustpan.n.02
+    	floor.n.01_1 - floor.n.01
+    	bar_soap.n.01_1 - bar_soap.n.01
     	cabinet.n.01_1 - cabinet.n.01
     	rag.n.01_1 rag.n.01_2 - rag.n.01
-    	cleansing_agent.n.01_1 - cleansing_agent.n.01
-    	window.n.01_1 window.n.01_2 - window.n.01
+    	newspaper.n.03_1 - newspaper.n.03
     	sink.n.01_1 - sink.n.01
-    	floor.n.01_1 floor.n.01_2 - floor.n.01
-    	table.n.02_1 - table.n.02
-        agent.n.01_1 - agent.n.01
+    	scrub_brush.n.01_1 - scrub_brush.n.01
+    	oven.n.01_1 - oven.n.01
+    	agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (inside towel.n.01_1 cabinet.n.01_1) 
-        (inside towel.n.01_2 cabinet.n.01_1) 
+        (ontop dustpan.n.02_1 floor.n.01_1) 
+        (inside bar_soap.n.01_1 cabinet.n.01_1) 
         (inside rag.n.01_1 cabinet.n.01_1) 
         (inside rag.n.01_2 cabinet.n.01_1) 
-        (inside cleansing_agent.n.01_1 cabinet.n.01_1) 
-        (covered window.n.01_1 dust.n.01_1) 
-        (covered window.n.01_2 dust.n.01_1) 
-        (not 
-            (covered sink.n.01_1 dust.n.01_1)
-        ) 
-        (inroom floor.n.01_1 kitchen) 
-        (inroom floor.n.01_2 living_room) 
-        (inroom window.n.01_1 kitchen) 
-        (inroom window.n.01_2 living_room) 
+        (ontop newspaper.n.03_1 floor.n.01_1) 
+        (inside scrub_brush.n.01_1 cabinet.n.01_1) 
+        (covered oven.n.01_1 stain.n.01_1) 
+        (inroom oven.n.01_1 kitchen) 
         (inroom cabinet.n.01_1 kitchen) 
         (inroom sink.n.01_1 kitchen) 
-        (inroom table.n.02_1 living_room) 
+        (inroom floor.n.01_1 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (not 
-                (covered ?window.n.01_1 dust.n.01_1)
-            ) 
-            (not 
-                (covered ?window.n.01_2 dust.n.01_1)
+                (covered ?oven.n.01_1 ?stain.n.01_1)
             )
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/clearing_the_table_after_dinner/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/putting_up_outdoor_holiday_decorations/problem0.bddl`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,47 @@
-(define (problem clearing_the_table_after_dinner_0)
-    (:domain igibson)
+(define (problem putting_up_outdoor_holiday_decorations-0)
+    (:domain omnigibson)
 
     (:objects
-     	floor.n.01_1 - floor.n.01
-    	chair.n.01_1 chair.n.01_2 - chair.n.01
-    	table.n.02_1 - table.n.02
-    	cup.n.01_1 cup.n.01_2 - cup.n.01
-    	bucket.n.01_1 bucket.n.01_2 - bucket.n.01
-    	bowl.n.01_1 bowl.n.01_2 bowl.n.01_3 bowl.n.01_4 - bowl.n.01
-    	catsup.n.01_1 - catsup.n.01
-    	beverage.n.01_1 beverage.n.01_2 - beverage.n.01
-    	agent.n.01_1 - agent.n.01
+        rail_fence.n.01_1 - rail_fence.n.01
+        floor.n.01_1 floor.n.01_2 - floor.n.01
+        pot_plant.n.01_1 - pot_plant.n.01
+        carton.n.02_1 - carton.n.02
+        wreath.n.01_1 - wreath.n.01
+        fairy_light.n.01_1 - fairy_light.n.01
+        lawn.n.01_1 - lawn.n.01
+        wall.n.01_1 - wall.n.01
+        rose.n.01_1 - rose.n.01
+        agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (ontop cup.n.01_1 table.n.02_1) 
-        (ontop cup.n.01_2 table.n.02_1) 
-        (ontop bucket.n.01_1 floor.n.01_1) 
-        (ontop bowl.n.01_1 table.n.02_1) 
-        (ontop bowl.n.01_2 table.n.02_1) 
-        (ontop bowl.n.01_3 table.n.02_1) 
-        (ontop bowl.n.01_4 table.n.02_1) 
-        (ontop catsup.n.01_1 table.n.02_1) 
-        (ontop beverage.n.01_1 table.n.02_1) 
-        (ontop beverage.n.01_2 floor.n.01_1) 
-        (ontop bucket.n.01_2 floor.n.01_1) 
-        (inroom floor.n.01_1 dining_room) 
-        (inroom chair.n.01_1 dining_room) 
-        (inroom chair.n.01_2 dining_room) 
-        (inroom table.n.02_1 dining_room) 
-        (ontop agent.n.01_1 floor.n.01_1)
+        (ontop pot_plant.n.01_1 floor.n.01_1) 
+        (ontop carton.n.02_1 floor.n.01_2) 
+        (inside wreath.n.01_1 carton.n.02_1) 
+        (not
+            (attached wreath.n.01_1 wall.n.01_1)
+        )
+        (inside fairy_light.n.01_1 carton.n.02_1) 
+        (inside rose.n.01_1 carton.n.02_1) 
+        (not 
+            (toggled_on fairy_light.n.01_1)
+        ) 
+        (inroom floor.n.01_1 garden) 
+        (inroom lawn.n.01_1 garden) 
+        (inroom wall.n.01_1 garden) 
+        (inroom floor.n.01_2 living_room) 
+        (inroom rail_fence.n.01_1 garden) 
+        (ontop pot_plant.n.01_1 floor.n.01_1) 
+        (ontop agent.n.01_1 floor.n.01_2)
     )
     
     (:goal 
         (and 
-            (forall 
-                (?cup.n.01 - cup.n.01) 
-                (exists 
-                    (?bucket.n.01 - bucket.n.01) 
-                    (inside ?cup.n.01 ?bucket.n.01)
-                )
-            ) 
-            (forall 
-                (?bowl.n.01 - bowl.n.01) 
-                (exists 
-                    (?bucket.n.01 - bucket.n.01) 
-                    (inside ?bowl.n.01 ?bucket.n.01)
-                )
-            ) 
-            (exists 
-                (?bucket.n.01 - bucket.n.01) 
-                (inside ?catsup.n.01_1 ?bucket.n.01)
-            )
+            (attached ?wreath.n.01_1 ?wall.n.01_1)
+            (draped ?fairy_light.n.01_1 ?pot_plant.n.01_1) 
+            (toggled_on ?fairy_light.n.01_1) 
+            (ontop ?rose.n.01_1 ?lawn.n.01_1)
+            (ontop ?pot_plant.n.01_1 ?lawn.n.01_1)
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/collecting_aluminum_cans/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/rearrange_your_room/problem0.bddl`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-(define (problem collecting_aluminum_cans_0)
-    (:domain igibson)
+(define (problem rearrange_your_room-0)
+    (:domain omnigibson)
 
     (:objects
-     	pop.n.02_1 pop.n.02_2 pop.n.02_3 pop.n.02_4 pop.n.02_5 pop.n.02_6 - pop.n.02
-    	bed.n.01_1 - bed.n.01
-    	floor.n.01_1 - floor.n.01
-    	bucket.n.01_1 - bucket.n.01
+        mattress.n.01_1 - mattress.n.01
+        floor.n.01_1 - floor.n.01
+        pillow.n.01_1 pillow.n.01_2 - pillow.n.01
+        bed.n.01_1 - bed.n.01
+        shelf.n.01_1 - shelf.n.01
         agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (ontop pop.n.02_1 bed.n.01_1) 
-        (ontop pop.n.02_2 bed.n.01_1) 
-        (ontop pop.n.02_3 bed.n.01_1) 
-        (ontop pop.n.02_4 floor.n.01_1) 
-        (ontop pop.n.02_5 floor.n.01_1) 
-        (ontop pop.n.02_6 floor.n.01_1) 
-        (ontop bucket.n.01_1 bed.n.01_1) 
-        (inroom bed.n.01_1 bedroom) 
+        (ontop mattress.n.01_1 floor.n.01_1) 
+        (ontop pillow.n.01_1 mattress.n.01_1) 
+        (ontop pillow.n.01_2 floor.n.01_1) 
         (inroom floor.n.01_1 bedroom) 
+        (inroom bed.n.01_1 bedroom) 
+        (inroom shelf.n.01_1 bedroom) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
+            (ontop ?mattress.n.01_1 ?bed.n.01_1) 
             (forall 
-                (?pop.n.02 - pop.n.02) 
-                (inside ?pop.n.02 ?bucket.n.01_1)
-            )
+                (?pillow.n.01 - pillow.n.01) 
+                (ontop ?pillow.n.01 ?mattress.n.01_1)
+            ) 
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/defrosting_freezer/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/wash_fruit_and_vegetables/problem0.bddl`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,63 @@
-(define (problem defrosting_freezer_0)
-    (:domain igibson)
+(define (problem wash_fruit_and_vegetables-0)
+    (:domain omnigibson)
 
     (:objects
-        stain.n.01_1 - stain.n.01
-     	floor.n.01_1 - floor.n.01
-    	electric_refrigerator.n.01_1 - electric_refrigerator.n.01
-    	sink.n.01_1 - sink.n.01
-    	countertop.n.01_1 - countertop.n.01
-    	receptacle.n.01_1 - receptacle.n.01
-    	bucket.n.01_1 - bucket.n.01
-    	scraper.n.01_1 - scraper.n.01
-    	towel.n.01_1 - towel.n.01
-    	rag.n.01_1 - rag.n.01
-    	food.n.02_1 food.n.02_2 food.n.02_3 - food.n.02
-    	agent.n.01_1 - agent.n.01
+        grape.n.01_1 grape.n.01_2 - grape.n.01
+        electric_refrigerator.n.01_1 - electric_refrigerator.n.01
+        apple.n.01_1 - apple.n.01
+        countertop.n.01_1 - countertop.n.01
+        broccoli.n.02_1 - broccoli.n.02
+        cauliflower.n.02_1 - cauliflower.n.02
+        colander.n.01_1 - colander.n.01
+        dust.n.01_1 - dust.n.01
+        dirt.n.02_1 - dirt.n.02
+        paper_towel.n.01_1 paper_towel.n.01_2 - paper_towel.n.01
+        water.n.06_1 - water.n.06
+        sink.n.01_1 - sink.n.01
+        floor.n.01_1 - floor.n.01
+        agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (not 
-            (covered sink.n.01_1 stain.n.01_1)
-        ) 
-        (ontop receptacle.n.01_1 floor.n.01_1) 
-        (ontop bucket.n.01_1 floor.n.01_1) 
-        (ontop scraper.n.01_1 countertop.n.01_1) 
-        (ontop towel.n.01_1 countertop.n.01_1) 
-        (not 
-            (covered towel.n.01_1 stain.n.01_1)
-        ) 
-        (ontop rag.n.01_1 countertop.n.01_1) 
-        (inside food.n.02_1 electric_refrigerator.n.01_1) 
-        (inside food.n.02_2 electric_refrigerator.n.01_1) 
-        (inside food.n.02_3 electric_refrigerator.n.01_1) 
+        (inside grape.n.01_1 electric_refrigerator.n.01_1) 
+        (inside grape.n.01_2 electric_refrigerator.n.01_1) 
+        (covered grape.n.01_1 dust.n.01_1)
+        (covered grape.n.01_2 dust.n.01_1)
+        (ontop apple.n.01_1 countertop.n.01_1) 
+        (covered apple.n.01_1 dust.n.01_1)
+        (inside broccoli.n.02_1 electric_refrigerator.n.01_1) 
+        (covered broccoli.n.02_1 dirt.n.02_1)
+        (inside cauliflower.n.02_1 electric_refrigerator.n.01_1)
+        (covered cauliflower.n.02_1 dirt.n.02_1)
+        (ontop colander.n.01_1 countertop.n.01_1) 
+        (ontop paper_towel.n.01_1 countertop.n.01_1) 
+        (ontop paper_towel.n.01_2 countertop.n.01_1) 
+        (insource sink.n.01_1 water.n.06_1) 
         (inroom floor.n.01_1 kitchen) 
-        (inroom electric_refrigerator.n.01_1 kitchen) 
         (inroom sink.n.01_1 kitchen) 
         (inroom countertop.n.01_1 kitchen) 
+        (inroom electric_refrigerator.n.01_1 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
+    
     )
     
     (:goal 
         (and 
-            (nextto ?receptacle.n.01_1 ?electric_refrigerator.n.01_1) 
-            (nextto ?bucket.n.01_1 ?countertop.n.01_1) 
-            (ontop ?scraper.n.01_1 ?electric_refrigerator.n.01_1) 
-            (ontop ?towel.n.01_1 ?countertop.n.01_1) 
-            (inside ?rag.n.01_1 ?sink.n.01_1) 
             (forall 
-                (?food.n.02 - food.n.02) 
-                (inside ?food.n.02 ?bucket.n.01_1)
+                (?grape.n.01 - grape.n.01) 
+                (not
+                    (covered ?grape.n.01 ?dust.n.01_1)
+                )
+            ) 
+            (not
+                (covered ?apple.n.01_1 ?dust.n.01_1)
+            )
+            (not
+                (covered ?broccoli.n.02_1 ?dirt.n.02_1)
+            )
+            (not
+                (covered ?cauliflower.n.02_1 ?dirt.n.02_1)
             )
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/installing_a_fax_machine/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/clean_carpets/problem0.bddl`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-(define (problem installing_a_fax_machine_0)
-    (:domain igibson)
+(define (problem clean_carpets-0)
+    (:domain omnigibson)
 
     (:objects
-     	facsimile.n.02_1 - facsimile.n.02
-    	floor.n.01_1 - floor.n.01
-    	table.n.02_1 - table.n.02
-    	agent.n.01_1 - agent.n.01
+        rug.n.01_1 - rug.n.01
+        dust.n.01_1 - dust.n.01
+        vacuum.n.04_1 - vacuum.n.04
+        floor.n.01_1 - floor.n.01
+        agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (ontop facsimile.n.02_1 floor.n.01_1) 
-        (not 
-            (toggled_on facsimile.n.02_1)
-        ) 
-        (inroom table.n.02_1 private_office) 
-        (inroom floor.n.01_1 private_office) 
-        (ontop agent.n.01_1 floor.n.01_1)
+        (covered rug.n.01_1 dust.n.01_1) 
+        (ontop vacuum.n.04_1 floor.n.01_1) 
+        (ontop agent.n.01_1 floor.n.01_1) 
+        (inroom floor.n.01_1 playroom) 
+        (ontop rug.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
-            (ontop ?facsimile.n.02_1 ?table.n.02_1) 
-            (toggled_on ?facsimile.n.02_1)
+            (not 
+                (covered ?rug.n.01_1 ?dust.n.01_1)
+            )
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/installing_a_modem/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/installing_a_modem/problem0.bddl`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem installing_a_modem_0)
-    (:domain igibson)
+(define (problem installing_a_modem-0)
+    (:domain omnigibson)
 
     (:objects
      	modem.n.01_1 - modem.n.01
     	table.n.02_1 - table.n.02
     	floor.n.01_1 - floor.n.01
     	agent.n.01_1 - agent.n.01
     )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/installing_a_printer/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/installing_a_printer/problem0.bddl`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem installing_a_printer_0)
-    (:domain igibson)
+(define (problem installing_a_printer-0)
+    (:domain omnigibson)
 
     (:objects
      	printer.n.03_1 - printer.n.03
     	floor.n.01_1 - floor.n.01
     	table.n.02_1 - table.n.02
         agent.n.01_1 - agent.n.01
     )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/installing_a_scanner/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/installing_a_scanner/problem0.bddl`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem installing_a_scanner_0)
-    (:domain igibson)
+(define (problem installing_a_scanner-0)
+    (:domain omnigibson)
 
     (:objects
      	scanner.n.02_1 - scanner.n.02
     	table.n.02_1 - table.n.02
     	floor.n.01_1 - floor.n.01
     	agent.n.01_1 - agent.n.01
     )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/installing_alarms/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/installing_alarms/problem0.bddl`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem installing_alarms_0)
-    (:domain igibson)
+(define (problem installing_alarms-0)
+    (:domain omnigibson)
 
     (:objects
      	alarm.n.02_1 alarm.n.02_2 - alarm.n.02
     	table.n.02_1 table.n.02_2 - table.n.02
     	floor.n.01_1 - floor.n.01
     	agent.n.01_1 - agent.n.01
     )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/laying_tile_floors/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/laying_tile_floors/problem0.bddl`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem laying_tile_floors_0)
-    (:domain igibson)
+(define (problem laying_tile_floors-0)
+    (:domain omnigibson)
 
     (:objects
         tile.n.01_1 tile.n.01_2 tile.n.01_3 tile.n.01_4 - tile.n.01
         floor.n.01_1 floor.n.01_2 - floor.n.01
         agent.n.01_1 - agent.n.01
     )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/laying_wood_floors/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/laying_wood_floors/problem0.bddl`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem laying_wood_floors_0)
-    (:domain igibson)
+(define (problem laying_wood_floors-0)
+    (:domain omnigibson)
 
     (:objects
      	plywood.n.01_1 plywood.n.01_2 plywood.n.01_3 plywood.n.01_4 - plywood.n.01
     	floor.n.01_1 floor.n.01_2 - floor.n.01
     	hammer.n.02_1 - hammer.n.02
     	saw.n.02_1 - saw.n.02
     	agent.n.01_1 - agent.n.01
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/loading_the_dishwasher/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/loading_the_dishwasher/problem0.bddl`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem loading_the_dishwasher_0)
-    (:domain igibson)
+(define (problem loading_the_dishwasher-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
         plate.n.04_1 plate.n.04_2 plate.n.04_3 - plate.n.04
        countertop.n.01_1 - countertop.n.01
         mug.n.04_1 - mug.n.04
         bowl.n.01_1 bowl.n.01_2 - bowl.n.01
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/mopping_floors/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/clean_a_watch/problem0.bddl`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-(define (problem mopping_floors_0)
-    (:domain igibson)
+(define (problem clean_a_watch-0)
+    (:domain omnigibson)
 
     (:objects
-        stain.n.01_1 - stain.n.01
-     	broom.n.01_1 - broom.n.01
-    	floor.n.01_1 floor.n.01_2 - floor.n.01
-    	soap.n.01_1 - soap.n.01
-    	bucket.n.01_1 - bucket.n.01
-    	piece_of_cloth.n.01_1 - piece_of_cloth.n.01
+     	watch.n.01_1 - watch.n.01
+    	countertop.n.01_1 - countertop.n.01
+    	tissue.n.02_1 - tissue.n.02
+    	dirt.n.02_1 - dirt.n.02
+    	water.n.06_1 - water.n.06
     	sink.n.01_1 - sink.n.01
+    	floor.n.01_1 - floor.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (ontop broom.n.01_1 floor.n.01_2) 
-        (ontop soap.n.01_1 floor.n.01_1) 
-        (ontop bucket.n.01_1 floor.n.01_1) 
-        (ontop piece_of_cloth.n.01_1 floor.n.01_1) 
-        (covered floor.n.01_1 stain.n.01_1) 
-        (inroom floor.n.01_1 bathroom) 
-        (inroom floor.n.01_2 corridor) 
-        (inroom sink.n.01_1 bathroom) 
+        (ontop watch.n.01_1 countertop.n.01_1) 
+        (ontop tissue.n.02_1 countertop.n.01_1) 
+        (covered watch.n.01_1 dirt.n.02_1) 
+        (insource sink.n.01_1 water.n.06_1) 
+        (inroom sink.n.01_1 kitchen) 
+        (inroom countertop.n.01_1 kitchen) 
+        (inroom floor.n.01_1 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (not 
-                (covered ?floor.n.01_1 stain.n.01_1)
+                (covered ?watch.n.01_1 ?dirt.n.02_1)
             ) 
-            (nextto ?bucket.n.01_1 ?sink.n.01_1) 
-            (inside ?soap.n.01_1 ?bucket.n.01_1) 
-            (nextto ?broom.n.01_1 ?sink.n.01_1)
         )
     )
-)
+)
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/moving_boxes_to_storage/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/moving_boxes_to_storage/problem0.bddl`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem moving_boxes_to_storage_0)
-    (:domain igibson)
+(define (problem moving_boxes_to_storage-0)
+    (:domain omnigibson)
 
     (:objects
         carton.n.02_1 carton.n.02_2 - carton.n.02
     	floor.n.01_1 floor.n.01_2 - floor.n.01
     	shelf.n.01_1 - shelf.n.01
     	agent.n.01_1 - agent.n.01
     )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/organizing_boxes_in_garage/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/organizing_boxes_in_garage/problem0.bddl`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem organizing_boxes_in_garage_0)
-    (:domain igibson)
+(define (problem organizing_boxes_in_garage-0)
+    (:domain omnigibson)
 
     (:objects
      	carton.n.02_1 carton.n.02_2 - carton.n.02
     	floor.n.01_1 - floor.n.01
     	ball.n.01_1 ball.n.01_2 - ball.n.01
     	plate.n.04_1 plate.n.04_2 plate.n.04_3 - plate.n.04
     	cabinet.n.01_1 - cabinet.n.01
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/organizing_file_cabinet/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/organizing_file_cabinet/problem0.bddl`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-(define (problem organizing_file_cabinet_0)
-    (:domain igibson)
+(define (problem organizing_file_cabinet-0)
+    (:domain omnigibson)
 
     (:objects
         floor.n.01_1 - floor.n.01
         marker.n.03_1 - marker.n.03
         chair.n.01_1 - chair.n.01
         document.n.01_1 document.n.01_2 document.n.01_3 document.n.01_4 - document.n.01
         table.n.02_1 - table.n.02
         cabinet.n.01_1 - cabinet.n.01
         folder.n.02_1 folder.n.02_2 - folder.n.02
         agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (ontop marker.n.03_1 chair.n.01_1) 
+        (ontop marker.n.03_1 chair.n.01_1)
         (ontop document.n.01_1 table.n.02_1) 
         (inside document.n.01_2 cabinet.n.01_1) 
         (ontop document.n.01_3 table.n.02_1) 
         (inside document.n.01_4 cabinet.n.01_1) 
         (ontop folder.n.02_1 table.n.02_1)
         (ontop folder.n.02_2 floor.n.01_1) 
         (inroom cabinet.n.01_1 private_office) 
         (inroom table.n.02_1 private_office) 
-        (inroom chair.n.01_1 private_office) 
+        (inroom chair.n.01_1 private_office)
         (inroom floor.n.01_1 private_office) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (ontop ?marker.n.03_1 ?table.n.02_1)
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/organizing_school_stuff/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/organizing_school_stuff/problem0.bddl`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-(define (problem organizing_school_stuff_0)
-    (:domain igibson)
+(define (problem organizing_school_stuff-0)
+    (:domain omnigibson)
 
     (:objects
-     	highlighter.n.02_1 - highlighter.n.02
-    	bed.n.01_1 - bed.n.01
-    	pencil.n.01_1 - pencil.n.01
-    	pen.n.01_1 - pen.n.01
-    	floor.n.01_1 - floor.n.01
-    	calculator.n.02_1 - calculator.n.02
-    	book.n.02_1 - book.n.02
-    	folder.n.02_1 - folder.n.02
+        marker.n.03_1 - marker.n.03
+        bed.n.01_1 - bed.n.01
+        pencil.n.01_1 - pencil.n.01
+        pen.n.01_1 - pen.n.01
+        floor.n.01_1 - floor.n.01
+        calculator.n.02_1 - calculator.n.02
+        book.n.02_1 - book.n.02
+        folder.n.02_1 - folder.n.02
         table.n.02_1 - table.n.02
-    	backpack.n.01_1 - backpack.n.01
-    	agent.n.01_1 - agent.n.01
+        backpack.n.01_1 - backpack.n.01
+        agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (ontop highlighter.n.02_1 bed.n.01_1) 
+        (ontop marker.n.03_1 bed.n.01_1)
         (ontop pencil.n.01_1 bed.n.01_1) 
         (ontop pen.n.01_1 floor.n.01_1) 
         (ontop calculator.n.02_1 floor.n.01_1) 
         (ontop book.n.02_1 bed.n.01_1) 
         (ontop folder.n.02_1 bed.n.01_1) 
         (ontop backpack.n.01_1 floor.n.01_1) 
         (inroom floor.n.01_1 bedroom) 
@@ -32,15 +32,15 @@
     (:goal 
         (and 
             (and 
                 (nextto ?folder.n.02_1 ?book.n.02_1) 
                 (nextto ?folder.n.02_1 ?backpack.n.01_1) 
                 (nextto ?book.n.02_1 ?backpack.n.01_1)
             ) 
-            (inside ?highlighter.n.02_1 ?backpack.n.01_1) 
+            (inside ?marker.n.03_1 ?backpack.n.01_1)
             (inside ?pencil.n.01_1 ?backpack.n.01_1) 
             (inside ?pen.n.01_1 ?backpack.n.01_1) 
             (inside ?calculator.n.02_1 ?backpack.n.01_1) 
             (ontop ?backpack.n.01_1 ?bed.n.01_1)
         )
     )
-)
+)
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/packing_bags_or_suitcase/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/prepare_an_emergency_school_kit/problem0.bddl`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,45 @@
-(define (problem packing_bags_or_suitcase_0)
-    (:domain igibson)
+(define (problem prepare_an_emergency_school_kit-0)
+    (:domain omnigibson)
 
     (:objects
      	backpack.n.01_1 - backpack.n.01
+    	pen.n.01_1 - pen.n.01
     	floor.n.01_1 - floor.n.01
-    	toothbrush.n.01_1 - toothbrush.n.01
-    	bed.n.01_1 - bed.n.01
-    	shampoo.n.01_1 - shampoo.n.01
-    	hardback.n.01_1 - hardback.n.01
-    	underwear.n.01_1 underwear.n.01_2 - underwear.n.01
-    	toothpaste.n.01_1 - toothpaste.n.01
-    	door.n.01_1 - door.n.01
-    	window.n.01_1 - window.n.01
+    	notebook.n.01_1 - notebook.n.01
+    	bottle__of__perfume.n.01_1 - bottle__of__perfume.n.01
+    	granola_bar.n.01_1 - granola_bar.n.01
+    	wallet.n.01_1 - wallet.n.01
+    	tissue.n.02_1 - tissue.n.02
+    	box__of__candy.n.01_1 - box__of__candy.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
+        (open backpack.n.01_1) 
+        (ontop pen.n.01_1 floor.n.01_1) 
+        (ontop notebook.n.01_1 floor.n.01_1) 
+        (ontop bottle__of__perfume.n.01_1 floor.n.01_1) 
+        (ontop granola_bar.n.01_1 floor.n.01_1) 
+        (ontop wallet.n.01_1 floor.n.01_1) 
+        (ontop tissue.n.02_1 floor.n.01_1) 
+        (ontop box__of__candy.n.01_1 floor.n.01_1) 
         (ontop backpack.n.01_1 floor.n.01_1) 
-        (ontop toothbrush.n.01_1 bed.n.01_1) 
-        (ontop shampoo.n.01_1 bed.n.01_1) 
-        (ontop hardback.n.01_1 bed.n.01_1) 
-        (ontop underwear.n.01_1 bed.n.01_1) 
-        (ontop underwear.n.01_2 bed.n.01_1) 
-        (ontop toothpaste.n.01_1 bed.n.01_1) 
-        (inroom bed.n.01_1 bedroom) 
-        (inroom floor.n.01_1 bedroom) 
-        (inroom door.n.01_1 bedroom) 
-        (inroom window.n.01_1 bedroom) 
+        (inroom floor.n.01_1 corridor) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
-        (and 
-            (forall 
-                (?underwear.n.01 - underwear.n.01) 
-                (inside ?underwear.n.01 ?backpack.n.01_1)
-            ) 
-            (inside ?toothbrush.n.01_1 ?backpack.n.01_1) 
-            (inside ?shampoo.n.01_1 ?backpack.n.01_1) 
-            (inside ?hardback.n.01_1 ?backpack.n.01_1) 
-            (inside ?toothpaste.n.01_1 ?backpack.n.01_1) 
-            (or 
-                (ontop ?backpack.n.01_1 ?bed.n.01_1) 
-                (ontop ?backpack.n.01_1 ?floor.n.01_1)
+        (and
+            (not
+                (open ?backpack.n.01_1)
             )
+            (inside ?pen.n.01_1 ?backpack.n.01_1) 
+            (inside ?notebook.n.01_1 ?backpack.n.01_1) 
+            (inside ?bottle__of__perfume.n.01_1 ?backpack.n.01_1) 
+            (inside ?granola_bar.n.01_1 ?backpack.n.01_1) 
+            (inside ?wallet.n.01_1 ?backpack.n.01_1) 
+            (inside ?tissue.n.02_1 ?backpack.n.01_1) 
+            (inside ?box__of__candy.n.01_1 ?backpack.n.01_1)
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/picking_up_take-out_food/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/picking_up_take_out_food/problem0.bddl`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem picking_up_take-out_food_0)
-    (:domain igibson)
+(define (problem picking_up_take_out_food-0)
+    (:domain omnigibson)
 
     (:objects
     	floor.n.01_1 - floor.n.01
     	carton.n.02_1 - carton.n.02
         table.n.02_1 - table.n.02
         sushi.n.01_1 - sushi.n.01
         hamburger.n.01_1 - hamburger.n.01
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/picking_up_trash/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/picking_up_trash/problem0.bddl`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-(define (problem picking_up_trash_0)
-    (:domain igibson)
+(define (problem picking_up_trash-0)
+    (:domain omnigibson)
 
     (:objects
         ashcan.n.01_1 - ashcan.n.01
         pad.n.01_1 pad.n.01_2 pad.n.01_3 - pad.n.01
-        pop.n.02_1 pop.n.02_2 - pop.n.02
+        can__of__soda.n.01_1 can__of__soda.n.01_2 - can__of__soda.n.01
         floor.n.01_1 floor.n.01_2 - floor.n.01
         agent.n.01_1 - agent.n.01
     )
     
     (:init 
         (ontop ashcan.n.01_1 floor.n.01_2) 
         (ontop pad.n.01_1 floor.n.01_2) 
         (ontop pad.n.01_2 floor.n.01_2) 
         (ontop pad.n.01_3 floor.n.01_1) 
-        (ontop pop.n.02_1 floor.n.01_1) 
-        (ontop pop.n.02_2 floor.n.01_1) 
+        (ontop can__of__soda.n.01_1 floor.n.01_1) 
+        (ontop can__of__soda.n.01_2 floor.n.01_1) 
         (inroom floor.n.01_2 kitchen) 
         (inroom floor.n.01_1 living_room) 
         (ontop agent.n.01_1 floor.n.01_2)
     )
     
     (:goal 
         (and 
             (forall 
                 (?pad.n.01 - pad.n.01) 
                 (inside ?pad.n.01 ?ashcan.n.01_1)
             ) 
             (forall 
-                (?pop.n.02 - pop.n.02) 
-                (inside ?pop.n.02 ?ashcan.n.01_1)
+                (?can__of__soda.n.01 - can__of__soda.n.01) 
+                (inside ?can__of__soda.n.01 ?ashcan.n.01_1)
             )
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/polishing_furniture/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/polishing_furniture/problem0.bddl`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem polishing_furniture_0)
-    (:domain igibson)
+(define (problem polishing_furniture-0)
+    (:domain omnigibson)
 
     (:objects
         dust.n.01_1 - dust.n.01
      	shelf.n.01_1 - shelf.n.01
     	table.n.02_1 - table.n.02
     	rag.n.01_1 - rag.n.01
     	floor.n.01_1 - floor.n.01
@@ -19,16 +19,16 @@
         (inroom floor.n.01_1 living_room) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (not 
-                (covered ?table.n.02_1 dust.n.01_1)
+                (covered ?table.n.02_1 ?dust.n.01_1)
             ) 
             (not 
-                (covered ?shelf.n.01_1 dust.n.01_1)
+                (covered ?shelf.n.01_1 ?dust.n.01_1)
             ) 
             (under ?rag.n.01_1 ?table.n.02_1)
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/polishing_shoes/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/polishing_shoes/problem0.bddl`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem polishing_shoes_0)
-    (:domain igibson)
+(define (problem polishing_shoes-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
     	shoe.n.01_1 shoe.n.01_2 - shoe.n.01
     	rag.n.01_1 - rag.n.01
     	floor.n.01_1 - floor.n.01
     	sink.n.01_1 - sink.n.01
@@ -22,16 +22,16 @@
     )
     
     (:goal 
         (and 
             (nextto ?rag.n.01_1 ?sink.n.01_1) 
             (and 
                 (not 
-                    (covered ?shoe.n.01_1 stain.n.01_1)
+                    (covered ?shoe.n.01_1 ?stain.n.01_1)
                 ) 
                 (not 
-                    (covered ?shoe.n.01_2 stain.n.01_1)
+                    (covered ?shoe.n.01_2 ?stain.n.01_1)
                 )
             )
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/polishing_silver/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/make_coffee/problem0.bddl`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,38 @@
-(define (problem polishing_silver_0)
-    (:domain igibson)
+(define (problem make_coffee-0)
+    (:domain omnigibson)
 
     (:objects
-        dust.n.01_1 - dust.n.01
-     	spoon.n.01_1 spoon.n.01_2 spoon.n.01_3 spoon.n.01_4 - spoon.n.01
-    	rag.n.01_1 - rag.n.01
-    	cabinet.n.01_1 - cabinet.n.01
-    	floor.n.01_1 - floor.n.01
-    	agent.n.01_1 - agent.n.01
+        coffee_bean.n.01_1 - coffee_bean.n.01
+        water.n.06_1 - water.n.06
+        drip_coffee.n.01_1 - drip_coffee.n.01
+        coffee_maker.n.01_1 - coffee_maker.n.01
+        mug.n.04_1 - mug.n.04
+        coffee_bean__jar.n.01_1 - coffee_bean__jar.n.01
+        countertop.n.01_1 - countertop.n.01
+        cabinet.n.01_1 - cabinet.n.01
+        sink.n.01_1 - sink.n.01
+        agent.n.01_1 - agent.n.01
+        floor.n.01_1 - floor.n.01
     )
     
     (:init 
-        (covered spoon.n.01_1 dust.n.01_1) 
-        (covered spoon.n.01_2 dust.n.01_1) 
-        (covered spoon.n.01_3 dust.n.01_1) 
-        (covered spoon.n.01_4 dust.n.01_1) 
-        (inside rag.n.01_1 cabinet.n.01_1) 
-        (inside spoon.n.01_1 cabinet.n.01_1) 
-        (inside spoon.n.01_2 cabinet.n.01_1) 
-        (inside spoon.n.01_3 cabinet.n.01_1) 
-        (inside spoon.n.01_4 cabinet.n.01_1) 
-        (inroom cabinet.n.01_1 kitchen) 
+        (filled coffee_bean__jar.n.01_1 coffee_bean.n.01_1) 
+        (inside coffee_bean__jar.n.01_1 cabinet.n.01_1) 
+        (ontop coffee_maker.n.01_1 countertop.n.01_1) 
+        (ontop mug.n.04_1 countertop.n.01_1)
+        (insource sink.n.01_1 water.n.06_1) 
+        (inroom sink.n.01_1 kitchen) 
+        (inroom countertop.n.01_1 kitchen) 
+        (future drip_coffee.n.01_1) 
         (inroom floor.n.01_1 kitchen) 
+        (inroom cabinet.n.01_1 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
-            (not 
-                (covered ?spoon.n.01_1 dust.n.01_1)
-            ) 
-            (not 
-                (covered ?spoon.n.01_2 dust.n.01_1)
-            ) 
-            (not 
-                (covered ?spoon.n.01_3 dust.n.01_1)
-            ) 
-            (not 
-                (covered ?spoon.n.01_4 dust.n.01_1)
-            ) 
-            (not 
-                (inside ?rag.n.01_1 ?cabinet.n.01_1)
-            ) 
-            (inside ?spoon.n.01_1 ?cabinet.n.01_1) 
-            (inside ?spoon.n.01_2 ?cabinet.n.01_1) 
-            (inside ?spoon.n.01_3 ?cabinet.n.01_1) 
-            (inside ?spoon.n.01_4 ?cabinet.n.01_1)
+            (real ?drip_coffee.n.01_1) 
+            (contains ?mug.n.04_1 ?drip_coffee.n.01_1)
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/putting_away_Christmas_decorations/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/putting_away_Christmas_decorations/problem0.bddl`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem putting_away_Christmas_decorations_0)
-    (:domain igibson)
+(define (problem putting_away_Christmas_decorations-0)
+    (:domain omnigibson)
 
     (:objects
      	wreath.n.01_1 wreath.n.01_2 - wreath.n.01
     	floor.n.01_1 - floor.n.01
     	bow.n.08_1 bow.n.08_2 bow.n.08_3 - bow.n.08
     	ribbon.n.01_1 ribbon.n.01_2 ribbon.n.01_3 - ribbon.n.01
     	cabinet.n.01_1 - cabinet.n.01
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/putting_away_Halloween_decorations/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/putting_away_Halloween_decorations/problem0.bddl`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-(define (problem putting_away_Halloween_decorations_0)
-    (:domain igibson)
+(define (problem putting_away_Halloween_decorations-0)
+    (:domain omnigibson)
 
     (:objects
-     	pumpkin.n.02_1 pumpkin.n.02_2 - pumpkin.n.02
-    	floor.n.01_1 - floor.n.01
-    	caldron.n.01_1 - caldron.n.01
-    	sheet.n.03_1 - sheet.n.03
-    	table.n.02_1 - table.n.02
-    	candle.n.01_1 candle.n.01_2 candle.n.01_3 - candle.n.01
-    	cabinet.n.01_1 - cabinet.n.01
-    	sofa.n.01_1 - sofa.n.01
-    	agent.n.01_1 - agent.n.01
+        pumpkin.n.02_1 pumpkin.n.02_2 - pumpkin.n.02
+        floor.n.01_1 - floor.n.01
+        caldron.n.01_1 - caldron.n.01
+        table.n.02_1 - table.n.02
+        candle.n.01_1 candle.n.01_2 candle.n.01_3 - candle.n.01
+        cabinet.n.01_1 - cabinet.n.01
+        sofa.n.01_1 - sofa.n.01
+        agent.n.01_1 - agent.n.01
     )
     
     (:init 
         (ontop pumpkin.n.02_1 floor.n.01_1) 
         (ontop pumpkin.n.02_2 floor.n.01_1) 
         (ontop caldron.n.01_1 floor.n.01_1) 
-        (ontop sheet.n.03_1 table.n.02_1) 
         (ontop candle.n.01_1 floor.n.01_1) 
         (ontop candle.n.01_2 floor.n.01_1) 
         (ontop candle.n.01_3 floor.n.01_1) 
         (inroom floor.n.01_1 living_room) 
         (inroom cabinet.n.01_1 living_room) 
         (inroom table.n.02_1 living_room) 
         (inroom sofa.n.01_1 living_room) 
@@ -34,15 +32,11 @@
                 (?pumpkin.n.02 - pumpkin.n.02) 
                 (inside ?pumpkin.n.02 ?cabinet.n.01_1)
             ) 
             (forall 
                 (?candle.n.01 - candle.n.01) 
                 (inside ?candle.n.01 ?cabinet.n.01_1)
             ) 
-            (or 
-                (nextto ?sheet.n.03_1 ?table.n.02_1) 
-                (ontop ?sheet.n.03_1 ?table.n.02_1)
-            ) 
             (nextto ?caldron.n.01_1 ?table.n.02_1)
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/putting_away_toys/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/putting_away_toys/problem0.bddl`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem putting_away_toys_0)
-    (:domain igibson)
+(define (problem putting_away_toys-0)
+    (:domain omnigibson)
 
     (:objects
         plaything.n.01_1 plaything.n.01_2 plaything.n.01_3 plaything.n.01_4 plaything.n.01_5 plaything.n.01_6 plaything.n.01_7 plaything.n.01_8 - plaything.n.01
         floor.n.01_1 floor.n.01_2 - floor.n.01
         carton.n.02_1 carton.n.02_2 - carton.n.02
         agent.n.01_1 - agent.n.01
         table.n.02_1 - table.n.02
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/putting_dishes_away_after_cleaning/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/putting_dishes_away_after_cleaning/problem0.bddl`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem putting_dishes_away_after_cleaning_0)
-    (:domain igibson)
+(define (problem putting_dishes_away_after_cleaning-0)
+    (:domain omnigibson)
 
     (:objects
      	plate.n.04_1 plate.n.04_2 plate.n.04_3 plate.n.04_4 plate.n.04_5 plate.n.04_6 plate.n.04_7 plate.n.04_8 - plate.n.04
     	countertop.n.01_1 countertop.n.01_2 - countertop.n.01
     	cabinet.n.01_1 - cabinet.n.01
     	floor.n.01_1 - floor.n.01
     	agent.n.01_1 - agent.n.01
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/putting_leftovers_away/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/putting_meal_on_plate/problem0.bddl`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,53 @@
-(define (problem putting_leftovers_away_0)
-    (:domain igibson)
+(define (problem putting_meal_on_plate-0)
+    (:domain omnigibson)
 
     (:objects
-     	pasta.n.02_1 pasta.n.02_2 pasta.n.02_3 pasta.n.02_4 - pasta.n.02
-    	floor.n.01_1 - floor.n.01
-    	sauce.n.01_1 sauce.n.01_2 sauce.n.01_3 sauce.n.01_4 - sauce.n.01
+     	porkchop.n.01_1 porkchop.n.01_2 - porkchop.n.01
     	electric_refrigerator.n.01_1 - electric_refrigerator.n.01
+    	oven.n.01_1 - oven.n.01
+    	plate.n.04_1 plate.n.04_2 - plate.n.04
     	countertop.n.01_1 - countertop.n.01
+    	water_glass.n.02_1 - water_glass.n.02
+    	apple.n.01_1 apple.n.01_2 - apple.n.01
+    	floor.n.01_1 - floor.n.01
+    	cabinet.n.01_1 - cabinet.n.01
+    	window.n.01_1 - window.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (ontop pasta.n.02_1 countertop.n.01_1) 
-        (ontop pasta.n.02_2 countertop.n.01_1) 
-        (ontop pasta.n.02_3 countertop.n.01_1) 
-        (ontop pasta.n.02_4 countertop.n.01_1) 
-        (ontop sauce.n.01_1 countertop.n.01_1) 
-        (ontop sauce.n.01_2 countertop.n.01_1) 
-        (ontop sauce.n.01_3 countertop.n.01_1) 
-        (ontop sauce.n.01_4 countertop.n.01_1) 
-        (inroom countertop.n.01_1 kitchen) 
-        (inroom electric_refrigerator.n.01_1 kitchen) 
+        (inside porkchop.n.01_1 electric_refrigerator.n.01_1) 
+        (inside porkchop.n.01_2 oven.n.01_1) 
+        (open electric_refrigerator.n.01_1) 
+        (open oven.n.01_1) 
+        (ontop plate.n.04_1 countertop.n.01_1) 
+        (ontop plate.n.04_2 countertop.n.01_1) 
+        (ontop water_glass.n.02_1 countertop.n.01_1) 
+        (inside apple.n.01_1 electric_refrigerator.n.01_1) 
+        (inside apple.n.01_2 electric_refrigerator.n.01_1) 
         (inroom floor.n.01_1 kitchen) 
+        (inroom electric_refrigerator.n.01_1 kitchen) 
+        (inroom cabinet.n.01_1 kitchen) 
+        (inroom window.n.01_1 kitchen) 
+        (inroom oven.n.01_1 kitchen) 
+        (inroom countertop.n.01_1 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
-            (forall 
-                (?pasta.n.02 - pasta.n.02) 
-                (inside ?pasta.n.02 ?electric_refrigerator.n.01_1)
-            ) 
-            (forall 
-                (?sauce.n.01 - sauce.n.01) 
-                (inside ?sauce.n.01 ?electric_refrigerator.n.01_1)
+            (ontop ?porkchop.n.01_1 ?plate.n.04_1) 
+            (ontop ?porkchop.n.01_2 ?plate.n.04_2) 
+            (hot ?porkchop.n.01_2) 
+            (frozen ?porkchop.n.01_1) 
+            (or
+                (not
+                    (open ?oven.n.01_1)
+                )
+                (not
+                    (open ?oven.n.01_1)
+                )
             )
         )
     )
-)
+)
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/putting_up_Christmas_decorations_inside/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/putting_up_Christmas_decorations_inside/problem0.bddl`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-(define (problem putting_up_Christmas_decorations_inside_0)
-    (:domain igibson)
+(define (problem putting_up_Christmas_decorations_inside-0)
+    (:domain omnigibson)
 
-    (:objects 
+    (:objects
         christmas_tree.n.05_1 - christmas_tree.n.05
         wreath.n.01_1 - wreath.n.01
         bow.n.08_1 bow.n.08_2 bow.n.08_3 - bow.n.08
         candle.n.01_1 candle.n.01_2 - candle.n.01
-        wrapping.n.01_1 wrapping.n.01_2 wrapping.n.01_3 - wrapping.n.01
+        gift_box.n.01_1 gift_box.n.01_2 gift_box.n.01_3 - gift_box.n.01
         carton.n.02_1 - carton.n.02
         floor.n.01_1 - floor.n.01
         table.n.02_1 - table.n.02
         sofa.n.01_1 - sofa.n.01
         agent.n.01_1 - agent.n.01
     )
     
@@ -19,30 +19,30 @@
         (ontop carton.n.02_1 floor.n.01_1)
         (inside wreath.n.01_1 carton.n.02_1)
         (inside bow.n.08_1 carton.n.02_1)
         (inside bow.n.08_2 carton.n.02_1)
         (inside bow.n.08_3 carton.n.02_1)
         (inside candle.n.01_1 carton.n.02_1)
         (inside candle.n.01_2 carton.n.02_1)
-        (ontop wrapping.n.01_1 floor.n.01_1)
-        (ontop wrapping.n.01_2 floor.n.01_1)
-        (ontop wrapping.n.01_3 floor.n.01_1)
+        (ontop gift_box.n.01_1 floor.n.01_1)
+        (ontop gift_box.n.01_2 floor.n.01_1)
+        (ontop gift_box.n.01_3 floor.n.01_1)
         (inroom floor.n.01_1 living_room)
         (inroom table.n.02_1 dining_room)
         (inroom sofa.n.01_1 living_room)
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (forall 
-                (?wrapping.n.01 - wrapping.n.01)
+                (?gift_box.n.01 - gift_box.n.01)
                 (or 
-                    (nextto ?wrapping.n.01 ?christmas_tree.n.05_1)
-                    (under ?wrapping.n.01 ?christmas_tree.n.05_1)
+                    (nextto ?gift_box.n.01 ?christmas_tree.n.05_1)
+                    (under ?gift_box.n.01 ?christmas_tree.n.05_1)
                 )
             )
             (forall 
                 (?candle.n.01 - candle.n.01)
                 (ontop ?candle.n.01 ?table.n.02_1)
             )
             (forn
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/re-shelving_library_books/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/re_shelving_library_books/problem0.bddl`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem re-shelving_library_books_0)
-    (:domain igibson)
+(define (problem re_shelving_library_books-0)
+    (:domain omnigibson)
 
     (:objects
      	book.n.02_1 book.n.02_2 book.n.02_3 book.n.02_4 book.n.02_5 book.n.02_6 book.n.02_7 book.n.02_8 - book.n.02
     	table.n.02_1 - table.n.02
     	shelf.n.01_1 - shelf.n.01
     	floor.n.01_1 - floor.n.01
     	agent.n.01_1 - agent.n.01
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/rearranging_furniture/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/rearranging_furniture/problem0.bddl`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-(define (problem rearranging_furniture_0)
-    (:domain igibson)
+(define (problem rearranging_furniture-0)
+    (:domain omnigibson)
 
     (:objects
      	lamp.n.02_1 lamp.n.02_2 - lamp.n.02
     	floor.n.01_1 - floor.n.01
-    	seat.n.03_1 seat.n.03_2 - seat.n.03
+    	chair.n.01_1 chair.n.01_2 - chair.n.01
     	bed.n.01_1 - bed.n.01
     	window.n.01_1 - window.n.01
     	door.n.01_1 - door.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
         (ontop lamp.n.02_1 floor.n.01_1) 
         (ontop lamp.n.02_2 floor.n.01_1) 
-        (ontop seat.n.03_1 floor.n.01_1) 
-        (ontop seat.n.03_2 bed.n.01_1) 
+        (ontop chair.n.01_1 floor.n.01_1)
+        (ontop chair.n.01_2 bed.n.01_1)
         (inroom window.n.01_1 bedroom) 
         (inroom bed.n.01_1 bedroom) 
         (inroom floor.n.01_1 bedroom) 
         (inroom door.n.01_1 bedroom) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (nextto ?lamp.n.02_1 ?door.n.01_1) 
             (nextto ?lamp.n.02_2 ?window.n.01_1) 
-            (touching ?seat.n.03_1 ?bed.n.01_1) 
-            (nextto ?seat.n.03_2 ?window.n.01_1)
+            (touching ?chair.n.01_1 ?bed.n.01_1)
+            (nextto ?chair.n.01_2 ?window.n.01_1)
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/serving_hors_d_oeuvres/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/serving_hors_d_oeuvres/problem0.bddl`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-(define (problem serving_hors_d_oeuvres_0)
-    (:domain igibson)
+(define (problem serving_hors_d_oeuvres-0)
+    (:domain omnigibson)
 
     (:objects
         cabinet.n.01_1 - cabinet.n.01
     	salad.n.01_1 salad.n.01_2 salad.n.01_3 salad.n.01_4 - salad.n.01
     	electric_refrigerator.n.01_1 - electric_refrigerator.n.01
     	tray.n.01_1 - tray.n.01
     	parsley.n.02_1 parsley.n.02_2 parsley.n.02_3 parsley.n.02_4 - parsley.n.02
     	cracker.n.01_1 cracker.n.01_2 cracker.n.01_3 cracker.n.01_4 - cracker.n.01
     	table.n.02_1 - table.n.02
-    	cheese.n.01_1 cheese.n.01_2 cheese.n.01_3 cheese.n.01_4 - cheese.n.01
+    	cheddar.n.02_1 cheddar.n.02_2 cheddar.n.02_3 cheddar.n.02_4 - cheddar.n.02
     	floor.n.01_1 - floor.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
         (inside salad.n.01_1 electric_refrigerator.n.01_1) 
         (inside salad.n.01_2 electric_refrigerator.n.01_1) 
@@ -24,18 +24,18 @@
         (inside parsley.n.02_3 electric_refrigerator.n.01_1) 
         (inside parsley.n.02_4 electric_refrigerator.n.01_1) 
         (ontop tray.n.01_1 floor.n.01_1) 
         (ontop cracker.n.01_1 table.n.02_1) 
         (ontop cracker.n.01_2 table.n.02_1) 
         (ontop cracker.n.01_3 table.n.02_1) 
         (ontop cracker.n.01_4 table.n.02_1) 
-        (inside cheese.n.01_1 electric_refrigerator.n.01_1) 
-        (inside cheese.n.01_2 electric_refrigerator.n.01_1) 
-        (inside cheese.n.01_3 electric_refrigerator.n.01_1) 
-        (inside cheese.n.01_4 electric_refrigerator.n.01_1) 
+        (inside cheddar.n.02_1 electric_refrigerator.n.01_1) 
+        (inside cheddar.n.02_2 electric_refrigerator.n.01_1) 
+        (inside cheddar.n.02_3 electric_refrigerator.n.01_1) 
+        (inside cheddar.n.02_4 electric_refrigerator.n.01_1) 
         (inroom table.n.02_1 dining_room) 
         (inroom electric_refrigerator.n.01_1 kitchen) 
         (inroom cabinet.n.01_1 kitchen) 
         (inroom floor.n.01_1 dining_room) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
@@ -48,14 +48,14 @@
             ) 
             (forpairs 
                 (?salad.n.01 - salad.n.01)
                 (?cracker.n.01 - cracker.n.01)
                 (nextto ?salad.n.01 ?cracker.n.01)
             )
             (forpairs 
-                (?cheese.n.01 - cheese.n.01) 
+                (?cheddar.n.02 - cheddar.n.02) 
                 (?parsley.n.02 - parsley.n.02) 
-                (ontop ?parsley.n.02 ?cheese.n.01)
+                (ontop ?parsley.n.02 ?cheddar.n.02)
             ) 
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/setting_mousetraps/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/setting_mousetraps/problem0.bddl`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem setting_mousetraps_0)
-    (:domain igibson)
+(define (problem setting_mousetraps-0)
+    (:domain omnigibson)
 
     (:objects
      	mousetrap.n.01_1 mousetrap.n.01_2 mousetrap.n.01_3 mousetrap.n.01_4 - mousetrap.n.01
     	sink.n.01_1 - sink.n.01
     	floor.n.01_1 floor.n.01_2 - floor.n.01
     	toilet.n.02_1 - toilet.n.02
         bed.n.01_1 - bed.n.01
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/sorting_mail/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/sorting_mail/problem0.bddl`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem sorting_mail_0)
-    (:domain igibson)
+(define (problem sorting_mail-0)
+    (:domain omnigibson)
 
     (:objects
         envelope.n.01_1 envelope.n.01_2 envelope.n.01_3 envelope.n.01_4 - envelope.n.01
         floor.n.01_1 - floor.n.01
         sofa.n.01_1 - sofa.n.01
         newspaper.n.03_1 newspaper.n.03_2 newspaper.n.03_3 newspaper.n.03_4 - newspaper.n.03
         agent.n.01_1 - agent.n.01
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/storing_food/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/make_meatloaf/problem0.bddl`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,59 @@
-(define (problem storing_food_0)
-    (:domain igibson)
+(define (problem make_meatloaf-0)
+    (:domain omnigibson)
 
     (:objects
-     	oatmeal.n.01_1 oatmeal.n.01_2 - oatmeal.n.01
-    	countertop.n.01_1 - countertop.n.01
-    	chip.n.04_1 chip.n.04_2 - chip.n.04
-    	vegetable_oil.n.01_1 vegetable_oil.n.01_2 - vegetable_oil.n.01
-    	sugar.n.01_1 sugar.n.01_2 - sugar.n.01
-    	cabinet.n.01_1 - cabinet.n.01
-    	floor.n.01_1 - floor.n.01
-    	agent.n.01_1 - agent.n.01
+        ground_beef.n.01_1 - ground_beef.n.01
+        ground_beef__package.n.01_1 - ground_beef__package.n.01
+        whole_milk.n.01_1 - whole_milk.n.01
+        vidalia_onion.n.01_1 - vidalia_onion.n.01
+        breadcrumb.n.01_1 - breadcrumb.n.01
+        brown_sugar.n.01_1 - brown_sugar.n.01
+        catsup.n.01_1 - catsup.n.01
+        meat_loaf.n.01_1 - meat_loaf.n.01
+        oven.n.01_1 - oven.n.01
+        casserole.n.02_1 - casserole.n.02
+        brown_sugar__sack.n.01_1 - brown_sugar__sack.n.01
+        catsup__bottle.n.01_1 - catsup__bottle.n.01
+        chopping_board.n.01_1 - chopping_board.n.01
+        carving_knife.n.01_1 - carving_knife.n.01
+        countertop.n.01_1 - countertop.n.01
+        bowl.n.01_1 - bowl.n.01
+        milk__carton.n.01_1 - milk__carton.n.01
+        electric_refrigerator.n.01_1 - electric_refrigerator.n.01
+        cabinet.n.01_1 - cabinet.n.01
+        agent.n.01_1 - agent.n.01
+        floor.n.01_1 - floor.n.01
     )
     
     (:init 
-        (ontop oatmeal.n.01_1 countertop.n.01_1) 
-        (ontop oatmeal.n.01_2 countertop.n.01_1) 
-        (ontop chip.n.04_1 countertop.n.01_1) 
-        (ontop chip.n.04_2 countertop.n.01_1) 
-        (ontop vegetable_oil.n.01_1 countertop.n.01_1) 
-        (ontop vegetable_oil.n.01_2 countertop.n.01_1) 
-        (ontop sugar.n.01_1 countertop.n.01_1) 
-        (ontop sugar.n.01_2 countertop.n.01_1) 
+        (filled ground_beef__package.n.01_1 ground_beef.n.01_1) 
+        (inside ground_beef__package.n.01_1 electric_refrigerator.n.01_1) 
+        (ontop chopping_board.n.01_1 countertop.n.01_1) 
+        (ontop carving_knife.n.01_1 chopping_board.n.01_1) 
+        (filled milk__carton.n.01_1 whole_milk.n.01_1) 
+        (inside milk__carton.n.01_1 electric_refrigerator.n.01_1) 
+        (ontop vidalia_onion.n.01_1 countertop.n.01_1) 
+        (filled bowl.n.01_1 breadcrumb.n.01_1) 
+        (ontop bowl.n.01_1 countertop.n.01_1) 
+        (filled brown_sugar__sack.n.01_1 brown_sugar.n.01_1) 
+        (inside brown_sugar__sack.n.01_1 cabinet.n.01_1) 
+        (filled catsup__bottle.n.01_1 catsup.n.01_1) 
+        (inside catsup__bottle.n.01_1 electric_refrigerator.n.01_1) 
+        (inroom oven.n.01_1 kitchen) 
+        (inroom electric_refrigerator.n.01_1 kitchen) 
         (inroom countertop.n.01_1 kitchen) 
         (inroom cabinet.n.01_1 kitchen) 
+        (ontop casserole.n.02_1 countertop.n.01_1) 
+        (future meat_loaf.n.01_1) 
         (inroom floor.n.01_1 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
-            (inside ?oatmeal.n.01_1 ?cabinet.n.01_1) 
-            (inside ?oatmeal.n.01_2 ?cabinet.n.01_1) 
-            (inside ?chip.n.04_1 ?cabinet.n.01_1) 
-            (inside ?chip.n.04_2 ?cabinet.n.01_1) 
-            (inside ?vegetable_oil.n.01_1 ?cabinet.n.01_1) 
-            (inside ?vegetable_oil.n.01_2 ?cabinet.n.01_1) 
-            (inside ?sugar.n.01_1 ?cabinet.n.01_1) 
-            (inside ?sugar.n.01_2 ?cabinet.n.01_1)
+            (real ?meat_loaf.n.01_1) 
+            (cooked ?meat_loaf.n.01_1) 
+            (covered ?meat_loaf.n.01_1 ?catsup.n.01_1)
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/thawing_frozen_food/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/thawing_frozen_food/problem0.bddl`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-(define (problem thawing_frozen_food_0)
-    (:domain igibson)
+(define (problem thawing_frozen_food-0)
+    (:domain omnigibson)
 
     (:objects
      	date.n.08_1 - date.n.08
     	electric_refrigerator.n.01_1 - electric_refrigerator.n.01
     	olive.n.04_1 - olive.n.04
     	fish.n.02_1 fish.n.02_2 fish.n.02_3 fish.n.02_4 - fish.n.02
     	sink.n.01_1 - sink.n.01
@@ -28,16 +28,22 @@
         (inroom electric_refrigerator.n.01_1 kitchen) 
         (inroom floor.n.01_1 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
-            (nextto ?date.n.08_1 ?fish.n.02_1) 
-            (nextto ?fish.n.02_1 ?sink.n.01_1) 
-            (nextto ?fish.n.02_2 ?sink.n.01_1) 
-            (nextto ?fish.n.02_3 ?sink.n.01_1) 
-            (nextto ?fish.n.02_4 ?sink.n.01_1) 
-            (nextto ?olive.n.04_1 ?sink.n.01_1)
+            (forall 
+                (?fish.n.02 - fish.n.02)
+                (not
+                    (frozen ?fish.n.02)
+                )
+            )
+            (not
+                (frozen ?date.n.08_1)
+            )
+            (not
+                (frozen ?olive.n.04_1)
+            )
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/unpacking_suitcase/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/unpacking_suitcase/problem0.bddl`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-(define (problem unpacking_suitcase_0)
-    (:domain igibson)
+(define (problem unpacking_suitcase-0)
+    (:domain omnigibson)
 
     (:objects
      	sock.n.01_1 sock.n.01_2 - sock.n.01
     	floor.n.01_1 - floor.n.01
         carton.n.02_1 - carton.n.02
-        perfume.n.02_1 - perfume.n.02
+        bottle__of__perfume.n.01_1 - bottle__of__perfume.n.01
         toothbrush.n.01_1 - toothbrush.n.01
         notebook.n.01_1 - notebook.n.01
     	sofa.n.01_1 - sofa.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
         (ontop carton.n.02_1 floor.n.01_1) 
         (inside sock.n.01_1 carton.n.02_1) 
         (inside sock.n.01_2 carton.n.02_1) 
-        (inside perfume.n.02_1 carton.n.02_1) 
+        (inside bottle__of__perfume.n.01_1 carton.n.02_1)
         (inside toothbrush.n.01_1 carton.n.02_1) 
         (inside notebook.n.01_1 carton.n.02_1) 
         (inroom floor.n.01_1 living_room) 
         (inroom sofa.n.01_1 living_room) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (ontop ?carton.n.02_1 ?floor.n.01_1) 
             (forall 
                 (?sock.n.01 - sock.n.01) 
                 (ontop ?sock.n.01 ?sofa.n.01_1)
             ) 
-            (ontop ?perfume.n.02_1 ?sofa.n.01_1) 
+            (ontop ?bottle__of__perfume.n.01_1 ?sofa.n.01_1)
             (ontop ?toothbrush.n.01_1 ?sofa.n.01_1) 
             (ontop ?notebook.n.01_1 ?sofa.n.01_1)
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/vacuuming_floors/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/store_whole_grains/problem0.bddl`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-(define (problem vacuuming_floors_0)
-    (:domain igibson)
+(define (problem store_whole_grains-0)
+    (:domain omnigibson)
 
     (:objects
-        dust.n.01_1 - dust.n.01
-     	floor.n.01_1 - floor.n.01
-    	vacuum.n.04_1 - vacuum.n.04
-        ashcan.n.01_1 - ashcan.n.01
+     	white_rice.n.01_1 - white_rice.n.01
+    	sack.n.01_1 - sack.n.01
+    	floor.n.01_1 - floor.n.01
+    	mason_jar.n.01_1 - mason_jar.n.01
+    	cabinet.n.01_1 - cabinet.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
-        (covered floor.n.01_1 dust.n.01_1) 
-        (ontop vacuum.n.04_1 floor.n.01_1) 
-        (ontop ashcan.n.01_1 floor.n.01_1) 
-        (inroom floor.n.01_1 bedroom) 
+        (filled sack.n.01_1 white_rice.n.01_1)
+        (ontop sack.n.01_1 floor.n.01_1) 
+        (inside mason_jar.n.01_1 cabinet.n.01_1) 
+        (inroom cabinet.n.01_1 kitchen) 
+        (inroom floor.n.01_1 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
-            (not 
-                (covered ?floor.n.01_1 dust.n.01_1)
-            )
+            (contains ?mason_jar.n.01_1 ?white_rice.n.01_1)
+            (inside ?mason_jar.n.01_1 ?cabinet.n.01_1) 
+            (ontop ?sack.n.01_1 ?floor.n.01_1)
         )
     )
-)
+)
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/washing_floor/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/washing_floor/problem0.bddl`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-(define (problem washing_floor_0)
-    (:domain igibson)
+(define (problem washing_floor-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
         dust.n.01_1 - dust.n.01
      	bucket.n.01_1 - bucket.n.01
     	floor.n.01_1 - floor.n.01
-    	soap.n.01_1 - soap.n.01
+    	bar_soap.n.01_1 - bar_soap.n.01
     	towel.n.01_1 - towel.n.01
     	shower.n.01_1 - shower.n.01
     	toilet.n.02_1 - toilet.n.02
     	bed.n.01_1 - bed.n.01
     	sink.n.01_1 - sink.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
         (ontop bucket.n.01_1 floor.n.01_1) 
-        (ontop soap.n.01_1 towel.n.01_1) 
-        (ontop soap.n.01_1 floor.n.01_1) 
+        (ontop bar_soap.n.01_1 floor.n.01_1) 
         (ontop towel.n.01_1 floor.n.01_1) 
         (not 
             (covered towel.n.01_1 stain.n.01_1)
         ) 
         (covered floor.n.01_1 dust.n.01_1) 
         (covered floor.n.01_1 stain.n.01_1) 
         (inroom floor.n.01_1 bathroom) 
@@ -33,15 +32,15 @@
         (ontop agent.n.01_1 floor.n.01_1)
     )
     
     (:goal 
         (and 
             (not 
                 (or 
-                    (covered ?floor.n.01_1 dust.n.01_1) 
-                    (covered ?floor.n.01_1 stain.n.01_1)
+                    (covered ?floor.n.01_1 ?dust.n.01_1) 
+                    (covered ?floor.n.01_1 ?stain.n.01_1)
                 )
             )
         )
     )
 )
```

### Comparing `bddl-3.0.0b1/bddl/activity_definitions/washing_pots_and_pans/problem0.bddl` & `bddl-3.1.0/bddl/activity_definitions/washing_pots_and_pans/problem0.bddl`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-(define (problem washing_pots_and_pans_0)
-    (:domain igibson)
+(define (problem washing_pots_and_pans-0)
+    (:domain omnigibson)
 
     (:objects
         stain.n.01_1 - stain.n.01
      	teapot.n.01_1 - teapot.n.01
         kettle.n.01_1 - kettle.n.01
     	pan.n.01_1 pan.n.01_2 pan.n.01_3 - pan.n.01
     	countertop.n.01_1 countertop.n.01_2 - countertop.n.01
     	sink.n.01_1 - sink.n.01
     	scrub_brush.n.01_1 - scrub_brush.n.01
-    	soap.n.01_1 - soap.n.01
+    	bar_soap.n.01_1 - bar_soap.n.01
     	cabinet.n.01_1 cabinet.n.01_2 - cabinet.n.01
     	floor.n.01_1 - floor.n.01
     	agent.n.01_1 - agent.n.01
     )
     
     (:init 
         (ontop teapot.n.01_1 countertop.n.01_1) 
@@ -23,15 +23,15 @@
         (ontop pan.n.01_1 countertop.n.01_1) 
         (covered pan.n.01_1 stain.n.01_1) 
         (ontop pan.n.01_2 countertop.n.01_1) 
         (covered pan.n.01_2 stain.n.01_1) 
         (ontop pan.n.01_3 countertop.n.01_2) 
         (covered pan.n.01_3 stain.n.01_1) 
         (ontop scrub_brush.n.01_1 countertop.n.01_2) 
-        (inside soap.n.01_1 sink.n.01_1) 
+        (ontop bar_soap.n.01_1 sink.n.01_1)
         (inroom cabinet.n.01_1 kitchen) 
         (inroom cabinet.n.01_2 kitchen) 
         (inroom sink.n.01_1 kitchen) 
         (inroom countertop.n.01_1 kitchen) 
         (inroom floor.n.01_1 kitchen) 
         (inroom countertop.n.01_2 kitchen) 
         (ontop agent.n.01_1 floor.n.01_1)
```

### Comparing `bddl-3.0.0b1/bddl/activity_manifest.txt` & `bddl-3.1.0/bddl/activity_manifest.txt`

 * *Files identical despite different names*

### Comparing `bddl-3.0.0b1/bddl/activity_to_preselected_scenes.json` & `bddl-3.1.0/bddl/activity_to_preselected_scenes.json`

 * *Files identical despite different names*

### Comparing `bddl-3.0.0b1/bddl/condition_evaluation.py` & `bddl-3.1.0/bddl/condition_evaluation.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,148 +13,177 @@
 
 #################### RECURSIVE PREDICATES ####################
 
 # -JUNCTIONS
 
 
 class Conjunction(Expression):
-    def __init__(self, scope, backend, body, object_map):
+    def __init__(self, scope, backend, body, object_map, generate_ground_options=True):
         super().__init__(scope, backend, body, object_map)
 
         new_scope = copy.copy(scope)
         child_predicates = [
-            get_predicate_for_token(subexpression[0], backend)(new_scope, backend, subexpression[1:], object_map)
+            get_predicate_for_token(subexpression[0], backend)(
+                scope, 
+                backend, 
+                subexpression[1:],
+                object_map,
+                generate_ground_options=generate_ground_options
+            )
             for subexpression in body
         ]
         self.children.extend(child_predicates)
 
-        self.get_ground_options()
+        if generate_ground_options:
+            self.get_ground_options()
 
     def evaluate(self):
         self.child_values = [child.evaluate() for child in self.children]
         assert all([val is not None for val in self.child_values]), "child_values has NoneTypes"
         return all(self.child_values)
 
     def get_ground_options(self):
         options = list(itertools.product(*[child.flattened_condition_options for child in self.children]))
         self.flattened_condition_options = []
         for option in options:
             self.flattened_condition_options.append(list(itertools.chain(*option)))
 
 
 class Disjunction(Expression):
-    def __init__(self, scope, backend, body, object_map):
+    def __init__(self, scope, backend, body, object_map, generate_ground_options=True):
         super().__init__(scope, backend, body, object_map)
 
         # body = [[predicate1], [predicate2], ..., [predicateN]]
         new_scope = copy.copy(scope)
         child_predicates = [
-            get_predicate_for_token(subexpression[0], backend)(new_scope, backend, subexpression[1:], object_map)
+            get_predicate_for_token(subexpression[0], backend)(
+                scope, 
+                backend, 
+                subexpression[1:],
+                object_map,
+                generate_ground_options=generate_ground_options
+            )
             for subexpression in body
         ]
         self.children.extend(child_predicates)
 
-        self.get_ground_options()
+        if generate_ground_options:
+            self.get_ground_options()
 
     def evaluate(self):
         self.child_values = [child.evaluate() for child in self.children]
         assert all([val is not None for val in self.child_values]), "child_values has NoneTypes"
         return any(self.child_values)
 
     def get_ground_options(self):
         self.flattened_condition_options = []
         for child in self.children:
             self.flattened_condition_options.extend(child.flattened_condition_options)
 
 
 # QUANTIFIERS
 class Universal(Expression):
-    def __init__(self, scope, backend, body, object_map):
+    def __init__(self, scope, backend, body, object_map, generate_ground_options=True):
         super().__init__(scope, backend, body, object_map)
         iterable, subexpression = body
         param_label, __, category = iterable
         param_label = param_label.strip("?")
         assert __ == "-", "Middle was not a hyphen"
         for obj_name, obj in scope.items():
             if obj_name in object_map[category]:
                 new_scope = copy.copy(scope)
                 new_scope[param_label] = obj_name
                 self.children.append(
                     get_predicate_for_token(subexpression[0], backend)(
-                        new_scope, backend, subexpression[1:], object_map
+                        new_scope, 
+                        backend, 
+                        subexpression[1:],
+                        object_map,
+                        generate_ground_options=generate_ground_options
                     )
                 )
 
-        self.get_ground_options()
-
+        if generate_ground_options:
+            self.get_ground_options()
+            
     def evaluate(self):
         self.child_values = [child.evaluate() for child in self.children]
         assert all([val is not None for val in self.child_values]), "child_values has NoneTypes"
         return all(self.child_values)
 
     def get_ground_options(self):
         # Accept just a few possible options
         options = list(truncated_product(*[child.flattened_condition_options for child in self.children]))
         self.flattened_condition_options = []
         for option in options:
             self.flattened_condition_options.append(list(itertools.chain(*option)))
 
 
 class Existential(Expression):
-    def __init__(self, scope, backend, body, object_map):
+    def __init__(self, scope, backend, body, object_map, generate_ground_options=True):
         super().__init__(scope, backend, body, object_map)
         iterable, subexpression = body
         param_label, __, category = iterable
         param_label = param_label.strip("?")
         assert __ == "-", "Middle was not a hyphen"
         for obj_name, obj in scope.items():
             if obj_name in object_map[category]:
                 new_scope = copy.copy(scope)
                 new_scope[param_label] = obj_name
                 # body = [["param_label", "-", "category"], [predicate]]
                 self.children.append(
                     get_predicate_for_token(subexpression[0], backend)(
-                        new_scope, backend, subexpression[1:], object_map
+                        new_scope, 
+                        backend, 
+                        subexpression[1:],
+                        object_map,
+                        generate_ground_options=generate_ground_options
                     )
                 )
 
-        self.get_ground_options()
-
+        if generate_ground_options:
+            self.get_ground_options()
+            
     def evaluate(self):
         self.child_values = [child.evaluate() for child in self.children]
         assert all([val is not None for val in self.child_values]), "child_values has NoneTypes"
         return any(self.child_values)
 
     def get_ground_options(self):
         self.flattened_condition_options = []
         for child in self.children:
             self.flattened_condition_options.extend(child.flattened_condition_options)
 
 
 class NQuantifier(Expression):
-    def __init__(self, scope, backend, body, object_map):
+    def __init__(self, scope, backend, body, object_map, generate_ground_options=True):
         super().__init__(scope, backend, body, object_map)
 
         N, iterable, subexpression = body
         self.N = int(N[0])
         param_label, __, category = iterable
         param_label = param_label.strip("?")
         assert __ == "-", "Middle was not a hyphen"
         for obj_name, obj in scope.items():
             if obj_name in object_map[category]:
                 new_scope = copy.copy(scope)
                 new_scope[param_label] = obj_name
                 self.children.append(
                     get_predicate_for_token(subexpression[0], backend)(
-                        new_scope, backend, subexpression[1:], object_map
+                        new_scope, 
+                        backend, 
+                        subexpression[1:],
+                        object_map,
+                        generate_ground_options=generate_ground_options
                     )
                 )
 
-        self.get_ground_options()
-
+        if generate_ground_options:
+            self.get_ground_options()
+            
     def evaluate(self):
         self.child_values = [child.evaluate() for child in self.children]
         assert all([val is not None for val in self.child_values]), "child_values has NoneTypes"
         return sum(self.child_values) == self.N
 
     def get_ground_options(self):
         # Accept just a few possible options
@@ -164,15 +193,15 @@
             # for combination in [combo for num_el in range(self.N - 1, len(option)) for combo in itertools.combinations(option, num_el + 1)]:
             # Use a minimal solution (exactly N fulfilled, rather than >=N fulfilled)
             for combination in itertools.combinations(option, self.N):
                 self.flattened_condition_options.append(list(itertools.chain(*combination)))
 
 
 class ForPairs(Expression):
-    def __init__(self, scope, backend, body, object_map):
+    def __init__(self, scope, backend, body, object_map, generate_ground_options=True):
         super().__init__(scope, backend, body, object_map)
 
         iterable1, iterable2, subexpression = body
         param_label1, __, category1 = iterable1
         param_label2, __, category2 = iterable2
         param_label1 = param_label1.strip("?")
         param_label2 = param_label2.strip("?")
@@ -182,21 +211,26 @@
                 for obj_name_2, obj_2 in scope.items():
                     if obj_name_2 in object_map[category2] and obj_name_1 != obj_name_2:
                         new_scope = copy.copy(scope)
                         new_scope[param_label1] = obj_name_1
                         new_scope[param_label2] = obj_name_2
                         sub.append(
                             get_predicate_for_token(subexpression[0], backend)(
-                                new_scope, backend, subexpression[1:], object_map
+                                new_scope, 
+                                backend, 
+                                subexpression[1:],
+                                object_map,
+                                generate_ground_options=generate_ground_options
                             )
                         )
                 self.children.append(sub)
 
-        self.get_ground_options()
-
+        if generate_ground_options:
+            self.get_ground_options()
+            
     def evaluate(self):
         self.child_values = np.array([np.array([subchild.evaluate() for subchild in child]) for child in self.children])
 
         L = min(len(self.children), len(self.children[0]))
         return (np.sum(np.any(self.child_values, axis=1), axis=0) >= L) and (
             np.sum(np.any(self.child_values, axis=0), axis=0) >= L
         )
@@ -221,15 +255,15 @@
                 unpacked_choice_options = []
                 for choice_option in choice_options:
                     unpacked_choice_options.append(list(itertools.chain(*choice_option)))
                 self.flattened_condition_options.extend(unpacked_choice_options)
 
 
 class ForNPairs(Expression):
-    def __init__(self, scope, backend, body, object_map):
+    def __init__(self, scope, backend, body, object_map, generate_ground_options=True):
         super().__init__(scope, backend, body, object_map)
 
         N, iterable1, iterable2, subexpression = body
         self.N = int(N[0])
         param_label1, __, category1 = iterable1
         param_label2, __, category2 = iterable2
         param_label1 = param_label1.strip("?")
@@ -240,21 +274,26 @@
                 for obj_name_2, obj_2 in scope.items():
                     if obj_name_2 in object_map[category2] and obj_name_1 != obj_name_2:
                         new_scope = copy.copy(scope)
                         new_scope[param_label1] = obj_name_1
                         new_scope[param_label2] = obj_name_2
                         sub.append(
                             get_predicate_for_token(subexpression[0], backend)(
-                                new_scope, backend, subexpression[1:], object_map
+                                new_scope, 
+                                backend, 
+                                subexpression[1:],
+                                object_map,
+                                generate_ground_options=generate_ground_options
                             )
                         )
                 self.children.append(sub)
 
-        self.get_ground_options()
-
+        if generate_ground_options:
+            self.get_ground_options()
+            
     def evaluate(self):
         self.child_values = np.array([np.array([subchild.evaluate() for subchild in child]) for child in self.children])
         return (np.sum(np.any(self.child_values, axis=1), axis=0) >= self.N) and (
             np.sum(np.any(self.child_values, axis=0), axis=0) >= self.N
         )
 
     def get_ground_options(self):
@@ -274,26 +313,33 @@
                 for choice_option in choice_options:
                     unpacked_choice_options.append(list(itertools.chain(*choice_option)))
                 self.flattened_condition_options.extend(unpacked_choice_options)
 
 
 # NEGATION
 class Negation(Expression):
-    def __init__(self, scope, backend, body, object_map):
+    def __init__(self, scope, backend, body, object_map, generate_ground_options=True):
         super().__init__(scope, backend, body, object_map)
 
         # body = [[predicate]]
         subexpression = body[0]
         self.children.append(
-            get_predicate_for_token(subexpression[0], backend)(scope, backend, subexpression[1:], object_map)
+            get_predicate_for_token(subexpression[0], backend)(
+                scope, 
+                backend, 
+                subexpression[1:],
+                object_map,
+                generate_ground_options=generate_ground_options
+            )
         )
         assert len(self.children) == 1, "More than one child."
 
-        self.get_ground_options()
-
+        if generate_ground_options:
+            self.get_ground_options()
+            
     def evaluate(self):
         self.child_values = [child.evaluate() for child in self.children]
         assert len(self.child_values) == 1, "More than one child value"
         assert all([val is not None for val in self.child_values]), "child_values has NoneTypes"
         return not self.child_values[0]
 
     def get_ground_options(self):
@@ -309,28 +355,41 @@
         # only picking one condition from each set of disjuncts
         for negated_option_selections in itertools.product(*negated_options):
             self.flattened_condition_options.append(list(itertools.chain(negated_option_selections)))
 
 
 # IMPLICATION
 class Implication(Expression):
-    def __init__(self, scope, backend, body, object_map):
+    def __init__(self, scope, backend, body, object_map, generate_ground_options=True):
         super().__init__(scope, backend, body, object_map)
 
         # body = [[antecedent], [consequent]]
         antecedent, consequent = body
         self.children.append(
-            get_predicate_for_token(antecedent[0], backend)(scope, backend, antecedent[1:], object_map)
+            get_predicate_for_token(antecedent[0], backend)(
+                scope, 
+                backend, 
+                antecedent[1:],
+                object_map,
+                generate_ground_options=generate_ground_options
+            )
         )
         self.children.append(
-            get_predicate_for_token(consequent[0], backend)(scope, backend, consequent[1:], object_map)
+            get_predicate_for_token(consequent[0], backend)(
+                scope, 
+                backend, 
+                consequent[1:],
+                object_map,
+                generate_ground_options=generate_ground_options
+            )
         )
 
-        self.get_ground_options()
-
+        if generate_ground_options:
+            self.get_ground_options()
+            
     def evaluate(self):
         self.child_values = [child.evaluate() for child in self.children]
         assert all([val is not None for val in self.child_values]), "child_values has NoneTypes"
         ante, cons = self.child_values
         return (not ante) or cons
 
     def get_ground_options(self):
@@ -351,26 +410,33 @@
         self.flattened_condition_options = flattened_neg_antecedent_options + flattened_consequent_options
 
 
 # HEAD
 
 
 class HEAD(Expression):
-    def __init__(self, scope, backend, body, object_map):
+    def __init__(self, scope, backend, body, object_map, generate_ground_options=True):
         super().__init__(scope, backend, body, object_map)
 
         subexpression = body
         self.children.append(
-            get_predicate_for_token(subexpression[0], backend)(scope, backend, subexpression[1:], object_map)
+            get_predicate_for_token(subexpression[0], backend)(
+                scope, 
+                backend, 
+                subexpression[1:],
+                object_map,
+                generate_ground_options=generate_ground_options
+            )
         )
 
         self.terms = [term.lstrip("?") for term in list(flatten_list(self.body))]
 
-        self.get_ground_options()
-
+        if generate_ground_options:
+            self.get_ground_options()
+            
     def evaluate(self):
         self.child_values = [child.evaluate() for child in self.children]
         assert len(self.child_values) == 1, "More than one child value"
         self.currently_satisfied = self.child_values[0]
         return self.currently_satisfied
 
     def get_relevant_objects(self):
@@ -402,19 +468,25 @@
     scope = {}
     for object_cat in object_terms:
         for object_inst in object_terms[object_cat]:
             scope[object_inst] = None
     return scope
 
 
-def compile_state(parsed_state, backend, scope=None, object_map=None):
+def compile_state(parsed_state, backend, scope=None, object_map=None, generate_ground_options=True):
     compiled_state = []
     for parsed_condition in parsed_state:
         scope = scope if scope is not None else {}
-        compiled_state.append(HEAD(scope, backend, parsed_condition, object_map))
+        compiled_state.append(HEAD(
+            scope, 
+            backend, 
+            parsed_condition, 
+            object_map, 
+            generate_ground_options=generate_ground_options
+        ))
     return compiled_state
 
 def evaluate_state(compiled_state):
     results = {"satisfied": [], "unsatisfied": []}
     for i, compiled_condition in enumerate(compiled_state):
         if compiled_condition.evaluate():
             results["satisfied"].append(i)
```

### Comparing `bddl-3.0.0b1/bddl/config.py` & `bddl-3.1.0/bddl/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 
 # PATHS
-ACTIVITY_CONFIGS_PATH = os.path.join(
-    os.path.dirname(__file__), 'activity_definitions')
+ACTIVITY_CONFIGS_PATH = os.path.join(os.path.dirname(__file__), 'activity_definitions')
 
 # BDDL
 SUPPORTED_BDDL_REQUIREMENTS = [':strips', ':negative-preconditions', ':typing', ':adl']
 
 READABLE_PREDICATE_NAMES = {
     'ontop': 'on top of',
     'nextto': 'next to'
```

### Comparing `bddl-3.0.0b1/bddl/logic_base.py` & `bddl-3.1.0/bddl/logic_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,31 +23,32 @@
     def __init__(self, scope, backend, body, object_map):
         super().__init__(scope, backend, body, object_map)
 
 
 class BinaryAtomicFormula(AtomicFormula):
     STATE_NAME = None
 
-    def __init__(self, scope, backend, body, object_map):
+    def __init__(self, scope, backend, body, object_map, generate_ground_options=True):
         super().__init__(scope, backend, body, object_map)
-        assert len(body) == 2, 'Param list should have 2 args'
+        assert len(body) == 2, f'Param list for predicate {self.STATE_NAME} should have 2 args'
         self.input1, self.input2 = [inp.strip('?') for inp in body]
         self.scope = scope
         try:
             if isinstance(self.scope[self.input1], str):
                 self.input1 = self.scope[self.input1]
-        except KeyError:
-            raise UncontrolledCategoryError
+        except KeyError as e:
+            raise UncontrolledCategoryError(e)
         try:
             if isinstance(self.scope[self.input2], str):
                 self.input2 = self.scope[self.input2]
-        except KeyError:
-            raise UncontrolledCategoryError
+        except KeyError as e:
+            raise UncontrolledCategoryError(e)
 
-        self.get_ground_options()
+        if generate_ground_options:
+            self.get_ground_options()
 
     @abstractmethod
     def _evaluate(self, obj1, obj2):
         pass
 
     def evaluate(self):
         if (self.scope[self.input1] is not None) and (self.scope[self.input2] is not None):
@@ -71,26 +72,27 @@
         self.flattened_condition_options = [
             [[self.STATE_NAME, self.input1, self.input2]]]
 
 
 class UnaryAtomicFormula(AtomicFormula):
     STATE_NAME = None
 
-    def __init__(self, scope, backend, body, object_map):
+    def __init__(self, scope, backend, body, object_map, generate_ground_options=True):
         super().__init__(scope, backend, body, object_map)
-        assert len(body) == 1, 'Param list should have 1 arg'
+        assert len(body) == 1, f'Param list for predicate {self.STATE_NAME} should have 1 arg'
         self.input = body[0].strip('?')
         self.scope = scope
         try:
             if isinstance(self.scope[self.input], str):
                 self.input = self.scope[self.input]
-        except KeyError:
-            raise UncontrolledCategoryError
-
-        self.get_ground_options()
+        except KeyError as e:
+            raise UncontrolledCategoryError(e)
+        
+        if generate_ground_options:
+            self.get_ground_options()
 
     @abstractmethod
     def _evaluate(self, obj):
         pass
 
     def evaluate(self):
         if self.scope[self.input] is not None:
```

### Comparing `bddl-3.0.0b1/bddl/parsing.py` & `bddl-3.1.0/bddl/parsing.py`

 * *Files 18% similar despite different names*

```diff
@@ -60,19 +60,16 @@
                 domain_name = group[0]
             elif t == ':requirements':
                 for req in group:
                     if not req in supported_requirements:
                         raise Exception('Requirement %s not supported' % req)
                 requirements = group
             elif t == ':predicates':
-                predicate_name, arguments = parse_predicates(group)
-                if predicate_name in predicates:
-                    raise Exception(
-                        'Predicate %s defined multiple times' % predicate_name)
-                predicates[predicate_name] = arguments
+                # predicate_name, arguments = parse_predicates(group)
+                predicates = parse_predicates(group)
             elif t == ':types':
                 types = group
             elif t == ':action':
                 name = group.pop(0)
                 for act in actions:
                     if act.name == name:
                         raise Exception(
@@ -83,14 +80,15 @@
         return domain_name, requirements, types, actions, predicates
     else:
         raise Exception('File %s does not match domain pattern' %
                         domain_filename)
 
 
 def parse_predicates(group):
+    predicates = {}
     for pred in group:
         predicate_name = pred.pop(0)
         arguments = {}
         untyped_variables = []
         while pred:
             t = pred.pop(0)
             if t == '-':
@@ -99,15 +97,17 @@
                 var_type = pred.pop(0)
                 while untyped_variables:
                     arguments[untyped_variables.pop(0)] = var_type
             else:
                 untyped_variables.append(t)
         while untyped_variables:
             arguments[untyped_variables.pop(0)] = 'object'
-        return predicate_name, arguments
+        # print(predicates)
+        predicates[predicate_name] = arguments
+    return predicates
 
 
 def parse_action(group):
     name = group.pop(0)
     if not isinstance(name, str):
         raise Exception('Action without name definition')
     parameters = []
@@ -440,12 +440,72 @@
                 {object_list}\n
                 {init_state}\n
                 {goal_state}\n
                )"""
     return bddl
 
 
+def construct_bddl_from_parsed(behavior_activity, activity_definition, parsed_object_list, parsed_init_state, parsed_goal_state, domain="omnigibson"):
+    object_list = "(:objects\n"
+    for object_cat, object_insts in parsed_object_list.items():
+        object_list += f"        " + " ".join(object_insts) + f" - {object_cat}\n"
+    object_list += "    )"
+
+    init_state = f"(:init"
+    for literal in parsed_init_state:
+        if literal[0] == "not": 
+            init_state += f" (not ({' '.join(literal[1])}))"
+        else:
+            init_state += f" ({' '.join(literal)})"
+    init_state += ")"
+    init_state = add_bddl_whitespace(string=init_state, save=False)
+    init_state = "\n    ".join(init_state.split("\n"))
+    
+    goal_state = f"(:goal {build_goal(['and'] + parsed_goal_state)})"
+    goal_state = add_bddl_whitespace(string=goal_state, save=False)
+    goal_state = "\n    ".join(goal_state.split("\n"))
+
+    bddl = f"""(define (problem {behavior_activity}_{activity_definition})
+    (:domain {domain})\n
+    {object_list}
+    {init_state}
+    {goal_state}
+)"""
+    return bddl
+
+
+def build_goal(goal_expr):
+    if type(goal_expr[1]) == list:
+        return f"({goal_expr[0]} {' '.join([build_goal(subexpr) for subexpr in goal_expr[1:]])})"
+    else: 
+        return f"({' '.join(goal_expr)})"
+
+
 if __name__ == '__main__':
     if sys.argv[1] == 'add':
         refined_bddl = add_bddl_whitespace()
     if sys.argv[1] == 'remove':
         refined_bddl = remove_bddl_whitespace()
+    if sys.argv[1] == "construct_from_parsed":
+        activity = "cleaning_up_after_a_meal"
+        __, objs, init, goal = parse_problem(activity, 0, "igibson")
+        reconstruction = construct_bddl_from_parsed(activity, 0, objs, init, goal, domain="igibson")
+        with open(f"activity_definitions/{activity}/problem0.bddl", "r") as f:
+            defn_lines = f.read().split("\n")
+        reconstruction_lines = reconstruction.split("\n")
+        print("Length same:", len(defn_lines) == len(reconstruction_lines))
+        print(len(defn_lines))
+        print(len(reconstruction_lines))
+        # pprint.pprint(defn_lines)
+        # pprint.pprint(reconstruction_lines)
+        # print(reconstruction)
+        for i in range(len(reconstruction_lines)): 
+            # print(defn_lines[i].strip() == reconstruction_lines[i].strip())
+            if defn_lines[i].strip() != reconstruction_lines[i].strip():
+                print(defn_lines[i].strip())
+                print(reconstruction_lines[i].strip())
+                print(f"{i} doesn't match")
+                print()
+                import sys; sys.exit()
+            else:
+                continue
+                # print(i)
```

### Comparing `bddl-3.0.0b1/bddl/utils.py` & `bddl-3.1.0/bddl/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,16 @@
         else:
             return
 
 
 ########## CUSTOM ERRORS ############
 
 class UncontrolledCategoryError(Exception):
-    pass
+    def __init__(self, malformed_cat):
+        self.malformed_cat = malformed_cat
 
 class UnsupportedPredicateError(Exception):
     def __init__(self, predicate):
         self.predicate = predicate
 
 
 if __name__ == "__main__":
```

### Comparing `bddl-3.0.0b1/bddl.egg-info/PKG-INFO` & `bddl-3.1.0/bddl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: bddl
-Version: 3.0.0b1
+Version: 3.1.0
 Home-page: https://github.com/StanfordVL/bddl
 Author: Stanford University
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Behavior Domain Definition Language 
 
-**Note: You are reading the docs for the 3.0.0b1 release, which is a backwards-incompatible version of BDDL containing a subset of BEHAVIOR-1K activities released as part of the BEHAVIOR-1K beta release. Please go to the tags menu to see BEHAVIOR-100 code and files.**
+**Note: You are reading the docs for the 3.1.0 release, which is a backwards-incompatible version of BDDL containing a subset of BEHAVIOR-1K activities released as part of the BEHAVIOR-1K beta release. Please go to the tags menu to see BEHAVIOR-100 code and files.**
 
 The Behavior Domain Definition Language (BDDL) is a domain-specific language designed for the Benchmark for Everyday Household Activities in Virtual, Interactive, and ecOlogical enviRonments (BEHAVIOR). 
 
 BDDL is a predicate logic-based language inspired by, but distinct from, the Planning Domain Definition Language [1]. It defines each BEHAVIOR activity definition as a BDDL `problem`, consisting of of a categorized object list (`:objects`), an initial condition that has only ground literals (`:init`), and a goal condition that is a logical expression (`:goal`). 
 
 ## Installation
```

### Comparing `bddl-3.0.0b1/setup.py` & `bddl-3.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 # TODO package data
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='bddl',
-    version='3.0.0b1',
+    version='3.1.0',
     author='Stanford University',
     long_description_content_type='text/markdown',
     long_description=long_description,
     url='https://github.com/StanfordVL/bddl',
     zip_safe=False,
     packages=find_packages(),
     install_requires=[
         'pytest',
         'numpy',
         'networkx',
-        'jupytext'
+        'jupytext',
+        'future',
     ],
     package_data={},
     include_package_data=True
 )
```

