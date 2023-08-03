# Comparing `tmp/LagRochePlot-1.1.3.tar.gz` & `tmp/LagRochePlot-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LagRochePlot-1.1.3.tar", last modified: Thu Aug  3 02:05:57 2023, max compression
+gzip compressed data, was "LagRochePlot-1.2.0.tar", last modified: Thu Aug  3 19:47:27 2023, max compression
```

## Comparing `LagRochePlot-1.1.3.tar` & `LagRochePlot-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 02:05:57.958554 LagRochePlot-1.1.3/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       77 2023-08-03 01:12:03.000000 LagRochePlot-1.1.3/.gitignore
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1073 2023-08-01 19:12:17.000000 LagRochePlot-1.1.3/LICENSE
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 02:05:57.954554 LagRochePlot-1.1.3/LagRochePlot/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8428 2023-08-03 01:06:39.000000 LagRochePlot-1.1.3/LagRochePlot/LagRoche.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-08-01 19:12:17.000000 LagRochePlot-1.1.3/LagRochePlot/__init__.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 02:05:57.954554 LagRochePlot-1.1.3/LagRochePlot.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4228 2023-08-03 02:05:57.000000 LagRochePlot-1.1.3/LagRochePlot.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      281 2023-08-03 02:05:57.000000 LagRochePlot-1.1.3/LagRochePlot.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-08-03 02:05:57.000000 LagRochePlot-1.1.3/LagRochePlot.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       29 2023-08-03 02:05:57.000000 LagRochePlot-1.1.3/LagRochePlot.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       13 2023-08-03 02:05:57.000000 LagRochePlot-1.1.3/LagRochePlot.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4228 2023-08-03 02:05:57.958554 LagRochePlot-1.1.3/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3892 2023-08-01 19:12:17.000000 LagRochePlot-1.1.3/README.md
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      122 2023-08-01 19:12:17.000000 LagRochePlot-1.1.3/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-08-03 02:05:57.958554 LagRochePlot-1.1.3/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      586 2023-08-03 01:06:22.000000 LagRochePlot-1.1.3/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 19:47:27.675531 LagRochePlot-1.2.0/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       77 2023-08-03 01:12:03.000000 LagRochePlot-1.2.0/.gitignore
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1073 2023-08-01 19:12:17.000000 LagRochePlot-1.2.0/LICENSE
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 19:47:27.671529 LagRochePlot-1.2.0/LagRochePlot/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8183 2023-08-03 19:44:01.000000 LagRochePlot-1.2.0/LagRochePlot/LagRoche.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-08-01 19:12:17.000000 LagRochePlot-1.2.0/LagRochePlot/__init__.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 19:47:27.671529 LagRochePlot-1.2.0/LagRochePlot.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4273 2023-08-03 19:47:27.000000 LagRochePlot-1.2.0/LagRochePlot.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      296 2023-08-03 19:47:27.000000 LagRochePlot-1.2.0/LagRochePlot.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-08-03 19:47:27.000000 LagRochePlot-1.2.0/LagRochePlot.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       29 2023-08-03 19:47:27.000000 LagRochePlot-1.2.0/LagRochePlot.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       13 2023-08-03 19:47:27.000000 LagRochePlot-1.2.0/LagRochePlot.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4273 2023-08-03 19:47:27.675531 LagRochePlot-1.2.0/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3918 2023-08-03 19:36:24.000000 LagRochePlot-1.2.0/README.md
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      122 2023-08-01 19:12:17.000000 LagRochePlot-1.2.0/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-08-03 19:47:27.675531 LagRochePlot-1.2.0/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2023-08-03 19:33:58.000000 LagRochePlot-1.2.0/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 19:47:27.675531 LagRochePlot-1.2.0/tests/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      372 2023-08-03 19:39:37.000000 LagRochePlot-1.2.0/tests/test1.py
```

### Comparing `LagRochePlot-1.1.3/LICENSE` & `LagRochePlot-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LagRochePlot-1.1.3/LagRochePlot/LagRoche.py` & `LagRochePlot-1.2.0/LagRochePlot/LagRoche.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,16 +137,7 @@
     def plot(self):
         '''
         Realiza el trazado inicial del gráfico.
         '''
         self.calculo()  # Calcula los valores iniciales para el trazado del gráfico
         self.update_plot(0)  # Actualiza el gráfico inicial
         plt.show()
