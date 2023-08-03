# Comparing `tmp/CRYSTALpytools-2023.7.6.tar.gz` & `tmp/CRYSTALpytools-2023.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CRYSTALpytools-2023.7.6.tar", last modified: Thu Jul  6 11:04:33 2023, max compression
+gzip compressed data, was "CRYSTALpytools-2023.8.3.tar", last modified: Thu Aug  3 14:27:30 2023, max compression
```

## Comparing `CRYSTALpytools-2023.7.6.tar` & `CRYSTALpytools-2023.8.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-07-06 11:04:33.185194 CRYSTALpytools-2023.7.6/
-drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-07-06 11:04:33.178927 CRYSTALpytools-2023.7.6/CRYSTALpytools/
--rw-r--r--   0 brunocamino   (501) staff       (20)      520 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/__init__.py
--rw-r--r--   0 brunocamino   (501) staff       (20)     1052 2023-06-28 14:24:12.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/adsorb.py
-drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-07-06 11:04:33.184692 CRYSTALpytools-2023.7.6/CRYSTALpytools/base/
--rw-r--r--   0 brunocamino   (501) staff       (20)      203 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/base/__init__.py
--rw-r--r--   0 brunocamino   (501) staff       (20)    11964 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/base/basisset.py
--rw-r--r--   0 brunocamino   (501) staff       (20)    50980 2023-07-06 11:02:41.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/base/crysd12.py
--rw-r--r--   0 brunocamino   (501) staff       (20)     7467 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/base/crysout.py
--rw-r--r--   0 brunocamino   (501) staff       (20)     9265 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/base/inputbase.py
--rw-r--r--   0 brunocamino   (501) staff       (20)    14464 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/base/propout.py
--rw-r--r--   0 brunocamino   (501) staff       (20)     1233 2023-06-28 14:24:12.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/calculate.py
--rw-r--r--   0 brunocamino   (501) staff       (20)    16954 2023-06-28 15:28:44.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/convert.py
--rw-r--r--   0 brunocamino   (501) staff       (20)   102312 2023-07-06 11:02:41.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/crystal_io.py
--rw-r--r--   0 brunocamino   (501) staff       (20)     4426 2023-06-28 14:24:12.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/execute.py
--rw-r--r--   0 brunocamino   (501) staff       (20)   162807 2023-07-06 11:02:41.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/plot.py
--rw-r--r--   0 brunocamino   (501) staff       (20)   122869 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/thermodynamics.py
--rw-r--r--   0 brunocamino   (501) staff       (20)    12902 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/unit_test.py
--rw-r--r--   0 brunocamino   (501) staff       (20)     1259 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/units.py
--rw-r--r--   0 brunocamino   (501) staff       (20)      693 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools/utils.py
-drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-07-06 11:04:33.181538 CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/
--rw-r--r--   0 brunocamino   (501) staff       (20)      706 2023-07-06 11:04:33.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/PKG-INFO
--rw-r--r--   0 brunocamino   (501) staff       (20)      717 2023-07-06 11:04:33.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/SOURCES.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)        1 2023-07-06 11:04:33.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/dependency_links.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)      138 2023-07-06 11:04:33.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/requires.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)       15 2023-07-06 11:04:33.000000 CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/top_level.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)     1167 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.7.6/LICENSE.txt
--rw-r--r--   0 brunocamino   (501) staff       (20)      706 2023-07-06 11:04:33.184981 CRYSTALpytools-2023.7.6/PKG-INFO
--rw-r--r--   0 brunocamino   (501) staff       (20)     4207 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.7.6/README.md
--rw-r--r--   0 brunocamino   (501) staff       (20)      105 2022-12-21 17:23:54.000000 CRYSTALpytools-2023.7.6/pyproject.toml
--rw-r--r--   0 brunocamino   (501) staff       (20)       38 2023-07-06 11:04:33.185239 CRYSTALpytools-2023.7.6/setup.cfg
--rw-r--r--   0 brunocamino   (501) staff       (20)     1190 2023-07-06 11:04:24.000000 CRYSTALpytools-2023.7.6/setup.py
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-08-03 14:27:30.626792 CRYSTALpytools-2023.8.3/
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-08-03 14:27:30.621387 CRYSTALpytools-2023.8.3/CRYSTALpytools/
+-rw-r--r--   0 brunocamino   (501) staff       (20)      520 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/__init__.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     1052 2023-06-28 14:24:12.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/adsorb.py
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-08-03 14:27:30.626444 CRYSTALpytools-2023.8.3/CRYSTALpytools/base/
+-rw-r--r--   0 brunocamino   (501) staff       (20)      244 2023-08-03 14:25:02.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/base/__init__.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    11964 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/base/basisset.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    50980 2023-07-06 11:14:53.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/base/crysd12.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     7467 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/base/crysout.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     9265 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/base/inputbase.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    54561 2023-08-03 14:25:02.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/base/plotbase.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    14464 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/base/propout.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     1233 2023-06-28 14:24:12.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/calculate.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    16954 2023-06-28 15:28:44.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/convert.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)   102690 2023-08-03 14:25:02.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/crystal_io.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     4426 2023-06-28 14:24:12.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/execute.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)   111316 2023-08-03 14:25:02.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/plot.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)   122869 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/thermodynamics.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)    12902 2023-06-06 15:10:07.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/unit_test.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)     1259 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/units.py
+-rw-r--r--   0 brunocamino   (501) staff       (20)      693 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools/utils.py
+drwxr-xr-x   0 brunocamino   (501) staff       (20)        0 2023-08-03 14:27:30.622687 CRYSTALpytools-2023.8.3/CRYSTALpytools.egg-info/
+-rw-r--r--   0 brunocamino   (501) staff       (20)      706 2023-08-03 14:27:30.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools.egg-info/PKG-INFO
+-rw-r--r--   0 brunocamino   (501) staff       (20)      749 2023-08-03 14:27:30.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools.egg-info/SOURCES.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)        1 2023-08-03 14:27:30.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools.egg-info/dependency_links.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)      138 2023-08-03 14:27:30.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools.egg-info/requires.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)       15 2023-08-03 14:27:30.000000 CRYSTALpytools-2023.8.3/CRYSTALpytools.egg-info/top_level.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)     1167 2022-09-15 16:48:47.000000 CRYSTALpytools-2023.8.3/LICENSE.txt
+-rw-r--r--   0 brunocamino   (501) staff       (20)      706 2023-08-03 14:27:30.626653 CRYSTALpytools-2023.8.3/PKG-INFO
+-rw-r--r--   0 brunocamino   (501) staff       (20)     4207 2023-06-28 12:35:39.000000 CRYSTALpytools-2023.8.3/README.md
+-rw-r--r--   0 brunocamino   (501) staff       (20)      105 2022-12-21 17:23:54.000000 CRYSTALpytools-2023.8.3/pyproject.toml
+-rw-r--r--   0 brunocamino   (501) staff       (20)       38 2023-08-03 14:27:30.626840 CRYSTALpytools-2023.8.3/setup.cfg
+-rw-r--r--   0 brunocamino   (501) staff       (20)     1190 2023-08-03 14:27:19.000000 CRYSTALpytools-2023.8.3/setup.py
```

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/__init__.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/__init__.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/adsorb.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/adsorb.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/base/basisset.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/base/basisset.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/base/crysd12.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/base/crysd12.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/base/crysout.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/base/crysout.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/base/inputbase.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/base/inputbase.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/base/propout.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/base/propout.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/calculate.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/calculate.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/convert.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/convert.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/crystal_io.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/crystal_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -817,41 +817,51 @@
                 begin = begin+i
         config_list = []
 
         # Read all the configurations
         for line in self.data[begin:]:
             if not re.match(r'^   WARNING', line):
                 config_list.extend(line.split())
+        '''multiplicity = []
+
+        for i in range(len(config_list)):
+            if config_list[i] == 'MULTIPLICITY' and i < len(config_list) - 1:
+                number = re.findall(r'\d+', config_list[i+1])
+                if number:
+                    config_list.append(int(number[0]))'''
+
         config_list = np.array(config_list)
         warning = np.where(config_list == 'WARNING')
         config_list = np.delete(config_list, warning)
         atom1_begin = np.where(config_list == original_atom)[0]
         atom1_end = np.where(
             config_list == dash_line)[0]
         atom2_begin = np.where(config_list == 'XX')[0]
         atom2_end = np.where(
             config_list == '<><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><>')[0]
         end = np.where(
             config_list == '===============================================================================')[0][-1]
         atom2_end = np.append(atom2_end, end)
         atom_type1 = []
         atom_type2 = []
-        multiplicity_tmp = config_list[np.where(config_list == 'MULTIPLICITY')[0]+2]
-        multiplicity = [int(x) for x in multiplicity_tmp]
+        if return_multiplicity == True:
+            multiplicity_tmp = config_list[np.where(config_list == 'MULTIPLICITY')[0]+2]
+            multiplicity = [int(re.sub(r'\D', '', x)) for x in multiplicity_tmp]
+            self.multiplicity = multiplicity
         config_list = config_list.tolist()
         for i in range(len(atom1_end)):
             atom_type1.append(
                 [int(x) for x in config_list[atom1_begin[i+1]+1:atom1_end[i]]])
             atom_type2.append(
                 [int(x) for x in config_list[atom2_begin[i]+1:atom2_end[i]]])
 
         self.atom_type1 = atom_type1
         self.atom_type2 = atom_type2
 
-        self.multiplicity = multiplicity
+        
         if return_multiplicity == True:
             return [self.atom_type1, self.atom_type2, multiplicity]
         else:
             return [self.atom_type1, self.atom_type2]
 
     def get_phonon(self, read_eigvt=False, rm_imaginary=True, rm_overlap=True,
                    imaginary_tol=-1e-4, q_overlap_tol=1e-4):
@@ -1533,23 +1543,14 @@
                     if s == (ncol - 1):
                         r += 1
                         s = 0
                     else:
                         s += 1
         return self
 
-    def read_cry_bands(self, properties_output):
-        """
-        Deprecated.
-        """
-        import warnings
-
-        warnings.warn('Deprecated. Use read_electron_band instead.')
-        return self.read_electron_band(properties_output)
-
     def read_electron_band(self, properties_output):
         """
         Generate bands object from CRYSTAL BAND.DAT or fort.25 file.
         Energy unit: eV.
 
         Args:
             properties_output (str): File name
@@ -1563,23 +1564,14 @@
         if '-%-' in self.data[0]: #fort.25 file format
             self.bands = BandsBASE.f25_parser(self.data)
         else: #BAND.DAT file format
             self.bands = BandsBASE.BAND_parser(self.data)
 
         return self.bands
 
-    def read_cry_doss(self, properties_output):
-        """
-        Deprecated.
-        """
-        import warnings
-
-        warnings.warn('Deprecated. Use read_electron_dos instead.')
-        return self.read_electron_dos(properties_output)
-
     def read_electron_dos(self, properties_output):
         """
         Generate doss object from CRYSTAL DOSS.DAT or fort.25 file.
         Energy unit: eV.
 
         Args:
             properties_output (str): File name
@@ -1593,14 +1585,32 @@
         if '-%-' in self.data[0]: #fort.25 file format
             self.doss = DOSBASE.f25_parser(self.data)
         else: #DOSS.DAT file format
             self.doss = DOSBASE.DOSS_parser(self.data)
 
         return self.doss
 
+    def read_cry_bands(self, properties_output):
+        """
+        Deprecated.
+        """
+        import warnings
+
+        warnings.warn('Deprecated. Use read_electron_band instead.')
+        return self.read_electron_band(properties_output)
+
+    def read_cry_doss(self, properties_output):
+        """
+        Deprecated.
+        """
+        import warnings
+
+        warnings.warn('Deprecated. Use read_electron_dos instead.')
+        return self.read_electron_dos(properties_output)
+
     def read_cry_contour(self, properties_output):
         """Read the CRYSTAL contour files to create the contour objects.
 
         Args:
             properties_output (str): The properties output file.
         Returns:
             Properties_output: The updated Properties_output object.
```

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/execute.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/execute.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/plot.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/plot.py`

 * *Files 26% similar despite different names*

```diff
@@ -402,14 +402,15 @@
 
     Raises:
         ValueError: If the specified unit is unknown.
 
     """
     import matplotlib.pyplot as plt
     from CRYSTALpytools.units import thz_to_cm, cm_to_thz
+    from CRYSTALpytools.base.plotbase import plot_cry_bands
     import re
 
     if re.match(r'^cm\-1$', unit, re.IGNORECASE):
         unit = 'cm-1'
         is_thz = False
     elif re.match(r'^THz$', unit, re.IGNORECASE):
         unit = 'THz'
@@ -483,14 +484,15 @@
 
     Raises:
         ValueError: If the specified unit is unknown.
 
     """
     import matplotlib.pyplot as plt
     from CRYSTALpytools.units import eV_to_H, H_to_eV
