# Comparing `tmp/pyjt-0.2.1.tar.gz` & `tmp/pyjt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjt-0.2.1.tar", last modified: Wed Aug  2 17:48:19 2023, max compression
+gzip compressed data, was "pyjt-0.3.0.tar", last modified: Thu Aug  3 08:07:33 2023, max compression
```

## Comparing `pyjt-0.2.1.tar` & `pyjt-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:48:19.170328 pyjt-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-02 17:47:30.000000 pyjt-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-02 17:48:19.170328 pyjt-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 17:47:30.000000 pyjt-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:48:19.170328 pyjt-0.2.1/pyjt/
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/ComponentFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/Fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/Frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/Inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/Proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/Robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyjt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:48:19.170328 pyjt-0.2.1/pyjt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-02 17:48:19.000000 pyjt-0.2.1/pyjt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-02 17:48:19.000000 pyjt-0.2.1/pyjt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:48:19.000000 pyjt-0.2.1/pyjt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 17:48:19.000000 pyjt-0.2.1/pyjt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 17:48:19.000000 pyjt-0.2.1/pyjt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-02 17:47:30.000000 pyjt-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:48:19.170328 pyjt-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:48:19.170328 pyjt-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 17:47:30.000000 pyjt-0.2.1/tests/test_framefinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-02 17:47:30.000000 pyjt-0.2.1/tests/test_textfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:33.600980 pyjt-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-03 08:06:43.000000 pyjt-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-03 08:07:33.600980 pyjt-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-03 08:06:43.000000 pyjt-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:33.596980 pyjt-0.3.0/pyjt/
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/ComponentFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/Fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/Proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/Robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyjt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:33.600980 pyjt-0.3.0/pyjt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-03 08:07:33.000000 pyjt-0.3.0/pyjt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 08:07:33.000000 pyjt-0.3.0/pyjt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:07:33.000000 pyjt-0.3.0/pyjt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 08:07:33.000000 pyjt-0.3.0/pyjt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 08:07:33.000000 pyjt-0.3.0/pyjt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-03 08:06:43.000000 pyjt-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:07:33.600980 pyjt-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:33.600980 pyjt-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 08:06:43.000000 pyjt-0.3.0/tests/test_framefinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-03 08:06:43.000000 pyjt-0.3.0/tests/test_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-03 08:06:43.000000 pyjt-0.3.0/tests/test_textfield.py
```

### Comparing `pyjt-0.2.1/LICENSE` & `pyjt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjt-0.2.1/PKG-INFO` & `pyjt-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.2.1
+Version: 0.3.0
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyjt-0.2.1/README.md` & `pyjt-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyjt-0.2.1/pyjt/ComponentFinder.py` & `pyjt-0.3.0/pyjt/ComponentFinder.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,39 +6,63 @@
 log = logging.getLogger(__name__)
 
 
 class Locator:
     def __init__(self, **kwargs):
         self._filters = kwargs
         self._contains = []
+        self._has = []
 
     def update(self, **kwargs):
         self._filters.update(**kwargs)
 
     def contains(self, **kwargs):
+        """ Ensure the control has a sub-component with the given attributes
+            somewhere in the tree.
+        """
         self._contains.append(Locator(**kwargs))
         return self
 
+    def has(self, **kwargs):
+        """ Ensure the control has a directo sub-component with the given
+            attributes.
+        """
+        self._has.append(Locator(**kwargs))
+        return self
+
     def matches(self, component):
-        if not self._has(component):
+        if not _matches(component, **self._filters):
             return False
 
+        log.debug(f"found {component}, checking childs...")
         for locator in self._contains:
             log.debug(f"contains {locator}")
             if ComponentFinder._locate(window=component, locator=locator) is None:
                 return False
-        return True
 
-    def _has(self, component):
-        return _matches(component, **self._filters)
+        for locator in self._has:
+            log.debug(f"has {locator}")
+            if not _child_matches(component, locator):
+                return False
+        return True
 
     def __repr__(self):
         return f"Locator({self._filters})"
 
 
