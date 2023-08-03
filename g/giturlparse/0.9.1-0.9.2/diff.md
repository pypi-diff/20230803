# Comparing `tmp/giturlparse-0.9.1.tar.gz` & `tmp/giturlparse-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/giturlparse-0.9.1.tar", last modified: Sat Jan 20 08:55:53 2018, max compression
+gzip compressed data, was "dist/giturlparse-0.9.2.tar", last modified: Sat Oct 27 13:31:02 2018, max compression
```

## Comparing `giturlparse-0.9.1.tar` & `giturlparse-0.9.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwsr-x   0 yakky     (1000)     1004        0 2018-01-20 08:55:53.000000 giturlparse-0.9.1/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2018-01-20 08:55:53.000000 giturlparse-0.9.1/giturlparse/
--rw-rw-r--   0 yakky     (1000)     1004      429 2018-01-20 08:55:29.000000 giturlparse-0.9.1/giturlparse/__init__.py
--rw-rw-r--   0 yakky     (1000)     1004     1783 2018-01-20 08:45:09.000000 giturlparse-0.9.1/giturlparse/parser.py
-drwxrwsr-x   0 yakky     (1000)     1004        0 2018-01-20 08:55:53.000000 giturlparse-0.9.1/giturlparse/platforms/
--rw-rw-r--   0 yakky     (1000)     1004      395 2018-01-20 08:45:09.000000 giturlparse-0.9.1/giturlparse/platforms/friendcode.py
--rw-rw-r--   0 yakky     (1000)     1004      504 2018-01-20 08:45:09.000000 giturlparse-0.9.1/giturlparse/platforms/assembla.py
--rw-rw-r--   0 yakky     (1000)     1004      626 2018-01-20 08:45:09.000000 giturlparse-0.9.1/giturlparse/platforms/__init__.py
--rw-rw-r--   0 yakky     (1000)     1004      833 2018-01-20 08:45:09.000000 giturlparse-0.9.1/giturlparse/platforms/gitlab.py
--rw-rw-r--   0 yakky     (1000)     1004      596 2018-01-20 08:45:09.000000 giturlparse-0.9.1/giturlparse/platforms/bitbucket.py
--rw-rw-r--   0 yakky     (1000)     1004      983 2018-01-20 08:45:09.000000 giturlparse-0.9.1/giturlparse/platforms/base.py
--rw-rw-r--   0 yakky     (1000)     1004      724 2018-01-20 08:45:09.000000 giturlparse-0.9.1/giturlparse/platforms/github.py
-drwxrwsr-x   0 yakky     (1000)     1004        0 2018-01-20 08:55:53.000000 giturlparse-0.9.1/giturlparse/tests/
--rw-rw-r--   0 yakky     (1000)     1004      135 2018-01-20 08:45:09.000000 giturlparse-0.9.1/giturlparse/tests/__init__.py
--rw-rw-r--   0 yakky     (1000)     1004     3195 2018-01-20 08:45:09.000000 giturlparse-0.9.1/giturlparse/tests/parse.py
--rw-rw-r--   0 yakky     (1000)     1004     3121 2018-01-20 08:45:09.000000 giturlparse-0.9.1/giturlparse/tests/rewrite.py
--rw-rw-r--   0 yakky     (1000)     1004     2404 2018-01-20 08:45:09.000000 giturlparse-0.9.1/giturlparse/result.py
-drwxrwsr-x   0 yakky     (1000)     1004        0 2018-01-20 08:55:53.000000 giturlparse-0.9.1/giturlparse.egg-info/
--rw-rw-r--   0 yakky     (1000)     1004        1 2018-01-20 08:55:53.000000 giturlparse-0.9.1/giturlparse.egg-info/dependency_links.txt
--rw-rw-r--   0 yakky     (1000)     1004      576 2018-01-20 08:55:53.000000 giturlparse-0.9.1/giturlparse.egg-info/SOURCES.txt
--rw-rw-r--   0 yakky     (1000)     1004     3149 2018-01-20 08:55:53.000000 giturlparse-0.9.1/giturlparse.egg-info/PKG-INFO
--rw-rw-r--   0 yakky     (1000)     1004       12 2018-01-20 08:55:53.000000 giturlparse-0.9.1/giturlparse.egg-info/top_level.txt
--rw-rw-r--   0 yakky     (1000)     1004    10273 2018-01-20 08:45:09.000000 giturlparse-0.9.1/LICENSE
--rw-rw-r--   0 yakky     (1000)     1004       69 2018-01-20 08:45:09.000000 giturlparse-0.9.1/MANIFEST.in
--rw-rw-r--   0 yakky     (1000)     1004     3149 2018-01-20 08:55:53.000000 giturlparse-0.9.1/PKG-INFO
--rw-rw-r--   0 yakky     (1000)     1004     1273 2018-01-20 08:45:09.000000 giturlparse-0.9.1/setup.py
--rw-rw-r--   0 yakky     (1000)     1004      367 2018-01-20 08:55:53.000000 giturlparse-0.9.1/setup.cfg
--rw-rw-r--   0 yakky     (1000)     1004     1534 2018-01-20 08:55:25.000000 giturlparse-0.9.1/README.rst
+drwxrwxr-x   0 yakky     (1000) utentiwww  (1004)        0 2018-10-27 13:31:02.000000 giturlparse-0.9.2/
+drwxrwxr-x   0 yakky     (1000) utentiwww  (1004)        0 2018-10-27 13:31:02.000000 giturlparse-0.9.2/giturlparse/
+drwxrwxr-x   0 yakky     (1000) utentiwww  (1004)        0 2018-10-27 13:31:02.000000 giturlparse-0.9.2/giturlparse/platforms/
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)      626 2018-10-27 12:09:50.000000 giturlparse-0.9.2/giturlparse/platforms/__init__.py
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)      504 2018-10-27 12:09:50.000000 giturlparse-0.9.2/giturlparse/platforms/assembla.py
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)      974 2018-10-27 12:50:42.000000 giturlparse-0.9.2/giturlparse/platforms/base.py
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)      596 2018-10-27 12:09:50.000000 giturlparse-0.9.2/giturlparse/platforms/bitbucket.py
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)      395 2018-10-27 12:09:50.000000 giturlparse-0.9.2/giturlparse/platforms/friendcode.py
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)      724 2018-10-27 12:09:50.000000 giturlparse-0.9.2/giturlparse/platforms/github.py
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)      833 2018-10-27 12:09:50.000000 giturlparse-0.9.2/giturlparse/platforms/gitlab.py
+drwxrwxr-x   0 yakky     (1000) utentiwww  (1004)        0 2018-10-27 13:31:02.000000 giturlparse-0.9.2/giturlparse/tests/
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)      135 2018-10-27 12:09:50.000000 giturlparse-0.9.2/giturlparse/tests/__init__.py
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)     3798 2018-10-27 12:50:42.000000 giturlparse-0.9.2/giturlparse/tests/parse.py
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)     3121 2018-10-27 12:09:50.000000 giturlparse-0.9.2/giturlparse/tests/rewrite.py
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)      429 2018-10-27 12:51:01.000000 giturlparse-0.9.2/giturlparse/__init__.py
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)     1783 2018-10-27 12:09:50.000000 giturlparse-0.9.2/giturlparse/parser.py
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)     2404 2018-10-27 12:09:50.000000 giturlparse-0.9.2/giturlparse/result.py
+drwxrwxr-x   0 yakky     (1000) utentiwww  (1004)        0 2018-10-27 13:31:02.000000 giturlparse-0.9.2/giturlparse.egg-info/
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)     3207 2018-10-27 13:31:02.000000 giturlparse-0.9.2/giturlparse.egg-info/PKG-INFO
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)      576 2018-10-27 13:31:02.000000 giturlparse-0.9.2/giturlparse.egg-info/SOURCES.txt
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)        1 2018-10-27 13:31:02.000000 giturlparse-0.9.2/giturlparse.egg-info/dependency_links.txt
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)       12 2018-10-27 13:31:02.000000 giturlparse-0.9.2/giturlparse.egg-info/top_level.txt
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)    10273 2018-10-27 12:09:50.000000 giturlparse-0.9.2/LICENSE
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)       69 2018-10-27 12:09:50.000000 giturlparse-0.9.2/MANIFEST.in
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)     1528 2018-10-27 12:54:07.000000 giturlparse-0.9.2/README.rst
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)      367 2018-10-27 13:31:02.000000 giturlparse-0.9.2/setup.cfg
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)     1331 2018-10-27 13:22:28.000000 giturlparse-0.9.2/setup.py
+-rw-rw-r--   0 yakky     (1000) utentiwww  (1004)     3207 2018-10-27 13:31:02.000000 giturlparse-0.9.2/PKG-INFO
```

### Comparing `giturlparse-0.9.1/giturlparse/parser.py` & `giturlparse-0.9.2/giturlparse/parser.py`

 * *Files identical despite different names*

### Comparing `giturlparse-0.9.1/giturlparse/platforms/__init__.py` & `giturlparse-0.9.2/giturlparse/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `giturlparse-0.9.1/giturlparse/platforms/gitlab.py` & `giturlparse-0.9.2/giturlparse/platforms/gitlab.py`

 * *Files identical despite different names*

