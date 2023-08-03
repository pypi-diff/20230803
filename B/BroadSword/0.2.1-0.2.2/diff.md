# Comparing `tmp/BroadSword-0.2.1.tar.gz` & `tmp/BroadSword-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BroadSword-0.2.1.tar", last modified: Fri Jul 28 16:51:58 2023, max compression
+gzip compressed data, was "BroadSword-0.2.2.tar", last modified: Thu Aug  3 20:14:58 2023, max compression
```

## Comparing `BroadSword-0.2.1.tar` & `BroadSword-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:58.070477 BroadSword-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-28 16:51:39.000000 BroadSword-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-07-28 16:51:58.070477 BroadSword-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-28 16:51:39.000000 BroadSword-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 16:51:39.000000 BroadSword-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-28 16:51:58.074478 BroadSword-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:58.066477 BroadSword-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:58.070477 BroadSword-0.2.1/src/BroadSword/
--rw-r--r--   0 runner    (1001) docker     (123)    57155 2023-07-28 16:51:39.000000 BroadSword-0.2.1/src/BroadSword/BroadSword.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:51:39.000000 BroadSword-0.2.1/src/BroadSword/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20584 2023-07-28 16:51:39.000000 BroadSword-0.2.1/src/BroadSword/libmatrices.so
--rw-r--r--   0 runner    (1001) docker     (123)    33748 2023-07-28 16:51:39.000000 BroadSword-0.2.1/src/BroadSword/libmatrices_ARM64.dylib
--rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-07-28 16:51:39.000000 BroadSword-0.2.1/src/BroadSword/libmatrices_x86_64.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-28 16:51:39.000000 BroadSword-0.2.1/src/BroadSword/matrices.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:58.070477 BroadSword-0.2.1/src/BroadSword.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-07-28 16:51:58.000000 BroadSword-0.2.1/src/BroadSword.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-28 16:51:58.000000 BroadSword-0.2.1/src/BroadSword.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:51:58.000000 BroadSword-0.2.1/src/BroadSword.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 16:51:58.000000 BroadSword-0.2.1/src/BroadSword.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 16:51:58.000000 BroadSword-0.2.1/src/BroadSword.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:51:57.000000 BroadSword-0.2.1/src/BroadSword.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:14:58.150870 BroadSword-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-03 20:14:45.000000 BroadSword-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-08-03 20:14:58.150870 BroadSword-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-08-03 20:14:45.000000 BroadSword-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-03 20:14:45.000000 BroadSword-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-03 20:14:58.150870 BroadSword-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:14:58.146870 BroadSword-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:14:58.150870 BroadSword-0.2.2/src/BroadSword/
+-rw-r--r--   0 runner    (1001) docker     (123)    61737 2023-08-03 20:14:45.000000 BroadSword-0.2.2/src/BroadSword/BroadSword.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:14:45.000000 BroadSword-0.2.2/src/BroadSword/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20584 2023-08-03 20:14:45.000000 BroadSword-0.2.2/src/BroadSword/libmatrices.so
+-rw-r--r--   0 runner    (1001) docker     (123)    33748 2023-08-03 20:14:45.000000 BroadSword-0.2.2/src/BroadSword/libmatrices_ARM64.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-08-03 20:14:45.000000 BroadSword-0.2.2/src/BroadSword/libmatrices_x86_64.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-08-03 20:14:45.000000 BroadSword-0.2.2/src/BroadSword/matrices.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:14:58.150870 BroadSword-0.2.2/src/BroadSword.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-08-03 20:14:58.000000 BroadSword-0.2.2/src/BroadSword.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-03 20:14:58.000000 BroadSword-0.2.2/src/BroadSword.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:14:58.000000 BroadSword-0.2.2/src/BroadSword.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-03 20:14:58.000000 BroadSword-0.2.2/src/BroadSword.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 20:14:58.000000 BroadSword-0.2.2/src/BroadSword.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:14:57.000000 BroadSword-0.2.2/src/BroadSword.egg-info/zip-safe
```

### Comparing `BroadSword-0.2.1/LICENSE` & `BroadSword-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BroadSword-0.2.1/PKG-INFO` & `BroadSword-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BroadSword
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/Cody-Somers/BroadSword
 Author: Cody Somers
 Author-email: cas003@usask.ca
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `BroadSword-0.2.1/README.md` & `BroadSword-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `BroadSword-0.2.1/setup.cfg` & `BroadSword-0.2.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = BroadSword
-version = 0.2.1
+version = 0.2.2
 author = Cody Somers
 author_email = cas003@usask.ca
 description = Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Cody-Somers/BroadSword
 project_urls =
