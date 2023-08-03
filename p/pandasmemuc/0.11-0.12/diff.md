# Comparing `tmp/pandasmemuc-0.11.tar.gz` & `tmp/pandasmemuc-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasmemuc-0.11.tar", last modified: Mon Jul 31 02:49:49 2023, max compression
+gzip compressed data, was "pandasmemuc-0.12.tar", last modified: Thu Aug  3 19:44:03 2023, max compression
```

## Comparing `pandasmemuc-0.11.tar` & `pandasmemuc-0.12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 02:49:49.533095 pandasmemuc-0.11/
--rw-rw-rw-   0        0        0     1148 2023-07-31 02:49:37.000000 pandasmemuc-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      104 2023-07-31 02:49:35.000000 pandasmemuc-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     2347 2023-07-31 02:49:49.534071 pandasmemuc-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 02:49:49.529191 pandasmemuc-0.11/pandasmemuc/
--rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.11/pandasmemuc/README.MD
--rw-rw-rw-   0        0        0    95548 2023-07-31 02:44:44.000000 pandasmemuc-0.11/pandasmemuc/__init__.py
--rw-rw-rw-   0        0        0      147 2023-07-31 02:49:48.000000 pandasmemuc-0.11/pandasmemuc/requirements.txt
--rw-rw-rw-   0        0        0    22457 2023-07-31 02:49:48.000000 pandasmemuc-0.11/pandasmemuc/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-31 02:49:49.533095 pandasmemuc-0.11/pandasmemuc.egg-info/
--rw-rw-rw-   0        0        0     2347 2023-07-31 02:49:49.000000 pandasmemuc-0.11/pandasmemuc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-07-31 02:49:49.000000 pandasmemuc-0.11/pandasmemuc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 02:49:49.000000 pandasmemuc-0.11/pandasmemuc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2023-07-31 02:49:49.000000 pandasmemuc-0.11/pandasmemuc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-31 02:49:49.000000 pandasmemuc-0.11/pandasmemuc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-31 02:49:49.535048 pandasmemuc-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1584 2023-07-31 02:49:48.000000 pandasmemuc-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:44:03.231665 pandasmemuc-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-08-03 19:43:45.000000 pandasmemuc-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      104 2023-08-03 19:43:43.000000 pandasmemuc-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     2347 2023-08-03 19:44:03.231665 pandasmemuc-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 19:44:03.228736 pandasmemuc-0.12/pandasmemuc/
+-rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.12/pandasmemuc/README.MD
+-rw-rw-rw-   0        0        0   101447 2023-08-03 19:32:09.000000 pandasmemuc-0.12/pandasmemuc/__init__.py
+-rw-rw-rw-   0        0        0      177 2023-08-03 19:44:02.000000 pandasmemuc-0.12/pandasmemuc/requirements.txt
+-rw-rw-rw-   0        0        0    35393 2023-08-03 19:44:02.000000 pandasmemuc-0.12/pandasmemuc/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-08-03 19:44:03.231665 pandasmemuc-0.12/pandasmemuc.egg-info/
+-rw-rw-rw-   0        0        0     2347 2023-08-03 19:44:02.000000 pandasmemuc-0.12/pandasmemuc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-08-03 19:44:03.000000 pandasmemuc-0.12/pandasmemuc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 19:44:02.000000 pandasmemuc-0.12/pandasmemuc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2023-08-03 19:44:02.000000 pandasmemuc-0.12/pandasmemuc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-03 19:44:02.000000 pandasmemuc-0.12/pandasmemuc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-08-03 19:44:03.233616 pandasmemuc-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1656 2023-08-03 19:44:02.000000 pandasmemuc-0.12/setup.py
```

### Comparing `pandasmemuc-0.11/LICENSE.rst` & `pandasmemuc-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pandasmemuc-0.11/PKG-INFO` & `pandasmemuc-0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasmemuc
-Version: 0.11
+Version: 0.12
 Summary: Automating memu emulator with pandas
 Home-page: https://github.com/hansalemaos/pandasmemuc
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: memu,memnuc,pandas
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pandasmemuc-0.11/README.md` & `pandasmemuc-0.12/README.md`

 * *Files identical despite different names*

### Comparing `pandasmemuc-0.11/pandasmemuc/README.MD` & `pandasmemuc-0.12/pandasmemuc/README.MD`

 * *Files identical despite different names*

### Comparing `pandasmemuc-0.11/pandasmemuc/__init__.py` & `pandasmemuc-0.12/pandasmemuc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import random
 import sys