+    from CRYSTALpytools.base.plotbase import plot_cry_bands
     import re
 
     if re.match(r'^eV$', unit, re.IGNORECASE):
         unit = 'eV'
         is_ev = True
     elif re.match(r'^Hartree$', unit, re.IGNORECASE):
         unit = 'Hartree'
@@ -521,523 +523,14 @@
         fig.supylabel('$E-E_{F}$ (Hartree)')
 
     if save_to_file != None:
         save_plot(save_to_file)
 
     plt.show()
 
-def plot_cry_bands(bands, k_labels, energy_range, title, not_scaled, mode, linestl,
-                   linewidth, color, fermi, k_range, labels, figsize, scheme,
-                   sharex, sharey):
-    """
-    The base function to plot electron / phonon density of states.
-
-    Args:
-        bands (Union[List, object]): List of band objects or a single band object.
-        k_labels (Union[List[str], None]): List of strings specifying the labels for high symmetry points along the path.
-        energy_range (Union[List[Union[int, float]], None]): List of two integers or floats specifying the energy range (min, max).
-        title (Union[str, None]): Title of the plot.
-        not_scaled (bool): Flag indicating whether to scale the band structure for comparison.
-        mode (str): Mode of the plot ('single', 'multi', 'compare', 'surface').
-        linestl (Union[str, List[str]]): Line style or list of line styles for the bands.
-        linewidth (Union[int, List[int]]): Line width or list of line widths for the bands.
-        color (Union[str, List[str]]): Color or list of colors for the bands.
-        fermi (str): Color of the Fermi level.
-        k_range (Union[List[str], None]): List of two strings specifying the range of k points to plot.
-        labels (Union[List[str], None]): List of labels for the bands in multi-mode.
-        figsize (Union[Tuple[int, int], None]): Figure size.
-        scheme (Union[List[int], Tuple[int, int], None]): Subplot scheme in compare-mode (number of rows, number of columns).
-        sharex (Union[bool, str]): Flag or 'row' or 'col' specifying sharing of x-axis.
-        sharey (Union[bool, str]): Flag or 'row' or 'col' specifying sharing of y-axis.
-
-    Raises:
-        ValueError: If an invalid mode flag is specified or if there are errors in the input parameters.
-
-    Returns:
-        None
-    """
-    import matplotlib.pyplot as plt
-    # import matplotlib.lines as mlines
-    import numpy as np
-    import sys
-    import warnings
-
-    greek = {'Alpha': '\u0391', 'Beta': '\u0392', 'Gamma': '\u0393', 'Delta': '\u0394', 'Epsilon': '\u0395', 'Zeta': '\u0396', 'Eta': '\u0397',
-             'Theta': '\u0398', 'Iota': '\u0399', 'Kappa': '\u039A', 'Lambda': '\u039B', 'Mu': '\u039C', 'Nu': '\u039D', 'Csi': '\u039E',
-             'Omicron': '\u039F', 'Pi': '\u03A0', 'Rho': '\u03A1', 'Sigma': '\u03A3', 'Tau': '\u03A4', 'Upsilon': '\u03A5', 'Phi': '\u03A6',
-             'Chi': '\u03A7', 'Psi': '\u03A8', 'Omega': '\u03A9', 'Sigma_1': '\u03A3\u2081'}
-
-    # Error check on the mode flag
-    modes = ['single', 'multi', 'compare', 'surface']
-    if mode not in modes:
-        raise ValueError('The selected mode '+mode+' is not among the possible ones: ' + modes[0]+', ' + modes[1] + ', '+modes[2] + ', or '+modes[3])
-
-    # Error chenk on k_label
-    if k_labels is not None:
-
-        if isinstance(k_labels, list):
-            for element in k_labels:
-                if not isinstance(element, str):
-                    raise ValueError('k_label must be a list of strings:' +str(element)+' is not a string')
-
-            if isinstance(bands, list):
-                ref = bands[0].n_tick
-
-                for i, file in enumerate(bands):
-                    if file.n_tick != ref:
-                        i = str(i)
-                        raise ValueError('The ' + i + 'element your file list has a different number of High Symmetry Point!')
-            else:
-                ref = bands.n_tick
-
-            if len(k_labels) < ref:
-                diff = str(ref-len(k_labels))
-                raise ValueError('You are lacking ' + diff +' High Symmetry Points in k_labels!')
-
-            elif len(k_labels) > ref:
-                diff = str(len(k_labels)-ref)
-                raise ValueError('You have ' + diff + 'High Symmetry Points in excess in k_labels')
-
-        else:
-            raise ValueError('k_labels must be a list of strings')
-
-    # Error check on energy range
-    if energy_range != None:
-
-        if isinstance(energy_range, list):
-
-            if len(energy_range) > 2:
-                raise ValueError('energy_range must be a list of two int or float (min,max)')
-
-            for element in energy_range:
-                if (not isinstance(element, int)) and (not isinstance(element, float)):
-                    raise ValueError('energy_range must be a list of two int or float (min,max): ' +str(element)+', is neither a float or an int')
-
-        else:
-            raise ValueError('energy_range must be a list of two int or float (min,max)')
-
-    # Error check on k_range
-    if k_range is not None:
-        if isinstance(k_range, list):
-            if len(k_range) > 2:
-                raise ValueError('k_range must be a list of two strings')
-
-            for element in k_range:
-                if not isinstance(element, str):
-                    raise ValueError('k_label must be a list of two strings:' +str(element)+' is not a string')
-
-        else:
-            raise ValueError('k_range must be a list of two strings')
-
-    # Error check on title
-    if title != None:
-        if not isinstance(title, str):
-            raise ValueError('title needs to be a string')
-
-    if (mode == modes[0]) or (mode == modes[1]) or (mode == modes[3]):
-
-        # plotting of a single band object
-        if mode == modes[0]:
-
-            dx = bands.k_point_plot
-
-            pltband = bands.bands
-            no_bands = np.shape(pltband)[0]
-            ymin = np.amin(pltband)
-            ymax = np.amax(pltband)
-            xmin = min(dx)
-            xmax = max(dx)
-            count1 = 0
-            count2 = 0
-
-            # band plot
-            if figsize != None:
-                fig, ax = plt.subplots(nrows=1, ncols=1, sharex=sharex, sharey=sharey, figsize=figsize)
-            else:
-                fig, ax = plt.subplots(nrows=1, ncols=1, sharex=sharex, sharey=sharey)
-
-            for i in range(no_bands):
-
-                if bands.spin == 1:
-                    ax.plot(dx, pltband[i, :], color=color, linestyle=linestl, linewidth=linewidth)
-
-                elif bands.spin == 2:
-                    if count1 == count2:
-                        ax.plot(dx, pltband[i, :, 0], color='red',
-                                linestyle=linestl, linewidth=linewidth, label='Alpha')
-                        ax.plot(dx, pltband[i, :, 1], color='black',
-                                linestyle=linestl, linewidth=linewidth, label='Beta')
-                    else:
-                        ax.plot(dx, pltband[i, :, 0], color='red',
-                                 linestyle=linestl, linewidth=linewidth)
-                        ax.plot(dx, pltband[i, :, 1], color='black',
-                                linestyle=linestl, linewidth=linewidth)
-                    count1 += 1
-
-        # plot of multiple band objects on a single plot
-        elif mode == modes[1]:
-
-            # Error check on the band on the 'multi' mode flag
-            if not isinstance(bands, list):
-                raise ValueError('When you choose a ' +modes[1]+' plot bands needs to be a list of band objects')
-            # Error check on color for the 'multi' mode flag
-            if isinstance(color, list):
-                if len(color) != len(bands):
-                    raise ValueError('The number of colors is inconsistent with the number of objects you want to plot')
-            else:
-                color = ['dimgrey', 'blue', 'indigo', 'slateblue',
-                         'thistle', 'purple', 'orchid', 'crimson']
-
-            # Warning comparison with band.spin==2
-            for m in bands:
-                if m.spin == 2:
-                    warnings.warn("The 'multi' plot is not fully implemented at the moment for file with NSPIN = 2")
-
-            # scaling that enables the comparison of band structure calculated at different pressures
-            if not_scaled is False:
-                reference = xmax = np.amax(bands[0].k_point_plot)
-                xmin = np.amin(bands[0].k_point_plot)
-
-            else:
-                xmax = []
-                xmin = []
-
-            ymin = []
-            ymax = []
-
-            if figsize != None:
-                fig, ax = plt.subplots(nrows=1, ncols=1, sharex=sharex, sharey=sharey, figsize=figsize)
-            else:
-                fig, ax = plt.subplots(nrows=1, ncols=1, sharex=sharex, sharey=sharey)
-
-            # plot of all the bands obj present in the list
-            for index, data in enumerate(bands):
-                # scaling that enables the comparison of band structure calculated at different pressures
-                if not_scaled == False:
-                    k_max = np.amax(data.k_point_plot)
-                    dx = (data.k_point_plot/k_max)*reference
-                else:
-                    dx = data.k_point_plot
-                    xmin.append(np.amin(dx))
-                    xmax.append(np.amax(dx))
-
-                pltband = data.bands
-                no_bands = np.shape(pltband)[0]
-                ymin.append(np.amin(pltband))
-                ymax.append(np.amax(pltband))
-
-                count1 = 0
-                count2 = 0
-
-                # Effective plot
-                for j in range(no_bands):
-
-                    if (count1 == count2) and (labels is not None):
-                        if data.spin == 1:
-                            if isinstance(linestl, list):
-                                if isinstance(linewidth, list):
-                                    ax.plot(dx, pltband[j, :], color=color[index],
-                                            linestyle=linestl[index], linewidth=linewidth[index], label=labels[index])
-                                else:
-                                    ax.plot(dx, pltband[j, :], color=color[index],
-                                            linestyle=linestl[index], linewidth=linewidth, label=labels[index])
-                            else:
-                                if isinstance(linewidth, list):
-                                    ax.plot(dx, pltband[j, :], color=color[index],
-                                            linestyle=linestl, linewidth=linewidth[index], label=labels[index])
-                                else:
-                                    ax.plot(dx, pltband[j, :], color=color[index],
-                                            linestyle=linestl, linewidth=linewidth, label=labels[index])
-                        elif data.spin == 2:
-                            ax.plot(dx, pltband[j, :, 0], color=color[index],
-                                    linestyle=linestl, linewidth=linewidth, label=labels[index]+' Alpha')
-                            ax.plot(dx, pltband[j, :, 1], color=color[index],
-                                    linestyle='--', linewidth=linewidth, label=labels[index]+' Beta')
-
-                    else:
-                        if data.spin == 1:
-                            if isinstance(linestl, list):
-                                if isinstance(linewidth, list):
-                                    ax.plot(dx, pltband[j, :], color=color[index],
-                                            linestyle=linestl[index], linewidth=linewidth[index])
-                                else:
-                                    ax.plot(dx, pltband[j, :], color=color[index],
-                                            linestyle=linestl[index], linewidth=linewidth)
-                            else:
-                                if isinstance(linewidth, list):
-                                    ax.plot(dx, pltband[j, :], color=color[index],
-                                            linestyle=linestl, linewidth=linewidth[index])
-                                else:
-                                    ax.plot(dx, pltband[j, :], color=color[index],
-                                            linestyle=linestl, linewidth=linewidth)
-                        elif data.spin == 2:
-                            ax.plot(dx, pltband[j, :, 0], color=color[index],
-                                    linestyle=linestl, linewidth=linewidth)
-                            ax.plot(dx, pltband[j, :, 1], color=color[index],
-                                    linestyle='--', linewidth=linewidth)
-
-                    count1 += 1
-
-            if (isinstance(xmin, list)) or (isinstance(xmax, list)):
-                xmin = min(xmin)
-                xmax = max(xmax)
-
-            ymin = min(ymin)
-            ymax = max(ymax)
-
-        if mode == modes[3]:
-            warnings.warn('The surface bands is not ready yet')
-            sys.exit(0)
-
-        # HSP line plot
-        if isinstance(bands, list):
-            hsp = bands[0].tick_position
-        else:
-            hsp = bands.tick_position
-
-        if k_labels is not None:
-            if len(hsp) != len(k_labels):
-                if len(hsp) > len(k_labels):
-                    raise ValueError('You have specified a number of label smalle than the number of High Simmetry Point along the path')
-                elif len(hsp) < len(k_labels):
-                    raise ValueError('You have more labels than the High Simmetry point along the path')
-
-        hsp[len(hsp)-1] = xmax
-
-        y_band = np.linspace(ymin*1.05, ymax*1.05, 2)
-
-        for j in hsp:
-            x_band = np.ones(2)*j
-            ax.plot(x_band, y_band, color='black', linewidth=0.5)
-
-        # plot of the fermi level
-        x = np.linspace(xmin, xmax, 2)
-        y = np.zeros(2)
-        ax.plot(x, y, color=fermi, linewidth=2.5)
-
-        # definition of the plot title
-        if title is not None:
-            fig.suptitle(title)
-
-        if not isinstance(bands, list):
-            if bands.spin == 2:
-                fig.legend()
-        else:
-            if labels is not None:
-                fig.legend()
-
-    # compare mode plot
-    elif mode == modes[2]:
-
-        # Error check on type(bands)
-        if not isinstance(bands, list):
-            raise ValueError('When you choose a ' +modes[2]+' plot bands needs to be a list of band objects')
-        # Error check on sharex and sharey option
-        if (not isinstance(sharex, bool)) or (not isinstance(sharey, bool)):
-            accepted_str = ['row', 'col']
-
-            if (isinstance(sharex, str)) or (isinstance(sharey, str)):
-                if sharex not in accepted_str:
-                    raise ValueError('sharex can only be equal to row or col')
-                elif sharey not in accepted_str:
-                    raise ValueError('sharey can only be equal to row or col')
-            else:
-                raise ValueError('sharex and sharey have to be boolean')
-
-        # Error check and definition of scheme
-        if scheme is None:
-            n_rows = 1
-            n_col = len(bands)
-        else:
-            if (not isinstance(scheme, tuple)) and (not isinstance(scheme, list)):
-                raise ValueError('scheme needs to be a tuple or a list')
-                sys.exit(1)
-            elif len(scheme) > 2:
-                raise ValueError('scheme needs to be a tuple or a list of two elements (nrow,ncol)')
-            else:
-                n_rows = scheme[0]
-                n_col = scheme[1]
-        # Creation of the subplots
-        if figsize is None:
-            fig, axs = plt.subplots(nrows=n_rows, ncols=n_col,
-                                    sharex=sharex, sharey=sharey, figsize=figsize)
-        else:
-            fig, axs = plt.subplots(nrows=n_rows, ncols=n_col,
-                                    sharex=sharex, sharey=sharey, figsize=figsize)
-        if n_rows == 1 and n_col == 1: # When axs is not a list
-            axs = [axs]
-        # Scaling with different size of the same brillouin zone
-        if not_scaled is False:
-            reference = xmax = np.amax(bands[0].k_point_plot)
-            xmin = np.amin(bands[0].k_point_plot)
-
-        else:
-            xmax = []
-            xmin = []
-
-        ymin = []
-        ymax = []
-        count3 = 0
-
-        # Plot of the different band structure into the subplots
-        for col in range(n_col):
-            for row in range(n_rows):
-                data = bands[count3]
-                if count3 == 0:
-                    hsp = data.tick_position
-                pltband = data.bands
-                no_bands = np.shape(pltband)[0]
-                if not_scaled is False:
-                    k_max = np.amax(data.k_point_plot)
-                    dx = (data.k_point_plot/k_max)*reference
-                else:
-                    dx = data.k_point_plot
-                    xmin.append(np.amin(dx))
-                    xmax.append(np.amax(dx))
-                ymin.append(np.amin(pltband))
-                ymax.append(np.amax(pltband))
-                # Effective plotting action
-                for j in range(no_bands):
-                    if data.spin == 1:
-                        if n_rows == 1:
-                            axs[col].plot(
-                                dx, pltband[j, :], color=color, linestyle=linestl, linewidth=linewidth)
-                        else:
-                            axs[row, col].plot(
-                                dx, pltband[j, :], color=color, linestyle=linestl, linewidth=linewidth)
-                    elif data.spin == 2:
-                        if n_rows == 1:
-                            axs[col].plot(dx, pltband[j, :, 0], color=color,
-                                          linestyle='-', linewidth=linewidth, label='Alpha')
-                            axs[col].plot(dx, pltband[j, :, 0], color=color,
-                                          linestyle='--', linewidth=linewidth, label='Beta')
-                        else:
-                            axs[row, col].plot(
-                                dx, pltband[j, :, 0], color=color, linestyle='-', linewidth=linewidth, label='Alpha')
-                            axs[row, col].plot(
-                                dx, pltband[j, :, 0], color=color, linestyle='--', linewidth=linewidth, label='Beta')
-
-                # Plot of the HSPs lines
-                yhsp = np.linspace(np.amin(pltband)+5, np.amax(pltband)+5, 2)
-                for j in hsp:
-                    xhsp = np.ones(2)*j
-                    if n_rows == 1:
-                        axs[col].plot(
-                            xhsp, yhsp, color='black', linewidth=0.5)
-                    else:
-                        axs[row, col].plot(
-                            xhsp, yhsp, color='black', linewidth=0.5)
-
-                # Fermi level line plot
-                xfermi = np.linspace(np.amin(pltband), np.amax(pltband), 2)
-                yfermi = np.zeros(2)
-                if n_rows == 1:
-                    axs[col].plot(
-                        xfermi, yfermi, color=fermi, linewidth=2.5)
-                else:
-                    axs[row, col].plot(
-                        xfermi, yfermi, color=fermi, linewidth=2.5)
-
-                # Definition of x and y limits
-                if n_rows == 1:
-                    if sharex is not True:
-                        """hsp_label = []
-                        for element in k_labels:
-                            if element in k_labels:
-                                g = greek.get(element)
-                                hsp_label.append(g)
-                        axs[col].set_xticks(hsp)
-                        if k_labels is not None:
-                            axs[col].set_xlabels(hsp_label)"""
-                        warnings.warn('The sharex = False option has not been developed yet')
-                    axs[col].set_xlim([np.amin(dx), np.amax(dx)])
-                    if (sharey is not True) and (energy_range is not None):
-                        axs[col].set_ylim([energy_range[0], energy_range[1]])
-                    else:
-                        axs[col].set_ylim([np.amin(pltband), np.amax(pltband)])
-                else:
-                    if sharex is not True:
-                        """hsp_label = []
-                        for element in k_labels:
-                            if element in k_labels:
-                                g = greek.get(element)
-                                hsp_label.append(g)
-                        axs[row, col].set_xticks(hsp)
-                        if k_labels is not None:
-                            axs[row, col].set_xlabels(hsp_label)"""
-                        warnings.warn('The sharex = False option has not been developed yet')
-                    axs[row, col].set_xlim([np.amin(dx), np.amax(dx)])
-                    if (sharey is not True) and (energy_range is not False):
-                        axs[row, col].set_ylim(
-                            [energy_range[0], energy_range[1]])
-                    else:
-                        axs[row, col].set_ylim(
-                            [np.amin(pltband), np.amax(pltband)])
-
-                count3 += 1
-
-        if (isinstance(ymin, list)) or (isinstance(ymax, list)):
-            ymin = min(ymin)
-            ymax = max(ymax)
-
-    hsp_label = []
-    high_sym_point = []
-    if k_labels is not None:
-        for n in k_labels:
-            if n in greek:
-                g = greek.get(n)
-                hsp_label.append(g)
-                high_sym_point.append(n)
-            else:
-                hsp_label.append(n)
-                high_sym_point.append(n)
-
-    # give the possibility through the k_range to select a shorter path than the one calculated
-    high_sym_point2 = high_sym_point
-    count = 0
-    for i in high_sym_point2:
-        repeat = high_sym_point2.count(i)
-        if repeat != 1:
-            for p in range(0, len(high_sym_point2)):
-                if p != count:
-                    repeat_count = 1
-                    q = high_sym_point2[p]
-                    r = high_sym_point[p]
-                    if (q == i) & (q == r):
-                        high_sym_point2[p] = i+str(repeat_count)
-                        repeat_count += 1
-                        if repeat_count > repeat:
-                            repeat_count = 0
-        count += 1
-
-    path_dict = dict(zip(high_sym_point2, hsp))
-
-    # definition of the ylim
-    if (energy_range != None) and (sharey == True):
-        ymin = energy_range[0]
-        ymax = energy_range[1]
-
-    # definition of the xlim
-    if k_range != None:
-        xmin = path_dict[k_range[0]]
-        xmax = path_dict[k_range[1]]
-
-    if k_labels != None:
-        plt.xticks(hsp, hsp_label)
-    else:
-        plt.xticks(hsp)
-
-    plt.ylim(ymin, ymax)
-    if (mode == modes[0]) or (mode == modes[1]):
-        plt.xlim(xmin, xmax)
-    elif (mode == modes[2]) and (k_range is not None):
-        warnings.warn('The k_range is not available yet for the compare mode')
-
-    return fig
-
 
 def plot_electron_dos(doss, unit='eV', beta='up', overlap=False, prj=None,
                       energy_range=None, dos_range=None, color='blue',
                       labels=None, linestl=None, linewidth=1, fermi='forestgreen',
                       title=None, figsize=None, save_to_file=None):
     """
     A wrapper of plot_cry_doss for electron density of states.
@@ -1065,14 +558,15 @@
         save_to_file (str): File name.
 
     Returns:
         None
     """
     import matplotlib.pyplot as plt
     from CRYSTALpytools.units import H_to_eV, eV_to_H
