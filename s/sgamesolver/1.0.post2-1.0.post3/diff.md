# Comparing `tmp/sgamesolver-1.0.post2.tar.gz` & `tmp/sgamesolver-1.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgamesolver-1.0.post2.tar", last modified: Mon Jul 11 09:52:08 2022, max compression
+gzip compressed data, was "sgamesolver-1.0.post3.tar", last modified: Mon Jul 18 22:43:21 2022, max compression
```

## Comparing `sgamesolver-1.0.post2.tar` & `sgamesolver-1.0.post3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-07-11 09:52:08.575658 sgamesolver-1.0.post2/
--rw-rw-rw-   0        0        0     1116 2021-04-29 19:01:19.000000 sgamesolver-1.0.post2/LICENSE
--rw-rw-rw-   0        0        0       44 2022-06-05 21:59:47.000000 sgamesolver-1.0.post2/MANIFEST.in
--rw-rw-rw-   0        0        0     7529 2022-07-11 09:52:08.574661 sgamesolver-1.0.post2/PKG-INFO
--rw-rw-rw-   0        0        0     6066 2022-06-05 19:27:48.000000 sgamesolver-1.0.post2/README.md
--rw-rw-rw-   0        0        0       42 2022-07-11 09:52:08.575658 sgamesolver-1.0.post2/setup.cfg
--rw-rw-rw-   0        0        0     5770 2022-07-11 09:46:52.000000 sgamesolver-1.0.post2/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-11 09:52:08.542747 sgamesolver-1.0.post2/sgamesolver/
--rw-rw-rw-   0        0        0      136 2022-06-05 10:47:39.000000 sgamesolver-1.0.post2/sgamesolver/__init__.py
--rw-rw-rw-   0        0        0    41573 2022-06-05 14:34:18.000000 sgamesolver-1.0.post2/sgamesolver/homcont.py
-drwxrwxrwx   0        0        0        0 2022-07-11 09:52:08.569676 sgamesolver-1.0.post2/sgamesolver/homotopy/
--rw-rw-rw-   0        0        0       60 2022-06-05 14:14:21.000000 sgamesolver-1.0.post2/sgamesolver/homotopy/__init__.py
--rw-rw-rw-   0        0        0    17401 2022-06-05 18:55:41.000000 sgamesolver-1.0.post2/sgamesolver/homotopy/_logtracing.py
--rw-rw-rw-   0        0        0  1159956 2022-06-05 21:37:02.000000 sgamesolver-1.0.post2/sgamesolver/homotopy/_logtracing_ct.c
--rw-rw-rw-   0        0        0    15276 2022-05-13 14:59:24.000000 sgamesolver-1.0.post2/sgamesolver/homotopy/_logtracing_ct.pyx
--rw-rw-rw-   0        0        0    12950 2022-06-05 18:55:41.000000 sgamesolver-1.0.post2/sgamesolver/homotopy/_qre.py
--rw-rw-rw-   0        0        0  1123152 2022-06-05 21:37:04.000000 sgamesolver-1.0.post2/sgamesolver/homotopy/_qre_ct.c
--rw-rw-rw-   0        0        0    15732 2022-05-13 14:59:24.000000 sgamesolver-1.0.post2/sgamesolver/homotopy/_qre_ct.pyx
--rw-rw-rw-   0        0        0  1048627 2022-06-05 21:37:06.000000 sgamesolver-1.0.post2/sgamesolver/homotopy/_shared_ct.c
--rw-rw-rw-   0        0        0     1631 2022-05-06 20:14:33.000000 sgamesolver-1.0.post2/sgamesolver/homotopy/_shared_ct.pxd
--rw-rw-rw-   0        0        0    17369 2022-06-05 18:55:41.000000 sgamesolver-1.0.post2/sgamesolver/homotopy/_shared_ct.pyx
--rw-rw-rw-   0        0        0    25052 2022-06-05 19:13:37.000000 sgamesolver-1.0.post2/sgamesolver/sgame.py
-drwxrwxrwx   0        0        0        0 2022-07-11 09:52:08.573664 sgamesolver-1.0.post2/sgamesolver/utility/
--rw-rw-rw-   0        0        0    18384 2022-06-05 14:23:26.000000 sgamesolver-1.0.post2/sgamesolver/utility/excel_timings.py
--rw-rw-rw-   0        0        0    10255 2022-06-04 16:12:45.000000 sgamesolver-1.0.post2/sgamesolver/utility/sgame_conversion.py
-drwxrwxrwx   0        0        0        0 2022-07-11 09:52:08.552720 sgamesolver-1.0.post2/sgamesolver.egg-info/
--rw-rw-rw-   0        0        0     7529 2022-07-11 09:52:07.000000 sgamesolver-1.0.post2/sgamesolver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      878 2022-07-11 09:52:08.000000 sgamesolver-1.0.post2/sgamesolver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-11 09:52:07.000000 sgamesolver-1.0.post2/sgamesolver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2022-07-11 09:52:07.000000 sgamesolver-1.0.post2/sgamesolver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-06-05 19:29:07.000000 sgamesolver-1.0.post2/sgamesolver.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       37 2022-07-11 09:52:08.000000 sgamesolver-1.0.post2/sgamesolver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-07-11 09:52:08.000000 sgamesolver-1.0.post2/sgamesolver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-07-18 22:43:21.029866 sgamesolver-1.0.post3/
+-rw-rw-rw-   0        0        0     1116 2021-04-29 19:01:19.000000 sgamesolver-1.0.post3/LICENSE
+-rw-rw-rw-   0        0        0       44 2022-06-05 21:59:47.000000 sgamesolver-1.0.post3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7529 2022-07-18 22:43:21.028432 sgamesolver-1.0.post3/PKG-INFO
+-rw-rw-rw-   0        0        0     6066 2022-06-05 19:27:48.000000 sgamesolver-1.0.post3/README.md
+-rw-rw-rw-   0        0        0       42 2022-07-18 22:43:21.029866 sgamesolver-1.0.post3/setup.cfg
+-rw-rw-rw-   0        0        0     5770 2022-07-18 22:40:33.000000 sgamesolver-1.0.post3/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-18 22:43:20.944049 sgamesolver-1.0.post3/sgamesolver/
+-rw-rw-rw-   0        0        0      136 2022-07-18 22:40:33.000000 sgamesolver-1.0.post3/sgamesolver/__init__.py
+-rw-rw-rw-   0        0        0    41573 2022-06-05 14:34:18.000000 sgamesolver-1.0.post3/sgamesolver/homcont.py
+drwxrwxrwx   0        0        0        0 2022-07-18 22:43:21.022446 sgamesolver-1.0.post3/sgamesolver/homotopy/
+-rw-rw-rw-   0        0        0       60 2022-06-05 14:14:21.000000 sgamesolver-1.0.post3/sgamesolver/homotopy/__init__.py
+-rw-rw-rw-   0        0        0    17401 2022-06-05 18:55:41.000000 sgamesolver-1.0.post3/sgamesolver/homotopy/_logtracing.py
+-rw-rw-rw-   0        0        0  1159956 2022-06-05 21:37:02.000000 sgamesolver-1.0.post3/sgamesolver/homotopy/_logtracing_ct.c
+-rw-rw-rw-   0        0        0    15276 2022-05-13 14:59:24.000000 sgamesolver-1.0.post3/sgamesolver/homotopy/_logtracing_ct.pyx
+-rw-rw-rw-   0        0        0    12950 2022-06-05 18:55:41.000000 sgamesolver-1.0.post3/sgamesolver/homotopy/_qre.py
+-rw-rw-rw-   0        0        0  1123152 2022-06-05 21:37:04.000000 sgamesolver-1.0.post3/sgamesolver/homotopy/_qre_ct.c
+-rw-rw-rw-   0        0        0    15732 2022-05-13 14:59:24.000000 sgamesolver-1.0.post3/sgamesolver/homotopy/_qre_ct.pyx
+-rw-rw-rw-   0        0        0  1048627 2022-06-05 21:37:06.000000 sgamesolver-1.0.post3/sgamesolver/homotopy/_shared_ct.c
+-rw-rw-rw-   0        0        0     1631 2022-05-06 20:14:33.000000 sgamesolver-1.0.post3/sgamesolver/homotopy/_shared_ct.pxd
+-rw-rw-rw-   0        0        0    17369 2022-06-05 18:55:41.000000 sgamesolver-1.0.post3/sgamesolver/homotopy/_shared_ct.pyx
+-rw-rw-rw-   0        0        0    25052 2022-06-05 19:13:37.000000 sgamesolver-1.0.post3/sgamesolver/sgame.py
+drwxrwxrwx   0        0        0        0 2022-07-18 22:43:21.026868 sgamesolver-1.0.post3/sgamesolver/utility/
+-rw-rw-rw-   0        0        0    18384 2022-06-05 14:23:26.000000 sgamesolver-1.0.post3/sgamesolver/utility/excel_timings.py
+-rw-rw-rw-   0        0        0    10263 2022-07-18 22:33:17.000000 sgamesolver-1.0.post3/sgamesolver/utility/sgame_conversion.py
+drwxrwxrwx   0        0        0        0 2022-07-18 22:43:20.982945 sgamesolver-1.0.post3/sgamesolver.egg-info/
+-rw-rw-rw-   0        0        0     7529 2022-07-18 22:43:19.000000 sgamesolver-1.0.post3/sgamesolver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      878 2022-07-18 22:43:20.000000 sgamesolver-1.0.post3/sgamesolver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-18 22:43:19.000000 sgamesolver-1.0.post3/sgamesolver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2022-07-18 22:43:19.000000 sgamesolver-1.0.post3/sgamesolver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-06-05 19:29:07.000000 sgamesolver-1.0.post3/sgamesolver.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       37 2022-07-18 22:43:19.000000 sgamesolver-1.0.post3/sgamesolver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-07-18 22:43:20.000000 sgamesolver-1.0.post3/sgamesolver.egg-info/top_level.txt
```

### Comparing `sgamesolver-1.0.post2/LICENSE` & `sgamesolver-1.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `sgamesolver-1.0.post2/PKG-INFO` & `sgamesolver-1.0.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgamesolver
-Version: 1.0.post2
+Version: 1.0.post3
 Summary: A homotopy-based solver for stochastic games
 Home-page: https://github.com/davidpoensgen/sgamesolver
 Author: Steffen Eibelshäuser, David Poensgen
 Author-email: steffen.eibelshaeuser@gmail.com, davidpoensgenecon@gmail.com
 License: UNKNOWN
 Project-URL: github, https://github.com/davidpoensgen/sgamesolver/
 Project-URL: Bug Tracker, https://github.com/davidpoensgen/sgamesolver/issues
```

