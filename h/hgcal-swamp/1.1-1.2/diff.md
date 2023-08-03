# Comparing `tmp/hgcal_swamp-1.1.tar.gz` & `tmp/hgcal_swamp-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgcal_swamp-1.1.tar", last modified: Thu Aug  3 09:33:28 2023, max compression
+gzip compressed data, was "hgcal_swamp-1.2.tar", last modified: Thu Aug  3 09:43:26 2023, max compression
```

## Comparing `hgcal_swamp-1.1.tar` & `hgcal_swamp-1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-08-03 09:33:28.639003 hgcal_swamp-1.1/
--rw-r--r--   0 simondejean   (501) staff       (20)      134 2023-08-03 09:33:28.638891 hgcal_swamp-1.1/PKG-INFO
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-08-03 09:33:28.638088 hgcal_swamp-1.1/hgcal_swamp/
--rw-r--r--   0 simondejean   (501) staff       (20)      628 2023-08-03 09:31:54.000000 hgcal_swamp-1.1/hgcal_swamp/__init__.py
--rw-r--r--   0 simondejean   (501) staff       (20)     5721 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/app.py
--rw-r--r--   0 simondejean   (501) staff       (20)    27319 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/econ.py
--rw-r--r--   0 simondejean   (501) staff       (20)     4172 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/econ_control.py
--rwxr-xr-x   0 simondejean   (501) staff       (20)     2820 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/emp_interface.py
--rw-r--r--   0 simondejean   (501) staff       (20)     2537 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/gpio_control.py
--rw-r--r--   0 simondejean   (501) staff       (20)     4451 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/lpgbt_adc.py
--rw-r--r--   0 simondejean   (501) staff       (20)     2512 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/lpgbt_control.py
--rw-r--r--   0 simondejean   (501) staff       (20)     2392 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/lpgbt_gpio.py
--rw-r--r--   0 simondejean   (501) staff       (20)     4053 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/lpgbt_i2c.py
--rw-r--r--   0 simondejean   (501) staff       (20)     5459 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/lpgbt_ic.py
--rw-r--r--   0 simondejean   (501) staff       (20)     3938 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/lpgbt_ic_emp.py
--rw-r--r--   0 simondejean   (501) staff       (20)     1430 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/pt1000.py
--rw-r--r--   0 simondejean   (501) staff       (20)    19118 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/roc.py
--rw-r--r--   0 simondejean   (501) staff       (20)     3667 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/roc_control.py
--rw-r--r--   0 simondejean   (501) staff       (20)     7857 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/sc_lpgbt.py
--rw-r--r--   0 simondejean   (501) staff       (20)     4717 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/sc_transactor_interface.py
--rw-r--r--   0 simondejean   (501) staff       (20)      250 2023-07-25 14:26:03.000000 hgcal_swamp-1.1/hgcal_swamp/setup.py
--rw-r--r--   0 simondejean   (501) staff       (20)     6795 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/swampObject.py
--rw-r--r--   0 simondejean   (501) staff       (20)     5799 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/temperature_read_test.py
--rw-r--r--   0 simondejean   (501) staff       (20)     3256 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/testECON.py
--rw-r--r--   0 simondejean   (501) staff       (20)     2374 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/testROC.py
--rw-r--r--   0 simondejean   (501) staff       (20)     2797 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/transactorDecoding.py
--rw-r--r--   0 simondejean   (501) staff       (20)     4745 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/transactorEncoding.py
--rw-r--r--   0 simondejean   (501) staff       (20)     8276 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/util.py
--rw-r--r--   0 simondejean   (501) staff       (20)     2053 2023-07-25 13:32:51.000000 hgcal_swamp-1.1/hgcal_swamp/vtrx.py
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-08-03 09:33:28.638730 hgcal_swamp-1.1/hgcal_swamp.egg-info/
--rw-r--r--   0 simondejean   (501) staff       (20)      134 2023-08-03 09:33:28.000000 hgcal_swamp-1.1/hgcal_swamp.egg-info/PKG-INFO
--rw-r--r--   0 simondejean   (501) staff       (20)      858 2023-08-03 09:33:28.000000 hgcal_swamp-1.1/hgcal_swamp.egg-info/SOURCES.txt
--rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-08-03 09:33:28.000000 hgcal_swamp-1.1/hgcal_swamp.egg-info/dependency_links.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       61 2023-08-03 09:33:28.000000 hgcal_swamp-1.1/hgcal_swamp.egg-info/requires.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       12 2023-08-03 09:33:28.000000 hgcal_swamp-1.1/hgcal_swamp.egg-info/top_level.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-08-03 09:33:28.639037 hgcal_swamp-1.1/setup.cfg
--rw-r--r--   0 simondejean   (501) staff       (20)      324 2023-08-03 09:33:19.000000 hgcal_swamp-1.1/setup.py
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-08-03 09:43:26.244836 hgcal_swamp-1.2/
+-rw-r--r--   0 simondejean   (501) staff       (20)      134 2023-08-03 09:43:26.244714 hgcal_swamp-1.2/PKG-INFO
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-08-03 09:43:26.243819 hgcal_swamp-1.2/hgcal_swamp/
+-rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-08-03 09:37:34.000000 hgcal_swamp-1.2/hgcal_swamp/__init__.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     5853 2023-08-03 09:39:30.000000 hgcal_swamp-1.2/hgcal_swamp/app.py
+-rw-r--r--   0 simondejean   (501) staff       (20)    27326 2023-08-03 09:42:24.000000 hgcal_swamp-1.2/hgcal_swamp/econ.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     4193 2023-08-03 09:40:36.000000 hgcal_swamp-1.2/hgcal_swamp/econ_control.py
+-rwxr-xr-x   0 simondejean   (501) staff       (20)     2820 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/emp_interface.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     2537 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/gpio_control.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     4451 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/lpgbt_adc.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     2512 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/lpgbt_control.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     2392 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/lpgbt_gpio.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     4053 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/lpgbt_i2c.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     5459 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/lpgbt_ic.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     3938 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/lpgbt_ic_emp.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     1430 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/pt1000.py
+-rw-r--r--   0 simondejean   (501) staff       (20)    19118 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/roc.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     3667 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/roc_control.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     7857 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/sc_lpgbt.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     4717 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/sc_transactor_interface.py
+-rw-r--r--   0 simondejean   (501) staff       (20)      250 2023-07-25 14:26:03.000000 hgcal_swamp-1.2/hgcal_swamp/setup.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     6795 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/swampObject.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     5799 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/temperature_read_test.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     3256 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/testECON.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     2374 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/testROC.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     2797 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/transactorDecoding.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     4745 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/transactorEncoding.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     8276 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/util.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     2053 2023-07-25 13:32:51.000000 hgcal_swamp-1.2/hgcal_swamp/vtrx.py
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-08-03 09:43:26.244531 hgcal_swamp-1.2/hgcal_swamp.egg-info/
+-rw-r--r--   0 simondejean   (501) staff       (20)      134 2023-08-03 09:43:26.000000 hgcal_swamp-1.2/hgcal_swamp.egg-info/PKG-INFO
+-rw-r--r--   0 simondejean   (501) staff       (20)      858 2023-08-03 09:43:26.000000 hgcal_swamp-1.2/hgcal_swamp.egg-info/SOURCES.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-08-03 09:43:26.000000 hgcal_swamp-1.2/hgcal_swamp.egg-info/dependency_links.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       61 2023-08-03 09:43:26.000000 hgcal_swamp-1.2/hgcal_swamp.egg-info/requires.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       12 2023-08-03 09:43:26.000000 hgcal_swamp-1.2/hgcal_swamp.egg-info/top_level.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-08-03 09:43:26.244882 hgcal_swamp-1.2/setup.cfg
+-rw-r--r--   0 simondejean   (501) staff       (20)      324 2023-08-03 09:43:19.000000 hgcal_swamp-1.2/setup.py
```

### Comparing `hgcal_swamp-1.1/hgcal_swamp/app.py` & `hgcal_swamp-1.2/hgcal_swamp/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,18 @@
-import logging
+"""import logging
 import argparse
 import sc_lpgbt, vtrx, roc
 import lpgbt_ic, lpgbt_i2c
-import util
+import util"""
+from . import logging
+from . import sc_lpgbt, vtrx, roc
+from . import lpgbt_ic, lpgbt_i2c
+from . import util
+
+import argparse
 import yaml
 from time import sleep
 
 def setup_core(lpgbt,id):
     if id=='A':
         with open("./configs/setup_daq_lpgbt.yaml") as fin:
             lpgbt_config = yaml.safe_load(fin)['daq_lpgbt']
