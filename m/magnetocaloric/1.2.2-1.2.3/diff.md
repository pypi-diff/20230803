# Comparing `tmp/magnetocaloric-1.2.2.tar.gz` & `tmp/magnetocaloric-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnetocaloric-1.2.2.tar", last modified: Wed Aug  2 12:17:55 2023, max compression
+gzip compressed data, was "magnetocaloric-1.2.3.tar", last modified: Thu Aug  3 03:33:38 2023, max compression
```

## Comparing `magnetocaloric-1.2.2.tar` & `magnetocaloric-1.2.3.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 12:17:55.137944 magnetocaloric-1.2.2/
--rw-rw-rw-   0        0        0       84 2022-04-14 07:58:46.000000 magnetocaloric-1.2.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-27 08:24:00.000000 magnetocaloric-1.2.2/Licence.txt
--rw-rw-rw-   0        0        0       81 2022-04-14 07:58:45.000000 magnetocaloric-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3969 2023-08-02 12:17:55.137944 magnetocaloric-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3222 2023-08-02 12:16:03.000000 magnetocaloric-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 12:17:55.122312 magnetocaloric-1.2.2/magnetocaloric/
--rw-rw-rw-   0        0        0      560 2023-07-31 06:14:28.000000 magnetocaloric-1.2.2/magnetocaloric/Color_marker.py
--rw-rw-rw-   0        0        0     1397 2023-07-30 11:40:32.000000 magnetocaloric-1.2.2/magnetocaloric/M_H_reshaping.py
--rw-rw-rw-   0        0        0     2059 2023-07-30 11:43:59.000000 magnetocaloric-1.2.2/magnetocaloric/RCP_plot.py
--rw-rw-rw-   0        0        0     3548 2023-07-30 11:43:19.000000 magnetocaloric-1.2.2/magnetocaloric/T_FWHM_RCP.py
--rw-rw-rw-   0        0        0      831 2023-07-30 12:08:19.000000 magnetocaloric-1.2.2/magnetocaloric/__init__.py
--rw-rw-rw-   0        0        0     1487 2023-07-30 11:41:26.000000 magnetocaloric-1.2.2/magnetocaloric/arrott_plot.py
--rw-rw-rw-   0        0        0     1424 2023-07-30 11:37:12.000000 magnetocaloric-1.2.2/magnetocaloric/collect_from_database.py
--rw-rw-rw-   0        0        0     5564 2023-07-31 06:14:23.000000 magnetocaloric-1.2.2/magnetocaloric/data_visualization.py
--rw-rw-rw-   0        0        0     2433 2023-07-31 06:15:05.000000 magnetocaloric-1.2.2/magnetocaloric/entropy_change01.py
--rw-rw-rw-   0        0        0     1229 2023-07-30 11:38:43.000000 magnetocaloric-1.2.2/magnetocaloric/entropy_change02.py
--rw-rw-rw-   0        0        0     5644 2023-08-02 12:12:35.000000 magnetocaloric-1.2.2/magnetocaloric/mcepy.py
--rw-rw-rw-   0        0        0     2434 2023-07-30 11:42:47.000000 magnetocaloric-1.2.2/magnetocaloric/modified_arrott_plot.py
--rw-rw-rw-   0        0        0     2164 2023-07-30 11:39:58.000000 magnetocaloric-1.2.2/magnetocaloric/store_to_database.py
--rw-rw-rw-   0        0        0      930 2023-07-30 11:36:24.000000 magnetocaloric-1.2.2/magnetocaloric/take_temp.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:17:55.137944 magnetocaloric-1.2.2/magnetocaloric.egg-info/
--rw-rw-rw-   0        0        0     3969 2023-08-02 12:17:54.000000 magnetocaloric-1.2.2/magnetocaloric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-08-02 12:17:54.000000 magnetocaloric-1.2.2/magnetocaloric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 12:17:54.000000 magnetocaloric-1.2.2/magnetocaloric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-08-02 12:17:54.000000 magnetocaloric-1.2.2/magnetocaloric.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-08-02 12:17:54.000000 magnetocaloric-1.2.2/magnetocaloric.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 12:17:55.153573 magnetocaloric-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1190 2023-08-02 12:15:29.000000 magnetocaloric-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:33:38.513958 magnetocaloric-1.2.3/
+-rw-rw-rw-   0        0        0       84 2022-04-14 07:58:46.000000 magnetocaloric-1.2.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-27 08:24:00.000000 magnetocaloric-1.2.3/Licence.txt
+-rw-rw-rw-   0        0        0       81 2022-04-14 07:58:45.000000 magnetocaloric-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3969 2023-08-03 03:33:38.513958 magnetocaloric-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3222 2023-08-03 03:31:24.000000 magnetocaloric-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 03:33:38.467065 magnetocaloric-1.2.3/magnetocaloric/
+-rw-rw-rw-   0        0        0      560 2023-07-31 06:14:28.000000 magnetocaloric-1.2.3/magnetocaloric/Color_marker.py
+-rw-rw-rw-   0        0        0     1397 2023-07-30 11:40:32.000000 magnetocaloric-1.2.3/magnetocaloric/M_H_reshaping.py
+-rw-rw-rw-   0        0        0     2059 2023-07-30 11:43:59.000000 magnetocaloric-1.2.3/magnetocaloric/RCP_plot.py
+-rw-rw-rw-   0        0        0     3548 2023-07-30 11:43:19.000000 magnetocaloric-1.2.3/magnetocaloric/T_FWHM_RCP.py
+-rw-rw-rw-   0        0        0      831 2023-07-30 12:08:19.000000 magnetocaloric-1.2.3/magnetocaloric/__init__.py
+-rw-rw-rw-   0        0        0     1487 2023-07-30 11:41:26.000000 magnetocaloric-1.2.3/magnetocaloric/arrott_plot.py
+-rw-rw-rw-   0        0        0     1424 2023-07-30 11:37:12.000000 magnetocaloric-1.2.3/magnetocaloric/collect_from_database.py
+-rw-rw-rw-   0        0        0     5566 2023-08-03 03:03:55.000000 magnetocaloric-1.2.3/magnetocaloric/data_visualization01.py
+-rw-rw-rw-   0        0        0     6058 2023-08-03 03:29:23.000000 magnetocaloric-1.2.3/magnetocaloric/data_visualization02.py
+-rw-rw-rw-   0        0        0     2433 2023-07-31 06:15:05.000000 magnetocaloric-1.2.3/magnetocaloric/entropy_change01.py
+-rw-rw-rw-   0        0        0     1229 2023-07-30 11:38:43.000000 magnetocaloric-1.2.3/magnetocaloric/entropy_change02.py
+-rw-rw-rw-   0        0        0     5656 2023-08-03 03:13:25.000000 magnetocaloric-1.2.3/magnetocaloric/mcepy.py
+-rw-rw-rw-   0        0        0     2434 2023-07-30 11:42:47.000000 magnetocaloric-1.2.3/magnetocaloric/modified_arrott_plot.py
+-rw-rw-rw-   0        0        0     2166 2023-08-03 03:09:46.000000 magnetocaloric-1.2.3/magnetocaloric/store_to_database01.py
+-rw-rw-rw-   0        0        0     2408 2023-08-03 03:29:18.000000 magnetocaloric-1.2.3/magnetocaloric/store_to_database02.py
+-rw-rw-rw-   0        0        0      930 2023-07-30 11:36:24.000000 magnetocaloric-1.2.3/magnetocaloric/take_temp.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:33:38.513958 magnetocaloric-1.2.3/magnetocaloric.egg-info/
+-rw-rw-rw-   0        0        0     3969 2023-08-03 03:33:37.000000 magnetocaloric-1.2.3/magnetocaloric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2023-08-03 03:33:37.000000 magnetocaloric-1.2.3/magnetocaloric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 03:33:37.000000 magnetocaloric-1.2.3/magnetocaloric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-08-03 03:33:37.000000 magnetocaloric-1.2.3/magnetocaloric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-03 03:33:37.000000 magnetocaloric-1.2.3/magnetocaloric.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 03:33:38.513958 magnetocaloric-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1190 2023-08-03 03:31:35.000000 magnetocaloric-1.2.3/setup.py
```

### Comparing `magnetocaloric-1.2.2/Licence.txt` & `magnetocaloric-1.2.3/Licence.txt`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.2/PKG-INFO` & `magnetocaloric-1.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnetocaloric
-Version: 1.2.2
+Version: 1.2.3
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
 
 
-# magnetocaloric 1.2.2
+# magnetocaloric 1.2.3
 #### Developed by Supratim Das
 
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
 
 Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
 
 ## What's New
@@ -38,15 +38,15 @@
 
 ### 1. Installation 
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
 
 ```bash
 
