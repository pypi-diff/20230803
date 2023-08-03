# Comparing `tmp/spelunker-1.0.0.tar.gz` & `tmp/spelunker-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spelunker-1.0.0.tar", last modified: Mon Jul 24 23:48:17 2023, max compression
+gzip compressed data, was "spelunker-1.0.1.tar", last modified: Thu Aug  3 01:37:26 2023, max compression
```

## Comparing `spelunker-1.0.0.tar` & `spelunker-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-24 23:48:17.179870 spelunker-1.0.0/
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     1085 2023-07-19 23:46:23.000000 spelunker-1.0.0/LICENSE
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4561 2023-07-24 23:48:17.180246 spelunker-1.0.0/PKG-INFO
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4022 2023-07-21 13:51:03.000000 spelunker-1.0.0/README.md
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      160 2023-07-24 23:48:17.181407 spelunker-1.0.0/setup.cfg
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     1047 2023-07-20 15:20:44.000000 spelunker-1.0.0/setup.py
-drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-24 23:48:17.174606 spelunker-1.0.0/spelunker.egg-info/
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4561 2023-07-24 23:48:16.000000 spelunker-1.0.0/spelunker.egg-info/PKG-INFO
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      298 2023-07-24 23:48:17.000000 spelunker-1.0.0/spelunker.egg-info/SOURCES.txt
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)        1 2023-07-24 23:48:16.000000 spelunker-1.0.0/spelunker.egg-info/dependency_links.txt
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)        1 2023-07-24 23:48:16.000000 spelunker-1.0.0/spelunker.egg-info/not-zip-safe
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       74 2023-07-24 23:48:16.000000 spelunker-1.0.0/spelunker.egg-info/requires.txt
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       10 2023-07-24 23:48:16.000000 spelunker-1.0.0/spelunker.egg-info/top_level.txt
-drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-07-24 23:48:17.178588 spelunker-1.0.0/src/
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      121 2023-07-19 19:56:38.000000 spelunker-1.0.0/src/__init__.py
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       21 2023-07-24 23:47:02.000000 spelunker-1.0.0/src/_version.py
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      420 2023-07-20 15:20:44.000000 spelunker-1.0.0/src/dashboard.py
--rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)    50750 2023-07-24 23:47:30.000000 spelunker-1.0.0/src/spelunker.py
+drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-08-03 01:37:26.811106 spelunker-1.0.1/
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     1085 2023-07-19 23:46:23.000000 spelunker-1.0.1/LICENSE
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4693 2023-08-03 01:37:26.811249 spelunker-1.0.1/PKG-INFO
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4154 2023-08-03 01:35:57.000000 spelunker-1.0.1/README.md
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      160 2023-08-03 01:37:26.811787 spelunker-1.0.1/setup.cfg
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     1047 2023-08-03 01:06:37.000000 spelunker-1.0.1/setup.py
+drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-08-03 01:37:26.808675 spelunker-1.0.1/spelunker.egg-info/
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)     4693 2023-08-03 01:37:26.000000 spelunker-1.0.1/spelunker.egg-info/PKG-INFO
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      298 2023-08-03 01:37:26.000000 spelunker-1.0.1/spelunker.egg-info/SOURCES.txt
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)        1 2023-08-03 01:37:26.000000 spelunker-1.0.1/spelunker.egg-info/dependency_links.txt
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)        1 2023-08-03 01:37:26.000000 spelunker-1.0.1/spelunker.egg-info/not-zip-safe
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       74 2023-08-03 01:37:26.000000 spelunker-1.0.1/spelunker.egg-info/requires.txt
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       10 2023-08-03 01:37:26.000000 spelunker-1.0.1/spelunker.egg-info/top_level.txt
+drwxr-xr-x   0 ddeal     (5761) STSCI\science  (1031)        0 2023-08-03 01:37:26.810710 spelunker-1.0.1/src/
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      121 2023-07-19 19:56:38.000000 spelunker-1.0.1/src/__init__.py
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)       21 2023-08-03 00:59:24.000000 spelunker-1.0.1/src/_version.py
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)      420 2023-07-20 15:20:44.000000 spelunker-1.0.1/src/dashboard.py
+-rw-r--r--   0 ddeal     (5761) STSCI\science  (1031)    51745 2023-08-03 01:26:23.000000 spelunker-1.0.1/src/spelunker.py
```

### Comparing `spelunker-1.0.0/LICENSE` & `spelunker-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spelunker-1.0.0/PKG-INFO` & `spelunker-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spelunker
-Version: 1.0.0
+Version: 1.0.1
 Summary: spelunker: a library to extract guidestar data and observe technical and stellar events
 Home-page: https://github.com/GalagaBits/JWST-FGS-Spelunker
 Author: Derod Deal
 Author-email: dealderod@ufl.edu
 License: MIT
 Keywords: guidestars
 Requires: numpy