+def _child_matches(component, locator):
+    log.debug(f"_child_matches({component}, {locator}")
+    for subcontrol in component.getComponents():
+        if locator.matches(subcontrol):
+            log.debug(f"_child_matches({component}, {locator}: found {subcontrol}")
+            return True
+    log.debug(f"_child_matches({component}, {locator}: FAILED")
+    return False
+
+
 class Timer:
     def __init__(self, timeout=None, cycle=None):
         self._timeout = timeout
         self._cycle = cycle
         self._first = True
 
     def start(self):
@@ -51,15 +75,15 @@
         self._first = False
         now = time.time()
         timeout = seconds if seconds else self._timeout
         return self._started + timeout <= now
 
 
 class ComponentFinder:
-    DEFAULT_TIMEOUT = 5
+    DEFAULT_TIMEOUT = 1
     DEFAULT_DELAY = 1
 
     @staticmethod
     def find(window, locator=None, timeout=None, **kwargs):
         timeout = timeout if timeout else ComponentFinder.DEFAULT_TIMEOUT
         timer = Timer(timeout, ComponentFinder.DEFAULT_DELAY).start()
         locator = locator if locator else Locator(**kwargs)
@@ -84,15 +108,14 @@
                 if hit is not None:
                     return hit
         return None
 
     @staticmethod
     def _locate(window, locator):
         log.debug(f"locate({locator})")
-        log.debug(f"locate({locator})")
         if locator.matches(window):
             return window
         components = window.getComponents()
         for cmpt in components:
             log.debug(f"found component: {cmpt.getName()} {type(cmpt)}")
             hit = ComponentFinder._locate(cmpt, locator)
             if hit:
@@ -105,15 +128,17 @@
     # log.debug(f"_matches({cmpt}, name={name}, text={text})")
     for name, value in kwargs.items():
         if name == 'role':
             cc = cmpt.instance if isinstance(cmpt, Proxy) else cmpt
             log.debug(f"\tcheck01 {name} {type(cc)}={value}")
             check = isinstance(cc, value)
             log.debug(f"\t\tcheck01: {check}")
-            return check
+            if not check:
+                return False
+            continue
         fname = f"get{name[0].capitalize()}{name[1:]}"
         log.debug(f"check({name}, {value}) -> {fname}: {cmpt}")
         if not hasattr(cmpt, fname):
             log.debug(f"\tcheck({name}) component has no attr {fname}")
             return False
         fnc = getattr(cmpt, fname)
         _value = fnc()
```

### Comparing `pyjt-0.2.1/pyjt/Fixture.py` & `pyjt-0.3.0/pyjt/Fixture.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 import logging
 from enum import Enum
 from pyjt.Robot import Robot
-
+from pyjt.ComponentFinder import ComponentFinder, Locator
+from pyjt.Errors import ElementNotFoundError
 
 log = logging.getLogger(__name__)
 
 FillMode = Enum('FillMode', ['TYPE', 'SET', 'PASTE'])
 
 
 class Fixture:
     def __init__(self, control):
         self._control = control
         self.robot = Robot()
 
+    def locate(self, locator=None, **kwargs):
+        log.debug(f"frame.find({locator}, {kwargs})")
+        locator = locator if locator else Locator(**kwargs)
+        control = ComponentFinder.findIn(self._control.getComponents, locator)
+        if not control:
+            raise ElementNotFoundError(f"Control({kwargs}) not found!")
+        return Fixture(control)
+
+    def find(self, role, **kwargs):
+        kwargs['role'] = role
+        return self.locate(**kwargs)
+
     def click(self):
         log.debug(f"click({self._control})")
         self.robot.move(self._control)
         log.debug(f"executing click({self._control})")
         self.robot.click()
 
     def fill(self, text, mode=FillMode.TYPE, clear=True):
@@ -46,7 +59,10 @@
                 self.robot.selectAll()
             self.robot.type(text)
         if mode == FillMode.SET:
             self._control.setText(text)
 
     def __getattr__(self, name):
         return getattr(self._control, name)
+
+    def __repr__(self):
+        return str(self._control)
```

### Comparing `pyjt-0.2.1/pyjt/Frame.py` & `pyjt-0.3.0/pyjt/Frame.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,39 @@
 import logging
 
 from pyjt.Errors import ElementNotFoundError
-from pyjt.ComponentFinder import ComponentFinder, Locator
+from pyjt.ComponentFinder import Locator
 from pyjt.Fixture import Fixture
 from pyjt.Inspector import Inspector
 from pyjt import Proxy
 
 log = logging.getLogger(__name__)
 
 
 class FrameFinder:
     @staticmethod
     def find(locator=None, **kwargs):
         from java.awt import Window
         locator = locator if locator else Locator(**kwargs)
         wp = Proxy(Window)
