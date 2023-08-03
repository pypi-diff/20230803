# Comparing `tmp/pyphasefield-1.2.0.tar.gz` & `tmp/pyphasefield-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphasefield-1.2.0.tar", last modified: Wed Nov 10 04:39:37 2021, max compression
+gzip compressed data, was "pyphasefield-2.0.0.tar", last modified: Thu Aug  3 15:28:40 2023, max compression
```

## Comparing `pyphasefield-1.2.0.tar` & `pyphasefield-2.0.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxrwx   0        0        0        0 2021-11-10 04:39:37.215595 pyphasefield-1.2.0/
--rw-rw-rw-   0        0        0      668 2021-11-10 04:39:37.215595 pyphasefield-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      163 2019-12-03 18:01:44.000000 pyphasefield-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2021-11-10 04:39:37.168730 pyphasefield-1.2.0/pyphasefield/
-drwxrwxrwx   0        0        0        0 2021-11-10 04:39:37.199974 pyphasefield-1.2.0/pyphasefield/Engines/
--rw-rw-rw-   0        0        0    27731 2021-04-23 19:03:11.000000 pyphasefield-1.2.0/pyphasefield/Engines/AnisoDorrGPU.py
--rw-rw-rw-   0        0        0    16161 2021-04-16 17:12:00.000000 pyphasefield-1.2.0/pyphasefield/Engines/CahnAllen.py
--rw-rw-rw-   0        0        0    18538 2021-04-16 17:11:54.000000 pyphasefield-1.2.0/pyphasefield/Engines/CahnHilliard.py
--rw-rw-rw-   0        0        0    35567 2021-04-28 18:38:32.000000 pyphasefield-1.2.0/pyphasefield/Engines/Diffusion.py
--rw-rw-rw-   0        0        0     4957 2021-04-28 18:35:56.000000 pyphasefield-1.2.0/pyphasefield/Engines/DiffusionGPU.py
--rw-rw-rw-   0        0        0    31856 2021-10-13 04:56:29.000000 pyphasefield-1.2.0/pyphasefield/Engines/NCGPU.py
--rw-rw-rw-   0        0        0    34677 2021-10-13 06:12:21.000000 pyphasefield-1.2.0/pyphasefield/Engines/NCGPU_new.py
--rw-rw-rw-   0        0        0    62327 2021-04-16 17:14:49.000000 pyphasefield-1.2.0/pyphasefield/Engines/NComponent.py
--rw-rw-rw-   0        0        0     1922 2021-02-16 22:10:46.000000 pyphasefield-1.2.0/pyphasefield/Engines/Template.py
--rw-rw-rw-   0        0        0    16308 2021-06-01 16:58:47.000000 pyphasefield-1.2.0/pyphasefield/Engines/Warren1995.py
--rw-rw-rw-   0        0        0      766 2021-02-08 18:50:39.000000 pyphasefield-1.2.0/pyphasefield/Engines/__init__.py
--rw-rw-rw-   0        0        0       84 2020-09-08 22:05:23.000000 pyphasefield-1.2.0/pyphasefield/__init__.py
--rw-rw-rw-   0        0        0     3139 2021-02-08 18:50:39.000000 pyphasefield-1.2.0/pyphasefield/field.py
--rw-rw-rw-   0        0        0    27227 2021-03-04 19:31:05.000000 pyphasefield-1.2.0/pyphasefield/ppf_gpu_utils.py
--rw-rw-rw-   0        0        0     7824 2021-04-14 16:51:58.000000 pyphasefield-1.2.0/pyphasefield/ppf_utils.py
--rw-rw-rw-   0        0        0    36675 2021-10-13 04:51:02.000000 pyphasefield-1.2.0/pyphasefield/simulation.py
-drwxrwxrwx   0        0        0        0 2021-11-10 04:39:37.215595 pyphasefield-1.2.0/pyphasefield/tests/
--rw-rw-rw-   0        0        0        0 2020-08-25 02:59:15.000000 pyphasefield-1.2.0/pyphasefield/tests/__init__.py
--rw-rw-rw-   0        0        0     3761 2020-08-25 02:59:15.000000 pyphasefield-1.2.0/pyphasefield/tests/test_Diffusion.py
--rw-rw-rw-   0        0        0     1250 2020-08-25 02:59:15.000000 pyphasefield-1.2.0/pyphasefield/tests/test_NComponent.py
--rw-rw-rw-   0        0        0     1625 2020-08-25 02:59:15.000000 pyphasefield-1.2.0/pyphasefield/tests/test_SaveLoad.py
--rw-rw-rw-   0        0        0      140 2020-08-25 02:59:15.000000 pyphasefield-1.2.0/pyphasefield/tests/test_Warren1995.py
-drwxrwxrwx   0        0        0        0 2021-11-10 04:39:37.199974 pyphasefield-1.2.0/pyphasefield.egg-info/
--rw-rw-rw-   0        0        0      668 2021-11-10 04:39:37.000000 pyphasefield-1.2.0/pyphasefield.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      886 2021-11-10 04:39:37.000000 pyphasefield-1.2.0/pyphasefield.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-10 04:39:37.000000 pyphasefield-1.2.0/pyphasefield.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2021-11-10 04:39:37.000000 pyphasefield-1.2.0/pyphasefield.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2021-11-10 04:39:37.000000 pyphasefield-1.2.0/pyphasefield.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-11-10 04:39:37.215595 pyphasefield-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      757 2021-11-10 04:39:36.000000 pyphasefield-1.2.0/setup.py
+drwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)        0 2023-08-03 15:28:40.722958 pyphasefield-2.0.0/
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)     1091 2023-03-14 21:06:00.000000 pyphasefield-2.0.0/LICENSE
+-rw-r--r--   0 peters42 (1433879) Domain Users (1049089)      601 2023-08-03 15:28:40.722958 pyphasefield-2.0.0/PKG-INFO
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)      163 2023-03-14 21:06:04.000000 pyphasefield-2.0.0/README.md
+drwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)        0 2023-08-03 15:28:40.667954 pyphasefield-2.0.0/pyphasefield/
+drwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)        0 2023-08-03 15:28:40.707957 pyphasefield-2.0.0/pyphasefield/Engines/
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)    27239 2023-07-18 17:47:00.000000 pyphasefield-2.0.0/pyphasefield/Engines/AnisoDorrGPU.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)    15888 2023-07-18 17:46:39.000000 pyphasefield-2.0.0/pyphasefield/Engines/CahnAllen.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)    18274 2023-07-18 17:47:30.000000 pyphasefield-2.0.0/pyphasefield/Engines/CahnHilliard.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)    35434 2023-07-18 17:48:04.000000 pyphasefield-2.0.0/pyphasefield/Engines/Diffusion.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)    31981 2023-04-21 19:26:58.000000 pyphasefield-2.0.0/pyphasefield/Engines/NCGPU.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)    60340 2023-06-16 23:26:06.000000 pyphasefield-2.0.0/pyphasefield/Engines/NCGPU_new.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)    62327 2023-03-14 21:06:00.000000 pyphasefield-2.0.0/pyphasefield/Engines/NComponent.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)     1686 2023-07-18 17:51:47.000000 pyphasefield-2.0.0/pyphasefield/Engines/Template.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)    15755 2023-07-18 19:06:20.000000 pyphasefield-2.0.0/pyphasefield/Engines/Warren1995.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)      754 2023-04-21 18:40:29.000000 pyphasefield-2.0.0/pyphasefield/Engines/__init__.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)      574 2023-05-01 18:23:42.000000 pyphasefield-2.0.0/pyphasefield/__init__.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)     7100 2023-04-27 16:01:42.000000 pyphasefield-2.0.0/pyphasefield/__main__.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)    15800 2023-06-09 22:33:58.000000 pyphasefield-2.0.0/pyphasefield/field.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)      337 2023-04-21 19:23:50.000000 pyphasefield-2.0.0/pyphasefield/jit_placeholder.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)     9568 2023-03-22 16:05:50.000000 pyphasefield-2.0.0/pyphasefield/parallel_utils.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)    21954 2023-07-18 15:34:57.000000 pyphasefield-2.0.0/pyphasefield/ppf_gpu_utils.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)    14055 2023-06-21 19:34:45.000000 pyphasefield-2.0.0/pyphasefield/ppf_utils.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)    72674 2023-07-18 20:56:52.000000 pyphasefield-2.0.0/pyphasefield/simulation.py
+drwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)        0 2023-08-03 15:28:40.720973 pyphasefield-2.0.0/pyphasefield/tests/
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)        0 2023-03-14 21:06:04.000000 pyphasefield-2.0.0/pyphasefield/tests/__init__.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)     3761 2023-03-14 21:06:03.000000 pyphasefield-2.0.0/pyphasefield/tests/test_Diffusion.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)     1250 2023-03-14 21:06:03.000000 pyphasefield-2.0.0/pyphasefield/tests/test_NComponent.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)     1625 2023-03-14 21:06:04.000000 pyphasefield-2.0.0/pyphasefield/tests/test_SaveLoad.py
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)      140 2023-03-14 21:06:04.000000 pyphasefield-2.0.0/pyphasefield/tests/test_Warren1995.py
+drwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)        0 2023-08-03 15:28:40.677953 pyphasefield-2.0.0/pyphasefield.egg-info/
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)      601 2023-08-03 15:28:40.000000 pyphasefield-2.0.0/pyphasefield.egg-info/PKG-INFO
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)      910 2023-08-03 15:28:40.000000 pyphasefield-2.0.0/pyphasefield.egg-info/SOURCES.txt
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)        1 2023-08-03 15:28:40.000000 pyphasefield-2.0.0/pyphasefield.egg-info/dependency_links.txt
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)       13 2023-08-03 15:28:40.000000 pyphasefield-2.0.0/pyphasefield.egg-info/top_level.txt
+-rw-r--r--   0 peters42 (1433879) Domain Users (1049089)       38 2023-08-03 15:28:40.723958 pyphasefield-2.0.0/setup.cfg
+-rwxr-xr-x   0 peters42 (1433879) Domain Users (1049089)      683 2023-04-27 17:39:01.000000 pyphasefield-2.0.0/setup.py
```

### Comparing `pyphasefield-1.2.0/PKG-INFO` & `pyphasefield-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
-Name: pyphasefield
-Version: 1.2.0
-Summary: Python phase field simulation
-Home-page: https://github.com/AdditiveModeling/pyphasefield
-Author: Scott Peters
-Author-email: scott@dpeters.net
-License: UNKNOWN
-Description: # PyPhaseField
-        
-        Python-based phase field software, built using numpy and pycalphad. 
-        Content will be added soon-TM, once i figure out this whole packaging thing
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: pyphasefield
+Version: 2.0.0
+Summary: Python phase field simulation
+Home-page: https://github.com/AdditiveModeling/pyphasefield
+Author: Scott Peters
+Author-email: scott@dpeters.net
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PyPhaseField
+
+Python-based phase field software, built using numpy and pycalphad. 
+Content will be added soon-TM, once i figure out this whole packaging thing
```

### Comparing `pyphasefield-1.2.0/pyphasefield/Engines/AnisoDorrGPU.py` & `pyphasefield-2.0.0/pyphasefield/Engines/AnisoDorrGPU.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 import numpy as np
 import sympy as sp
 from scipy.sparse.linalg import gmres
