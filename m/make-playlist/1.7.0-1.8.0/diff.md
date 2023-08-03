# Comparing `tmp/make_playlist-1.7.0.tar.gz` & `tmp/make_playlist-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "make_playlist-1.7.0.tar", last modified: Mon Jun 12 13:19:28 2023, max compression
+gzip compressed data, was "make_playlist-1.8.0.tar", last modified: Thu Aug  3 11:03:54 2023, max compression
```

## Comparing `make_playlist-1.7.0.tar` & `make_playlist-1.8.0.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-06-12 13:19:28.626745 make_playlist-1.7.0/
--rwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    34916 2022-09-09 08:34:13.000000 make_playlist-1.7.0/LICENSE.md
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       19 2022-09-09 08:34:13.000000 make_playlist-1.7.0/MANIFEST.in
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8842 2023-06-12 13:19:28.626745 make_playlist-1.7.0/PKG-INFO
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8033 2023-06-12 13:15:40.000000 make_playlist-1.7.0/README.md
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1089 2023-06-12 13:15:40.000000 make_playlist-1.7.0/__info__.py
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-06-12 13:19:28.625744 make_playlist-1.7.0/make_playlist.egg-info/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8842 2023-06-12 13:19:28.000000 make_playlist-1.7.0/make_playlist.egg-info/PKG-INFO
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      285 2023-06-12 13:19:28.000000 make_playlist-1.7.0/make_playlist.egg-info/SOURCES.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        1 2023-06-12 13:19:28.000000 make_playlist-1.7.0/make_playlist.egg-info/dependency_links.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       61 2023-06-12 13:19:28.000000 make_playlist-1.7.0/make_playlist.egg-info/entry_points.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        8 2023-06-12 13:19:28.000000 make_playlist-1.7.0/make_playlist.egg-info/requires.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        5 2023-06-12 13:19:28.000000 make_playlist-1.7.0/make_playlist.egg-info/top_level.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    15935 2023-06-12 13:15:40.000000 make_playlist-1.7.0/mkpl.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       38 2023-06-12 13:19:28.626745 make_playlist-1.7.0/setup.cfg
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     2026 2023-06-12 13:15:40.000000 make_playlist-1.7.0/setup.py
+drwxrwxr-x   0 gu        (1000) gu        (1000)        0 2023-08-03 11:03:54.299885 make_playlist-1.8.0/
+-rwxrwxr-x   0 gu        (1000) gu        (1000)    34916 2022-10-24 16:51:45.000000 make_playlist-1.8.0/LICENSE.md
+-rw-rw-r--   0 gu        (1000) gu        (1000)     9110 2023-08-03 11:03:54.299885 make_playlist-1.8.0/PKG-INFO
+-rw-rw-r--   0 gu        (1000) gu        (1000)     8401 2023-08-03 11:01:53.000000 make_playlist-1.8.0/README.md
+drwxrwxr-x   0 gu        (1000) gu        (1000)        0 2023-08-03 11:03:54.299885 make_playlist-1.8.0/make_playlist.egg-info/
+-rw-rw-r--   0 gu        (1000) gu        (1000)     9110 2023-08-03 11:03:54.000000 make_playlist-1.8.0/make_playlist.egg-info/PKG-INFO
+-rw-rw-r--   0 gu        (1000) gu        (1000)      267 2023-08-03 11:03:54.000000 make_playlist-1.8.0/make_playlist.egg-info/SOURCES.txt
+-rw-rw-r--   0 gu        (1000) gu        (1000)        1 2023-08-03 11:03:54.000000 make_playlist-1.8.0/make_playlist.egg-info/dependency_links.txt
+-rw-rw-r--   0 gu        (1000) gu        (1000)       61 2023-08-03 11:03:54.000000 make_playlist-1.8.0/make_playlist.egg-info/entry_points.txt
+-rw-rw-r--   0 gu        (1000) gu        (1000)        8 2023-08-03 11:03:54.000000 make_playlist-1.8.0/make_playlist.egg-info/requires.txt
+-rw-rw-r--   0 gu        (1000) gu        (1000)        5 2023-08-03 11:03:54.000000 make_playlist-1.8.0/make_playlist.egg-info/top_level.txt
+-rw-rw-r--   0 gu        (1000) gu        (1000)    18599 2023-08-03 11:01:53.000000 make_playlist-1.8.0/mkpl.py
+-rw-rw-r--   0 gu        (1000) gu        (1000)      929 2023-08-03 11:01:53.000000 make_playlist-1.8.0/pyproject.toml
+-rw-rw-r--   0 gu        (1000) gu        (1000)       38 2023-08-03 11:03:54.299885 make_playlist-1.8.0/setup.cfg
```

### Comparing `make_playlist-1.7.0/LICENSE.md` & `make_playlist-1.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `make_playlist-1.7.0/PKG-INFO` & `make_playlist-1.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 Metadata-Version: 2.1
 Name: make_playlist
-Version: 1.7.0
-Summary: Make M3U format playlist from command line
-Home-page: https://github.com/MatteoGuadrini/mkpl
-Author: Matteo Guadrini
-Author-email: matteo.guadrini@hotmail.it
-Maintainer: Matteo Guadrini
-Maintainer-email: matteo.guadrini@hotmail.it
-License: GNU General Public License v3.0
-Project-URL: Documentation, https://github.com/MatteoGuadrini/mkpl
-Project-URL: GitHub Project, https://github.com/MatteoGuadrini/mkpl
-Project-URL: Issue Tracker, https://github.com/MatteoGuadrini/mkpl/issues
+Version: 1.8.0
+Summary: Make M3U format playlist from command line.
+Author-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
+Maintainer-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
+Project-URL: homepage, https://github.com/MatteoGuadrini/mkpl
+Project-URL: documentation, https://matteoguadrini.github.io/mkpl/
+Project-URL: changelog, https://github.com/MatteoGuadrini/mkpl/blob/master/CHANGES.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# ``make_playlist``: Make playlist command line tool
+# ``make_playlist``: Playlist maker
+
+<img src="img/mkpl_logo.svg" alt="mkpl" title="mkpl" width="200" height="200" />
 
 ``mkpl`` is a _command line tool_ to create playlist files (**[M3U](https://en.wikipedia.org/wiki/M3U) format**).
 
 ## Installation
 
 To install ``mkpl``, see here:
 
 ```console
 $ pip install make_playlist               # for python enviroment
 
 $ dnf copr enable matteoguadrini/mkpl
 $ dnf install python-make_playlist -y     # for Red Hat and fedora
 
 $ git clone https://github.com/MatteoGuadrini/mkpl.git && cd mkpl
