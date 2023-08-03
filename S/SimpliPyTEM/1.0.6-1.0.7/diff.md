# Comparing `tmp/SimpliPyTEM-1.0.6.tar.gz` & `tmp/SimpliPyTEM-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpliPyTEM-1.0.6.tar", last modified: Tue Jun 27 15:39:05 2023, max compression
+gzip compressed data, was "SimpliPyTEM-1.0.7.tar", last modified: Thu Aug  3 10:13:41 2023, max compression
```

## Comparing `SimpliPyTEM-1.0.6.tar` & `SimpliPyTEM-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-06-27 15:39:05.533205 SimpliPyTEM-1.0.6/
--rw-r--r--   0 gabriel    (501) staff       (20)    35149 2023-01-20 17:02:41.000000 SimpliPyTEM-1.0.6/LICENSE
--rw-r--r--   0 gabriel    (501) staff       (20)     1661 2023-06-27 15:39:05.532871 SimpliPyTEM-1.0.6/PKG-INFO
--rw-r--r--   0 gabriel    (501) staff       (20)     2373 2023-04-03 10:12:55.000000 SimpliPyTEM-1.0.6/README.md
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-06-27 15:39:05.524594 SimpliPyTEM-1.0.6/SimpliPyTEM/
--rw-r--r--   0 gabriel    (501) staff       (20)     4267 2023-05-24 11:02:21.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/App_functions.py
--rw-r--r--   0 gabriel    (501) staff       (20)    88246 2023-05-31 17:12:48.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/MicroVideo_class.py
--rw-r--r--   0 gabriel    (501) staff       (20)    74806 2023-06-26 13:33:53.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/Micrograph_class.py
--rw-r--r--   0 gabriel    (501) staff       (20)     3407 2023-05-23 12:31:46.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/Motion_correction.py
--rw-r--r--   0 gabriel    (501) staff       (20)     7491 2023-05-23 12:31:57.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/PDF_generator.py
--rw-r--r--   0 gabriel    (501) staff       (20)    19160 2023-06-08 16:26:21.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/Particle_analysis.py
--rw-r--r--   0 gabriel    (501) staff       (20)     4836 2023-05-23 12:31:57.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/Particle_tracking.py
--rwxr-xr-x   0 gabriel    (501) staff       (20)    27247 2023-06-07 15:24:10.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/SimpliPyTEM_GUI.py
--rw-r--r--   0 gabriel    (501) staff       (20)     7463 2023-06-07 15:23:27.000000 SimpliPyTEM-1.0.6/SimpliPyTEM/html_writer.py
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-06-27 15:39:05.532416 SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/
--rw-r--r--   0 gabriel    (501) staff       (20)     1661 2023-06-27 15:39:05.000000 SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/PKG-INFO
--rw-r--r--   0 gabriel    (501) staff       (20)      517 2023-06-27 15:39:05.000000 SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/SOURCES.txt
--rw-r--r--   0 gabriel    (501) staff       (20)        1 2023-06-27 15:39:05.000000 SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/dependency_links.txt
--rw-r--r--   0 gabriel    (501) staff       (20)       69 2023-06-27 15:39:05.000000 SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/entry_points.txt
--rw-r--r--   0 gabriel    (501) staff       (20)      276 2023-06-27 15:39:05.000000 SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/requires.txt
--rw-r--r--   0 gabriel    (501) staff       (20)       12 2023-06-27 15:39:05.000000 SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/top_level.txt
--rw-r--r--   0 gabriel    (501) staff       (20)       38 2023-06-27 15:39:05.533303 SimpliPyTEM-1.0.6/setup.cfg
--rw-r--r--   0 gabriel    (501) staff       (20)     2216 2023-05-24 11:37:38.000000 SimpliPyTEM-1.0.6/setup.py
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-08-03 10:13:41.229848 SimpliPyTEM-1.0.7/
+-rw-r--r--   0 gabriel    (501) staff       (20)    35149 2023-01-20 17:02:41.000000 SimpliPyTEM-1.0.7/LICENSE
+-rw-r--r--   0 gabriel    (501) staff       (20)     1661 2023-08-03 10:13:41.229510 SimpliPyTEM-1.0.7/PKG-INFO
+-rw-r--r--   0 gabriel    (501) staff       (20)     2373 2023-04-03 10:12:55.000000 SimpliPyTEM-1.0.7/README.md
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-08-03 10:13:41.213395 SimpliPyTEM-1.0.7/SimpliPyTEM/
+-rw-r--r--   0 gabriel    (501) staff       (20)     4267 2023-05-24 11:02:21.000000 SimpliPyTEM-1.0.7/SimpliPyTEM/App_functions.py
+-rw-r--r--   0 gabriel    (501) staff       (20)    93881 2023-07-13 16:33:54.000000 SimpliPyTEM-1.0.7/SimpliPyTEM/MicroVideo_class.py
+-rw-r--r--   0 gabriel    (501) staff       (20)    80250 2023-07-14 08:15:14.000000 SimpliPyTEM-1.0.7/SimpliPyTEM/Micrograph_class.py
+-rw-r--r--   0 gabriel    (501) staff       (20)     3407 2023-05-23 12:31:46.000000 SimpliPyTEM-1.0.7/SimpliPyTEM/Motion_correction.py
+-rw-r--r--   0 gabriel    (501) staff       (20)     7491 2023-05-23 12:31:57.000000 SimpliPyTEM-1.0.7/SimpliPyTEM/PDF_generator.py
+-rw-r--r--   0 gabriel    (501) staff       (20)    19160 2023-06-30 14:56:27.000000 SimpliPyTEM-1.0.7/SimpliPyTEM/Particle_analysis.py
+-rw-r--r--   0 gabriel    (501) staff       (20)     4836 2023-05-23 12:31:57.000000 SimpliPyTEM-1.0.7/SimpliPyTEM/Particle_tracking.py
+-rwxr-xr-x   0 gabriel    (501) staff       (20)    27247 2023-06-07 15:24:10.000000 SimpliPyTEM-1.0.7/SimpliPyTEM/SimpliPyTEM_GUI.py
+-rw-r--r--   0 gabriel    (501) staff       (20)     7463 2023-06-07 15:23:27.000000 SimpliPyTEM-1.0.7/SimpliPyTEM/html_writer.py
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2023-08-03 10:13:41.228932 SimpliPyTEM-1.0.7/SimpliPyTEM.egg-info/
+-rw-r--r--   0 gabriel    (501) staff       (20)     1661 2023-08-03 10:13:41.000000 SimpliPyTEM-1.0.7/SimpliPyTEM.egg-info/PKG-INFO
+-rw-r--r--   0 gabriel    (501) staff       (20)      517 2023-08-03 10:13:41.000000 SimpliPyTEM-1.0.7/SimpliPyTEM.egg-info/SOURCES.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)        1 2023-08-03 10:13:41.000000 SimpliPyTEM-1.0.7/SimpliPyTEM.egg-info/dependency_links.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)       69 2023-08-03 10:13:41.000000 SimpliPyTEM-1.0.7/SimpliPyTEM.egg-info/entry_points.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)      312 2023-08-03 10:13:41.000000 SimpliPyTEM-1.0.7/SimpliPyTEM.egg-info/requires.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)       12 2023-08-03 10:13:41.000000 SimpliPyTEM-1.0.7/SimpliPyTEM.egg-info/top_level.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)       38 2023-08-03 10:13:41.229951 SimpliPyTEM-1.0.7/setup.cfg
+-rw-r--r--   0 gabriel    (501) staff       (20)     2262 2023-08-03 10:10:57.000000 SimpliPyTEM-1.0.7/setup.py
```

### Comparing `SimpliPyTEM-1.0.6/LICENSE` & `SimpliPyTEM-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.6/PKG-INFO` & `SimpliPyTEM-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpliPyTEM
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python package to simplify the processing and analysis of TEM and in situ TEM images and videos
 Home-page: https://github/gabriel-ing/Micrograph-analysis-scripts
 Author: Gabriel Ing
 Author-email: ucbtgrb@ucl.ac.uk
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `SimpliPyTEM-1.0.6/README.md` & `SimpliPyTEM-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.6/SimpliPyTEM/App_functions.py` & `SimpliPyTEM-1.0.7/SimpliPyTEM/App_functions.py`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.6/SimpliPyTEM/MicroVideo_class.py` & `SimpliPyTEM-1.0.7/SimpliPyTEM/MicroVideo_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import os
 import subprocess as sb
 import time
 from copy import deepcopy
