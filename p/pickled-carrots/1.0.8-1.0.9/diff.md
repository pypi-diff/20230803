# Comparing `tmp/pickled_carrots-1.0.8.tar.gz` & `tmp/pickled_carrots-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickled_carrots-1.0.8.tar", max compression
+gzip compressed data, was "pickled_carrots-1.0.9.tar", max compression
```

## Comparing `pickled_carrots-1.0.8.tar` & `pickled_carrots-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-08-01 18:37:10.807525 pickled_carrots-1.0.8/README.md
--rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-1.0.8/pickled_carrots/DPData.py
--rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-1.0.8/pickled_carrots/DPPlot.py
--rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-1.0.8/pickled_carrots/DPUtil.py
--rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-1.0.8/pickled_carrots/__init__.py
--rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-1.0.8/pickled_carrots/database.py
--rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-1.0.8/pickled_carrots/dataclass.py
--rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-1.0.8/pickled_carrots/mathutil.py
--rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-1.0.8/pickled_carrots/plot.py
--rwxr-xr-x   0        0        0     1034 2023-05-24 14:49:39.883632 pickled_carrots-1.0.8/pickled_carrots/resources/event_type_lookup.pickle
--rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-1.0.8/pickled_carrots/vinegar/__init__.py
--rw-r--r--   0        0        0    13845 2023-05-26 13:00:40.817419 pickled_carrots-1.0.8/pickled_carrots/vinegar/core.py
--rw-r--r--   0        0        0     9312 2023-05-29 12:55:11.279181 pickled_carrots-1.0.8/pickled_carrots/vinegar/event.py
--rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-1.0.8/pickled_carrots/vinegar/inventory.py
--rw-r--r--   0        0        0     1069 2023-05-25 14:36:27.387680 pickled_carrots-1.0.8/pickled_carrots/vinegar/tests/test_read_hsf.py
--rw-r--r--   0        0        0   141094 2023-08-01 18:37:10.807525 pickled_carrots-1.0.8/pickled_carrots/waveforms.py
--rw-r--r--   0        0        0      678 2023-08-01 18:37:20.295963 pickled_carrots-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 pickled_carrots-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-01 18:37:10.807525 pickled_carrots-1.0.9/README.md
+-rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-1.0.9/pickled_carrots/DPData.py
+-rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-1.0.9/pickled_carrots/DPPlot.py
+-rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-1.0.9/pickled_carrots/DPUtil.py
+-rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-1.0.9/pickled_carrots/__init__.py
+-rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-1.0.9/pickled_carrots/database.py
+-rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-1.0.9/pickled_carrots/dataclass.py
+-rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-1.0.9/pickled_carrots/mathutil.py
+-rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-1.0.9/pickled_carrots/plot.py
+-rwxr-xr-x   0        0        0     1034 2023-05-24 14:49:39.883632 pickled_carrots-1.0.9/pickled_carrots/resources/event_type_lookup.pickle
+-rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-1.0.9/pickled_carrots/vinegar/__init__.py
+-rw-r--r--   0        0        0    13850 2023-08-01 20:48:28.421008 pickled_carrots-1.0.9/pickled_carrots/vinegar/core.py
+-rw-r--r--   0        0        0     9312 2023-05-29 12:55:11.279181 pickled_carrots-1.0.9/pickled_carrots/vinegar/event.py
+-rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-1.0.9/pickled_carrots/vinegar/inventory.py
+-rw-r--r--   0        0        0     1069 2023-05-25 14:36:27.387680 pickled_carrots-1.0.9/pickled_carrots/vinegar/tests/test_read_hsf.py
+-rw-r--r--   0        0        0   141203 2023-08-01 20:48:28.421008 pickled_carrots-1.0.9/pickled_carrots/waveforms.py
+-rw-r--r--   0        0        0      678 2023-08-01 20:48:36.821399 pickled_carrots-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 pickled_carrots-1.0.9/PKG-INFO
```

### Comparing `pickled_carrots-1.0.8/pickled_carrots/DPData.py` & `pickled_carrots-1.0.9/pickled_carrots/DPData.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.8/pickled_carrots/DPPlot.py` & `pickled_carrots-1.0.9/pickled_carrots/DPPlot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.8/pickled_carrots/DPUtil.py` & `pickled_carrots-1.0.9/pickled_carrots/DPUtil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.8/pickled_carrots/database.py` & `pickled_carrots-1.0.9/pickled_carrots/database.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.8/pickled_carrots/dataclass.py` & `pickled_carrots-1.0.9/pickled_carrots/dataclass.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.8/pickled_carrots/mathutil.py` & `pickled_carrots-1.0.9/pickled_carrots/mathutil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.8/pickled_carrots/plot.py` & `pickled_carrots-1.0.9/pickled_carrots/plot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.8/pickled_carrots/resources/event_type_lookup.pickle` & `pickled_carrots-1.0.9/pickled_carrots/resources/event_type_lookup.pickle`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.8/pickled_carrots/vinegar/core.py` & `pickled_carrots-1.0.9/pickled_carrots/vinegar/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         return SeismicDataEnsemble(self.stream, self.catalog, self.inventory)
 
     @classmethod
     def read(cls, file_path, network, experimental=False):
         if isinstance(file_path, Path):
             file_path = str(file_path)
         with tempfile.NamedTemporaryFile(delete=True) as tmpfile:
-            st, head = waveforms.hsf_to_obspy(file_path, print_out=False,
+            st, head = waveforms.hsf_to_obspy(file=file_path, print_out=False,
                                               groundmotion=False, return_head=True,
                                               experimental=experimental)
 
         # convert voltage into 32 bits integer (ADC counts)
         volt_ranges = expand_list(head['volt_range'], head['ch_descr'])
         previous_stations = []
         i = 0
```