-$ python setup.py install                 # for others
+$ pip install .                           # for others
 ```
 
 ## Command arguments
 
 ``mkpl`` have many command line arguments. They are explained in this table:
 
 | short | long            | description                                   | args                      |
@@ -48,26 +46,28 @@
 | -p    | --pattern       | Regular expression inclusion pattern          | Regular expression string |
 | -f    | --format        | Select only a file format                     | Format of file. ex. mp3   |
 | -s    | --size          | Start size in bytes                           | Bytes number              |
 | -m    | --max-tracks    | Maximum number of tracks                      | Number                    |
 | -t    | --title         | Playlist title                                | Title string              |
 | -g    | --encoding      | Text encoding                                 | UTF-8,ASCII,UNICODE       |
 | -I    | --image         | Playlist image                                | Image path                |
-| -l    | --link          | Add remote file links                         | Links                     |
+| -l    | --link          | Add local or remote files                     | Files                     |
+| -j    | --join          | Join one or more other playlist files         | Playlist files            |
 | -r    | --recursive     | Recursive search                              |                           |
 | -a    | --absolute      | Absolute file name                            |                           |
 | -s    | --shuffle       | Casual order                                  |                           |
 | -u    | --unique        | The same files are not placed in the playlist |                           |
 | -c    | --append        | Continue playlist instead of override it      |                           |
 | -w    | --windows       | Windows style folder separator                |                           |
 | -v    | --verbose       | Enable verbosity (debug mode)                 |                           |
 | -S    | --split         | Split playlist by directories                 |                           |
 | -o    | --orderby-name  | Order playlist files by name                  |                           |
 | -O    | --orderby-date  | Order playlist files by creation date         |                           |
 | -T    | --orderby-track | Order playlist files by track                 |                           |
+| -y    | --orderby-year  | Order playlist files by year                  |                           |
 
 ## Examples
 
 1. Create a playlist for one music album:
 
     ```bash
     cd myalbum
@@ -158,33 +158,39 @@
     my_music.m3u
     folder1.m3u
     folder2.m3u
     folder3.m3u
     ...
     ```
 
-15. Sort playlist files by name (`-o`), by creation date (`-O`) or by track number (`-T`):
+15. Sort playlist files by name (`-o`), by creation date (`-O`), by track number (`-T`) or by year (`-y`):
 
     ```bash
     mkpl -d "new_collection" -r "my music.m3u" -o
     mkpl -d "new_collection" -r "my music.m3u" -O
     mkpl -d "new_collection" -r "my music.m3u" -T
