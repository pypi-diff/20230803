# Comparing `tmp/FRion-1.0.tar.gz` & `tmp/FRion-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FRion-1.0.tar", last modified: Thu Feb 24 18:48:13 2022, max compression
+gzip compressed data, was "dist/FRion-1.1.0.tar", last modified: Thu Aug  3 09:05:04 2023, max compression
```

## Comparing `FRion-1.0.tar` & `FRion-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 cvaneck    (501) staff       (20)        0 2022-02-24 18:48:13.816279 FRion-1.0/
-drwxr-xr-x   0 cvaneck    (501) staff       (20)        0 2022-02-24 18:48:13.810760 FRion-1.0/FRion/
--rw-r--r--   0 cvaneck    (501) staff       (20)    14494 2022-02-24 17:00:37.000000 FRion-1.0/FRion/correct.py
--rw-r--r--   0 cvaneck    (501) staff       (20)    30526 2022-02-24 18:30:34.000000 FRion-1.0/FRion/predict.py
-drwxr-xr-x   0 cvaneck    (501) staff       (20)        0 2022-02-24 18:48:13.814828 FRion-1.0/FRion.egg-info/
--rw-r--r--   0 cvaneck    (501) staff       (20)     1601 2022-02-24 18:48:13.000000 FRion-1.0/FRion.egg-info/PKG-INFO
--rw-r--r--   0 cvaneck    (501) staff       (20)      228 2022-02-24 18:48:13.000000 FRion-1.0/FRion.egg-info/SOURCES.txt
--rw-r--r--   0 cvaneck    (501) staff       (20)        1 2022-02-24 18:48:13.000000 FRion-1.0/FRion.egg-info/dependency_links.txt
--rw-r--r--   0 cvaneck    (501) staff       (20)      144 2022-02-24 18:48:13.000000 FRion-1.0/FRion.egg-info/entry_points.txt
--rw-r--r--   0 cvaneck    (501) staff       (20)       22 2022-02-24 18:48:13.000000 FRion-1.0/FRion.egg-info/requires.txt
--rw-r--r--   0 cvaneck    (501) staff       (20)        6 2022-02-24 18:48:13.000000 FRion-1.0/FRion.egg-info/top_level.txt
--rw-r--r--   0 cvaneck    (501) staff       (20)     1601 2022-02-24 18:48:13.815703 FRion-1.0/PKG-INFO
--rw-r--r--   0 cvaneck    (501) staff       (20)      671 2022-02-24 18:38:57.000000 FRion-1.0/README.md
--rw-r--r--   0 cvaneck    (501) staff       (20)       38 2022-02-24 18:48:13.816478 FRion-1.0/setup.cfg
--rw-r--r--   0 cvaneck    (501) staff       (20)     1822 2022-02-24 18:38:06.000000 FRion-1.0/setup.py
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-08-03 09:05:04.311554 FRion-1.1.0/
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-08-03 09:05:04.307765 FRion-1.1.0/FRion/
+-rw-r--r--   0 cvaneck    (503) staff       (20)    14115 2023-08-02 06:18:33.000000 FRion-1.1.0/FRion/correct.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)     4541 2023-08-02 03:37:32.000000 FRion-1.1.0/FRion/download_IONEX_CDDIS.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)    32624 2023-08-03 06:24:05.000000 FRion-1.1.0/FRion/predict.py
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-08-03 09:05:04.310763 FRion-1.1.0/FRion.egg-info/
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1908 2023-08-03 09:05:03.000000 FRion-1.1.0/FRion.egg-info/PKG-INFO
+-rw-r--r--   0 cvaneck    (503) staff       (20)      266 2023-08-03 09:05:04.000000 FRion-1.1.0/FRion.egg-info/SOURCES.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)        1 2023-08-03 09:05:03.000000 FRion-1.1.0/FRion.egg-info/dependency_links.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)      143 2023-08-03 09:05:03.000000 FRion-1.1.0/FRion.egg-info/entry_points.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)       31 2023-08-03 09:05:03.000000 FRion-1.1.0/FRion.egg-info/requires.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)        6 2023-08-03 09:05:03.000000 FRion-1.1.0/FRion.egg-info/top_level.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1072 2021-04-14 19:26:44.000000 FRion-1.1.0/LICENSE
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1908 2023-08-03 09:05:04.311218 FRion-1.1.0/PKG-INFO
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1091 2023-08-03 07:10:22.000000 FRion-1.1.0/README.md
+-rw-r--r--   0 cvaneck    (503) staff       (20)       38 2023-08-03 09:05:04.311612 FRion-1.1.0/setup.cfg
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1833 2023-08-02 06:36:22.000000 FRion-1.1.0/setup.py
```

### Comparing `FRion-1.0/FRion/correct.py` & `FRion-1.1.0/FRion/correct.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,14 +200,15 @@
     loader = '  [' + ('=' * int(marks)) + (' ' * int(spaces)) + ']'
     sys.stdout.write("%s %d%%\r" % (loader, percent))
     if percent >= 100:
         sys.stdout.write("\n")
     sys.stdout.flush()
 
 