+    from CRYSTALpytools.base.plotbase import plot_cry_doss
     import re
 
     if re.match(r'^ev$', unit, re.IGNORECASE):
         unit = 'eV'
         is_ev = True
     elif re.match(r'^hartree$', unit, re.IGNORECASE):
         unit = 'Hartree'
@@ -1107,14 +601,15 @@
         fig.supxlabel('Energy (Hartree)')
 
     if save_to_file != None:
         save_plot(save_to_file)
 
     plt.show()
 
+
 def plot_phonon_dos(doss, unit='cm-1', overlap=False, prj=None,
                     freq_range=None, dos_range=None, color='blue',
                     labels=None, linestl=None, linewidth=1, line_freq0=None,
                     title=None, figsize=None, save_to_file=None):
     """
     A wrapper of plot_cry_doss for electron density of states.
 
@@ -1140,14 +635,15 @@
         save_to_file (str): File name.
 
     Returns:
         None
     """
     import matplotlib.pyplot as plt
     from CRYSTALpytools.units import cm_to_thz, thz_to_cm
+    from CRYSTALpytools.base.plotbase import plot_cry_doss
     import re
 
     if re.match(r'^cm\-1$', unit, re.IGNORECASE):
         unit = 'cm-1'
         is_thz = False
     elif re.match(r'^thz$', unit, re.IGNORECASE):
         unit = 'THz'