### Comparing `giturlparse-0.9.1/giturlparse/platforms/bitbucket.py` & `giturlparse-0.9.2/giturlparse/platforms/bitbucket.py`

 * *Files identical despite different names*

### Comparing `giturlparse-0.9.1/giturlparse/platforms/github.py` & `giturlparse-0.9.2/giturlparse/platforms/github.py`

 * *Files identical despite different names*

### Comparing `giturlparse-0.9.1/giturlparse/tests/parse.py` & `giturlparse-0.9.2/giturlparse/tests/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,24 +26,40 @@
         'repo': 'Repo',
 
         'protocol': 'https',
         'github': True,
         'bitbucket': False,
         'assembla': False
     })),
+    ('HTTPS', ('https://github.com/foo-bar/xpwn', {
+        'host': 'github.com',
+        'user': 'git',
+        'owner': 'foo-bar',
+        'repo': 'xpwn',
+
+        'protocol': 'https',
+        'github': True,
+    })),
     ('GIT', ('git://github.com/Org/Repo.git', {
         'host': 'github.com',
         'user': 'git',
         'owner': 'Org',
         'repo': 'Repo',
 
         'protocol': 'git',
         'github': True,
-        'bitbucket': False,
-        'assembla': False
+    })),
+    ('GIT', ('git://github.com/foo-bar/xpwn', {
+        'host': 'github.com',
+        'user': 'git',
+        'owner': 'foo-bar',
+        'repo': 'xpwn',
+
+        'protocol': 'git',
+        'github': True,
     })),
 
     # BitBucket
     ('SSH', ('git@bitbucket.org:Org/Repo.git', {
         'host': 'bitbucket.org',
         'user': 'git',
         'owner': 'Org',
@@ -59,14 +75,23 @@
         'user': 'git',
         'owner': 'Org',
         'repo': 'Repo',
 
         'protocol': 'ssh',
         'platform': 'gitlab'
     })),
