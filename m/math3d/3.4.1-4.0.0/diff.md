# Comparing `tmp/math3d-3.4.1.tar.gz` & `tmp/math3d-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math3d-3.4.1.tar", last modified: Thu Mar  4 10:52:16 2021, max compression
+gzip compressed data, was "math3d-4.0.0.tar", last modified: Thu Aug  3 13:53:30 2023, max compression
```

## Comparing `math3d-3.4.1.tar` & `math3d-4.0.0.tar`

### file list

```diff
@@ -1,32 +1,44 @@
-drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2021-03-04 10:52:16.349520 math3d-3.4.1/
--rw-r--r--   0 ml        (1000) ml        (1000)    34523 2021-03-04 10:13:23.497193 math3d-3.4.1/COPYING
--rw-r--r--   0 ml        (1000) ml        (1000)      577 2021-03-04 10:52:16.349520 math3d-3.4.1/PKG-INFO
--rw-r--r--   0 ml        (1000) ml        (1000)     7116 2019-05-07 09:29:47.520976 math3d-3.4.1/README.md
-drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2021-03-04 10:52:16.345520 math3d-3.4.1/math3d/
--rw-r--r--   0 ml        (1000) ml        (1000)      534 2021-03-04 10:51:29.249576 math3d-3.4.1/math3d/__init__.py
-drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2021-03-04 10:52:16.345520 math3d-3.4.1/math3d/dynamics/
--rw-r--r--   0 ml        (1000) ml        (1000)      365 2021-01-20 12:50:36.107183 math3d-3.4.1/math3d/dynamics/__init__.py
--rw-r--r--   0 ml        (1000) ml        (1000)     6807 2021-01-20 12:50:36.115183 math3d-3.4.1/math3d/dynamics/twist.py
--rw-r--r--   0 ml        (1000) ml        (1000)     6822 2021-01-20 12:50:36.119183 math3d-3.4.1/math3d/dynamics/wrench.py
-drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2021-03-04 10:52:16.345520 math3d-3.4.1/math3d/geometry/
--rw-r--r--   0 ml        (1000) ml        (1000)      332 2021-01-20 12:50:36.127183 math3d-3.4.1/math3d/geometry/__init__.py
--rw-r--r--   0 ml        (1000) ml        (1000)     5423 2021-01-20 12:50:36.131183 math3d-3.4.1/math3d/geometry/line.py
--rw-r--r--   0 ml        (1000) ml        (1000)     9178 2021-01-20 12:50:36.135183 math3d-3.4.1/math3d/geometry/plane.py
-drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2021-03-04 10:52:16.349520 math3d-3.4.1/math3d/interpolation/
--rw-r--r--   0 ml        (1000) ml        (1000)      425 2021-01-20 12:50:36.139183 math3d-3.4.1/math3d/interpolation/__init__.py
--rw-r--r--   0 ml        (1000) ml        (1000)     1870 2021-01-20 12:50:36.139183 math3d-3.4.1/math3d/interpolation/r3interpolation.py
--rw-r--r--   0 ml        (1000) ml        (1000)     2593 2021-01-20 12:50:36.143183 math3d-3.4.1/math3d/interpolation/se3interpolation.py
--rw-r--r--   0 ml        (1000) ml        (1000)     2832 2021-01-20 12:50:36.151183 math3d-3.4.1/math3d/interpolation/so3interpolation.py
--rw-r--r--   0 ml        (1000) ml        (1000)    27755 2021-01-20 12:50:36.155183 math3d-3.4.1/math3d/orientation.py
--rw-r--r--   0 ml        (1000) ml        (1000)     2576 2021-01-20 12:50:36.163183 math3d-3.4.1/math3d/orientation_computer.py
--rw-r--r--   0 ml        (1000) ml        (1000)    20219 2021-03-04 09:43:57.106242 math3d-3.4.1/math3d/quaternion.py
-drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2021-03-04 10:52:16.349520 math3d-3.4.1/math3d/reference_system/
--rw-r--r--   0 ml        (1000) ml        (1000)      425 2021-01-20 12:50:36.175183 math3d-3.4.1/math3d/reference_system/__init__.py
--rw-r--r--   0 ml        (1000) ml        (1000)     2291 2021-01-20 12:50:36.175183 math3d-3.4.1/math3d/reference_system/frame.py
--rw-r--r--   0 ml        (1000) ml        (1000)     2058 2021-01-20 12:50:36.175183 math3d-3.4.1/math3d/reference_system/free_vector.py
--rw-r--r--   0 ml        (1000) ml        (1000)     1957 2021-01-20 12:50:36.179183 math3d-3.4.1/math3d/reference_system/point.py
--rw-r--r--   0 ml        (1000) ml        (1000)     6925 2021-01-20 12:50:36.187183 math3d-3.4.1/math3d/reference_system/reference_system.py
--rw-r--r--   0 ml        (1000) ml        (1000)    14439 2021-03-02 15:16:47.773968 math3d-3.4.1/math3d/transform.py
--rw-r--r--   0 ml        (1000) ml        (1000)     1951 2021-01-20 12:50:36.195183 math3d-3.4.1/math3d/utils.py
--rw-r--r--   0 ml        (1000) ml        (1000)    17178 2021-01-20 12:50:36.203183 math3d-3.4.1/math3d/vector.py
--rw-r--r--   0 ml        (1000) ml        (1000)      911 2021-03-04 10:51:19.473587 math3d-3.4.1/setup.py
+drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2023-08-03 13:53:30.304815 math3d-4.0.0/
+-rw-r--r--   0 ml        (1000) ml        (1000)     7652 2022-12-15 08:16:02.000000 math3d-4.0.0/COPYING.LESSER
+-rw-r--r--   0 ml        (1000) ml        (1000)      585 2023-08-03 13:53:30.304815 math3d-4.0.0/PKG-INFO
+-rw-r--r--   0 ml        (1000) ml        (1000)     7116 2021-08-04 08:53:55.000000 math3d-4.0.0/README.md
+drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2023-08-03 13:53:30.288815 math3d-4.0.0/math3d/
+-rw-r--r--   0 ml        (1000) ml        (1000)      576 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/__init__.py
+drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2023-08-03 13:53:30.296815 math3d-4.0.0/math3d/dynamics/
+-rw-r--r--   0 ml        (1000) ml        (1000)      368 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/dynamics/__init__.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     6818 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/dynamics/twist.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     6825 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/dynamics/wrench.py
+drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2023-08-03 13:53:30.296815 math3d-4.0.0/math3d/geometry/
+-rw-r--r--   0 ml        (1000) ml        (1000)      371 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/geometry/__init__.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     7042 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/geometry/line.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     6784 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/geometry/line_segment.py
+-rw-r--r--   0 ml        (1000) ml        (1000)    10702 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/geometry/plane.py
+drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2023-08-03 13:53:30.300815 math3d-4.0.0/math3d/interpolation/
+-rw-r--r--   0 ml        (1000) ml        (1000)      422 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/interpolation/__init__.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     3681 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/interpolation/e3interpolator.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     1212 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/interpolation/interpolator.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     3580 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/interpolation/se3interpolator.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     3119 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/interpolation/so3interpolator.py
+-rw-r--r--   0 ml        (1000) ml        (1000)    31250 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/orientation.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     2579 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/orientation_computer.py
+-rw-r--r--   0 ml        (1000) ml        (1000)    19986 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/quaternion.py
+drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2023-08-03 13:53:30.304815 math3d-4.0.0/math3d/reference_system/
+-rw-r--r--   0 ml        (1000) ml        (1000)      428 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/reference_system/__init__.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     2294 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/reference_system/frame.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     2061 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/reference_system/free_vector.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     1960 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/reference_system/point.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     6928 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/reference_system/reference_system.py
+-rw-r--r--   0 ml        (1000) ml        (1000)    23044 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/transform.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     1962 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/utils.py
+-rw-r--r--   0 ml        (1000) ml        (1000)    21073 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/vector.py
+drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2023-08-03 13:53:30.304815 math3d-4.0.0/math3d/visualization/
+-rw-r--r--   0 ml        (1000) ml        (1000)      292 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/visualization/__init__.py
+-rw-r--r--   0 ml        (1000) ml        (1000)     2224 2022-12-15 08:16:02.000000 math3d-4.0.0/math3d/visualization/transform_visualizer.py
+drwxr-xr-x   0 ml        (1000) ml        (1000)        0 2023-08-03 13:53:30.292815 math3d-4.0.0/math3d.egg-info/
+-rw-r--r--   0 ml        (1000) ml        (1000)      585 2023-08-03 13:53:30.000000 math3d-4.0.0/math3d.egg-info/PKG-INFO
+-rw-r--r--   0 ml        (1000) ml        (1000)      968 2023-08-03 13:53:30.000000 math3d-4.0.0/math3d.egg-info/SOURCES.txt
+-rw-r--r--   0 ml        (1000) ml        (1000)        1 2023-08-03 13:53:30.000000 math3d-4.0.0/math3d.egg-info/dependency_links.txt
+-rw-r--r--   0 ml        (1000) ml        (1000)       17 2023-08-03 13:53:30.000000 math3d-4.0.0/math3d.egg-info/requires.txt
+-rw-r--r--   0 ml        (1000) ml        (1000)        7 2023-08-03 13:53:30.000000 math3d-4.0.0/math3d.egg-info/top_level.txt
+-rw-r--r--   0 ml        (1000) ml        (1000)       38 2023-08-03 13:53:30.304815 math3d-4.0.0/setup.cfg
+-rw-r--r--   0 ml        (1000) ml        (1000)      912 2023-08-03 13:53:24.000000 math3d-4.0.0/setup.py
```

### Comparing `math3d-3.4.1/README.md` & `math3d-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `math3d-3.4.1/math3d/__init__.py` & `math3d-4.0.0/math3d/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Module for top level imports in PyMath3D.
 """
 
 __author__ = "Morten Lind"
 __copyright__ = "Morten Lind 2012-2021"
 __credits__ = ["Morten Lind"]
-__license__ = "AGPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
 __email__ = "morten@lind.fairuse.org"
 __status__ = "Production"
 
-__version__ = "3.4.1"
+__version__ = "4.0-dev"
 
 
 from .utils import set_precision
-from .quaternion import Quaternion, Versor, UnitQuaternion
-from .orientation import Orientation
+from .quaternion import Quaternion, Versor
+from .orientation import Orientation, RotationVector
 from .orientation_computer import OrientationComputer
-from .vector import Vector
-from .transform import Transform
+from .vector import Vector, FreeVector, PositionVector
+from .transform import Transform, PoseVector
```

### Comparing `math3d-3.4.1/math3d/dynamics/twist.py` & `math3d-4.0.0/math3d/dynamics/twist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 # coding=utf-8
 """
 Module implementing the Twist class(es). A twist is generally a
 spatial velocity of a rigid body. It has a linear and an angular part;
-relating to e(3) and se(3), respectively. Different ways of 
+relating to e(3) and se(3), respectively. Different ways of
 """
 
 __author__ = "Morten Lind"
-__copyright__ = "Morten Lind 2013"
+__copyright__ = "Morten Lind 2013-2021"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
-__status__ = "Production"
+__email__ = "morten@lind.fairuse.org"
+__status__ = "Development"
+
 
 import numpy as np
 import math3d as m3d
 
-class OrigoTwist(object):
+
+class OrigoTwist:
     """An OrigoTwist instance is a representation of the motion of the
     defining coordinate system at its origo."""
 
     def __init__(self, *args, **kwargs):
         """Construct an OrigoTwist from arguments. 'kwargs' take
         precedence over given 'args'.
 
         'kwargs' may contain:
 
         * 'v_lin' and 'v_ang', each an iterable of three
           floats, either are optional.
 
-        'args' may contain: 
-        
+        'args' may contain:
+
         * One iterable of six floats. The first three are taken as
           linear and the last three are taken as angular velocities.
 
         * Two iterables of three floats. The first is linear and the
           second angular velocities.
 
         * An OrigoTwist instance (copy constructor).
         """
         if len(args) == 0 and len(kwargs) == 0:
             # Default constructor
-            self._v_lin = m3d.Vector()
-            self._v_ang = m3d.Vector()            
+            self._v_lin = m3d.FreeVector()
+            self._v_ang = m3d.FreeVector()
         elif 'v_lin' in kwargs or 'v_ang' in kwargs:
-            self._v_lin = m3d.Vector(kwargs.get('v_lin', m3d.Vector()))
-            self._v_ang = m3d.Vector(kwargs.get('v_ang', m3d.Vector()))
+            self._v_lin = m3d.FreeVector(kwargs.get('v_lin', m3d.FreeVector()))
+            self._v_ang = m3d.FreeVector(kwargs.get('v_ang', m3d.FreeVector()))
         elif len(args) == 1 and type(args[0]) == OrigoTwist:
             self._v_lin = args[0].linear
             self._v_ang = args[0].angular
         elif len(args) == 1 and len(args[0]) == 6:
-            self._v_lin = m3d.Vector(args[0][:3])
-            self._v_ang = m3d.Vector(args[0][3:])
+            self._v_lin = m3d.FreeVector(args[0][:3])
+            self._v_ang = m3d.FreeVector(args[0][3:])
         elif len(args) == 2 and len(args[0]) == 3 and len(args[1]) == 3:
-            self._v_lin = m3d.Vector(args[0])
-            self._v_ang = m3d.Vector(args[1])
+            self._v_lin = m3d.FreeVector(args[0])
+            self._v_ang = m3d.FreeVector(args[1])
         else:
             raise Exception(
-                self.__class__.__name__ + 
-                'Could not construct on given arguments: *args=' + 
+                self.__class__.__name__ +
+                'Could not construct on given arguments: *args=' +
                 str(args) + ' *kwargs=' + str(kwargs))
 
     def equivalent(self, ref):
         """Compute the eqivalent twist at 'ref'. If 'ref' is a
         transform, compute the transformed equivalent twist at the
         origo of 'ref' and in the orientation of 'ref'. If 'ref' is a
         vector, compute the equivalent twist at 'ref' in the current
@@ -70,77 +72,82 @@
         possibly reoriented. The new v_lin is the old one, possibly
         reoriented, plus the action of the v_ang acting at the old
         origo. Beware that the constant velocity motion obtained by
         the transformed twist is, at the new origo, only
         instantaneously in accord with the current twist, since it
         introduces a translation of the line of rotation.
         """