-
+import hyperspy.api as hs
+from cherrypicker import CherryPicker
 import cv2 as cv
 import matplotlib.animation as animation
 import matplotlib.pyplot as plt
 import mrcfile
 import ncempy.io as nci
 import numpy as np
 import pandas as pd
@@ -111,15 +112,25 @@
         SECTION: IMPORT IMAGES
 
             can be imported as dm3, dm4, mrc, **numpy array or tifs ** add the tifs 
             need to add numpy and tif functionality
 
 
         """
+    def copy(self):
+        '''Returns a copy of the object 
+
+        Returns
+        -------
 
+            MicroVideo: MicroVideo
+                Copy of original MicroVideo object'''
+
+        return deepcopy(self)
+        
     def open_dm(self, file, pixelcorrection=True):
         """
         Imports digital micrograph files into the micrograph object, initialising all the default attributes required, including saving the metadata into self.metadata_tags.
         By default, video dm files (dose fractionations) will be summed to create a single image file, there is also an option (video_average) to use the first frame only.
 
         Some DM files have 'hot pixels' which have anomalously high signal due to detector malfunction, these often lead to contrast issues.
         To correct for this any pixel which has a higher value than the mean value + (20 x standard deviation) is set to the mean pixel value, this is on by default but can be turned off using pixel_correction=False
