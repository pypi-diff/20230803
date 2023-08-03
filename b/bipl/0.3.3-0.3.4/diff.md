# Comparing `tmp/bipl-0.3.3.tar.gz` & `tmp/bipl-0.3.4.tar.gz`

## Comparing `bipl-0.3.3.tar` & `bipl-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/__init__.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/_env.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/py.typed
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/__init__.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_dzi.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_gdal.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_libs.py
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_openslide.py
--rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_slide.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_slide_bases.py
--rw-r--r--   0        0        0    13962 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_tiff.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_util.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/ops/__init__.py
--rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/ops/_mosaic.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/ops/_util.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.3.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.3.3/LICENSE
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.3.3/README.md
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.3.3/hatch_build.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 bipl-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 bipl-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/__init__.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/_env.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/py.typed
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/__init__.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_dzi.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_gdal.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_libs.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_openslide.py
+-rw-r--r--   0        0        0     6843 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_slide.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_slide_bases.py
+-rw-r--r--   0        0        0    13949 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_tiff.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/io/_util.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/ops/__init__.py
+-rw-r--r--   0        0        0    15302 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/ops/_mosaic.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 bipl-0.3.4/src/bipl/ops/_util.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.3.4/README.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.3.4/hatch_build.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 bipl-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 bipl-0.3.4/PKG-INFO
```

### Comparing `bipl-0.3.3/src/bipl/io/__init__.py` & `bipl-0.3.4/src/bipl/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.3/src/bipl/io/_dzi.py` & `bipl-0.3.4/src/bipl/io/_dzi.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.3/src/bipl/io/_gdal.py` & `bipl-0.3.4/src/bipl/io/_gdal.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,32 +48,30 @@
 @dataclass(frozen=True)
 class _Lod(Lod):
     index: int
     g: Gdal
     bands: tuple[gdal.Band, ...]
 
     def crop(self, slices: tuple[slice, ...]) -> np.ndarray:
-        (y_min2, y_max2), (x_min2, x_max2) = box_ \
-            = [(s.start, s.stop) for s in slices]  # noqa: UP027
-        box = np.array(box_, int)
-        valid_box = box.T.clip([0, 0], self.shape[:2]).T.tolist()
+        box, valid_box, shape = self._unpack_loc(slices)
 
-        (y_min, y_max), (x_min, x_max) = valid_box
-        if y_min == y_max or x_min == x_max:  # Patch is outside slide
+        (y0, y1), (x0, x1) = valid_box.tolist()
+        if y0 == y1 or x0 == x1:  # Patch is outside slide
             return np.broadcast_to(self.g.bg_color,
-                                   (y_max2 - y_min2, x_max2 - x_min2, 3))
+                                   shape)
 
-        h, w = y_max - y_min, x_max - x_min
+        h, w = y1 - y0, x1 - x0
         c = self.g.num_channels
         chw = np.empty((c, h, w), 'u1')
 
         with self.g.lock:
             for b, hw in zip(self.bands, np.split(chw, c, 0)):
-                gdal_array.BandReadAsArray(b, x_min, y_min, w, h, buf_obj=hw)
+                gdal_array.BandReadAsArray(b, x0, y0, w, h, buf_obj=hw)
 
+        # TODO: add pad if necessary
         return chw.transpose(1, 2, 0)
 
 
 class Gdal(Driver):
     def __init__(self, path: str):
         path = _fix_if_url(path)
         self.ds: gdal.Dataset = gdal.OpenEx(path, gdal.GA_ReadOnly)
```

### Comparing `bipl-0.3.3/src/bipl/io/_libs.py` & `bipl-0.3.4/src/bipl/io/_libs.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.3/src/bipl/io/_openslide.py` & `bipl-0.3.4/src/bipl/io/_openslide.py`

 * *Files 12% similar despite different names*

```diff
@@ -99,44 +99,33 @@
 @dataclass(frozen=True)
 class _Lod(Lod):
     pool: int
     index: int
     osd: Openslide
 
     def crop(self, slices: tuple[slice, ...]) -> np.ndarray:
-        (y_min2, y_max2), (x_min2, x_max2) = box_ \
-            = [(s.start, s.stop) for s in slices]  # noqa: UP027
-        box = np.array(box_)
-        valid_box = box.T.clip([0, 0], self.shape[:2]).T
-
-        (y_min, y_max), (x_min, x_max) = valid_box
-        if y_min == y_max or x_min == x_max:  # Patch is outside slide
-            return np.broadcast_to(self.osd.bg_color,
-                                   (y_max2 - y_min2, x_max2 - x_min2, 3))
+        box, valid_box, shape = self._unpack_loc(slices)
 
