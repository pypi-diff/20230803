# Comparing `tmp/mopidy-yamusic-2.2.1.tar.gz` & `tmp/mopidy-yamusic-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mopidy-yamusic-2.2.1.tar", last modified: Tue Sep 27 22:26:56 2022, max compression
+gzip compressed data, was "mopidy-yamusic-2.2.2.tar", last modified: Thu Aug  3 02:34:54 2023, max compression
```

## Comparing `mopidy-yamusic-2.2.1.tar` & `mopidy-yamusic-2.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 22:26:56.674767 mopidy-yamusic-2.2.1/
--rw-r--r--   0 root         (0) root         (0)    35149 2022-04-06 15:13:17.000000 mopidy-yamusic-2.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1394 2022-09-27 22:26:56.674767 mopidy-yamusic-2.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      791 2022-05-29 08:55:56.000000 mopidy-yamusic-2.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 22:26:56.674767 mopidy-yamusic-2.2.1/mopidy_yamusic/
--rw-r--r--   0 root         (0) root         (0)     1458 2022-05-29 08:56:30.000000 mopidy-yamusic-2.2.1/mopidy_yamusic/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1523 2022-05-29 08:56:30.000000 mopidy-yamusic-2.2.1/mopidy_yamusic/backend.py
--rw-r--r--   0 root         (0) root         (0)     3523 2022-05-29 08:56:30.000000 mopidy-yamusic-2.2.1/mopidy_yamusic/caches.py
--rw-r--r--   0 root         (0) root         (0)     6063 2022-05-29 08:56:30.000000 mopidy-yamusic-2.2.1/mopidy_yamusic/classes.py
--rw-r--r--   0 root         (0) root         (0)      126 2022-05-29 08:56:30.000000 mopidy-yamusic-2.2.1/mopidy_yamusic/ext.conf
--rw-r--r--   0 root         (0) root         (0)     9973 2022-06-04 21:46:07.000000 mopidy-yamusic-2.2.1/mopidy_yamusic/library_provider.py
--rw-r--r--   0 root         (0) root         (0)     4521 2022-05-29 08:56:30.000000 mopidy-yamusic-2.2.1/mopidy_yamusic/oauth.py
--rw-r--r--   0 root         (0) root         (0)      992 2022-05-29 08:56:30.000000 mopidy-yamusic-2.2.1/mopidy_yamusic/playback_provider.py
--rw-r--r--   0 root         (0) root         (0)    13919 2022-09-27 22:23:26.000000 mopidy-yamusic-2.2.1/mopidy_yamusic/playlist_provider.py
--rw-r--r--   0 root         (0) root         (0)      624 2022-05-29 08:56:30.000000 mopidy-yamusic-2.2.1/mopidy_yamusic/t.py
--rw-r--r--   0 root         (0) root         (0)     5960 2022-05-29 08:56:30.000000 mopidy-yamusic-2.2.1/mopidy_yamusic/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-27 22:26:56.674767 mopidy-yamusic-2.2.1/mopidy_yamusic.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1394 2022-09-27 22:26:56.000000 mopidy-yamusic-2.2.1/mopidy_yamusic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      557 2022-09-27 22:26:56.000000 mopidy-yamusic-2.2.1/mopidy_yamusic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-27 22:26:56.000000 mopidy-yamusic-2.2.1/mopidy_yamusic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2022-09-27 22:26:56.000000 mopidy-yamusic-2.2.1/mopidy_yamusic.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-09-27 22:26:56.000000 mopidy-yamusic-2.2.1/mopidy_yamusic.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-09-27 22:26:56.000000 mopidy-yamusic-2.2.1/mopidy_yamusic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-27 22:26:56.674767 mopidy-yamusic-2.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      930 2022-09-27 22:26:23.000000 mopidy-yamusic-2.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 02:34:54.159364 mopidy-yamusic-2.2.2/
+-rw-r--r--   0 root         (0) root         (0)    35149 2022-04-06 15:13:17.000000 mopidy-yamusic-2.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-08-03 02:34:54.159364 mopidy-yamusic-2.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      791 2022-05-29 08:55:56.000000 mopidy-yamusic-2.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 02:34:54.159364 mopidy-yamusic-2.2.2/mopidy_yamusic/
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-08-03 02:30:09.000000 mopidy-yamusic-2.2.2/mopidy_yamusic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2022-09-27 22:23:29.000000 mopidy-yamusic-2.2.2/mopidy_yamusic/backend.py
+-rw-r--r--   0 root         (0) root         (0)     3523 2022-09-27 22:23:29.000000 mopidy-yamusic-2.2.2/mopidy_yamusic/caches.py
+-rw-r--r--   0 root         (0) root         (0)     6063 2022-09-27 22:23:29.000000 mopidy-yamusic-2.2.2/mopidy_yamusic/classes.py
+-rw-r--r--   0 root         (0) root         (0)      126 2022-09-27 22:23:29.000000 mopidy-yamusic-2.2.2/mopidy_yamusic/ext.conf
+-rw-r--r--   0 root         (0) root         (0)     9973 2022-09-27 22:23:29.000000 mopidy-yamusic-2.2.2/mopidy_yamusic/library_provider.py
+-rw-r--r--   0 root         (0) root         (0)     4521 2022-09-27 22:23:29.000000 mopidy-yamusic-2.2.2/mopidy_yamusic/oauth.py
+-rw-r--r--   0 root         (0) root         (0)      992 2022-09-27 22:23:29.000000 mopidy-yamusic-2.2.2/mopidy_yamusic/playback_provider.py
+-rw-r--r--   0 root         (0) root         (0)    14115 2023-08-03 02:29:33.000000 mopidy-yamusic-2.2.2/mopidy_yamusic/playlist_provider.py
+-rw-r--r--   0 root         (0) root         (0)      624 2022-09-27 22:23:29.000000 mopidy-yamusic-2.2.2/mopidy_yamusic/t.py
+-rw-r--r--   0 root         (0) root         (0)     5960 2022-09-27 22:23:29.000000 mopidy-yamusic-2.2.2/mopidy_yamusic/web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 02:34:54.159364 mopidy-yamusic-2.2.2/mopidy_yamusic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-08-03 02:34:54.000000 mopidy-yamusic-2.2.2/mopidy_yamusic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      557 2023-08-03 02:34:54.000000 mopidy-yamusic-2.2.2/mopidy_yamusic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 02:34:54.000000 mopidy-yamusic-2.2.2/mopidy_yamusic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-08-03 02:34:54.000000 mopidy-yamusic-2.2.2/mopidy_yamusic.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-03 02:34:54.000000 mopidy-yamusic-2.2.2/mopidy_yamusic.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-03 02:34:54.000000 mopidy-yamusic-2.2.2/mopidy_yamusic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 02:34:54.159364 mopidy-yamusic-2.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      930 2023-08-03 02:29:57.000000 mopidy-yamusic-2.2.2/setup.py
```

### Comparing `mopidy-yamusic-2.2.1/LICENSE` & `mopidy-yamusic-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mopidy-yamusic-2.2.1/README.md` & `mopidy-yamusic-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mopidy-yamusic-2.2.1/mopidy_yamusic/__init__.py` & `mopidy-yamusic-2.2.2/mopidy_yamusic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from mopidy import ext, config
 import pathlib
 from .backend import YaMusicBackend
 import yandex_music
