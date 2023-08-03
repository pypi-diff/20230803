# Comparing `tmp/chartart-0.0.3.dev22.tar.gz` & `tmp/chartart-0.0.3.dev23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartart-0.0.3.dev22.tar", last modified: Wed Aug  2 08:13:58 2023, max compression
+gzip compressed data, was "chartart-0.0.3.dev23.tar", last modified: Thu Aug  3 09:22:19 2023, max compression
```

## Comparing `chartart-0.0.3.dev22.tar` & `chartart-0.0.3.dev23.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-02 08:13:58.988657 chartart-0.0.3.dev22/
--rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/LICENSE
--rw-r--r--   0 dhananjay   (504) staff       (20)     2846 2023-08-02 08:13:58.989050 chartart-0.0.3.dev22/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)     2324 2023-08-02 08:12:46.000000 chartart-0.0.3.dev22/README.md
--rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/pyproject.toml
--rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-08-02 08:13:58.991735 chartart-0.0.3.dev22/setup.cfg
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-02 08:13:58.936402 chartart-0.0.3.dev22/src/
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-02 08:13:58.959720 chartart-0.0.3.dev22/src/chartart/
--rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/src/chartart/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/src/chartart/conftest.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/src/chartart/helpers.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    87470 2023-08-02 06:55:51.000000 chartart-0.0.3.dev22/src/chartart/plot.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/src/chartart/simple_eda_template.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/src/chartart/test_plot.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-02 08:13:58.983384 chartart-0.0.3.dev22/src/chartart/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/src/chartart/tests/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/src/chartart/tests/test_simple.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-02 08:13:58.980856 chartart-0.0.3.dev22/src/chartart.egg-info/
--rw-r--r--   0 dhananjay   (504) staff       (20)     2846 2023-08-02 08:13:58.000000 chartart-0.0.3.dev22/src/chartart.egg-info/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-08-02 08:13:58.000000 chartart-0.0.3.dev22/src/chartart.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-08-02 08:13:58.000000 chartart-0.0.3.dev22/src/chartart.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-08-02 08:13:58.000000 chartart-0.0.3.dev22/src/chartart.egg-info/requires.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-08-02 08:13:58.000000 chartart-0.0.3.dev22/src/chartart.egg-info/top_level.txt
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-02 08:13:58.987207 chartart-0.0.3.dev22/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-03 09:22:19.537534 chartart-0.0.3.dev23/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev23/LICENSE
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2903 2023-08-03 09:22:19.537809 chartart-0.0.3.dev23/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2382 2023-08-03 09:22:00.000000 chartart-0.0.3.dev23/README.md
+-rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev23/pyproject.toml
+-rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-08-03 09:22:19.538848 chartart-0.0.3.dev23/setup.cfg
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-03 09:22:19.510992 chartart-0.0.3.dev23/src/
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-03 09:22:19.524593 chartart-0.0.3.dev23/src/chartart/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev23/src/chartart/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev23/src/chartart/conftest.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev23/src/chartart/helpers.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    87981 2023-08-03 08:55:44.000000 chartart-0.0.3.dev23/src/chartart/plot.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev23/src/chartart/simple_eda_template.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev23/src/chartart/test_plot.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-03 09:22:19.535216 chartart-0.0.3.dev23/src/chartart/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev23/src/chartart/tests/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev23/src/chartart/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-03 09:22:19.532722 chartart-0.0.3.dev23/src/chartart.egg-info/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2903 2023-08-03 09:22:19.000000 chartart-0.0.3.dev23/src/chartart.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-08-03 09:22:19.000000 chartart-0.0.3.dev23/src/chartart.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-08-03 09:22:19.000000 chartart-0.0.3.dev23/src/chartart.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-08-03 09:22:19.000000 chartart-0.0.3.dev23/src/chartart.egg-info/requires.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-08-03 09:22:19.000000 chartart-0.0.3.dev23/src/chartart.egg-info/top_level.txt
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-03 09:22:19.536574 chartart-0.0.3.dev23/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev23/tests/test_simple.py
```

### Comparing `chartart-0.0.3.dev22/LICENSE` & `chartart-0.0.3.dev23/LICENSE`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev22/PKG-INFO` & `chartart-0.0.3.dev23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev22
+Version: 0.0.3.dev23
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
@@ -86,7 +86,11 @@
 - preview and previewPost url should route should start with /  e.g  earlier http://localhost:port/#preview  now http://localhost:port/#/preview
 
 - 0.0.3.dev21
 Fix for communicate with Jupyter kernel
 
 - 0.0.3.dev22
 Fix for setting axis type on figure object
+
+- 0.0.3.dev23
+Added tooltip related parameters for map
+
```

### Comparing `chartart-0.0.3.dev22/README.md` & `chartart-0.0.3.dev23/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -69,8 +69,12 @@
 0.0.3.dev20
 - preview and previewPost url should route should start with /  e.g  earlier http://localhost:port/#preview  now http://localhost:port/#/preview
 
 - 0.0.3.dev21
 Fix for communicate with Jupyter kernel
 
 - 0.0.3.dev22