@@ -1186,379 +682,14 @@
         fig.supxlabel('Frequency (cm$^{-1}$)')
 
     if save_to_file != None:
         save_plot(save_to_file)
 
     plt.show()
 
-def plot_cry_doss(doss, color, fermi, overlap, labels, figsize, linestl,
-                  linewidth, title, beta, energy_range, dos_range, prj):
-    """
-    The base function to plot electron / phonon density of states.
-
-    Args:
-        doss (object): The density of states object.
-        color (str or list): The color(s) of the plot(s).
-        fermi (str): The color of the Fermi level line.
-        overlap (bool): True if the projections should overlap, False otherwise.
-        labels (str or list): The label(s) for the plot(s).
-        figsize (tuple): The figure size (width, height) in inches.
-        linestl (str or list): The line style(s) for the plot(s).
-        linewidth (float): The width of the line(s) in points.
-        title (str): The title of the plot.
-        beta (str): The beta value ('up' or 'down').
-        energy_range (tuple): The energy range (xmin, xmax) for the x-axis.
-        dos_range (tuple): The density of states range (ymin, ymax) for the y-axis.
-        prj (None or list): The projection(s) to plot.
-
-    Returns:
-        None
-    """
-    import matplotlib.pyplot as plt
-    import numpy as np
-    import sys
-    import warnings
-    from os import path
-
-    # Error check on beta
-    accepted_beta = ['up', 'down']
-    if beta not in accepted_beta:
-        raise ValueError("Beta can be defined only as: 'up' or 'down'.")
-
-    # Plot for overlap == True
-    if overlap == True:
-
-        # Error check on color for color in overlap == true and default list of color
-        if (not isinstance(color, list)) and (doss.n_proj > 1):
-            warnings.warn('When overlap is true color has to be a list!', stacklevel=2)
-            color = ['blue', 'indigo', 'midgrey', 'crimson']
-            if (len(color) < doss.n_proj) or (len(color) < len(prj)):
-                raise ValueError('When overlap is true color has to be a list!')
-
-        # Error check on labels for overlap == true
-        if labels is not None:
-            if not isinstance(labels, list) and (doss.n_proj > 1):
-                raise ValueError('When overlap is true labels has to be a list')
-
-        # Default for figsize
-        if figsize is None:
-            figsize = (12, 5)
-
-        # Error check on color, labels, and linestl
-        if (isinstance(color, list)) or (isinstance(labels, list)) or (isinstance(linestl, list)):
-            if color is not None:
-                if prj is None:
-                    if (len(color) > doss.n_proj) or (len(color) < doss.n_proj):
-                        if len(color) > doss.n_proj:
-                            raise ValueError('The number of colors is greater than the number of projections!')
-                        elif len(color) < doss.n_proj:
-                            raise ValueError('The number of colors is less than the number of projections!')
-                else:
-                    if (len(color) > len(prj)) or (len(color) < len(prj)):
-                        if len(color) > len(prj):
-                            raise ValueError('The number of colors is greater than the number of projections required!')
-                        elif len(color) < len(prj):
-                            raise ValueError('The number of colors is less than the number of projections required!')
-
-            if labels is not None:
-                if prj is None:
-                    if (len(labels) > doss.n_proj) or (len(labels) < doss.n_proj):
-                        if len(labels) > doss.n_proj:
-                            raise ValueError('The number of labels is greater than the number of projections!')
-                        elif len(labels) < doss.n_proj:
-                            raise ValueError('The number of labels is less than the number of projections!')
-                else:
-                    if (len(labels) > len(prj)) or (len(labels) < len(prj)):
-                        if len(labels) > len(prj):
-                            raise ValueError('The number of labels is greater than the number of projections required!')
-                        elif len(color) < len(prj):
-                            raise ValueError('The number of labels is less than the number of projections required!')
-
-            if linestl is not None:
-                if prj is None:
-                    if (len(linestl) > doss.n_proj) or (len(linestl) < doss.n_proj):
-                        if len(linestl) > doss.n_proj:
-                            raise ValueError('The number of linestl is greater than the number of projections!')
-                        elif len(linestl) < doss.n_proj:
-                            raise ValueError('The number of linestl is less than the number of projections!')
-                else:
-                    if (len(linestl) > len(prj)) or (len(linestl) < len(prj)):
-                        if len(linestl) > len(prj):
-                            raise ValueError('The number of linestl is greater than the number of projections required!')
-                        elif len(color) < len(prj):
-                            raise ValueError('The number of linestl is less than the number of projections required!')
-
-        # Creation of the figure
-        fig, ax = plt.subplots(nrows=1, ncols=1, figsize=figsize)
-        # Creation of dx for the plot
-        if doss.spin == 1:
-            dx = doss.doss[:, 0]
-        elif doss.spin == 2:
-            dx = doss.doss[:, 0, :]
-            dx_alpha = doss.doss[:, 0, 0]
-            dx_beta = doss.doss[:, 0, 1]
-
-        # Determination of xmin, xmax, ymin, and ymax
-        xmin = np.amin(dx)
-        xmax = np.amax(dx)
-        ymin = np.amin(doss.doss[1:, :, :])
-        ymax = np.amax(doss.doss[1:, :, :])
-
-        # Plot of all projections
-        if prj == None:
-            for projection in range(1, doss.n_proj+1):
-                # for projection in range(1, 2):
-                if doss.spin == 1:
-                    if doss.n_proj > 1:
-                        if linestl is None:
-                            ax.plot(dx, doss.doss[:, projection], color=color[projection-1],
-                                    label=labels[projection-1], linewidth=linewidth)
-                        else:
-                            ax.plot(dx, doss.doss[:, projection], color=color[projection-1],
-                                    label=labels[projection-1], linestyle=linestl[projection-1], linewidth=linewidth)
-                    else:
-                        ax.plot(dx, doss.doss[:, projection], color=color, linewidth=linewidth)
-                elif doss.spin == 2:
-                    if beta == accepted_beta[0]:
-                        if doss.n_proj > 1:
-                            ax.plot(dx_alpha, doss.doss[:, projection, 0], color=color[projection-1],
-                                    label=labels[projection-1], linestyle='-', linewidth=linewidth)
-                            ax.plot(dx_beta, -doss.doss[:, projection, 1], color=color[projection-1],
-                                    label=labels[projection-1], linestyle='--', linewidth=linewidth)
-                        else:
-                            ax.plot(dx_alpha, doss.doss[:, projection, 0],
-                                    linestyle='-', linewidth=linewidth)
-                            ax.plot(dx_beta, -doss.doss[:, projection, 1],
-                                    linestyle='--', linewidth=linewidth)
-                    elif beta == accepted_beta[1]:
-                        if doss.n_proj > 1:
-                            ax.plot(dx_alpha, doss.doss[:, projection, 0], color=color[projection-1],
-                                    label=labels[projection-1], linestyle='-', linewidth=linewidth)
-                            ax.plot(dx_beta, doss.doss[:, projection, 1], color=color[projection-1],
-                                    label=labels[projection-1], linestyle='--', linewidth=linewidth)
-
-                        else:
-                            ax.plot(dx_alpha, doss.doss[:, projection, 0], color=color,
-                                    linestyle='-', linewidth=linewidth)
-                            ax.plot(dx_beta, doss.doss[:, projection, 1], color=color,
-                                    linestyle='--', linewidth=linewidth)
-
-        # Plot of selected projections
-        else:
-            for index, projection in enumerate(prj):
-                if doss.spin == 1:
-                    if doss.n_proj > 1:
-                        if linestl is None:
-                            ax.plot(dx, doss.doss[:, projection], color=color[index],
-                                    label=labels[index], linewidth=linewidth)
-                        else:
-                            ax.plot(dx, doss.doss[:, projection], color=color[index],
-                                    label=labels[index], linestyle=linestl[index], linewidth=linewidth)
-                    else:
-                        ax.plot(dx, doss.doss[:, projection], color=color, linewidth=linewidth)
-                elif doss.spin == 2:
-                    if beta == accepted_beta[0]:
-                        if doss.n_proj > 1:
-                            ax.plot(dx_alpha, doss.doss[:, projection, 0], color=color[index],
-                                    label=labels[index], linestyle='-', linewidth=linewidth)
-                            ax.plot(dx_beta, -doss.doss[:, projection, 1], color=color[index],
-                                    label=labels[index], linestyle='--', linewidth=linewidth)
-                        else:
-                            ax.plot(dx_alpha, doss.doss[:, projection, 0],
-                                    linestyle='-', linewidth=linewidth)
-                            ax.plot(dx_beta, -doss.doss[:, projection, 1],
-                                    linestyle='--', linewidth=linewidth)
-                    elif beta == accepted_beta[1]:
-                        if doss.n_proj > 1:
-                            ax.plot(dx_alpha, doss.doss[:, projection, 0], color=color[index],
-                                    label=labels[index], linestyle='-', linewidth=linewidth)
-                            ax.plot(dx_beta, doss.doss[:, projection, 1], color=color[index],
-                                    label=labels[index], linestyle='--', linewidth=linewidth)
-                        else:
-                            ax.plot(dx_alpha, doss.doss[:, projection, 0], color=color,
-                                    linestyle='-', linewidth=linewidth)
-                            ax.plot(dx_beta, doss.doss[:, projection, 1], color=color,
-                                    linestyle='--', linewidth=linewidth)
-
-        yfermi_level = np.linspace(ymin*1.05, ymax*1.05, 2)
-        xfermi_level = np.zeros(2)
-        if beta == accepted_beta[0]:
-            ax.plot(xfermi_level, yfermi_level, color=fermi, linewidth=1.5)
-        else:
-            yfermi_level = np.linspace(ymin*1.05, ymax*1.05, 2)
-            ax.plot(xfermi_level, yfermi_level, color=fermi, linewidth=1.5)
-        y_zero = np.zeros(2)
-        x_zero = np.linspace(xmin, xmax, 2)
-        ax.plot(x_zero, y_zero, color='black', linewidth=0.4)
-        if dos_range is not None:
-            ymin = dos_range[0]
-            ymax = dos_range[1]
-            plt.ylim(ymin, ymax)
-        else:
-            if doss.spin == 1:
-                ymin = 0
-                plt.ylim(ymin, ymax*1.05)
-            elif doss.spin == 2:
-                if beta == accepted_beta[0]:
-                    ymin = 0
-                    plt.ylim(ymin, ymax*1.05)
-                elif beta == accepted_beta[1]:
-                    plt.ylim(ymin*1.05, ymax*1.05)
-
-    # Plot for overlap == False
-    else:
-        # Error checks on colors, labels, and linestl
-        if isinstance(color, list):
-            warnings.warn('When overlap is false color should be a string!',
-                          stacklevel=2)
-            color = 'blue'
-
-        if isinstance(labels, list):
-            warnings.warn('When overlap is false labels should be a string!',
-                          stacklevel=2)
-            labels = None
-
-        if isinstance(linestl, list):
-            warnings.warn('When overlap is false color should be a string!',
-                          stacklevel=2)
-            linestl = '-'
-
-        # Creation of dx for the plot
-        if doss.spin == 1:
-            dx = doss.doss[:, 0]
-        elif doss.spin == 2:
-            dx = doss.doss[:, 0, :]
-            dx_alpha = doss.doss[:, 0, 0]
-            dx_beta = doss.doss[:, 0, 1]
-
-        # Determination of xmin and xmax
-        xmin = np.amin(dx)
-        xmax = np.amax(dx)
-
-        # Creation xfermi, x_zero, and y_zero
-        xfermi = np.zeros(2)
-        x_zero = np.linspace(xmin, xmax, 2)
-        y_zero = np.zeros(2)
-
-        # Creation of subplots for all projections
-        if prj is None:
-            fig, axs = plt.subplots(nrows=doss.n_proj, ncols=1, sharex=True, figsize=figsize)
-            # If only one projection is generated, axs is not subscriptable
-            if doss.n_proj == 1:
-                axs = [axs]
-        # Creation of subplots for selected projections
-        else:
-            fig, axs = plt.subplots(nrows=len(prj), ncols=1, sharex=True, figsize=figsize)
-            # If only one projection is generated, axs is not subscriptable
-            if len(prj) == 1:
-                axs = [axs]
-
-        # Plot for all projections
-        if prj is None:
-            for projection in range(doss.n_proj):
-                if doss.spin == 1:
-                    ymin = 0
-                    ymax = np.amax(doss.doss[:, projection+1])
-                    yfermi = np.linspace(ymin*1.05, ymax*1.05, 2)
-                    axs[projection].plot(dx, doss.doss[:, projection+1],
-                                         color=color, linestyle=linestl, linewidth=linewidth)
-                    axs[projection].plot(xfermi, yfermi, color=fermi, linewidth=1.5)
-                    if dos_range is not None:
-                        ymin = dos_range[0]
-                        ymax = dos_range[1]
-                    axs[projection].set_ylim(ymin, ymax)
-                elif doss.spin == 2:
-                    if beta == accepted_beta[0]:
-                        ymin = 0
-                        ymax = np.amax(doss.doss[:, projection+1, :])
-                        yfermi = np.linspace(ymin, ymax, 2)
-                        axs[projection].plot(dx_alpha, doss.doss[:, projection+1, 0], color=color,
-                                             linestyle='-', linewidth=linewidth, label='Alpha')
-                        axs[projection].plot(dx_beta, -doss.doss[:, projection+1, 1], color=color,
-                                             linestyle='--', linewidth=linewidth, label='Beta')
-                        axs[projection].plot(xfermi, yfermi, color=fermi, linewidth=1.5)
-                        if dos_range is not None:
-                            ymin = dos_range[0]
-                            ymax = dos_range[1]
-                        axs[projection].set_ylim(ymin, ymax)
-                    elif beta == accepted_beta[1]:
-                        ymin = -np.amax(doss.doss[:, projection+1, :])
-                        ymax = np.amax(doss.doss[:, projection+1, :])
-                        yfermi = np.linspace(ymin, ymax, 2)
-                        axs[projection].plot(dx_alpha, doss.doss[:, projection+1, 0], color=color,
-                                             linestyle='-', linewidth=linewidth, label='Alpha')
-                        axs[projection].plot(dx_beta, doss.doss[:, projection+1, 1], color=color,
-                                             linestyle='--', linewidth=linewidth, label='Beta')
-                        axs[projection].plot(x_zero, y_zero, linewidth=0.4)
-                        axs[projection].plot(xfermi, yfermi, color=fermi, linewidth=2.5)
-                        if dos_range is not None:
-                            ymin = dos_range[0]
-                            ymax = dos_range[1]
-                        axs[projection].set_ylim(ymin, ymax)
-
-        # Plot for selected projections
-        else:
-            for index, projection in enumerate(prj):
-                if doss.spin == 1:
-                    ymin = 0
-                    ymax = np.amax(doss.doss[:, projection])
-                    yfermi = np.linspace(ymin*1.05, ymax*1.05, 2)
-                    axs[index].plot(dx, doss.doss[:, projection],
-                                    color=color, linestyle=linestl, linewidth=linewidth)
-                    axs[index].plot(xfermi, yfermi, color=fermi, linewidth=1.5)
-                    if dos_range is not None:
-                        ymin = dos_range[0]
-                        ymax = dos_range[1]
-                    axs[index].set_ylim(ymin, ymax)
-                elif doss.spin == 2:
-                    if beta == accepted_beta[0]:
-                        ymin = 0
-                        ymax = np.amax(doss.doss[:, projection, :])
-                        yfermi = np.linspace(ymin*1.05, ymax*1.05, 2)
-                        axs[index].plot(dx_alpha, doss.doss[:, projection, 0], color=color,
-                                        linestyle='-', linewidth=linewidth, label='Alpha')
-                        axs[index].plot(dx_beta, -doss.doss[:, projection, 1], color=color,
-                                        linestyle='--', linewidth=linewidth, label='Beta')
-                        axs[index].plot(
-                            xfermi, yfermi, color=fermi, linewidth=1.5)
-                        if dos_range is not None:
-                            ymin = dos_range[0]
-                            ymax = dos_range[1]
-                        axs[index].set_ylim(ymin, ymax)
-                    elif beta == accepted_beta[1]:
-                        ymin = -np.amax(doss.doss[:, projection, :])
-                        ymax = np.amax(doss.doss[:, projection, :])
-                        yfermi = np.linspace(ymin*1.05, ymax*1.05, 2)
-                        axs[index].plot(dx_alpha, doss.doss[:, projection, 0], color=color,
-                                        linestyle='-', linewidth=linewidth, label='Alpha')
-                        axs[index].plot(dx_beta, doss.doss[:, projection, 1], color=color,
-                                        linestyle='--', linewidth=linewidth, label='Beta')
-                        axs[index].plot(x_zero, y_zero, linewidth=0.4)
-                        axs[index].plot(
-                            xfermi, yfermi, color=fermi, linewidth=1.5)
-                        if dos_range is not None:
-                            ymin = dos_range[0]
-                            ymax = dos_range[1]
-                        axs[index].set_ylim(ymin, ymax)
-
-        if (doss.spin == 2) and (beta == accepted_beta[1]):
-            plt.legend()
-
-    if energy_range is not None:
-        xmin = energy_range[0]
-        xmax = energy_range[1]
-    plt.xlim(xmin, xmax)
-
-    if title is not None:
-        fig.suptitle(title)
-    if labels is not None:
-        plt.legend()
-
-    return fig
-
 
 def plot_electron_banddos(bands, doss, unit='eV', k_labels=None, dos_beta='down',
                           dos_prj=None, energy_range=None, dos_max_range=None,
                           color_band='blue', color_dos='blue', labels=None, linestl_band='-',
                           linestl_dos=None, linewidth=1, fermi='forestgreen',
                           title=None, figsize=None, save_to_file=None):
     """
@@ -1594,14 +725,15 @@
 
     Raises:
         ValueError: If the unit parameter is unknown.
 
     """
     import matplotlib.pyplot as plt
     from CRYSTALpytools.units import H_to_eV, eV_to_H
