# Comparing `tmp/name-of-thrones-0.2.7.tar.gz` & `tmp/name-of-thrones-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/name-of-thrones-0.2.7.tar", last modified: Fri Mar  4 21:28:54 2016, max compression
+gzip compressed data, was "name-of-thrones-0.2.8.tar", last modified: Thu Aug  3 11:42:15 2023, max compression
```

## Comparing `name-of-thrones-0.2.7.tar` & `name-of-thrones-0.2.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 matt      (1000) users      (100)        0 2016-03-04 21:28:54.000000 name-of-thrones-0.2.7/
-drwxr-xr-x   0 matt      (1000) users      (100)        0 2016-03-04 21:28:54.000000 name-of-thrones-0.2.7/game_of_thrones/
--rw-r--r--   0 matt      (1000) users      (100)     5049 2016-03-04 21:27:10.000000 name-of-thrones-0.2.7/game_of_thrones/__init__.py
--rw-r--r--   0 matt      (1000) users      (100)     2067 2016-03-04 21:25:09.000000 name-of-thrones-0.2.7/game_of_thrones/main.py
-drwxr-xr-x   0 matt      (1000) users      (100)        0 2016-03-04 21:28:54.000000 name-of-thrones-0.2.7/name_of_thrones.egg-info/
--rw-r--r--   0 matt      (1000) users      (100)     3212 2016-03-04 21:28:54.000000 name-of-thrones-0.2.7/name_of_thrones.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) users      (100)      307 2016-03-04 21:28:54.000000 name-of-thrones-0.2.7/name_of_thrones.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) users      (100)        1 2016-03-04 21:28:54.000000 name-of-thrones-0.2.7/name_of_thrones.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) users      (100)       63 2016-03-04 21:28:54.000000 name-of-thrones-0.2.7/name_of_thrones.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) users      (100)       30 2016-03-04 21:28:54.000000 name-of-thrones-0.2.7/name_of_thrones.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) users      (100)       16 2016-03-04 21:28:54.000000 name-of-thrones-0.2.7/name_of_thrones.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) users      (100)     1820 2016-03-04 21:26:30.000000 name-of-thrones-0.2.7/README.rst
--rw-r--r--   0 matt      (1000) users      (100)     1468 2015-08-28 08:12:27.000000 name-of-thrones-0.2.7/setup.py
--rw-r--r--   0 matt      (1000) users      (100)     3212 2016-03-04 21:28:54.000000 name-of-thrones-0.2.7/PKG-INFO
--rw-r--r--   0 matt      (1000) users      (100)       59 2016-03-04 21:28:54.000000 name-of-thrones-0.2.7/setup.cfg
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-03 11:42:15.012932 name-of-thrones-0.2.8/
+-rw-r--r--   0 matt      (1000) users      (985)      745 2023-08-03 11:07:45.000000 name-of-thrones-0.2.8/LICENCE
+-rw-r--r--   0 matt      (1000) users      (985)     2634 2023-08-03 11:42:15.012932 name-of-thrones-0.2.8/PKG-INFO
+-rw-r--r--   0 matt      (1000) users      (985)     1592 2023-08-03 11:31:49.000000 name-of-thrones-0.2.8/README.md
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-03 11:42:15.009599 name-of-thrones-0.2.8/game_of_thrones/
+-rw-r--r--   0 matt      (1000) users      (985)     5049 2023-08-03 11:38:38.000000 name-of-thrones-0.2.8/game_of_thrones/__init__.py
+-rw-r--r--   0 matt      (1000) users      (985)     2067 2016-03-04 21:25:09.000000 name-of-thrones-0.2.8/game_of_thrones/main.py
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-03 11:42:15.012932 name-of-thrones-0.2.8/name_of_thrones.egg-info/
+-rw-r--r--   0 matt      (1000) users      (985)     2634 2023-08-03 11:42:14.000000 name-of-thrones-0.2.8/name_of_thrones.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) users      (985)      314 2023-08-03 11:42:15.000000 name-of-thrones-0.2.8/name_of_thrones.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) users      (985)        1 2023-08-03 11:42:14.000000 name-of-thrones-0.2.8/name_of_thrones.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) users      (985)       62 2023-08-03 11:42:14.000000 name-of-thrones-0.2.8/name_of_thrones.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) users      (985)       30 2023-08-03 11:42:14.000000 name-of-thrones-0.2.8/name_of_thrones.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) users      (985)       16 2023-08-03 11:42:14.000000 name-of-thrones-0.2.8/name_of_thrones.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) users      (985)       38 2023-08-03 11:42:15.012932 name-of-thrones-0.2.8/setup.cfg
+-rw-r--r--   0 matt      (1000) users      (985)     1521 2023-08-03 11:42:03.000000 name-of-thrones-0.2.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `name-of-thrones-0.2.7/game_of_thrones/__init__.py` & `name-of-thrones-0.2.8/game_of_thrones/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
 Command line tool to generate words that sound like characters from Game of
 Thrones. Good for naming projects, servers and stray cats.
 """
 __author__ = 'Matt Deacalion Stevens'
-__version__ = '0.2.7'
+__version__ = '0.2.8'
 
 import random
 import string
 from itertools import islice
 from collections import defaultdict, deque
```