-        bgra = np.empty((y_max - y_min, x_max - x_min, 4), dtype='u1')
+        (y0, y1), (x0, x1) = valid_box
+        if y0 == y1 or x0 == x1:  # Patch is outside slide
+            return np.broadcast_to(self.osd.bg_color, (*shape, 3))
+
+        bgra = np.empty((y1 - y0, x1 - x0, 4), dtype='u1')
         OSD.openslide_read_region(
             self.osd.ptr,
             c_void_p(bgra.ctypes.data),
-            int(x_min * self.pool),
-            int(y_min * self.pool),
+            int(x0 * self.pool),
+            int(y0 * self.pool),
             self.index,
-            int(x_max - x_min),
-            int(y_max - y_min),
+            int(x1 - x0),
+            int(y1 - y0),
         )
-
         rgb = _mbgra_to_rgb(bgra, self.osd.bg_color)
 
-        offsets = np.abs(valid_box - box).ravel().tolist()
-        if any(offsets):
-            bg_color = self.osd.bg_color.tolist()
-            return cv2.copyMakeBorder(
-                rgb, *offsets, borderType=cv2.BORDER_CONSTANT, value=bg_color)
-
-        return np.ascontiguousarray(rgb)
+        return self._expand(rgb, valid_box, box, self.osd.bg_color)
 
 
 class Openslide(Driver):
     def __init__(self, path: str):
         self.ptr = OSD.openslide_open(path.encode())
         if not self.ptr:
             raise ValueError(f'File {path} cannot be opened')
```

### Comparing `bipl-0.3.3/src/bipl/io/_slide.py` & `bipl-0.3.4/src/bipl/io/_slide.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 from warnings import warn
 
 import cv2
 import numpy as np
 from glow import memoize, shared_call, weak_memoize
 
 from bipl import env
+from bipl.ops import normalize_loc
 
 from ._openslide import Openslide
-from ._slide_bases import REGISTRY, Driver, Item, Lod, normalize
+from ._slide_bases import REGISTRY, Driver, Item, Lod
 from ._tiff import Tiff
 
 # TODO: inside Slide.open import ._slide.registry,
 # TODO: and in ._slide.registry do registration and DLL loading
 # TODO: to make Slide export not require DLL presence
 
 try:
@@ -145,29 +146,30 @@
         if p == zoom:
             return lod
         return lod.rescale(p / zoom)
 
     def __getitem__(self, key: slice | tuple[slice, ...]) -> np.ndarray:
         """Retrieves tile"""
         # TODO: Ignore step, always redirect to self.lods[0].__getitem__
-        slices = normalize(key, self.shape)
+        y_loc, x_loc, c_loc = normalize_loc(key, self.shape)
 
-        step0, step1 = (s.step for s in slices)
+        step0, step1 = y_loc.step, x_loc.step
         if step0 != step1:
             raise ValueError('slice steps should be the same for each axis')
         if step0 <= 0:
             raise ValueError('slice steps should be positive')
 
         pool, lod = self.best_lod_for(step0)
