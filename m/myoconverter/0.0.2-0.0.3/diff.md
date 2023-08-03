# Comparing `tmp/myoconverter-0.0.2.tar.gz` & `tmp/myoconverter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myoconverter-0.0.2.tar", last modified: Wed Aug  2 12:36:45 2023, max compression
+gzip compressed data, was "myoconverter-0.0.3.tar", last modified: Thu Aug  3 16:04:16 2023, max compression
```

## Comparing `myoconverter-0.0.2.tar` & `myoconverter-0.0.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.373465 myoconverter-0.0.2/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    11357 2023-08-02 12:04:59.000000 myoconverter-0.0.2/LICENSE
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      459 2023-08-02 12:36:45.373465 myoconverter-0.0.2/PKG-INFO
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    12366 2023-08-02 12:04:59.000000 myoconverter-0.0.2/README.md
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.367465 myoconverter-0.0.2/examples/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:00.000000 myoconverter-0.0.2/examples/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3666 2023-08-02 12:05:00.000000 myoconverter-0.0.2/examples/example_models_convert.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.367465 myoconverter-0.0.2/myoconverter/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     8561 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/O2MPipeline.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       22 2023-08-02 12:05:51.000000 myoconverter-0.0.2/myoconverter/__init__.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.368465 myoconverter-0.0.2/myoconverter/conversion_steps/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    11705 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/conversion_steps/O2MStep1.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    30245 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/conversion_steps/O2MStep2.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    23489 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/conversion_steps/O2MStep3.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    13786 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/conversion_steps/O2MSteps.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/conversion_steps/__init__.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.368465 myoconverter-0.0.2/myoconverter/utils/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/utils/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    16722 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/utils/generate_pdf.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.369465 myoconverter-0.0.2/myoconverter/xml/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/__init__.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.369465 myoconverter-0.0.2/myoconverter/xml/bodies/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     4041 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/bodies/Body.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2912 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/bodies/Ground.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       84 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/bodies/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2963 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/bodies/utils.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     5065 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/config.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.369465 myoconverter-0.0.2/myoconverter/xml/constraints/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     4646 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/constraints/CoordinateCouplerConstraint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       90 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/constraints/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     7773 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/converter.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.370465 myoconverter-0.0.2/myoconverter/xml/forces/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      566 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/BushingForce.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2336 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/CoordinateActuator.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     4151 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/CoordinateLimitForce.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      618 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/FunctionBasedBushingForce.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1814 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/Ligament.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1129 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/Millard2012EquilibriumMuscle.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     5468 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/Muscle.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      556 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/PointActuator.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1534 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/Schutte1993Muscle_Deprecated.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      603 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/SpringGeneralizedForce.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1030 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/Thelen2003Muscle.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      560 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/TorqueActuator.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       85 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2770 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/forces/utils.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.371465 myoconverter-0.0.2/myoconverter/xml/joints/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    16303 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/CustomJoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2118 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/Joint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1983 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/PinJoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1944 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/SliderJoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2334 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/UniversalJoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      652 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/WeldJoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       85 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3670 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/joints/utils.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.371465 myoconverter-0.0.2/myoconverter/xml/markers/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1070 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/markers/Marker.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       86 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/markers/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     6461 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/parsers.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.372465 myoconverter-0.0.2/myoconverter/xml/path_points/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     8604 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_points/ConditionalPathPoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     6144 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_points/MovingPathPoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1537 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_points/PathPoint.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       89 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_points/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     6796 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_points/utils.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.372465 myoconverter-0.0.2/myoconverter/xml/path_wraps/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3327 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_wraps/PathWrap.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3977 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_wraps/PathWrapSet.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       88 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_wraps/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     7758 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/path_wraps/utils.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    11328 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/utils.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.373465 myoconverter-0.0.2/myoconverter/xml/wrap_objects/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1670 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapCylinder.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1729 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapEllipsoid.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3594 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapObject.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1580 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapSphere.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1429 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapTorus.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       90 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/wrap_objects/__init__.py
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     8219 2023-08-02 12:05:01.000000 myoconverter-0.0.2/myoconverter/xml/wrap_objects/utils.py
-drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:36:45.367465 myoconverter-0.0.2/myoconverter.egg-info/
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      459 2023-08-02 12:36:45.000000 myoconverter-0.0.2/myoconverter.egg-info/PKG-INFO
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2650 2023-08-02 12:36:45.000000 myoconverter-0.0.2/myoconverter.egg-info/SOURCES.txt
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        1 2023-08-02 12:36:45.000000 myoconverter-0.0.2/myoconverter.egg-info/dependency_links.txt
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      215 2023-08-02 12:36:45.000000 myoconverter-0.0.2/myoconverter.egg-info/requires.txt
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       22 2023-08-02 12:36:45.000000 myoconverter-0.0.2/myoconverter.egg-info/top_level.txt
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      533 2023-08-02 12:05:01.000000 myoconverter-0.0.2/pyproject.toml
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       38 2023-08-02 12:36:45.373465 myoconverter-0.0.2/setup.cfg
--rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1001 2023-08-02 12:35:41.000000 myoconverter-0.0.2/setup.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.772606 myoconverter-0.0.3/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    11357 2023-08-02 12:04:59.000000 myoconverter-0.0.3/LICENSE
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      459 2023-08-03 16:04:16.772606 myoconverter-0.0.3/PKG-INFO
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    12601 2023-08-03 15:27:19.000000 myoconverter-0.0.3/README.md
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.757604 myoconverter-0.0.3/examples/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:00.000000 myoconverter-0.0.3/examples/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3666 2023-08-02 12:05:00.000000 myoconverter-0.0.3/examples/example_models_convert.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.758603 myoconverter-0.0.3/myoconverter/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     8561 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/O2MPipeline.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       22 2023-08-03 15:26:24.000000 myoconverter-0.0.3/myoconverter/__init__.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.759604 myoconverter-0.0.3/myoconverter/conversion_steps/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    11705 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/conversion_steps/O2MStep1.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    30245 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/conversion_steps/O2MStep2.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    23489 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/conversion_steps/O2MStep3.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    13786 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/conversion_steps/O2MSteps.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/conversion_steps/__init__.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.760604 myoconverter-0.0.3/myoconverter/utils/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/utils/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    16722 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/utils/generate_pdf.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.761604 myoconverter-0.0.3/myoconverter/xml/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        0 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/__init__.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.762604 myoconverter-0.0.3/myoconverter/xml/bodies/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     4041 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/bodies/Body.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2912 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/bodies/Ground.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       84 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/bodies/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2963 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/bodies/utils.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     5065 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/config.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.762604 myoconverter-0.0.3/myoconverter/xml/constraints/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     4646 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/constraints/CoordinateCouplerConstraint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       90 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/constraints/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     7773 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/converter.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.766605 myoconverter-0.0.3/myoconverter/xml/forces/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      566 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/forces/BushingForce.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2336 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/forces/CoordinateActuator.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     4151 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/forces/CoordinateLimitForce.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      618 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/forces/FunctionBasedBushingForce.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1814 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/forces/Ligament.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1129 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/forces/Millard2012EquilibriumMuscle.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     5468 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/forces/Muscle.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      556 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/forces/PointActuator.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1534 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/forces/Schutte1993Muscle_Deprecated.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      603 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/forces/SpringGeneralizedForce.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1030 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/forces/Thelen2003Muscle.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      560 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/forces/TorqueActuator.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       85 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/forces/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2770 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/forces/utils.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.768605 myoconverter-0.0.3/myoconverter/xml/joints/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    16303 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/joints/CustomJoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2118 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/joints/Joint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1983 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/joints/PinJoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1944 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/joints/SliderJoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2334 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/joints/UniversalJoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      652 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/joints/WeldJoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       85 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/joints/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3670 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/joints/utils.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.768605 myoconverter-0.0.3/myoconverter/xml/markers/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1070 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/markers/Marker.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       86 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/markers/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     6461 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/parsers.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.769605 myoconverter-0.0.3/myoconverter/xml/path_points/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     8604 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/path_points/ConditionalPathPoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     6144 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/path_points/MovingPathPoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1537 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/path_points/PathPoint.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       89 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/path_points/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     6796 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/path_points/utils.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.770605 myoconverter-0.0.3/myoconverter/xml/path_wraps/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3327 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/path_wraps/PathWrap.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3977 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/path_wraps/PathWrapSet.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       88 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/path_wraps/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     7758 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/path_wraps/utils.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)    11328 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/utils.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.772606 myoconverter-0.0.3/myoconverter/xml/wrap_objects/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1670 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/wrap_objects/WrapCylinder.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1729 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/wrap_objects/WrapEllipsoid.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     3594 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/wrap_objects/WrapObject.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1580 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/wrap_objects/WrapSphere.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1429 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/wrap_objects/WrapTorus.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       90 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/wrap_objects/__init__.py
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     8219 2023-08-02 12:05:01.000000 myoconverter-0.0.3/myoconverter/xml/wrap_objects/utils.py
+drwxrwxr-x   0 aleksi    (1000) aleksi    (1000)        0 2023-08-03 16:04:16.758603 myoconverter-0.0.3/myoconverter.egg-info/
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      459 2023-08-03 16:04:16.000000 myoconverter-0.0.3/myoconverter.egg-info/PKG-INFO
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     2650 2023-08-03 16:04:16.000000 myoconverter-0.0.3/myoconverter.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)        1 2023-08-03 16:04:16.000000 myoconverter-0.0.3/myoconverter.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      218 2023-08-03 16:04:16.000000 myoconverter-0.0.3/myoconverter.egg-info/requires.txt
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       22 2023-08-03 16:04:16.000000 myoconverter-0.0.3/myoconverter.egg-info/top_level.txt
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)      533 2023-08-02 12:05:01.000000 myoconverter-0.0.3/pyproject.toml
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)       38 2023-08-03 16:04:16.772606 myoconverter-0.0.3/setup.cfg
+-rw-rw-r--   0 aleksi    (1000) aleksi    (1000)     1004 2023-08-03 16:03:09.000000 myoconverter-0.0.3/setup.py
```

### Comparing `myoconverter-0.0.2/LICENSE` & `myoconverter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/README.md` & `myoconverter-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 | [myoSuite](https://sites.google.com/view/myosuite/myosim?authuser=0) | [Current Limitations](---)
 
 ## Example models
 Here we present a collection of models, as examples, that have been processed with the myoConverter tool. We try to keep these converted models up-to-date (in case of bug fixes etc.), but it is recommended to run the conversions yourself to ensure up-to-date models.
 
 |   | Model name| Source | Validation | Conversion Speed | 
 |--------------------|--------------|:-------:|:--------:|-------|
-|<img src="https://github.com/MyoHub/myoConverter/blob/main/docs/source/images/tug-of-war.png" width="200">| [Turg of War](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/TugOfWar/Tug_of_War_cvt3.xml) <br> - 1 DoF <br> - 2 Muscles | [Osim](https://github.com/MyoHub/myoConverter/tree/main/models/osim/TugOfWar)  |   [Report](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/TugOfWar/Tug_of_War_conversion_report.pdf) | Regular: 30 sec <br> Speedy: 30 sec |
+|<img src="https://github.com/MyoHub/myoConverter/blob/main/docs/source/images/tug-of-war.png" width="200">| [Tug of War](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/TugOfWar/Tug_of_War_cvt3.xml) <br> - 1 DoF <br> - 2 Muscles | [Osim](https://github.com/MyoHub/myoConverter/tree/main/models/osim/TugOfWar)  |   [Report](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/TugOfWar/Tug_of_War_conversion_report.pdf) | Regular: 30 sec <br> Speedy: 30 sec |
 |<img src="https://github.com/MyoHub/myoConverter/blob/main/docs/source/images/arm26.png" width="200">| [Simple Arm](https://github.com/MyoHub/myo_sim/blob/main/elbow/myoelbow_2dof6muscles.xml)  <br> - 2 DoFs <br> - 6 Muscles | [Osim](https://github.com/MyoHub/myoConverter/tree/main/models/osim/Arm26)  |   [Report](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/Arm26/arm26_conversion_report.pdf) | Regular: 5 min 30 sec <br> Speedy: 4 min 37 sec |
 |<img src="https://github.com/MyoHub/myoConverter/blob/main/docs/source/images/leg6dof.png" width="200">| [Single Leg](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/Leg6Dof9Musc/leg6dof9musc_cvt3.xml)   <br> - 6 DoFs <br> - 9 Muscles | [Osim](https://github.com/MyoHub/myoConverter/tree/main/models/osim/Leg6Dof9Musc)  |   [Report](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/Leg6Dof9Musc/leg6dof9musc_conversion_report.pdf) | Regular: 4 min 3 sec <br> Speedy: 3 min 41 sec |
 |<img src="https://github.com/MyoHub/myoConverter/blob/main/docs/source/images/gait10.png" width="200">| [2D Gait Model](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/Gait10dof18musc/gait10dof18musc_cvt3.xml) <br> - 10 DoFs <br> - 18 Muscles | [Osim](https://github.com/MyoHub/myoConverter/tree/main/models/osim/Gait10dof18musc)  |   [Report](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/Gait10dof18musc/gait10dof18musc_conversion_report.pdf) | Regular: 8 min 21 sec <br> Speedy: 7 min 33 sec |
 |<img src="https://github.com/MyoHub/myoConverter/blob/main/docs/source/images/gait23.png" width="200">| [3D Gait Model](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/Gait2354Simbody/gait2354_simbody_cvt3.xml)  <br> - 23 DoFs <br> - 54 Muscles | [Osim](https://github.com/MyoHub/myoConverter/tree/main/models/osim/Gait2354Simbody)  |   [Report](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/Gait2354Simbody/gait2354_simbody_conversion_report.pdf) | Regular: 34 min 21 sec <br> Speedy: 22 min 58 sec |
 |<img src="https://github.com/MyoHub/myoConverter/blob/main/docs/source/images/neck6d.png" width="200">| [Neck Model](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/Neck6D/HYOID_1.2_ScaledStrenght_UpdatedInertia_adjusted_cvt3.xml) <br> - 6 DoFs <br> - 72 Muscles | [Osim](https://github.com/MyoHub/myoConverter/tree/main/models/osim/Neck6D)  |   [Report](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/Neck6D/HYOID_1.2_ScaledStrenght_UpdatedInertia_adjusted_conversion_report.pdf) | Regular: 200 min 14 sec <br> Speedy: 57 min 43 sec |
 <!--|<img src="https://github.com/MyoHub/myoConverter/blob/main/docs/source/images/fullbody3d.png" width="200">| [Full Body Model](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/FullBody3D/FullBodyModel_Hamner2010_v2_0_cvt3.xml)  <br> - 36 DoFs <br> - 86 Muscles | [Osim](https://github.com/MyoHub/myoConverter/tree/main/models/osim/FullBody3D)  |   [Report](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/FullBody3D/FullBodyModel_Hamner2010_v2_0_conversion_report.pdf) | Regular: 75 min 17 sec <br> Speedy: 58 min 46 sec | -->
 <!--|<img src="https://github.com/MyoHub/myoConverter/blob/main/docs/source/images/wristhand.png" width="200">| [Wrist-Hand Model](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/WristHandModel/wrist_cvt3.xml)  <br> - 10 DoFs <br> - 25 Muscles | [Osim](https://github.com/MyoHub/myoConverter/tree/main/models/osim/WristHandModel)  |   [Report](https://github.com/MyoHub/myoConverter/blob/main/models/mjc/WristHandModel/wrist_conversion_report.pdf) | Regular: 54 min 06 sec <br> Speedy: 18 min 26 sec | -->
@@ -40,47 +40,53 @@
 Besides, a list of third-party converted models using this tool can be found [here]().
 
 We encourage you to review these models before embarking on any redundant efforts. However, we must emphasize that we cannot guarantee the accuracy of these models, as there is no universal test for this. If you have specific concerns or questions regarding any of the models, we recommend reaching out directly to the respective model creators for further information and clarification.
 
 
 ## Download & Setup
 
-### Linux
-If you would like to convert your own MSK model, you can use myoConverter by following the steps outlined below:
+For Linux we recommend installing via pip or conda. For Windows/MacOS users we provide a docker image, as the conda installation seems to be very slow.
+
+### Conda
+
+`conda install -c conda-forge myoconverter`
+
+### Pip
+
+`pip install myoconverter`
+
+### Docker
+
+In Windows and MacOS, we provide a docker image that has the myoConverter ready to be used. Please follow the following usage [instructions](./docker/README.md).
+
+## Development
+
+If you'd like to contribute to the development of this project, we recommend cloning the repo and creating a conda environment with the provided `conda_env.yml` file.
 
 - Clone the repo
 ```bash
 git clone git@github.com:MyoHub/myoConverter.git; cd myoConverter
 ```
 
-
 - Create a conda environment with the `conda_env.yml` file
 ```bash
 conda env create -f conda_env.yml
 conda activate myoConverter
 ```
 
-- Test installation
-```bash
-python -c "import myoConverter"
-```
-
-### Windows/MacOS
-In Windows and MacOS, we provide a docker image that has the myoConverter ready to be used. Please follow the following usage instructions:
-.... 
 
 ## Quick example
 
 #### Call a Python function
 
 ```python
 from myoconverter import O2MPipeline
 O2MPipeline(osim_file, geometry_folder, output_folder, **kwargs)
 ```
-converts "/path/to/*.osim" to a MuJoCo XML file and outputs the model into folder "/path/to/output/folder". The `**kwargs` may contain the optional parameters as listed below:
+converts `osim_file` to a MuJoCo XML file and outputs the model into folder `output_folder`. The `**kwargs` may contain the optional parameters as listed below:
 - `convert_steps` : Selected conversion steps, could be any subset of `[1, 2, 3]` based on the needs, Default = `[1, 2, 3]`
 - `muscle_list` : Selected specific muscles for the conversion and validation steps, Default = None
 - `osim_data_overwrite` : If true, overwrite extracted Osim model state files, Default = False [overwrite is needed, if Osim model has changed]
 - `conversion` : If true, perform the conversion functions of selected steps, Default = True
 - `validation` : If true, perform the validation functions of selected steps, Default = True
 - `speedy` : If true, reduce the number of checking notes in optimization steps to increase speed, Default = False
 - `generate_pdf` : If true, generate a pdf report of the validation results, Default = False
```

### Comparing `myoconverter-0.0.2/examples/example_models_convert.py` & `myoconverter-0.0.3/examples/example_models_convert.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/O2MPipeline.py` & `myoconverter-0.0.3/myoconverter/O2MPipeline.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/conversion_steps/O2MStep1.py` & `myoconverter-0.0.3/myoconverter/conversion_steps/O2MStep1.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/conversion_steps/O2MStep2.py` & `myoconverter-0.0.3/myoconverter/conversion_steps/O2MStep2.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/conversion_steps/O2MStep3.py` & `myoconverter-0.0.3/myoconverter/conversion_steps/O2MStep3.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/conversion_steps/O2MSteps.py` & `myoconverter-0.0.3/myoconverter/conversion_steps/O2MSteps.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/utils/generate_pdf.py` & `myoconverter-0.0.3/myoconverter/utils/generate_pdf.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/bodies/Body.py` & `myoconverter-0.0.3/myoconverter/xml/bodies/Body.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/bodies/Ground.py` & `myoconverter-0.0.3/myoconverter/xml/bodies/Ground.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/bodies/utils.py` & `myoconverter-0.0.3/myoconverter/xml/bodies/utils.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/config.py` & `myoconverter-0.0.3/myoconverter/xml/config.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/constraints/CoordinateCouplerConstraint.py` & `myoconverter-0.0.3/myoconverter/xml/constraints/CoordinateCouplerConstraint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/converter.py` & `myoconverter-0.0.3/myoconverter/xml/converter.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/forces/BushingForce.py` & `myoconverter-0.0.3/myoconverter/xml/forces/BushingForce.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/forces/CoordinateActuator.py` & `myoconverter-0.0.3/myoconverter/xml/forces/CoordinateActuator.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/forces/CoordinateLimitForce.py` & `myoconverter-0.0.3/myoconverter/xml/forces/CoordinateLimitForce.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/forces/FunctionBasedBushingForce.py` & `myoconverter-0.0.3/myoconverter/xml/forces/FunctionBasedBushingForce.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/forces/Ligament.py` & `myoconverter-0.0.3/myoconverter/xml/forces/Ligament.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/forces/Millard2012EquilibriumMuscle.py` & `myoconverter-0.0.3/myoconverter/xml/forces/Millard2012EquilibriumMuscle.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/forces/Muscle.py` & `myoconverter-0.0.3/myoconverter/xml/forces/Muscle.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/forces/PointActuator.py` & `myoconverter-0.0.3/myoconverter/xml/forces/PointActuator.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/forces/Schutte1993Muscle_Deprecated.py` & `myoconverter-0.0.3/myoconverter/xml/forces/Schutte1993Muscle_Deprecated.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/forces/SpringGeneralizedForce.py` & `myoconverter-0.0.3/myoconverter/xml/forces/SpringGeneralizedForce.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/forces/Thelen2003Muscle.py` & `myoconverter-0.0.3/myoconverter/xml/forces/Thelen2003Muscle.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/forces/TorqueActuator.py` & `myoconverter-0.0.3/myoconverter/xml/forces/TorqueActuator.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/forces/utils.py` & `myoconverter-0.0.3/myoconverter/xml/forces/utils.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/joints/CustomJoint.py` & `myoconverter-0.0.3/myoconverter/xml/joints/CustomJoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/joints/Joint.py` & `myoconverter-0.0.3/myoconverter/xml/joints/Joint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/joints/PinJoint.py` & `myoconverter-0.0.3/myoconverter/xml/joints/PinJoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/joints/SliderJoint.py` & `myoconverter-0.0.3/myoconverter/xml/joints/SliderJoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/joints/UniversalJoint.py` & `myoconverter-0.0.3/myoconverter/xml/joints/UniversalJoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/joints/WeldJoint.py` & `myoconverter-0.0.3/myoconverter/xml/joints/WeldJoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/joints/utils.py` & `myoconverter-0.0.3/myoconverter/xml/joints/utils.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/markers/Marker.py` & `myoconverter-0.0.3/myoconverter/xml/markers/Marker.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/parsers.py` & `myoconverter-0.0.3/myoconverter/xml/parsers.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/path_points/ConditionalPathPoint.py` & `myoconverter-0.0.3/myoconverter/xml/path_points/ConditionalPathPoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/path_points/MovingPathPoint.py` & `myoconverter-0.0.3/myoconverter/xml/path_points/MovingPathPoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/path_points/PathPoint.py` & `myoconverter-0.0.3/myoconverter/xml/path_points/PathPoint.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/path_points/utils.py` & `myoconverter-0.0.3/myoconverter/xml/path_points/utils.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/path_wraps/PathWrap.py` & `myoconverter-0.0.3/myoconverter/xml/path_wraps/PathWrap.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/path_wraps/PathWrapSet.py` & `myoconverter-0.0.3/myoconverter/xml/path_wraps/PathWrapSet.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/path_wraps/utils.py` & `myoconverter-0.0.3/myoconverter/xml/path_wraps/utils.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/utils.py` & `myoconverter-0.0.3/myoconverter/xml/utils.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapCylinder.py` & `myoconverter-0.0.3/myoconverter/xml/wrap_objects/WrapCylinder.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapEllipsoid.py` & `myoconverter-0.0.3/myoconverter/xml/wrap_objects/WrapEllipsoid.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapObject.py` & `myoconverter-0.0.3/myoconverter/xml/wrap_objects/WrapObject.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapSphere.py` & `myoconverter-0.0.3/myoconverter/xml/wrap_objects/WrapSphere.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/wrap_objects/WrapTorus.py` & `myoconverter-0.0.3/myoconverter/xml/wrap_objects/WrapTorus.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter/xml/wrap_objects/utils.py` & `myoconverter-0.0.3/myoconverter/xml/wrap_objects/utils.py`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/myoconverter.egg-info/SOURCES.txt` & `myoconverter-0.0.3/myoconverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/pyproject.toml` & `myoconverter-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myoconverter-0.0.2/setup.py` & `myoconverter-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="myoconverter",
-    version="0.0.2",
+    version="0.0.3",
     author="Huawei Wang, Aleksi Ikkala",
     author_email="",
     description="Tool for converting OpenSim musculoskeletal (MSK) models to the MuJoCo model format with optimized muscle kinematics and kinetics",
     long_description="Check the [GitHub repository](https://github.com/MyoHub/myo-converter) for up-to-date documentation",
     long_description_content_type="text/markdown",
     url="https://github.com/MyoHub/myo-converter",
     packages=setuptools.find_packages(),
     install_requires=[
-      'python>=3.9',
+      'python==3.9.16',
       'mujoco-python==2.3.3',
       'loguru==0.5.3',
       'lxml==4.9.1',
       'numpy==1.21.5',
       'scipy==1.10.0',
       'scikit-learn==1.2.0',
       'opensim==4.4',
```