### Comparing `name-of-thrones-0.2.7/game_of_thrones/main.py` & `name-of-thrones-0.2.8/game_of_thrones/main.py`

 * *Files identical despite different names*

### Comparing `name-of-thrones-0.2.7/name_of_thrones.egg-info/PKG-INFO` & `name-of-thrones-0.2.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,73 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: name-of-thrones
-Version: 0.2.7
+Version: 0.2.8
 Summary: Command line tool to generate words that sound like characters from Game of Thrones. Good for naming projects, servers and stray cats.
-Home-page: http://dirtymonkey.co.uk/name-of-thrones
+Home-page: https://codeberg.org/Dokana/Name-of-Thrones
 Author: Matt Deacalion Stevens
 Author-email: matt@dirtymonkey.co.uk
 License: MIT
-Description: ===============
-        Name of Thrones
-        ===============
-        Command line tool to generate words that sound like characters from Game of Thrones. Useful for
-        unique project names, host names and the occasional stray cat.
-        
-        .. image:: https://raw.githubusercontent.com/Matt-Deacalion/Name-of-Thrones/master/screenshot.png
-            :alt: Name of Thrones screenshot
-        
-        Installation
-        ------------
-        You can install the *Name of Thrones* using pip:
-        
-        .. code-block:: bash
-        
-            $ pip install name-of-thrones
-        
-        Usage
-        -----
-        You can use the `name-of-thrones` command from the shell to run Name of Thrones::
-        
-            $ name-of-thrones --help
-        
-            Generate words that sound like characters from Game of Thrones.
-        
-            Usage:
-              name-of-thrones [--quantity=<number>] [--min=<length>] [--max=<length>]
-                              [--json] [--nocolour] [--alphabetical] [--length] [--reverse]
-              name-of-thrones (-h | --help | --version)
-        
-            Options:
-              --version                show program's version number and exit.
-              -h, --help               show this help message and exit.
-              -q, --quantity=<number>  the quantity of words to generate [default: 10].
-              --min=<length>           the minimum length of each word [default: 4].
-              --max=<length>           the maximum length of each word [default: 10].
-              -j, --json               output the words in JSON format.
-              -n, --nocolour           output the words without colourization.
-              -a, --alphabetical       output the words in alphabetical order.
-              -l, --length             output the words in order of their length.
-              -r, --reverse            reverse the order of the words.
-        
-        License
-        -------
-        Copyright © 2016 `Matt Deacalion Stevens`_, released under The `MIT License`_.
-        
-        .. _Matt Deacalion Stevens: http://dirtymonkey.co.uk
-        .. _MIT License: http://deacalion.mit-license.org
-        
 Keywords: game of thrones naming namer project tools
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# Name of Thrones
+
+Command line tool to generate words that sound like characters from Game of
+Thrones. Useful for unique project names, host names and the occasional stray
+cat.
+
+![Name of Thrones screenshot](screenshot.png)
+
+
+## Installation
+
+You can install the **Name of Thrones** using pip:
+
+```console
+    $ pip install name-of-thrones
+```
+
+
+## Usage
+
+You can use the `name-of-thrones` command from the shell to run Name of Thrones:
+
+```console
+    $ name-of-thrones --help
+    Generate words that sound like characters from Game of Thrones.
+
+    Usage:
+      name-of-thrones [--quantity=<number>] [--min=<length>] [--max=<length>]
+                      [--json] [--nocolour] [--alphabetical] [--length] [--reverse]
+      name-of-thrones (-h | --help | --version)
+
+    Options:
+      --version                show program's version number and exit.
+      -h, --help               show this help message and exit.
+      -q, --quantity=<number>  the quantity of words to generate [default: 10].
+      --min=<length>           the minimum length of each word [default: 4].
+      --max=<length>           the maximum length of each word [default: 10].
+      -j, --json               output the words in JSON format.
+      -n, --nocolour           output the words without colourization.
+      -a, --alphabetical       output the words in alphabetical order.
+      -l, --length             output the words in order of their length.
+      -r, --reverse            reverse the order of the words.
+```
+
+
+## Licence
+
+Copyright © 2023 Matthew Stevens, released under the [ISC Licence](LICENCE).
```

### Comparing `name-of-thrones-0.2.7/README.rst` & `name-of-thrones-0.2.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-===============
-Name of Thrones
-===============
-Command line tool to generate words that sound like characters from Game of Thrones. Useful for
-unique project names, host names and the occasional stray cat.
-
-.. image:: https://raw.githubusercontent.com/Matt-Deacalion/Name-of-Thrones/master/screenshot.png
-    :alt: Name of Thrones screenshot
-
-Installation
-------------
-You can install the *Name of Thrones* using pip:
+# Name of Thrones
 
