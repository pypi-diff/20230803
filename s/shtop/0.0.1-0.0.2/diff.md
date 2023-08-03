# Comparing `tmp/shtop-0.0.1.tar.gz` & `tmp/shtop-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shtop-0.0.1.tar", last modified: Wed Jul 19 13:35:58 2023, max compression
+gzip compressed data, was "shtop-0.0.2.tar", last modified: Thu Aug  3 13:00:16 2023, max compression
```

## Comparing `shtop-0.0.1.tar` & `shtop-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lukasplevac  (1000) lukasplevac  (1000)        0 2023-07-19 13:35:58.728266 shtop-0.0.1/
--rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)      534 2023-07-19 13:35:58.720266 shtop-0.0.1/PKG-INFO
--rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)      418 2023-07-19 13:22:51.000000 shtop-0.0.1/pyproject.toml
-drwxr-xr-x   0 lukasplevac  (1000) lukasplevac  (1000)        0 2023-07-19 13:35:58.624268 shtop-0.0.1/scripts/
--rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)     4075 2023-07-19 13:33:05.000000 shtop-0.0.1/scripts/shtop
--rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)       38 2023-07-19 13:35:58.728266 shtop-0.0.1/setup.cfg
--rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)      842 2023-07-19 13:33:46.000000 shtop-0.0.1/setup.py
-drwxr-xr-x   0 lukasplevac  (1000) lukasplevac  (1000)        0 2023-07-19 13:35:58.652267 shtop-0.0.1/shtop/
--rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)       20 2023-07-19 13:35:39.000000 shtop-0.0.1/shtop/__init__.py
--rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)     1136 2023-07-19 11:47:15.000000 shtop-0.0.1/shtop/tui.py
-drwxr-xr-x   0 lukasplevac  (1000) lukasplevac  (1000)        0 2023-07-19 13:35:58.708266 shtop-0.0.1/shtop.egg-info/
--rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)      534 2023-07-19 13:35:57.000000 shtop-0.0.1/shtop.egg-info/PKG-INFO
--rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)      184 2023-07-19 13:35:58.000000 shtop-0.0.1/shtop.egg-info/SOURCES.txt
--rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)        1 2023-07-19 13:35:57.000000 shtop-0.0.1/shtop.egg-info/dependency_links.txt
--rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)        6 2023-07-19 13:35:57.000000 shtop-0.0.1/shtop.egg-info/top_level.txt
+drwxr-xr-x   0 lukasplevac  (1000) lukasplevac  (1000)        0 2023-08-03 13:00:16.332407 shtop-0.0.2/
+-rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)      534 2023-08-03 13:00:16.328407 shtop-0.0.2/PKG-INFO
+-rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)      418 2023-07-19 13:22:51.000000 shtop-0.0.2/pyproject.toml
+drwxr-xr-x   0 lukasplevac  (1000) lukasplevac  (1000)        0 2023-08-03 13:00:16.280408 shtop-0.0.2/scripts/
+-rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)     4049 2023-08-03 12:56:47.000000 shtop-0.0.2/scripts/shtop
+-rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)       38 2023-08-03 13:00:16.336407 shtop-0.0.2/setup.cfg
+-rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)      843 2023-08-03 13:00:04.000000 shtop-0.0.2/setup.py
+drwxr-xr-x   0 lukasplevac  (1000) lukasplevac  (1000)        0 2023-08-03 13:00:16.296408 shtop-0.0.2/shtop/
+-rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)       20 2023-07-19 13:35:39.000000 shtop-0.0.2/shtop/__init__.py
+-rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)     1136 2023-07-19 11:47:15.000000 shtop-0.0.2/shtop/tui.py
+drwxr-xr-x   0 lukasplevac  (1000) lukasplevac  (1000)        0 2023-08-03 13:00:16.324407 shtop-0.0.2/shtop.egg-info/
+-rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)      534 2023-08-03 13:00:15.000000 shtop-0.0.2/shtop.egg-info/PKG-INFO
+-rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)      184 2023-08-03 13:00:16.000000 shtop-0.0.2/shtop.egg-info/SOURCES.txt
+-rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)        1 2023-08-03 13:00:15.000000 shtop-0.0.2/shtop.egg-info/dependency_links.txt
+-rw-r--r--   0 lukasplevac  (1000) lukasplevac  (1000)        6 2023-08-03 13:00:15.000000 shtop-0.0.2/shtop.egg-info/top_level.txt
```

### Comparing `shtop-0.0.1/PKG-INFO` & `shtop-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: shtop
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple tui slurm job viewer.
 Home-page: UNKNOWN
 Author: Lukáš Plevač
 Author-email: <lukas@plevac.eu>
 License: UNKNOWN
 Description: Simple tui slurm job viewer. Using /etc/hosts and ssh to get CPU and RAM utilization of all cluster nodes. Distrubuted using PIP and writen in python.
 Keywords: python,slurm,shtop,top,htop
