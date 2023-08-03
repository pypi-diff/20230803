# Comparing `tmp/lastfm-mpris2-scrobbler-0.2.1.tar.gz` & `tmp/lastfm-mpris2-scrobbler-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lastfm-mpris2-scrobbler-0.2.1.tar", last modified: Wed Aug  2 10:58:52 2023, max compression
+gzip compressed data, was "lastfm-mpris2-scrobbler-0.3.0.tar", last modified: Thu Aug  3 03:43:05 2023, max compression
```

## Comparing `lastfm-mpris2-scrobbler-0.2.1.tar` & `lastfm-mpris2-scrobbler-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-02 10:58:52.659799 lastfm-mpris2-scrobbler-0.2.1/
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     1064 2023-08-02 08:55:19.000000 lastfm-mpris2-scrobbler-0.2.1/LICENSE
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     2003 2023-08-02 10:58:52.659799 lastfm-mpris2-scrobbler-0.2.1/PKG-INFO
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     1706 2023-08-02 10:55:50.000000 lastfm-mpris2-scrobbler-0.2.1/README.md
-drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-02 10:58:52.659799 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     2003 2023-08-02 10:58:52.000000 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/PKG-INFO
--rw-rw-r--   0 firefly   (1000) firefly   (1000)      388 2023-08-02 10:58:52.000000 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/SOURCES.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-02 10:58:52.000000 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/dependency_links.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)       62 2023-08-02 10:58:52.000000 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/entry_points.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-02 08:42:31.000000 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/not-zip-safe
--rw-rw-r--   0 firefly   (1000) firefly   (1000)       51 2023-08-02 10:58:52.000000 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/requires.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)        4 2023-08-02 10:58:52.000000 lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/top_level.txt
--rw-rw-r--   0 firefly   (1000) firefly   (1000)       38 2023-08-02 10:58:52.659799 lastfm-mpris2-scrobbler-0.2.1/setup.cfg
--rw-rw-r--   0 firefly   (1000) firefly   (1000)      909 2023-08-02 10:58:39.000000 lastfm-mpris2-scrobbler-0.2.1/setup.py
-drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-02 10:58:52.659799 lastfm-mpris2-scrobbler-0.2.1/src/
--rw-rw-r--   0 firefly   (1000) firefly   (1000)        0 2023-08-02 08:41:31.000000 lastfm-mpris2-scrobbler-0.2.1/src/__init__.py
--rw-rw-r--   0 firefly   (1000) firefly   (1000)     6098 2023-08-02 10:55:16.000000 lastfm-mpris2-scrobbler-0.2.1/src/__main__.py
+drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-03 03:43:05.548173 lastfm-mpris2-scrobbler-0.3.0/
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     1064 2023-08-02 08:55:19.000000 lastfm-mpris2-scrobbler-0.3.0/LICENSE
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     2738 2023-08-03 03:43:05.548173 lastfm-mpris2-scrobbler-0.3.0/PKG-INFO
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     2441 2023-08-03 03:25:48.000000 lastfm-mpris2-scrobbler-0.3.0/README.md
+drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-03 03:43:05.548173 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     1943 2023-08-03 03:32:51.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/PlayerState.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     4379 2023-08-03 03:40:31.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/Scrobbler.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)        0 2023-08-02 08:41:31.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/__init__.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     1449 2023-08-03 03:40:23.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/__main__.py
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)      249 2023-08-03 02:39:01.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/globals.py
+drwxrwxr-x   0 firefly   (1000) firefly   (1000)        0 2023-08-03 03:43:05.548173 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)     2738 2023-08-03 03:43:05.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/PKG-INFO
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)      539 2023-08-03 03:43:05.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/SOURCES.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-03 03:43:05.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/dependency_links.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       82 2023-08-03 03:43:05.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/entry_points.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)        1 2023-08-02 08:42:31.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/not-zip-safe
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       45 2023-08-03 03:43:05.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/requires.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       24 2023-08-03 03:43:05.000000 lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/top_level.txt
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)       38 2023-08-03 03:43:05.548173 lastfm-mpris2-scrobbler-0.3.0/setup.cfg
+-rw-rw-r--   0 firefly   (1000) firefly   (1000)      912 2023-08-03 03:33:32.000000 lastfm-mpris2-scrobbler-0.3.0/setup.py
```

### Comparing `lastfm-mpris2-scrobbler-0.2.1/LICENSE` & `lastfm-mpris2-scrobbler-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lastfm-mpris2-scrobbler-0.2.1/PKG-INFO` & `lastfm-mpris2-scrobbler-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastfm-mpris2-scrobbler
-Version: 0.2.1
+Version: 0.3.0
 Summary: Last.fm scrobbler via MPRIS2 in Linux
 Home-page: https://github.com/Ladbaby/lastfm-scrobbler
 Author: Ladbaby
 Author-email: Ladbabyms@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -32,31 +32,59 @@
 
 ## What is MPRIS2?
 
 > MPRIS (Media Player Remote Interfacing Specification) is a standard D-Bus (Desktop Bus) interface that allows applications to communicate with and control media players running on a Linux desktop environment.
 
 Thus, this scrobbler is a general-purpose one under the Linux desktop environment, supporting scrobble music from media players without a built-in Last.fm scrobbling feature.
 
