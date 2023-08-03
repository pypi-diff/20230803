# Comparing `tmp/Widget_Controller-2.0.1.tar.gz` & `tmp/Widget_Controller-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Widget Controller-2.0.1.tar", last modified: Tue Jul 25 03:16:09 2023, max compression
+gzip compressed data, was "Widget_Controller-2.0.2.tar", last modified: Thu Aug  3 03:57:30 2023, max compression
```

## Comparing `Widget_Controller-2.0.1.tar` & `Widget_Controller-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 03:16:09.074127 Widget Controller-2.0.1/
--rw-rw-rw-   0        0        0     2238 2023-06-12 17:07:48.000000 Widget Controller-2.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4063 2023-07-25 03:16:09.074127 Widget Controller-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3551 2023-06-29 02:47:43.000000 Widget Controller-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 03:16:09.002124 Widget Controller-2.0.1/WC/
--rw-rw-rw-   0        0        0    14920 2023-07-24 21:48:00.000000 Widget Controller-2.0.1/WC/WC.py
--rw-rw-rw-   0        0        0       19 2023-07-25 02:48:03.000000 Widget Controller-2.0.1/WC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 03:16:09.066238 Widget Controller-2.0.1/Widget_Controller.egg-info/
--rw-rw-rw-   0        0        0     4063 2023-07-25 03:16:08.000000 Widget Controller-2.0.1/Widget_Controller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-25 03:16:08.000000 Widget Controller-2.0.1/Widget_Controller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 03:16:08.000000 Widget Controller-2.0.1/Widget_Controller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-07-25 03:16:08.000000 Widget Controller-2.0.1/Widget_Controller.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 03:16:09.074127 Widget Controller-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      689 2023-07-25 03:15:53.000000 Widget Controller-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:57:30.802587 Widget_Controller-2.0.2/
+drwxrwxrwx   0        0        0        0 2023-08-03 03:57:30.516976 Widget_Controller-2.0.2/BUILD 2/
+drwxrwxrwx   0        0        0        0 2023-08-03 03:57:30.771172 Widget_Controller-2.0.2/BUILD 2/WC/
+-rw-rw-rw-   0        0        0    14924 2023-08-03 03:29:58.000000 Widget_Controller-2.0.2/BUILD 2/WC/WC.py
+-rw-rw-rw-   0        0        0       19 2023-08-03 03:24:46.000000 Widget_Controller-2.0.2/BUILD 2/WC/__init__.py
+-rw-rw-rw-   0        0        0     2222 2023-08-03 03:53:38.000000 Widget_Controller-2.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     6962 2023-08-03 03:57:30.801074 Widget_Controller-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4085 2023-08-03 03:46:53.000000 Widget_Controller-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 03:57:30.797638 Widget_Controller-2.0.2/Widget_Controller.egg-info/
+-rw-rw-rw-   0        0        0     6962 2023-08-03 03:57:29.000000 Widget_Controller-2.0.2/Widget_Controller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-08-03 03:57:29.000000 Widget_Controller-2.0.2/Widget_Controller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 03:57:29.000000 Widget_Controller-2.0.2/Widget_Controller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-03 03:57:29.000000 Widget_Controller-2.0.2/Widget_Controller.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 03:57:30.803601 Widget_Controller-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-08-03 03:57:26.000000 Widget_Controller-2.0.2/setup.py
```

### Comparing `Widget Controller-2.0.1/LICENSE.txt` & `Widget_Controller-2.0.2/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Para Z3R0_GT || Z3R0GT  Licencia de Software - Version 0.4 - Junio 12 - 2023
+Para Z3R0_GT - Z3R0GT  Licencia de Software - Version 0.4 - Junio 12 - 2023
 
-Contacto: contac.es.z3r0.gt@gmail.com
+Contacto de gmail: contac.es.z3r0.gt
 
 Por la presente se otorga permiso, sin cargo, a cualquier persona, excepto a organizaciones (compañias), obtener una copia del software y la documentación adjunta cubiertos por esta licencia (el "Software")
 para usar, mostrar, ejecutar y transmitir el Software, se debe cumplir las siguientes condiciones:
 
