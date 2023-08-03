# Comparing `tmp/math2d-0.6.tar.gz` & `tmp/math2d-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/math2d-0.6.tar", last modified: Mon Feb 10 15:49:06 2020, max compression
+gzip compressed data, was "math2d-0.7.tar", last modified: Thu Aug  3 13:18:38 2023, max compression
```

## Comparing `math2d-0.6.tar` & `math2d-0.7.tar`

### file list

```diff
@@ -1,12 +1,21 @@
-drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2020-02-10 15:49:06.000000 math2d-0.6/
--rw-r--r--   0 ml        (1000) ml        (1000)      550 2020-02-10 15:49:06.000000 math2d-0.6/PKG-INFO
-drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2020-02-10 15:49:06.000000 math2d-0.6/math2d/
--rw-r--r--   0 ml        (1000) ml        (1000)      439 2019-09-10 05:33:47.000000 math2d-0.6/math2d/__init__.py
-drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2020-02-10 15:49:06.000000 math2d-0.6/math2d/geometry/
--rw-r--r--   0 ml        (1000) ml        (1000)    14563 2019-09-12 08:30:05.000000 math2d-0.6/math2d/geometry/__init__.py
--rw-r--r--   0 ml        (1000) ml        (1000)     2348 2019-09-10 05:33:47.000000 math2d-0.6/math2d/geometry/patch.py
--rw-r--r--   0 ml        (1000) ml        (1000)     3143 2019-09-10 05:33:47.000000 math2d-0.6/math2d/orientation.py
--rw-r--r--   0 ml        (1000) ml        (1000)     1040 2019-09-10 05:33:47.000000 math2d-0.6/math2d/test.py
--rw-r--r--   0 ml        (1000) ml        (1000)     2988 2019-09-10 05:33:47.000000 math2d-0.6/math2d/transform.py
--rw-r--r--   0 ml        (1000) ml        (1000)     4034 2019-09-10 05:33:47.000000 math2d-0.6/math2d/vector.py
--rw-r--r--   0 ml        (1000) ml        (1000)      700 2020-02-10 15:43:49.000000 math2d-0.6/setup.py
+drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2023-08-03 13:18:38.979558 math2d-0.7/
+-rw-r--r--   0 ml        (1000) ml        (1000)     7652 2023-06-09 09:18:50.000000 math2d-0.7/COPYING.LESSER
+-rw-r--r--   0 ml        (1000) ml        (1000)      553 2023-08-03 13:18:38.979558 math2d-0.7/PKG-INFO
+drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2023-08-03 13:18:38.971558 math2d-0.7/math2d/
+-rw-r--r--   0 ml        (1000) ml        (1000)      439 2023-06-09 09:20:46.000000 math2d-0.7/math2d/__init__.py
+drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2023-08-03 13:18:38.975558 math2d-0.7/math2d/geometry/
+-rw-r--r--   0 ml        (1000) ml        (1000)    16901 2021-09-13 21:47:23.000000 math2d-0.7/math2d/geometry/__init__.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     2351 2021-09-13 21:47:23.000000 math2d-0.7/math2d/geometry/patch.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     3106 2023-06-09 09:18:50.000000 math2d-0.7/math2d/orientation.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     1043 2021-09-13 21:47:23.000000 math2d-0.7/math2d/test.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     2992 2023-06-09 09:18:50.000000 math2d-0.7/math2d/transform.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     4440 2023-06-09 09:18:50.000000 math2d-0.7/math2d/vector.py
+drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2023-08-03 13:18:38.975558 math2d-0.7/math2d.egg-info/
+-rw-r--r--   0 ml        (1000) ml        (1000)      553 2023-08-03 13:18:38.000000 math2d-0.7/math2d.egg-info/PKG-INFO
+-rw-r--r--   0 ml        (1000) ml        (1000)      315 2023-08-03 13:18:38.000000 math2d-0.7/math2d.egg-info/SOURCES.txt
+-rw-r--r--   0 ml        (1000) ml        (1000)        1 2023-08-03 13:18:38.000000 math2d-0.7/math2d.egg-info/dependency_links.txt
+-rw-r--r--   0 ml        (1000) ml        (1000)        7 2023-08-03 13:18:38.000000 math2d-0.7/math2d.egg-info/top_level.txt
+-rw-r--r--   0 ml        (1000) ml        (1000)       38 2023-08-03 13:18:38.979558 math2d-0.7/setup.cfg
+-rw-r--r--   0 ml        (1000) ml        (1000)      767 2023-08-03 13:18:34.000000 math2d-0.7/setup.py
+drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2023-08-03 13:18:38.975558 math2d-0.7/test/
+-rw-r--r--   0 ml        (1000) ml        (1000)      812 2021-09-13 21:47:23.000000 math2d-0.7/test/test_line_segment.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `math2d-0.6/math2d/geometry/__init__.py` & `math2d-0.7/math2d/geometry/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,48 +2,52 @@
 
 """
 """
 
 __author__ = "Morten Lind"
 __copyright__ = "Morten Lind 2016-2019"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Development"
 
 
+import itertools
+
 import numpy as np
 from .. import Vector, Transform
 from .. import EPS
 from .patch import Patch
 
+
 class Line(object):
     """A mathematical line, i.e. double infinite."""
 
     def __init__(self, start, end):
         self._start = Vector(start)
         self._end = Vector(end)
         self._update()
 
     def __repr__(self):
         return 'Line(p{}, d{})'.format(self._start.tolist(),
                                        self._dir.tolist())
 
-    def fit_points(self, points):
-        """Compute the line from a set of points. 'points'
-        must be an array of row position vectors, such that
-        points[i] is a position vector."""
-        points = np.array(points)
+    def fit_points(self, points: np.ndarray):
+        """Compute this line from a set of points. 'points' must be an
+        (N,2)-array of row position vectors, such that points[i] is a
+        position vector.
+        """
         centre = np.sum(points, axis=0)/len(points)
         eigen = np.linalg.eig(np.cov(points.T))
         max_ev_i = np.where(eigen[0] == max(eigen[0]))[0][0]
         direction = eigen[1].T[max_ev_i]
         self._start = Vector(centre)
         self._dir = Vector(direction)
+        # End should not be used on a line
         self._end = self._start + self._dir
 
     @classmethod
     def new_fitted_points(cls, points):
         obj = cls(1, 2)
         obj.fit_points(points)
         return obj
@@ -56,30 +60,34 @@
     @classmethod
     def new_from_coeffs(cls, a, b):
         start = Vector(0, b)
         end = Vector(1, b + a)
         return cls(start, end)
 
     @property
-    def dir(self):
+    def direction(self):
         """Get the direction of the line."""
         return self._dir.copy()
 
+    dir = direction
+
     @property
     def point(self):
         """Get a point on the line"""
         return self._start.copy()
 
     @property
     def unit_direction(self):
-        return self._dir.copy()
+        return self._dir.normalized
 
+    udir = unit_direction
+    
     def _update(self):
         """Update derived data from changed fundamental data."""
-        self._dir = (self._end - self._start).normalized
+        self._dir = (self._end - self._start)
 
     def reverse(self):
         """Simply reverses the unit direction vector and swaps the start and
         end points.
         """
         start = self._end
         end = self._start
@@ -87,15 +95,14 @@
         self._end = Vector(end)
         self._update()
 
     @property
     def reversed(self):
         return LineSegment(self._end, self._start)
 
-    
     def transform(self, trf):
         """Apply the given transform inline."""
         self._start = trf * self._start
         self._end = trf * self._end
         Line._update(self)
 
     def __rmul__(self, trf):
@@ -132,20 +139,30 @@
         if type(other) == Line:
             return self._l_intersect(other)
         else:
             return other.intersection(self)
 
     def dist(self, other):
         """Compute the distance to 'other'."""
+        if type(other) == np.ndarray and len(other) == 2:
+            other = Vector(other)
         if type(other) == Vector:
             pp = self.project(other)
             return other.dist(pp)
+        if type(other) == LineSegment:
+            return other.dist(self)
         else:
             raise NotImplementedError
 
+    def angle(self, other):
+        if type(other) in (Line, LineSegment):
+            return self.dir.angle(other.dir, minimal=True)
+        elif type(other) == Vector:
+            return self.dir.angle(other, minimal=True)
+
     @property
     def coeffs(self):
         """Return the coefficients, (inclination, intercept) for this line."""
         a = self._dir.y / self._dir.x
         b = self._start.y - self._start.x * a
         return (a, b)
 
@@ -161,19 +178,14 @@
         """Update derived data from changed fundamental data."""
         self._delta = self._end - self._start
         self._dir = self._delta.normalized
         self.length = self._delta.norm
         self.centre = self._start + 0.5 * self._delta
 
     @property
-    def dir(self):
-        """Get the direction of the line segment."""
-        return self._dir.copy()
-
-    @property
     def delta(self):
         """Get the segment vector of the line segment."""
         return self._delta.copy()
 
     @property
     def start(self):
         """Get the start of the line segment."""
@@ -201,15 +213,14 @@
 
     @classmethod
     def new_fitted_points(cls, points):
         """Fit the given points to a line, and set start and end according to
         the min and max projection of the points. 'points' must be a
         2D iterable of row vectors, i.e. shape == (n, 2).
         """
-        points = np.array(points)
         line = Line.new_fitted_points(points)
         projs = (points - line.point) * line.unit_direction
         start = line.point + projs.min() * line.unit_direction
         end = line.point + projs.max() * line.unit_direction
         return LineSegment(start, end)
 
     def __contains__(self, p):
@@ -238,23 +249,64 @@
             return NotImplemented
 
     def __repr__(self):
         return 'LineSegment({} -> {})'.format(self._start.tolist(),
                                               self._end.tolist())
 
     def dist(self, other):
-        """Compute the distance to 'other'."""
+        """Compute the distance to 'other'. """
+        if type(other) == np.ndarray and len(other) == 2:
+            other = Vector(other)
         if type(other) == Vector:
             pp = self.project(other)
             if pp in self:
                 return other.dist(pp)
             else:
                 return min(other.dist(self._start), other.dist(self._end))
+        elif type(other) == Line:
+            # If the line intersects, return 0. Otherwise, one of the
+            # end-points of this segment is the closest point.
+            if len(self.intersection(other)) == 0:
+                return 0.0
+            else:
+                return min(other.dist(self.start), other.dist(self.end))
+        elif type(other) == LineSegment:
+            # If the line segments intersects, return 0. Otherwise, one of the
+            # end-points of this segment is the closest point.
+            if len(self.intersection(other)) > 0:
+                # SOLUTION FOUND, RETURNING
+                return 0.0
+            # Go through all end points' projections on the opposing
+            # line, and see if it is within the segment
+            epp_dists = []
+            slos = self.project(other.start)
+            if slos in self:
+                print('slos projects')
+                epp_dists.append(slos.dist(other.start))
+            sloe = self.project(other.end)
+            if sloe in self:
+                print('sloe projects')
+                epp_dists.append(sloe.dist(other.end))
+            olss = other.project(self.start)
+            if olss in other:
+                print('olss projects')
+                epp_dists.append(olss.dist(self.start))
+            olse = other.project(self.end)
+            if olse in other:
+                print('olse projects')
+                epp_dists.append(olse.dist(self.end))
+            # Add the opposing end point pairs distances
+            epp_dists += [ep[0].dist(ep[1])
+                          for ep in itertools.product(
+                                  (self.start, self.end),
+                                  (other.start, other.end))]
+            return min(epp_dists)
         else:
-            raise NotImplementedError
+            raise NotImplementedError(
+                f'Can not calculate distance to a {type(other)}')
 
     def _ls_intersect(self, ls):
         """http://stackoverflow.com/a/565282"""
         s = self
         o = ls
         s2o = o._start - s._start
         dcross = np.cross(s._delta, o._delta)
@@ -428,25 +480,26 @@
     ls0 = LineSegment((1, 2), (2, 4))
     ls1 = LineSegment((1, 0), (0, 2))
     assert len(ls1.intersection(ls0)) == 0
     ls2 = LineSegment((0, 0), (1, 2))
     assert (ls1.intersection(ls2)[0] -
             Vector(0.5, 1)).norm == 0.0
     # Testing line fitting
-    points = [[2, 2],
-              [1, 1],
-              [3, 3]]
+    points = np.array([[2, 3],
+                       [1, 2],
+                       [3, 4]])
     fl = Line.new_fitted_points(points)
-    assert(fl.point == Vector(2, 2))
+    assert(fl.point == Vector(2, 3))
     assert(1.0 - np.abs(fl.dir * Vector(1, 1).normalized)
            < 10 * EPS)
     fls = LineSegment.new_fitted_points(points)
-    assert(fls.point == Vector(1, 1))
+    assert(fls.start == Vector(1, 2))
+    assert(fls.end == Vector(3, 4))
     assert(abs(1.0 - np.abs(fls.dir * Vector(1, 1).normalized))
-               < 10 * EPS)
+           < 10 * EPS)
     assert(abs(fls.length - 2 * np.sqrt(2)) < 10 * EPS)
     # Testing LineSegment coefficients property
     ls = LineSegment.new_from_coeffs(1, 2, 1, 2)
     assert (ls.start.x == 1 and ls.start.y == 3 and
             ls.end.x == 2 and ls.end.y == 4)
     assert ls.coeffs[0] == 1 and ls.coeffs[1] == 2
     # Test reversal of Line and LineSegment
```