-.. code-block:: bash
+Command line tool to generate words that sound like characters from Game of
+Thrones. Useful for unique project names, host names and the occasional stray
+cat.
 
+![Name of Thrones screenshot](screenshot.png)
+
+
+## Installation
+
+You can install the **Name of Thrones** using pip:
+
+```console
     $ pip install name-of-thrones
+```
 
-Usage
------
-You can use the `name-of-thrones` command from the shell to run Name of Thrones::
 
-    $ name-of-thrones --help
+## Usage
+
+You can use the `name-of-thrones` command from the shell to run Name of Thrones:
 
+```console
+    $ name-of-thrones --help
     Generate words that sound like characters from Game of Thrones.
 
     Usage:
       name-of-thrones [--quantity=<number>] [--min=<length>] [--max=<length>]
                       [--json] [--nocolour] [--alphabetical] [--length] [--reverse]
       name-of-thrones (-h | --help | --version)
 
@@ -35,14 +36,13 @@
       --min=<length>           the minimum length of each word [default: 4].
       --max=<length>           the maximum length of each word [default: 10].
       -j, --json               output the words in JSON format.
       -n, --nocolour           output the words without colourization.
       -a, --alphabetical       output the words in alphabetical order.
       -l, --length             output the words in order of their length.
       -r, --reverse            reverse the order of the words.
+```
+
 
-License
--------
-Copyright © 2016 `Matt Deacalion Stevens`_, released under The `MIT License`_.
+## Licence
 