-        if type(ref) == m3d.Vector:
+        if type(ref) == m3d.PositionVector:
             # 'ref' is given in current coordinates, and represents
             # the point at which the equivalent twist should be
             # found.
             va_n = self._v_ang
             vl_n = self._v_lin - ref.cross(va_n)
             return OrigoTwist(v_lin=vl_n, v_ang=va_n)
-        elif type(ref) == m3d.Transform:            
+        elif type(ref) == m3d.Transform:
             # 'ref' is a transformation to the new coordinate system,
             # at the origo of whom the equivalent twist is sought, in
             # new coordinates.
             m = self._v_ang
             va_n = ref.orient * self._v_ang
             vl_n = ref.orient * self._v_lin + ref.pos.cross(va_n)
             return OrigoTwist(v_lin=vl_n, v_ang=va_n)
-    
+
     def displacement(self, delta_t):
         """Compute the displacement resulting from applying the twist
         for time 'delta_t'. The returned transform will be given in the current
         coordinates and represent the moved coordinate system."""
         return m3d.Transform(delta_t * self.array)
-    
+
     def __rmul__(self, left):
         """Handle a left-operator."""
-        if np.isreal(left):
+        if np.isscalar(left):
             return OrigoTwist(left * self.array)
-        elif type(left) in [m3d.Transform, m3d.Vector]:
+        elif type(left) in (m3d.Transform, m3d.PositionVector):
             return self.equivalent(left)
         elif type(left) == m3d.Orientation:
             # Perform a reorientation of the twist, as observed from a
             # coordinate system with the orientation given in 'left'
-            vl_n = left * self._v_lin 
+            vl_n = left * self._v_lin
             va_n = left * self._v_ang
             return OrigoTwist(v_lin=vl_n, v_ang=va_n)
         else:
             return NotImplemented
 
     # Angular property
     def get_angular(self):
         """Get the angular part."""
-        return self._v_ang.copy()
+        return self._v_ang
+
     def set_angular(self, new_v_ang):
         """Set the angular part."""
-        self._v_ang = m3d.Vector(new_v_ang)
-    angular = property(get_angular, set_angular)
+        self._v_ang = m3d.FreeVector(new_v_ang)
+
+    angular = ang = property(get_angular, set_angular)
 
     # Raw array data access
     def get_array(self):
         return np.append(self._v_lin._data, self._v_ang._data)
+
     array = property(get_array)
 
     # Linear property
     def get_linear(self):
         """Get the linear part."""
-        return self._v_lin.copy()
+        return self._v_lin
+
     def set_linear(self, new_v_lin):
         """Set the linear part."""
-        self._v_lin = m3d.Vector(new_v_lin)
-    linear = property(get_linear, set_linear)
+        self._v_lin = m3d.FreeVector(new_v_lin)
+
+    linear = lin = property(get_linear, set_linear)
 
     def __mul__(self, right):
         """Handle right operation."""
-        if np.isreal(right):
+        if np.isscalar(right):
             return OrigoTwist(right * self.array)
         else:
             return NotImplemented
 
     def __add__(self, v_add):
         """Add two twists. Note that they are percieved as belonging
         to the same origo in the same coordinate system!.
@@ -158,18 +165,17 @@
     def __neg__(self):
         """Return the negative twist."""
         return OrigoTwist(v_lin=-self._v_lin, v_ang=-self._v_ang.data)
 
     # def __copy__(self):
     #     """Copy method for creating a copy of this Vector."""
     #     return (self)
-    
+
     # def __deepcopy__(self, memo):
     #     return self.__copy__()
-        
-    
+
+
     def __repr__(self):
         """String represenstation of the twist."""
         return ('<{} lin=[{:.3f}, {:.3f}, {:.3f}] ang=[{:.3f}, {:.3f}, {:.3f}]>'
-                .format(*([self.__class__.__name__] + 
+                .format(*([self.__class__.__name__] +
                           self._v_lin.list + self._v_ang.list)))
-
```

### Comparing `math3d-3.4.1/math3d/dynamics/wrench.py` & `math3d-4.0.0/math3d/dynamics/wrench.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 composed of a force and a moment acting at a point. The two components
 transform in a different way than two separate vectors.
 """
 
 __author__ = "Morten Lind"
 __copyright__ = "Morten Lind 2013"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Production"
 
 
 import numpy as np
 import math3d as m3d
 
 class OrigoWrench(object):
```

### Comparing `math3d-3.4.1/math3d/geometry/line.py` & `math3d-4.0.0/math3d/geometry/line.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 # coding=utf-8
 
 """
 Module for line class
 """
 
 __author__ = "Morten Lind"
-__copyright__ = "Morten Lind 2016-2019"
+__copyright__ = "Morten Lind 2016-2021"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
 __email__ = "morten@lind.fairuse.org"
 __status__ = "Development"
 
 
 import math3d as m3d
 import numpy as np
 
-from . import plane
 
-class Line(object):
+class Line:
     """A line class."""
 
-    def __init__(self, **kwargs):
-        """Supported, named constructor arguments:
+    def __init__(self, *args, **kwargs):
+        """Supported positional arguments:
+
+        * Two arguments of type FreeVector and PositionVector, one of
+          each in any order.
+
+        Supported named arguments:
 
         * 'point_direction' or 'pd_pair': An ordered pair of vectors
           representing a point on the line and the line's
           direction. The direction does not have to be a unit vector.
 
         * 'point', 'direction': Separate vectors for point on line and
           direction of line in named arguments. The direction does not
@@ -34,99 +38,132 @@
 
         * 'point0', 'point1': Two points defining the line, in named
          arguments.
 
         * 'points': A set of at least two points is used for
         PCA-identification of the direction of the line, and where the
         line point is chosen as the average position.
-        """
 
-        if 'point_direction' in kwargs:
-            self._p, self._d = [m3d.Vector(e)
-                                for e in kwargs['point_direction']]
+        The internal representation is point-direction.
+        """
+        if len(args) not in [0, 2]:
+            raise Exception(
+                self.__class__.__name__ +
+                ': Can only create on two positional arguments ' +
+                'as of types PositionVector and FreeVector!' +
+                f' Was given "{args}"')
+        elif len(args) == 2:
+            # Infer on types Position- and FreeVector
+            if(type(args[0]) == m3d.PositionVector
+               and type(args[1]) == m3d.FreeVector):
+                self._p = args[0].copy()
+                self._d = args[1].copy()
+            elif (type(args[1]) == m3d.PositionVector
+                  and type(args[0]) == m3d.FreeVector):
+                self._p = args[1].copy()
+                self._d = args[0].copy()
+            else:
+                raise Exception(
+                    self.__class__.__name__ +
+                    ': Can only create on two positional arguments' +
+                    ' of types PositionVector and FreeVector (in any order). ' +
+                    f'Was given "{args}"')
+        elif 'point_direction' in kwargs:
+            p, d = kwargs['point_direction']
+            self._p = m3d.PositionVector(p)
+            self._d = m3d.FreeVector(d)
         elif 'pd_pair' in kwargs:
-            self._p, self._d = [m3d.Vector(e)
-                                for e in kwargs['pd_pair']]
+            p, d = kwargs['pd_pair']
+            self._p = m3d.PositionVector(p)
+            self._d = m3d.FreeVector(d)
         elif 'point' in kwargs and 'direction' in kwargs:
-            self._p = m3d.Vector(kwargs['point'])
-            self._d = m3d.Vector(kwargs['direction'])
+            self._p = m3d.PositionVector(kwargs['point'])
+            self._d = m3d.FreeVector(kwargs['direction'])
         elif 'point0' in kwargs and 'point1' in kwargs:
-            self._p = m3d.Vector(kwargs['point0'])
-            self._d = m3d.Vector(kwargs['point1']) - self._p
+            self._p = m3d.PositionVector(kwargs['point0'])
+            self._d = m3d.PositionVector(kwargs['point1']) - self._p
         elif 'points' in kwargs:
             self.fit_points(kwargs['points'])
         else:
             raise Exception(
-                'Can not create Line object on given arguments: "{}"'
-                .format(kwargs))
+                self.__class__.__name__ +
+                f'Can not create Line object on arguments "{args}" ' +
+                f'and kw-arguments "{kwargs}"')
         # Create the unit direction vector
         self._ud = self._d.normalized
 
     def __repr__(self):
-        return '<Line: p=[{:.3f}, {:.3f}, {:.3f}] ud=[{:.3f}, {:.3f}, {:.3f}]>'.format(
-            *tuple(self._p), *tuple(self._ud))
+        return ('<Line: p=[{:.3f}, {:.3f}, {:.3f}] ' +
+                'ud=[{:.3f}, {:.3f}, {:.3f}]>').format(
+                    *tuple(self._p), *tuple(self._ud))
 
     @property
     def point(self):
-        return m3d.Vector(self._p)
+        return self._p.copy()
 
     @property
     def direction(self):
-        return m3d.Vector(self._d)
+        return self._d.copy()
 
     @property
     def unit_direction(self):
-        return m3d.Vector(self._ud)
+        return self._ud.copy()
+
+    ud = unit_direction
+    
+    def __rmul__(self, trf: m3d.Transform):
+        """Return a new line transformed to new coordinate reference as given
+        by 'trf'.
+        """
+        return Line(trf * self._p, trf * self._d)
 
     def fit_points(self, points):
         """Compute the line from a set of points. 'points'
         must be an array of row position vectors, such that
         points[i] is a position vector."""
         points = np.array(points)
         centre = np.sum(points, axis=0)/len(points)
         eigen = np.linalg.eig(np.cov(points.T))
         max_ev_i = np.where(eigen[0] == max(eigen[0]))[0][0]
         direction = eigen[1].T[max_ev_i]
-        self._p = m3d.Vector(centre)
-        self._d = self._ud = m3d.Vector(direction)
+        self._p = m3d.PositionVector(centre)
+        self._d = self._ud = m3d.FreeVector(direction)
 
     @classmethod
     def new_fitted_points(cls, points):
         return cls(points=points)
 
-    def projected_point(self, p):
+    def projected_point(self, p: m3d.PositionVector):
         """Return the projection of 'p' onto this line."""
         p2p = (self._p - p)
         return p + p2p - (self._ud * p2p) * self._ud
 
-    def projected_line(self, line):
+    def projected_line(self, line: 'Line'):
         """Return the projection of 'line' onto this line. I.e. return the
         point in this line, closest to 'line'. If the lines are
-        parallel, the origin point of this line is returned. The
-        'use_plane' argument flags for using the Plane class
-        implementation for implementation simplicity.  See
+        parallel, the origin point of this line is returned. See
         https://en.wikipedia.org/wiki/Skew_lines#Nearest_Points.
         """
         # Check if the lines are parallel
         if (1 - self._ud * line._ud) < 10 * m3d.utils.eps:
+            # Return any point on the line
             return self.point
-        # https://en.wikipedia.org/wiki/Skew_lines#Nearest_Points
         p1 = self._p
         p2 = line._p
         d1 = self._ud
         d2 = line._ud
         n2 = d2.cross(d1.cross(d2))
         return p1 + ((p2-p1) * n2 / (d1 * n2)) * d1
 
     def nearest_points(self, line):
         """Return the pair of closest points on this line and 'line'. The
         first of the returned points is on this line. See
         https://en.wikipedia.org/wiki/Skew_lines#Nearest_Points
-        """ 
-           # Check if the lines are parallel
+        """
+        # Check if the lines are parallel
         if (1 - self._ud * line._ud) < 10 * m3d.utils.eps:
             return self.point
         # https://en.wikipedia.org/wiki/Skew_lines#Nearest_Points
         p1 = self._p
         p2 = line._p
         d1 = self._ud
         d2 = line._ud
@@ -136,19 +173,24 @@
                 p2 + ((p1-p2) * n1 / (d2 * n1)) * d2)
 
 
 def _test():
     # Simple test of projected line.
     l1 = Line(point=(0, 1, 1), direction=(0, 0.1, 1))
     l2 = Line(point=(1, 1, 0.1), direction=(0, 1, 0))
+    print(f'Line 1: {l1}')
+    print(f'Line 2: {l2}')
+    nps = l1.nearest_points(l2)
+    print(f'Nearest points: {nps}')
     pl = l1.projected_line(l2)
     # print('Projected line: {}'.format(str(pl)))
     assert((pl-l1.projected_point(pl))
            .length < 10 * m3d.utils.eps)
     # Test line fitting.
     fl = Line.new_fitted_points([[1, 1, 1],
                                  [2, 2, 2],
                                  [3, 3, 3]])
-    # print('Fitted line: {}'.format(str(fl)))
-    assert(fl.point == m3d.Vector(2, 2, 2))
-    assert(1.0 - np.abs(fl.direction * m3d.Vector(1, 1, 1).normalized)
+    print('Fitted line: {}'.format(str(fl)))
+    print(f'fl.point: {fl.point}')
+    assert(fl.point == m3d.PositionVector(2, 2, 2))
+    assert(1.0 - np.abs(fl.direction * m3d.FreeVector(1, 1, 1).normalized)
            < 10 * m3d.utils.eps)
```

### Comparing `math3d-3.4.1/math3d/geometry/plane.py` & `math3d-4.0.0/math3d/geometry/plane.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # coding=utf-8
 
 """
 Module for Plane class.
 """
 
 __author__ = "Morten Lind"
-__copyright__ = "Morten Lind 2013-2019"
+__copyright__ = "Morten Lind 2013-2021"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
 __email__ = "morten@lind.fairuse.org"
 __status__ = "Development"
 
 
 import math3d as m3d
 import numpy as np
 
 from .. import utils
 
 
-class Plane(object):
-    def __init__(self, **kwargs):
+class Plane:
+    def __init__(self, *args, **kwargs):
         """Create a plane representation by one of the following named
         arguments:
+        
+        * Two arguments of type FreeVector (normal) and PositionVector
+          (point).
 
         * 'plane_vector': A normalized plane vector. The normal will
         be pointing away from the origo. If kw-argument 'origo_inside'
         is given, this will determine the direction of the plane
         normal; otherwise origo will be set inside.
 
         * 'pn_pair': An ordered sequence for creating a reference