@@ -95,14 +95,15 @@
 ```
 <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/mnemonics.png">
 
 For more information on the tools under `spelunker` and how to get started, visit the [quickstart guide](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/fgs-spelunker_quickstart.ipynb). Get acquainted with `spelunker` with the following example notebooks:
 
 - [Guidestar Targets](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/guidestar_targets.ipynb)
 - [Pixel centroid changes and mnemonics](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/pixel_centroid_mnemonics.ipynb)
+- [TSOS Guidestar Demo](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/fgs-spelunker-and-tsos.ipynb)
 
 
 ## Licence and attribution
 
 This project is under the MIT License, which can be viewed [here](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/LICENSE).
 
 ## Acknowledgments
```

### Comparing `spelunker-1.0.0/README.md` & `spelunker-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 ```
 <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/mnemonics.png">
 
 For more information on the tools under `spelunker` and how to get started, visit the [quickstart guide](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/fgs-spelunker_quickstart.ipynb). Get acquainted with `spelunker` with the following example notebooks:
 
 - [Guidestar Targets](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/guidestar_targets.ipynb)
 - [Pixel centroid changes and mnemonics](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/pixel_centroid_mnemonics.ipynb)
+- [TSOS Guidestar Demo](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/fgs-spelunker-and-tsos.ipynb)
 
 
 ## Licence and attribution
 
 This project is under the MIT License, which can be viewed [here](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/LICENSE).
 
 ## Acknowledgments
```

### Comparing `spelunker-1.0.0/setup.py` & `spelunker-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `spelunker-1.0.0/spelunker.egg-info/PKG-INFO` & `spelunker-1.0.1/spelunker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spelunker
-Version: 1.0.0
+Version: 1.0.1
 Summary: spelunker: a library to extract guidestar data and observe technical and stellar events
 Home-page: https://github.com/GalagaBits/JWST-FGS-Spelunker
 Author: Derod Deal
 Author-email: dealderod@ufl.edu
 License: MIT
 Keywords: guidestars
 Requires: numpy
@@ -95,14 +95,15 @@
 ```
 <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/mnemonics.png">
 
 For more information on the tools under `spelunker` and how to get started, visit the [quickstart guide](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/fgs-spelunker_quickstart.ipynb). Get acquainted with `spelunker` with the following example notebooks:
 
 - [Guidestar Targets](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/guidestar_targets.ipynb)
 - [Pixel centroid changes and mnemonics](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/pixel_centroid_mnemonics.ipynb)
+- [TSOS Guidestar Demo](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/fgs-spelunker-and-tsos.ipynb)
 
 
 ## Licence and attribution
 
 This project is under the MIT License, which can be viewed [here](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/LICENSE).
 
 ## Acknowledgments
```

### Comparing `spelunker-1.0.0/src/spelunker.py` & `spelunker-1.0.1/src/spelunker.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,43 +36,37 @@
 except ImportError:
     jwstuser_installed = False
     print('jwstuser is not installed. mnemonics() will not work.')
 
 
 class load:
 
-    init_dir = os.getcwd()
 
     def __init__(self, dir='None', pid='None', obs_num='None',  visit='None', visit_group='None', parallel_sequnence_id='None', 
-                 activity_number='None', exposure_number='None', dir_seg='None', guider='None', calib_level=2, save=False):
-        
-        os.chdir(self.init_dir)
+                 activity_number='None', exposure_number='None', dir_seg='None', guider='None', calib_level=2, save=False, token = None):
+
+        self.init_dir = os.getcwd()
 
         created_dir = "spelunker_outputs"