-Fix for setting axis type on figure object
+Fix for setting axis type on figure object
+
+- 0.0.3.dev23
+Added tooltip related parameters for map
+
```

### Comparing `chartart-0.0.3.dev22/setup.cfg` & `chartart-0.0.3.dev23/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chartart
-version = 0.0.3.dev22
+version = 0.0.3.dev23
 author = BR-Advisers
 author_email = info@br-advisers.com
 description = ChartArt python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `chartart-0.0.3.dev22/src/chartart/__init__.py` & `chartart-0.0.3.dev23/src/chartart/__init__.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev22/src/chartart/conftest.py` & `chartart-0.0.3.dev23/src/chartart/conftest.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev22/src/chartart/helpers.py` & `chartart-0.0.3.dev23/src/chartart/helpers.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev22/src/chartart/plot.py` & `chartart-0.0.3.dev23/src/chartart/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1373,15 +1373,16 @@
         treemap_info["enableDrilldown"] =  True
         levels.append(values)
         treemap_info['data'] = data[levels].to_dict(orient='records')
         self.data.insert(treemap_info)
 
     def map(self, mapOf: str, shapeDataField:  Optional[str] = None, data: Optional[Union[str, list, np.ndarray, pd.Series]] = None, primaryValueMapper : Optional[str] = None, zoomLevel: Optional[float] = None, focalLatitude: Optional[float] = None, 
             focalLongitude: Optional[float] = None, shapeColorValueMapper: Optional[str] = None, shapeColorMapper: Optional[list] = None, 
-            bubbleSizeMapper: Optional[str] = None, bubbleColorValueMapper: Optional[str] = None, bubbleColorMappers: Optional[list] = None, legend: Optional[dict] = None, marker: Optional[list] = None, layers: Optional[list] = None):
+            bubbleSizeMapper: Optional[str] = None, bubbleColorValueMapper: Optional[str] = None, bubbleColorMappers: Optional[list] = None, legend: Optional[dict] = None, marker: Optional[list] = None, layers: Optional[list] = None,
+            toolTipMapper: Optional[str] = None, toolTipType: Optional[str] = None, toolTipDisplay: Optional[str] = None):
         """Generate Map.
 
         :param mapOf: world or india 
         :shapeDataField: this is key from geojson. The shapeDataField property is used to refer the unique field name in the .json source to identify each shapes. 
          This shapeDataField will be used to map with respective value returned in primaryValueMapper from the data source.
         :param data: list of input data values , see example below
         :param primaryValueMapper: key to bind given data to jeo json data.
@@ -1392,14 +1393,17 @@
         :param shapeColorMapper: A value or range of values and its corresponding color mapping for shapes. 
         :param bubbleSizeMapper: A field from data which decides size of bubble.
         :param bubbleColorValueMapper: A field from data which decides color of shape.
         :param bubbleColorMappers: A value or range of values and its corresponding color mapping for bubbles.
         :param legend: legends for a map.
         :param marker: place icon markers and tooltip on it.
         :param layers: add sublayers on top of main chart. (line / arc / polyline/ circle / polygon / shape(geojson))
+        :toolTipMapper column for tool tip,
+        :toolTipType html / Text
+        :toolTipDisplay  hover / popup
         :return:
         """
         current_fig_type: str = 'map'
         if self.check_multi_axes_consistency(current_fig_type):
             self.fig_type = current_fig_type
         self.set_datagrid_figure_details()
         map_info: dict = {
@@ -1427,14 +1431,20 @@
             map_info['bubbleColorValueMapper'] = bubbleColorValueMapper
         if bubbleColorMappers is not None:
             map_info['bubbleColorMappers'] = bubbleColorMappers
         if legend is not None:
             map_info['legend'] = legend
         if marker is not None:
             map_info['marker'] = marker
+        if toolTipMapper is not None:
+            map_info['toolTipMapper'] = toolTipMapper
+        if toolTipType is not None:
+            map_info['toolTipType'] = toolTipType
+        if toolTipDisplay is not None:
+            map_info['toolTipDisplay'] = toolTipDisplay
         if layers is not None:
             # Convert 'coordinates':[[10,20], [50,60]] into  'coordinates': [{'latitude': 10, 'longitude': 20}, {'latitude': 50, 'longitude': 60}]
             # This is because firebase dont allow nested array. For user interface we allowed nested array because geojson has same format.  
             for layer in layers:
                 if ('coordinates' in layer):
                     for index, coordinate in enumerate(layer['coordinates']):
                         if isinstance(coordinate, list):
```

### Comparing `chartart-0.0.3.dev22/src/chartart/simple_eda_template.py` & `chartart-0.0.3.dev23/src/chartart/simple_eda_template.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev22/src/chartart/test_plot.py` & `chartart-0.0.3.dev23/src/chartart/test_plot.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev22/src/chartart.egg-info/PKG-INFO` & `chartart-0.0.3.dev23/src/chartart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev22
+Version: 0.0.3.dev23
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
@@ -86,7 +86,11 @@
 - preview and previewPost url should route should start with /  e.g  earlier http://localhost:port/#preview  now http://localhost:port/#/preview
 
 - 0.0.3.dev21
 Fix for communicate with Jupyter kernel
 
 - 0.0.3.dev22
 Fix for setting axis type on figure object
+
+- 0.0.3.dev23
+Added tooltip related parameters for map
+
```