-from numba import cuda
-import numba
 import matplotlib.pyplot as plt
 np.set_printoptions(threshold=np.inf)
-import math
-from numba.cuda.random import create_xoroshiro128p_states, xoroshiro128p_uniform_float32
-
+from pyphasefield.field import Field
+from pyphasefield.simulation import Simulation
+from pyphasefield.ppf_utils import COLORMAP_OTHER, COLORMAP_PHASE
+        
 try:
-    #import from within Engines folder
-    from ..field import Field
-    from ..simulation import Simulation
-    from ..ppf_utils import COLORMAP_OTHER, COLORMAP_PHASE
+    from numba import cuda
+    import numba
+    from numba.cuda.random import create_xoroshiro128p_states, xoroshiro128p_uniform_float32
 except:
-    try:
-        #import classes from pyphasefield library
-        from pyphasefield.field import Field
-        from pyphasefield.simulation import Simulation
-        from pyphasefield.ppf_utils import COLORMAP_OTHER, COLORMAP_PHASE
-    except:
-        raise ImportError("Cannot import from pyphasefield library!")
+    import pyphasefield.jit_placeholder as cuda
+    import pyphasefield.jit_placeholder as numba
 
 @cuda.jit(device=True)
 def divagradb(a, axp, axm, ayp, aym, b, bxp, bxm, byp, bym, idx):
     return 0.5*idx*idx*((axp+a)*(bxp-b) - (a+axm)*(b-bxm) + (ayp+a)*(byp-b) - (a+aym)*(b-bym))
     #return (idx*idx*a*(bxp+bxm+byp+bym-4*b) + 0.25*idx*idx*((axp - axm)*(bxp - bxm) + (ayp - aym)*(byp - bym)))
 
 @cuda.jit(device=True)
