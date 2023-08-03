# Comparing `tmp/unitclass-1.0.7.tar.gz` & `tmp/unitclass-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitclass-1.0.7.tar", last modified: Mon Jul 17 21:48:19 2023, max compression
+gzip compressed data, was "unitclass-1.0.8.tar", last modified: Thu Aug  3 00:53:39 2023, max compression
```

## Comparing `unitclass-1.0.7.tar` & `unitclass-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-17 21:48:19.570690 unitclass-1.0.7/
--rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.0.7/LICENSE
--rw-r--r--   0 blake      (501) staff       (20)     7249 2023-07-17 21:48:19.570548 unitclass-1.0.7/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)     6480 2023-07-17 21:47:14.000000 unitclass-1.0.7/README.md
--rw-r--r--   0 blake      (501) staff       (20)      852 2023-07-17 21:47:37.000000 unitclass-1.0.7/pyproject.toml
--rw-r--r--   0 blake      (501) staff       (20)       38 2023-07-17 21:48:19.570724 unitclass-1.0.7/setup.cfg
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-17 21:48:19.570370 unitclass-1.0.7/unitclass.egg-info/
--rw-r--r--   0 blake      (501) staff       (20)     7249 2023-07-17 21:48:19.000000 unitclass-1.0.7/unitclass.egg-info/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)      177 2023-07-17 21:48:19.000000 unitclass-1.0.7/unitclass.egg-info/SOURCES.txt
--rw-r--r--   0 blake      (501) staff       (20)        1 2023-07-17 21:48:19.000000 unitclass-1.0.7/unitclass.egg-info/dependency_links.txt
--rw-r--r--   0 blake      (501) staff       (20)       10 2023-07-17 21:48:19.000000 unitclass-1.0.7/unitclass.egg-info/top_level.txt
--rw-r--r--   0 blake      (501) staff       (20)    48408 2023-07-17 21:39:22.000000 unitclass-1.0.7/unitclass.py
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-08-03 00:53:39.093286 unitclass-1.0.8/
+-rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.0.8/LICENSE
+-rw-r--r--   0 blake      (501) staff       (20)     7249 2023-08-03 00:53:39.093158 unitclass-1.0.8/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)     6480 2023-07-17 21:47:14.000000 unitclass-1.0.8/README.md
+-rw-r--r--   0 blake      (501) staff       (20)      852 2023-08-03 00:52:25.000000 unitclass-1.0.8/pyproject.toml
+-rw-r--r--   0 blake      (501) staff       (20)       38 2023-08-03 00:53:39.093323 unitclass-1.0.8/setup.cfg
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-08-03 00:53:39.093000 unitclass-1.0.8/unitclass.egg-info/
+-rw-r--r--   0 blake      (501) staff       (20)     7249 2023-08-03 00:53:39.000000 unitclass-1.0.8/unitclass.egg-info/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)      177 2023-08-03 00:53:39.000000 unitclass-1.0.8/unitclass.egg-info/SOURCES.txt
+-rw-r--r--   0 blake      (501) staff       (20)        1 2023-08-03 00:53:39.000000 unitclass-1.0.8/unitclass.egg-info/dependency_links.txt
+-rw-r--r--   0 blake      (501) staff       (20)       10 2023-08-03 00:53:39.000000 unitclass-1.0.8/unitclass.egg-info/top_level.txt
+-rw-r--r--   0 blake      (501) staff       (20)    48588 2023-08-03 00:50:50.000000 unitclass-1.0.8/unitclass.py
```

### Comparing `unitclass-1.0.7/LICENSE` & `unitclass-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `unitclass-1.0.7/PKG-INFO` & `unitclass-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 1.0.7
+Version: 1.0.8
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `unitclass-1.0.7/README.md` & `unitclass-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `unitclass-1.0.7/pyproject.toml` & `unitclass-1.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unitclass"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Blake Garretson", email="blake@blakeg.net" },
 ]
 description = "Physical unit class suitable for calculations in the sciences."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `unitclass-1.0.7/unitclass.egg-info/PKG-INFO` & `unitclass-1.0.8/unitclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 1.0.7