-.. _Matt Deacalion Stevens: http://dirtymonkey.co.uk
-.. _MIT License: http://deacalion.mit-license.org
+Copyright © 2023 Matthew Stevens, released under the [ISC Licence](LICENCE).
```

### Comparing `name-of-thrones-0.2.7/setup.py` & `name-of-thrones-0.2.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup
 
 import game_of_thrones
 
 setup(
     name='name-of-thrones',
     version=game_of_thrones.__version__.strip(),
-    url='http://dirtymonkey.co.uk/name-of-thrones',
+    url='https://codeberg.org/Dokana/Name-of-Thrones',
     license='MIT',
     author=game_of_thrones.__author__.strip(),
     author_email='matt@dirtymonkey.co.uk',
     description=game_of_thrones.__doc__.strip().replace('\n', ' '),
-    long_description=open('README.rst').read(),
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     keywords='game of thrones naming namer project tools',
     packages=['game_of_thrones'],
     include_package_data=True,
     test_suite='tests',
     entry_points={
         'console_scripts': [
             'name-of-thrones = game_of_thrones.main:main',
```

### Comparing `name-of-thrones-0.2.7/PKG-INFO` & `name-of-thrones-0.2.8/name_of_thrones.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,73 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: name-of-thrones
-Version: 0.2.7
+Version: 0.2.8
 Summary: Command line tool to generate words that sound like characters from Game of Thrones. Good for naming projects, servers and stray cats.
-Home-page: http://dirtymonkey.co.uk/name-of-thrones
+Home-page: https://codeberg.org/Dokana/Name-of-Thrones
 Author: Matt Deacalion Stevens
 Author-email: matt@dirtymonkey.co.uk
 License: MIT
-Description: ===============
-        Name of Thrones
-        ===============
-        Command line tool to generate words that sound like characters from Game of Thrones. Useful for
-        unique project names, host names and the occasional stray cat.
-        
-        .. image:: https://raw.githubusercontent.com/Matt-Deacalion/Name-of-Thrones/master/screenshot.png
-            :alt: Name of Thrones screenshot
-        
-        Installation
-        ------------
-        You can install the *Name of Thrones* using pip:
-        
-        .. code-block:: bash
-        
-            $ pip install name-of-thrones
-        
-        Usage
-        -----
-        You can use the `name-of-thrones` command from the shell to run Name of Thrones::
-        
-            $ name-of-thrones --help
-        
-            Generate words that sound like characters from Game of Thrones.
-        
-            Usage:
-              name-of-thrones [--quantity=<number>] [--min=<length>] [--max=<length>]
-                              [--json] [--nocolour] [--alphabetical] [--length] [--reverse]
-              name-of-thrones (-h | --help | --version)
-        
-            Options:
-              --version                show program's version number and exit.
-              -h, --help               show this help message and exit.
-              -q, --quantity=<number>  the quantity of words to generate [default: 10].
-              --min=<length>           the minimum length of each word [default: 4].
-              --max=<length>           the maximum length of each word [default: 10].
-              -j, --json               output the words in JSON format.
-              -n, --nocolour           output the words without colourization.
-              -a, --alphabetical       output the words in alphabetical order.
-              -l, --length             output the words in order of their length.
-              -r, --reverse            reverse the order of the words.
-        
-        License
-        -------
-        Copyright © 2016 `Matt Deacalion Stevens`_, released under The `MIT License`_.
-        
-        .. _Matt Deacalion Stevens: http://dirtymonkey.co.uk
-        .. _MIT License: http://deacalion.mit-license.org
-        
 Keywords: game of thrones naming namer project tools
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# Name of Thrones
+
+Command line tool to generate words that sound like characters from Game of
+Thrones. Useful for unique project names, host names and the occasional stray
+cat.
+
+![Name of Thrones screenshot](screenshot.png)
+
+
+## Installation
+
+You can install the **Name of Thrones** using pip:
+
+```console
+    $ pip install name-of-thrones
+```
+
+
+## Usage
+
+You can use the `name-of-thrones` command from the shell to run Name of Thrones:
+
+```console
+    $ name-of-thrones --help
+    Generate words that sound like characters from Game of Thrones.
+
+    Usage:
+      name-of-thrones [--quantity=<number>] [--min=<length>] [--max=<length>]
+                      [--json] [--nocolour] [--alphabetical] [--length] [--reverse]
+      name-of-thrones (-h | --help | --version)
+
+    Options:
+      --version                show program's version number and exit.
+      -h, --help               show this help message and exit.
+      -q, --quantity=<number>  the quantity of words to generate [default: 10].
+      --min=<length>           the minimum length of each word [default: 4].
+      --max=<length>           the maximum length of each word [default: 10].
+      -j, --json               output the words in JSON format.
+      -n, --nocolour           output the words without colourization.
+      -a, --alphabetical       output the words in alphabetical order.
+      -l, --length             output the words in order of their length.
+      -r, --reverse            reverse the order of the words.
+```
+
+
+## Licence
+
+Copyright © 2023 Matthew Stevens, released under the [ISC Licence](LICENCE).
```