@@ -580,19 +573,14 @@
                 c_n += initial_concentration_array[0]
                 self.add_field(c_n, "c_CU", colormap=COLORMAP_OTHER)
 
             except: #initial_concentration array isnt defined?
                 c_n = np.zeros(dim)
                 c_n += 0.5
                 self.add_field(c_n, "c_CU", colormap=COLORMAP_OTHER)
-        
-    def initialize_fields_and_imported_data(self):
-        super().initialize_fields_and_imported_data()
-        #initialization of fields/imported data goes below
-        #runs *after* tdb, thermal, fields, and boundary conditions are loaded/initialized
                         
     def just_before_simulating(self):
         super().just_before_simulating()
         #additional code to run just before beginning the simulation goes below
         #runs immediately before simulating, no manual changes permitted to changes implemented here
         
     def simulation_loop(self):
```

### Comparing `pyphasefield-1.2.0/pyphasefield/Engines/CahnAllen.py` & `pyphasefield-2.0.0/pyphasefield/Engines/CahnAllen.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,20 +306,14 @@
             
     def init_fields(self):
         #initialization of fields code goes here
         #runs *after* tdb and thermal data is loaded/initialized
         #runs *before* boundary conditions are initialized
         phi = 0.001*np.random.random(self.dimensions) + 0.4995
         self.add_field(phi, "phi")