```

### Comparing `shtop-0.0.1/scripts/shtop` & `shtop-0.0.2/scripts/shtop`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 	stdout = stdout.split("\n")
 
 	for i in range(len(stdout)):
 		stdout[i] = stdout[i][12:]
 
 	stdout[0] += " " * (os.get_terminal_size().columns - len(stdout[0]))  
-	stdout[0] = colored(stdout[0], "blue", attrs=['reverse', 'blink'])
+	stdout[0] = colored(stdout[0], "blue", attrs=['reverse'])
 
 	stdout = "\n".join(stdout)
 
 	tui.setVar("jobs", stdout)
 	tui.setVar("update", datetime.now().strftime("%d/%m/%Y %H:%M:%S"))
 	
 
@@ -93,15 +93,15 @@
 			color = 'yellow'
 		elif node > 50:
 			color = 'orange'
 
 		if node > 99:
 			node = 99
 
-		nodesLoadText += ' ' + colored('(%02d)' % node, color, attrs=['reverse', 'blink']) + ' '
+		nodesLoadText += ' ' + colored('(%02d)' % node, color, attrs=['reverse']) + ' '
 
 
 	nodesRamText = ""
 	for i in range(len(nodesRam)):
 		node = int(nodesRam[i] / nodestotalRAM[i] * 100)
 
 		color = 'green'
@@ -111,15 +111,15 @@
 			color = 'yellow'
 		elif node > 50:
 			color = 'orange'
 
 		if node > 99:
 			node = 99
 
-		nodesRamText += ' ' + colored('(%02d)' % node, color, attrs=['reverse', 'blink']) + ' '
+		nodesRamText += ' ' + colored('(%02d)' % node, color, attrs=['reverse']) + ' '
 
 	tui.setVar("nodesCpus", nodesLoadText)
 	tui.setVar("load", progressbar(loadSum, count * 100, '%', size=30))
 	tui.setVar("usedRAM", progressbar(ramSum, totalRAM, 'M', size=30))
 	tui.setVar("nodesRams", nodesRamText)
 	tui.setVar("nodes", count)
 
@@ -159,8 +159,8 @@
 tui.addTextLine("%nodesRams%")
 tui.addTextLine("")
 tui.addTextLine("%jobs%")
 
 while True:
 	updateData()
 	slurmGet()
-	tui.update()
+	tui.update()
```

### Comparing `shtop-0.0.1/setup.py` & `shtop-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'Simple tui slurm job viewer.'
 LONG_DESCRIPTION = 'Simple tui slurm job viewer. Using /etc/hosts and ssh to get CPU and RAM utilization of all cluster nodes. Distrubuted using PIP and writen in python.'
 
 # Setting up
 setup(
         name="shtop", 
         version=VERSION,
@@ -19,8 +19,8 @@
 
         keywords=['python', 'slurm', 'shtop', 'top', 'htop'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 3"
         ]
-)
+)
```

### Comparing `shtop-0.0.1/shtop/tui.py` & `shtop-0.0.2/shtop/tui.py`

 * *Files identical despite different names*

### Comparing `shtop-0.0.1/shtop.egg-info/PKG-INFO` & `shtop-0.0.2/shtop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: shtop
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple tui slurm job viewer.
 Home-page: UNKNOWN
 Author: Lukáš Plevač
 Author-email: <lukas@plevac.eu>
 License: UNKNOWN
 Description: Simple tui slurm job viewer. Using /etc/hosts and ssh to get CPU and RAM utilization of all cluster nodes. Distrubuted using PIP and writen in python.
 Keywords: python,slurm,shtop,top,htop
```