-Check if your media player supports MPRIS2 via [playerctl](https://github.com/altdesktop/playerctl) (when it is running)
+Check if your media player supports MPRIS2 via (make sure the player is running):
 
 ```bash
-playerctl --list-all
+lastfm-mpris2-scrobbler --list-players
 ```
 
+The uri names of players will be shown
+
 ## Installation
 
-The package is now available via PyPI
+There're two options available now:
 
-```bash
-pip install lastfm-mpris2-scrobbler
-```
+- grab the stand-alone binary from [release page](https://github.com/Ladbaby/lastfm-scrobbler/releases)
+
+- or, via PyPI
+
+    ```bash
+    pip install lastfm-mpris2-scrobbler
+    ```
 
 ## Configurations
 
-The program expect a `config.yaml` file, example and detailed information can be found in `config.yaml.example`
+The program expects a `config.yaml` file, example and detailed information can be found in `config.yaml.example`:
+
+```yaml
+# username for that service
+user_name: foo
+
+# md5 hash of your password (obtained via `echo -n password | md5sum`)
+password_hash: abc123492abccf4f1997f7ccaabc123b
+
+# last.fm api, which can be created via https://www.last.fm/api/account/create
+api_key: 11111111111111111111111111111111
+api_secret: 11111111111111111111111111111111
+
+# the app's uri you want to scrobble
+# use `lastfm-mpris2-scrobbler --list-players` to check the uri name
+application_whitelist: [ "org.mpris.MediaPlayer2.harmonoid" ]
+```
 
 ## Usage
 
 ```bash
-lastfm-mpris2-scrobbler PATH_TO_YOUR_CONFIG/config.yaml
+lastfm-mpris2-scrobbler -c PATH_TO_YOUR_CONFIG/config.yaml
+```
+
+For more options, see:
+
+```bash
+lastfm-mpris2-scrobbler --help
 ```
```

### Comparing `lastfm-mpris2-scrobbler-0.2.1/lastfm_mpris2_scrobbler.egg-info/PKG-INFO` & `lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastfm-mpris2-scrobbler
-Version: 0.2.1
+Version: 0.3.0
 Summary: Last.fm scrobbler via MPRIS2 in Linux
 Home-page: https://github.com/Ladbaby/lastfm-scrobbler
 Author: Ladbaby
 Author-email: Ladbabyms@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -32,31 +32,59 @@
 
 ## What is MPRIS2?
 
 > MPRIS (Media Player Remote Interfacing Specification) is a standard D-Bus (Desktop Bus) interface that allows applications to communicate with and control media players running on a Linux desktop environment.
 
 Thus, this scrobbler is a general-purpose one under the Linux desktop environment, supporting scrobble music from media players without a built-in Last.fm scrobbling feature.
 
-Check if your media player supports MPRIS2 via [playerctl](https://github.com/altdesktop/playerctl) (when it is running)
+Check if your media player supports MPRIS2 via (make sure the player is running):
 
 ```bash
-playerctl --list-all
+lastfm-mpris2-scrobbler --list-players
 ```
 
+The uri names of players will be shown
+
 ## Installation
 
-The package is now available via PyPI
+There're two options available now:
 
-```bash
-pip install lastfm-mpris2-scrobbler
-```
+- grab the stand-alone binary from [release page](https://github.com/Ladbaby/lastfm-scrobbler/releases)
+
+- or, via PyPI
+
+    ```bash
+    pip install lastfm-mpris2-scrobbler
+    ```
 
 ## Configurations
 
-The program expect a `config.yaml` file, example and detailed information can be found in `config.yaml.example`
+The program expects a `config.yaml` file, example and detailed information can be found in `config.yaml.example`:
+
+```yaml
+# username for that service
+user_name: foo
+
+# md5 hash of your password (obtained via `echo -n password | md5sum`)
+password_hash: abc123492abccf4f1997f7ccaabc123b
+
+# last.fm api, which can be created via https://www.last.fm/api/account/create
+api_key: 11111111111111111111111111111111
+api_secret: 11111111111111111111111111111111
+
+# the app's uri you want to scrobble
+# use `lastfm-mpris2-scrobbler --list-players` to check the uri name
+application_whitelist: [ "org.mpris.MediaPlayer2.harmonoid" ]
+```
 
 ## Usage
 
 ```bash
-lastfm-mpris2-scrobbler PATH_TO_YOUR_CONFIG/config.yaml
+lastfm-mpris2-scrobbler -c PATH_TO_YOUR_CONFIG/config.yaml
+```
+
+For more options, see:
+
+```bash
+lastfm-mpris2-scrobbler --help
 ```
```

### Comparing `lastfm-mpris2-scrobbler-0.2.1/setup.py` & `lastfm-mpris2-scrobbler-0.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,32 +3,31 @@
 
 root = path.abspath(path.dirname(__file__))
 with open(path.join(root, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='lastfm-mpris2-scrobbler',
-    version='0.2.1',
+    version='0.3.0',
     description="Last.fm scrobbler via MPRIS2 in Linux",
     url="https://github.com/Ladbaby/lastfm-scrobbler",
     author="Ladbaby",
     author_email="Ladbabyms@outlook.com",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
-        "click",
         "coloredlogs",
         "mpris2",
         "pylast",
         "PyYAML",
         "dbus-python",
     ],
     tests_require=["pytest"],
     entry_points={
         "console_scripts": [
-            "lastfm-mpris2-scrobbler = src.__main__:main",
+            "lastfm-mpris2-scrobbler = lastfm_mpris2_scrobbler.__main__:main",
         ],
     },
     zip_safe=False,
 )
```

### Comparing `lastfm-mpris2-scrobbler-0.2.1/src/__main__.py` & `lastfm-mpris2-scrobbler-0.3.0/lastfm_mpris2_scrobbler/Scrobbler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,46 @@
-import time
-import click
 
-import datetime
-import logging
-import coloredlogs
-from mpris2 import get_players_uri, Player
 import pylast
+from mpris2 import get_players_uri, Player
 
-def get_unix_timestamp():
-    return int(time.mktime(datetime.datetime.now().timetuple()))
-
-class PlayerState:
-    def __init__(self, metadata_dict, playback_status) -> None:
-        self.total_played_time = 0
-        self.last_observation_timestamp = get_unix_timestamp()
-        self.trackid = ""
-        self.if_scrobbled = False
-        self.update_status(metadata_dict, playback_status, self.last_observation_timestamp)
-
-    def handle_multiple_artists(self, artist_array):
-        # convert artist array into a single string
-        return ", ".join(artist_array)
-    
-    def update_status(self, metadata_dict, playback_status, timestamp):
-        # time length of the current song in seconds
-        self.length = int(metadata_dict["mpris:length"] / 1000000)
-        # image file path
-        self.artUrl = str(metadata_dict["mpris:artUrl"])
-        self.album = str(metadata_dict["xesam:album"])
-        self.albumArtist = self.handle_multiple_artists(metadata_dict["xesam:albumArtist"])
-        self.artist = self.handle_multiple_artists(metadata_dict["xesam:artist"])
-        self.discNumber = int(metadata_dict["xesam:discNumber"])
-        self.firstUsed = str(metadata_dict["xesam:firstUsed"])
-        self.title = str(metadata_dict["xesam:title"])
-        self.trackNumber = int(metadata_dict["xesam:trackNumber"])
-        self.url = str(metadata_dict["xesam:url"])
-
-        # record the timestamp of last observation
-        if self.trackid == str(metadata_dict["mpris:trackid"]):
-            self.total_played_time += (timestamp - self.last_observation_timestamp) if playback_status == "Playing" else 0
-        else:
-            self.total_played_time = 0
-            self.if_scrobbled = False
-        self.trackid = str(metadata_dict["mpris:trackid"])
-        self.last_observation_timestamp = timestamp
-
-        # record the playback status in observation
-        # May be 'Playing', 'Paused' or 'Stopped'.
-        self.playback_status = playback_status
+from lastfm_mpris2_scrobbler.globals import logger, get_unix_timestamp
+from lastfm_mpris2_scrobbler.PlayerState import PlayerState
 
 class Scrobbler:
     def __init__(self, **kwargs):
-        self.logger = logging.getLogger("dbus-scrobbler")
-        coloredlogs.install(level="DEBUG", logger=self.logger)
-
+        self.kwargs = kwargs
         self.player_dict = {}
 
         # TODO: handle network error
-        self.network = pylast.LastFMNetwork(
-            api_key=kwargs["api_key"],
-            api_secret=kwargs["api_secret"],
-            username=kwargs["user_name"],
-            password_hash=kwargs["password_hash"],
-        )
-        self.user = self.network.get_user(kwargs["user_name"])
+        self.network = None
+        self.init_network()
+            
         self.application_whitelist = kwargs["application_whitelist"]
 
         self.now_playing_tracks_dict = {}
         for app in self.application_whitelist:
             self.now_playing_tracks_dict[app] = ""
 
         # scrobbler will upload if the track has been played for 4 mins or half the total length
         self.scrobble_time_threshold = 4 * 60
 
+    def init_network(self):
+        try:
+            logger.debug("Try logging in now...")
+            self.network = pylast.LastFMNetwork(
+                api_key=self.kwargs["api_key"],
+                api_secret=self.kwargs["api_secret"],
+                username=self.kwargs["user_name"],
+                password_hash=self.kwargs["password_hash"],
+            )
+            logger.info(f"Successfully login to Last.fm as {self.kwargs['user_name']}")
+        except Exception as e:
+            logger.debug(f"LastFMNetwork initialization failed: {e=}")
+            logger.warning("Running in OFFLINE mode")
+
     def connect_to_all_players(self):
         last_observation_uri_list = list(self.player_dict)
         for uri in get_players_uri():
             uri = str(uri)
             if uri in self.application_whitelist:
                 p = Player(dbus_interface_info={'dbus_uri': uri})
                 if uri in self.player_dict.keys():
@@ -84,66 +48,47 @@
                     last_observation_uri_list.remove(uri)
                 else:
                     self.player_dict[uri] = PlayerState(p.Metadata, p.PlaybackStatus)
         for uri in last_observation_uri_list:
             del self.player_dict[uri]
 
     def scrobble_all_players(self):
-        for uri, player_obj in self.player_dict.items():
-            if player_obj.playback_status == "Playing":
-                self.network.update_now_playing(
-                    artist=player_obj.artist,
-                    title=player_obj.title,
-                    album=player_obj.album,
-                    album_artist=player_obj.albumArtist,
-                    track_number=player_obj.trackNumber,
-                )
-            if player_obj.total_played_time >= min(self.scrobble_time_threshold, int(player_obj.length / 2)) and not player_obj.if_scrobbled:
-                self.network.scrobble(
-                    artist=player_obj.artist, 
-                    title=player_obj.title,
-                    timestamp=player_obj.last_observation_timestamp,
-                    album=player_obj.album,
-                    album_artist=player_obj.albumArtist,
-                    track_number=player_obj.trackNumber,
-                    duration=int(player_obj.length)
-                )
-                player_obj.if_scrobbled = True
-                self.logger.debug("scrobbled track: " + player_obj.title)
-                self.logger.debug("artist: " + player_obj.artist)
-                self.logger.debug("timestamp: " + str(player_obj.last_observation_timestamp))
-                self.logger.debug("album: " + player_obj.album)
-                self.logger.debug("albumArtist: " + player_obj.albumArtist)
-                self.logger.debug("trackNumber: " + str(player_obj.trackNumber))
-                self.logger.debug("duration: " + str(int(player_obj.length)))
-                self.logger.debug("played time: " + str(int(player_obj.total_played_time)))
-            else:
-                # self.logger.debug("scrobble condition unmet")
-                pass
-
-    def update_now_playing(self):
-        pass
-
-@click.command()
-@click.argument("config_file")
-def main(config_file):
-    from dbus.mainloop.glib import DBusGMainLoop
-    import yaml
-
-    dbus_loop = DBusGMainLoop(set_as_default=True)
-
-    # load config
-    with open(config_file, "r") as file:
-        config = yaml.safe_load(file)
-
-    scrobbler = Scrobbler(**config)
-
-    while True:
-        try: 
-            scrobbler.connect_to_all_players()
-            scrobbler.scrobble_all_players()
-        except Exception as e:
-            pass
-        time.sleep(5)
-
-if __name__ == "__main__":
-    main()
+        if self.network is not None:
+            for uri, player_obj in self.player_dict.items():
+                if player_obj.playback_status == "Playing":
+                    try:
+                        self.network.update_now_playing(
+                            artist=player_obj.artist,
+                            title=player_obj.title,
+                            album=player_obj.album,
+                            album_artist=player_obj.albumArtist,
+                            track_number=player_obj.trackNumber,
+                        )
+                    except Exception as e:
+                        logger.error(f"Failed to report now playing status: {e=}")
+                if player_obj.total_played_time >= min(self.scrobble_time_threshold, int(player_obj.length / 2)) and not player_obj.if_scrobbled:
+                    try:
+                        self.network.scrobble(
+                            artist=player_obj.artist, 
+                            title=player_obj.title,
+                            timestamp=player_obj.last_observation_timestamp,
+                            album=player_obj.album,
+                            album_artist=player_obj.albumArtist,
+                            track_number=player_obj.trackNumber,
+                            duration=int(player_obj.length)
+                        )
+                    except Exception as e:
+                        logger.error(f"Failed to scrobble: {e=}")
+                    player_obj.if_scrobbled = True
+                    logger.debug("scrobbled track: " + player_obj.title)
+                    logger.debug("artist: " + player_obj.artist)
+                    logger.debug("timestamp: " + str(player_obj.last_observation_timestamp))
+                    logger.debug("album: " + player_obj.album)
+                    logger.debug("albumArtist: " + player_obj.albumArtist)
+                    logger.debug("trackNumber: " + str(player_obj.trackNumber))
+                    logger.debug("duration: " + str(int(player_obj.length)))
+                    logger.debug("played time: " + str(int(player_obj.total_played_time)))
+                else:
+                    logger.debug("scrobble condition unmet")
+                    pass
+        else:
+            self.init_network()
```

