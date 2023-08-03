# Comparing `tmp/xraydb-4.5.0.tar.gz` & `tmp/xraydb-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xraydb-4.5.0.tar", last modified: Thu Jan 26 21:43:53 2023, max compression
+gzip compressed data, was "xraydb-4.5.1.tar", last modified: Thu Aug  3 18:00:48 2023, max compression
```

## Comparing `xraydb-4.5.0.tar` & `xraydb-4.5.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-01-26 21:43:53.947585 xraydb-4.5.0/
--rw-r--r--   0 Newville   (501) staff       (20)       32 2023-01-26 21:41:42.000000 xraydb-4.5.0/.gitattributes
--rw-r--r--   0 Newville   (501) staff       (20)      640 2023-01-26 21:41:42.000000 xraydb-4.5.0/LICENSE
--rw-r--r--   0 Newville   (501) staff       (20)      206 2023-01-26 21:41:42.000000 xraydb-4.5.0/MANIFEST.in
--rw-r--r--   0 Newville   (501) staff       (20)      598 2023-01-26 21:43:53.947664 xraydb-4.5.0/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)      263 2023-01-26 21:41:42.000000 xraydb-4.5.0/README
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-01-26 21:43:53.939446 xraydb-4.5.0/examples/
--rw-r--r--   0 Newville   (501) staff       (20)     1104 2023-01-26 21:41:42.000000 xraydb-4.5.0/examples/darwin_widths.py
--rw-r--r--   0 Newville   (501) staff       (20)      603 2023-01-26 21:41:42.000000 xraydb-4.5.0/examples/mirror_comparison.py
--rw-r--r--   0 Newville   (501) staff       (20)      615 2023-01-26 21:41:42.000000 xraydb-4.5.0/examples/mu_calcite.py
--rw-r--r--   0 Newville   (501) staff       (20)      871 2023-01-26 21:41:42.000000 xraydb-4.5.0/examples/mu_components_C.py
--rw-r--r--   0 Newville   (501) staff       (20)      874 2023-01-26 21:41:42.000000 xraydb-4.5.0/examples/mu_components_Fe.py
--rw-r--r--   0 Newville   (501) staff       (20)      598 2023-01-26 21:41:42.000000 xraydb-4.5.0/examples/mu_elements.py
--rw-r--r--   0 Newville   (501) staff       (20)      595 2023-01-26 21:41:42.000000 xraydb-4.5.0/examples/mu_water.py
--rw-r--r--   0 Newville   (501) staff       (20)       39 2023-01-26 21:41:42.000000 xraydb-4.5.0/requirements.txt
--rw-r--r--   0 Newville   (501) staff       (20)      197 2023-01-26 21:43:53.947995 xraydb-4.5.0/setup.cfg
--rw-r--r--   0 Newville   (501) staff       (20)     1234 2023-01-26 21:41:42.000000 xraydb-4.5.0/setup.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-01-26 21:43:53.939937 xraydb-4.5.0/tests/
--rw-r--r--   0 Newville   (501) staff       (20)     7365 2023-01-26 21:41:42.000000 xraydb-4.5.0/tests/test_chem_materials.py
--rw-r--r--   0 Newville   (501) staff       (20)    36364 2023-01-26 21:41:42.000000 xraydb-4.5.0/tests/test_xray.py
--rw-r--r--   0 Newville   (501) staff       (20)     2054 2023-01-26 21:41:42.000000 xraydb-4.5.0/tests/test_xraydb.py
--rw-r--r--   0 Newville   (501) staff       (20)    68611 2023-01-26 21:41:42.000000 xraydb-4.5.0/versioneer.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-01-26 21:43:53.948173 xraydb-4.5.0/xraydb/
--rw-r--r--   0 Newville   (501) staff       (20)     1197 2023-01-26 21:41:42.000000 xraydb-4.5.0/xraydb/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)      497 2023-01-26 21:43:53.948207 xraydb-4.5.0/xraydb/_version.py
--rw-r--r--   0 Newville   (501) staff       (20)     6358 2023-01-26 21:41:42.000000 xraydb-4.5.0/xraydb/chemparser.py
--rw-r--r--   0 Newville   (501) staff       (20)     7069 2023-01-26 21:41:42.000000 xraydb-4.5.0/xraydb/materials.dat
--rw-r--r--   0 Newville   (501) staff       (20)     9976 2023-01-26 21:41:42.000000 xraydb-4.5.0/xraydb/materials.py
--rw-r--r--   0 Newville   (501) staff       (20)     4126 2023-01-26 21:41:42.000000 xraydb-4.5.0/xraydb/utils.py
--rw-r--r--   0 Newville   (501) staff       (20)    54923 2023-01-26 21:41:42.000000 xraydb-4.5.0/xraydb/xray.py
--rwxr-xr-x   0 Newville   (501) staff       (20)    26138 2023-01-26 21:41:42.000000 xraydb-4.5.0/xraydb/xraydb.py
--rw-r--r--   0 Newville   (501) staff       (20) 10297344 2023-01-26 21:41:42.000000 xraydb-4.5.0/xraydb/xraydb.sqlite
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-01-26 21:43:53.947475 xraydb-4.5.0/xraydb.egg-info/
--rw-r--r--   0 Newville   (501) staff       (20)      598 2023-01-26 21:43:53.000000 xraydb-4.5.0/xraydb.egg-info/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)      659 2023-01-26 21:43:53.000000 xraydb-4.5.0/xraydb.egg-info/SOURCES.txt
--rw-r--r--   0 Newville   (501) staff       (20)        1 2023-01-26 21:43:53.000000 xraydb-4.5.0/xraydb.egg-info/dependency_links.txt
--rw-r--r--   0 Newville   (501) staff       (20)       23 2023-01-26 21:43:53.000000 xraydb-4.5.0/xraydb.egg-info/requires.txt
--rw-r--r--   0 Newville   (501) staff       (20)        7 2023-01-26 21:43:53.000000 xraydb-4.5.0/xraydb.egg-info/top_level.txt
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-08-03 18:00:48.779768 xraydb-4.5.1/
+-rw-r--r--   0 Newville   (501) staff       (20)       32 2023-08-03 17:53:16.000000 xraydb-4.5.1/.gitattributes
+-rw-r--r--   0 Newville   (501) staff       (20)     1128 2023-08-03 17:53:16.000000 xraydb-4.5.1/LICENSE
+-rw-r--r--   0 Newville   (501) staff       (20)      206 2023-08-03 17:53:16.000000 xraydb-4.5.1/MANIFEST.in
+-rw-r--r--   0 Newville   (501) staff       (20)     1473 2023-08-03 18:00:48.779914 xraydb-4.5.1/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)      263 2023-08-03 17:53:16.000000 xraydb-4.5.1/README
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-08-03 18:00:48.772012 xraydb-4.5.1/examples/
+-rw-r--r--   0 Newville   (501) staff       (20)     1104 2023-08-03 17:53:16.000000 xraydb-4.5.1/examples/darwin_widths.py
+-rw-r--r--   0 Newville   (501) staff       (20)      603 2023-08-03 17:53:16.000000 xraydb-4.5.1/examples/mirror_comparison.py
+-rw-r--r--   0 Newville   (501) staff       (20)      615 2023-08-03 17:53:16.000000 xraydb-4.5.1/examples/mu_calcite.py
+-rw-r--r--   0 Newville   (501) staff       (20)      871 2023-08-03 17:53:16.000000 xraydb-4.5.1/examples/mu_components_C.py
+-rw-r--r--   0 Newville   (501) staff       (20)      874 2023-08-03 17:53:16.000000 xraydb-4.5.1/examples/mu_components_Fe.py
+-rw-r--r--   0 Newville   (501) staff       (20)      598 2023-08-03 17:53:16.000000 xraydb-4.5.1/examples/mu_elements.py
+-rw-r--r--   0 Newville   (501) staff       (20)      595 2023-08-03 17:53:16.000000 xraydb-4.5.1/examples/mu_water.py
+-rw-r--r--   0 Newville   (501) staff       (20)      213 2023-08-03 17:53:16.000000 xraydb-4.5.1/pyproject.toml
+-rw-r--r--   0 Newville   (501) staff       (20)       38 2023-08-03 17:53:16.000000 xraydb-4.5.1/requirements.txt
+-rw-r--r--   0 Newville   (501) staff       (20)     1495 2023-08-03 18:00:48.780378 xraydb-4.5.1/setup.cfg
+-rw-r--r--   0 Newville   (501) staff       (20)       91 2023-08-03 17:59:04.000000 xraydb-4.5.1/setup.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-08-03 18:00:48.772413 xraydb-4.5.1/tests/
+-rw-r--r--   0 Newville   (501) staff       (20)     7365 2023-08-03 17:53:16.000000 xraydb-4.5.1/tests/test_chem_materials.py
+-rw-r--r--   0 Newville   (501) staff       (20)    36350 2023-08-03 17:53:16.000000 xraydb-4.5.1/tests/test_xray.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2054 2023-08-03 17:53:16.000000 xraydb-4.5.1/tests/test_xraydb.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-08-03 18:00:48.773571 xraydb-4.5.1/xraydb/
+-rw-r--r--   0 Newville   (501) staff       (20)     1160 2023-08-03 17:53:16.000000 xraydb-4.5.1/xraydb/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)     6358 2023-08-03 17:53:16.000000 xraydb-4.5.1/xraydb/chemparser.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7069 2023-08-03 17:53:16.000000 xraydb-4.5.1/xraydb/materials.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     9976 2023-08-03 17:53:16.000000 xraydb-4.5.1/xraydb/materials.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4126 2023-08-03 17:53:16.000000 xraydb-4.5.1/xraydb/utils.py
+-rw-r--r--   0 Newville   (501) staff       (20)      160 2023-08-03 18:00:48.000000 xraydb-4.5.1/xraydb/version.py
+-rw-r--r--   0 Newville   (501) staff       (20)    52776 2023-08-03 17:53:16.000000 xraydb-4.5.1/xraydb/xray.py
+-rwxr-xr-x   0 Newville   (501) staff       (20)    28337 2023-08-03 17:53:16.000000 xraydb-4.5.1/xraydb/xraydb.py
+-rw-r--r--   0 Newville   (501) staff       (20) 10305536 2023-08-03 17:53:16.000000 xraydb-4.5.1/xraydb/xraydb.sqlite
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-08-03 18:00:48.779651 xraydb-4.5.1/xraydb.egg-info/
+-rw-r--r--   0 Newville   (501) staff       (20)     1473 2023-08-03 18:00:48.000000 xraydb-4.5.1/xraydb.egg-info/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)      659 2023-08-03 18:00:48.000000 xraydb-4.5.1/xraydb.egg-info/SOURCES.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        1 2023-08-03 18:00:48.000000 xraydb-4.5.1/xraydb.egg-info/dependency_links.txt
+-rw-r--r--   0 Newville   (501) staff       (20)       68 2023-08-03 18:00:48.000000 xraydb-4.5.1/xraydb.egg-info/requires.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        7 2023-08-03 18:00:48.000000 xraydb-4.5.1/xraydb.egg-info/top_level.txt
```

### Comparing `xraydb-4.5.0/examples/darwin_widths.py` & `xraydb-4.5.1/examples/darwin_widths.py`

 * *Files identical despite different names*

### Comparing `xraydb-4.5.0/examples/mirror_comparison.py` & `xraydb-4.5.1/examples/mirror_comparison.py`

 * *Files identical despite different names*

### Comparing `xraydb-4.5.0/examples/mu_calcite.py` & `xraydb-4.5.1/examples/mu_calcite.py`

 * *Files identical despite different names*

### Comparing `xraydb-4.5.0/examples/mu_components_C.py` & `xraydb-4.5.1/examples/mu_components_C.py`

 * *Files identical despite different names*

### Comparing `xraydb-4.5.0/examples/mu_components_Fe.py` & `xraydb-4.5.1/examples/mu_components_Fe.py`

 * *Files identical despite different names*

### Comparing `xraydb-4.5.0/examples/mu_elements.py` & `xraydb-4.5.1/examples/mu_elements.py`

 * *Files identical despite different names*

### Comparing `xraydb-4.5.0/examples/mu_water.py` & `xraydb-4.5.1/examples/mu_water.py`

 * *Files identical despite different names*

### Comparing `xraydb-4.5.0/tests/test_chem_materials.py` & `xraydb-4.5.1/tests/test_chem_materials.py`

 * *Files identical despite different names*

### Comparing `xraydb-4.5.0/tests/test_xray.py` & `xraydb-4.5.1/tests/test_xray.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                     atomic_symbol, atomic_mass, atomic_density, xray_edges,
                     xray_edge, xray_lines, xray_line, fluor_yield,
                     ck_probability, core_width, guess_edge,
                     xray_delta_beta, darwin_width, mirror_reflectivity,
                     ionchamber_fluxes, XrayDB)
 
 
