# Comparing `tmp/plutoplots-0.2.0.tar.gz` & `tmp/plutoplots-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutoplots-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "plutoplots-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `plutoplots-0.2.0.tar` & `plutoplots-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       51 2023-08-03 01:19:01.770626 plutoplots-0.2.0/.gitignore
--rw-r--r--   0        0        0     1083 2023-08-02 23:26:02.452269 plutoplots-0.2.0/LICENSE
--rw-r--r--   0        0        0      575 2023-08-02 17:41:45.099199 plutoplots-0.2.0/README.md
--rw-r--r--   0        0        0       43 2023-08-03 06:27:53.299490 plutoplots-0.2.0/plutoplots/__init__.py
--rw-r--r--   0        0        0     2790 2023-08-03 06:24:37.276379 plutoplots-0.2.0/plutoplots/plot.py
--rw-r--r--   0        0        0      404 2023-08-03 01:27:22.456392 plutoplots-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 plutoplots-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-08-03 01:19:01.770626 plutoplots-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1083 2023-08-02 23:26:02.452269 plutoplots-0.3.0/LICENSE
+-rw-r--r--   0        0        0      575 2023-08-02 17:41:45.099199 plutoplots-0.3.0/README.md
+-rw-r--r--   0        0        0       43 2023-08-03 06:33:04.240483 plutoplots-0.3.0/plutoplots/__init__.py
+-rw-r--r--   0        0        0     3706 2023-08-03 06:33:04.237374 plutoplots-0.3.0/plutoplots/plot.py
+-rw-r--r--   0        0        0      404 2023-08-03 01:27:22.456392 plutoplots-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 plutoplots-0.3.0/PKG-INFO
```

### Comparing `plutoplots-0.2.0/LICENSE` & `plutoplots-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plutoplots-0.2.0/README.md` & `plutoplots-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `plutoplots-0.2.0/plutoplots/plot.py` & `plutoplots-0.3.0/plutoplots/plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         plt.figure(figsize=dim)
         return self
 
     def grid(self, c="#EAEAF1"):
         # grid color
         self.axes.set_facecolor(c)
         # grid lines
-        self.axes.grid(True, linestyle='-', color='white', linewidth=0.5, alpha=0.5)
+        self.axes.grid(True, linestyle='-', color='white', linewidth=0.5, alpha=0.5, zorder=1)
         return self
 
     def label(self, xlabel, ylabel, tlabel):
         self.axes.set_ylabel(ylabel, fontsize=10)
         self.axes.set_xlabel(xlabel, fontsize=10)
         self.axes.set_title(tlabel, pad=10)
         return self
@@ -32,58 +32,89 @@
         return self
 
     def tick(self, left=False, bottom=False, labelleft=False, labelbottom=False):
         self.axes.tick_params(labelcolor='black', labelsize='small', width=0.5, labelleft=labelleft,
                               labelbottom=labelbottom, left=left, bottom=bottom)
         return self
 
+    def legend(self):
+        self.axes.legend(bbox_to_anchor=(1.05, 1), loc="upper left", prop={"family": "Arial", "size": 12})
+        return self
+
     def set_axes(self, ax):
         self.axes = ax
 
     def render(self):
         plt.show()
 
 
 class Barplot(Plot):
 
     def create(self, x, y, data, hue=None, width=0.8, c="#69b3a2", ax=None):
         self.axes = sns.barplot(x=x, y=y, hue=hue, data=data, width=width,
-                                estimator="sum", errorbar=None, color=c, ax=ax)
+                                estimator="sum", errorbar=None, color=c, ax=ax, zorder=2)
         return self
 
-    def bar_label(self, fmt='%.0f', pad=1):
-        self.axes.bar_label(self.axes.containers[0], fmt=fmt, padding=pad, color='black',
-                            fontweight=None, fontstyle='italic', family=['monospace'], fontsize=10)
+    def bar_label(self, fmt='%.0f', pad=1, fs=10):
+        for c in self.axes.containers:
+            self.axes.bar_label(c, fmt=fmt, padding=pad, color='black',
+                                fontweight=None, fontstyle='italic', family=['monospace'], fontsize=fs)
         return self
 
 
 class Lineplot(Plot):
 
     def create(self, x, y, data):
-        self.axes = sns.lineplot(data=data, x=x, y=y)
+        self.axes = sns.lineplot(data=data, x=x, y=y, marker='.', markersize=15)
         return self
 
     def limit(self, y_start, y_end):
         self.axes.set_ylim(y_start, y_end)
         return self
 
+    def fill(self, x, y):
+        self.axes.fill_between(x, y, alpha=0.7, zorder=2)
+        return self
+
 
 class Mapplot(Plot):
 
     def create(self, ct, data, x, y, c, ct_name, ax=None):
         self.axes = ax
         self.country_shape_plot(ct)
         self.data_plot(data, x, y, c)
         self.country_name_plot(ct, ct_name)
         return self
 
     def country_shape_plot(self, ct):
-        ct.plot(ax=self.axes, facecolor="white", edgecolor="k", alpha=1, linewidth=1)
+        ct.plot(ax=self.axes, facecolor="white", edgecolor="k", alpha=1, linewidth=1, zorder=2)
 
     def data_plot(self, data, x, y, c):
-        data.plot(x=x, y=y, kind="scatter", c=c, colormap="Set2", ax=self.axes)
+        data.plot(x=x, y=y, kind="scatter", c=c, colormap="Set2", ax=self.axes, zorder=2)
 
     def country_name_plot(self, ct, ct_name):
         for a, b, label in zip(
                 ct.geometry.centroid.x, ct.geometry.centroid.y, ct[ct_name]
         ):
             plt.text(a, b, label, fontsize=8, ha="center")
+
+
+class Kdeplot(Plot):
+
+    def create(self, data, x, hue, ax=None):
+        self.axes = sns.kdeplot(data=data, x=x, hue=hue, multiple="stack", ax=ax, zorder=2)
+        return self
+
+
+class Histplot(Plot):
+
+    def create(self, data, x, hue, ax=None):
+        self.axes = sns.histplot(data=data, x=x, hue=hue,
+                                 binwidth=3, stat="count", palette="Set2", ax=ax, zorder=2)
+        return self
+
+
+class Boxplot(Plot):
+
+    def create(self, data, x, y):
+        self.axes = sns.boxplot(x=x, y=y, data=data, zorder=2)
+        return self
```

### Comparing `plutoplots-0.2.0/PKG-INFO` & `plutoplots-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutoplots
-Version: 0.2.0
+Version: 0.3.0
 Summary: visualization 
 Author-email: Oluwole Ilesanmi <oluwoleilesanmi@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/oluwoleilesanmi/pluto
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plutoplots Version: 0.2.0 Summary: visualization
+Metadata-Version: 2.1 Name: plutoplots Version: 0.3.0 Summary: visualization
 Author-email: Oluwole Ilesanmi
 gmail.com> Description-Content-Type: text/markdown Classifier: License :: OSI
 Approved :: MIT License Project-URL: Home, https://github.com/oluwoleilesanmi/
 pluto
                               ****** Pluto ******
         Visualization library built on top of Seaborn and Matplotlib.
                                Easier plotting
```