- pip install magnetocaloric==1.2.2
+ pip install magnetocaloric==1.2.3
 
 ```
 ### 2. Manage Excel Spreadsheet
 -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
 
 ![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
```

### Comparing `magnetocaloric-1.2.2/README.md` & `magnetocaloric-1.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# magnetocaloric 1.2.2
+# magnetocaloric 1.2.3
 #### Developed by Supratim Das
 
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
 
 Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
 
 ## What's New
@@ -21,15 +21,15 @@
 
 ### 1. Installation 
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
 
 ```bash
 
- pip install magnetocaloric==1.2.2
+ pip install magnetocaloric==1.2.3
 
 ```
 ### 2. Manage Excel Spreadsheet
 -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
 
 ![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
```

### Comparing `magnetocaloric-1.2.2/magnetocaloric/Color_marker.py` & `magnetocaloric-1.2.3/magnetocaloric/Color_marker.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.2/magnetocaloric/M_H_reshaping.py` & `magnetocaloric-1.2.3/magnetocaloric/M_H_reshaping.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.2/magnetocaloric/RCP_plot.py` & `magnetocaloric-1.2.3/magnetocaloric/RCP_plot.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.2/magnetocaloric/T_FWHM_RCP.py` & `magnetocaloric-1.2.3/magnetocaloric/T_FWHM_RCP.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.2/magnetocaloric/__init__.py` & `magnetocaloric-1.2.3/magnetocaloric/__init__.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.2/magnetocaloric/arrott_plot.py` & `magnetocaloric-1.2.3/magnetocaloric/arrott_plot.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.2/magnetocaloric/collect_from_database.py` & `magnetocaloric-1.2.3/magnetocaloric/collect_from_database.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.2/magnetocaloric/data_visualization.py` & `magnetocaloric-1.2.3/magnetocaloric/data_visualization01.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib.pyplot as plt
 import itertools
 
-def data_visualization(one_n, n, T, H, colour, marker, Label_one, plot_legend, one_M_plot_final, two_M_plot_final, H_plot_final, temperatures, five_entropy_change_con, M_sqr, one_H_by_M_con):
+def data_visualization01(one_n, n, T, H, colour, marker, Label_one, plot_legend, one_M_plot_final, two_M_plot_final, H_plot_final, temperatures, five_entropy_change_con, M_sqr, one_H_by_M_con):
     """
     Visualize the data using Matplotlib.
 
     Args:
         one_n (int): Number of data points along one direction.
         n (int): Total number of data points.
         T (list): List of temperature values.
```

### Comparing `magnetocaloric-1.2.2/magnetocaloric/entropy_change01.py` & `magnetocaloric-1.2.3/magnetocaloric/entropy_change01.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.2/magnetocaloric/entropy_change02.py` & `magnetocaloric-1.2.3/magnetocaloric/entropy_change02.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.2/magnetocaloric/mcepy.py` & `magnetocaloric-1.2.3/magnetocaloric/mcepy.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 import sys
 import itertools
 
 
 from .arrott_plot import arrott_plot
 from .collect_from_database import collect_from_database
 from .Color_marker import Color_marker
-from .data_visualization import data_visualization
+from .data_visualization01 import data_visualization01
 from .entropy_change01 import entropy_change01
 from .entropy_change02 import entropy_change02
 from .M_H_reshaping import M_H_reshaping
 from .modified_arrott_plot import modified_arrott_plot
 from .RCP_plot import RCP_plot
-from .store_to_database import store_to_database
+from .store_to_database01 import store_to_database01
 from .T_FWHM_RCP import T_FWHM_RCP
 from .take_temp import take_temp
 
 if not sys.warnoptions:
     import warnings
     warnings.simplefilter("ignore")
 
@@ -90,27 +90,27 @@
     # Magnetization and Field Reshaping
     one_M_plot_final, two_M_plot_final = M_H_reshaping(one_n, n, M, H)
 
     # Arrott Plot
     H_plot_final, M_sqr, one_H_by_M_con = arrott_plot(one_n, n, M, H, T, one_M_plot_final)
 
     # Data Visualization
-    data_visualization(one_n, n, T, H, colour, marker, Label_one, plot_legend, one_M_plot_final, two_M_plot_final, H_plot_final, temperatures, five_entropy_change_con, M_sqr, one_H_by_M_con)
+    data_visualization01(one_n, n, T, H, colour, marker, Label_one, plot_legend, one_M_plot_final, two_M_plot_final, H_plot_final, temperatures, five_entropy_change_con, M_sqr, one_H_by_M_con)
 
     # Modified Arrott Plot
     modified_arrott_plot(n, one_M_plot_final, one_H_by_M_con)
 
     # Calculate T_FWHM and RCP
     T_FWHM_con, RCP_con, RCP_final, H_for_RCP = T_FWHM_RCP(n, Label_one, six_entropy_change_con)
 
     # Plot RCP and T_FWHM
     RCP_plot(T_FWHM_con, Label_one, RCP_con, RCP_final, H_for_RCP, samp_name)
 
     # Store Data to Excel Files
-    store_to_database(n, T, one_H_by_M_con, M_sqr, path_two, path_three, six_entropy_change_con)
+    store_to_database01(n, T, one_H_by_M_con, M_sqr, path_two, path_three, six_entropy_change_con)
 
     return
 
 
 def sysdtpas():
     cekch_ady = [2, 5, 8, 11, 14, 17, 20, 23, 26, 29]
     for i in range(0, len(cekch_ady), 1):
```

### Comparing `magnetocaloric-1.2.2/magnetocaloric/modified_arrott_plot.py` & `magnetocaloric-1.2.3/magnetocaloric/modified_arrott_plot.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.2/magnetocaloric/store_to_database.py` & `magnetocaloric-1.2.3/magnetocaloric/store_to_database01.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import xlsxwriter
 
-def store_to_database(n, T, one_H_by_M_con, M_sqr, path_two, path_three, six_entropy_change_con):
+def store_to_database01(n, T, one_H_by_M_con, M_sqr, path_two, path_three, six_entropy_change_con):
     """
     Store data to two separate Excel spreadsheets.
 
     Args:
         n (int): Number of data points.
         T (list): List of temperature values.
         one_H_by_M_con (list): List of lists containing H/M values for each temperature.
```

### Comparing `magnetocaloric-1.2.2/magnetocaloric/take_temp.py` & `magnetocaloric-1.2.3/magnetocaloric/take_temp.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.2/magnetocaloric.egg-info/PKG-INFO` & `magnetocaloric-1.2.3/magnetocaloric.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnetocaloric
-Version: 1.2.2
+Version: 1.2.3
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
 
 
-# magnetocaloric 1.2.2
+# magnetocaloric 1.2.3
 #### Developed by Supratim Das
 
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
 
 Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
 
 ## What's New
@@ -38,15 +38,15 @@
 
 ### 1. Installation 
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
 
 ```bash
 
- pip install magnetocaloric==1.2.2
+ pip install magnetocaloric==1.2.3
 
 ```
 ### 2. Manage Excel Spreadsheet
 -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
 
 ![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
```

### Comparing `magnetocaloric-1.2.2/magnetocaloric.egg-info/SOURCES.txt` & `magnetocaloric-1.2.3/magnetocaloric.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 magnetocaloric/Color_marker.py
 magnetocaloric/M_H_reshaping.py
 magnetocaloric/RCP_plot.py
 magnetocaloric/T_FWHM_RCP.py
 magnetocaloric/__init__.py
 magnetocaloric/arrott_plot.py
 magnetocaloric/collect_from_database.py
-magnetocaloric/data_visualization.py
+magnetocaloric/data_visualization01.py
+magnetocaloric/data_visualization02.py
 magnetocaloric/entropy_change01.py
 magnetocaloric/entropy_change02.py
 magnetocaloric/mcepy.py
 magnetocaloric/modified_arrott_plot.py
-magnetocaloric/store_to_database.py
+magnetocaloric/store_to_database01.py
+magnetocaloric/store_to_database02.py
 magnetocaloric/take_temp.py
 magnetocaloric.egg-info/PKG-INFO
 magnetocaloric.egg-info/SOURCES.txt
 magnetocaloric.egg-info/dependency_links.txt
 magnetocaloric.egg-info/requires.txt
 magnetocaloric.egg-info/top_level.txt
```

### Comparing `magnetocaloric-1.2.2/setup.py` & `magnetocaloric-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='magnetocaloric',
-  version='1.2.2',
+  version='1.2.3',
   description='Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python',
   long_description=long_description,
   long_description_content_type="text/markdown",
   url='https://github.com/supratimdasinfo/Magnetocaloric-Effect',  
   author='Supratim Das',
   author_email='supratim0707@gmail.com',
   license='MIT',
```