-from xraydb.xray import (chantler_data, formula_to_mass_fracs, 
+from xraydb.xray import (chantler_data, formula_to_mass_fracs,
                          _validate_mass_fracs, mass_fracs_to_molar_fracs,
                          transmission_sample)
 
 def test_atomic_data():
     assert atomic_number('zn') == 30
     assert atomic_symbol(26) == 'Fe'
     assert atomic_mass(45) > 102.8
@@ -620,35 +620,35 @@
 
     ic3 = ionchamber_fluxes(gas={'nitrogen':0.5, 'helium': 0.5}, volts=1.25,
                             length=20.0, energy=15000.0, sensitivity=1.e-6)
 
     ic4 = ionchamber_fluxes(gas='Ar', volts=1.25, length=20.0,
                             energy=15000.0, sensitivity=1.e-6)
 
+    assert_allclose(ic1.transmitted/ic1.incident, 0.999, rtol=0.03)
+    assert_allclose(ic1.incident, 2.503e11, rtol=0.03)
 
-    assert_allclose(ic1.transmitted/ic1.incident, 0.999, rtol=0.001)
-    assert_allclose(ic1.incident, 4.91084e11, rtol=0.01)
+    assert_allclose(ic2.transmitted/ic2.incident, 0.970, rtol=0.03)
+    assert_allclose(ic2.incident, 3.75e11, rtol=0.03)
 
-    assert_allclose(ic2.transmitted/ic2.incident, 0.9696, rtol=0.01)
-    assert_allclose(ic2.incident, 7.5417e11, rtol=0.01)
+    assert_allclose(ic3.transmitted/ic3.incident, 0.984, rtol=0.03)
+    assert_allclose(ic3.incident, 8.40e11, rtol=0.03)
 
-    assert_allclose(ic3.transmitted/ic3.incident, 0.992, rtol=0.01)
-    assert_allclose(ic3.incident, 1.636e12, rtol=0.01)
+    assert_allclose(ic4.transmitted/ic4.incident, 0.493, rtol=0.03)
+    assert_allclose(ic4.incident, 1.394e10, rtol=0.03)
 
-    assert_allclose(ic4.transmitted/ic4.incident, 0.4928, rtol=0.01)
-    assert_allclose(ic4.incident, 2.7615e10, rtol=0.01)
 
 
 def test_formula_to_mass_fracs():
     mf1 = formula_to_mass_fracs('Fe2O3')
     desired1 = {'Fe': 0.69943, 'O': 0.30056}
     assert_allclose(mf1['Fe'], desired1['Fe'], rtol=0.001)
     assert_allclose(mf1['O'], desired1['O'], rtol=0.001)
     assert_allclose(sum(mf1.values()), 1.0, rtol=0.001)
-    
+
     mf2 = formula_to_mass_fracs({'Fe2O3':1, 'FeO':2})
     desired2 = {'Fe': 0.7363, 'O': 0.2637}
     assert_allclose(mf2['Fe'], desired2['Fe'], rtol=0.001)
     assert_allclose(mf2['O'], desired2['O'], rtol=0.001)
     assert_allclose(sum(mf2.values()), 1.0, rtol=0.001)
```

### Comparing `xraydb-4.5.0/tests/test_xraydb.py` & `xraydb-4.5.1/tests/test_xraydb.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from numpy.testing import assert_allclose
 
 from xraydb import XrayDB
 
 def test_xraydb_version():
     xdb = XrayDB()
     version = xdb.get_version()
-    assert 'XrayDB Version: 8.1, Python' in version
+    assert 'XrayDB Version: 9.1, Python' in version
 
     hist = xdb.get_version(with_history=True)
     assert len(hist) > 350
     hist = hist.split('\n')
     assert len(hist) > 4
 
 def test_molar_mass():
```

### Comparing `xraydb-4.5.0/xraydb/__init__.py` & `xraydb-4.5.1/xraydb/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 """Python interface to XrayDB:
 
    X-ray Reference Data for the Elements
 
-   last update: 30-August-2019
+   last update: 2-August-2023
    License: Public Domain
    Author:  Matthew Newville <newville@cars.uchicago.edu>
             Center for Advanced Radiation Sources,
             The University of Chicago
 """
 
+from .version import version as __version__
 
 from .xraydb import XrayDB
 
 from .chemparser import chemparse, validate_formula
 
 from .materials import (material_mu, material_mu_components, get_materials,
                         get_material, find_material, add_material)
 
-from .xray import (atomic_number, atomic_symbol, atomic_mass,
+from .xray import (atomic_number, atomic_symbol, atomic_name, atomic_mass,
                    atomic_density, xray_edges, xray_edge, xray_lines,
                    xray_line, fluor_yield, ck_probability, core_width, f0,
                    f0_ions, chantler_energies, f1_chantler, f2_chantler,
                    mu_chantler, mu_elam, coherent_cross_section_elam,
                    incoherent_cross_section_elam, guess_edge,
                    xray_delta_beta, get_xraydb, darwin_width,
                    mirror_reflectivity, ionchamber_fluxes,
                    ionization_potential, transmission_sample)
-
-from ._version import get_versions
-__version__ = get_versions()['version']
-del get_versions
```

### Comparing `xraydb-4.5.0/xraydb/chemparser.py` & `xraydb-4.5.1/xraydb/chemparser.py`

 * *Files identical despite different names*

### Comparing `xraydb-4.5.0/xraydb/materials.dat` & `xraydb-4.5.1/xraydb/materials.dat`

 * *Files identical despite different names*

### Comparing `xraydb-4.5.0/xraydb/materials.py` & `xraydb-4.5.1/xraydb/materials.py`

 * *Files identical despite different names*

### Comparing `xraydb-4.5.0/xraydb/utils.py` & `xraydb-4.5.1/xraydb/utils.py`

 * *Files identical despite different names*

### Comparing `xraydb-4.5.0/xraydb/xray.py` & `xraydb-4.5.1/xraydb/xray.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 R0 = 1.e8 * R_ELECTRON_CM
 
 from .xraydb import XrayDB,  XrayLine
 from .chemparser import chemparse
 
 fluxes = namedtuple('IonChamberFluxes', ('incident', 'transmitted',
-                                         'photo', 'incoherent'))
+                                         'photo', 'incoherent', 'coherent'))
 
 DarwinWidth = namedtuple('DarwinWidth', ('theta', 'theta_offset',
                                          'theta_width', 'theta_fwhm',
                                          'energy_width', 'energy_fwhm',
                                          'zeta', 'dtheta', 'denergy',
                                          'intensity'))
 
@@ -368,14 +368,27 @@
     Returns:
         atomic symbol
     """
     xdb = get_xraydb()
     return xdb._elem_data(z).symbol
 
 
+def atomic_name(z):
+    """atomic name for atomic number
+
+    Args:
+        z (int):  atomic number
+
+    Returns:
+        atomic name (English)
+    """
+    xdb = get_xraydb()
+    return xdb._elem_data(z).name
+
+
 def atomic_mass(element):
     """molar mass for an element
 
     Args:
         element (int, str):  atomic number, atomic symbol for element
 
     Return:
@@ -812,32 +825,33 @@
 
     r_amp = (kiz - ktz)/(kiz + ktz)
     if roughness > 1.e-12:
         r_amp = r_amp * np.exp(-2*(roughness**2*kiz*ktz))
     return (r_amp*r_amp.conjugate()).real
 
 