@@ -185,14 +196,54 @@
         self.frames = self.frames.astype("float32")
         # for frame in self.frames:
         #    frame = frame.astype('float32')
         self.shape = self.frames.shape
         print(file + " opened as a MicroVideo object")
 
     #       #return image, x, y, pixel_size, pixel_unit
+    def open_hyperspy(self, filename):
+        '''
+        Opens filetypes with [hyperspy](https://hyperspy.org/) - this is excellent for a range of electron microscope signal types, I recommend checking it out.
+
+        This will allow opening a number of filetypes which will make SimpliPyTEM more accessible for more users, however I cannot verify that this will work with all filetypes and may cause an issue if non-image signals are included. 
+
+        Please report any issues with this on github and I will try to fix them.
+
+        Parameters
+        ----------
+
+            filename: str
+                Name of file to open
+        ''' 
+        s = hs.load(filename)
+
+        if len(s.data.shape)==3:
+            self.frames = s.data
+        elif len(s.data.shape)==2:
+            print('Error - this appears to be an image, thus returning an image')
+            raise Exception
+
+        elif len(s.data.shape)>3: 
+            print('Error - there are more than 3 dimensions, unclear what these are.')
+            raise Exception
+
+            
+        self.filename = filename
+        self.pixel_size = s.axes_manager[-1].scale
+        self.pixel_unit = s.axes_manager[-1].units
+        picker = CherryPicker(s.metadata.as_dictionary())
+
+        self.metadata_tags = picker.flatten(delim='.').get()
+
+        if 'Acquisition_instrument.TEM.Camera.exposure' in self.metadata_tags:
+            self.fps = float(self.metadata_tags['Acquisition_instrument.TEM.Camera.exposure'])/s.data.shape[0]
+        else:
+            self.fps= -1
+        self.reset_xy()
+
 
     def open_mrc(self, file):
         mrc = mrcfile.open(file)
         print(mrc.voxel_size)
         voxel_size = mrc.voxel_size
 
         self.pixel_size = float(str(voxel_size).split(",")[0].strip("("))
@@ -290,15 +341,22 @@
 
     def open_file(self, filename):
         if filename[-4:] == ".dm3" or filename[-4:] == ".dm4":
             self.open_dm(filename)
         elif filename[-4:] == ".mrc":
             self.open_mrc(filename)
         else:
-            self.open_video(filename)
+            try:
+                self.open_hyperspy()
+            except:
+                try:
+                    self.open_video(filename)
+                except:
+                    print("Error - unknown or unsupported filetype, if you think this should be supported please raise an issue on github")
+                    raise Exception
 
     def reset_xy(self):
         """
         Resets the image attributes for the x, y and shape of the image. Used by the binning method and is also useful following cropping of the micrograph
 
         """
         self.x = self.frames[0].shape[1]
@@ -577,17 +635,18 @@
 
         if name[-4:] != ".mrc":
             name += ".mrc"
 
         if outdir:
             make_outdir(outdir)
             name = outdir + "/" + name
-
+        frames_yflipped =  np.flip(self.frames, axis=1)
         with mrcfile.new(name, overwrite=overwrite) as mrc:
-            mrc.set_data(self.frames)
+            mrc.set_data(frames_yflipped)
+        
 
     def toMicrograph(self):
         """
         Returns a micrograph object with the average of the image so the video average can be treated as a single image
 
         Returns
         -------
@@ -969,17 +1028,20 @@
             ]
         except KeyError:
             try:
                 self.indicated_mag = self.metadata_tags[
                     ".ImageList.2.ImageTags.Microscope Info.Formatted Indicated Mag"
                 ]
             except KeyError:
-                print(
-                    "Sorry, indicated mag could not be found, try searching for it manually with the show_metadata method"
-                )
+                try:
+                    self.indicated_mag = self.metadata_tags["Acquisition_instrument.TEM.magnification"]
+                except:
+                    print(
+                        "Sorry, indicated mag cannot be located in tags, please find manually using .show_metadata()"
+                    )
         try:
             self.actual_mag = self.metadata_tags[
                 ".ImageList.2.ImageTags.Microscope Info.Actual Magnification"
             ]
         except KeyError:
             try:
                 actual_mag = self.metadata_tags[
@@ -990,86 +1052,105 @@
                     "Sorry, indicated mag could not be found, try searching for it manually with the show_metadata method"
                 )
 
         if hasattr(self, "actual_mag") and hasattr(self, "indicated_mag"):
             # print('Indicated mag: {}'.format(self.indicated_mag))
             # print('Actual mag: {}'.format(self.actual_mag))
             return self.indicated_mag, self.actual_mag
+        elif hasattr(self, "indicated_mag"):
+            return self.indicated_mag, -1
+        else:
+            return -1, -1
 
     def get_voltage(self):
         """
         Returns voltage and saves is as micrograph attribute
 
         Returns
         -------
 
             Voltage:int
                 Microscope voltage for the image
         """
-        self.voltage = self.metadata_tags[
-            ".ImageList.2.ImageTags.Microscope Info.Voltage"
-        ]
-        return self.voltage
+        try:
+            self.voltage = self.metadata_tags[
+                ".ImageList.2.ImageTags.Microscope Info.Voltage"
+            ]
+            return self.voltage
+        except:
+            try: 
+                self.voltage = self.metadata_tags['Acquisition_instrument.TEM.beam_energy']
+                return self.voltage
+            except KeyError:
+                print("Voltage was not found")
+                return -1
 
     def get_exposure(self, print_values=True):
         """
         Prints and returns the frame rate, exposure time per frame, imaging time and number of frames.
 
         Returns
         -------
 
             fps:int
                 Frame rate of the video in frames per second
 
             Imaging_time:int
                 The total imaging time for the video. s
         """
-        # print('Frame rate : {}fps'.format(self.fps))
-        # print('Exposure time per frame: {}s '.format(1/self.fps))
-        if print_values == True:
-            print("Frame rate : {}fps".format(self.fps))
-            print("Exposure time per frame: {}s ".format(1 / self.fps))
-            print(
-                "Imaging time: {}s".format(
-                    self.metadata_tags[
-                        ".ImageList.2.ImageTags.Acquisition.Parameters.High Level.Exposure (s)"
-                    ]
-                )
-            )
-            print("Number of frames: {}".format(self.frames.shape[0]))
+        try:
+            self.exposure = self.metadata_tags[
+                ".ImageList.2.ImageTags.Acquisition.Parameters.High Level.Exposure (s)"
+            ]
+        except: 
+            try:
+                self.exposure = self.metadata_tags['Acquisition_instrument.TEM.Camera.exposure']
+            except:
+                self.exposure = -1
         return (
             self.fps,
-            self.metadata_tags[
-                ".ImageList.2.ImageTags.Acquisition.Parameters.High Level.Exposure (s)"
-            ],
+            self.exposure
         )
 
     def get_date_time(self):
         """
         Prints and returns the aquisition date and time for the image.
 
         Returns
         -------
 
             AqDate:str
                 Date on which the micrograph was captured
             AqTime:str
                 Time at which the micrograph was captured
         """
-        self.AqDate = self.metadata_tags[
-            ".ImageList.2.ImageTags.DataBar.Acquisition Date"
-        ]
-        self.AqTime = self.metadata_tags[
-            ".ImageList.2.ImageTags.DataBar.Acquisition Time"
-        ]
+        try:
+            self.AqDate = self.metadata_tags[
+                ".ImageList.2.ImageTags.DataBar.Acquisition Date"
+            ]
+            self.AqTime = self.metadata_tags[
+                ".ImageList.2.ImageTags.DataBar.Acquisition Time"
+            ]
         # print('Date: {} '.format(self.AqDate))
         # print('Time {} '.format(self.AqTime))
-        return self.AqDate, self.AqTime
+            return self.AqDate, self.AqTime
+        except:
+            try:
+                self.AqDate = self.metadata_tags[
+                    "General.date"
+                ]
+                self.AqTime = self.metadata_tags[
+                    "General.time"
+                ]            
+                return self.AqDate, self.AqTime 
+            except:
+
+                return "UNK", "UNK"
 
-    def export_metadata(self, name=None, outdir="."):
+    def export_metadata(self, name='metadata.csv', outdir="."):
         """ """
         make_outdir(outdir)
 
         dt = self.get_date_time()
         date_time = pd.to_datetime(dt[0] + " " + dt[1])
 
         metadata = {
@@ -1431,14 +1512,66 @@
             # magnitude_spectrum_filter = np.log(np.abs(f_filtered_shifted))
             inv_image = np.fft.ifft2(f_filtered_shifted)
             filtered_object.frames[i] = np.abs(inv_image)
             filtered_object.frames[i] -= filtered_object.frames[i].min()
         filtered_object.log.append("low_pass_filter({})".format(radius))
         return filtered_object
 
+    def high_pass_filter(self, radius):
+        """
+        This high pass filters the image. This can be effective for evening out uneven contrast in the image. The pixel size is used to scale the radius to whatever the pixel unit is (ie radius 10 is 10nm/10um)
+        If pixelsize is undefined the radius will refer to pixels only
+
+        Parameters
+        ----------
+
+            radius : int (or potentially float)
+                The effects of this vary depending on if the pixelsize is defined in self.pixel_size.:
+                     - Assuming your micrograph object has a pixel size defined, the filter works by removing any features smaller than the size you input as a parameter (the unit is the same as the pixelsize), A larger number yields a stronger filter, if it is too large, you won't see any features.
+                    Effective filter sizes depends on features and magnification, so with something between 1-5 and tune it to your needs.
+                    - If your micrograph is missing a pixelsize the size input will be the radius of a circle kept in the power spectrum. Here the input number does the inverse - a smaller number leads to stronger filter. In this case, much larger numbers will be needed, 50 is a good starting value.
+
+        Returns
+        -------
+                Low_pass_filtered_object :MicroVideo
+                    Low pass filtered copy of the microvideo object.
+
+        """
+        # print(N)
+        N = self.frames[0].shape[0]
+        if (
+            type(self.pixel_size) == int
+            or type(self.pixel_size) == float
+            and self.pixel_size != 0
+        ):
+            radius = int((N * self.pixel_size) / radius)
+
+        filtered_object = deepcopy(self)
+        for i in range(len(filtered_object.frames)):
+            fft = np.fft.fft2(filtered_object.frames[i])
+            fshift = np.fft.fftshift(fft)
+            magnitude_spectrum = np.log(np.abs(fshift))
+            crow, ccol = int(self.y / 2), int(self.x / 2)
+            fshift_filtered = np.copy(fshift)
+            mask = np.zeros_like(self.frames[i])
+
+            mask = cv.circle(cv.UMat(mask), (crow, ccol), radius * 2, 1, -1)
+            # print(fshift_filtered)
+            mask = mask.get()
+            mask =~mask.astype(bool)
+            fcomplex = fshift[:, :] * 1j
+            fshift_filtered = mask * fcomplex
+            f_filtered_shifted = np.fft.fftshift(fshift_filtered)
+            # magnitude_spectrum_filter = np.log(np.abs(f_filtered_shifted))
+            inv_image = np.fft.ifft2(f_filtered_shifted)
+            filtered_object.frames[i] = np.abs(inv_image)
+            filtered_object.frames[i] -= filtered_object.frames[i].min()
+        filtered_object.log.append("high_pass_filter({})".format(radius))
+        return filtered_object
+
     def median_filter(self, kernal=3):
         """
         Returns a median filtered copy of the Microvideo object, kernal size defined in the call (default is 3)
 
             Parameters
             ----------
                 kernal:int
