# Comparing `tmp/pgcooldown-0.2.1.tar.gz` & `tmp/pgcooldown-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgcooldown-0.2.1.tar", last modified: Wed Aug  2 11:45:52 2023, max compression
+gzip compressed data, was "pgcooldown-0.2.2.tar", last modified: Thu Aug  3 12:59:07 2023, max compression
```

## Comparing `pgcooldown-0.2.1.tar` & `pgcooldown-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 11:45:52.110210 pgcooldown-0.2.1/
--rw-rw-rw-   0        0        0     1093 2023-08-02 10:18:55.000000 pgcooldown-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2429 2023-08-02 11:45:52.110210 pgcooldown-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1935 2023-08-02 10:18:55.000000 pgcooldown-0.2.1/README.md
--rw-rw-rw-   0        0        0      852 2023-08-02 11:45:21.000000 pgcooldown-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-02 11:45:52.110210 pgcooldown-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-02 11:45:52.092274 pgcooldown-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-02 11:45:52.095571 pgcooldown-0.2.1/src/pgcooldown/
--rw-rw-rw-   0        0        0     5179 2023-08-02 10:58:38.000000 pgcooldown-0.2.1/src/pgcooldown/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 11:45:52.107749 pgcooldown-0.2.1/src/pgcooldown.egg-info/
--rw-rw-rw-   0        0        0     2429 2023-08-02 11:45:52.000000 pgcooldown-0.2.1/src/pgcooldown.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-08-02 11:45:52.000000 pgcooldown-0.2.1/src/pgcooldown.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 11:45:52.000000 pgcooldown-0.2.1/src/pgcooldown.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-08-02 11:45:52.000000 pgcooldown-0.2.1/src/pgcooldown.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 11:45:52.109204 pgcooldown-0.2.1/tests/
--rw-rw-rw-   0        0        0     2318 2023-08-02 10:19:32.000000 pgcooldown-0.2.1/tests/test_cooldown.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:59:07.703198 pgcooldown-0.2.2/
+-rw-rw-rw-   0        0        0     1093 2023-08-02 10:18:55.000000 pgcooldown-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2671 2023-08-03 12:59:07.703198 pgcooldown-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2177 2023-08-02 12:09:26.000000 pgcooldown-0.2.2/README.md
+-rw-rw-rw-   0        0        0      852 2023-08-03 11:40:56.000000 pgcooldown-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 12:59:07.703198 pgcooldown-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 12:59:07.678893 pgcooldown-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 12:59:07.681885 pgcooldown-0.2.2/src/pgcooldown/
+-rw-rw-rw-   0        0        0     6656 2023-08-03 11:40:56.000000 pgcooldown-0.2.2/src/pgcooldown/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 12:59:07.700261 pgcooldown-0.2.2/src/pgcooldown.egg-info/
+-rw-rw-rw-   0        0        0     2671 2023-08-03 12:59:07.000000 pgcooldown-0.2.2/src/pgcooldown.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-08-03 12:59:07.000000 pgcooldown-0.2.2/src/pgcooldown.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 12:59:07.000000 pgcooldown-0.2.2/src/pgcooldown.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-03 12:59:07.000000 pgcooldown-0.2.2/src/pgcooldown.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 12:59:07.702199 pgcooldown-0.2.2/tests/
+-rw-rw-rw-   0        0        0     2704 2023-08-03 11:40:56.000000 pgcooldown-0.2.2/tests/test_cooldown.py
```

### Comparing `pgcooldown-0.2.1/LICENSE` & `pgcooldown-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pgcooldown-0.2.1/PKG-INFO` & `pgcooldown-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pgcooldown
-Version: 0.2.1
+Version: 0.2.2
 Summary: A cooldown/counter class to wait for stuff in games
 Author-email: Michael Lamertz <michael.lamertz@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries :: pygame
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# cooldown
+# pgcooldown
 
 A cooldown class, checking the delta time between start and now.
 
     cooldown = Cooldown(5)
 
 A trigger class to wait for n seconds.
 