-def ionchamber_fluxes(gas='nitrogen', volts=1.0, length=100.0,
-                      energy=10000.0, sensitivity=1.e-6,
-                      sensitivity_units='A/V', with_compton=1):
-
+def ionchamber_fluxes(gas='nitrogen', volts=1.0, length=100.0, energy=10000.0,
+                      sensitivity=1.e-6, sensitivity_units='A/V',
+                      with_compton=True, both_carriers=True):
     """return ion chamber and PIN diode fluxes for a gas, mixture of gases, or
     semiconductor material, ion chamber length (or diode thickness), X-ray energy,
     recorded voltage and current amplifier sensitivity.  See note for details.
 
     Args:
         gas (string or dict):  name or formula of fill gas (see note 1) ['nitrogen']
         volts (float):  measured voltage output of current amplifier  [1.0]
         length (float): active length of ion chamber in cm [100]
         energy (float): X-ray energy in eV [10000]
         sensitivity (float): current amplifier sensitivity [1.e-6]
         sensitivity_units (string): units of current amplifier sensitivity
                                     (see note 2 for options) ['A/V']
-        with_compton (int): switch to control the contribution of Compton
-                            scattering (see note 3) [1]
+        with_compton (bool): switch to control the contribution of Compton
+                            scattering (see note 3) [True]
+        both_carriers (bool): switch to control whether to count both electron
+                            and ion current (see note 4) [True]
 
 
     Returns:
         named tuple IonchamberFluxes with fields
 
             `incident`    flux of beam incident on ion chamber in Hz
 
@@ -847,182 +861,118 @@
 
             `incoherent`  flux attenuated by incoherent scattering in Hz
 
 
     Examples:
 
         >>> from xraydb import ionchamber_fluxes
-        >>> fl = ionchamber_fluxes(gas='helium', volts=1.25, length=20.0,
-                                   energy=10000.0, sensitivity=1.e-9)
-
-        >>> print(f"Fluxes: In={fl.incident:g}, Out={fl.transmitted:g}, Transmitted={100*fl.transmitted/fl.incident:.2f}%")
-        Fluxes: In=2.79631e+11, Out=2.79383e+11, Transmitted=99.91%
-
-        >>> fl = ionchamber_fluxes(gas='nitrogen', volts=1.25, length=20.0,
-                                   energy=10000.0, sensitivity=1.e-6)
+        >>> fl = ionchamber_fluxes(gas='nitrogen', volts=1.25,
+                                   length=20.0, energy=10e3, sensitivity=1.e-6)
 
         >>> print(f"Fluxes: In={fl.incident:g}, Out={fl.transmitted:g}, Transmitted={100*fl.transmitted/fl.incident:.2f}%")
         Fluxes: In=3.20045e+11, Out=2.90464e+11, Transmitted=90.76%
 
         >>> fl = ionchamber_fluxes(gas={'nitrogen':0.5, 'helium': 0.5},
-                                  volts=1.25, length=20.0, energy=10000.0,
-                                  sensitivity=1.e-6)
+                                   volts=1.25, length=20.0, energy=10000.0,
+                                   sensitivity=1.e-6)
 
         >>> print(f"Fluxes: In={fl.incident:g}, Out={fl.transmitted:g}, Transmitted={100*fl.transmitted/fl.incident:.2f}%")
         Fluxes: In=6.83845e+11, Out=6.51188e+11, Transmitted=95.22%
 
     Notes:
-       1. The gas value can either be a string for the name of chemical
-          formula for the gas or diode material, or dictionary with keys
-          that are gas names or formulas and values that are the relative
-          fraction for mixes gases.  For diode materials, mixtures are not
-          supported.
-
-          The gas formula is used both the contributions for mu and to get
-          get the weighted effective ionization potential for the material.
-
-          The effective ionization potentials are known for a handful of
-          gases and diodes (see `ionization_potential` function), and range
-          between 20 and 45 eV for gases, and around 3 eV for semiconductors.
-          For unknown gases the value of 32.0 eV will be used.
+       1. The gas value can either be a string for the name of chemical formula
+          for the gas or diode material, or dictionary with keys that are gas
+          names or formulas and values that are the relative fraction for mixes
+          gases.  For diode materials, mixtures are not supported.
+
+          The gas formula is used both the contributions for mu and to get the
+          weighted effective ionization potential for the material.
+
+          The effective ionization potentials are known for a handful of gases
+          and diodes (see `ionization_potential` function), and range between
+          20 and 45 eV for gases, and around 3 eV for semiconductors. For
+          unknown gases the value of 32.0 eV will be used.
 
        2. The `sensitivity` and `sensitivity_units` arguments have some overlap
-          to specify the sensitivity or gain of the current amplifier.
-          Generally, the units in `A/V`, but you can add a common SI prefix of
-          'p', 'pico', 'n', 'nano', (unicode 'u03bc'), 'u', 'micro', 'm', 'milli'
-          so that, `ionchamber_fluxes(..., sensitivity=1.e-6)` and
+          to specify the sensitivity of the current amplifier. Generally, the
+          units are in `A/V`, but you can add a common SI prefix of 'p', 'pico',
+          'n', 'nano', (unicode 'u03bc'), 'u', 'micro', 'm', 'milli' so that,
+          `ionchamber_fluxes(..., sensitivity=1.e-6)` and
           `ionchamber_fluxes(..., sensitivity=1, sensitivity_units='uA/V')`
-          will both give a sensitivity of 1 microAmp / Volt .
-
-       3. The effect of Compton scattering on the ion chamber current can be approximated
-          in 3 ways with different values for `with_compton` (default=1):
-
-             >0:  use Compton-shifted electron energy (best approximation)
-
-             =0:  completely ignore the effect of Compton scattering on current
-
-             <0:  use incident energy as Compton energy.
-
-          Using -1 should reproduce the calculation from Hephaestus reasonably
-          well, but using 1 is highly recommended.
-
-       4. Ion Chamber Current calculation: the total attenuation in an ion
-          chamber includes photo, incoherent (Compton), and coherent (Rayleigh)
-          scattering contributions:
-
-            Flux_transmitted = Flux_in * exp(-t*mu_total)
-
-          The current in an Ion Chamber has a contribution from both the
-          photo-electric and incoherent (Compton) cross-section, but not
-          the coherent scattering. For an incident flux (in Hz) of Flux_in,
-          the fluxes of X-rays attenuated by the different processes are:
-
-             Flux_photo = Flux_in * [1 - exp(-t*mu_photo)]
-
-             Flux_incoh = Flux_in * [1 - exp(-t*mu_incoh)]
-
-             Flux_coh   = Flux_in * [1 - exp(-t*mu_coh)]
-
-             Flux_transmitted = Flux_in - Flux_total
-
-          For Flux_photo, all of the X-ray energy is converted to current:
-
-             IC_current_photo = Flux_photo * Energy * q_e / ion_pot
-
-          where q_e is the electron charge (1.602e-19 C), and ion_pot is the
-          effective ionization potential (see `ionization_potential`).
-
-          For Flux_incoh, the energy transferred to the electron is converted
-          to electron and ion current as:
-
-             IC_current_incoh = Flux_incoh * Energy_Compton * q_e / ion_pot
-
-          where:
-
-             Energy_Compton = Energy/(1+m_e*c^2/Energy)
-
-          is the approximate energy of the Compton-scattered electron.  This
-          estimate of the energy is a simplification: the transferred energy will
-          be angle-dependent, ranging from 0 to 2*Energy_Compton, with a
-          distribution that depends on Energy and polarization.
+          will both give a sensitivity of 1 microAmp / Volt.
 
+       3. The effect of Compton scattering on the ion chamber current can be
+          approximated using the mean energy of the Compton-scattered electron.
+          See the documentation for more details. Set `with_compton=False` to
+          turn off this correction.
+
+       4. The effective ionization potential generates an electron and ions
+          pair, and normally both carriers will contribute to the current. Thus,
+          the number of carries below, `N_carriers` is 2.  To consider the
+          current from 1 carrier, for example if using a Frisch grid, use
+          `both_carries=False`, which will set `N_carriers` to 1.
     """
     from .materials import material_mu
 
+    xdb = get_xraydb()
     fin = fout = fphoto = 0.0
 
     units = sensitivity_units.replace('Volts', 'V').replace('Volt', 'V')
     units = units.replace('Amperes', 'A').replace('Ampere', 'A')
     units = units.replace('Amps', 'A').replace('Amp', 'A')
     units = units.replace('A/V', '')
     sensitivity *= SI_PREFIXES.get(units, 1)
 
+    ncarriers = 2 if both_carriers else 1
     if isinstance(gas, str):
         gas = {gas: 1.0}
 
     gas_total = 0.0
     gas_comps = []
     for gname, frac in gas.items():
         ionpot = ionization_potential(gname)
         if gname == 'N2': gname = 'nitrogen'
         if gname == 'O2': gname = 'oxygen'
         gas_total += frac
         gas_comps.append((gname, frac, ionpot))
 
-    # energy of Compton-scattered electron: median energy, approximate
-    # can turn off Compton energy with with_compton switch:
-    energy_compton = 0      # no Compton contribution
-    if with_compton > 0:    # median Compton energy
-        energy_compton = energy/(1 + E_MASS/energy)
-    elif with_compton < 0:  # use incident X-ray energy: hephaestus
-        energy_compton = energy
+    # energy of Compton-scattered electron: mean energy, found from
+    # tabulated values of integration over the Klein-Nishina cross-section
+    energy_compton = 0   # if no Compton contribution
+    if with_compton:     # mean energy of the Compton-scattered electron
+        energy_compton = xdb.compton_energies(energy).electron_mean
 
     # use weighted sums for mu values and ionization potential
-    mu_photo, mu_incoh, mu_total, ion_pot =  0.0, 0.0, 0.0, 0.0
+    mu_photo, mu_incoh, mu_total, mu_coh, ion_pot =  0.0, 0.0, 0.0, 0.0, 0.0
     for gas_name, gas_frac, gas_ion_pot in gas_comps:
         gasmu_photo = material_mu(gas_name, energy=energy, kind='photo')
         gasmu_total = material_mu(gas_name, energy=energy, kind='total')
         gasmu_incoh = material_mu(gas_name, energy=energy, kind='incoh')
+        gasmu_coh   = material_mu(gas_name, energy=energy, kind='coh')
 
         mu_photo += gasmu_photo * gas_frac/gas_total
         mu_total += gasmu_total * gas_frac/gas_total
         mu_incoh += gasmu_incoh * gas_frac/gas_total
+        mu_coh   += gasmu_coh * gas_frac/gas_total
         ion_pot  += gas_ion_pot * gas_frac/gas_total
 
-    atten_total = 1.0 - np.exp(-length* mu_total)
+    atten_total = 1.0 - np.exp(-length*mu_total)
     atten_photo = atten_total*mu_photo/mu_total
     atten_incoh = atten_total*mu_incoh/mu_total
-    atten_coh   = atten_total - atten_photo - atten_incoh
-
-    absorbed_energy = energy*atten_photo + energy_compton*atten_incoh
+    atten_coh   = atten_total*mu_coh/mu_total
 
+    absorbed_energy = ncarriers*(energy*atten_photo + energy_compton*atten_incoh)
     flux_in    = volts*sensitivity*ion_pot/(QCHARGE*absorbed_energy)
     flux_photo = flux_in * atten_photo
     flux_incoh = flux_in * atten_incoh
     flux_out   = flux_in * (1-atten_total)
     flux_coh   = flux_in * atten_coh
 
