# Comparing `tmp/magnetocaloric-1.2.7.tar.gz` & `tmp/magnetocaloric-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnetocaloric-1.2.7.tar", last modified: Thu Aug  3 04:35:09 2023, max compression
+gzip compressed data, was "magnetocaloric-1.2.8.tar", last modified: Thu Aug  3 04:49:11 2023, max compression
```

## Comparing `magnetocaloric-1.2.7.tar` & `magnetocaloric-1.2.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 04:35:09.535555 magnetocaloric-1.2.7/
--rw-rw-rw-   0        0        0       84 2022-04-14 07:58:46.000000 magnetocaloric-1.2.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-27 08:24:00.000000 magnetocaloric-1.2.7/Licence.txt
--rw-rw-rw-   0        0        0       81 2022-04-14 07:58:45.000000 magnetocaloric-1.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3969 2023-08-03 04:35:09.535555 magnetocaloric-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     3222 2023-08-03 04:33:37.000000 magnetocaloric-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 04:35:09.504295 magnetocaloric-1.2.7/magnetocaloric/
--rw-rw-rw-   0        0        0      560 2023-07-31 06:14:28.000000 magnetocaloric-1.2.7/magnetocaloric/Color_marker.py
--rw-rw-rw-   0        0        0     1397 2023-07-30 11:40:32.000000 magnetocaloric-1.2.7/magnetocaloric/M_H_reshaping.py
--rw-rw-rw-   0        0        0     2059 2023-07-30 11:43:59.000000 magnetocaloric-1.2.7/magnetocaloric/RCP_plot.py
--rw-rw-rw-   0        0        0     3548 2023-07-30 11:43:19.000000 magnetocaloric-1.2.7/magnetocaloric/T_FWHM_RCP.py
--rw-rw-rw-   0        0        0     1010 2023-08-03 04:11:16.000000 magnetocaloric-1.2.7/magnetocaloric/__init__.py
--rw-rw-rw-   0        0        0     1487 2023-07-30 11:41:26.000000 magnetocaloric-1.2.7/magnetocaloric/arrott_plot.py
--rw-rw-rw-   0        0        0     1424 2023-07-30 11:37:12.000000 magnetocaloric-1.2.7/magnetocaloric/collect_from_database.py
--rw-rw-rw-   0        0        0     5566 2023-08-03 03:03:55.000000 magnetocaloric-1.2.7/magnetocaloric/data_visualization01.py
--rw-rw-rw-   0        0        0     6058 2023-08-03 03:29:23.000000 magnetocaloric-1.2.7/magnetocaloric/data_visualization02.py
--rw-rw-rw-   0        0        0     2433 2023-07-31 06:15:05.000000 magnetocaloric-1.2.7/magnetocaloric/entropy_change01.py
--rw-rw-rw-   0        0        0     1229 2023-07-30 11:38:43.000000 magnetocaloric-1.2.7/magnetocaloric/entropy_change02.py
--rw-rw-rw-   0        0        0    13892 2023-08-03 04:34:22.000000 magnetocaloric-1.2.7/magnetocaloric/mcepy.py
--rw-rw-rw-   0        0        0     2434 2023-07-30 11:42:47.000000 magnetocaloric-1.2.7/magnetocaloric/modified_arrott_plot.py
--rw-rw-rw-   0        0        0     2166 2023-08-03 03:09:46.000000 magnetocaloric-1.2.7/magnetocaloric/store_to_database01.py
--rw-rw-rw-   0        0        0     2408 2023-08-03 03:29:18.000000 magnetocaloric-1.2.7/magnetocaloric/store_to_database02.py
--rw-rw-rw-   0        0        0      930 2023-07-30 11:36:24.000000 magnetocaloric-1.2.7/magnetocaloric/take_temp.py
-drwxrwxrwx   0        0        0        0 2023-08-03 04:35:09.519925 magnetocaloric-1.2.7/magnetocaloric.egg-info/
--rw-rw-rw-   0        0        0     3969 2023-08-03 04:35:09.000000 magnetocaloric-1.2.7/magnetocaloric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      776 2023-08-03 04:35:09.000000 magnetocaloric-1.2.7/magnetocaloric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 04:35:09.000000 magnetocaloric-1.2.7/magnetocaloric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-08-03 04:35:09.000000 magnetocaloric-1.2.7/magnetocaloric.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-08-03 04:35:09.000000 magnetocaloric-1.2.7/magnetocaloric.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 04:35:09.535555 magnetocaloric-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1190 2023-08-03 04:33:24.000000 magnetocaloric-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 04:49:11.759707 magnetocaloric-1.2.8/
+-rw-rw-rw-   0        0        0       84 2022-04-14 07:58:46.000000 magnetocaloric-1.2.8/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-27 08:24:00.000000 magnetocaloric-1.2.8/Licence.txt
+-rw-rw-rw-   0        0        0       81 2022-04-14 07:58:45.000000 magnetocaloric-1.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3969 2023-08-03 04:49:11.759707 magnetocaloric-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3222 2023-08-03 04:47:43.000000 magnetocaloric-1.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 04:49:11.728448 magnetocaloric-1.2.8/magnetocaloric/
+-rw-rw-rw-   0        0        0      560 2023-07-31 06:14:28.000000 magnetocaloric-1.2.8/magnetocaloric/Color_marker.py
+-rw-rw-rw-   0        0        0     1397 2023-07-30 11:40:32.000000 magnetocaloric-1.2.8/magnetocaloric/M_H_reshaping.py
+-rw-rw-rw-   0        0        0     2059 2023-07-30 11:43:59.000000 magnetocaloric-1.2.8/magnetocaloric/RCP_plot.py
+-rw-rw-rw-   0        0        0     3548 2023-07-30 11:43:19.000000 magnetocaloric-1.2.8/magnetocaloric/T_FWHM_RCP.py
+-rw-rw-rw-   0        0        0     1010 2023-08-03 04:11:16.000000 magnetocaloric-1.2.8/magnetocaloric/__init__.py
+-rw-rw-rw-   0        0        0     1487 2023-07-30 11:41:26.000000 magnetocaloric-1.2.8/magnetocaloric/arrott_plot.py
+-rw-rw-rw-   0        0        0     1424 2023-07-30 11:37:12.000000 magnetocaloric-1.2.8/magnetocaloric/collect_from_database.py
+-rw-rw-rw-   0        0        0     5566 2023-08-03 03:03:55.000000 magnetocaloric-1.2.8/magnetocaloric/data_visualization01.py
+-rw-rw-rw-   0        0        0     6058 2023-08-03 03:29:23.000000 magnetocaloric-1.2.8/magnetocaloric/data_visualization02.py
+-rw-rw-rw-   0        0        0     2433 2023-07-31 06:15:05.000000 magnetocaloric-1.2.8/magnetocaloric/entropy_change01.py
+-rw-rw-rw-   0        0        0     1229 2023-07-30 11:38:43.000000 magnetocaloric-1.2.8/magnetocaloric/entropy_change02.py
+-rw-rw-rw-   0        0        0    13886 2023-08-03 04:48:53.000000 magnetocaloric-1.2.8/magnetocaloric/mcepy.py
+-rw-rw-rw-   0        0        0     2434 2023-07-30 11:42:47.000000 magnetocaloric-1.2.8/magnetocaloric/modified_arrott_plot.py
+-rw-rw-rw-   0        0        0     2166 2023-08-03 03:09:46.000000 magnetocaloric-1.2.8/magnetocaloric/store_to_database01.py
+-rw-rw-rw-   0        0        0     2408 2023-08-03 03:29:18.000000 magnetocaloric-1.2.8/magnetocaloric/store_to_database02.py
+-rw-rw-rw-   0        0        0      930 2023-07-30 11:36:24.000000 magnetocaloric-1.2.8/magnetocaloric/take_temp.py
+drwxrwxrwx   0        0        0        0 2023-08-03 04:49:11.759707 magnetocaloric-1.2.8/magnetocaloric.egg-info/
+-rw-rw-rw-   0        0        0     3969 2023-08-03 04:49:11.000000 magnetocaloric-1.2.8/magnetocaloric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2023-08-03 04:49:11.000000 magnetocaloric-1.2.8/magnetocaloric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 04:49:11.000000 magnetocaloric-1.2.8/magnetocaloric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-08-03 04:49:11.000000 magnetocaloric-1.2.8/magnetocaloric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-03 04:49:11.000000 magnetocaloric-1.2.8/magnetocaloric.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 04:49:11.759707 magnetocaloric-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1190 2023-08-03 04:47:29.000000 magnetocaloric-1.2.8/setup.py
```

### Comparing `magnetocaloric-1.2.7/Licence.txt` & `magnetocaloric-1.2.8/Licence.txt`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/PKG-INFO` & `magnetocaloric-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnetocaloric
-Version: 1.2.7
+Version: 1.2.8
 Summary: Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python
 Home-page: https://github.com/supratimdasinfo/Magnetocaloric-Effect
 Author: Supratim Das
 Author-email: supratim0707@gmail.com
 License: MIT
 Keywords: magnetocaloric,mcepy,magnetic,programming,code,python,supratim,das,bhaskar,biswas,physics
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: Licence.txt
 
 
-# magnetocaloric 1.2.7
+# magnetocaloric 1.2.8
 #### Developed by Supratim Das
 
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
 
 Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
 
 ## What's New
@@ -38,15 +38,15 @@
 
 ### 1. Installation 
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
 
 ```bash
 
