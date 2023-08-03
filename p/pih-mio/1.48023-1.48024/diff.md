# Comparing `tmp/pih-mio-1.48023.tar.gz` & `tmp/pih-mio-1.48024.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48023.tar", last modified: Thu Aug  3 07:26:27 2023, max compression
+gzip compressed data, was "pih-mio-1.48024.tar", last modified: Thu Aug  3 07:33:18 2023, max compression
```

## Comparing `pih-mio-1.48023.tar` & `pih-mio-1.48024.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 07:26:25.652731 pih-mio-1.48023/
-drwxrwxrwx   0        0        0        0 2023-08-03 07:26:26.387111 pih-mio-1.48023/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48023/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48023/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165345 2023-08-03 07:25:43.000000 pih-mio-1.48023/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48023/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9434 2023-08-01 00:38:40.000000 pih-mio-1.48023/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48023/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-08-03 07:26:27.921293 pih-mio-1.48023/PKG-INFO
--rw-rw-rw-   0        0        0     1651 2023-08-03 07:25:38.000000 pih-mio-1.48023/pih-mio_setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:26:27.530673 pih-mio-1.48023/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      279 2023-08-03 07:26:23.000000 pih-mio-1.48023/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-08-03 07:26:25.000000 pih-mio-1.48023/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 07:26:23.000000 pih-mio-1.48023/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-03 07:26:24.000000 pih-mio-1.48023/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-08-03 07:26:24.000000 pih-mio-1.48023/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-03 07:26:24.000000 pih-mio-1.48023/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 07:26:27.968204 pih-mio-1.48023/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 07:33:15.604016 pih-mio-1.48024/
+drwxrwxrwx   0        0        0        0 2023-08-03 07:33:17.560090 pih-mio-1.48024/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48024/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48024/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165341 2023-08-03 07:32:13.000000 pih-mio-1.48024/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48024/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9434 2023-08-01 00:38:40.000000 pih-mio-1.48024/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48024/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-08-03 07:33:18.131667 pih-mio-1.48024/PKG-INFO
+-rw-rw-rw-   0        0        0     1651 2023-08-03 07:25:38.000000 pih-mio-1.48024/pih-mio_setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:33:18.084794 pih-mio-1.48024/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-08-03 07:33:11.000000 pih-mio-1.48024/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-08-03 07:33:15.000000 pih-mio-1.48024/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 07:33:12.000000 pih-mio-1.48024/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-03 07:33:13.000000 pih-mio-1.48024/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-08-03 07:33:14.000000 pih-mio-1.48024/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-03 07:33:14.000000 pih-mio-1.48024/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 07:33:18.147295 pih-mio-1.48024/setup.cfg
```

### Comparing `pih-mio-1.48023/MobileHelperCore/api.py` & `pih-mio-1.48024/MobileHelperCore/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from MobileHelperContent.content import MEDIA_CONTENT
 import requests
 from io import BytesIO
 
 class MIO:
 
     NAME: str = "mio"       
-    VERSION: str = "1.48023"  
+    VERSION: str = "1.48024"  
 
 class InternalInterrupt(Exception):
 
     @property
     def type(self) -> int:
         return self.args[0]
 
@@ -1039,15 +1039,15 @@
         #######################
         self.address_as_link_node: CommandNode = self.create_command_link(
             f"link|{LINK_SYMBOL}", LINK_SYMBOL, i("Адресовать ссылку на команду"), MobileHelper.ADM, True)
         self.address_as_link_node.order_value = 3
         additional_nodes.append(self.address_as_link_node)
         #######################
         about_pih_node: CommandNode = CommandNode(
-            "about|o", i("О PIH"), description="\n...", text=f"Я бот-помощник для решения Ваших задач. Моё имя составлено из первых букв нашей организации: {b('P')} acific {b('I')} nternational {b('H')} ospital или {b('П')} асифик {b('И')} нтернейшнл {b('Х')} оспитал.\n\n{i('Автор')}: {i(b('Караченцев Никита Александрович'))} \n{i('Версия')}: {b(A.V.MIO.local())}", show_in_root_menu=True, wait_for_input=False, show_always=True)
+            "about|o", i("О PIH"), description="\n...", text=f"Я бот-помощник для решения Ваших задач. Моё имя составлено из первых букв нашей организации: {b('P')} acific {b('I')} nternational {b('H')} ospital или {b('П')} асифик {b('И')} нтернейшнл {b('Х')} оспитал.\n\n{i('Автор')}: {i(b('Караченцев Никита Александрович'))} \n{i('Версия')}: {b(MIO.VERSION)}", show_in_root_menu=True, wait_for_input=False, show_always=True)
         about_pih_node.order_value = 4
         additional_nodes.append(about_pih_node)
         #######################
         self.exit_node: CommandNode = CommandNode(
             "exit", i("Выход"), self.session.exit, show_in_root_menu=True, wait_for_input=False, show_always=True, as_link=True)
         self.exit_node.order_value = 0
         additional_nodes.append(self.exit_node)
```

### Comparing `pih-mio-1.48023/MobileHelperCore/service.py` & `pih-mio-1.48024/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48023/MobileHelperCore/service_api.py` & `pih-mio-1.48024/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48023/MobileHelperCore/tools.py` & `pih-mio-1.48024/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48023/pih-mio_setup.py` & `pih-mio-1.48024/pih-mio_setup.py`

 * *Files identical despite different names*