@@ -41,57 +44,82 @@
 
         The internal representation is point and normal. If given as a
         pn_pair, A boolean, 'origo_inside', is held to decide the
         direction of the normal vector, such that the origo of the
         defining coordinate system is on the inside when true.
         """
 
-        self._origo_inside = kwargs.get('origo_inside', True)
-        if 'plane_vector' in kwargs:
-            pv = m3d.Vector(kwargs['plane_vector'])
-            (self._p, self._n) = self.pv_to_pn(pv)
-        elif 'pn_pair' in kwargs:
-            (self._p, self._n) = [m3d.Vector(e) for e in kwargs['pn_pair']]
-            # # Override a given origo inside.
-            self._origo_inside = (self._p * self._n) > 0
-            # Ensure unit normal
-            #self._n.normalize()
-            # Make point a 'minimal' point on the plane, i.e. the
-            # projection of origo in the plane.
-            self._p = (self._p * self._n) * self._n
-        elif 'points' in kwargs:
-            self.fit_points(kwargs['points'])
-        elif 'coeffs' in kwargs:
-            self.coeffs = kwargs['coeffs']
-        else:
+        if len(args) == 2:
+            if(isinstance(args[0], m3d.PositionVector)
+               and isinstance(args[1], m3d.FreeVector)):
+                self._p = m3d.PositionVector(args[0])
+                self._n = m3d.FreeVector(args[1]).normalized
+            elif(isinstance(args[1], m3d.PositionVector)
+                 and isinstance(args[0], m3d.FreeVector)):
+                self._p = m3d.PositionVector(args[1])
+                self._n = m3d.FreeVector(args[0]).normalized
+            else:
+                raise Exception(
+                    'Plane.__init__: When give positional arguments, exactly ' +
+                    ' two must be given and types must be one FreeVector and ' +
+                    f'one PositionVector! Was given {args}')
+        elif len(args) != 0:
             raise Exception(
-                'Plane.__init__ : Must have either of constructor ' +
-                'kw-arguments: "plane_vector", "pn_pair", or ' +
-                '"points". Neither given!')
+                'Plane.__init__: When give positional arguments, exactly ' +
+                ' two must be given and types must be one FreeVector and ' +
+                f'one PositionVector! Was given {args}')
+        else:
+            self._origo_inside = kwargs.get('origo_inside', True)
+            if 'plane_vector' in kwargs:
+                pv = m3d.Vector(kwargs['plane_vector'])
+                (self._p, self._n) = self.pv_to_pn(pv)
+            elif 'pn_pair' in kwargs:
+                pn_pair = kwargs['pn_pair']
+                self._p = m3d.PositionVector(pn_pair[0])
+                self._n = m3d.FreeVector(pn_pair[1]).normalized
+                # Override a given origo inside.
+                self._origo_inside = (self._p * self._n) > 0
+                # Make point a 'minimal' point on the plane, i.e. the
+                # projection of origo in the plane.
+                self._p = m3d.PositionVector((self._p * self._n) * self._n)
+            elif 'points' in kwargs:
+                self.fit_points(kwargs['points'])
+            elif 'coeffs' in kwargs:
+                self.coeffs = kwargs['coeffs']
+            else:
+                raise Exception(
+                    'Plane.__init__ : Must have either of constructor ' +
+                    'kw-arguments: "plane_vector", "pn_pair", or ' +
+                    '"points". Neither given!')
 
     def copy(self):
         return Plane(pn_pair=(self._p, self._n))
 
     def __repr__(self):
-        return '<Plane: [{:.5f}, {:.5f}, {:.5f}]>'.format(
-            *tuple(self.plane_vector.array))
+        return ('<Plane: p=[{:.3f}, {:.3f}, {:.3f}] ' +
+                'un=[{:.3f}, {:.3f}, {:.3f}]>').format(
+                    *tuple(self._p), *tuple(self._n))
+
+    # def __repr__(self):
+    #     return '<Plane: [{:.5f}, {:.5f}, {:.5f}]>'.format(
+    #         *tuple(self.plane_vector.array))
 
     def __rmul__(self, transf):
         """Support transformation of this plane to another coordinate
         system by multiplication of an m3d.Transform from left."""
         if type(transf) != m3d.Transform:
             return NotImplemented
-        tnormal = transf.orient * self._n
+        tnormal = transf * self._n
         tpoint = transf * self._p
         return Plane(pn_pair=(tpoint, tnormal))
 
-    def dist(self, p):
+    def dist(self, p: m3d.PositionVector):
         """Signed distance to a point, measured positive along the
         normal vector direction."""
-        return (m3d.Vector(p) - self._p) * self._n
+        return (m3d.PositionVector(p) - self._p) * self._n
 
     def get_plane_vector(self):
         return self.pn_to_pv(self._p, self._n)
 
     def set_plane_vector(self, pv):
         (self._p, self._n) = self.pv_to_pn(pv)
 
@@ -132,56 +160,55 @@
         must be an array of row position vectors, such that
         points[i] is a position vector."""
         points = np.array(points)
         centre = np.sum(points, axis=0)/len(points)
         eigen = np.linalg.eig(np.cov(points.T))
         min_ev_i = np.where(eigen[0] == min(eigen[0]))[0][0]
         normal = eigen[1].T[min_ev_i]
-        (self._p, self._n) = (m3d.Vector(centre), m3d.Vector(normal))
+        (self._p, self._n) = (m3d.PositionVector(centre), m3d.FreeVector(normal))
 
     @classmethod
     def new_fitted_points(cls, points):
         return cls(points=points)
 
     def fit_plane(self, points):
         print('Deprecation warning: fit_plane -> fit_points')
         self.fit_points(points)
 
     @classmethod
     def pn_to_pv(cls, point, normal):
         """Compute the plane vector of a plane represented by a point
         and normal."""
-        if not isinstance(point, m3d.Vector):
-            point = m3d.Vector(point)
-        if not isinstance(normal, m3d.Vector):
-            normal = m3d.Vector(normal)
-        normal.normalize()
+        if not isinstance(point, m3d.PositionVector):
+            point = m3d.PositionVector(point)
+        if not isinstance(normal, m3d.FreeVector):
+            normal = m3d.FreeVector(normal)
+        un = normal.normalized
         # Origo projection on plane
-        p0 = (point * normal) * normal
+        p0 = (point * un) * un
         # Square of offset from origo
         d2 = p0.length_squared
         # return the plane vector
-        return p0 / (d2)
+        return m3d.Vector(p0 / d2)
 
-    def pv_to_pn(self, pv):
+    @classmethod
+    def pv_to_pn(cls, pv):
         """Calculate a point-normal representation of the plane
         described by the given plane vector."""
         if isinstance(pv, m3d.Vector):
             pv = m3d.Vector(pv)
         d = pv.length
-        n = pv / pv.length
-        p = n / d
-        if not self._origo_inside:
-            n = -n
+        n = m3d.FreeVector(pv / d)
+        p = m3d.PositionVector(n / d)
         return (p, n)
 
     def projection(self, point):
         """Return the projection of the 'point' on the plane."""
-        if isinstance(point, m3d.Vector):
-            point = m3d.Vector(point)
+        if isinstance(point, m3d.PositionVector):
+            point = m3d.PositionVector(point)
         return point - self._n * (point - self._p) * self._n
 
     def line_intersection(self, line):
         """Compute the intersection with the given 'line'. If the line is
         parallel to the plane, None is returned, irregardless of
         whether the line is lying in the plane. See
         http://geomalgorithms.com/a05-_intersect-1.html. In-line
```

### Comparing `math3d-3.4.1/math3d/interpolation/se3interpolation.py` & `math3d-4.0.0/math3d/interpolation/se3interpolator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # coding=utf-8
 
 """
 Module implementing the SE(3) interpolator class.
 """
 
 __author__ = "Morten Lind"
-__copyright__ = "Morten Lind 2009-2018"
+__copyright__ = "Morten Lind 2009-2021"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Production"
 
-from ..transform import Transform
+
+import typing
+
+from ..transform import Transform, PoseVector
 from .. import utils
-from .so3interpolation import SO3Interpolation
-from .r3interpolation import R3Interpolation
+from .so3interpolator import SO3Interpolator
+from .e3interpolator import E3Interpolator
+from .interpolator import Interpolator
 
 
-class SE3Interpolation(SO3Interpolation, R3Interpolation):
+class SE3Interpolator(Interpolator):
     """A class for object representing a linear interpolation in task
     space, SE(3), between two points. Interpolation is done from one
     configuration, trf0, to another, trf1. trf0 and trf1 can be given
     as Transform objects."""
 
     class Error(Exception):
         """Exception class."""
@@ -30,40 +34,64 @@
         def __init__(self, message):
             self.message = 'SE3Interpolation Error: ' + message
             Exception.__init__(self, self.message)
 
         def __repr__(self):
             return self.message
 
-    def __init__(self, trf0, trf1, shortest=True):
+    def __init__(self,
+                 trf0: typing.Union[Transform, PoseVector],
+                 trf1: typing.Union[Transform, PoseVector],
+                 shortest: bool = True,
+                 t_range: tuple[float, float] = None,
+                 v0: float = None):
         """Initialise an SE(3) interpolation from transform 'trf0' to
         transform 'trf1'. If 'shortest' is True, the shortest rotation
         path is chosen, if False, the long rotation is used, and if
         None it is indeterminate, given by the Versor objects being
         constructed from the transforms.
         """
-        self._trf0 = trf0
-        self._trf1 = trf1
-        SO3Interpolation.__init__(self, self._trf0.orient,
-                                  self._trf1.orient, shortest)
-        R3Interpolation.__init__(self, self._trf0.pos, self._trf1.pos)
+        Interpolator.__init__(self, t_range)
+        self._trf0 = Transform(trf0)
+        self._trf1 = Transform(trf1)
+        self._so3i = SO3Interpolator(self._trf0.orient,
+                                     self._trf1.orient,
+                                     shortest=shortest,
+                                     t_range=None)
+        self._v0 = v0
+        self._e3i = E3Interpolator(self._trf0.pos, self._trf1.pos,
+                                   t_range=None,
+                                   v0=None)
+
+    def _s(self, t, checkrange=True):
+        """Special calculus for path parameter possibly taking acceleration
+        into account.
+        """
+        if self._v0 is None:
+            return super()._s(t, checkrange)
+        else:
+            t_path = t - self._t_range[0]
+            s = (self._v0 * t_path + 0.5 * self._acc *
+                 t_path**2) / self._e3i._dlength
+            if checkrange:
+                super()._checkrange(s)
+            return s
 
-    def __call__(self, time, checkrange=True):
+    def __call__(self, t, checkrange=True):
         """Class callable method for giving the transform at time
-        'time'; in [0,1]."""
-        if checkrange:
-            time = utils.flt(time)
-            if time < 0.0 or time > 1.0:
-                raise self.Error('"time" must be number in [0.0 ; 1.0]. ' +
-                                 'It was {}.'.format(time))
-        return Transform(self.orient(time, False), self.pos(time, False))
+        't'; in [0,1] or in 't_range'."""
+        # Use the R3 interpolator for handling the acceleration if any
+        s = self._s(t, checkrange)
+        return Transform(self._so3i.orient(s, checkrange=checkrange),
+                         self._e3i.pos(s, checkrange=checkrange))
 
 
-TaskLinearInterpolation = SE3Interpolation
-EuclideanInterpolation = SE3Interpolation
+SE3Interpolation = SE3Interpolator
+TaskLinearInterpolation = SE3Interpolator
+EuclideanInterpolation = SE3Interpolator
 
 
 def _test():
     """Simple test function."""
     global o0, o1, tint, p0, p1
     from math3d.orientation import Orientation
     from math3d.vector import Vector
```

### Comparing `math3d-3.4.1/math3d/interpolation/so3interpolation.py` & `math3d-4.0.0/math3d/interpolation/so3interpolator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,95 @@
 # coding=utf-8
 
 """
 Module implementing the SO(3) interpolator class; Slerp.
 """
 
 __author__ = "Morten Lind"
-__copyright__ = "Morten Lind 2009-2018"
+__copyright__ = "Morten Lind 2009-2021"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Production"
 
+
+import typing
+
 import numpy as np
 
-from ..orientation import Orientation
-from ..quaternion import Versor, UnitQuaternion
+from ..orientation import Orientation, RotationVector
+from ..quaternion import Versor
 from .. import utils
+from .interpolator import Interpolator
 
 
-class SO3Interpolation(object):
+class SO3Interpolator(Interpolator):
     """A SLERP interpolator class in SO(3)."""
 
     class Error(Exception):
         """Exception class."""
 
         def __init__(self, message):
             self.message = 'SO3Interpolation Error: ' + message
             Exception.__init__(self, self.message)
 
         def __repr__(self):
             return self.message
 
-    def __init__(self, start, end, shortest=True):
+    def __init__(self,
+                 start: typing.Union[Orientation, Versor, RotationVector],
+                 end: typing.Union[Orientation, Versor, RotationVector],
+                 t_range: tuple[float, float] = None,
+                 shortest: bool = True):
         """Initialise an SO(3) interpolation from orientation 'start' to
-        orientation 'end'. If 'shortest' is True the shortest rotation
-        path is chosen, if False the long rotation is used, and if
-        None it is indeterminate, given by the Versor objects
-        constructed over 'start' and 'end'.
+        orientation 'end'. If t_range is given, it must be a time
+        interval in form of a sorted pair of floats. If 'shortest' is
+        True the shortest rotation path is chosen, if False the long
+        rotation is used, and if None it is indeterminate, given by
+        the Versor objects constructed over 'start' and 'end'.
         """
+        Interpolator.__init__(self, t_range)
         self._qstart = Versor(start)
         self._qend = Versor(end)
         self._qstart.normalize()
         self._qend.normalize()
         if shortest is not None:
             if shortest and (self._qstart.dist(self._qend) >
                              self._qstart.dist(-self._qend)):
                 self._qend = -self._qend
             elif not shortest and (self._qstart.dist(self._qend) <
                                    self._qstart.dist(-self._qend)):
                 self._qend = -self._qend
         self._qstartconj = self._qstart.conjugated.normalized
         self._qstartconjqend = (self._qstartconj * self._qend).normalized
 
-    def __call__(self, t):
-        return self.versor(t)
+    def __call__(self, t, checkrange=True):
+        return self.versor(t, checkrange)
 
-    def versor(self, time, checkrange=True):
+    def versor(self, t, checkrange=True):
         """Return the versor of the slerp at 'time'; in [0,1]."""
-        if checkrange:
-            time = utils.flt(time)
-            if time < 0.0 or time > 1.0:
-                raise self.Error('"time" must be number in [0.0 ; 1.0]. ' +
-                                 'I was {}'.format(time))
-        return self._qstart * (self._qstartconjqend) ** time
+        return self._qstart * (self._qstartconjqend) ** self._s(t, checkrange)
 
     def orient(self, time, checkrange=True):
         """Return the orientation in the slerp at 'time'; in [0,1]. """
         return self.versor(time, checkrange).orientation
 
 