-        
-        
-    def initialize_fields_and_imported_data(self):
-        super().initialize_fields_and_imported_data()
-        #initialization of fields/imported data goes below
-        #runs *after* tdb, thermal, fields, and boundary conditions are loaded/initialized
                         
     def just_before_simulating(self):
         super().just_before_simulating()
         #additional code to run just before beginning the simulation goes below
         #runs immediately before simulating, no manual changes permitted to changes implemented here
         
     def simulation_loop(self):
```

### Comparing `pyphasefield-1.2.0/pyphasefield/Engines/CahnHilliard.py` & `pyphasefield-2.0.0/pyphasefield/Engines/CahnHilliard.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,19 +364,14 @@
 
     def init_fields(self):
         #initialization of fields code goes here
         #runs *after* tdb and thermal data is loaded/initialized
         #runs *before* boundary conditions are initialized
         phi = 0.001*np.random.random(self.dimensions) + 0.4995
         self.add_field(phi, "phi")
-        
-    def initialize_fields_and_imported_data(self):
-        super().initialize_fields_and_imported_data()
-        #initialization of fields/imported data goes below
-        #runs *after* tdb, thermal, fields, and boundary conditions are loaded/initialized
                         
     def just_before_simulating(self):
         super().just_before_simulating()
         #additional code to run just before beginning the simulation goes below
         #runs immediately before simulating, no manual changes permitted to changes implemented here
         
     def simulation_loop(self):
```

### Comparing `pyphasefield-1.2.0/pyphasefield/Engines/Diffusion.py` & `pyphasefield-2.0.0/pyphasefield/Engines/Diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 import numpy as np
 from scipy.sparse.linalg import gmres
-
-try:
-    #import from within Engines folder
-    from ..field import Field
-    from ..simulation import Simulation
-    from ..ppf_utils import COLORMAP_OTHER, COLORMAP_PHASE
-except:
-    try:
-        #import classes from pyphasefield library
-        from pyphasefield.field import Field
-        from pyphasefield.simulation import Simulation
-        from pyphasefield.ppf_utils import COLORMAP_OTHER, COLORMAP_PHASE
-    except:
-        raise ImportError("Cannot import from pyphasefield library!")
+from pyphasefield.field import Field
+from pyphasefield.simulation import Simulation
+from pyphasefield.ppf_utils import COLORMAP_OTHER, COLORMAP_PHASE
         
 try:
     from numba import cuda
 except:
-    pass
+    import pyphasefield.jit_placeholder as cuda
+
+
 
 def diffusion_matrix_1d(xsize, centervalue, neighborvalue):
     """
     Creates a matrix for the solution of 1d implicit or crank nickolson discretizations
     
     Because the exact format changes between implicit and C-N, and this method is reused 
     in 2D and 3D cases, centervalue and neighbor value must be explicitly specified
@@ -638,46 +629,46 @@
             c[i, j], exitCode = gmres(matrix1d_x, c[i, j], atol='legacy')
     sim.fields[0].data = c   
     
 @cuda.jit
 def diffusion_kernel_1D(fields, fields_out, D, dx, dt):
     startx = cuda.grid(1)      
     stridex = cuda.gridsize(1) 
-    
+
     alpha = D*dt/(dx*dx) #laplacian coefficient in diffusion discretization
-    
+
     c = fields[0]
     c_out = fields_out[0]
 
     # assuming x and y inputs are same length
     for i in range(startx, c.shape[1], stridex):
         c_out[i] = c[i]+alpha*(-2*c[i]+c[i+1]+c[i-1])
-            
+
 @cuda.jit
 def diffusion_kernel_2D(fields, fields_out, D, dx, dt):
     startx, starty = cuda.grid(2)      
     stridex, stridey = cuda.gridsize(2) 
-    
+
     alpha = D*dt/(dx*dx) #laplacian coefficient in diffusion discretization
-    
+
     c = fields[0]
     c_out = fields_out[0]
 
     # assuming x and y inputs are same length
     for i in range(starty, c.shape[0], stridey):
         for j in range(startx, c.shape[1], stridex):
             c_out[i][j] = c[i][j]+alpha*(-4*c[i][j]+c[i+1][j]+c[i-1][j]+c[i][j+1]+c[i][j-1])
-            
+
 @cuda.jit
 def diffusion_kernel_3D(fields, fields_out, D, dx, dt):
     startx, starty, startz = cuda.grid(3)      
     stridex, stridey, startz = cuda.gridsize(3) 
-    
+
     alpha = D*dt/(dx*dx) #laplacian coefficient in diffusion discretization
-    
+
     c = fields[0]
     c_out = fields_out[0]
 
     # assuming x and y inputs are same length
     for i in range(startz, c.shape[0], stridez):
         for j in range(starty, c.shape[1], stridey):
             for k in range(startx, c.shape[2], stridex):
@@ -691,15 +682,14 @@
     elif(len(sim.dimensions) == 2):
         diffusion_kernel_2D[sim._gpu_blocks_per_grid_2D, sim._gpu_threads_per_block_2D](sim._fields_gpu_device, sim._fields_out_gpu_device, 
                                                                   sim.user_data["D"], sim.dx, sim.dt)
     elif(len(sim.dimensions) == 3):
         diffusion_kernel_3D[sim._gpu_blocks_per_grid_3D, sim._gpu_threads_per_block_3D](sim._fields_gpu_device, sim._fields_out_gpu_device, 
                                                                   sim.user_data["D"], sim.dx, sim.dt)
     cuda.synchronize()
-    sim._fields_gpu_device, sim._fields_out_gpu_device = sim._fields_out_gpu_device, sim._fields_gpu_device
 
 class Diffusion(Simulation):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
             
     def init_fields(self):
         #initialization of fields code goes here
@@ -709,45 +699,48 @@
             self.user_data["D"] = 0.1
         if not ("solver" in self.user_data):
             self.user_data["solver"] = "explicit"
         if not ("adi" in self.user_data):
             self.user_data["adi"] = False
         if not ("gmres" in self.user_data):
             self.user_data["gmres"] = False
+            
+        #create field using local dimensions, but modify the array using global dimensions
+        #slicing the field will account for the global -> local conversion!
+        dim_global = self._global_dimensions
         dim = self.dimensions
         c = np.zeros(dim)
+        
+        self.add_field(c, "c")
+        field = self.fields[0]
         if(len(dim) == 1):
-            length = dim[0]
-            c[length // 4:3 * length // 4] = 1
+            for i in range(dim_global[0]//100 + 1):
+                field[100*i:100*i+50] = 1
         elif(len(dim) == 2):
-            length = dim[0]
-            width = dim[1]
-            c[length // 4:3 * length // 4, width // 4:3 * width // 4] = 1
+            for i in range(dim_global[0]//100 + 1):
+                for j in range(dim_global[1]//100 + 1):
+                    field[100*i:100*i+50, 100*j:100*j+50] = 1
+                    field[100*i+50:100*i+100, 100*j+50:100*j+100] = 1
         elif(len(dim) == 3):
-            length = dim[0]
-            width = dim[1]
-            depth = dim[2]
-            c[length // 4:3 * length // 4, width // 4:3 * width // 4, depth // 4:3 * depth // 4] = 1
-        self.add_field(c, "c")
-        
-    def initialize_fields_and_imported_data(self):
-        super().initialize_fields_and_imported_data()
-        #initialization of fields/imported data goes below
-        #runs *after* tdb, thermal, fields, and boundary conditions are loaded/initialized
+            for i in range(dim_global[0]//100 + 1):
+                for j in range(dim_global[1]//100 + 1):
+                    for k in range(dim_global[2]//100 + 1):
+                        field[100*i:100*i+50, 100*j:100*j+50, 100*j:100*j+50] = 1
+                        field[100*i+50:100*i+100, 100*j+50:100*j+100, 100*j+50:100*j+100] = 1
                         
     def just_before_simulating(self):
         super().just_before_simulating()
         #additional code to run just before beginning the simulation goes below
         #runs immediately before simulating, no manual changes permitted to changes implemented here
         
     def simulation_loop(self):
         solver = self.user_data["solver"]
         gmres = self.user_data["gmres"]
         adi = self.user_data["adi"]
-        if(self._framework == "GPU_SERIAL"):
+        if(self._framework == "GPU_SERIAL" or self._framework == "GPU_PARALLEL"):
             engine_DiffusionGPU(self)
         else: #"CPU_SERIAL"
             if (solver == "explicit"):
                 engine_ExplicitDiffusion(self)
             elif (solver == "implicit"):
                 if(len(dim) == 1):
                     if(gmres):
```

### Comparing `pyphasefield-1.2.0/pyphasefield/Engines/NCGPU.py` & `pyphasefield-2.0.0/pyphasefield/Engines/NCGPU.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 import numpy as np
 import sympy as sp
 from scipy.sparse.linalg import gmres
-from numba import cuda
-import numba
 import matplotlib.pyplot as plt
 np.set_printoptions(threshold=np.inf)
 import math
-from numba.cuda.random import create_xoroshiro128p_states, xoroshiro128p_uniform_float32
+from pyphasefield.field import Field
+from pyphasefield.simulation import Simulation
+from pyphasefield.ppf_utils import COLORMAP_OTHER, COLORMAP_PHASE
 
 try:
-    #import from within Engines folder
-    from ..field import Field
-    from ..simulation import Simulation
-    from ..ppf_utils import COLORMAP_OTHER, COLORMAP_PHASE
+    from numba import cuda
+    import numba
+    from numba.cuda.random import create_xoroshiro128p_states, xoroshiro128p_uniform_float32
 except:
-    try:
-        #import classes from pyphasefield library
-        from pyphasefield.field import Field
-        from pyphasefield.simulation import Simulation
-        from pyphasefield.ppf_utils import COLORMAP_OTHER, COLORMAP_PHASE
-    except:
-        raise ImportError("Cannot import from pyphasefield library!")
+    import pyphasefield.jit_placeholder as numba
+    import pyphasefield.jit_placeholder as cuda
 
 ufunc_g_l = None
 ufunc_g_s = None
 
 @cuda.jit(device=True)
 def divagradb(a, axp, axm, ayp, aym, b, bxp, bxm, byp, bym, idx): 
     return 0.5*idx*idx*((axp+a)*(bxp-b) - (a+axm)*(b-bxm) + (ayp+a)*(byp-b) - (a+aym)*(b-bym))
@@ -305,14 +299,16 @@
     stridex, stridey = cuda.gridsize(2) 
     threadId = startx + starty*stridex
     
     v_m = params[2]
     D_L = params[7]
     D_S = params[8]
     noise_amp_c = params[13]
+    thermo_finite_diff_incr = params[15]
+    tfdi_inv = 1./thermo_finite_diff_incr
     W = c_params[4]
     
     phi = fields[0]
     q1 = fields[1]
     q4 = fields[2]
     #c is fields 3 to k, where k equals the number of components +1. 
     #For N components this is N-1 fields, the last one being implicitly defined
@@ -339,25 +335,25 @@
             #NEEDS FIXING vvvvvvvvvv
             G_L[i][j] = get_thermodynamics(ufunc_g_l, ufunc_array[i][j])
             G_S[i][j] = get_thermodynamics(ufunc_g_s, ufunc_array[i][j])
             
             g = (phi[i][j]**2)*(1-phi[i][j])**2
             h = (phi[i][j]**3)*(6.*phi[i][j]**2 - 15.*phi[i][j] + 10.)
             
-            ufunc_array[i][j][len(fields)-3] -= 0.0000001
+            ufunc_array[i][j][len(fields)-3] -= thermo_finite_diff_incr
             for l in range(3, len(fields)):
-                ufunc_array[i][j][l-3] += 0.0000001
-                dGLdc = 10000000.*(get_thermodynamics(ufunc_g_l, ufunc_array[i][j])-G_L[i][j])
-                dGSdc = 10000000.*(get_thermodynamics(ufunc_g_s, ufunc_array[i][j])-G_S[i][j])
+                ufunc_array[i][j][l-3] += thermo_finite_diff_incr
+                dGLdc = tfdi_inv*(get_thermodynamics(ufunc_g_l, ufunc_array[i][j])-G_L[i][j])
+                dGSdc = tfdi_inv*(get_thermodynamics(ufunc_g_s, ufunc_array[i][j])-G_S[i][j])
                 M_c = transfer[l-1]
                 dFdc = transfer[l-1+len(fields)-3]
                 M_c[i][j] = v_m*fields[l][i][j]*(D_L + h*(D_S - D_L))/(8.314*T[i][j])
                 dFdc[i][j] = (dGLdc + h*(dGSdc-dGLdc))/v_m + (W[l-3]-W[len(fields)-3])*g*T[i][j]
-                ufunc_array[i][j][l-3] -= 0.0000001
-            ufunc_array[i][j][len(fields)-3] += 0.0000001
+                ufunc_array[i][j][l-3] -= thermo_finite_diff_incr
+            ufunc_array[i][j][len(fields)-3] += thermo_finite_diff_incr
                     
                 
 def make_seed(phi, q1, q4, x, y, angle, seed_radius):
     shape = phi.shape
     qrad = seed_radius+5
     x_size = shape[1]
     y_size = shape[0]
@@ -531,14 +527,17 @@
             self.user_data["d_ratio"] = 4.
         if not "noise_phi" in self.user_data:
             self.user_data["noise_phi"] = 1.
         if not "noise_c" in self.user_data:
             self.user_data["noise_c"] = 1.
         if not "noise_q" in self.user_data:
             self.user_data["noise_q"] = 1.
+        #initialize finite diff approximation for thermodynamic gradient terms to 1e-7, approx. half the digits of precision of doubles
+        if not "thermo_finite_diff_incr" in self.user_data:
+            self.user_data["thermo_finite_diff_incr"] = 0.0000001;
         params = []
         c_params = []
         params.append(self.dx)
         params.append(self.user_data["d"])
         params.append(self.user_data["v_m"])
         params.append(self.user_data["M_qmax"])
         params.append(self.user_data["H"])
@@ -548,14 +547,15 @@
         params.append(self.user_data["D_S"])
         params.append(self.dt)
         params.append(self.user_data["ebar"])
         params.append(self.user_data["eqbar"])
         params.append(self.user_data["noise_phi"])
         params.append(self.user_data["noise_c"])
         params.append(self.user_data["noise_q"])
+        params.append(self.user_data["thermo_finite_diff_incr"])
         c_params.append(self.user_data["L"])
         c_params.append(self.user_data["T_M"])
         c_params.append(self.user_data["S"])
         c_params.append(self.user_data["B"])
         c_params.append(self.user_data["W"])
         c_params.append(self.user_data["M"])
         self.user_data["params"] = np.array(params)
@@ -604,9 +604,8 @@
                                                                       self.user_data["rng_states"], self._tdb_ufunc_gpu_device, 
                                                                       self.user_data["params"], self.user_data["c_params"])
             cuda.synchronize()
             NComponent_kernel[self._gpu_blocks_per_grid_3D, self._gpu_threads_per_block_3D](self._fields_gpu_device, 
                                                                       self._temperature_gpu_device, self._fields_transfer_gpu_device, 
                                                                       self._fields_out_gpu_device, self.user_data["rng_states"], 
                                                                       self.user_data["params"], self.user_data["c_params"])
-        cuda.synchronize()
-        self._fields_gpu_device, self._fields_out_gpu_device = self._fields_out_gpu_device, self._fields_gpu_device
+        cuda.synchronize()
```

### Comparing `pyphasefield-1.2.0/pyphasefield/Engines/NComponent.py` & `pyphasefield-2.0.0/pyphasefield/Engines/NComponent.py`

 * *Files identical despite different names*

### Comparing `pyphasefield-1.2.0/pyphasefield/Engines/Warren1995.py` & `pyphasefield-2.0.0/pyphasefield/Engines/Warren1995.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,18 @@
 import numpy as np
 import math
-
-try:
-    #import from within Engines folder
-    from ..field import Field
-    from ..simulation import Simulation
-    from ..ppf_utils import COLORMAP_OTHER, COLORMAP_PHASE_INV
-except:
-    try:
-        #import classes from pyphasefield library
-        from pyphasefield.field import Field
-        from pyphasefield.simulation import Simulation
-        from pyphasefield.ppf_utils import COLORMAP_OTHER, COLORMAP_PHASE_INV
-    except:
-        raise ImportError("Cannot import from pyphasefield library!")
+from pyphasefield.field import Field
+from pyphasefield.simulation import Simulation
+from pyphasefield.ppf_utils import COLORMAP_OTHER, COLORMAP_PHASE_INV
         
 try:
     from numba import cuda
     from numba.cuda.random import create_xoroshiro128p_states, xoroshiro128p_uniform_float32
 except:
-    pass
+    import pyphasefield.jit_placeholder as cuda
 
 def __p(phi):
     return phi*phi*phi*(10-15*phi+6*phi*phi)
 
 def __g(phi):
     return (phi*phi*(1-phi)*(1-phi))
 
@@ -322,20 +311,14 @@
         diamond_size = self.user_data["diamond_size"]
         for i in range(diamond_size):
             phi[(int)(dim[0]/2-i):(int)(dim[0]/2+i), ((int)(dim[1]/2-(diamond_size-i))):(int)(dim[1]/2+(diamond_size-i))] = 0
         self.add_field(phi, "phi", colormap=COLORMAP_PHASE_INV)
         c = np.zeros(dim)
         c += self.user_data["initial_concentration"]
         self.add_field(c, "c", colormap=COLORMAP_OTHER)
-        
-        
-    def initialize_fields_and_imported_data(self):
-        super().initialize_fields_and_imported_data()
-        #initialization of fields/imported data goes below
-        #runs *after* tdb, thermal, fields, and boundary conditions are loaded/initialized
                         
     def just_before_simulating(self):
         super().just_before_simulating()
         #additional code to run just before beginning the simulation goes below
         #runs immediately before simulating, no manual changes permitted to changes implemented here
         self.set_time_step_length(self.get_cell_spacing()**2/5./self.user_data["D_L"])
         self.user_data["d"] = self.get_cell_spacing()/0.94 #interfacial thickness
@@ -358,16 +341,16 @@
             params.append(self.user_data["alpha"])
             c_params.append([self.user_data["L_A"], self.user_data["L_B"]])
             c_params.append([self.user_data["T_MA"], self.user_data["T_MB"]])
             c_params.append([self.user_data["S_A"], self.user_data["S_B"]])
             c_params.append([self.user_data["B_A"], self.user_data["B_B"]])
             c_params.append([self.user_data["W_A"], self.user_data["W_B"]])
             c_params.append([self.user_data["M_A"], self.user_data["M_B"]])
-            self.user_data["params"] = np.array(params)
-            self.user_data["c_params"] = np.array(c_params)
+            self.user_data["params"] = cuda.to_device(np.array(params))
+            self.user_data["c_params"] = cuda.to_device(np.array(c_params))
             self.user_data["rng_states"] = create_xoroshiro128p_states(256*256, seed=1)
         
     def simulation_loop(self):
         #code to run each simulation step goes here
         if(self._uses_gpu):
             cuda.synchronize()
             Warren1995_helper_kernel[self._gpu_blocks_per_grid_2D, self._gpu_threads_per_block_2D](self._fields_gpu_device,
```

### Comparing `pyphasefield-1.2.0/pyphasefield/Engines/__init__.py` & `pyphasefield-2.0.0/pyphasefield/Engines/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from inspect import isclass
 from pkgutil import iter_modules
 from pathlib import Path
 from importlib import import_module
 
-from .Diffusion import Diffusion
-
 # iterate through the modules in the current package
 package_dir = Path(__file__).resolve().parent
 for (_, module_name, _) in iter_modules([package_dir]):
 
     try:
         # import the module and iterate through its attributes
         module = import_module(f"{__name__}.{module_name}")
         for attribute_name in dir(module):
             attribute = getattr(module, attribute_name)
     
             if isclass(attribute):            
                 # Add the class to this package's variables
                 globals()[attribute_name] = attribute
     except Exception as e:
-        print(e)
+        print(module_name+", "+str(e))
         pass
```

### Comparing `pyphasefield-1.2.0/pyphasefield/tests/test_Diffusion.py` & `pyphasefield-2.0.0/pyphasefield/tests/test_Diffusion.py`

 * *Files identical despite different names*

### Comparing `pyphasefield-1.2.0/pyphasefield/tests/test_NComponent.py` & `pyphasefield-2.0.0/pyphasefield/tests/test_NComponent.py`

 * *Files identical despite different names*

### Comparing `pyphasefield-1.2.0/pyphasefield/tests/test_SaveLoad.py` & `pyphasefield-2.0.0/pyphasefield/tests/test_SaveLoad.py`

 * *Files identical despite different names*

### Comparing `pyphasefield-1.2.0/pyphasefield.egg-info/PKG-INFO` & `pyphasefield-2.0.0/pyphasefield.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
-Name: pyphasefield
-Version: 1.2.0
-Summary: Python phase field simulation
-Home-page: https://github.com/AdditiveModeling/pyphasefield
-Author: Scott Peters
-Author-email: scott@dpeters.net
-License: UNKNOWN
-Description: # PyPhaseField
-        
-        Python-based phase field software, built using numpy and pycalphad. 
-        Content will be added soon-TM, once i figure out this whole packaging thing
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: pyphasefield
+Version: 2.0.0
+Summary: Python phase field simulation
+Home-page: https://github.com/AdditiveModeling/pyphasefield
+Author: Scott Peters
+Author-email: scott@dpeters.net
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PyPhaseField
+
+Python-based phase field software, built using numpy and pycalphad. 
+Content will be added soon-TM, once i figure out this whole packaging thing
```

### Comparing `pyphasefield-1.2.0/pyphasefield.egg-info/SOURCES.txt` & `pyphasefield-2.0.0/pyphasefield.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+LICENSE
 README.md
 setup.py
 pyphasefield/__init__.py
+pyphasefield/__main__.py
 pyphasefield/field.py
+pyphasefield/jit_placeholder.py
+pyphasefield/parallel_utils.py
 pyphasefield/ppf_gpu_utils.py
 pyphasefield/ppf_utils.py
 pyphasefield/simulation.py
 pyphasefield.egg-info/PKG-INFO
 pyphasefield.egg-info/SOURCES.txt
 pyphasefield.egg-info/dependency_links.txt
-pyphasefield.egg-info/requires.txt
 pyphasefield.egg-info/top_level.txt
 pyphasefield/Engines/AnisoDorrGPU.py
 pyphasefield/Engines/CahnAllen.py
 pyphasefield/Engines/CahnHilliard.py
 pyphasefield/Engines/Diffusion.py
-pyphasefield/Engines/DiffusionGPU.py
 pyphasefield/Engines/NCGPU.py
 pyphasefield/Engines/NCGPU_new.py
 pyphasefield/Engines/NComponent.py
 pyphasefield/Engines/Template.py
 pyphasefield/Engines/Warren1995.py
 pyphasefield/Engines/__init__.py
 pyphasefield/tests/__init__.py
```

### Comparing `pyphasefield-1.2.0/setup.py` & `pyphasefield-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyphasefield",
-    version="1.2.0",
+    version="2.0.0",
     author="Scott Peters",
     author_email="scott@dpeters.net",
     description="Python phase field simulation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AdditiveModeling/pyphasefield",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 	install_requires=[
-        "numpy",
-		"scipy",
-		"matplotlib",
-		"meshio",
-        "tinydb",
     ],
     python_requires='>=3.6',
 )
```