@@ -81,10 +81,24 @@
 
 	if cooldown.cold:
 	    launch_stuff()
 	    cooldown.reset()
 
 """
 
+## Installation
+
+The project home is https://github.com/dickerdackel/pgcooldown
+
+### Getting it from pypi
+
+```
+pip install pgcooldown
+```
+
+### Tarball from github
+
+Found at https://github.com/dickerdackel/pgcooldown/releases
+
 ## Licensing stuff
 
 This lib is under the MIT license.
```

### Comparing `pgcooldown-0.2.1/README.md` & `pgcooldown-0.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# cooldown
+# pgcooldown
 
 A cooldown class, checking the delta time between start and now.
 
     cooldown = Cooldown(5)
 
 A trigger class to wait for n seconds.
 
@@ -68,10 +68,24 @@
 
 	if cooldown.cold:
 	    launch_stuff()
 	    cooldown.reset()
 
 """
 
+## Installation
+
+The project home is https://github.com/dickerdackel/pgcooldown
+
+### Getting it from pypi
+
+```
+pip install pgcooldown
+```
+
+### Tarball from github
+
+Found at https://github.com/dickerdackel/pgcooldown/releases
+
 ## Licensing stuff
 
 This lib is under the MIT license.
```

### Comparing `pgcooldown-0.2.1/pyproject.toml` & `pgcooldown-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pgcooldown"
 description = "A cooldown/counter class to wait for stuff in games"
-version = "0.2.1"
+version = "0.2.2"
 readme = "README.md"
 
 authors = [
     { name="Michael Lamertz", email="michael.lamertz@gmail.com" }
 ]
 
 classifiers = [
```

### Comparing `pgcooldown-0.2.1/src/pgcooldown.egg-info/PKG-INFO` & `pgcooldown-0.2.2/src/pgcooldown.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pgcooldown
-Version: 0.2.1
+Version: 0.2.2
 Summary: A cooldown/counter class to wait for stuff in games
 Author-email: Michael Lamertz <michael.lamertz@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries :: pygame
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# cooldown
+# pgcooldown
 
 A cooldown class, checking the delta time between start and now.
 
     cooldown = Cooldown(5)
 
 A trigger class to wait for n seconds.
 
@@ -81,10 +81,24 @@
 
 	if cooldown.cold:
 	    launch_stuff()
 	    cooldown.reset()
 
 """
 
+## Installation
+
+The project home is https://github.com/dickerdackel/pgcooldown
+
+### Getting it from pypi
+
+```
+pip install pgcooldown
+```
+
+### Tarball from github
+
+Found at https://github.com/dickerdackel/pgcooldown/releases
+
 ## Licensing stuff
 
 This lib is under the MIT license.
```

### Comparing `pgcooldown-0.2.1/tests/test_cooldown.py` & `pgcooldown-0.2.2/tests/test_cooldown.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,15 +71,14 @@
     c.remaining = 4.1
     assert c.remaining == 4.1
     c.start()
     sleep(0.1)
     assert round(c.remaining) == 4
 
 
-
 def test_cold():
     c = Cooldown(1)
     c.cold = True
     assert c.cold
     assert not c.hot
     assert c.duration == 1
     assert c.remaining == 0
@@ -96,14 +95,34 @@
     sleep(1)
     assert round(c.normalized * 100) == 75
     sleep(1)
     assert round(c.normalized * 100) == 100
     assert c.cold
 
 
+def test_copyconstructor():
+    c = Cooldown(10).pause()
+    d = Cooldown(c)
+    assert d.duration == 10
+    assert d.paused is False
+
+
+def test_compare():
+    c = Cooldown(10).pause()
+    assert c == 10
+    assert c > 5
+    assert c >= 10
+    assert c < 15
+    assert c <= 10
+    assert c != 5
+    assert bool(c)
+    assert int(c) == 10
+    assert float(c) == 10.0
+
+
 if __name__ == '__main__':
     test_init()
     test_reset()
     test_pause()
     test_cold()
     test_remaining()
     test_normalized()
```

