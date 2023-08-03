# Comparing `tmp/wbFontParts-0.2.0.tar.gz` & `tmp/wbFontParts-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbFontParts-0.2.0.tar", last modified: Sun Jul  9 06:12:20 2023, max compression
+gzip compressed data, was "wbFontParts-0.2.1.tar", last modified: Thu Aug  3 07:11:17 2023, max compression
```

## Comparing `wbFontParts-0.2.0.tar` & `wbFontParts-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:20.420700 wbFontParts-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:20.416700 wbFontParts-0.2.0/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:20.419700 wbFontParts-0.2.0/Lib/wbFontParts/
--rw-rw-rw-   0 root         (0) root         (0)      502 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/anchor.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/bPoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2061 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/color.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/component.py
--rw-rw-rw-   0 root         (0) root         (0)     4184 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/contour.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/features.py
--rw-rw-rw-   0 root         (0) root         (0)     9918 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/font.py
--rw-rw-rw-   0 root         (0) root         (0)     2089 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/glyph.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/guideline.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/image.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/info.py
--rw-rw-rw-   0 root         (0) root         (0)      656 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/kerning.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/layer.py
--rw-rw-rw-   0 root         (0) root         (0)      604 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/lib.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/point.py
--rw-rw-rw-   0 root         (0) root         (0)      537 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/Lib/wbFontParts/segment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:20.420700 wbFontParts-0.2.0/Lib/wbFontParts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1604 2023-07-09 06:12:20.000000 wbFontParts-0.2.0/Lib/wbFontParts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      689 2023-07-09 06:12:20.000000 wbFontParts-0.2.0/Lib/wbFontParts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 06:12:20.000000 wbFontParts-0.2.0/Lib/wbFontParts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-09 06:12:20.000000 wbFontParts-0.2.0/Lib/wbFontParts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-09 06:12:20.000000 wbFontParts-0.2.0/Lib/wbFontParts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1604 2023-07-09 06:12:20.420700 wbFontParts-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2249 2023-07-09 06:12:20.420700 wbFontParts-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-09 06:12:19.000000 wbFontParts-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:11:17.867367 wbFontParts-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:11:17.862367 wbFontParts-0.2.1/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:11:17.866367 wbFontParts-0.2.1/Lib/wbFontParts/
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/anchor.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/bPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/color.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/component.py
+-rw-rw-rw-   0 root         (0) root         (0)     4184 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/contour.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/features.py
+-rw-rw-rw-   0 root         (0) root         (0)     9918 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/font.py
+-rw-rw-rw-   0 root         (0) root         (0)     5810 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/glyph.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/guideline.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/image.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/info.py
+-rw-rw-rw-   0 root         (0) root         (0)      656 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/kerning.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/layer.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/point.py
+-rw-rw-rw-   0 root         (0) root         (0)      537 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/segment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:11:17.867367 wbFontParts-0.2.1/Lib/wbFontParts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-08-03 07:11:17.000000 wbFontParts-0.2.1/Lib/wbFontParts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      689 2023-08-03 07:11:17.000000 wbFontParts-0.2.1/Lib/wbFontParts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 07:11:17.000000 wbFontParts-0.2.1/Lib/wbFontParts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-08-03 07:11:17.000000 wbFontParts-0.2.1/Lib/wbFontParts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-08-03 07:11:17.000000 wbFontParts-0.2.1/Lib/wbFontParts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-08-03 07:11:17.867367 wbFontParts-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2249 2023-08-03 07:11:17.868367 wbFontParts-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/setup.py
```

### Comparing `wbFontParts-0.2.0/LICENSE` & `wbFontParts-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/anchor.py` & `wbFontParts-0.2.1/Lib/wbFontParts/anchor.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/bPoint.py` & `wbFontParts-0.2.1/Lib/wbFontParts/bPoint.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/color.py` & `wbFontParts-0.2.1/Lib/wbFontParts/color.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/component.py` & `wbFontParts-0.2.1/Lib/wbFontParts/component.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/contour.py` & `wbFontParts-0.2.1/Lib/wbFontParts/contour.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/features.py` & `wbFontParts-0.2.1/Lib/wbFontParts/features.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/font.py` & `wbFontParts-0.2.1/Lib/wbFontParts/font.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/glyph.py` & `wbFontParts-0.2.1/Lib/wbFontParts/layer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,59 @@
 """
-glyph
+layer
 ===============================================================================
 """
