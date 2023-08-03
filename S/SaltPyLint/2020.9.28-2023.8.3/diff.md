# Comparing `tmp/SaltPyLint-2020.9.28.tar.gz` & `tmp/SaltPyLint-2023.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SaltPyLint-2020.9.28.tar", last modified: Mon Sep 28 14:52:10 2020, max compression
+gzip compressed data, was "SaltPyLint-2023.8.3.tar", last modified: Thu Aug  3 14:43:46 2023, max compression
```

## Comparing `SaltPyLint-2020.9.28.tar` & `SaltPyLint-2023.8.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 vampas    (1000) vampas    (1000)        0 2020-09-28 14:52:10.000000 SaltPyLint-2020.9.28/
--rw-r--r--   0 vampas    (1000) vampas    (1000)    12904 2017-06-22 22:55:17.000000 SaltPyLint-2020.9.28/.pylintrc
--rwxr-xr-x   0 vampas    (1000) vampas    (1000)     3547 2020-09-28 14:49:31.000000 SaltPyLint-2020.9.28/setup.py
-drwxr-xr-x   0 vampas    (1000) vampas    (1000)        0 2020-09-28 14:52:10.000000 SaltPyLint-2020.9.28/saltpylint/
--rw-r--r--   0 vampas    (1000) vampas    (1000)     7827 2020-09-28 14:37:39.000000 SaltPyLint-2020.9.28/saltpylint/thirdparty.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)     5082 2019-06-07 20:13:50.000000 SaltPyLint-2020.9.28/saltpylint/fileperms.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)     2414 2019-06-07 20:13:50.000000 SaltPyLint-2020.9.28/saltpylint/virt.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)      428 2020-09-28 14:51:29.000000 SaltPyLint-2020.9.28/saltpylint/version.py
-drwxr-xr-x   0 vampas    (1000) vampas    (1000)        0 2020-09-28 14:52:10.000000 SaltPyLint-2020.9.28/saltpylint/py3modernize/
-drwxr-xr-x   0 vampas    (1000) vampas    (1000)        0 2020-09-28 14:52:10.000000 SaltPyLint-2020.9.28/saltpylint/py3modernize/fixes/
--rw-r--r--   0 vampas    (1000) vampas    (1000)      405 2017-02-22 11:48:59.000000 SaltPyLint-2020.9.28/saltpylint/py3modernize/fixes/fix_dict_salt_six.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)      207 2014-11-20 23:52:11.000000 SaltPyLint-2020.9.28/saltpylint/py3modernize/fixes/fix_xrange_salt_six.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)      182 2014-11-20 23:52:20.000000 SaltPyLint-2020.9.28/saltpylint/py3modernize/fixes/fix_zip_salt_six.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)      182 2014-11-20 23:52:00.000000 SaltPyLint-2020.9.28/saltpylint/py3modernize/fixes/fix_map_salt_six.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)       24 2015-05-06 12:00:50.000000 SaltPyLint-2020.9.28/saltpylint/py3modernize/fixes/__init__.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)      689 2015-05-06 12:02:26.000000 SaltPyLint-2020.9.28/saltpylint/py3modernize/fixes/fix_input_salt_six.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)      197 2014-11-20 23:51:19.000000 SaltPyLint-2020.9.28/saltpylint/py3modernize/fixes/fix_filter_salt_six.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)      483 2017-03-09 13:57:41.000000 SaltPyLint-2020.9.28/saltpylint/py3modernize/fixes/fix_imports_salt_six.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)     9132 2018-08-09 13:16:58.000000 SaltPyLint-2020.9.28/saltpylint/py3modernize/__init__.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)       24 2015-03-28 13:49:51.000000 SaltPyLint-2020.9.28/saltpylint/__init__.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)    25781 2020-09-28 14:46:06.000000 SaltPyLint-2020.9.28/saltpylint/blacklist.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)     2485 2019-06-07 20:13:50.000000 SaltPyLint-2020.9.28/saltpylint/minpyver.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)     1526 2019-06-07 20:13:50.000000 SaltPyLint-2020.9.28/saltpylint/dunder_del.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)    10111 2019-06-07 20:13:50.000000 SaltPyLint-2020.9.28/saltpylint/strings.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)     1258 2018-10-12 14:18:52.000000 SaltPyLint-2020.9.28/saltpylint/smartup.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)     4025 2018-08-09 13:16:58.000000 SaltPyLint-2020.9.28/saltpylint/pep263.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)      646 2018-08-09 13:16:58.000000 SaltPyLint-2020.9.28/saltpylint/checkers.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)     4204 2019-10-21 09:55:17.000000 SaltPyLint-2020.9.28/saltpylint/process.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)    15356 2019-11-13 16:55:46.000000 SaltPyLint-2020.9.28/saltpylint/pep8.py
-drwxr-xr-x   0 vampas    (1000) vampas    (1000)        0 2020-09-28 14:52:10.000000 SaltPyLint-2020.9.28/saltpylint/ext/
--rw-r--r--   0 vampas    (1000) vampas    (1000)    13095 2017-02-22 11:32:42.000000 SaltPyLint-2020.9.28/saltpylint/ext/pyqver2.py
--rw-r--r--   0 vampas    (1000) vampas    (1000)       24 2015-05-06 12:08:45.000000 SaltPyLint-2020.9.28/saltpylint/ext/__init__.py
-drwxr-xr-x   0 vampas    (1000) vampas    (1000)        0 2020-09-28 14:52:10.000000 SaltPyLint-2020.9.28/SaltPyLint.egg-info/
--rw-r--r--   0 vampas    (1000) vampas    (1000)       41 2020-09-28 14:52:10.000000 SaltPyLint-2020.9.28/SaltPyLint.egg-info/requires.txt
--rw-r--r--   0 vampas    (1000) vampas    (1000)     1059 2020-09-28 14:52:10.000000 SaltPyLint-2020.9.28/SaltPyLint.egg-info/SOURCES.txt
--rw-r--r--   0 vampas    (1000) vampas    (1000)      945 2020-09-28 14:52:10.000000 SaltPyLint-2020.9.28/SaltPyLint.egg-info/PKG-INFO
--rw-r--r--   0 vampas    (1000) vampas    (1000)       65 2020-09-28 14:52:10.000000 SaltPyLint-2020.9.28/SaltPyLint.egg-info/top_level.txt
--rw-r--r--   0 vampas    (1000) vampas    (1000)        1 2020-09-28 14:52:10.000000 SaltPyLint-2020.9.28/SaltPyLint.egg-info/dependency_links.txt
--rw-r--r--   0 vampas    (1000) vampas    (1000)       45 2018-10-12 14:39:37.000000 SaltPyLint-2020.9.28/requirements.txt
--rw-r--r--   0 vampas    (1000) vampas    (1000)      161 2020-09-28 14:52:10.000000 SaltPyLint-2020.9.28/setup.cfg
--rw-r--r--   0 vampas    (1000) vampas    (1000)     4151 2017-12-13 11:42:10.000000 SaltPyLint-2020.9.28/.testing.pylintrc
--rw-r--r--   0 vampas    (1000) vampas    (1000)    11325 2015-01-25 01:22:12.000000 SaltPyLint-2020.9.28/LICENSE
--rw-r--r--   0 vampas    (1000) vampas    (1000)      945 2020-09-28 14:52:10.000000 SaltPyLint-2020.9.28/PKG-INFO
--rw-r--r--   0 vampas    (1000) vampas    (1000)      675 2015-01-25 01:22:12.000000 SaltPyLint-2020.9.28/.gitignore
+drwxr-xr-x   0 vampas    (1000) vampas    (1000)        0 2023-08-03 14:43:46.085347 SaltPyLint-2023.8.3/
+-rw-r--r--   0 vampas    (1000) vampas    (1000)      675 2015-01-25 01:22:12.000000 SaltPyLint-2023.8.3/.gitignore
+-rw-r--r--   0 vampas    (1000) vampas    (1000)    12904 2017-06-22 22:55:17.000000 SaltPyLint-2023.8.3/.pylintrc
+-rw-r--r--   0 vampas    (1000) vampas    (1000)     4151 2017-12-13 11:42:10.000000 SaltPyLint-2023.8.3/.testing.pylintrc
+-rw-r--r--   0 vampas    (1000) vampas    (1000)    11325 2015-01-25 01:22:12.000000 SaltPyLint-2023.8.3/LICENSE
+-rw-r--r--   0 vampas    (1000) vampas    (1000)      911 2023-08-03 14:43:46.085347 SaltPyLint-2023.8.3/PKG-INFO
+drwxr-xr-x   0 vampas    (1000) vampas    (1000)        0 2023-08-03 14:43:46.082013 SaltPyLint-2023.8.3/SaltPyLint.egg-info/
+-rw-r--r--   0 vampas    (1000) vampas    (1000)      911 2023-08-03 14:43:46.000000 SaltPyLint-2023.8.3/SaltPyLint.egg-info/PKG-INFO
+-rw-r--r--   0 vampas    (1000) vampas    (1000)     1059 2023-08-03 14:43:46.000000 SaltPyLint-2023.8.3/SaltPyLint.egg-info/SOURCES.txt
+-rw-r--r--   0 vampas    (1000) vampas    (1000)        1 2023-08-03 14:43:46.000000 SaltPyLint-2023.8.3/SaltPyLint.egg-info/dependency_links.txt
+-rw-r--r--   0 vampas    (1000) vampas    (1000)       41 2023-08-03 14:43:46.000000 SaltPyLint-2023.8.3/SaltPyLint.egg-info/requires.txt
+-rw-r--r--   0 vampas    (1000) vampas    (1000)       65 2023-08-03 14:43:46.000000 SaltPyLint-2023.8.3/SaltPyLint.egg-info/top_level.txt
+-rw-r--r--   0 vampas    (1000) vampas    (1000)       45 2018-10-12 14:39:37.000000 SaltPyLint-2023.8.3/requirements.txt
+drwxr-xr-x   0 vampas    (1000) vampas    (1000)        0 2023-08-03 14:43:46.085347 SaltPyLint-2023.8.3/saltpylint/
+-rw-r--r--   0 vampas    (1000) vampas    (1000)       24 2015-03-28 13:49:51.000000 SaltPyLint-2023.8.3/saltpylint/__init__.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)    25781 2020-09-28 14:46:06.000000 SaltPyLint-2023.8.3/saltpylint/blacklist.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)      646 2018-08-09 13:16:58.000000 SaltPyLint-2023.8.3/saltpylint/checkers.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)     1526 2019-06-07 20:13:50.000000 SaltPyLint-2023.8.3/saltpylint/dunder_del.py
+drwxr-xr-x   0 vampas    (1000) vampas    (1000)        0 2023-08-03 14:43:46.085347 SaltPyLint-2023.8.3/saltpylint/ext/
+-rw-r--r--   0 vampas    (1000) vampas    (1000)       24 2015-05-06 12:08:45.000000 SaltPyLint-2023.8.3/saltpylint/ext/__init__.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)    13095 2017-02-22 11:32:42.000000 SaltPyLint-2023.8.3/saltpylint/ext/pyqver2.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)     5082 2019-06-07 20:13:50.000000 SaltPyLint-2023.8.3/saltpylint/fileperms.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)     2485 2019-06-07 20:13:50.000000 SaltPyLint-2023.8.3/saltpylint/minpyver.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)     4025 2018-08-09 13:16:58.000000 SaltPyLint-2023.8.3/saltpylint/pep263.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)    15356 2019-11-13 16:55:46.000000 SaltPyLint-2023.8.3/saltpylint/pep8.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)     4204 2019-10-21 09:55:17.000000 SaltPyLint-2023.8.3/saltpylint/process.py
+drwxr-xr-x   0 vampas    (1000) vampas    (1000)        0 2023-08-03 14:43:46.085347 SaltPyLint-2023.8.3/saltpylint/py3modernize/
+-rw-r--r--   0 vampas    (1000) vampas    (1000)     9132 2018-08-09 13:16:58.000000 SaltPyLint-2023.8.3/saltpylint/py3modernize/__init__.py
+drwxr-xr-x   0 vampas    (1000) vampas    (1000)        0 2023-08-03 14:43:46.085347 SaltPyLint-2023.8.3/saltpylint/py3modernize/fixes/
+-rw-r--r--   0 vampas    (1000) vampas    (1000)       24 2015-05-06 12:00:50.000000 SaltPyLint-2023.8.3/saltpylint/py3modernize/fixes/__init__.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)      405 2017-02-22 11:48:59.000000 SaltPyLint-2023.8.3/saltpylint/py3modernize/fixes/fix_dict_salt_six.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)      197 2014-11-20 23:51:19.000000 SaltPyLint-2023.8.3/saltpylint/py3modernize/fixes/fix_filter_salt_six.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)      483 2017-03-09 13:57:41.000000 SaltPyLint-2023.8.3/saltpylint/py3modernize/fixes/fix_imports_salt_six.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)      689 2015-05-06 12:02:26.000000 SaltPyLint-2023.8.3/saltpylint/py3modernize/fixes/fix_input_salt_six.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)      182 2014-11-20 23:52:00.000000 SaltPyLint-2023.8.3/saltpylint/py3modernize/fixes/fix_map_salt_six.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)      207 2014-11-20 23:52:11.000000 SaltPyLint-2023.8.3/saltpylint/py3modernize/fixes/fix_xrange_salt_six.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)      182 2014-11-20 23:52:20.000000 SaltPyLint-2023.8.3/saltpylint/py3modernize/fixes/fix_zip_salt_six.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)     1258 2018-10-12 14:18:52.000000 SaltPyLint-2023.8.3/saltpylint/smartup.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)    10111 2019-06-07 20:13:50.000000 SaltPyLint-2023.8.3/saltpylint/strings.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)     7822 2023-08-03 14:39:15.000000 SaltPyLint-2023.8.3/saltpylint/thirdparty.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)      427 2023-08-03 14:39:51.000000 SaltPyLint-2023.8.3/saltpylint/version.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)     2414 2019-06-07 20:13:50.000000 SaltPyLint-2023.8.3/saltpylint/virt.py
+-rw-r--r--   0 vampas    (1000) vampas    (1000)      161 2023-08-03 14:43:46.085347 SaltPyLint-2023.8.3/setup.cfg
+-rwxr-xr-x   0 vampas    (1000) vampas    (1000)     3548 2023-08-03 14:41:39.000000 SaltPyLint-2023.8.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `SaltPyLint-2020.9.28/.pylintrc` & `SaltPyLint-2023.8.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/setup.py` & `SaltPyLint-2023.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,19 +83,19 @@
     version=VERSION,
     description=DESCRIPTION,
     author='Pedro Algarvio',
     author_email='pedro@algarvio.me',
     url='https://github.com/saltstack/salt-pylint',
     classifiers=[
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX :: Linux',
```