-        slices = *(slice(s.start // pool, s.stop // pool) for s in slices),
-        image = lod.crop(slices)
+        yx_loc = *(slice(s.start // pool, s.stop // pool)
+                   for s in (y_loc, x_loc)),
+        image = lod.crop(yx_loc)
 
         ratio = pool / step0
         dsize = *(round(ratio * s) for s in image.shape[:2]),
-        return _fit_to(image, dsize)
+        return _fit_to(image, dsize)[:, :, c_loc]
 
     def at(self,
            z0_yx_offset: tuple[int, ...],
            dsize: int | tuple[int, ...],
            scale: float = 1) -> np.ndarray:
         """Read square region starting with offset"""
         dsize = dsize if isinstance(dsize, tuple) else (dsize, dsize)
```

### Comparing `bipl-0.3.3/src/bipl/io/_slide_bases.py` & `bipl-0.3.4/src/bipl/io/_slide_bases.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,17 @@
 import re
 from dataclasses import dataclass
 from typing import final
 
 import cv2
 import numpy as np
 
-REGISTRY: dict[re.Pattern, list[type[Driver]]] = {}
-
+from bipl.ops import normalize_loc
 
-def normalize(slices: tuple[slice, ...] | slice,
-              shape: tuple[int, ...]) -> tuple[slice, ...]:
-    """Ensures slices to be exactly 2 slice with non-none endpoints"""
-    if isinstance(slices, slice):
-        slices = slices, slice(None)
-    assert len(slices) == 2
-    return *(slice(
-        s.start if s.start is not None else 0,
-        s.stop if s.stop is not None else axis_len,
-        s.step if s.step is not None else 1,
-    ) for s, axis_len in zip(slices, shape)),
+REGISTRY: dict[re.Pattern, list[type[Driver]]] = {}
 
 
 @dataclass(frozen=True)
 class Item:
     shape: tuple[int, ...]
 
     @property
@@ -49,17 +38,17 @@
     def crop(self, slices: tuple[slice, ...]) -> np.ndarray:
         """Reads crop of LOD. Overridable"""
         raise NotImplementedError
 
     @final
     def __getitem__(self, key: slice | tuple[slice, ...]) -> np.ndarray:
         """Reads crop of LOD"""
-        slices = normalize(key, self.shape)
-        assert all(s.step == 1 for s in slices)
-        return self.crop(slices)
+        (y_loc, x_loc, c_loc) = normalize_loc(key, self.shape)
+        assert y_loc.step == x_loc.step == 1
+        return self.crop((y_loc, x_loc))[:, :, c_loc]
 
     @final
     def __array__(self) -> np.ndarray:
         """Reads whole LOD in single call"""
         return self[:, :]
 
     def rescale(self, scale: float) -> Lod:
@@ -70,14 +59,32 @@
             # TODO: round/ceil/floor ?
             (round(h * scale), round(w * scale), c),
             (self.spacing / scale if self.spacing else None),
             scale,
             self.base if isinstance(self, ProxyLod) else self,
         )
 
+    def _unpack_loc(
+        self,
+        slices: tuple[slice, ...],
+    ) -> tuple[np.ndarray, np.ndarray, list[int]]:
+        box = np.array([(s.start, s.stop) for s in slices])
+        valid_box = box.T.clip([0, 0], self.shape[:2]).T  # (2, lo-hi)
+        shape = (box[:, 1] - box[:, 0]).tolist()
+        return box, valid_box, shape
+
+    def _expand(self, rgb: np.ndarray, valid_box: np.ndarray, box: np.ndarray,
+                bg_color: np.ndarray) -> np.ndarray:
+        offsets = np.abs(valid_box - box)
+        if offsets.any():
+            tp, bm, lt, rt = offsets.ravel().tolist()
+            rgb = cv2.copyMakeBorder(rgb, tp, bm, lt, rt, cv2.BORDER_CONSTANT,
+                                     None, bg_color.tolist())
+        return np.ascontiguousarray(rgb)
+
 
 @dataclass(frozen=True)
 class ProxyLod(Lod):
     scale: float
     base: Lod
 
     def crop(self, slices: tuple[slice, ...]) -> np.ndarray:
```

### Comparing `bipl-0.3.3/src/bipl/io/_tiff.py` & `bipl-0.3.4/src/bipl/io/_tiff.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,35 +273,36 @@
             return JpegArray(data, self.jpt, self.color.space.value)
         return ImageArray(data)
 
     def crop(self, slices: tuple[slice, ...]) -> np.ndarray:
         box = np.array([(s.start, s.stop) for s in slices])
 
         *tile, spp = self.tile
-        dy, dx = (low for low, _ in box)
+        dyx = box[:, 0]  # (2 lo-hi) -> (2)
         out = np.ascontiguousarray(
-            np.broadcast_to(self.bg_color,
-                            [hi - lo for lo, hi in box] + [spp]))
+            np.broadcast_to(
+                self.bg_color,
+                np.r_[box[:, 1] - box[:, 0], spp],
+            ))
 
-        hw = self.shape[:2]
-        bmin, bmax = np.transpose(box).clip(0, hw)
+        bmin, bmax = box.T.clip(0, self.shape[:2])
 
         axes = *map(slice, bmin // tile, -(-bmax // tile)),
         t_lo = np.mgrid[axes].reshape(2, -1).T * tile  # [N, 2]
         if not t_lo.size:
             return out
 
         with self.tiff.ifd(self.index) as ptr:
             parts = [self._get_tile(y, x, ptr) for y, x in t_lo.tolist()]
 
         # [N, lo-hi, yx]
         crops = np.stack([t_lo, t_lo + tile], 1).clip(bmin, bmax)
 
         # [N, yx, lo-hi]
-        o_crops = (crops - [dy, dx]).transpose(0, 2, 1)
+        o_crops = (crops - dyx).transpose(0, 2, 1)
         t_crops = (crops - t_lo[:, None, :]).transpose(0, 2, 1)
         for part, (oy, ox), (ty, tx) in zip(parts, o_crops, t_crops):
             patch = np.array(part, copy=False)
             out[slice(*oy), slice(*ox)] = patch[slice(*ty), slice(*tx)]
 
         return out
```

### Comparing `bipl-0.3.3/src/bipl/io/_util.py` & `bipl-0.3.4/src/bipl/io/_util.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.3/src/bipl/ops/_mosaic.py` & `bipl-0.3.4/src/bipl/ops/_mosaic.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from itertools import chain
 from typing import NamedTuple, Protocol, TypeVar, cast
 
 import cv2
 import numpy as np
 from glow import chunked, map_n
 
-from ._util import get_trapz
+from ._util import get_trapz, normalize_loc
 
 Vec = tuple[int, int]
 
 # TODO: allow result of .map/.map_batched to have different tile and step
 
 # ------------------------------- basic types --------------------------------
 
@@ -70,14 +70,25 @@
         yield Tile(
             idx=iyx,
             vec=(y, x),
             data=tile[:h - y, :w - x],
         )
 
 
+def _padslice(a: NumpyLike, loc: tuple[slice, ...]) -> np.ndarray:
+    loc = normalize_loc(loc, a.shape)
+
+    pos_loc = *(slice(max(s.start, 0), s.stop) for s in loc),
+    a = a[pos_loc]
+
+    pad = [(pos.start - raw.start, pos.stop - pos.start - size)
+           for raw, pos, size in zip(loc, pos_loc, a.shape)]
+    return np.pad(a, pad) if np.any(pad) else a
+
+
 def get_fusion(tiles: Iterable[Tile],
                shape: tuple[int, ...] | None = None) -> np.ndarray | None:
     r: np.ndarray | None = None
 
     if shape is None:  # Collect all the tiles to compute destination size
         tiles = [*tiles]
         # N arrays of (yx + hw)
@@ -336,27 +347,16 @@
     def _slice_tile(self, iy: int, ix: int) -> Tile:
         """Slice source image to get overlapping tiles"""
         (y0, y1), (x0, x1) = ((
             self.m.step * i - self.m.overlap,
             self.m.step * (i + 1),
         ) for i in (iy, ix))
 
-        y0_u = max(y0, 0)
-        x0_u = max(x0, 0)
-        data = self.data[y0_u:y1, x0_u:x1]
-        pad = [
-            (y0_u - y0, y1 - y0_u - data.shape[0]),
-            (x0_u - x0, x1 - x0_u - data.shape[1]),
-            (0, 0),
-        ]
-        return Tile(
-            idx=(iy, ix),
-            vec=(y0, x0),
-            data=np.pad(data, pad),
-        )
+        data = _padslice(self.data, (slice(y0, y1), slice(x0, x1)))
+        return Tile(idx=(iy, ix), vec=(y0, x0), data=data)
 
     def _get_tile(self, iy: int, ix: int) -> Tile:
         """Read non-overlapping tile of source image"""
         (y0, y1), (x0, x1) = ((
             self.m.step * i - self.m.overlap,
             self.m.step * (i + 1),
         ) for i in (iy, ix))
@@ -407,14 +407,18 @@
         ys, xs = np.where(self.cells)
         if isinstance(self.data, np.ndarray):
             return map(self._slice_tile, ys, xs)
 
         parts = map_n(self._get_tile, ys, xs, max_workers=self.max_workers)
         return self._rejoin_tiles(parts) if self.m.overlap else iter(parts)
 
+    def get_tile(self, idx: int) -> Tile:
+        iy, ix = np.argwhere(self.cells)[idx]
+        return self._slice_tile(iy, ix)
+
 
 @dataclass
 class _UniqueTileView(_BaseView):
     """
     Applies weighted average over overlapping regions.
     Yields tiles without overlaps, so their size can differ.
     """
```

### Comparing `bipl-0.3.3/LICENSE` & `bipl-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bipl-0.3.3/README.md` & `bipl-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `bipl-0.3.3/hatch_build.py` & `bipl-0.3.4/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.3/pyproject.toml` & `bipl-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch.build.targets.wheel]
 artifacts = ["*.dll"]  # only wheel keeps DLLs
 
 [tool.hatch.build.hooks.custom]  # enable "custom" hook
 
 [project]
 name = "bipl"
-version = "0.3.3"
+version = "0.3.4"
 description = "Big Image Python Library"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["TIFF", "SVS", "OpenSlide", "tiles"]
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
```

### Comparing `bipl-0.3.3/PKG-INFO` & `bipl-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipl
-Version: 0.3.3
+Version: 0.3.4
 Summary: Big Image Python Library
 Project-URL: homepage, https://github.com/arquolo/bipl
 Project-URL: repository, https://github.com
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
```