-
-from typing import Optional
+import logging
 
 import wbDefcon
 from fontParts import fontshell
-from fontParts.base import BaseGlyph
-from fontParts.base.deprecated import DeprecatedGlyph, RemovedGlyph
-from fontParts.base.normalizers import normalizeColor
-
-from .anchor import RAnchor
-from .color import Color
-from .component import RComponent
-from .contour import RContour
-from .guideline import RGuideline
-from .image import RImage
+from fontParts.base import BaseLayer, normalizers
+from fontParts.base.deprecated import DeprecatedLayer, RemovedLayer
+
+from .glyph import RGlyph
 from .lib import RLib
 
-BaseGlyph.__bases__ = tuple(
-    b for b in BaseGlyph.__bases__ if b not in (RemovedGlyph, DeprecatedGlyph)
+BaseLayer.__bases__ = tuple(
+    b for b in BaseLayer.__bases__ if b not in (DeprecatedLayer, RemovedLayer)
 )
 
+log = logging.getLogger(__name__)
 
-class RGlyph(fontshell.RGlyph):
-    wrapClass = wbDefcon.Glyph
-    contourClass = RContour
-    componentClass = RComponent
-    anchorClass = RAnchor
-    guidelineClass = RGuideline
-    imageClass = RImage
+
+class RLayer(fontshell.RLayer):
+    wrapClass = wbDefcon.Layer
     libClass = RLib
-    colorClass = Color
+    glyphClass = RGlyph
 
     def _init(self, wrap=None):
         if wrap is None:
             wrap = self.wrapClass()
-        self._wrapped: wbDefcon.Glyph = wrap
-
-    def _get_selected(self) -> bool:
-        return self._wrapped.selected
+        self._wrapped: wbDefcon.Layer = wrap
 
-    def _set_selected(self, value: bool):
-        self._wrapped.selected = value
-
-    def _transformBy(self, matrix, **kwargs) -> None:
-        self._wrapped.holdNotifications()
-        super()._transformBy(matrix, **kwargs)
-        self._wrapped.releaseHeldNotifications()
-        self._wrapped.postNotification(notification="Glyph.ContoursChanged")
-
-    def _moveBy(self, value, **kwargs) -> None:
-        self._wrapped.move(value)
+    def naked(self) -> wbDefcon.Layer:
+        return self._wrapped
 
-    def show(self, newPage=False, view=None) -> None:
-        self._wrapped.show(newPage, view)
+    def newGlyph(self, name, clear=True):
+        """
+        Make a new glyph with **name** in the layer. ::
+
+            >>> glyph = layer.newGlyph("A")
+
+        The newly created :class:`BaseGlyph` will be returned.
+
+        If the glyph exists in the layer and clear is set to ``False``,
+        the existing glyph will be returned, otherwise the default
+        behavior is to clear the exisiting glyph.
+        """
+        name = normalizers.normalizeGlyphName(name)
+        if name not in self or clear:
+            glyph = self._newGlyph(name)
+        else:
+            glyph = self._getItem(name)
+        self._setLayerInGlyph(glyph)
+        return glyph
 
-    def naked(self) -> wbDefcon.Glyph:
-        return self._wrapped
+    def _get_selectedGlyphs(self):
+        return tuple(self[g] for g in self._wrapped.selectedGlyphNames)
 
-    # Mark
-    def _get_base_markColor(self) -> Optional[Color]:
-        value = self._get_markColor()
-        if value is not None:
-            value = self.colorClass(normalizeColor(value))
-        return value
-
-    def _set_base_markColor(self, value):
-        if value is not None:
-            value = normalizeColor(self.colorClass(value))
-        self._set_markColor(value)
+    def _get_selectedGlyphNames(self):
+        return self._wrapped.selectedGlyphNames
```

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/groups.py` & `wbFontParts-0.2.1/Lib/wbFontParts/groups.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/guideline.py` & `wbFontParts-0.2.1/Lib/wbFontParts/guideline.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/image.py` & `wbFontParts-0.2.1/Lib/wbFontParts/image.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/info.py` & `wbFontParts-0.2.1/Lib/wbFontParts/info.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/kerning.py` & `wbFontParts-0.2.1/Lib/wbFontParts/kerning.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/lib.py` & `wbFontParts-0.2.1/Lib/wbFontParts/lib.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/point.py` & `wbFontParts-0.2.1/Lib/wbFontParts/point.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts/segment.py` & `wbFontParts-0.2.1/Lib/wbFontParts/segment.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts.egg-info/PKG-INFO` & `wbFontParts-0.2.1/Lib/wbFontParts.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbFontParts
-Version: 0.2.0
+Version: 0.2.1
 Summary: A wrapper around fontParts for UFO Workbench.
 Home-page: https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts
 Project-URL: Documentation, https://workbench2.gitlab.io/WorkBenchExtensions/wbFontParts/
 Project-URL: Tracker, https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts/-/issues
@@ -31,7 +31,26 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# wbFontParts
+
+## A wrapper around fontParts for Workbench applications.
+
+[fontparts](https://pypi.org/project/fontParts/) is an API for interacting 
+with the parts of fonts during the font development process.
+
+This provides the API layer for UFO-Workbench.
+
+## Installation
+
+```shell
+pip install wbFontParts
+```
+
+## Documentation
+
+For details read the [Documentation](https://workbench2.gitlab.io/WorkBenchExtensions/wbFontParts).
```

### Comparing `wbFontParts-0.2.0/Lib/wbFontParts.egg-info/SOURCES.txt` & `wbFontParts-0.2.1/Lib/wbFontParts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.0/PKG-INFO` & `wbFontParts-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbFontParts
-Version: 0.2.0
+Version: 0.2.1
 Summary: A wrapper around fontParts for UFO Workbench.
 Home-page: https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts
 Project-URL: Documentation, https://workbench2.gitlab.io/WorkBenchExtensions/wbFontParts/
 Project-URL: Tracker, https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts/-/issues
@@ -31,7 +31,26 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# wbFontParts
+
+## A wrapper around fontParts for Workbench applications.
+
+[fontparts](https://pypi.org/project/fontParts/) is an API for interacting 
+with the parts of fonts during the font development process.
+
+This provides the API layer for UFO-Workbench.
+
+## Installation
+
+```shell
+pip install wbFontParts
+```
+
+## Documentation
+
+For details read the [Documentation](https://workbench2.gitlab.io/WorkBenchExtensions/wbFontParts).
```

### Comparing `wbFontParts-0.2.0/setup.cfg` & `wbFontParts-0.2.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.2.1
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -12,15 +12,15 @@
 replace = __version__ = "{new_version}"
 
 [metadata]
 name = wbFontParts
 version = attr: wbFontParts.__version__
 author = Andreas Eigendorf
 description = A wrapper around fontParts for UFO Workbench.
-long_description = file: README.md
+long_description = file: readme.md
 long_description_content_type = text/markdown
 license = MIT
 license_files = LICENSE
 url = https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts
 project_urls = 
 	Source = https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts
 	Documentation = https://workbench2.gitlab.io/WorkBenchExtensions/wbFontParts/
@@ -57,19 +57,19 @@
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	wbDefcon>=0.2.0
-	compreffor>=0.5.3
-	glyphsLib>=6.2.3
+	wbDefcon>=0.2.3
+	compreffor>=0.5.4
+	glyphsLib>=6.3.0
 	psautohint>=2.4.0
-	ufo2ft>=2.32.0
+	ufo2ft>=2.33.3
 
 [options.packages.find]
 where = Lib
 
 [tox:tox]
 min_version = 4.6
 env_list =
```