### Comparing `math2d-0.6/math2d/geometry/patch.py` & `math2d-0.7/math2d/geometry/patch.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 """
 """
 
 __author__ = "Morten Lind"
 __copyright__ = "Morten Lind 2016-2017"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Development"
 
 import itertools
 import collections
 
 import numpy as np
```

### Comparing `math2d-0.6/math2d/orientation.py` & `math2d-0.7/math2d/orientation.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,31 @@
 
 """
 """
 
 __author__ = "Morten Lind"
 __copyright__ = "Morten Lind 2016-2017"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Development"
 
 
-from collections import Iterable
-from numbers import Number
+from collections.abc import Iterable
 
 import numpy as np
 
 from .vector import Vector
-import math2d
 
 
 class Orientation(np.ndarray):
 
     def __new__(cls, *args, **kwargs):
-        return np.ndarray.__new__(cls, (2, 2), dtype=np.float)
+        return np.ndarray.__new__(cls, (2, 2), dtype=float)
 
     def __init__(self, *args, **kwargs):
         if len(args) == 0:
             self[:, :] = np.identity(2)
         elif len(args) == 1:
             if isinstance(args[0], Iterable):
                 self[:, :] = np.array(args[0], copy=False)
```

### Comparing `math2d-0.6/math2d/test.py` & `math2d-0.7/math2d/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 """
 """
 
 __author__ = "Morten Lind"
 __copyright__ = "Morten Lind 2016-2017"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Development"
 
 from . import Vector, Orientation, Transform
 
 def test_ref():
     """Test that the 'orient' and 'pos' properties of a Transform gets
     reference to the Transform data.
