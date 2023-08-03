# Comparing `tmp/thinks_dash_components-0.4.9.tar.gz` & `tmp/thinks_dash_components-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinks_dash_components-0.4.9.tar", last modified: Wed Aug  2 09:50:06 2023, max compression
+gzip compressed data, was "thinks_dash_components-0.5.0.tar", last modified: Thu Aug  3 03:44:21 2023, max compression
```

## Comparing `thinks_dash_components-0.4.9.tar` & `thinks_dash_components-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 09:50:06.201286 thinks_dash_components-0.4.9/
--rw-rw-rw-   0        0        0        0 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.9/LICENSE
--rw-rw-rw-   0        0        0      464 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4087 2023-08-02 09:50:06.200289 thinks_dash_components-0.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     3802 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.9/README.md
--rw-rw-rw-   0        0        0     2373 2023-08-02 09:49:28.000000 thinks_dash_components-0.4.9/package.json
--rw-rw-rw-   0        0        0       42 2023-08-02 09:50:06.201286 thinks_dash_components-0.4.9/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 09:50:06.194306 thinks_dash_components-0.4.9/thinks_dash_components/
--rw-rw-rw-   0        0        0     1857 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/Alert.py
--rw-rw-rw-   0        0        0     1700 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/DesignableRadioItems.py
--rw-rw-rw-   0        0        0     2183 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/IndexedDB.py
--rw-rw-rw-   0        0        0     1088 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/InputNumber.py
--rw-rw-rw-   0        0        0     1092 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/IosScrollWrapper.py
--rw-rw-rw-   0        0        0     1913 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/LoadingWrapper.py
--rw-rw-rw-   0        0        0     1542 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/MobileDropdown.py
--rw-rw-rw-   0        0        0     2192 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/Notice.py
--rw-rw-rw-   0        0        0     1352 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/OperationObserver.py
--rw-rw-rw-   0        0        0     1388 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/Rotate.py
--rw-rw-rw-   0        0        0     1613 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/SelectableBox.py
--rw-rw-rw-   0        0        0     1343 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.9/thinks_dash_components/StorageObserver.py
--rw-rw-rw-   0        0        0     1878 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/TouchableComponent.py
--rw-rw-rw-   0        0        0      999 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/UrlObserver.py
--rw-rw-rw-   0        0        0     1598 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/_ComponentTemplate.py
--rw-rw-rw-   0        0        0     2360 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.9/thinks_dash_components/__init__.py
--rw-rw-rw-   0        0        0      899 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/_imports_.py
--rw-rw-rw-   0        0        0    44750 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/metadata.json
--rw-rw-rw-   0        0        0     2373 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/package-info.json
--rw-rw-rw-   0        0        0   123815 2023-08-02 09:49:37.000000 thinks_dash_components-0.4.9/thinks_dash_components/thinks_dash_components.min.js
--rw-rw-rw-   0        0        0      106 2023-08-02 09:49:37.000000 thinks_dash_components-0.4.9/thinks_dash_components/thinks_dash_components.min.js.map
-drwxrwxrwx   0        0        0        0 2023-08-02 09:50:06.199292 thinks_dash_components-0.4.9/thinks_dash_components.egg-info/
--rw-rw-rw-   0        0        0     4087 2023-08-02 09:50:06.000000 thinks_dash_components-0.4.9/thinks_dash_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-08-02 09:50:06.000000 thinks_dash_components-0.4.9/thinks_dash_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 09:50:06.000000 thinks_dash_components-0.4.9/thinks_dash_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-08-02 09:50:06.000000 thinks_dash_components-0.4.9/thinks_dash_components.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 03:44:21.865530 thinks_dash_components-0.5.0/
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:35:24.000000 thinks_dash_components-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0      464 2023-05-31 06:35:24.000000 thinks_dash_components-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4087 2023-08-03 03:44:21.864533 thinks_dash_components-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3802 2023-05-31 06:35:24.000000 thinks_dash_components-0.5.0/README.md
+-rw-rw-rw-   0        0        0     2373 2023-08-03 03:43:57.000000 thinks_dash_components-0.5.0/package.json
+-rw-rw-rw-   0        0        0       42 2023-08-03 03:44:21.865530 thinks_dash_components-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-05-31 06:35:25.000000 thinks_dash_components-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:44:21.859546 thinks_dash_components-0.5.0/thinks_dash_components/
+-rw-rw-rw-   0        0        0     1857 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/Alert.py
+-rw-rw-rw-   0        0        0     1700 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/DesignableRadioItems.py
+-rw-rw-rw-   0        0        0     2183 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/IndexedDB.py
+-rw-rw-rw-   0        0        0     1088 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/InputNumber.py
+-rw-rw-rw-   0        0        0     1092 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/IosScrollWrapper.py
+-rw-rw-rw-   0        0        0     1913 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/LoadingWrapper.py
+-rw-rw-rw-   0        0        0     1542 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/MobileDropdown.py
+-rw-rw-rw-   0        0        0     2192 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/Notice.py
+-rw-rw-rw-   0        0        0     1352 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/OperationObserver.py
+-rw-rw-rw-   0        0        0     1388 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/Rotate.py
+-rw-rw-rw-   0        0        0     1613 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/SelectableBox.py
+-rw-rw-rw-   0        0        0     1343 2023-05-31 06:35:25.000000 thinks_dash_components-0.5.0/thinks_dash_components/StorageObserver.py
+-rw-rw-rw-   0        0        0     1878 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/TouchableComponent.py
+-rw-rw-rw-   0        0        0      999 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/UrlObserver.py
+-rw-rw-rw-   0        0        0     1598 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/_ComponentTemplate.py
+-rw-rw-rw-   0        0        0     2360 2023-05-31 06:35:25.000000 thinks_dash_components-0.5.0/thinks_dash_components/__init__.py
+-rw-rw-rw-   0        0        0      899 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/_imports_.py
+-rw-rw-rw-   0        0        0    44750 2023-08-03 03:44:12.000000 thinks_dash_components-0.5.0/thinks_dash_components/metadata.json
+-rw-rw-rw-   0        0        0     2373 2023-08-03 03:44:11.000000 thinks_dash_components-0.5.0/thinks_dash_components/package-info.json
+-rw-rw-rw-   0        0        0   123788 2023-08-03 03:44:10.000000 thinks_dash_components-0.5.0/thinks_dash_components/thinks_dash_components.min.js
+-rw-rw-rw-   0        0        0      106 2023-08-03 03:44:10.000000 thinks_dash_components-0.5.0/thinks_dash_components/thinks_dash_components.min.js.map
+drwxrwxrwx   0        0        0        0 2023-08-03 03:44:21.863536 thinks_dash_components-0.5.0/thinks_dash_components.egg-info/
+-rw-rw-rw-   0        0        0     4087 2023-08-03 03:44:21.000000 thinks_dash_components-0.5.0/thinks_dash_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-08-03 03:44:21.000000 thinks_dash_components-0.5.0/thinks_dash_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 03:44:21.000000 thinks_dash_components-0.5.0/thinks_dash_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-08-03 03:44:21.000000 thinks_dash_components-0.5.0/thinks_dash_components.egg-info/top_level.txt
```

### Comparing `thinks_dash_components-0.4.9/PKG-INFO` & `thinks_dash_components-0.5.0/thinks_dash_components.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: thinks_dash_components
-Version: 0.4.9
+Name: thinks-dash-components
+Version: 0.5.0
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.4.9/README.md` & `thinks_dash_components-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/package.json` & `thinks_dash_components-0.5.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.5.0'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.4.9"
+    "version": "0.5.0"
 }
