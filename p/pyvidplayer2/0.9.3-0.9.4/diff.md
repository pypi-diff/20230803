# Comparing `tmp/pyvidplayer2-0.9.3.tar.gz` & `tmp/pyvidplayer2-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvidplayer2-0.9.3.tar", last modified: Mon Jul 31 18:31:06 2023, max compression
+gzip compressed data, was "pyvidplayer2-0.9.4.tar", last modified: Thu Aug  3 00:39:48 2023, max compression
```

## Comparing `pyvidplayer2-0.9.3.tar` & `pyvidplayer2-0.9.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 18:31:06.017113 pyvidplayer2-0.9.3/
--rw-rw-rw-   0        0        0     1085 2023-07-19 21:30:21.000000 pyvidplayer2-0.9.3/LICENSE
--rw-rw-rw-   0        0        0     2493 2023-07-31 18:31:06.017113 pyvidplayer2-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     2160 2023-07-30 14:05:34.000000 pyvidplayer2-0.9.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 18:31:06.003109 pyvidplayer2-0.9.3/pyvidplayer2/
--rw-rw-rw-   0        0        0      694 2023-07-30 13:39:04.000000 pyvidplayer2-0.9.3/pyvidplayer2/__init__.py
--rw-rw-rw-   0        0        0     2678 2023-07-31 02:21:17.000000 pyvidplayer2-0.9.3/pyvidplayer2/audio_handler.py
--rw-rw-rw-   0        0        0     1339 2023-07-30 13:44:08.000000 pyvidplayer2-0.9.3/pyvidplayer2/post_processing.py
--rw-rw-rw-   0        0        0     2232 2023-07-29 04:31:47.000000 pyvidplayer2-0.9.3/pyvidplayer2/subtitles.py
--rw-rw-rw-   0        0        0     7477 2023-07-31 02:20:08.000000 pyvidplayer2-0.9.3/pyvidplayer2/video.py
--rw-rw-rw-   0        0        0     9558 2023-07-31 02:29:04.000000 pyvidplayer2-0.9.3/pyvidplayer2/video_player.py
--rw-rw-rw-   0        0        0     1336 2023-07-30 14:33:49.000000 pyvidplayer2-0.9.3/pyvidplayer2/video_pygame.py
--rw-rw-rw-   0        0        0     1531 2023-07-26 18:35:59.000000 pyvidplayer2-0.9.3/pyvidplayer2/video_pyglet.py
--rw-rw-rw-   0        0        0     1662 2023-07-30 14:49:19.000000 pyvidplayer2-0.9.3/pyvidplayer2/video_pyqt.py
--rw-rw-rw-   0        0        0     1500 2023-07-30 02:15:43.000000 pyvidplayer2-0.9.3/pyvidplayer2/video_tkinter.py
-drwxrwxrwx   0        0        0        0 2023-07-31 18:31:06.016112 pyvidplayer2-0.9.3/pyvidplayer2.egg-info/
--rw-rw-rw-   0        0        0     2493 2023-07-31 18:31:05.000000 pyvidplayer2-0.9.3/pyvidplayer2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-07-31 18:31:05.000000 pyvidplayer2-0.9.3/pyvidplayer2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 18:31:05.000000 pyvidplayer2-0.9.3/pyvidplayer2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-07-31 18:31:05.000000 pyvidplayer2-0.9.3/pyvidplayer2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-31 18:31:05.000000 pyvidplayer2-0.9.3/pyvidplayer2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 18:31:06.017113 pyvidplayer2-0.9.3/setup.cfg
--rw-rw-rw-   0        0        0      734 2023-07-31 18:30:29.000000 pyvidplayer2-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:39:48.081952 pyvidplayer2-0.9.4/
+-rw-rw-rw-   0        0        0     1085 2023-08-02 19:17:31.000000 pyvidplayer2-0.9.4/LICENSE
+-rw-rw-rw-   0        0        0     2493 2023-08-03 00:39:48.081394 pyvidplayer2-0.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2160 2023-08-02 19:17:31.000000 pyvidplayer2-0.9.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 00:39:48.028466 pyvidplayer2-0.9.4/pyvidplayer2/
+-rw-rw-rw-   0        0        0      694 2023-08-02 21:57:17.000000 pyvidplayer2-0.9.4/pyvidplayer2/__init__.py
+-rw-rw-rw-   0        0        0     2678 2023-08-02 19:17:32.000000 pyvidplayer2-0.9.4/pyvidplayer2/audio_handler.py
+-rw-rw-rw-   0        0        0     1339 2023-08-02 19:17:32.000000 pyvidplayer2-0.9.4/pyvidplayer2/post_processing.py
+-rw-rw-rw-   0        0        0     2232 2023-08-02 19:17:32.000000 pyvidplayer2-0.9.4/pyvidplayer2/subtitles.py
+-rw-rw-rw-   0        0        0     7699 2023-08-02 22:49:24.000000 pyvidplayer2-0.9.4/pyvidplayer2/video.py
+-rw-rw-rw-   0        0        0     9558 2023-08-02 19:17:32.000000 pyvidplayer2-0.9.4/pyvidplayer2/video_player.py
+-rw-rw-rw-   0        0        0     1336 2023-08-02 19:17:32.000000 pyvidplayer2-0.9.4/pyvidplayer2/video_pygame.py
+-rw-rw-rw-   0        0        0     1531 2023-08-02 19:17:32.000000 pyvidplayer2-0.9.4/pyvidplayer2/video_pyglet.py
+-rw-rw-rw-   0        0        0     1662 2023-08-02 19:17:32.000000 pyvidplayer2-0.9.4/pyvidplayer2/video_pyqt.py
+-rw-rw-rw-   0        0        0     1500 2023-08-02 19:17:32.000000 pyvidplayer2-0.9.4/pyvidplayer2/video_tkinter.py
+drwxrwxrwx   0        0        0        0 2023-08-03 00:39:48.080218 pyvidplayer2-0.9.4/pyvidplayer2.egg-info/
+-rw-rw-rw-   0        0        0     2493 2023-08-03 00:39:47.000000 pyvidplayer2-0.9.4/pyvidplayer2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-08-03 00:39:47.000000 pyvidplayer2-0.9.4/pyvidplayer2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 00:39:47.000000 pyvidplayer2-0.9.4/pyvidplayer2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-08-03 00:39:47.000000 pyvidplayer2-0.9.4/pyvidplayer2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-03 00:39:47.000000 pyvidplayer2-0.9.4/pyvidplayer2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 00:39:48.081952 pyvidplayer2-0.9.4/setup.cfg
+-rw-rw-rw-   0        0        0      734 2023-08-03 00:37:03.000000 pyvidplayer2-0.9.4/setup.py
```

### Comparing `pyvidplayer2-0.9.3/LICENSE` & `pyvidplayer2-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.3/PKG-INFO` & `pyvidplayer2-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvidplayer2
-Version: 0.9.3
+Version: 0.9.4
 Summary: Video playback in Python
 Home-page: https://github.com/ree1261/pyvidplayer2
 Author: Anray Liu
 Author-email: anrayliu@gmail.com
 License: MIT
 Keywords: pygame,video,playback
 Platform: windows