+    from CRYSTALpytools.base.plotbase import plot_cry_es
     import re
 
     if re.match(r'^ev$', unit, re.IGNORECASE):
         unit = 'eV'
         is_ev = True
     elif re.match(r'^hartree$', unit, re.IGNORECASE):
         unit = 'Hartree'
@@ -1676,14 +808,15 @@
 
     Raises:
         ValueError: If the unit parameter is unknown.
 
     """
     import matplotlib.pyplot as plt
     from CRYSTALpytools.units import cm_to_thz, thz_to_cm
+    from CRYSTALpytools.base.plotbase import plot_cry_es
     import re
 
     if re.match(r'^cm\-1$', unit, re.IGNORECASE):
         unit = 'cm-1'
         is_thz = False
     elif re.match(r'^thz$', unit, re.IGNORECASE):
         unit = 'THz'
@@ -1721,302 +854,66 @@
 
     if save_to_file != None:
         save_plot(save_to_file)
 
     plt.show()
 
 
-def plot_cry_es(bands, doss, k_labels, color_bd, color_doss, fermi, energy_range, linestl_bd,
-                linestl_doss, linewidth, prj, figsize, labels, dos_max_range, title, dos_beta):
+def plot_cry_bands(bands, k_labels=None, energy_range=None, title=None,
+                   not_scaled=False, mode='single', linestl='-', linewidth=1,
+                   color='blue', fermi='forestgreen', k_range=None, labels=None,
+                   figsize=None, scheme=None, sharex=True, sharey=True, save_to_file=None):
     """