```

### Comparing `thinks_dash_components-0.4.9/setup.py` & `thinks_dash_components-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/Alert.py` & `thinks_dash_components-0.5.0/thinks_dash_components/Alert.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/DesignableRadioItems.py` & `thinks_dash_components-0.5.0/thinks_dash_components/DesignableRadioItems.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/IndexedDB.py` & `thinks_dash_components-0.5.0/thinks_dash_components/IndexedDB.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/InputNumber.py` & `thinks_dash_components-0.5.0/thinks_dash_components/InputNumber.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/IosScrollWrapper.py` & `thinks_dash_components-0.5.0/thinks_dash_components/IosScrollWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/LoadingWrapper.py` & `thinks_dash_components-0.5.0/thinks_dash_components/LoadingWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/MobileDropdown.py` & `thinks_dash_components-0.5.0/thinks_dash_components/MobileDropdown.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/Notice.py` & `thinks_dash_components-0.5.0/thinks_dash_components/Notice.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/OperationObserver.py` & `thinks_dash_components-0.5.0/thinks_dash_components/OperationObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/Rotate.py` & `thinks_dash_components-0.5.0/thinks_dash_components/Rotate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/SelectableBox.py` & `thinks_dash_components-0.5.0/thinks_dash_components/SelectableBox.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/StorageObserver.py` & `thinks_dash_components-0.5.0/thinks_dash_components/StorageObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/TouchableComponent.py` & `thinks_dash_components-0.5.0/thinks_dash_components/TouchableComponent.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/UrlObserver.py` & `thinks_dash_components-0.5.0/thinks_dash_components/UrlObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/_ComponentTemplate.py` & `thinks_dash_components-0.5.0/thinks_dash_components/_ComponentTemplate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/__init__.py` & `thinks_dash_components-0.5.0/thinks_dash_components/__init__.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/_imports_.py` & `thinks_dash_components-0.5.0/thinks_dash_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/metadata.json` & `thinks_dash_components-0.5.0/thinks_dash_components/metadata.json`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/package-info.json` & `thinks_dash_components-0.5.0/thinks_dash_components/package-info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.5.0'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.4.9"
+    "version": "0.5.0"
 }
```

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components/thinks_dash_components.min.js` & `thinks_dash_components-0.5.0/thinks_dash_components/thinks_dash_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -64,15 +64,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(o()),
                 r = i(e);
             if (!t) return r;
             var n = r.split("/"),
                 a = n.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_4_9m1690969775"), n.splice(-1, 1, a.join(".")), n.join("/")