-__version__ = '0.8'
+__version__ = '2.2.2'
 import logging
 logger = logging.getLogger("yandex")
 from .oauth import OAuthManager
 
 class Extension(ext.Extension):
     dist_name = "Mopidy-YaMusic"
     ext_name = "yamusic"
```

### Comparing `mopidy-yamusic-2.2.1/mopidy_yamusic/backend.py` & `mopidy-yamusic-2.2.2/mopidy_yamusic/backend.py`

 * *Files identical despite different names*

### Comparing `mopidy-yamusic-2.2.1/mopidy_yamusic/caches.py` & `mopidy-yamusic-2.2.2/mopidy_yamusic/caches.py`

 * *Files identical despite different names*

### Comparing `mopidy-yamusic-2.2.1/mopidy_yamusic/classes.py` & `mopidy-yamusic-2.2.2/mopidy_yamusic/classes.py`

 * *Files identical despite different names*

### Comparing `mopidy-yamusic-2.2.1/mopidy_yamusic/library_provider.py` & `mopidy-yamusic-2.2.2/mopidy_yamusic/library_provider.py`

 * *Files identical despite different names*

### Comparing `mopidy-yamusic-2.2.1/mopidy_yamusic/oauth.py` & `mopidy-yamusic-2.2.2/mopidy_yamusic/oauth.py`

 * *Files identical despite different names*

### Comparing `mopidy-yamusic-2.2.1/mopidy_yamusic/playback_provider.py` & `mopidy-yamusic-2.2.2/mopidy_yamusic/playback_provider.py`

 * *Files identical despite different names*

### Comparing `mopidy-yamusic-2.2.1/mopidy_yamusic/playlist_provider.py` & `mopidy-yamusic-2.2.2/mopidy_yamusic/playlist_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,23 +35,24 @@
         if self._client == None:
           return []
 
         if self._playlist_cache.get_list() != {}:
           return self._playlist_cache.get_list()
 
         yandex_daily = YMRef.from_raw(_YM_GENERATED, "yamusic-daily", "Микс дня", "avatars.yandex.net/get-music-user-playlist/70586/r5l8ziDPSKyp02/%1x%2", True)