+    ('SSH', ('git@host.org:9999/Org-hyphen/Repo.git', {
+        'host': 'host.org',
+        'user': 'git',
+        'owner': 'Org-hyphen',
+        'repo': 'Repo',
+
+        'protocol': 'ssh',
+        'platform': 'gitlab'
+    })),
     ('SSH', ('git@host.org:Org/Repo.git', {
         'host': 'host.org',
         'user': 'git',
         'owner': 'Org',
         'repo': 'Repo',
 
         'protocol': 'ssh',
@@ -89,15 +114,15 @@
 
         'protocol': 'https',
         'platform': 'gitlab'
     })),
 )
 
 INVALID_PARSE_URLS = (
-    ('SSH Bad Username', 'gitx@github.com:Org/Repo.git'),
+    ('SSH No Username', '@github.com:Org/Repo.git'),
     ('SSH No Repo', 'git@github.com:Org'),
     ('HTTPS No Repo', 'https://github.com/Org'),
     ('GIT No Repo', 'git://github.com/Org'),
 )
 
 
 # Here's our "unit tests".
```

### Comparing `giturlparse-0.9.1/giturlparse/tests/rewrite.py` & `giturlparse-0.9.2/giturlparse/tests/rewrite.py`

 * *Files identical despite different names*

### Comparing `giturlparse-0.9.1/giturlparse/result.py` & `giturlparse-0.9.2/giturlparse/result.py`

 * *Files identical despite different names*

### Comparing `giturlparse-0.9.1/giturlparse.egg-info/SOURCES.txt` & `giturlparse-0.9.2/giturlparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giturlparse-0.9.1/giturlparse.egg-info/PKG-INFO` & `giturlparse-0.9.2/giturlparse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
 Name: giturlparse
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Git URL parsing module (supports parsing and rewriting)
-Home-page: https://github.com/yakky/giturlparse
+Home-page: https://github.com/nephila/giturlparse
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.it
 License: Apache v2
 Description-Content-Type: UNKNOWN
 Description: ===========
         giturlparse
         ===========