-SLERP = SO3Interpolation
-OrientationInterpolation = SO3Interpolation
+SO3Interpolation = SO3Interpolator
+SLERP = SO3Interpolator
+OrientationInterpolation = SO3Interpolator
 
 
 def _test():
     """Simple test function."""
     global o, o1, q, q1, osl, qsl
     from math import pi
     o = Orientation()
     o.set_to_x_rotation(pi / 2)
     o1 = Orientation()
     o1.set_to_z_rotation(pi / 2)
     q = Versor(o)
     q1 = Versor(o1)
-    qsl = SO3Interpolation(q, q1)
-    osl = SO3Interpolation(o, o1)
+    qsl = SO3Interpolator(q, q1)
+    osl = SO3Interpolator(o, o1)
+    print(osl(0.5), qsl(0.5))
```

### Comparing `math3d-3.4.1/math3d/orientation.py` & `math3d-4.0.0/math3d/orientation.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,29 +2,104 @@
 
 """
 Module implementing the Orientation class. The orientation is
 represented internally by an orthogonal 3x3 matrix.
 """
 
 __author__ = "Morten Lind"
-__copyright__ = "Morten Lind 2012-2019"
+__copyright__ = "Morten Lind 2012-2021"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
 __email__ = "morten@lind.fairuse.org"
 __status__ = "Production"
 
 import numpy as np
 
 # Circular dependencies prevents direct import of Versor, hence
 # global addressing.
 import math3d as m3d
 
 from . import utils
-from .vector import Vector
+from .vector import Vector, FreeVector
+
+
+class RotationVector:  # (np.ndarray):
+    class Error(Exception):
+        def __init__(self, message):
+            self.message = message
+            Exception.__init__(self, self.message)
+
+        def __repr__(self):
+            return self.__class__.__qualname__ + ': ' + self.message
+
+    def __init__(self, *args, **kwargs):
+        self._data = np.zeros(3)
+        if len(args) > 0:
+            # args take precedence
+            if len(args) == 1:
+                # Take three numbers
+                if type(args[0]) in (Vector, FreeVector, RotationVector):
+                    self._data[:] = args[0]._data
+                elif len(args[0]) == 3:
+                    self._data[:] = args[0]
+                else:
+                    raise self.Error('Given one positional argument which ' +
+                                     f'was not of length three: {args[0]}')
+            elif len(args) == 3:
+                self._data[:] = args
+            else:
+                raise self.Error(f'Can not create on {len(args)} ' +
+                                 'positional arguments')
+
+    def __repr__(self):
+        return ('<RotVec: ({:.5f}, {:.5f}, {:.5f})>'
+                .format(*self._data))
+
+    def copy(self):
+        return self.__class__(self._data.copy())
+
+    def get_length_squared(self):
+        """Return the square of the standard Euclidean length."""
+        return self._data @ self._data
+
+    length_squared = property(get_length_squared)
+
+    def get_length(self):
+        """Return the Euclidean length."""
+        return np.sqrt(self.length_squared)
+
+    length = property(get_length)
+
+    def get_array(self):
+        """Return a copy of the ndarray which is the fundamental data
+        of the Vector."""
+        return self._data.copy()
+
+    def set_array(self, array, check=True):
+        """Set the vector by three values in the iterable 'array'.
+        """
+        if check and len(array) != 3:
+            raise utils.Error(
+                self.__class__.__name__ +
+                'Setting the value by the "array" property needs exactly'
+                + ' three values. ({} were given)'.format(len(array)))
+        self._data[:] = array
+
+    array = property(get_array, set_array)
+
+    def get_array_ref(self):
+        """Return a reference to the (3,)-ndarray, which is the
+        fundamental data of the RotationVector.  Caution: Use this method
+        only for optimization, since it eliminates copying, and be
+        sure not to compromize the data.
+        """
+        return self._data
+
+    array_ref = property(get_array_ref)
 
 
 class Orientation(object):
     """An Orientation is a member of SO(3) which can be used either to
     perform a rotational transformation, or for keeping an orientation
     in 3D.
     """
@@ -47,43 +122,47 @@
                               '(3,), (9,) or (3,3)!')
 
     def __init__(self, *args):
         """Create an orientation on either of the following arguments:
 
         * An Orientation.
 
-        * A Versor (UnitQuaternion).
+        * A RotationVector
+
+        * A Versor
 
-        * Three Vectors or numpy arrays of shape (3,) interpreted as
+        * Three FreeVectors or numpy arrays of shape (3,) interpreted as
           columns of the matrix.
 
-        * One Vector, numpy array, list, or tuple of shape (3,)
+        * One FreeVector, numpy array, list, or tuple of shape (3,)
           interpreted as a rotation vector.
 
         * A numpy array, list, or tuple of shape (3,3) or (9,) for
           giving direct matrix data; using row major order.
         """
         if len(args) == 1:
             arg = args[0]
             if type(arg) == Orientation:
                 self._data = arg.array
-            elif type(arg) in (m3d.Versor, m3d.UnitQuaternion):
+            elif type(arg) == m3d.Versor:
                 self._data = arg.orientation._data
-            elif type(arg) == Vector:
+            elif type(arg) in [FreeVector, RotationVector]:
+                if type(arg) == FreeVector:
+                    utils._deprecation_warning('RotationVector')
                 # Interpret as a rotation vector
                 self._data = np.identity(3)
                 self.rotation_vector = arg
             elif utils.is_sequence(arg):
                 self.__create_on_sequence(arg)
             else:
                 raise utils.Error(
                     'Creating on type {} is not supported'
                     .format(str(type(arg))))
         elif len(args) == 3:
-            if np.all(np.array([type(a) == Vector for a in args])):
+            if np.all(np.array([type(a) == FreeVector for a in args])):
                 array_args = (a._data for a in args)
             elif np.all(np.array([type(a) == np.ndarray for a in args])):
                 array_args = args
             else:
                 raise utils.Error(
                     'Creating on three arguments requires three vectors ' +
                     'or three numpy arrays of shape (3,)!')
@@ -109,48 +188,48 @@
         if other is None:
             return Orientation(self)
         else:
             self._data[:, :] = other._data
 
     def get_vec_x(self):
         """Return the x-direction of the moving coordinate system in
-        base reference as a Vector.
+        base reference as a FreeVector.
         """
-        return Vector(self._data[:, 0])
+        return FreeVector(self._data[:, 0])
 
     vec_x = property(get_vec_x)
 
     def get_col_x(self):
         """Return the x-direction of the moving coordinate system in
         base reference as an array."""
         return self._data[:, 0]
 
     col_x = property(get_col_x)
 
     def get_vec_y(self):
         """Return the y-direction of the moving coordinate system in
-        base reference as a Vector.
+        base reference as a FreeVector.
         """
-        return Vector(self._data[:, 1])
+        return FreeVector(self._data[:, 1])
 
     vec_y = property(get_vec_y)
 
     def get_col_y(self):
         """Return the y-direction of the moving coordinate system in
         base reference as an array.
         """
         return self._data[:, 1]
 
     col_y = property(get_col_y)
 
     def get_vec_z(self):
         """Return the z-direction of the moving coordinate system in
-        base reference as a Vector.
+        base reference as a FreeVector.
         """
-        return Vector(self._data[:, 2])
+        return FreeVector(self._data[:, 2])
 
     vec_z = property(get_vec_z)
 
     def get_col_z(self):
         """Return the z-direction of the moving coordinate system in
         base reference as an array.
         """
@@ -190,69 +269,70 @@
     repr_error = property(get_repr_error)
 
     def orthonormalize(self):
         """Perform an in-place Gram-Schmidt."""
         # Trust the x-vector but normalize
         self._data[:, 0] /= np.linalg.norm(self._data[:, 0])
         # Form y-vector by removing x-projection and normalizing
-        self._data[:, 1] -= np.dot(self._data[:, 1], self._data[:, 0]) * self._data[:, 0]
+        self._data[:, 1] -= (self._data[:, 1] @
+                                   self._data[:, 0]) * self._data[:, 0]
         self._data[:, 1] /= np.linalg.norm(self._data[:, 1])
         # Form z-vector by cross product #  and normalization
         self._data[:, 2] = np.cross(self._data[:, 0], self._data[:, 1])
         # self._data[:, 2] /= np.linalg.norm(self._data[:, 2])
 
     # def renormalize(self):
     #     """Correct the axis vectors by a Gram-Schmidt procedure."""
     #     colx = self._data[:,0]
     #     coly = self._data
 
     def from_xy(self, x_vec, y_vec):
         """Reset this orientation to the one that conforms with the
         given x and y directions.
         """
-        if type(x_vec) != m3d.Vector:
-            x_vec = m3d.Vector(x_vec)
-        if type(y_vec) != m3d.Vector:
-            y_vec = m3d.Vector(y_vec)
+        if type(x_vec) != FreeVector:
+            x_vec = FreeVector(x_vec)
+        if type(y_vec) != FreeVector:
+            y_vec = FreeVector(y_vec)
         x_vec = x_vec.normalized
         y_vec = y_vec.normalized
         if np.abs(x_vec * y_vec) > utils.eps:
             print('Warning: Orthonormalizing y_vec on x_vec!')
             y_vec -= (x_vec * y_vec) * x_vec
             y_vec.normalize()
         self._data[:, 0] = x_vec._data
         self._data[:, 1] = y_vec._data
         self._data[:, 2] = x_vec.cross(y_vec)._data
 
     def from_xz(self, x_vec, z_vec):
         """Reset this orientation to the one that conforms with the
         given x and z directions.
         """
-        if type(x_vec) != m3d.Vector:
-            x_vec = m3d.Vector(x_vec)
-        if type(z_vec) != m3d.Vector:
-            z_vec = m3d.Vector(z_vec)
+        if type(x_vec) != FreeVector:
+            x_vec = FreeVector(x_vec)
+        if type(z_vec) != FreeVector:
+            z_vec = FreeVector(z_vec)
         x_vec = x_vec.normalized
         z_vec = z_vec.normalized
         if np.abs(x_vec * z_vec) > utils.eps:
             print('Warning: Orthonormalizing z_vec on x_vec!')
             z_vec -= (x_vec * z_vec) * x_vec
             z_vec.normalize()
         self._data[:, 0] = x_vec._data
         self._data[:, 1] = z_vec.cross(x_vec)._data
         self._data[:, 2] = z_vec._data
 
     def from_yz(self, y_vec, z_vec):
         """Reset this orientation to the one that conforms with the
         given x and z directions.
         """
-        if type(y_vec) != m3d.Vector:
-            y_vec = m3d.Vector(y_vec)
-        if type(z_vec) != m3d.Vector:
-            z_vec = m3d.Vector(z_vec)
+        if type(y_vec) != FreeVector:
+            y_vec = FreeVector(y_vec)
+        if type(z_vec) != FreeVector:
+            z_vec = FreeVector(z_vec)
         y_vec = y_vec.normalized
         z_vec = z_vec.normalized
         if np.abs(y_vec * z_vec) > utils.eps:
             print('Warning: Orthonormalizing z_vec on x_vec!')
             z_vec -= (y_vec * z_vec) * y_vec
             z_vec.normalize()
         self._data[:, 0] = y_vec.cross(z_vec)._data
@@ -279,85 +359,93 @@
 
     versor = property(get_versor, set_versor)
 
     # Deprecated
     unit_quaternion = versor
     quaternion = unit_quaternion
 
-    def get_rotation_vector(self):
-        """Return a rotation vector representing this
-        orientation. This is essentially the logarithm of the rotation
-        matrix. """
+    def get_logarithm(self):
+        """Return a rotation vector representing this orientation. This is
+        essentially the logarithm of the rotation matrix.
+        """
         return self.versor.rotation_vector
 
-    def set_rotation_vector(self, rot_vec):
-        """Set this Orientation to represent the one given in a
-        rotation vector in 'rot_vec'. 'rot_vec' must be a Vector or an
-        numpy array of shape (3,)."""
-        if type(rot_vec) == Vector:
-            rot_vec = rot_vec.array
-        angle = np.linalg.norm(rot_vec)
-        if np.abs(angle) < utils.eps:
+    # Deprecated
+    get_rotation_vector = get_logarithm
+
+    def set_logarithm(self, rot_vec):
+        """Set this Orientation to represent the one given in a rotation
+        vector in 'rot_vec'. 'rot_vec' must be a FreeVector or an
+        numpy array of shape (3,).
+        """
+        if type(rot_vec) not in (FreeVector, RotationVector):
+            rot_vec = RotationVector(rot_vec)
+        angle = rot_vec.length
+        if np.isclose(angle, 0.0):
             self._data = np.identity(3)
         else:
-            axis = rot_vec / angle
+            axis = FreeVector(rot_vec._data / angle)
             self.axis_angle = (axis, angle)
 
-    rotation_vector = property(get_rotation_vector, set_rotation_vector)
+    # Deprecated
+    set_rotation_vector = set_logarithm
+
+    logarithm = log = rotation_vector = rot_vec = rv = property(get_logarithm,
+                                                                set_logarithm)
 
     def get_axis_angle(self):
         """Return an (axis,angle) pair representing the equivalent
         orientation."""
         return m3d.Versor(self).axis_angle
 
     def set_axis_angle(self, ax_ang):
         """Set this orientation to the equivalent to rotation of 'angle'
         around 'axis'. Only the direction of the 'axis' is used, so it
         may have any length greater than zero.
         """
         axis, angle = ax_ang
-        if type(axis) == Vector:
+        if type(axis) in (Vector, FreeVector):
             axis = axis.array
         # Force normalization
         axis /= np.linalg.norm(axis)
         x = axis[0]
         y = axis[1]
         z = axis[2]
         ca = np.cos(angle)
         sa = np.sin(angle)
-        self._data[:, :] = np.array([
-            [ca + (1 - ca) * x**2,
+        self._data[:, :] = np.array((
+            (ca + (1 - ca) * x**2,
              (1 - ca) * x * y - sa * z,
-             (1 - ca) * x * z + sa * y],
-            [(1 - ca) * x * y + sa * z,
+             (1 - ca) * x * z + sa * y),
+            ((1 - ca) * x * y + sa * z,
              ca + (1 - ca) * y**2,
-             (1 - ca) * y * z - sa * x],
-            [(1 - ca) * x * z - sa * y,
+             (1 - ca) * y * z - sa * x),
+            ((1 - ca) * x * z - sa * y,
              (1 - ca) * y * z + sa * x,
-             ca + (1 - ca) * z**2]])
+             ca + (1 - ca) * z**2)))
 
-    axis_angle = property(get_axis_angle, set_axis_angle)
+    axis_angle = ax_ang = aa = property(get_axis_angle, set_axis_angle)
 
     def set_to_x_rotation(self, angle):
         """Replace this orientation by that of a rotation around x."""
         ca = np.cos(angle)
         sa = np.sin(angle)