-        window = ComponentFinder.findIn(func=wp.getWindows, locator=locator)
-        if not window:
-            raise ElementNotFoundError(f"Window {kwargs} not found!")
-        return Frame(window=window)
+        for window in wp.getWindows():
+            if locator.matches(window):
+                return Frame(window)
+        raise ElementNotFoundError(f"Window {kwargs} not found!")
 
     @staticmethod
     def inspect():
         from java.awt import Window
         wp = Proxy(Window)
         result = []
         for window in wp.getWindows():
             result.append(Inspector.inspect(window))
         return result
 
 
-class Frame:
-    def __init__(self, window=None):
-        self._window = window
-
-    def find(self, locator=None, **kwargs):
-        log.debug(f"frame.find({locator}, {kwargs})")
-        locator = locator if locator else Locator(**kwargs)
-        control = ComponentFinder.find(self._window, locator)
-        if not control:
-            raise ElementNotFoundError(f"Control({kwargs}) not found!")
-        return Fixture(control)
-
-    def locate(self, role, **kwargs):
-        kwargs['role'] = role
-        return self.find(**kwargs)
-
+class Frame(Fixture):
     def dispose(self):
-        self._window.dispose()
+        self._control.dispose()
 
     def close(self):
         from java.awt.event import WindowEvent
-        self._window.instance.dispatchEvent(WindowEvent(self._window.instance, WindowEvent.WINDOW_CLOSING))
+        self._control.instance.dispatchEvent(WindowEvent(self._component.instance, WindowEvent.WINDOW_CLOSING))
```

### Comparing `pyjt-0.2.1/pyjt/Inspector.py` & `pyjt-0.3.0/pyjt/Inspector.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.2.1/pyjt/Proxy.py` & `pyjt-0.3.0/pyjt/Proxy.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.2.1/pyjt/Robot.py` & `pyjt-0.3.0/pyjt/Robot.py`

 * *Files identical despite different names*

### Comparing `pyjt-0.2.1/pyjt/__init__.py` & `pyjt-0.3.0/pyjt/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,9 +41,10 @@
 def shutdown():
     """ Shuts down pyjt and the JVM. """
     jpype.shutdownJVM()
 
 from .Proxy import Proxy
 from .Frame import Frame, FrameFinder
 from .Fixture import Fixture, FillMode
+from .Errors import ElementNotFoundError
 from .ComponentFinder import Locator
 from .Inspector import Inspector
```

### Comparing `pyjt-0.2.1/pyjt.egg-info/PKG-INFO` & `pyjt-0.3.0/pyjt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjt
-Version: 0.2.1
+Version: 0.3.0
 Summary: test automation for java UI applications from python
 Author-email: Claudio Klingler <ck@realtime-projects.com>
 Project-URL: Homepage, https://github.com/realtimeprojects/pyjt
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/pyjt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyjt-0.2.1/pyproject.toml` & `pyjt-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyjt"
-version = "0.2.1"
+version = "0.3.0"
 description="test automation for java UI applications from python"
 authors = [
     { name="Claudio Klingler", email="ck@realtime-projects.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pyjt-0.2.1/tests/test_textfield.py` & `pyjt-0.3.0/tests/test_textfield.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pyjt import FillMode
 
 
 def test_type_textfield(helloworld, javax):
-    tf1 = helloworld.locate(javax.swing.JTextField, name="tf1")
+    tf1 = helloworld.find(javax.swing.JTextField, name="tf1")
     txt = "Hello@World!$~_-()%[]{}\"'?#&*"
     assert tf1 is not None
     assert tf1.getText() == "textfield1"
     tf1.fill(txt, mode=FillMode.TYPE)
     assert tf1.getText() == txt
 
 
 def test_set_textfield(helloworld, javax):
-    tf2 = helloworld.locate(javax.swing.JTextField, text="tf2")
+    tf2 = helloworld.find(javax.swing.JTextField, text="tf2")
     tf2.fill("_Hello@World!$~", mode=FillMode.SET)
     assert tf2.getText() == "_Hello@World!$~"
```