```

### Comparing `math2d-0.6/math2d/transform.py` & `math2d-0.7/math2d/transform.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 """
 """
 
 __author__ = "Morten Lind"
 __copyright__ = "Morten Lind 2016-2017"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Development"
 
 
-from collections import Iterable
+from collections.abc import Iterable
 
 import numpy as np
 
 from .vector import Vector
 from .orientation import Orientation
 
 
 class Transform(np.ndarray):
     def __new__(cls, *args, **kwargs):
-        return np.ndarray.__new__(cls, (3, 3), dtype=np.float)
+        return np.ndarray.__new__(cls, (3, 3), dtype=float)
 
     def __init__(self, *args):
         self[:, :] = np.identity(3)
         if len(args) == 2:
             if isinstance(args[1], Iterable):
                 # Argument at index 1 must be a vector
                 self[:2, :2] = Orientation(args[0])
```

### Comparing `math2d-0.6/math2d/vector.py` & `math2d-0.7/math2d/vector.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 
 """
 """
 
 __author__ = "Morten Lind"
 __copyright__ = "Morten Lind 2016-2017"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Development"
 
 
 from numbers import Number
-from collections import Iterable
 
 import numpy as np
 import math2d as m2d
 
 from . import EPS
 
 
@@ -37,21 +36,21 @@
     def unit_vectors(self):
         return [Vector.ex, Vector.ey]
 
 
 class Vector(np.ndarray, metaclass=_UnitVectors):
 
     def __new__(cls, *args, **kwargs):
