# Comparing `tmp/tempo120-0.8.0.tar.gz` & `tmp/tempo120-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\products\tempo120\github - Kopie\dist\.tmp-t31fwyc4\tempo120-0.8.0.tar", last modified: Wed Aug  2 18:59:15 2023, max compression
+gzip compressed data, was "D:\products\tempo120\github - Kopie\dist\.tmp-vimra197\tempo120-1.0.0.tar", last modified: Thu Aug  3 15:32:28 2023, max compression
```

## Comparing `tempo120-0.8.0.tar` & `tempo120-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 18:59:15.743493 tempo120-0.8.0/
--rw-rw-rw-   0        0        0    35149 2023-07-11 18:42:22.000000 tempo120-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     4802 2023-08-02 18:59:15.742493 tempo120-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     3789 2023-08-02 18:55:52.000000 tempo120-0.8.0/README.md
--rw-rw-rw-   0        0        0       42 2023-08-02 18:59:15.743493 tempo120-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1922 2023-08-02 17:44:32.000000 tempo120-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 18:59:15.741493 tempo120-0.8.0/tempo120.egg-info/
--rw-rw-rw-   0        0        0     4802 2023-08-02 18:59:15.000000 tempo120-0.8.0/tempo120.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-08-02 18:59:15.000000 tempo120-0.8.0/tempo120.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 18:59:15.000000 tempo120-0.8.0/tempo120.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-08-02 18:59:15.000000 tempo120-0.8.0/tempo120.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-08-02 18:59:15.000000 tempo120-0.8.0/tempo120.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17160 2023-08-02 17:46:18.000000 tempo120-0.8.0/tempo120.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:32:28.571536 tempo120-1.0.0/
+-rw-rw-rw-   0        0        0    35149 2023-07-11 18:42:22.000000 tempo120-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     4976 2023-08-03 15:32:28.570536 tempo120-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3955 2023-08-03 14:52:04.000000 tempo120-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 15:32:28.515523 tempo120-1.0.0/gfx/
+-rw-rw-rw-   0        0        0     6941 2023-07-08 15:23:15.000000 tempo120-1.0.0/gfx/car.png
+-rw-rw-rw-   0        0        0   107076 2023-07-08 20:36:33.000000 tempo120-1.0.0/gfx/screenshot1.png
+-rw-rw-rw-   0        0        0    29421 2023-07-08 20:36:19.000000 tempo120-1.0.0/gfx/screenshot2.png
+-rw-rw-rw-   0        0        0    17458 2023-07-08 20:36:06.000000 tempo120-1.0.0/gfx/screenshot3.png
+-rw-rw-rw-   0        0        0    16872 2023-07-08 20:35:55.000000 tempo120-1.0.0/gfx/screenshot4.png
+-rw-rw-rw-   0        0        0    85199 2023-07-08 19:53:15.000000 tempo120-1.0.0/gfx/title.png
+-rw-rw-rw-   0        0        0    30108 2023-08-02 17:31:30.000000 tempo120-1.0.0/gfx/track01.png
+drwxrwxrwx   0        0        0        0 2023-08-03 15:32:28.536529 tempo120-1.0.0/muzak/
+-rw-rw-rw-   0        0        0    16512 2023-07-23 13:45:55.000000 tempo120-1.0.0/muzak/engine.ogg
+-rw-rw-rw-   0        0        0  1955997 2023-07-08 18:57:12.000000 tempo120-1.0.0/muzak/track.ogg
+drwxrwxrwx   0        0        0        0 2023-08-03 15:32:28.563534 tempo120-1.0.0/scores/
+-rw-rw-rw-   0        0        0       55 2023-07-10 18:10:59.000000 tempo120-1.0.0/scores/scores.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 15:32:28.571536 tempo120-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2069 2023-08-03 15:13:18.000000 tempo120-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:32:28.570536 tempo120-1.0.0/tempo120.egg-info/
+-rw-rw-rw-   0        0        0     4976 2023-08-03 15:32:28.000000 tempo120-1.0.0/tempo120.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-08-03 15:32:28.000000 tempo120-1.0.0/tempo120.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 15:32:28.000000 tempo120-1.0.0/tempo120.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-08-03 15:32:28.000000 tempo120-1.0.0/tempo120.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-08-03 15:32:28.000000 tempo120-1.0.0/tempo120.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17472 2023-08-03 15:14:17.000000 tempo120-1.0.0/tempo120.py
```

### Comparing `tempo120-0.8.0/LICENSE` & `tempo120-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tempo120-0.8.0/PKG-INFO` & `tempo120-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tempo120
-Version: 0.8.0
+Version: 1.0.0
 Summary: A party car racing game
 Home-page: https://dkrajzew.itch.io/tempo120
 Download-URL: http://pypi.python.org/pypi/tempo120
 Author: dkrajzew
 Author-email: d.krajzewicz@gmail.com