### Comparing `SaltPyLint-2020.9.28/saltpylint/thirdparty.py` & `SaltPyLint-2023.8.3/saltpylint/thirdparty.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     known_py2_modules = ['__builtin__', 'exceptions']
     known_py3_modules = ['builtins']
 
     unix_modules = ('posix', 'pwd', 'spwd', 'grp', 'crypt', 'termios', 'tty', 'pty', 'fcntl', 'pipes', 'resource', 'nis', 'syslog', 'posixpath')
     win_modules = ('msilib', 'msvcrt', 'winreg', 'winsound', 'ntpath')
 
-    all_modules = {m[1]: m[0].path for m in pkgutil.iter_modules()}
+    all_modules = {m[1]: m[0] for m in pkgutil.iter_modules()}
     std_modules_path = all_modules["os"]
     std_modules = []
     for mod, path in all_modules.items():
         if path == std_modules_path and mod not in unix_modules + win_modules:
             std_modules.append(mod)
 
     known_std_modules = known_py2_modules + known_py3_modules + std_modules
```

### Comparing `SaltPyLint-2020.9.28/saltpylint/fileperms.py` & `SaltPyLint-2023.8.3/saltpylint/fileperms.py`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/saltpylint/virt.py` & `SaltPyLint-2023.8.3/saltpylint/virt.py`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/saltpylint/py3modernize/fixes/fix_input_salt_six.py` & `SaltPyLint-2023.8.3/saltpylint/py3modernize/fixes/fix_input_salt_six.py`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/saltpylint/py3modernize/__init__.py` & `SaltPyLint-2023.8.3/saltpylint/py3modernize/__init__.py`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/saltpylint/blacklist.py` & `SaltPyLint-2023.8.3/saltpylint/blacklist.py`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/saltpylint/minpyver.py` & `SaltPyLint-2023.8.3/saltpylint/minpyver.py`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/saltpylint/dunder_del.py` & `SaltPyLint-2023.8.3/saltpylint/dunder_del.py`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/saltpylint/strings.py` & `SaltPyLint-2023.8.3/saltpylint/strings.py`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/saltpylint/smartup.py` & `SaltPyLint-2023.8.3/saltpylint/smartup.py`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/saltpylint/pep263.py` & `SaltPyLint-2023.8.3/saltpylint/pep263.py`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/saltpylint/checkers.py` & `SaltPyLint-2023.8.3/saltpylint/checkers.py`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/saltpylint/process.py` & `SaltPyLint-2023.8.3/saltpylint/process.py`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/saltpylint/pep8.py` & `SaltPyLint-2023.8.3/saltpylint/pep8.py`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/saltpylint/ext/pyqver2.py` & `SaltPyLint-2023.8.3/saltpylint/ext/pyqver2.py`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/SaltPyLint.egg-info/SOURCES.txt` & `SaltPyLint-2023.8.3/SaltPyLint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/SaltPyLint.egg-info/PKG-INFO` & `SaltPyLint-2023.8.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: SaltPyLint
-Version: 2020.9.28
+Version: 2023.8.3
 Summary: Required PyLint plugins needed in the several SaltStack projects.
 Home-page: https://github.com/saltstack/salt-pylint
 Author: Pedro Algarvio
 Author-email: pedro@algarvio.me
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
+License-File: LICENSE
```

### Comparing `SaltPyLint-2020.9.28/.testing.pylintrc` & `SaltPyLint-2023.8.3/.testing.pylintrc`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/LICENSE` & `SaltPyLint-2023.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SaltPyLint-2020.9.28/PKG-INFO` & `SaltPyLint-2023.8.3/SaltPyLint.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: SaltPyLint
-Version: 2020.9.28
+Version: 2023.8.3
 Summary: Required PyLint plugins needed in the several SaltStack projects.
 Home-page: https://github.com/saltstack/salt-pylint
 Author: Pedro Algarvio
 Author-email: pedro@algarvio.me
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
+License-File: LICENSE
```

### Comparing `SaltPyLint-2020.9.28/.gitignore` & `SaltPyLint-2023.8.3/.gitignore`

 * *Files identical despite different names*