```

### Comparing `SimpliPyTEM-1.0.6/SimpliPyTEM/Micrograph_class.py` & `SimpliPyTEM-1.0.7/SimpliPyTEM/Micrograph_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import itertools
 import os
 import subprocess as sb
 import time
 from copy import deepcopy
-
+import hyperspy.api as hs
+from cherrypicker import CherryPicker
 import cv2 as cv
 import matplotlib.pyplot as plt
 import mrcfile
 import ncempy.io as nci
 import numpy as np
 import pandas as pd
 import tifffile
@@ -122,14 +123,26 @@
             self.filename = ""
             self.image = "Undefined"
             self.pixel_size = "Undefined"
             self.log = []
             self.video = False
             self.nframes = 1
 
+    def copy(self):
+        '''
+        Returns a copy of the object 
+
+        Returns
+        -------
+
+            Micrograph: Micrograph
+                Copy of original Micrograph object
+        '''
+        return deepcopy(self)
+        
     def open_dm(self, file, video_average=True, pixel_correction=True):
         """
         Imports digital micrograph files into the micrograph object, initialising all the default attributes required, including saving the metadata into self.metadata_tags.
         By default, video dm files (dose fractionations) will be summed to create a single image file, there is also an option (video_average) to use the first frame only.
 
         Some DM files have 'hot pixels' which have anomalously high signal due to detector malfunction, these often lead to contrast issues.
         To correct for this any pixel which has a higher value than the mean value + (20 x standard deviation) is set to the mean pixel value, this is on by default but can be turned off using pixel_correction=False
@@ -204,15 +217,18 @@
                 The name of an MRC file to open, the path to the file can also be included.
         """
 
         mrc = mrcfile.open(file)
         print(mrc.voxel_size)
         voxel_size = mrc.voxel_size
         self.pixel_size = float(str(voxel_size).split(",")[0].strip("("))