-        return np.ndarray.__new__(cls, (2,), dtype=np.float)
+        return np.ndarray.__new__(cls, (2,), dtype=float)
 
     def __init__(self, *args, **kwargs):
         if len(args) > 0:
             self[:] = np.array(args).flatten()[:2]
         else:
-            self[:] = np.zeros(2, dtype=np.float)
+            self[:] = np.zeros(2, dtype=float)
 
     def __array_finalize__(self, obj):
         if obj is None:
             return
 
     def __array_wrap__(self, out_arr, context=None):
         return np.ndarray.__array_wrap__(self, out_arr, context)
@@ -89,15 +88,15 @@
         if type(other) == Vector:
             return np.allclose(self, other)
         else:
             return NotImplemented
 
     def __mul__(self, other):
         """Return the dot product of the two vectors."""
-        if type(other) == Vector:
+        if type(other) in (Vector, np.ndarray):
             return self.dot(other)
         elif isinstance(other, Number):
             return other * self[:]
         else:
             return NotImplemented
 
     def rotate(self, angle):
@@ -105,30 +104,41 @@
         self[:] = m2d.Orientation(angle) * self
 
     def rotated(self, angle):
         """Return a vector which is equal to this vector rotated by 'angle'."""
         return m2d.Orientation(angle) * self
 
     def dist(self, other):