-from time import sleep
 import regex
 from flexible_partial import FlexiblePartialOwnName
 from adbkit import ADBTools
 import subprocess
 import io
 
 from reggisearch import search_values
-import os
 from a_pandas_ex_apply_ignore_exceptions import pd_add_apply_ignore_exceptions
 from subprocesskiller import subprocess_timeout
 from a_pandas_ex_xml2df import pd_add_read_xml_files
 import pandas as pd
 from PrettyColorPrinter import add_printer
+import os
+import tempfile
+from time import sleep
+
+import requests
+from touchtouch import touch
+from isiter import isiter
 
 add_printer(1)
 pd_add_read_xml_files()
 pd_add_apply_ignore_exceptions()
 di = search_values(
     mainkeys=(
         g := r"HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\Microsoft\Windows\CurrentVersion\Uninstall\MEmu"
@@ -34,14 +39,89 @@
 memumanage = os.sep.join(memuc.split(os.sep)[:-2] + ["MEmuHyperv", "MEmuManage.exe"])
 adb_path = memucfolder + "adb.exe"
 phoneconfig = sys.modules[__name__]
 phoneconfig.phone_dataframe = pd.DataFrame()
 phoneconfig.mac_address_prefix = "52:54:00"
 
 
+def tempfolder_and_files(fileprefix="tmp_", numberoffiles=1, suffix=".bin", zfill=8):
+    tempfolder = tempfile.TemporaryDirectory()
+    tempfolder.cleanup()
+    allfiles = []
+
+    for fi in range(numberoffiles):
+        tempfile____txtlist = os.path.join(
+            tempfolder.name, f"{fileprefix}_{str(fi).zfill(zfill)}{suffix}"
+        )
+        allfiles.append(tempfile____txtlist)
+        touch(tempfile____txtlist)
+
+    return (
+        [(k,) for k in allfiles],
+        tempfolder.name.split(os.sep)[-1],
+        tempfolder.name,
+    )
+
+
+def get_hosts_files(
+    allhosts=(
+        "https://adaway.org/hosts.txt",
+        "https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts",
+        "https://pgl.yoyo.org/adservers/serverlist.php?hostformat=hosts&showintro=0&mimetype=plaintext",
+        "https://winhelp2002.mvps.org/hosts.txt",
+    )
+):
+    allurls = []
+    for url in allhosts:
+        try:
+            resp = requests.get(url)
+
+            allurls.extend(
+                [
+                    tuple(x.strip().split(maxsplit=1))
+                    for x in resp.content.decode("utf-8").splitlines()
+                    if x and x[0] != "#"
+                ]
+            )
+        except Exception as fe:
+            print(fe)
+            continue
+    df = pd.DataFrame(sorted(list(set(allurls))))
+    df = df.loc[df[0] == "0.0.0.0"]
+    df = df.drop(df.loc[(df[0] == "0.0.0.0") & (df[1] == "0.0.0.0")].index[0])
+
+    newhostheader = """
+    127.0.0.1 localhost
+    127.0.0.1 localhost.localdomain
+    127.0.0.1 local
+    255.255.255.255 broadcasthost
+    ::1 localhost
+    ::1 ip6-localhost
+    ::1 ip6-loopback
+    fe80::1%lo0 localhost
+    ff00::0 ip6-localnet
+    ff00::0 ip6-mcastprefix
+    ff02::1 ip6-allnodes
+    ff02::2 ip6-allrouters
+    ff02::3 ip6-allhosts
+    0.0.0.0 0.0.0.0""".strip()
+
+    newhost = "\n".join(
+        [x[0] + " " + x[1] for x in zip(df[0].to_list(), df[1].to_list())]
+    )
+    newhost = newhostheader + "\n" + newhost
+    fo = tempfolder_and_files(fileprefix="", numberoffiles=0, suffix="", zfill=0)[-1]
+    if not os.path.exists(fo):
+        os.makedirs(fo)
+    hostfile = os.path.normpath(os.path.join(fo, "hosts"))
+    with open(hostfile, "w", newline="\n", encoding="utf-8") as f:
+        f.write(newhost)
+    return hostfile
+
+
 def connect_adb_tools(x):
     if "ERROR: " in x.aa_cpucap:
         ad = ADBTools(adb_path=adb_path, deviceserial=x.bb_serial)
         return ad
     return pd.NA
 
 
@@ -79,20 +159,31 @@
         stderr=subprocess.PIPE,
     )
 
 
 def list_all_emulators():
     p = run_subprocess("listvms")
     i = io.StringIO(p.stdout.decode("utf-8").strip())
-    return pd.read_csv(
+    dfr = pd.read_csv(
         i,
         header=None,
         names=["aa_index", "aa_title", "aa_handle", "aa_status", "aa_pid"],
         sep=",",
     )
+    df2 = dfr.ds_apply_ignore(
+        pd.NA,
+        lambda x: subprocess.run(
+            [memuc, "rename", "-i", str(x.aa_index), str(x.aa_title)],
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        ),
+        axis=1,
+    )
+    #print(df2)
+    return dfr
 
 
 def get_all_config(df):
     configcmds = [
         "cpus",
         "memory",
         "cpucap",
@@ -467,17 +558,21 @@
     dfallinfos = pd.concat(dfa, ignore_index=True)
     dfallinfos.columns = [f"cc_{x}" for x in dfallinfos.columns]
     newiond = []
     for acc in range(len(dfallinfos)):
         dfxax = pd.Q_Xml2df(
             dfallinfos.cc_Config_file.iloc[acc], add_xpath_and_snippet=False
         ).reset_index()
-        nameindex = dfxax.loc[dfxax.aa_value.str.contains("name_tag", na=False)].index[
-            0
-        ]
+        try:
+            nameindex = dfxax.loc[
+                dfxax.aa_value.str.contains("name_tag", na=False)
+            ].index[0]
+        except Exception as fe:
+            print(fe)
+            continue
         nameacc = ""
         for key, item in dfxax[nameindex:].iterrows():
             if "value" in item["aa_all_keys"]:
                 nameacc = item["aa_value"]
                 newiond.append(str(nameacc))
                 break
 
@@ -2978,14 +3073,86 @@
             [memuc, "rename", "-i", str(self.df.aa_index.iloc[-1]), name],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         self.change_config(0)
         return self
 
+    def patch_hosts(
+        self,
+        vms_aa_index,
+        hostfiles=(
+            "https://adaway.org/hosts.txt",
+            "https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts",
+            "https://pgl.yoyo.org/adservers/serverlist.php?hostformat=hosts&showintro=0&mimetype=plaintext",
+            "https://winhelp2002.mvps.org/hosts.txt",
+        ),
+    ):
+        hostfile = get_hosts_files(allhosts=hostfiles)
+
+        if not isiter(vms_aa_index):
+            vms_aa_index = [vms_aa_index]
+        df2 = self.df.loc[self.df.aa_index.isin(vms_aa_index)]
+        suenabled = df2.loc[df2.aa_enable_su == "1"]
+        sudisabled = df2.loc[df2.aa_enable_su == "0"]
+        for key, item in suenabled.iterrows():
+            aa_index = item.aa_index
+            item.bb_start()
+            sleep(3)
+
+            self2 = pd.DataFrame()
+            while self2.empty:
+                self23 = self.__class__()
+                self2 = self23.loc[self23.aa_index == aa_index]
+                if pd.isna(self2.iloc[0].bb_adbtools):
+                    self2 = pd.DataFrame()
+            self2.iloc[0].bb_adbtools.aa_execute_non_shell_adb_command("remount")
+            self2.iloc[0].bb_adbtools.aa_enable_root()
+            self2.iloc[0].bb_adbtools.aa_execute_multiple_adb_shell_commands(
+                ["rm ./etc/hosts"]
+            )
+            self2.iloc[0].bb_adbtools.aa_push_file_to_path(hostfile, "./etc")
+            print(
+                f"len of host file: {len(self2.iloc[0].bb_adbtools.aa_execute_multiple_adb_shell_commands(['cat ./etc/hosts']))}"
+            )
+            item.bb_stop()
+
+        for key, item in sudisabled.iterrows():
+            aa_index = item.aa_index
+            for ita in range(2):
+                item.bb_stop()
+                item.set_enable_su(1)
+                item.bb_start()
+                sleep(3)
+                self2 = pd.DataFrame()
+                while self2.empty:
+                    self23 = self.__class__()
+                    self2 = self23.loc[self23.aa_index == aa_index]
+                    if pd.isna(self2.iloc[0].bb_adbtools):
+                        self2 = pd.DataFrame()
+                self2.iloc[0].bb_adbtools.aa_execute_non_shell_adb_command("remount")
+                self2.iloc[0].bb_adbtools.aa_enable_root()
+                self2.iloc[0].bb_adbtools.aa_execute_multiple_adb_shell_commands(
+                    ["rm ./etc/hosts"]
+                )
+                self2.iloc[0].bb_adbtools.aa_push_file_to_path(hostfile, "./etc")
+                if ita ==1:
+                    print(
+                        f"len of host file: {len(self2.iloc[0].bb_adbtools.aa_execute_multiple_adb_shell_commands(['cat ./etc/hosts']))}"
+                    )
+                    self2.iloc[0].set_enable_su(0)
+                item.bb_stop()
+
+        try:
+            os.remove(hostfile)
+
+        except Exception:
+            pass
+        self.update_status()
+        return self
     def change_config(self, i):
         self.df.iloc[i].set_enable_audio(0)
         try:
             sa = phoneconfig.phone_dataframe.sample(1)
 
             self.df.iloc[i].set_linenum(sa.phone_number.iloc[0])
             self.df.iloc[i].set_imei(sa.imei.iloc[0])
@@ -3061,15 +3228,15 @@
         tmp_folder_on_sd_card="AUTOMAT",
         bluestacks_divider=32767,
     ):
         df2 = self.df.loc[self.df.aa_index == i]
         try:
             df2.bb_adbtools.iloc[0].aa_update_screenshot()
         except Exception:
-            print('Could not get screenshot')
+            print("Could not get screenshot")
             save_screenshot = False
             screenshotfolder = None
         df3 = df2.bb_adbtools.iloc[0].aa_get_all_displayed_items_from_uiautomator(
             screenshotfolder=screenshotfolder,
             max_variation_percent_x=max_variation_percent_x,
             max_variation_percent_y=max_variation_percent_y,
             loung_touch_delay=loung_touch_delay,
```

### Comparing `pandasmemuc-0.11/pandasmemuc/thirdparty.json` & `pandasmemuc-0.12/pandasmemuc/thirdparty.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7395833333333334%*

 * *Differences: {'3': "{'Version': '0.24'}",*

 * * 'insert': "[(5, OrderedDict([('License', 'MIT'), ('LicenseText', '\\n\\n The MIT License "*

 * *           '(MIT)\\n\\n Copyright (c) 2022 Johannes Fischer\\n\\n \\n\\n Permission is hereby '*

 * *           'granted, free of charge, to any person obtaining a copy\\n\\n of this software and '*

 * *           'associated documentation files (the "Software"), to deal\\n\\n in the Software without '*

 * *           'restriction, including without limitation the rights\\n\\n to use, copy, modify, '*

 * *   […]*

```diff
@@ -17,23 +17,29 @@
         "Name": "a-pandas-ex-xml2df",
         "Version": "0.13"
     },
     {
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "adbkit",
-        "Version": "0.19"
+        "Version": "0.24"
     },
     {
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2022 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "flexible-partial",
         "Version": "0.12"
     },
     {
+        "License": "MIT",
+        "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2022 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
+        "Name": "isiter",
+        "Version": "0.10"
+    },
+    {
         "License": "BSD License",
         "LicenseText": "BSD 3-Clause License\n\nCopyright (c) 2008-2011, AQR Capital Management, LLC, Lambda Foundry, Inc. and PyData Development Team\nAll rights reserved.\n\nCopyright (c) 2011-2023, Open source contributors.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n* Redistributions of source code must retain the above copyright notice, this\n  list of conditions and the following disclaimer.\n\n* Redistributions in binary form must reproduce the above copyright notice,\n  this list of conditions and the following disclaimer in the documentation\n  and/or other materials provided with the distribution.\n\n* Neither the name of the copyright holder nor the names of its\n  contributors may be used to endorse or promote products derived from\n  this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
         "Name": "pandas",
         "Version": "2.0.1"
     },
     {
         "License": "Apache Software License",
@@ -44,13 +50,25 @@
     {
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "reggisearch",
         "Version": "0.10"
     },
     {
+        "License": "Apache Software License",
+        "LicenseText": "\n                                 Apache License\n                           Version 2.0, January 2004\n                        http://www.apache.org/licenses/\n\n   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION\n\n   1. Definitions.\n\n      \"License\" shall mean the terms and conditions for use, reproduction,\n      and distribution as defined by Sections 1 through 9 of this document.\n\n      \"Licensor\" shall mean the copyright owner or entity authorized by\n      the copyright owner that is granting the License.\n\n      \"Legal Entity\" shall mean the union of the acting entity and all\n      other entities that control, are controlled by, or are under common\n      control with that entity. For the purposes of this definition,\n      \"control\" means (i) the power, direct or indirect, to cause the\n      direction or management of such entity, whether by contract or\n      otherwise, or (ii) ownership of fifty percent (50%) or more of the\n      outstanding shares, or (iii) beneficial ownership of such entity.\n\n      \"You\" (or \"Your\") shall mean an individual or Legal Entity\n      exercising permissions granted by this License.\n\n      \"Source\" form shall mean the preferred form for making modifications,\n      including but not limited to software source code, documentation\n      source, and configuration files.\n\n      \"Object\" form shall mean any form resulting from mechanical\n      transformation or translation of a Source form, including but\n      not limited to compiled object code, generated documentation,\n      and conversions to other media types.\n\n      \"Work\" shall mean the work of authorship, whether in Source or\n      Object form, made available under the License, as indicated by a\n      copyright notice that is included in or attached to the work\n      (an example is provided in the Appendix below).\n\n      \"Derivative Works\" shall mean any work, whether in Source or Object\n      form, that is based on (or derived from) the Work and for which the\n      editorial revisions, annotations, elaborations, or other modifications\n      represent, as a whole, an original work of authorship. For the purposes\n      of this License, Derivative Works shall not include works that remain\n      separable from, or merely link (or bind by name) to the interfaces of,\n      the Work and Derivative Works thereof.\n\n      \"Contribution\" shall mean any work of authorship, including\n      the original version of the Work and any modifications or additions\n      to that Work or Derivative Works thereof, that is intentionally\n      submitted to Licensor for inclusion in the Work by the copyright owner\n      or by an individual or Legal Entity authorized to submit on behalf of\n      the copyright owner. For the purposes of this definition, \"submitted\"\n      means any form of electronic, verbal, or written communication sent\n      to the Licensor or its representatives, including but not limited to\n      communication on electronic mailing lists, source code control systems,\n      and issue tracking systems that are managed by, or on behalf of, the\n      Licensor for the purpose of discussing and improving the Work, but\n      excluding communication that is conspicuously marked or otherwise\n      designated in writing by the copyright owner as \"Not a Contribution.\"\n\n      \"Contributor\" shall mean Licensor and any individual or Legal Entity\n      on behalf of whom a Contribution has been received by Licensor and\n      subsequently incorporated within the Work.\n\n   2. Grant of Copyright License. Subject to the terms and conditions of\n      this License, each Contributor hereby grants to You a perpetual,\n      worldwide, non-exclusive, no-charge, royalty-free, irrevocable\n      copyright license to reproduce, prepare Derivative Works of,\n      publicly display, publicly perform, sublicense, and distribute the\n      Work and such Derivative Works in Source or Object form.\n\n   3. Grant of Patent License. Subject to the terms and conditions of\n      this License, each Contributor hereby grants to You a perpetual,\n      worldwide, non-exclusive, no-charge, royalty-free, irrevocable\n      (except as stated in this section) patent license to make, have made,\n      use, offer to sell, sell, import, and otherwise transfer the Work,\n      where such license applies only to those patent claims licensable\n      by such Contributor that are necessarily infringed by their\n      Contribution(s) alone or by combination of their Contribution(s)\n      with the Work to which such Contribution(s) was submitted. If You\n      institute patent litigation against any entity (including a\n      cross-claim or counterclaim in a lawsuit) alleging that the Work\n      or a Contribution incorporated within the Work constitutes direct\n      or contributory patent infringement, then any patent licenses\n      granted to You under this License for that Work shall terminate\n      as of the date such litigation is filed.\n\n   4. Redistribution. You may reproduce and distribute copies of the\n      Work or Derivative Works thereof in any medium, with or without\n      modifications, and in Source or Object form, provided that You\n      meet the following conditions:\n\n      (a) You must give any other recipients of the Work or\n          Derivative Works a copy of this License; and\n\n      (b) You must cause any modified files to carry prominent notices\n          stating that You changed the files; and\n\n      (c) You must retain, in the Source form of any Derivative Works\n          that You distribute, all copyright, patent, trademark, and\n          attribution notices from the Source form of the Work,\n          excluding those notices that do not pertain to any part of\n          the Derivative Works; and\n\n      (d) If the Work includes a \"NOTICE\" text file as part of its\n          distribution, then any Derivative Works that You distribute must\n          include a readable copy of the attribution notices contained\n          within such NOTICE file, excluding those notices that do not\n          pertain to any part of the Derivative Works, in at least one\n          of the following places: within a NOTICE text file distributed\n          as part of the Derivative Works; within the Source form or\n          documentation, if provided along with the Derivative Works; or,\n          within a display generated by the Derivative Works, if and\n          wherever such third-party notices normally appear. The contents\n          of the NOTICE file are for informational purposes only and\n          do not modify the License. You may add Your own attribution\n          notices within Derivative Works that You distribute, alongside\n          or as an addendum to the NOTICE text from the Work, provided\n          that such additional attribution notices cannot be construed\n          as modifying the License.\n\n      You may add Your own copyright statement to Your modifications and\n      may provide additional or different license terms and conditions\n      for use, reproduction, or distribution of Your modifications, or\n      for any such Derivative Works as a whole, provided Your use,\n      reproduction, and distribution of the Work otherwise complies with\n      the conditions stated in this License.\n\n   5. Submission of Contributions. Unless You explicitly state otherwise,\n      any Contribution intentionally submitted for inclusion in the Work\n      by You to the Licensor shall be under the terms and conditions of\n      this License, without any additional terms or conditions.\n      Notwithstanding the above, nothing herein shall supersede or modify\n      the terms of any separate license agreement you may have executed\n      with Licensor regarding such Contributions.\n\n   6. Trademarks. This License does not grant permission to use the trade\n      names, trademarks, service marks, or product names of the Licensor,\n      except as required for reasonable and customary use in describing the\n      origin of the Work and reproducing the content of the NOTICE file.\n\n   7. Disclaimer of Warranty. Unless required by applicable law or\n      agreed to in writing, Licensor provides the Work (and each\n      Contributor provides its Contributions) on an \"AS IS\" BASIS,\n      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or\n      implied, including, without limitation, any warranties or conditions\n      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A\n      PARTICULAR PURPOSE. You are solely responsible for determining the\n      appropriateness of using or redistributing the Work and assume any\n      risks associated with Your exercise of permissions under this License.\n\n   8. Limitation of Liability. In no event and under no legal theory,\n      whether in tort (including negligence), contract, or otherwise,\n      unless required by applicable law (such as deliberate and grossly\n      negligent acts) or agreed to in writing, shall any Contributor be\n      liable to You for damages, including any direct, indirect, special,\n      incidental, or consequential damages of any character arising as a\n      result of this License or out of the use or inability to use the\n      Work (including but not limited to damages for loss of goodwill,\n      work stoppage, computer failure or malfunction, or any and all\n      other commercial damages or losses), even if such Contributor\n      has been advised of the possibility of such damages.\n\n   9. Accepting Warranty or Additional Liability. While redistributing\n      the Work or Derivative Works thereof, You may choose to offer,\n      and charge a fee for, acceptance of support, warranty, indemnity,\n      or other liability obligations and/or rights consistent with this\n      License. However, in accepting such obligations, You may act only\n      on Your own behalf and on Your sole responsibility, not on behalf\n      of any other Contributor, and only if You agree to indemnify,\n      defend, and hold each Contributor harmless for any liability\n      incurred by, or claims asserted against, such Contributor by reason\n      of your accepting any such warranty or additional liability.\n",
+        "Name": "requests",
+        "Version": "2.30.0"
+    },
+    {
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "subprocesskiller",
         "Version": "0.11"
+    },
+    {
+        "License": "MIT",
+        "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2022 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
+        "Name": "touchtouch",
+        "Version": "0.11"
     }
 ]
```

### Comparing `pandasmemuc-0.11/pandasmemuc.egg-info/PKG-INFO` & `pandasmemuc-0.12/pandasmemuc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasmemuc
-Version: 0.11
+Version: 0.12
 Summary: Automating memu emulator with pandas
 Home-page: https://github.com/hansalemaos/pandasmemuc
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: memu,memnuc,pandas
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pandasmemuc-0.11/setup.py` & `pandasmemuc-0.12/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.11'''
+VERSION = '''0.12'''
 DESCRIPTION = '''Automating memu emulator with pandas'''
 
 # Setting up
 setup(
     name="pandasmemuc",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/pandasmemuc',
     author="Johannes Fischer",
     author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
 long_description = long_description,
 long_description_content_type="text/markdown",
-    #packages=['PrettyColorPrinter', 'a_pandas_ex_apply_ignore_exceptions', 'a_pandas_ex_xml2df', 'adbkit', 'flexible_partial', 'pandas', 'regex', 'reggisearch', 'subprocesskiller'],
+    #packages=['PrettyColorPrinter', 'a_pandas_ex_apply_ignore_exceptions', 'a_pandas_ex_xml2df', 'adbkit', 'flexible_partial', 'isiter', 'pandas', 'regex', 'reggisearch', 'requests', 'subprocesskiller', 'touchtouch'],
     keywords=['memu', 'memnuc', 'pandas'],
     classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
-    install_requires=['PrettyColorPrinter', 'a_pandas_ex_apply_ignore_exceptions', 'a_pandas_ex_xml2df', 'adbkit', 'flexible_partial', 'pandas', 'regex', 'reggisearch', 'subprocesskiller'],
+    install_requires=['PrettyColorPrinter', 'a_pandas_ex_apply_ignore_exceptions', 'a_pandas_ex_xml2df', 'adbkit', 'flexible_partial', 'isiter', 'pandas', 'regex', 'reggisearch', 'requests', 'subprocesskiller', 'touchtouch'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

