# Comparing `tmp/cosmicfrog-0.3.4.tar.gz` & `tmp/cosmicfrog-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmicfrog-0.3.4.tar", last modified: Tue Aug  1 14:48:36 2023, max compression
+gzip compressed data, was "cosmicfrog-0.3.5.tar", last modified: Thu Aug  3 13:09:25 2023, max compression
```

## Comparing `cosmicfrog-0.3.4.tar` & `cosmicfrog-0.3.5.tar`

### file list

```diff
@@ -1,234 +1,234 @@
-drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-08-01 14:48:36.109935 cosmicfrog-0.3.4/
--rw-r--r--   0 gordon    (1000) gordon    (1000)      352 2023-08-01 14:48:36.109935 cosmicfrog-0.3.4/PKG-INFO
--rw-r--r--   0 gordon    (1000) gordon    (1000)      486 2023-06-13 10:31:10.000000 cosmicfrog-0.3.4/README.md
-drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-08-01 14:48:36.069935 cosmicfrog-0.3.4/cosmicfrog/
--rw-r--r--   0 gordon    (1000) gordon    (1000)       92 2023-06-27 13:30:38.000000 cosmicfrog-0.3.4/cosmicfrog/__init__.py
-drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-08-01 14:48:36.069935 cosmicfrog-0.3.4/cosmicfrog/anura/
-drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-08-01 14:48:36.109935 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/
--rw-r--r--   0 gordon    (1000) gordon    (1000)     8022 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_AdvancedQueueingDetails.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2629 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Analytics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5905 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_BillsOfMaterials.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2198 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_BusinessCalendars.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10838 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_BusinessHours.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6637 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ChangeoverTimes.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6430 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomSimulationScripts.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13497 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomerDemand.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    15862 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    17710 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12342 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomerOrderProfiles.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18271 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomerOrders.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6525 2023-06-07 11:19:52.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomerRiskConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13321 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomerTransitConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18203 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Customers.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12984 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomersMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    31026 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Facilities.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    23117 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_FacilitiesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7737 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_FacilityCountConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13103 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_FacilityDemand.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7405 2023-06-07 11:19:52.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_FacilityRiskConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13263 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_FlowConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13438 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_FlowCountConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13943 2023-06-07 11:19:52.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_GeographicRiskConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4504 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_GreenfieldServiceBands.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    11840 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_GreenfieldSettings.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5179 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Groups.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2401 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Histograms.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9384 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_InputFactors.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10320 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_InventoryConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9604 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_InventoryCountConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    37919 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_InventoryPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    39657 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_InventoryPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6883 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Lookups.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3239 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Maps.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5949 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ModelInfo.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7320 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ModelRunOptions.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    19168 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ModelSettings.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9656 2023-06-07 11:19:52.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_NetworkRiskConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9469 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_OrderFulfillmentPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3602 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_OrderProfileProductAffinity.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5317 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_OrderProfileProductSelection.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4329 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_OrderedProductSubstitution.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2583 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Organizations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6687 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_OutputFactors.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2796 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Periods.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    28592 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Processes.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    26042 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProcessesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12346 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProcurementOrderProfiles.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    15370 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProcurementOrders.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    14833 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProcurementPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16683 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProcurementPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3296 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductUnitsOfMeasure.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13669 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductionConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13977 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductionCountConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12389 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductionOrderProfiles.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12870 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductionOrders.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13999 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductionPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    15546 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductionPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13797 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Products.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7335 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductsMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12348 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrderProfiles.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    15376 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrders.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16715 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ReplenishmentPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18561 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ReplenishmentPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3189 2023-06-07 11:19:52.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_RiskBandDefinitions.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3278 2023-06-07 11:19:52.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_RiskRatingConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4718 2023-06-07 11:19:52.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_RiskSummaryConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2879 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ScenarioItemAssignments.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5353 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ScenarioItems.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4340 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Scenarios.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6460 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_SequentialObjectives.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10685 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Shipments.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5798 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_StepCosts.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4536 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_SupplierCapabilities.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6481 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_SupplierCapabilitiesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5864 2023-06-07 11:19:52.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_SupplierRiskConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    11580 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Suppliers.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6647 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_SuppliersMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3162 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TableFilters.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16686 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationAssets.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18492 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationAssetsMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9955 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationLaneModeQueueDetails.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9181 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationLaneQueueDetails.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    22940 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationModes.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    21819 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationModesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    32814 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    30886 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9956 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationRates.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4705 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_UnitsOfMeasure.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5569 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_UserDefinedConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4111 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_UserDefinedCosts.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4092 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_UserDefinedForecasts.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3647 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_UserDefinedForecastsData.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    25027 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_UserDefinedVariables.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6574 2023-06-07 11:19:52.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_UtilizationRiskConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13974 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WarehousingPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    15701 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WarehousingPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9490 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WorkCenterCountConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7661 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WorkCenterQueueDetails.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18790 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WorkCenters.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18860 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WorkCentersMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10171 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WorkResources.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    11935 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WorkResourcesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     8862 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationBillsOfMaterialSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10784 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationConstraintSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3526 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeParentInformationReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    20156 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7056 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationCustomerRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16396 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationCustomerSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16803 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationDemandSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    21094 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationFacilityCostToServeSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7914 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationFacilityRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    34222 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationFacilitySummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    22234 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationFlowSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9424 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGeographicRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6017 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10219 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6970 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilityRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    17471 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilitySummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12634 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFlowSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9490 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldGeographicRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4522 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10498 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5722 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldRiskMetricsSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4787 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldServiceBandSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6799 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    14082 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16823 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationInventorySummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6246 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationNetworkRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    28983 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationNetworkSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    14164 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationProcessSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4063 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationProductRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12557 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationProductionSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5709 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationRiskMetricsSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4864 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationSequentialObjectiveSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9345 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationShipmentSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6767 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationSupplierRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12537 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationSupplierSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9475 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationSupplySummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4764 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedCostSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     1961 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedVariableSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6460 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationUtilizationRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7043 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationValidationErrorReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    15917 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationWarehousingSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    17090 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationWorkCenterSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    34065 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    33862 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18726 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18541 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7903 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7715 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    39373 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    40023 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    20366 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    20172 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2128 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmInputFactorReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2969 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmOutputFactorReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2411 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    55257 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    55033 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    32669 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    32484 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7506 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7319 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    63682 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    63410 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    26655 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    26664 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    14419 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFlowSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    14419 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFlowSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10273 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10109 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6316 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationInventoryOnHandReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4594 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueDepthReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     8524 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     8551 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4040 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueDepthReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7970 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7997 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12980 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13007 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5341 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5368 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    60336 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    60255 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    31510 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    31476 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2944 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueDepthReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5725 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5764 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10657 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationOrderReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16391 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationProcessReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    11893 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationProcessSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    11920 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationProcessSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3619 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3646 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7968 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationProductionReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6540 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6364 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12327 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationShipmentReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6846 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6885 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6204 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6263 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     8923 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     8950 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5664 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationValidationErrorReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4045 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueDepthReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6275 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6302 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9604 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9631 2023-05-26 16:01:42.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummaryReplicationDetail.json
-drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-08-01 14:48:36.109935 cosmicfrog-0.3.4/cosmicfrog/anura/table_masterlists/
--rw-r--r--   0 gordon    (1000) gordon    (1000)    57001 2023-06-07 11:19:52.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_masterlists/anuraMasterTableList.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    25920 2023-06-07 11:19:52.000000 cosmicfrog-0.3.4/cosmicfrog/anura/table_masterlists/anuraOutputTableList.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    15602 2023-08-01 14:24:32.000000 cosmicfrog-0.3.4/cosmicfrog/frog_data.py
--rw-r--r--   0 gordon    (1000) gordon    (1000)      288 2023-04-14 21:19:53.000000 cosmicfrog-0.3.4/cosmicfrog/frog_excel.py
--rw-r--r--   0 gordon    (1000) gordon    (1000)     1502 2023-06-22 17:23:48.000000 cosmicfrog-0.3.4/cosmicfrog/frog_log.py
-drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-08-01 14:48:36.069935 cosmicfrog-0.3.4/cosmicfrog.egg-info/
--rw-r--r--   0 gordon    (1000) gordon    (1000)      352 2023-08-01 14:48:36.000000 cosmicfrog-0.3.4/cosmicfrog.egg-info/PKG-INFO
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16502 2023-08-01 14:48:36.000000 cosmicfrog-0.3.4/cosmicfrog.egg-info/SOURCES.txt
--rw-r--r--   0 gordon    (1000) gordon    (1000)        1 2023-08-01 14:48:36.000000 cosmicfrog-0.3.4/cosmicfrog.egg-info/dependency_links.txt
--rw-r--r--   0 gordon    (1000) gordon    (1000)      114 2023-08-01 14:48:36.000000 cosmicfrog-0.3.4/cosmicfrog.egg-info/requires.txt
--rw-r--r--   0 gordon    (1000) gordon    (1000)       11 2023-08-01 14:48:36.000000 cosmicfrog-0.3.4/cosmicfrog.egg-info/top_level.txt
--rw-r--r--   0 gordon    (1000) gordon    (1000)       38 2023-08-01 14:48:36.109935 cosmicfrog-0.3.4/setup.cfg
--rw-r--r--   0 gordon    (1000) gordon    (1000)      899 2023-08-01 14:07:18.000000 cosmicfrog-0.3.4/setup.py
+drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-08-03 13:09:25.668184 cosmicfrog-0.3.5/
+-rw-r--r--   0 gordon    (1000) gordon    (1000)      352 2023-08-03 13:09:25.668184 cosmicfrog-0.3.5/PKG-INFO
+-rw-r--r--   0 gordon    (1000) gordon    (1000)      486 2023-06-13 10:31:10.000000 cosmicfrog-0.3.5/README.md
+drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-08-03 13:09:25.616184 cosmicfrog-0.3.5/cosmicfrog/
+-rw-r--r--   0 gordon    (1000) gordon    (1000)       92 2023-06-27 13:30:38.000000 cosmicfrog-0.3.5/cosmicfrog/__init__.py
+drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-08-03 13:09:25.612184 cosmicfrog-0.3.5/cosmicfrog/anura/
+drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-08-03 13:09:25.664184 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     8022 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_AdvancedQueueingDetails.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2629 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Analytics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5905 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_BillsOfMaterials.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2198 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_BusinessCalendars.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10838 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_BusinessHours.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6637 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ChangeoverTimes.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6430 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomSimulationScripts.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13497 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomerDemand.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    15862 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    17710 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12342 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomerOrderProfiles.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18271 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomerOrders.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6525 2023-06-07 11:19:52.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomerRiskConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13321 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomerTransitConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18203 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Customers.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12984 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomersMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    31026 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Facilities.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    23117 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_FacilitiesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7737 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_FacilityCountConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13103 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_FacilityDemand.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7405 2023-06-07 11:19:52.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_FacilityRiskConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13263 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_FlowConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13438 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_FlowCountConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13943 2023-06-07 11:19:52.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_GeographicRiskConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4504 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_GreenfieldServiceBands.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    11840 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_GreenfieldSettings.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5179 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Groups.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2401 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Histograms.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9384 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_InputFactors.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10320 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_InventoryConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9604 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_InventoryCountConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    37919 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_InventoryPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    39657 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_InventoryPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6883 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Lookups.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3239 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Maps.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5949 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ModelInfo.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7320 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ModelRunOptions.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    19168 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ModelSettings.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9656 2023-06-07 11:19:52.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_NetworkRiskConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9469 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_OrderFulfillmentPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3602 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_OrderProfileProductAffinity.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5317 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_OrderProfileProductSelection.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4329 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_OrderedProductSubstitution.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2583 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Organizations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6687 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_OutputFactors.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2796 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Periods.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    28592 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Processes.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    26042 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProcessesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12346 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProcurementOrderProfiles.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    15370 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProcurementOrders.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    14833 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProcurementPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16683 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProcurementPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3296 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductUnitsOfMeasure.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13669 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductionConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13977 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductionCountConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12389 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductionOrderProfiles.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12870 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductionOrders.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13999 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductionPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    15546 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductionPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13797 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Products.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7335 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductsMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12348 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrderProfiles.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    15376 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrders.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16715 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ReplenishmentPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18561 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ReplenishmentPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3189 2023-06-07 11:19:52.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_RiskBandDefinitions.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3278 2023-06-07 11:19:52.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_RiskRatingConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4718 2023-06-07 11:19:52.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_RiskSummaryConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2879 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ScenarioItemAssignments.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5353 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ScenarioItems.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4340 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Scenarios.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6460 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_SequentialObjectives.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10685 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Shipments.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5798 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_StepCosts.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4536 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_SupplierCapabilities.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6481 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_SupplierCapabilitiesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5864 2023-06-07 11:19:52.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_SupplierRiskConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    11580 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Suppliers.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6647 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_SuppliersMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3162 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TableFilters.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16686 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationAssets.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18492 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationAssetsMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9955 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationLaneModeQueueDetails.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9181 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationLaneQueueDetails.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    22940 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationModes.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    21819 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationModesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    32814 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    30886 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9956 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationRates.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4705 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_UnitsOfMeasure.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5569 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_UserDefinedConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4111 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_UserDefinedCosts.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4092 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_UserDefinedForecasts.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3647 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_UserDefinedForecastsData.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    25027 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_UserDefinedVariables.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6574 2023-06-07 11:19:52.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_UtilizationRiskConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13974 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WarehousingPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    15701 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WarehousingPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9490 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WorkCenterCountConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7661 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WorkCenterQueueDetails.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18790 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WorkCenters.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18860 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WorkCentersMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10171 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WorkResources.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    11935 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WorkResourcesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     8862 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationBillsOfMaterialSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10784 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationConstraintSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3526 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeParentInformationReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    20156 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7056 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationCustomerRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16396 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationCustomerSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16803 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationDemandSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    21094 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationFacilityCostToServeSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7914 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationFacilityRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    34222 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationFacilitySummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    22234 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationFlowSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9424 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGeographicRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6017 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10219 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6970 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilityRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    17471 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilitySummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12634 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFlowSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9490 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldGeographicRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4522 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10498 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5722 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldRiskMetricsSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4787 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldServiceBandSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6799 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    14082 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16823 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationInventorySummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6246 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationNetworkRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    28983 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationNetworkSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    14164 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationProcessSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4063 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationProductRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12557 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationProductionSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5709 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationRiskMetricsSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4864 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationSequentialObjectiveSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9345 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationShipmentSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6767 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationSupplierRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12537 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationSupplierSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9475 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationSupplySummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4764 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedCostSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     1961 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedVariableSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6460 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationUtilizationRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7043 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationValidationErrorReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    15917 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationWarehousingSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    17090 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationWorkCenterSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    34065 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    33862 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18726 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18541 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7903 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7715 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    39373 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    40023 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    20366 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    20172 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2128 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmInputFactorReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2969 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmOutputFactorReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2411 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    55257 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    55033 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    32669 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    32484 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7506 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7319 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    63682 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    63410 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    26655 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    26664 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    14419 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFlowSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    14419 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFlowSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10273 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10109 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6316 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationInventoryOnHandReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4594 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueDepthReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     8524 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     8551 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4040 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueDepthReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7970 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7997 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12980 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13007 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5341 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5368 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    60336 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    60255 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    31510 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    31476 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2944 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueDepthReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5725 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5764 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10657 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationOrderReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16391 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationProcessReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    11893 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationProcessSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    11920 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationProcessSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3619 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3646 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7968 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationProductionReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6540 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6364 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12327 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationShipmentReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6846 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6885 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6204 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6263 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     8923 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     8950 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5664 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationValidationErrorReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4045 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueDepthReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6275 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6302 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9604 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9631 2023-05-26 16:01:42.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummaryReplicationDetail.json
+drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-08-03 13:09:25.668184 cosmicfrog-0.3.5/cosmicfrog/anura/table_masterlists/
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    57001 2023-06-07 11:19:52.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_masterlists/anuraMasterTableList.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    25920 2023-06-07 11:19:52.000000 cosmicfrog-0.3.5/cosmicfrog/anura/table_masterlists/anuraOutputTableList.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    15890 2023-08-03 12:54:02.000000 cosmicfrog-0.3.5/cosmicfrog/frog_data.py
+-rw-r--r--   0 gordon    (1000) gordon    (1000)      288 2023-04-14 21:19:53.000000 cosmicfrog-0.3.5/cosmicfrog/frog_excel.py
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     1502 2023-06-22 17:23:48.000000 cosmicfrog-0.3.5/cosmicfrog/frog_log.py
+drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-08-03 13:09:25.616184 cosmicfrog-0.3.5/cosmicfrog.egg-info/
+-rw-r--r--   0 gordon    (1000) gordon    (1000)      352 2023-08-03 13:09:25.000000 cosmicfrog-0.3.5/cosmicfrog.egg-info/PKG-INFO
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16502 2023-08-03 13:09:25.000000 cosmicfrog-0.3.5/cosmicfrog.egg-info/SOURCES.txt
+-rw-r--r--   0 gordon    (1000) gordon    (1000)        1 2023-08-03 13:09:25.000000 cosmicfrog-0.3.5/cosmicfrog.egg-info/dependency_links.txt
+-rw-r--r--   0 gordon    (1000) gordon    (1000)      114 2023-08-03 13:09:25.000000 cosmicfrog-0.3.5/cosmicfrog.egg-info/requires.txt
+-rw-r--r--   0 gordon    (1000) gordon    (1000)       11 2023-08-03 13:09:25.000000 cosmicfrog-0.3.5/cosmicfrog.egg-info/top_level.txt
+-rw-r--r--   0 gordon    (1000) gordon    (1000)       38 2023-08-03 13:09:25.668184 cosmicfrog-0.3.5/setup.cfg
+-rw-r--r--   0 gordon    (1000) gordon    (1000)      899 2023-08-03 13:01:51.000000 cosmicfrog-0.3.5/setup.py
```

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_AdvancedQueueingDetails.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_AdvancedQueueingDetails.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Analytics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Analytics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_BillsOfMaterials.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_BillsOfMaterials.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_BusinessCalendars.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_BusinessCalendars.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_BusinessHours.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_BusinessHours.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ChangeoverTimes.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ChangeoverTimes.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomSimulationScripts.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomSimulationScripts.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomerDemand.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomerDemand.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPolicies.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomerOrderProfiles.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomerOrderProfiles.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomerOrders.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomerOrders.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomerRiskConfigurations.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomerRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomerTransitConstraints.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomerTransitConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Customers.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Customers.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_CustomersMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_CustomersMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Facilities.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Facilities.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_FacilitiesMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_FacilitiesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_FacilityCountConstraints.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_FacilityCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_FacilityDemand.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_FacilityDemand.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_FacilityRiskConfigurations.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_FacilityRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_FlowConstraints.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_FlowConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_FlowCountConstraints.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_FlowCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_GeographicRiskConfigurations.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_GeographicRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_GreenfieldServiceBands.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_GreenfieldServiceBands.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_GreenfieldSettings.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_GreenfieldSettings.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Groups.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Groups.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Histograms.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Histograms.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_InputFactors.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_InputFactors.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_InventoryConstraints.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_InventoryConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_InventoryCountConstraints.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_InventoryCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_InventoryPolicies.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_InventoryPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_InventoryPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_InventoryPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Lookups.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Lookups.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Maps.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Maps.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ModelInfo.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ModelInfo.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ModelRunOptions.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ModelRunOptions.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ModelSettings.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ModelSettings.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_NetworkRiskConfigurations.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_NetworkRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_OrderFulfillmentPolicies.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_OrderFulfillmentPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_OrderProfileProductAffinity.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_OrderProfileProductAffinity.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_OrderProfileProductSelection.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_OrderProfileProductSelection.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_OrderedProductSubstitution.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_OrderedProductSubstitution.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Organizations.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Organizations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_OutputFactors.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_OutputFactors.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Periods.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Periods.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Processes.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Processes.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProcessesMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProcessesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProcurementOrderProfiles.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProcurementOrderProfiles.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProcurementOrders.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProcurementOrders.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProcurementPolicies.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProcurementPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProcurementPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProcurementPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductUnitsOfMeasure.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductUnitsOfMeasure.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductionConstraints.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductionConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductionCountConstraints.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductionCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductionOrderProfiles.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductionOrderProfiles.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductionOrders.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductionOrders.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductionPolicies.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductionPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductionPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductionPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Products.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Products.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ProductsMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ProductsMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrderProfiles.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrderProfiles.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrders.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrders.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ReplenishmentPolicies.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ReplenishmentPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ReplenishmentPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ReplenishmentPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_RiskBandDefinitions.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_RiskBandDefinitions.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_RiskRatingConfigurations.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_RiskRatingConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_RiskSummaryConfigurations.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_RiskSummaryConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ScenarioItemAssignments.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ScenarioItemAssignments.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_ScenarioItems.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_ScenarioItems.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Scenarios.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Scenarios.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_SequentialObjectives.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_SequentialObjectives.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Shipments.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Shipments.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_StepCosts.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_StepCosts.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_SupplierCapabilities.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_SupplierCapabilities.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_SupplierCapabilitiesMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_SupplierCapabilitiesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_SupplierRiskConfigurations.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_SupplierRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_Suppliers.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_Suppliers.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_SuppliersMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_SuppliersMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TableFilters.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TableFilters.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationAssets.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationAssets.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationAssetsMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationAssetsMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationLaneModeQueueDetails.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationLaneModeQueueDetails.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationLaneQueueDetails.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationLaneQueueDetails.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationModes.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationModes.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationModesMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationModesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationPolicies.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_TransportationRates.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_TransportationRates.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_UnitsOfMeasure.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_UnitsOfMeasure.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_UserDefinedConstraints.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_UserDefinedConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_UserDefinedCosts.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_UserDefinedCosts.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_UserDefinedForecasts.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_UserDefinedForecasts.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_UserDefinedForecastsData.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_UserDefinedForecastsData.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_UserDefinedVariables.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_UserDefinedVariables.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_UtilizationRiskConfigurations.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_UtilizationRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WarehousingPolicies.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WarehousingPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WarehousingPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WarehousingPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WorkCenterCountConstraints.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WorkCenterCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WorkCenterQueueDetails.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WorkCenterQueueDetails.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WorkCenters.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WorkCenters.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WorkCentersMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WorkCentersMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WorkResources.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WorkResources.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/anura_WorkResourcesMultiTimePeriod.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/anura_WorkResourcesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationBillsOfMaterialSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationBillsOfMaterialSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationConstraintSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationConstraintSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeParentInformationReport.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeParentInformationReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationCustomerRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationCustomerRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationCustomerSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationCustomerSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationDemandSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationDemandSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationFacilityCostToServeSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationFacilityCostToServeSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationFacilityRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationFacilityRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationFacilitySummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationFacilitySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationFlowSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationFlowSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGeographicRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGeographicRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilityRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilityRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilitySummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilitySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFlowSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFlowSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldGeographicRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldGeographicRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldRiskMetricsSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldRiskMetricsSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldServiceBandSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldServiceBandSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationInventorySummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationInventorySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationNetworkRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationNetworkRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationNetworkSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationNetworkSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationProcessSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationProcessSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationProductRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationProductRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationProductionSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationProductionSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationRiskMetricsSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationRiskMetricsSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationSequentialObjectiveSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationSequentialObjectiveSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationShipmentSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationShipmentSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationSupplierRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationSupplierRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationSupplierSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationSupplierSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationSupplySummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationSupplySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedCostSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedCostSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedVariableSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedVariableSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationUtilizationRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationUtilizationRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationValidationErrorReport.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationValidationErrorReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationWarehousingSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationWarehousingSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_OptimizationWorkCenterSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_OptimizationWorkCenterSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmInputFactorReport.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmInputFactorReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmOutputFactorReport.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmOutputFactorReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFlowSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFlowSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationFlowSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationFlowSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationInventoryOnHandReport.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationInventoryOnHandReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueDepthReport.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueDepthReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueDepthReport.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueDepthReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationLaneSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationLaneSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueDepthReport.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueDepthReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationOrderReport.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationOrderReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationProcessReport.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationProcessReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationProcessSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationProcessSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationProcessSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationProcessSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationProductionReport.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationProductionReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationShipmentReport.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationShipmentReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetrics.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationValidationErrorReport.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationValidationErrorReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueDepthReport.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueDepthReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummary.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummaryReplicationDetail.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_masterlists/anuraMasterTableList.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_masterlists/anuraMasterTableList.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/anura/table_masterlists/anuraOutputTableList.json` & `cosmicfrog-0.3.5/cosmicfrog/anura/table_masterlists/anuraOutputTableList.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog/frog_data.py` & `cosmicfrog-0.3.5/cosmicfrog/frog_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
 
         if table_name not in FrogModel.anura_tables:
             #Skip it
             self.log.warning(f"""Worksheet name not recognised as Anura table (skipping): {table_name}""")
             return
 
         self.log.info(f"""Importing worksheet to table: {table_name}""")
-        self.log.info(f"""Inserting {len(data)} rows""")
+        self.log.info(f"""Source data has {len(data)} rows""")
 
         # Behavior rules:
         # Key columns - get used to match (Note: possible future requirement, some custom columns may also be key columns)
         # Other Anura columns - get updated
         # Other Custom columns - get updated
         # Other columns (neither Anura or Custom) - get ignored
 
@@ -377,16 +377,14 @@
             # so doing insert and update separately
 
             all_columns_list = ", ".join([f'"{col_name}"' for col_name in all_column_names])
 
             if combined_key_columns:
 
                 update_column_list = ", ".join([f'"{col_name}" = "{temp_table_name}"."{col_name}"' for col_name in update_columns])
-
-
                 key_condition = " AND ".join([f'COALESCE("{table_name}"."{key_col}", \'{placeholder_value}\') = COALESCE("{temp_table_name}"."{key_col}", \'{placeholder_value}\')' for key_col in combined_key_columns])
 
                 update_query = f"""
                     UPDATE {table_name}
                     SET {update_column_list}
                     FROM {temp_table_name}
                     WHERE {key_condition};
@@ -394,21 +392,26 @@
 
                 start_time = time.time()
                 cursor.execute(update_query)
                 updated_rows = cursor.rowcount
                 end_time = time.time()
                 self.log.info(f"Update query took {end_time - start_time} seconds")
 
+
+                temp_columns_list = ", ".join([f'"{temp_table_name}"."{col_name}"' for col_name in all_column_names])
+                null_conditions = [f"{table_name}.{col} IS NULL" for col in combined_key_columns]
+                null_conditions_clause = " AND ".join(null_conditions)
+
                 insert_query = f"""
                     INSERT INTO {table_name} ({all_columns_list})
-                    SELECT {all_columns_list} FROM {temp_table_name}
-                    WHERE NOT EXISTS (
-                        SELECT 1 FROM {table_name}
-                        WHERE {key_condition}
-                    );
+                    SELECT {temp_columns_list}
+                    FROM {temp_table_name}
+                    LEFT JOIN {table_name}
+                    ON {key_condition}
+                    WHERE {null_conditions_clause}
                 """
 
                 start_time = time.time()
                 cursor.execute(insert_query)
                 inserted_rows = cursor.rowcount 
                 end_time = time.time()
                 self.log.info(f"Insert query took {end_time - start_time} seconds")
```

### Comparing `cosmicfrog-0.3.4/cosmicfrog/frog_log.py` & `cosmicfrog-0.3.5/cosmicfrog/frog_log.py`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/cosmicfrog.egg-info/SOURCES.txt` & `cosmicfrog-0.3.5/cosmicfrog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.4/setup.py` & `cosmicfrog-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cosmicfrog",
     
     include_package_data=True,
 
-    version="0.3.4",
+    version="0.3.5",
     description='Helpful utilities for working with Cosmic Frog models',
     url='https://cosmicfrog.com',
     author='Optilogic',
     packages=['cosmicfrog'],
     package_data={
         'cosmicfrog': ['anura/table_definitions/*.json',
                         'anura/table_masterlists/*.json'
```