+
 def apply_correction_large_cube(Qfile,Ufile,predictionfile,Qoutfile,Uoutfile,
                               overwrite=False):
     """Functions as apply_correction_to_files, but for files too large to
     hold in memory. Combines the correct_cubes() and write_corrected_cubes()
     steps into a single function so that it can operate on smaller pieces
     of data at one time.
     
@@ -280,45 +281,42 @@
         fobj.seek(len(output_header.tostring()) + (np.product(shape) * np.abs(output_header['BITPIX']//8)) - 1)
         fobj.write(b'\0')
 
 
     Qout_hdu=pf.open(Qoutfile,mode='update',memmap=True)
     Uout_hdu=pf.open(Uoutfile,mode='update',memmap=True)
 
-    Npix=output_header['NAXIS1']*output_header['NAXIS2']
 
-    for i in range(Npix):
-        x=i % output_header['NAXIS1'] 
-        y=i // output_header['NAXIS1']
-        if N_dim==4:
-            Pdata=Qdata[:,:,y,x]+1.j*Udata[:,:,y,x] #Input complex polarization
-        elif N_dim==3:
-            Pdata=Qdata[:,y,x]+1.j*Udata[:,y,x] #Input complex polarization
-        arrshape=np.array(Pdata.shape)  #the correction needs the same number of
-        arrshape[:]=1                   #axes as the input data
-        arrshape[N_dim-freq_axis]=theta.size     #(but they can all be degenerate)
-        Pcorr=np.true_divide(Pdata,np.reshape(theta,arrshape))
-        if N_dim==4:
-            Qout_hdu[0].data[:,:,y,x]=Pcorr.real
-            Uout_hdu[0].data[:,:,y,x]=Pcorr.imag
-        elif N_dim==3:
-            Qout_hdu[0].data[:,y,x]=Pcorr.real
-            Uout_hdu[0].data[:,y,x]=Pcorr.imag
-        if x == 0:
-            progress(40, i/Npix*100)
+
+    for i in range(theta.size): #Iterate over channels.
+        if N_dim==4 & freq_axis == 3:
+            Pdata=Qdata[:,i]+1.j*Udata[:,i] #Input complex polarization
+        else:
+            Pdata=Qdata[i]+1.j*Udata[i] #Input complex polarization
+
+        Pcorr=np.true_divide(Pdata,theta[i])
+        if N_dim==4 & freq_axis == 3:
+            Qout_hdu[0].data[:,i]=Pcorr.real
+            Uout_hdu[0].data[:,i]=Pcorr.imag
+        else:
+            Qout_hdu[0].data[i]=Pcorr.real
+            Uout_hdu[0].data[i]=Pcorr.imag
+
+        progress(40, i/theta.size*100)
 
     Qout_hdu.flush()
     Uout_hdu.flush()
     Qout_hdu.close()
     Uout_hdu.close()
 
 
 
 
 
+
 def command_line():
     """When invoked from the command line, parse the input options to get the
     filenames and other parameters, then invoke apply_correction_to_files
     to run all the steps and save the output cubes.
     
     """
```

### Comparing `FRion-1.0/FRion/predict.py` & `FRion-1.1.0/FRion/predict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,73 +1,83 @@
 #!/usr/bin/env python3
 
 """
-Functions for predicting ionospheric Faraday rotation effects, both 
+Functions for predicting ionospheric Faraday rotation effects, both
 time-dependent and time-averaged.
-Uses RMextract package to get time-dependent ionospheric RMs for a given 
+Uses RMextract package to get time-dependent ionospheric RMs for a given
 observation, then performs the time-integration to work out the effective