+Version: 1.0.8
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `unitclass-1.0.7/unitclass.py` & `unitclass-1.0.8/unitclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 #     factor is set to 1 below to make it obvious that no scaling is done
 
 _unit_list = [
     # SI base units
     ('time', 's', 'second seconds sec secs', 1, ''),
     ('length', 'm', 'meter meters metre metres', 1, ''),
     ('current', 'A', 'ampere amperes amp amps', 1, ''),
-    ('temperature', '°K', 'K kelvin Kelvin degK', 1, ''),
+    ('temperature', 'K', '°K kelvin Kelvin degK', 1, ''),
     ('amount', 'mol', 'mols mole moles', 1, ''),
     ('luminous_intensity', 'cd', 'candela candelas', 1, ''),
     ('energy', 'J', 'joule joules ', 1, ''),
     ('mass', 'kg', 'kilogram kilograms', 1, ''),
     ('force', 'N', 'newton newtons', 1, ''),
     ('charge', 'C', 'coulomb coulombs', 1, ''),
     ('catalytic_activity', 'kat', 'katal katals', 1, ''),
@@ -323,14 +323,15 @@
 _prefix_units_names = 'meter gram second amp liter joule newton pascal weber ohm volt coulomb farad henry hertz'.split()
 _prefix_mult = (1e18, 1e15, 1e12, 1e9, 1e6, 1e3, 1e-1, 1e-2, 1e-3, 1e-6, 1e-9,
                 1e-12, 1e-15)
 _prefixes = list("EPTGMkdcmμnpf")
 _prefix_aliases = ['exa', 'peta', 'tera', 'giga', 'mega', 'kilo',
                    'deci', 'centi', 'milli', 'micro', 'nano', 'pico', 'femto']
 
+no_space_units = ['°', '%']
 
 def _expand_units(unitlist):
     """Take a list of units and return a list with exponents
     expanded to individual units.  e.g. ["N","m2"] -> ["N", "m", "m"]
     """
     newlist = []
     for u in unitlist:
@@ -666,21 +667,21 @@
 
     both = _get_unit_name(from_unit, ignore_error=True) + \
         _get_unit_name(to_unit, ignore_error=True)
     if both == '°C°F':
         newvalue = _convert_C2F(value)
     elif both == '°F°C':
         newvalue = _convert_F2C(value)
-    elif both == '°K°C':
+    elif both == 'K°C':
         newvalue = _convert_K2C(value)
-    elif both == '°C°K':
+    elif both == '°CK':
         newvalue = _convert_C2K(value)
-    elif both == '°F°K':
+    elif both == '°FK':
         newvalue = _convert_C2K(_convert_F2C(value))
-    elif both == '°K°F':
+    elif both == 'K°F':
         newvalue = _convert_C2F(_convert_K2C(value))
     else:
         forcemass_counts = _check_consistent_units(from_unit, to_unit, handle_mass_conversion=True)
         mass_factor = 1
         if isinstance(forcemass_counts, list):
             num_force, num_mass = forcemass_counts[0]
             den_force, den_mass = forcemass_counts[1]
@@ -1039,15 +1040,18 @@
         """
         if isinstance(self.value, numbers.Number):
             unit_str = self.unit.translate(self.to_specials)
             prefix = ''
             if 'USD' in unit_str:
                 prefix = '$'
                 unit_str = unit_str.replace('USD', '')
-            return "{}{:g} {}".format(prefix, self.value, unit_str).strip()
+            if unit_str and (unit_str in no_space_units):
+                return "{}{:g}{}".format(prefix, self.value, unit_str).strip()
+            else:
+                return "{}{:g} {}".format(prefix, self.value, unit_str).strip()
         else:
             return ""
 
     def __mul__(self, other):
         other = Unit(other)
         if all([_check_consistent_units(self.unit, other.unit, silent=True),
                 (self.unit != other.unit), all([self.unit, other.unit])]):
```