-        self.image = mrc.data
+        if len(mrc.data==3):
+            self.image = np.sum(mrc.data, axis=0)
+        else:
+            self.image = mrc.data
         self.image.setflags(write=1)
         self.x = self.image.shape[1]
         self.y = self.image.shape[0]
         self.image = np.flip(self.image, axis=0)
         self.pixel_unit = "nm"
         self.filename = file
         if pixel_correction:
@@ -221,14 +237,48 @@
             ] = self.image.mean()
         # this line converts the image to a float32 datatype, this will make it run slower if it starts out as a 8 or 16 bit, I maybe should account for this, but its also required for median filter and others, so I'm performing as default.
         self.image = self.image.astype("float32")
         self.shape = self.image.shape
         self.original_image = self.image
 
     ##write a hyperspy opening function
+    def open_hyperspy(self, filename):
+        '''
+        Opens filetypes with [hyperspy](https://hyperspy.org/) - this is excellent for a range of electron microscope signal types, I recommend checking it out.
+
+        This will allow opening a number of filetypes which will make SimpliPyTEM more accessible for more users, however I cannot verify that this will work with all filetypes and may cause an issue if non-image signals are included. 
+
+        Please report any issues with this on github and I will try to fix them.
+
+        Parameters
+        ----------
+
+            filename: str
+                Name of file to open
+        ''' 
+        s = hs.load(filename)
+        if len(s.data.shape)==3:
+            self.image = np.sum(s.data, axis=0)
+            self.video= True
+        elif len(s.data.shape)==2:
+            self.image = s.data
+        elif len(s.data.shape)==1:
+            print('Error - there is only one dimension, this is not image data')
+            raise Exception
+        else: 
+            print('Error - there are more than 3 dimensions, unclear what these are.')
+            raise Exception
+            
+        self.filename = filename
+        self.pixel_size = s.axes_manager[-1].scale
+        self.pixel_unit = s.axes_manager[-1].units
+        picker = CherryPicker(s.metadata.as_dictionary())
+
+        self.metadata_tags = picker.flatten(delim='.').get()
+        self.reset_xy()
 
     def open_image(self, filename, pixel_size=None, pixel_unit=None):
         """
         Open a jpg, png or tif file into the micrograph object. If the tif has any metadata tags, these should be saved into the metadata_tags and will then be accessible with .show_metadata()
         The pixel size is likely to be included somewhere within the metadata and may be loaded, but the name of the tags are not always constant, and so this may need to be searched in  the .show_metadata output.
 
         Parameters
@@ -317,20 +367,25 @@
             self.pixel_unit = pixel_unit
 
         self.original_image = self.image
 
     def open_file(self, filename):
         if filename[-4:] == ".dm3" or filename[-4:] == ".dm4":
             self.open_dm(filename)
-        elif filename[-4:] == ".mrc":
-            self.open_mrc(filename)
+        #elif filename[-4:] == ".mrc":
+        #    self.open_mrc(filename)
         elif filename[-4:].lower() in [".jpg", ".png", ".tif", "tiff"]:
             self.open_image(filename)
         elif filename[-4:].lower() in [".mp4", ".avi", ".mov"]:
             self.open_video(filename)
+        else:
+            try:
+                self.open_hyperspy(filename)
+            except:
+                print('Error, unknown or unsupported file type - if you think this should be available, please contact developers by raising issue on github')
 
     def open_video(
         self,
         filename,
         pixel_size=1,
         pixel_unit="pixels",
     ):
@@ -1108,14 +1163,64 @@
         filtered_image -= filtered_image.min()
         filtered_object = deepcopy(self)
         filtered_object.image = filtered_image
 
         filtered_object.log.append("low_pass_filter({})".format(radius))
         return filtered_object
 
+    def high_pass_filter(self, radius):
+        """
+        This high pass filters the image. High pass filtering can be useful for evening out the contrast in the image. The pixel size is used to scale the radius to whatever the pixel unit is (ie radius 10 is 10nm/10um)
+        If pixelsize is undefined the radius will refer to pixels only
+    
+        Parameters
+        ----------
+            radius : int (or potentially float)
+                The effects of this vary depending on if the pixelsize is defined in self.pixel_size.:
+                     - Assuming your micrograph object has a pixel size defined, the filter works by removing any features larger than the size you input as a parameter (the unit is the same as the pixelsize). A larger number yields a stronger filter.
+                    Effective filter sizes depend on features and magnification, so start with something between 1-5 and tune it to your needs.
+                    - If your micrograph is missing a pixelsize, the size input will be the radius of a circle kept in the power spectrum. Here the input number does the inverse - a smaller number leads to a stronger filter. In this case, much larger numbers will be needed; 50 is a good starting value.
+    
+        Returns
+        -------
+                High_pass_filtered_object : Micrograph
+                    High pass filtered copy of micrograph object.
+    
+        """
+        N = self.image.shape[0]
+        if (
+            type(self.pixel_size) == int
+            or type(self.pixel_size) == float
+            and self.pixel_size != 0
+        ):
+            radius = int((N * self.pixel_size) / radius)
+    
+        fft = np.fft.fft2(self.image)
+        fshift = np.fft.fftshift(fft)
+        magnitude_spectrum = np.log(np.abs(fshift))
+        rows, cols = self.image.shape
+        crow, ccol = int(cols / 2), int(rows / 2)
+        fshift_filtered = np.copy(fshift)
+        mask = np.zeros_like(self.image)
+    
+        mask = cv.circle(cv.UMat(mask), (crow, ccol), radius * 2, 1, -1)
+        mask = mask.get()
+        mask = ~mask.astype(bool)
+        fcomplex = fshift[:, :] * 1j
+        fshift_filtered = mask * fcomplex
+        f_filtered_shifted = np.fft.fftshift(fshift_filtered)
+        inv_image = np.fft.ifft2(f_filtered_shifted)
+        filtered_image = np.abs(inv_image)
+        filtered_image -= filtered_image.min()
+        filtered_object = deepcopy(self)
+        filtered_object.image = filtered_image
+    
+        filtered_object.log.append("high_pass_filter({})".format(radius))
+        return filtered_object
+
     def median_filter(self, kernal=3):
         """
         Returns a median filtered copy of the micrograph object, kernal size defined in the call (default is 3)
 
             Parameters
             ----------
                 kernal:int
