# Comparing `tmp/nifc-wildfires-0.3.0.tar.gz` & `tmp/nifc-wildfires-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifc-wildfires-0.3.0.tar", last modified: Sun Apr  2 11:06:36 2023, max compression
+gzip compressed data, was "nifc-wildfires-0.4.0.tar", last modified: Wed Aug  2 23:07:07 2023, max compression
```

## Comparing `nifc-wildfires-0.3.0.tar` & `nifc-wildfires-0.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 11:06:36.679814 nifc-wildfires-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 11:06:36.675814 nifc-wildfires-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 11:06:36.679814 nifc-wildfires-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/.github/workflows/continuous-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/.github/workflows/scrape.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-02 11:06:36.679814 nifc-wildfires-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    34344 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 11:06:36.679814 nifc-wildfires-0.3.0/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1117773 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/data/perimeters.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 11:06:36.679814 nifc-wildfires-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 11:06:36.675814 nifc-wildfires-0.3.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 11:06:36.679814 nifc-wildfires-0.3.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 11:06:36.679814 nifc-wildfires-0.3.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/docs/_templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 11:06:36.679814 nifc-wildfires-0.3.0/nifc_wildfires/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/nifc_wildfires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/nifc_wildfires/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 11:06:36.679814 nifc-wildfires-0.3.0/nifc_wildfires.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-02 11:06:36.000000 nifc-wildfires-0.3.0/nifc_wildfires.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-02 11:06:36.000000 nifc-wildfires-0.3.0/nifc_wildfires.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 11:06:36.000000 nifc-wildfires-0.3.0/nifc_wildfires.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-02 11:06:36.000000 nifc-wildfires-0.3.0/nifc_wildfires.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-02 11:06:36.000000 nifc-wildfires-0.3.0/nifc_wildfires.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-02 11:06:36.000000 nifc-wildfires-0.3.0/nifc_wildfires.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-02 11:06:36.679814 nifc-wildfires-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-02 11:06:13.000000 nifc-wildfires-0.3.0/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:07:07.392592 nifc-wildfires-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:07:07.376591 nifc-wildfires-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:07:07.380591 nifc-wildfires-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/.github/workflows/scrape.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-02 23:07:07.392592 nifc-wildfires-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    51131 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:07:07.380591 nifc-wildfires-0.4.0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  7282454 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/data/perimeters.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:07:07.392592 nifc-wildfires-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:07:07.376591 nifc-wildfires-0.4.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:07:07.392592 nifc-wildfires-0.4.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:07:07.392592 nifc-wildfires-0.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/docs/_templates/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:07:07.392592 nifc-wildfires-0.4.0/nifc_wildfires/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/nifc_wildfires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/nifc_wildfires/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:07:07.392592 nifc-wildfires-0.4.0/nifc_wildfires.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-02 23:07:07.000000 nifc-wildfires-0.4.0/nifc_wildfires.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-02 23:07:07.000000 nifc-wildfires-0.4.0/nifc_wildfires.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:07:07.000000 nifc-wildfires-0.4.0/nifc_wildfires.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-02 23:07:07.000000 nifc-wildfires-0.4.0/nifc_wildfires.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 23:07:07.000000 nifc-wildfires-0.4.0/nifc_wildfires.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 23:07:07.000000 nifc-wildfires-0.4.0/nifc_wildfires.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-02 23:07:07.392592 nifc-wildfires-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 23:06:37.000000 nifc-wildfires-0.4.0/test.py
```

### Comparing `nifc-wildfires-0.3.0/.github/workflows/continuous-deployment.yml` & `nifc-wildfires-0.4.0/.github/workflows/continuous-deployment.yml`

 * *Files identical despite different names*

### Comparing `nifc-wildfires-0.3.0/.github/workflows/docs.yml` & `nifc-wildfires-0.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nifc-wildfires-0.3.0/.github/workflows/scrape.yml` & `nifc-wildfires-0.4.0/.github/workflows/scrape.yml`

 * *Files identical despite different names*

### Comparing `nifc-wildfires-0.3.0/.gitignore` & `nifc-wildfires-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nifc-wildfires-0.3.0/.pre-commit-config.yaml` & `nifc-wildfires-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nifc-wildfires-0.3.0/LICENSE` & `nifc-wildfires-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nifc-wildfires-0.3.0/PKG-INFO` & `nifc-wildfires-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifc-wildfires
-Version: 0.3.0
+Version: 0.4.0
 Summary: Download wildfires data from the National Interagency Fire Center
 Home-page: https://palewi.re/docs/nifc-wildfires/
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Maintainer, https://github.com/datadesk
 Project-URL: Source, https://github.com/datadesk/nifc-wildfires
```

### Comparing `nifc-wildfires-0.3.0/docs/Makefile` & `nifc-wildfires-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nifc-wildfires-0.3.0/docs/_static/css/custom.css` & `nifc-wildfires-0.4.0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `nifc-wildfires-0.3.0/docs/_templates/nav.html` & `nifc-wildfires-0.4.0/docs/_templates/nav.html`

 * *Files identical despite different names*

### Comparing `nifc-wildfires-0.3.0/docs/conf.py` & `nifc-wildfires-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nifc-wildfires-0.3.0/docs/index.md` & `nifc-wildfires-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `nifc-wildfires-0.3.0/docs/make.bat` & `nifc-wildfires-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nifc-wildfires-0.3.0/nifc_wildfires/__init__.py` & `nifc-wildfires-0.4.0/nifc_wildfires/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 
 def get_incidents():
     """Get year-to-date fire incident points from NIFC situation reports. Includes active and inctive incidents.
 
     Returns a GeoJSON object with point geometry.
     """
     r = requests.get(
-        "https://services3.arcgis.com/T4QMspbfLg3qTGWY/arcgis/rest/services/WFIGS_Incident_Locations_YearToDate/FeatureServer/0/query?outFields=*&where=1%3D1&f=geojson"
+        "https://services3.arcgis.com/T4QMspbfLg3qTGWY/arcgis/rest/services/WFIGS_Incident_Locations_Current/FeatureServer/0/query?outFields=*&where=1%3D1&f=geojson"
     )
     if r.status_code != 200:
         raise Exception(f"Request for data failed with {r.status_code} status code")
     return r.json()
```

### Comparing `nifc-wildfires-0.3.0/nifc_wildfires/cli.py` & `nifc-wildfires-0.4.0/nifc_wildfires/cli.py`

 * *Files identical despite different names*

### Comparing `nifc-wildfires-0.3.0/nifc_wildfires.egg-info/PKG-INFO` & `nifc-wildfires-0.4.0/nifc_wildfires.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifc-wildfires
-Version: 0.3.0
+Version: 0.4.0
 Summary: Download wildfires data from the National Interagency Fire Center
 Home-page: https://palewi.re/docs/nifc-wildfires/
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Maintainer, https://github.com/datadesk
 Project-URL: Source, https://github.com/datadesk/nifc-wildfires
```

### Comparing `nifc-wildfires-0.3.0/nifc_wildfires.egg-info/SOURCES.txt` & `nifc-wildfires-0.4.0/nifc_wildfires.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nifc-wildfires-0.3.0/setup.py` & `nifc-wildfires-0.4.0/setup.py`

 * *Files identical despite different names*