-    if False: # documenting old, incorrect formula before deleting:
-        ab_old = (energy*(1-np.exp(-length* mu_photo)) +
-                  energy_compton*(1-np.exp(-length* mu_incoh)))
-
-        fold_in    = volts*sensitivity*ion_pot/(QCHARGE*ab_old)
-        fold_photo = fold_in * (1-np.exp(-length* mu_photo))
-        fold_incoh = fold_in * (1-np.exp(-length* mu_incoh))
-        fold_out   = fold_in * np.exp(-length*mu_total)
-        fold_coh   = fold_in - fold_photo - fold_incoh - fold_out
-
-        # print(f"Flux In   : {flux_in:.3e} was {fold_in:.3e}")
-        # print(f"Flux Out  : {flux_out:.3e} was {fold_out:.3e}")
-        # print(f"Flux Photo: {flux_photo:.3e} was {fold_photo:.3e}")
-        # print(f"Flux Incoh: {flux_incoh:.3e} was {fold_incoh:.3e}")
-        # print(f"Flux Coher: {flux_coh:.3e} was {fold_coh:.3e}")
-
     return fluxes(incident=flux_in, transmitted=flux_out,
-                  photo=flux_photo, incoherent=flux_incoh)
+                  photo=flux_photo, incoherent=flux_incoh, coherent=flux_coh)
 
 
 def darwin_width(energy, crystal='Si', hkl=(1, 1, 1), a=None,
                  polarization='s', ignore_f2=False, ignore_f1=False, m=1):
 
     """darwin width for a crystal reflection and energy
```

### Comparing `xraydb-4.5.0/xraydb/xraydb.py` & `xraydb-4.5.1/xraydb/xraydb.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 from sqlalchemy.pool import SingletonThreadPool
 
 from .utils import elam_spline, as_ndarray
 
 XrayEdge = namedtuple('XrayEdge', ('energy', 'fyield', 'jump_ratio'))
 XrayLine = namedtuple('XrayLine', ('energy', 'intensity', 'initial_level',
                                    'final_level'))
-ElementData = namedtuple('ElementData', ('Z', 'symbol', 'mass', 'density'))
+ElementData = namedtuple('ElementData', ('Z', 'symbol', 'name', 'mass', 'density'))
+ComptonEnergies = namedtuple('ComptonEnergies', ('incident', 'xray_90deg', 'xray_mean', 'electron_mean'))
 
-__version__ = '1.4'
+__version__ = '1.5'
 
 def make_engine(dbname):
     "create engine for sqlite connection"
     return create_engine('sqlite:///%s' % (dbname), future=True,
                          poolclass=SingletonThreadPool,
                          connect_args={'check_same_thread': False})
 
@@ -42,16 +43,16 @@
 
     Notes:
       1. must be a sqlite db file, with tables named 'elements',
         'photoabsorption', 'scattering', 'xray_levels', 'Coster_Kronig',
         'Chantler', 'Waasmaier', and 'KeskiRahkonen_Krause'
     """
     _tables = ('Chantler', 'Waasmaier', 'Coster_Kronig',
-               'KeskiRahkonen_Krause', 'xray_levels',
-               'elements', 'photoabsorption', 'scattering')
+               'KeskiRahkonen_Krause', 'xray_levels', 'elements',
+               'photoabsorption', 'scattering')
     result = False
     try:
         engine = make_engine(dbname)
         meta = MetaData() #
         meta.reflect(engine)
         result = all([t in meta.tables for t in _tables])
     except:
@@ -78,15 +79,15 @@
             parent, _ = os.path.split(__file__)
             dbname = os.path.join(parent, dbname)
             if not os.path.exists(dbname):
                 raise IOError("Database '%s' not found!" % dbname)
 
         if not isxrayDB(dbname):
             raise ValueError("'%s' is not a valid X-ray Database file!" % dbname)
-
+        self._cache = {}
         self.dbname = os.path.abspath(dbname)
         self.engine = make_engine(dbname)
         self.conn = self.engine.connect()
         kwargs = {}
         if read_only:
             kwargs = {'autoflush': True, 'autocommit': False}
 
@@ -98,41 +99,69 @@
         else:
             self.session = sessionmaker(bind=self.engine, **kwargs)()
 
         self.metadata = MetaData()
         self.metadata.reflect(self.engine)
         self.tables = self.metadata.tables
 
-        q = self.tables['elements'].select()
-        elems = self.session.execute(q).fetchall()
-        self.atomic_symbols = [e.element for e in elems]
+        elems = self.get_cache('elements')
+        self.__atomic_symbols = [e.element for e in elems]
+        self.__atomic_names = [e.name for e in elems]
 
     def close(self):
         "close session"
         self.session.flush()
         self.session.close()
 
     def query(self, *args, **kws):
         "generic query"
         return self.session.query(*args, **kws)
 
+    def get_cache(self, tablename, column=None, value=None):
+        """for some tables, we will just cache all the data"""
+        if column is None:
+            if tablename in self._cache:
+                rows = self._cache[tablename]
+            else:
+                q = self.tables[tablename].select()
+                rows = self.session.execute(q).fetchall()
+                self._cache[tablename] = rows
+                # print("cached ", tablename)
+        else:
+            if tablename in self._cache:
+                data = self._cache[tablename]
+            else:
+                data = self._cache[tablename] = {}
+
+            key = f"{column:s}_{repr(value)}"
+            if key not in data:
+                tab = self.tables[tablename]
+                col = getattr(tab.c, column, None)
+                if col is None:
+                    raise ValueError(f"now column {column} for table {tablename}")
+                data[key] = self.query(tab).filter(col==value).all()
+                # print("cached ", tablename, key)
+            if key in data:
+                rows = data[key]
+        return rows
+
+
     def get_version(self, long=False, with_history=False):
         """
         return sqlite3 database and python library version numbers
 
         Parameters:
             long (bool): show timestamp and notes of latest version [False]
             with_history (bool): show complete version history [False]
 
         Returns:
             string: version information
         """
         out = []
-        q = self.tables['Version'].select()
-        rows = self.session.execute(q).fetchall()
+        rows = self.get_cache('Version')
         if not with_history:
             rows = rows[-1:]
         if long or with_history:
             for row in rows:
                 out.append("XrayDB Version: %s [%s] '%s'" % (row.tag,
                                                              row.date,
                                                              row.notes))
@@ -163,20 +192,18 @@
 
         Notes:
             Z values from 1 to 98 (and symbols 'H' to 'Cf') are supported.
 
         References:
             Waasmaier and Kirfel
         """
-        wtab = self.tables['Waasmaier']
-        rows = self.query(wtab)
+        rows = self.get_cache('Waasmaier')
         if element is not None:
-            elem = self.symbol(element)
-            rows = rows.filter(wtab.c.element == elem)
-        return [str(r.ion) for r in rows.all()]
+            rows = [r for r in rows if r.element==element]
+        return [str(r.ion) for r in rows]
 
     def f0(self, ion, q):
         """
         return f0(q) -- elastic X-ray scattering factor from Waasmaier and Kirfel
 
         Parameters:
             ion (string, int, or None):  atomic number, symbol or ionic symbol
@@ -200,21 +227,25 @@
 
             Z values from 1 to 98 (and symbols 'H' to 'Cf') are supported.
             The list of ionic symbols can be read with the function .f0_ions()
 
         References:
             Waasmaier and Kirfel
         """
-        wtab = self.tables['Waasmaier']
+        f0_rows = self.get_cache('Waasmaier')
+        row = [None]
         if isinstance(ion, int):
-            row = self.query(wtab).filter(wtab.c.atomic_number == ion).all()[0]
-        elif ion not in self.f0_ions():
-            raise ValueError('No ion {:s} from Waasmaier table'.format(repr(ion)))
+            rows = [r for r in f0_rows if ion == r.atomic_number]
+            if len(rows) == 0:
+                raise ValueError(f'No ion {ion} from Waasmaier table')
         else:
-            row = self.query(wtab).filter(wtab.c.ion == ion.title()).all()[0]
+            rows = [r for r in f0_rows if ion.title() == r.ion]
+            if len(rows) == 0:
+                raise ValueError(f'No ion {ion} from Waasmaier table')
+        row = rows[0]
         q = as_ndarray(q)
         f0 = row.offset
         for s, e in zip(json.loads(row.scale), json.loads(row.exponents)):
             f0 += s * np.exp(-e*q*q)
         return f0
 
     def _from_chantler(self, element, energy, column='f1', smoothing=0):
@@ -225,21 +256,20 @@
             element (string or int): atomic number or symbol.
             eneregy (float or ndarray):
         columns: f1, f2, mu_photo, mu_incoh, mu_total
 
         Notes:
            this function is meant for internal use.
         """
-        ctab = self.tables['Chantler']
         elem = self.symbol(element)
-        row = self.query(ctab).filter(ctab.c.element == elem).one()
-
         energy = as_ndarray(energy)
         emin, emax = min(energy), max(energy)
 
+        row = self.get_cache('Chantler', column='element', value=elem)[0]
+
         te = np.array(json.loads(row.energy))
         nemin = max(0, -3 + max(np.where(te <= emin)[0]))
         nemax = min(len(te), 3 + max(np.where(te <= emax)[0]))
 
         te = te[nemin:nemax+1]
         if column == 'mu':
             column = 'mu_total'
@@ -345,27 +375,45 @@
         col = 'mu_total'
         if photo:
             col = 'mu_photo'
         elif incoh:
             col = 'mu_incoh'
         return self._from_chantler(element, energy, column=col)
 
+    def compton_energies(self, incident_energy):
+        """
+        return tuple of Compton energies for an incident energy
+        """
+        row = self.get_cache('Compton_energies')[0]
+        _en   = json.loads(row.incident)
+        _xe90 = json.loads(row.xray_90deg)
+        _xave = json.loads(row.xray_mean)
+        _eave = json.loads(row.electron_mean)
+
+        xray_90deg = np.interp(incident_energy, _en, _xe90)
+        xray_mean = np.interp(incident_energy, _en, _xave)
+        electron_mean = np.interp(incident_energy, _en, _eave)
+
+        return ComptonEnergies(incident_energy, xray_90deg, xray_mean, electron_mean)
+
     def _elem_data(self, element):
         "return data from elements table: internal use"
-        etab = self.tables['elements']
-        row = self.query(etab)
+
+        rows = self.get_cache('elements')
         if isinstance(element, int):
-            row = row.filter(etab.c.atomic_number == element).one()
+            row = [r for r in rows if r.atomic_number == element][0]
         else:
-            elem = element.title()
-            if not elem in self.atomic_symbols:
-                raise ValueError("unknown element '%s'" % repr(elem))
-            row = row.filter(etab.c.element == elem).one()
+            if element.title() in self.__atomic_symbols:
+                row = [r for r in rows if r.element == element.title()][0]
+            elif element.lower() in self.__atomic_names:
+                row = [r for r in rows if r.name == element.lower()][0]
+            else:
+                raise ValueError("unknown element '%s'" % repr(element))
         return ElementData(int(row.atomic_number),
-                           row.element.title(),
+                           row.element.title(), row.name,
                            row.molar_mass, row.density)
 
     def atomic_number(self, element):
         """
         return element's atomic number
 
         Parameters:
@@ -384,14 +432,26 @@
             element (string or int): atomic number or symbol
 
         Returns:
             string: element symbol
         """
         return self._elem_data(element).symbol
 
+    def atomic_name(self, element):
+        """
+        return element's name (English)
+
+        Parameters:
+            element (string or int): atomic number or symbol
+
+        Returns:
+            string: element name
+        """
+        return self._elem_data(element).name
+
     def molar_mass(self, element):
         """
         return molar mass of element
 
         Parameters:
             element (string or int): atomic number or symbol
 
@@ -634,19 +694,17 @@
             Elam, Ravel, and Sieber.
         """
         elem = self.symbol(element)
         kind = kind.lower()
         if kind not in ('coh', 'incoh', 'photo'):
             raise ValueError('unknown cross section kind=%s' % kind)
 
-        stab = self.tables['scattering']
-        if kind == 'photo':
-            stab = self. tables['photoabsorption']
+        tablename = 'photoabsorption' if kind == 'photo' else 'scattering'
 
-        row = self.query(stab).filter(stab.c.element == elem).all()[0]
+        row = self.get_cache(tablename, column='element', value=elem)[0]
 
         tab_lne = np.array(json.loads(row.log_energy))
         if kind.startswith('coh'):
             tab_val = np.array(json.loads(row.log_coherent_scatter))
             tab_spl = np.array(json.loads(row.log_coherent_scatter_spline))
         elif kind.startswith('incoh'):
             tab_val = np.array(json.loads(row.log_incoherent_scatter))