@@ -71,17 +71,17 @@
             # => {
             #     'ssh': 'git@github.com:Org/Private-repo.git',
             #     'https': 'https://github.com/Org/Private-repo.git',
             #     'git': 'git://github.com/Org/Private-repo.git'
             # }
         
         
-        **********
-        Validate::
-        **********
+        ********
+        Validate
+        ********
         
         ::
         
             from giturlparse import parse, validate
         
             url = 'git@github.com:Org/Private-repo.git'
         
@@ -110,14 +110,15 @@
         
         Apache v2 (Check out LICENSE file)
         
 Keywords: git url parse ssh github bitbucket
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
```

### Comparing `giturlparse-0.9.1/LICENSE` & `giturlparse-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `giturlparse-0.9.1/PKG-INFO` & `giturlparse-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
 Name: giturlparse
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Git URL parsing module (supports parsing and rewriting)
-Home-page: https://github.com/yakky/giturlparse
+Home-page: https://github.com/nephila/giturlparse
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.it
 License: Apache v2
 Description-Content-Type: UNKNOWN
 Description: ===========
         giturlparse
         ===========
@@ -71,17 +71,17 @@
             # => {
             #     'ssh': 'git@github.com:Org/Private-repo.git',
             #     'https': 'https://github.com/Org/Private-repo.git',
             #     'git': 'git://github.com/Org/Private-repo.git'
             # }
         
         
-        **********
-        Validate::
-        **********
+        ********
+        Validate
+        ********
         
         ::
         
             from giturlparse import parse, validate
         
             url = 'git@github.com:Org/Private-repo.git'
         
@@ -110,14 +110,15 @@
         
         Apache v2 (Check out LICENSE file)
         
 Keywords: git url parse ssh github bitbucket
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
```

### Comparing `giturlparse-0.9.1/setup.py` & `giturlparse-0.9.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,28 +17,28 @@
     name='giturlparse',
     version=version,
     description='A Git URL parsing module (supports parsing and rewriting)',
     long_description=readme,
     license='Apache v2',
     author="Aaron O'Mullan",
     author_email='aaron@friendco.de',
-    url='https://github.com/yakky/giturlparse',
+    url='https://github.com/nephila/giturlparse',
     maintainer='Iacopo Spalletti',
     maintainer_email='i.spalletti@nephila.it',
     packages=['giturlparse', 'giturlparse.platforms'],
     include_package_data=True,
-    install_requires=[
-    ],
+    install_requires=[],
     keywords='git url parse ssh github bitbucket',
     test_suite='giturlparse.tests',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
+        'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
     ],
 )
```

### Comparing `giturlparse-0.9.1/README.rst` & `giturlparse-0.9.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,17 @@
     # => {
     #     'ssh': 'git@github.com:Org/Private-repo.git',
     #     'https': 'https://github.com/Org/Private-repo.git',
     #     'git': 'git://github.com/Org/Private-repo.git'
     # }
 
 
-**********
-Validate::
-**********
+********
+Validate
+********
 
 ::
 
     from giturlparse import parse, validate
 
     url = 'git@github.com:Org/Private-repo.git'
```