-        self._data[:, :] = np.array([[1, 0, 0], [0, ca, -sa], [0, sa, ca]])
+        self._data[:, :] = np.array(((1, 0, 0), (0, ca, -sa), (0, sa, ca)))
 
     def set_to_y_rotation(self, angle):
         """Replace this orientation by that of a rotation around y."""
         ca = np.cos(angle)
         sa = np.sin(angle)
-        self._data[:, :] = np.array([[ca, 0, sa], [0, 1, 0], [-sa, 0, ca]])
+        self._data[:, :] = np.array(((ca, 0, sa), (0, 1, 0), (-sa, 0, ca)))
 
     def set_to_z_rotation(self, angle):
         """Replace this orientation by that of a rotation around z."""
         ca = np.cos(angle)
         sa = np.sin(angle)
-        self._data[:, :] = np.array([[ca, -sa, 0], [sa, ca, 0], [0, 0, 1]])
+        self._data[:, :] = np.array(((ca, -sa, 0), (sa, ca, 0), (0, 0, 1)))
 
     def rotate_t(self, axis, angle):
         """In-place rotation of this orientation angle radians in axis
         perceived in the transformed reference system.
         """
         o = Orientation()
         o.axis_angle = (axis, angle)
@@ -422,15 +510,17 @@
         z axis in the transformed reference system. (Inefficient!)
         """
         self.rotate_t(Vector.e2, angle)
 
     rotate_z = rotateZ = rotateZT = rotate_zt
 
     def __repr__(self):
-        return '<Orientation: \n' + repr(self._data) + '>'
+        # return '<Orientation: \n' + repr(self._data) + '>'
+        rvr = self.rot_vec.array_ref
+        return f'<Orientation: RV({rvr[0]:.3f}, {rvr[1]:.3f}, {rvr[2]:.3f})>'
 
     def __str__(self):
         return self.__repr__()
 
     def get_ang_norm(self):
         """Return the angular norm, i.e. the angular rotation, of
         this orientation."""
@@ -452,38 +542,42 @@
         """Return an inverse of this orientation as a rotation."""
         o = Orientation(self._data)
         o.invert()
         return o
 
     inverse = property(get_inverse)
 
-    def __mul__(self, other):
-        if type(other) == Vector:
-            return Vector(np.dot(self._data, other._data))
+    def __matmul__(self, other):
+        if type(other) == FreeVector:
+            return FreeVector(self._data @ other._data)
         elif type(other) == Orientation:
-            return Orientation(np.dot(self._data, other._data))
-        elif type(other) in (m3d.Versor, m3d.UnitQuaternion):
+            return Orientation(self._data @ other._data)
+        elif type(other) == m3d.Versor:
             return self * other.orientation
-        elif type(other) == np.ndarray and other.shape == (3,):
-            return np.dot(self._data, other)
-        elif type(other) == np.ndarray and other.shape == (6,):
-            # Individually transfor two appended free vectors,
-            # e.g. twists or wrenches
-            return self._data.dot(
-                other.reshape((3, 2), order='F')
-                ).reshape(6, order='F')
+        elif type(other) == RotationVector:
+            return RotationVector(self._data @ other._data)
+        elif isinstance(other, np.ndarray):
+            if other.shape == (3,):
+                return self._data @ other
+            elif other.shape == (6,):
+                # Individually transfor two appended free vectors,
+                # e.g. twists or wrenches
+                return (self._data @ other.reshape((3, 2), order='F')
+                        ).reshape(6, order='F')
         # elif utils.is_sequence(other):
         #     # Assume a sequence of objects that may be multiplied
         #     return [self * o for o in other]
         else:
             return NotImplemented
             # raise utils.Error('Multiplication by something other than'
-            #                  + 'Orientation, Vector, or a sequence '
+            #                  + 'Orientation, FreeVector, or a sequence '
             #                  + 'of these, is not allowed!')
 
+    __mul__ = __matmul__
+
     def get_matrix(self):
         """Return an np-matrix with the data from the orientation.
         """
         return np.matrix(self._data)
 
     matrix = property(get_matrix)
 
@@ -588,48 +682,50 @@
 
     # // The Euler encoding map is used to easily apply rotations
     # according the the 'xyzXYZ' encoding scheme for Euler angles
     _euler_encoding_map = {'x': rotate_xb, 'y': rotate_yb, 'z': rotate_zb,
                            'X': rotate_xt, 'Y': rotate_yt, 'Z': rotate_zt}
 
     @classmethod
-    def new_vec_to_vec(cls, from_vec, to_vec):
+    def new_from_vec_to_vec(cls, from_vec, to_vec):
         """Factory for a new orientation which is the minimal rotation which
         rotates 'from_vec' to 'to_vec'. Technically the axis-angle
         that can be computed for the two vectors.
         """
         # Ensure that the vectors are m3d unit vectors
-        from_vec = m3d.Vector(from_vec).normalized
-        to_vec = m3d.Vector(to_vec).normalized
+        from_vec = FreeVector(from_vec).normalized
+        to_vec = FreeVector(to_vec).normalized
         # Angle between the vectords
         angle = from_vec.angle(to_vec)
         # Consider cases
         if angle <= utils.sqrt_eps:
             # // Identity
             return Orientation()
         elif angle < np.pi - utils.sqrt_eps:
             # // Regular, minimal rotation
             return Orientation(angle * from_vec.cross(to_vec).normalized)
         else:
             # // Find any suitable rotation axis
-            x_angle = Vector.ex.angle(from_vec)
+            x_angle = FreeVector.ex.angle(from_vec)
             if x_angle > 1e-3 and x_angle < np.pi - 1.0e-3:
                 return Orientation(angle *
-                                   Vector.ex.cross(from_vec).normalized)
-            y_angle = Vector.ey.angle(from_vec)
+                                   FreeVector.ex.cross(from_vec).normalized)
+            y_angle = FreeVector.ey.angle(from_vec)
             if y_angle > 1e-3 and y_angle < np.pi - 1.0e-3:
                 return Orientation(angle *
-                                   Vector.ey.cross(from_vec).normalized)
-            z_angle = Vector.ez.angle(from_vec)
+                                   FreeVector.ey.cross(from_vec).normalized)
+            z_angle = FreeVector.ez.angle(from_vec)
             if z_angle > 1e-3 and z_angle < np.pi - 1.0e-3:
                 return Orientation(angle *
-                                   Vector.ez.cross(from_vec).normalized)
+                                   FreeVector.ez.cross(from_vec).normalized)
+
+    new_vec_to_vec = new_from_vec_to_vec
 
     @classmethod
-    def new_euler(cls, angles, encoding='ZYX'):
+    def new_from_euler(cls, angles, encoding='ZYX'):
         """Factory for generating a new orientation from Euler or
         Tait-Bryan angles. 'angles' must be a sequence of three real
         numbers giving the Euler or Tait-Bryan angles. 'encoding' must
         be three characters, all from the set 'xyzXYZ'. The encoding
         denotes the sequence of axes to rotate around and the case of
         the characters in the encoding string tells if it should be
         intrinsic or extrinsic axes for the rotation; all rotations
@@ -660,14 +756,16 @@
             raise utils.Error(
                 'Rotation encoding must either be all intrinsic or extrinsic!')
         o = Orientation()
         for r, a in zip(encoding, angles):
             cls._euler_encoding_map[r](o, a)
         return o
 
+    new_euler = new_from_euler
+
     def to_euler(self, encoding):
         """The Euler angles 'encoding' follow the documentation for
         the factory method 'new_euler'. The routine is taken from Ken
         Shoemake's chapter 'Euler Angle Conversion' in 'Graphics Gems
         IV', Academic Press, 1994, ISBN 0-12-336155-9.
         """
         enc = encoding
@@ -678,17 +776,17 @@
             intrinsic = False
         else:
             raise utils.Error(
                 'Rotation encoding must either be all intrinsic or extrinsic!')
         lenc = enc.lower()
         repetition = lenc[0] == lenc[2]
         if intrinsic:
-            parity = lenc[1:] not in ['yx', 'zy', 'xz']
+            parity = lenc[1:] not in ('yx', 'zy', 'xz')
         else:
-            parity = lenc[:2] not in ['xy', 'yz', 'zx']
+            parity = lenc[:2] not in ('xy', 'yz', 'zx')
         inner = lenc[2] if intrinsic else lenc[0]
         i = 'xyz'.index(inner)
         j = (i + 1 + parity) % 3
         k = (i + 2 - parity) % 3
         # h = k if repetition else i
         m = self._data
         if repetition:
@@ -711,39 +809,43 @@
                 ax = np.arctan2(-m[j, k], m[j, j])
                 ay = np.arctan2(-m[k, i], cy)
                 az = 0.0
         if parity:
             ax, ay, az = -ax, -ay, -az
         if intrinsic:
             ax, az = az, ax
-        return np.array([ax, ay, az])
+        return np.array((ax, ay, az))
 
     @classmethod
-    def new_axis_angle(self, axis, angle):
+    def new_from_axis_angle(self, axis, angle):
         """Create and return a new orientation that rotates the given 'angle'
         (scalar) around the given 'axis' (Vector).
         """
-        if type(axis) != Vector:
-            axis = Vector(axis)
+        if type(axis) != FreeVector:
+            axis = FreeVector(axis)
         oaa = Orientation()
         oaa.axis_angle = (axis, angle)
         return oaa
 
+    new_axis_angle = new_from_axis_angle
+
     @classmethod
-    def new_rotation_vector(self, rotation_vector):
+    def new_from_rotation_vector(self, rotation_vector):
         """Create and return a new orientation that represents the given
         'rotation_vector', given as a sequence of three numbers.
         """
         return Orientation(rotation_vector)
 
+    new_rotation_vector = new_from_rotation_vector
+
 
 def _test():
     o = Orientation()
     r = Orientation()
-    o.from_xy(Vector(1, 1, 0), Vector(-1, 1, 0))
+    o.from_xy(Vector(1, 1, 0), FreeVector(-1, 1, 0))
     r.set_to_z_rotation(np.pi / 2)
     ro = r * o
     print(ro.ang_dist(r))
     print(ro.axis_angle)
 
 
 def _test_to_euler():
@@ -754,18 +856,18 @@
     oo = Orientation.new_euler(o_ang, enc)
     oo_ang = oo.to_euler(enc)
     print(np.allclose(o_ang, oo_ang))
 
 
 def _test_from_nn():
     o = Orientation.new_from_xy((1, 0, 0), (1, 1, 0))
-    if o.vec_y != m3d.Vector.ey or o.vec_x != m3d.Vector.ex:
+    if o.vec_y != FreeVector.ey or o.vec_x != FreeVector.ex:
         print('Test-Error in new_from_xy')
     o = Orientation.new_from_xz((1, 0, 0), (1, 0, 1))
-    if o.vec_z != m3d.Vector.ez or o.vec_x != m3d.Vector.ex:
+    if o.vec_z != FreeVector.ez or o.vec_x != FreeVector.ex:
         print('Test-Error in new_from_xz')
 
 
 def _test_array_property():
     o = Orientation()
     try:
         o.array = [[1, 1, 1], [0, 0, 0], [2]]
@@ -777,11 +879,11 @@
     o.orthonormalize()
     print(o.repr_error)
 
 
 # def _test_vectorized_multiplication():
 #     # Test multiplication of a list
 #     o = Orientation.new_rot_z(np.pi/2)
-#     vs = [Vector(1, 0, 0), Vector(0, 1, 0)]
+#     vs = [Vector(1, 0, 0), FreeVector(0, 1, 0)]
 #     rs = o * vs
 #     assert(rs[0] == o * vs[0])
 #     assert(rs[1] == o * vs[1])
```

### Comparing `math3d-3.4.1/math3d/orientation_computer.py` & `math3d-4.0.0/math3d/orientation_computer.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 Module implementing facilities for orientation computation.
 """
 
 __author__ = "Morten Lind"
 __copyright__ = "Morten Lind 2012-2017"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Development"
 
 
 from .vector import Vector
 from .orientation import Orientation
 
 class OrientationComputer:
```

### Comparing `math3d-3.4.1/math3d/quaternion.py` & `math3d-4.0.0/math3d/quaternion.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,56 +3,56 @@
 """
 Module implementing the Quaternion class.
 """
 
 __author__ = "Morten Lind"
 __copyright__ = "Morten Lind 2012-2021"
 __credits__ = ["Morten Lind"]
-__license__ = "AGPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
 __email__ = "morten@lind.fairuse.org"
 __status__ = "Production"
 
 import numpy as np
 
-# # Circular dependencies prevents direct import of Orientation, hence
-# # global addressing
-import math3d as m3d
 
 from . import utils
-from .vector import Vector
+from .vector import FreeVector, Vector
+from .orientation import Orientation, RotationVector
 
 
 class Quaternion(object):
 
     class Error(Exception):
         """Exception class."""
+
         def __init__(self, message):
             self.message = message
             Exception.__init__(self, self.message)
 
         def __repr__(self):
             return self.message
 
     def __init__(self, *args, **kwargs):
         if len(args) == 0:
             self._s = 1
-            self._v = m3d.Vector(0, 0, 0)
+            self._v = FreeVector(0, 0, 0)
         if len(args) == 1:
             if type(args[0]) in [Quaternion]:
                 self._s = args[0]._s
                 self._v = args[0]._v.copy()
         elif len(args) == 2:
-            if utils.is_num_type(args[0]) and type(args[1]) == Vector:
+            if(utils.is_num_type(args[0]) and
+               type(args[1]) in (Vector, FreeVector)):
                 # Interpret as s, v
                 self._s = utils.flt(args[0])
-                self._v = args[1].copy()
+                self._v = FreeVector(args[1])
         elif len(args) == 4:
             self._s = args[0]
-            self._v = Vector(args[1:])
+            self._v = FreeVector(args[1:])
 
     def __getattr__(self, name):
         if name == 's':
             return self._s
         elif name == 'x':
             return self._v.x
         elif name == 'y':
@@ -94,15 +94,15 @@
             return self.__class__(self)
         else:
             self._s = other._s
             self._v = other._v.copy()
 
     def __eq__(self, other):
         return np.isclose(self._s, other._s) and self._v == other._v
-    
+
     def get_vector_part(self):
         """Return a copy of the vector part of the versor."""
         return self._v.copy()
 
     vector_part = property(get_vector_part)
 
     def get_scalar_part(self):
@@ -112,17 +112,17 @@
     scalar_part = property(get_scalar_part)
 
     def __mul__(self, other):
         """Multiplication of this with an 'other' Quaternion or Versor, or
         with a scalar.
         """
         if isinstance(other, Quaternion):
-            return Quaternion(self._s*other._s - self._v*other._v,
-                               self._v.cross(other._v)
-                               + self._s*other._v + other._s*self._v)
+            return self.__class__(self._s*other._s - self._v*other._v,
+                                  self._v.cross(other._v)
+                                  + self._s*other._v + other._s*self._v)
         elif utils.is_num_type(other):
             return Quaternion(other*self._s, other*self._v)
         else:
             return NotImplemented
 
     def __rmul__(self, rother):
         # """Right-multiply by Versor or scalar. """
@@ -139,26 +139,26 @@
         return self
 
     def __ipow__(self, x):
         """In-place exponentiation of this versor to the power of
         'x'."""
         # if abs(1 - abs(self._s)) < utils.sqrt_eps:
         #     self._s = utils.flt(1)
-        #     self._v = Vector(0, 0, 0)
+        #     self._v = FreeVector(0, 0, 0)
         # else:
         #     theta = np.arccos(self._s)
         #     sintheta = np.sin(theta)
         #     logv = theta / sintheta * self._v
         #     alpha = x * logv.length
         #     v = logv.normalized
         #     self._s = np.cos(alpha)
         #     self._v = np.sin(alpha) * v
         theta = x * np.arccos(self._s/self.norm)
         if np.isclose(self._v.length, 0):
-            n = m3d.Vector(0, 0, 0)
+            n = FreeVector(0, 0, 0)
         else:
             n = self._v.normalized
         norm = self.norm ** x
         self._s = norm * np.cos(theta)
         self._v = norm * n * np.sin(theta)
         return self
 
@@ -208,15 +208,15 @@
     conjugated = property(get_conjugated)
 
     def normalize(self):
         """Normalize this versor. """
         n = self.norm
         if abs(n) < 1e-10:
             self._s = utils.flt(1)
-            self._v = Vector(0.0, 0.0, 0.0)
+            self._v = FreeVector(0.0, 0.0, 0.0)
         else:
             ninv = 1.0 / n
             self._s *= ninv
             self._v *= ninv
 
     def get_normalized(self):
         """Return a normalised version of this quaternion. """
@@ -255,97 +255,100 @@
         remainder, slice [1:].
         """
         return [self._s]+self._v.list
 
     list = property(get_list)
 
     def get_matrix(self):