```

### Comparing `pyvidplayer2-0.9.3/README.md` & `pyvidplayer2-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.3/pyvidplayer2/__init__.py` & `pyvidplayer2-0.9.4/pyvidplayer2/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.3/pyvidplayer2/audio_handler.py` & `pyvidplayer2-0.9.4/pyvidplayer2/audio_handler.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.3/pyvidplayer2/post_processing.py` & `pyvidplayer2-0.9.4/pyvidplayer2/post_processing.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.3/pyvidplayer2/subtitles.py` & `pyvidplayer2-0.9.4/pyvidplayer2/subtitles.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.3/pyvidplayer2/video.py` & `pyvidplayer2-0.9.4/pyvidplayer2/video.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,31 @@
     def _threaded_load(self) -> None:
         self._chunks_claimed += 1
         i = self._chunks_claimed # assigned to variable so another thread does not change it
 
         self._chunks.append(None)
 
         s = self._convert_seconds(self._starting_time + (self._chunks_claimed - 1) * self.chunk_size)
-        p = subprocess.run(f'"{get_ffmpeg_path()}" -i "{self.path}" -ss {s} -t {self._convert_seconds(self.chunk_size)} -f wav -loglevel quiet -', capture_output=True)
+
+        command = [
+            get_ffmpeg_path(),
+            "-i",
+            self.path,
+            "-ss",
+            str(s),
+            "-t",
+            str(self._convert_seconds(self.chunk_size)),
+            "-f",
+            "wav",
+            "-loglevel",
+            "quiet",
+            "-"
+        ]
+
+        p = subprocess.run(command, capture_output=True)
         
         self._chunks[i - self._chunks_played - 1] = p.stdout
 
     def _update_threads(self) -> None:
         for t in self._threads:
             if not t.is_alive():
                 self._threads.remove(t)
```

### Comparing `pyvidplayer2-0.9.3/pyvidplayer2/video_player.py` & `pyvidplayer2-0.9.4/pyvidplayer2/video_player.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.3/pyvidplayer2/video_pygame.py` & `pyvidplayer2-0.9.4/pyvidplayer2/video_pygame.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.3/pyvidplayer2/video_pyglet.py` & `pyvidplayer2-0.9.4/pyvidplayer2/video_pyglet.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.3/pyvidplayer2/video_pyqt.py` & `pyvidplayer2-0.9.4/pyvidplayer2/video_pyqt.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.3/pyvidplayer2/video_tkinter.py` & `pyvidplayer2-0.9.4/pyvidplayer2/video_tkinter.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.3/pyvidplayer2.egg-info/PKG-INFO` & `pyvidplayer2-0.9.4/pyvidplayer2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvidplayer2
-Version: 0.9.3
+Version: 0.9.4
 Summary: Video playback in Python
 Home-page: https://github.com/ree1261/pyvidplayer2
 Author: Anray Liu
 Author-email: anrayliu@gmail.com
 License: MIT
 Keywords: pygame,video,playback
 Platform: windows
```

### Comparing `pyvidplayer2-0.9.3/setup.py` & `pyvidplayer2-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", 'r') as f:
     long_desc = f.read()
 
 
 setup(
     name="pyvidplayer2",
-    version="0.9.3",
+    version="0.9.4",
     description="Video playback in Python",
     long_description=long_desc,
     long_description_content_type = "text/markdown",
     author="Anray Liu",
     author_email="anrayliu@gmail.com",
     license="MIT",
     packages=["pyvidplayer2"],
```

