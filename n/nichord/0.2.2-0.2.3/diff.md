# Comparing `tmp/nichord-0.2.2.tar.gz` & `tmp/nichord-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nichord-0.2.2.tar", last modified: Sun Jul 30 22:01:01 2023, max compression
+gzip compressed data, was "nichord-0.2.3.tar", last modified: Thu Aug  3 16:02:44 2023, max compression
```

## Comparing `nichord-0.2.2.tar` & `nichord-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 22:01:01.703082 nichord-0.2.2/
--rw-rw-rw-   0        0        0      850 2023-07-30 22:01:01.703082 nichord-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     9250 2023-07-30 21:49:33.000000 nichord-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 22:01:01.697081 nichord-0.2.2/nichord/
--rw-rw-rw-   0        0        0      756 2022-11-12 03:49:12.000000 nichord-0.2.2/nichord/__init__.py
--rw-rw-rw-   0        0        0    34573 2023-07-30 17:47:59.000000 nichord-0.2.2/nichord/chord.py
--rw-rw-rw-   0        0        0     4893 2022-11-13 19:54:36.000000 nichord-0.2.2/nichord/combine.py
--rw-rw-rw-   0        0        0      482 2022-05-22 13:31:30.000000 nichord-0.2.2/nichord/convert.py
--rw-rw-rw-   0        0        0     5683 2023-07-30 02:58:52.000000 nichord-0.2.2/nichord/coord_labeler.py
--rw-rw-rw-   0        0        0     5731 2022-11-12 03:52:39.000000 nichord-0.2.2/nichord/glassbrain.py
--rw-rw-rw-   0        0        0     2156 2023-07-24 20:52:49.000000 nichord-0.2.2/nichord/patch_RendererAgg.py
-drwxrwxrwx   0        0        0        0 2023-07-30 22:01:01.702082 nichord-0.2.2/nichord.egg-info/
--rw-rw-rw-   0        0        0      850 2023-07-30 22:01:01.000000 nichord-0.2.2/nichord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-07-30 22:01:01.000000 nichord-0.2.2/nichord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 22:01:01.000000 nichord-0.2.2/nichord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-30 22:01:01.000000 nichord-0.2.2/nichord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 22:01:01.000000 nichord-0.2.2/nichord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 22:01:01.704083 nichord-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1530 2023-07-30 22:00:49.000000 nichord-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:02:44.280580 nichord-0.2.3/
+-rw-rw-rw-   0        0        0      850 2023-08-03 16:02:44.279579 nichord-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9376 2023-07-30 22:02:27.000000 nichord-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 16:02:44.273579 nichord-0.2.3/nichord/
+-rw-rw-rw-   0        0        0      756 2022-11-12 03:49:12.000000 nichord-0.2.3/nichord/__init__.py
+-rw-rw-rw-   0        0        0    34573 2023-07-30 17:47:59.000000 nichord-0.2.3/nichord/chord.py
+-rw-rw-rw-   0        0        0     4893 2022-11-13 19:54:36.000000 nichord-0.2.3/nichord/combine.py
+-rw-rw-rw-   0        0        0      482 2022-05-22 13:31:30.000000 nichord-0.2.3/nichord/convert.py
+-rw-rw-rw-   0        0        0     5404 2023-08-03 16:00:59.000000 nichord-0.2.3/nichord/coord_labeler.py
+-rw-rw-rw-   0        0        0     5731 2022-11-12 03:52:39.000000 nichord-0.2.3/nichord/glassbrain.py
+-rw-rw-rw-   0        0        0     2156 2023-07-24 20:52:49.000000 nichord-0.2.3/nichord/patch_RendererAgg.py
+-rw-rw-rw-   0        0        0     4394 2023-08-03 16:00:59.000000 nichord-0.2.3/nichord/peak.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:02:44.279579 nichord-0.2.3/nichord.egg-info/
+-rw-rw-rw-   0        0        0      850 2023-08-03 16:02:43.000000 nichord-0.2.3/nichord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-08-03 16:02:43.000000 nichord-0.2.3/nichord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 16:02:43.000000 nichord-0.2.3/nichord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-08-03 16:02:43.000000 nichord-0.2.3/nichord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-03 16:02:43.000000 nichord-0.2.3/nichord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 16:02:44.280580 nichord-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1492 2023-08-03 15:58:14.000000 nichord-0.2.3/setup.py
```

### Comparing `nichord-0.2.2/PKG-INFO` & `nichord-0.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nichord
-Version: 0.2.2
+Version: 0.2.3
 Summary: Creates chord diagrams for connectivity/graph data
 Home-page: https://github.com/paulcbogdan/NiChord
 Author: paulcbogdan
 Author-email: paulcbogdan@gmail.com
 License: MIT
 Keywords: plotting,fmri,plotting,chord
 Classifier: Programming Language :: Python