-        """Return a 4x4 matrix representation of the UnitQuaternion. See
+        """Return a 4x4 matrix representation of the Quaternion. See
         http://en.wikipedia.org/wiki/Quaternion#Matrix_representations.
         """
         a, b, c, d = self._s, self._v.x, self._v.y, self._v.z
         return np.array([[a, b, c, d],
                          [-b, a, -d, c],
                          [-c, d, a, -b],
                          [-d, -c, b, a]])
 
     matrix = property(get_matrix)
 
 
 class Versor(Quaternion):
-    """UnitQuaternion class."""
+    """Versor class for representing unit quaternions."""
 
     class Error(Exception):
         """Exception class."""
+
         def __init__(self, message):
             self.message = message
             Exception.__init__(self, self.message)
 
         def __repr__(self):
             return self.message
 
     def __init__(self, *args, **kwargs):
         """Create a versor. Args may be () for default
         constructor; (Orientation) for createing a quaternion
         representing the given orientation; (Versor) for a copy
-        constructor, (s,x,y,z) or (s,Vector) for the direct versor
-        data; (Vector) for creating the equivalent to a rotation
-        vector; or (Vector, angle) for creating the equivalent of axis
+        constructor, (s,x,y,z) or (s,FreeVector) for the direct versor
+        data; (FreeVector) for creating the equivalent to a rotation
+        vector; or (FreeVector, angle) for creating the equivalent of axis
         angle. A named option 'norm_warn' is supported as a kwargs and
         defaults to True. If set to false, nomalization is performed
         tacitly.
         """
         norm_warn = kwargs.get('norm_warn', True)
         self._s = utils.flt(0.0)
-        self._v = Vector(1, 0, 0)
+        self._v = FreeVector(1, 0, 0)
         if len(args) == 0:
             # Default constructor
             pass
         elif len(args) == 1:
             # Try with orientation or versor
-            if type(args[0]) == m3d.Orientation:
+            if type(args[0]) == Orientation:
                 self.orientation = args[0]
             # Try with rotation vector
-            elif type(args[0]) == Vector:
-                self.rotation_vector = args[0]
+            elif type(args[0]) in (Vector, FreeVector, RotationVector):
+                self.log = args[0]
             # Copy constructor
-            elif type(args[0]) in [Versor, UnitQuaternion]:
+            elif type(args[0]) == Versor:
                 self._s = args[0]._s
-                self._v = args[0]._v.copy()
+                self._v = FreeVector(args[0])
             elif type(args[0]) in (list, tuple, np.ndarray):
                 raise utils.Error(
                     'A Versor can not be constructed on a list, ' +
                     'a tuple, or an np.ndarray. Was given "{}".'
                     .format(args[0]))
             else:
                 raise utils.Error(
                     'Unknown argument given for Versor constructor: ' +
                     '"{}".'.format(args[0]))
         elif len(args) == 2:
             # Test for (axis, angle) and (s, v) determined by order
-            if utils.is_num_type(args[0]) and type(args[1]) == Vector:
+            if(utils.is_num_type(args[0]) and
+               type(args[1]) in (Vector, FreeVector)):
                 # Interpret as s, v
                 self._s = utils.flt(args[0])
-                self._v = args[1].copy()
-            elif utils.is_num_type(args[1]) and type(args[0]) == Vector:
+                self._v = FreeVector(args[1])
+            elif (utils.is_num_type(args[1]) and
+                  type(args[0]) in (Vector, FreeVector)):
                 # Interpret as axis-angle
-                axis = args[0].copy()
+                axis = FreeVector(args[0])
                 ang = args[1]
                 self.axis_angle = (axis, ang)
             else:
                 raise utils.Error(
                     'Unknown arguments given for Versor constructor' +
                     ': "{}".'.format(args[0]))
         elif len(args) == 3 and np.all(np.isreal(args)):
             # Assume three components of a rotation vector
-            self.rotation_vector = Vector(args)
+            self.rotation_vector = args
         elif len(args) == 4 and np.all(np.isreal(args)):
             # Assume numbers for s, x, y, and z
             self._s = utils.flt(args[0])
-            self._v = Vector(args[1:])
+            self._v = FreeVector(args[1:])
         else:
             raise utils.Error(
                 'Creating on type {} is not supported'
                 .format(str(type(args))))
         err = np.abs(self.norm - 1.0)
         if err > utils.eps:
             if norm_warn and err > 1.0e-4:
@@ -355,23 +358,24 @@
                       .format(self.norm-1))
             self.normalize()
 
     def __mul__(self, other):
         """Multiplication is interpreted by either transforming
         (rotating) a Vector, ordinary versor multiplication, or
         multiplication by scalar."""
-        if type(other) == Vector:
+        if type(other) in (Vector, FreeVector):
             # Do a rotation of the vector
-            return (self * Versor(0, other) * self.inverse)._v
-        elif type(other) in (Versor, UnitQuaternion):
+            return (self * Versor(0, other) * self.inverse)._v.copy()
+        elif type(other) == Versor:
             # Ordinary quaternion multiplication
-            return Versor(self._s * other._s - self._v * other._v,
-                                  self._v.cross(other._v) +
-                                  self._s * other._v + other._s * self._v)
-        elif type(other) == m3d.Orientation:
+            return Quaternion.__mul__(self, other)
+            # return Versor(self._s * other._s - self._v * other._v,
+            #               self._v.cross(other._v) +
+            #               self._s * other._v + other._s * self._v)
+        elif type(other) == Orientation:
             return self * other.versor
         # elif utils.is_num_type(other):
         #     return Versor(other * self._s, other * self._v)
         else:
             return NotImplemented
 
     def __rmul__(self, rother):
@@ -379,25 +383,25 @@
         # if utils.is_num_type(rother):
         #     return Versor(rother * self._s, rother * self._v)
         # else:
         return NotImplemented
 
     def __imul__(self, other):
         """In-place multiply."""
-        if other in [m3d.Orientation, Versor, UnitQuaternion]:
+        if other in (Orientation, Versor):
             new_versor = self * other
             self._s = new_versor._s
             self._v = new_versor._v
         else:
             return NotImplemented
         return self
 
     # Inversion is a simple conjugation
     invert = Quaternion.conjugate
-    
+
     def get_ang_norm(self, shortest=True):
         """Return the angular norm, i.e. the angular rotation, of this
         versor. If 'shortest' is True, the default, the shortest
         norm is returned, i.e. the minimal geodesic path length
         from the unit element to this unit versor.
         """
         if shortest is None:
@@ -438,55 +442,56 @@
         """Return an '(axis, angle)' pair representing the orientation of this
         versor. References:
         https://en.wikipedia.org/wiki/Quaternions_and_spatial_rotation#Recovering_the_axis-angle_representation
         https://en.wikipedia.org/wiki/Axis%E2%80%93angle_representation#Unit_quaternions
         """
         vlen = self._v.length
         if np.isclose(vlen, 0.0):
-            return (m3d.Vector(), 0.0)
+            return (FreeVector(), 0.0)
         else:
             angle = 2 * np.arctan2(vlen, self._s)
             return (self._v/vlen, angle)
 
     def set_axis_angle(self, axisangle):
         """Set this versor to the equivalent of the given axis
         and angle given in the ordered pair 'axisangle'."""
         axis, angle = axisangle
-        if type(axis) != Vector:
-            axis = Vector(axis)
+        if type(axis) not in (Vector, FreeVector):
+            axis = FreeVector(axis)
         angle = utils.flt(angle)
         sa = np.sin(0.5 * angle)
         ca = np.cos(0.5 * angle)
         axis.normalize()
         self._s = ca
         self._v._data[:] = (sa * axis)._data
 
     axis_angle = property(get_axis_angle, set_axis_angle)
 
-    def get_rotation_vector(self):
+    def get_logarithm(self):
         """Return a rotation vector representing the rotation of this
         versor."""
         axis, angle = self.axis_angle
-        return (angle * axis)._data
+        return RotationVector((angle * axis)._data)
 
-    def set_rotation_vector(self, rot_vec):
+    def set_logarithm(self, rot_vec):
         """Set this versor to the equivalent of the given
         rotation vector 'rot_vec'."""
-        if type(rot_vec) != Vector:
-            rot_vec = Vector(rot_vec)
+        if type(rot_vec) != RotationVector:
+            rot_vec = RotationVector(rot_vec)
         angle = rot_vec.length
         if angle > utils.eps:
             axis = rot_vec.normalized
         else:
             # Select arbitrary x-direction as axis and set angle to zero
             axis = Vector.e1
             angle = 0.0
         self.axis_angle = (axis, angle)
 
-    rotation_vector = property(get_rotation_vector, set_rotation_vector)
+    logarithm = log = property(get_logarithm, set_logarithm)
+    rotation_vector = rot_vec = logarithm
 
     def get_orientation(self):
         """Return an Orientation object representing the same rotation as this
         versor. The method is taken from
         http://en.wikipedia.org/wiki/Quaternions_and_spatial_rotation.
         """
         self.normalize()
@@ -494,19 +499,19 @@
         v = self._v
         x = v.x
         y = v.y
         z = v.z
         x2 = x**2
         y2 = y**2
         z2 = z**2
-        return m3d.Orientation(np.array([
+        return Orientation(np.array([
             [1 - 2 * (y2 + z2), 2 * x * y - 2 * s * z, 2 * s * y + 2 * x * z],
             [2 * x * y + 2 * s * z, 1 - 2 * (x2 + z2), -2 * s * x + 2 * y * z],
             [-2 * s * y + 2 * x * z, 2 * s * x + 2 * y * z, 1 - 2 * (x2 + y2)]
-            ]))
+        ]))
 
     def set_orientation(self, orient, positive=True):
         """Set this versor to represent the given orientation matrix in
         'orient'. The used method should be robust;
         cf. http://en.wikipedia.org/wiki/Quaternions_and_spatial_rotation.
         The mentioned method from wikipedia has problems with certain
         orientations, like the identity. Therfore another robust
@@ -526,15 +531,15 @@
             diag = M.diagonal()
             u = diag.argmax()
             v = (u + 1) % 3
             w = (v + 1) % 3
             r = np.sqrt(1 + M[u, u] - M[v, v] - M[w, w])
             if abs(r) < 1e-10:
                 self._s = utils.flt(1.0)
-                self._v = Vector(0, 0, 0)
+                self._v = FreeVector(0, 0, 0)
             else:
                 tworinv = 1.0 / (2 * r)
                 self._s = utils.flt((M[w, v] - M[v, w]) * tworinv)
                 self._v[u] = 0.5 * r
                 self._v[v] = (M[u, v] + M[v, u]) * tworinv
                 self._v[w] = (M[w, u] + M[u, w]) * tworinv
         if positive and self._s < 0:
@@ -543,36 +548,28 @@
 
     orientation = property(get_orientation, set_orientation)
 
 
 # Backwards compatibility
 UnitQuaternion = Versor
 
-# class UnitQuaternion(Versor):
-#     def __init__(self, *args, **kwargs):
-#         utils._deprecation_warning(
-#             'The class currently called "UnitQuaternion" is in fact a ' +
-#             'a Versor. It is implemented by the class "Versor", ' +
-#             'also found in the current code base. Please update your code.')
-#         Versor.__init__(self, *args, **kwargs)
-
 
 def _test():
     print('Here should come a norm-warning:')
     Versor(1, 2, 3, 4, norm_warn=True)
     print('Here should be *no* norm-warning:')
     Versor(1, 2, 3, 4, norm_warn=False)
     print('Done')
     print('Testing power operator on Versor')