-    The base function to plot electron / phonon band structure + DOS
-
-    Args:
-        bands (object): Object containing band structure data
-        doss (object): Object containing density of states data
-        k_labels (list or None): List of labels for high symmetry points along the path
-        color_bd (str): Color for the band structure plot
-        color_doss (str or list or tuple): Color(s) for the density of states plot
-        fermi (str): Color for the Fermi level lines
-        energy_range (list or None): Range of energy values for the y-axis
-        linestl_bd (str): Linestyle for the band structure plot
-        linestl_doss (str or list or tuple or None): Linestyle(s) for the density of states plot
-        linewidth (float): Width of the lines
-        prj (list or None): List of projection indices for plotting specific projections
-        figsize (tuple): Figure size (width, height)
-        labels (str or list or tuple or None): Labels for the density of states plot
-        dos_max_range (float or None): Maximum range of the density of states plot
-        title (str or None): Title of the figure
-        dos_beta (str): Beta state for the density of states plot ('up' or 'down')
-
-    Returns:
-        fig (object): Figure object containing the plotted data
+    Deprecated
     """
-    import numpy as np
-    import matplotlib.pyplot as plt
     import warnings
-    from os import path
-
-    # Dictionary of greek letters for the band plot in the electronic structure
-    greek = {'Alpha': '\u0391', 'Beta': '\u0392', 'Gamma': '\u0393', 'Delta': '\u0394', 'Epsilon': '\u0395', 'Zeta': '\u0396', 'Eta': '\u0397',
-             'Theta': '\u0398', 'Iota': '\u0399', 'Kappa': '\u039A', 'Lambda': '\u039B', 'Mu': '\u039C', 'Nu': '\u039D', 'Csi': '\u039E',
-             'Omicron': '\u039F', 'Pi': '\u03A0', 'Rho': '\u03A1', 'Sigma': '\u03A3', 'Tau': '\u03A4', 'Upsilon': '\u03A5', 'Phi': '\u03A6',
-             'Chi': '\u03A7', 'Psi': '\u03A8', 'Omega': '\u03A9', 'Sigma_1': '\u03A3\u2081'}
-
-    if isinstance(color_doss, list) or isinstance(color_doss, tuple):
-        # Error check on linestl_doss length when the prj kwargs is not used
-        if (prj is None) and (len(color_doss) != doss.n_proj):
-            if len(color_doss) > doss.n_proj:
-                warnings.warn('You have a number of linestl_doss elements is greater than the number of projection!',
-                              stacklevel=2)
-            else:
-                raise ValueError("You don't have enough elements in linestl_doss for the number of projection required")
-        # Error check on linestl_doss length when the prj kwargs is used
-        elif (prj is not None) and (len(color_doss) != len(prj)):
-            if len(color_doss) > len(prj):
-                warnings.warn('You have a number of linestl_doss element greater than the number of projection required(prj elements)!',
-                              stacklevel=2)
-            else:
-                raise ValueError("You don't have enough elements in linestl_doss for the number of projection required(prj elements)")
-    else:
-        if prj == None:
-            nprj = doss.n_proj
-        else:
-            nprj = len(prj)
-        if nprj > 1:
-            warnings.warn('Only one color / no color is given. All DOS projections are in the same color.')
-        color_doss = [color_doss for i in range(nprj)]
-
-    if isinstance(labels, list) or isinstance(labels, tuple):
-        # Error check on labels length when the prj kwargs is not used
-        if (prj is None) and (len(labels) != doss.n_proj):
-            if len(labels) > doss.n_proj:
-                warnings.warn('You have a number of labels greater than the number of projection!')
-            else:
-                raise ValueError("You don't have enough elements in labels for the numeber of projection required")
-        # Error check on labels length when the prj kwargs is used
-        elif (prj is not None) and (len(labels) != len(prj)):
-            if len(labels) > len(prj):
-                warnings.warn('You have a number of linestl_doss element greater than the number of projection required(prj elements)!',
-                              stacklevel=2)
-            else:
-                raise ValueError("You don't have enough elements in linestl_doss for the number of projection required(prj elements)")
-    else:
-        if prj == None:
-            nprj = doss.n_proj
-        else:
-            nprj = len(prj)
-        if nprj > 1:
-            warnings.warn('Label not given. No label is available for DOS.')
-        labels = [None for i in range(nprj)]
-
-    # DOS beta state
-    if dos_beta == 'up':
-        spin_idx = -1 # DOS in crystal output is distinguished by +/- sign already
-        line_0 = False
-    elif dos_beta == 'down':
-        spin_idx = 1
-        line_0 = True
-    else:
-        raise ValueError("'dos_beta' should be either 'up' or 'down'.")
-    if doss.doss.shape[2] == 2:
-        doss.doss[:, :, 1] = doss.doss[:, :, 1] * spin_idx
-
-    # Definition and creation of the figure and the axes
-    fig, axs = plt.subplots(nrows=1, ncols=2, gridspec_kw={'width_ratios': [2, 1]},
-                            sharex=False, sharey=True, figsize=figsize)
-    if title != None:
-        fig.suptitle(title)
-
-    # Definition of the hsp position variables
-    hsp = bands.tick_position
-
-    # Error check on k_labels lenght against the HSP poisitions
-    if k_labels is not None:
-        if len(hsp) != len(k_labels):
-            if len(hsp) > len(k_labels):
-                raise ValueError('You have specified a number of label smaller than the number of High Simmetry Point along the path')
-            elif len(hsp) < len(k_labels):
-                raise ValueError('You have more labels than the High Simmetry point along the path')
-
-    # Local variable definition for the band plot
-    dx_bd = bands.k_point_plot
-    pltband = bands.bands
-    no_bands = np.shape(pltband)[0]
-    ymin_bd = np.amin(pltband)
-    ymax_bd = np.amax(pltband)
-    xmin_bd = np.amin(dx_bd)
-    xmax_bd = np.amax(dx_bd)
-    count1 = 0
-    count2 = 0
-
-    # band plot
-    for i in range(no_bands):
-        if bands.spin == 1:
-            axs[0].plot(dx_bd, pltband[i, :], color=color_bd,
-                        linestyle=linestl_bd, linewidth=linewidth)
-
-        elif bands.spin == 2:
-            if count1 == count2:
-                axs[0].plot(dx_bd, pltband[i, :, 0], color=color_bd,
-                            linestyle='-', linewidth=linewidth, label='Alpha')
-                axs[0].plot(dx_bd, pltband[i, :, 1], color=color_bd,
-                            linestyle='--', linewidth=linewidth, label='Beta')
-            else:
-                axs[0].plot(dx_bd, pltband[i, :, 0], color=color_bd,
-                            linestyle='-', linewidth=linewidth)
-                axs[0].plot(dx_bd, pltband[i, :, 1], color=color_bd,
-                            linestyle='--', linewidth=linewidth)
-
-        count1 += 1
-
-    # Definition of dx for the doss plot
-    if doss.spin == 1:
-        dx_dos = doss.doss[:, 0]
-    elif doss.spin == 2:
-        dx_dos = doss.doss[:, 0, :]
-        dx_alpha = doss.doss[:, 0, 0]
-        dx_beta = doss.doss[:, 0, 1]
-
-    # Determination of xmin, xmax, ymin, and ymax
-    if prj != None:
-        argplt = prj
-    else:
-        argplt = range(1, doss.doss.shape[1])
-
-    # Plot a vertical line at 0 DOS. Only for spin polarized cases
-    if line_0 == True and doss.spin == 2:
-        xmin_dos = np.amin(doss.doss[:, argplt, 1])
-        xmax_dos = np.amax(doss.doss[:, argplt, 0])
-        # make the scale symmetric, for comparison
-        xmin_dos = -max([abs(xmin_dos), abs(xmax_dos)])
-        xmax_dos = -xmin_dos
-    else:
-        xmin_dos = 0.
-        xmax_dos = np.amax(doss.doss[:, argplt, :])
-
-    ymin_dos = np.amin(dx_dos)
-    ymax_dos = np.amax(dx_dos)
-
-    # Plot of all projections
-    if prj is None:
-        for projection in range(1, doss.n_proj+1):
-            if doss.spin == 1:
-
-                if doss.n_proj > 1:
-
-                    if linestl_doss is None:
-                        axs[1].plot(doss.doss[:, projection], dx_dos, color=color_doss[projection-1],
-                                    label=labels[projection-1], linewidth=linewidth)
-
-                    else:
-                        axs[1].plot(doss.doss[:, projection], dx_dos, color=color_doss[projection-1],
-                                    label=labels[projection-1], linestyle=linestl_doss[projection-1], linewidth=linewidth)
-
-                else:
-                    axs[1].plot(doss.doss[:, projection], dx_dos, color=color_doss[0],
-                                linewidth=linewidth)
-
-            elif doss.spin == 2:
-                if doss.n_proj > 1:
-                    axs[1].plot(doss.doss[:, projection, 0], dx_alpha, color=color_doss[projection-1],
-                                label=labels[projection-1], linestyle='-', linewidth=linewidth)
-                    axs[1].plot(doss.doss[:, projection, 1], dx_beta, color=color_doss[projection-1],
-                                label=labels[projection-1], linestyle='--', linewidth=linewidth)
-                else:
-                    axs[1].plot(doss.doss[:, projection, 0], dx_alpha, color=color_doss[0],
-                                linestyle='-', linewidth=linewidth)
-                    axs[1].plot(doss.doss[:, projection, 1], dx_beta, color=color_doss[0],
-                                linestyle='--', linewidth=linewidth)
-
-    # Plot of a selected number of projections
-    else:
-        for index, projection in enumerate(prj):
-            if doss.spin == 1:
-                if doss.n_proj > 1:
-                    if linestl_doss is None:
-                        axs[1].plot(doss.doss[:, projection], dx_dos, color=color_doss[index],
-                                    label=labels[index], linewidth=linewidth)
-                    else:
-                        axs[1].plot(doss.doss[:, projection], dx_dos, color=color_doss[index],
-                                    label=labels[index], linestyle=linestl_doss[index], linewidth=linewidth)
-                else:
-                    axs[1].plot(doss.doss[:, projection], dx_dos, color=color_doss[0],
-                                linewidth=linewidth)
-            elif doss.spin == 2:
-                if doss.n_proj > 1:
-                    axs[1].plot(doss.doss[:, projection, 0], dx_alpha, color=color_doss[index],
-                                label=labels[index], linestyle='-', linewidth=linewidth)
-                    axs[1].plot(doss.doss[:, projection, 1], dx_beta, color=color_doss[index],
-                                label=labels[index], linestyle='--', linewidth=linewidth)
-                else:
-                    axs[1].plot(doss.doss[:, projection, 0], dx_alpha, color=color_doss[0],
-                                linestyle='-', linewidth=linewidth)
-                    axs[1].plot(doss.doss[:, projection, 1], dx_beta, color=color_doss[0],
-                                linestyle='--', linewidth=linewidth)
-
-    if ymin_bd > ymin_dos:
-        ymin = ymin_dos
-    elif ymin_bd <= ymin_dos:
-        ymin = ymin_bd
-
-    if ymax_bd >= ymax_dos:
-        ymax = ymax_bd
-    elif ymax_bd < ymax_dos:
-        ymax = ymax_dos
-
-    xmax_bd = hsp[len(hsp)-1]
-    # Plot of HSP lines
-    yhsp = np.linspace(ymin-5, ymax+5, 2)
-    for j in hsp:
-        xhsp = np.ones(2)*j
-        axs[0].plot(xhsp, yhsp, color='black', linewidth=0.5)
-
-    # Creation if HSP label ticks
-    hsp_label = []
-    if k_labels is not None:
-        for n in k_labels:
-            if n in greek:
-                g = greek.get(n)
-                hsp_label.append(g)
-            else:
-                hsp_label.append(n)
-
-    axs[0].set_xticks(hsp)
-    if k_labels is not None:
-        axs[0].set_xticklabels(hsp_label)
 
-    xfermi_bd = np.linspace(xmin_bd, xmax_bd, 2)
-    xfermi_dos = np.linspace(xmin_dos*1.05, xmax_dos*1.05, 2)
-    yfermi = np.zeros(2)
+    warnings.warn("Deprecated. This function calls 'plot_electron_band' with unit = eV",
+                   stacklevel=2)
 
-    # Plot of fermi level lines both in the band and the doss plot
-    axs[0].plot(xfermi_bd, yfermi, color=fermi, linewidth=1.5)
-    axs[1].plot(xfermi_dos, yfermi, color=fermi, linewidth=1.5)
+    plot_electron_band(bands, k_labels=k_labels, mode=mode, not_scaled=not_scaled,
+                       energy_range=energy_range, k_range=k_range, color=color,
+                       labels=labels, linestl=linestl, linewidth=linewidth,
+                       fermi=fermi, title=title, figsize=figsize, scheme=scheme,
+                       sharex=sharex, sharey=sharey, save_to_file=save_to_file)
 
-    axs[0].set_xlim(xmin_bd, xmax_bd)
 
-    if dos_max_range is not None:
-        xmax_dos = dos_max_range
-
-    # if (prj is None) and (doss.n_proj not in prj):
-    #    xmax_dos = np.amax(doss.doss[:, 1:doss.n_proj-1, :])
+def plot_cry_doss(doss, color='blue', fermi='forestgreen', overlap=False, labels=None,
+                  figsize=None, linestl=None, linewidth=1, title=None, beta='up',
+                  energy_range=None, dos_range=None, prj=None, save_to_file=None):
+    """
+    Deprecated
+    """
+    import warnings
 
-    if line_0 == True:
-        axs[1].plot(np.zeros([2,]), [ymin, ymax], color='black', linewidth=0.5)
-    axs[1].set_xlim(xmin_dos*1.05, xmax_dos*1.05)
+    warnings.warn("Deprecated. This function calls 'plot_electron_dos' with unit = eV",
+                  stacklevel=2)
+    plot_electron_dos(doss, beta=beta, overlap=overlap, prj=prj, energy_range=energy_range,
+                      dos_range=dos_range, color=color, labels=labels, linestl=linestl,
+                      linewidth=linewidth, fermi=fermi, title=title, figsize=figsize,
+                      save_to_file=save_to_file)
 
-    if energy_range is not None:
-        ymin = energy_range[0]
-        ymax = energy_range[1]
 
-    plt.ylim(ymin, ymax)
-    plt.legend()
+def plot_cry_es(bands, doss, k_labels=None, color_bd='blue', color_doss='blue',
+                fermi='forestgreen', energy_range=None, linestl_bd='-',
+                linestl_doss=None, linewidth=1, prj=None, figsize=None, labels=None,
+                dos_max_range=None, title=None, dos_beta='down', save_to_file=None):
+    """
+    Deprecated
+    """
+    import warnings
 
-    return fig
+    warnings.warn("Deprecated. This function calls 'plot_electron_banddos' with unit = eV.",
+                  stacklevel=2)
+    plot_electron_banddos(bands, doss, k_labels=None, dos_beta=dos_beta, dos_prj=prj,
+                          energy_range=energy_range, dos_max_range=dos_max_range,
+                          color_band=color_bd, color_dos=color_doss, labels=labels,
+                          linestl_band=linestl_bd, linestl_dos=linestl_doss,
+                          linewidth=linewidth, fermi=fermi, title=title, figsize=figsize,
+                          save_to_file=save_to_file)
 
 
 def plot_cry_contour(contour_obj, save_to_file=False):
     """
     Plot a contour plot.
 
     Args:
```

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/thermodynamics.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/unit_test.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/unit_test.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/units.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/units.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools/utils.py` & `CRYSTALpytools-2023.8.3/CRYSTALpytools/utils.py`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/PKG-INFO` & `CRYSTALpytools-2023.8.3/CRYSTALpytools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CRYSTALpytools
-Version: 2023.7.6
+Version: 2023.8.3
 Summary: Python tools for the CRYSTAL code developed and mantained by the CRYSTAL code developers.
 Home-page: https://github.com/crystal-code-tools/CRYSTALpytools
 Author-email: crystalcodetools@gmail.com
 Project-URL: Bug Tracker, https://github.com/crystal-code-tools/CRYSTALpytools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.7.6 Summary: Python
+Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.8.3 Summary: Python
 tools for the CRYSTAL code developed and mantained by the CRYSTAL code
 developers. Home-page: https://github.com/crystal-code-tools/CRYSTALpytools
 Author-email: crystalcodetools@gmail.com Project-URL: Bug Tracker, https://
 github.com/crystal-code-tools/CRYSTALpytools/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE.txt Python tools for the CRYSTAL_code developed
```

### Comparing `CRYSTALpytools-2023.7.6/CRYSTALpytools.egg-info/SOURCES.txt` & `CRYSTALpytools-2023.8.3/CRYSTALpytools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 CRYSTALpytools.egg-info/requires.txt
 CRYSTALpytools.egg-info/top_level.txt
 CRYSTALpytools/base/__init__.py
 CRYSTALpytools/base/basisset.py
 CRYSTALpytools/base/crysd12.py
 CRYSTALpytools/base/crysout.py
 CRYSTALpytools/base/inputbase.py