```

### Comparing `hgcal_swamp-1.1/hgcal_swamp/econ.py` & `hgcal_swamp-1.2/hgcal_swamp/econ.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from swampObject import Chip,Transport
+from .swampObject import Chip,Transport
 import json
 import logging
-
 import functools
 import time
-import util
+from . import util
 
 def memoize(fn):
     """ Readable memoize decorator. """
 
     fn.cache = {}
     @functools.wraps(fn)
     def inner(inst, *key):
```

### Comparing `hgcal_swamp-1.1/hgcal_swamp/econ_control.py` & `hgcal_swamp-1.2/hgcal_swamp/econ_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import argparse
-import sc_lpgbt
-import econ, lpgbt_i2c
-import util
+from . import sc_lpgbt
+from . import econ, lpgbt_i2c
+from . import util
 import yaml
 import re
 from time import sleep
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
```

### Comparing `hgcal_swamp-1.1/hgcal_swamp/emp_interface.py` & `hgcal_swamp-1.2/hgcal_swamp/emp_interface.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/gpio_control.py` & `hgcal_swamp-1.2/hgcal_swamp/gpio_control.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/lpgbt_adc.py` & `hgcal_swamp-1.2/hgcal_swamp/lpgbt_adc.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/lpgbt_control.py` & `hgcal_swamp-1.2/hgcal_swamp/lpgbt_control.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/lpgbt_gpio.py` & `hgcal_swamp-1.2/hgcal_swamp/lpgbt_gpio.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/lpgbt_i2c.py` & `hgcal_swamp-1.2/hgcal_swamp/lpgbt_i2c.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/lpgbt_ic.py` & `hgcal_swamp-1.2/hgcal_swamp/lpgbt_ic.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/lpgbt_ic_emp.py` & `hgcal_swamp-1.2/hgcal_swamp/lpgbt_ic_emp.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/pt1000.py` & `hgcal_swamp-1.2/hgcal_swamp/pt1000.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/roc.py` & `hgcal_swamp-1.2/hgcal_swamp/roc.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/roc_control.py` & `hgcal_swamp-1.2/hgcal_swamp/roc_control.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/sc_lpgbt.py` & `hgcal_swamp-1.2/hgcal_swamp/sc_lpgbt.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/sc_transactor_interface.py` & `hgcal_swamp-1.2/hgcal_swamp/sc_transactor_interface.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/swampObject.py` & `hgcal_swamp-1.2/hgcal_swamp/swampObject.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/temperature_read_test.py` & `hgcal_swamp-1.2/hgcal_swamp/temperature_read_test.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/testECON.py` & `hgcal_swamp-1.2/hgcal_swamp/testECON.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/testROC.py` & `hgcal_swamp-1.2/hgcal_swamp/testROC.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/transactorDecoding.py` & `hgcal_swamp-1.2/hgcal_swamp/transactorDecoding.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/transactorEncoding.py` & `hgcal_swamp-1.2/hgcal_swamp/transactorEncoding.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/util.py` & `hgcal_swamp-1.2/hgcal_swamp/util.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp/vtrx.py` & `hgcal_swamp-1.2/hgcal_swamp/vtrx.py`

 * *Files identical despite different names*

### Comparing `hgcal_swamp-1.1/hgcal_swamp.egg-info/SOURCES.txt` & `hgcal_swamp-1.2/hgcal_swamp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