+        if type(other) == np.ndarray and len(other) == 2:
+            other = Vector(other)
         if type(other) == Vector:
             return (self - other).norm
         else:
             raise NotImplementedError
 
     def cross(self, other):
         """Cross product with 'other'. The result is a real number, c. If
         considering R2 embedded in R3, the resulting vector (0, 0, c)
         is the cross product in R3 of the R3-extension of the
         operands.
         """
-        return np.float(np.cross(self, other))
+        return float(np.cross(self, other))
 
-    def angle(self, other):
-        """Numerical angle with 'other' in [0, pi]."""
-        return np.arccos(self * other / (self.norm * other.norm))
+    def angle(self, other, minimal=False):
+        """Numerical angle with 'other' in [0, pi]. If 'minimal', the angle
+        between lines corresponding to the vectors is returned in [0,
+        pi/2].
+        """
+        direction_angle = np.arccos(self * other / (self.norm * other.norm))
+        if minimal:
+            return min(
+                direction_angle,
+                np.arccos(self * -other / (self.norm * other.norm)))
+        else:
+            return direction_angle
 
     def signed_angle_to(self, other):
         """Signed rotation angle to 'other' in [-pi; pi]."""
         cprod = self.cross(other)
         if np.abs(cprod) < EPS:
             cprod = 1.0
         return np.sign(cprod) * self.angle(other)
```

### Comparing `math2d-0.6/setup.py` & `math2d-0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from distutils.core import setup
 from distutils.command.install_data import install_data
 
 setup (
     name='math2d',
-    version='0.6',
+    version='0.7',
     description='2D mathematics package for Python.',
     author='Morten Lind',
-    author_email='morten@lind.dyndns.dk',
-    url='http://git.automatics.dyndns.dk/?p=pymath2d.git',
+    author_email='morten@lind.fairuse.org',
+    url='https://codeberg.org/moli/pymath2d',
     packages=['math2d', 'math2d.geometry'],
     provides=['math2d'],
     classifiers=[
         'Development Status :: 3 - Alpha',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+        'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Natural Language :: English',
         'Programming Language :: Python',
         'Topic :: Scientific/Engineering',
     ],
-    license='GNU General Public License v3'
+    license='GNU Lesser General Public License v3 (LGPLv3)',
+    data_files=[('share/doc/pymath2d', ['COPYING'])]
 )
```