-change in polarization angle, and the effective depolarization (together, 
-called the ionospheric *modulation*, which is called Theta in the derivation).
+change in polarization angle, and the effective depolarization (together,
+called the ionospheric *modulation*\ , which is called Theta in the derivation).
+
+The ionospheric prediction is currently derived from RMExtract (https://github.com/lofar-astron/RMextract/).
+Other ionosphere RM codes are available (ionFR, ALBUS) are available, but
+RMextract was selected for its comparative ease of install and use.
+
+RMextract relies on external maps of Total Electron Content (TEC). As of 
+version 1.1, the default is to get the TEC data from CDDIS
+(https://cddis.nasa.gov/Data_and_Derived_Products/GNSS/atmospheric_products.html).
+This requires an account and a .netrc file with the credentials
+(https://cddis.nasa.gov/Data_and_Derived_Products/CreateNetrcFile.html).
+Advanced users can change the TEC source using the kwargs for RMextract's
+getRM function, with the caveat that this is not supported for the command line
+tools.
+The default TEC maps are now the JPL global maps, based on the results of
+Porayko et al. 2019 who found they performed the best.
 
-The ionospheric prediction is currently derived from RMExtract
-(https://github.com/lofar-astron/RMextract/). 
-Other ionosphere RM codes are available (ionFR, ALBUS) are available, but 
-RMextract was selected for its ease of install and use.
-
-RMextract relies on external maps of Total Electron Content (TEC). Currently
-the CODG TEC maps are used (this is default for RMextract), but other data
-sources are available. Changing TEC sources would require changing the 
-RMExtract call in get_RM(). If anyone knows how to invoke RMExtract with
-alternative TEC sources, please consider contacting me or submitting a pull
-request to add that functionality.
 
 Two command line functions are available and documented below:
     - predict(): time-averaged Faraday rotation.
     - timeseries(): time-dependent Faraday rotation.
-    
+
 
 """
 
 
 try:
     import RMextract.getRM as RME
+    from RMextract import getIONEX as ionex
 except:
     #This is the easiest solution to the documentation problem:
-    #This code needs to be importable when RMextract isn't installed, for 
+    #This code needs to be importable when RMextract isn't installed, for
     #ReadTheDocs to work. Getting RMextract to install properly in RTD is too
     #much work, so this is my workaround.
     print('Cannot import RMextract. Continuing import, but will fail if called.')
 from astropy.time import Time,TimeDelta
 import numpy as np
 from astropy.coordinates import EarthLocation,SkyCoord,Angle, UnknownSiteException
 import astropy.units as u
 from FRion.correct import find_freq_axis
 import astropy
+from FRion.download_IONEX_CDDIS import get_CDDIS_IONEXfile
 
 C = 2.99792458e8 # Speed of light [m/s]
 
 
 def predict():
-    """Wrapper for command line interface, for time-averaging mode. 
-    Gets command line arguments, calculates ionospheric effects, and saves 
+    """Wrapper for command line interface, for time-averaging mode.
+    Gets command line arguments, calculates ionospheric effects, and saves
     modulation and/or figure if specified.
-    
+
     If the package is installed, it can be called as frion_predict,
     otherwise as python predict.py
-    
+
     Call with the -h flag to see command line options.
     """
     import argparse
     descStr = """
     Calculate ionospheric Faraday rotation and predict time-integrated effect
     as a function of frequency.
-    Can determine the frequency, location, direction, and observation time 
+    Can determine the frequency, location, direction, and observation time
     parameters from a supplied FITS cube or PSRFITS file, if it has the correct
-    keywords, otherwise from those parameters must be supplied on the command 
+    keywords, otherwise from those parameters must be supplied on the command
     line.
+    
+    By default, gets ionosphere TEC data from CDDIS (https://cddis.nasa.gov/Data_and_Derived_Products/GNSS/atmospheric_products.html)
+    This requires an account and a .netrc file with the credentials to run.
+    (https://cddis.nasa.gov/Data_and_Derived_Products/CreateNetrcFile.html)
     """
 
     parser = argparse.ArgumentParser(description=descStr,
                                  formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument("-F",dest="fits",default=None,metavar='FILENAME',
                         help="FITS cube relevant information in header.")
     parser.add_argument("-d", dest="times", nargs=2,type=str,default=None,
@@ -96,411 +106,463 @@
 
     start_time=None
     end_time=None
     freq_arr=None
     telescope=None
     ra=None
     dec=None
-    
+
 
     #If a FITS file is present, try to fill in any missing keywords.
     #But since FITS headers can be very different, it may be that not all
     #keywords can be found.
     if args.fits is not None:
         start_time,end_time,freq_arr,telescope,ra,dec=get_parms_from_FITS(args.fits)
-            
+
     #Any parametrs taken from FITS header can be overridden by manual inputs:
     if args.times is not None:
         start_time=Time(args.times[0])
         end_time=Time(args.times[1])
-        
+
     if args.freq_parms is not None:
         freq_arr=np.arange(args.freq_parms[0],args.freq_parms[1],args.freq_parms[2])
 
     if args.telescope_name is not None:
         telescope = get_telescope_coordinates(args.telescope_name)
     if args.telescope_coords is not None:
         telescope = get_telescope_coordinates(args.telescope_coords)
-    
+
     if args.pointing is not None:
         ra=args.pointing[0]
         dec=args.pointing[1]
-    
+
     #Check that all parameters are set:
     missing_parms=[]
     if (start_time is None): missing_parms.append('Start time')
     if (end_time is None): missing_parms.append('End time')
     if (freq_arr is None): missing_parms.append('Frequency array')
     if (telescope is None): missing_parms.append('Telescope')
     if (ra is None): missing_parms.append('Pointing center')
 
     if len(missing_parms) > 0:
         print("\n\nMissing parameters:",missing_parms,'\n')
         raise Exception("Cannot continue without parameters listed above.")
-    
+
     times,RMs,theta=calculate_modulation(start_time, end_time, freq_arr, telescope,
                          ra,dec, timestep=args.timestep,ionexPath='./IONEXdata/')
-    
+
     if args.savefile is not None:
         write_modulation(freq_arr,theta,args.savefile)
 
     if args.savefig is not None:
         generate_plots(times,RMs,theta,freq_arr,position=[ra,dec],savename=args.savefig)
 
 
 def calculate_modulation(start_time, end_time, freq_array, telescope_location,
-                         ra,dec, timestep=600.,ionexPath='./IONEXdata/'):
-    """Calculate the ionospheric FR modulation (time-averaged effect), 
+                         ra,dec, timestep=600.,ionexPath='./IONEXdata/', **kwargs):
+    """Calculate the ionospheric FR modulation (time-averaged effect),
     as a function of frequency, for a given observation (time, location, target direction).
-    
-    
-    
+
+
+
     Args:
-        start_time (astropy.time Time, or string readable by astropy.time Time): 
+        start_time (astropy.time Time, or string readable by astropy.time Time):
             Starting time of observation.
             Example time string: '2010-01-02T00:00:00'
-        end_time (astropy.time.Time, or string readable by astropy.time.Time): 
+        end_time (astropy.time.Time, or string readable by astropy.time.Time):
             ending time of observation.
-        freq_array (array-like, either floats or Astropy Quantity): 
+        freq_array (array-like, either floats or Astropy Quantity):
             vector of channel frequencies (in Hz)
         telescope_location (astropy.coordinates EarthLocation or string):
-            location of telescope, or name of telescope known to 
+            location of telescope, or name of telescope known to
             get_telescope_coordinates() function.
-        ra (astropy.coordinates Angle, astropy.units Quantity, or float): 
+        ra (astropy.coordinates Angle, astropy.units Quantity, or float):
             right ascension of observation center (if float: in deg, J2000)
-        dec (astropy.coordinates Angle, astropy.units Quantity, or float): 
+        dec (astropy.coordinates Angle, astropy.units Quantity, or float):
             declination of observation center (if float: in deg, J2000)
         timestep (astropy.time TimeDelta, astropy.units Quantity, or float):
             time between ionosphere FR estimates. If float, time must be in seconds.
         ionexPath (str, default='./IONEXdata/'): path to download IONEX files to
             for ionosphere calculations.
+        **kwargs: additional keyword arguments to pass to RMextract.getRM()
         
     Returns:
         tuple containing
-        
-        -times (astropy Time array): vector of times of each ionospheric RM calculation   
-        
-        -RMs (array): vector of RM values computed for each time step  
-        
+
+        -times (astropy Time array): vector of times of each ionospheric RM calculation
+
+        -RMs (array): vector of RM values computed for each time step
+
         -theta (array) vector containing the (complex) ionospheric polarization
-        for each frequency channel.  
-    
+        for each frequency channel.
+
     """
-    
+
     #Convert frequencies to have units if needed.
     if type(freq_array) == astropy.units.quantity.Quantity:
         frequencies=freq_array
-    else: 
+    else:
         frequencies=freq_array*u.Hz
 
     #Calculation of the time-dependent RMs.
     times,RMs=get_RM(start_time, end_time, telescope_location,
-                         ra,dec, timestep=600.,ionexPath='./IONEXdata/')
+                         ra,dec, timestep=timestep,ionexPath=ionexPath, **kwargs)
 
-    
-    #Compute the time-integrated change in polarization. 
+
+    #Compute the time-integrated change in polarization.
     theta=numeric_integration(times.mjd*86400.,RMs,frequencies.to(u.Hz).value)
-    
+
     #Verify that we are not in a regime where numerical instabilities might occur.
     check_numeric_problems(RMs, frequencies.to(u.Hz).value,theta)
-    
-    
+
+
     return times,RMs, theta
-    
+
 
 def get_RM(start_time, end_time, telescope_location,
-                         ra,dec, timestep=600.,ionexPath='./IONEXdata/'):
+                         ra,dec, timestep=600.,ionexPath='./IONEXdata/',
+                         pre_download=True,**kwargs):
     """
-    Calculate the ionospheric Faraday rotation as a function of time, 
+    Calculate the ionospheric Faraday rotation as a function of time,
     for a given observation (time, location, target direction).
-    
+
     Args:
-        start_time (astropy.time Time, or string readable by astropy.time Time): 
+        start_time (astropy.time Time, or string readable by astropy.time Time):
             Starting time of observation.
             Example time string: '2010-01-02T00:00:00'
-        end_time (astropy.time.Time, or string readable by astropy.time.Time): 
+        end_time (astropy.time.Time, or string readable by astropy.time.Time):
             ending time of observation.
         telescope_location (astropy.coordinates EarthLocation or string):
-            location of telescope, or name of telescope known to 
+            location of telescope, or name of telescope known to
             get_telescope_coordinates() function.
-        ra (astropy.coordinates Angle, astropy.units Quantity, or float): 
+        ra (astropy.coordinates Angle, astropy.units Quantity, or float):
             right ascension of observation center (if float: in deg, J2000)
-        dec (astropy.coordinates Angle, astropy.units Quantity, or float): 
+        dec (astropy.coordinates Angle, astropy.units Quantity, or float):
             declination of observation center (if float: in deg, J2000)
         timestep (astropy.time TimeDelta, astropy.units Quantity, or float):
             time between ionosphere FR estimates. If float, time must be in seconds.
         ionexPath (str, default='./IONEXdata/'): path to download IONEX files to
             for ionosphere calculations.
+        **kwargs: additional keyword arguments to pass to RMextract.getRM()
         
     Returns:
         tuple containing
-        
-        -times (astropy Time array): vector of times of each ionospheric RM calculation   
-        
-        -RMs (array): vector of RM values computed for each time step  
-    
+
+        -times (astropy Time array): vector of times of each ionospheric RM calculation
+
+        -RMs (array): vector of RM values computed for each time step
+
     """
-    #If necessary, convert telescope name into telescope location object:    
+    #If necessary, convert telescope name into telescope location object:
     if type(telescope_location) != EarthLocation:
         telescope_location=get_telescope_coordinates(telescope_location)
 
     #RMextract wants time ranges in MJD seconds:
     timerange=[Time(start_time).mjd*86400.0,
-               Time(end_time).mjd*86400.0] 
+               Time(end_time).mjd*86400.0]
 
     #Extract telescope coordinates into expected format (geodetic x,y,z):
     telescope_coordinates=[telescope_location.x.value,
                            telescope_location.y.value,
                            telescope_location.z.value]
-    
+
     #Handle all forms of angle input:
     if type(ra) == float or type(ra) == int:
         ra_angle=Angle(ra,'deg')
-    elif type(ra) == astropy.units.quantity.Quantity: 
+    elif type(ra) == astropy.units.quantity.Quantity:
         ra_angle=Angle(ra)
     elif type(ra) == astropy.coordinates.angles.Angle:
         ra_angle=ra
     else:
         raise Exception("""RA input object type not recognized.
                         Only astropy.coordinates Angle, astropy.units Quantity, or float (in deg) allowed.""")
 
     if type(dec) == float or type(dec) == int:
         dec_angle=Angle(dec,'deg')
-    elif type(dec) == astropy.units.quantity.Quantity: 
+    elif type(dec) == astropy.units.quantity.Quantity:
         dec_angle=Angle(dec)
     elif type(dec) == astropy.coordinates.angles.Angle:
-        dec_angle=dec        
+        dec_angle=dec
     else:
         raise Exception("""Dec input object type not recognized.
                         Only astropy.coordinates Angle, astropy.units Quantity, or float (in deg) allowed.""")
 
     #Handle all forms of time input:
     if type(timestep) == float or type(timestep) == int:
         timestep_Delta=TimeDelta(timestep*u.second)
     elif type(timestep) == astropy.units.quantity.Quantity:
         timestep_Delta=TimeDelta(timestep)
     elif type(timestep) == astropy.time.core.TimeDelta:
         timestep_Delta=timestep
     else:
         raise Exception("""Timestep input object type not recognized.
                         Only astropy.time TimeDelta, astropy.units Quantity, or float (in seconds) allowed.""")
-        
-    
+
+
+    #Pre-download the IONEX data from CDDIS, to work around the RMextract lack
+    #of support for CDDIS downloads.
+    if 'prefix' in kwargs:
+        prefix = kwargs['prefix']
+    else:
+        prefix = 'jplg'
+
+    if 'pre_download' in kwargs:
+        pre_download = kwargs['pre_download']        
     
-    #Get RMExtract to generate it's RM predictions
-    predictions=RME.getRM(ionexPath=ionexPath, 
-                          radec=[ra_angle.rad,dec_angle.rad], 
-                          timestep=timestep_Delta.sec, 
-                          timerange = timerange, 
-                          stat_positions=[telescope_coordinates,])
+    if pre_download == True:
+        _predownload_CDDIS(start_time, end_time,prefix,outpath=ionexPath)
+
+
+    ionexf=ionex.get_urllib_IONEXfile(time=start_time.value,prefix=prefix,outpath=ionexPath,overwrite = False)
+
+    assert (ionexf!=-1),"RMextract fails to recognize IONEX file."
+
+    #Get RMExtract to generate its RM predictions
+    predictions=RME.getRM(ionexPath=ionexPath,
+                          radec=[ra_angle.rad,dec_angle.rad],
+                          timestep=timestep_Delta.sec,
+                          timerange = timerange,
+                          stat_positions=[telescope_coordinates,],
+                          prefix=prefix,
+                          server='http://cddis.gsfc.nasa.gov',
+                          **kwargs)
     #predictions dictionary contains STEC, Bpar, BField, AirMass, elev, azimuth
     #  RM, times, timestep, station_names, stat_pos, flags, reference_time
     times=Time(predictions['times']/86400.,format='mjd')
     RMs=np.squeeze(predictions['RM']['st1'])
 
 
     return times, RMs
 
+
+def _predownload_CDDIS(start_time,end_time,prefix='jplg',outpath='./IONEXdata/'):
+    """Downloads the IONEX maps for the required dates from CDDIS.
+    This must occur before RMextract is invoked, otherwise RMextract will try
+    to use its own download tool which is broken.
+    
+    Will try to download all the days between the start and end dates.
+    Is slightly greedy (downloading more days than) may be necessary) as a safety
+    against edge cases.
+    
+    """
+    from math import ceil, floor
+    
+    
+    #Work out how many days need to be downloaded:
+    start_date=Time(start_time)
+    end_date=Time(end_time)
+    
+    #Download each day one by one:
+    for day_mjd in range(floor(start_date.mjd)-1,ceil(end_date.mjd)+1):
+        day = Time(day_mjd,format='mjd')
+        _=get_CDDIS_IONEXfile(time=day.to_value('isot'),
+                            prefix=prefix,
+                            outpath=outpath,
+                            overwrite=False)
+    
+
+
+
 def numeric_integration(times,RMs,freq_array):
-    """Numerical integration of the time-varying ionospheric polariation 
-    modulation. Testing has shown that numerical integration is accurate 
+    """Numerical integration of the time-varying ionospheric polariation
+    modulation. Testing has shown that numerical integration is accurate
     to better than 1% accuracy except where depolarization is extreme (>99%).
-    
+
     Args:
         times (array): ionosphere sampling times (in MJD seconds, as used in RMextract)
         RMs (array): ionospheric RMs at each time (in rad/m^2)
         freq_array (array): channel frequencies (in Hz)
-    
+
     Returns: array: time-integrated ionospheric modulation per channel.
     """
 
     from scipy.integrate import simps
     l2_arr=(C/freq_array)**2
     z=np.exp(2.j*np.outer(l2_arr,RMs))
-    
+
     #Scipy's numerical integrators can't handle complex numbers, so the
     # integral needs to be broken into real and complex components.
     real=simps(z.real,times,axis=1)
     imag=simps(z.imag,times,axis=1)
     theta=(real+1.j*imag)/(times[-1]-times[0])
     return theta
-    
+
 
 
 def check_numeric_problems(RMs, freq_array,theta):
     """Checks for conditions that might cause numeric instability in the
     time-integration, and warns the user if there might be concerns.
-    
+
     Specifically, checks for extreme jumps in polarization angle between
-    timesteps (will cause integration errorrs), 
+    timesteps (will cause integration errorrs),
     and for extreme depolarization (high liklihood of large errors).
-    
+
     Args:
         RMs (array): ionospheric RMs per time step
         freq_array (array): channel frequencies (in Hz)
         theta (array): ionospheric modulation per channel.
     """
     import warnings
-    
+
     #Check for large jumps in RM/polarization angle between steps.
     #These can cause the numeric integrator to not catch angle wraps.
     longest_l2=(C/np.min(freq_array))**2
     max_deltaRM=np.max(np.diff(RMs))
     max_delta_polangle=longest_l2*max_deltaRM  #in radians
     if max_delta_polangle > 0.5:
         warnings.warn(("\nLarge variations in RM between points, which may "
                        "introduce numerical errors.\n"
                        "Consider trying a smaller timestep."))
-    
+
     #Warn about very low values of theta (very strong depolarization)
     # as these can probably not be corrected reliably.
     if np.min(np.abs(theta)) < 0.02:
         warnings.warn(("\nExtreme depolarization predicted (>98%). "
                        "Corrected polarization will almost certainly not "
                        "be trustworthy in affected channels."))
     elif np.min(np.abs(theta)) < 0.1:
         warnings.warn(("\nSignificant depolarization predicted (>90%). "
                        "Errors in corrected polarization are likely to be "
                        "very large in some channels."))
-    
-    
-    
+
+
+
 def write_modulation(freq_array,theta,filename):
     """Saves predicted ionospheric modulation to a text file.
     File has two columns, whitespace-delimited.
-    
+
     Args:
         freq_array (array): channel frequencies (in Hz)
         theta (array): ionospheric (complex) modulation at each frequency
         filename (str): file path to save data to.
 """
     np.savetxt(filename, list(zip(freq_array,theta.real,theta.imag)))
 
 
 
 
 def get_telescope_coordinates(telescope):
     """Return the astropy.coordinates EarthLocation object associated
     with the position of the telescope.
     The input must be either a string with the name of a telescope listed in
-    Astropy's sites list 
+    Astropy's sites list
     (https://github.com/astropy/astropy-data/blob/gh-pages/coordinates/sites.json),
     an EarthLocation object (which is passed through unchanged),
-    or a 3-component tuple with the latitude [deg], longitude [deg], 
+    or a 3-component tuple with the latitude [deg], longitude [deg],
     and height [m].
-    
+
     Since ASKAP is not yet listed in the Astropy sites list, it's position is
     manually coded in as a temporary measure.
-    
+
     """
     if type(telescope) == EarthLocation: #Pass EarthLocations through without processing
         return telescope
     elif type(telescope) == str: #Hardcoded coordinates for some telescopes.
         if telescope == 'ASKAP':
             lat = -1*26+42/60+15/3600 #degree
             long = +1*116+39/60+32/3600 # degree
             height = 381.0 #
         else:
             return EarthLocation.of_site(telescope)
         return EarthLocation(lat=lat*u.deg, lon=long*u.deg, height=height*u.m)
     elif (type(telescope) == tuple) or (type(telescope) == list):
-        return EarthLocation(lat=telescope[0]*u.deg, lon=telescope[1]*u.deg, 
+        return EarthLocation(lat=telescope[0]*u.deg, lon=telescope[1]*u.deg,
                              height=telescope[2]*u.m)
 
 
 
 
-    
+
 
 def generate_plots(times,RMs,theta,freq_array,position=None,savename=None):
-    """Makes a figure with two plots: the RM variation over time, 
+    """Makes a figure with two plots: the RM variation over time,
     and the (modulus of the) modulation as a function of frequency.
     If savename contains a string it will save the plots to that filename,
     otherwise the plots are not saved.
     If position ([ra,dec]) is given, it will be printed above the plots.
-    
+
     Args:
         times (astropy Time array): ionosphere sampling times
         RMs (array): ionospheric RMs at each time (in rad/m^2)
         theta (array): ionospheric (complex) modulation at each frequency
         freq_array (array): channel frequencies (in Hz)
         position (list): [ra, dec] in degrees, left blank if not supplied.
         savename (str): File path to save plot to; if 'screen' will send to display.
 
     """
     from matplotlib import pyplot as plt
     from matplotlib import dates as mdates
     plot_times=times.plot_date
-    
-    
+
+
     fig,(ax1,ax2)=plt.subplots(2,1,figsize=(8,8))
     ax1.plot_date(plot_times,RMs,fmt='k.')
     locator=mdates.AutoDateLocator(minticks=3,maxticks=7)
     formatter = mdates.ConciseDateFormatter(locator)
     ax1.xaxis.set_major_locator(locator)
     ax1.xaxis.set_major_formatter(formatter)
     ax1.set_ylabel('$\phi_\mathrm{ion}$ [rad m$^{-2}$]')
-    
+
     ax2.plot(freq_array,np.abs(theta),'k.')
     ax2.set_xlabel('Frequency [Hz]')
     ax2.set_ylabel('|$\Theta(\lambda^2)$|')
     if position is not None:
         ax1.set_title("RA: {:.2f}°, Dec: {:.2f}°".format(position[0],position[1]))
-    
+
     if savename is not None:
         if savename == "screen":
-            plt.show()    
+            plt.show()
         else:
             plt.savefig(savename,bbox_inches='tight')
 
 
 
 
 
 def get_parms_from_FITS(filename):
     """Extract relevant parameters (start time, end time, telescope, ra, dec,
     and frequencies) from a FITS file, possibly a PSRFITS file.
     If the missing keywords are not found in the FITS file, they are left blank
     and the user
-    
+
     Args:
         filename (str): path to the FITS file.
-        
-    Returns: 
+
+    Returns:
         start_time
         end_time
         freq_arr
         telescope
         ra
         dec
     """
     import astropy.io.fits as pf
     hdulist=pf.open(filename)
     header=hdulist[0].header
 
-    
+
     start_time=None
     end_time=None
     freq_arr=None
     telescope=None
     ra=None
     dec=None
 
-    #PSRFITS files have a different format, so split prpcesing depending on 
+    #PSRFITS files have a different format, so split prpcesing depending on
     #PSRFITS vs FITS image:
     if 'FITSTYPE' in header.keys() and header['FITSTYPE']=='PSRFITS':
         #PRSFITS code adapted from example by David Kaplan.
         #I'm trying to avoid using a PSRFITS reader module, to minimize dependencies,
         #at risk of not handling all variations of PSRFITS properly.
 
         if 'STT_IMJD' in header.keys():
             start_time=Time(float(header['STT_IMJD']) +
                         (float(header['STT_SMJD'])+
                          float(header['STT_OFFS']))/float(86400),
-                        format='mjd')        
+                        format='mjd')
 
             try:
                 end_time = start_time + np.sum(hdulist['SUBINT'].data['TSUBINT']) * u.s
             except:
                 pass
 
         if 'TELESCOP' in header.keys():
@@ -512,29 +574,29 @@
                                                      header['ANT_Z'],
                                                      unit=u.m)
 
         if 'RA' in header.keys():
             ra=Angle(hdulist[0].header['RA'],unit='hour')
         if 'DEC' in header.keys():
             dec=Angle(hdulist[0].header['DEC'],unit='deg')
-        
+
         if 'OBSFREQ' in header.keys() and 'OBSNCHAN' in header.keys() and 'OBSBW' in header.keys():
             chan_bw=header['OBSBW']/header['OBSNCHAN']
-            
+
             startchan= header['OBSFREQ'] - (header['OBSNCHAN']/2 - 1)*chan_bw
             freq_arr=np.arange(header['OBSNCHAN'])*chan_bw+startchan
 
 
     #FITS images/cubes:
     else:
         if 'DATE-OBS' in header.keys():
             start_time=Time(header['DATE-OBS'])
         if 'DATE-OBS' in header.keys() and 'DURATION' in header.keys():
             end_time=Time(header['DATE-OBS'])+TimeDelta(header['DURATION'],format="sec")
-        
+
         #For coordinates, the code will always use the middle pixel to derive
         #the RA and Dec. Assumes position coordinates are in first 2 axes.
         if 'RA' in header['CTYPE1']:
             ra=header['CRVAL1']+header['CDELT1']*(header['NAXIS1']/2-header['CRPIX1'])
         if 'DEC' in header['CTYPE2']:
             dec=header['CRVAL2']+header['CDELT2']*(header['NAXIS2']/2-header['CRPIX2'])
         if 'GLON' in header['CTYPE1'] and 'GLAT' in header['CTYPE2']:
@@ -543,45 +605,45 @@
             gb=header['CRVAL2']+header['CDELT2']*(header['NAXIS2']/2-header['CRPIX2'])
             position=SkyCoord(gl,gb,frame='galactic',unit='deg')
             ra=position.fk5.ra.deg
             dec=position.fk5.dec.deg
 
         if 'TELESCOP' in header.keys():
             telescope=header['TELESCOP']
-                
+
         freq_axis=str(find_freq_axis(header))
-        if freq_axis != '0':  
+        if freq_axis != '0':
             chan0=header['CRVAL'+freq_axis]-header['CDELT'+freq_axis]*(header['CRPIX'+freq_axis]-1)
             chan_final=chan0+(header['NAXIS'+freq_axis]-1)*header['CDELT'+freq_axis]
             freq_arr=np.linspace(chan0,chan_final,header['NAXIS'+freq_axis])
 
     return start_time,end_time,freq_arr,telescope,ra,dec
 
 
 
-    
-    
-    
+
+
+
 
 def timeseries():
     """
     Wrapper for command line interface, for time-series mode.
-    Gets command line arguments, feeds them into RMextract, and saves the 
+    Gets command line arguments, feeds them into RMextract, and saves the
     output to the file if specified or prints to terminal.
-    
+
     If the package is installed, it can be called as frion_timeseries,
     otherwise as python -c 'import FRion.predict; predict.timeseries()'
-    
+
     Call with the -h flag to see command line options.
     """
     import argparse
     descStr = """
     Calculate ionospheric Faraday rotation as a function of time.
-    Can determine the observation time, direction, and location parameters 
-    from a supplied FITS cube or PSRFITS file, if it has the correct keywords, 
+    Can determine the observation time, direction, and location parameters
+    from a supplied FITS cube or PSRFITS file, if it has the correct keywords,
     otherwise from those parameters must be supplied on the command line.
     """
 
     parser = argparse.ArgumentParser(description=descStr,
                                  formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument("-F",dest="fits",default=None,metavar='FILENAME',
                         help="FITS cube relevant information in header.")
@@ -610,51 +672,51 @@
 
     start_time=None
     end_time=None
     freq_arr=None
     telescope=None
     ra=None
     dec=None
-    
+
 
     #If a FITS file is present, try to fill in any missing keywords.
     #But since FITS headers can be very different, it may be that not all
     #keywords can be found.
     if args.fits is not None:
         start_time,end_time,freq_arr,telescope,ra,dec=get_parms_from_FITS(args.fits)
-            
+
     #Any parametrs taken from FITS header can be overridden by manual inputs:
     if args.times is not None:
         start_time=Time(args.times[0])
         end_time=Time(args.times[1])
-        
+
 
     if args.telescope_name is not None:
         telescope = get_telescope_coordinates(args.telescope_name)
     if args.telescope_coords is not None:
         telescope = get_telescope_coordinates(args.telescope_coords)
-    
+
     if args.pointing is not None:
         ra=args.pointing[0]
         dec=args.pointing[1]
-    
+
     #Check that all parameters are set:
     missing_parms=[]
     if (start_time is None): missing_parms.append('Start time')
     if (end_time is None): missing_parms.append('End time')
     if (telescope is None): missing_parms.append('Telescope')
     if (ra is None): missing_parms.append('Pointing center')
 
     if len(missing_parms) > 0:
         print("\n\nMissing parameters:",missing_parms,'\n')
         raise Exception("Cannot continue without parameters listed above.")
-    
+
     times,RMs=get_RM(start_time, end_time, telescope,
                          ra,dec, timestep=args.timestep,ionexPath='./IONEXdata/')
-    
+
     if args.savefile is not None:
         write_timeseries(times,RMs,args.savefile,timeformat=args.timeformat)
     else:
         print('Times:      RM:')
         for tm, rm in zip(times.to_value(args.timeformat),RMs):
             print(tm,rm)
 
@@ -667,66 +729,66 @@
 
 
 
 def write_timeseries(times,RMs,filename,timeformat='mjd'):
     """Saves the predicted ionospheric RMs as a function of time to a text file.
     File has two columns, whitespace-delimited (Be aware that some time formats
     will add whitespace to the time column.)
-    
+
     Args:
         times (astropy Time array): ionosphere sampling times
         RMs (array): ionospheric RMs at each time (in rad/m^2)
         filename (str): file path to save data to.
         timeformat (str): preferred format for writing times.
             Possible values can be found at
             https://docs.astropy.org/en/stable/time/index.html#time-format
             default is 'mjd' (e.g., ‘51544.0’).
-    
+
     """
     fout = open(filename, "w")
     for tm, rm in zip(times.to_value(timeformat),RMs):
             print(tm,rm, file=fout)
 
 
 
 
 
 def plot_timeseries(times,RMs,position=None,savename=None):
-    """Makes a figure plotting the RM variation over time, 
+    """Makes a figure plotting the RM variation over time,
     If savename contains a string it will save the plots to that filename
     (unless the name is 'screen', in which case it will plot on screen),
     otherwise the plots are not saved.
     If position ([ra,dec]) is given, it will be printed above the plots.
-    
+
     Args:
         times (astropy Time array): ionosphere sampling times
         RMs (array): ionospheric RMs at each time (in rad/m^2)
         position (list): [ra, dec] in degrees, left blank if not supplied.
         savename (str): File path to save plot to; if 'screen' will send to display.
 
     """
     from matplotlib import pyplot as plt
     from matplotlib import dates as mdates
     plot_times=times.plot_date
-    
-    
+
+
     fig,ax1=plt.subplots(1,1,figsize=(8,8))
     ax1.plot_date(plot_times,RMs,fmt='k.')
     locator=mdates.AutoDateLocator(minticks=3,maxticks=7)
     formatter = mdates.ConciseDateFormatter(locator)
     ax1.xaxis.set_major_locator(locator)
     ax1.xaxis.set_major_formatter(formatter)
     ax1.set_ylabel('$\phi_\mathrm{ion}$ [rad m$^{-2}$]')
-    
+
     if position is not None:
         ax1.set_title("RA: {:.2f}°, Dec: {:.2f}°".format(position[0],position[1]))
-    
+
     if savename is not None:
         if savename == "screen":
-            plt.show()    
+            plt.show()
         else:
             plt.savefig(savename,bbox_inches='tight')
 
 
 
 if __name__ == "__main__":
     predict()
```

### Comparing `FRion-1.0/README.md` & `FRion-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Ionospheric Faraday rotation corrections.
 
 Scripts for calculating and applying ionospheric Faraday rotation corrections for radio polarization data, primarily time-independent corrections.
 
 **Full documentation can be found [here](https://frion.readthedocs.io/en/latest/).**
+Note that there are significant changes in **Version 1.1**, which are documented there.
 
 The core underlying tool is [RMextract](https://github.com/lofar-astron/RMextract/) which calculates the time-dependent ionospheric Faraday rotation. This script uses that to generate the time-integrated correction for a given observation.
 
 This is being written for the POSSUM pipeline, but with hopes that it can be general enough to apply to other data sets.
 
+This packages original author, and maintainer as of Mar 2022, is Cameron Van Eck (cameron.van.eck (at) utoronto.ca).
+Please submit bug reports and feature requests fo the GitHub issues page, and feel free to email me with questions or comments.
+
+More information on the Canadian Initiative for Radio Astronomy Data Analysis (CIRADA) can be found at cirada.ca.
 
-Cameron Van Eck, April 2021
```

### Comparing `FRion-1.0/setup.py` & `FRion-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from setuptools import find_packages, setup, Command
 
 NAME = 'FRion'
 DESCRIPTION = 'Ionospheric Faraday rotation prediction and correction for radio astronomy polarization cubes.'
 URL = 'https://github.com/Cameron-Van-Eck/FRion'
 REQUIRES_PYTHON = '>=3.5.0'
-VERSION = '1.0'
+VERSION = '1.1.0'
 DOWNLOAD_URL = 'https://github.com/Cameron-Van-Eck/FRion/archive/refs/heads/main.zip'
 
 REQUIRED = [
-    'numpy', 'astropy', 'pyephem',
+    'numpy', 'astropy', 'pyephem', 'requests'
     ]
 
 extras_require={}
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 try:
@@ -53,9 +53,9 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Astronomy',
     ],
     maintainer='Cameron Van Eck',
-    maintainer_email='cameron.van.eck@utoronto.ca',
+    maintainer_email='cameron.vaneck@anu.edu.au',
 )
```

