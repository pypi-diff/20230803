# Comparing `tmp/py_astrolab-0.6.5.tar.gz` & `tmp/py_astrolab-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.6.5.tar", max compression
+gzip compressed data, was "py_astrolab-0.6.6.tar", max compression
```

## Comparing `py_astrolab-0.6.5.tar` & `py_astrolab-0.6.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.6.5/README.md
--rwxr-xr-x   0        0        0     4901 2023-08-01 09:27:23.596932 py_astrolab-0.6.5/py_astrolab/__init__.py
--rwxr-xr-x   0        0        0    15760 2023-07-30 15:40:50.145067 py_astrolab-0.6.5/py_astrolab/aspects.py
--rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.6.5/py_astrolab/charts/__init__.py
--rwxr-xr-x   0        0        0    80380 2023-07-29 10:08:55.050610 py_astrolab-0.6.5/py_astrolab/charts/charts_svg.py
--rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.6.5/py_astrolab/charts/templates/basic.xml
--rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.6.5/py_astrolab/charts/templates/extended.xml
--rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.6.5/py_astrolab/charts/templates/minimal.xml
--rwxr-xr-x   0        0        0    71492 2023-07-28 15:58:20.983796 py_astrolab-0.6.5/py_astrolab/charts/wonderful_mistake.py
--rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.6.5/py_astrolab/fetch_geonames.py
--rwxr-xr-x   0        0        0    12935 2023-07-27 22:22:27.571322 py_astrolab-0.6.5/py_astrolab/kr.config.json
--rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.6.5/py_astrolab/main.py
--rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.6.5/py_astrolab/print_all_data.py
--rwxr-xr-x   0        0        0     7533 2023-07-28 15:50:57.383513 py_astrolab-0.6.5/py_astrolab/relationship_score.py
--rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.6.5/py_astrolab/report.py
--rwxr-xr-x   0        0        0    18590 2023-08-02 17:25:56.651200 py_astrolab-0.6.5/py_astrolab/transits.py
--rwxr-xr-x   0        0        0     5061 2023-07-30 17:36:22.186828 py_astrolab-0.6.5/py_astrolab/types.py
--rwxr-xr-x   0        0        0    10147 2023-07-28 15:51:20.189316 py_astrolab-0.6.5/py_astrolab/utilities.py
--rwxr-xr-x   0        0        0      664 2023-08-02 17:27:48.299087 py_astrolab-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.6.5/PKG-INFO
+-rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.6.6/README.md
+-rwxr-xr-x   0        0        0     4901 2023-08-01 09:27:23.596932 py_astrolab-0.6.6/py_astrolab/__init__.py
+-rwxr-xr-x   0        0        0    15760 2023-07-30 15:40:50.145067 py_astrolab-0.6.6/py_astrolab/aspects.py
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.6.6/py_astrolab/charts/__init__.py
+-rwxr-xr-x   0        0        0    80380 2023-07-29 10:08:55.050610 py_astrolab-0.6.6/py_astrolab/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.6.6/py_astrolab/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.6.6/py_astrolab/charts/templates/extended.xml
+-rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.6.6/py_astrolab/charts/templates/minimal.xml
+-rwxr-xr-x   0        0        0    71492 2023-07-28 15:58:20.983796 py_astrolab-0.6.6/py_astrolab/charts/wonderful_mistake.py
+-rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.6.6/py_astrolab/fetch_geonames.py
+-rwxr-xr-x   0        0        0    12935 2023-07-27 22:22:27.571322 py_astrolab-0.6.6/py_astrolab/kr.config.json
+-rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.6.6/py_astrolab/main.py
+-rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.6.6/py_astrolab/print_all_data.py
+-rwxr-xr-x   0        0        0     7533 2023-07-28 15:50:57.383513 py_astrolab-0.6.6/py_astrolab/relationship_score.py
+-rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.6.6/py_astrolab/report.py
+-rwxr-xr-x   0        0        0    18590 2023-08-02 18:39:26.606720 py_astrolab-0.6.6/py_astrolab/transits.py
+-rwxr-xr-x   0        0        0     5061 2023-07-30 17:36:22.186828 py_astrolab-0.6.6/py_astrolab/types.py
+-rwxr-xr-x   0        0        0    10147 2023-07-28 15:51:20.189316 py_astrolab-0.6.6/py_astrolab/utilities.py
+-rwxr-xr-x   0        0        0      664 2023-08-02 18:39:40.730601 py_astrolab-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.6.6/PKG-INFO
```

### Comparing `py_astrolab-0.6.5/py_astrolab/__init__.py` & `py_astrolab-0.6.6/py_astrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/py_astrolab/aspects.py` & `py_astrolab-0.6.6/py_astrolab/aspects.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.6.6/py_astrolab/charts/charts_svg.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.6.6/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.6.6/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/py_astrolab/charts/templates/minimal.xml` & `py_astrolab-0.6.6/py_astrolab/charts/templates/minimal.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/py_astrolab/charts/wonderful_mistake.py` & `py_astrolab-0.6.6/py_astrolab/charts/wonderful_mistake.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/py_astrolab/fetch_geonames.py` & `py_astrolab-0.6.6/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/py_astrolab/kr.config.json` & `py_astrolab-0.6.6/py_astrolab/kr.config.json`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/py_astrolab/main.py` & `py_astrolab-0.6.6/py_astrolab/main.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/py_astrolab/print_all_data.py` & `py_astrolab-0.6.6/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/py_astrolab/relationship_score.py` & `py_astrolab-0.6.6/py_astrolab/relationship_score.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/py_astrolab/report.py` & `py_astrolab-0.6.6/py_astrolab/report.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/py_astrolab/transits.py` & `py_astrolab-0.6.6/py_astrolab/transits.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -125,17 +125,17 @@
         while jd2 - jd1 > 6.94e-4:  # 1 minuto in giorni.
             jd = jd1 + (jd2 - jd1) / 2
             orb = self.calc_orb(jd, planet1, planet2, aspect, natal_planet_orb)  # Calcola l'orbita
             if abs(orb - target_orb) < 0.1:  # Se l'orbita è vicina a target_orb
                 jd = round(jd * 1440) / 1440  # Arrotonda al minuto più vicino
                 return self.jd_to_datetime(jd), orb
             if orb > target_orb:
-                jd1 = jd
-            else:
                 jd2 = jd
+            else:
+                jd1 = jd
         jd1 = round(jd1 * 1440) / 1440  # Arrotonda al minuto più vicino
         orb = self.calc_orb(jd1, planet1, planet2, aspect, natal_planet_orb)  # Calcola l'orbita
         return self.jd_to_datetime(jd1), orb
 
     def backward_binary_search(self, planet1, planet2, aspect, orbit_tolerance, natal_planet_orb, interval):
         # Prima, determina se l'aspetto è presente all'inizio.
         # interval = min(self.planet_names[planet1]['interval'], self.planet_names[planet2]['interval'])
```

### Comparing `py_astrolab-0.6.5/py_astrolab/types.py` & `py_astrolab-0.6.6/py_astrolab/types.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/py_astrolab/utilities.py` & `py_astrolab-0.6.6/py_astrolab/utilities.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.5/pyproject.toml` & `py_astrolab-0.6.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.6.5"
+version = "0.6.6"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.6.5/PKG-INFO` & `py_astrolab-0.6.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.6.5
+Version: 0.6.6
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