```

### Comparing `nichord-0.2.2/README.md` & `nichord-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-![PyPI](https://img.shields.io/pypi/v/nichord)
+![PyPI](https://img.shields.io/pypi/v/nichord) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nichord?link=https%3A%2F%2Fpypi.org%2Fproject%2Fnichord%2F)
+
 
 # NiChord
 
 `NiChord` is a Python package for visualizing functional connectivity data. This package was inspired by [NeuroMArVL](https://immersive.erc.monash.edu/neuromarvl/?example=40496078-effa-4ac3-9d3e-cb7f946e7dd1_137.147.133.145), an online visualization tool. Although the code was designed for neuroscience research, it can be used with any configuration of edge and label data.
 
 <p align="center">
   <img src="example\outside_chord_example.png"  width="600" />
```

### Comparing `nichord-0.2.2/nichord/__init__.py` & `nichord-0.2.3/nichord/__init__.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.2/nichord/chord.py` & `nichord-0.2.3/nichord/chord.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.2/nichord/combine.py` & `nichord-0.2.3/nichord/combine.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.2/nichord/coord_labeler.py` & `nichord-0.2.3/nichord/coord_labeler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-import numpy as np
-
 from typing import Union, Tuple
 
+import numpy as np
+from scipy.spatial import distance
+
+from nichord.peak import _read_atlas_peak
 
 def get_idx_to_label(coords: list, atlas: str = 'yeo',
                      search_closest: bool = True,
                      max_dist: Union[float, int] = 5,
                      must_have=None) -> dict:
     """
     Gets a dictionary where each ROI (idx) in the list of coords is mapped to a
-        label. By default, the this is mapping to a Yeo network parcellations.
+        label. By default, this is mapping to a Yeo network parcellations.
         If the coordinate does not correspond to any parcellation, the string
         "Uncertain" will be used.
 
     :param coords: List of tuples (x, y, z)
     :param atlas: string. "yeo" is used by default, although you can also
         pass a string corresponding to an atlas from the atlasreader package.
         These include: 'aal', 'aicha', 'desikan_killiany', 'destrieux',
@@ -25,32 +27,30 @@
     :param max_dist: If search_closest == True, max_dist corresponds to the
         distance that will be searched before using "Uncertain."
     :param must_have: used to filter what labels are considered valid. see
         find_closest(...)
     :return:
     """
 
-    from atlasreader.atlasreader import read_atlas_peak # import statements here
-                                                        # to speed things up
     idx_to_label = {}
     if atlas.lower() == 'yeo':
         atlas = get_yeo_atlas()
 
     for idx, (x, y, z) in enumerate(coords):
         if search_closest:
-            region, dist = find_closest(atlas, (x, y, z), max_dist=max_dist,
+            region, dist = find_closest(atlas, [x, y, z], max_dist=max_dist,
                                         must_have=must_have)
         else:
-            region = read_atlas_peak(atlas, (x, y, z), prob_thresh=0.1)
+            region = _read_atlas_peak(atlas, [x, y, z])
         region = region.replace('uncertain', 'Uncertain')
         idx_to_label[idx] = region
     return idx_to_label
 
 
-def find_closest(atlas: Union[str, object], coord: tuple,
+def find_closest(atlas: Union[str, object], coord: Union[tuple, list],
                  must_have: Union[list, None] = None,
                  max_dist: Union[int, float] = 5) -> Tuple[str, float]:
     """
     This will find the parcellation closest to the passed coord. If no
         parcellation is found within max_dist of the coord, it will be
         labeled 'uncertain'.
 
@@ -62,19 +62,16 @@
         else it will not be used. For example, if you are interested in getting
         Brodmann areas with the 'talairach_ba' atlas, you would pass
         must_have=["Brodmann"]
     :param max_dist: max_dist corresponds to the distance that will be
         searched before using "Uncertain."
     :return: the label and the distance from the coord to the label
     """
-    from atlasreader.atlasreader import read_atlas_peak # import statements here
-                                                        # to speed things up
-    from scipy.spatial import distance
 
-    region = read_atlas_peak(atlas, coord, prob_thresh=0.01)
+    region = _read_atlas_peak(atlas, coord)
     if isinstance(region, float) and np.isnan(region):
         region = 'uncertain'
 
     bad_keys = ['uncertain', 'Background', 'Cerebral',
                 'Cerebellum']  # these are labels  are too vague and are skipped
     if not any(key in region for key in bad_keys) and (
             must_have is None or any(key in region for key in must_have)):
@@ -84,20 +81,21 @@
     spread_dist = sorted(spread_dist, key=lambda x: abs(x))
     min_dist = max_dist
 
     min_region = 'uncertain'
     for x_move in spread_dist:
         for y_move in spread_dist:
             for z_move in spread_dist:
-                coord_new = (
-                coord[0] + x_move, coord[1] + y_move, coord[2] + z_move)
+                coord_new = [coord[0] + x_move,
+                             coord[1] + y_move,
+                             coord[2] + z_move]
                 dist = distance.euclidean(coord, coord_new)
                 if dist > min_dist:
                     continue
-                region = read_atlas_peak(atlas, coord_new, prob_thresh=0.1)
+                region = _read_atlas_peak(atlas, coord_new)
                 if isinstance(region, float) and np.isnan(region):
                     region = 'uncertain'
                 if not any(key in region for key in bad_keys) and (
                         must_have is None or any(
                         key in region for key in must_have)):
                     min_region = region
                     min_dist = dist
```

### Comparing `nichord-0.2.2/nichord/glassbrain.py` & `nichord-0.2.3/nichord/glassbrain.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.2/nichord/patch_RendererAgg.py` & `nichord-0.2.3/nichord/patch_RendererAgg.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.2/nichord.egg-info/PKG-INFO` & `nichord-0.2.3/nichord.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nichord
-Version: 0.2.2
+Version: 0.2.3
 Summary: Creates chord diagrams for connectivity/graph data
 Home-page: https://github.com/paulcbogdan/NiChord
 Author: paulcbogdan
 Author-email: paulcbogdan@gmail.com
 License: MIT
 Keywords: plotting,fmri,plotting,chord
 Classifier: Programming Language :: Python
```

### Comparing `nichord-0.2.2/setup.py` & `nichord-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,26 @@
 'To find out more about the package and see an example, see its .'
 
 setup(
     name="nichord",
     description="Creates chord diagrams for connectivity/graph data",
     long_description=desc,
     long_description_content_type="text/markdown",
-    version="v0.2.2",
+    version="v0.2.3",
     packages=["nichord"],
     python_requires=">=3.7",
     url="https://github.com/paulcbogdan/NiChord",
     author="paulcbogdan",
     author_email="paulcbogdan@gmail.com",
     install_requires=["nilearn",
                       "pandas",
                       "matplotlib",
                       "numpy",
                       "scipy",
-                      "pillow",
-                      "atlasreader"],
+                      "pillow"],
     keywords=["plotting", "fmri", "plotting", "chord"],
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