- pip install magnetocaloric==1.2.7
+ pip install magnetocaloric==1.2.8
 
 ```
 ### 2. Manage Excel Spreadsheet
 -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
 
 ![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
```

### Comparing `magnetocaloric-1.2.7/README.md` & `magnetocaloric-1.2.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# magnetocaloric 1.2.7
+# magnetocaloric 1.2.8
 #### Developed by Supratim Das
 
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
 
 Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
 
 ## What's New
@@ -21,15 +21,15 @@
 
 ### 1. Installation 
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
 
 ```bash
 
- pip install magnetocaloric==1.2.7
+ pip install magnetocaloric==1.2.8
 
 ```
 ### 2. Manage Excel Spreadsheet
 -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
 
 ![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
```

### Comparing `magnetocaloric-1.2.7/magnetocaloric/Color_marker.py` & `magnetocaloric-1.2.8/magnetocaloric/Color_marker.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric/M_H_reshaping.py` & `magnetocaloric-1.2.8/magnetocaloric/M_H_reshaping.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric/RCP_plot.py` & `magnetocaloric-1.2.8/magnetocaloric/RCP_plot.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric/T_FWHM_RCP.py` & `magnetocaloric-1.2.8/magnetocaloric/T_FWHM_RCP.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric/__init__.py` & `magnetocaloric-1.2.8/magnetocaloric/__init__.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric/arrott_plot.py` & `magnetocaloric-1.2.8/magnetocaloric/arrott_plot.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric/collect_from_database.py` & `magnetocaloric-1.2.8/magnetocaloric/collect_from_database.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric/data_visualization01.py` & `magnetocaloric-1.2.8/magnetocaloric/data_visualization01.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric/data_visualization02.py` & `magnetocaloric-1.2.8/magnetocaloric/data_visualization02.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric/entropy_change01.py` & `magnetocaloric-1.2.8/magnetocaloric/entropy_change01.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric/entropy_change02.py` & `magnetocaloric-1.2.8/magnetocaloric/entropy_change02.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric/mcepy.py` & `magnetocaloric-1.2.8/magnetocaloric/mcepy.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             cpt = bcrypt.hashpw((str(psasrwdo3)).encode(), bcrypt.gensalt())
             break
 
     return cpt
 
 def chkdtpas(stored_password, entered_password):
     return bcrypt.checkpw(entered_password.encode(), stored_password)
-    
+
 def datavisualizationtwo(code, one_n, n, T, H, colour, marker, Label_one, plot_legend, one_M_plot_final, two_M_plot_final, H_plot_final, temperatures, five_entropy_change_con, M_sqr, one_H_by_M_con):
     """
     Visualize the data using Matplotlib.
 
     Args:
         one_n (int): Number of data points along one direction.
         n (int): Total number of data points.
@@ -173,15 +173,15 @@
 
     Returns:
         None: The function displays plots based on the data.
     """
     funcval = sysdtpas()
     if chkdtpas(funcval, code):
         
-        if plot_legend == 'YES':
+        if (plot_legend == 1):
 
             # Plotting magnetization vs. applied field for each temperature.
             for k in range(n):
                 plt.plot(H_plot_final, one_M_plot_final[k], linestyle='solid', label=T[n - (k + 1)], marker=next(marker), markersize=6, linewidth=2)
             plt.legend(loc='upper left', frameon=False, ncol=3)
             plt.xlabel("Magnetic Field (H)", fontname="Georgia")
             plt.ylabel("Magnetization (M)", fontname="Georgia")
```

### Comparing `magnetocaloric-1.2.7/magnetocaloric/modified_arrott_plot.py` & `magnetocaloric-1.2.8/magnetocaloric/modified_arrott_plot.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric/store_to_database01.py` & `magnetocaloric-1.2.8/magnetocaloric/store_to_database01.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric/store_to_database02.py` & `magnetocaloric-1.2.8/magnetocaloric/store_to_database02.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric/take_temp.py` & `magnetocaloric-1.2.8/magnetocaloric/take_temp.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/magnetocaloric.egg-info/PKG-INFO` & `magnetocaloric-1.2.8/magnetocaloric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnetocaloric
-Version: 1.2.7
+Version: 1.2.8
 Summary: Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python
 Home-page: https://github.com/supratimdasinfo/Magnetocaloric-Effect
 Author: Supratim Das
 Author-email: supratim0707@gmail.com
 License: MIT
 Keywords: magnetocaloric,mcepy,magnetic,programming,code,python,supratim,das,bhaskar,biswas,physics
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: Licence.txt
 
 
-# magnetocaloric 1.2.7
+# magnetocaloric 1.2.8
 #### Developed by Supratim Das
 
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
 
 Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
 
 ## What's New
@@ -38,15 +38,15 @@
 
 ### 1. Installation 
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
 
 ```bash
 
- pip install magnetocaloric==1.2.7
+ pip install magnetocaloric==1.2.8
 
 ```
 ### 2. Manage Excel Spreadsheet
 -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
 
 ![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
```

### Comparing `magnetocaloric-1.2.7/magnetocaloric.egg-info/SOURCES.txt` & `magnetocaloric-1.2.8/magnetocaloric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.7/setup.py` & `magnetocaloric-1.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='magnetocaloric',
-  version='1.2.7',
+  version='1.2.8',
   description='Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python',
   long_description=long_description,
   long_description_content_type="text/markdown",
   url='https://github.com/supratimdasinfo/Magnetocaloric-Effect',  
   author='Supratim Das',
   author_email='supratim0707@gmail.com',
   license='MIT',
```