+            return a.splice(1, 0, "v0_5_0m1691034248"), n.splice(-1, 1, a.join(".")), n.join("/")
         }
     }
     return r(r.s = 13)
 }([function(e, t) {
     e.exports = window.PropTypes
 }, function(e, t) {
     e.exports = window.React
@@ -3747,15 +3747,15 @@
                 return function(e, t) {
                     if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                 }(this, i), (t = o.call(this, e)).state = {
                     open: !1,
                     listStyle: {
                         display: "none"
                     }
-                }, t.wrapRef = h.a.createRef(), t.listRef = h.a.createRef(), t.valueRef = h.a.createRef(), t.labelRef = h.a.createRef(), t.options = t.props.options, t.isScroll = !1, t.isTouch = !1, t.interval = 300, t.pos = 1, t.id = Math.random().toString(32).substring(2), t.closeStyle = {
+                }, t.wrapRef = h.a.createRef(), t.listRef = h.a.createRef(), t.valueRef = h.a.createRef(), t.options = t.props.options, t.isScroll = !1, t.isTouch = !1, t.interval = 300, t.pos = 1, t.id = Math.random().toString(32).substring(2), t.closeStyle = {
                     display: "none"
                 }, t.toggle = t.toggle.bind(Ye(t)), t.select = t.select.bind(Ye(t)), t.clear = t.clear.bind(Ye(t)), t.close = t.close.bind(Ye(t)), t.scroll = t.scroll.bind(Ye(t)), t.touchStart = t.touchStart.bind(Ye(t)), t.touchEnd = t.touchEnd.bind(Ye(t)), t
             }
             return t = i, (r = [{
                 key: "toggle",
                 value: function() {
                     if (!this.props.disable) {
```

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components.egg-info/PKG-INFO` & `thinks_dash_components-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: thinks-dash-components
-Version: 0.4.9
+Name: thinks_dash_components
+Version: 0.5.0
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.4.9/thinks_dash_components.egg-info/SOURCES.txt` & `thinks_dash_components-0.5.0/thinks_dash_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