```

### Comparing `BroadSword-0.2.1/src/BroadSword/BroadSword.py` & `BroadSword-0.2.2/src/BroadSword/BroadSword.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             Specify the file name (ASCII or .csv) including the extension.
             Header lines are allowed, as long as they are specified properly in the function.
         GS_fermi : float
             Specify the fermi energy for the ground state calculated spectra. Found in .scf2
         headerlines : [int]
             Specify the number of headerlines for the XES and XANES files respectively. 
         """
-
+        
         try:
             with open(basedir+"/"+XES, "r") as xesFile: # Measured XES
                 df = pd.read_csv(xesFile, delimiter='\s+', header=None, skiprows=headerlines[0]) # Change to '\s*' and specify engine='python' if this breaks in jupyter notebook
                 c1 = 0
                 maxEXP = 0
                 for i in range(len(df)): 
                     ExpSXS[0][c1][0] = df[0][c1] # Energy
@@ -533,24 +533,26 @@
             ("(x,y)", "($x, $y)")
         ]))
         self.plotBroadCalc(p)
         self.plotExp(p)
         show(p)
         return
 
-    def broaden(self,separate=True):
+    def broaden(self,separate=True, Ængus=False):
         """
         This will take the shifted calculated spectra and broaden it based on the lifetime, instrument, and general disorder broadening.
         It creates a series of gaussians and lorentzians before applying it to the spectra appropriately.
 
         Parameters
         ----------
         separate : True/False
             Specify whether or not to create a separate output plot of XES and XAS
         """
+        if Ængus == "yup":
+            Ængus = True
 
         Econd = np.zeros(40)
         type = False
         energy_0 = 20
         Pi = 3.14159265; # The Pi constant used for the distribution functions.
 
         if XESbandScale == 0: # Applying a singular scale to XES
@@ -656,47 +658,83 @@
 
                 BroadSXS[6,:,c2,c1] = 0 # Line 990
                 for c3 in range(BroadSXSCount[c2][c1]):
                     BroadSXS[6,:,c2,c1] = BroadSXS[6,:,c2,c1]+(Disorder[c3,:]*BroadSXS[5][c3][c2][c1]*(BroadSXS[0][1][c2][c1]-BroadSXS[0][0][c2][c1]))
         self.add()
 
         if separate is False:
-            # Creating the figure for plotting the broadened data.
-            p = figure(height=450, width=900, title="Broadened Data", x_axis_label="Energy (eV)", y_axis_label="Normalized Intensity (arb. units)",
-                    tools="pan,wheel_zoom,box_zoom,reset,crosshair,save")
-            p.add_tools(HoverTool(show_arrow=False, line_policy='next', tooltips=[
-                ("(x,y)", "(Energy, Intensity)"),
-                ("(x,y)", "($x, $y)")
-            ]))
-            self.plotBroadCalc(p)
-            self.plotExp(p)
-            p.add_layout(p.legend[0], 'right')
-            show(p)
+            if Ængus is True:
+                # Creating the figure for plotting the broadened data.
+                p = figure(height=450, width=900, title="Broadened Data", x_axis_label="Energy (eV)", y_axis_label="Normalized Intensity (arb. units)",
+                        tools="pan,wheel_zoom,box_zoom,reset,crosshair,save")
+                p.add_tools(HoverTool(show_arrow=False, line_policy='next', tooltips=[
+                    ("(x,y)", "(Energy, Intensity)"),
+                    ("(x,y)", "($x, $y)")
+                ]))
+                self.plotÆngus(p)
+                self.plotExp(p)
+                p.add_layout(p.legend[0], 'right')
+                show(p)
+            else:
+                # Creating the figure for plotting the broadened data.
+                p = figure(height=450, width=900, title="Broadened Data", x_axis_label="Energy (eV)", y_axis_label="Normalized Intensity (arb. units)",
+                        tools="pan,wheel_zoom,box_zoom,reset,crosshair,save")
+                p.add_tools(HoverTool(show_arrow=False, line_policy='next', tooltips=[
+                    ("(x,y)", "(Energy, Intensity)"),
+                    ("(x,y)", "($x, $y)")
+                ]))
+                self.plotBroadCalc(p)
+                self.plotExp(p)
+                p.add_layout(p.legend[0], 'right')
+                show(p)
         else:
-            p = figure(height=450, width=900, title="Broadened Data", x_axis_label="Energy (eV)", y_axis_label="Normalized Intensity (arb. units)",
-                    tools="pan,wheel_zoom,box_zoom,reset,crosshair,save")
-            p.add_tools(HoverTool(show_arrow=False, line_policy='next', tooltips=[
-                ("(x,y)", "(Energy, Intensity)"),
-                ("(x,y)", "($x, $y)")
-            ]))
-            self.plotExpXES(p)
-            self.plotBroadXES(p)
-            p.add_layout(p.legend[0], 'right')
-            show(p)
-
-            p = figure(height=450, width=900, title="Broadened Data", x_axis_label="Energy (eV)", y_axis_label="Normalized Intensity (arb. units)",
-                    tools="pan,wheel_zoom,box_zoom,reset,crosshair,save")
-            p.add_tools(HoverTool(show_arrow=False, line_policy='next', tooltips=[
-                ("(x,y)", "(Energy, Intensity)"),
-                ("(x,y)", "($x, $y)")
-            ]))
-            self.plotExpXANES(p)
-            self.plotBroadXANES(p)
-            p.add_layout(p.legend[0], 'right')
-            show(p)
+            if Ængus is True:
+                p = figure(height=450, width=900, title="Broadened Data", x_axis_label="Energy (eV)", y_axis_label="Normalized Intensity (arb. units)",
+                        tools="pan,wheel_zoom,box_zoom,reset,crosshair,save")
+                p.add_tools(HoverTool(show_arrow=False, line_policy='next', tooltips=[
+                    ("(x,y)", "(Energy, Intensity)"),
+                    ("(x,y)", "($x, $y)")
+                ]))
+                self.plotExpXES(p)
+                self.plotBroadXES(p)
+                p.add_layout(p.legend[0], 'right')
+                show(p)
+
+                p = figure(height=450, width=900, title="Broadened Data", x_axis_label="Energy (eV)", y_axis_label="Normalized Intensity (arb. units)",
+                        tools="pan,wheel_zoom,box_zoom,reset,crosshair,save")
+                p.add_tools(HoverTool(show_arrow=False, line_policy='next', tooltips=[
+                    ("(x,y)", "(Energy, Intensity)"),
+                    ("(x,y)", "($x, $y)")
+                ]))
+                self.plotExpXANES(p)
+                self.plotÆngusXANES(p)
+                p.add_layout(p.legend[0], 'right')
+                show(p)
+            else:
+                p = figure(height=450, width=900, title="Broadened Data", x_axis_label="Energy (eV)", y_axis_label="Normalized Intensity (arb. units)",
+                        tools="pan,wheel_zoom,box_zoom,reset,crosshair,save")
+                p.add_tools(HoverTool(show_arrow=False, line_policy='next', tooltips=[
+                    ("(x,y)", "(Energy, Intensity)"),
+                    ("(x,y)", "($x, $y)")
+                ]))
+                self.plotExpXES(p)
+                self.plotBroadXES(p)
+                p.add_layout(p.legend[0], 'right')
+                show(p)
+
+                p = figure(height=450, width=900, title="Broadened Data", x_axis_label="Energy (eV)", y_axis_label="Normalized Intensity (arb. units)",
+                        tools="pan,wheel_zoom,box_zoom,reset,crosshair,save")
+                p.add_tools(HoverTool(show_arrow=False, line_policy='next', tooltips=[
+                    ("(x,y)", "(Energy, Intensity)"),
+                    ("(x,y)", "($x, $y)")
+                ]))
+                self.plotExpXANES(p)
+                self.plotBroadXANES(p)
+                p.add_layout(p.legend[0], 'right')
+                show(p)
 
         return
 
     def add(self):
         """
         A function that will sum together the individual inequivalent sites after they have been broadened with the matrices above.
         Scales the sites as appropriate, then does a linear interpolation of each data point to sum together different sites.
