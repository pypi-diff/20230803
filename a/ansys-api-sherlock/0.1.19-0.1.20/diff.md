# Comparing `tmp/ansys-api-sherlock-0.1.19.tar.gz` & `tmp/ansys-api-sherlock-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-sherlock-0.1.19.tar", last modified: Thu Jul 27 14:02:59 2023, max compression
+gzip compressed data, was "ansys-api-sherlock-0.1.20.tar", last modified: Thu Aug  3 14:31:35 2023, max compression
```

## Comparing `ansys-api-sherlock-0.1.19.tar` & `ansys-api-sherlock-0.1.20.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:02:59.866054 ansys-api-sherlock-0.1.19/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-27 14:02:59.866054 ansys-api-sherlock-0.1.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:02:59.866054 ansys-api-sherlock-0.1.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:02:59.866054 ansys-api-sherlock-0.1.19/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:02:59.862054 ansys-api-sherlock-0.1.19/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:02:59.862054 ansys-api-sherlock-0.1.19/src/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:02:59.866054 ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:02:59.866054 ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/
--rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockCommonService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockLayerService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    27755 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockModelService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockPartsService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockProjectService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-07-27 14:02:45.000000 ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockStackupService.proto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:02:59.866054 ansys-api-sherlock-0.1.19/src/ansys_api_sherlock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-27 14:02:59.000000 ansys-api-sherlock-0.1.19/src/ansys_api_sherlock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-27 14:02:59.000000 ansys-api-sherlock-0.1.19/src/ansys_api_sherlock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:02:59.000000 ansys-api-sherlock-0.1.19/src/ansys_api_sherlock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 14:02:59.000000 ansys-api-sherlock-0.1.19/src/ansys_api_sherlock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 14:02:59.000000 ansys-api-sherlock-0.1.19/src/ansys_api_sherlock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 14:02:59.000000 ansys-api-sherlock-0.1.19/src/ansys_api_sherlock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:31:35.248880 ansys-api-sherlock-0.1.20/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-03 14:31:35.248880 ansys-api-sherlock-0.1.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:31:35.248880 ansys-api-sherlock-0.1.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:31:35.248880 ansys-api-sherlock-0.1.20/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:31:35.244881 ansys-api-sherlock-0.1.20/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:31:35.248880 ansys-api-sherlock-0.1.20/src/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:31:35.248880 ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:31:35.248880 ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockCommonService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockLayerService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    27755 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockModelService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockPartsService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockProjectService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-08-03 14:31:19.000000 ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockStackupService.proto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:31:35.248880 ansys-api-sherlock-0.1.20/src/ansys_api_sherlock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-03 14:31:35.000000 ansys-api-sherlock-0.1.20/src/ansys_api_sherlock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-03 14:31:35.000000 ansys-api-sherlock-0.1.20/src/ansys_api_sherlock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:31:35.000000 ansys-api-sherlock-0.1.20/src/ansys_api_sherlock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-03 14:31:35.000000 ansys-api-sherlock-0.1.20/src/ansys_api_sherlock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 14:31:35.000000 ansys-api-sherlock-0.1.20/src/ansys_api_sherlock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 14:31:35.000000 ansys-api-sherlock-0.1.20/src/ansys_api_sherlock.egg-info/top_level.txt
```

### Comparing `ansys-api-sherlock-0.1.19/LICENSE` & `ansys-api-sherlock-0.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.19/PKG-INFO` & `ansys-api-sherlock-0.1.20/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-sherlock
-Version: 0.1.19
-Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 14:02:59 on 27 July 2023
+Version: 0.1.20
+Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 14:31:35 on 03 August 2023
 Home-page: https://github.com/ansys/ansys-api-sherlock
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-sherlock-0.1.19/README.md` & `ansys-api-sherlock-0.1.20/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.19/setup.py` & `ansys-api-sherlock-0.1.20/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto` & `ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto`

 * *Files 10% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     repeated EventStrainMap eventStrainMaps	= 2;
   }
 
   repeated StrainMapAnalysis strainMapAnalyses = 3;
 }
 
 /**
- * Enumeration defining the types of suppored element orders.
+ * Enumeration defining the types of supported element orders.
  */
 enum ElementOrder {
   UnknownOrder	= 0;	// Default enum to catch invalid element order.
   Linear		= 1;	// Enum for first order linear elements.
   Quadratic		= 2;	// Enum for second order quadratic elements.
   SolidShell	= 3;	// Enum for solid shell elements.
 }
@@ -295,14 +295,31 @@
 	optional bool partTempRiseMinEnabled = 5;				// Flag indicating if part temperature minimum rise should be enabled.
 	optional bool partValidationEnabled = 6;				// Flag indicating if part validation should be performed.
   }
   
   repeated SolderFatigue solderFatigueProperties = 2;
 }
 
+/**
+ * Request to update FEA Part Modeling Properties
+ */
+message UpdatePartModelingRequest {
+  string project	 						= 1;	// Sherlock project name.
+  string ccaName 							= 2;	// The CCA name.
+  bool partEnabled			 				= 3;	// Whether to enable part modeling. Ignores all other fields if part modeling is disabled.
+  optional double partMinSize 				= 4;	// The minimum part size
+  optional string partMinSizeUnits 			= 5;	// Units for minimum part size
+  optional string partElemOrder 			= 6;	// Element order
+  optional double partMaxEdgeLength 		= 7;	// Maximum mesh size
+  optional string partMaxEdgeLengthUnits 	= 8;	// Units for maximum mesh size
+  optional double partMaxVertical 			= 9;	// Vertical mesh size
+  optional string partMaxVerticalUnits 		= 10;	// Units for vertical mesh size
+  optional bool partResultsFiltered 		= 11;	// Whether to enable filtered part results
+}
+
 service SherlockAnalysisService {
   // Runs one or more Sherlock analysis.
   rpc runAnalysis(RunAnalysisRequest) returns (ReturnCode);
   
   // Run Sherlock strain map analysis.
   rpc runStrainMapAnalysis(RunStrainMapAnalysisRequest) returns (ReturnCode);
   
@@ -340,8 +357,11 @@
   rpc getPcbModelingInputFields(GetPcbModelingInputFieldsRequest) returns (GetPcbModelingInputFieldsResponse);
   
   // Updates the PCB modeling properties for the provided analysis types.
   rpc updatePcbModelingProps(UpdatePcbModelingPropsRequest) returns (ReturnCode);
   
   // Returns the list of valid Solder Fatigue property fields given the user configuration.
   rpc getSolderFatigueInputFields(GetSolderFatigueInputFieldsRequest) returns (GetSolderFatigueInputFieldsResponse);
+  
+  // Updates the part modeling properties for a given project's CCA.
+  rpc updatePartModelingProperties(UpdatePartModelingRequest) returns (ReturnCode);
 }
```

### Comparing `ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockCommonService.proto` & `ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockCommonService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockLayerService.proto` & `ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockLayerService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto` & `ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockModelService.proto` & `ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockModelService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockPartsService.proto` & `ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockPartsService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockProjectService.proto` & `ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockProjectService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.19/src/ansys/api/sherlock/v0/SherlockStackupService.proto` & `ansys-api-sherlock-0.1.20/src/ansys/api/sherlock/v0/SherlockStackupService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.19/src/ansys_api_sherlock.egg-info/PKG-INFO` & `ansys-api-sherlock-0.1.20/src/ansys_api_sherlock.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-sherlock
-Version: 0.1.19
-Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 14:02:59 on 27 July 2023
+Version: 0.1.20
+Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 14:31:35 on 03 August 2023
 Home-page: https://github.com/ansys/ansys-api-sherlock
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-sherlock-0.1.19/src/ansys_api_sherlock.egg-info/SOURCES.txt` & `ansys-api-sherlock-0.1.20/src/ansys_api_sherlock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