+CRYSTALpytools/base/plotbase.py
 CRYSTALpytools/base/propout.py
```

### Comparing `CRYSTALpytools-2023.7.6/LICENSE.txt` & `CRYSTALpytools-2023.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/PKG-INFO` & `CRYSTALpytools-2023.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CRYSTALpytools
-Version: 2023.7.6
+Version: 2023.8.3
 Summary: Python tools for the CRYSTAL code developed and mantained by the CRYSTAL code developers.
 Home-page: https://github.com/crystal-code-tools/CRYSTALpytools
 Author-email: crystalcodetools@gmail.com
 Project-URL: Bug Tracker, https://github.com/crystal-code-tools/CRYSTALpytools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.7.6 Summary: Python
+Metadata-Version: 2.1 Name: CRYSTALpytools Version: 2023.8.3 Summary: Python
 tools for the CRYSTAL code developed and mantained by the CRYSTAL code
 developers. Home-page: https://github.com/crystal-code-tools/CRYSTALpytools
 Author-email: crystalcodetools@gmail.com Project-URL: Bug Tracker, https://
 github.com/crystal-code-tools/CRYSTALpytools/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE.txt Python tools for the CRYSTAL_code developed
```

### Comparing `CRYSTALpytools-2023.7.6/README.md` & `CRYSTALpytools-2023.8.3/README.md`

 * *Files identical despite different names*

### Comparing `CRYSTALpytools-2023.7.6/setup.py` & `CRYSTALpytools-2023.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 long_description = 'Python tools for the <a href="https://www.crystal.unito.it/index.php">CRYSTAL code</a> developed and mantained by the CRYSTAL code developers'
 
 setuptools.setup(
     name="CRYSTALpytools",        
-    version="2023.07.06",
+    version="2023.08.03",
     author_email="crystalcodetools@gmail.com",
     description="Python tools for the CRYSTAL code developed and mantained by the CRYSTAL code developers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/crystal-code-tools/CRYSTALpytools",
     project_urls={
         "Bug Tracker": "https://github.com/crystal-code-tools/CRYSTALpytools/issues",
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 import setuptools long_description = 'Python tools for the CRYSTAL_code
 developed and mantained by the CRYSTAL code developers' setuptools.setup
-( name="CRYSTALpytools", version="2023.07.06",
+( name="CRYSTALpytools", version="2023.08.03",
 author_email="crystalcodetools@gmail.com", description="Python tools for the
 CRYSTAL code developed and mantained by the CRYSTAL code developers.",
 long_description=long_description, long_description_content_type="text/
 markdown", url="https://github.com/crystal-code-tools/CRYSTALpytools",
 project_urls={ "Bug Tracker": "https://github.com/crystal-code-tools/
 CRYSTALpytools/issues", }, classifiers=[ "Programming Language :: Python :: 3",
 "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",
```