-        current_dir = self.init_dir
 
         if dir != 'None':
-            os.chdir(dir)
             if not os.path.exists(dir+'/'+created_dir):  #https://www.geeksforgeeks.org/how-to-create-directory-if-it-does-not-exist-using-python/
                 os.makedirs(created_dir)
-                temp_dirc = created_dir
-            else:
-                temp_dirc = created_dir
+        
+            self.directory = dir+created_dir
 
         else:
-            if not os.path.exists(current_dir+'/'+created_dir):
+            if not os.path.exists(self.init_dir+'/'+created_dir):
                 os.makedirs(created_dir)
-                temp_dirc = created_dir
-            else:
-                temp_dirc = created_dir
+        
+            self.directory = os.getcwd()+'/'+created_dir
 
-        self.directory = os.getcwd()+'/'+temp_dirc
         print('Current working directory for spelunker: '+self.directory+'\n')
 
-        self.mast_api_token = None
+        self.mast_api_token = token
         self.fg_table = None
 
         self.fg_array = None
         self.fg_time = None
         self.fg_flux = None
 
         self.gaussfit_results = None
@@ -80,15 +74,15 @@
 
         self.object_properties = None
 
         self.fontsize = 14
         
         if pid != 'None':
             self.download(pid, obs_num=obs_num, visit=visit, visit_group=visit_group, parallel_sequnence_id=parallel_sequnence_id,
-                          activity_number=activity_number, exposure_number=exposure_number, dir_seg=dir_seg, guider=guider, calib_level=calib_level, save=save)
+                          activity_number=activity_number, exposure_number=exposure_number, dir_seg=dir_seg, guider=guider, calib_level=calib_level, save=save, token = token)
 
     def stitcher(self, fg_timeseries):
         '''
         Stitches multiple projectids with respect to epoch in one single array.
         '''
         fg_cube = []
         for data in fg_timeseries:
@@ -154,15 +148,14 @@
         table['fg_flux'] = fg_flux
 
         sort_table = table.sort(['fg_time'])
 
         return np.array(table['fg_array']), np.array(table['fg_time']), np.array(table['fg_flux'])
 
 