### Comparing `sgamesolver-1.0.post2/README.md` & `sgamesolver-1.0.post3/README.md`

 * *Files identical despite different names*

### Comparing `sgamesolver-1.0.post2/setup.py` & `sgamesolver-1.0.post3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         ['sgamesolver/homotopy/_logtracing_ct.pyx'],
         include_dirs=[np.get_include()]
     ),
 ]
 
 setup(
     name='sgamesolver',
-    version='1.0.post2',
+    version='1.0.post3',
     description='A homotopy-based solver for stochastic games',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/davidpoensgen/sgamesolver',
     project_urls={
         'github': 'https://github.com/davidpoensgen/sgamesolver/',
         'Bug Tracker': 'https://github.com/davidpoensgen/sgamesolver/issues',
```

### Comparing `sgamesolver-1.0.post2/sgamesolver/homcont.py` & `sgamesolver-1.0.post3/sgamesolver/homcont.py`

 * *Files identical despite different names*

### Comparing `sgamesolver-1.0.post2/sgamesolver/homotopy/_logtracing.py` & `sgamesolver-1.0.post3/sgamesolver/homotopy/_logtracing.py`

 * *Files identical despite different names*

### Comparing `sgamesolver-1.0.post2/sgamesolver/homotopy/_logtracing_ct.c` & `sgamesolver-1.0.post3/sgamesolver/homotopy/_logtracing_ct.c`

 * *Files identical despite different names*

### Comparing `sgamesolver-1.0.post2/sgamesolver/homotopy/_logtracing_ct.pyx` & `sgamesolver-1.0.post3/sgamesolver/homotopy/_logtracing_ct.pyx`

 * *Files identical despite different names*

### Comparing `sgamesolver-1.0.post2/sgamesolver/homotopy/_qre.py` & `sgamesolver-1.0.post3/sgamesolver/homotopy/_qre.py`

 * *Files identical despite different names*

### Comparing `sgamesolver-1.0.post2/sgamesolver/homotopy/_qre_ct.c` & `sgamesolver-1.0.post3/sgamesolver/homotopy/_qre_ct.c`

 * *Files identical despite different names*

### Comparing `sgamesolver-1.0.post2/sgamesolver/homotopy/_qre_ct.pyx` & `sgamesolver-1.0.post3/sgamesolver/homotopy/_qre_ct.pyx`

 * *Files identical despite different names*

### Comparing `sgamesolver-1.0.post2/sgamesolver/homotopy/_shared_ct.c` & `sgamesolver-1.0.post3/sgamesolver/homotopy/_shared_ct.c`

 * *Files identical despite different names*

### Comparing `sgamesolver-1.0.post2/sgamesolver/homotopy/_shared_ct.pxd` & `sgamesolver-1.0.post3/sgamesolver/homotopy/_shared_ct.pxd`

 * *Files identical despite different names*

### Comparing `sgamesolver-1.0.post2/sgamesolver/homotopy/_shared_ct.pyx` & `sgamesolver-1.0.post3/sgamesolver/homotopy/_shared_ct.pyx`

 * *Files identical despite different names*

### Comparing `sgamesolver-1.0.post2/sgamesolver/sgame.py` & `sgamesolver-1.0.post3/sgamesolver/sgame.py`

 * *Files identical despite different names*

### Comparing `sgamesolver-1.0.post2/sgamesolver/utility/excel_timings.py` & `sgamesolver-1.0.post3/sgamesolver/utility/excel_timings.py`

 * *Files identical despite different names*

### Comparing `sgamesolver-1.0.post2/sgamesolver/utility/sgame_conversion.py` & `sgamesolver-1.0.post3/sgamesolver/utility/sgame_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
                     raise ValueError
             except ValueError:
                 row_no = ", ".join(map(str, list(rows['idx_column'] + row_offset)))
                 error_list.append(f'Format (u) > state: {state}, '
                                   f'actions: {", ".join(action_profile)} > row: {row_no}')
             if to_state_format:
                 phi[index + (slice(None),)] = 0
-                to_state = state_list.index(str(rows['to_state']))
+                to_state = state_list.index(str(rows['to_state'].iloc[0]))
                 phi[index + (to_state,)] = 1
             else:
                 try:
                     phi[index + (slice(None),)] = rows[to_state_col_list]
                     if np.isnan(phi[index + (slice(None),)]).any():
                         raise ValueError
                 except ValueError:
```

### Comparing `sgamesolver-1.0.post2/sgamesolver.egg-info/PKG-INFO` & `sgamesolver-1.0.post3/sgamesolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgamesolver
-Version: 1.0.post2
+Version: 1.0.post3
 Summary: A homotopy-based solver for stochastic games
 Home-page: https://github.com/davidpoensgen/sgamesolver
 Author: Steffen Eibelshäuser, David Poensgen
 Author-email: steffen.eibelshaeuser@gmail.com, davidpoensgenecon@gmail.com
 License: UNKNOWN
 Project-URL: github, https://github.com/davidpoensgen/sgamesolver/
 Project-URL: Bug Tracker, https://github.com/davidpoensgen/sgamesolver/issues
```

### Comparing `sgamesolver-1.0.post2/sgamesolver.egg-info/SOURCES.txt` & `sgamesolver-1.0.post3/sgamesolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