@@ -1494,17 +1599,20 @@
         except KeyError:
             try:
                 self.indicated_mag = self.metadata_tags[
                     ".ImageList.2.ImageTags.Microscope Info.Formatted Indicated Mag"
                 ]
 
             except KeyError:
-                print(
-                    "Sorry, indicated mag cannot be located in tags, please find manually using .show_metadata()"
-                )
+                try:
+                    self.indicated_mag = self.metadata_tags["Acquisition_instrument.TEM.magnification"]
+                except:
+                    print(
+                        "Sorry, indicated mag cannot be located in tags, please find manually using .show_metadata()"
+                    )
 
         try:
             self.actual_mag = self.metadata_tags[
                 ".ImageList.2.ImageTags.Microscope Info.Actual Magnification"
             ]
         except KeyError:
             try:
@@ -1517,14 +1625,17 @@
                 )
 
         # self.indicated_mag = self.metadata_tags['.ImageList.2.ImageTags.Microscope Info.Indicated Magnification']
         if hasattr(self, "indicated_mag") and hasattr(self, "actual_mag"):
             # print('Indicated mag: {}'.format(self.indicated_mag))
             # print('Actual mag: {}'.format(self.actual_mag))
             return self.indicated_mag, self.actual_mag
+        elif hasattr(self, "indicated_mag"):
+            return self.indicated_mag, -1
+
         else:
             return -1, -1
 
     def get_voltage(self):
         """
         Returns voltage and saves is as micrograph attribute
 
@@ -1557,17 +1668,22 @@
         # print('Exposure time per frame: {}s '.format(1/self.fps))
         # print('Imaging time: {}s'.format(self.metadata_tags['.ImageList.2.ImageTags.Acquisition.Parameters.High Level.Exposure (s)']))
         try:
             self.exposure = self.metadata_tags[
                 ".ImageList.2.ImageTags.Acquisition.Parameters.High Level.Exposure (s)"
             ]
             return self.exposure
-        except KeyError:
-            return -1
 
+        except KeyError:
+            try:
+                self.exposure = self.metadata_tags['Acquisition_instrument.TEM.Camera.exposure']
+                return self.exposure
+            except:
+                print('Sorry, exposure cannot be located')
+                return -1
     def get_date_time(self):
         """
         Prints and returns the aquisition date and time for the image.
 
         Returns
         -------
 