-   1. el uso del código fuente presente en este Software no puede ser replicado por ningún razón, a excepción de la version 1.0 (escrito en el lenguaje de python) que puede ser utilizado por una autorización directa o por escrito del creador de este Software (las bibliotecas presentes en el código de caracter externo, no son propiedad del autor).
+   1. el uso del codigo fuente presente en este Software no puede ser replicado por ningun razon, a excepción de la version 1.0 (escrito en el lenguaje de python) que puede ser utilizado por una autorización directa o por escrito del creador de este Software (las bibliotecas presentes en el codigo de caracter externo, no son propiedad del autor).
  
-   2. El uso del código solo debe ser para proyecto personales, mas no para aplicaciones de tipo comercial o empresarial, siendo el caso, la entidad (organicaciones, empresas....) deben de incluir en su acuerdo o en su defecto los creditos de dicho proyecto una acreditación que este Software se empleo para su creación en conjunto con el autor de este, a si mismo notificar a este mismo el uso este Software.
+   2. El uso del codigo solo debe ser para proyecto personales, mas no para aplicaciones de tipo comercial o empresarial, siendo el caso, la entidad (organicaciones, empresas....) deben de incluir en su acuerdo o en su defecto los creditos de dicho proyecto una acreditación que este Software se empleo para su creación en conjunto con el autor de este, a si mismo notificar a este mismo el uso este Software.
 
    3. Las versiones presentes, sin importar si estan bajo soporte o no, cuentan con el respaldo de esta licencia (a excepcion de los expuesto en el punto 1. ).
 
 Los avisos de derechos de autor en el Software y toda esta declaración, incluida la licencia anterior, esta restricción y el siguiente descargo de responsabilidad deben incluirse en todas las copias del Software, en su totalidad, y cualquier trabajo que utilice alguna version de este (a excepcion de lo expuesto en el punto 1.)
 
-EL SOFTWARE SE PROPORCIONA "TAL CUAL" SIN GARANTÍA DE NINGÚN TIPO, EXPRESA O IMPLÍCITA, INCLUYENDO PERO NO LIMITADO A GARANTÍAS DE COMERCIABILIDAD, IDONEIDAD PARA UN FIN DETERMINADO,
-TÍTULO Y NO INFRACCIÓN. EN NINGÚN CASO LOS TITULARES DE LOS DERECHOS DE AUTOR O CUALQUIER PERSONA QUE DISTRIBUYA EL SOFTWARE SERÁ RESPONSABLE DE CUALQUIER DAÑO U OTRA RESPONSABILIDAD, YA SEA POR CONTRATO, AGRAVIO O DE CUALQUIER OTRA FORMA, QUE SURJA O ESTÉ RELACIONADO CON EL SOFTWARE O EL USO O DE OTRO MODO TRATAMIENTOS EN EL SOFTWARE.
+EL SOFTWARE SE PROPORCIONA "TAL CUAL" SIN GARANTIA DE NINGUN TIPO, EXPRESA O IMPLICITA, INCLUYENDO PERO NO LIMITADO A GARANTIAS DE COMERCIABILIDAD, IDONEIDAD PARA UN FIN DETERMINADO,
+TITULO Y NO INFRACCION. EN NINGUN CASO LOS TITULARES DE LOS DERECHOS DE AUTOR O CUALQUIER PERSONA QUE DISTRIBUYA EL SOFTWARE SERA RESPONSABLE DE CUALQUIER DAÑO U OTRA RESPONSABILIDAD, YA SEA POR CONTRATO, AGRAVIO O DE CUALQUIER OTRA FORMA, QUE SURJA O ESTE RELACIONADO CON EL SOFTWARE O EL USO O DE OTRO MODO TRATAMIENTOS EN EL SOFTWARE.
```

### Comparing `Widget Controller-2.0.1/PKG-INFO` & `Widget_Controller-2.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,68 @@
-Metadata-Version: 2.1
-Name: Widget Controller
-Version: 2.0.1
-Summary: Una libreria para crear facilmente UI (traducido de Tkinter y otros)
-Home-page: https://github.com/Z3R0GT/WC
-Download-URL: https://github.com/Z3R0GT/WC/releases/tag/BUILD-2.0
-Author: Z3R0_GT
-Author-email: contac.es.z3r0.gt@gmail.com
-License: OTHER
-Keywords: ui,UI,Tkinter,logging,build
-Requires: Tk
-Requires: Pillow
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-![logo](logo.png)
-
 # WC