@@ -1067,14 +1105,47 @@
 
         p.line(sumxesX,sumxesY,line_color="limegreen",legend_label="Broadened XES/XANES") # XES plot
         p.line(sumxasX,sumxasY,line_color="blue",legend_label="Broadened XAS") # XAS plot
         p.line(sumxanesX,sumxanesY,line_color="limegreen") # XANES plot
         #show(p)
         return
     
+    def plotÆngus(self,p):
+        """
+        Plot the final calculated and broadened data.
+        The bokeh figure needs to be created and configured outside of the function. This simply adds the XANES and XES to a figure.
+
+        Parameters
+        ----------
+        p : figure()
+            The bokeh figure needs to be created outside of the function.
+        """
+        MaxBroadSXS = np.zeros([3])
+        for c3 in range(3): # Find the maximum value for normalization
+            for c2 in range(SumSXSCount[c3]):
+                if MaxBroadSXS[c3] < SumSXS[1][c2][c3]:
+                    MaxBroadSXS[c3] = SumSXS[1][c2][c3]
+        #p = figure()
+        sumxesX = np.zeros([SumSXSCount[0]])
+        sumxesY = np.zeros([SumSXSCount[0]])
+        sumxanesX = np.zeros([SumSXSCount[2]])
+        sumxanesY = np.zeros([SumSXSCount[2]])
+        for c2 in range(SumSXSCount[0]): # Calculated XES spectra
+            sumxesX[c2] = SumSXS[0][c2][0]
+            sumxesY[c2] = SumSXS[1][c2][0] / MaxBroadSXS[0]
+
+        for c2 in range(SumSXSCount[2]): # Calculated XANES spectra
+            sumxanesX[c2] = SumSXS[0][c2][2]
+            sumxanesY[c2] = SumSXS[1][c2][2] / MaxBroadSXS[2]
+
+        p.line(sumxesX,sumxesY,line_color="limegreen",legend_label="Broadened XES/XANES") # XES plot
+        p.line(sumxanesX,sumxanesY,line_color="limegreen") # XANES plot
+        #show(p)
+        return
+        
     def plotBroadXANES(self,p):
         """
         Plot the final calculated and broadened data for XAS and XANES
         The bokeh figure needs to be created and configured outside of the function. This simply adds the XANES and XAS to a figure.
 
         Parameters
         ----------
@@ -1099,14 +1170,40 @@
         for c2 in range(SumSXSCount[2]): # Calculated XANES spectra
             sumxanesX[c2] = SumSXS[0][c2][2]
             sumxanesY[c2] = SumSXS[1][c2][2] / MaxBroadSXS[2]
 
         p.line(sumxasX,sumxasY,line_color="blue",legend_label="Broadened XAS") # XAS plot
         p.line(sumxanesX,sumxanesY,line_color="limegreen",legend_label="Broadened XANES") # XANES plot
         return
+    
+    def plotÆngusXANES(self,p):
+        """
+        Plot the final calculated and broadened data for XANES
+        The bokeh figure needs to be created and configured outside of the function. This simply adds the XANES to a figure.
+
+        Parameters
+        ----------
+        p : figure()
+            The bokeh figure needs to be created outside of the function.
+        """
+        MaxBroadSXS = np.zeros([3])
+        for c3 in range(3): # Find the maximum value for normalization
+            for c2 in range(SumSXSCount[c3]):
+                if MaxBroadSXS[c3] < SumSXS[1][c2][c3]:
+                    MaxBroadSXS[c3] = SumSXS[1][c2][c3]
+        #p = figure()
+        sumxanesX = np.zeros([SumSXSCount[2]])
+        sumxanesY = np.zeros([SumSXSCount[2]])
+
+        for c2 in range(SumSXSCount[2]): # Calculated XANES spectra
+            sumxanesX[c2] = SumSXS[0][c2][2]
+            sumxanesY[c2] = SumSXS[1][c2][2] / MaxBroadSXS[2]
+        
+        p.line(sumxanesX,sumxanesY,line_color="limegreen",legend_label="Broadened XANES") # XANES plot
+        return
 
     def plotBroadXES(self,p):
         """
         Plot the final calculated and broadened data for XES
         The bokeh figure needs to be created and configured outside of the function. This simply adds the XES to a figure.
 
         Parameters
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `BroadSword-0.2.1/src/BroadSword/libmatrices.so` & `BroadSword-0.2.2/src/BroadSword/libmatrices.so`

 * *Files identical despite different names*

### Comparing `BroadSword-0.2.1/src/BroadSword/libmatrices_ARM64.dylib` & `BroadSword-0.2.2/src/BroadSword/libmatrices_ARM64.dylib`

 * *Files identical despite different names*

### Comparing `BroadSword-0.2.1/src/BroadSword/libmatrices_x86_64.dylib` & `BroadSword-0.2.2/src/BroadSword/libmatrices_x86_64.dylib`

 * *Files identical despite different names*

### Comparing `BroadSword-0.2.1/src/BroadSword/matrices.c` & `BroadSword-0.2.2/src/BroadSword/matrices.c`

 * *Files identical despite different names*

### Comparing `BroadSword-0.2.1/src/BroadSword.egg-info/PKG-INFO` & `BroadSword-0.2.2/src/BroadSword.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BroadSword
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/Cody-Somers/BroadSword
 Author: Cody Somers
 Author-email: cas003@usask.ca
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