-License: BSD
+License: GPLv3
 Project-URL: Source, https://github.com/dkrajzew/tempo120
 Project-URL: Tracker, https://github.com/dkrajzew/tempo120/issues
 Project-URL: Discussions, https://github.com/dkrajzew/tempo120/discussions
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,14 +27,16 @@
 [![PyPI version](https://badge.fury.io/py/tempo120.svg)](https://pypi.python.org/pypi/tempo120)
 [![Downloads](https://pepy.tech/badge/tempo120)](https://pepy.tech/project/tempo120)
 [![Downloads](https://static.pepy.tech/badge/tempo120/week)](https://pepy.tech/project/tempo120)
 
 
 A racing game written using Python/pygame during the [bpb](https://www.bpb.de/) ([Bundeszentrale für politische Bildung](https://www.bpb.de/)) [game jam 2023](https://www.bpb.de/veranstaltungen/veranstaltungskalender/518950/bpb-game-jam-2023/). The game jam's topic was mobility.
 
+<img src="./gfx/screenshot1.png" width="40%"/> <img src="./gfx/screenshot3.png" width="40%"/>
+
 You may download an executable version on [itch.io](https://dkrajzew.itch.io/tempo120).
 
 # About
 
 __Tempo120__ is a very simple car racing game. You may control your vehicle using the cursor keys or WASD.
 
 The higher the speed the more difficult it is to control the vehicle. You do not need to accelerate all the time. The speed stays same unless you brake or drive besides the road.
@@ -87,14 +89,18 @@
 * some kind of an integration of further tracks
 * multiplayer mode
 
 I like the game and may port it to c++ once.
 
 # Change Log
 
+## v1.0.0 (03.08.2023)
+
+* adding missing assets to the Python release
+
 ## v0.8.0 (02.08.2023)
 
 * included track debugging from [MapleMonarch](https://maplemonarch.itch.io/)
 * added a setup script, you may now download the current release from [PyPi](https://pypi.org/project/degrotesque/)
 
 ## v0.6.0 (23.07.2023)
```

### Comparing `tempo120-0.8.0/README.md` & `tempo120-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 [![PyPI version](https://badge.fury.io/py/tempo120.svg)](https://pypi.python.org/pypi/tempo120)
 [![Downloads](https://pepy.tech/badge/tempo120)](https://pepy.tech/project/tempo120)
 [![Downloads](https://static.pepy.tech/badge/tempo120/week)](https://pepy.tech/project/tempo120)
 
 
 A racing game written using Python/pygame during the [bpb](https://www.bpb.de/) ([Bundeszentrale für politische Bildung](https://www.bpb.de/)) [game jam 2023](https://www.bpb.de/veranstaltungen/veranstaltungskalender/518950/bpb-game-jam-2023/). The game jam's topic was mobility.
 
+<img src="./gfx/screenshot1.png" width="40%"/> <img src="./gfx/screenshot3.png" width="40%"/>
+
 You may download an executable version on [itch.io](https://dkrajzew.itch.io/tempo120).
 
 # About
 
 __Tempo120__ is a very simple car racing game. You may control your vehicle using the cursor keys or WASD.
 
 The higher the speed the more difficult it is to control the vehicle. You do not need to accelerate all the time. The speed stays same unless you brake or drive besides the road.
@@ -64,14 +66,18 @@
 * some kind of an integration of further tracks
 * multiplayer mode
 
 I like the game and may port it to c++ once.
 
 # Change Log
 
+## v1.0.0 (03.08.2023)
+
+* adding missing assets to the Python release
+
 ## v0.8.0 (02.08.2023)
 
 * included track debugging from [MapleMonarch](https://maplemonarch.itch.io/)
 * added a setup script, you may now download the current release from [PyPi](https://pypi.org/project/degrotesque/)
 
 ## v0.6.0 (23.07.2023)
```

### Comparing `tempo120-0.8.0/setup.py` & `tempo120-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,30 +20,36 @@
 
 # --- definitions ---------------------------------------------------
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tempo120",
-    version="0.8.0",
+    version="1.0.0",
     author="dkrajzew",
     author_email="d.krajzewicz@gmail.com",
     description="A party car racing game",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://dkrajzew.itch.io/tempo120',
     download_url='http://pypi.python.org/pypi/tempo120',
     project_urls={
         'Source': 'https://github.com/dkrajzew/tempo120',
         'Tracker': 'https://github.com/dkrajzew/tempo120/issues',
         'Discussions': 'https://github.com/dkrajzew/tempo120/discussions',
     },
-    license='BSD',
+    license='GPLv3',
     # add modules
     py_modules = ['tempo120'],
+    packages = ['gfx','muzak','scores'],
+    package_data = {
+        'gfx': ['*'],
+        'muzak': ['*'],
+        'scores': ['*']
+    },
     entry_points = {
         'console_scripts': [
             'tempo120 = tempo120:main'
         ]
     },
     # see https://pypi.org/classifiers/
     classifiers=[
```

### Comparing `tempo120-0.8.0/tempo120.egg-info/PKG-INFO` & `tempo120-1.0.0/tempo120.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tempo120
-Version: 0.8.0
+Version: 1.0.0
 Summary: A party car racing game
 Home-page: https://dkrajzew.itch.io/tempo120
 Download-URL: http://pypi.python.org/pypi/tempo120
 Author: dkrajzew
 Author-email: d.krajzewicz@gmail.com
-License: BSD
+License: GPLv3
 Project-URL: Source, https://github.com/dkrajzew/tempo120
 Project-URL: Tracker, https://github.com/dkrajzew/tempo120/issues
 Project-URL: Discussions, https://github.com/dkrajzew/tempo120/discussions
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,14 +27,16 @@
 [![PyPI version](https://badge.fury.io/py/tempo120.svg)](https://pypi.python.org/pypi/tempo120)
 [![Downloads](https://pepy.tech/badge/tempo120)](https://pepy.tech/project/tempo120)
 [![Downloads](https://static.pepy.tech/badge/tempo120/week)](https://pepy.tech/project/tempo120)
 
 
 A racing game written using Python/pygame during the [bpb](https://www.bpb.de/) ([Bundeszentrale für politische Bildung](https://www.bpb.de/)) [game jam 2023](https://www.bpb.de/veranstaltungen/veranstaltungskalender/518950/bpb-game-jam-2023/). The game jam's topic was mobility.
 
+<img src="./gfx/screenshot1.png" width="40%"/> <img src="./gfx/screenshot3.png" width="40%"/>
+
 You may download an executable version on [itch.io](https://dkrajzew.itch.io/tempo120).
 
 # About
 
 __Tempo120__ is a very simple car racing game. You may control your vehicle using the cursor keys or WASD.
 
 The higher the speed the more difficult it is to control the vehicle. You do not need to accelerate all the time. The speed stays same unless you brake or drive besides the road.
@@ -87,14 +89,18 @@
 * some kind of an integration of further tracks
 * multiplayer mode
 
 I like the game and may port it to c++ once.
 
 # Change Log
 
+## v1.0.0 (03.08.2023)
+
+* adding missing assets to the Python release
+
 ## v0.8.0 (02.08.2023)
 
 * included track debugging from [MapleMonarch](https://maplemonarch.itch.io/)
 * added a setup script, you may now download the current release from [PyPi](https://pypi.org/project/degrotesque/)
 
 ## v0.6.0 (23.07.2023)
```

### Comparing `tempo120-0.8.0/tempo120.py` & `tempo120-1.0.0/tempo120.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,27 +95,27 @@
         """Loads the scores.
         
         Loads scores from "scores.txt", sorts them by the needed time and prunes
         them to the maximum length of 15 entries.
         """
         scores = []
         try:
-            with open("scores.txt") as fd:
+            with open(os.path.join(os.path.dirname(__file__), "scores", "scores.txt")) as fd:
                 for l in fd:
                     name, t = l.strip().split("\t")
                     scores.append([name, int(t)])
             scores.sort(key=lambda x: x[1])
         except: pass
         self._scores = scores[:15]
         
         
     def save(self):
         """Saves the scores into "scores.txt"
         """
-        fd = open("scores.txt", "w")
+        fd = open(os.path.join(os.path.dirname(__file__), "scores", "scores.txt"), "w")
         for s in self._scores:
             fd.write("%s\t%s\n" % (s[0], s[1]))    
         fd.close()
 
 
     def add(self, name, t):
         """Adds an entry to the scores
@@ -307,20 +307,20 @@
 
 class Game:
     """The game class"""
     
     def __init__(self):
         """Initialises the game
         """
-        self._car_image = pygame.image.load("./gfx/car.png")
-        self._title_image = pygame.image.load("./gfx/title.png")
-        track_image = pygame.image.load("./gfx/track01.png")
-        self._theme_sound = pygame.mixer.Sound("./muzak/track.ogg")
+        self._car_image = pygame.image.load(os.path.join(os.path.dirname(__file__), "gfx", "car.png"))
+        self._title_image = pygame.image.load(os.path.join(os.path.dirname(__file__), "gfx", "title.png"))
+        track_image = pygame.image.load(os.path.join(os.path.dirname(__file__), "gfx", "track01.png"))
+        self._theme_sound = pygame.mixer.Sound(os.path.join(os.path.dirname(__file__), "muzak", "track.ogg"))
         self._theme_sound.set_volume(1)
-        self._engine_sound = pygame.mixer.Sound("./muzak/engine.ogg")
+        self._engine_sound = pygame.mixer.Sound(os.path.join(os.path.dirname(__file__), "muzak", "engine.ogg"))
         self._engine_sound.set_volume(.2)
         self._font = pygame.font.SysFont(None, 48)
         self._height = track_image.get_height()
         self._width = track_image.get_width()
         self._track = Track(track_image)
         self._theme_channel = pygame.mixer.Channel(0)
         self._engine_channel = pygame.mixer.Channel(1)
```