-Window Controller (controlador de ventanas) o WC es una libreria que empaqueta otras tanto grandes como pequeÃ±as, proveyendo multiples funciones para facilitar el crear GUIs, creado por
+***
+Window Controller (controlador de ventanas) o WC es una libreria que empaqueta otras tanto grandes como pequeñas, proveyendo multiples funciones para facilitar el crear GUIs, creado por
 Z3R0_GT con la iniciativa de "Facilitar el desarrollo de GUIs con python, sin perder mucho tiempo en el proceso con investigaciones para averiguar como lograrlo".
 
-tenemos la vision de ser una libreria usada por varias personas como compaÃ±iar para facilitarles el proceso, con el objetivo de ser lo mas simples posibles
+tenemos la vision de ser una libreria usada por varias personas para facilitarles el proceso del desarrollo, con el objetivo de ser lo mas simples posibles
+
+## INSLACIÓN
+***
+Usa el siguiente comando para poder instalar la libreria (actualmente alojada gracias a Pypi)
+
+pip install Widget-Controller
 
 ## LIBRERIAS
+***
 - Usamos las siguientes librerias externas (no viene pre-instalados con python):
     - Pillow.
     - tkVideoPlayer.
 
 - Pre-instalados:
     - os.
     - json.
     - winsound
 
-# Â¿QUE OFRECEMOS?
-
-- Usamos un tipeado similar a java para crear GUIs basicas, teniendo las siguientes funciones:
+# ¿QUE OFRECEMOS?
+***
+- Usamos un tipeado quizas similar a java para crear GUIs basicas, teniendo las siguientes funciones:
     - Inicio de aplicacion para correr mutiples ventanas como un solo proceso
     - Nodos:
-        - Botones, Areas de texto, etiquetas tanto para incluir imagenes adaptables como texto corriente, areas especificas para incluir entrada de usuario, menu de opciones, lista de botones.
+        - Botones, areas de texto, Etiquetas tanto para incluir imagenes adaptables como texto corriente, areas especificas para incluir entrada de usuario, menu de opciones, lista de botones.
     - Procesos:
-        - Puedes crear fuentes de texto (todas provenientes de tkinter), editar areas de texto, crear ventanas (necesario para ejecucion de programa), centrar ventanas, incluir barra de movimiento (scroll).
+        - Puedes crear fuentes de texto (todas provenientes de tkinter), Editar areas de texto, crear ventanas (necesario para ejecución de programa), centrar ventanas, incluir barra de movimiento (scroll).
     - Sistema:
-        - guardar y cargar archivos json (se usa diccionarios para este caso).
-    - ConfiguraciÃ³n:
+        - guardar y cargar archivos json (se usa diccionarios para este caso), la carga de videos, imagenes e otros, todo guardados para solo servir como llamada.
         - crear y almacenar direcciones para su posterior uso.
     - Desarrollador:
-        - puedas tambien revisar un listado de objetos en general, tanto datos almacenados, funciones y ventana creadas y objetos guardados en general.
+        - puedas tambien revisar un listado de objetos en general, tanto datos almacenados, funciones y ventana creadas y objetos guardados dentro de la libreria.
 
-dentro de cada carpeta, se encuentra la version correspondiente a WC con un pequeÃ±o ejemplo para que puedas testear las capacidades de la version elegida, tambiÃ©n es compatible (Version 4) para usarlo con consola
+dentro de cada carpeta, se encuentra la version correspondiente a WC con un pequeño ejemplo para que puedas testear las capacidades de la version elegida, tambien es compatible (Version 4) para usarlo con consola.
 
 # VERSIONES
-Numero de versiÃ³n que resive o no soporte, ademas del tiempo de experaciÃ³n de soporte.
+***
+Numero de version que resibe o no soporte, ademas del tiempo de experación de soporte.
 
