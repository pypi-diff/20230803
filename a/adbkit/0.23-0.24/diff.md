# Comparing `tmp/adbkit-0.23.tar.gz` & `tmp/adbkit-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbkit-0.23.tar", last modified: Mon May 29 05:41:36 2023, max compression
+gzip compressed data, was "adbkit-0.24.tar", last modified: Thu Aug  3 05:02:46 2023, max compression
```

## Comparing `adbkit-0.23.tar` & `adbkit-0.24.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 05:41:36.696308 adbkit-0.23/
--rw-rw-rw-   0        0        0     1148 2023-05-29 05:41:00.000000 adbkit-0.23/LICENSE.rst
--rw-rw-rw-   0        0        0       89 2023-05-29 05:40:58.000000 adbkit-0.23/MANIFEST.in
--rw-rw-rw-   0        0        0   162598 2023-05-29 05:41:36.697306 adbkit-0.23/PKG-INFO
--rw-rw-rw-   0        0        0   160932 2023-05-29 05:40:11.000000 adbkit-0.23/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 05:41:36.693316 adbkit-0.23/adbkit/
--rw-rw-rw-   0        0        0   160932 2023-05-29 05:40:11.000000 adbkit-0.23/adbkit/README.MD
--rw-rw-rw-   0        0        0   130248 2023-05-29 00:06:17.000000 adbkit-0.23/adbkit/__init__.py
--rw-rw-rw-   0        0        0      696 2023-05-29 05:41:35.000000 adbkit-0.23/adbkit/requirements.txt
--rw-rw-rw-   0        0        0   284867 2023-05-29 05:41:35.000000 adbkit-0.23/adbkit/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-29 05:41:36.696308 adbkit-0.23/adbkit.egg-info/
--rw-rw-rw-   0        0        0   162598 2023-05-29 05:41:36.000000 adbkit-0.23/adbkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-05-29 05:41:36.000000 adbkit-0.23/adbkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 05:41:36.000000 adbkit-0.23/adbkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      660 2023-05-29 05:41:36.000000 adbkit-0.23/adbkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-29 05:41:36.000000 adbkit-0.23/adbkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-29 05:41:36.698303 adbkit-0.23/setup.cfg
--rw-rw-rw-   0        0        0     2803 2023-05-29 05:41:35.000000 adbkit-0.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 05:02:46.237656 adbkit-0.24/
+-rw-rw-rw-   0        0        0     1148 2023-08-03 05:02:03.000000 adbkit-0.24/LICENSE.rst
+-rw-rw-rw-   0        0        0       89 2023-08-03 05:01:59.000000 adbkit-0.24/MANIFEST.in
+-rw-rw-rw-   0        0        0   164625 2023-08-03 05:02:46.238631 adbkit-0.24/PKG-INFO
+-rw-rw-rw-   0        0        0   162899 2023-08-03 04:58:57.000000 adbkit-0.24/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 05:02:46.232776 adbkit-0.24/adbkit/
+-rw-rw-rw-   0        0        0   162899 2023-08-03 04:58:57.000000 adbkit-0.24/adbkit/README.MD
+-rw-rw-rw-   0        0        0   132732 2023-08-03 04:45:19.000000 adbkit-0.24/adbkit/__init__.py
+-rw-rw-rw-   0        0        0      696 2023-08-03 05:02:41.000000 adbkit-0.24/adbkit/requirements.txt
+-rw-rw-rw-   0        0        0   284867 2023-08-03 05:02:41.000000 adbkit-0.24/adbkit/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-08-03 05:02:46.236679 adbkit-0.24/adbkit.egg-info/
+-rw-rw-rw-   0        0        0   164625 2023-08-03 05:02:45.000000 adbkit-0.24/adbkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-08-03 05:02:46.000000 adbkit-0.24/adbkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 05:02:45.000000 adbkit-0.24/adbkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      660 2023-08-03 05:02:45.000000 adbkit-0.24/adbkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-03 05:02:45.000000 adbkit-0.24/adbkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-08-03 05:02:46.250851 adbkit-0.24/setup.cfg
+-rw-rw-rw-   0        0        0     2803 2023-08-03 05:02:41.000000 adbkit-0.24/setup.py
```

### Comparing `adbkit-0.23/LICENSE.rst` & `adbkit-0.24/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `adbkit-0.23/PKG-INFO` & `adbkit-0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbkit
-Version: 0.23
+Version: 0.24
 Summary: Big automation package for ADB
 Home-page: https://github.com/hansalemaos/adbkit
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb,android,automation,shell,root
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 
 # Easier ADB automation 
 
-## Tested against Windows 10, Python 3.9.13, BlueStacks 5.9.300.1014 N32
+## Tested against Windows 10, Python 3.10, BlueStacks 5.9.300.1014 N32 / Google Pixel 5
 ### Cygwin is necessary: https://www.cygwin.com/setup-x86_64.exe and needs to be added to the path variable!
 
 ### pip install adbkit
 
 #### If you are using Python 3.10 and get and Exception due to requests, execute pip install requests==2.31.0
 
 **Don't get confused about the instance "self". I did it because it is faster copying methods from the class :)** 
@@ -34,14 +34,74 @@
 
 [![YT](https://github.com/hansalemaos/adbkit/raw/main/adbv/tiktok.jpg)](https://www.youtube.com/watch?v=pWoDaTeobCw)
 [https://www.youtube.com/watch?v=pWoDaTeobCw]()
 
 [![YT](https://github.com/hansalemaos/adbkit/raw/main/adbv/youtube.jpg)](https://www.youtube.com/watch?v=sRYspWNviQI)
 [https://www.youtube.com/watch?v=sRYspWNviQI]()
 
+
+**03/08/2023: Added 2 methods to find parents/children** 
+
+```python
+
+### self.aa_get_all_displayed_items_from_uiautomator_parents_children
+
+# can be called without an existing DataFrame
+# *args, **kwargs are passed to: self.aa_get_all_displayed_items_from_uiautomator
+
+self.aa_update_screenshot()
+self.aa_get_all_displayed_items_from_uiautomator_parents_children(screenshotfolder='c:\\shotfolder')
+
+# can be called with an existing DataFrame from self.aa_get_all_displayed_items_from_uiautomator
+self.aa_get_all_displayed_items_from_uiautomator_parents_children(df,screenshotfolder='c:\\shotfolder')
+
+Adds 2 columns:
+   bb_index_parent  bb_index_child
+0               24             252
+1               38              70
+2               38             213
+3               43              38
+4               43              54
+5               43              70
+6               43              86
+7               43             102
+8               43             118
+9               43             134
+....
+
+
+### self.aa_get_all_displayed_items_from_activities_parents_children
+
+# can be called without an existing DataFrame
+# *args, **kwargs are passed to: self.aa_get_all_displayed_items_from_activities
+
+self.aa_update_screenshot()
+self.aa_get_all_displayed_items_from_activities_parents_children(screenshotfolder='c:\\shotfolder')
+
+# can be called with an existing DataFrame from self.aa_get_all_displayed_items_from_activities
+self.aa_get_all_displayed_items_from_activities_parents_children(df,screenshotfolder='c:\\shotfolder')
+
+
+Adds 2 columns:
+   aa_index_parent  aa_index_child
+0               24             252
+1               38              70
+2               38             213
+3               43              38
+4               43              54
+5               43              70
+6               43              86
+7               43             102
+8               43             118
+9               43             134
+....
+
+```
+
+
 **28/05/2023: Added fast screenshots with scrcpy - no root required and some other methods** 
 
 ```python
 from adbkit import ADBTools
 from kthread_sleep import sleep
 
 adb_path = r'C:\ProgramData\chocolatey\bin\adb.exe'