@@ -1581,15 +1697,25 @@
                 ".ImageList.2.ImageTags.DataBar.Acquisition Date"
             ]
             self.AqTime = self.metadata_tags[
                 ".ImageList.2.ImageTags.DataBar.Acquisition Time"
             ]
             return self.AqDate, self.AqTime
         except:
-            return "UNK", "UNK"
+            try:
+                self.AqDate = self.metadata_tags[
+                    "General.date"
+                ]
+                self.AqTime = self.metadata_tags[
+                    "General.time"
+                ]            
+                return self.AqDate, self.AqTime 
+            except:
+
+                return "UNK", "UNK"
         # print('Date: {} '.format(self.AqDate))
         # print('Time {} '.format(self.AqTime))
 
     def export_metadata(self, name=None, outdir="."):
         make_outdir(outdir)
 
         if not name:
```

### Comparing `SimpliPyTEM-1.0.6/SimpliPyTEM/Motion_correction.py` & `SimpliPyTEM-1.0.7/SimpliPyTEM/Motion_correction.py`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.6/SimpliPyTEM/PDF_generator.py` & `SimpliPyTEM-1.0.7/SimpliPyTEM/PDF_generator.py`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.6/SimpliPyTEM/Particle_analysis.py` & `SimpliPyTEM-1.0.7/SimpliPyTEM/Particle_analysis.py`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.6/SimpliPyTEM/Particle_tracking.py` & `SimpliPyTEM-1.0.7/SimpliPyTEM/Particle_tracking.py`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.6/SimpliPyTEM/SimpliPyTEM_GUI.py` & `SimpliPyTEM-1.0.7/SimpliPyTEM/SimpliPyTEM_GUI.py`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.6/SimpliPyTEM/html_writer.py` & `SimpliPyTEM-1.0.7/SimpliPyTEM/html_writer.py`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/PKG-INFO` & `SimpliPyTEM-1.0.7/SimpliPyTEM.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpliPyTEM
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python package to simplify the processing and analysis of TEM and in situ TEM images and videos
 Home-page: https://github/gabriel-ing/Micrograph-analysis-scripts
 Author: Gabriel Ing
 Author-email: ucbtgrb@ucl.ac.uk
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `SimpliPyTEM-1.0.6/SimpliPyTEM.egg-info/SOURCES.txt` & `SimpliPyTEM-1.0.7/SimpliPyTEM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SimpliPyTEM-1.0.6/setup.py` & `SimpliPyTEM-1.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup 
 
 setup(
 	name='SimpliPyTEM',
-	version='1.0.6',
+	version='1.0.7',
 	description='A python package to simplify the processing and analysis of TEM and in situ TEM images and videos',
 	long_description='''SimpliPyTEM is a python package to make python-based analysis of Transmission electron microscopy images easier and more approachable. Although TEM is the focus, this could also easily be adapted to other microscopy images. Importantly, SimpliPyTEM is designed to make automated, basic work accessible for beginners (through a simple GUI), while more complicated methods can be accessed through simple python code. This package centers around the image data being held in a Numpy array which makes the image data easy to access for further analysis.
 	This project aims to make use of the rapid automation of image analysis methods available through python while making it approachable for the user.
 	Functions to generate pdf and html files containing images and videos are also included in this package. This allows easy viewing and sharing of all the images/videos taken in an imaging session, making experiment evaluation significantly easier. 
 	For more info, please see: https://micrograph-analysis-scripts.readthedocs.io/en/latest/''',
 	url='https://github/gabriel-ing/Micrograph-analysis-scripts',
 	author='Gabriel Ing',
@@ -27,15 +27,17 @@
 	 'imutils==0.5.4',
 	 'fpdf==1.7.2',
 	 'PyQt6==6.5.0',
 	 'sphinx',
 	 'sphinx_rtd_theme',
 	 'nbsphinx',
 	 'pandas==1.5.3',
-	 'seaborn==0.12.2'],
+	 'seaborn==0.12.2',
+	 'hyperspy==1.7.5',
+	 'cherrypicker==0.4.0'],
 	entry_points={'console_scripts':['SimpliPyTEM-GUI = SimpliPyTEM.SimpliPyTEM_GUI:main']},
 	classifiers=[
 		'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',  
         'Operating System :: POSIX :: Linux',     
         'Programming Language :: Python :: 3',
```