-
-
-#Datos de ejemplo: (en un futuro debería ser el usuario el que ingrese estos valores)
-#Establecer en el input que m1 => m2
-#moon = 7.3477e22 #[Kg]
-#earth = 5.97219e24 #[Kg]
-#distance = 384399000/149597870700 #[AU]
-
-#Plot(earth,moon,distance)
```

### Comparing `LagRochePlot-1.1.3/LagRochePlot.egg-info/PKG-INFO` & `LagRochePlot-1.2.0/LagRochePlot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: LagRochePlot
-Version: 1.1.3
+Version: 1.2.0
 Summary: Herramienta gráfica para visualizar los puntos de Lagrange y potencial de Roche.
 Home-page: https://github.com/Thomas-thief/LagRochePlot
-Author: Thomas Salazar, Esteban Sanchez, Sebastian Lopez
+Author: Thomas Salazar, Esteban Sanchez, Sebastian Lopez, Andres Rumillanca
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Lagrange_points
 Project of software development
 
@@ -17,14 +17,15 @@
 
 
 #Dependencias para su funcionamiento:
 
 * Numpy(Version: >= 1.7)
 * Matpllotlib(Version >= 3.0.0)
 * PyAstronomy(Version = 0.20.0)
+* SciPy(Version = 1.11.1)
 
 #Como usar:(Example ejecution)
 
 NombredeClase(Masa1,Masa2,Distancia, opcional)
 
 * Parametros:
   * Masa1 (Float)= Masa del objeto más masivo, al tratarse de numeros grandes,en kilogramos. Se puede expresar como potencia de 10 con Numpy(Ej: 1e10)
```

### Comparing `LagRochePlot-1.1.3/PKG-INFO` & `LagRochePlot-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: LagRochePlot
-Version: 1.1.3
+Version: 1.2.0
 Summary: Herramienta gráfica para visualizar los puntos de Lagrange y potencial de Roche.
 Home-page: https://github.com/Thomas-thief/LagRochePlot
-Author: Thomas Salazar, Esteban Sanchez, Sebastian Lopez
+Author: Thomas Salazar, Esteban Sanchez, Sebastian Lopez, Andres Rumillanca
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Lagrange_points
 Project of software development
 
@@ -17,14 +17,15 @@
 
 
 #Dependencias para su funcionamiento:
 
 * Numpy(Version: >= 1.7)
 * Matpllotlib(Version >= 3.0.0)
 * PyAstronomy(Version = 0.20.0)
+* SciPy(Version = 1.11.1)
 
 #Como usar:(Example ejecution)
 
 NombredeClase(Masa1,Masa2,Distancia, opcional)
 
 * Parametros:
   * Masa1 (Float)= Masa del objeto más masivo, al tratarse de numeros grandes,en kilogramos. Se puede expresar como potencia de 10 con Numpy(Ej: 1e10)
```

### Comparing `LagRochePlot-1.1.3/README.md` & `LagRochePlot-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 #Dependencias para su funcionamiento:
 
 * Numpy(Version: >= 1.7)
 * Matpllotlib(Version >= 3.0.0)
 * PyAstronomy(Version = 0.20.0)
+* SciPy(Version = 1.11.1)
 
 #Como usar:(Example ejecution)
 
 NombredeClase(Masa1,Masa2,Distancia, opcional)
 
 * Parametros:
   * Masa1 (Float)= Masa del objeto más masivo, al tratarse de numeros grandes,en kilogramos. Se puede expresar como potencia de 10 con Numpy(Ej: 1e10)
```