```

### Comparing `adbkit-0.23/README.md` & `adbkit-0.24/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Easier ADB automation 
 
-## Tested against Windows 10, Python 3.9.13, BlueStacks 5.9.300.1014 N32
+## Tested against Windows 10, Python 3.10, BlueStacks 5.9.300.1014 N32 / Google Pixel 5
 ### Cygwin is necessary: https://www.cygwin.com/setup-x86_64.exe and needs to be added to the path variable!
 
 ### pip install adbkit
 
 #### If you are using Python 3.10 and get and Exception due to requests, execute pip install requests==2.31.0
 
 **Don't get confused about the instance "self". I did it because it is faster copying methods from the class :)** 
@@ -16,14 +16,74 @@
 
 [![YT](https://github.com/hansalemaos/adbkit/raw/main/adbv/tiktok.jpg)](https://www.youtube.com/watch?v=pWoDaTeobCw)
 [https://www.youtube.com/watch?v=pWoDaTeobCw]()
 
 [![YT](https://github.com/hansalemaos/adbkit/raw/main/adbv/youtube.jpg)](https://www.youtube.com/watch?v=sRYspWNviQI)
 [https://www.youtube.com/watch?v=sRYspWNviQI]()
 
+
+**03/08/2023: Added 2 methods to find parents/children** 
+
+```python
+
+### self.aa_get_all_displayed_items_from_uiautomator_parents_children
+
+# can be called without an existing DataFrame
+# *args, **kwargs are passed to: self.aa_get_all_displayed_items_from_uiautomator
+
+self.aa_update_screenshot()
+self.aa_get_all_displayed_items_from_uiautomator_parents_children(screenshotfolder='c:\\shotfolder')
+
+# can be called with an existing DataFrame from self.aa_get_all_displayed_items_from_uiautomator
+self.aa_get_all_displayed_items_from_uiautomator_parents_children(df,screenshotfolder='c:\\shotfolder')
+
+Adds 2 columns:
+   bb_index_parent  bb_index_child
+0               24             252
+1               38              70
+2               38             213
+3               43              38
+4               43              54
+5               43              70
+6               43              86
+7               43             102
+8               43             118
+9               43             134
+....
+
+
+### self.aa_get_all_displayed_items_from_activities_parents_children
+
+# can be called without an existing DataFrame
+# *args, **kwargs are passed to: self.aa_get_all_displayed_items_from_activities
+
+self.aa_update_screenshot()
+self.aa_get_all_displayed_items_from_activities_parents_children(screenshotfolder='c:\\shotfolder')
+
+# can be called with an existing DataFrame from self.aa_get_all_displayed_items_from_activities
+self.aa_get_all_displayed_items_from_activities_parents_children(df,screenshotfolder='c:\\shotfolder')
+
+
+Adds 2 columns:
+   aa_index_parent  aa_index_child
+0               24             252
+1               38              70
+2               38             213
+3               43              38
+4               43              54
+5               43              70
+6               43              86
+7               43             102
+8               43             118
+9               43             134
+....
+
+```
+
+
 **28/05/2023: Added fast screenshots with scrcpy - no root required and some other methods** 
 
 ```python
 from adbkit import ADBTools
 from kthread_sleep import sleep
 
 adb_path = r'C:\ProgramData\chocolatey\bin\adb.exe'
```

### Comparing `adbkit-0.23/adbkit/README.MD` & `adbkit-0.24/adbkit/README.MD`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Easier ADB automation 
 
-## Tested against Windows 10, Python 3.9.13, BlueStacks 5.9.300.1014 N32
+## Tested against Windows 10, Python 3.10, BlueStacks 5.9.300.1014 N32 / Google Pixel 5
 ### Cygwin is necessary: https://www.cygwin.com/setup-x86_64.exe and needs to be added to the path variable!
 
 ### pip install adbkit
 
 #### If you are using Python 3.10 and get and Exception due to requests, execute pip install requests==2.31.0
 
 **Don't get confused about the instance "self". I did it because it is faster copying methods from the class :)** 
@@ -16,14 +16,74 @@
 
 [![YT](https://github.com/hansalemaos/adbkit/raw/main/adbv/tiktok.jpg)](https://www.youtube.com/watch?v=pWoDaTeobCw)
 [https://www.youtube.com/watch?v=pWoDaTeobCw]()
 
 [![YT](https://github.com/hansalemaos/adbkit/raw/main/adbv/youtube.jpg)](https://www.youtube.com/watch?v=sRYspWNviQI)
 [https://www.youtube.com/watch?v=sRYspWNviQI]()
 
+
+**03/08/2023: Added 2 methods to find parents/children** 
+
+```python
+
+### self.aa_get_all_displayed_items_from_uiautomator_parents_children
+
+# can be called without an existing DataFrame
+# *args, **kwargs are passed to: self.aa_get_all_displayed_items_from_uiautomator
+
+self.aa_update_screenshot()
+self.aa_get_all_displayed_items_from_uiautomator_parents_children(screenshotfolder='c:\\shotfolder')
+
+# can be called with an existing DataFrame from self.aa_get_all_displayed_items_from_uiautomator
+self.aa_get_all_displayed_items_from_uiautomator_parents_children(df,screenshotfolder='c:\\shotfolder')
+
+Adds 2 columns:
+   bb_index_parent  bb_index_child
+0               24             252
+1               38              70
+2               38             213
+3               43              38
+4               43              54
+5               43              70
+6               43              86
+7               43             102
+8               43             118
+9               43             134
+....
+
+
+### self.aa_get_all_displayed_items_from_activities_parents_children
+
+# can be called without an existing DataFrame
+# *args, **kwargs are passed to: self.aa_get_all_displayed_items_from_activities
+
+self.aa_update_screenshot()
+self.aa_get_all_displayed_items_from_activities_parents_children(screenshotfolder='c:\\shotfolder')
+
+# can be called with an existing DataFrame from self.aa_get_all_displayed_items_from_activities
+self.aa_get_all_displayed_items_from_activities_parents_children(df,screenshotfolder='c:\\shotfolder')
+
+
+Adds 2 columns:
+   aa_index_parent  aa_index_child
+0               24             252
+1               38              70
+2               38             213
+3               43              38
+4               43              54
+5               43              70
+6               43              86
+7               43             102
+8               43             118
+9               43             134
+....
+
+```
+
+
 **28/05/2023: Added fast screenshots with scrcpy - no root required and some other methods** 
 
 ```python
 from adbkit import ADBTools
 from kthread_sleep import sleep
 
 adb_path = r'C:\ProgramData\chocolatey\bin\adb.exe'
```

### Comparing `adbkit-0.23/adbkit/__init__.py` & `adbkit-0.24/adbkit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2815,14 +2815,27 @@
             bluestacks_divider=bluestacks_divider,
         )
         andf.screenshot = self.screenshot
         andf.get_df_from_view(with_screenshot=with_screenshot)
         _, df_uiautomator, _ = andf.get_all_results()
         return df_uiautomator
 
+    def aa_get_all_displayed_items_from_uiautomator_parents_children(
+        self, df=None, *args, **kwargs
+    ):
+        try:
+            fetchdf = df.empty
+        except Exception:
+            fetchdf = True
+
+        if fetchdf:
+            df = self.aa_get_all_displayed_items_from_uiautomator(*args, **kwargs)
+
+        return self._find_children_parents(df, prefix="bb")
+
     def aa_get_all_displayed_items_from_activities(
         self,
         screenshotfolder: Union[str, None] = None,
         max_variation_percent_x: int = 10,
         max_variation_percent_y: int = 10,
         loung_touch_delay: tuple[int, int] = (1000, 1500),
         swipe_variation_startx: int = 10,
@@ -2850,14 +2863,60 @@
             bluestacks_divider=bluestacks_divider,
         )
         andf.screenshot = self.screenshot
         andf.get_df_from_activity(with_screenshot=with_screenshot)
         df_activities, _, _ = andf.get_all_results()
         return df_activities
 
+    def aa_get_all_displayed_items_from_activities_parents_children(
+        self, df=None, *args, **kwargs
+    ):
+        try:
+            fetchdf = df.empty
+        except Exception:
+            fetchdf = True
+
+        if fetchdf:
+            df = self.aa_get_all_displayed_items_from_activities(*args, **kwargs)
+
+        return self._find_children_parents(df, prefix="aa")
+
+    def _find_children_parents(self, df, prefix):
+        dfnotna = df.loc[
+            (~df[f"{prefix}_shapely"].isna())
+            & (df[f"{prefix}_area"] > 0)
+            & (df[f"{prefix}_area"] < (df[f"{prefix}_area"].max()))
+        ]
+        splitdf = [dfnotna.iloc[i : i + 1].copy() for i in range(len(dfnotna))]
+        df3 = dfnotna.ds_apply_ignore(
+            pd.NA,
+            lambda x: g
+            if not (
+                g := pd.concat(
+                    [
+                        item.assign(**{f"{prefix}_index_parent": x.name})
+                        for item in splitdf
+                        if x[f"{prefix}_shapely"].contains(
+                            item[f"{prefix}_shapely"].iloc[0]
+                        )
+                        and x.name != item.index[0]
+                        and (item[f"{prefix}_area"].iloc[0] < x[f"{prefix}_area"])
+                    ]
+                )
+            ).empty
+            else pd.NA,
+            axis=1,
+        )
+        dfparentchild = (
+            pd.concat(df3.dropna().to_list())
+            .assign(**{f"{prefix}_index_child": lambda x: x.index.__array__().copy()})
+            .reset_index(drop=True)
+        )
+        return dfparentchild
+
     def aa_list_folder_content(self, folder_to_search):
         return get_folder_df(self.deviceserial, self.adb_path, folder=folder_to_search)
 
     def aa_list_all_files_on_device(self):
         return get_folder_df(self.deviceserial, self.adb_path, folder="")
 
     def aa_list_all_packages(
@@ -3887,15 +3946,28 @@
             THRESH_OTSU=THRESH_OTSU,
         )
 
     def aa_path_exists(self, path):
         return adb_path_exists(self.adb_path, self.deviceserial, path)
 
     def aa_get_screen_resolution(self):
-        return get_screen_height_width(self.adb_path, self.deviceserial)
+        try:
+            return get_screen_height_width(self.adb_path, self.deviceserial)
+        except Exception:
+            screenshot=_get_n_adb_screenshots(
+                self.adb_path,
+                self.deviceserial,
+                sleeptime=None,
+                n=1,
+                gray=False,
+                ADAPTIVE_THRESH_MEAN_C=False,
+                ADAPTIVE_THRESH_GAUSSIAN_C=False,
+                THRESH_OTSU=False,
+            )
+            return screenshot.shape[:2][::-1]
 
     def aa_connect_to_device(self):
         connect_to_adb(self.adb_path, self.deviceserial)
 
     def aa_restart_server(self, killadb=True):
         self.aa_kill_server()
         sleep(2)
```

### Comparing `adbkit-0.23/adbkit/requirements.txt` & `adbkit-0.24/adbkit/requirements.txt`

 * *Files identical despite different names*

### Comparing `adbkit-0.23/adbkit/thirdparty.json` & `adbkit-0.24/adbkit/thirdparty.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967105263157895%*

 * *Differences: {'13': "{'Version': '0.11'}"}*

```diff
@@ -77,15 +77,15 @@
         "Name": "adb-grep-search",
         "Version": "0.12"
     },
     {
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "adb-push-create",
-        "Version": "0.10"
+        "Version": "0.11"
     },
     {
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "adb-unicode-keyboard",
         "Version": "0.11"
     },
```

### Comparing `adbkit-0.23/adbkit.egg-info/PKG-INFO` & `adbkit-0.24/adbkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbkit
-Version: 0.23
+Version: 0.24
 Summary: Big automation package for ADB
 Home-page: https://github.com/hansalemaos/adbkit
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb,android,automation,shell,root
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 
 # Easier ADB automation 
 
-## Tested against Windows 10, Python 3.9.13, BlueStacks 5.9.300.1014 N32
+## Tested against Windows 10, Python 3.10, BlueStacks 5.9.300.1014 N32 / Google Pixel 5
 ### Cygwin is necessary: https://www.cygwin.com/setup-x86_64.exe and needs to be added to the path variable!
 
 ### pip install adbkit
 
 #### If you are using Python 3.10 and get and Exception due to requests, execute pip install requests==2.31.0
 
 **Don't get confused about the instance "self". I did it because it is faster copying methods from the class :)** 
@@ -34,14 +34,74 @@
 
 [![YT](https://github.com/hansalemaos/adbkit/raw/main/adbv/tiktok.jpg)](https://www.youtube.com/watch?v=pWoDaTeobCw)
 [https://www.youtube.com/watch?v=pWoDaTeobCw]()
 
 [![YT](https://github.com/hansalemaos/adbkit/raw/main/adbv/youtube.jpg)](https://www.youtube.com/watch?v=sRYspWNviQI)
 [https://www.youtube.com/watch?v=sRYspWNviQI]()
 
+
+**03/08/2023: Added 2 methods to find parents/children** 
+
+```python
+
+### self.aa_get_all_displayed_items_from_uiautomator_parents_children
+
+# can be called without an existing DataFrame
+# *args, **kwargs are passed to: self.aa_get_all_displayed_items_from_uiautomator
+
+self.aa_update_screenshot()
+self.aa_get_all_displayed_items_from_uiautomator_parents_children(screenshotfolder='c:\\shotfolder')
+
+# can be called with an existing DataFrame from self.aa_get_all_displayed_items_from_uiautomator
+self.aa_get_all_displayed_items_from_uiautomator_parents_children(df,screenshotfolder='c:\\shotfolder')
+
+Adds 2 columns:
+   bb_index_parent  bb_index_child
+0               24             252
+1               38              70
+2               38             213
+3               43              38
+4               43              54
+5               43              70
+6               43              86
+7               43             102
+8               43             118
+9               43             134
+....
+
+
+### self.aa_get_all_displayed_items_from_activities_parents_children
+
+# can be called without an existing DataFrame
+# *args, **kwargs are passed to: self.aa_get_all_displayed_items_from_activities
+
+self.aa_update_screenshot()
+self.aa_get_all_displayed_items_from_activities_parents_children(screenshotfolder='c:\\shotfolder')
+
+# can be called with an existing DataFrame from self.aa_get_all_displayed_items_from_activities
+self.aa_get_all_displayed_items_from_activities_parents_children(df,screenshotfolder='c:\\shotfolder')
+
+
+Adds 2 columns:
+   aa_index_parent  aa_index_child
+0               24             252
+1               38              70
+2               38             213
+3               43              38
+4               43              54
+5               43              70
+6               43              86
+7               43             102
+8               43             118
+9               43             134
+....
+
+```
+
+
 **28/05/2023: Added fast screenshots with scrcpy - no root required and some other methods** 
 
 ```python
 from adbkit import ADBTools
 from kthread_sleep import sleep
 
 adb_path = r'C:\ProgramData\chocolatey\bin\adb.exe'
```

### Comparing `adbkit-0.23/adbkit.egg-info/requires.txt` & `adbkit-0.24/adbkit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `adbkit-0.23/setup.py` & `adbkit-0.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.23'''
+VERSION = '''0.24'''
 DESCRIPTION = '''Big automation package for ADB'''
 
 # Setting up
 setup(
     name="adbkit",
     version=VERSION,
     license='MIT',
```