### Comparing `pickled_carrots-1.0.8/pickled_carrots/vinegar/event.py` & `pickled_carrots-1.0.9/pickled_carrots/vinegar/event.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.8/pickled_carrots/vinegar/inventory.py` & `pickled_carrots-1.0.9/pickled_carrots/vinegar/inventory.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.8/pickled_carrots/vinegar/tests/test_read_hsf.py` & `pickled_carrots-1.0.9/pickled_carrots/vinegar/tests/test_read_hsf.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.8/pickled_carrots/waveforms.py` & `pickled_carrots-1.0.9/pickled_carrots/waveforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,17 +90,16 @@
     st = read(file_path, format='MSEED')
 
     # returning obspy stream to the user
     return st
 
 
 def hsf_to_obspy(file=None, head=None, data=None, rotate=True, correct_g_to_mss=True,
-                 print_out=True,
-                 groundmotion=True, rotate_to_zrt=False, force_positive_down=False,
-                 experimental=False,
+                 return_head=True, print_out=True, groundmotion=True,
+                 rotate_to_zrt=False, force_positive_down=False, experimental=False,
                  force_python_decompress=False, rotate_to_lqt=False):
     """
     Function to convert the information read from the hsf file by read_hsf into an obspy trace object
     There is some additional information saved to the header of each trace:
     stats.t0 - The P arrival time in seconds - 0 if there is no P arrival
     stats.t1 - The S arrival time in seconds - 0 if there is no S arrival
     stats.t2 - The origin time in seconds
@@ -113,14 +112,15 @@
     :param head: the header information from read_hsf
     :param data: the (assumed acceleration) data read from the hsf file in the format
         [num traces, num points]
         Also using this to provide the AWS s3 data which we want to extract the hsf data from if relevant
     :param file: the name of the file to be used to read the hsf data from
     :param rotate: if True, rotates the data into a ZNE coordinate system
     :param correct_g_to_mss: if True, corrects accelerometer data from g to m/s/s
+    :param return_head: if true, return head.
     :param print_out: if True, prints to screen when traces don't have P or S values
     :param groundmotion: if True, returns output in SI units rather than volts
     :param rotate_to_zrt: if True, rotates the data to radial and transverse - transverse contains mostly SH energy, and
         radial contains mostly P and Sv energy. Vertical component remains. For reference, H component in WaveVis is
         the same as the T component here, and the V component is the Radial. R component in WaveVis is the polarity
         flipped down component, which is the same as the vertical component here. WaveVis uses down as positive
         sometimes - might need futher work to build this in here.
@@ -490,15 +490,18 @@
 
                 # flipping the amplitude of the Q component to agree with the output that we see in WaveVis
                 if head['use_elevation']:
                     sttemp = stream.select(station=stat_names[jk], channel='**Q')
                     for tr in sttemp:
                         tr.data = tr.data * -1
 
-    return stream
+    if return_head:
+        return stream, head
+    else:
+        return stream
 
 
 def create_obspy_inv(stream):
     """
     Function for creating an obspy inventory object from the stream without using a station xml
     Based on the obspy tutorials for creating xml files from scratch
     This inventory does not include the response data, just the data needed for rotation
```

### Comparing `pickled_carrots-1.0.8/pyproject.toml` & `pickled_carrots-1.0.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pickled_carrots"
-version = "1.0.8"
+version = "1.0.9"
 description = ""
 authors = ["pickled cattots team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 plotly = "^5.14.1"
```

### Comparing `pickled_carrots-1.0.8/PKG-INFO` & `pickled_carrots-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickled-carrots
-Version: 1.0.8
+Version: 1.0.9
 Summary: 
 Author: pickled cattots team
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