+    mkpl -d "new_collection" -r "my music.m3u" -y
     ```
 
+16. Join the _"First playlist.m3u"_ and  _"Second playlist.m3u8"_ with new **"Third playlist.m3u"**:
+
+    ```bash
+    mkpl -d "new_collection" -r "Third playlist" -j "First playlist.m3u" "Second playlist.m3u8"
+
 ## Use it like Python module
 
 `mkpl` can also be used as a Python module to customize your scripts.
 
 ```python
 from make_playlist import *
 
 # Prepare playlist list: find multimedia files with name starts between a and f
 playlist = make_playlist('/Music/collections',
-                         '^[a-f].*',
                          ('mp3', 'mp4', 'aac'),
+                         '^[a-f].*',
                          recursive=True,
                          unique=True)
 
 # Write playlist to file
 write_playlist('/Music/AtoF.m3u', 'wt', playlist)
 ```
    
@@ -201,16 +207,14 @@
 
 For [Telethon](http://www.telethon.it/)
 
 The Telethon Foundation is a non-profit organization recognized by the Ministry of University and Scientific and Technological Research.
 They were born in 1990 to respond to the appeal of patients suffering from rare diseases.
 Come today, we are organized to dare to listen to them and answers, every day of the year.
 
-<a href="https://www.telethon.it/sostienici/dona-ora"> <img src="https://www.telethon.it/dev/_nuxt/img/c6d474e.svg" alt="Telethon" title="Telethon" width="200" height="104" /> </a>
-
 [Adopt the future](https://www.ioadottoilfuturo.it/)
 
 
 ## Treeware  
 
 This package is [Treeware](https://treeware.earth). If you use it in production, 
 then we ask that you [**buy the world a tree**](https://plant.treeware.earth/matteoguadrini/mkpl) to thank us for our work.
```

### Comparing `make_playlist-1.7.0/README.md` & `make_playlist-1.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-# ``make_playlist``: Make playlist command line tool
+# ``make_playlist``: Playlist maker
+
+<img src="img/mkpl_logo.svg" alt="mkpl" title="mkpl" width="200" height="200" />
 
 ``mkpl`` is a _command line tool_ to create playlist files (**[M3U](https://en.wikipedia.org/wiki/M3U) format**).
 
 ## Installation
 
 To install ``mkpl``, see here:
 
 ```console
 $ pip install make_playlist               # for python enviroment
 
 $ dnf copr enable matteoguadrini/mkpl
 $ dnf install python-make_playlist -y     # for Red Hat and fedora
 
 $ git clone https://github.com/MatteoGuadrini/mkpl.git && cd mkpl
-$ python setup.py install                 # for others
+$ pip install .                           # for others
 ```
 
 ## Command arguments
 
 ``mkpl`` have many command line arguments. They are explained in this table:
 
 | short | long            | description                                   | args                      |
@@ -28,26 +30,28 @@
 | -p    | --pattern       | Regular expression inclusion pattern          | Regular expression string |
 | -f    | --format        | Select only a file format                     | Format of file. ex. mp3   |
 | -s    | --size          | Start size in bytes                           | Bytes number              |
 | -m    | --max-tracks    | Maximum number of tracks                      | Number                    |
 | -t    | --title         | Playlist title                                | Title string              |
 | -g    | --encoding      | Text encoding                                 | UTF-8,ASCII,UNICODE       |
 | -I    | --image         | Playlist image                                | Image path                |
-| -l    | --link          | Add remote file links                         | Links                     |
+| -l    | --link          | Add local or remote files                     | Files                     |
+| -j    | --join          | Join one or more other playlist files         | Playlist files            |
 | -r    | --recursive     | Recursive search                              |                           |
 | -a    | --absolute      | Absolute file name                            |                           |
 | -s    | --shuffle       | Casual order                                  |                           |
 | -u    | --unique        | The same files are not placed in the playlist |                           |
 | -c    | --append        | Continue playlist instead of override it      |                           |
 | -w    | --windows       | Windows style folder separator                |                           |
 | -v    | --verbose       | Enable verbosity (debug mode)                 |                           |
 | -S    | --split         | Split playlist by directories                 |                           |
 | -o    | --orderby-name  | Order playlist files by name                  |                           |
 | -O    | --orderby-date  | Order playlist files by creation date         |                           |
 | -T    | --orderby-track | Order playlist files by track                 |                           |
+| -y    | --orderby-year  | Order playlist files by year                  |                           |
 
 ## Examples
 
 1. Create a playlist for one music album:
 
     ```bash
     cd myalbum
@@ -138,33 +142,39 @@
     my_music.m3u
     folder1.m3u
     folder2.m3u
     folder3.m3u
     ...
     ```
 
-15. Sort playlist files by name (`-o`), by creation date (`-O`) or by track number (`-T`):
+15. Sort playlist files by name (`-o`), by creation date (`-O`), by track number (`-T`) or by year (`-y`):
 
     ```bash
     mkpl -d "new_collection" -r "my music.m3u" -o
     mkpl -d "new_collection" -r "my music.m3u" -O
     mkpl -d "new_collection" -r "my music.m3u" -T
+    mkpl -d "new_collection" -r "my music.m3u" -y
     ```
 
+16. Join the _"First playlist.m3u"_ and  _"Second playlist.m3u8"_ with new **"Third playlist.m3u"**:
+
+    ```bash
+    mkpl -d "new_collection" -r "Third playlist" -j "First playlist.m3u" "Second playlist.m3u8"
+
 ## Use it like Python module
 
 `mkpl` can also be used as a Python module to customize your scripts.
 
 ```python
 from make_playlist import *
 
 # Prepare playlist list: find multimedia files with name starts between a and f
 playlist = make_playlist('/Music/collections',
-                         '^[a-f].*',
                          ('mp3', 'mp4', 'aac'),
+                         '^[a-f].*',
                          recursive=True,
                          unique=True)
 
 # Write playlist to file
 write_playlist('/Music/AtoF.m3u', 'wt', playlist)
 ```
    
@@ -181,16 +191,14 @@
 
 For [Telethon](http://www.telethon.it/)
 
 The Telethon Foundation is a non-profit organization recognized by the Ministry of University and Scientific and Technological Research.
 They were born in 1990 to respond to the appeal of patients suffering from rare diseases.
 Come today, we are organized to dare to listen to them and answers, every day of the year.
 
-<a href="https://www.telethon.it/sostienici/dona-ora"> <img src="https://www.telethon.it/dev/_nuxt/img/c6d474e.svg" alt="Telethon" title="Telethon" width="200" height="104" /> </a>
-
 [Adopt the future](https://www.ioadottoilfuturo.it/)
 
 
 ## Treeware  
 
 This package is [Treeware](https://treeware.earth). If you use it in production, 
 then we ask that you [**buy the world a tree**](https://plant.treeware.earth/matteoguadrini/mkpl) to thank us for our work.
```

### Comparing `make_playlist-1.7.0/make_playlist.egg-info/PKG-INFO` & `make_playlist-1.8.0/make_playlist.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 Metadata-Version: 2.1
 Name: make-playlist
-Version: 1.7.0
-Summary: Make M3U format playlist from command line
-Home-page: https://github.com/MatteoGuadrini/mkpl
-Author: Matteo Guadrini
-Author-email: matteo.guadrini@hotmail.it
-Maintainer: Matteo Guadrini
-Maintainer-email: matteo.guadrini@hotmail.it
-License: GNU General Public License v3.0
-Project-URL: Documentation, https://github.com/MatteoGuadrini/mkpl
-Project-URL: GitHub Project, https://github.com/MatteoGuadrini/mkpl
-Project-URL: Issue Tracker, https://github.com/MatteoGuadrini/mkpl/issues
+Version: 1.8.0
+Summary: Make M3U format playlist from command line.
+Author-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
+Maintainer-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
+Project-URL: homepage, https://github.com/MatteoGuadrini/mkpl
+Project-URL: documentation, https://matteoguadrini.github.io/mkpl/
+Project-URL: changelog, https://github.com/MatteoGuadrini/mkpl/blob/master/CHANGES.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# ``make_playlist``: Make playlist command line tool
+# ``make_playlist``: Playlist maker
+
+<img src="img/mkpl_logo.svg" alt="mkpl" title="mkpl" width="200" height="200" />
 
 ``mkpl`` is a _command line tool_ to create playlist files (**[M3U](https://en.wikipedia.org/wiki/M3U) format**).
 
 ## Installation
 
 To install ``mkpl``, see here:
 
 ```console
 $ pip install make_playlist               # for python enviroment
 
 $ dnf copr enable matteoguadrini/mkpl
 $ dnf install python-make_playlist -y     # for Red Hat and fedora
 
 $ git clone https://github.com/MatteoGuadrini/mkpl.git && cd mkpl
-$ python setup.py install                 # for others
+$ pip install .                           # for others
 ```
 
 ## Command arguments
 
 ``mkpl`` have many command line arguments. They are explained in this table:
 
 | short | long            | description                                   | args                      |
@@ -48,26 +46,28 @@
 | -p    | --pattern       | Regular expression inclusion pattern          | Regular expression string |
 | -f    | --format        | Select only a file format                     | Format of file. ex. mp3   |
 | -s    | --size          | Start size in bytes                           | Bytes number              |
 | -m    | --max-tracks    | Maximum number of tracks                      | Number                    |
 | -t    | --title         | Playlist title                                | Title string              |
 | -g    | --encoding      | Text encoding                                 | UTF-8,ASCII,UNICODE       |
 | -I    | --image         | Playlist image                                | Image path                |
-| -l    | --link          | Add remote file links                         | Links                     |
+| -l    | --link          | Add local or remote files                     | Files                     |
+| -j    | --join          | Join one or more other playlist files         | Playlist files            |
 | -r    | --recursive     | Recursive search                              |                           |
 | -a    | --absolute      | Absolute file name                            |                           |
 | -s    | --shuffle       | Casual order                                  |                           |
 | -u    | --unique        | The same files are not placed in the playlist |                           |
 | -c    | --append        | Continue playlist instead of override it      |                           |
 | -w    | --windows       | Windows style folder separator                |                           |
 | -v    | --verbose       | Enable verbosity (debug mode)                 |                           |
 | -S    | --split         | Split playlist by directories                 |                           |
 | -o    | --orderby-name  | Order playlist files by name                  |                           |
 | -O    | --orderby-date  | Order playlist files by creation date         |                           |
 | -T    | --orderby-track | Order playlist files by track                 |                           |
+| -y    | --orderby-year  | Order playlist files by year                  |                           |
 
 ## Examples
 
 1. Create a playlist for one music album:
 
     ```bash
     cd myalbum
@@ -158,33 +158,39 @@
     my_music.m3u
     folder1.m3u
     folder2.m3u
     folder3.m3u
     ...
     ```
 
-15. Sort playlist files by name (`-o`), by creation date (`-O`) or by track number (`-T`):
+15. Sort playlist files by name (`-o`), by creation date (`-O`), by track number (`-T`) or by year (`-y`):
 
     ```bash
     mkpl -d "new_collection" -r "my music.m3u" -o
     mkpl -d "new_collection" -r "my music.m3u" -O
     mkpl -d "new_collection" -r "my music.m3u" -T
+    mkpl -d "new_collection" -r "my music.m3u" -y
     ```
 
+16. Join the _"First playlist.m3u"_ and  _"Second playlist.m3u8"_ with new **"Third playlist.m3u"**:
+
+    ```bash
+    mkpl -d "new_collection" -r "Third playlist" -j "First playlist.m3u" "Second playlist.m3u8"
+
 ## Use it like Python module
 
 `mkpl` can also be used as a Python module to customize your scripts.
 
 ```python
 from make_playlist import *
 
 # Prepare playlist list: find multimedia files with name starts between a and f
 playlist = make_playlist('/Music/collections',
-                         '^[a-f].*',
                          ('mp3', 'mp4', 'aac'),
+                         '^[a-f].*',
                          recursive=True,
                          unique=True)
 
 # Write playlist to file
 write_playlist('/Music/AtoF.m3u', 'wt', playlist)
 ```
    
@@ -201,16 +207,14 @@
 
 For [Telethon](http://www.telethon.it/)
 
 The Telethon Foundation is a non-profit organization recognized by the Ministry of University and Scientific and Technological Research.
 They were born in 1990 to respond to the appeal of patients suffering from rare diseases.
 Come today, we are organized to dare to listen to them and answers, every day of the year.
 
-<a href="https://www.telethon.it/sostienici/dona-ora"> <img src="https://www.telethon.it/dev/_nuxt/img/c6d474e.svg" alt="Telethon" title="Telethon" width="200" height="104" /> </a>
-
 [Adopt the future](https://www.ioadottoilfuturo.it/)
 
 
 ## Treeware  
 
 This package is [Treeware](https://treeware.earth). If you use it in production, 
 then we ask that you [**buy the world a tree**](https://plant.treeware.earth/matteoguadrini/mkpl) to thank us for our work.
```

### Comparing `make_playlist-1.7.0/mkpl.py` & `make_playlist-1.8.0/mkpl.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,23 +20,24 @@
 #     You should have received a copy of the GNU General Public License
 #     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """mkpl module. This is command line utility for playlist creation."""
 
 # region imports
 import argparse
+import os.path
 import re
 from filecmp import cmp
 from os.path import basename, dirname, exists, getctime, getsize, isdir, join, normpath
 from pathlib import Path
 from random import shuffle
 from re import sub
 from string import capwords
 
-from mutagen import File
+from mutagen import File, MutagenError, id3
 
 # endregion
 
 # region globals
 AUDIO_FORMAT = {
     "mp1",
     "mp2",
@@ -46,31 +47,48 @@
     "wav",
     "wma",
     "m4a",
     "aiff",
     "flac",
     "alac",
     "opus",
+    "ape",
+    "webm",
+}
+VIDEO_FORMAT = {
+    "mp4",
+    "avi",
+    "xvid",
+    "divx",
+    "mpeg",
+    "mpg",
+    "mov",
+    "wmv",
+    "flv",
+    "vob",
+    "asf",
+    "m4v",
+    "3gp",
+    "f4a",
 }
-VIDEO_FORMAT = {"mp4", "avi", "xvid", "divx", "mpeg", "mpg", "mov", "wmv"}
 FILE_FORMAT = AUDIO_FORMAT.union(VIDEO_FORMAT)
-__version__ = "1.7.0"
+__version__ = "1.8.0"
 
 
 # endregion
 
 
 # region functions
 def get_args():
     """Get command-line arguments"""
 
     global FILE_FORMAT
 
     parser = argparse.ArgumentParser(
-        description="Command line tool to create media playlists in M3U format.",
+        description="Command line tool to creates playlist file in M3U format.",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         epilog="See latest release from https://github.com/MatteoGuadrini/mkpl",
     )
     orderby_group = parser.add_mutually_exclusive_group()
 
     parser.add_argument("playlist", help="Playlist file", type=str)
     parser.add_argument("-v", "--verbose", help="Enable verbosity", action="store_true")
@@ -95,15 +113,15 @@
         "-i",
         "--include",
         help="Include other file format",
         nargs=argparse.ONE_OR_MORE,
         metavar="FORMAT",
     )
     parser.add_argument(
-        "-p", "--pattern", help="Regular expression inclusion pattern", default=".*"
+        "-p", "--pattern", help="Regular expression inclusion pattern", default=None
     )
     parser.add_argument(
         "-f",
         "--format",
         help="Select only a file format",
         type=str,
         choices=FILE_FORMAT,
@@ -127,16 +145,25 @@
         choices=("UTF-8", "ASCII", "UNICODE"),
         default=None,
     )
     parser.add_argument("-I", "--image", help="Playlist image", default=None)
     parser.add_argument(
         "-l",
         "--link",
-        help="Add remote file links",
+        help="Add local or remote file links",
+        nargs=argparse.ONE_OR_MORE,
+        metavar='FILES',
+        default=[],
+    )
+    parser.add_argument(
+        "-j",
+        "--join",
+        help="Join one or more other playlist files",
         nargs=argparse.ONE_OR_MORE,
+        metavar='PLAYLISTS',
         default=[],
     )
     parser.add_argument(
         "-r", "--recursive", help="Recursive search", action="store_true"
     )
     parser.add_argument(
         "-a", "--absolute", help="Absolute file name", action="store_true"
@@ -170,14 +197,20 @@
     )
     orderby_group.add_argument(
         "-T",
         "--orderby-track",
         help="Order playlist files by track",
         action="store_true",
     )
+    orderby_group.add_argument(
+        "-y",
+        "--orderby-year",
+        help="Order playlist files by year",
+        action="store_true",
+    )
 
     args = parser.parse_args()
 
     # Check extension of playlist file
     if not args.playlist.endswith(".m3u"):
         if args.encoding == "UNICODE":
             if not args.playlist.endswith(".m3u8"):
@@ -237,102 +270,161 @@
     for f in playlist:
         # Skip extended tags
         if f.startswith("#"):
             continue
         # Check if absolute path in playlist
         if root:
             f = join(root, f)
+        # Make standard the path
+        f = unix_to_dos(f, viceversa=True)
         # Compare two files
         if cmp(f, file):
             return True
 
 
+def join_playlist(playlist, *others):
+    """Join current playlist with others"""
+    for file in others:
+        try:
+            # open playlist, remove extensions and extend current playlist file
+            lines = open(file).readlines()
+            playlist.extend([line.rstrip() for line in lines if not line.startswith('#')])
+        except FileNotFoundError:
+            print(f"warning: {file} file not found")
+        except OSError as err:
+            print(f"warning: {file} generated error: {err}")
+
+
 def report_issue(exc):
     """Report issue"""
     print(
         "error: {0} on line {1}, with error {2}".format(
             type(exc).__name__, exc.__traceback__.tb_lineno, str(exc)
         )
     )
     exit(1)
 
 
+def open_multimedia_file(path):
+    """Open multimedia file
+
+    :param path: multimedia file to open
+    """
+    try:
+        file = File(path)
+    except MutagenError:
+        print(f"warning: file '{path}' loading failed")
+        return False
+    return file
+
+
 def get_track(file):
-    """Sort file by track"""
-    file = File(file)
-    if hasattr(file, "tags"):
-        return file.tags.get("TRCK", "0")[0]
+    """Get file by track for sort"""
+    file = open_multimedia_file(file)
+    if file and hasattr(file, "tags"):
+        default = id3.TRCK(text="0")
+        return file.tags.get("TRCK", default)[0]
+
+
+def get_year(file):
+    """Get file by year for sort"""
+    file = open_multimedia_file(file)
+    if file and hasattr(file, "tags"):
+        default = id3.TDOR(text="0")
+        return file.tags.get("TDOR", default)[0]
 
 
 def find_pattern(pattern, path):
     """Find patter in a file and tags"""
-    file = File(path)
+    global AUDIO_FORMAT
+
     # Create compiled pattern
     if not isinstance(pattern, re.Pattern):
         pattern = re.compile(pattern)
     # Check pattern into filename
-    if pattern.findall(file.filename):
+    if pattern.findall(path):
         return True
-    # Check supports of ID3 tagsadd compiled pattern
-    if hasattr(file, "ID3"):
-        # Check pattern into title
-        for title in file.tags.get("TIT2"):
-            if pattern.findall(title):
-                return True
-        # Check pattern into album
-        for album in file.tags.get("TALB"):
-            if pattern.findall(album):
-                return True
+    # Check type of file
+    ext = os.path.splitext(path)[1].replace('.', '').lower()
+    if ext in AUDIO_FORMAT:
+        file = open_multimedia_file(path)
+        # Check supports of ID3 tagsadd compiled pattern
+        if file and hasattr(file, "ID3"):
+            # Check pattern into title
+            if file.tags.get("TIT2"):
+                if pattern.findall(file.tags.get("TIT2")[0]):
+                    return True
+            # Check pattern into album
+            if file.tags.get("TALB"):
+                if pattern.findall(file.tags.get("TALB")[0]):
+                    return True
 
 
 def vprint(verbose, *messages):
     """Verbose print"""
     if verbose:
         print("debug:", *messages)
 
 
+def unix_to_dos(path, viceversa=False):
+    """Substitute folder separator with windows separator
+
+    :param path: path to substitute folder separator
+    :param viceversa: dos to unix
+    """
+    if viceversa:
+        old_sep = r"\\"
+        new_sep = "/"
+    else:
+        old_sep = "/"
+        new_sep = r"\\"
+    return sub(old_sep, new_sep, path)
+
+
 def write_playlist(
         playlist,
         open_mode,
         files,
         encoding,
         enabled_extensions=False,
         image=None,
         ext_part=None,
         max_tracks=None,
         verbose=False,
 ):
     """Write playlist into file"""
-    with open(
-            playlist,
-            mode=open_mode,
-            encoding="UTF-8" if encoding == "UNICODE" else encoding,
-            errors="ignore",
-    ) as pl:
-        if image and enabled_extensions:
-            vprint(verbose, f"set image {image}")
-            joined_string = f"\n#EXTIMG: {image}\n"
-        else:
-            joined_string = "\n"
-        end_file_string = "\n"
-        # Write extensions if exists
-        if ext_part:
-            pl.write("\n".join(files[:ext_part]) + joined_string)
-        # Write all multimedia files
-        vprint(verbose, f"write playlist {pl.name}")
-        pl.write(joined_string.join(files[ext_part:max_tracks]) + end_file_string)
+    if playlist:
+        with open(
+                playlist,
+                mode=open_mode,
+                encoding="UTF-8" if encoding == "UNICODE" else encoding,
+                errors="ignore",
+        ) as pl:
+            if image and enabled_extensions:
+                vprint(verbose, f"set image {image}")
+                joined_string = f"\n#EXTIMG: {image}\n"
+            else:
+                joined_string = "\n"
+            end_file_string = "\n"
+            # Write extensions if exists
+            if ext_part:
+                pl.write("\n".join(files[:ext_part]) + joined_string)
+            # Write all multimedia files
+            vprint(verbose, f"write playlist {pl.name}")
+            pl.write(joined_string.join(files[ext_part:max_tracks]) + end_file_string)
 
 
 def make_playlist(
         directory,
-        pattern,
         file_formats,
+        pattern=None,
         sortby_name=False,
         sortby_date=False,
         sortby_track=False,
+        sortby_year=False,
         recursive=False,
         exclude_dirs=None,
         unique=False,
         absolute=False,
         min_size=1,
         windows=False,
         verbose=False,
@@ -351,43 +443,49 @@
     path = Path(directory)
     root = path.parent
     vprint(verbose, f"current directory={path}, root={root}")
     for fmt in file_formats:
         # Check recursive
         folder = "**/*" if recursive else "*"
         files = path.glob(folder + f".{fmt}")
+        # Process found files
         for file in files:
+            # Get size of file
+            size = file.stat().st_size
+            # Check absolute file names
+            file = str(file.resolve()) if absolute else str(file)
+            # Check file match pattern
+            if pattern:
+                # Check re pattern
+                compiled_pattern = re.compile(pattern)
+                if not find_pattern(compiled_pattern, file):
+                    continue
             # Check if in exclude dirs
-            if any([e_path in str(file) for e_path in exclude_dirs]):
+            if any([e_path in file for e_path in exclude_dirs]):
                 continue
             # Check if file is in playlist
             if unique:
                 if file_in_playlist(
-                        filelist, str(file), root=root if not absolute else None
+                        filelist, file, root=root if not absolute else None
                 ):
                     continue
-            # Get size of file
-            size = file.stat().st_size
-            # Check absolute file names
-            file_for_pattern = str(file)
-            file = str(file) if absolute else str(file.relative_to(path.parent))
-            # Check re pattern
-            compiled_pattern = re.compile(pattern)
-            if find_pattern(compiled_pattern, file_for_pattern):
-                # Check file size
-                if size >= min_size:
-                    vprint(verbose, f"add multimedia file {file}")
-                    filelist.append(sub("/", r"\\", file) if windows else file)
+            # Check file size
+            if size <= min_size:
+                continue
+            vprint(verbose, f"add multimedia file {file}")
+            filelist.append(unix_to_dos(file) if windows else file)
     # Check sort
     if sortby_name:
         filelist = sorted(filelist)
     elif sortby_date:
         filelist = sorted(filelist, key=getctime)
     elif sortby_track:
         filelist = sorted(filelist, key=get_track)
+    elif sortby_year:
+        filelist = sorted(filelist, key=get_year)
     return filelist
 
 
 def add_extension(filelist, cli_args, verbose=False):
     """Add extension to playlist list"""
     if not isinstance(filelist, list):
         raise ValueError(f"{filelist} is not a list object")
@@ -426,14 +524,18 @@
             else:
                 print("warning: encoding is already configured")
 
 
 def _process_playlist(files, cli_args, other_playlist=None):
     """Private function cli only for process arguments and make playlist"""
 
+    # Join other playlist files
+    if cli_args.join:
+        join_playlist(files, *cli_args.join)
+
     # Add link
     files.extend(cli_args.link)
 
     # Build a playlist
     if files:
         # Check shuffle
         if cli_args.shuffle:
@@ -473,19 +575,20 @@
             f"pattern={args.pattern}, split={args.split}",
         )
 
         # Make multimedia list
         for directory in args.directories:
             directory_files = make_playlist(
                 directory,
-                args.pattern,
                 FILE_FORMAT,
+                args.pattern,
                 sortby_name=args.orderby_name,
                 sortby_date=args.orderby_date,
                 sortby_track=args.orderby_track,
+                sortby_year=args.orderby_year,
                 recursive=args.recursive,
                 exclude_dirs=args.exclude_dirs,
                 unique=args.unique,
                 absolute=args.absolute,
                 min_size=args.size,
                 windows=args.windows,
                 verbose=args.verbose,
```