-    assert(np.allclose((Versor(Vector(1, 0, 0))**2).rotation_vector,
+    assert(np.allclose((Versor(FreeVector(1, 0, 0))**2).log,
                        np.array([2, 0, 0])))
     print('Test for closeness of long and short rotation vectors (logarithm).')
-    q = Versor(m3d.Vector(0, 0, -1/2 * np.pi))
-    p = Versor(m3d.Vector(0, 0, 3/2 * np.pi))
-    assert(np.allclose(q.rotation_vector, p.rotation_vector)
-           or np.allclose(q.rotation_vector, (-p).rotation_vector))
+    q = Versor(FreeVector(0, 0, -1/2 * np.pi))
+    p = Versor(FreeVector(0, 0, 3/2 * np.pi))
+    assert(np.allclose(q.rotation_vector, p.log)
+           or np.allclose(q.log, (-p).log))
     print('Test multiplicative inverse')
-    q = Quaternion(1,2,3,4)
+    q = Quaternion(1, 2, 3, 4)
     assert(q * q.inverse == Quaternion())
     print('Testing versor transformation of vector')
-    assert(Versor(m3d.Vector(0, 0, 3/2 * np.pi)) * m3d.Vector(1, 0, 0)
-           == m3d.Vector(0, -1, 0))
+    assert(Versor(FreeVector(0, 0, 3/2 * np.pi)) * FreeVector(1, 0, 0)
+           == FreeVector(0, -1, 0))
```

### Comparing `math3d-3.4.1/math3d/reference_system/frame.py` & `math3d-4.0.0/math3d/reference_system/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Module for class Frame in the ReferenceSystem class.
 """
 
 __author__ = "Morten Lind"
 __copyright__ = "Morten Lind 2012"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Development"
 
 import numpy as np
 
 from ..transform import Transform
 
 class Frame(object):
```

### Comparing `math3d-3.4.1/math3d/reference_system/free_vector.py` & `math3d-4.0.0/math3d/reference_system/point.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,54 @@
 """
-Module for class Vector in the ReferenceSystem class.
+Module for class Point in the ReferenceSystem class.
 """
 
 __author__ = "Morten Lind"
 __copyright__ = "Morten Lind 2012"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Development"
 
 import numpy as np
 
-from ..vector import Vector 
+from ..vector import Vector
 #from .ref_sys_object import RefSysObject
 
-class FreeVector(object): 
+class Point(object): 
     """A point in the reference system is identified by a label name,
     and a vector with reference to a specific reference frame in the
     reference system. The vector representing the point is to be
     considered a position vector, and must transform as such. The
     reference system will be able to express the point in any
     registered frame of reference."""
 
-    def __init__(self, name, root_frame=None, free_vec=None, by_ref=True):
+    def __init__(self, name, root_frame=None, pos_vec=None, by_ref=True):
         """ Create a new point with given 'name', defined in
         'root_frame' and with position vector 'pos_vec'. 'root_frame'
         and 'pos_vec' may be None at creation time. If None, the
         position vector will be initialized to the zero vector. At
         time of registering in a reference system instance, the
-        reference frame must be filled in to make sense.If 'by_ref' is
-        True, the default, then the given object is stored by
-        reference; which is practical for external, implicit
-        update."""
+        reference frame must be filled in to make sense. If 'by_ref'
+        is True, the default, then the given object is stored by
+        reference; which is practical for external, implicit update."""
         self._name = name
         self._root_frame = root_frame
-        if free_vec is None:
-            free_vec = Vector()
+        if pos_vec is None:
+            pos_vec = Vector()
         self._by_ref = by_ref
         if by_ref:
-            self._free_vec = free_vec
+            self._pos_vec = pos_vec
         else:
-            self._free_vec = free_vec.copy()
+            self._pos_vec = pos_vec.copy()
 
     @property
-    def free_vec(self):
+    def pos_vec(self):
         """Give access to the position vector in the natural frame of
         reference."""
-        return self._free_vec
-    @property
-    def root_frame(self):
-        return self._root_frame
+        return self._pos_vec
 
     def __repr__(self):
         return (
-            'FreeVector: "{self._name}" in frame "{self._root_frame}" ' 
-            'with vector {self._free_vec}').format(self=self)
+            'Point: "{self._name}" in frame "{self._root_frame}" ' 
+            'with vector {self._pos_vec}').format(self=self)
```

### Comparing `math3d-3.4.1/math3d/reference_system/point.py` & `math3d-4.0.0/math3d/reference_system/free_vector.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 """
-Module for class Point in the ReferenceSystem class.
+Module for class Vector in the ReferenceSystem class.
 """
 
 __author__ = "Morten Lind"
 __copyright__ = "Morten Lind 2012"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Development"
 
 import numpy as np
 
-from ..vector import Vector
+from ..vector import Vector 
 #from .ref_sys_object import RefSysObject
 
-class Point(object): 
+class FreeVector(object): 
     """A point in the reference system is identified by a label name,
     and a vector with reference to a specific reference frame in the
     reference system. The vector representing the point is to be
     considered a position vector, and must transform as such. The
     reference system will be able to express the point in any
     registered frame of reference."""
 
-    def __init__(self, name, root_frame=None, pos_vec=None, by_ref=True):
+    def __init__(self, name, root_frame=None, free_vec=None, by_ref=True):
         """ Create a new point with given 'name', defined in
         'root_frame' and with position vector 'pos_vec'. 'root_frame'
         and 'pos_vec' may be None at creation time. If None, the
         position vector will be initialized to the zero vector. At
         time of registering in a reference system instance, the
-        reference frame must be filled in to make sense. If 'by_ref'
-        is True, the default, then the given object is stored by
-        reference; which is practical for external, implicit update."""
+        reference frame must be filled in to make sense.If 'by_ref' is
+        True, the default, then the given object is stored by
+        reference; which is practical for external, implicit
+        update."""
         self._name = name
         self._root_frame = root_frame
-        if pos_vec is None:
-            pos_vec = Vector()
+        if free_vec is None:
+            free_vec = Vector()
         self._by_ref = by_ref
         if by_ref:
-            self._pos_vec = pos_vec
+            self._free_vec = free_vec
         else:
-            self._pos_vec = pos_vec.copy()
+            self._free_vec = free_vec.copy()
 
     @property
-    def pos_vec(self):
+    def free_vec(self):
         """Give access to the position vector in the natural frame of
         reference."""
-        return self._pos_vec
+        return self._free_vec
+    @property
+    def root_frame(self):
+        return self._root_frame
 
     def __repr__(self):
         return (
-            'Point: "{self._name}" in frame "{self._root_frame}" ' 
-            'with vector {self._pos_vec}').format(self=self)
+            'FreeVector: "{self._name}" in frame "{self._root_frame}" ' 
+            'with vector {self._free_vec}').format(self=self)
```

### Comparing `math3d-3.4.1/math3d/reference_system/reference_system.py` & `math3d-4.0.0/math3d/reference_system/reference_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Module implementing the Reference System class.
 """
 
 __author__ = "Morten Lind"
 __copyright__ = "Morten Lind 2012"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Development"
 
 import functools
 
 import numpy as np
 from .frame import Frame
 from .point import Point
```

### Comparing `math3d-3.4.1/math3d/utils.py` & `math3d-4.0.0/math3d/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # coding=utf-8
 
 """
 Utility function and definitions library for PyMath3D.
 """
 
 __author__ = "Morten Lind"
-__copyright__ = "Morten Lind 2009-2015"
+__copyright__ = "Morten Lind 2009-2021"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Production"
 
 
 import numbers
 import inspect
 import collections
 
@@ -44,20 +44,20 @@
         raise Error('Supported precision (int): 16, 32, 64.')
     sqrt_eps = np.sqrt(eps)
 
 set_precision(64)
 
 def is_sequence(obj):
     """Test if "obj" is a sequence."""
-    return isinstance(obj, collections.Iterable)
+    return isinstance(obj, collections.abc.Iterable)
 
 
 def is_three_sequence(obj):
     """Test if "obj" is of a sequence type and three long."""
-    return isinstance(obj, collections.Iterable) and len(obj) == 3
+    return isinstance(obj, collections.abc.Iterable) and len(obj) == 3
 
 
 # Standard numeric types
 _number_bases = (np.number, numbers.Number)
 
 
 def is_num_type(val):
```

### Comparing `math3d-3.4.1/math3d/vector.py` & `math3d-4.0.0/math3d/vector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 # coding=utf-8
 
 """
 Module implementing the Vector class.
 """
 
 __author__ = "Morten Lind"
-__copyright__ = "Morten Lind 2012-2018"
+__copyright__ = "Morten Lind 2012-2021"
 __credits__ = ["Morten Lind"]
-__license__ = "GPLv3"
+__license__ = "LGPLv3"
 __maintainer__ = "Morten Lind"
-__email__ = "morten@lind.dyndns.dk"
+__email__ = "morten@lind.fairuse.org"
 __status__ = "Production"
 
 
+import typing
+
 import numpy as np
 
 from . import utils
 
 
 class _UnitVectors(type):
 
     @property
     def e0(self):
-        return Vector(1, 0, 0)
+        return FreeVector(1, 0, 0)
     ex = e0
 
     @property
     def e1(self):
-        return Vector(0, 1, 0)
+        return FreeVector(0, 1, 0)
     ey = e1
 
     @property
     def e2(self):
-        return Vector(0, 0, 1)
+        return FreeVector(0, 0, 1)
     ez = e2
 
     @property
     def unit_vectors(self):
         return [Vector.ex, Vector.ey, Vector.ez]
 
 
-class Vector(object, metaclass=_UnitVectors):
+class _Vector4(object, metaclass=_UnitVectors):
     """A Vector is a 3D vector (member of R3) with standard Euclidian
     operations."""
 
     @classmethod
     def canCreateOn(cls, *arg):
         if type(arg) == cls:
             return True
@@ -88,24 +90,24 @@
             raise utils.Error('__init__ : could not create vector on ' +
                               'argument : "{}" of type "{}"'
                               .format(str(args[0]), str(type(args[0]))))
         self._is_position = kwargs.get('position', 1)
 
     def __copy__(self):
         """Copy method for creating a copy of this Vector."""
-        return Vector(self)
+        return self.__class__(self)
 
     def __deepcopy__(self, memo):
         return self.__copy__()
 
     def copy(self, other=None):
         """Copy data from 'other' to self. If no argument given,
         i.e. 'other==None', return a copy of this Vector."""
         if other is None:
-            return Vector(self)
+            return self.__class__(self)
         else:
             self._data[:] = other._data
 
     def __getattr__(self, name):
         if name == 'x':
             return self._data[0]
         elif name == 'y':
@@ -145,46 +147,65 @@
     def __getitem__(self, n):
         return self._data[n]
 
     def __setitem__(self, n, val):
         self._data[n] = val
 
     def __eq__(self, other):
-        if type(other) == Vector:
+        if isinstance(other, Vector):
             return np.allclose(self._data, other._data)
         else:
             return NotImplemented
 
     def __repr__(self):
-        return ('<Vector: ({:.5f}, {:.5f}, {:.5f})>'
+        return ('<Vector4: ({:.5f}, {:.5f}, {:.5f})>'
                 .format(*self._data))
 
     def __str__(self):
         return self.__repr__()
 
     def get_is_position(self):
         """If the vector is a position vector, the default, then it
         transforms differently than a real vector.
         """
         return self._is_position
 
     is_position = property(get_is_position)
 
-    def projection(self, v, normalize=True):
-        """Get the projection vector of this vector onto a direction given by
+    def __or__(self, v: 'Vector',
+               normalize: bool = True):
+        """Get the projection vector of this vector along a direction given by
         another vector, 'v'. If 'normalize' is True, the default, 'v'
-        is first normalized. For performance reasons, normalization of
-        'v' can be avoided if the caller assures that it is of unit
-        length, and this can be flagged by setting normalize to False.
+        is first normalized. It is not mathematically clear, what the
+        meaning of projections of and onto position vectors is, so use
+        with care!
         """
+        if type(v) == np.ndarray and v.shape == (3,):
+            v = FreeVector(v)
+        if not isinstance(v, Vector):
+            return NotImplemented
         if normalize:
             v_hat = v.normalized
         else:
             v_hat = v
-        return (self * v_hat) * v_hat
+        return FreeVector((self * v_hat) * v_hat)
+
+    projected_along = __or__
+
+    def __xor__(self, v: typing.Union['Vector', np.ndarray],
+                normalize: bool = True):
+        """Return a new vector which is this vector with it's component along
+        'v' removed. If 'normalize' is True, the default, a normalized
+        version of 'v' is used. It is not mathematically clear, what
+        the meaning of projections of and onto position vectors is, so
+        use with care!
+        """
+        return self - self.projected_along(v, normalize)
+
+    removed_along = __xor__
 
     def angle(self, other, minimal=False):
         """Return the angle (radians) to the 'other' vector. This is the
         absolute, positive angle unless minimal is True, in which case
         the minimal of the two angles between the vectors is returned.
         """
         costheta = (self * other) / (self.length * other.length)
@@ -200,15 +221,15 @@
 
     def signed_angle_to(self, other, ref_vec=None):
         """With default reference rotation vector as Z-axis (if
         'ref_vec' == None), compute the signed angle of rotation from
         self to 'other'.
         """
         theta = self.angle(other)
-        xprod = self.cross(other)
+        xprod = self & other
         if ref_vec is not None:
             if xprod * ref_vec < 0:
                 theta = -theta
         else:
             if xprod.z < 0:
                 theta = -theta
         return theta
@@ -221,62 +242,68 @@
         """Return the Euclidean length."""
         return np.sqrt(self.length_squared)
 
     length = property(get_length)
 
     def get_length_squared(self):
         """Return the square of the standard Euclidean length."""
-        return np.dot(self._data, self._data)
+        return self._data @ self._data
 
     length_squared = property(get_length_squared)
 
     def normalize(self):
         """In-place normalization of this Vector."""
         length = self.length
         if length != 1.0:
             self._data = self._data / length
 
     def get_normalized(self):
         """Return a normalized Vector with same direction as this
         one.
         """
-        nv = Vector(self)
+        nv = self.__class__(self)
         nv.normalize()
         return nv
 
     normalized = property(get_normalized)
 
     def dist(self, other):
-        """Compute euclidean distance between points given by self
+        """Compute the Euclidean distance between points given by self
         and 'other'."""
-        return np.sqrt(self.dist_squared(other))
+        if isinstance(other, Vector):
+            return np.linalg.norm(self._data - other._data)
+        else:
+            return NotImplemented
 
     def dist_squared(self, other):
-        """Compute euclidean distance between points given by self
+        """Compute the square of the Euclidean distance between points given by self
         and 'other'."""
-        if type(other) == Vector:
-            sub = np.subtract(self._data, other._data)
-            return np.dot(sub, sub)
+        utils._deprecation_warning('dist()**2')
+        if isinstance(other, Vector):
+            return self.dist(other) ** 2
         else:
             return NotImplemented
 
     def get_cross_operator(self):
         """Return the cross product operator for this Vector. I.e. the
         skew-symmetric operator cross_op, such that cross_op * u == v
         x u, for any vector u."""
-        cross_op = np.zeros((3, 3))
-        cross_op[0, 1] = -self._data[2]
-        cross_op[0, 2] = self._data[1]
-        cross_op[1, 0] = self._data[2]
-        cross_op[1, 2] = -self._data[0]
-        cross_op[2, 0] = -self._data[1]
-        cross_op[2, 1] = self._data[0]
-        return cross_op
+        # cross_op = np.zeros((3,3))
+        # cross_op[0, 1] = -self._data[2]
+        # cross_op[0, 2] = self._data[1]
+        # cross_op[1, 0] = self._data[2]
+        # cross_op[1, 2] = -self._data[0]
+        # cross_op[2, 0] = -self._data[1]
+        # cross_op[2, 1] = self._data[0]
+        # return cross_op
+        x, y, z = self._data
+        return np.array(
+            (0, -z, y), (z, 0, -x), (-y, x, 0))
 
-    cross_operator = property(get_cross_operator)
+    cross_operator = skew = property(get_cross_operator)
 
     def get_alt_cross_operator(self):
         """Return the cross product operator for this Vector. I.e. the
         skew-symmetric operator cross_op, such that cross_op * u == v
         x u, for any vector u."""
         cross_op = np.zeros((3, 3))
         # cross_op[0, 1] = -self._data[2]
@@ -285,28 +312,36 @@
         # cross_op[1, 2] = -self._data[0]
         # cross_op[2, 0] = -self._data[1]
         cross_op[2, 1] = self._data[0]
         return cross_op - cross_op.T
 
     alt_cross_operator = property(get_alt_cross_operator)
 
-    def cross(self, other):
+    def __and__(self, other):
         """Return the cross product with 'other'."""
-        return Vector(np.cross(self._data, other._data))
+        # If other is a Vector, take out data
+        if isinstance(other, Vector):
+            other = other._data
+        # Check that other now is an ndarray of correct shape
+        if type(other) != np.ndarray or other.shape != (3,):
+            return NotImplemented
+        return FreeVector(np.cross(self._data, other))
+
+    cross = __and__
 
     def get_array(self):
         """Return a copy of the ndarray which is the fundamental data
         of the Vector."""
         return self._data.copy()
 
     def set_array(self, array, check=True):
         """Set the vector by three values in the iterable 'array'.
         """
         if check and len(array) != 3:
-            raise Exception(
+            raise utils.Error(
                 self.__class__.__name__ +
                 'Setting the value by the "array" property needs exactly'
                 + ' three values. ({} were given)'.format(len(array)))
         self._data[:] = array
 
     array = property(get_array, set_array)
 
@@ -341,45 +376,65 @@
 
     def __sub__(self, other):
         """Subtract another vector from this. The semantics regarding
         free and position vectors should be: If this is free, and
         other is a position, or opposite, the new should be
         position. If both are free or both are positions, the new
         should be free."""
-        if type(other) == Vector:
-            return Vector(self._data - other._data)
-        elif type(other) == np.ndarray and other.shape == (3,):
-            # Other is given as a triplet in ndarray
-            return Vector(self._data - other)
+        if type(self) == Vector:
+            if isinstance(other, Vector):
+                return Vector(self._data - other._data)
+            elif type(other) == np.ndarray and other.shape == (3,):
+                # Other is given as a triplet in ndarray
+                return Vector(self._data - other)
+            else:
+                return NotImplemented
+        elif isinstance(other, Vector):
+            if type(self) == PositionVector:
+                if type(other) == FreeVector:
+                    return PositionVector(self._data - other._data)
+                elif type(other) == PositionVector:
+                    return FreeVector(self._data - other._data)
+                else:
+                    return NotImplemented
+            elif type(self) == FreeVector:
+                if type(other) == FreeVector:
+                    return FreeVector(self._data - other._data)
+                else:
+                    # raise utils.Error('Can only subtract a free vector from a free vector.')
+                    return NotImplemented
+            else:
+                return NotImplemented
         # elif utils.is_sequence(other):
         #     # Assume a sequence of objects that may be multiplied
         #     return [self - o for o in other]
         else:
             return NotImplemented
 
     def __isub__(self, other):
-        if type(other) == Vector:
-            self._data -= other._data
-        elif type(other) == np.ndarray and other.shape == (3,):
-            # Other is given as a triplet in ndarray
-            self._data -= other
-        else:
-            return NotImplemented
+        # if type(other) == Vector:
+        #     self._data -= other._data
+        # elif type(other) == np.ndarray and other.shape == (3,):
+        #     # Other is given as a triplet in ndarray
+        #     self._data -= other
+        # else:
+        #     return NotImplemented
+        self._data[:] = (self - other)._data
         return self
 
     def __mul__(self, other):
         """Multiplication with an 'other' Vector (inner product) or
         with a scalar."""
-        if type(other) == Vector:
-            return np.dot(self._data, other._data)
+        if isinstance(other, Vector):
+            return self._data @ other._data
         elif utils.is_num_type(other):
-            return Vector(self._data * other)
+            return self.__class__(self._data * other)
         elif type(other) == np.ndarray and other.shape == (3,):
             # Other is given as a triplet in ndarray
-            return Vector(self._data * other)
+            return self.__class__(self._data * other)
         # elif utils.is_sequence(other):
         #     # Assume a sequence of objects that may be multiplied
         #     # WARNING: v * [1,2,3] == [1*v, 2*v, 3*v] !
         #     return [self * o for o in other]
         else:
             return NotImplemented
 
@@ -391,92 +446,109 @@
             return NotImplemented
             # raise utils.Error('__imul__ : Could not multiply by non-number')
         return self
 
     def __rmul__(self, other):
         """Right multiplication with a scalar, 'other'. """
         if utils.is_num_type(other):
-            return Vector(other * self._data)
+            return self.__class__(other * self._data)
         else:
             raise utils.Error('__rmul__ : Could not multiply by non-number')
 
     def __truediv__(self, other):
         """Division with a scalar, 'other'. """
         if utils.is_num_type(other):
             if np.isclose(other, 0.0):
-                raise ZeroDivisionError('In division of vector by scalar')            
-            return Vector(1.0 / other * self._data)
+                raise ZeroDivisionError(f'In division of vector by scalar. Divisor: {other}')
+            return self.__class__((1.0 / other) * self._data)
         else:
             raise utils.Error('__truediv__ : Could not divide by non-number')
     __div__ = __truediv__
 
     def __add__(self, other):
         """Return the sum of this and the 'other' vector."""
-        if type(other) == Vector:
-            return Vector(self._data + other._data)
-        elif type(other) == np.ndarray and other.shape == (3,):
-            # Other is given as a triplet in ndarray
-            return Vector(self._data + other)
-        # elif utils.is_sequence(other):
-        #     # Assume a sequence of objects that may be added
-        #     return [self + o for o in other]
+        if type(self) == Vector:
+            if type(other) == Vector:
+                return Vector(self._data + other._data)
+            elif type(other) == np.ndarray and other.shape == (3,):
+                # Other is given as a triplet in ndarray
+                return self.__class__(self._data + other)
+            else:
+                return NotImplemented
+        elif isinstance(other, Vector):
+            if((type(self) == PositionVector and type(other) == FreeVector) or
+               (type(self) == FreeVector and type(other) == PositionVector)):
+                return PositionVector(self._data + other._data)
+            elif type(self) == FreeVector and type(other) == FreeVector:
+                return FreeVector(self._data + other._data)
+            else:
+                return NotImplemented
         else:
             return NotImplemented
             # raise utils.Error('__add__ : Could not add non-vector')
 
     def __iadd__(self, other):
         """In-place add the 'other' vector to this vector."""
-        if type(other) == Vector:
-            self._data += other._data
-        elif type(other) == np.ndarray and other.shape == (3,):
-            # Other is given as a triplet in ndarray
-            self._data += other
-        else:
-            return NotImplemented
-            # raise utils.Error('__iadd__ : Could not add non-vector')
+        # if type(other) == Vector:
+        #     self._data += other._data
+        # elif type(other) == np.ndarray and other.shape == (3,):
+        #     # Other is given as a triplet in ndarray
+        #     self._data += other
+        # else:
+        #     return NotImplemented
+        #     # raise utils.Error('__iadd__ : Could not add non-vector')
+        # return self
+        self._data[:] = (self + other)._data
         return self
 
     def __neg__(self):
-        return Vector(-self._data)
+        return self.__class__(-self._data)
 
     @classmethod
     def new_random_unit_vector(cls):
         """Generator for random vectors uniformly sampled on S2. Use the
         Muller's algorithm from "A note on a method for generating
         points uniformly on n-dimensional spheres", Communications of
         the ACM, Volume 2, Issue 4, April 1959, pp 19-20.
         """
-        v = Vector(np.random.normal(size=3))
+        v = cls(np.random.normal(size=3))
         v.normalize()
         return v
 
 
+class Vector(_Vector4):
+
+    def __repr__(self):
+        return ('<Vector: ({:.5f}, {:.5f}, {:.5f})>'
+                .format(*self._data))
+
+
+class FreeVector(Vector):
 
+    def __repr__(self):
+        return ('<FreeVec: ({:.5f}, {:.5f}, {:.5f})>'
+                .format(*self._data))
 
 
-def random_unit_vector():
-    """Generator for random vectors uniformly sampled on S2. Use the
-    Muller's algorithm from "A note on a method for generating points
-    uniformly on n-dimensional spheres". Communications of the
-    ACM. Volume 2, Issue 4, April 1959, pp 19-20."""
-    utils._deprecation_warning('Vector.new_random_unit_vector')
-    v = Vector(np.random.normal(size=3))
-    v.normalize()
-    return v
+class PositionVector(Vector):
+
+    def __repr__(self):
+        return ('<PosVec: ({:.5f}, {:.5f}, {:.5f})>'
+                .format(*self._data))
 
 
 def _test_construction():
     print((Vector.canCreateOn(1, 2, 3),
            Vector.canCreateOn((1, 2, 3)),
            Vector.canCreateOn(1, 2)))
 
 
 def _test_signed_angle():
-    v = Vector(1, 2, 3)
-    u = Vector(3, 1, 2)
+    v = FreeVector(1, 2, 3)
+    u = FreeVector(3, 1, 2)
     print(v.signed_angle_to(u))
     return True
 
 
 def _test_rops():
     """Test that rop on other is called when NotImplemented is
     returned from the Vector object."""
@@ -493,24 +565,60 @@
     if v != 2 * v_origin:
         return False
     u = Vector(3, 1, 2)
     print(v.signed_angle_to(u))
     return True
 
 
-def _test_projection():
-    v0 = Vector([1, 1, 3])
-    v1 = Vector([1, 1, 0])
-    v0prj = v0.projection(v1)
-    if (v0prj - v1).length > utils.eps:
-        return False
-    v0prj = v0.projection(v1.normalized, normalize=False)
-    if (v0prj - v1).length > utils.eps:
-        return False
-    return True
+def _test_projections_and_cross_product():
+    v0 = FreeVector([1, 1, 3])
+    print(f'v0: {v0}')
+    v1 = FreeVector([1, 1, 0])
+    print(f'v1: {v1}')
+    p0 = PositionVector([1, 2, 1])
+    print(f'p0: {p0}')
+    v0prj = v0 | v1
+    print(f'Projected v0 along v1 "|": {v0prj}')
+    assert((v0prj - v1).length < utils.eps)
+    v0prj = v0.projected_along(v1.normalized, normalize=False)
+    assert((v0prj - v1).length < utils.eps)
+    v0orth = v0 ^ v1
+    print(f'Removed v1 component from v0 "^": {v0orth}')
+    assert(abs(v0orth * v1) < utils.eps)
+    # Also test cross operator
+    vx = v0 & v1
+    print(f'Cross product "v0 & v1": {vx}')
+    assert((vx | v0).length < utils.eps and (vx | v0).length < utils.eps)
+    vxp = v0 & p0
+    print(f'Cross product "v0 & p0": {vxp}')
+    a = np.array([0,1,0])
+    pxa = p0 & a
+    print(f'Cross product "p0 & {a}": {pxa}')
+
+
+def _test_free_pos_vectors():
+    v = FreeVector(1, 2, 3)
+    v1 = FreeVector(0, 1, 2)
+    p = PositionVector(1, 2, 3)
+    p1 = PositionVector(1, 1, 1)
+    print('p + v', p + v)
+    print('v + p', v + p)
+    print('v + v', v + v)
+    print('p - p1', p - p1)
+    print('p - v', p - v)
+    print('v - v1', v - v1)
+    try:
+        print('p + p', p + p)
+    except TypeError:
+        print('TypeError correctly raised when attempting "p + p".')
+    try:
+        print('v - p', v - p)
+    except TypeError:
+        print('TypeError correctly raised when attempting "v - p".')
+
 
 
 # def _test_vectorized_operations():
 #     # Test multiplication of a list
 #     v = Vector(1, 0, 0)
 #     vs = [Vector(1, 0, 0), Vector(0, 1, 0)]
 #     rms = v * vs
@@ -518,8 +626,7 @@
 #     assert(rms[1] == v * vs[1])
 #     ras = v + vs
 #     assert(ras[0] == v + vs[0])
 #     assert(ras[1] == v + vs[1])
 #     rss = v + vs
 #     assert(rss[0] == v + vs[0])
 #     assert(rss[1] == v + vs[1])
-
```

### Comparing `math3d-3.4.1/setup.py` & `math3d-4.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from distutils.core import setup
-from distutils.command.install_data import install_data
+from setuptools import setup
 
 setup(
     name='math3d',
-    version='3.4.1',
+    version='4.0.0',
     description='3D Special Euclidean mathematics package for Python.',
     author='Morten Lind',
     author_email='morten@lind.fairuse.org',
-    url='https://gitlab.com/morlin/pymath3d',
+    url='https://codeberg.org/moli/pymath3d',
     packages=['math3d', 'math3d.interpolation', 'math3d.reference_system',
-              'math3d.dynamics', 'math3d.geometry'],
+              'math3d.dynamics', 'math3d.geometry', 'math3d.visualization'],
     provides=['math3d'],
-    # install_requires=['numpy'],
+    install_requires=['numpy', 'matplotlib'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
-        'License :: OSI Approved :: GNU Affero General Public License v3',
+        'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Natural Language :: English',
         'Programming Language :: Python',
         'Topic :: Scientific/Engineering',
     ],
-    license='GNU Affero General Public License v3',
-    data_files=[('share/doc/pymath3d', ['README.md', 'COPYING'])]
+    license='GNU Lesser General Public License v3 (LGPLv3)',
+    data_files=[('share/doc/pymath3d', ['README.md', 'COPYING.LESSER'])]
 )
```