-
     '''
     DOWNLOADING FROM ASTROQUERY AND READING FILES
     ------------------------------------------------------------------------------------------------------
     '''
 
     def duplicate_rm(self, products):
         '''
@@ -180,23 +173,26 @@
             else:
                 duplicates_mask.append(False)
         
         return products[duplicates_mask]
 
 
     def download(self, pid, obs_num='None',  visit='None', visit_group='None', parallel_sequnence_id='None', 
-                 activity_number='None', exposure_number='None', dir_seg='None', guider='None', calib_level=2, save=False):
+                 activity_number='None', exposure_number='None', dir_seg='None', guider='None', calib_level=2, 
+                 save=False, token=None):
         '''
         Downloads the data from the projectid website. Turns the projectid into a manageable
         fits file. Downloads the files onto a local directory.
         '''
 
-        self.pid = pid
+        if token is not None:
+
+            Observations.login(token=token)
 
-        os.chdir(self.directory)
+        self.pid = pid
 
         if obs_num == 'None' and visit != 'None':
             raise ValueError('When a visit is identified, the obs_num needs to be identified.')
 
         print("Connecting with astroquery...")
         
         if obs_num != 'None' and visit != 'None':
@@ -285,23 +281,28 @@
             mask = products['calib_level'] == int(calib_level)
             productsx = products[mask]
 
         productsx = self.duplicate_rm(productsx)
 
         manifest = Observations.download_products(productsx,)
 
-        os.chdir(self.directory+'/mastDownload/JWST/')
-        fg_raw = sorted(glob.glob('**/jw0'+str(pid)+'**_gs-fg_**_cal.fits'))
+        fg_raw = sorted(glob.glob(self.directory+'/mastDownload/JWST/'+'**/jw0'+str(pid)+'**_gs-fg_**_cal.fits'))
+
+        if len(fg_raw) == 0:
+
+            raise Exception('No files were downloaded for program '+str(pid)+'. Two common causes of this issue are: \n'+\
+                           +' 1.- You do not have exclusive access rights to see the data. If you have a MAST API, ingest it via spelunker.load(..., token = "yourtoken").\n'+\
+                           +' 2.- There is no guidestar data for your program as of yet in MAST.')
 
         fg = []
         sliced_directory = []
 
         for i in fg_raw:
                 fg.append(i.rsplit('/')[-1])
-                sliced_directory.append(i.split('/')[0])
+                sliced_directory.append(i.split('/')[-2])
 
         fg_table = Table()
 
         fg_table['filenames'] = fg
         fg_table['sliced_directory'] = sliced_directory
 
         obs_num_col = []
@@ -374,19 +375,21 @@
                 fg_table = fg_table[mask8]
 
         elif guider != 'None':
                 mask8 = fg_table['guider'] == int(guider)
                 fg_table = fg_table[mask8]    
 
         f_slash = []
+        mastDownload_dir = []
         for i in range(len(fg_table['filenames'])):
             f_slash.append('/')
+            mastDownload_dir.append(self.directory+'/mastDownload/JWST/')
 
         reformed_directory = np.char.add(np.char.add(fg_table['sliced_directory'], f_slash), fg_table['filenames'])
-        fg_table['reformed_directory'] = reformed_directory
+        fg_table['reformed_directory'] = np.char.add(mastDownload_dir, reformed_directory)
 
         gs_id = []
         guidestar_time = []
         object_fg = []
 
         self.fg_datamodel = datamodels.open(list(fg_table['reformed_directory']))
 
@@ -398,15 +401,15 @@
 
         fg_table['gs_id'] = gs_id
         fg_table['guidestar_time'] = guidestar_time
         fg_table['object_fg'] = object_fg
         # Reads in all fits files from reformed_directory
         #fg1 = datamodels.open(list(reformed_directory))
 
-        sort_table = fg_table.sort(['guidestar_time'])
+        _ = fg_table.sort(['guidestar_time'])
 
         self.fg_datamodel = list(fg_table['object_fg'])
         self.fg_table = fg_table
 
         self.fg_timeseries = [fn for fn in self.fg_datamodel]
 
         all_times = []
@@ -435,41 +438,47 @@
 
             norm_array, norm_flux = self.normalization_flux_preprocessing()
 
             fg_time = self.stitcher(all_times)
 
             fg_array, fg_time, fg_flux = self.negative_flux_preprocessing(norm_array, fg_time, norm_flux)
 
+        data_table = Table()
+        data_table['spatial'] = fg_array
+        data_table['time'] = fg_time
+        data_table['flux'] = fg_flux
 
-        # Saving numpy arrays
+        _ = data_table.sort(['time'])
 
-        os.chdir(self.directory)
+        
+        # Saving numpy arrays
 
         if save:
             data_arrays_dir = 'data_arrays'
             if not os.path.exists(data_arrays_dir):
                 os.makedirs(data_arrays_dir)
 
-            os.chdir(self.directory+'/'+data_arrays_dir)
-            np.save('pid_'+str(pid)+'_fg_array', fg_array)
-            np.save('pid_'+str(pid)+'_fg_time', fg_time)
-            np.save('pid_'+str(pid)+'_fg_flux', fg_flux)
-
-            os.chdir(self.directory)
-
-        self.fg_array = fg_array
-        self.fg_time = fg_time
-        self.fg_flux = fg_flux
+            np.save(self.directory+'/'+data_arrays_dir+'/'+'pid_'+str(pid)+'_fg_array', list(data_table['spatial']))
+            np.save(self.directory+'/'+data_arrays_dir+'/'+'pid_'+str(pid)+'_fg_time', list(data_table['time']))
+            np.save(self.directory+'/'+data_arrays_dir+'/'+'pid_'+str(pid)+'_fg_flux', list(data_table['flux']))
+
+        self.fg_array = data_table['spatial']
+        self.fg_time = data_table['time']
+        self.fg_flux = data_table['flux']
 
         self.fg_table = self.table()
         self.object_properties = self.object_properties_func()
+
+        if token is not None:
+
+            Observations.logout()
     
     def object_properties_func(self,):
 
-        object_table = pd.DataFrame(columns=['guidestar_catalog_id', 'gaiadr1ID','gaiadr1ID', 'int_start', 'int_stop', 'ra', 'dec', 'Jmag', 'Hmag'])
+        object_table = pd.DataFrame(columns=['guidestar_catalog_id', 'gaiadr1ID','gaiadr2ID', 'int_start', 'int_stop', 'ra', 'dec', 'Jmag', 'Hmag'])
 
         for idx, gs_id in enumerate(self.fg_table['gs_id']):
 
             row = []
 
             if gs_id not in list(object_table['guidestar_catalog_id']):
 
@@ -554,14 +563,15 @@
 
 
     '''
     FITTING TOOLS
     ------------------------------------------------------------------------------------------------------
     '''
 
+
     def gauss2d_fit(self, fg_array='None', ncpus=4, save=False):
         '''
         Applies a spatial gaussian fit to a data array for guide star data. The gaussian parameters
         include amplitude, centriods, stddev, and theta. Uses ray. Outputs an astopy table.
         '''
         if type(fg_array) == str:
             if fg_array == 'None':
@@ -656,17 +666,17 @@
 
         table = Table(rows=rows5, names=['amplitude','x_mean', 'y_mean', 'x_stddev', 'y_stddev', 'theta', 'offset'])
 
         self.gaussfit_results = table
         
         if save:
             gaussfits_array_dir = 'gaussfits'
-            if not os.path.exists(gaussfits_array_dir):
-                os.makedirs(gaussfits_array_dir)
-            table.write(str(self.pid)+'_'+gaussfits_array_dir+'.dat', format='ascii', overwrite=True)
+            if not os.path.exists(self.directory+'/'+gaussfits_array_dir):
+                os.makedirs(self.directory+'/'+gaussfits_array_dir)
+            table.write(self.directory+'/'+gaussfits_array_dir+'/'+str(self.pid)+'_'+gaussfits_array_dir+'.dat', format='ascii', overwrite=True)
 
         return table
     
     def quick_fit(self, fg_array='None', save=False):
         '''
         Performs a quick fit to an array of fg data. Outputs an astropy table
         '''
@@ -718,17 +728,17 @@
         quick_fit_table['theta'] = 0
         quick_fit_table['offset'] = 0
 
         self.quickfit_results = quick_fit_table
         
         if save:
             quickfits_array_dir = 'quickfits'
-            if not os.path.exists(quickfits_array_dir):
-                os.makedirs(quickfits_array_dir)
-            quick_fit_table.write(str(self.pid)+'_'+quickfits_array_dir+'.dat', format='ascii', overwrite=True)
+            if not os.path.exists(self.directory+'/'+quickfits_array_dir):
+                os.makedirs(self.directory+'/'+quickfits_array_dir)
+            quick_fit_table.write(self.directory+'/'+quickfits_array_dir+'/'+str(self.pid)+'_'+quickfits_array_dir+'.dat', format='ascii', overwrite=True)
 
         return quick_fit_table
 
 
     '''
     POSTPROCESSING METHODS 
     ------------------------------------------------------------------------------------------------------
@@ -1127,17 +1137,17 @@
         self.pgram_x_stddev = pgram_table['frequency_x_stddev'], pgram_table['power_x_stddev']
         self.pgram_y_stddev = pgram_table['frequency_y_stddev'], pgram_table['power_y_stddev']
         self.pgram_theta = pgram_table['frequency_theta'], pgram_table['power_theta']
         self.pgram_offset = pgram_table['frequency_offset'], pgram_table['power_offset']
 
         if save:
             periodogram_dir = 'periodograms'
-            if not os.path.exists(periodogram_dir):
-                os.makedirs(periodogram_dir)
-            table.write(str(self.pid)+'_'+periodogram_dir+'.dat', format='ascii', overwrite=True)
+            if not os.path.exists(self.directory+'/'+periodogram_dir):
+                os.makedirs(self.directory+'/'+periodogram_dir)
+            table.write(self.directory+'/'+periodogram_dir+'/'+str(self.pid)+'_'+periodogram_dir+'.dat', format='ascii', overwrite=True)
         
         return ax
 
 
     '''
     ANIMATIONS 
     ------------------------------------------------------------------------------------------------------
```