-| Version    | Soporte                       | Cotenido               |
-| -------    | ------------------            | ---------              |
-| 5.0 > ...  | :white_check_mark:            |VersiÃ³n de MP3 Y MP4    |
-| 4.0 > 4.9  | :white_check_mark:            |Carga pantalla          |
-| 1.0 > 2.0  | :negative_squared_cross_mark: |Base de libreria        |
-
-Las versiones se aplicaran bajo el siguiente condicionamiento para identificar y tener la capacidad de leer:
---(Nombre de contrucciÃ³n) (Version numerica de lanamizamiento).(NÃºmero de revisiÃ³n actulizado)--, por ejemplo: 
-
-BUILD 3.2   -- en este caso se puede que la versiÃ³n a tratar es la BUILD de version 3 cuya revisiÃ³n de codigo corresponde a la segunda vez desde que se lanzo, sin embargo en caso de encontrar un tercer numero como en este caso: 
-BUILD 5.0.1 -- se puede intertrepar que la BUILD esta en su versiÃ³n 5 que no se a revisado desde que se lanzo pero es la primera versiÃ³n pre-liminar para lanzar una revisiÃ³n pronto (el tercer numero).
+| Version    | Soporte                       | Cotenido                 |
+| -------    | ------------------            | ---------                |
+| 6.0 > ...  |  X                            |aun en pruebas  25/07/2023|
+| 5.0 > 6.0  |  Y                            |Version de MP3 Y MP4      |
+| 4.0 > 4.9  |  Y                            |Carga pantalla            |
+| 1.0 > 2.0  |  X                            |Base de librería          |
+
+Las versiones se aplicarán bajo el siguiente condicionamiento para identificar y tener la capacidad de leer:
+--(Nombre de contrucción) (Version numerica de lanzamiento).(Número de revision actulizado)--, por ejemplo: 
+
+BUILD 3.2   -- en este caso se puede decir, que la version a tratar es la BUILD cuya version 3, la revisión de codigo corresponde a la segunda vez desde que se lanzó. 
+Sin embargo en caso de encontrar un tercer numero como en este caso: 
+BUILD 5.0.1 -- se puede interpretar que la BUILD esta en su version 5, no se a revisado desde que se lanzó pero es la primera version pre-liminar para lanzar una revisión pronto (el tercer numero).
 
 ## Notas
+***
+1. Soporte implica solución de errores, mas no significa actualización, si quiere una version con mas funciones mira las versiones presentes y sus respectivos datos.
 
-1. Soporte implica soluciÃ³n de errores, mÃ¡s no significa actualizaciÃ³n, si quiere una version con mas funciones mira las versiones presentes y sus respectivos datos.
-
-2. no somos dueÃ±os de ninguna libreria usada en este proyecto, en caso obtenga algun error, puede reportarlo o consultar en la paginÃ¡ de GitHub (https://github.com/Z3R0GT/WC/issues).
+2. no somos dueños de ninguna libreria externa (expuesto en "LIBRERIAS") usada en este proyecto, en caso obtenga algun error de estas, puede reportarlo a la misma o consultar en la pgina de GitHub (https://github.com/Z3R0GT/WC/issues).
 
+3. las librerias que aparecen en [ LIBRERIAS](#librerias) pueden llegar a pertenecer a la ultima version sea que se halla publicado o aun se este trabajando en ella
 ## Capturas
-
-<img src="https://github.com/Z3R0GT/WC/blob/main/Screenshot/ExampleCode.png">
+***
+<img src="https://github.com/Z3R0GT/WC/blob/main/Screenshot/ExampleCode.png">
```

### Comparing `Widget Controller-2.0.1/WC/WC.py` & `Widget_Controller-2.0.2/BUILD 2/WC/WC.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import json
 
 from tkinter import Text, Label, Entry, StringVar, Scrollbar, Listbox, Button,  OptionMenu
 from tkinter.font import Font
 from PIL import Image, ImageTk
 
 ## ---------Constant of Lib---------##
-LIB_VERSION = 2.0
+LIB_VERSION = "2.0.2"
 CURRENT_WINDOW = ["CONTINUE"]
 
 _ClassNodes__ITEM_SELECT = []
 __DIR_FOLDER = None
 __ITEM_CHOICE = None
 ID = 1
```