+        yandex_dejavu = YMRef.from_raw(_YM_GENERATED, "yamusic-dejavu", "Дежавю", "avatars.yandex.net/get-music-user-playlist/28719/r5lljeHXSjXZUw/%1x%2", True)
         yandex_podcasts = YMRef.from_raw(_YM_GENERATED, "yamusic-podcasts", "Подкасты","avatars.yandex.net/get-music-user-playlist/28719/r5loh7rM0HS0tl/%1x%2", True)
         yandex_premier = YMRef.from_raw(_YM_GENERATED, "yamusic-premiere", "Премьера","avatars.yandex.net/get-music-user-playlist/27701/r5ldfjP1rJoson/%1x%2", True)
         yandex_liked = YMRef.from_raw(_YM_LIKED, "yamusic-like", "Мне нравится","music.yandex.ru/blocks/playlist-cover/playlist-cover_like.png", True)
         yandex_liked_last = YMRef.from_raw(_YM_LIKED_LAST, "yamusic-likelast", "Понравилось","music.yandex.ru/blocks/playlist-cover/playlist-cover_like.png", True)
-        yandex_try = YMRef.from_raw(_YM_TRY, "yamusic-try", "Попробуйте","avatars.yandex.net/get-music-misc/70683/mix.5f632be0dc6c364f3f1a4bf7.background-image.1663940728198/%1x%2",True)
-        yandex_blog = YMRef.from_raw(_YM_BLOG, "1234", "Новые хиты","avatars.yandex.net/get-music-user-playlist/34120/103372440.1234.39116ru/%1x%2?1648715240098", True)
+        yandex_try = YMRef.from_raw(_YM_TRY, "yamusic-try", "Попробуйте","avatars.yandex.net/get-music-misc/30221/mix.5d9b5f2451c8385312d775f9.background-image.1690533495987/%1x%2",True)
+        yandex_blog = YMRef.from_raw(_YM_BLOG, "1234", "Новые хиты","avatars.yandex.net/get-music-misc/29541/mix.5f215a08418dac34d35e8da6.background-image.1690810669410/%1x%2", True)
         playlists = self._client.users_playlists_list()
         refs = []
-        refs.extend([yandex_daily, yandex_premier, yandex_liked, yandex_liked_last, yandex_try, yandex_blog, yandex_podcasts])
+        refs.extend([yandex_daily, yandex_dejavu, yandex_premier, yandex_liked, yandex_liked_last, yandex_try, yandex_blog, yandex_podcasts])
         user_refs = list(map(YMRef.from_playlist, playlists))
         refs.extend(user_refs)
         self._playlist_cache.put_list(refs)
         logger.debug(refs)
         return refs
 
     def get_items(self, uri: str) -> YMRef:
```

### Comparing `mopidy-yamusic-2.2.1/mopidy_yamusic/t.py` & `mopidy-yamusic-2.2.2/mopidy_yamusic/t.py`

 * *Files identical despite different names*

### Comparing `mopidy-yamusic-2.2.1/mopidy_yamusic/web.py` & `mopidy-yamusic-2.2.2/mopidy_yamusic/web.py`

 * *Files identical despite different names*

### Comparing `mopidy-yamusic-2.2.1/mopidy_yamusic.egg-info/SOURCES.txt` & `mopidy-yamusic-2.2.2/mopidy_yamusic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mopidy-yamusic-2.2.1/setup.py` & `mopidy-yamusic-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
     name='mopidy-yamusic',
-    version='2.2.1',
+    version='2.2.2',
     description='Mopidy extension for playing music from YandexMusic',
     description_file='README.md',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/stffart/mopidy-yamusic',
     author='stffart',
     author_email='stffart@gmail.com',
```