```

### Comparing `xraydb-4.5.0/xraydb/xraydb.sqlite` & `xraydb-4.5.1/xraydb/xraydb.sqlite`

 * *Files 0% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -5591,113 +5591,133 @@
 INSERT INTO Waasmaier VALUES(206,94,'Pu','Pu4+',3.4804080000000001682,'[15.416219, 32.610569, 22.256662, 0.719495, 15.518152]','[0.061456, 0.607938, 3.411848, 37.628792, 14.46436]');
 INSERT INTO Waasmaier VALUES(207,94,'Pu','Pu6+',3.5023249999999999104,'[15.436506, 32.289719, 14.726737, 15.012391, 7.024677]','[0.061815, 0.606541, 3.245363, 13.616438, 3.245364]');
 INSERT INTO Waasmaier VALUES(208,95,'Am','Am',3.5411600000000000854,'[33.435162, 23.657259, 15.576339, 3.027023, 15.7461]','[0.612785, 3.792942, 16.195778, 117.757004, 0.061755]');
 INSERT INTO Waasmaier VALUES(209,96,'Cm','Cm',3.3908399999999998541,'[15.804837, 33.480801, 24.150198, 3.655563, 15.499866]','[0.058619, 0.59016, 3.67472, 100.736191, 15.408296]');
 INSERT INTO Waasmaier VALUES(210,97,'Bk','Bk',3.2131690000000001639,'[15.889072, 33.625286, 24.710381, 3.707139, 15.839268]','[0.055503, 0.569571, 3.615472, 97.694786, 14.754303]');
 INSERT INTO Waasmaier VALUES(211,98,'Cf','Cf',3.0053260000000001639,'[33.794075, 25.467693, 16.048487, 3.657525, 16.008982]','[0.550447, 3.581973, 14.357388, 96.064972, 0.05245]');
 CREATE TABLE elements (atomic_number integer primary key,
-        element text, molar_mass real, density real);
-INSERT INTO elements VALUES(1,'H',1.0078000000000000291,8.9900000000000003241e-05);
-INSERT INTO elements VALUES(2,'He',4.0026000000000001577,0.00017860000000000000441);
-INSERT INTO elements VALUES(3,'Li',6.9400000000000003907,0.53400000000000003019);
-INSERT INTO elements VALUES(4,'Be',9.0121999999999999886,1.8500000000000000888);
-INSERT INTO elements VALUES(5,'B',10.810000000000000497,2.3399999999999998578);
-INSERT INTO elements VALUES(6,'C',12.010999999999999232,2.266999999999999904);
-INSERT INTO elements VALUES(7,'N',14.006999999999999673,0.0012509999999999999419);
-INSERT INTO elements VALUES(8,'O',15.999000000000000553,0.0014289999999999999317);
-INSERT INTO elements VALUES(9,'F',18.998400000000000176,0.0016960000000000000248);
-INSERT INTO elements VALUES(10,'Ne',20.179700000000000414,0.00090019999999999998022);
-INSERT INTO elements VALUES(11,'Na',22.989799999999998903,0.96799999999999997157);
-INSERT INTO elements VALUES(12,'Mg',24.304999999999999716,1.7379999999999999893);
-INSERT INTO elements VALUES(13,'Al',26.981500000000000483,2.7000000000000001776);
-INSERT INTO elements VALUES(14,'Si',28.085000000000000853,2.3290000000000001811);
-INSERT INTO elements VALUES(15,'P',30.973800000000000665,1.8229999999999999538);
-INSERT INTO elements VALUES(16,'S',32.060000000000002274,2.080000000000000071);
-INSERT INTO elements VALUES(17,'Cl',35.453000000000002955,3.2000000000000001776);
-INSERT INTO elements VALUES(18,'Ar',39.948000000000000397,0.0017839999999999999955);
-INSERT INTO elements VALUES(19,'K',39.09830000000000183,0.89000000000000001332);
-INSERT INTO elements VALUES(20,'Ca',40.078000000000002954,1.5500000000000000444);
-INSERT INTO elements VALUES(21,'Sc',44.955899999999999749,2.9849999999999998756);
-INSERT INTO elements VALUES(22,'Ti',47.866999999999997328,4.5060000000000002273);
-INSERT INTO elements VALUES(23,'V',50.941499999999997781,6.1100000000000003197);
-INSERT INTO elements VALUES(24,'Cr',51.996000000000002216,7.1500000000000003552);
-INSERT INTO elements VALUES(25,'Mn',54.938000000000002387,7.2099999999999999644);
-INSERT INTO elements VALUES(26,'Fe',55.844999999999998863,7.8600000000000003197);
-INSERT INTO elements VALUES(27,'Co',58.933199999999999361,8.9000000000000003552);
-INSERT INTO elements VALUES(28,'Ni',58.693399999999996906,8.9079999999999994741);
-INSERT INTO elements VALUES(29,'Cu',63.545999999999999373,8.9600000000000008526);
-INSERT INTO elements VALUES(30,'Zn',65.379999999999995454,7.1399999999999996802);
-INSERT INTO elements VALUES(31,'Ga',69.719999999999998862,5.9100000000000001421);
-INSERT INTO elements VALUES(32,'Ge',72.629999999999995453,5.3230000000000003979);
-INSERT INTO elements VALUES(33,'As',74.921599999999997977,5.7270000000000003126);
-INSERT INTO elements VALUES(34,'Se',78.971000000000003637,4.8099999999999996092);
-INSERT INTO elements VALUES(35,'Br',79.903999999999996361,3.1099999999999998756);
-INSERT INTO elements VALUES(36,'Kr',83.798000000000001817,0.0037490000000000001621);
-INSERT INTO elements VALUES(37,'Rb',85.467799999999996881,1.5320000000000000284);
-INSERT INTO elements VALUES(38,'Sr',87.620000000000004547,2.6400000000000001243);
-INSERT INTO elements VALUES(39,'Y',88.905799999999999272,4.4720000000000004192);
-INSERT INTO elements VALUES(40,'Zr',91.224000000000003748,6.5199999999999995736);
-INSERT INTO elements VALUES(41,'Nb',92.906400000000004977,8.5700000000000002842);
-INSERT INTO elements VALUES(42,'Mo',95.950000000000002838,10.27999999999999936);
-INSERT INTO elements VALUES(43,'Tc',97.906999999999996479,11.0);
-INSERT INTO elements VALUES(44,'Ru',101.06999999999999317,12.449999999999999289);
-INSERT INTO elements VALUES(45,'Rh',102.9060000000000059,12.410000000000000142);
-INSERT INTO elements VALUES(46,'Pd',106.4200000000000017,12.022999999999999687);
-INSERT INTO elements VALUES(47,'Ag',107.86799999999999499,10.490000000000000212);
-INSERT INTO elements VALUES(48,'Cd',112.41400000000000147,8.6500000000000003552);
-INSERT INTO elements VALUES(49,'In',114.81799999999999783,7.3099999999999996092);
-INSERT INTO elements VALUES(50,'Sn',118.70999999999999374,7.2649999999999996802);
-INSERT INTO elements VALUES(51,'Sb',121.76000000000000511,6.67900000000000027);
-INSERT INTO elements VALUES(52,'Te',127.59999999999999431,6.2400000000000002131);
-INSERT INTO elements VALUES(53,'I',126.90500000000000113,4.9329999999999998294);
-INSERT INTO elements VALUES(54,'Xe',131.29300000000000636,0.0058939999999999999336);
-INSERT INTO elements VALUES(55,'Cs',132.90500000000000113,1.8700000000000001065);
-INSERT INTO elements VALUES(56,'Ba',137.32699999999999818,3.5099999999999997868);
-INSERT INTO elements VALUES(57,'La',138.90500000000000113,6.1619999999999999218);
-INSERT INTO elements VALUES(58,'Ce',140.11600000000001386,6.7699999999999995736);
-INSERT INTO elements VALUES(59,'Pr',140.90799999999998703,6.7699999999999995736);
-INSERT INTO elements VALUES(60,'Nd',144.24199999999999022,7.0099999999999997868);
-INSERT INTO elements VALUES(61,'Pm',145.0,7.2599999999999997868);
-INSERT INTO elements VALUES(62,'Sm',150.36000000000001364,7.5199999999999995736);
-INSERT INTO elements VALUES(63,'Eu',151.96000000000000795,5.2439999999999997726);
-INSERT INTO elements VALUES(64,'Gd',157.24999999999999999,7.9000000000000003552);
-INSERT INTO elements VALUES(65,'Tb',158.92500000000001136,8.2300000000000004263);
-INSERT INTO elements VALUES(66,'Dy',162.5,8.5399999999999991473);
-INSERT INTO elements VALUES(67,'Ho',164.93000000000000681,8.7899999999999991473);
-INSERT INTO elements VALUES(68,'Er',167.25899999999998612,9.0660000000000007247);
-INSERT INTO elements VALUES(69,'Tm',168.93399999999999749,9.3200000000000002842);
-INSERT INTO elements VALUES(70,'Yb',173.04499999999998749,6.9000000000000003552);
-INSERT INTO elements VALUES(71,'Lu',174.96700000000001295,9.8409999999999993036);
-INSERT INTO elements VALUES(72,'Hf',178.4900000000000091,13.310000000000000497);
-INSERT INTO elements VALUES(73,'Ta',180.94800000000000749,16.690000000000001278);
-INSERT INTO elements VALUES(74,'W',183.84000000000000341,19.25);
-INSERT INTO elements VALUES(75,'Re',186.20699999999999363,21.019999999999999574);
-INSERT INTO elements VALUES(76,'Os',190.22999999999998976,22.589999999999999858);
-INSERT INTO elements VALUES(77,'Ir',192.21700000000001295,22.559999999999998721);
-INSERT INTO elements VALUES(78,'Pt',195.08400000000000318,21.449999999999999288);
-INSERT INTO elements VALUES(79,'Au',196.96700000000001295,19.30000000000000071);
-INSERT INTO elements VALUES(80,'Hg',200.59200000000001295,13.534000000000000696);
-INSERT INTO elements VALUES(81,'Tl',204.38300000000000978,11.849999999999999644);
-INSERT INTO elements VALUES(82,'Pb',207.19999999999998863,11.339999999999999857);
-INSERT INTO elements VALUES(83,'Bi',208.97999999999998976,9.7799999999999993605);
-INSERT INTO elements VALUES(84,'Po',209.0,9.1959999999999997299);
-INSERT INTO elements VALUES(85,'At',210.0,6.3499999999999996447);
-INSERT INTO elements VALUES(86,'Rn',222.0,0.009730000000000000801);
-INSERT INTO elements VALUES(87,'Fr',223.0,2.4799999999999999822);
-INSERT INTO elements VALUES(88,'Ra',226.0,5.5);
-INSERT INTO elements VALUES(89,'Ac',227.0,10.0);
-INSERT INTO elements VALUES(90,'Th',232.03800000000001091,11.699999999999999289);
-INSERT INTO elements VALUES(91,'Pa',231.03600000000000136,15.369999999999999218);
-INSERT INTO elements VALUES(92,'U',238.02899999999999635,19.100000000000001421);
-INSERT INTO elements VALUES(93,'Np',237.04800000000000182,20.199999999999999288);
-INSERT INTO elements VALUES(94,'Pu',239.05199999999999249,19.815999999999998948);
-INSERT INTO elements VALUES(95,'Am',243.0,12.0);
-INSERT INTO elements VALUES(96,'Cm',247.0,13.509999999999999786);
-INSERT INTO elements VALUES(97,'Bk',247.0,14.77999999999999936);
-INSERT INTO elements VALUES(98,'Cf',251.0,15.099999999999999644);
+        element text, name text, molar_mass real, density real);
+INSERT INTO elements VALUES(1,'H','hydrogen',1.0078000000000000291,8.9900000000000003241e-05);
+INSERT INTO elements VALUES(2,'He','helium',4.0026000000000001577,0.00017860000000000000441);
+INSERT INTO elements VALUES(3,'Li','lithium',6.9400000000000003907,0.53400000000000003019);
+INSERT INTO elements VALUES(4,'Be','beryllium',9.0121999999999999886,1.8500000000000000888);
+INSERT INTO elements VALUES(5,'B','boron',10.810000000000000497,2.3399999999999998578);
+INSERT INTO elements VALUES(6,'C','carbon',12.010999999999999232,2.266999999999999904);
+INSERT INTO elements VALUES(7,'N','nitrogen',14.006999999999999673,0.0012509999999999999419);
+INSERT INTO elements VALUES(8,'O','oxygen',15.999000000000000553,0.0014289999999999999317);
+INSERT INTO elements VALUES(9,'F','fluorine',18.998400000000000176,0.0016960000000000000248);
+INSERT INTO elements VALUES(10,'Ne','neon',20.179700000000000414,0.00090019999999999998022);
+INSERT INTO elements VALUES(11,'Na','sodium',22.989799999999998903,0.96799999999999997157);
+INSERT INTO elements VALUES(12,'Mg','magnesium',24.304999999999999716,1.7379999999999999893);
+INSERT INTO elements VALUES(13,'Al','aluminum',26.981500000000000483,2.7000000000000001776);
+INSERT INTO elements VALUES(14,'Si','silicon',28.085000000000000853,2.3290000000000001811);
+INSERT INTO elements VALUES(15,'P','phosphorus',30.973800000000000665,1.8229999999999999538);
+INSERT INTO elements VALUES(16,'S','sulfur',32.060000000000002274,2.080000000000000071);
+INSERT INTO elements VALUES(17,'Cl','chlorine',35.453000000000002955,3.2000000000000001776);
+INSERT INTO elements VALUES(18,'Ar','argon',39.948000000000000397,0.0017839999999999999955);
+INSERT INTO elements VALUES(19,'K','potassium',39.09830000000000183,0.89000000000000001332);
+INSERT INTO elements VALUES(20,'Ca','calcium',40.078000000000002954,1.5500000000000000444);
+INSERT INTO elements VALUES(21,'Sc','scandium',44.955899999999999749,2.9849999999999998756);
+INSERT INTO elements VALUES(22,'Ti','titanium',47.866999999999997328,4.5060000000000002273);
+INSERT INTO elements VALUES(23,'V','vanadium',50.941499999999997781,6.1100000000000003197);
+INSERT INTO elements VALUES(24,'Cr','chromium',51.996000000000002216,7.1500000000000003552);
+INSERT INTO elements VALUES(25,'Mn','manganese',54.938000000000002387,7.2099999999999999644);
+INSERT INTO elements VALUES(26,'Fe','iron',55.844999999999998863,7.8600000000000003197);
+INSERT INTO elements VALUES(27,'Co','cobalt',58.933199999999999361,8.9000000000000003552);
+INSERT INTO elements VALUES(28,'Ni','nickel',58.693399999999996906,8.9079999999999994741);
+INSERT INTO elements VALUES(29,'Cu','copper',63.545999999999999373,8.9600000000000008526);
+INSERT INTO elements VALUES(30,'Zn','zinc',65.379999999999995454,7.1399999999999996802);
+INSERT INTO elements VALUES(31,'Ga','gallium',69.719999999999998862,5.9100000000000001421);
+INSERT INTO elements VALUES(32,'Ge','germanium',72.629999999999995453,5.3230000000000003979);
+INSERT INTO elements VALUES(33,'As','arsenic',74.921599999999997977,5.7270000000000003126);
+INSERT INTO elements VALUES(34,'Se','selenium',78.971000000000003637,4.8099999999999996092);
+INSERT INTO elements VALUES(35,'Br','bromine',79.903999999999996361,3.1099999999999998756);
+INSERT INTO elements VALUES(36,'Kr','krypton',83.798000000000001817,0.0037490000000000001621);
+INSERT INTO elements VALUES(37,'Rb','rubidium',85.467799999999996881,1.5320000000000000284);
+INSERT INTO elements VALUES(38,'Sr','strontium',87.620000000000004547,2.6400000000000001243);
+INSERT INTO elements VALUES(39,'Y','yttrium',88.905799999999999272,4.4720000000000004192);
+INSERT INTO elements VALUES(40,'Zr','zirconium',91.224000000000003748,6.5199999999999995736);
+INSERT INTO elements VALUES(41,'Nb','niobium',92.906400000000004977,8.5700000000000002842);
+INSERT INTO elements VALUES(42,'Mo','molybdenum',95.950000000000002838,10.27999999999999936);
+INSERT INTO elements VALUES(43,'Tc','technetium',97.906999999999996479,11.0);
+INSERT INTO elements VALUES(44,'Ru','ruthenium',101.06999999999999317,12.449999999999999289);
+INSERT INTO elements VALUES(45,'Rh','rhodium',102.9060000000000059,12.410000000000000142);
+INSERT INTO elements VALUES(46,'Pd','palladium',106.4200000000000017,12.022999999999999687);
+INSERT INTO elements VALUES(47,'Ag','silver',107.86799999999999499,10.490000000000000212);
+INSERT INTO elements VALUES(48,'Cd','cadmium',112.41400000000000147,8.6500000000000003552);
+INSERT INTO elements VALUES(49,'In','indium',114.81799999999999783,7.3099999999999996092);
+INSERT INTO elements VALUES(50,'Sn','tin',118.70999999999999374,7.2649999999999996802);
+INSERT INTO elements VALUES(51,'Sb','antimony',121.76000000000000511,6.67900000000000027);
+INSERT INTO elements VALUES(52,'Te','tellurium',127.59999999999999431,6.2400000000000002131);
+INSERT INTO elements VALUES(53,'I','iodine',126.90500000000000113,4.9329999999999998294);
+INSERT INTO elements VALUES(54,'Xe','xenon',131.29300000000000636,0.0058939999999999999336);
+INSERT INTO elements VALUES(55,'Cs','cesium',132.90500000000000113,1.8700000000000001065);
+INSERT INTO elements VALUES(56,'Ba','barium',137.32699999999999818,3.5099999999999997868);
+INSERT INTO elements VALUES(57,'La','lanthanum',138.90500000000000113,6.1619999999999999218);
+INSERT INTO elements VALUES(58,'Ce','cerium',140.11600000000001386,6.7699999999999995736);
+INSERT INTO elements VALUES(59,'Pr','praseodymium',140.90799999999998703,6.7699999999999995736);
+INSERT INTO elements VALUES(60,'Nd','neodymium',144.24199999999999022,7.0099999999999997868);
+INSERT INTO elements VALUES(61,'Pm','promethium',145.0,7.2599999999999997868);
+INSERT INTO elements VALUES(62,'Sm','samarium',150.36000000000001364,7.5199999999999995736);
+INSERT INTO elements VALUES(63,'Eu','europium',151.96000000000000795,5.2439999999999997726);
+INSERT INTO elements VALUES(64,'Gd','gadolinium',157.24999999999999999,7.9000000000000003552);
+INSERT INTO elements VALUES(65,'Tb','terbium',158.92500000000001136,8.2300000000000004263);
+INSERT INTO elements VALUES(66,'Dy','dysprosium',162.5,8.5399999999999991473);
+INSERT INTO elements VALUES(67,'Ho','holmium',164.93000000000000681,8.7899999999999991473);
+INSERT INTO elements VALUES(68,'Er','erbium',167.25899999999998612,9.0660000000000007247);
+INSERT INTO elements VALUES(69,'Tm','thulium',168.93399999999999749,9.3200000000000002842);
+INSERT INTO elements VALUES(70,'Yb','ytterbium',173.04499999999998749,6.9000000000000003552);
+INSERT INTO elements VALUES(71,'Lu','lutetium',174.96700000000001295,9.8409999999999993036);
+INSERT INTO elements VALUES(72,'Hf','hafnium',178.4900000000000091,13.310000000000000497);
+INSERT INTO elements VALUES(73,'Ta','tantalum',180.94800000000000749,16.690000000000001278);
+INSERT INTO elements VALUES(74,'W','tungsten',183.84000000000000341,19.25);
+INSERT INTO elements VALUES(75,'Re','rhenium',186.20699999999999363,21.019999999999999574);
+INSERT INTO elements VALUES(76,'Os','osmium',190.22999999999998976,22.589999999999999858);
+INSERT INTO elements VALUES(77,'Ir','iridium',192.21700000000001295,22.559999999999998721);
+INSERT INTO elements VALUES(78,'Pt','platinum',195.08400000000000318,21.449999999999999288);
+INSERT INTO elements VALUES(79,'Au','gold',196.96700000000001295,19.30000000000000071);
+INSERT INTO elements VALUES(80,'Hg','mercury',200.59200000000001295,13.534000000000000696);
+INSERT INTO elements VALUES(81,'Tl','thallium',204.38300000000000978,11.849999999999999644);
+INSERT INTO elements VALUES(82,'Pb','lead',207.19999999999998863,11.339999999999999857);
+INSERT INTO elements VALUES(83,'Bi','bismuth',208.97999999999998976,9.7799999999999993605);
+INSERT INTO elements VALUES(84,'Po','polonium',209.0,9.1959999999999997299);
+INSERT INTO elements VALUES(85,'At','astatine',210.0,6.3499999999999996447);
+INSERT INTO elements VALUES(86,'Rn','radon',222.0,0.009730000000000000801);
+INSERT INTO elements VALUES(87,'Fr','francium',223.0,2.4799999999999999822);
+INSERT INTO elements VALUES(88,'Ra','radium',226.0,5.5);
+INSERT INTO elements VALUES(89,'Ac','actinium',227.0,10.0);
+INSERT INTO elements VALUES(90,'Th','thorium',232.03800000000001091,11.699999999999999289);
+INSERT INTO elements VALUES(91,'Pa','protactinium',231.03600000000000136,15.369999999999999218);
+INSERT INTO elements VALUES(92,'U','uranium',238.02899999999999635,19.100000000000001421);
+INSERT INTO elements VALUES(93,'Np','neptunium',237.04800000000000182,20.199999999999999288);
+INSERT INTO elements VALUES(94,'Pu','plutonium',239.05199999999999249,19.815999999999998948);
+INSERT INTO elements VALUES(95,'Am','americium',243.0,12.0);
+INSERT INTO elements VALUES(96,'Cm','curium',247.0,13.509999999999999786);
+INSERT INTO elements VALUES(97,'Bk','berkelium',247.0,14.77999999999999936);
+INSERT INTO elements VALUES(98,'Cf','californium',251.0,15.099999999999999644);
+INSERT INTO elements VALUES(99,'Es','einsteinium',252.0,8.8399999999999998578);
+INSERT INTO elements VALUES(100,'Fm','fermium',257.0,9.6999999999999992894);
+INSERT INTO elements VALUES(101,'Md','mendelevium',258.0,10.30000000000000071);
+INSERT INTO elements VALUES(102,'No','nobelium',259.0,9.9000000000000003552);
+INSERT INTO elements VALUES(103,'Lr','lawrencium',266.0,14.400000000000000355);
+INSERT INTO elements VALUES(104,'Rf','rutherfordium',267.0,17.0);
+INSERT INTO elements VALUES(105,'Db','dubnium',268.0,21.600000000000001421);
+INSERT INTO elements VALUES(106,'Sg','seaborgium',269.0,23.0);
+INSERT INTO elements VALUES(107,'Bh','bohrium',270.0,26.0);
+INSERT INTO elements VALUES(108,'Hs','hassium',269.0,27.0);
+INSERT INTO elements VALUES(109,'Mt','meitnerium',278.0,27.0);
+INSERT INTO elements VALUES(110,'Ds','darmstadtium',281.0,26.0);
+INSERT INTO elements VALUES(111,'Rg','roentgenium',282.0,22.0);
+INSERT INTO elements VALUES(112,'Cn','copernicium',285.0,14.0);
+INSERT INTO elements VALUES(113,'Nh','nihonium',286.0,16.0);
+INSERT INTO elements VALUES(114,'Fl','flerovium',289.0,11.400000000000000355);
+INSERT INTO elements VALUES(115,'Mc','moscovium',290.0,13.5);
+INSERT INTO elements VALUES(116,'Lv','livermorium',293.0,12.900000000000000355);
+INSERT INTO elements VALUES(117,'Ts','tennessine',294.0,7.0999999999999996447);
+INSERT INTO elements VALUES(118,'Og','oganesson',294.0,7.0);
 CREATE TABLE ionization_potentials (gas text,  potential real);
 INSERT INTO ionization_potentials VALUES('argon',26.399999999999998578);
 INSERT INTO ionization_potentials VALUES('helium',41.299999999999997156);
 INSERT INTO ionization_potentials VALUES('hydrogen',36.5);
 INSERT INTO ionization_potentials VALUES('nitrogen',34.799999999999997157);
 INSERT INTO ionization_potentials VALUES('air',33.799999999999997158);
 INSERT INTO ionization_potentials VALUES('oxygen',30.80000000000000071);
@@ -5719,14 +5739,16 @@
 INSERT INTO ionization_potentials VALUES('Ne',35.399999999999998579);
 INSERT INTO ionization_potentials VALUES('Kr',24.399999999999998578);
 INSERT INTO ionization_potentials VALUES('Xe',22.10000000000000142);
 INSERT INTO ionization_potentials VALUES('Si',3.6800000000000001598);
 INSERT INTO ionization_potentials VALUES('silicon',3.6800000000000001598);
 INSERT INTO ionization_potentials VALUES('Ge',2.9700000000000001953);
 INSERT INTO ionization_potentials VALUES('germanium',2.9700000000000001953);
+CREATE TABLE Compton_energies (incident text, xray_90deg text, xray_mean text, electron_mean text);
+INSERT INTO Compton_energies VALUES('[10.0, 11.0, 12.0, 13.0, 14.0, 15.0, 16.0, 17.0, 18.0, 19.0, 20.0, 22.0, 24.0, 25.0, 26.0, 28.0, 30.0, 33.0, 35.0, 38.0, 40.0, 43.0, 45.0, 48.0, 50.0, 55.0, 60.0, 65.0, 70.0, 75.0, 80.0, 85.0, 90.0, 95.0, 100.0, 110.0, 120.0, 130.0, 140.0, 150.0, 160.0, 170.0, 180.0, 190.0, 200.0, 220.0, 240.0, 250.0, 260.0, 280.0, 300.0, 330.0, 350.0, 380.0, 400.0, 430.0, 450.0, 480.0, 500.0, 550.0, 600.0, 650.0, 700.0, 750.0, 800.0, 850.0, 900.0, 950.0, 1000.0, 1100.0, 1200.0, 1300.0, 1400.0, 1500.0, 1600.0, 1700.0, 1800.0, 1900.0, 2000.0, 2200.0, 2400.0, 2500.0, 2600.0, 2800.0, 3000.0, 3300.0, 3500.0, 3800.0, 4000.0, 4300.0, 4500.0, 4800.0, 5000.0, 5500.0, 6000.0, 6500.0, 7000.0, 7500.0, 8000.0, 8500.0, 9000.0, 9500.0, 10000.0, 11000.0, 12000.0, 13000.0, 14000.0, 15000.0, 16000.0, 17000.0, 18000.0, 19000.0, 20000.0, 22000.0, 24000.0, 25000.0, 26000.0, 28000.0, 30000.0, 33000.0, 35000.0, 38000.0, 40000.0, 43000.0, 45000.0, 48000.0, 50000.0, 55000.0, 60000.0, 65000.0, 70000.0, 75000.0, 80000.0, 85000.0, 90000.0, 95000.0, 100000.0, 110000.0, 120000.0, 130000.0, 140000.0, 150000.0, 160000.0, 170000.0, 180000.0, 190000.0, 200000.0, 220000.0, 240000.0, 250000.0, 260000.0, 280000.0, 300000.0, 330000.0, 350000.0, 380000.0, 400000.0, 430000.0, 450000.0, 480000.0, 500000.0, 550000.0, 600000.0, 650000.0, 700000.0, 750000.0, 800000.0, 850000.0, 900000.0, 950000.0, 1000000.0]','[9.999804309, 10.99976321, 11.99971821, 12.99966928, 13.99961645, 14.9995597, 15.99949904, 16.99943446, 17.99936597, 18.99929357, 19.99921725, 21.99905288, 23.99887285, 24.99877697, 25.99867717, 27.99846583, 29.99823885, 32.99786902, 34.9976029, 37.99717437, 39.99686912, 42.9963819, 44.99603752, 47.99549161, 49.9951081, 54.99408086, 59.9929558, 64.99173293, 69.99041225, 74.98899376, 79.98747747, 84.98586338, 89.98415149, 94.9823418, 99.98043432, 109.976326, 119.9718265, 129.9669359, 139.9616543, 149.9559815, 159.9499177, 169.9434629, 179.9366171, 189.9293803, 199.9217526, 219.9053243, 239.8873325, 249.8777504, 259.8677774, 279.846659, 299.8239777, 329.7870256, 349.7604376, 379.7176262, 399.6871327, 429.638464, 449.6040661, 479.5495416, 499.5112404, 549.4086587, 599.2963238, 649.1742385, 699.0424057, 748.9008282, 798.749509, 848.5884508, 898.4176565, 948.2371289, 998.046871, 1097.637175, 1197.188592, 1296.701145, 1396.174856, 1495.609747, 1595.005842, 1694.363164, 1793.681734, 1892.961577, 1992.202713, 2190.56896, 2388.780655, 2487.828602, 2586.837979, 2784.741113, 2982.490237, 3278.825545, 3476.190428, 3771.950215, 3968.931975, 4264.117916, 4460.71767, 4755.331433, 4951.550289, 5441.432601, 5930.367363, 6418.357322, 6905.405214, 7391.513763, 7876.685685, 8360.923684, 8844.230455, 9326.60868, 9808.061034, 10768.19877, 11724.66484, 12677.48027, 13626.66592, 14572.24249, 15514.23053, 16452.65043, 17387.52241, 18318.86658, 19246.70284, 21091.93067, 22923.36237, 23833.95294, 24741.1521, 26545.45171, 28336.41082, 30998.1579, 32756.40594, 35369.75818, 37096.18321, 39662.44855, 41357.90679, 43878.34646, 45543.66367, 49655.46712, 53695.25986, 57664.91718, 61566.24982, 65401.00669, 69170.87755, 72877.49542, 76522.43902, 80107.23492, 83633.35976, 90515.26496, 97179.04285, 103634.9022, 109892.4246, 115960.6116, 121847.9284, 127562.3428, 133111.3615, 138502.0627, 143741.1265, 153789.2346, 163302.1564, 167871.1088, 172321.5408, 180884.8242, 189025.7503, 200511.1344, 207723.4037, 217934.7136, 224368.623, 233506.6883, 239281.7677, 247507.3218, 252719.8223, 264891.3295, 275967.2905, 286089.2488, 295375.3717, 303925.0846, 311822.6449, 319139.9284, 325938.6231, 332271.9722, 338186.1715]','[9.999804315, 10.99976322, 11.99971822, 12.9996693, 13.99961647, 14.99955972, 15.99949906, 16.99943449, 17.99936601, 18.99929361, 19.9992173, 21.99905295, 23.99887294, 24.99877707, 25.99867729, 27.99846598, 29.99823903, 32.99786926, 34.99760319, 37.99717474, 39.99686955, 42.99638243, 44.99603813, 47.99549235, 49.99510894, 54.99408197, 59.99295725, 64.99173477, 69.99041455, 74.98899659, 79.9874809, 84.98586749, 89.98415637, 94.98234754, 99.98044101, 109.9763349, 119.9718381, 129.9669506, 139.9616726, 149.9560041, 159.9499452, 169.9434958, 179.9366561, 189.9294262, 199.9218061, 219.9053956, 239.887425, 249.8778549, 259.867895, 279.8468059, 299.8241583, 329.7872659, 349.7607242, 379.7179931, 399.6875605, 429.6389953, 449.604675, 479.5502804, 499.5120754, 549.4097697, 599.2977657, 649.1760711, 699.0446938, 748.9036416, 798.7529222, 848.5925435, 898.4225132, 948.242839, 998.0535288, 1097.646031, 1197.200082, 1296.715743, 1396.193076, 1495.632143, 1595.033005, 1694.395723, 1793.720358, 1893.006972, 1992.255626, 2190.639294, 2388.871848, 2487.931608, 2586.953771, 2784.885544, 2982.667648, 3279.061215, 3476.471228, 3772.308883, 3969.349761, 4264.635914, 4461.310585, 4756.049606, 4952.360968, 5442.508108, 5931.759131, 6420.121098, 6907.600998, 7394.205754, 7879.942224, 8364.817198, 8848.837401, 9332.009493, 9814.340072, 10776.50276, 11735.37699, 12691.01331, 13643.4613, 14592.76962, 15538.98599, 16482.15725, 17422.32936, 18359.5474, 19293.85564, 21153.9156, 23002.84706, 23923.24178, 24840.97549, 26668.61446, 28486.06617, 31193.77689, 32987.01197, 35659.67126, 37430.35256, 40070.34466, 41819.99173, 44429.49666, 46159.49972, 50452.14529, 54700.9246, 58908.58694, 63077.65788, 67210.46007, 71309.13187, 75375.64412, 79411.81532, 83419.32518, 87399.72691, 95284.8519, 103077.4817, 110786.4914, 118419.5675, 125983.395, 133483.8129, 140925.9415, 148314.2901, 155652.8451, 162945.1448, 177403.2566, 191710.1114, 198812.3933, 205883.1353, 219936.6577, 233882.6138, 254621.4539, 268339.3407, 288771.3876, 302304.7062, 322485.0413, 335865.093, 355834.2702, 369084.5841, 402012.5008, 434687.8935, 467142.3697, 499401.9616, 531488.4126, 563420.0951, 595212.6843, 626879.6661, 658432.7267, 689882.058]','[0.000195685, 0.000236777, 0.000281783, 0.000330702, 0.000383534, 0.000440278, 0.000500936, 0.000565507, 0.000633991, 0.000706387, 0.000782696, 0.000947052, 0.001127058, 0.00122293, 0.001322714, 0.001534019, 0.001760972, 0.002130741, 0.002396814, 0.00282526, 0.003130448, 0.003617566, 0.003961867, 0.004507651, 0.004891062, 0.005918026, 0.00704275, 0.008265227, 0.00958545, 0.011003409, 0.012519098, 0.014132507, 0.01584363, 0.017652459, 0.019558985, 0.023665099, 0.028161909, 0.033049352, 0.038327365, 0.043995884, 0.050054847, 0.056504191, 0.063343853, 0.070573769, 0.078193878, 0.094604419, 0.112574972, 0.122145096, 0.132105034, 0.153194102, 0.175841674, 0.212734125, 0.239275756, 0.282006942, 0.312439494, 0.36100471, 0.395325048, 0.449719592, 0.487924584, 0.590230277, 0.70223431, 0.823928872, 0.955306163, 1.096358386, 1.247077757, 1.407456494, 1.577486827, 1.757160992, 1.946471233, 2.353968954, 2.799918092, 3.28425687, 3.806923633, 4.367856846, 4.966995095, 5.604277087, 6.279641648, 6.993027724, 7.744374381, 9.360706298, 11.12815231, 12.06839203, 13.04622921, 15.11445571, 17.33235237, 20.93878477, 23.5287716, 27.69111741, 30.65023869, 35.36408591, 38.68941461, 43.95039404, 47.63903153, 57.49189208, 68.24086854, 79.87890211, 92.39900217, 105.7942455, 120.0577756, 135.182802, 151.1625993, 167.9905069, 185.6599279, 223.4972381, 264.6230064, 308.986688, 356.538696, 407.2303807, 461.0140098, 517.8427492, 577.6706436, 640.4525982, 706.1443607, 846.0844045, 997.1529382, 1076.758215, 1159.024509, 1331.385538, 1513.933832, 1806.223106, 2012.98803, 2340.328737, 2569.647445, 2929.655345, 3180.008268, 3570.503339, 3840.500285, 4547.854709, 5299.0754, 6091.413064, 6922.342118, 7789.539927, 8690.868134, 9624.355876, 10588.18468, 11580.67482, 12600.27309, 14715.1481, 16922.51828, 19213.50856, 21580.43252, 24016.60496, 26516.18713, 29074.05846, 31685.70989, 34347.15492, 37054.85517, 42596.74337, 48289.88863, 51187.60669, 54116.8647, 60063.34229, 66117.38617, 75378.54613, 81660.6593, 91228.61242, 97695.29382, 107514.9587, 114134.907, 124165.7298, 130915.4159, 147987.4992, 165312.1065, 182857.6303, 200598.0384, 218511.5874, 236579.9049, 254787.3157, 273120.3339, 291567.2733, 310117.942]');
 CREATE TABLE KeskiRahkonen_Krause (id integer primary key,
         atomic_number integer, element text, edge text, width float);
 INSERT INTO KeskiRahkonen_Krause VALUES(1,1,'H','K',0.020099999999999999811);
 INSERT INTO KeskiRahkonen_Krause VALUES(2,2,'He','K',0.026900000000000000299);
 INSERT INTO KeskiRahkonen_Krause VALUES(3,3,'Li','K',0.035999999999999997279);
 INSERT INTO KeskiRahkonen_Krause VALUES(4,3,'Li','L1',0.11260000000000000563);
 INSERT INTO KeskiRahkonen_Krause VALUES(5,4,'Be','K',0.048300000000000002653);
@@ -9096,8 +9118,10 @@
 INSERT INTO Version VALUES(3,'3.0','2016-11-16 10:00:00','Fix Mz emission line (was M4,5-N6,7, now M4,5-N2,3)');
 INSERT INTO Version VALUES(4,'4.0','2017-11-15 13:00:00','Add Krause and Oliver data for improved core hole widths');
 INSERT INTO Version VALUES(5,'5.0','2020-07-15 11:38:00','Use elemental data (mass and density) from Wikipedia.');
 INSERT INTO Version VALUES(6,'6.0','2020-07-17 11:32:00','Add ionization potential values from Knoll.');
 INSERT INTO Version VALUES(7,'7.0','2020-08-02 08:25:00','Fix mu_total in Chantler table');
 INSERT INTO Version VALUES(8,'8.0','2020-08-13 10:25:00','Fix repeated energy for Mo in fine Chantler data');
 INSERT INTO Version VALUES(9,'8.1','2020-08-21 12:30:00','Add ionization potentials for Si/Ge PIN diodes');
+INSERT INTO Version VALUES(10,'9.0','2023-03-31 20:30:00','Add Compton table for mean X-ray and electron energies, X-ray energy scattered at 90 deg');
+INSERT INTO Version VALUES(11,'9.1','2023-08-02 13:20:00','Add element names to element table, include elements to Z=118');
 COMMIT;
```

### Comparing `xraydb-4.5.0/xraydb.egg-info/SOURCES.txt` & `xraydb-4.5.1/xraydb.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 .gitattributes
 LICENSE
 MANIFEST.in
 README
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
-versioneer.py
 examples/darwin_widths.py
 examples/mirror_comparison.py
 examples/mu_calcite.py
 examples/mu_components_C.py
 examples/mu_components_Fe.py
 examples/mu_elements.py
 examples/mu_water.py
 tests/test_chem_materials.py
 tests/test_xray.py
 tests/test_xraydb.py
 xraydb/__init__.py
-xraydb/_version.py
 xraydb/chemparser.py
 xraydb/materials.dat
 xraydb/materials.py
 xraydb/utils.py
+xraydb/version.py
 xraydb/xray.py
 xraydb/xraydb.py
 xraydb/xraydb.sqlite
 xraydb.egg-info/PKG-INFO
 xraydb.egg-info/SOURCES.txt
 xraydb.egg-info/dependency_links.txt
 xraydb.egg-info/requires.txt
```

